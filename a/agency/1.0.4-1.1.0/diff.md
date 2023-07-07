# Comparing `tmp/agency-1.0.4.tar.gz` & `tmp/agency-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.0.4.tar", max compression
+gzip compressed data, was "agency-1.1.0.tar", max compression
```

## Comparing `agency-1.0.4.tar` & `agency-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35148 2023-06-20 04:23:57.867662 agency-1.0.4/LICENSE
--rw-r--r--   0        0        0    25161 2023-06-20 04:23:57.867662 agency-1.0.4/README.md
--rw-r--r--   0        0        0       40 2023-06-20 04:23:57.871662 agency-1.0.4/agency/__init__.py
--rw-r--r--   0        0        0    10347 2023-06-20 04:23:57.871662 agency-1.0.4/agency/agent.py
--rw-r--r--   0        0        0      801 2023-06-20 04:23:57.871662 agency-1.0.4/agency/schema.py
--rwxr-xr-x   0        0        0     3261 2023-06-20 04:23:57.871662 agency-1.0.4/agency/space.py
--rw-r--r--   0        0        0     4280 2023-06-20 04:23:57.871662 agency-1.0.4/agency/util.py
--rw-r--r--   0        0        0      517 2023-06-20 04:23:59.359765 agency-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    25841 1970-01-01 00:00:00.000000 agency-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-07 21:43:06.527332 agency-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9474 2023-07-07 21:43:06.527332 agency-1.1.0/README.md
+-rw-r--r--   0        0        0       40 2023-07-07 21:43:06.527332 agency-1.1.0/agency/__init__.py
+-rw-r--r--   0        0        0     9470 2023-07-07 21:43:06.527332 agency-1.1.0/agency/agent.py
+-rw-r--r--   0        0        0      802 2023-07-07 21:43:06.527332 agency-1.1.0/agency/schema.py
+-rwxr-xr-x   0        0        0     8762 2023-07-07 21:43:06.527332 agency-1.1.0/agency/space.py
+-rw-r--r--   0        0        0     3824 2023-07-07 21:43:06.527332 agency-1.1.0/agency/util.py
+-rw-r--r--   0        0        0      560 2023-07-07 21:43:07.647329 agency-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10191 1970-01-01 00:00:00.000000 agency-1.1.0/PKG-INFO
```

### Comparing `agency-1.0.4/LICENSE` & `agency-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.0.4/agency/agent.py` & `agency-1.1.0/agency/agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from abc import abstractmethod
+from agency import util
 from agency.schema import ActionSchema, MessageSchema
+from colorama import Fore, Style
+from typing import List
 import inspect
-import queue
 import re
-import threading
-
 
 # access keys
 ACCESS = "access"
 ACCESS_PERMITTED = "permitted"
 ACCESS_DENIED = "denied"
 ACCESS_REQUESTED = "requested"
 
@@ -16,130 +15,97 @@
 def access_policy(level):
     def decorator(func):
         func.access_policy = level
         return func
     return decorator
 
 
-ACTION_METHOD_PREFIX = "_action__"
-
-
 class Agent():
     """
-    An Actor that may represent a human, AI, or other system.
+    An Actor that may represent an AI agent, computing system, or human user
     """
 
-    def __init__(self, id: str) -> None:
-        self.__id = id
-        self.__message_queue = queue.Queue()
-        self.__cached__get_action_help = None
-        # threading related
-        self.__thread = None
-        self.running = threading.Event()
-        self.stopping = threading.Event()
-        # set by parent Space when added
-        self.space = None
-        # A basic approach to storing messages
-        self._message_log = []
-
-    def id(self, fully_qualified=True) -> str:
-        """
-        Returns the fully qualified id of this agent
-        """
-        if fully_qualified:
-            _id = self.__id
-            if self.space is not None:
-                _id = f"{self.__id}.{self.space.id()}"
-            return _id
-        else:
-            return self.__id
+    ACTION_METHOD_PREFIX = "_action__"
 
