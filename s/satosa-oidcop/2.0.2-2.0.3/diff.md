# Comparing `tmp/satosa_oidcop-2.0.2.tar.gz` & `tmp/satosa_oidcop-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosa_oidcop-2.0.2.tar", last modified: Wed Jun 21 10:03:03 2023, max compression
+gzip compressed data, was "satosa_oidcop-2.0.3.tar", last modified: Fri Jul  7 09:48:46 2023, max compression
```

## Comparing `satosa_oidcop-2.0.2.tar` & `satosa_oidcop-2.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:03.598061 satosa_oidcop-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-21 10:03:03.598061 satosa_oidcop-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:03.594061 satosa_oidcop-2.0.2/satosa_oidcop/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:03.598061 satosa_oidcop-2.0.2/satosa_oidcop/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:03.598061 satosa_oidcop-2.0.2/satosa_oidcop/core/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/user_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/core/user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/satosa_oidcop/idpy_oidcop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:03.594061 satosa_oidcop-2.0.2/satosa_oidcop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-21 10:03:03.000000 satosa_oidcop-2.0.2/satosa_oidcop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-21 10:03:03.000000 satosa_oidcop-2.0.2/satosa_oidcop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:03:03.000000 satosa_oidcop-2.0.2/satosa_oidcop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 10:03:03.000000 satosa_oidcop-2.0.2/satosa_oidcop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 10:03:03.000000 satosa_oidcop-2.0.2/satosa_oidcop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 10:03:03.598061 satosa_oidcop-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-21 10:02:22.000000 satosa_oidcop-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.347530 satosa_oidcop-2.0.3/satosa_oidcop/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/satosa_oidcop/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/user_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/idpy_oidcop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/setup.py
```

### Comparing `satosa_oidcop-2.0.2/LICENSE` & `satosa_oidcop-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/PKG-INFO` & `satosa_oidcop-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosa_oidcop
-Version: 2.0.2
+Version: 2.0.3
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -15,22 +15,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SATOSA oidcop frontend
 
