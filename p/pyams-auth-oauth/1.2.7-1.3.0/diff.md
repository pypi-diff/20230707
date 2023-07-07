# Comparing `tmp/pyams_auth_oauth-1.2.7.tar.gz` & `tmp/pyams_auth_oauth-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_auth_oauth-1.2.7.tar", last modified: Tue Dec 27 01:43:27 2022, max compression
+gzip compressed data, was "dist/pyams_auth_oauth-1.3.0.tar", last modified: Fri Jul  7 21:52:21 2023, max compression
```

## Comparing `pyams_auth_oauth-1.2.7.tar` & `pyams_auth_oauth-1.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2807 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1171 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2662 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/
--rw-rw-rw-   0 root         (0) root         (0)      899 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    10367 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1061 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/include.py
--rw-rw-rw-   0 root         (0) root         (0)     6762 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5821 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.mo
--rw-rw-rw-   0 root         (0) root         (0)     8543 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.po
--rw-rw-rw-   0 root         (0) root         (0)     6245 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/pyams_auth_oauth.pot
--rw-rw-rw-   0 root         (0) root         (0)    22191 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/skin/
--rw-rw-rw-   0 root         (0) root         (0)     5210 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      567 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/skin/templates/login-providers.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/tests/
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1835 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1873 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      561 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8620 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/folder.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3891 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    10592 2022-12-27 01:43:05.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2807 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1137 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      301 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-12-27 01:43:27.000000 pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1135 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2688 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    10453 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     6762 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.mo
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.po
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/pyams_auth_oauth.pot
+-rw-rw-rw-   0 root         (0) root         (0)    20583 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     5210 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/skin/templates/login-providers.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8620 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3891 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    10592 2023-07-07 21:52:04.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      318 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-07 21:52:21.000000 pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/top_level.txt
```

### Comparing `pyams_auth_oauth-1.2.7/LICENSE` & `pyams_auth_oauth-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/PKG-INFO` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_auth_oauth
-Version: 1.2.7
+Name: pyams-auth-oauth
+Version: 1.3.0
 Summary: PyAMS security plug-in for OAuth authentication
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -47,14 +47,18 @@
 You have to include this package in your Pyramid configuration to activate this plug-in, but also
 to register providers for which you want to allow access from.
 
 
 Changelog
 =========
 
+1.3.0
+-----
+ - added support for MicrosoftOnline OAuth2 provider
+
 1.2.7
 -----
  - updated management interface
  - updated providers viewlet
  - small code refactoring to simplify super() calls
  - added missing parent class to OAuth provider connection
  - added support for Python 3.11
```

### Comparing `pyams_auth_oauth-1.2.7/docs/HISTORY.rst` & `pyams_auth_oauth-1.3.0/docs/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.3.0
+-----
+ - added support for MicrosoftOnline OAuth2 provider
+
 1.2.7
 -----
  - updated management interface
  - updated providers viewlet
  - small code refactoring to simplify super() calls
  - added missing parent class to OAuth provider connection
  - added support for Python 3.11
```

### Comparing `pyams_auth_oauth-1.2.7/docs/README.rst` & `pyams_auth_oauth-1.3.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/setup.py` & `pyams_auth_oauth-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.2.7'
+version = '1.3.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_site',
     'pyams_skin',
     'pyams_viewlet',
