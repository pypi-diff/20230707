# Comparing `tmp/pyams_zfiles-1.4.5.tar.gz` & `tmp/pyams_zfiles-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_zfiles-1.4.5.tar", last modified: Tue May 16 15:02:25 2023, max compression
+gzip compressed data, was "dist/pyams_zfiles-1.4.6.tar", last modified: Fri Jul  7 15:41:47 2023, max compression
```

## Comparing `pyams_zfiles-1.4.5.tar` & `pyams_zfiles-1.4.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3802 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1831 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    93884 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/docs/graphql-api.json
--rw-rw-rw-   0 root         (0) root         (0)    64214 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/docs/rest-api.json
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2940 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/api/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12553 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/api/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    28203 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/api/rest.py
--rw-rw-rw-   0 root         (0) root         (0)    11249 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/api/rpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    11997 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    14592 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/document.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/folder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/generations/
--rw-rw-rw-   0 root         (0) root         (0)     4315 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2577 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     2317 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/generations/evolve2.py
--rw-rw-rw-   0 root         (0) root         (0)     7218 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/include.py
--rw-rw-rw-   0 root         (0) root         (0)    15780 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15088 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo
--rw-rw-rw-   0 root         (0) root         (0)    24071 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po
--rw-rw-rw-   0 root         (0) root         (0)    17093 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/locales/pyams_zfiles.pot
--rw-rw-rw-   0 root         (0) root         (0)     8043 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/skin/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/skin/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/skin/file.py
--rw-rw-rw-   0 root         (0) root         (0)     6776 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/synchronizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/tests/
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)    12735 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/utility.py
--rw-rw-rw-   0 root         (0) root         (0)    10714 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4877 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4807 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    11289 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/synchronizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/templates/properties-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     4460 2023-05-16 15:02:03.000000 pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3802 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1585 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      463 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 15:02:25.000000 pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1887 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    93884 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/docs/graphql-api.json
+-rw-rw-rw-   0 root         (0) root         (0)    64214 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/docs/rest-api.json
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2940 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/api/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12553 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/api/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    28382 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/api/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    11249 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/api/rpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    11997 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14592 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/folder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/generations/evolve2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7218 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    15780 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15088 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo
+-rw-rw-rw-   0 root         (0) root         (0)    24071 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po
+-rw-rw-rw-   0 root         (0) root         (0)    17093 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/locales/pyams_zfiles.pot
+-rw-rw-rw-   0 root         (0) root         (0)     8101 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/skin/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/skin/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/synchronizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12735 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)    10714 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4807 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    11289 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/synchronizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/templates/properties-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4460 2023-07-07 15:41:28.000000 pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 15:41:47.000000 pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/top_level.txt
```

### Comparing `pyams_zfiles-1.4.5/LICENSE` & `pyams_zfiles-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/PKG-INFO` & `pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_zfiles
-Version: 1.4.5
+Name: pyams-zfiles
+Version: 1.4.6
 Summary: PyAMS files storage manager
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -52,14 +52,18 @@
 ZFiles is just a storage manager for these documents; the lifecycle management is delegated to
 the applications which use it as storage backend.
 
 
 Changelog
 =========
 
+1.4.6
+-----
+ - updated REST document search API schema
+
 1.4.5
 -----
  - updated access and update modes management
 
 1.4.4
 -----
  - updated Colander API schemas for better OpenAPI specifications
```

### Comparing `pyams_zfiles-1.4.5/docs/HISTORY.rst` & `pyams_zfiles-1.4.6/docs/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.4.6
+-----
+ - updated REST document search API schema
+
 1.4.5
 -----
  - updated access and update modes management
 
 1.4.4
 -----
  - updated Colander API schemas for better OpenAPI specifications
```

### Comparing `pyams_zfiles-1.4.5/docs/README.rst` & `pyams_zfiles-1.4.6/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/docs/graphql-api.json` & `pyams_zfiles-1.4.6/docs/graphql-api.json`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/docs/rest-api.json` & `pyams_zfiles-1.4.6/docs/rest-api.json`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/setup.py` & `pyams_zfiles-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.4.5'
+version = '1.4.6'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_form',
     'pyams_pagelet',
     'pyams_skin',
     'pyams_table',
