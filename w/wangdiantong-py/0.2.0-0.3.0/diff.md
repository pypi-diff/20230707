# Comparing `tmp/wangdiantong-py-0.2.0.tar.gz` & `tmp/wangdiantong-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wangdiantong-py-0.2.0.tar", last modified: Thu Jul  6 09:43:02 2023, max compression
+gzip compressed data, was "wangdiantong-py-0.3.0.tar", last modified: Fri Jul  7 01:40:30 2023, max compression
```

## Comparing `wangdiantong-py-0.2.0.tar` & `wangdiantong-py-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     1068 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/LICENSE
--rw-rw-r--   0 xoss      (1000) xoss      (1000)      128 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/MANIFEST.in
--rw-r--r--   0 xoss      (1000) xoss      (1000)      744 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/PKG-INFO
--rw-rw-r--   0 xoss      (1000) xoss      (1000)      757 2023-07-06 09:41:26.000000 wangdiantong-py-0.2.0/README.md
--rw-rw-r--   0 xoss      (1000) xoss      (1000)      286 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/setup.cfg
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     2332 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/setup.py
-drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.769773 wangdiantong-py-0.2.0/wangdiantong/
--rw-r--r--   0 xoss      (1000) xoss      (1000)      212 2023-07-06 09:40:58.000000 wangdiantong-py-0.2.0/wangdiantong/__init__.py
-drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/wangdiantong/api/
--rw-rw-r--   0 xoss      (1000) xoss      (1000)      266 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/__init__.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)      868 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/base.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     8229 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/goods.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     1766 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/logistics.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     5022 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/order.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     3112 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/stocks.py
-drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/wangdiantong/client/
--rw-rw-r--   0 xoss      (1000) xoss      (1000)      574 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/client/__init__.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     3197 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/client/base.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)      502 2023-07-06 09:37:41.000000 wangdiantong-py-0.2.0/wangdiantong/settings.py
--rw-rw-r--   0 xoss      (1000) xoss      (1000)     1972 2023-07-06 09:31:27.000000 wangdiantong-py-0.2.0/wangdiantong/utils.py
-drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/
--rw-r--r--   0 xoss      (1000) xoss      (1000)      744 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/PKG-INFO
--rw-r--r--   0 xoss      (1000) xoss      (1000)      575 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/SOURCES.txt
--rw-r--r--   0 xoss      (1000) xoss      (1000)        1 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/dependency_links.txt
--rw-r--r--   0 xoss      (1000) xoss      (1000)        1 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/not-zip-safe
--rw-r--r--   0 xoss      (1000) xoss      (1000)       38 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/requires.txt
--rw-r--r--   0 xoss      (1000) xoss      (1000)       13 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/top_level.txt
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-07 01:40:30.719039 wangdiantong-py-0.3.0/
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     1068 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/LICENSE
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      128 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/MANIFEST.in
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      744 2023-07-07 01:40:30.719039 wangdiantong-py-0.3.0/PKG-INFO
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      757 2023-07-07 01:39:57.000000 wangdiantong-py-0.3.0/README.md
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      286 2023-07-07 01:40:30.719039 wangdiantong-py-0.3.0/setup.cfg
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     2339 2023-07-07 01:39:35.000000 wangdiantong-py-0.3.0/setup.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-07 01:40:30.715039 wangdiantong-py-0.3.0/wangdiantong/
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      208 2023-07-07 01:39:48.000000 wangdiantong-py-0.3.0/wangdiantong/__init__.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-07 01:40:30.719039 wangdiantong-py-0.3.0/wangdiantong/api/
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      266 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/api/__init__.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      868 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/api/base.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     8229 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/api/goods.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     1766 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/api/logistics.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     5022 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/api/order.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     3112 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/api/stocks.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-07 01:40:30.719039 wangdiantong-py-0.3.0/wangdiantong/client/
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      574 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/client/__init__.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     3197 2023-07-06 09:16:39.000000 wangdiantong-py-0.3.0/wangdiantong/client/base.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      502 2023-07-06 09:37:41.000000 wangdiantong-py-0.3.0/wangdiantong/settings.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     1972 2023-07-06 09:31:27.000000 wangdiantong-py-0.3.0/wangdiantong/utils.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-07 01:40:30.719039 wangdiantong-py-0.3.0/wangdiantong_py.egg-info/
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      744 2023-07-07 01:40:30.000000 wangdiantong-py-0.3.0/wangdiantong_py.egg-info/PKG-INFO
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      575 2023-07-07 01:40:30.000000 wangdiantong-py-0.3.0/wangdiantong_py.egg-info/SOURCES.txt
+-rw-r--r--   0 xoss      (1000) xoss      (1000)        1 2023-07-07 01:40:30.000000 wangdiantong-py-0.3.0/wangdiantong_py.egg-info/dependency_links.txt
+-rw-r--r--   0 xoss      (1000) xoss      (1000)        1 2023-07-06 09:43:02.000000 wangdiantong-py-0.3.0/wangdiantong_py.egg-info/not-zip-safe
+-rw-r--r--   0 xoss      (1000) xoss      (1000)       42 2023-07-07 01:40:30.000000 wangdiantong-py-0.3.0/wangdiantong_py.egg-info/requires.txt
+-rw-r--r--   0 xoss      (1000) xoss      (1000)       13 2023-07-07 01:40:30.000000 wangdiantong-py-0.3.0/wangdiantong_py.egg-info/top_level.txt
```

### Comparing `wangdiantong-py-0.2.0/LICENSE` & `wangdiantong-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/PKG-INFO` & `wangdiantong-py-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wangdiantong-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: wangdiantong python openapi
 Home-page: https://github.com/AoAoStudio/wangdiantong-py
 Author: Ranger Huang
 Author-email: ranger_huang@yeah.net
 Keywords: wangdiantong
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wangdiantong-py-0.2.0/README.md` & `wangdiantong-py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/setup.py` & `wangdiantong-py-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         readme = readme_file.read()
 
     # with open(join(LIB_DIR, 'HISTORY.md')) as history_file:
     #     history = history_file.read()
     # return readme + '\n\n' + history
 
 
