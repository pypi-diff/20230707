# Comparing `tmp/winnie-0.0.5.tar.gz` & `tmp/winnie-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winnie-0.0.5.tar", last modified: Mon Jun 19 15:27:27 2023, max compression
+gzip compressed data, was "winnie-0.0.6.tar", last modified: Fri Jul  7 14:15:21 2023, max compression
```

## Comparing `winnie-0.0.5.tar` & `winnie-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 15:27:27.865940 winnie-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 15:27:11.000000 winnie-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 15:27:11.000000 winnie-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-19 15:27:27.865940 winnie-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 15:27:11.000000 winnie-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.861940 winnie-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/src/winnie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/listops.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/resourceMask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/src/winnie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 15:27:11.000000 winnie-0.0.5/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:15:21.371772 winnie-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 14:15:02.000000 winnie-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 14:15:21.371772 winnie-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-07 14:15:02.000000 winnie-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-07 14:15:02.000000 winnie-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-07 14:15:21.371772 winnie-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 14:15:02.000000 winnie-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:15:21.363772 winnie-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:15:21.367772 winnie-0.0.6/src/winnie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/byteops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/listops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/resourceMask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/sessionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 14:15:02.000000 winnie-0.0.6/src/winnie/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:15:21.367772 winnie-0.0.6/src/winnie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 14:15:21.000000 winnie-0.0.6/src/winnie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-07 14:15:21.000000 winnie-0.0.6/src/winnie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:15:21.000000 winnie-0.0.6/src/winnie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:15:21.000000 winnie-0.0.6/src/winnie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 14:15:21.000000 winnie-0.0.6/src/winnie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 14:15:21.000000 winnie-0.0.6/src/winnie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:15:21.371772 winnie-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-07 14:15:02.000000 winnie-0.0.6/tests/test_byteops.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 14:15:02.000000 winnie-0.0.6/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-07 14:15:02.000000 winnie-0.0.6/tests/test_resourceMask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-07 14:15:02.000000 winnie-0.0.6/tests/test_sessionStatus.py
```

### Comparing `winnie-0.0.5/PKG-INFO` & `winnie-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.5
+Version: 0.0.6
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
 
 # winnie
 
 <!-- Remember to change the URL from winnie to the name of your project -->
 ![Tests](https://github.com/HWRacing/winnie/actions/workflows/tests.yml/badge.svg)
 
 A library for the CAN calibration protocol
```

### Comparing `winnie-0.0.5/setup.cfg` & `winnie-0.0.6/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = winnie
-version = v0.0.5
+version = v0.0.6
 author = HWRacing
 author_email = fs60@hw.ac.uk
 description = CCP library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/winnie
 project_urls = 
@@ -12,14 +12,15 @@
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	License :: OSI Approved :: MIT License
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 zip_safe = no
```

### Comparing `winnie-0.0.5/src/winnie/listops.py` & `winnie-0.0.6/src/winnie/listops.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 		output.reverse()
 	return output
 
 def padToLength(l: List, targetLength: int, padding=None) -> List:
 	currentLength = len(l)
 	if currentLength > targetLength:
 		raise ValueError(f"List too long ({currentLength}) for target length ({targetLength})")
-	l.extend([padding] * targetLength - currentLength)
+	l.extend([padding] * (targetLength - currentLength))
 	return l
 
 def listToInt(l: List[int]) -> int:
 	result = 0
 	for i in l:
 		result = (result << 8) | i
 	return result
```

### Comparing `winnie-0.0.5/src/winnie.egg-info/PKG-INFO` & `winnie-0.0.6/src/winnie.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.5
+Version: 0.0.6
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
 
 # winnie
 
 <!-- Remember to change the URL from winnie to the name of your project -->
 ![Tests](https://github.com/HWRacing/winnie/actions/workflows/tests.yml/badge.svg)
 
 A library for the CAN calibration protocol
```