-    def run(self):
-        """Starts the agent in a thread"""
-        if not self.running.is_set():
-            self.__thread = threading.Thread(target=self.__process)
-            self.__thread.start()
-            self.running.set()
-
-    def stop(self):
-        """Stops the agents thread"""
-        self.stopping.set()
-        self.__thread.join()
-
-    def _send(self, action: ActionSchema):
-        """
-        Validates and sends (out) an action
-        """
-        # define message, validate, and route it
-        message = MessageSchema(**{
-          **action,
-          "from": self.id(),
-        }).dict(by_alias=True)
-        # Record message and route it
-        self._message_log.append(message)
-        self.space._route(message)
+    def __init__(self, id: str) -> None:
+        if len(id) < 1 or len(id) > 255:
+            raise ValueError("id must be between 1 and 255 characters")
+        if re.match(r"^amq\.", id):
+            raise ValueError("id cannot start with \"amq.\"")
+        self.__id: str = id
+        # set by Space when added
+        self._space = None
+        # a basic approach to storing messages
+        self._message_log: List[MessageSchema] = []
+        self.__cached__help = None
+
+    def id(self) -> str:
+        """
+        Returns the id of this agent. The id is a string that identifies this
+        agent within the space. ID's are not necessarily unique. If two agents
+        have the same id they will both receive messages sent to that id.
+        """
+        return self.__id
 
-    def _receive(self, message: MessageSchema):
+    def _send(self, action: dict):
         """
-        Validates and enqueues an incoming action to be processed
+        Sends (out) an action
         """
-        message = MessageSchema(**message).dict(by_alias=True)
-        # Record message and place on queue
+        action = ActionSchema(**action).dict(by_alias=True)  # validate
+        message = self._space._route(sender=self, action=action)
         self._message_log.append(message)
-        self.__message_queue.put(message)
 
-    def __process(self) -> str:
+    def _receive(self, message: dict):
         """
-        Continually processes queued messages/actions
+        Receives and processes an incoming message
         """
-        while not self.stopping.is_set():
-            try:
-                message = self.__message_queue.get(timeout=0.01)
-                try:
-                    self.__commit_action(message)
-                except Exception as e:
-                    # Here we handle exceptions that occur while committing an
-                    # action, including PermissionError's from access denial, by
-                    # reporting the error back to the sender. If an error occurs
-                    # here, indicating that basic _send() functionality is
-                    # broken, the application will exit.
-                    self._send({
-                      "to": message['from'],
-                      "thoughts": "An error occurred",
-                      "action": "error",
-                      "args": {
-                        "original_message": message,
-                        "error": f"{e}",
-                      },
-                    })
-            except queue.Empty:
-                continue
+        message = MessageSchema(**message).dict(by_alias=True)  # validate
+        try:
+            # Record message and commit action
+            self._message_log.append(message)
+            self.__commit(message)
+        except Exception as e:
+            # Here we handle exceptions that occur while committing an
+            # action, including PermissionError's from access denial, by
+            # reporting the error back to the sender.
+            self._send({
+                "to": message['from'],
+                "thoughts": "An error occurred",
+                "action": "error",
+                "args": {
+                    "original_message": message,
+                    "error": f"{e}",
+                },
+            })
 
-    def __commit_action(self, message: MessageSchema):
+    def __commit(self, message: dict):
         """
         Invokes action if permitted otherwise raises PermissionError
         """
-        # Check if the action exists
+        # Check if the action method exists
         action_method = None
         try:
             action_method = getattr(
-              self, f"{ACTION_METHOD_PREFIX}{message['action']}")
+              self, f"{self.ACTION_METHOD_PREFIX}{message['action']}")
         except AttributeError as e:
             # the action was not found
             if message['to'] == self.id():
                 # if it was point to point, raise an error
                 raise AttributeError(
                     f"\"{message['action']}\" action not found on \"{self.id()}\"")
             else:
                 # broadcasts will not raise an error
                 return
 
+        self._before_action(message)
+
         return_value = None
         error = None
         try:
+
             # Check if the action is permitted
             if self.__permitted(message):
 
                 # Invoke the action method
                 # (set _current_message so that it can be used by the action)
                 self._current_message = message
                 return_value = action_method(**message['args'])
