# Comparing `tmp/goalzero-0.2.1.tar.gz` & `tmp/goalzero-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goalzero-0.2.1.tar", last modified: Tue Nov  9 17:38:28 2021, max compression
+gzip compressed data, was "goalzero-0.2.2.tar", last modified: Fri Jul  7 21:52:12 2023, max compression
```

## Comparing `goalzero-0.2.1.tar` & `goalzero-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tkdrob     (501) staff       (20)        0 2021-11-09 17:38:28.244961 goalzero-0.2.1/
--rw-r--r--   0 tkdrob     (501) staff       (20)     1070 2021-10-15 09:05:28.000000 goalzero-0.2.1/LICENSE
--rw-r--r--   0 tkdrob     (501) staff       (20)      702 2021-11-09 17:38:28.244424 goalzero-0.2.1/PKG-INFO
--rw-r--r--   0 tkdrob     (501) staff       (20)      242 2021-10-15 09:05:28.000000 goalzero-0.2.1/README.md
-drwxr-xr-x   0 tkdrob     (501) staff       (20)        0 2021-11-09 17:38:28.239342 goalzero-0.2.1/goalzero/
--rw-r--r--   0 tkdrob     (501) staff       (20)     5541 2021-11-09 17:28:07.000000 goalzero-0.2.1/goalzero/__init__.py
--rw-r--r--   0 tkdrob     (501) staff       (20)      218 2021-11-09 17:08:58.000000 goalzero-0.2.1/goalzero/exceptions.py
-drwxr-xr-x   0 tkdrob     (501) staff       (20)        0 2021-11-09 17:38:28.242735 goalzero-0.2.1/goalzero.egg-info/
--rw-r--r--   0 tkdrob     (501) staff       (20)      702 2021-11-09 17:38:28.000000 goalzero-0.2.1/goalzero.egg-info/PKG-INFO
--rw-r--r--   0 tkdrob     (501) staff       (20)      229 2021-11-09 17:38:28.000000 goalzero-0.2.1/goalzero.egg-info/SOURCES.txt
--rw-r--r--   0 tkdrob     (501) staff       (20)        1 2021-11-09 17:38:28.000000 goalzero-0.2.1/goalzero.egg-info/dependency_links.txt
--rw-r--r--   0 tkdrob     (501) staff       (20)       15 2021-11-09 17:38:28.000000 goalzero-0.2.1/goalzero.egg-info/requires.txt
--rw-r--r--   0 tkdrob     (501) staff       (20)        9 2021-11-09 17:38:28.000000 goalzero-0.2.1/goalzero.egg-info/top_level.txt
--rw-r--r--   0 tkdrob     (501) staff       (20)       38 2021-11-09 17:38:28.245159 goalzero-0.2.1/setup.cfg
--rw-r--r--   0 tkdrob     (501) staff       (20)      702 2021-11-09 17:26:25.000000 goalzero-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:52:12.073564 goalzero-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 21:52:03.000000 goalzero-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-07 21:52:12.073564 goalzero-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-07 21:52:03.000000 goalzero-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:52:12.073564 goalzero-0.2.2/goalzero/
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-07 21:52:03.000000 goalzero-0.2.2/goalzero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 21:52:03.000000 goalzero-0.2.2/goalzero/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:52:12.073564 goalzero-0.2.2/goalzero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-07 21:52:12.000000 goalzero-0.2.2/goalzero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 21:52:12.000000 goalzero-0.2.2/goalzero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:52:12.000000 goalzero-0.2.2/goalzero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 21:52:12.000000 goalzero-0.2.2/goalzero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 21:52:12.000000 goalzero-0.2.2/goalzero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:52:12.073564 goalzero-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-07 21:52:10.000000 goalzero-0.2.2/setup.py
```

### Comparing `goalzero-0.2.1/LICENSE` & `goalzero-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goalzero-0.2.1/goalzero/__init__.py` & `goalzero-0.2.2/goalzero/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 HEADER = {
     "Content-Type": "application/json",
     "User-Agent": "YetiApp/1340 CFNetwork/1125.2 Darwin/19.4.0",
     "Connection": "keep-alive",
     "Accept": "application/json",
     "Accept-Language": "en-us",
-    "Content-Length": "19",
     "Accept-Encoding": "gzip, deflate",
     "Cache-Control": "no-cache",
 }
 TIMEOUT = 10
 
 semaphore = asyncio.Semaphore()
```

### Comparing `goalzero-0.2.1/setup.py` & `goalzero-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="goalzero",
-    version="0.2.1",
+    version="v0.2.2",
     author="Robert Hillis",
     author_email="tkdrob4390@yahoo.com",
     description="Goal Zero REST Api Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tkdrob/goalzero",
     packages=setuptools.find_packages(),
```

