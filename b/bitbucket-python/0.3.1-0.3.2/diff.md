# Comparing `tmp/bitbucket_python-0.3.1.tar.gz` & `tmp/bitbucket_python-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbucket_python-0.3.1.tar", max compression
+gzip compressed data, was "bitbucket_python-0.3.2.tar", max compression
```

## Comparing `bitbucket_python-0.3.1.tar` & `bitbucket_python-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-03-27 21:06:04.140442 bitbucket_python-0.3.1/LICENSE
--rw-r--r--   0        0        0     2762 2023-04-11 01:04:01.443767 bitbucket_python-0.3.1/README.md
--rw-r--r--   0        0        0      117 2023-04-01 19:06:34.079408 bitbucket_python-0.3.1/bitbucket/__init__.py
--rw-r--r--   0        0        0    19438 2023-04-11 01:04:01.443970 bitbucket_python-0.3.1/bitbucket/aclient.py
--rw-r--r--   0        0        0     2265 2023-04-11 01:04:01.444132 bitbucket_python-0.3.1/bitbucket/base.py
--rw-r--r--   0        0        0    12863 2023-04-11 01:04:01.444295 bitbucket_python-0.3.1/bitbucket/client.py
--rw-r--r--   0        0        0      264 2023-03-27 21:06:04.140882 bitbucket_python-0.3.1/bitbucket/exceptions.py
--rw-r--r--   0        0        0      501 2023-04-11 01:04:01.444667 bitbucket_python-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 bitbucket_python-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-27 21:06:04.140442 bitbucket_python-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2762 2023-04-11 01:04:01.443767 bitbucket_python-0.3.2/README.md
+-rw-r--r--   0        0        0      117 2023-04-01 19:06:34.079408 bitbucket_python-0.3.2/bitbucket/__init__.py
+-rw-r--r--   0        0        0    19754 2023-07-07 13:59:22.789086 bitbucket_python-0.3.2/bitbucket/aclient.py
+-rw-r--r--   0        0        0     3119 2023-07-07 13:59:22.789275 bitbucket_python-0.3.2/bitbucket/base.py
+-rw-r--r--   0        0        0    14657 2023-07-07 13:59:22.789458 bitbucket_python-0.3.2/bitbucket/client.py
+-rw-r--r--   0        0        0      264 2023-03-27 21:06:04.140882 bitbucket_python-0.3.2/bitbucket/exceptions.py
+-rw-r--r--   0        0        0      501 2023-07-07 13:59:33.049732 bitbucket_python-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 bitbucket_python-0.3.2/PKG-INFO
```

### Comparing `bitbucket_python-0.3.1/LICENSE` & `bitbucket_python-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbucket_python-0.3.1/README.md` & `bitbucket_python-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket_python-0.3.1/bitbucket/aclient.py` & `bitbucket_python-0.3.2/bitbucket/aclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,29 @@
     async with Client('myusername', 'mypassword', 'myaccount') as client:
         response = await client.get_user()
         print(response)
     ```
     """
 
     async def __aenter__(self):
-        self._session = httpx.AsyncClient(
-            auth=(
-                self.user,
-                self.password,
+        if self.use_password:
+            self._session = httpx.AsyncClient(
+                auth=(
+                    self.user,
+                    self.password,
+                )
+            )
+        elif self.use_token:
+            headers = {
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.token}"
+            }
+            self._session = httpx.AsyncClient(
+                headers=headers
             )
-        )
 
         user_data = await self.get_user()
 
         # for shared repo, set baseURL to owner
         if self.username is None and user_data is not None:
             self.username = user_data.get("username")
```

### Comparing `bitbucket_python-0.3.1/bitbucket/base.py` & `bitbucket_python-0.3.2/bitbucket/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 import typing
+import requests
 
 from .exceptions import (
     InvalidIDError,
     NotAuthenticatedError,
     NotFoundIDError,
     PermissionError,
     UnknownError,
 )
 
 
 class BaseClient(object):
     BASE_URL = "https://api.bitbucket.org/"
+    TOKEN_URL = 'https://bitbucket.org/site/oauth2/access_token'
 
-    def __init__(self, user: str, password: str, owner: typing.Union[str, None] = None):
+    def __init__(self, user: str=None, password: str=None,token: str=None,client_id: str=None, client_secret: str=None, owner: typing.Union[str, None] = None):
         self.user = user
         self.password = password
         self.username = owner
