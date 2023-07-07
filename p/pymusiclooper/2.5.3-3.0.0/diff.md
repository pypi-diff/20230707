# Comparing `tmp/pymusiclooper-2.5.3.tar.gz` & `tmp/pymusiclooper-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymusiclooper-2.5.3.tar", last modified: Fri Jan 13 21:05:53 2023, max compression
+gzip compressed data, was "pymusiclooper-3.0.0.tar", max compression
```

## Comparing `pymusiclooper-2.5.3.tar` & `pymusiclooper-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 21:05:53.541955 pymusiclooper-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-01-13 21:05:53.541955 pymusiclooper-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 21:05:53.541955 pymusiclooper-2.5.3/pymusiclooper/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/pymusiclooper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/pymusiclooper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/pymusiclooper/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/pymusiclooper/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/pymusiclooper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 21:05:53.541955 pymusiclooper-2.5.3/pymusiclooper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-01-13 21:05:53.000000 pymusiclooper-2.5.3/pymusiclooper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-01-13 21:05:53.000000 pymusiclooper-2.5.3/pymusiclooper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 21:05:53.000000 pymusiclooper-2.5.3/pymusiclooper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-13 21:05:53.000000 pymusiclooper-2.5.3/pymusiclooper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-13 21:05:53.000000 pymusiclooper-2.5.3/pymusiclooper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-13 21:05:53.000000 pymusiclooper-2.5.3/pymusiclooper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-13 21:05:53.541955 pymusiclooper-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 21:05:42.000000 pymusiclooper-2.5.3/setup.py
+-rw-r--r--   0        0        0     1067 2023-07-07 15:55:51.972223 pymusiclooper-3.0.0/LICENSE
+-rw-r--r--   0        0        0    10363 2023-07-07 15:55:51.972223 pymusiclooper-3.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/__main__.py
+-rw-r--r--   0        0        0    23955 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/analysis.py
+-rw-r--r--   0        0        0     3736 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/audio.py
+-rw-r--r--   0        0        0    18617 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/cli.py
+-rw-r--r--   0        0        0     1789 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/console.py
+-rw-r--r--   0        0        0     6218 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/core.py
+-rw-r--r--   0        0        0      205 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/exceptions.py
+-rw-r--r--   0        0        0    13736 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/handler.py
+-rw-r--r--   0        0        0     4637 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/playback.py
+-rw-r--r--   0        0        0     2284 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/youtube.py
+-rw-r--r--   0        0        0     1511 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11997 1970-01-01 00:00:00.000000 pymusiclooper-3.0.0/PKG-INFO
```

### Comparing `pymusiclooper-2.5.3/LICENSE` & `pymusiclooper-3.0.0/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Hazem Nabil
+Copyright (c) 2023 Hazem Nabil
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

