# Comparing `tmp/afex-sso-0.0.59.tar.gz` & `tmp/afex-sso-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-sso-0.0.59.tar", last modified: Thu Jun 15 09:28:37 2023, max compression
+gzip compressed data, was "afex-sso-0.0.60.tar", last modified: Fri Jul  7 15:44:03 2023, max compression
```

## Comparing `afex-sso-0.0.59.tar` & `afex-sso-0.0.60.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.383061 afex-sso-0.0.59/
--rw-rw-rw-   0        0        0     1069 2023-04-05 13:47:57.000000 afex-sso-0.0.59/LICENSE
--rw-rw-rw-   0        0        0     2315 2023-06-15 09:28:37.383061 afex-sso-0.0.59/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2023-06-08 16:38:28.000000 afex-sso-0.0.59/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.285704 afex-sso-0.0.59/app/
-drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.316775 afex-sso-0.0.59/app/AFEX_SSO/
--rw-rw-rw-   0        0        0       36 2023-04-05 13:47:57.000000 afex-sso-0.0.59/app/AFEX_SSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.355975 afex-sso-0.0.59/app/AFEX_SSO/src/
--rw-rw-rw-   0        0        0        0 2023-04-05 13:47:57.000000 afex-sso-0.0.59/app/AFEX_SSO/src/__init__.py
--rw-rw-rw-   0        0        0      270 2023-06-07 09:13:59.000000 afex-sso-0.0.59/app/AFEX_SSO/src/get_hash_key.py
--rw-rw-rw-   0        0        0     2155 2023-06-08 16:53:35.000000 afex-sso-0.0.59/app/AFEX_SSO/src/sso.py
--rw-rw-rw-   0        0        0     2218 2023-06-14 13:06:41.000000 afex-sso-0.0.59/app/AFEX_SSO/src/views.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.383061 afex-sso-0.0.59/app/afex_sso.egg-info/
--rw-rw-rw-   0        0        0     2315 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-04-05 13:47:57.000000 afex-sso-0.0.59/pyproject.toml
--rw-rw-rw-   0        0        0      497 2023-06-15 09:28:37.383061 afex-sso-0.0.59/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-06-15 09:27:12.000000 afex-sso-0.0.59/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:44:03.924264 afex-sso-0.0.60/
+-rw-rw-rw-   0        0        0     1069 2023-04-05 13:47:57.000000 afex-sso-0.0.60/LICENSE
+-rw-rw-rw-   0        0        0     2315 2023-07-07 15:44:03.924264 afex-sso-0.0.60/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-06-08 16:38:28.000000 afex-sso-0.0.60/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 15:44:03.889115 afex-sso-0.0.60/app/
+drwxrwxrwx   0        0        0        0 2023-07-07 15:44:03.900151 afex-sso-0.0.60/app/AFEX_SSO/
+-rw-rw-rw-   0        0        0       36 2023-04-05 13:47:57.000000 afex-sso-0.0.60/app/AFEX_SSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:44:03.905158 afex-sso-0.0.60/app/AFEX_SSO/src/
+-rw-rw-rw-   0        0        0        0 2023-04-05 13:47:57.000000 afex-sso-0.0.60/app/AFEX_SSO/src/__init__.py
+-rw-rw-rw-   0        0        0      270 2023-06-07 09:13:59.000000 afex-sso-0.0.60/app/AFEX_SSO/src/get_hash_key.py
+-rw-rw-rw-   0        0        0     2293 2023-07-07 15:43:17.000000 afex-sso-0.0.60/app/AFEX_SSO/src/sso.py
+-rw-rw-rw-   0        0        0     2218 2023-06-14 13:06:41.000000 afex-sso-0.0.60/app/AFEX_SSO/src/views.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:44:03.922266 afex-sso-0.0.60/app/afex_sso.egg-info/
+-rw-rw-rw-   0        0        0     2315 2023-07-07 15:44:03.000000 afex-sso-0.0.60/app/afex_sso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-07-07 15:44:03.000000 afex-sso-0.0.60/app/afex_sso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:44:03.000000 afex-sso-0.0.60/app/afex_sso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-07 15:44:03.000000 afex-sso-0.0.60/app/afex_sso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 15:44:03.000000 afex-sso-0.0.60/app/afex_sso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-04-05 13:47:57.000000 afex-sso-0.0.60/pyproject.toml
+-rw-rw-rw-   0        0        0      497 2023-07-07 15:44:03.927276 afex-sso-0.0.60/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-07-07 15:43:57.000000 afex-sso-0.0.60/setup.py
```

### Comparing `afex-sso-0.0.59/LICENSE` & `afex-sso-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.59/PKG-INFO` & `afex-sso-0.0.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.59
+Version: 0.0.60
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Description: 
         # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.59/README.md` & `afex-sso-0.0.60/README.md`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.59/app/AFEX_SSO/src/sso.py` & `afex-sso-0.0.60/app/AFEX_SSO/src/sso.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,32 +26,37 @@
     #     self.session = session_key
 
     # def __call__(self):
     #     return self.check_credentials(self.api, self.hash, self.session)
 
 
     def check_credentials(self, session_key):
-        try:
-            HASH_KEY = get_hash_key(
-                api_key=API_KEY,
-                secret_key=SECRET_KEY,
-                idempotency_key=session_key
-            )
-            headers = {
-                "api-key": API_KEY,
-                "hash-key":  HASH_KEY,
-                "request-ts": session_key
-            }
-            response = requests.get(
-                f"{URL}/v1/api/verify_sp/{session_key}", headers=headers)
-            data = json.loads(response.text)
-            return data
+        # try:
+        print("API_KEY:", API_KEY)
+        print("SECRET:", SECRET_KEY)
+        HASH_KEY = get_hash_key(
+            api_key=API_KEY,
+            secret_key=SECRET_KEY,
+            idempotency_key=session_key
+        )
+        print("HASH:", HASH_KEY)
+        headers = {
+            "api-key": API_KEY,
+            "hash-key": HASH_KEY,
+            "request-ts": session_key
+        }
+        response = requests.get(
+            f"{URL}/v1/api/verify_sp/{session_key}", headers=headers)
+        print("response:", response)
+        print("response text:", response.text)
+        data = json.loads(response.text)
+        return data
 
-        except Exception as e:
-            return f"Something went wrong, please confirm the credentials and try again: {e}"
+        # except Exception as e:
+        #     return f"Something went wrong, please confirm the credentials and try again: {e}"
 
     def sign_out(self, email: str):
         try:
             REQUEST_TS = timezone.now()
             HASH_KEY = get_hash_key(
                 api_key=API_KEY,
                 secret_key=SECRET_KEY,
```

### Comparing `afex-sso-0.0.59/app/AFEX_SSO/src/views.py` & `afex-sso-0.0.60/app/AFEX_SSO/src/views.py`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.59/app/afex_sso.egg-info/PKG-INFO` & `afex-sso-0.0.60/app/afex_sso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.59
+Version: 0.0.60
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Description: 
         # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.59/setup.py` & `afex-sso-0.0.60/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="afex-sso",
-    version="0.0.59",
+    version="0.0.60",
     description="For integrating sso",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="AFEX NIGERIA",
```

