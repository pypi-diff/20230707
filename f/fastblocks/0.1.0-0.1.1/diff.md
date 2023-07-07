# Comparing `tmp/fastblocks-0.1.0.tar.gz` & `tmp/fastblocks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.1.0.tar", last modified: Sun Apr 16 09:00:22 2023, max compression
+gzip compressed data, was "fastblocks-0.1.1.tar", last modified: Fri Jul  7 14:18:32 2023, max compression
```

## Comparing `fastblocks-0.1.0.tar` & `fastblocks-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,11 @@
--rw-r--r--   0        0        0       41 2023-04-16 08:56:13.794232 fastblocks-0.1.0/README.md
--rw-r--r--   0        0        0      342 2023-04-16 09:00:22.269375 fastblocks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      233 1970-01-01 00:00:00.000000 fastblocks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.1.1/LICENSE
+-rw-r--r--   0        0        0      996 2023-06-18 12:37:27.109447 fastblocks-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 06:50:50.221974 fastblocks-0.1.1/fastblocks/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-12 06:50:49.105116 fastblocks-0.1.1/fastblocks/applications.py
+-rw-r--r--   0        0        0     5940 2023-07-07 13:49:10.956883 fastblocks-0.1.1/fastblocks/mail.py
+-rw-r--r--   0        0        0     2670 2023-07-07 14:07:02.536213 fastblocks-0.1.1/fastblocks/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-13 09:14:27.689475 fastblocks-0.1.1/fastblocks/sitemap.py
+-rw-r--r--   0        0        0     1598 2023-07-07 14:11:19.069432 fastblocks-0.1.1/fastblocks/templating.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:25:40.777905 fastblocks-0.1.1/fastblocks/theme/__init__.py
+-rw-r--r--   0        0        0     1276 2023-07-07 14:18:32.072899 fastblocks-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 fastblocks-0.1.1/PKG-INFO
```

