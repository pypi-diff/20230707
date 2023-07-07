# Comparing `tmp/p-template-crawler-0.0.84.tar.gz` & `tmp/p-template-crawler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-template-crawler-0.0.84.tar", last modified: Fri Jul  7 08:14:44 2023, max compression
+gzip compressed data, was "p-template-crawler-0.0.9.tar", last modified: Tue Mar 21 03:16:03 2023, max compression
```

## Comparing `p-template-crawler-0.0.84.tar` & `p-template-crawler-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 08:14:44.343087 p-template-crawler-0.0.84/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-template-crawler-0.0.84/LICENSE
--rw-rw-rw-   0        0        0      382 2023-07-07 08:14:44.343087 p-template-crawler-0.0.84/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-05 11:31:50.000000 p-template-crawler-0.0.84/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 08:14:44.335086 p-template-crawler-0.0.84/mecord_crawler/
--rw-rw-rw-   0        0        0        0 2023-07-05 11:31:50.000000 p-template-crawler-0.0.84/mecord_crawler/__init__.py
--rw-rw-rw-   0        0        0    11333 2023-06-29 07:31:58.000000 p-template-crawler-0.0.84/mecord_crawler/aaaapp_crawler.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:14:44.336087 p-template-crawler-0.0.84/mecord_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-07-05 11:31:50.000000 p-template-crawler-0.0.84/mecord_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0     5545 2023-05-16 02:14:40.000000 p-template-crawler-0.0.84/mecord_crawler/bin/gellary.txt.py
--rw-rw-rw-   0        0        0    11709 2023-05-27 03:28:34.000000 p-template-crawler-0.0.84/mecord_crawler/civitai_crawler.py
--rw-rw-rw-   0        0        0    20388 2023-07-07 08:14:17.000000 p-template-crawler-0.0.84/mecord_crawler/group_crawler.py
--rw-rw-rw-   0        0        0     2958 2023-07-06 03:26:01.000000 p-template-crawler-0.0.84/mecord_crawler/main.py
--rw-rw-rw-   0        0        0     1287 2023-05-27 03:28:34.000000 p-template-crawler-0.0.84/mecord_crawler/template_utils.py
--rw-rw-rw-   0        0        0      363 2023-06-26 10:18:59.000000 p-template-crawler-0.0.84/mecord_crawler/test.py
--rw-rw-rw-   0        0        0    13406 2023-07-03 07:33:30.000000 p-template-crawler-0.0.84/mecord_crawler/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:14:44.341088 p-template-crawler-0.0.84/p_template_crawler.egg-info/
--rw-rw-rw-   0        0        0      382 2023-07-07 08:14:44.000000 p-template-crawler-0.0.84/p_template_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-07-07 08:14:44.000000 p-template-crawler-0.0.84/p_template_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 08:14:44.000000 p-template-crawler-0.0.84/p_template_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-07 08:14:44.000000 p-template-crawler-0.0.84/p_template_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      136 2023-07-07 08:14:44.000000 p-template-crawler-0.0.84/p_template_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-07 08:14:44.000000 p-template-crawler-0.0.84/p_template_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 08:14:44.343087 p-template-crawler-0.0.84/setup.cfg
--rw-rw-rw-   0        0        0     1068 2023-07-07 08:14:36.000000 p-template-crawler-0.0.84/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-21 03:16:03.735860 p-template-crawler-0.0.9/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-template-crawler-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-03-21 03:16:03.735860 p-template-crawler-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-03-14 06:24:47.000000 p-template-crawler-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-21 03:16:03.728860 p-template-crawler-0.0.9/mecord_crawler/
+-rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 p-template-crawler-0.0.9/mecord_crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-21 03:16:03.729860 p-template-crawler-0.0.9/mecord_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 p-template-crawler-0.0.9/mecord_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0     6178 2023-03-21 02:07:32.000000 p-template-crawler-0.0.9/mecord_crawler/main.py
+-rw-rw-rw-   0        0        0     4989 2023-03-21 03:15:47.000000 p-template-crawler-0.0.9/mecord_crawler/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-21 03:16:03.734861 p-template-crawler-0.0.9/p_template_crawler.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-03-21 03:16:03.000000 p-template-crawler-0.0.9/p_template_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-03-21 03:16:03.000000 p-template-crawler-0.0.9/p_template_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-21 03:16:03.000000 p-template-crawler-0.0.9/p_template_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-03-21 03:16:03.000000 p-template-crawler-0.0.9/p_template_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-03-21 03:16:03.000000 p-template-crawler-0.0.9/p_template_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-03-21 03:16:03.000000 p-template-crawler-0.0.9/p_template_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-21 03:16:03.735860 p-template-crawler-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-03-21 03:15:55.000000 p-template-crawler-0.0.9/setup.py
```

### Comparing `p-template-crawler-0.0.84/LICENSE` & `p-template-crawler-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `p-template-crawler-0.0.84/setup.py` & `p-template-crawler-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-template-crawler",
-    version="0.0.84",
+    version="0.0.9",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -16,23 +16,14 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     py_modules=[],
     install_requires=[
         'requests',
         'oss2',
-        'Image',
-        'Pillow',
-        'fake_useragent',
-        'lxml',
-        'UserAgent',
-        'urlparser',
-        'p-template-generator>=0.1.71',
-        'p-template-res>=0.1.28',
-        'yt-dlp==2023.3.4',
     ],
     dependency_links=[],
     entry_points={
         'console_scripts':[
             'crawler = mecord_crawler.main:main'
         ]
     },
```