```

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/__init__.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/api/__init__.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/api/graph.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/api/graph.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/api/rest.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pyramid.httpexceptions import HTTPBadRequest, HTTPCreated, HTTPError, HTTPForbidden, HTTPNotFound, HTTPOk, \
     HTTPServiceUnavailable
 
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_utils.dict import merge_dict
 from pyams_utils.registry import get_utility, query_utility
 from pyams_utils.rest import BaseResponseSchema, DateRangeSchema, FileUploadType, PropertiesMapping, STATUS, \
-    StringListSchema, http_error, rest_responses
+    StringArraySchema, StringListSchema, http_error, rest_responses
 from pyams_zfiles.interfaces import ACCESS_MODE, CREATE_DOCUMENT_PERMISSION, CREATE_DOCUMENT_WITH_OWNER_PERMISSION, \
     DEFAULT_CONFIGURATION_NAME, IDocumentContainer, IDocumentSynchronizer, READ_DOCUMENT_PERMISSION, \
     REST_CONTAINER_ROUTE, REST_DOCUMENT_ROUTE, REST_SYNCHRONIZER_ROUTE, STATE, SYNCHRONIZE_PERMISSION
 
 
 __docformat__ = 'restructuredtext'
 
@@ -303,14 +303,17 @@
                               description="Document last update dates range in ISO-8601 format, separated by "
                                           "commas; unset values should be replaced by *null*",
                               missing=drop)
     status_update_date = SchemaNode(String(),
                                     description="Last workflow status update dates range in ISO-8601 format, separated "
                                                 "by commas; unset values should be replaced by *null*",
                                     missing=drop)
+    tags = SchemaNode(StringArraySchema(),
+                      description="List of documents tags, separated by commas",
+                      missing=drop)
     fields = SchemaNode(String(),
                         description="List of requested field names, separated by commas",
                         missing=drop)
 
 
 class DocumentsSynchronizeInfo(MappingSchema):
     """Documents synchronize schema"""
```

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/api/rpc.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/api/rpc.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/doctests/README.rst` & `pyams_zfiles-1.4.6/src/pyams_zfiles/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/document.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/document.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/folder.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/generations/__init__.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/generations/evolve1.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/generations/evolve2.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/generations/evolve2.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             modes = list(ACCESS_MODE)
             for index, document in enumerate(find_objects_providing(container, IDocument)):
                 print('.', end='')
                 for version in IWorkflowVersions(document).get_versions():
                     access_mode = version.access_mode
                     if isinstance(access_mode, int):
                         access_mode = modes[access_mode].value
-                    if  isinstance(access_mode, Enum):
+                    if isinstance(access_mode, Enum):
                         access_mode = access_mode.value
                     version.access_mode = access_mode
                     update_mode = version.update_mode
                     if isinstance(update_mode, int):
                         update_mode = modes[update_mode].value
                     if isinstance(update_mode, Enum):
                         update_mode = update_mode.value
```

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/include.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/include.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/interfaces.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/layer.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/layer.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo` & `pyams_zfiles-1.4.6/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po` & `pyams_zfiles-1.4.6/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/locales/pyams_zfiles.pot` & `pyams_zfiles-1.4.6/src/pyams_zfiles/locales/pyams_zfiles.pot`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/search.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from urllib.parse import parse_qsl
 
 from dateutil import parser
 from hypatia.query import All, Any, Comparator, Eq, Ge, Le
 
 from pyams_catalog.query import and_, or_
 from pyams_utils.date import date_to_datetime
+from pyams_utils.interfaces.form import NO_VALUE_STRING
 from pyams_utils.timezone import gmtime
 
 
 __docformat__ = 'restructuredtext'
 
 
 NULL_STRING = 'null'
@@ -219,15 +220,15 @@
 }
 
 
 def make_query(catalog, params):
     """Make query from input parameters"""
     query = None
     for key, value in params.copy().items():
-        if (value is None) or (value == {'--NOVALUE--'}):
+        if (value is None) or (value == {NO_VALUE_STRING}):
             params.pop(key)
         elif key not in INDEX_ARGS:
             params.setdefault('properties', {}).setdefault(key, params.pop(key))
     for key, value in params.items():
         args = INDEX_ARGS.get(key)
         if args is None:
             continue
```

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/skin/__init__.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/skin/container.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/skin/container.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/skin/file.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/skin/file.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/synchronizer.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/tests/__init__.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/tests/test_utilsdocs.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/tests/test_utilsdocstrings.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/utility.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/workflow.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/__init__.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/document.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/document.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/properties.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/properties.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/search.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/synchronizer.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles/zmi/workflow.py` & `pyams_zfiles-1.4.6/src/pyams_zfiles/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/PKG-INFO` & `pyams_zfiles-1.4.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-zfiles
-Version: 1.4.5
+Name: pyams_zfiles
+Version: 1.4.6
 Summary: PyAMS files storage manager
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -52,14 +52,18 @@
 ZFiles is just a storage manager for these documents; the lifecycle management is delegated to
 the applications which use it as storage backend.
 
 
 Changelog
 =========
 
+1.4.6
+-----
+ - updated REST document search API schema
+
 1.4.5
 -----
  - updated access and update modes management
 
 1.4.4
 -----
  - updated Colander API schemas for better OpenAPI specifications
```

### Comparing `pyams_zfiles-1.4.5/src/pyams_zfiles.egg-info/SOURCES.txt` & `pyams_zfiles-1.4.6/src/pyams_zfiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

