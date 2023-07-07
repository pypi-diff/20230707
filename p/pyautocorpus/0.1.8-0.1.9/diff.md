# Comparing `tmp/pyautocorpus-0.1.8.tar.gz` & `tmp/pyautocorpus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautocorpus-0.1.8.tar", last modified: Mon Dec  6 09:21:19 2021, max compression
+gzip compressed data, was "pyautocorpus-0.1.9.tar", last modified: Wed Oct 26 10:03:46 2022, max compression
```

## Comparing `pyautocorpus-0.1.8.tar` & `pyautocorpus-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.430003 pyautocorpus-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.426003 pyautocorpus-0.1.8/AutoCorpus/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.426003 pyautocorpus-0.1.8/AutoCorpus/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.426003 pyautocorpus-0.1.8/AutoCorpus/src/common/
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2021-12-06 09:21:08.000000 pyautocorpus-0.1.8/AutoCorpus/src/common/PCREMatcher.h
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-12-06 09:21:08.000000 pyautocorpus-0.1.8/AutoCorpus/src/common/merge.h
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2021-12-06 09:21:08.000000 pyautocorpus-0.1.8/AutoCorpus/src/common/utilities.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.426003 pyautocorpus-0.1.8/AutoCorpus/src/ngrams/
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-12-06 09:21:08.000000 pyautocorpus-0.1.8/AutoCorpus/src/ngrams/NGramCounter.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.426003 pyautocorpus-0.1.8/AutoCorpus/src/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2021-12-06 09:21:08.000000 pyautocorpus-0.1.8/AutoCorpus/src/wikipedia/SentenceExtractor.h
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2021-12-06 09:21:08.000000 pyautocorpus-0.1.8/AutoCorpus/src/wikipedia/Textifier.h
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-12-06 09:21:07.000000 pyautocorpus-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2021-12-06 09:21:19.430003 pyautocorpus-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-12-06 09:21:07.000000 pyautocorpus-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.430003 pyautocorpus-0.1.8/pyautocorpus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2021-12-06 09:21:19.000000 pyautocorpus-0.1.8/pyautocorpus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      450 2021-12-06 09:21:19.000000 pyautocorpus-0.1.8/pyautocorpus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-06 09:21:19.000000 pyautocorpus-0.1.8/pyautocorpus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-06 09:21:19.000000 pyautocorpus-0.1.8/pyautocorpus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-06 09:21:19.430003 pyautocorpus-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-12-06 09:21:07.000000 pyautocorpus-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:21:19.430003 pyautocorpus-0.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (121)    12485 2021-12-06 09:21:07.000000 pyautocorpus-0.1.8/src/Textifier.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4577 2021-12-06 09:21:07.000000 pyautocorpus-0.1.8/src/pyautocorpus.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2021-12-06 09:21:07.000000 pyautocorpus-0.1.8/src/utilities.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.683287 pyautocorpus-0.1.9/AutoCorpus/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.683287 pyautocorpus-0.1.9/AutoCorpus/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/AutoCorpus/src/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-10-26 10:03:35.000000 pyautocorpus-0.1.9/AutoCorpus/src/common/PCREMatcher.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-10-26 10:03:35.000000 pyautocorpus-0.1.9/AutoCorpus/src/common/merge.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-10-26 10:03:35.000000 pyautocorpus-0.1.9/AutoCorpus/src/common/utilities.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/AutoCorpus/src/ngrams/
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-26 10:03:35.000000 pyautocorpus-0.1.9/AutoCorpus/src/ngrams/NGramCounter.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/AutoCorpus/src/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-10-26 10:03:35.000000 pyautocorpus-0.1.9/AutoCorpus/src/wikipedia/SentenceExtractor.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-10-26 10:03:35.000000 pyautocorpus-0.1.9/AutoCorpus/src/wikipedia/Textifier.h
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-26 10:03:34.000000 pyautocorpus-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-10-26 10:03:34.000000 pyautocorpus-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/pyautocorpus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-26 10:03:46.000000 pyautocorpus-0.1.9/pyautocorpus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-26 10:03:46.000000 pyautocorpus-0.1.9/pyautocorpus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 10:03:46.000000 pyautocorpus-0.1.9/pyautocorpus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-26 10:03:46.000000 pyautocorpus-0.1.9/pyautocorpus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-10-26 10:03:34.000000 pyautocorpus-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 10:03:46.687287 pyautocorpus-0.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (121)    12485 2022-10-26 10:03:34.000000 pyautocorpus-0.1.9/src/Textifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4577 2022-10-26 10:03:34.000000 pyautocorpus-0.1.9/src/pyautocorpus.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-10-26 10:03:34.000000 pyautocorpus-0.1.9/src/utilities.cpp
```

### Comparing `pyautocorpus-0.1.8/AutoCorpus/src/common/PCREMatcher.h` & `pyautocorpus-0.1.9/AutoCorpus/src/common/PCREMatcher.h`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/AutoCorpus/src/common/merge.h` & `pyautocorpus-0.1.9/AutoCorpus/src/common/merge.h`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/AutoCorpus/src/common/utilities.h` & `pyautocorpus-0.1.9/AutoCorpus/src/common/utilities.h`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/AutoCorpus/src/ngrams/NGramCounter.h` & `pyautocorpus-0.1.9/AutoCorpus/src/ngrams/NGramCounter.h`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/AutoCorpus/src/wikipedia/SentenceExtractor.h` & `pyautocorpus-0.1.9/AutoCorpus/src/wikipedia/SentenceExtractor.h`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/AutoCorpus/src/wikipedia/Textifier.h` & `pyautocorpus-0.1.9/AutoCorpus/src/wikipedia/Textifier.h`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/PKG-INFO` & `pyautocorpus-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: pyautocorpus
-Version: 0.1.8
-Summary: UNKNOWN
+Version: 0.1.9
 Home-page: https://github.com/seanmacavaney/pyautocorpus
 Author: Sean MacAvaney
 Author-email: sean.macavaney@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PyAutoCorpus
 
 A python interface to the excellent [AutoCorpus](https://github.com/mpacula/AutoCorpus) library.
@@ -71,9 +68,7 @@
 
 [AutoCorpus](https://github.com/mpacula/AutoCorpus)
 
 Contributors to this repository:
 
  - Sean MacAvaney (University of Glasgow)
  - Thomas Jänich (University of Glasgow)
-
-
```

### Comparing `pyautocorpus-0.1.8/README.md` & `pyautocorpus-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/pyautocorpus.egg-info/PKG-INFO` & `pyautocorpus-0.1.9/pyautocorpus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: pyautocorpus
-Version: 0.1.8
-Summary: UNKNOWN
+Version: 0.1.9
 Home-page: https://github.com/seanmacavaney/pyautocorpus
 Author: Sean MacAvaney
 Author-email: sean.macavaney@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PyAutoCorpus
 
 A python interface to the excellent [AutoCorpus](https://github.com/mpacula/AutoCorpus) library.
@@ -71,9 +68,7 @@
 
 [AutoCorpus](https://github.com/mpacula/AutoCorpus)
 
 Contributors to this repository:
 
  - Sean MacAvaney (University of Glasgow)
  - Thomas Jänich (University of Glasgow)
-
-
```

### Comparing `pyautocorpus-0.1.8/setup.py` & `pyautocorpus-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "src/pyautocorpus.cpp",
         "src/utilities.cpp", # custom version of AutoCorpus/src/common/utilities.cpp because of the Windows build
         "src/Textifier.cpp", # custom version of AutoCorpus/src/wikipedia/Textifier.cpp because of the Windows build
     ]
 
 setuptools.setup(
     name="pyautocorpus",
-    version="0.1.8",
+    version="0.1.9",
     author="Sean MacAvaney",
     author_email="sean.macavaney@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/seanmacavaney/pyautocorpus",
     include_package_data = True,
```

### Comparing `pyautocorpus-0.1.8/src/Textifier.cpp` & `pyautocorpus-0.1.9/src/Textifier.cpp`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/src/pyautocorpus.cpp` & `pyautocorpus-0.1.9/src/pyautocorpus.cpp`

 * *Files identical despite different names*

### Comparing `pyautocorpus-0.1.8/src/utilities.cpp` & `pyautocorpus-0.1.9/src/utilities.cpp`

 * *Files identical despite different names*

