# Comparing `tmp/snsphd-0.1.0.tar.gz` & `tmp/snsphd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snsphd-0.1.0.tar", max compression
+gzip compressed data, was "snsphd-0.1.1.tar", max compression
```

## Comparing `snsphd-0.1.0.tar` & `snsphd-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1102 2023-03-07 02:00:39.348518 snsphd-0.1.0/LICENSE
--rw-r--r--   0        0        0      606 2023-07-06 22:51:26.544064 snsphd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2922 2023-07-02 20:30:56.000000 snsphd-0.1.0/README.md
--rw-r--r--   0        0        0      306 2023-05-05 20:48:28.940066 snsphd-0.1.0/src/snsphd/__init__.py
--rw-r--r--   0        0        0    15740 2023-03-07 02:24:50.243662 snsphd-0.1.0/src/snsphd/clock.py
--rw-r--r--   0        0        0      408 2023-05-02 18:34:57.875684 snsphd-0.1.0/src/snsphd/help.py
--rw-r--r--   0        0        0     7280 2023-05-05 20:41:38.401450 snsphd-0.1.0/src/snsphd/hist.py
--rw-r--r--   0        0        0     2140 2023-05-05 20:55:55.151276 snsphd-0.1.0/src/snsphd/layout.py
--rw-r--r--   0        0        0     6136 2022-11-01 18:06:20.775888 snsphd-0.1.0/src/snsphd/obj.py
--rw-r--r--   0        0        0    18250 2023-06-20 22:53:32.157388 snsphd-0.1.0/src/snsphd/viz.py
--rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 snsphd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-03-07 02:00:39.348518 snsphd-0.1.1/LICENSE
+-rw-r--r--   0        0        0      606 2023-07-06 23:00:26.582696 snsphd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2968 2023-07-06 22:59:02.747851 snsphd-0.1.1/README.md
+-rw-r--r--   0        0        0      306 2023-05-05 20:48:28.940066 snsphd-0.1.1/src/snsphd/__init__.py
+-rw-r--r--   0        0        0    15740 2023-03-07 02:24:50.243662 snsphd-0.1.1/src/snsphd/clock.py
+-rw-r--r--   0        0        0      408 2023-05-02 18:34:57.875684 snsphd-0.1.1/src/snsphd/help.py
+-rw-r--r--   0        0        0     7280 2023-05-05 20:41:38.401450 snsphd-0.1.1/src/snsphd/hist.py
+-rw-r--r--   0        0        0     2140 2023-05-05 20:55:55.151276 snsphd-0.1.1/src/snsphd/layout.py
+-rw-r--r--   0        0        0     6136 2022-11-01 18:06:20.775888 snsphd-0.1.1/src/snsphd/obj.py
+-rw-r--r--   0        0        0    18250 2023-06-20 22:53:32.157388 snsphd-0.1.1/src/snsphd/viz.py
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 snsphd-0.1.1/PKG-INFO
```

### Comparing `snsphd-0.1.0/LICENSE` & `snsphd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snsphd-0.1.0/pyproject.toml` & `snsphd-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snsphd"
-version = "0.1.0"
+version = "0.1.1"
 description = "Utility and styling functions for A. Mueller's phd thesis"
 authors = ["Andrew Mueller <andrewstermueller@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/sansseriff/snsphd"
 repository = "https://github.com/sansseriff/snsphd"
```

### Comparing `snsphd-0.1.0/README.md` & `snsphd-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!-- ![SNSPHD](./snsphd.svg) -->
 
 <p align="center">
-  <img src="./snsphd.svg" alt="SNSPHD" width="400"/>
+  <img src="https://github.com/sansseriff/snsphd/raw/master/snsphd.svg" alt="SNSPHD" width="400"/>
 </p>
 
 
 This is a python package of utility and styling functions used for:
 
 <h3 style="text-align: center; color: lightblue;"><em>Optimization Techniques for Single Photon Detection and Quantum Optics</em></h3>
```

### Comparing `snsphd-0.1.0/src/snsphd/clock.py` & `snsphd-0.1.1/src/snsphd/clock.py`

 * *Files identical despite different names*

### Comparing `snsphd-0.1.0/src/snsphd/hist.py` & `snsphd-0.1.1/src/snsphd/hist.py`

 * *Files identical despite different names*

### Comparing `snsphd-0.1.0/src/snsphd/layout.py` & `snsphd-0.1.1/src/snsphd/layout.py`

 * *Files identical despite different names*

### Comparing `snsphd-0.1.0/src/snsphd/obj.py` & `snsphd-0.1.1/src/snsphd/obj.py`

 * *Files identical despite different names*

### Comparing `snsphd-0.1.0/src/snsphd/viz.py` & `snsphd-0.1.1/src/snsphd/viz.py`

 * *Files identical despite different names*

### Comparing `snsphd-0.1.0/PKG-INFO` & `snsphd-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snsphd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility and styling functions for A. Mueller's phd thesis
 Home-page: https://github.com/sansseriff/snsphd
 License: MIT
 Author: Andrew Mueller
 Author-email: andrewstermueller@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Project-URL: Repository, https://github.com/sansseriff/snsphd
 Description-Content-Type: text/markdown
 
 <!-- ![SNSPHD](./snsphd.svg) -->
 
 <p align="center">
-  <img src="./snsphd.svg" alt="SNSPHD" width="400"/>
+  <img src="https://github.com/sansseriff/snsphd/raw/master/snsphd.svg" alt="SNSPHD" width="400"/>
 </p>
 
 
 This is a python package of utility and styling functions used for:
 
 <h3 style="text-align: center; color: lightblue;"><em>Optimization Techniques for Single Photon Detection and Quantum Optics</em></h3>
```

