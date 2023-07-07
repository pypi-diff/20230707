# Comparing `tmp/numpydoc-1.6.0rc0.tar.gz` & `tmp/numpydoc-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpydoc-1.6.0rc0.tar", last modified: Thu Jun 29 21:35:01 2023, max compression
+gzip compressed data, was "numpydoc-1.6.0rc1.tar", last modified: Fri Jul  7 17:42:03 2023, max compression
```

## Comparing `numpydoc-1.6.0rc0.tar` & `numpydoc-1.6.0rc1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.460235 numpydoc-1.6.0rc0/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1298 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/LICENSE.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      306 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/MANIFEST.in
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2003 2023-06-29 21:35:01.460235 numpydoc-1.6.0rc0/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1215 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/README.rst
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1500 2023-06-29 21:33:27.000000 numpydoc-1.6.0rc0/RELEASE.rst
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.449235 numpydoc-1.6.0rc0/doc/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     7213 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/Makefile
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4585 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/conf.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4109 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/example.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      251 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/example.rst
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    24124 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/format.rst
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      790 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/index.rst
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6197 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/doc/install.rst
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6721 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/make.bat
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    21266 2023-06-29 21:26:11.000000 numpydoc-1.6.0rc0/doc/release_notes.rst
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     5173 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/doc/validation.rst
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.452235 numpydoc-1.6.0rc0/numpydoc/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      280 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/__init__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1550 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/__main__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       25 2023-06-29 21:26:38.000000 numpydoc-1.6.0rc0/numpydoc/_version.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    23449 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/numpydoc/docscrape.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    15214 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/docscrape_sphinx.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.454235 numpydoc-1.6.0rc0/numpydoc/hooks/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       39 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/hooks/__init__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1393 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/hooks/utils.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    13601 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/hooks/validate_docstrings.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    17055 2023-06-08 22:44:13.000000 numpydoc-1.6.0rc0/numpydoc/numpydoc.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.455235 numpydoc-1.6.0rc0/numpydoc/templates/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      227 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/templates/numpydoc_docstring.rst
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.457235 numpydoc-1.6.0rc0/numpydoc/tests/
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.458235 numpydoc-1.6.0rc0/numpydoc/tests/hooks/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       23 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/__init__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      497 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/example_module.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1027 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/test_utils.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    14473 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/test_validate_hook.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    36826 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_docscrape.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3761 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_full.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2828 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_main.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     7652 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_numpydoc.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    37154 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_validate.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6285 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_xref.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.459235 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      249 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/Makefile
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      670 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/conf.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      146 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/index.rst
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      925 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/numpydoc_test_module.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    21812 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/validate.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6541 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/xref.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.453235 numpydoc-1.6.0rc0/numpydoc.egg-info/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2003 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1270 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/SOURCES.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/dependency_links.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       80 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/entry_points.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      121 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/requires.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/top_level.txt
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.460235 numpydoc-1.6.0rc0/requirements/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       16 2023-06-27 17:09:18.000000 numpydoc-1.6.0rc0/requirements/developer.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       64 2023-06-27 17:49:05.000000 numpydoc-1.6.0rc0/requirements/doc.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       29 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/requirements/test.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      302 2023-06-29 21:35:01.461235 numpydoc-1.6.0rc0/setup.cfg
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2285 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/setup.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.244806 numpydoc-1.6.0rc1/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1298 2023-07-07 17:34:31.000000 numpydoc-1.6.0rc1/LICENSE.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      306 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3550 2023-07-07 17:42:03.244806 numpydoc-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1215 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc1/README.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1507 2023-07-02 15:27:01.000000 numpydoc-1.6.0rc1/RELEASE.rst
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.228806 numpydoc-1.6.0rc1/doc/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     7213 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/doc/Makefile
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4585 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/doc/conf.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4109 2023-07-02 06:48:54.000000 numpydoc-1.6.0rc1/doc/example.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      251 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/doc/example.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    24124 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/doc/format.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      790 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/doc/index.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6197 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc1/doc/install.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6721 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/doc/make.bat
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    21265 2023-07-07 17:36:32.000000 numpydoc-1.6.0rc1/doc/release_notes.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     5173 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/doc/validation.rst
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.231806 numpydoc-1.6.0rc1/numpydoc/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      280 2023-07-02 06:48:54.000000 numpydoc-1.6.0rc1/numpydoc/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1550 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/__main__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       25 2023-07-07 17:37:06.000000 numpydoc-1.6.0rc1/numpydoc/_version.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    23449 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc1/numpydoc/docscrape.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    15214 2023-07-02 06:48:54.000000 numpydoc-1.6.0rc1/numpydoc/docscrape_sphinx.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.234806 numpydoc-1.6.0rc1/numpydoc/hooks/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       39 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/hooks/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1393 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/hooks/utils.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    13601 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/hooks/validate_docstrings.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    17055 2023-07-02 06:48:54.000000 numpydoc-1.6.0rc1/numpydoc/numpydoc.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.234806 numpydoc-1.6.0rc1/numpydoc/templates/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      227 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/templates/numpydoc_docstring.rst
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.237806 numpydoc-1.6.0rc1/numpydoc/tests/
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.239806 numpydoc-1.6.0rc1/numpydoc/tests/hooks/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       23 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/tests/hooks/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      497 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/tests/hooks/example_module.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1027 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/tests/hooks/test_utils.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    14473 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/tests/hooks/test_validate_hook.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    36826 2023-07-02 06:48:54.000000 numpydoc-1.6.0rc1/numpydoc/tests/test_docscrape.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3761 2023-07-02 06:48:54.000000 numpydoc-1.6.0rc1/numpydoc/tests/test_full.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2828 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/tests/test_main.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     7652 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/tests/test_numpydoc.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    37154 2023-07-02 06:48:54.000000 numpydoc-1.6.0rc1/numpydoc/tests/test_validate.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6285 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/tests/test_xref.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.242806 numpydoc-1.6.0rc1/numpydoc/tests/tinybuild/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      249 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/tests/tinybuild/Makefile
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      670 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/tests/tinybuild/conf.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      146 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/tests/tinybuild/index.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      925 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/tests/tinybuild/numpydoc_test_module.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    21812 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc1/numpydoc/validate.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6541 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/numpydoc/xref.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.233806 numpydoc-1.6.0rc1/numpydoc.egg-info/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3550 2023-07-07 17:42:03.000000 numpydoc-1.6.0rc1/numpydoc.egg-info/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1266 2023-07-07 17:42:03.000000 numpydoc-1.6.0rc1/numpydoc.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-07-07 17:42:03.000000 numpydoc-1.6.0rc1/numpydoc.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       80 2023-07-07 17:42:03.000000 numpydoc-1.6.0rc1/numpydoc.egg-info/entry_points.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      189 2023-07-07 17:42:03.000000 numpydoc-1.6.0rc1/numpydoc.egg-info/requires.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-07-07 17:42:03.000000 numpydoc-1.6.0rc1/numpydoc.egg-info/top_level.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-07-07 17:34:31.000000 numpydoc-1.6.0rc1/pyproject.toml
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-07 17:42:03.243806 numpydoc-1.6.0rc1/requirements/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       22 2023-07-02 17:53:13.000000 numpydoc-1.6.0rc1/requirements/developer.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       64 2023-07-02 15:38:56.000000 numpydoc-1.6.0rc1/requirements/doc.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       29 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc1/requirements/test.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-07-07 17:42:03.244806 numpydoc-1.6.0rc1/setup.cfg
```

### Comparing `numpydoc-1.6.0rc0/LICENSE.txt` & `numpydoc-1.6.0rc1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2008-2022 Stefan van der Walt <stefan@mentat.za.net>, Pauli Virtanen <pav@iki.fi>
+Copyright (C) 2008-2023 Stefan van der Walt <stefan@mentat.za.net>, Pauli Virtanen <pav@iki.fi>
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
  1. Redistributions of source code must retain the above copyright
     notice, this list of conditions and the following disclaimer.
