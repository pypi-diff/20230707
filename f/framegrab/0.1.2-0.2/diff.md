# Comparing `tmp/framegrab-0.1.2.tar.gz` & `tmp/framegrab-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framegrab-0.1.2.tar", max compression
+gzip compressed data, was "framegrab-0.2.tar", max compression
```

## Comparing `framegrab-0.1.2.tar` & `framegrab-0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2906 2023-06-16 19:22:23.911372 framegrab-0.1.2/README.md
--rw-r--r--   0        0        0      487 2023-06-25 22:41:55.703134 framegrab-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      388 2023-06-25 22:41:55.703396 framegrab-0.1.2/src/framegrab/__init__.py
--rw-r--r--   0        0        0    10360 2023-06-16 19:22:23.911782 framegrab-0.1.2/src/framegrab/grabber.py
--rw-r--r--   0        0        0     2456 2023-06-24 01:53:17.596683 framegrab-0.1.2/src/framegrab/motion.py
--rw-r--r--   0        0        0     3678 1970-01-01 00:00:00.000000 framegrab-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.2/LICENSE.txt
+-rw-r--r--   0        0        0     5638 2023-07-07 20:44:56.340056 framegrab-0.2/README.md
+-rw-r--r--   0        0        0      485 2023-07-07 20:44:56.340418 framegrab-0.2/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-06-25 22:41:55.703396 framegrab-0.2/src/framegrab/__init__.py
+-rw-r--r--   0        0        0    30230 2023-07-07 20:44:56.340879 framegrab-0.2/src/framegrab/grabber.py
+-rw-r--r--   0        0        0     2456 2023-07-07 20:44:37.695695 framegrab-0.2/src/framegrab/motion.py
+-rw-r--r--   0        0        0     6408 1970-01-01 00:00:00.000000 framegrab-0.2/PKG-INFO
```

### Comparing `framegrab-0.1.2/LICENSE.txt` & `framegrab-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `framegrab-0.1.2/src/framegrab/motion.py` & `framegrab-0.2/src/framegrab/motion.py`

 * *Files identical despite different names*

