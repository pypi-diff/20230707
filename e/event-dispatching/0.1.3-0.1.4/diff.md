# Comparing `tmp/event_dispatching-0.1.3.tar.gz` & `tmp/event_dispatching-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_dispatching-0.1.3.tar", max compression
+gzip compressed data, was "event_dispatching-0.1.4.tar", max compression
```

## Comparing `event_dispatching-0.1.3.tar` & `event_dispatching-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/LICENSE
--rw-r--r--   0        0        0     1627 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/README.md
--rw-r--r--   0        0        0      238 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/__init__.py
--rw-r--r--   0        0        0     1876 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/_dispatcher.py
--rw-r--r--   0        0        0      922 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/async_dispatcher.py
--rw-r--r--   0        0        0      786 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/sync_dispatcher.py
--rw-r--r--   0        0        0      237 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/types.py
--rw-r--r--   0        0        0     1718 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 event_dispatching-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1627 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/README.md
+-rw-r--r--   0        0        0      238 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/__init__.py
+-rw-r--r--   0        0        0     1895 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/_dispatcher.py
+-rw-r--r--   0        0        0      953 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/async_dispatcher.py
+-rw-r--r--   0        0        0      817 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/sync_dispatcher.py
+-rw-r--r--   0        0        0      237 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/types.py
+-rw-r--r--   0        0        0     1717 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 event_dispatching-0.1.4/PKG-INFO
```

### Comparing `event_dispatching-0.1.3/LICENSE` & `event_dispatching-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.3/README.md` & `event_dispatching-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.3/event_dispatcher/_dispatcher.py` & `event_dispatching-0.1.4/event_dispatcher/_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This module is meant for internal usage, not for users of the library.
 If you want implement custom event dispatcher
 use `event_dispatcher.BaseEventDispatcher`
 """
 
 import collections
 from abc import ABC, abstractmethod
-from typing import Callable, Generic, TypeVar
+from typing import Callable, Generic, List, Optional, TypeVar
 
 from event_dispatcher import types
 
 _CallbackT = TypeVar("_CallbackT", covariant=True)
 
 
 class BaseEventDispatcher(ABC, Generic[_CallbackT]):
@@ -29,15 +29,15 @@
             return callback
 
         return decorator
 
     def subscribers_count(self, event_name: str) -> int:
         return len(self._subscribers[event_name])
 
-    def subscribers(self, event_name: str) -> list[_CallbackT]:
+    def subscribers(self, event_name: str) -> List[_CallbackT]:
         return self._subscribers[event_name].copy()
 
     def unsubscribe(self, event_name, callback: _CallbackT) -> int:
         event_subscribers = self._subscribers[event_name]
         if not event_subscribers:
             return 0
 
@@ -50,10 +50,10 @@
                 total_removed += 1
 
             event_subscribers_idx -= 1
         return total_removed
 
     @abstractmethod
     def dispatch(
-        self, event_name: str, data: types.EventData | None = None
+        self, event_name: str, data: Optional[types.EventData] = None
     ) -> bool:  # pragma: no cover
         pass
```

### Comparing `event_dispatching-0.1.3/event_dispatcher/async_dispatcher.py` & `event_dispatching-0.1.4/event_dispatcher/async_dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 
   dispatcher = AsyncEventDispatcher()
   dispatcher.subscribe("event.name", async_callback)
   await dispatcher.dispatch("event.name", {"event": "data"})
 """
 
 import asyncio
+from typing import Optional
 
 from event_dispatcher import _dispatcher, types
 
 
 class AsyncEventDispatcher(_dispatcher.BaseEventDispatcher[types.AsyncCallback]):
     async def dispatch(
-        self, event_name: str, data: types.EventData | None = None
+        self, event_name: str, data: Optional[types.EventData] = None
     ) -> bool:
         subscribers = self._subscribers[event_name]
 
         if not subscribers:
             return False
 
         await asyncio.gather(*[callback(data) for callback in subscribers])
```

### Comparing `event_dispatching-0.1.3/event_dispatcher/sync_dispatcher.py` & `event_dispatching-0.1.4/event_dispatcher/sync_dispatcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 Typical usage example:
 
   dispatcher = SyncEventDispatcher()
   dispatcher.subscribe("event.name", async_callback)
   dispatcher.dispatch("event.name", {"event": "data"})
 """
+from typing import Optional
 
 from event_dispatcher import _dispatcher, types
 
 
 class SyncEventDispatcher(_dispatcher.BaseEventDispatcher[types.SyncCallback]):
-    def dispatch(self, event_name: str, data: types.EventData | None = None) -> bool:
+    def dispatch(self, event_name: str, data: Optional[types.EventData] = None) -> bool:
         subscribers = self._subscribers[event_name]
 
         if not subscribers:
             return False
 
         for subscriber in subscribers:
             subscriber(data)
```

### Comparing `event_dispatching-0.1.3/pyproject.toml` & `event_dispatching-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-dispatching"
-version = "0.1.3"
+version = "0.1.4"
 description = "Pure python implementation of event dispatcher"
 authors = ["Ruslan Saiko <ruslan.saiko.dev@gmail.com>"]
 repository = "https://github.com/trabem/event-dispatcher"
 readme = "README.md"
 packages = [{ include = "event_dispatcher" }]
 license = "MIT"
 classifiers = [
@@ -24,15 +24,15 @@
     "asynchronous",
     "event-driven",
     "event management"
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.0"
 coverage = "^7.2.7"
```

### Comparing `event_dispatching-0.1.3/PKG-INFO` & `event_dispatching-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: event-dispatching
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pure python implementation of event dispatcher
 Home-page: https://github.com/trabem/event-dispatcher
 License: MIT
 Keywords: event-dispatcher,event-dispatching,events,event handling,python,asynchronous,event-driven,event management
 Author: Ruslan Saiko
 Author-email: ruslan.saiko.dev@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/trabem/event-dispatcher
 Description-Content-Type: text/markdown
```

