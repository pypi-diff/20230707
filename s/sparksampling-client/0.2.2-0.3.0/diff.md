# Comparing `tmp/sparksampling_client-0.2.2.tar.gz` & `tmp/sparksampling_client-0.3.0.tar.gz`

## Comparing `sparksampling_client-0.2.2.tar` & `sparksampling_client-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/RELEASE.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/dockerbuild/config.json
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/dockerbuild/ssc.Dockerfile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/cli.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/logging.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/proto/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/proto/sampling_service_pb2.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/sparksampling_client/proto/sampling_service_pb2_grpc.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/tests/test_apply.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/.gitignore
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/LICENSE
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/README.md
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 sparksampling_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/dockerbuild/config.json
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/dockerbuild/ssc.Dockerfile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/cli.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/logging.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/proto/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/proto/sampling_service_pb2.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/sparksampling_client/proto/sampling_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/tests/test_apply.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/README.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 sparksampling_client-0.3.0/PKG-INFO
```

### Comparing `sparksampling_client-0.2.2/RELEASE.md` & `sparksampling_client-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/sparksampling_client/cli.py` & `sparksampling_client-0.3.0/sparksampling_client/cli.py`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/sparksampling_client/config.py` & `sparksampling_client-0.3.0/sparksampling_client/config.py`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/sparksampling_client/session.py` & `sparksampling_client-0.3.0/sparksampling_client/session.py`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/tests/test_apply.py` & `sparksampling_client-0.3.0/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/.gitignore` & `sparksampling_client-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/LICENSE` & `sparksampling_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/README.md` & `sparksampling_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sparksampling_client-0.2.2/pyproject.toml` & `sparksampling_client-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "sparksampling_client"
 description = "client for sparksampling"
 keywords = ["sparksampling_client", "pyspark-sampling"]
 requires-python = ">=3.7"
 dependencies = [
     'click',
-    'sparksampling_proto==0.0.1',
+    'sparksampling_proto==0.1.0',
 ]
 dynamic = ["version", ]
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `sparksampling_client-0.2.2/PKG-INFO` & `sparksampling_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksampling_client
-Version: 0.2.2
+Version: 0.3.0
 Summary: client for sparksampling
 Project-URL: Source, https://github.com/Wh1isper/pyspark-sampling
 Author-email: Wh1isper <9573586@qq.com>
 License: Apache License 2.0
 License-File: LICENSE
 Keywords: pyspark-sampling,sparksampling_client
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Requires-Dist: click
-Requires-Dist: sparksampling-proto==0.0.1
+Requires-Dist: sparksampling-proto==0.1.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 This is a Python Grpc Stub for ``sparksampling``
 
 # sparksampling
```