@@ -158,55 +124,53 @@
                         "return_value": return_value,
                       },
                     })
             else:
                 raise PermissionError(
                   f"\"{self.id()}.{message['action']}\" not permitted")
         except Exception as e:
-            # If an error occurs, we reraise it to be handled by the process loop
-            error = e
+            error = e # save the error for _after_action
             raise Exception(e)
         finally:
-            # Always call _after_action
             self._after_action(message, return_value, error)
 
-    def __permitted(self, message) -> bool:
+    def __permitted(self, message: dict) -> bool:
         """
         Checks whether the action represented by the message is allowed
         """
         policy = getattr(
-          self, f"{ACTION_METHOD_PREFIX}{message['action']}").access_policy
+          self, f"{self.ACTION_METHOD_PREFIX}{message['action']}").access_policy
         if policy == ACCESS_PERMITTED:
             return True
         elif policy == ACCESS_DENIED:
             return False
         elif policy == ACCESS_REQUESTED:
             return self._request_permission(message)
         else:
             raise Exception(
               f"Invalid access policy for method: {message['action']}, got '{policy}'")
 
-    def _get_help(self, action_name: str = None) -> list:
+    def _help(self, action_name: str = None) -> list:
         """
         Returns an array of all action methods on this class that match
         'action_name'. If no action_name is passed, returns all actions.
         [
           {
-            "space.agent": "<space_name>.<agent_name>",
+            "to": "<agent_id>",
             "thoughts": "<docstring_of_action_method>",
             "action": "<action_method_name>",
             "args": {
               "arg_name": "<arg_type>",
               ...
             }
           },
           ...
         ]
         """
