# Comparing `tmp/emailalert-1.4.2.tar.gz` & `tmp/emailalert-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.4.2.tar", last modified: Tue Jul  4 05:18:52 2023, max compression
+gzip compressed data, was "emailalert-1.4.3.tar", last modified: Fri Jul  7 01:30:31 2023, max compression
```

## Comparing `emailalert-1.4.2.tar` & `emailalert-1.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 05:18:52.720605 emailalert-1.4.2/
--rw-rw-rw-   0        0        0      178 2023-07-04 05:18:52.717355 emailalert-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 05:18:52.621991 emailalert-1.4.2/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 05:18:52.697830 emailalert-1.4.2/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.4.2/sck/__init__.py
--rw-rw-rw-   0        0        0     2406 2023-07-04 05:14:01.000000 emailalert-1.4.2/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-07-04 05:18:52.721621 emailalert-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-07-04 05:18:44.000000 emailalert-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:30:31.650388 emailalert-1.4.3/
+-rw-rw-rw-   0        0        0      178 2023-07-07 01:30:31.646904 emailalert-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 01:30:31.611881 emailalert-1.4.3/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-07 01:30:31.000000 emailalert-1.4.3/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 01:30:31.633114 emailalert-1.4.3/sck/
+-rw-rw-rw-   0        0        0        0 2023-07-07 01:24:44.000000 emailalert-1.4.3/sck/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-07 01:29:36.000000 emailalert-1.4.3/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 01:30:31.651910 emailalert-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-07-07 01:30:27.000000 emailalert-1.4.3/setup.py
```

### Comparing `emailalert-1.4.2/README.md` & `emailalert-1.4.3/README.md`

 * *Files identical despite different names*

