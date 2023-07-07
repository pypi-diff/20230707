# Comparing `tmp/vgis_database-1.0.1.tar.gz` & `tmp/vgis_database-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_database-1.0.1.tar", last modified: Tue Jun 27 09:21:33 2023, max compression
+gzip compressed data, was "dist\vgis_database-1.0.2.tar", last modified: Fri Jul  7 09:41:21 2023, max compression
```

## Comparing `vgis_database-1.0.1.tar` & `vgis_database-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:21:33.770305 vgis_database-1.0.1/
--rw-rw-rw-   0        0        0     1047 2023-06-27 09:21:33.769339 vgis_database-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-27 09:06:18.000000 vgis_database-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 09:21:33.770305 vgis_database-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2183 2023-06-27 09:11:20.000000 vgis_database-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:21:33.759306 vgis_database-1.0.1/vgis_database/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_database-1.0.1/vgis_database/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-06-27 06:41:10.000000 vgis_database-1.0.1/vgis_database/pgTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:21:33.767305 vgis_database-1.0.1/vgis_database.egg-info/
--rw-rw-rw-   0        0        0     1047 2023-06-27 09:21:33.000000 vgis_database-1.0.1/vgis_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-27 09:21:33.000000 vgis_database-1.0.1/vgis_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:21:33.000000 vgis_database-1.0.1/vgis_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 09:21:33.000000 vgis_database-1.0.1/vgis_database.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-27 09:21:33.000000 vgis_database-1.0.1/vgis_database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 09:41:21.905372 vgis_database-1.0.2/
+-rw-rw-rw-   0        0        0     1047 2023-07-07 09:41:21.905372 vgis_database-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-27 09:06:18.000000 vgis_database-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 09:41:21.906343 vgis_database-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2196 2023-07-07 09:40:47.000000 vgis_database-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:41:21.895344 vgis_database-1.0.2/vgis_database/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_database-1.0.2/vgis_database/__init__.py
+-rw-rw-rw-   0        0        0     2630 2023-07-07 09:38:17.000000 vgis_database-1.0.2/vgis_database/pgTools.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:41:21.903344 vgis_database-1.0.2/vgis_database.egg-info/
+-rw-rw-rw-   0        0        0     1047 2023-07-07 09:41:21.000000 vgis_database-1.0.2/vgis_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-07-07 09:41:21.000000 vgis_database-1.0.2/vgis_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 09:41:21.000000 vgis_database-1.0.2/vgis_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-07 09:41:21.000000 vgis_database-1.0.2/vgis_database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 09:41:21.000000 vgis_database-1.0.2/vgis_database.egg-info/top_level.txt
```

### Comparing `vgis_database-1.0.1/PKG-INFO` & `vgis_database-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_database
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for database operator
 Home-page: https://github.com/gisfanmachel/vgisDatabase
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis database lib
```

### Comparing `vgis_database-1.0.1/setup.py` & `vgis_database-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_database",  # Required 项目名称
-    version="1.0.1",  # Required 发布版本号
+    version="1.0.2",  # Required 发布版本号
     description="A libary for database operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisDatabase",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
@@ -48,10 +48,10 @@
 
     keywords="database,setuptools,development",  # Optional 搜索关键字
 
     packages=find_packages(),  # Required
 
     python_requires=">=3.7, <4",  # python 版本要求
 
-    install_requires=["psycopg2-binary","vgis-utils"],  # Optional 第三方依赖库
+    install_requires=["psycopg2-binary", "vgis-utils", "loguru"],  # Optional 第三方依赖库
 
-)
+)
```

### Comparing `vgis_database-1.0.1/vgis_database.egg-info/PKG-INFO` & `vgis_database-1.0.2/vgis_database.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-database
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for database operator
 Home-page: https://github.com/gisfanmachel/vgisDatabase
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis database lib
```

