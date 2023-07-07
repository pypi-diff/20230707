# Comparing `tmp/testadd-0.1.0.tar.gz` & `tmp/testadd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testadd-0.1.0.tar", max compression
+gzip compressed data, was "testadd-0.3.0.tar", max compression
```

## Comparing `testadd-0.1.0.tar` & `testadd-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      274 2023-07-07 10:34:11.842575 testadd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        5 2023-07-07 10:36:21.617018 testadd-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-07 10:35:59.054944 testadd-0.1.0/testadd/__init__.py
--rw-r--r--   0        0        0       41 2023-07-07 10:29:37.026650 testadd-0.1.0/testadd/add.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 testadd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-07-07 10:39:40.387700 testadd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-07-07 10:36:21.617018 testadd-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 10:35:59.054944 testadd-0.3.0/testadd/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-07 10:29:37.026650 testadd-0.3.0/testadd/add.py
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 testadd-0.3.0/PKG-INFO
```

