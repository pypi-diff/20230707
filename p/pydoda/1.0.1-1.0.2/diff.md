# Comparing `tmp/pydoda-1.0.1.tar.gz` & `tmp/pydoda-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoda-1.0.1.tar", last modified: Fri Jul  7 20:47:04 2023, max compression
+gzip compressed data, was "pydoda-1.0.2.tar", last modified: Fri Jul  7 21:41:32 2023, max compression
```

## Comparing `pydoda-1.0.1.tar` & `pydoda-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 20:47:04.977097 pydoda-1.0.1/
--rw-rw-r--   0 saad      (1000) saad      (1000)     2572 2023-07-07 12:52:32.000000 pydoda-1.0.1/LICENSE
--rw-rw-r--   0 saad      (1000) saad      (1000)     5651 2023-07-07 20:47:04.977097 pydoda-1.0.1/PKG-INFO
--rw-rw-r--   0 saad      (1000) saad      (1000)     4742 2023-07-07 12:52:53.000000 pydoda-1.0.1/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 20:47:04.973097 pydoda-1.0.1/pydoda/
--rw-rw-r--   0 saad      (1000) saad      (1000)      795 2023-06-26 22:43:54.000000 pydoda-1.0.1/pydoda/__init__.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     4719 2023-06-26 12:14:41.000000 pydoda-1.0.1/pydoda/category.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     4014 2023-06-26 23:18:19.000000 pydoda-1.0.1/pydoda/custom_category.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 20:47:04.973097 pydoda-1.0.1/pydoda/dataset/
--rw-rw-r--   0 saad      (1000) saad      (1000)     1235 2023-06-26 11:43:35.000000 pydoda-1.0.1/pydoda/dataset/LICENSE
--rw-rw-r--   0 saad      (1000) saad      (1000)     3877 2023-06-26 11:43:35.000000 pydoda-1.0.1/pydoda/dataset/README.md
--rw-rw-r--   0 saad      (1000) saad      (1000)    49090 2023-06-26 11:43:35.000000 pydoda-1.0.1/pydoda/dataset/imagenet_b_darija.csv
--rw-rw-r--   0 saad      (1000) saad      (1000)      460 2023-06-26 11:43:35.000000 pydoda-1.0.1/pydoda/dataset/progress.py
--rw-rw-r--   0 saad      (1000) saad      (1000)   589131 2023-06-26 11:43:35.000000 pydoda-1.0.1/pydoda/dataset/sentences.csv
--rw-rw-r--   0 saad      (1000) saad      (1000)     3786 2023-06-26 23:07:25.000000 pydoda-1.0.1/pydoda/loader.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     2772 2023-06-26 23:45:18.000000 pydoda-1.0.1/pydoda/py_doda.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     3497 2023-06-26 22:45:08.000000 pydoda-1.0.1/pydoda/sentence.py
--rw-rw-r--   0 saad      (1000) saad      (1000)      278 2023-06-27 12:10:29.000000 pydoda-1.0.1/pydoda/utils.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 20:47:04.973097 pydoda-1.0.1/pydoda.egg-info/
--rw-rw-r--   0 saad      (1000) saad      (1000)     5651 2023-07-07 20:47:04.000000 pydoda-1.0.1/pydoda.egg-info/PKG-INFO
--rw-rw-r--   0 saad      (1000) saad      (1000)      513 2023-07-07 20:47:04.000000 pydoda-1.0.1/pydoda.egg-info/SOURCES.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-07 20:47:04.000000 pydoda-1.0.1/pydoda.egg-info/dependency_links.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)        7 2023-07-07 20:47:04.000000 pydoda-1.0.1/pydoda.egg-info/requires.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       13 2023-07-07 20:47:04.000000 pydoda-1.0.1/pydoda.egg-info/top_level.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-07 20:47:04.977097 pydoda-1.0.1/setup.cfg
--rw-rw-r--   0 saad      (1000) saad      (1000)     1221 2023-07-07 20:46:48.000000 pydoda-1.0.1/setup.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 20:47:04.977097 pydoda-1.0.1/tests/
--rw-rw-r--   0 saad      (1000) saad      (1000)        0 2023-06-27 12:10:35.000000 pydoda-1.0.1/tests/__init__.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     4646 2023-06-27 12:10:35.000000 pydoda-1.0.1/tests/test_category.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     2555 2023-06-27 12:10:35.000000 pydoda-1.0.1/tests/test_py_doda.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.496249 pydoda-1.0.2/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2572 2023-07-07 12:52:32.000000 pydoda-1.0.2/LICENSE
+-rw-rw-r--   0 saad      (1000) saad      (1000)     5809 2023-07-07 21:41:32.496249 pydoda-1.0.2/PKG-INFO
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4900 2023-07-07 21:39:16.000000 pydoda-1.0.2/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.492249 pydoda-1.0.2/pydoda/
+-rw-rw-r--   0 saad      (1000) saad      (1000)      795 2023-06-26 22:43:54.000000 pydoda-1.0.2/pydoda/__init__.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4719 2023-06-26 12:14:41.000000 pydoda-1.0.2/pydoda/category.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4014 2023-06-26 23:18:19.000000 pydoda-1.0.2/pydoda/custom_category.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.492249 pydoda-1.0.2/pydoda/dataset/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1235 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/LICENSE
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3877 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/README.md
+-rw-rw-r--   0 saad      (1000) saad      (1000)    49090 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/imagenet_b_darija.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)      460 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/progress.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)   589131 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/sentences.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3786 2023-06-26 23:07:25.000000 pydoda-1.0.2/pydoda/loader.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2772 2023-06-26 23:45:18.000000 pydoda-1.0.2/pydoda/py_doda.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3497 2023-06-26 22:45:08.000000 pydoda-1.0.2/pydoda/sentence.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)      367 2023-07-07 21:32:50.000000 pydoda-1.0.2/pydoda/utils.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.492249 pydoda-1.0.2/pydoda.egg-info/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     5809 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/PKG-INFO
+-rw-rw-r--   0 saad      (1000) saad      (1000)      513 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/SOURCES.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/dependency_links.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)        7 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/requires.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       13 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/top_level.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-07 21:41:32.496249 pydoda-1.0.2/setup.cfg
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1222 2023-07-07 21:41:22.000000 pydoda-1.0.2/setup.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.496249 pydoda-1.0.2/tests/
+-rw-rw-r--   0 saad      (1000) saad      (1000)        0 2023-06-27 12:10:35.000000 pydoda-1.0.2/tests/__init__.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4646 2023-06-27 12:10:35.000000 pydoda-1.0.2/tests/test_category.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2555 2023-06-27 12:10:35.000000 pydoda-1.0.2/tests/test_py_doda.py
```

### Comparing `pydoda-1.0.1/LICENSE` & `pydoda-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/PKG-INFO` & `pydoda-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoda
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper Python library for working with the DODa dataset
 Home-page: https://github.com/saad-out/pydoda
 Author: Saad Outchakoucht
 Author-email: outsaad03@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -133,14 +133,17 @@
 
 # Get the English translation of a word
 english_translation = my_category.get_english_translation('mch')
 print(english_translation)
 # Output: 'cat'
 ```
 
+# Documentation
+For a detailed documentation on the Pydoda library, please refer to the [official Pydoda documentation](https://saad-out.github.io/pydoda/).
+
 # Clone Repository
 To clone the Pydoda repository, use the following command:
 ```
 git clone https://github.com/saad-out/pydoda.git --recurse-submodule
 ```
 The `--recurse-submodule` flag is used to ensure that you also clone the submodules associated with the repository. In this case, the Pydoda library has a submodule named dataset (The Darija Open Dataset), which contains the linguistic dataset used by Pydoda. Cloning the repository with the `--recurse-submodule` flag ensures that you have access to both the Pydoda library code and the necessary dataset.
```

