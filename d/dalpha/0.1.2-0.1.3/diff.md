# Comparing `tmp/dalpha-0.1.2.tar.gz` & `tmp/dalpha-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.1.2.tar", max compression
+gzip compressed data, was "dalpha-0.1.3.tar", max compression
```

## Comparing `dalpha-0.1.2.tar` & `dalpha-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      459 2023-05-28 23:48:43.785059 dalpha-0.1.2/README.md
--rw-r--r--   0        0        0     6431 2023-06-24 02:59:46.421105 dalpha-0.1.2/dalpha/__init__.py
--rw-r--r--   0        0        0      745 2023-06-24 04:10:36.493493 dalpha-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      459 2023-05-27 07:33:56.211092 dalpha-0.1.3/README.md
+-rw-r--r--   0        0        0     6455 2023-07-07 11:54:23.808631 dalpha-0.1.3/dalpha/__init__.py
+-rw-r--r--   0        0        0      745 2023-07-07 11:53:39.519356 dalpha-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.3/PKG-INFO
```

### Comparing `dalpha-0.1.2/dalpha/__init__.py` & `dalpha-0.1.3/dalpha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             if len(ret) == 0:
                 return None
             elif len(ret) == 1:
                 return ret[0]
             else:
                 return ret
 
+        time.sleep(0.2)
         url = f"{self.evaluate_url}/poll"
 
         headers = {
         'token': self.token
         }
         response = requests.request("GET", url, headers=headers)
         if response.status_code == 422:
```

### Comparing `dalpha-0.1.2/pyproject.toml` & `dalpha-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dalpha-0.1.2/PKG-INFO` & `dalpha-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

