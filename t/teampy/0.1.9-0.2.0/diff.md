# Comparing `tmp/teampy-0.1.9.tar.gz` & `tmp/teampy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/teampy-0.1.9.tar", last modified: Wed Aug 15 08:31:00 2018, max compression
+gzip compressed data, was "teampy-0.2.0.tar", last modified: Fri Jul  7 05:18:06 2023, max compression
```

## Comparing `teampy-0.1.9.tar` & `teampy-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2018-08-15 08:31:00.000000 teampy-0.1.9/
--rw-r--r--   0 kraemer    (501) staff       (20)      626 2018-08-15 08:31:00.000000 teampy-0.1.9/PKG-INFO
--rw-r--r--   0 kraemer    (501) staff       (20)      950 2018-08-15 08:30:52.000000 teampy-0.1.9/setup.py
--rw-r--r--   0 kraemer    (501) staff       (20)       40 2017-11-26 20:50:12.000000 teampy-0.1.9/setup.cfg
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2018-08-15 08:31:00.000000 teampy-0.1.9/teampy/
--rw-r--r--   0 kraemer    (501) staff       (20)     1696 2018-07-16 18:14:24.000000 teampy-0.1.9/teampy/command_line_setup.py
--rw-r--r--   0 kraemer    (501) staff       (20)    13494 2017-01-18 13:31:30.000000 teampy-0.1.9/teampy/scratch.pdf
--rw-r--r--   0 kraemer    (501) staff       (20)     1615 2018-08-15 08:29:24.000000 teampy-0.1.9/teampy/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)    16641 2018-08-13 19:47:24.000000 teampy-0.1.9/teampy/core.py
--rw-r--r--   0 kraemer    (501) staff       (20)     3839 2018-07-06 06:11:14.000000 teampy-0.1.9/teampy/latex_preamble.tex
--rw-r--r--   0 kraemer    (501) staff       (20)     6779 2018-08-15 08:28:07.000000 teampy-0.1.9/teampy/command_line_rat.py
--rw-r--r--   0 kraemer    (501) staff       (20)    25702 2017-01-24 18:37:10.000000 teampy-0.1.9/teampy/rat-box.pdf
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2023-07-07 05:18:06.307371 teampy-0.2.0/
+-rw-r--r--   0 kraemer    (501) staff       (20)    35147 2023-07-06 15:03:33.000000 teampy-0.2.0/LICENSE
+-rw-r--r--   0 kraemer    (501) staff       (20)      810 2023-07-07 05:18:06.307428 teampy-0.2.0/PKG-INFO
+-rw-r--r--   0 kraemer    (501) staff       (20)      103 2023-07-06 15:03:33.000000 teampy-0.2.0/README.md
+-rw-r--r--   0 kraemer    (501) staff       (20)       79 2023-07-07 05:18:06.307616 teampy-0.2.0/setup.cfg
+-rw-r--r--   0 kraemer    (501) staff       (20)     1917 2023-07-06 15:03:33.000000 teampy-0.2.0/setup.py
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2023-07-07 05:18:06.306713 teampy-0.2.0/teampy/
+-rw-r--r--   0 kraemer    (501) staff       (20)      505 2023-07-07 05:15:03.000000 teampy-0.2.0/teampy/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)    21868 2023-07-07 04:55:28.000000 teampy-0.2.0/teampy/command_line_rat.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     2914 2023-07-06 15:03:33.000000 teampy-0.2.0/teampy/command_line_setup.py
+-rw-r--r--   0 kraemer    (501) staff       (20)    60764 2023-07-07 05:12:42.000000 teampy-0.2.0/teampy/core.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     5034 2023-07-07 04:55:03.000000 teampy-0.2.0/teampy/latex_preamble.tex
+-rw-r--r--   0 kraemer    (501) staff       (20)     3890 2023-07-06 15:03:33.000000 teampy-0.2.0/teampy/latex_preamble_old.tex
+-rw-r--r--   0 kraemer    (501) staff       (20)    25702 2023-07-06 15:03:33.000000 teampy-0.2.0/teampy/rat-box.pdf
+-rw-r--r--   0 kraemer    (501) staff       (20)    13494 2023-07-06 15:03:33.000000 teampy-0.2.0/teampy/scratch.pdf
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2023-07-07 05:18:06.307282 teampy-0.2.0/teampy.egg-info/
+-rw-r--r--   0 kraemer    (501) staff       (20)      810 2023-07-07 05:18:06.000000 teampy-0.2.0/teampy.egg-info/PKG-INFO
+-rw-r--r--   0 kraemer    (501) staff       (20)      402 2023-07-07 05:18:06.000000 teampy-0.2.0/teampy.egg-info/SOURCES.txt
+-rw-r--r--   0 kraemer    (501) staff       (20)        1 2023-07-07 05:18:06.000000 teampy-0.2.0/teampy.egg-info/dependency_links.txt
+-rw-r--r--   0 kraemer    (501) staff       (20)       94 2023-07-07 05:18:06.000000 teampy-0.2.0/teampy.egg-info/entry_points.txt
+-rw-r--r--   0 kraemer    (501) staff       (20)       97 2023-07-07 05:18:06.000000 teampy-0.2.0/teampy.egg-info/requires.txt
+-rw-r--r--   0 kraemer    (501) staff       (20)        7 2023-07-07 05:18:06.000000 teampy-0.2.0/teampy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `teampy-0.1.9/PKG-INFO` & `teampy-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: teampy
-Version: 0.1.9
+Version: 0.2.0
 Summary: Tools for Team-Based Learning
 Home-page: https://github.com/falkr/teampy
+Download-URL: https://github.com/falkr/teampy/archive/0.2.tar.gz
 Author: Frank Alexander Kraemer
 Author-email: kraemer.frank@gmail.com
 License: GPLv3
-Download-URL: https://github.com/falkr/teampy/archive/0.2.tar.gz
-Description: UNKNOWN
 Keywords: education
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
```

### Comparing `teampy-0.1.9/teampy/scratch.pdf` & `teampy-0.2.0/teampy/scratch.pdf`

 * *Files identical despite different names*

### Comparing `teampy-0.1.9/teampy/rat-box.pdf` & `teampy-0.2.0/teampy/rat-box.pdf`

 * *Files identical despite different names*

