# Comparing `tmp/huhangkai-1.5.1.tar.gz` & `tmp/huhangkai-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\huhangkai-1.5.1.tar", last modified: Tue Jul  4 16:47:44 2023, max compression
+gzip compressed data, was "huhangkai-1.5.2.tar", last modified: Fri Jul  7 07:38:11 2023, max compression
```

## Comparing `huhangkai-1.5.1.tar` & `huhangkai-1.5.2.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 16:47:44.000000 huhangkai-1.5.1/
--rw-rw-rw-   0        0        0      158 2023-07-04 16:47:44.000000 huhangkai-1.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 16:47:44.000000 huhangkai-1.5.1/commen/
--rw-rw-rw-   0        0        0      933 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:47:44.000000 huhangkai-1.5.1/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0      803 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-04 16:47:44.000000 huhangkai-1.5.1/commen/case_project/version.py
--rw-rw-rw-   0        0        0    29301 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/init_project.py
--rw-rw-rw-   0        0        0      276 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:47:44.000000 huhangkai-1.5.1/commen/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:47:44.000000 huhangkai-1.5.1/commen/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-04 16:21:28.000000 huhangkai-1.5.1/commen/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-03 15:22:10.000000 huhangkai-1.5.1/commen/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7080 2023-07-04 16:46:57.000000 huhangkai-1.5.1/commen/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0     1548 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2148 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      568 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2621 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1696 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      519 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      553 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    19634 2023-07-04 16:44:35.000000 huhangkai-1.5.1/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    23691 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-04 15:00:15.000000 huhangkai-1.5.1/commen/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:47:44.000000 huhangkai-1.5.1/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      158 2023-07-04 16:47:44.000000 huhangkai-1.5.1/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-07-04 16:47:44.000000 huhangkai-1.5.1/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 16:47:44.000000 huhangkai-1.5.1/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-04 16:47:44.000000 huhangkai-1.5.1/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 16:47:44.000000 huhangkai-1.5.1/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 16:47:44.000000 huhangkai-1.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.694006 huhangkai-1.5.2/
+-rw-rw-rw-   0        0        0      228 2023-07-07 07:38:11.693009 huhangkai-1.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.639644 huhangkai-1.5.2/commen/
+-rw-rw-rw-   0        0        0      933 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.649584 huhangkai-1.5.2/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-05 09:37:54.000000 huhangkai-1.5.2/commen/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      822 2023-07-05 06:26:21.000000 huhangkai-1.5.2/commen/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-07 07:38:11.000000 huhangkai-1.5.2/commen/case_project/version.py
+-rw-rw-rw-   0        0        0    29301 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/init_project.py
+-rw-rw-rw-   0        0        0      276 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.650581 huhangkai-1.5.2/commen/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.682037 huhangkai-1.5.2/commen/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7080 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      521 2023-07-05 08:50:31.000000 huhangkai-1.5.2/commen/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1548 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2621 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    21837 2023-07-05 10:01:08.000000 huhangkai-1.5.2/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    24518 2023-07-07 07:38:01.000000 huhangkai-1.5.2/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.691013 huhangkai-1.5.2/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 07:38:11.694006 huhangkai-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.5.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `huhangkai-1.5.1/commen/__init__.py` & `huhangkai-1.5.2/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/case_project/base_project.py` & `huhangkai-1.5.2/commen/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/case_project/setup_set.py` & `huhangkai-1.5.2/commen/case_project/setup_set.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,11 +23,12 @@
         "xlsxwriter",
         "pandas",
         "apache-beam",
         "pytest",
         "setuptools",
         "twine",
         "requests==2.29.0",
+        "pandas",
     ],
 )
```

