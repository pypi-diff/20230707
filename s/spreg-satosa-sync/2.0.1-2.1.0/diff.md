# Comparing `tmp/spreg-satosa-sync-2.0.1.tar.gz` & `tmp/spreg-satosa-sync-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spreg-satosa-sync-2.0.1.tar", last modified: Thu Mar  9 13:42:41 2023, max compression
+gzip compressed data, was "spreg-satosa-sync-2.1.0.tar", last modified: Fri Jul  7 11:22:13 2023, max compression
```

## Comparing `spreg-satosa-sync-2.0.1.tar` & `spreg-satosa-sync-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 13:42:41.867103 spreg-satosa-sync-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-02-07 14:39:21.000000 spreg-satosa-sync-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      290 2023-03-09 13:42:41.867103 spreg-satosa-sync-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-03-09 13:09:07.000000 spreg-satosa-sync-2.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-09 13:42:41.867103 spreg-satosa-sync-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-02-15 15:47:34.000000 spreg-satosa-sync-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 13:42:41.843103 spreg-satosa-sync-2.0.1/spreg_satosa_sync/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-07 14:39:21.000000 spreg-satosa-sync-2.0.1/spreg_satosa_sync/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9379 2023-03-09 13:09:07.000000 spreg-satosa-sync-2.0.1/spreg_satosa_sync/spreg_satosa_sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 13:42:41.867103 spreg-satosa-sync-2.0.1/spreg_satosa_sync.egg-info/
--rw-r--r--   0 root         (0) root         (0)      290 2023-03-09 13:42:41.000000 spreg-satosa-sync-2.0.1/spreg_satosa_sync.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      309 2023-03-09 13:42:41.000000 spreg-satosa-sync-2.0.1/spreg_satosa_sync.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 13:42:41.000000 spreg-satosa-sync-2.0.1/spreg_satosa_sync.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-03-09 13:42:41.000000 spreg-satosa-sync-2.0.1/spreg_satosa_sync.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-09 13:42:41.000000 spreg-satosa-sync-2.0.1/spreg_satosa_sync.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:22:13.130135 spreg-satosa-sync-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-07 11:14:21.000000 spreg-satosa-sync-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      290 2023-07-07 11:22:13.130135 spreg-satosa-sync-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-07-07 11:14:21.000000 spreg-satosa-sync-2.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-07 11:22:13.130135 spreg-satosa-sync-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-07 11:14:21.000000 spreg-satosa-sync-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:22:13.130135 spreg-satosa-sync-2.1.0/spreg_satosa_sync/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-07 11:14:21.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9379 2023-07-07 11:14:21.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync/spreg_satosa_sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:22:13.130135 spreg-satosa-sync-2.1.0/spreg_satosa_sync.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-07-07 11:22:12.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-07 11:22:13.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 11:22:12.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-07 11:22:12.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-07 11:22:12.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-07 11:22:12.000000 spreg-satosa-sync-2.1.0/spreg_satosa_sync.egg-info/top_level.txt
```

### Comparing `spreg-satosa-sync-2.0.1/LICENSE` & `spreg-satosa-sync-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spreg-satosa-sync-2.0.1/README.md` & `spreg-satosa-sync-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spreg-satosa-sync-2.0.1/spreg_satosa_sync/spreg_satosa_sync.py` & `spreg-satosa-sync-2.1.0/spreg_satosa_sync/spreg_satosa_sync.py`

 * *Files identical despite different names*

