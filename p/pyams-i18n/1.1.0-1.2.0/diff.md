# Comparing `tmp/pyams_i18n-1.1.0.tar.gz` & `tmp/pyams_i18n-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_i18n-1.1.0.tar", last modified: Mon Mar  8 21:57:54 2021, max compression
+gzip compressed data, was "dist/pyams_i18n-1.2.0.tar", last modified: Fri Jul  7 21:21:34 2023, max compression
```

## Comparing `pyams_i18n-1.1.0.tar` & `pyams_i18n-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      104 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2876 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/PKG-INFO
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)      690 2021-03-08 21:53:00.000000 pyams_i18n-1.1.0/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1057 2020-10-09 12:05:57.000000 pyams_i18n-1.1.0/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2403 2021-03-08 21:53:00.000000 pyams_i18n-1.1.0/setup.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n/
--rw-rw-rw-   0 root         (0) root         (0)      866 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3068 2020-12-26 23:00:45.000000 pyams_i18n-1.1.0/src/pyams_i18n/attr.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/content.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    18148 2021-03-08 21:53:00.000000 pyams_i18n-1.1.0/src/pyams_i18n/doctests/README.rst
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1321 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/include.py
--rw-rw-rw-   0 root         (0) root         (0)     4253 2020-12-26 23:00:45.000000 pyams_i18n-1.1.0/src/pyams_i18n/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    15048 2020-10-09 12:05:57.000000 pyams_i18n-1.1.0/src/pyams_i18n/language.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n/locales/
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n/locales/fr/
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    21351 2020-12-26 23:00:45.000000 pyams_i18n-1.1.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.mo
--rw-rw-rw-   0 root         (0) root         (0)    34630 2020-12-26 23:00:45.000000 pyams_i18n-1.1.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.po
--rw-rw-rw-   0 root         (0) root         (0)    28981 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/locales/pyams_i18n.pot
--rw-rw-rw-   0 root         (0) root         (0)     5609 2020-12-26 23:00:45.000000 pyams_i18n-1.1.0/src/pyams_i18n/negotiator.py
--rw-rw-rw-   0 root         (0) root         (0)     5070 2020-10-09 12:05:57.000000 pyams_i18n-1.1.0/src/pyams_i18n/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2020-12-26 23:00:45.000000 pyams_i18n-1.1.0/src/pyams_i18n/tales.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n/tests/
--rw-rw-rw-   0 root         (0) root         (0)      799 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     2899 2020-01-18 02:00:49.000000 pyams_i18n-1.1.0/src/pyams_i18n/vocabulary.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2876 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      171 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-03-08 21:57:54.000000 pyams_i18n-1.1.0/src/pyams_i18n.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      846 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2403 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/attr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    18148 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     4253 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    15048 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/language.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    21351 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.mo
+-rw-rw-rw-   0 root         (0) root         (0)    34630 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.po
+-rw-rw-rw-   0 root         (0) root         (0)    28981 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/locales/pyams_i18n.pot
+-rw-rw-rw-   0 root         (0) root         (0)     5609 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/negotiator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/tales.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2899 2023-07-07 21:21:20.000000 pyams_i18n-1.2.0/src/pyams_i18n/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-07 21:21:34.000000 pyams_i18n-1.2.0/src/pyams_i18n.egg-info/top_level.txt
```

### Comparing `pyams_i18n-1.1.0/docs/HISTORY.txt` & `pyams_i18n-1.2.0/docs/HISTORY.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.2.0
+-----
+ - added support for default value when using I18n query_attribute method
+   or i18n TALES extension
+ - added support for Python 3.10 and 3.11
+
 1.1.0
 -----
  - removed support for Python < 3.7
  - updated doctests
 
 1.0.7
 -----
```

### Comparing `pyams_i18n-1.1.0/docs/README.txt` & `pyams_i18n-1.2.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/setup.py` & `pyams_i18n-1.2.0/setup.py`

 * *Files 7% similar despite different names*

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
 
-version = '1.1.0'
+version = '1.2.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyramid_zodbconn',
     'pyams_template'
 ]
```

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/__init__.py` & `pyams_i18n-1.2.0/src/pyams_i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/attr.py` & `pyams_i18n-1.2.0/src/pyams_i18n/attr.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 from pyams_utils.registry import query_utility
 from pyams_utils.request import check_request
 
 
 __docformat__ = 'restructuredtext'
 
 
