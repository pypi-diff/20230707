# Comparing `tmp/pyams_mail-1.2.0.tar.gz` & `tmp/pyams_mail-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_mail-1.2.0.tar", last modified: Fri Feb 18 11:26:44 2022, max compression
+gzip compressed data, was "dist/pyams_mail-1.3.0.tar", last modified: Fri Jul  7 21:41:43 2023, max compression
```

## Comparing `pyams_mail-1.2.0.tar` & `pyams_mail-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2480 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)      408 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1006 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2264 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail/
--rw-rw-rw-   0 root         (0) root         (0)      852 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     4312 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/include.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/locales/fr/LC_MESSAGES/pyams_mail.po
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/locales/pyams_mail.pot
--rw-rw-rw-   0 root         (0) root         (0)     1020 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/mailer.py
--rw-rw-rw-   0 root         (0) root         (0)     2559 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail/tests/
--rw-rw-rw-   0 root         (0) root         (0)      799 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2022-02-18 11:26:25.000000 pyams_mail-1.2.0/src/pyams_mail/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2480 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       94 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-02-18 11:26:44.000000 pyams_mail-1.2.0/src/pyams_mail.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      501 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2264 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail/
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/locales/fr/LC_MESSAGES/pyams_mail.po
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/locales/pyams_mail.pot
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/mailer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-07-07 21:41:29.000000 pyams_mail-1.3.0/src/pyams_mail/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-07 21:41:43.000000 pyams_mail-1.3.0/src/pyams_mail.egg-info/top_level.txt
```

### Comparing `pyams_mail-1.2.0/docs/README.txt` & `pyams_mail-1.3.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/setup.py` & `pyams_mail-1.3.0/setup.py`

 * *Files 3% similar despite different names*

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
 
-version = '1.2.0'
+version = '1.3.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = []
 
 setup(name='pyams_mail',
       version=version,
       description="PyAMS mailing helper package",
```

### Comparing `pyams_mail-1.2.0/src/pyams_mail/__init__.py` & `pyams_mail-1.3.0/src/pyams_mail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail/doctests/README.rst` & `pyams_mail-1.3.0/src/pyams_mail/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail/include.py` & `pyams_mail-1.3.0/src/pyams_mail/include.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 #
 
 """PyAMS_mail.include module
 
 This module is used for Pyramid integration
 """
 
-from pyramid_mailer import IMailer, Mailer
+from pyramid_mailer.interfaces import IMailer
+from pyramid_mailer.mailer import DebugMailer, Mailer
 
 
 __docformat__ = 'restructuredtext'
 
 
 def include_package(config):
     """Pyramid package include"""
@@ -29,9 +30,13 @@
 
     config.scan()
 
     settings = config.registry.settings
     mailers = settings.get('pyams_mail.mailers')
     if mailers:
         for prefix in mailers.split():
-            config.registry.registerUtility(Mailer.from_settings(settings, prefix), IMailer,
-                                            name=settings['{0}name'.format(prefix)])
+            if settings.get(f'{prefix}mode') == 'debug':
+                config.registry.registerUtility(DebugMailer.from_settings(settings, prefix), IMailer,
+                                                name=settings[f'{prefix}name'])
+            else:
+                config.registry.registerUtility(Mailer.from_settings(settings, prefix), IMailer,
+                                                name=settings[f'{prefix}name'])
```

### Comparing `pyams_mail-1.2.0/src/pyams_mail/interfaces.py` & `pyams_mail-1.3.0/src/pyams_mail/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail/mailer.py` & `pyams_mail-1.3.0/src/pyams_mail/mailer.py`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail/message.py` & `pyams_mail-1.3.0/src/pyams_mail/message.py`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail/tests/__init__.py` & `pyams_mail-1.3.0/src/pyams_mail/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail/tests/test_utilsdocs.py` & `pyams_mail-1.3.0/src/pyams_mail/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail/tests/test_utilsdocstrings.py` & `pyams_mail-1.3.0/src/pyams_mail/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_mail-1.2.0/src/pyams_mail.egg-info/SOURCES.txt` & `pyams_mail-1.3.0/src/pyams_mail.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
 setup.py
-docs/HISTORY.txt
-docs/README.txt
+docs/HISTORY.rst
+docs/README.rst
 src/pyams_mail/__init__.py
 src/pyams_mail/include.py
 src/pyams_mail/interfaces.py
 src/pyams_mail/mailer.py
 src/pyams_mail/message.py
 src/pyams_mail.egg-info/PKG-INFO
 src/pyams_mail.egg-info/SOURCES.txt
```

