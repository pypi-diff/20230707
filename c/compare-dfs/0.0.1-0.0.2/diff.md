# Comparing `tmp/compare_dfs-0.0.1.tar.gz` & `tmp/compare_dfs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compare_dfs-0.0.1.tar", last modified: Fri Jul  7 08:59:47 2023, max compression
+gzip compressed data, was "compare_dfs-0.0.2.tar", last modified: Fri Jul  7 09:01:32 2023, max compression
```

## Comparing `compare_dfs-0.0.1.tar` & `compare_dfs-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 08:59:47.673330 compare_dfs-0.0.1/
--rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.1/LICENSE
--rw-r--r--   0 rikka      (501) staff       (20)     1333 2023-07-07 08:59:47.673156 compare_dfs-0.0.1/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      907 2023-07-07 08:45:43.000000 compare_dfs-0.0.1/README.md
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 08:59:47.672255 compare_dfs-0.0.1/compare_dfs/
--rw-r--r--   0 rikka      (501) staff       (20)     2395 2023-07-07 08:44:18.000000 compare_dfs-0.0.1/compare_dfs/__init__.py
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 08:59:47.672953 compare_dfs-0.0.1/compare_dfs.egg-info/
--rw-r--r--   0 rikka      (501) staff       (20)     1333 2023-07-07 08:59:47.000000 compare_dfs-0.0.1/compare_dfs.egg-info/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-07 08:59:47.000000 compare_dfs-0.0.1/compare_dfs.egg-info/SOURCES.txt
--rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-07 08:59:47.000000 compare_dfs-0.0.1/compare_dfs.egg-info/dependency_links.txt
--rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-07 08:59:47.000000 compare_dfs-0.0.1/compare_dfs.egg-info/top_level.txt
--rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-07 08:59:47.673384 compare_dfs-0.0.1/setup.cfg
--rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-07 08:59:04.000000 compare_dfs-0.0.1/setup.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:01:32.685760 compare_dfs-0.0.2/
+-rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.2/LICENSE
+-rw-r--r--   0 rikka      (501) staff       (20)     1342 2023-07-07 09:01:32.685592 compare_dfs-0.0.2/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)      916 2023-07-07 09:01:10.000000 compare_dfs-0.0.2/README.md
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:01:32.684517 compare_dfs-0.0.2/compare_dfs/
+-rw-r--r--   0 rikka      (501) staff       (20)     2395 2023-07-07 08:44:18.000000 compare_dfs-0.0.2/compare_dfs/__init__.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:01:32.685403 compare_dfs-0.0.2/compare_dfs.egg-info/
+-rw-r--r--   0 rikka      (501) staff       (20)     1342 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/SOURCES.txt
+-rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/dependency_links.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-07 09:01:32.000000 compare_dfs-0.0.2/compare_dfs.egg-info/top_level.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-07 09:01:32.685812 compare_dfs-0.0.2/setup.cfg
+-rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-07 09:01:18.000000 compare_dfs-0.0.2/setup.py
```

### Comparing `compare_dfs-0.0.1/LICENSE` & `compare_dfs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.1/PKG-INFO` & `compare_dfs-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: compare_dfs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # compare_df
 ## 介绍
-找出两个几乎DataFrame的差异
+找出两个几乎相同的DataFrame的差异
 
 ## 安装
 ```bash
 pip install compare_df
 ```
 
 ## 使用
```

### Comparing `compare_dfs-0.0.1/README.md` & `compare_dfs-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # compare_df
 ## 介绍
-找出两个几乎DataFrame的差异
+找出两个几乎相同的DataFrame的差异
 
 ## 安装
 ```bash
 pip install compare_df
 ```
 
 ## 使用
```

### Comparing `compare_dfs-0.0.1/compare_dfs/__init__.py` & `compare_dfs-0.0.2/compare_dfs/__init__.py`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.1/compare_dfs.egg-info/PKG-INFO` & `compare_dfs-0.0.2/compare_dfs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: compare-dfs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # compare_df
 ## 介绍
-找出两个几乎DataFrame的差异
+找出两个几乎相同的DataFrame的差异
 
 ## 安装
 ```bash
 pip install compare_df
 ```
 
 ## 使用
```

### Comparing `compare_dfs-0.0.1/setup.py` & `compare_dfs-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="compare_dfs", # Replace with your own username
-    version="0.0.1",
+    version="0.0.2",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

