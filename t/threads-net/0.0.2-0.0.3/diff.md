# Comparing `tmp/threads-net-0.0.2.tar.gz` & `tmp/threads-net-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-net-0.0.2.tar", last modified: Fri Jul  7 10:32:10 2023, max compression
+gzip compressed data, was "threads-net-0.0.3.tar", last modified: Fri Jul  7 11:49:54 2023, max compression
```

## Comparing `threads-net-0.0.2.tar` & `threads-net-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.559877 threads-net-0.0.2/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.2/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43404 2023-07-07 10:32:10.559777 threads-net-0.0.2/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    42575 2023-07-07 10:29:58.000000 threads-net-0.0.2/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.558661 threads-net-0.0.2/examples/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.2/examples/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      243 2023-07-07 10:23:26.000000 threads-net-0.0.2/examples/get_post.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      230 2023-07-07 10:23:34.000000 threads-net-0.0.2/examples/get_user.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      262 2023-07-07 10:23:42.000000 threads-net-0.0.2/examples/get_user_replies.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      264 2023-07-07 10:23:50.000000 threads-net-0.0.2/examples/get_user_threads.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.558761 threads-net-0.0.2/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:44:21.000000 threads-net-0.0.2/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 10:32:10.559912 threads-net-0.0.2/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1227 2023-07-07 10:31:48.000000 threads-net-0.0.2/setup.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.558980 threads-net-0.0.2/threads/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.2/threads/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3175 2023-07-07 09:42:09.000000 threads-net-0.0.2/threads/main.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.559587 threads-net-0.0.2/threads_net.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43404 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      386 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/top_level.txt
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.642738 threads-net-0.0.3/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.3/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.3/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43426 2023-07-07 11:49:54.642630 threads-net-0.0.3/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    42575 2023-07-07 10:29:58.000000 threads-net-0.0.3/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.641565 threads-net-0.0.3/examples/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.3/examples/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      243 2023-07-07 10:23:26.000000 threads-net-0.0.3/examples/get_post.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      230 2023-07-07 10:23:34.000000 threads-net-0.0.3/examples/get_user.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      262 2023-07-07 10:23:42.000000 threads-net-0.0.3/examples/get_user_replies.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      264 2023-07-07 10:23:50.000000 threads-net-0.0.3/examples/get_user_threads.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.641666 threads-net-0.0.3/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:44:21.000000 threads-net-0.0.3/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 11:49:54.642771 threads-net-0.0.3/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-07 11:49:26.000000 threads-net-0.0.3/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.641912 threads-net-0.0.3/threads/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.3/threads/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3175 2023-07-07 09:42:09.000000 threads-net-0.0.3/threads/main.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.642440 threads-net-0.0.3/threads_net.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43426 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      394 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/top_level.txt
```

### Comparing `threads-net-0.0.2/PKG-INFO` & `threads-net-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.2
+Version: 0.0.3
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
```

### Comparing `threads-net-0.0.2/README.md` & `threads-net-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `threads-net-0.0.2/setup.py` & `threads-net-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Setup the package.
 """
 from setuptools import find_packages, setup
 
-with open('README.md', 'r') as read_me:
+with open('README.md', 'r', encoding='utf-8') as read_me:
     long_description = read_me.read()
 
 with open('requirements/project.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version='0.0.2',
+    version='0.0.3',
     name='threads-net',
     description='Threads (threads.net) Python API wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/threads',
     license='MIT',
     author='Dmytro Striletskyi',
```

### Comparing `threads-net-0.0.2/threads/main.py` & `threads-net-0.0.3/threads/main.py`

 * *Files identical despite different names*

### Comparing `threads-net-0.0.2/threads_net.egg-info/PKG-INFO` & `threads-net-0.0.3/threads_net.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.2
+Version: 0.0.3
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
```

