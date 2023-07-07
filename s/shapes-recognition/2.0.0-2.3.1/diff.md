# Comparing `tmp/shapes_recognition-2.0.0.tar.gz` & `tmp/shapes_recognition-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.0.0.tar", last modified: Mon Jun  5 11:08:24 2023, max compression
+gzip compressed data, was "shapes_recognition-2.3.1.tar", last modified: Fri Jul  7 09:55:45 2023, max compression
```

## Comparing `shapes_recognition-2.0.0.tar` & `shapes_recognition-2.3.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.851884 shapes_recognition-2.0.0/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-05 11:08:24.851557 shapes_recognition-2.0.0/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.0.0/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-05 11:08:24.851972 shapes_recognition-2.0.0/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-05 11:07:55.000000 shapes_recognition-2.0.0/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.848701 shapes_recognition-2.0.0/shapes_recognition/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      266 2023-06-04 14:33:45.000000 shapes_recognition-2.0.0/shapes_recognition/__init__.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.850372 shapes_recognition-2.0.0/shapes_recognition/pure_cython/
--rwxr-xr-x   0 boriskravtsov   (501) staff       (20)   656872 2023-06-05 10:09:55.000000 shapes_recognition-2.0.0/shapes_recognition/pure_cython/ai_tables.cpython-310-darwin.so
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.850038 shapes_recognition-2.0.0/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      280 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 09:55:45.499114 shapes_recognition-2.3.1/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1206 2023-07-07 09:55:45.498858 shapes_recognition-2.3.1/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.3.1/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-07-07 09:55:45.499233 shapes_recognition-2.3.1/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1248 2023-07-07 09:42:17.000000 shapes_recognition-2.3.1/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 09:55:45.496269 shapes_recognition-2.3.1/shapes_recognition/
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 09:55:45.498247 shapes_recognition-2.3.1/shapes_recognition/pure_cython/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      301 2022-12-10 15:57:51.000000 shapes_recognition-2.3.1/shapes_recognition/pure_cython/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 09:55:45.497948 shapes_recognition-2.3.1/shapes_recognition.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1206 2023-07-07 09:55:45.000000 shapes_recognition-2.3.1/shapes_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      226 2023-07-07 09:55:45.000000 shapes_recognition-2.3.1/shapes_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-07-07 09:55:45.000000 shapes_recognition-2.3.1/shapes_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-07-07 09:55:45.000000 shapes_recognition-2.3.1/shapes_recognition.egg-info/top_level.txt
```

### Comparing `shapes_recognition-2.0.0/PKG-INFO` & `shapes_recognition-2.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: shapes_recognition
-Version: 2.0.0
+Version: 2.3.1
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 
 ## SHAPES_RECOGNITION
 "shapes_recognition" is a New Recognition Technology.
 
 ### Installation
```

### Comparing `shapes_recognition-2.0.0/README.md` & `shapes_recognition-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `shapes_recognition-2.0.0/setup.py` & `shapes_recognition-2.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="shapes_recognition",
-    version="2.0.0",
+    version="2.3.1",
     description="New Shape Matching Technology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: MacOS :: MacOS X"
     ],
     packages=['shapes_recognition'],
     package_dir={'shapes_recognition': 'shapes_recognition/pure_cython'},
     package_data={'shapes_recognition': ['shapes_recognition/pure_cython/ai_tables.cpython-310-darwin.so']},
     include_package_data=True,
     install_requires=[]
```

### Comparing `shapes_recognition-2.0.0/shapes_recognition.egg-info/PKG-INFO` & `shapes_recognition-2.3.1/shapes_recognition.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: shapes-recognition
-Version: 2.0.0
+Version: 2.3.1
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 
 ## SHAPES_RECOGNITION
 "shapes_recognition" is a New Recognition Technology.
 
 ### Installation
```

