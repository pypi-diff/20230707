# Comparing `tmp/moore-itertools-0.0.1.tar.gz` & `tmp/moore-itertools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moore-itertools-0.0.1.tar", last modified: Thu Jul  6 01:53:42 2023, max compression
+gzip compressed data, was "moore-itertools-0.0.2.tar", last modified: Fri Jul  7 06:11:12 2023, max compression
```

## Comparing `moore-itertools-0.0.1.tar` & `moore-itertools-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-06 01:53:42.692348 moore-itertools-0.0.1/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1475 2023-07-06 01:22:24.000000 moore-itertools-0.0.1/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       33 2023-07-06 01:40:22.000000 moore-itertools-0.0.1/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)      613 2023-07-06 01:53:42.688348 moore-itertools-0.0.1/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      165 2023-07-06 01:21:23.000000 moore-itertools-0.0.1/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-06 01:53:42.688348 moore-itertools-0.0.1/moore_itertools/
--rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-07-06 01:30:00.000000 moore-itertools-0.0.1/moore_itertools/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2701 2023-07-06 01:50:10.000000 moore-itertools-0.0.1/moore_itertools/product.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-07-06 01:40:26.000000 moore-itertools-0.0.1/moore_itertools/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-06 01:53:42.688348 moore-itertools-0.0.1/moore_itertools.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)      613 2023-07-06 01:53:42.000000 moore-itertools-0.0.1/moore_itertools.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      322 2023-07-06 01:53:42.000000 moore-itertools-0.0.1/moore_itertools.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-07-06 01:53:42.000000 moore-itertools-0.0.1/moore_itertools.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      100 2023-07-06 01:53:42.000000 moore-itertools-0.0.1/moore_itertools.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       16 2023-07-06 01:53:42.000000 moore-itertools-0.0.1/moore_itertools.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1344 2023-07-06 01:25:18.000000 moore-itertools-0.0.1/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-07-06 01:53:42.692348 moore-itertools-0.0.1/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1475 2023-07-06 01:22:24.000000 moore-itertools-0.0.2/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       33 2023-07-06 01:40:22.000000 moore-itertools-0.0.2/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)      612 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      164 2023-07-07 06:10:06.000000 moore-itertools-0.0.2/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/moore_itertools/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-07-07 06:09:43.000000 moore-itertools-0.0.2/moore_itertools/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2693 2023-07-07 06:07:15.000000 moore-itertools-0.0.2/moore_itertools/product.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-07-06 01:40:26.000000 moore-itertools-0.0.2/moore_itertools/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/moore_itertools.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      612 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      322 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      100 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       16 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1344 2023-07-06 01:25:18.000000 moore-itertools-0.0.2/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/setup.cfg
```

### Comparing `moore-itertools-0.0.1/LICENSE.txt` & `moore-itertools-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moore-itertools-0.0.1/PKG-INFO` & `moore-itertools-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: moore-itertools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Moore Itertools
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# `moore_itertools` 
+# `moore_itertools`
 
 This exists mostly as a pun on `more_itertools`.
 
 So far there's only one thing in it, a memoizing cartesian product for unbounded iterators.
```

### Comparing `moore-itertools-0.0.1/moore_itertools/product.py` & `moore-itertools-0.0.2/moore_itertools/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Iterable, Iterator, Tuple, TypeVar
 
-TypeA = TypeVar("A")
-TypeB = TypeVar("B")
+A = TypeVar("A")
+B = TypeVar("B")
 
 
 def product(iterable1: Iterable[A], iterable2: Iterable[B]) -> Iterator[Tuple[A, B]]:
     """Return the cartesian product of two iterables, iterable1 and iterable2,
     in such a way that either or both can be infinite, or at least very large.
 
     Values from the iterables are memoized until they are no longer needed.
```

### Comparing `moore-itertools-0.0.1/moore_itertools.egg-info/PKG-INFO` & `moore-itertools-0.0.2/moore_itertools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: moore-itertools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Moore Itertools
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# `moore_itertools` 
+# `moore_itertools`
 
 This exists mostly as a pun on `more_itertools`.
 
 So far there's only one thing in it, a memoizing cartesian product for unbounded iterators.
```

### Comparing `moore-itertools-0.0.1/pyproject.toml` & `moore-itertools-0.0.2/pyproject.toml`

 * *Files identical despite different names*