+        self.use_password = False
+        self.use_token = False
+        if user and password:
+            self.use_password = True
+        self.token = token
+        if token:
+            self.use_token = True
+        elif client_id and client_secret:
+            token_req_payload = {'grant_type': 'client_credentials'}
+            response = requests.post(self.TOKEN_URL, data=token_req_payload, allow_redirects=False, auth=(client_id, client_secret))
+            response = self.parse(response)
+            self.token = response['access_token']
+            self.use_token = True
+
+        if not (self.use_password or self.token):
+            raise NotAuthenticatedError("Insufficient credentials")
 
     def parse(self, response) -> typing.Union[typing.Dict[str, typing.Any], None]:
         """
         Parses the response from the BitBucket API and returns the response data or raises an exception if the response
         indicates an error.
 
         Args:
```

### Comparing `bitbucket_python-0.3.1/bitbucket/client.py` & `bitbucket_python-0.3.2/bitbucket/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typing
 import requests
 
 from .base import BaseClient
-
+from .exceptions import NotAuthenticatedError
 
 class Client(BaseClient):
-    def __init__(self, user, password, owner=None):
+    def __init__(self, user=None, password=None, token=None, client_id=None, client_secret=None, owner=None):
         """Initial session with user/password, and setup repository owner
 
         Args:
             params:
 
         Returns:
 
         """
-        super().__init__(user, password, owner)
+        super().__init__(user, password,token,client_id,client_secret, owner)
 
         # for shared repo, set baseURL to owner
         if owner is None:
             user_data = self.get_user()
             owner = user_data.get("username")
         self.workspace = owner
 
@@ -420,38 +420,78 @@
         return self._delete(
             "2.0/repositories/{}/{}/hooks/{}".format(
                 self.workspace, repository_slug, webhook_uid
             ),
             params=params,
         )
 
-    def _get(self, endpoint: str, params=None):
-        response = requests.get(
-            endpoint if endpoint.startswith("http") else self.BASE_URL + endpoint,
-            params=params,
-            auth=(self.user, self.password),
-        )
+    def _get(self, endpoint, params=None):
+        if self.use_password:
+            response = requests.get(self.BASE_URL + endpoint, params=params, auth=(self.user, self.password))
+        elif self.use_token:
+            headers = {
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.token}"
+            }
+            response = requests.request(
+                "GET",
+                self.BASE_URL + endpoint,
+                params=params,
+                headers=headers
+            )
+        else:
+            raise NotAuthenticatedError("Insufficient credentials")
         return self.parse(response)
 
     def _post(self, endpoint, params=None, data=None):
-        response = requests.post(
-            self.BASE_URL + endpoint,
-            params=params,
-            json=data,
-            auth=(self.user, self.password),
-        )
+        if self.use_password:
+            response = requests.post(self.BASE_URL + endpoint, params=params, json=data, auth=(self.user, self.password))
+        elif self.use_token:
+            headers = {
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.token}"
+            }
+            response = requests.request(
+                "POST",
+                self.BASE_URL + endpoint,
+                params=params, json=data,
+                headers=headers
+            )
+        else:
+            raise NotAuthenticatedError("Insufficient credentials")
         return self.parse(response)
 
     def _put(self, endpoint, params=None, data=None):
-        response = requests.put(
-            self.BASE_URL + endpoint,
-            params=params,
-            json=data,
-            auth=(self.user, self.password),
-        )
+        if self.use_password:
+            response = requests.put(self.BASE_URL + endpoint, params=params, json=data, auth=(self.user, self.password))
+        elif self.use_token:
+            headers = {
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.token}"
+            }
+            response = requests.request(
+                "PUT",
+                self.BASE_URL + endpoint,
+                params=params, json=data,
+                headers=headers
+            )
+        else:
+            raise NotAuthenticatedError("Insufficient credentials")
         return self.parse(response)
 
     def _delete(self, endpoint, params=None):
-        response = requests.delete(
-            self.BASE_URL + endpoint, params=params, auth=(self.user, self.password)
-        )
+        if self.use_password:
+            response = requests.delete(self.BASE_URL + endpoint, params=params, auth=(self.user, self.password))
+        elif self.use_token:
+            headers = {
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.token}"
+            }
+            response = requests.request(
+                "DELETE",
+                self.BASE_URL + endpoint,
+                params=params,
+                headers=headers
+            )
+        else:
+            raise NotAuthenticatedError("Insufficient credentials")
         return self.parse(response)
```

### Comparing `bitbucket_python-0.3.1/PKG-INFO` & `bitbucket_python-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-python
-Version: 0.3.1
+Version: 0.3.2
 Summary: API wrapper for Bitbucket written in Python
 License: MIT
 Author: Miguel Ferrer
 Author-email: ingferrermiguel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

