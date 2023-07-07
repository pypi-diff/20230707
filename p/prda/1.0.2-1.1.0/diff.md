# Comparing `tmp/prda-1.0.2.tar.gz` & `tmp/prda-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prda-1.0.2.tar", last modified: Mon May 22 08:06:29 2023, max compression
+gzip compressed data, was "prda-1.1.0.tar", last modified: Fri Jul  7 06:45:47 2023, max compression
```

## Comparing `prda-1.0.2.tar` & `prda-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-22 08:06:29.237162 prda-1.0.2/
--rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.0.2/LICENSE
--rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-22 08:06:29.236989 prda-1.0.2/PKG-INFO
--rw-r--r--   0 minshaojie   (501) staff       (20)     2769 2023-05-07 14:06:10.000000 prda-1.0.2/README.md
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-22 08:06:29.235759 prda-1.0.2/prda/
--rw-r--r--   0 minshaojie   (501) staff       (20)      108 2022-12-18 07:50:04.000000 prda-1.0.2/prda/__init__.py
--rw-r--r--   0 minshaojie   (501) staff       (20)    12932 2023-05-16 06:36:16.000000 prda-1.0.2/prda/graphic.py
--rw-r--r--   0 minshaojie   (501) staff       (20)      856 2023-05-05 07:16:05.000000 prda-1.0.2/prda/iostream.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     7314 2023-05-03 13:03:18.000000 prda-1.0.2/prda/ml.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     8779 2023-05-03 07:16:35.000000 prda-1.0.2/prda/prep.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     3389 2022-12-03 12:39:17.000000 prda-1.0.2/prda/utility.py
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-22 08:06:29.236718 prda-1.0.2/prda.egg-info/
--rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/PKG-INFO
--rw-r--r--   0 minshaojie   (501) staff       (20)      255 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/SOURCES.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/dependency_links.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/requires.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        5 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/top_level.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-05-22 08:06:29.237210 prda-1.0.2/setup.cfg
--rw-r--r--   0 minshaojie   (501) staff       (20)      901 2023-05-22 07:56:02.000000 prda-1.0.2/setup.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.235671 prda-1.1.0/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.1.0/LICENSE
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-07-07 06:45:47.235510 prda-1.1.0/PKG-INFO
+-rw-r--r--   0 minshaojie   (501) staff       (20)     2713 2023-06-30 05:36:38.000000 prda-1.1.0/README.md
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.234207 prda-1.1.0/prda/
+-rw-r--r--   0 minshaojie   (501) staff       (20)      107 2023-07-07 03:33:54.000000 prda-1.1.0/prda/__init__.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)    12932 2023-05-16 06:36:16.000000 prda-1.1.0/prda/graphic.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)      856 2023-05-05 07:16:05.000000 prda-1.1.0/prda/iostream.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.235299 prda-1.1.0/prda/ml/
+-rw-r--r--   0 minshaojie   (501) staff       (20)       61 2023-07-07 03:02:46.000000 prda-1.1.0/prda/ml/__init__.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     3460 2023-07-07 03:02:12.000000 prda-1.1.0/prda/ml/clusters.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     5470 2023-07-07 03:09:34.000000 prda-1.1.0/prda/ml/evaluations.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     5506 2023-07-07 04:11:25.000000 prda-1.1.0/prda/ml/neighbors.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     8809 2023-07-07 03:12:15.000000 prda-1.1.0/prda/prep.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     3389 2022-12-03 12:39:17.000000 prda-1.1.0/prda/utility.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.234796 prda-1.1.0/prda.egg-info/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/PKG-INFO
+-rw-r--r--   0 minshaojie   (501) staff       (20)      328 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/SOURCES.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/dependency_links.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/requires.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        5 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/top_level.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-07-07 06:45:47.235719 prda-1.1.0/setup.cfg
+-rw-r--r--   0 minshaojie   (501) staff       (20)      901 2023-07-07 06:45:43.000000 prda-1.1.0/setup.py
```

### Comparing `prda-1.0.2/LICENSE` & `prda-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prda-1.0.2/PKG-INFO` & `prda-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prda
-Version: 1.0.2
+Version: 1.1.0
 Summary: Prda contains packages for data processing, analysis and visualization. The ultimate goal is to fill the “last mile” between analysts and packages.
 Home-page: https://github.com/4AlexMin/prda
 Author: Shaojie Min
 Author-email: alexmin@cqu.edu.cn
 License: MIT License
         
         Copyright (c) 2021 Shaojie Min
```

### Comparing `prda-1.0.2/README.md` & `prda-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## How to Use
 ```
 pip install prda
 ```
 
 See details in: https://pypi.org/project/prda/
 
-You are welcome to clone *prda* for personal use (**to use, simply add the folder to your system path**) and **pull request** of your modification is super!! encouraged.
+You are welcome to clone *prda* for personal use and **pull request** of your modification is super!! encouraged.
 
 ----
 
 
 ~~To utilize prda, you only need to be familiar with `pandas` as most inputs is `pd.DataFrame`.~~
 
 Currently with the help of **ChatGPT**, you can just tailor the input of demonstration code below to your data. And you don't need to be familiar with pandas or even python.
```

### Comparing `prda-1.0.2/prda/graphic.py` & `prda-1.1.0/prda/graphic.py`

 * *Files identical despite different names*

### Comparing `prda-1.0.2/prda/iostream.py` & `prda-1.1.0/prda/iostream.py`

 * *Files identical despite different names*

### Comparing `prda-1.0.2/prda/prep.py` & `prda-1.1.0/prda/prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
         X_std = (X - X.min) / (X.max - X.min)
         X_scaled = X_std * (max_ - min_) + min_
 
     Parameters
     ----------
     data : numpy.ndarray
+    ndarray as original shape
     """
     data = np.asarray(data)
     datalen = 1
     for i in data.shape:
         if i != 0:
             datalen = datalen * i
     scaler = preprocessing.MinMaxScaler(feature_range=(min_, max_))
```

### Comparing `prda-1.0.2/prda/utility.py` & `prda-1.1.0/prda/utility.py`

 * *Files identical despite different names*

### Comparing `prda-1.0.2/prda.egg-info/PKG-INFO` & `prda-1.1.0/prda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prda
-Version: 1.0.2
+Version: 1.1.0
 Summary: Prda contains packages for data processing, analysis and visualization. The ultimate goal is to fill the “last mile” between analysts and packages.
 Home-page: https://github.com/4AlexMin/prda
 Author: Shaojie Min
 Author-email: alexmin@cqu.edu.cn
 License: MIT License
         
         Copyright (c) 2021 Shaojie Min
```

### Comparing `prda-1.0.2/setup.py` & `prda-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('LICENSE', 'r') as f:
     license = f.read()
 
 
 setup(
     name='prda',
-    version='1.0.2',
+    version='1.1.0',
     author='Shaojie Min',
     author_email='alexmin@cqu.edu.cn',
     description='Prda contains packages for data processing, analysis and visualization. The ultimate goal is to fill the “last mile” between analysts and packages.',
     url='https://github.com/4AlexMin/prda',
     license=license,
     packages=find_packages(),
     install_requires=[
```

