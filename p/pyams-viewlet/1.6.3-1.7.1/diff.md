# Comparing `tmp/pyams_viewlet-1.6.3.tar.gz` & `tmp/pyams_viewlet-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_viewlet-1.6.3.tar", last modified: Wed Jul 13 14:07:43 2022, max compression
+gzip compressed data, was "dist/pyams_viewlet-1.7.1.tar", last modified: Fri Jul  7 21:37:09 2023, max compression
```

## Comparing `pyams_viewlet-1.6.3.tar` & `pyams_viewlet-1.7.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4213 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1601 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1122 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2346 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    19929 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/include.py
--rw-rw-rw-   0 root         (0) root         (0)     2690 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/locales/fr/LC_MESSAGES/pyams_viewlet.po
--rw-rw-rw-   0 root         (0) root         (0)      491 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/locales/pyams_viewlet.pot
--rw-rw-rw-   0 root         (0) root         (0)    13156 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6449 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     9773 2022-07-13 14:07:21.000000 pyams_viewlet-1.6.3/src/pyams_viewlet/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4213 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      123 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-07-13 14:07:43.000000 pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3480 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1785 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2346 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    19929 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/locales/fr/LC_MESSAGES/pyams_viewlet.po
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/locales/pyams_viewlet.pot
+-rw-rw-rw-   0 root         (0) root         (0)    13156 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6631 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9773 2023-07-07 21:36:54.000000 pyams_viewlet-1.7.1/src/pyams_viewlet/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3480 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      800 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      123 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-07 21:37:09.000000 pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/top_level.txt
```

### Comparing `pyams_viewlet-1.6.3/docs/HISTORY.txt` & `pyams_viewlet-1.7.1/docs/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+1.7.1
+-----
+ - packaging issue
+
+1.7.0
+-----
+ - added support for undefined content providers
+ - added support for boolean provider arguments
+ - added support for Python 3.10 and 3.11
+
 1.6.3
 -----
  - updated Gitlab-CI configuration file
 
 1.6.2
 -----
  - added method to base content provider to load required Fanstatic resources
```

### Comparing `pyams_viewlet-1.6.3/docs/README.txt` & `pyams_viewlet-1.7.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/setup.py` & `pyams_viewlet-1.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import os
 from setuptools import setup, find_packages
 
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
-README = os.path.join(DOCS, 'README.txt')
-HISTORY = os.path.join(DOCS, 'HISTORY.txt')
+README = os.path.join(DOCS, 'README.rst')
+HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.6.3'
+version = '1.7.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = []
 
 setup(name='pyams_viewlet',
       version=version,
       description="PyAMS viewlets management package",
```

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/__init__.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/doctests/README.rst` & `pyams_viewlet-1.7.1/src/pyams_viewlet/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/include.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/include.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/interfaces.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/manager.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/provider.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     def get_value(arg):
         """Extract argument value from context
 
         Extension expression language is quite simple. Values can be given as
         positioned strings, integers or named arguments of the same types.
         """
         arg = arg.strip()
+        if arg in ('True', 'False'):
+            return arg == 'True'
         if arg.startswith('"') or arg.startswith("'"):
             # may be a quoted string...
             return arg[1:-1]
         if '=' in arg:
             key, value = arg.split('=', 1)
             value = get_value(value)
             return {key.strip(): value}
@@ -142,15 +144,18 @@
     request = get_context_arg('request')
     view = get_context_arg('view')
 
     registry = request.registry
     provider = get_provider(name)
 
     # raise an exception if the provider was not found.
+    ignore_missing = get_context_arg('ignore_missing')
     if provider is None:
+        if ignore_missing is True:
+            return ''
         raise ContentProviderLookupError(name)
 
     # add the __name__ attribute if it implements ILocation
     if ILocation.providedBy(provider):
         provider.__name__ = name
 
     # Insert the data gotten from the context
```

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/tests/__init__.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/tests/test_utilsdocs.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/tests/test_utilsdocstrings.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet/viewlet.py` & `pyams_viewlet-1.7.1/src/pyams_viewlet/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_viewlet-1.6.3/src/pyams_viewlet.egg-info/SOURCES.txt` & `pyams_viewlet-1.7.1/src/pyams_viewlet.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
 setup.py
-docs/HISTORY.txt
-docs/README.txt
+docs/HISTORY.rst
+docs/README.rst
 src/pyams_viewlet/__init__.py
 src/pyams_viewlet/include.py
 src/pyams_viewlet/interfaces.py
 src/pyams_viewlet/manager.py
 src/pyams_viewlet/provider.py
 src/pyams_viewlet/viewlet.py
 src/pyams_viewlet.egg-info/PKG-INFO
```

