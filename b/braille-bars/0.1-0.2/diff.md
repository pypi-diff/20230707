# Comparing `tmp/braille-bars-0.1.tar.gz` & `tmp/braille-bars-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braille-bars-0.1.tar", last modified: Fri Jul  7 01:55:27 2023, max compression
+gzip compressed data, was "braille-bars-0.2.tar", last modified: Fri Jul  7 02:01:25 2023, max compression
```

## Comparing `braille-bars-0.1.tar` & `braille-bars-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 morgan    (1000) morgan    (1000)        0 2023-07-07 01:55:27.555950 braille-bars-0.1/
--rw-rw-r--   0 morgan    (1000) morgan    (1000)     1064 2023-07-07 01:44:30.000000 braille-bars-0.1/LICENSE.txt
--rw-rw-r--   0 morgan    (1000) morgan    (1000)      213 2023-07-07 01:55:27.555950 braille-bars-0.1/PKG-INFO
--rw-rw-r--   0 morgan    (1000) morgan    (1000)     1465 2023-07-07 01:54:41.000000 braille-bars-0.1/README.rst
--rw-rw-r--   0 morgan    (1000) morgan    (1000)      108 2023-07-07 01:55:27.555950 braille-bars-0.1/setup.cfg
--rw-rw-r--   0 morgan    (1000) morgan    (1000)      413 2023-07-07 01:50:07.000000 braille-bars-0.1/setup.py
-drwxrwxr-x   0 morgan    (1000) morgan    (1000)        0 2023-07-07 01:55:27.555950 braille-bars-0.1/src/
-drwxrwxr-x   0 morgan    (1000) morgan    (1000)        0 2023-07-07 01:55:27.555950 braille-bars-0.1/src/braille_bars.egg-info/
--rw-rw-r--   0 morgan    (1000) morgan    (1000)      213 2023-07-07 01:55:27.000000 braille-bars-0.1/src/braille_bars.egg-info/PKG-INFO
--rw-rw-r--   0 morgan    (1000) morgan    (1000)      201 2023-07-07 01:55:27.000000 braille-bars-0.1/src/braille_bars.egg-info/SOURCES.txt
--rw-rw-r--   0 morgan    (1000) morgan    (1000)        1 2023-07-07 01:55:27.000000 braille-bars-0.1/src/braille_bars.egg-info/dependency_links.txt
--rw-rw-r--   0 morgan    (1000) morgan    (1000)        1 2023-07-07 01:55:27.000000 braille-bars-0.1/src/braille_bars.egg-info/top_level.txt
+drwxrwxr-x   0 morgan    (1000) morgan    (1000)        0 2023-07-07 02:01:25.937621 braille-bars-0.2/
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)     1064 2023-07-07 01:44:30.000000 braille-bars-0.2/LICENSE.txt
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)     1720 2023-07-07 02:01:25.937621 braille-bars-0.2/PKG-INFO
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)     1465 2023-07-07 01:54:41.000000 braille-bars-0.2/README.md
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)      108 2023-07-07 02:01:25.937621 braille-bars-0.2/setup.cfg
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)      598 2023-07-07 02:00:02.000000 braille-bars-0.2/setup.py
+drwxrwxr-x   0 morgan    (1000) morgan    (1000)        0 2023-07-07 02:01:25.937621 braille-bars-0.2/src/
+drwxrwxr-x   0 morgan    (1000) morgan    (1000)        0 2023-07-07 02:01:25.937621 braille-bars-0.2/src/braille_bars.egg-info/
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)     1720 2023-07-07 02:01:25.000000 braille-bars-0.2/src/braille_bars.egg-info/PKG-INFO
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)      200 2023-07-07 02:01:25.000000 braille-bars-0.2/src/braille_bars.egg-info/SOURCES.txt
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)        1 2023-07-07 02:01:25.000000 braille-bars-0.2/src/braille_bars.egg-info/dependency_links.txt
+-rw-rw-r--   0 morgan    (1000) morgan    (1000)        1 2023-07-07 02:01:25.000000 braille-bars-0.2/src/braille_bars.egg-info/top_level.txt
```

### Comparing `braille-bars-0.1/LICENSE.txt` & `braille-bars-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `braille-bars-0.1/README.rst` & `braille-bars-0.2/README.md`

 * *Files identical despite different names*

