# Comparing `tmp/bullhorn-0.0.2.tar.gz` & `tmp/bullhorn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullhorn-0.0.2.tar", last modified: Fri Jul  7 07:52:32 2023, max compression
+gzip compressed data, was "bullhorn-0.0.3.tar", last modified: Fri Jul  7 07:56:02 2023, max compression
```

## Comparing `bullhorn-0.0.2.tar` & `bullhorn-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.496494 bullhorn-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-07-07 06:22:40.000000 bullhorn-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      532 2023-07-07 07:52:32.494491 bullhorn-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-06-05 13:48:02.000000 bullhorn-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.410265 bullhorn-0.0.2/bullhorn/
--rw-rw-rw-   0        0        0       93 2023-07-07 07:50:10.000000 bullhorn-0.0.2/bullhorn/__init__.py
--rw-rw-rw-   0        0        0     6371 2023-07-07 07:48:05.000000 bullhorn-0.0.2/bullhorn/client.py
--rw-rw-rw-   0        0        0     4924 2023-07-07 06:20:06.000000 bullhorn-0.0.2/bullhorn/exceptions.py
--rw-rw-rw-   0        0        0     1739 2023-07-07 06:25:00.000000 bullhorn-0.0.2/bullhorn/route.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.476442 bullhorn-0.0.2/bullhorn/types/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.2/bullhorn/types/__init__.py
--rw-rw-rw-   0        0        0       70 2023-07-07 06:28:51.000000 bullhorn-0.0.2/bullhorn/types/candidate.py
--rw-rw-rw-   0        0        0       38 2023-06-13 12:11:53.000000 bullhorn-0.0.2/bullhorn/types/ping.py
--rw-rw-rw-   0        0        0      216 2023-07-07 06:10:37.000000 bullhorn-0.0.2/bullhorn/types/placement.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.465411 bullhorn-0.0.2/bullhorn.egg-info/
--rw-rw-rw-   0        0        0      532 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.481456 bullhorn-0.0.2/examples/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.2/examples/__init__.py
--rw-rw-rw-   0        0        0      845 2023-07-07 07:48:13.000000 bullhorn-0.0.2/examples/get_placements_and_candidates.py
--rw-rw-rw-   0        0        0       42 2023-07-07 07:52:32.497496 bullhorn-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-07-07 07:52:06.000000 bullhorn-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.490479 bullhorn-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:33:32.000000 bullhorn-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      994 2023-07-07 07:48:16.000000 bullhorn-0.0.2/tests/test_client.py
--rw-rw-rw-   0        0        0     1074 2023-07-04 16:16:33.000000 bullhorn-0.0.2/tests/test_route.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:56:02.460854 bullhorn-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-07 06:22:40.000000 bullhorn-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      532 2023-07-07 07:56:02.458850 bullhorn-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-06-05 13:48:02.000000 bullhorn-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 07:56:02.393110 bullhorn-0.0.3/bullhorn/
+-rw-rw-rw-   0        0        0       93 2023-07-07 07:55:59.000000 bullhorn-0.0.3/bullhorn/__init__.py
+-rw-rw-rw-   0        0        0     6371 2023-07-07 07:48:05.000000 bullhorn-0.0.3/bullhorn/client.py
+-rw-rw-rw-   0        0        0     4924 2023-07-07 06:20:06.000000 bullhorn-0.0.3/bullhorn/exceptions.py
+-rw-rw-rw-   0        0        0     1739 2023-07-07 06:25:00.000000 bullhorn-0.0.3/bullhorn/route.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:56:02.441833 bullhorn-0.0.3/bullhorn/types/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.3/bullhorn/types/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-07-07 06:28:51.000000 bullhorn-0.0.3/bullhorn/types/candidate.py
+-rw-rw-rw-   0        0        0       38 2023-06-13 12:11:53.000000 bullhorn-0.0.3/bullhorn/types/ping.py
+-rw-rw-rw-   0        0        0      216 2023-07-07 06:10:37.000000 bullhorn-0.0.3/bullhorn/types/placement.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:56:02.430829 bullhorn-0.0.3/bullhorn.egg-info/
+-rw-rw-rw-   0        0        0      532 2023-07-07 07:56:02.000000 bullhorn-0.0.3/bullhorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-07-07 07:56:02.000000 bullhorn-0.0.3/bullhorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:56:02.000000 bullhorn-0.0.3/bullhorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-07 07:56:02.000000 bullhorn-0.0.3/bullhorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-07 07:56:02.000000 bullhorn-0.0.3/bullhorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 07:56:02.446815 bullhorn-0.0.3/examples/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.3/examples/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-07-07 07:48:13.000000 bullhorn-0.0.3/examples/get_placements_and_candidates.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 07:56:02.461857 bullhorn-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-07 07:55:53.000000 bullhorn-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:56:02.454838 bullhorn-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:33:32.000000 bullhorn-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      994 2023-07-07 07:48:16.000000 bullhorn-0.0.3/tests/test_client.py
+-rw-rw-rw-   0        0        0     1074 2023-07-04 16:16:33.000000 bullhorn-0.0.3/tests/test_route.py
```

### Comparing `bullhorn-0.0.2/LICENSE` & `bullhorn-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/PKG-INFO` & `bullhorn-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullhorn
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper for the Bullhorn REST API
 Home-page: https://github.com/recruithub/bullhorn
 Author: lloydtao (Lewis Lloyd)
 Author-email: lewis@recruit-hub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bullhorn-0.0.2/bullhorn/client.py` & `bullhorn-0.0.3/bullhorn/client.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/bullhorn/exceptions.py` & `bullhorn-0.0.3/bullhorn/exceptions.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/bullhorn/route.py` & `bullhorn-0.0.3/bullhorn/route.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/bullhorn.egg-info/PKG-INFO` & `bullhorn-0.0.3/bullhorn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullhorn
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper for the Bullhorn REST API
 Home-page: https://github.com/recruithub/bullhorn
 Author: lloydtao (Lewis Lloyd)
 Author-email: lewis@recruit-hub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bullhorn-0.0.2/examples/get_placements_and_candidates.py` & `bullhorn-0.0.3/examples/get_placements_and_candidates.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/setup.py` & `bullhorn-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="bullhorn",
-    version="0.0.2",
+    version="0.0.3",
     author="lloydtao (Lewis Lloyd)",
     author_email="lewis@recruit-hub.com",
     description="Python wrapper for the Bullhorn REST API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/recruithub/bullhorn",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.8.4",
-        "black==23.3.0",
-        "coverage==7.2.7",
-        "pytest==7.3.1",
-        "pytest-mock==3.10.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
```

### Comparing `bullhorn-0.0.2/tests/test_client.py` & `bullhorn-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/tests/test_route.py` & `bullhorn-0.0.3/tests/test_route.py`

 * *Files identical despite different names*

