# Comparing `tmp/shaarpec-2.3.3.tar.gz` & `tmp/shaarpec-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaarpec-2.3.3.tar", max compression
+gzip compressed data, was "shaarpec-2.4.0.tar", max compression
```

## Comparing `shaarpec-2.3.3.tar` & `shaarpec-2.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2022-07-19 21:50:58.228912 shaarpec-2.3.3/LICENSE
--rw-r--r--   0        0        0    11309 2023-05-08 11:50:47.491411 shaarpec-2.3.3/README.md
--rw-r--r--   0        0        0     1287 2023-05-08 11:53:21.313596 shaarpec-2.3.3/pyproject.toml
--rw-r--r--   0        0        0       77 2022-07-08 12:22:12.414817 shaarpec-2.3.3/shaarpec/__init__.py
--rw-r--r--   0        0        0    16262 2023-03-27 11:44:05.074127 shaarpec-2.3.3/shaarpec/client.py
--rw-r--r--   0        0        0     1681 2023-05-02 08:39:32.060980 shaarpec-2.3.3/shaarpec/tasks.py
--rw-r--r--   0        0        0      178 2023-01-12 08:38:33.681606 shaarpec-2.3.3/shaarpec/utils.py
--rw-r--r--   0        0        0    12919 1970-01-01 00:00:00.000000 shaarpec-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-07-19 21:50:58.228912 shaarpec-2.4.0/LICENSE
+-rw-r--r--   0        0        0    11309 2023-06-19 15:02:25.598036 shaarpec-2.4.0/README.md
+-rw-r--r--   0        0        0     1280 2023-07-06 15:03:41.458631 shaarpec-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-07-06 12:15:57.120107 shaarpec-2.4.0/shaarpec/__init__.py
+-rw-r--r--   0        0        0    16415 2023-07-06 14:48:31.441423 shaarpec-2.4.0/shaarpec/client.py
+-rw-r--r--   0        0        0     1717 2023-07-06 14:47:44.308676 shaarpec-2.4.0/shaarpec/tasks.py
+-rw-r--r--   0        0        0      185 2023-07-06 12:00:48.139652 shaarpec-2.4.0/shaarpec/utils.py
+-rw-r--r--   0        0        0    12919 1970-01-01 00:00:00.000000 shaarpec-2.4.0/PKG-INFO
```

### Comparing `shaarpec-2.3.3/LICENSE` & `shaarpec-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shaarpec-2.3.3/README.md` & `shaarpec-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `shaarpec-2.3.3/shaarpec/client.py` & `shaarpec-2.4.0/shaarpec/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 from shaarpec.tasks import Task
 
 
 class Client:
     """Client for SHAARPEC Analytics API.
 
-    The input is the base URL to the Analytics API and authentication credentials via device or
-    code flow. The `.with_device(...)` and `.with_code(...)` class methods are provided and can
-    be used to construct a client. See examples of usage.
+    The input is the base URL to the Analytics API and authentication credentials via
+    device or code flow. The `.with_device(...)` and `.with_code(...)` class methods
+    are provided and can be used to construct a client. See examples of usage.
 
     API data is returned as `httpx.Response` objects.
     \f
     Examples
     --------
     >>> from shaarpec import Client
     >>> client = Client.with_device(
@@ -62,15 +62,18 @@
         'is_alive': True,
         'gender': 'F',
         'deceased_year': 0},
     ...
     """
 
     def __init__(
-        self, host: str, auth: Optional[Union[CodeFlow, DeviceFlow]], **kwargs
+        self,
+        host: str,
+        auth: Optional[Union[CodeFlow, DeviceFlow, CredentialsFlow]],
+        **kwargs,
     ) -> None:
         timeout = kwargs.pop("timeout", 60)
         self._auth = auth
         self._client = httpx.Client(
             base_url=host,
             timeout=timeout,
             headers={"accept": "application/json"},
@@ -214,18 +217,18 @@
 
     @classmethod
     def with_credentials(
         cls, host: str, auth: Union[dict[str, Any], str, None], **kwargs
     ) -> Client:
         """Authenticate with IDP host using client credentials flow.
 
-        The IDP host must support client credentials flow. Authentication can be provided to
-        `auth` as a dict, as environment variables, or as the path to an env file. The
-        environment variables are always prefixed with OIDCISH, so OIDCISH_CLIENT_ID
-        etc.
+        The IDP host must support client credentials flow. Authentication can be
+        provided to`auth` as a dict, as environment variables, or as the path to an
+        env file. The environment variables are always prefixed with OIDCISH, so
+        OIDCISH_CLIENT_ID etc.
         \f
         Parameters
         ----------
           host : str
             The Analytics API base URL.
           auth : dict or string
             Authentication details and other arguments.
@@ -262,15 +265,17 @@
         match auth:
             case None:
                 return cls(host=host, auth=None, **kwargs)
             case str():
                 return cls(host=host, auth=CredentialsFlow(_env_file=auth), **kwargs)
             case dict():
                 auth_host = auth.pop("host")
-                return cls(host=host, auth=CredentialsFlow(host=auth_host, **auth), **kwargs)
+                return cls(
+                    host=host, auth=CredentialsFlow(host=auth_host, **auth), **kwargs
+                )
             case _:
                 raise TypeError(
                     f"Object {auth} is not of recognized type ({type(auth)})."
                 )
 
     @classmethod
     def without_auth(cls, host: str, **kwargs) -> Client:
@@ -288,15 +293,15 @@
         >>> client = Client.without_auth("https://api.shaarpec.com")
         >>> client.get("terminology/allergy_type").json()
         ...
         """
         return cls(host=host, auth=None, **kwargs)
 
     @property
-    def auth(self) -> Optional[Union[CodeFlow, DeviceFlow]]:
+    def auth(self) -> Optional[Union[CodeFlow, DeviceFlow, CredentialsFlow]]:
         """Return the authentication credentials."""
         return self._auth
 
     def get(self, uri: str, **kwargs) -> httpx.Response:
         """Get the resource at `uri`.
 
         Keyword arguments are passed as query parameters.
@@ -394,15 +399,15 @@
             task_id=task_id,
             submitted_at=submitted_at,
             status="submitted",
             success=None,
             progress=None,
             result=None,
             error=None,
-            debugger=None,
+            _debugger=None,
         )
 
         if progress_bar:
             task.print()
 
         self._wait_for_task(task, poll_interval=poll_interval)
 
@@ -412,22 +417,24 @@
     def _wait_for_task(self, task: Task, poll_interval: float = 0.1) -> None:
         while task.status in ("submitted", "queued", "in_progress"):
             response = self.get(f"{task.service}/tasks/{task.task_id}/status")
 
             match response.status_code:
                 case 401:
                     print(
-                        f"Not authorized to run task id {task.task_id} on service {task.service}."
+                        f"Not authorized to run task id {task.task_id} "
+                        f"on service {task.service}."
                     )
                     task.success = False
                     task.status = "unauthorized"
 
                 case 404:
                     print(
-                        f"Task with id {task.task_id} could not be found on service {task.service}."
+                        f"Task with id {task.task_id} could not be found "
+                        f"on service {task.service}."
                     )
                     task.success = False
                     task.status = "not_found"
 
                 case 200:
                     match response.json():
                         case {"status": "not_found"}:
```

