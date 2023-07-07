# Comparing `tmp/dpackage-0.0.2.tar.gz` & `tmp/dpackage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpackage-0.0.2.tar", last modified: Fri Jul  7 18:03:47 2023, max compression
+gzip compressed data, was "dpackage-0.0.3.tar", last modified: Fri Jul  7 18:18:44 2023, max compression
```

## Comparing `dpackage-0.0.2.tar` & `dpackage-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:03:47.895673 dpackage-0.0.2/
--rw-rw-rw-   0        0        0      446 2023-07-07 18:03:47.895673 dpackage-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 18:03:47.877728 dpackage-0.0.2/_distutils_hack/
-drwxrwxrwx   0        0        0        0 2023-07-07 18:03:47.891687 dpackage-0.0.2/_distutils_hack/dpackage.egg-info/
--rw-rw-rw-   0        0        0      446 2023-07-07 18:03:47.000000 dpackage-0.0.2/_distutils_hack/dpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-07 18:03:47.000000 dpackage-0.0.2/_distutils_hack/dpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:03:47.000000 dpackage-0.0.2/_distutils_hack/dpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:03:47.000000 dpackage-0.0.2/_distutils_hack/dpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 18:03:47.895673 dpackage-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-07-07 18:03:44.000000 dpackage-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:18:44.851408 dpackage-0.0.3/
+-rw-rw-rw-   0        0        0      443 2023-07-07 18:18:44.850413 dpackage-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 18:18:44.839441 dpackage-0.0.3/_distutils_hack/
+drwxrwxrwx   0        0        0        0 2023-07-07 18:18:44.847419 dpackage-0.0.3/_distutils_hack/dpackage.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-07-07 18:18:44.000000 dpackage-0.0.3/_distutils_hack/dpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-07 18:18:44.000000 dpackage-0.0.3/_distutils_hack/dpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:18:44.000000 dpackage-0.0.3/_distutils_hack/dpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:18:44.000000 dpackage-0.0.3/_distutils_hack/dpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 18:18:44.852406 dpackage-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-07-07 18:18:34.000000 dpackage-0.0.3/setup.py
```

### Comparing `dpackage-0.0.2/setup.py` & `dpackage-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 
 setup(
     name="dpackage",
-    version="0.0.2",
+    version="0.0.3",
     description="test",
     package_dir={"": "_distutils_hack"},
     packages=find_packages(where="_distutils_hack"),
     long_description='sad',
     long_description_content_type="text/markdown",
-    url="https://github.com/ArjanCodes/2023-package",
+    url="https://github.com/ddjango786/-dpackage",
     author="DDjango",
     author_email="ddjango.786@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
```

