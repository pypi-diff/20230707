# Comparing `tmp/diffusechain-0.1.1.tar.gz` & `tmp/diffusechain-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusechain-0.1.1.tar", max compression
+gzip compressed data, was "diffusechain-0.1.1.1.tar", max compression
```

## Comparing `diffusechain-0.1.1.tar` & `diffusechain-0.1.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-06 19:05:26.814100 diffusechain-0.1.1/diffusechain/__init__.py
--rw-r--r--   0        0        0       20 2023-07-07 21:16:26.668185 diffusechain-0.1.1/diffusechain/diffusechain.py
--rw-r--r--   0        0        0      312 2023-07-07 21:30:07.845259 diffusechain-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       15 2023-07-06 19:14:58.750868 diffusechain-0.1.1/README.md
--rw-r--r--   0        0        0      352 1970-01-01 00:00:00.000000 diffusechain-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-06 19:05:26.814100 diffusechain-0.1.1.1/diffusechain/__init__.py
+-rw-r--r--   0        0        0       20 2023-07-07 21:16:26.668185 diffusechain-0.1.1.1/diffusechain/diffusechain.py
+-rw-r--r--   0        0        0      313 2023-07-07 21:33:41.278550 diffusechain-0.1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-07-06 19:14:58.750868 diffusechain-0.1.1.1/README.md
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 diffusechain-0.1.1.1/PKG-INFO
```

