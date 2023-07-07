# Comparing `tmp/rateToolsAC4RM-0.0.tar.gz` & `tmp/rateToolsAC4RM-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rateToolsAC4RM-0.0.tar", last modified: Tue Jun 20 15:04:14 2023, max compression
+gzip compressed data, was "rateToolsAC4RM-0.1.tar", last modified: Fri Jul  7 20:16:02 2023, max compression
```

## Comparing `rateToolsAC4RM-0.0.tar` & `rateToolsAC4RM-0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-06-20 15:04:14.000000 rateToolsAC4RM-0.0/
--rw-r--r--   0 tleitch1   (501) staff       (20)      216 2023-06-20 15:04:14.000000 rateToolsAC4RM-0.0/PKG-INFO
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-06-20 15:04:14.000000 rateToolsAC4RM-0.0/rateToolsAC4RM/
--rw-rw-r--   0 tleitch1   (501) staff       (20)      206 2023-06-20 15:04:02.000000 rateToolsAC4RM-0.0/rateToolsAC4RM/__init__.py
--rw-r--r--   0 tleitch1   (501) staff       (20)     3921 2023-06-20 14:59:54.000000 rateToolsAC4RM-0.0/rateToolsAC4RM/rateTools.py
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-06-20 15:04:14.000000 rateToolsAC4RM-0.0/rateToolsAC4RM.egg-info/
--rw-r--r--   0 tleitch1   (501) staff       (20)      216 2023-06-20 15:04:13.000000 rateToolsAC4RM-0.0/rateToolsAC4RM.egg-info/PKG-INFO
--rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-06-20 15:04:13.000000 rateToolsAC4RM-0.0/rateToolsAC4RM.egg-info/SOURCES.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 15:04:13.000000 rateToolsAC4RM-0.0/rateToolsAC4RM.egg-info/dependency_links.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.0/rateToolsAC4RM.egg-info/not-zip-safe
--rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-06-20 15:04:13.000000 rateToolsAC4RM-0.0/rateToolsAC4RM.egg-info/top_level.txt
--rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-06-20 15:04:14.000000 rateToolsAC4RM-0.0/setup.cfg
--rw-rw-r--   0 tleitch1   (501) staff       (20)      226 2023-06-20 03:42:15.000000 rateToolsAC4RM-0.0/setup.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:16:02.721797 rateToolsAC4RM-0.1/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      189 2023-07-07 20:16:02.721925 rateToolsAC4RM-0.1/PKG-INFO
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:16:02.718447 rateToolsAC4RM-0.1/rateToolsAC4RM/
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      272 2023-07-07 20:05:55.000000 rateToolsAC4RM-0.1/rateToolsAC4RM/__init__.py
+-rw-r--r--   0 tleitch1   (501) staff       (20)     4679 2023-07-07 19:56:59.000000 rateToolsAC4RM-0.1/rateToolsAC4RM/rateTools.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:16:02.721483 rateToolsAC4RM-0.1/rateToolsAC4RM.egg-info/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      189 2023-07-07 20:16:02.000000 rateToolsAC4RM-0.1/rateToolsAC4RM.egg-info/PKG-INFO
+-rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-07-07 20:16:02.000000 rateToolsAC4RM-0.1/rateToolsAC4RM.egg-info/SOURCES.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-07-07 20:16:02.000000 rateToolsAC4RM-0.1/rateToolsAC4RM.egg-info/dependency_links.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.1/rateToolsAC4RM.egg-info/not-zip-safe
+-rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-07-07 20:16:02.000000 rateToolsAC4RM-0.1/rateToolsAC4RM.egg-info/top_level.txt
+-rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-07-07 20:16:02.722583 rateToolsAC4RM-0.1/setup.cfg
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      226 2023-07-07 20:15:33.000000 rateToolsAC4RM-0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

