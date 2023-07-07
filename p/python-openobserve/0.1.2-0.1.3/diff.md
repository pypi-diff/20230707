# Comparing `tmp/python_openobserve-0.1.2.tar.gz` & `tmp/python_openobserve-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_openobserve-0.1.2.tar", max compression
+gzip compressed data, was "python_openobserve-0.1.3.tar", max compression
```

## Comparing `python_openobserve-0.1.2.tar` & `python_openobserve-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-07-07 07:42:34.442507 python_openobserve-0.1.2/LICENSE
--rw-r--r--   0        0        0     1180 2023-07-07 09:13:16.438280 python_openobserve-0.1.2/README.md
--rw-r--r--   0        0        0      714 2023-07-07 09:30:35.254048 python_openobserve-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 07:43:49.510022 python_openobserve-0.1.2/python_openobserve/__init__.py
--rw-r--r--   0        0        0     3947 2023-07-07 09:30:29.405524 python_openobserve-0.1.2/python_openobserve/openobserve.py
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_openobserve-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-07 07:42:34.442507 python_openobserve-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1180 2023-07-07 09:13:16.438280 python_openobserve-0.1.3/README.md
+-rw-r--r--   0        0        0      714 2023-07-07 10:19:20.355949 python_openobserve-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 07:43:49.510022 python_openobserve-0.1.3/python_openobserve/__init__.py
+-rw-r--r--   0        0        0     3569 2023-07-07 10:16:51.502643 python_openobserve-0.1.3/python_openobserve/openobserve.py
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_openobserve-0.1.3/PKG-INFO
```

### Comparing `python_openobserve-0.1.2/LICENSE` & `python_openobserve-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_openobserve-0.1.2/README.md` & `python_openobserve-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `python_openobserve-0.1.2/pyproject.toml` & `python_openobserve-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-openobserve"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Justin Guese <guese.justin@gmail.com>"]
 license = "GNUv3"
 readme = "README.md"
 homepage = "https://github.com/JustinGuese/python-openobserve"
 repository = "https://github.com/JustinGuese/python-openobserve"
 keywords = ["openobserve", "elasticsearch", "logging", "unstructured data"]
```

### Comparing `python_openobserve-0.1.2/python_openobserve/openobserve.py` & `python_openobserve-0.1.3/python_openobserve/openobserve.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,14 @@
     def __unixTimestampConvert(self, timestamp: int) -> datetime:
         try: 
             timestamp = datetime.fromtimestamp(timestamp/1000000)
         except:
             print("could not convert timestamp: " + str(timestamp))
         return timestamp
     
-    def __float2Int(self, flatdict: dict) -> dict:
-        # apparently openobserve does not support float values?!
-        for key, val in flatdict.items():
-            if isinstance(val, float):
-                flatdict[key] = int(val)
-        return flatdict
-    
     def __intts2datetime(self, flatdict: dict) -> dict:
         for key, val in flatdict.items():
             if "time" in key:
                 flatdict[key] = self.__unixTimestampConvert(val)
         return flatdict
 
     def __datetime2Str(self, flatdict: dict) -> dict:
@@ -53,16 +46,14 @@
         return flatdict
 
     def index(self, index: str, document: dict):
         assert isinstance(document, dict), "document must be a dict"
         # expects a flattened json
         document = flatten(document)
         document = self.__datetime2Str(document)
-        # apparently openobserve does not support float values?!
-        document = self.__float2Int(document)
 
         res = requests.post(self.openobserve_url.replace("[STREAM]", index) + "/_json", headers=self.headers, json=[document])
         if res.status_code != 200:
             raise Exception(f"Openobserve returned {res.status_code}. Text: {res.text}")
         res = res.json()
         if res["status"][0]["failed"] > 0:
             raise Exception(f"Openobserve index failed. {res['status'][0]['error']}. document: {document}")
```

### Comparing `python_openobserve-0.1.2/PKG-INFO` & `python_openobserve-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-openobserve
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/JustinGuese/python-openobserve
 License: GNUv3
 Keywords: openobserve,elasticsearch,logging,unstructured data
 Author: Justin Guese
 Author-email: guese.justin@gmail.com
 Requires-Python: >3.9
```

