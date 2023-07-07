# Comparing `tmp/huhangkai-1.5.2.tar.gz` & `tmp/huhangkai-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.5.2.tar", last modified: Fri Jul  7 07:38:11 2023, max compression
+gzip compressed data, was "huhangkai-1.5.3.tar", last modified: Fri Jul  7 08:33:19 2023, max compression
```

## Comparing `huhangkai-1.5.2.tar` & `huhangkai-1.5.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.694006 huhangkai-1.5.2/
--rw-rw-rw-   0        0        0      228 2023-07-07 07:38:11.693009 huhangkai-1.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.639644 huhangkai-1.5.2/commen/
--rw-rw-rw-   0        0        0      933 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.649584 huhangkai-1.5.2/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-05 09:37:54.000000 huhangkai-1.5.2/commen/case_project/json_coder.py
--rw-rw-rw-   0        0        0      822 2023-07-05 06:26:21.000000 huhangkai-1.5.2/commen/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-07 07:38:11.000000 huhangkai-1.5.2/commen/case_project/version.py
--rw-rw-rw-   0        0        0    29301 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/init_project.py
--rw-rw-rw-   0        0        0      276 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.650581 huhangkai-1.5.2/commen/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.682037 huhangkai-1.5.2/commen/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7080 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      521 2023-07-05 08:50:31.000000 huhangkai-1.5.2/commen/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1548 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2148 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      568 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2621 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1696 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      519 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      553 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    21837 2023-07-05 10:01:08.000000 huhangkai-1.5.2/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    24518 2023-07-07 07:38:01.000000 huhangkai-1.5.2/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-05 02:58:25.000000 huhangkai-1.5.2/commen/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:38:11.691013 huhangkai-1.5.2/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1088 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 07:38:11.000000 huhangkai-1.5.2/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 07:38:11.694006 huhangkai-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.807334 huhangkai-1.5.3/
+-rw-rw-rw-   0        0        0      228 2023-07-07 08:33:19.806337 huhangkai-1.5.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.755473 huhangkai-1.5.3/commen/
+-rw-rw-rw-   0        0        0      933 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.765446 huhangkai-1.5.3/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-05 09:37:54.000000 huhangkai-1.5.3/commen/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      822 2023-07-05 06:26:21.000000 huhangkai-1.5.3/commen/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-07 08:33:19.000000 huhangkai-1.5.3/commen/case_project/version.py
+-rw-rw-rw-   0        0        0    29301 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/init_project.py
+-rw-rw-rw-   0        0        0      276 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.767441 huhangkai-1.5.3/commen/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.796364 huhangkai-1.5.3/commen/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7080 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      521 2023-07-05 08:50:31.000000 huhangkai-1.5.3/commen/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1548 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2621 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    21837 2023-07-05 10:01:08.000000 huhangkai-1.5.3/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    24880 2023-07-07 08:33:07.000000 huhangkai-1.5.3/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.804342 huhangkai-1.5.3/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 08:33:19.807334 huhangkai-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.5.3/setup.py
```

### Comparing `huhangkai-1.5.2/commen/__init__.py` & `huhangkai-1.5.3/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/case_project/base_project.py` & `huhangkai-1.5.3/commen/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/case_project/json_coder.py` & `huhangkai-1.5.3/commen/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/case_project/setup_set.py` & `huhangkai-1.5.3/commen/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/init_project.py` & `huhangkai-1.5.3/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/beam_class.py` & `huhangkai-1.5.3/commen/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/data.py` & `huhangkai-1.5.3/commen/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/par_do.py` & `huhangkai-1.5.3/commen/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_cogroupbykey.py` & `huhangkai-1.5.3/commen/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_file.py` & `huhangkai-1.5.3/commen/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_fiter.py` & `huhangkai-1.5.3/commen/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_flatmap.py` & `huhangkai-1.5.3/commen/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_map.py` & `huhangkai-1.5.3/commen/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_par_do.py` & `huhangkai-1.5.3/commen/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_regex.py` & `huhangkai-1.5.3/commen/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_time.py` & `huhangkai-1.5.3/commen/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/testcase/apache/test_to_string.py` & `huhangkai-1.5.3/commen/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/unit_apache_beam.py` & `huhangkai-1.5.3/commen/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/unit_dict.py` & `huhangkai-1.5.3/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/unit_encryption.py` & `huhangkai-1.5.3/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/unit_fun.py` & `huhangkai-1.5.3/commen/unit_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -460,16 +460,17 @@
                         return [i.get(name) for i in value]
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
                             if isinstance(value2, list):
                                 return [i.get(name) for i in value2 if i.get(name)]
             return []
 
-    def excelWriter(self, filename, data, sheet_name="sheet", set_column=[], header_format=None, column_header=[],
-                    column_default=[]):
+    @staticmethod
+    def excelWriter(filename, data, sheet_name="sheet", set_column=[], header_format=None, column_header=[],
+                    column_default=[], isdigitl=True):
         from pandas import DataFrame, ExcelWriter
         filename = filename[:4] + filename[4:].replace(":", "").replace(' ', '_')
         try:
             with ExcelWriter(filename) as writer:
                 # 写入到第一个sheet
                 if data and isinstance(data[0], list):
                     h = data[0]
@@ -490,14 +491,22 @@
                                 _header[column_header[i]] = v
                             except:
                                 pass
                     for i, v in enumerate(data):
                         _data = _header.copy()
                         _data.update(v)
                         data[i] = _data
+                if isdigitl:
+                    for i, d in enumerate(data):
+                        for k, v in d.items():
+                            try:
+                                if v.isdigit():
+                                    data[i][k] = int(v)
+                            except:
+                                pass
                 result = DataFrame(data)
                 result.to_excel(writer, sheet_name=sheet_name, index=False, engine="openpyxl")
 
                 try:
                     worksheet = writer.sheets.get(sheet_name) or writer.sheets.get("sheet1")
                     for idx, v in enumerate(set_column):
                         try:
```

### Comparing `huhangkai-1.5.2/commen/unit_logger.py` & `huhangkai-1.5.3/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/unit_request.py` & `huhangkai-1.5.3/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/unit_tasks.py` & `huhangkai-1.5.3/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/commen/常用命令.py` & `huhangkai-1.5.3/commen/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.2/huhangkai.egg-info/SOURCES.txt` & `huhangkai-1.5.3/huhangkai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