### Comparing `shaarpec-2.3.3/shaarpec/tasks.py` & `shaarpec-2.4.0/shaarpec/tasks.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 class Task(BaseModel):
     """A running task."""
 
     service: str
     task_id: str
     submitted_at: str
     status: str
-    success: Optional[bool]
-    progress: Optional[float]
-    result: Optional[Any]
-    error: Optional[Any]
-    debugger: Optional[Debugger]
+    success: Optional[bool] = None
+    progress: Optional[float] = None
+    result: Optional[Any] = None
+    error: Optional[Any] = None
+    _debugger: Optional[Debugger] = None
 
     @background.task
     def print(self, update_interval: float = 0.1) -> None:
         """Print the progress of the task."""
         initial = 0 if self.progress is None else int(100 * self.progress)
 
         with tqdm(initial=initial, total=100) as pbar:
```

### Comparing `shaarpec-2.3.3/PKG-INFO` & `shaarpec-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: shaarpec
-Version: 2.3.3
+Version: 2.4.0
 Summary: Client for SHAARPEC Analytics API.
 Author: Erik G. Brandt
 Author-email: erik.brandt@shaarpec.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Babel (>=2.12.1,<3.0.0)
 Requires-Dist: anybadge (>=1.14.0,<2.0.0)
-Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: anyio (>=3.7.1,<4.0.0)
 Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0)
 Requires-Dist: argon2-cffi-bindings (>=21.2.0,<22.0.0)
 Requires-Dist: asttokens (>=2.2.1,<3.0.0)
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: backcall (>=0.2.0,<0.3.0)
 Requires-Dist: background (>=0.2.1,<0.3.0)
-Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: bleach (>=6.0.0,<7.0.0)
-Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
 Requires-Dist: cffi (>=1.15.1,<2.0.0)
 Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: debugpy (>=1.6.7,<2.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
 Requires-Dist: entrypoints (>=0.4,<0.5)
 Requires-Dist: executing (>=1.2.0,<2.0.0)
-Requires-Dist: fastjsonschema (>=2.16.3,<3.0.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
-Requires-Dist: jupyterlab-widgets (>=3.0.7,<4.0.0)
-Requires-Dist: oidcish (>=0.3.1,<0.4.0)
-Requires-Dist: pylint (>=2.17.2,<3.0.0)
+Requires-Dist: fastjsonschema (>=2.17.1,<3.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: ipywidgets (>=8.0.7,<9.0.0)
+Requires-Dist: jupyterlab-widgets (>=3.0.8,<4.0.0)
+Requires-Dist: oidcish (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <!-- PROJECT SHIELDS -->
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: shaarpec Version: 2.3.3 Summary: Client for
+Metadata-Version: 2.1 Name: shaarpec Version: 2.4.0 Summary: Client for
 SHAARPEC Analytics API. Author: Erik G. Brandt Author-email:
 erik.brandt@shaarpec.com Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Babel
 (>=2.12.1,<3.0.0) Requires-Dist: anybadge (>=1.14.0,<2.0.0) Requires-Dist:
-anyio (>=3.6.2,<4.0.0) Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) Requires-
+anyio (>=3.7.1,<4.0.0) Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) Requires-
 Dist: argon2-cffi-bindings (>=21.2.0,<22.0.0) Requires-Dist: asttokens
-(>=2.2.1,<3.0.0) Requires-Dist: attrs (>=22.2.0,<23.0.0) Requires-Dist:
+(>=2.2.1,<3.0.0) Requires-Dist: attrs (>=23.1.0,<24.0.0) Requires-Dist:
 backcall (>=0.2.0,<0.3.0) Requires-Dist: background (>=0.2.1,<0.3.0) Requires-
-Dist: beautifulsoup4 (>=4.12.1,<5.0.0) Requires-Dist: bleach (>=6.0.0,<7.0.0)
-Requires-Dist: certifi (>=2022.12.7,<2023.0.0) Requires-Dist: cffi
+Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: bleach (>=6.0.0,<7.0.0)
+Requires-Dist: certifi (>=2023.5.7,<2024.0.0) Requires-Dist: cffi
 (>=1.15.1,<2.0.0) Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0) Requires-
 Dist: click (>=8.1.3,<9.0.0) Requires-Dist: debugpy (>=1.6.7,<2.0.0) Requires-
 Dist: decorator (>=5.1.1,<6.0.0) Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0) Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
 Requires-Dist: entrypoints (>=0.4,<0.5) Requires-Dist: executing
-(>=1.2.0,<2.0.0) Requires-Dist: fastjsonschema (>=2.16.3,<3.0.0) Requires-Dist:
-httpx (>=0.23.3,<0.24.0) Requires-Dist: ipywidgets (>=8.0.6,<9.0.0) Requires-
-Dist: jupyterlab-widgets (>=3.0.7,<4.0.0) Requires-Dist: oidcish
-(>=0.3.1,<0.4.0) Requires-Dist: pylint (>=2.17.2,<3.0.0) Requires-Dist: tqdm
+(>=1.2.0,<2.0.0) Requires-Dist: fastjsonschema (>=2.17.1,<3.0.0) Requires-Dist:
+httpx (>=0.24.1,<0.25.0) Requires-Dist: ipywidgets (>=8.0.7,<9.0.0) Requires-
+Dist: jupyterlab-widgets (>=3.0.8,<4.0.0) Requires-Dist: oidcish
+(>=1.0.0,<2.0.0) Requires-Dist: pydantic (>=2.0.2,<3.0.0) Requires-Dist: tqdm
 (>=4.65.0,<5.0.0) Description-Content-Type: text/markdown   [![Contributors]
 [contributors-shield]][contributors-url] [![Forks][forks-shield]][forks-url] [!
 [Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
                                     [Logo]
                   Python client for SHAARPEC Analytics API.
                              Explore_the_docs_Â»
```

