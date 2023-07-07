# Comparing `tmp/otc_sphinx_directives-0.2.6.tar.gz` & `tmp/otc_sphinx_directives-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otc_sphinx_directives-0.2.6.tar", last modified: Thu Jul  6 12:31:41 2023, max compression
+gzip compressed data, was "otc_sphinx_directives-0.2.7.tar", last modified: Fri Jul  7 10:56:17 2023, max compression
```

## Comparing `otc_sphinx_directives-0.2.6.tar` & `otc_sphinx_directives-0.2.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.491681 otc_sphinx_directives-0.2.6/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/.stestr.conf
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     2025 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-06 12:31:41.491681 otc_sphinx_directives-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.488681 otc_sphinx_directives-0.2.6/doc/
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.489681 otc_sphinx_directives-0.2.6/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.489681 otc_sphinx_directives-0.2.6/doc/source/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/_static/.placeholder
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.489681 otc_sphinx_directives-0.2.6/doc/source/examples/
--rw-r--r--   0 root         (0) root         (0)      221 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/examples/directives_docsportal.rst
--rw-r--r--   0 root         (0) root         (0)      966 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/examples/directives_ecs.rst
--rw-r--r--   0 root         (0) root         (0)     1386 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/examples/directives_obs.rst
--rw-r--r--   0 root         (0) root         (0)      423 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/examples/directives_obs_clean.rst
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/examples/index.rst
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.490681 otc_sphinx_directives-0.2.6/otc_sphinx_directives/
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/container_item.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/document_navigator.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/navigator.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/otc_sphinx_directives_setup.py
--rw-r--r--   0 root         (0) root         (0)     3582 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/service_card.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/service_group.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/service_navigator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.491681 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.487681 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.491681 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/directive_wrapper/
--rw-r--r--   0 root         (0) root         (0)      791 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.491681 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/service_card/
--rw-r--r--   0 root         (0) root         (0)      791 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/service_card/conf.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/service_card/index.rst
--rw-r--r--   0 root         (0) root         (0)     2330 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/test_directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/test_service_card.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:31:41.490681 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-06 12:31:41.000000 otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-06 12:31:41.492681 otc_sphinx_directives-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/setup.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1366 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/tox.ini
--rw-r--r--   0 root         (0) root         (0)      245 2023-07-06 12:30:19.000000 otc_sphinx_directives-0.2.6/zuul.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/.stestr.conf
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/source/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/_static/.placeholder
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/source/examples/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_docsportal.rst
+-rw-r--r--   0 root         (0) root         (0)      966 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_ecs.rst
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_obs.rst
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_obs_clean.rst
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/index.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.575236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/container_item.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/document_navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/otc_sphinx_directives_setup.py
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_card.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_group.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_navigator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.573236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/conf.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_service_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-07 10:56:17.577236 otc_sphinx_directives-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/tox.ini
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/zuul.yaml
```

### Comparing `otc_sphinx_directives-0.2.6/ChangeLog` & `otc_sphinx_directives-0.2.7/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.2.7
+-----
+
+* fix doc type typo (#23)
+
 0.2.6
 -----
 
 * adding new doc types (#22)
 * Update service\_navigator.py for sorting of service panel (#21)
 * Adding sorting of metadadata before processing to navigator (#20)
```

### Comparing `otc_sphinx_directives-0.2.6/LICENSE` & `otc_sphinx_directives-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/PKG-INFO` & `otc_sphinx_directives-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc_sphinx_directives
-Version: 0.2.6
+Version: 0.2.7
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.6/doc/source/examples/directives_ecs.rst` & `otc_sphinx_directives-0.2.7/doc/source/examples/directives_ecs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/doc/source/examples/directives_obs.rst` & `otc_sphinx_directives-0.2.7/doc/source/examples/directives_obs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/container_item.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/container_item.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/directive_wrapper.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/document_navigator.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/document_navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/navigator.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/otc_sphinx_directives_setup.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/otc_sphinx_directives_setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/service_card.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         'operation-guide-lts': directives.unchanged,
         'parallel-file-system': directives.unchanged,
         'permissions-configuration-guide': directives.unchanged,
         'permissions': directives.unchanged,
         'swiftapi': directives.unchanged,
         's3api': directives.unchanged,
         'umn': directives.unchanged,
-        'best-practise': directives.unchanged,
+        'best-practice': directives.unchanged,
     }
 
     has_content = True
 
     def run(self):
         node = self.node_class()
         for k in self.option_spec:
```

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/service_group.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_group.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/service_navigator.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/base.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/base.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/templates/service_card/conf.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/test_directive_wrapper.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives/tests/test_service_card.py` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_service_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     '<div class="card-body">'
     '<h4>User Guide</h4><p></p></div></a></div>'
     '<div class="card item-sbv">'
     '<a href="api-ref/">'
     '<div class="card-body">'
     '<h4>API Reference</h4><p></p></div></a></div>'
     '<div class="card item-sbv">'
-    '<a href="best-practise/">'
+    '<a href="best-practice/">'
     '<div class="card-body">'
-    '<h4>Best Practise</h4><p></p></div></a></div>'
+    '<h4>Best Practice</h4><p></p></div></a></div>'
     '<div class="card item-sbv">'
     '<a href="dev-guide/">'
     '<div class="card-body">'
     '<h4>Developer Guide</h4><p></p></div></a></div></div>'
 )
```

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/PKG-INFO` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc-sphinx-directives
-Version: 0.2.6
+Version: 0.2.7
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.6/otc_sphinx_directives.egg-info/SOURCES.txt` & `otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/setup.cfg` & `otc_sphinx_directives-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/setup.py` & `otc_sphinx_directives-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.6/tox.ini` & `otc_sphinx_directives-0.2.7/tox.ini`

 * *Files identical despite different names*

