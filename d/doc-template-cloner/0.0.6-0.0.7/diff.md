# Comparing `tmp/doc_template_cloner-0.0.6.tar.gz` & `tmp/doc_template_cloner-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-rztfnmpu/doc_template_cloner-0.0.6.tar", last modified: Fri Jul  7 11:27:21 2023, max compression
+gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-6mb5mzwz/doc_template_cloner-0.0.7.tar", last modified: Fri Jul  7 11:46:05 2023, max compression
```

## Comparing `doc_template_cloner-0.0.6.tar` & `doc_template_cloner-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:27:21.358814 doc_template_cloner-0.0.6/
--rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.6/LICENSE
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:27:21.358248 doc_template_cloner-0.0.6/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.6/README.md
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:27:21.355713 doc_template_cloner-0.0.6/doc_template_cloner/
--rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.6/doc_template_cloner/__init__.py
--rw-r--r--   0 ihor       (501) staff       (20)    16089 2023-07-07 11:27:01.000000 doc_template_cloner-0.0.6/doc_template_cloner/utils.py
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:27:21.357729 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/requires.txt
--rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/top_level.txt
--rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 11:27:21.358947 doc_template_cloner-0.0.6/setup.cfg
--rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 11:27:15.000000 doc_template_cloner-0.0.6/setup.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:46:05.057556 doc_template_cloner-0.0.7/
+-rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.7/LICENSE
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:46:05.057272 doc_template_cloner-0.0.7/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.7/README.md
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:46:05.054996 doc_template_cloner-0.0.7/doc_template_cloner/
+-rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.7/doc_template_cloner/__init__.py
+-rw-r--r--   0 ihor       (501) staff       (20)    16089 2023-07-07 11:27:01.000000 doc_template_cloner-0.0.7/doc_template_cloner/utils.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:46:05.056754 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/requires.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/top_level.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 11:46:05.057648 doc_template_cloner-0.0.7/setup.cfg
+-rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 11:45:59.000000 doc_template_cloner-0.0.7/setup.py
```

### Comparing `doc_template_cloner-0.0.6/LICENSE` & `doc_template_cloner-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_template_cloner-0.0.6/PKG-INFO` & `doc_template_cloner-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc_template_cloner
-Version: 0.0.6
+Version: 0.0.7
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.6/doc_template_cloner/utils.py` & `doc_template_cloner-0.0.7/doc_template_cloner/utils.py`

 * *Files identical despite different names*

### Comparing `doc_template_cloner-0.0.6/doc_template_cloner.egg-info/PKG-INFO` & `doc_template_cloner-0.0.7/doc_template_cloner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-template-cloner
-Version: 0.0.6
+Version: 0.0.7
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.6/setup.py` & `doc_template_cloner-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 required_packages = [
     #"boto3>=1.20.21,<2.0",
     "pandas",
 ]
 
 setup(
     name="doc_template_cloner",
-    version="0.0.6",
+    version="0.0.7",
     description="Custom lib to clone lebaling from one image to another similar",
     long_description_content_type="text/markdown",
     long_description=read('README.md'),
     packages=find_packages(),
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob("doc_template_cloner/*.py")],
     include_package_data=True,
     author="Ihor Bilyk",
```

