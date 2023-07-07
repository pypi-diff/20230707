# Comparing `tmp/compare_dfs-0.0.2.tar.gz` & `tmp/compare_dfs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compare_dfs-0.0.2.tar", last modified: Fri Jul  7 09:01:32 2023, max compression
+gzip compressed data, was "compare_dfs-0.0.3.tar", last modified: Fri Jul  7 09:03:49 2023, max compression
```

## Comparing `compare_dfs-0.0.2.tar` & `compare_dfs-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:01:32.685760 compare_dfs-0.0.2/
--rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.2/LICENSE
--rw-r--r--   0 rikka      (501) staff       (20)     1342 2023-07-07 09:01:32.685592 compare_dfs-0.0.2/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      916 2023-07-07 09:01:10.000000 compare_dfs-0.0.2/README.md
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:01:32.684517 compare_dfs-0.0.2/compare_dfs/
--rw-r--r--   0 rikka      (501) staff       (20)     2395 2023-07-07 08:44:18.000000 compare_dfs-0.0.2/compare_dfs/__init__.py
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:01:32.685403 compare_dfs-0.0.2/compare_dfs.egg-info/
--rw-r--r--   0 rikka      (501) staff       (20)     1342 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/SOURCES.txt
--rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/dependency_links.txt
--rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/top_level.txt
--rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-07 09:01:32.685812 compare_dfs-0.0.2/setup.cfg
--rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-07 09:01:18.000000 compare_dfs-0.0.2/setup.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:03:49.779730 compare_dfs-0.0.3/
+-rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.3/LICENSE
+-rw-r--r--   0 rikka      (501) staff       (20)     1402 2023-07-07 09:03:49.779574 compare_dfs-0.0.3/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)      976 2023-07-07 09:02:55.000000 compare_dfs-0.0.3/README.md
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:03:49.778755 compare_dfs-0.0.3/compare_dfs/
+-rw-r--r--   0 rikka      (501) staff       (20)     2395 2023-07-07 08:44:18.000000 compare_dfs-0.0.3/compare_dfs/__init__.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:03:49.779383 compare_dfs-0.0.3/compare_dfs.egg-info/
+-rw-r--r--   0 rikka      (501) staff       (20)     1402 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/SOURCES.txt
+-rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/dependency_links.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/top_level.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-07 09:03:49.779782 compare_dfs-0.0.3/setup.cfg
+-rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-07 09:03:43.000000 compare_dfs-0.0.3/setup.py
```

### Comparing `compare_dfs-0.0.2/LICENSE` & `compare_dfs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.2/PKG-INFO` & `compare_dfs-0.0.3/compare_dfs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: compare_dfs
-Version: 0.0.2
+Name: compare-dfs
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,19 +14,22 @@
 
 # compare_df
 ## 介绍
 找出两个几乎相同的DataFrame的差异
 
 ## 安装
 ```bash
-pip install compare_df
+pip install compare_dfs
 ```
 
 ## 使用
 ```python
+import pandas as pd
+import compare_dfs.compare as compare
+
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
                    
 df2 = pd.DataFrame({
```

### Comparing `compare_dfs-0.0.2/README.md` & `compare_dfs-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # compare_df
 ## 介绍
 找出两个几乎相同的DataFrame的差异
 
 ## 安装
 ```bash
-pip install compare_df
+pip install compare_dfs
 ```
 
 ## 使用
 ```python
+import pandas as pd
+import compare_dfs.compare as compare
+
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
                    
 df2 = pd.DataFrame({
```

### Comparing `compare_dfs-0.0.2/compare_dfs/__init__.py` & `compare_dfs-0.0.3/compare_dfs/__init__.py`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.2/compare_dfs.egg-info/PKG-INFO` & `compare_dfs-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: compare-dfs
-Version: 0.0.2
+Name: compare_dfs
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,19 +14,22 @@
 
 # compare_df
 ## 介绍
 找出两个几乎相同的DataFrame的差异
 
 ## 安装
 ```bash
-pip install compare_df
+pip install compare_dfs
 ```
 
 ## 使用
 ```python
+import pandas as pd
+import compare_dfs.compare as compare
+
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
                    
 df2 = pd.DataFrame({
```

### Comparing `compare_dfs-0.0.2/setup.py` & `compare_dfs-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="compare_dfs", # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

