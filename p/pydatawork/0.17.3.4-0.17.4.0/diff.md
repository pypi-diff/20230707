# Comparing `tmp/pydatawork-0.17.3.4.tar.gz` & `tmp/pydatawork-0.17.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.3.4.tar", last modified: Mon Jul  3 21:43:04 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.4.0.tar", last modified: Fri Jul  7 08:13:26 2023, max compression
```

## Comparing `pydatawork-0.17.3.4.tar` & `pydatawork-0.17.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    14084 2023-07-03 21:28:52.000000 pydatawork-0.17.3.4/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    45236 2023-07-03 21:42:07.000000 pydatawork-0.17.3.4/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 21:43:04.000000 pydatawork-0.17.3.4/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 21:27:07.000000 pydatawork-0.17.3.4/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19799 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    14968 2023-07-07 08:10:53.000000 pydatawork-0.17.4.0/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    19799 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    50495 2023-07-07 08:11:43.000000 pydatawork-0.17.4.0/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-07 08:13:26.000000 pydatawork-0.17.4.0/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-07 08:08:58.000000 pydatawork-0.17.4.0/setup.py
```

### Comparing `pydatawork-0.17.3.4/PKG-INFO` & `pydatawork-0.17.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.4
+Version: 0.17.4.0
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -45,14 +45,36 @@
         ```
         
         
         
         # Basic Functions
         
         
+        
+        ## rename_by_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.0)
+        
+        ###### Fri Jul 7 16:06:42 CST 2023
+        
+        ```python
+        def rename_by_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+            """
+            功能：文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
+        
+            参数：
+        
+            path：一个路径（文件或文件夹）。
+        
+            keyword：一个关键词（字符串），默认为当前时间戳。
+        
+            index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+            """
+        ```
+        
+        
+        
         ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
         
         ###### Mon Jul 3 21:21:23 CST 2023
         
         ```python
         def file_split():
             """
```

### Comparing `pydatawork-0.17.3.4/README.md` & `pydatawork-0.17.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,36 @@
 ```
 
 
 
 # Basic Functions
 
 
+
+## rename_by_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.0)
+
+###### Fri Jul 7 16:06:42 CST 2023
+
+```python
+def rename_by_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+    """
+    功能：文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
+
+    参数：
+
+    path：一个路径（文件或文件夹）。
+
+    keyword：一个关键词（字符串），默认为当前时间戳。
+
+    index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+    """
+```
+
+
+
 ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
 
 ###### Mon Jul 3 21:21:23 CST 2023
 
 ```python
 def file_split():
     """