-![CI build](https://github.com/UniversitaDellaCalabria/satosa-oidcop/workflows/satosa_oidcop/badge.svg)
-![Python version](https://img.shields.io/badge/license-Affero%203-blue.svg)
+[![CI build](https://github.com/UniversitaDellaCalabria/satosa-oidcop/workflows/satosa_oidcop/badge.svg)](https://github.com/UniversitaDellaCalabria/SATOSA-oidcop/actions)
+[![License](https://img.shields.io/pypi/l/satosa_oidcop)](./LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/satosa_oidcop)](https://pypi.org/project/satosa-oidcop/)
 [![Downloads](https://pepy.tech/badge/satosa-oidcop)](https://pepy.tech/project/satosa-oidcop)
 [![Downloads per week](https://pepy.tech/badge/satosa-oidcop/week)](https://pepy.tech/project/satosa-oidcop)
-![License](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.11-blue.svg)
+[![Python version](https://img.shields.io/pypi/pyversions/satosa_oidcop)](https://pypi.org/project/satosa-oidcop/)
 [![Conventional commits](https://img.shields.io/badge/semantic--release-conventional-e10079?logo=semantic-release)](https://conventionalcommits.org/)
 
-SATOSA Frontend based on [identity python oidcop](https://github.com/IdentityPython/oidc-op).
+SATOSA Frontend based on [idpyoidc by Identity Python](https://github.com/IdentityPython/idpy-oidc)
+(previously [identity python oidcop](https://github.com/IdentityPython/oidc-op)).
 
 ## Features
 
 Endpoints:
 
 - [x] provider discovery
 - [x] jwks uri
```

### Comparing `satosa_oidcop-2.0.2/README.md` & `satosa_oidcop-2.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # SATOSA oidcop frontend
 
-![CI build](https://github.com/UniversitaDellaCalabria/satosa-oidcop/workflows/satosa_oidcop/badge.svg)
-![Python version](https://img.shields.io/badge/license-Affero%203-blue.svg)
+[![CI build](https://github.com/UniversitaDellaCalabria/satosa-oidcop/workflows/satosa_oidcop/badge.svg)](https://github.com/UniversitaDellaCalabria/SATOSA-oidcop/actions)
+[![License](https://img.shields.io/pypi/l/satosa_oidcop)](./LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/satosa_oidcop)](https://pypi.org/project/satosa-oidcop/)
 [![Downloads](https://pepy.tech/badge/satosa-oidcop)](https://pepy.tech/project/satosa-oidcop)
 [![Downloads per week](https://pepy.tech/badge/satosa-oidcop/week)](https://pepy.tech/project/satosa-oidcop)
-![License](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.11-blue.svg)
+[![Python version](https://img.shields.io/pypi/pyversions/satosa_oidcop)](https://pypi.org/project/satosa-oidcop/)
 [![Conventional commits](https://img.shields.io/badge/semantic--release-conventional-e10079?logo=semantic-release)](https://conventionalcommits.org/)
 
-SATOSA Frontend based on [identity python oidcop](https://github.com/IdentityPython/oidc-op).
+SATOSA Frontend based on [idpyoidc by Identity Python](https://github.com/IdentityPython/idpy-oidc)
+(previously [identity python oidcop](https://github.com/IdentityPython/oidc-op)).
 
 ## Features
 
 Endpoints:
 
 - [x] provider discovery
 - [x] jwks uri
```

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop/core/application.py` & `satosa_oidcop-2.0.3/satosa_oidcop/core/application.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop/core/claims.py` & `satosa_oidcop-2.0.3/satosa_oidcop/core/claims.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop/core/storage/base.py` & `satosa_oidcop-2.0.3/satosa_oidcop/core/storage/base.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop/core/storage/mongo.py` & `satosa_oidcop-2.0.3/satosa_oidcop/core/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop/core/user_authn.py` & `satosa_oidcop-2.0.3/satosa_oidcop/core/user_authn.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop/core/user_info.py` & `satosa_oidcop-2.0.3/satosa_oidcop/core/user_info.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop/idpy_oidcop.py` & `satosa_oidcop-2.0.3/satosa_oidcop/idpy_oidcop.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop.egg-info/PKG-INFO` & `satosa_oidcop-2.0.3/satosa_oidcop.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosa-oidcop
-Version: 2.0.2
+Version: 2.0.3
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -15,22 +15,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SATOSA oidcop frontend
 
-![CI build](https://github.com/UniversitaDellaCalabria/satosa-oidcop/workflows/satosa_oidcop/badge.svg)
-![Python version](https://img.shields.io/badge/license-Affero%203-blue.svg)
+[![CI build](https://github.com/UniversitaDellaCalabria/satosa-oidcop/workflows/satosa_oidcop/badge.svg)](https://github.com/UniversitaDellaCalabria/SATOSA-oidcop/actions)
+[![License](https://img.shields.io/pypi/l/satosa_oidcop)](./LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/satosa_oidcop)](https://pypi.org/project/satosa-oidcop/)
 [![Downloads](https://pepy.tech/badge/satosa-oidcop)](https://pepy.tech/project/satosa-oidcop)
 [![Downloads per week](https://pepy.tech/badge/satosa-oidcop/week)](https://pepy.tech/project/satosa-oidcop)
-![License](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.11-blue.svg)
+[![Python version](https://img.shields.io/pypi/pyversions/satosa_oidcop)](https://pypi.org/project/satosa-oidcop/)
 [![Conventional commits](https://img.shields.io/badge/semantic--release-conventional-e10079?logo=semantic-release)](https://conventionalcommits.org/)
 
-SATOSA Frontend based on [identity python oidcop](https://github.com/IdentityPython/oidc-op).
+SATOSA Frontend based on [idpyoidc by Identity Python](https://github.com/IdentityPython/idpy-oidc)
+(previously [identity python oidcop](https://github.com/IdentityPython/oidc-op)).
 
 ## Features
 
 Endpoints:
 
 - [x] provider discovery
 - [x] jwks uri
```

### Comparing `satosa_oidcop-2.0.2/satosa_oidcop.egg-info/SOURCES.txt` & `satosa_oidcop-2.0.3/satosa_oidcop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.2/setup.py` & `satosa_oidcop-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,11 +34,11 @@
         f"{_pkg_name}": [
             i.replace(f"{_pkg_name}/", "")
             for i in glob(f"{_pkg_name}/**", recursive=True)
         ]
     },
     install_requires=[
         "satosa>=8.0.0",
-        "pymongo>=3.11,<=4.3",
+        "pymongo>=3.11,<5.0",
         "idpyoidc>=2.0.0,<=2.1.0",
     ],
 )
```