### Comparing `pydoda-1.0.1/README.md` & `pydoda-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,17 @@
 
 # Get the English translation of a word
 english_translation = my_category.get_english_translation('mch')
 print(english_translation)
 # Output: 'cat'
 ```
 
+# Documentation
+For a detailed documentation on the Pydoda library, please refer to the [official Pydoda documentation](https://saad-out.github.io/pydoda/).
+
 # Clone Repository
 To clone the Pydoda repository, use the following command:
 ```
 git clone https://github.com/saad-out/pydoda.git --recurse-submodule
 ```
 The `--recurse-submodule` flag is used to ensure that you also clone the submodules associated with the repository. In this case, the Pydoda library has a submodule named dataset (The Darija Open Dataset), which contains the linguistic dataset used by Pydoda. Cloning the repository with the `--recurse-submodule` flag ensures that you have access to both the Pydoda library code and the necessary dataset.
```

### Comparing `pydoda-1.0.1/pydoda/__init__.py` & `pydoda-1.0.2/pydoda/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/category.py` & `pydoda-1.0.2/pydoda/category.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/custom_category.py` & `pydoda-1.0.2/pydoda/custom_category.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/dataset/LICENSE` & `pydoda-1.0.2/pydoda/dataset/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/dataset/README.md` & `pydoda-1.0.2/pydoda/dataset/README.md`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/dataset/imagenet_b_darija.csv` & `pydoda-1.0.2/pydoda/dataset/imagenet_b_darija.csv`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/dataset/sentences.csv` & `pydoda-1.0.2/pydoda/dataset/sentences.csv`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/loader.py` & `pydoda-1.0.2/pydoda/loader.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/py_doda.py` & `pydoda-1.0.2/pydoda/py_doda.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda/sentence.py` & `pydoda-1.0.2/pydoda/sentence.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/pydoda.egg-info/PKG-INFO` & `pydoda-1.0.2/pydoda.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoda
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper Python library for working with the DODa dataset
 Home-page: https://github.com/saad-out/pydoda
 Author: Saad Outchakoucht
 Author-email: outsaad03@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -133,14 +133,17 @@
 
 # Get the English translation of a word
 english_translation = my_category.get_english_translation('mch')
 print(english_translation)
 # Output: 'cat'
 ```
 
+# Documentation
+For a detailed documentation on the Pydoda library, please refer to the [official Pydoda documentation](https://saad-out.github.io/pydoda/).
+
 # Clone Repository
 To clone the Pydoda repository, use the following command:
 ```
 git clone https://github.com/saad-out/pydoda.git --recurse-submodule
 ```
 The `--recurse-submodule` flag is used to ensure that you also clone the submodules associated with the repository. In this case, the Pydoda library has a submodule named dataset (The Darija Open Dataset), which contains the linguistic dataset used by Pydoda. Cloning the repository with the `--recurse-submodule` flag ensures that you have access to both the Pydoda library code and the necessary dataset.
```

### Comparing `pydoda-1.0.1/pydoda.egg-info/SOURCES.txt` & `pydoda-1.0.2/pydoda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/setup.py` & `pydoda-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pydoda",
-    version="1.0.1",
+    version="1.0.2",
     author="Saad Outchakoucht",
     author_email="outsaad03@gmail.com",
     description="A wrapper Python library for working with the DODa dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saad-out/pydoda",
     packages=setuptools.find_packages(),
@@ -26,10 +26,10 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     include_package_data=True,
-    package_data={"pydoda": ["dataset/*"]},
+    package_data={"pydoda": ["dataset/**"]},
     python_requires=">=3.6",
 )
```

### Comparing `pydoda-1.0.1/tests/test_category.py` & `pydoda-1.0.2/tests/test_category.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.1/tests/test_py_doda.py` & `pydoda-1.0.2/tests/test_py_doda.py`

 * *Files identical despite different names*

