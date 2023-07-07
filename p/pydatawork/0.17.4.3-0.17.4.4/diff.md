# Comparing `tmp/pydatawork-0.17.4.3.tar.gz` & `tmp/pydatawork-0.17.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.4.3.tar", last modified: Fri Jul  7 08:32:00 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.4.4.tar", last modified: Fri Jul  7 10:34:07 2023, max compression
```

## Comparing `pydatawork-0.17.4.3.tar` & `pydatawork-0.17.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19864 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15033 2023-07-07 08:31:32.000000 pydatawork-0.17.4.3/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19864 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    50502 2023-07-07 08:28:32.000000 pydatawork-0.17.4.3/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-07 08:32:00.000000 pydatawork-0.17.4.3/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-07 08:31:25.000000 pydatawork-0.17.4.3/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20019 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15188 2023-07-07 10:33:21.000000 pydatawork-0.17.4.4/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20019 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    50594 2023-07-07 10:33:01.000000 pydatawork-0.17.4.4/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-07 10:34:07.000000 pydatawork-0.17.4.4/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-07 10:25:37.000000 pydatawork-0.17.4.4/setup.py
```

### Comparing `pydatawork-0.17.4.3/PKG-INFO` & `pydatawork-0.17.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.4.3
+Version: 0.17.4.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -46,30 +46,30 @@
         
         
         
         # Basic Functions
         
         
         
-        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.3)
+        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词（默认为当前时间戳），实现重命名或批量重命名 (v 0.17.4.4)
         
         ###### Fri Jul 7 16:06:42 CST 2023
         
         ```python
-        def rename_by_insert_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+        def rename_by_insert_keyword(path, index:int=-1,keyword:str=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")):
             """
-            功能：文件重命名或批量重命名。默认在文件名的后缀插入当前时间戳。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
+            功能：在文件名的指定位置插入关键词，进行文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个位置索引（从0开始），给定一个关键词（字符串），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。index和keyword有默认值，默认在文件名的后缀插入当前时间戳。
         
             参数：
         
             path：一个路径（文件或文件夹）。
         
-            keyword：一个关键词（字符串），默认为当前时间戳。
-        
             index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+            
+            keyword：一个关键词（字符串）。默认为当前时间戳(格式为：2023-07-07_18-17-13)。
             """
         ```
         
         
         
         ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
```

### Comparing `pydatawork-0.17.4.3/README.md` & `pydatawork-0.17.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,30 +38,30 @@
 
 
 
 # Basic Functions
 
 
 
-## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.3)
+## rename_by_insert_keyword() 在文件名的指定位置插入关键词（默认为当前时间戳），实现重命名或批量重命名 (v 0.17.4.4)
 
 ###### Fri Jul 7 16:06:42 CST 2023
 
 ```python
-def rename_by_insert_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+def rename_by_insert_keyword(path, index:int=-1,keyword:str=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")):
     """
-    功能：文件重命名或批量重命名。默认在文件名的后缀插入当前时间戳。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
+    功能：在文件名的指定位置插入关键词，进行文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个位置索引（从0开始），给定一个关键词（字符串），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。index和keyword有默认值，默认在文件名的后缀插入当前时间戳。
 
     参数：
 
     path：一个路径（文件或文件夹）。
 
-    keyword：一个关键词（字符串），默认为当前时间戳。
-
     index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+    
+    keyword：一个关键词（字符串）。默认为当前时间戳(格式为：2023-07-07_18-17-13)。
     """
 ```
 
 
 
 ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
```

### Comparing `pydatawork-0.17.4.3/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.4.4/pydatawork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.4.3
+Version: 0.17.4.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -46,30 +46,30 @@
         
         
         
         # Basic Functions
         
         
         
-        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.3)
+        ## rename_by_insert_keyword() 在文件名的指定位置插入关键词（默认为当前时间戳），实现重命名或批量重命名 (v 0.17.4.4)
         
         ###### Fri Jul 7 16:06:42 CST 2023
         
         ```python
-        def rename_by_insert_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+        def rename_by_insert_keyword(path, index:int=-1,keyword:str=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")):
             """
-            功能：文件重命名或批量重命名。默认在文件名的后缀插入当前时间戳。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
+            功能：在文件名的指定位置插入关键词，进行文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个位置索引（从0开始），给定一个关键词（字符串），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。index和keyword有默认值，默认在文件名的后缀插入当前时间戳。
         
             参数：
         
             path：一个路径（文件或文件夹）。
         
-            keyword：一个关键词（字符串），默认为当前时间戳。
-        
             index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+            
+            keyword：一个关键词（字符串）。默认为当前时间戳(格式为：2023-07-07_18-17-13)。
             """
         ```
         
         
         
         ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
