# Comparing `tmp/hugging_py_face-0.3.1.tar.gz` & `tmp/hugging_py_face-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hugging_py_face-0.3.1.tar", last modified: Fri Jul  7 16:04:20 2023, max compression
+gzip compressed data, was "dist\hugging_py_face-0.3.2.tar", last modified: Fri Jul  7 17:52:12 2023, max compression
```

## Comparing `hugging_py_face-0.3.1.tar` & `hugging_py_face-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/
--rw-rw-rw-   0        0        0     6177 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4692 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face/
--rw-rw-rw-   0        0        0      466 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/__about__.py
--rw-rw-rw-   0        0        0      321 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/__init__.py
--rw-rw-rw-   0        0        0     3927 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/audio_processing.py
--rw-rw-rw-   0        0        0      884 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/base_api.py
--rw-rw-rw-   0        0        0     2852 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/computer_vision.py
-drwxrwxrwx   0        0        0        0 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face/config/
--rw-rw-rw-   0        0        0      837 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/config/config.yaml
--rw-rw-rw-   0        0        0      265 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/config/logging.yaml
--rw-rw-rw-   0        0        0      320 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/config_parser.py
--rw-rw-rw-   0        0        0      171 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/exceptions.py
--rw-rw-rw-   0        0        0     2447 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/multimedia_processing.py
--rw-rw-rw-   0        0        0    24515 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/hugging_py_face/nlp.py
-drwxrwxrwx   0        0        0        0 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face.egg-info/
--rw-rw-rw-   0        0        0     6177 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/hugging_py_face.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 16:04:20.000000 hugging_py_face-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-07-07 16:04:01.000000 hugging_py_face-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/
+-rw-rw-rw-   0        0        0     6177 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4692 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face/
+-rw-rw-rw-   0        0        0      466 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/__about__.py
+-rw-rw-rw-   0        0        0      676 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/__init__.py
+-rw-rw-rw-   0        0        0     3927 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/audio_processing.py
+-rw-rw-rw-   0        0        0      884 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/base_api.py
+-rw-rw-rw-   0        0        0     2852 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face/config/
+-rw-rw-rw-   0        0        0      837 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/config/config.yaml
+-rw-rw-rw-   0        0        0      265 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/config/logging.yaml
+-rw-rw-rw-   0        0        0      320 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/config_parser.py
+-rw-rw-rw-   0        0        0      171 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/exceptions.py
+-rw-rw-rw-   0        0        0     2447 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/multimedia_processing.py
+-rw-rw-rw-   0        0        0    24515 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/hugging_py_face/nlp.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/
+-rw-rw-rw-   0        0        0     6177 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/hugging_py_face.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:52:12.000000 hugging_py_face-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-07 17:51:45.000000 hugging_py_face-0.3.2/setup.py
```

### Comparing `hugging_py_face-0.3.1/PKG-INFO` & `hugging_py_face-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging_py_face
-Version: 0.3.1
+Version: 0.3.2
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.3.1/README.md` & `hugging_py_face-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/hugging_py_face/audio_processing.py` & `hugging_py_face-0.3.2/hugging_py_face/audio_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/hugging_py_face/base_api.py` & `hugging_py_face-0.3.2/hugging_py_face/base_api.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/hugging_py_face/computer_vision.py` & `hugging_py_face-0.3.2/hugging_py_face/computer_vision.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/hugging_py_face/config/config.yaml` & `hugging_py_face-0.3.2/hugging_py_face/config/config.yaml`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/hugging_py_face/multimedia_processing.py` & `hugging_py_face-0.3.2/hugging_py_face/multimedia_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/hugging_py_face/nlp.py` & `hugging_py_face-0.3.2/hugging_py_face/nlp.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/hugging_py_face.egg-info/PKG-INFO` & `hugging_py_face-0.3.2/hugging_py_face.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging-py-face
-Version: 0.3.1
+Version: 0.3.2
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.3.1/hugging_py_face.egg-info/SOURCES.txt` & `hugging_py_face-0.3.2/hugging_py_face.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.3.1/setup.py` & `hugging_py_face-0.3.2/setup.py`

 * *Files identical despite different names*