-requirements = ['certifi', 'chardet', 'idna', 'requests', 'urllib3']
+requirements = ['certifi', 'chardet', 'idna', 'requests', 'urllib3', 'six']
 
 test_requirements = ['appnope==0.1.0', 'atomicwrites==1.1.5', 'attrs==18.1.0', 'backports.shutil-get-terminal-size==1.0.0', 'bumpversion==0.5.3', 'cov-core==1.15.0', 'coverage==4.5.1', 'decorator==4.3.0', 'enum34==1.1.6', 'funcsigs==1.0.2', 'ipython-genutils==0.2.0', 'ipython==5.7.0', 'lxml==4.2.1', 'more-itertools==4.2.0', 'namedlist==1.7',
                      'nose-allure-plugin==1.0.5', 'nose-cov==1.6', 'nose==1.3.7', 'pathlib2==2.3.2', 'pexpect==4.5.0', 'pickleshare==0.7.4', 'pluggy==0.6.0', 'prompt-toolkit==1.0.15', 'ptyprocess==0.5.2', 'py==1.5.3', 'pygments==2.2.0', 'pytest-allure-adaptor==1.7.10', 'pytest==3.6.0', 'scandir==1.7', 'simplegeneric==0.8.1', 'six==1.11.0', 'traitlets==4.3.2', 'wcwidth==0.1.7']
 
 
 setup(
     name='wangdiantong-py',
```

### Comparing `wangdiantong-py-0.2.0/wangdiantong/api/base.py` & `wangdiantong-py-0.3.0/wangdiantong/api/base.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong/api/goods.py` & `wangdiantong-py-0.3.0/wangdiantong/api/goods.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong/api/logistics.py` & `wangdiantong-py-0.3.0/wangdiantong/api/logistics.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong/api/order.py` & `wangdiantong-py-0.3.0/wangdiantong/api/order.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong/api/stocks.py` & `wangdiantong-py-0.3.0/wangdiantong/api/stocks.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong/client/__init__.py` & `wangdiantong-py-0.3.0/wangdiantong/client/__init__.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong/client/base.py` & `wangdiantong-py-0.3.0/wangdiantong/client/base.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong/utils.py` & `wangdiantong-py-0.3.0/wangdiantong/utils.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.2.0/wangdiantong_py.egg-info/PKG-INFO` & `wangdiantong-py-0.3.0/wangdiantong_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wangdiantong-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: wangdiantong python openapi
 Home-page: https://github.com/AoAoStudio/wangdiantong-py
 Author: Ranger Huang
 Author-email: ranger_huang@yeah.net
 Keywords: wangdiantong
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wangdiantong-py-0.2.0/wangdiantong_py.egg-info/SOURCES.txt` & `wangdiantong-py-0.3.0/wangdiantong_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