```

### Comparing `pydatawork-0.17.4.3/pydatawork.py` & `pydatawork-0.17.4.4/pydatawork.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,74 +200,57 @@
 
 
 # Basic Functions
 
 
 # 重命名
 
-def rename_by_insert_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+def rename_by_insert_keyword(path, index:int=-1,keyword:str=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")):
     """
-    功能：在文件名的指定位置插入关键词，进行文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。默认在文件名的后缀插入当前时间戳。
+    功能：在文件名的指定位置插入关键词，进行文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个位置索引（从0开始），给定一个关键词（字符串），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。index和keyword有默认值，默认在文件名的后缀插入当前时间戳。
 
     参数：
 
     path：一个路径（文件或文件夹）。
 
-    keyword：一个关键词（字符串），默认为当前时间戳。
-
     index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+    
+    keyword：一个关键词（字符串）。默认为当前时间戳(格式为：2023-07-07_18-17-13)。
     """
 
     path = path
-    keyword = keyword
     index = index
+    keyword = keyword
 
-    # 检查输入参数是否正确，壁面参数混乱引发错误
-
-
-    def process_parameters(path, keyword, index):
-        # 验证path参数是否存在且类型正确
-        if not isinstance(path, str):
-            print("参数错误：path应为字符串类型")
-            return
-        
-        # 判断path是否输入
+    # 检查输入参数的值是否正确——只需要验证“可设为默认值的参数的值”，以便提醒用户
+    def default_value_prompt(path,index,keyword):
+        # 判断path是否输入  （这里不做判断，系统也会自动判断。因为path在函数中是必须输入的参数，少了，会报错。）
         if path is None:
             print("请输入路径")
             return
         
         # 处理keyword和index参数的默认值
-        if keyword is None :
-            if index is None:
+        # if keyword is None : # 因为，当keyword和index为默认值的时候，默认值也是个具体的值，这已经在函数定义中写具体了，所以，这里不能用None，因为肯定不是None。keyword如果没有专门输入，那keyword的值应为：keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+
+        if keyword == datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S") : 
+            if index == -1:
                 # keyword和index都使用默认值，将当前时刻的时间戳添加到文件名的后缀部分
-                print("未提供keyword和index参数，默认将当前时刻的时间戳添加到文件名的后缀部分")
+                print("由于未提供keyword和index参数，默认将当前时刻的时间戳添加到文件名的后缀部分（keyword的默认值为当前时间戳，index的默认值为-1）")
             else:
                 # keyword使用默认值，当前的时间戳
-                print("未提供keyword参数，默认值已设置为当前时间戳")
+                print("由于未提供keyword参数，keyword默认已设置为当前时间戳")
         else:
-            if index is None:
+            if index == -1:
                 # index使用默认值，-1
                 index = -1
-                print("未提供index参数，默认值已设置为-1")
-            
-        # 验证keyword参数类型是否正确
-        if keyword is not None and not isinstance(keyword, str):
-            print("参数错误：keyword应为字符串类型")
-            return
-        
-        # 验证index参数类型是否正确
-        if index is not None and not isinstance(index, int):
-            print("参数错误：index应为整数类型")
-            return # @知识卡片  return就代表程序中断运行
-        
-        # # 参数验证通过，继续处理其他逻辑
-        # print("参数验证通过")
-        # # 其他逻辑...
+                print("由于未提供index参数，index默认已设置为-1")
+
+        # # 验证keyword参数类型是否正确   （参数的数据类型，已经在函数定义中指定，不需要在这里再次验证）
+
 
-    
     def file_rename(path):
         # 单个文件重命名
         directory, filename = os.path.split(path)
         name, extension = os.path.splitext(filename)  # @知识卡片 filename是包含后缀的
         
         # 考虑原文件名本身的长度，与index对比，确保index的值在有效范围
         # 先考虑正向，同时考虑长度
@@ -300,16 +283,17 @@
                     new_name = name[:index+1] + "_" + keyword + "_" + name[index+1:] + extension
                     new_path = os.path.join(directory, new_name)
                     os.rename(path, new_path)
                     print(f"renaming: {filename} 为 {new_name}")
             else:
                 print("index的值超出范围")
 
+
     # 参数验证    
-    process_parameters(path, keyword=None, index=None)
+    default_value_prompt(path, keyword, index)
 
     # 重命名
     if os.path.isfile(path):
         file_rename(path)
     elif os.path.isdir(path):
         # 文件夹中的文件批量重命名
         for filename in os.listdir(path):
```

### Comparing `pydatawork-0.17.4.3/setup.py` & `pydatawork-0.17.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.4.3',
+    version='0.17.4.4',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

