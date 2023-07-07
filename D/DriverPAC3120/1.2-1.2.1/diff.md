# Comparing `tmp/DriverPAC3120-1.2.tar.gz` & `tmp/DriverPAC3120-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DriverPAC3120-1.2.tar", last modified: Fri Jul  7 04:42:16 2023, max compression
+gzip compressed data, was "DriverPAC3120-1.2.1.tar", last modified: Fri Jul  7 16:26:47 2023, max compression
```

## Comparing `DriverPAC3120-1.2.tar` & `DriverPAC3120-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 04:42:16.484547 DriverPAC3120-1.2/
-drwxrwxrwx   0        0        0        0 2023-07-07 04:42:16.460544 DriverPAC3120-1.2/DriverPAC3120/
--rw-rw-rw-   0        0        0       96 2023-07-07 03:57:08.000000 DriverPAC3120-1.2/DriverPAC3120/DriverPAC3120.py
--rw-rw-rw-   0        0        0        0 2023-07-07 02:53:47.000000 DriverPAC3120-1.2/DriverPAC3120/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 04:42:16.476548 DriverPAC3120-1.2/DriverPAC3120.egg-info/
--rw-rw-rw-   0        0        0       58 2023-07-07 04:42:16.000000 DriverPAC3120-1.2/DriverPAC3120.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-07-07 04:42:16.000000 DriverPAC3120-1.2/DriverPAC3120.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 04:42:16.000000 DriverPAC3120-1.2/DriverPAC3120.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 04:42:16.000000 DriverPAC3120-1.2/DriverPAC3120.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       58 2023-07-07 04:42:16.476548 DriverPAC3120-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 04:42:16.484547 DriverPAC3120-1.2/setup.cfg
--rw-rw-rw-   0        0        0      170 2023-07-07 04:41:15.000000 DriverPAC3120-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 16:26:47.251920 DriverPAC3120-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-07-07 16:26:47.239917 DriverPAC3120-1.2.1/DriverPAC3120/
+-rw-rw-rw-   0        0        0        0 2023-07-07 02:53:47.000000 DriverPAC3120-1.2.1/DriverPAC3120/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-07-07 16:09:53.000000 DriverPAC3120-1.2.1/DriverPAC3120/funciones.py
+drwxrwxrwx   0        0        0        0 2023-07-07 16:26:47.248919 DriverPAC3120-1.2.1/DriverPAC3120.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-07-07 16:26:47.000000 DriverPAC3120-1.2.1/DriverPAC3120.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-07-07 16:26:47.000000 DriverPAC3120-1.2.1/DriverPAC3120.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 16:26:47.000000 DriverPAC3120-1.2.1/DriverPAC3120.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 16:26:47.000000 DriverPAC3120-1.2.1/DriverPAC3120.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 16:26:47.000000 DriverPAC3120-1.2.1/DriverPAC3120.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      242 2023-07-07 16:26:47.250918 DriverPAC3120-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 16:26:47.251920 DriverPAC3120-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      835 2023-07-07 16:26:17.000000 DriverPAC3120-1.2.1/setup.py
```

