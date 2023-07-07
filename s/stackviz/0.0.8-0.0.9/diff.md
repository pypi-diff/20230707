# Comparing `tmp/stackviz-0.0.8.tar.gz` & `tmp/stackviz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackviz-0.0.8.tar", last modified: Fri Jul  7 14:49:45 2023, max compression
+gzip compressed data, was "stackviz-0.0.9.tar", last modified: Fri Jul  7 14:55:07 2023, max compression
```

## Comparing `stackviz-0.0.8.tar` & `stackviz-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:49:45.431267 stackviz-0.0.8/
--rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.8/LICENSE
--rw-r--r--   0 youhaolin   (501) staff       (20)       29 2023-07-07 14:44:56.000000 stackviz-0.0.8/MANIFEST.in
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:49:45.431148 stackviz-0.0.8/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.8/README.md
--rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-07-07 14:49:45.431312 stackviz-0.0.8/setup.cfg
--rw-r--r--   0 youhaolin   (501) staff       (20)      452 2023-07-07 14:49:35.000000 stackviz-0.0.8/setup.py
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:49:45.429373 stackviz-0.0.8/stackviz/
--rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:44:45.000000 stackviz-0.0.8/stackviz/__init__.py
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:49:45.430477 stackviz-0.0.8/stackviz/display/
--rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 12:18:19.000000 stackviz-0.0.8/stackviz/display/__init__.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     1313 2023-07-07 13:47:02.000000 stackviz-0.0.8/stackviz/display/chart.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     1110 2023-07-07 13:23:20.000000 stackviz-0.0.8/stackviz/display/layout.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     2125 2023-07-07 14:49:27.000000 stackviz-0.0.8/stackviz/display/stack.py
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:49:45.430863 stackviz-0.0.8/stackviz/resources/
--rw-r--r--   0 youhaolin   (501) staff       (20)      332 2023-07-07 12:17:12.000000 stackviz-0.0.8/stackviz/resources/default.css
--rw-r--r--   0 youhaolin   (501) staff       (20)      417 2023-07-07 13:27:47.000000 stackviz-0.0.8/stackviz/resources/template.tpl
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:49:45.429953 stackviz-0.0.8/stackviz.egg-info/
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:49:45.000000 stackviz-0.0.8/stackviz.egg-info/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)      389 2023-07-07 14:49:45.000000 stackviz-0.0.8/stackviz.egg-info/SOURCES.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-07-07 14:49:45.000000 stackviz-0.0.8/stackviz.egg-info/dependency_links.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:49:45.000000 stackviz-0.0.8/stackviz.egg-info/requires.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        9 2023-07-07 14:49:45.000000 stackviz-0.0.8/stackviz.egg-info/top_level.txt
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:55:07.726911 stackviz-0.0.9/
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.9/LICENSE
+-rw-r--r--   0 youhaolin   (501) staff       (20)       29 2023-07-07 14:44:56.000000 stackviz-0.0.9/MANIFEST.in
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:55:07.726795 stackviz-0.0.9/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.9/README.md
+-rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-07-07 14:55:07.726951 stackviz-0.0.9/setup.cfg
+-rw-r--r--   0 youhaolin   (501) staff       (20)      452 2023-07-07 14:54:56.000000 stackviz-0.0.9/setup.py
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:55:07.724900 stackviz-0.0.9/stackviz/
+-rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:44:45.000000 stackviz-0.0.9/stackviz/__init__.py
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:55:07.726057 stackviz-0.0.9/stackviz/display/
+-rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 12:18:19.000000 stackviz-0.0.9/stackviz/display/__init__.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1313 2023-07-07 13:47:02.000000 stackviz-0.0.9/stackviz/display/chart.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1110 2023-07-07 13:23:20.000000 stackviz-0.0.9/stackviz/display/layout.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     2108 2023-07-07 14:54:52.000000 stackviz-0.0.9/stackviz/display/stack.py
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:55:07.726497 stackviz-0.0.9/stackviz/resources/
+-rw-r--r--   0 youhaolin   (501) staff       (20)      332 2023-07-07 12:17:12.000000 stackviz-0.0.9/stackviz/resources/default.css
+-rw-r--r--   0 youhaolin   (501) staff       (20)      417 2023-07-07 13:27:47.000000 stackviz-0.0.9/stackviz/resources/template.tpl
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:55:07.725533 stackviz-0.0.9/stackviz.egg-info/
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:55:07.000000 stackviz-0.0.9/stackviz.egg-info/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)      389 2023-07-07 14:55:07.000000 stackviz-0.0.9/stackviz.egg-info/SOURCES.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-07-07 14:55:07.000000 stackviz-0.0.9/stackviz.egg-info/dependency_links.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:55:07.000000 stackviz-0.0.9/stackviz.egg-info/requires.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        9 2023-07-07 14:55:07.000000 stackviz-0.0.9/stackviz.egg-info/top_level.txt
```

### Comparing `stackviz-0.0.8/LICENSE` & `stackviz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.8/stackviz/display/chart.py` & `stackviz-0.0.9/stackviz/display/chart.py`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.8/stackviz/display/layout.py` & `stackviz-0.0.9/stackviz/display/layout.py`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.8/stackviz/display/stack.py` & `stackviz-0.0.9/stackviz/display/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             css信息：若传文件路径 ，则读取对应文件的内容；否则直接将该信息作为内容
         """
         if os.path.exists(css):
             with open(css, 'r', encoding='utf-8') as css_file:
                 self.css = css_file.read()
         else:
             self.css = css
-        with open(os.path.join(os.path.dirname(os.path.dirname(__file__)), '/resources/template.tpl'), "r", encoding="UTF-8") as tpl_file:
+        with open(os.path.join(os.path.dirname(__file__), '/resources/template.tpl'), "r", encoding="UTF-8") as tpl_file:
             self.html = tpl_file.read()
         self.html = self.html.replace("${style}", css)
         self.rows_span = rows_span
         self.cols_span = cols_span
         self.layout = LayOut(rows_span, cols_span)
         self.layout_settings = []
         self.scripts = []
```