```

### Comparing `numpydoc-1.6.0rc0/README.rst` & `numpydoc-1.6.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/RELEASE.rst` & `numpydoc-1.6.0rc1/RELEASE.rst`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 - Review the github release page::
 
     https://github.com/numpy/numpydoc/releases
 
 - Publish on PyPi::
 
     git clean -fxd
-    pip install -U build wheel twine
+    pip install --upgrade build wheel twine
     python -m build --sdist --wheel
     twine upload -s dist/*
 
 - Update ``__version__`` in ``numpydoc/_version.py``.
 
 - Commit changes::
```

### Comparing `numpydoc-1.6.0rc0/doc/Makefile` & `numpydoc-1.6.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/doc/conf.py` & `numpydoc-1.6.0rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/doc/example.py` & `numpydoc-1.6.0rc1/doc/example.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/doc/format.rst` & `numpydoc-1.6.0rc1/doc/format.rst`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/doc/index.rst` & `numpydoc-1.6.0rc1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/doc/install.rst` & `numpydoc-1.6.0rc1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/doc/make.bat` & `numpydoc-1.6.0rc1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/doc/release_notes.rst` & `numpydoc-1.6.0rc1/doc/release_notes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
    :depth: 2
 
 .. note::
 
    For release notes (sparsely) kept prior to 1.0.0, look at the `releases page
    on GitHub <https://github.com/numpy/numpydoc/releases>`__.
 
