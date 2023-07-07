# Comparing `tmp/py-datalab-0.2.1.tar.gz` & `tmp/py-datalab-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.2.1.tar", last modified: Fri Jul  7 17:01:46 2023, max compression
+gzip compressed data, was "py-datalab-0.2.2.tar", last modified: Fri Jul  7 17:09:24 2023, max compression
```

## Comparing `py-datalab-0.2.1.tar` & `py-datalab-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:01:46.903205 py-datalab-0.2.1/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      802 2023-07-07 17:01:46.902205 py-datalab-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2860 2023-07-07 04:02:41.000000 py-datalab-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 17:01:46.880656 py-datalab-0.2.1/datalab/
--rw-rw-rw-   0        0        0    20812 2023-07-07 16:49:22.000000 py-datalab-0.2.1/datalab/Matrix.py
--rw-rw-rw-   0        0        0    12648 2023-07-07 15:11:17.000000 py-datalab-0.2.1/datalab/Vector.py
--rw-rw-rw-   0        0        0      196 2023-07-07 16:54:19.000000 py-datalab-0.2.1/datalab/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-07-07 16:59:02.000000 py-datalab-0.2.1/datalab/functions.py
--rw-rw-rw-   0        0        0     2110 2023-07-07 15:05:10.000000 py-datalab-0.2.1/datalab/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:01:46.900202 py-datalab-0.2.1/py_datalab.egg-info/
--rw-rw-rw-   0        0        0      802 2023-07-07 17:01:46.000000 py-datalab-0.2.1/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-07-07 17:01:46.000000 py-datalab-0.2.1/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:01:46.000000 py-datalab-0.2.1/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-07 17:01:46.000000 py-datalab-0.2.1/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:01:46.903205 py-datalab-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-07-07 17:00:42.000000 py-datalab-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:09:24.693171 py-datalab-0.2.2/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      802 2023-07-07 17:09:24.693171 py-datalab-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2860 2023-07-07 04:02:41.000000 py-datalab-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 17:09:24.669239 py-datalab-0.2.2/datalab/
+-rw-rw-rw-   0        0        0    20812 2023-07-07 16:49:22.000000 py-datalab-0.2.2/datalab/Matrix.py
+-rw-rw-rw-   0        0        0    12648 2023-07-07 15:11:17.000000 py-datalab-0.2.2/datalab/Vector.py
+-rw-rw-rw-   0        0        0      204 2023-07-07 17:04:55.000000 py-datalab-0.2.2/datalab/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-07-07 16:59:02.000000 py-datalab-0.2.2/datalab/functions.py
+-rw-rw-rw-   0        0        0     2110 2023-07-07 15:05:10.000000 py-datalab-0.2.2/datalab/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:09:24.691170 py-datalab-0.2.2/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0      802 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 17:09:24.000000 py-datalab-0.2.2/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:09:24.694169 py-datalab-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2023-07-07 17:09:20.000000 py-datalab-0.2.2/setup.py
```

### Comparing `py-datalab-0.2.1/LICENSE` & `py-datalab-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.1/PKG-INFO` & `py-datalab-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.2.1
+Version: 0.2.2
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.2.1/README.md` & `py-datalab-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.1/datalab/Matrix.py` & `py-datalab-0.2.2/datalab/Matrix.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.1/datalab/Vector.py` & `py-datalab-0.2.2/datalab/Vector.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.1/datalab/functions.py` & `py-datalab-0.2.2/datalab/functions.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.1/datalab/utils.py` & `py-datalab-0.2.2/datalab/utils.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.1/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.2.2/py_datalab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.2.1
+Version: 0.2.2
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.2.1/setup.py` & `py-datalab-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 10):
     sys.exit("Sorry, Python < 3.10 is not supported")
 
 setup(
     name="py-datalab",
-    version="0.2.1",
+    version="0.2.2",
     author="Mateusz Nowak",
     author_email="mateusz.nowak.pol@gmail.com",
     description="This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.",
     url="https://github.com/matuszen/Python-DataLab",
     packages=find_packages(),
+    install_requires=[
+        "typing_extensions",
+    ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
```

