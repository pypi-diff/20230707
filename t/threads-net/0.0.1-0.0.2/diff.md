# Comparing `tmp/threads-net-0.0.1.tar.gz` & `tmp/threads-net-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-net-0.0.1.tar", last modified: Fri Jul  7 09:51:21 2023, max compression
+gzip compressed data, was "threads-net-0.0.2.tar", last modified: Fri Jul  7 10:32:10 2023, max compression
```

## Comparing `threads-net-0.0.1.tar` & `threads-net-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:51:21.727810 threads-net-0.0.1/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.1/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      828 2023-07-07 09:51:21.727720 threads-net-0.0.1/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:44:29.000000 threads-net-0.0.1/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:51:21.726715 threads-net-0.0.1/examples/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.1/examples/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      305 2023-07-07 09:50:11.000000 threads-net-0.0.1/examples/get_post.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:51:21.726819 threads-net-0.0.1/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:44:21.000000 threads-net-0.0.1/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 09:51:21.727856 threads-net-0.0.1/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1227 2023-07-07 09:51:15.000000 threads-net-0.0.1/setup.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:51:21.727019 threads-net-0.0.1/threads/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.1/threads/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3175 2023-07-07 09:42:09.000000 threads-net-0.0.1/threads/main.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:51:21.727542 threads-net-0.0.1/threads_net.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      828 2023-07-07 09:51:21.000000 threads-net-0.0.1/threads_net.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      307 2023-07-07 09:51:21.000000 threads-net-0.0.1/threads_net.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 09:51:21.000000 threads-net-0.0.1/threads_net.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:51:21.000000 threads-net-0.0.1/threads_net.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:51:21.000000 threads-net-0.0.1/threads_net.egg-info/top_level.txt
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.559877 threads-net-0.0.2/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.2/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43404 2023-07-07 10:32:10.559777 threads-net-0.0.2/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    42575 2023-07-07 10:29:58.000000 threads-net-0.0.2/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.558661 threads-net-0.0.2/examples/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.2/examples/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      243 2023-07-07 10:23:26.000000 threads-net-0.0.2/examples/get_post.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      230 2023-07-07 10:23:34.000000 threads-net-0.0.2/examples/get_user.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      262 2023-07-07 10:23:42.000000 threads-net-0.0.2/examples/get_user_replies.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      264 2023-07-07 10:23:50.000000 threads-net-0.0.2/examples/get_user_threads.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.558761 threads-net-0.0.2/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:44:21.000000 threads-net-0.0.2/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 10:32:10.559912 threads-net-0.0.2/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1227 2023-07-07 10:31:48.000000 threads-net-0.0.2/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.558980 threads-net-0.0.2/threads/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.2/threads/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3175 2023-07-07 09:42:09.000000 threads-net-0.0.2/threads/main.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 10:32:10.559587 threads-net-0.0.2/threads_net.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43404 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      386 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 10:32:10.000000 threads-net-0.0.2/threads_net.egg-info/top_level.txt
```

### Comparing `threads-net-0.0.1/setup.py` & `threads-net-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('README.md', 'r') as read_me:
     long_description = read_me.read()
 
 with open('requirements/project.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version='0.0.1',
+    version='0.0.2',
     name='threads-net',
     description='Threads (threads.net) Python API wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/threads',
     license='MIT',
     author='Dmytro Striletskyi',
```

### Comparing `threads-net-0.0.1/threads/main.py` & `threads-net-0.0.2/threads/main.py`

 * *Files identical despite different names*