-1.6.0rc0
+1.6.0rc1
 --------
 
-Release date: 29 June 2023
+Release date: 7 July 2023
 
 Requires Python 3.8+ and Sphinx 5+.
 
 1.5.0
 -----
 
 Release date: 8 October 2022
```

### Comparing `numpydoc-1.6.0rc0/doc/validation.rst` & `numpydoc-1.6.0rc1/doc/validation.rst`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/__main__.py` & `numpydoc-1.6.0rc1/numpydoc/__main__.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/docscrape.py` & `numpydoc-1.6.0rc1/numpydoc/docscrape.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/docscrape_sphinx.py` & `numpydoc-1.6.0rc1/numpydoc/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/hooks/utils.py` & `numpydoc-1.6.0rc1/numpydoc/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/hooks/validate_docstrings.py` & `numpydoc-1.6.0rc1/numpydoc/hooks/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/numpydoc.py` & `numpydoc-1.6.0rc1/numpydoc/numpydoc.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/hooks/test_utils.py` & `numpydoc-1.6.0rc1/numpydoc/tests/hooks/test_utils.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/hooks/test_validate_hook.py` & `numpydoc-1.6.0rc1/numpydoc/tests/hooks/test_validate_hook.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/test_docscrape.py` & `numpydoc-1.6.0rc1/numpydoc/tests/test_docscrape.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/test_full.py` & `numpydoc-1.6.0rc1/numpydoc/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/test_main.py` & `numpydoc-1.6.0rc1/numpydoc/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/test_numpydoc.py` & `numpydoc-1.6.0rc1/numpydoc/tests/test_numpydoc.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/test_validate.py` & `numpydoc-1.6.0rc1/numpydoc/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/test_xref.py` & `numpydoc-1.6.0rc1/numpydoc/tests/test_xref.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/conf.py` & `numpydoc-1.6.0rc1/numpydoc/tests/tinybuild/conf.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/numpydoc_test_module.py` & `numpydoc-1.6.0rc1/numpydoc/tests/tinybuild/numpydoc_test_module.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/validate.py` & `numpydoc-1.6.0rc1/numpydoc/validate.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc/xref.py` & `numpydoc-1.6.0rc1/numpydoc/xref.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.6.0rc0/numpydoc.egg-info/SOURCES.txt` & `numpydoc-1.6.0rc1/numpydoc.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 RELEASE.rst
-setup.cfg
-setup.py
+pyproject.toml
 doc/Makefile
 doc/conf.py
 doc/example.py
 doc/example.rst
 doc/format.rst
 doc/index.rst
 doc/install.rst
```

