# Comparing `tmp/pyassorted-0.7.0.tar.gz` & `tmp/pyassorted-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassorted-0.7.0.tar", max compression
+gzip compressed data, was "pyassorted-0.7.1.tar", max compression
```

## Comparing `pyassorted-0.7.0.tar` & `pyassorted-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,28 @@
--rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.7.0/LICENSE
--rw-r--r--   0        0        0     6993 2023-05-27 10:21:48.697675 pyassorted-0.7.0/README.md
--rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.7.0/pyassorted/__init__.py
--rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.7.0/pyassorted/asyncio/__init__.py
--rw-r--r--   0        0        0      274 2023-02-17 09:42:49.535612 pyassorted-0.7.0/pyassorted/asyncio/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1464 2023-04-01 13:44:11.024962 pyassorted-0.7.0/pyassorted/asyncio/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0        0        0     4230 2023-05-15 11:57:36.220568 pyassorted-0.7.0/pyassorted/asyncio/__pycache__/io.cpython-38.pyc
--rw-r--r--   0        0        0     1122 2023-02-17 09:42:49.536169 pyassorted-0.7.0/pyassorted/asyncio/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.7.0/pyassorted/asyncio/executor.py
--rw-r--r--   0        0        0     2943 2023-05-15 11:57:33.581730 pyassorted-0.7.0/pyassorted/asyncio/io.py
--rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.7.0/pyassorted/asyncio/utils.py
--rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.7.0/pyassorted/cache/__init__.py
--rw-r--r--   0        0        0      234 2023-03-27 15:28:17.796798 pyassorted-0.7.0/pyassorted/cache/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8084 2023-03-27 15:28:17.797797 pyassorted-0.7.0/pyassorted/cache/__pycache__/cache.cpython-38.pyc
--rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.7.0/pyassorted/cache/cache.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:33.581794 pyassorted-0.7.0/pyassorted/collections/__init__.py
--rw-r--r--   0        0        0      161 2023-05-15 11:57:36.227591 pyassorted-0.7.0/pyassorted/collections/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      161 2023-05-12 10:18:30.820949 pyassorted-0.7.0/pyassorted/collections/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3543 2023-05-15 11:57:36.228447 pyassorted-0.7.0/pyassorted/collections/__pycache__/sqlitedict.cpython-38.pyc
--rw-r--r--   0        0        0     2397 2023-05-12 13:31:22.778494 pyassorted-0.7.0/pyassorted/collections/__pycache__/sqlitedict.cpython-39.pyc
--rw-r--r--   0        0        0     2853 2023-05-15 11:57:33.582142 pyassorted-0.7.0/pyassorted/collections/sqlitedict.py
--rw-r--r--   0        0        0      148 2023-05-15 11:57:33.582436 pyassorted-0.7.0/pyassorted/datetime/__init__.py
--rw-r--r--   0        0        0      307 2023-05-15 11:57:36.283378 pyassorted-0.7.0/pyassorted/datetime/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1329 2023-05-15 11:57:36.283815 pyassorted-0.7.0/pyassorted/datetime/__pycache__/datetime.cpython-38.pyc
--rw-r--r--   0        0        0     2677 2023-05-15 11:57:36.286067 pyassorted-0.7.0/pyassorted/datetime/__pycache__/timer.cpython-38.pyc
--rw-r--r--   0        0        0     1052 2023-05-15 11:57:33.582699 pyassorted-0.7.0/pyassorted/datetime/datetime.py
--rw-r--r--   0        0        0     2013 2023-05-15 11:57:33.582972 pyassorted-0.7.0/pyassorted/datetime/timer.py
--rw-r--r--   0        0        0     2602 2023-05-27 09:28:47.211929 pyassorted-0.7.0/pyassorted/io/__init__.py
--rw-r--r--   0        0        0     2977 2023-05-27 09:56:02.607170 pyassorted-0.7.0/pyassorted/io/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2077 2023-05-27 09:56:02.608697 pyassorted-0.7.0/pyassorted/io/__pycache__/watch.cpython-38.pyc
--rw-r--r--   0        0        0     2365 2023-05-27 09:28:47.212292 pyassorted-0.7.0/pyassorted/io/watch.py
--rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.7.0/pyassorted/lock/__init__.py
--rw-r--r--   0        0        0      217 2023-04-01 13:44:11.042381 pyassorted-0.7.0/pyassorted/lock/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2117 2023-03-30 05:48:46.562703 pyassorted-0.7.0/pyassorted/lock/__pycache__/filelock.cpython-38-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3807 2023-04-01 13:44:11.043169 pyassorted-0.7.0/pyassorted/lock/__pycache__/filelock.cpython-38.pyc
--rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.7.0/pyassorted/lock/filelock.py
--rw-r--r--   0        0        0       18 2023-05-27 09:28:47.212721 pyassorted-0.7.0/pyassorted/version.py
--rw-r--r--   0        0        0      546 2023-05-27 10:23:53.237973 pyassorted-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 pyassorted-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6993 2023-05-27 10:25:12.261799 pyassorted-0.7.1/README.md
+-rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.7.1/pyassorted/__init__.py
+-rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.7.1/pyassorted/asyncio/__init__.py
+-rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.7.1/pyassorted/asyncio/executor.py
+-rw-r--r--   0        0        0     2943 2023-05-15 11:57:33.581730 pyassorted-0.7.1/pyassorted/asyncio/io.py
+-rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.7.1/pyassorted/asyncio/utils.py
+-rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.7.1/pyassorted/cache/__init__.py
+-rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.7.1/pyassorted/cache/cache.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:57:33.581794 pyassorted-0.7.1/pyassorted/collections/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-15 11:57:33.582142 pyassorted-0.7.1/pyassorted/collections/sqlitedict.py
+-rw-r--r--   0        0        0      148 2023-05-15 11:57:33.582436 pyassorted-0.7.1/pyassorted/datetime/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-15 11:57:33.582699 pyassorted-0.7.1/pyassorted/datetime/datetime.py
+-rw-r--r--   0        0        0     2013 2023-05-15 11:57:33.582972 pyassorted-0.7.1/pyassorted/datetime/timer.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:04:26.629790 pyassorted-0.7.1/pyassorted/encrypt/__init__.py
+-rw-r--r--   0        0        0     2257 2023-07-07 10:20:46.735970 pyassorted-0.7.1/pyassorted/encrypt/io.py
+-rw-r--r--   0        0        0     2602 2023-05-27 10:25:12.262734 pyassorted-0.7.1/pyassorted/io/__init__.py
+-rw-r--r--   0        0        0     2365 2023-05-27 10:25:12.262951 pyassorted-0.7.1/pyassorted/io/watch.py
+-rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.7.1/pyassorted/lock/__init__.py
+-rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.7.1/pyassorted/lock/filelock.py
+-rw-r--r--   0        0        0        0 2023-07-07 10:23:45.350340 pyassorted-0.7.1/pyassorted/standard/__init__.py
+-rw-r--r--   0        0        0     2788 2023-07-07 10:57:46.398428 pyassorted-0.7.1/pyassorted/standard/language_code.py
+-rw-r--r--   0        0        0      130 2023-06-08 14:19:30.918842 pyassorted-0.7.1/pyassorted/string/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-08 14:18:59.300447 pyassorted-0.7.1/pyassorted/string/rand.py
+-rw-r--r--   0        0        0     1924 2023-06-06 09:03:20.787667 pyassorted-0.7.1/pyassorted/string/replace.py
+-rw-r--r--   0        0        0       18 2023-07-07 11:01:35.387512 pyassorted-0.7.1/pyassorted/version.py
+-rw-r--r--   0        0        0      546 2023-07-07 11:01:27.048472 pyassorted-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 pyassorted-0.7.1/PKG-INFO
```

### Comparing `pyassorted-0.7.0/LICENSE` & `pyassorted-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/README.md` & `pyassorted-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/asyncio/executor.py` & `pyassorted-0.7.1/pyassorted/asyncio/executor.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/asyncio/io.py` & `pyassorted-0.7.1/pyassorted/asyncio/io.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/asyncio/utils.py` & `pyassorted-0.7.1/pyassorted/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/cache/cache.py` & `pyassorted-0.7.1/pyassorted/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/collections/sqlitedict.py` & `pyassorted-0.7.1/pyassorted/collections/sqlitedict.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/datetime/datetime.py` & `pyassorted-0.7.1/pyassorted/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/datetime/timer.py` & `pyassorted-0.7.1/pyassorted/datetime/timer.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/io/__init__.py` & `pyassorted-0.7.1/pyassorted/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/io/watch.py` & `pyassorted-0.7.1/pyassorted/io/watch.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyassorted/lock/filelock.py` & `pyassorted-0.7.1/pyassorted/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.0/pyproject.toml` & `pyassorted-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyassorted"
-version = "0.7.0"
+version = "0.7.1"
 description = "A library has light-weight assorted utils in Prue-Python."
 authors = ["Allen Chou <f1470891079@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1, <4.0.0"
```

### Comparing `pyassorted-0.7.0/PKG-INFO` & `pyassorted-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyassorted
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library has light-weight assorted utils in Prue-Python.
 License: MIT
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

