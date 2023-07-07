# Comparing `tmp/pydatawork-0.17.4.2.tar.gz` & `tmp/pydatawork-0.17.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.4.2.tar", last modified: Fri Jul  7 08:29:57 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.4.3.tar", last modified: Fri Jul  7 08:32:00 2023, max compression
```

## Comparing `pydatawork-0.17.4.2.tar` & `pydatawork-0.17.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19864 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15033 2023-07-07 08:29:40.000000 pydatawork-0.17.4.2/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19864 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    50502 2023-07-07 08:28:32.000000 pydatawork-0.17.4.2/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-07 08:29:57.000000 pydatawork-0.17.4.2/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-07 08:29:06.000000 pydatawork-0.17.4.2/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19864 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15033 2023-07-07 08:31:32.000000 pydatawork-0.17.4.3/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19864 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    50502 2023-07-07 08:28:32.000000 pydatawork-0.17.4.3/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-07 08:31:25.000000 pydatawork-0.17.4.3/setup.py
```

### Comparing `pydatawork-0.17.4.2/PKG-INFO` & `pydatawork-0.17.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.4.2
+Version: 0.17.4.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -46,15 +46,15 @@
         
         
         
         # Basic Functions
         
         
         
-        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.2)
+        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.3)
         
         ###### Fri Jul 7 16:06:42 CST 2023
         
         ```python
         def rename_by_insert_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
             """
             功能：文件重命名或批量重命名。默认在文件名的后缀插入当前时间戳。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
```

### Comparing `pydatawork-0.17.4.2/README.md` & `pydatawork-0.17.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 
 # Basic Functions
 
 
 
-## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.2)
+## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.3)
 
 ###### Fri Jul 7 16:06:42 CST 2023
 
 ```python
 def rename_by_insert_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
     """
     功能：文件重命名或批量重命名。默认在文件名的后缀插入当前时间戳。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
```

### Comparing `pydatawork-0.17.4.2/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.4.3/pydatawork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.4.2
+Version: 0.17.4.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -46,15 +46,15 @@
         
         
         
         # Basic Functions
         
         
         
-        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.2)
+        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.3)
         
         ###### Fri Jul 7 16:06:42 CST 2023
         
         ```python
         def rename_by_insert_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
             """
             功能：文件重命名或批量重命名。默认在文件名的后缀插入当前时间戳。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
```

### Comparing `pydatawork-0.17.4.2/pydatawork.py` & `pydatawork-0.17.4.3/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.4.2/setup.py` & `pydatawork-0.17.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.4.2',
+    version='0.17.4.3',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

