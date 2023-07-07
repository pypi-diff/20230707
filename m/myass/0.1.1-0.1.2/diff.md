# Comparing `tmp/myass-0.1.1.tar.gz` & `tmp/myass-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myass-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "myass-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `myass-0.1.1.tar` & `myass-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1080 2023-07-06 18:58:54.600427 myass-0.1.1/LICENSE
--rw-r--r--   0        0        0       56 2023-07-06 22:09:52.816683 myass-0.1.1/README.md
--rw-r--r--   0        0        0      403 2023-07-07 14:41:42.624549 myass-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-07-07 14:39:12.385995 myass-0.1.1/src/myass/__init__.py
--rw-r--r--   0        0        0      730 2023-07-07 14:37:11.663825 myass-0.1.1/src/myass/assistant.py
--rw-r--r--   0        0        0      375 2023-07-07 14:43:46.730022 myass-0.1.1/src/myass/cli.py
--rw-r--r--   0        0        0      306 2023-07-07 14:37:18.963754 myass-0.1.1/src/myass/config.py
--rw-r--r--   0        0        0       25 2023-07-07 14:32:54.096308 myass-0.1.1/src/myass/config_default.yaml
--rw-r--r--   0        0        0      306 1970-01-01 00:00:00.000000 myass-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-06 18:58:54.600427 myass-0.1.2/LICENSE
+-rw-r--r--   0        0        0       56 2023-07-06 22:09:52.816683 myass-0.1.2/README.md
+-rw-r--r--   0        0        0      403 2023-07-07 14:41:42.624549 myass-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-07-07 14:49:59.023117 myass-0.1.2/src/myass/__init__.py
+-rw-r--r--   0        0        0      730 2023-07-07 14:37:11.663825 myass-0.1.2/src/myass/assistant.py
+-rw-r--r--   0        0        0      387 2023-07-07 14:49:50.373200 myass-0.1.2/src/myass/cli.py
+-rw-r--r--   0        0        0      306 2023-07-07 14:37:18.963754 myass-0.1.2/src/myass/config.py
+-rw-r--r--   0        0        0       25 2023-07-07 14:32:54.096308 myass-0.1.2/src/myass/config_default.yaml
+-rw-r--r--   0        0        0      306 1970-01-01 00:00:00.000000 myass-0.1.2/PKG-INFO
```

### Comparing `myass-0.1.1/LICENSE` & `myass-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myass-0.1.1/src/myass/assistant.py` & `myass-0.1.2/src/myass/assistant.py`

 * *Files identical despite different names*

