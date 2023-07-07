# Comparing `tmp/dafni-cli-dafni-facility-0.0.7.tar.gz` & `tmp/dafni-cli-dafni-facility-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dafni-cli-dafni-facility-0.0.7.tar", last modified: Tue Sep 21 13:39:29 2021, max compression
+gzip compressed data, was "dafni-cli-dafni-facility-0.0.8.tar", last modified: Fri Jul  7 16:27:55 2023, max compression
```

## Comparing `dafni-cli-dafni-facility-0.0.7.tar` & `dafni-cli-dafni-facility-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 13:39:29.787744 dafni-cli-dafni-facility-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-09-21 13:39:16.000000 dafni-cli-dafni-facility-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      724 2021-09-21 13:39:29.787744 dafni-cli-dafni-facility-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-09-21 13:39:16.000000 dafni-cli-dafni-facility-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 13:39:29.787744 dafni-cli-dafni-facility-0.0.7/dafni_cli/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-21 13:39:16.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2021-09-21 13:39:16.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2021-09-21 13:39:16.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli/nims.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2021-09-21 13:39:16.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 13:39:29.787744 dafni-cli-dafni-facility-0.0.7/dafni_cli_dafni_facility.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2021-09-21 13:39:29.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli_dafni_facility.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-09-21 13:39:29.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli_dafni_facility.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-21 13:39:29.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli_dafni_facility.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-21 13:39:29.000000 dafni-cli-dafni-facility-0.0.7/dafni_cli_dafni_facility.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-21 13:39:29.787744 dafni-cli-dafni-facility-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      782 2021-09-21 13:39:16.000000 dafni-cli-dafni-facility-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:55.483236 dafni-cli-dafni-facility-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-07 16:27:42.000000 dafni-cli-dafni-facility-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-07 16:27:55.483236 dafni-cli-dafni-facility-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-07 16:27:42.000000 dafni-cli-dafni-facility-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:55.483236 dafni-cli-dafni-facility-0.0.8/dafni_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 16:27:42.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-07 16:27:42.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-07 16:27:42.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli/nims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-07 16:27:42.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:55.483236 dafni-cli-dafni-facility-0.0.8/dafni_cli_dafni_facility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-07 16:27:55.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli_dafni_facility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-07 16:27:55.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli_dafni_facility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:27:55.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli_dafni_facility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 16:27:55.000000 dafni-cli-dafni-facility-0.0.8/dafni_cli_dafni_facility.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:27:55.483236 dafni-cli-dafni-facility-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-07 16:27:42.000000 dafni-cli-dafni-facility-0.0.8/setup.py
```

### Comparing `dafni-cli-dafni-facility-0.0.7/LICENSE` & `dafni-cli-dafni-facility-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dafni-cli-dafni-facility-0.0.7/PKG-INFO` & `dafni-cli-dafni-facility-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dafni-cli-dafni-facility
-Version: 0.0.7
+Version: 0.0.8
 Summary: The beginnings of a command line interface for DAFNI. This package is still in development and not ready for use.
 Home-page: https://github.com/dafnifacility/command-line-interface/
 Author: DAFNI Facility
 Author-email: support@dafni.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dafni-cli-dafni-facility-0.0.7/dafni_cli/login.py` & `dafni-cli-dafni-facility-0.0.8/dafni_cli/login.py`

 * *Files identical despite different names*

### Comparing `dafni-cli-dafni-facility-0.0.7/dafni_cli/nims.py` & `dafni-cli-dafni-facility-0.0.8/dafni_cli/nims.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import requests
+from json.decoder import JSONDecodeError
 from pathlib import Path
-from dafni_cli.urls import MODELS_API_URL
-from requests import Response
 from typing import Optional
-from json.decoder import JSONDecodeError
+
+import requests
+from requests import Response
+from urls import MODELS_API_URL
 
 
 class NIMSError(Exception):
     def __init__(self, prefix: str, response: Response):
         self.prefix = prefix
         self.response = response
 
@@ -60,18 +61,27 @@
     if urls_resp.status_code != 200:
         raise NIMSError("Getting upload URLs", urls_resp)
     upload_id = urls_resp.json()["id"]
     urls = urls_resp.json()["urls"]
     return upload_id, urls
 
 
+def replace_minio_url(presigned_url: str) -> str:
+    proxy_url = "https://fwd.secure.dafni.rl.ac.uk/nidminio/"
+    minio_url = "https://minio.secure.dafni.rl.ac.uk/"
+    stripped_url = presigned_url.removeprefix(minio_url)
+    return f"{proxy_url}{stripped_url}"
+
+
 def upload_file_to_minio(jwt: str, url: str, file_path: Path) -> None:
     upload_headers = {"Authorization": jwt, "Content-Type": "multipart/form-data"}
     with file_path.open("rb") as file_data:
-        response = requests.put(url, headers=upload_headers, data=file_data)
+        response = requests.put(
+            replace_minio_url(url), headers=upload_headers, data=file_data
+        )
         if response.status_code != 200:
             raise NIMSError("Uploading to Minio", response)
 
 
 def ingest_model(
     jwt: str, upload_id: str, version_message: str, model_id: Optional[str] = None
 ) -> None:
```

### Comparing `dafni-cli-dafni-facility-0.0.7/dafni_cli_dafni_facility.egg-info/PKG-INFO` & `dafni-cli-dafni-facility-0.0.8/dafni_cli_dafni_facility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dafni-cli-dafni-facility
-Version: 0.0.7
+Version: 0.0.8
 Summary: The beginnings of a command line interface for DAFNI. This package is still in development and not ready for use.
 Home-page: https://github.com/dafnifacility/command-line-interface/
 Author: DAFNI Facility
 Author-email: support@dafni.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dafni-cli-dafni-facility-0.0.7/setup.py` & `dafni-cli-dafni-facility-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dafni-cli-dafni-facility",
-    version="0.0.7",
+    version="0.0.8",
     author="DAFNI Facility",
     author_email="support@dafni.ac.uk",
     description="The beginnings of a command line interface for DAFNI. This package is still in development and not ready for use.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dafnifacility/command-line-interface/",
     packages=setuptools.find_packages(),
```

