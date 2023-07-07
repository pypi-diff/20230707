# Comparing `tmp/langchain_ray-0.0.1.tar.gz` & `tmp/langchain_ray-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ray-0.0.1.tar", last modified: Fri Jul  7 04:14:10 2023, max compression
+gzip compressed data, was "langchain_ray-0.0.2.tar", last modified: Fri Jul  7 05:23:29 2023, max compression
```

## Comparing `langchain_ray-0.0.1.tar` & `langchain_ray-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 04:14:10.524098 langchain_ray-0.0.1/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 langchain_ray-0.0.1/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 langchain_ray-0.0.1/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-07 04:14:10.524098 langchain_ray-0.0.1/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      127 2023-07-07 03:48:51.000000 langchain_ray-0.0.1/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 04:14:10.520098 langchain_ray-0.0.1/langchain_ray/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-07-07 03:59:42.000000 langchain_ray-0.0.1/langchain_ray/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1092 2023-07-07 03:59:42.000000 langchain_ray-0.0.1/langchain_ray/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2154 2023-07-07 03:59:42.000000 langchain_ray-0.0.1/langchain_ray/chains.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      884 2023-07-07 03:42:39.000000 langchain_ray-0.0.1/langchain_ray/imports.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 04:14:10.524098 langchain_ray-0.0.1/langchain_ray.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-07 04:14:10.000000 langchain_ray-0.0.1/langchain_ray.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      411 2023-07-07 04:14:10.000000 langchain_ray-0.0.1/langchain_ray.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 04:14:10.000000 langchain_ray-0.0.1/langchain_ray.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       48 2023-07-07 04:14:10.000000 langchain_ray-0.0.1/langchain_ray.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 03:48:41.000000 langchain_ray-0.0.1/langchain_ray.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       47 2023-07-07 04:14:10.000000 langchain_ray-0.0.1/langchain_ray.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       14 2023-07-07 04:14:10.000000 langchain_ray-0.0.1/langchain_ray.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      723 2023-07-07 04:08:24.000000 langchain_ray-0.0.1/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-07-07 04:14:10.524098 langchain_ray-0.0.1/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 langchain_ray-0.0.1/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 langchain_ray-0.0.2/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 langchain_ray-0.0.2/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      127 2023-07-07 04:36:43.000000 langchain_ray-0.0.2/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.793174 langchain_ray-0.0.2/langchain_ray/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5525 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2153 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/chains.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      914 2023-07-07 04:23:18.000000 langchain_ray-0.0.2/langchain_ray/imports.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/langchain_ray/pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5342 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/pdf/chains.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     6175 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/pdf/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/langchain_ray.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      496 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       48 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 03:48:41.000000 langchain_ray-0.0.2/langchain_ray.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       47 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       14 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      722 2023-07-07 05:23:19.000000 langchain_ray-0.0.2/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 langchain_ray-0.0.2/setup.py
```

### Comparing `langchain_ray-0.0.1/LICENSE` & `langchain_ray-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ray-0.0.1/PKG-INFO` & `langchain_ray-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_ray
-Version: 0.0.1
+Version: 0.0.2
 Summary: LangChain leveraging Ray.
 Home-page: https://github.com/HamzaFarhan/langchain_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langchain_ray-0.0.1/langchain_ray/chains.py` & `langchain_ray-0.0.2/langchain_ray/chains.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,7 @@
         output_variables=output_variables,
         transform=tfm,
     )
 
 
 def noop_chain():
     return transform_chain(noop)
-
```

### Comparing `langchain_ray-0.0.1/langchain_ray/imports.py` & `langchain_ray-0.0.2/langchain_ray/imports.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dreamai.imports import *
 from dreamai.core import *
 
 import ray
 from ray import serve
 from ray import data as rd
 from transformers import pipeline
 from langchain.schema import Document
```

### Comparing `langchain_ray-0.0.1/langchain_ray.egg-info/PKG-INFO` & `langchain_ray-0.0.2/langchain_ray.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-ray
-Version: 0.0.1
+Version: 0.0.2
 Summary: LangChain leveraging Ray.
 Home-page: https://github.com/HamzaFarhan/langchain_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langchain_ray-0.0.1/settings.ini` & `langchain_ray-0.0.2/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [DEFAULT]
 repo = langchain_ray
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.8
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = langchain_ray
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 branch = main
-custom_sidebar = False
+custom_sidebar = True
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 audience = Developers
 author = Hamza Farhan
 author_email = thehamza96@gmail.com
```

### Comparing `langchain_ray-0.0.1/setup.py` & `langchain_ray-0.0.2/setup.py`

 * *Files identical despite different names*

