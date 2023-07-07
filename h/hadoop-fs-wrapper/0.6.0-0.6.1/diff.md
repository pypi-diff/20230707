# Comparing `tmp/hadoop_fs_wrapper-0.6.0.tar.gz` & `tmp/hadoop_fs_wrapper-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadoop_fs_wrapper-0.6.0.tar", max compression
+gzip compressed data, was "hadoop_fs_wrapper-0.6.1.tar", max compression
```

## Comparing `hadoop_fs_wrapper-0.6.0.tar` & `hadoop_fs_wrapper-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/LICENSE
--rw-r--r--   0        0        0     1925 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/README.md
--rw-r--r--   0        0        0     1182 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/__init__.py
--rw-r--r--   0        0        0       22 2023-05-30 14:28:49.302048 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/_version.py
--rw-r--r--   0        0        0     1108 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/__init__.py
--rw-r--r--   0        0        0     1863 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_input_stream.py
--rw-r--r--   0        0        0     2726 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_output_stream.py
--rw-r--r--   0        0        0     1712 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_reader.py
--rw-r--r--   0        0        0     2505 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/file_status.py
--rw-r--r--   0        0        0     1385 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_input_stream.py
--rw-r--r--   0        0        0     1388 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_output_stream.py
--rw-r--r--   0        0        0     1682 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/glob_filter.py
--rw-r--r--   0        0        0     2493 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_file_status.py
--rw-r--r--   0        0        0     1720 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_fs_path.py
--rw-r--r--   0        0        0     2226 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/input_stream_reader.py
--rw-r--r--   0        0        0     2120 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/remote_iterator.py
--rw-r--r--   0        0        0     1626 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/uri.py
--rw-r--r--   0        0        0     1108 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/__init__.py
--rw-r--r--   0        0        0     7060 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/file_system.py
--rw-r--r--   0        0        0    11783 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py
--rw-r--r--   0        0        0      628 2023-05-30 14:28:49.302048 hadoop_fs_wrapper-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 hadoop_fs_wrapper-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1925 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/README.md
+-rw-r--r--   0        0        0     1182 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-07 11:11:36.734142 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/_version.py
+-rw-r--r--   0        0        0     1108 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/__init__.py
+-rw-r--r--   0        0        0     1863 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/buffered_input_stream.py
+-rw-r--r--   0        0        0     2726 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/buffered_output_stream.py
+-rw-r--r--   0        0        0     1712 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/buffered_reader.py
+-rw-r--r--   0        0        0     2505 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/file_status.py
+-rw-r--r--   0        0        0     1385 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/fs_data_input_stream.py
+-rw-r--r--   0        0        0     1388 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/fs_data_output_stream.py
+-rw-r--r--   0        0        0     1682 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/glob_filter.py
+-rw-r--r--   0        0        0     2493 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/hadoop_file_status.py
+-rw-r--r--   0        0        0     1720 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/hadoop_fs_path.py
+-rw-r--r--   0        0        0     2226 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/input_stream_reader.py
+-rw-r--r--   0        0        0     2120 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/remote_iterator.py
+-rw-r--r--   0        0        0     1626 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/uri.py
+-rw-r--r--   0        0        0     1108 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/wrappers/__init__.py
+-rw-r--r--   0        0        0     7060 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/wrappers/file_system.py
+-rw-r--r--   0        0        0    11783 2023-07-07 11:11:19.973867 hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py
+-rw-r--r--   0        0        0      628 2023-07-07 11:11:36.734142 hadoop_fs_wrapper-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 hadoop_fs_wrapper-0.6.1/PKG-INFO
```

### Comparing `hadoop_fs_wrapper-0.6.0/LICENSE` & `hadoop_fs_wrapper-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/README.md` & `hadoop_fs_wrapper-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/__init__.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/__init__.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_input_stream.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/buffered_input_stream.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_output_stream.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/buffered_output_stream.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_reader.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/buffered_reader.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/file_status.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/file_status.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_input_stream.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/fs_data_input_stream.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_output_stream.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/fs_data_output_stream.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/glob_filter.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/glob_filter.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_file_status.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/hadoop_file_status.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_fs_path.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/hadoop_fs_path.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/input_stream_reader.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/input_stream_reader.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/remote_iterator.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/remote_iterator.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/uri.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/models/uri.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/__init__.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/file_system.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/wrappers/file_system.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py` & `hadoop_fs_wrapper-0.6.1/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.6.0/pyproject.toml` & `hadoop_fs_wrapper-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hadoop-fs-wrapper"
-version = "0.6.0"
+version = "0.6.1"
 description = "Python Wrapper for Hadoop Java API"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/hadoop-fs-wrapper'
```

### Comparing `hadoop_fs_wrapper-0.6.0/PKG-INFO` & `hadoop_fs_wrapper-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadoop-fs-wrapper
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python Wrapper for Hadoop Java API
 Home-page: https://github.com/SneaksAndData/hadoop-fs-wrapper
 License: MIT
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

