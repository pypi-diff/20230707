# Comparing `tmp/py-datalab-0.1.9.tar.gz` & `tmp/py-datalab-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.1.9.tar", last modified: Thu Jul  6 12:22:59 2023, max compression
+gzip compressed data, was "py-datalab-0.2.0.tar", last modified: Fri Jul  7 15:29:09 2023, max compression
```

## Comparing `py-datalab-0.1.9.tar` & `py-datalab-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:22:59.882412 py-datalab-0.1.9/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     1006 2023-07-06 12:22:59.881411 py-datalab-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:22:59.867869 py-datalab-0.1.9/datalab/
--rw-rw-rw-   0        0        0    10355 2023-07-06 12:22:56.000000 py-datalab-0.1.9/datalab/Matrix.py
--rw-rw-rw-   0        0        0     7061 2023-07-06 12:22:50.000000 py-datalab-0.1.9/datalab/Vector.py
--rw-rw-rw-   0        0        0       56 2023-07-06 12:16:58.000000 py-datalab-0.1.9/datalab/__init__.py
--rw-rw-rw-   0        0        0     4231 2023-07-06 12:02:49.000000 py-datalab-0.1.9/datalab/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:22:59.880414 py-datalab-0.1.9/py_datalab.egg-info/
--rw-rw-rw-   0        0        0     1006 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 12:22:59.882412 py-datalab-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-06 12:21:56.000000 py-datalab-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:29:09.704870 py-datalab-0.2.0/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      802 2023-07-07 15:29:09.704870 py-datalab-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2860 2023-07-07 04:02:41.000000 py-datalab-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 15:29:09.691357 py-datalab-0.2.0/datalab/
+-rw-rw-rw-   0        0        0    20789 2023-07-07 15:26:32.000000 py-datalab-0.2.0/datalab/Matrix.py
+-rw-rw-rw-   0        0        0    12648 2023-07-07 15:11:17.000000 py-datalab-0.2.0/datalab/Vector.py
+-rw-rw-rw-   0        0        0       70 2023-07-06 13:53:44.000000 py-datalab-0.2.0/datalab/__init__.py
+-rw-rw-rw-   0        0        0     2110 2023-07-07 15:05:10.000000 py-datalab-0.2.0/datalab/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:29:09.703872 py-datalab-0.2.0/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0      802 2023-07-07 15:29:09.000000 py-datalab-0.2.0/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-07 15:29:09.000000 py-datalab-0.2.0/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:29:09.000000 py-datalab-0.2.0/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 15:29:09.000000 py-datalab-0.2.0/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:29:09.704870 py-datalab-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-07-07 15:29:05.000000 py-datalab-0.2.0/setup.py
```

### Comparing `py-datalab-0.1.9/LICENSE` & `py-datalab-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.9/PKG-INFO` & `py-datalab-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.9
+Version: 0.2.0
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `py-datalab-0.1.9/README.md` & `py-datalab-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,96 @@
-# Python DataLab
+# py-datalab
 
 This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 
 ## Prerequisites
 
 Before running this script, make sure you have the following requirements fulfilled:
 
-- Python 3.6 or higher
+- Python 3.10 or higher
 
 ## Installation
 
-Clone or download the repository to your local machine:
+To work in your python project you only need to install it via pip:
+
+```shell
+pip install py-datalab
+```
+
+Or, to work on repository on your local machine:
 
 ```shell
 git clone https://github.com/matuszen/Python-DataLab.git
 ```
 
-You don't need to install any other python packages.
+Depend on your python version you need to install typing_extensions package
 
 ## Usage
 
 The Matrix class represents a matrix and provides various operations and methods to work with matrices. Here are the main features of the Matrix class:
 
+### Import
+
+```python
+import datalab as dl
+```
+
 ### Initialization
 
 To create a new matrix, you need to provide the shape (number of rows and columns) and an optional data type. The default data type is int. Here's an example of creating a matrix:
 
 ```python
-matrix = Matrix(shape=(3, 3), dtype=int)
-vector = Vector(size=4, dtype=float)
+matrix = dl.Matrix(3, 3, dtype=int)
+matrix = dl.Matrix((3, 3), dtype=int)
+matrix = dl.Matrix([[1, 2, 3], [5, 3], [2, 5, 3]])
+# Lib validates shape correctly, regardless of the size of the all lists
+
+vector = dl.Vector(4, dtype=float)
+vector = dl.Vector([1, 2, 3, 4, 5])
 ```
 
 ### Setting and Getting Elements
 
 You can set and get individual elements of the matrix using the square bracket notation. The indices are zero-based.
 
 ```python
 # Set an element
+matrix[0][0] = 1
 matrix[0, 0] = 1
+
 vector[1] = 3.0
 
 # Get an element
+element = matrix[0][0]
 element = matrix[0, 0]
+
 element = vector[1]
 ```
 
 ### Changing Data Type
 
 You can change the data type of the matrix using the change_dtype method. The new data type must be one of the supported types: int, float, str, or bool.
 
 ```python
 matrix.change_dtype(bool)
-vactor.change_dtype(int)
+vector.change_dtype(int)
 
 # Or make it via property
 matrix.dtype = bool
 vector.dtype = int
 ```
 
 ### Change size, and reshaping
 
 You can change the shape of the matrix using the reshape method. It takes a tuple (rows, columns) as the new shape.
 
 ```python
 matrix.reshape((2, 4))
+matrix.reshape(2, 4)
+
 vector.size = 5
 
 # You can also modify shape using `rows`, `columns` and `size` property
 matrix.columns += 1
 matrix.rows += 1
 
 vector.size -= 2
```

### Comparing `py-datalab-0.1.9/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.2.0/py_datalab.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.9
+Version: 0.2.0
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