```

### Comparing `pydatawork-0.17.3.4/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.4.0/pydatawork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.4
+Version: 0.17.4.0
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -45,14 +45,36 @@
         ```
         
         
         
         # Basic Functions
         
         
+        
+        ## rename_by_keyword() 在文件名的指定位置插入关键词，实现重命名或批量重命名 (v 0.17.4.0)
+        
+        ###### Fri Jul 7 16:06:42 CST 2023
+        
+        ```python
+        def rename_by_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+            """
+            功能：文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。
+        
+            参数：
+        
+            path：一个路径（文件或文件夹）。
+        
+            keyword：一个关键词（字符串），默认为当前时间戳。
+        
+            index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+            """
+        ```
+        
+        
+        
         ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
         
         ###### Mon Jul 3 21:21:23 CST 2023
         
         ```python
         def file_split():
             """
```

### Comparing `pydatawork-0.17.3.4/pydatawork.py` & `pydatawork-0.17.4.0/pydatawork.py`

 * *Files 12% similar despite different names*

```diff
@@ -198,14 +198,144 @@
 
 
 
 
 # Basic Functions
 
 
+# 重命名
+
+def rename_by_keyword(path, keyword=datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S"), index=-1):
+    """
+    功能：在文件名的指定位置插入关键词，进行文件重命名或批量重命名。需要给定一个路径（文件或文件夹），给定一个关键词（字符串），给定一个位置索引（从0开始），程序会对其中的文件（忽略子文件夹）进行重命名或批量重命名，命名方式为：把keyword添加到原文件名的指定位置。默认在文件名的后缀插入当前时间戳。
+
+    参数：
+
+    path：一个路径（文件或文件夹）。
+
+    keyword：一个关键词（字符串），默认为当前时间戳。
+
+    index：一个位置索引（从0开始。前缀位置索引为0，后缀位置索引为-1）。默认为-1。
+    """
+
+    path = path
+    keyword = keyword
+    index = index
+
+    # 检查输入参数是否正确，壁面参数混乱引发错误
+
+
+    def process_parameters(path, keyword, index):
+        # 验证path参数是否存在且类型正确
+        if not isinstance(path, str):
+            print("参数错误：path应为字符串类型")
+            return
+        
+        # 判断path是否输入
+        if path is None:
+            print("请输入路径")
+            return
+        
+        # 处理keyword和index参数的默认值
+        if keyword is None :
+            if index is None:
+                # keyword和index都使用默认值，将当前时刻的时间戳添加到文件名的后缀部分
+                print("未提供keyword和index参数，默认将当前时刻的时间戳添加到文件名的后缀部分")
+            else:
+                # keyword使用默认值，当前的时间戳
+                print("未提供keyword参数，默认值已设置为当前时间戳")
+        else:
+            if index is None:
+                # index使用默认值，-1
+                index = -1
+                print("未提供index参数，默认值已设置为-1")
+            
+        # 验证keyword参数类型是否正确
+        if keyword is not None and not isinstance(keyword, str):
+            print("参数错误：keyword应为字符串类型")
+            return
+        
+        # 验证index参数类型是否正确
+        if index is not None and not isinstance(index, int):
+            print("参数错误：index应为整数类型")
+            return # @知识卡片  return就代表程序中断运行
+        
+        # # 参数验证通过，继续处理其他逻辑
+        # print("参数验证通过")
+        # # 其他逻辑...
+
+    
+    def file_rename(path):
+        # 单个文件重命名
+        directory, filename = os.path.split(path)
+        name, extension = os.path.splitext(filename)  # @知识卡片 filename是包含后缀的
+        
+        # 考虑原文件名本身的长度，与index对比，确保index的值在有效范围
+        # 先考虑正向，同时考虑长度
+        if int(index) >= 0: # 为正时
+            if abs(index) < len(name): # 长度有效时继续
+                # 区分正负，写法不一样
+                if index == 0: # 前缀
+                    new_name = keyword + "_" + filename  # @知识卡片 filename是包含后缀的
+                    new_path = os.path.join(directory, new_name)
+                    os.rename(path, new_path)
+                    print(f"renaming: {filename} 为 {new_name}")
+
+                elif int(index) > 0:
+                    new_name = name[:index] + "_" + keyword + "_" + name[index:] + extension
+                    new_path = os.path.join(directory, new_name)
+                    os.rename(path, new_path)
+                    print(f"renaming: {filename} 为 {new_name}")
+            else:
+                print("index的值超出范围")
+
+        else: # 为负时
+            if -abs(index) >= -len(name): # 长度有效时继续
+                if index == -1: # 后缀
+                    new_name = name + "_" + keyword + extension  # @知识卡片 filename是包含后缀的
+                    new_path = os.path.join(directory, new_name)
+                    os.rename(path, new_path)
+                    print(f"renaming: {filename} 为 {new_name}")
+
+                else:
+                    new_name = name[:index+1] + "_" + keyword + "_" + name[index+1:] + extension
+                    new_path = os.path.join(directory, new_name)
+                    os.rename(path, new_path)
+                    print(f"renaming: {filename} 为 {new_name}")
+            else:
+                print("index的值超出范围")
+
+    # 参数验证    
+    process_parameters(path, keyword=None, index=None)
+
+    # 重命名
+    if os.path.isfile(path):
+        file_rename(path)
+    elif os.path.isdir(path):
+        # 文件夹中的文件批量重命名
+        for filename in os.listdir(path):
+            file_path = os.path.join(path, filename)
+            if os.path.isfile(file_path):
+                file_rename(file_path)
+            else:
+                continue # 不遍历子文件夹；直接进入下一个处理，而不是打断循环
+    # 找不到文件
+    else:
+        print("无效路径，请检查输入路径")
+
+
+
+
+# 文件备份
+
+def file_backup():
+    pass
+
+
+
 # 分割
 
 def file_split():
     """
     功能：对文件夹中的文件按指定数量进行拆分。（会忽略文件夹，只处理文件）。如，文件夹中有1000张图片，可将其拆分为10个小文件夹，每个文件夹100张图片，文件夹编号为1-10。
 
     参数：无需提前输入参数，执行后，根据终端中的提示进行输入。
```

### Comparing `pydatawork-0.17.3.4/setup.py` & `pydatawork-0.17.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.3.4',
+    version='0.17.4.0',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