-@adapter_config(name='i18n', required=Interface, provides=ITraversable)
+@adapter_config(name='i18n',
+                required=Interface,
+                provides=ITraversable)
 class I18nAttributeTraverser(ContextAdapter):
     """++i18n++attr:lang namespace traverser
 
     This traverser is used, for example, by I18n file fields (see :py:mod:pyams_file).
     """
 
     def traverse(self, name, furtherpath=None):  # pylint: disable=unused-argument
@@ -40,15 +42,16 @@
         try:
             attr, lang = name.split(':')
             return getattr(self.context, attr, {}).get(lang)
         except (AttributeError, ValueError):
             raise NotFound
 
 
-@adapter_config(required=Interface, provides=II18n)
+@adapter_config(required=Interface,
+                provides=II18n)
 class I18nAttributeAdapter(ContextAdapter):
     """I18n attribute adapter"""
 
     def get_attribute(self, attribute, lang=None, request=None, default=None):
         """Extract attribute value for given language or request"""
         result = getattr(self.context, attribute)
         if not isinstance(result, dict):
@@ -60,15 +63,15 @@
         return result.get(lang, default)
 
     def query_attribute(self, attribute, lang=None, request=None, default=None):
         """Extract attribute value for given language or request
 
         If value is empty or None, value associated to server language is returned.
         """
-        result = getattr(self.context, attribute)
+        result = getattr(self.context, attribute, default)
         if not isinstance(result, dict):
             return result
         if lang is None:
             if request is None:
                 request = check_request()
             lang = request.params.get('lang') or request.locale_name
         value = result.get(lang)
```

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/content.py` & `pyams_i18n-1.2.0/src/pyams_i18n/content.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/doctests/README.rst` & `pyams_i18n-1.2.0/src/pyams_i18n/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/generations/__init__.py` & `pyams_i18n-1.2.0/src/pyams_i18n/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/include.py` & `pyams_i18n-1.2.0/src/pyams_i18n/include.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/interfaces.py` & `pyams_i18n-1.2.0/src/pyams_i18n/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/language.py` & `pyams_i18n-1.2.0/src/pyams_i18n/language.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.mo` & `pyams_i18n-1.2.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.mo`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.po` & `pyams_i18n-1.2.0/src/pyams_i18n/locales/fr/LC_MESSAGES/pyams_i18n.po`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/locales/pyams_i18n.pot` & `pyams_i18n-1.2.0/src/pyams_i18n/locales/pyams_i18n.pot`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/negotiator.py` & `pyams_i18n-1.2.0/src/pyams_i18n/negotiator.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/schema.py` & `pyams_i18n-1.2.0/src/pyams_i18n/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/tales.py` & `pyams_i18n-1.2.0/src/pyams_i18n/tales.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,13 +69,8 @@
     attributes.
     Please note that this extension returns default value when applied on a non-existent
     attribute, not on an attribute with an empty value for selected language!
     """
 
     def render(self, context, attribute, default=None):
         """Render TALES extension"""
-        try:
-            # pylint: disable=assignment-from-no-return
-            value = II18n(context).query_attribute(attribute, request=self.request)
-        except AttributeError:
-            value = default
-        return value
+        return II18n(context).query_attribute(attribute, request=self.request, default=default)
```

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/tests/__init__.py` & `pyams_i18n-1.2.0/src/pyams_i18n/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/tests/test_utilsdocs.py` & `pyams_i18n-1.2.0/src/pyams_i18n/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/tests/test_utilsdocstrings.py` & `pyams_i18n-1.2.0/src/pyams_i18n/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n/vocabulary.py` & `pyams_i18n-1.2.0/src/pyams_i18n/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pyams_i18n-1.1.0/src/pyams_i18n.egg-info/SOURCES.txt` & `pyams_i18n-1.2.0/src/pyams_i18n.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
 setup.py
-docs/HISTORY.txt
-docs/README.txt
+docs/HISTORY.rst
+docs/README.rst
 src/pyams_i18n/__init__.py
 src/pyams_i18n/attr.py
 src/pyams_i18n/content.py
 src/pyams_i18n/include.py
 src/pyams_i18n/interfaces.py
 src/pyams_i18n/language.py
 src/pyams_i18n/negotiator.py
```