### Comparing `huhangkai-1.5.1/commen/init_project.py` & `huhangkai-1.5.2/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/beam_class.py` & `huhangkai-1.5.2/commen/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/data.py` & `huhangkai-1.5.2/commen/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/par_do.py` & `huhangkai-1.5.2/commen/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_cogroupbykey.py` & `huhangkai-1.5.2/commen/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_fiter.py` & `huhangkai-1.5.2/commen/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_flatmap.py` & `huhangkai-1.5.2/commen/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_map.py` & `huhangkai-1.5.2/commen/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_par_do.py` & `huhangkai-1.5.2/commen/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_regex.py` & `huhangkai-1.5.2/commen/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_time.py` & `huhangkai-1.5.2/commen/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/testcase/apache/test_to_string.py` & `huhangkai-1.5.2/commen/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/unit_apache_beam.py` & `huhangkai-1.5.2/commen/unit_apache_beam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import datetime
+import json
 import time
-
+import pandas as pd
 import apache_beam as beam
 import uuid
 
 from apache_beam import PCollection
+from apache_beam.coders import Coder, StrUtf8Coder
+from apache_beam.io import fileio
 from apache_beam.pvalue import DoOutputsTuple
 from apache_beam.transforms import window
 
+from commen.case_project.json_coder import JsonCoder
+
 
 class ApacheFun:
     window = window
 
     def __init__(self, data=None, name="", out=None, data_type=1):
         """data_type: 1 管道， 2 数据"""
 
@@ -56,14 +61,20 @@
                 if isinstance(i, PCollection):
                     i | self._name() >> beam.Map(lambda x: _print(x))
                 else:
                     _print(i)
         if self.data_type == 1:
             self.run()
 
+    # def get_value(self):
+    #     class ProcessDataDoFn(beam.DoFn):
+    #         def process(self, element, side_input):
+    #             output_dictionary = "element"
+    #             return output_dictionary
+
     def set_data(self, data):
         self.data = data
         self.create(data)
         self.out = self.value
 
     def create(self, data=None):
         """创建"""
@@ -439,11 +450,50 @@
     def top_of(self, n, key=None, reverse=True):
         if isinstance(self.data[0], (list, tuple)):
             self.value = self.out = self.get_out() | self._name() >> beam.combiners.Top.PerKey(n, key, reverse=reverse)
         else:
             self.value = self.out = self.get_out() | self._name() >> beam.combiners.Top.Of(n, key, reverse=reverse)
         return self
 
+    def read_excel(self, file_path, sheet_name=0):
+        def process_excel_file(element):
+            file_name = element.metadata.path
+            df = pd.read_excel(file_name, sheet_name)
+            return df.values.tolist()
+        self.value = self.out = (
+                self.pipeline
+                | self._name() >> beam.io.fileio.MatchFiles(file_path)
+                | self._name() >> beam.io.fileio.ReadMatches()
+                | self._name() >> beam.Map(process_excel_file))
+        return self
+
+    def write_excel(self, file_path):
+        def process_excel_file(element):
+            file_name = element.metadata.path
+            info = pd.DataFrame()
+        self.value = self.out = (
+                self.pipeline
+                | self._name() >> beam.io.fileio.MatchFiles(file_path)
+                | self._name() >> beam.Map(process_excel_file))
+        #         beam.io.fileio.WriteToFiles( path=file_path,
+        # output_fn=pd.to_excel(file_name, sheet_name)
+        #   file_naming=beam.io.fileio.destination_prefix_naming(suffix=".xlsx"))
+        #  )
+        # beam.io.ReadFromText
+        return self
+
+    def read_file(self, path):
+        if path.split(".")[-1] == "txt":
+            self.value = self.out = self.pipeline | self._name() >> beam.io.ReadFromText(path)
+        elif path.split(".")[-1] == "json":
+            self.value = self.out = self.pipeline | self._name() >> beam.io.ReadFromJson(path, dtype=False, encodings='utf-8')
+        elif path.split(".")[-1] == "csv":
+            self.value = self.out = self.pipeline | self._name() >> beam.io.ReadFromCsv(path)
+        return self
+
+
 
 if __name__ == '__main__':
     from commen.testcase.apache.data import *
