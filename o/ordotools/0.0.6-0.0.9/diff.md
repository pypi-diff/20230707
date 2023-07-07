# Comparing `tmp/ordotools-0.0.6.tar.gz` & `tmp/ordotools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ordotools-0.0.6.tar", last modified: Fri Jul  7 19:37:28 2023, max compression
+gzip compressed data, was "ordotools-0.0.9.tar", last modified: Fri Jul  7 20:03:20 2023, max compression
```

## Comparing `ordotools-0.0.6.tar` & `ordotools-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 19:37:28.179049 ordotools-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-07 19:37:17.000000 ordotools-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/ordotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/sanctoral/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/sanctoral/country/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/country/australiae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/country/nameofcountry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/ordotools/sanctoral/diocese/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/bathurstensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/lismorensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/maitlandensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/melbournensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/nameofdiocese.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/rockhamptonensis.py
--rw-r--r--   0 runner    (1001) docker     (123)   193907 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/roman.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/ordotools/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/OLD_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    93647 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/feast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/liturgical_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/parts.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 19:37:17.000000 ordotools-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:37:28.179049 ordotools-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-07 19:37:17.000000 ordotools-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-07 19:37:17.000000 ordotools-0.0.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:20.761436 ordotools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 20:03:20.761436 ordotools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-07 20:03:11.000000 ordotools-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:20.757436 ordotools-0.0.9/ordotools/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 20:03:11.000000 ordotools-0.0.9/ordotools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:20.757436 ordotools-0.0.9/ordotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 20:03:20.000000 ordotools-0.0.9/ordotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 20:03:20.000000 ordotools-0.0.9/ordotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:03:20.000000 ordotools-0.0.9/ordotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 20:03:20.000000 ordotools-0.0.9/ordotools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 20:03:20.000000 ordotools-0.0.9/ordotools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 20:03:11.000000 ordotools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:03:20.761436 ordotools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-07 20:03:11.000000 ordotools-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:03:20.761436 ordotools-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 20:03:11.000000 ordotools-0.0.9/tests/test_.py
```

### Comparing `ordotools-0.0.6/PKG-INFO` & `ordotools-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ordotools
-Version: 0.0.6
+Version: 0.0.9
 Summary: A set of tools for producing a traditional Catholic Ordo, given a year and diocese
 Home-page: https://github.com/corei8/ordotools
 Author: corei8 (Fr. G.R.Barnes)
 Author-email: corei8.github@gmail.com
 License: GNU
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `ordotools-0.0.6/README.md` & `ordotools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.6/ordotools/ordotools.egg-info/PKG-INFO` & `ordotools-0.0.9/ordotools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ordotools
-Version: 0.0.6
+Version: 0.0.9
 Summary: A set of tools for producing a traditional Catholic Ordo, given a year and diocese
 Home-page: https://github.com/corei8/ordotools
 Author: corei8 (Fr. G.R.Barnes)
 Author-email: corei8.github@gmail.com
 License: GNU
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `ordotools-0.0.6/setup.py` & `ordotools-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ordotools",
-    version="0.0.6",
+    version="0.0.9",
     description="A set of tools for producing a traditional Catholic Ordo, given a year and diocese",
-    package_dir={"": "ordotools"},
-    packages=find_packages(where="ordotools"),
+    # package_dir={"": "ordotools"},
+    # packages=find_packages(where="ordotools"),
+    packages=["ordotools"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/corei8/ordotools",
     author="corei8 (Fr. G.R.Barnes)",
     author_email="corei8.github@gmail.com",
     license="GNU",
     classifiers=[
```