-        if self.__cached__get_action_help is None:
+        if self.__cached__help is None:
             def get_arguments(method):
                 sig = inspect.signature(method)
                 return {
                   k: v.annotation.__name__
                   if v.annotation != inspect.Parameter.empty else ""
                   for k, v in sig.parameters.items()
                   if v.default == inspect.Parameter.empty
@@ -214,77 +178,83 @@
 
             def get_docstring(method):
                 return re.sub(r'\s+', ' ', method.__doc__).strip() if method.__doc__ else ""
 
             methods = {
               name: getattr(self, name)
               for name in dir(self)
-              if name.startswith(ACTION_METHOD_PREFIX)
+              if name.startswith(self.ACTION_METHOD_PREFIX)
               and callable(getattr(self, name))
             }
-            self.__cached__get_action_help = [
+            self.__cached__help = [
               {
                 'to': self.id(),  # fully qualified agent id to send the action
-                'action': name.replace(ACTION_METHOD_PREFIX, ''),
+                'action': name.replace(self.ACTION_METHOD_PREFIX, ''),
                 'thoughts': get_docstring(method),
                 'args': get_arguments(method),
               }
               for name, method in methods.items()
               if method.access_policy != ACCESS_DENIED \
                 and re.search(r'^_action__(help|return|error)$', name) is None
             ]
         if action_name:
-            return self.__cached__get_action_help[action_name]
+            return self.__cached__help[action_name]
         else:
-            return self.__cached__get_action_help
-
-    def _action_exists(self, action_name: str):
-        """
-        Returns true if the action exists on this agent
-        """
-        return hasattr(self, f"{ACTION_METHOD_PREFIX}{action_name}")
+            return self.__cached__help
 
     # Override any of the following methods as needed to implement your agent
 
     @access_policy(ACCESS_PERMITTED)
     def _action__help(self, action_name: str = None) -> list:
         """
         Returns list of actions on this agent matching action_name, or all if none
         is passed.
         """
-        return self._get_help(action_name)
+        return self._help(action_name)
 
     @access_policy(ACCESS_PERMITTED)
-    def _action__return(self, original_message: MessageSchema, return_value: str):
+    def _action__return(self, original_message: dict, return_value: str):
         """
         Implement this action to handle returned data from a prior action. By
         default this action simply replaces it with an incoming "say".
         """
-        print("WARNING: Data was returned from an action. Implement _action__return to handle it.")
-        pass
+        print(f"{Fore.YELLOW}WARNING: Data was returned from an action. Implement _action__return to handle it.{Style.RESET_ALL}")
 
     @access_policy(ACCESS_PERMITTED)
-    def _action__error(self, original_message: MessageSchema, error: str):
+    def _action__error(self, original_message: dict, error: str):
         """
         Implement this action to handle errors from an action.
         """
-        print("WARNING: An error occurred in an action. Implement _action__error to handle it.")
-        pass
+        print(f"{Fore.YELLOW}WARNING: An error occurred in an action. Implement _action__error to handle it.{Style.RESET_ALL}")
+
+    def _before_action(self, message: dict):
+        """
+        Called before every action. Override and use this method for logging or
+        other situations where you may want to pass through all actions.
+        """
 
-    def _after_action(self, original_message: MessageSchema, return_value: str, error: str):
+    def _after_action(self, original_message: dict, return_value: str, error: str):
         """
         Called after every action. Override and use this method for logging or other
         situations where you may want to pass through all actions.
-
-        Note that this is only called if the action was actually attempted, meaning
-        BOTH the action exists AND is permitted.
         """
-        pass
 
-    @abstractmethod
-    def _request_permission(self, proposed_message: MessageSchema) -> bool:
+    def _request_permission(self, proposed_message: dict) -> bool:
         """
         Implement this method to receive a proposed action message and present it to
         the agent for review. Return true or false to indicate whether access
         should be permitted.
         """
-        raise NotImplementedError()
+        raise NotImplementedError(
+            "You must implement _request_permission to use ACCESS_REQUESTED")
+
+    def _after_add(self):
+        """
+        Called after the agent is added to a space. Override this method to
+        perform any additional setup.
+        """
+
+    def _before_remove(self):
+        """
+        Called before the agent is removed from a space. Override this method to
+        perform any cleanup.
+        """
```

### Comparing `agency-1.0.4/agency/schema.py` & `agency-1.1.0/agency/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Dict, Optional
 from pydantic import BaseModel, Field
+from typing import Dict, Optional
 
 
 class ActionSchema(BaseModel):
     """
-    Schema for validation when "sending" an action. This format is expected by the
-    "_send" method of the Agent class.
+    Schema for validation when "sending" an action. This format is expected by
+    the "_send" method of the Agent class.
     """
 
     # fully qualified name of the receiving agent.
     # if not specified the action is sent to all agents _but_ the sender
     to: Optional[str] = Field(None)
 
     # natural language explanation for the action
@@ -23,9 +23,10 @@
 
 
 class MessageSchema(ActionSchema):
     """
     Schema for validation of a received message. This format is expected by the
     "_receive" method of the Agent class.
     """
+
     # the sending agent
     from_field: str = Field(..., alias='from')
```

### Comparing `agency-1.0.4/agency/util.py` & `agency-1.1.0/agency/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -117,21 +117,7 @@
             debug_object_value = json.dumps(
                 object, indent=2, cls=CustomEncoder)
         except Exception as e:
             print(f"debug_text: {e}")
             pass
         debug_value = f"{debug_object_value}\n{END_STYLE}{'_'*5} {name} {'_'*5}"
     return f"\n{START_STYLE}{'>'*5} {name} {'<'*5}{Style.RESET_ALL}\n{debug_value}{Style.RESET_ALL}".replace("\\n", "\n")
-
-
-def parse_json_response(response_text, stopping_string) -> dict:
-    """
-    Parses a json command string into a valid action object
-    """
-    try:
-        message_json = json.loads(
-          # try to parse everything up to the first stopping string found
-          response_text.split(stopping_string)[0].strip()
-        )
-        return message_json
-    except Exception as e:
-        raise f"{e}: Could not parse command from: \"{response_text}\""
```

### Comparing `agency-1.0.4/pyproject.toml` & `agency-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "agency"
-version = "1.0.4"
+version = "1.1.0"
 description = "A fast and minimal actor model framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["agency/**/*"]
 exclude = ["*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncio = "^3.4"
 colorama = "^0.4"
 pydantic = "^1.8"
 eventlet = "^0.33.3"
+pika = "^1.3.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
+pytest-asyncio = "^0.21.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