-    ApacheFun(data_list_tuple).create().print()
+    path = r"C:\Users\hangkai.hu\Desktop\测试\雷达用例\111.txt"
+    path = r"C:\Users\hangkai.hu\Desktop\测试\雷达用例\222.json"
+    ApacheFun().read_file(path).print()
```

### Comparing `huhangkai-1.5.1/commen/unit_dict.py` & `huhangkai-1.5.2/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/unit_encryption.py` & `huhangkai-1.5.2/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/unit_fun.py` & `huhangkai-1.5.2/commen/unit_fun.py`

 * *Files 4% similar despite different names*

```diff
@@ -460,28 +460,44 @@
                         return [i.get(name) for i in value]
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
                             if isinstance(value2, list):
                                 return [i.get(name) for i in value2 if i.get(name)]
             return []
 
-    def excelWriter(self, filename, data, sheet_name="sheet", set_column=[], header_format=None):
+    def excelWriter(self, filename, data, sheet_name="sheet", set_column=[], header_format=None, column_header=[],
+                    column_default=[]):
         from pandas import DataFrame, ExcelWriter
         filename = filename[:4] + filename[4:].replace(":", "").replace(' ', '_')
         try:
             with ExcelWriter(filename) as writer:
                 # 写入到第一个sheet
                 if data and isinstance(data[0], list):
                     h = data[0]
                     data1 = []
                     for i in data[1:]:
                         data1.append({x[0]: str(x[1]) for x in zip(h, i)})
                     data = data1
                 elif data and isinstance(data[0], dict):
                     data = [{k: str(v) for k, v in i.items()} for i in data]
+
+                if column_header:
+                    column_header = column_header if isinstance(column_header, list) else column_header.split(",")
+                    _header = {k: None for k in column_header}
+                    if column_default:
+                        _default = column_default if isinstance(column_default, list) else column_default.split(",")
+                        for i, v in enumerate(_default):
+                            try:
+                                _header[column_header[i]] = v
+                            except:
+                                pass
+                    for i, v in enumerate(data):
+                        _data = _header.copy()
+                        _data.update(v)
+                        data[i] = _data
                 result = DataFrame(data)
                 result.to_excel(writer, sheet_name=sheet_name, index=False, engine="openpyxl")
 
                 try:
                     worksheet = writer.sheets.get(sheet_name) or writer.sheets.get("sheet1")
                     for idx, v in enumerate(set_column):
                         try:
```

### Comparing `huhangkai-1.5.1/commen/unit_logger.py` & `huhangkai-1.5.2/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/unit_request.py` & `huhangkai-1.5.2/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/unit_tasks.py` & `huhangkai-1.5.2/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/commen/常用命令.py` & `huhangkai-1.5.2/commen/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.1/huhangkai.egg-info/SOURCES.txt` & `huhangkai-1.5.2/huhangkai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+setup.py
 commen/__init__.py
 commen/init_project.py
 commen/setup_run.py
 commen/unit_apache_beam.py
 commen/unit_dict.py
 commen/unit_encryption.py
 commen/unit_fun.py
 commen/unit_logger.py
 commen/unit_request.py
 commen/unit_tasks.py
 commen/常用命令.py
 commen/case_project/__init__.py
 commen/case_project/base_project.py
+commen/case_project/json_coder.py
 commen/case_project/setup_set.py
 commen/case_project/version.py
 commen/testcase/__init__.py
 commen/testcase/apache/__init__.py
 commen/testcase/apache/beam_class.py
 commen/testcase/apache/data.py
 commen/testcase/apache/par_do.py
 commen/testcase/apache/test_cogroupbykey.py
+commen/testcase/apache/test_file.py
 commen/testcase/apache/test_fiter.py
 commen/testcase/apache/test_flatmap.py
 commen/testcase/apache/test_map.py
 commen/testcase/apache/test_par_do.py
 commen/testcase/apache/test_regex.py
 commen/testcase/apache/test_time.py
 commen/testcase/apache/test_to_string.py
```

