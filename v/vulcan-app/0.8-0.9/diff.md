# Comparing `tmp/vulcan-app-0.8.tar.gz` & `tmp/vulcan-app-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-app-0.8.tar", last modified: Fri Feb 24 10:12:33 2023, max compression
+gzip compressed data, was "vulcan-app-0.9.tar", last modified: Fri Feb 24 10:17:14 2023, max compression
```

## Comparing `vulcan-app-0.8.tar` & `vulcan-app-0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:12:33.108860 vulcan-app-0.8/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-0.8/LICENSE
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-02-24 10:12:33.108860 vulcan-app-0.8/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-0.8/README.md
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-02-24 10:12:33.108860 vulcan-app-0.8/setup.cfg
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1142 2023-02-24 10:12:22.000000 vulcan-app-0.8/setup.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:12:33.108860 vulcan-app-0.8/vulcan_app/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      472 2023-02-15 13:42:27.000000 vulcan-app-0.8/vulcan_app/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-0.8/vulcan_app/configuration.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:12:33.108860 vulcan-app-0.8/vulcan_app/database/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-0.8/vulcan_app/database/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-0.8/vulcan_app/database/mongo.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-0.8/vulcan_app/database/postgre.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-0.8/vulcan_app/database/tunnel.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     5132 2023-02-15 13:40:54.000000 vulcan-app-0.8/vulcan_app/security.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-0.8/vulcan_app/services.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-02-12 04:50:57.000000 vulcan-app-0.8/vulcan_app/worklog_processor.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:12:33.108860 vulcan-app-0.8/vulcan_app.egg-info/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-02-24 10:12:33.000000 vulcan-app-0.8/vulcan_app.egg-info/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-02-24 10:12:33.000000 vulcan-app-0.8/vulcan_app.egg-info/SOURCES.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-02-24 10:12:33.000000 vulcan-app-0.8/vulcan_app.egg-info/dependency_links.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      146 2023-02-24 10:12:33.000000 vulcan-app-0.8/vulcan_app.egg-info/requires.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-02-24 10:12:33.000000 vulcan-app-0.8/vulcan_app.egg-info/top_level.txt
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-0.9/LICENSE
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-02-24 10:17:14.643606 vulcan-app-0.9/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-0.9/README.md
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-02-24 10:17:14.647606 vulcan-app-0.9/setup.cfg
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1157 2023-02-24 10:17:08.000000 vulcan-app-0.9/setup.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/vulcan_app/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      472 2023-02-15 13:42:27.000000 vulcan-app-0.9/vulcan_app/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-0.9/vulcan_app/configuration.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/vulcan_app/database/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-0.9/vulcan_app/database/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-0.9/vulcan_app/database/mongo.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-0.9/vulcan_app/database/postgre.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-0.9/vulcan_app/database/tunnel.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     5132 2023-02-15 13:40:54.000000 vulcan-app-0.9/vulcan_app/security.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-0.9/vulcan_app/services.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-02-12 04:50:57.000000 vulcan-app-0.9/vulcan_app/worklog_processor.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/vulcan_app.egg-info/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/SOURCES.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/dependency_links.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      161 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/requires.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/top_level.txt
```

### Comparing `vulcan-app-0.8/LICENSE` & `vulcan-app-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/PKG-INFO` & `vulcan-app-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 0.8
+Version: 0.9
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-app-0.8/setup.py` & `vulcan-app-0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vulcan-app",
-    version="0.8",
+    version="0.9",
     author="Chatavut Viriyasuthee",
     author_email="chatavut@lab.ai",
     description="Vulcan's web application server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vulcan-coalition/vulcan-app.git",
     packages=["vulcan_app", "vulcan_app.database"],
@@ -22,23 +22,23 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
         "aiofiles",
         "fastapi",
-        "httpx",
+        "httpx==0.23.3",
         "pydantic",
         "PyJWT",
         "pytz",
         "requests",
         "requests-async",
         "SQLAlchemy",
         "PyDrive2",
         "pymongo",
         "boto3",
         "asyncpg",
         "shortuuid",
         "python-multipart",
-        "sshtunnel"
+        "sshtunnel==0.4.0"
     ]
 )
```

### Comparing `vulcan-app-0.8/vulcan_app/configuration.py` & `vulcan-app-0.9/vulcan_app/configuration.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/vulcan_app/database/__init__.py` & `vulcan-app-0.9/vulcan_app/database/__init__.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/vulcan_app/database/postgre.py` & `vulcan-app-0.9/vulcan_app/database/postgre.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/vulcan_app/database/tunnel.py` & `vulcan-app-0.9/vulcan_app/database/tunnel.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/vulcan_app/security.py` & `vulcan-app-0.9/vulcan_app/security.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/vulcan_app/services.py` & `vulcan-app-0.9/vulcan_app/services.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/vulcan_app/worklog_processor.py` & `vulcan-app-0.9/vulcan_app/worklog_processor.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.8/vulcan_app.egg-info/PKG-INFO` & `vulcan-app-0.9/vulcan_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 0.8
+Version: 0.9
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

