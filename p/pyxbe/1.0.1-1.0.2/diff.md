# Comparing `tmp/pyxbe-1.0.1.tar.gz` & `tmp/pyxbe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxbe-1.0.1.tar", last modified: Thu Aug 25 17:23:52 2022, max compression
+gzip compressed data, was "pyxbe-1.0.2.tar", last modified: Fri Jul  7 08:05:34 2023, max compression
```

## Comparing `pyxbe-1.0.1.tar` & `pyxbe-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:52.768241 pyxbe-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-08-25 17:23:42.000000 pyxbe-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-25 17:23:42.000000 pyxbe-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-08-25 17:23:52.768241 pyxbe-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5755 2022-08-25 17:23:42.000000 pyxbe-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-25 17:23:42.000000 pyxbe-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:52.768241 pyxbe-1.0.1/pyxbe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-08-25 17:23:52.000000 pyxbe-1.0.1/pyxbe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-08-25 17:23:52.000000 pyxbe-1.0.1/pyxbe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 17:23:52.000000 pyxbe-1.0.1/pyxbe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-25 17:23:52.000000 pyxbe-1.0.1/pyxbe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-25 17:23:52.768241 pyxbe-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-08-25 17:23:42.000000 pyxbe-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:52.768241 pyxbe-1.0.1/xbe/
--rw-r--r--   0 runner    (1001) docker     (121)    41354 2022-08-25 17:23:42.000000 pyxbe-1.0.1/xbe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-08-25 17:23:42.000000 pyxbe-1.0.1/xbe/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-07 08:04:24.000000 pyxbe-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 08:04:24.000000 pyxbe-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 08:05:34.868189 pyxbe-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-07 08:04:24.000000 pyxbe-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 08:04:24.000000 pyxbe-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/pyxbe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-07 08:05:34.868189 pyxbe-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 08:04:24.000000 pyxbe-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:24.000000 pyxbe-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 08:04:24.000000 pyxbe-1.0.2/tests/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/xbe/
+-rw-r--r--   0 runner    (1001) docker     (123)    50913 2023-07-07 08:04:24.000000 pyxbe-1.0.2/xbe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-07 08:04:24.000000 pyxbe-1.0.2/xbe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:24.000000 pyxbe-1.0.2/xbe/py.typed
```

### Comparing `pyxbe-1.0.1/LICENSE.txt` & `pyxbe-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

