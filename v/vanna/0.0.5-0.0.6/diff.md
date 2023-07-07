# Comparing `tmp/vanna-0.0.5.tar.gz` & `tmp/vanna-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.5.tar", last modified: Fri Jul  7 04:08:18 2023, max compression
+gzip compressed data, was "vanna-0.0.6.tar", last modified: Fri Jul  7 04:23:05 2023, max compression
```

## Comparing `vanna-0.0.5.tar` & `vanna-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 04:08:08.000000 vanna-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:08:18.743048 vanna-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 04:08:08.000000 vanna-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 04:08:08.000000 vanna-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 04:08:18.743048 vanna-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-07 04:08:08.000000 vanna-0.0.5/src/vanna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 04:08:08.000000 vanna-0.0.5/src/vanna/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.394998 vanna-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 04:22:55.000000 vanna-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:23:05.394998 vanna-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 04:22:55.000000 vanna-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 04:22:55.000000 vanna-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 04:23:05.394998 vanna-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.390998 vanna-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.390998 vanna-0.0.6/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-07 04:22:55.000000 vanna-0.0.6/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 04:22:55.000000 vanna-0.0.6/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.394998 vanna-0.0.6/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.5/LICENSE` & `vanna-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.5/PKG-INFO` & `vanna-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vanna-0.0.5/pyproject.toml` & `vanna-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vanna"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vanna-0.0.5/src/vanna/__init__.py` & `vanna-0.0.6/src/vanna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             return False
 
         status = Status(**d['result'])
 
         if not status.success:
             return False
 
-        otp = input("Enter OTP: ")
+        otp = input("Check your email for the code and enter it here: ")
 
     params = [UserOTP(email=email, otp=otp)]
 
     d = __unauthenticated_rpc_call(method="verify_otp", params=params)
 
     if 'result' not in d:
         return False
```

### Comparing `vanna-0.0.5/src/vanna/types.py` & `vanna-0.0.6/src/vanna/types.py`

 * *Files identical despite different names*

### Comparing `vanna-0.0.5/src/vanna.egg-info/PKG-INFO` & `vanna-0.0.6/src/vanna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