+    'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
 
 setup(name='pyams_auth_oauth',
       version=version,
       description="PyAMS security plug-in for OAuth authentication",
@@ -60,15 +61,15 @@
       # uncomment this to be able to run tests with setup.py
       test_suite="pyams_auth_oauth.tests.test_utilsdocs.test_suite",
       tests_require=tests_require,
       extras_require=dict(test=tests_require),
       install_requires=[
           'setuptools',
           # -*- Extra requirements: -*-
-          'authomatic',
+          'authomatic >= 1.2.0',
           'persistent',
           'pyams_form',
           'pyams_layer',
           'pyams_security >= 1.8.1',
           'pyams_security_views',
           'pyams_template',
           'pyams_utils',
```

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/__init__.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/doctests/README.rst` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/doctests/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     >>> include_zodbconn(config)
     >>> from cornice import includeme as include_cornice
     >>> include_cornice(config)
     >>> from pyams_utils import includeme as include_utils
     >>> include_utils(config)
     >>> from pyams_site import includeme as include_site
     >>> include_site(config)
+    >>> from pyams_form import includeme as include_form
+    >>> include_form(config)
     >>> from pyams_security import includeme as include_security
     >>> include_security(config)
     >>> from pyams_auth_oauth import includeme as include_auth_oauth
     >>> include_auth_oauth(config)
 
     >>> from pyams_site.generations import upgrade_site
     >>> request = DummyRequest()
```

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/include.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/include.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/interfaces.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.mo` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.mo`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.po` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/fr/LC_MESSAGES/pyams_auth_oauth.po`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/locales/pyams_auth_oauth.pot` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/locales/pyams_auth_oauth.pot`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/plugin.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -249,153 +249,128 @@
 
     name = FieldProperty(IOAuthLoginProviderInfo['name'])
     provider = None
     icon_class = FieldProperty(IOAuthLoginProviderInfo['icon_class'])
     icon_filename = FieldProperty(IOAuthLoginProviderInfo['icon_filename'])
     scope = FieldProperty(IOAuthLoginProviderInfo['scope'])
 
-    def __init__(self, name, provider, **kwargs):
-        self.name = name
+    def __init__(self, provider, **kwargs):
         self.provider = provider
+        self.name = kwargs.get('name') or provider.__name__
         for key, value in kwargs.items():
             setattr(self, key, value)
 
 
 PROVIDERS_INFO = {
-    'amazon': OAuthLoginProviderInfo(name=oauth2.Amazon.__name__,
-                                     provider=oauth2.Amazon,
+    'amazon': OAuthLoginProviderInfo(provider=oauth2.Amazon,
                                      icon_class='fab fa-fw fa-amazon',
                                      icon_filename='amazon.ico',
                                      scope=oauth2.Amazon.user_info_scope),
-    'behance': OAuthLoginProviderInfo(name=oauth2.Behance.__name__,
-                                      provider=oauth2.Behance,
+    'behance': OAuthLoginProviderInfo(provider=oauth2.Behance,
                                       icon_class='fab fa-fw fa-behance-square',
                                       icon_filename='behance.ico',
                                       scope=oauth2.Behance.user_info_scope),
-    'bitbucket': OAuthLoginProviderInfo(name=oauth1.Bitbucket.__name__,
-                                        provider=oauth1.Bitbucket,
+    'bitbucket': OAuthLoginProviderInfo(provider=oauth1.Bitbucket,
                                         icon_class='fab fa-fw fa-bitbucket',
                                         icon_filename='bitbucket.ico'),
-    'bitly': OAuthLoginProviderInfo(name=oauth2.Bitly.__name__,
-                                    provider=oauth2.Bitly,
+    'bitly': OAuthLoginProviderInfo(provider=oauth2.Bitly,
                                     icon_class='fab fa-fw fa-bitly',
                                     icon_filename='bitly.ico',
                                     scope=oauth2.Bitly.user_info_scope),
-    'cosm': OAuthLoginProviderInfo(name=oauth2.Cosm.__name__,
-                                   provider=oauth2.Cosm,
+    'cosm': OAuthLoginProviderInfo(provider=oauth2.Cosm,
                                    icon_class='fa fa-fw fa-share-alt',
                                    icon_filename='cosm.ico',
                                    scope=oauth2.Cosm.user_info_scope),
-    'devianart': OAuthLoginProviderInfo(name=oauth2.DeviantART.__name__,
-                                        provider=oauth2.DeviantART,
+    'devianart': OAuthLoginProviderInfo(provider=oauth2.DeviantART,
                                         icon_class='fab fa-fw fa-deviantart',
                                         icon_filename='deviantart.ico',
                                         scope=oauth2.DeviantART.user_info_scope),
-    'eventbrite': OAuthLoginProviderInfo(name=oauth2.Eventbrite.__name__,
-                                         provider=oauth2.Eventbrite,
+    'eventbrite': OAuthLoginProviderInfo(provider=oauth2.Eventbrite,
                                          icon_class='fa fa-fw fa-eventbrite',
                                          icon_filename='eventbrite.ico',
                                          scope=oauth2.Eventbrite.user_info_scope),
-    'facebook': OAuthLoginProviderInfo(name=oauth2.Facebook.__name__,
-                                       provider=oauth2.Facebook,
+    'facebook': OAuthLoginProviderInfo(provider=oauth2.Facebook,
                                        icon_class='fab fa-fw fa-facebook-square',
                                        icon_filename='facebook.ico',
                                        scope=oauth2.Facebook.user_info_scope),
-    'foursquare': OAuthLoginProviderInfo(name=oauth2.Foursquare.__name__,
-                                         provider=oauth2.Foursquare,
+    'foursquare': OAuthLoginProviderInfo(provider=oauth2.Foursquare,
                                          icon_class='fab fa-fw fa-foursquare',
                                          icon_filename='foursquare.ico',
                                          scope=oauth2.Foursquare.user_info_scope),
-    'flickr': OAuthLoginProviderInfo(name=oauth1.Flickr.__name__,
-                                     provider=oauth1.Flickr,
+    'flickr': OAuthLoginProviderInfo(provider=oauth1.Flickr,
                                      icon_class='fab fa-fw fa-flickr',
                                      icon_filename='flickr.ico'),
-    'github': OAuthLoginProviderInfo(name=oauth2.GitHub.__name__,
-                                     provider=oauth2.GitHub,
+    'github': OAuthLoginProviderInfo(provider=oauth2.GitHub,
                                      icon_class='fab fa-fw fa-github',
                                      icon_filename='github.ico',
                                      scope=oauth2.GitHub.user_info_scope),
-    'google': OAuthLoginProviderInfo(name=oauth2.Google.__name__,
-                                     provider=oauth2.Google,
+    'google': OAuthLoginProviderInfo(provider=oauth2.Google,
                                      icon_class='fab fa-fw fa-google',
                                      icon_filename='google.ico',
                                      scope=oauth2.Google.user_info_scope),
-    'linkedin': OAuthLoginProviderInfo(name=oauth2.LinkedIn.__name__,
-                                       provider=oauth2.LinkedIn,
+    'linkedin': OAuthLoginProviderInfo(provider=oauth2.LinkedIn,
                                        icon_class='fab fa-fw fa-linkedin-square',
                                        icon_filename='linkedin.ico',
                                        scope=oauth2.LinkedIn.user_info_scope),
-    'meetup': OAuthLoginProviderInfo(name=oauth1.Meetup.__name__,
-                                     provider=oauth1.Meetup,
+    'meetup': OAuthLoginProviderInfo(provider=oauth1.Meetup,
                                      icon_class='fab fa-fw fa-meetup',
                                      icon_filename='meetup.ico'),
-    'paypal': OAuthLoginProviderInfo(name=oauth2.PayPal.__name__,
-                                     provider=oauth2.PayPal,
+    'microsoft': OAuthLoginProviderInfo(provider=oauth2.MicrosoftOnline,
+                                        icon_class='fab fa-fw fa-windows',
+                                        icon_filename='microsoft.ico',
+                                        scope=oauth2.MicrosoftOnline.user_info_scope),
+    'paypal': OAuthLoginProviderInfo(provider=oauth2.PayPal,
                                      icon_class='fab fa-fw fa-paypal',
                                      icon_filename='paypal.ico',
                                      scope=oauth2.PayPal.user_info_scope),
-    'plurk': OAuthLoginProviderInfo(name=oauth1.Plurk.__name__,
-                                    provider=oauth1.Plurk,
+    'plurk': OAuthLoginProviderInfo(provider=oauth1.Plurk,
                                     icon_class='fa fa-fw fa-share-alt',
                                     icon_filename='plurk.ico'),
-    'reddit': OAuthLoginProviderInfo(name=oauth2.Reddit.__name__,
-                                     provider=oauth2.Reddit,
+    'reddit': OAuthLoginProviderInfo(provider=oauth2.Reddit,
                                      icon_class='fab fa-fw fa-reddit',
                                      icon_filename='reddit.ico',
                                      scope=oauth2.Reddit.user_info_scope),
-    'tumblr': OAuthLoginProviderInfo(name=oauth1.Tumblr.__name__,
-                                     provider=oauth1.Tumblr,
+    'tumblr': OAuthLoginProviderInfo(provider=oauth1.Tumblr,
                                      icon_class='fab fa-fw fa-tumblr-square',
                                      icon_filename='tumblr.ico'),
-    'twitter': OAuthLoginProviderInfo(name=oauth1.Twitter.__name__,
-                                      provider=oauth1.Twitter,
+    'twitter': OAuthLoginProviderInfo(provider=oauth1.Twitter,
                                       icon_class='fab fa-fw fa-twitter',
                                       icon_filename='twitter.ico'),
-    'ubuntuone': OAuthLoginProviderInfo(name=oauth1.UbuntuOne.__name__,
-                                        provider=oauth1.UbuntuOne,
+    'ubuntuone': OAuthLoginProviderInfo(provider=oauth1.UbuntuOne,
                                         icon_class='fab fa-fw fa-ubuntu',
                                         icon_filename='ubuntuone.ico'),
-    'viadeo': OAuthLoginProviderInfo(name=oauth2.Viadeo.__name__,
-                                     provider=oauth2.Viadeo,
+    'viadeo': OAuthLoginProviderInfo(provider=oauth2.Viadeo,
                                      icon_class='fab fa-fw fa-viadeo',
                                      icon_filename='viadeo.ico',
                                      scope=oauth2.Viadeo.user_info_scope),
-    'vimeo': OAuthLoginProviderInfo(name=oauth1.Vimeo.__name__,
-                                    provider=oauth1.Vimeo,
+    'vimeo': OAuthLoginProviderInfo(provider=oauth1.Vimeo,
                                     icon_class='fab fa-fw fa-vimeo-square',
                                     icon_filename='vimeo.ico'),
-    'vk': OAuthLoginProviderInfo(name=oauth2.VK.__name__,
-                                 provider=oauth2.VK,
+    'vk': OAuthLoginProviderInfo(provider=oauth2.VK,
                                  icon_class='fab fa-fw fa-vk',
                                  icon_filename='vk.ico',
                                  scope=oauth2.VK.user_info_scope),
-    'windowslive': OAuthLoginProviderInfo(name=oauth2.WindowsLive.__name__,
-                                          provider=oauth2.WindowsLive,
+    'windowslive': OAuthLoginProviderInfo(provider=oauth2.WindowsLive,
                                           icon_class='fab fa-fw fa-windows',
                                           icon_filename='windows_live.ico',
                                           scope=oauth2.WindowsLive.user_info_scope),
-    'xero': OAuthLoginProviderInfo(name=oauth1.Xero.__name__,
-                                   provider=oauth1.Xero,
+    'xero': OAuthLoginProviderInfo(provider=oauth1.Xero,
                                    icon_class='fa fa-fw fa-share-alt',
                                    icon_filename='xero.ico'),
-    'xing': OAuthLoginProviderInfo(name=oauth1.Xing.__name__,
-                                   provider=oauth1.Xing,
+    'xing': OAuthLoginProviderInfo(provider=oauth1.Xing,
                                    icon_class='fab fa-fw fa-xing',
                                    icon_filename='xing.ico'),
-    'yahoo': OAuthLoginProviderInfo(name=oauth1.Yahoo.__name__,
-                                    provider=oauth1.Yahoo,
+    'yahoo': OAuthLoginProviderInfo(provider=oauth1.Yahoo,
                                     icon_class='fab fa-fw fa-yahoo',
                                     icon_filename='yahoo.ico'),
-    'yammer': OAuthLoginProviderInfo(name=oauth2.Yammer.__name__,
-                                     provider=oauth2.Yammer,
+    'yammer': OAuthLoginProviderInfo(provider=oauth2.Yammer,
                                      icon_class='fab fa-fw fa-yammer',
                                      icon_filename='yammer.ico',
                                      scope=oauth2.Yammer.user_info_scope),
-    'yandex': OAuthLoginProviderInfo(name=oauth2.Yandex.__name__,
-                                     provider=oauth2.Yandex,
+    'yandex': OAuthLoginProviderInfo(provider=oauth2.Yandex,
                                      icon_class='fab fa-fw fa-yandex',
                                      icon_filename='yandex.ico',
                                      scope=oauth2.Yandex.user_info_scope)
 }
 
 
 def get_provider_info(provider_name):
```

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/skin/__init__.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/skin/templates/login-providers.pt` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/skin/templates/login-providers.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <fieldset tal:define="(has_providers, providers) tales:boolean_iter(view.providers)"
-		  tal:condition="has_providers"
-		  class="border"
-		  i18n:domain="pyams_auth_oauth">
-	<legend i18n:translate="">External login providers</legend>
-	<div class="d-flex pb-2">
-		<tal:loop repeat="provider providers">
-			<a tal:define="configuration provider.get_configuration()"
-			   href="/api/auth/oauth/${provider.provider_name}">
-				<i class="${configuration.icon_class} fa-3x"
-				   data-original-title="${configuration.name}"></i>
-			</a>
-		</tal:loop>
-	</div>
+          tal:condition="has_providers"
+          class="border"
+          i18n:domain="pyams_auth_oauth">
+    <legend class="ml-3 px-2 w-auto rounded border"
+            i18n:translate="">External login providers</legend>
+    <div class="d-flex px-3 pb-2">
+        <tal:loop repeat="provider providers">
+            <a tal:define="configuration provider.get_configuration()"
+               href="/api/auth/oauth/${provider.provider_name}">
+                <i class="${configuration.icon_class} fa-3x hint"
+                   data-original-title="${configuration.name}"></i>
+            </a>
+        </tal:loop>
+    </div>
 </fieldset>
```

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/tests/__init__.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/tests/test_utilsdocs.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/tests/test_utilsdocstrings.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/__init__.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/folder.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/interfaces.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/plugin.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth/zmi/provider.py` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth/zmi/provider.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/PKG-INFO` & `pyams_auth_oauth-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-auth-oauth
-Version: 1.2.7
+Name: pyams_auth_oauth
+Version: 1.3.0
 Summary: PyAMS security plug-in for OAuth authentication
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -47,14 +47,18 @@
 You have to include this package in your Pyramid configuration to activate this plug-in, but also
 to register providers for which you want to allow access from.
 
 
 Changelog
 =========
 
+1.3.0
+-----
+ - added support for MicrosoftOnline OAuth2 provider
+
 1.2.7
 -----
  - updated management interface
  - updated providers viewlet
  - small code refactoring to simplify super() calls
  - added missing parent class to OAuth provider connection
  - added support for Python 3.11
```

### Comparing `pyams_auth_oauth-1.2.7/src/pyams_auth_oauth.egg-info/SOURCES.txt` & `pyams_auth_oauth-1.3.0/src/pyams_auth_oauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

