# Comparing `tmp/GreatCirclePaths-1.1.0.tar.gz` & `tmp/greatcirclepaths-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GreatCirclePaths-1.1.0.tar", max compression
+gzip compressed data, was "greatcirclepaths-1.1.2.tar", max compression
```

## Comparing `GreatCirclePaths-1.1.0.tar` & `greatcirclepaths-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35149 2021-04-16 09:46:24.755539 GreatCirclePaths-1.1.0/LICENSE
--rw-r--r--   0        0        0      926 2021-04-16 09:46:24.755539 GreatCirclePaths-1.1.0/greatcirclepaths/__init__.py
--rw-r--r--   0        0        0     4584 2021-04-16 09:46:24.755539 GreatCirclePaths-1.1.0/greatcirclepaths/gcpsampling.py
--rw-r--r--   0        0        0     4774 2021-04-16 09:46:24.755539 GreatCirclePaths-1.1.0/greatcirclepaths/gcpwork.py
--rw-r--r--   0        0        0     3152 2021-04-16 09:46:24.755539 GreatCirclePaths-1.1.0/greatcirclepaths/main.py
--rw-r--r--   0        0        0      433 2021-04-16 09:46:24.755539 GreatCirclePaths-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      670 2021-04-16 09:46:36.077767 GreatCirclePaths-1.1.0/setup.py
--rw-r--r--   0        0        0      489 2021-04-16 09:46:36.078132 GreatCirclePaths-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-07 00:39:52.553799 greatcirclepaths-1.1.2/LICENSE
+-rw-r--r--   0        0        0      926 2023-07-07 00:39:52.553799 greatcirclepaths-1.1.2/greatcirclepaths/__init__.py
+-rw-r--r--   0        0        0     4584 2023-07-07 00:39:52.553799 greatcirclepaths-1.1.2/greatcirclepaths/gcpsampling.py
+-rw-r--r--   0        0        0     4774 2023-07-07 00:39:52.553799 greatcirclepaths-1.1.2/greatcirclepaths/gcpwork.py
+-rw-r--r--   0        0        0     3152 2023-07-07 00:39:52.553799 greatcirclepaths-1.1.2/greatcirclepaths/main.py
+-rw-r--r--   0        0        0      476 2023-07-07 00:39:52.553799 greatcirclepaths-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 greatcirclepaths-1.1.2/PKG-INFO
```

### Comparing `GreatCirclePaths-1.1.0/LICENSE` & `greatcirclepaths-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GreatCirclePaths-1.1.0/greatcirclepaths/__init__.py` & `greatcirclepaths-1.1.2/greatcirclepaths/__init__.py`

 * *Files identical despite different names*

### Comparing `GreatCirclePaths-1.1.0/greatcirclepaths/gcpsampling.py` & `greatcirclepaths-1.1.2/greatcirclepaths/gcpsampling.py`

 * *Files identical despite different names*

### Comparing `GreatCirclePaths-1.1.0/greatcirclepaths/gcpwork.py` & `greatcirclepaths-1.1.2/greatcirclepaths/gcpwork.py`

 * *Files identical despite different names*

### Comparing `GreatCirclePaths-1.1.0/greatcirclepaths/main.py` & `greatcirclepaths-1.1.2/greatcirclepaths/main.py`

 * *Files identical despite different names*

