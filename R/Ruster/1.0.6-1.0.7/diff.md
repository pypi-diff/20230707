# Comparing `tmp/Ruster-1.0.6.tar.gz` & `tmp/Ruster-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-1.0.6.tar", last modified: Thu Jul  6 20:33:43 2023, max compression
+gzip compressed data, was "Ruster-1.0.7.tar", last modified: Fri Jul  7 17:21:21 2023, max compression
```

## Comparing `Ruster-1.0.6.tar` & `Ruster-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 20:33:43.586496 Ruster-1.0.6/
--rw-rw-rw-   0        0        0      904 2023-07-06 20:33:43.582504 Ruster-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 20:33:43.533462 Ruster-1.0.6/Ruster/
--rw-rw-rw-   0        0        0      118 2023-07-06 20:33:19.000000 Ruster-1.0.6/Ruster/__init__.py
--rw-rw-rw-   0        0        0    13107 2023-07-06 20:18:13.000000 Ruster-1.0.6/Ruster/app.py
--rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.6/Ruster/blueprints.py
--rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.6/Ruster/exceptions.py
--rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.6/Ruster/hasher.py
--rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.6/Ruster/jwt.py
--rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.6/Ruster/limiter.py
--rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.6/Ruster/mailer.py
--rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.6/Ruster/sanitizer.py
--rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.6/Ruster/session.py
--rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.6/Ruster/wtf.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:33:43.579183 Ruster-1.0.6/Ruster.egg-info/
--rw-rw-rw-   0        0        0      904 2023-07-06 20:33:43.000000 Ruster-1.0.6/Ruster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-06 20:33:43.000000 Ruster-1.0.6/Ruster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 20:33:43.000000 Ruster-1.0.6/Ruster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-06 20:33:43.000000 Ruster-1.0.6/Ruster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-07-06 20:33:43.000000 Ruster-1.0.6/Ruster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 20:33:43.000000 Ruster-1.0.6/Ruster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 20:33:43.587496 Ruster-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-07-06 20:33:33.000000 Ruster-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:21:21.302455 Ruster-1.0.7/
+-rw-rw-rw-   0        0        0      904 2023-07-07 17:21:21.302455 Ruster-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 17:21:21.128911 Ruster-1.0.7/Ruster/
+-rw-rw-rw-   0        0        0      122 2023-07-07 17:17:23.000000 Ruster-1.0.7/Ruster/__init__.py
+-rw-rw-rw-   0        0        0    13107 2023-07-06 20:18:13.000000 Ruster-1.0.7/Ruster/app.py
+-rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.7/Ruster/blueprints.py
+-rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.7/Ruster/exceptions.py
+-rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.7/Ruster/hasher.py
+-rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.7/Ruster/jwt.py
+-rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.7/Ruster/limiter.py
+-rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.7/Ruster/mailer.py
+-rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.7/Ruster/sanitizer.py
+-rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.7/Ruster/session.py
+-rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.7/Ruster/wtf.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:21:21.294438 Ruster-1.0.7/Ruster.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:21:21.302455 Ruster-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-07-07 17:21:10.000000 Ruster-1.0.7/setup.py
```

### Comparing `Ruster-1.0.6/PKG-INFO` & `Ruster-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.6
+Version: 1.0.7
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.6/Ruster/app.py` & `Ruster-1.0.7/Ruster/app.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/blueprints.py` & `Ruster-1.0.7/Ruster/blueprints.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/hasher.py` & `Ruster-1.0.7/Ruster/hasher.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/jwt.py` & `Ruster-1.0.7/Ruster/jwt.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/limiter.py` & `Ruster-1.0.7/Ruster/limiter.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/mailer.py` & `Ruster-1.0.7/Ruster/mailer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/sanitizer.py` & `Ruster-1.0.7/Ruster/sanitizer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/session.py` & `Ruster-1.0.7/Ruster/session.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster/wtf.py` & `Ruster-1.0.7/Ruster/wtf.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.6/Ruster.egg-info/PKG-INFO` & `Ruster-1.0.7/Ruster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.6
+Version: 1.0.7
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.6/setup.py` & `Ruster-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Ruster",
-    version="1.0.6",
+    version="1.0.7",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/ruster",
     packages=find_packages(),
-    py_modules=['Ruster'],
+    py_modules=['ruster'],
     install_requires=[
         "itsdangerous",
         "werkzeug",
         "PyJWT",
         "cryptography",
         "jinja2",
         "uuid",
```

