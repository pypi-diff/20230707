# Comparing `tmp/emailalert-1.4.3.tar.gz` & `tmp/emailalert-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.4.3.tar", last modified: Fri Jul  7 01:30:31 2023, max compression
+gzip compressed data, was "emailalert-1.4.4.tar", last modified: Fri Jul  7 02:21:18 2023, max compression
```

## Comparing `emailalert-1.4.3.tar` & `emailalert-1.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 01:30:31.650388 emailalert-1.4.3/
--rw-rw-rw-   0        0        0      178 2023-07-07 01:30:31.646904 emailalert-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 01:30:31.611881 emailalert-1.4.3/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 01:30:31.633114 emailalert-1.4.3/sck/
--rw-rw-rw-   0        0        0        0 2023-07-07 01:24:44.000000 emailalert-1.4.3/sck/__init__.py
--rw-rw-rw-   0        0        0      858 2023-07-07 01:29:36.000000 emailalert-1.4.3/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-07-07 01:30:31.651910 emailalert-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-07-07 01:30:27.000000 emailalert-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:21:18.322411 emailalert-1.4.4/
+-rw-rw-rw-   0        0        0      178 2023-07-07 02:21:18.319631 emailalert-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-07-07 02:16:16.000000 emailalert-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 02:21:18.279300 emailalert-1.4.4/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-07 02:21:17.000000 emailalert-1.4.4/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-07 02:21:18.000000 emailalert-1.4.4/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:21:17.000000 emailalert-1.4.4/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-07 02:21:18.000000 emailalert-1.4.4/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 02:21:18.314826 emailalert-1.4.4/sck/
+-rw-rw-rw-   0        0        0        0 2023-07-07 01:24:44.000000 emailalert-1.4.4/sck/__init__.py
+-rw-rw-rw-   0        0        0     4398 2023-07-07 02:20:23.000000 emailalert-1.4.4/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:21:18.324413 emailalert-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-07-07 02:20:20.000000 emailalert-1.4.4/setup.py
```

### Comparing `emailalert-1.4.3/README.md` & `emailalert-1.4.4/README.md`

 * *Files identical despite different names*

