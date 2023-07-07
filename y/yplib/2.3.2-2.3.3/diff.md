# Comparing `tmp/yplib-2.3.2.tar.gz` & `tmp/yplib-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.2.tar", last modified: Fri Jul  7 00:45:15 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.3.tar", last modified: Fri Jul  7 01:02:48 2023, max compression
```

## Comparing `yplib-2.3.2.tar` & `yplib-2.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 00:45:15.080333 yplib-2.3.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-07 00:45:15.079560 yplib-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 00:45:15.080333 yplib-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-07 00:45:04.000000 yplib-2.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 00:45:15.074144 yplib-2.3.2/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.2/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.2/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.2/yplib/http_util.py
--rw-rw-rw-   0        0        0    30470 2023-07-07 00:24:58.000000 yplib-2.3.2/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.2/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.2/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.2/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.2/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-07 00:45:15.078433 yplib-2.3.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 00:45:15.000000 yplib-2.3.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 01:02:48.923077 yplib-2.3.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-07 01:02:48.922958 yplib-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 01:02:48.923483 yplib-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-07 01:01:47.000000 yplib-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:02:48.919192 yplib-2.3.3/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.3/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.3/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.3/yplib/http_util.py
+-rw-rw-rw-   0        0        0    30937 2023-07-07 00:55:03.000000 yplib-2.3.3/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.3/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.3/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.3/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.3/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:02:48.921989 yplib-2.3.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.2/LICENSE` & `yplib-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/setup.py` & `yplib-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.2",
+  version="2.3.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.2/yplib/__init__.py` & `yplib-2.3.3/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/chart.py` & `yplib-2.3.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/chart_html.py` & `yplib-2.3.3/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/db.py` & `yplib-2.3.3/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/file.py` & `yplib-2.3.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/http_util.py` & `yplib-2.3.3/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/index.py` & `yplib-2.3.3/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,14 +501,33 @@
 # 将一个文件中以空行作为分隔符,
 # 组成一个 list(list) 数据
 # 多行空行,自动合并到一行空行
 def to_list_from_txt_with_blank_row(file_name='a.txt'):
     return to_list_from_txt(file_name, sep_line='')
 
 
+# 将 list 切分成 list(list)
+# 组成一个 list(list) 数据
+# 多行空行,自动合并到一行空行
+def to_list_list(data_list=[], count=10):
+    r_list = []
+    o_list = []
+    c = 0
+    for i in range(len(data_list)):
+        o_list.append(data_list[i])
+        c += 1
+        if c == count:
+            r_list.append(o_list)
+            o_list = []
+            c = 0
+    if len(o_list):
+        r_list.append(o_list)
+    return r_list
+
+
 # 将一个文件中的数据按照行来区分,
 # 会自动过滤掉空格行,
 # 组成一个 list(json) 数据
 def to_list_json_from_txt(file_name='a.txt',
                           start_index=None,
                           start_line=None,
                           end_index=None,
```

### Comparing `yplib-2.3.2/yplib/mail.py` & `yplib-2.3.3/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/mail_html.py` & `yplib-2.3.3/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.2/yplib/markdown.py` & `yplib-2.3.3/yplib/markdown.py`

 * *Files identical despite different names*

