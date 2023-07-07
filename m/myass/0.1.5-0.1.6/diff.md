# Comparing `tmp/myass-0.1.5.tar.gz` & `tmp/myass-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myass-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "myass-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `myass-0.1.5.tar` & `myass-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1080 2023-07-06 18:58:54.600427 myass-0.1.5/LICENSE
--rw-r--r--   0        0        0       56 2023-07-07 14:55:52.306405 myass-0.1.5/README.md
--rw-r--r--   0        0        0      414 2023-07-07 17:55:24.753812 myass-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       35 2023-07-07 17:55:41.446999 myass-0.1.5/src/myass/__init__.py
--rw-r--r--   0        0        0      705 2023-07-07 14:54:09.034059 myass-0.1.5/src/myass/assistant.py
--rw-r--r--   0        0        0      444 2023-07-07 17:51:03.762760 myass-0.1.5/src/myass/cli.py
--rw-r--r--   0        0        0      306 2023-07-07 14:37:18.963754 myass-0.1.5/src/myass/config.py
--rw-r--r--   0        0        0       25 2023-07-07 14:32:54.096308 myass-0.1.5/src/myass/config_default.yaml
--rw-r--r--   0        0        0      419 2023-07-07 17:21:07.335117 myass-0.1.5/src/myass/history.py
--rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 myass-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-06 18:58:54.600427 myass-0.1.6/LICENSE
+-rw-r--r--   0        0        0       56 2023-07-07 14:55:52.306405 myass-0.1.6/README.md
+-rw-r--r--   0        0        0      414 2023-07-07 17:55:24.753812 myass-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-07-07 17:58:06.695727 myass-0.1.6/src/myass/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-07 14:54:09.034059 myass-0.1.6/src/myass/assistant.py
+-rw-r--r--   0        0        0      444 2023-07-07 17:51:03.762760 myass-0.1.6/src/myass/cli.py
+-rw-r--r--   0        0        0      306 2023-07-07 14:37:18.963754 myass-0.1.6/src/myass/config.py
+-rw-r--r--   0        0        0       25 2023-07-07 14:32:54.096308 myass-0.1.6/src/myass/config_default.yaml
+-rw-r--r--   0        0        0      425 2023-07-07 17:57:57.339142 myass-0.1.6/src/myass/history.py
+-rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 myass-0.1.6/PKG-INFO
```

### Comparing `myass-0.1.5/LICENSE` & `myass-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myass-0.1.5/src/myass/assistant.py` & `myass-0.1.6/src/myass/assistant.py`

 * *Files identical despite different names*

