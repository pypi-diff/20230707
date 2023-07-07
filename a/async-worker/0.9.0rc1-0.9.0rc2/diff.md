# Comparing `tmp/async-worker-0.9.0rc1.tar.gz` & `tmp/async-worker-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/async-worker-0.9.0rc1.tar", last modified: Sun Feb 17 16:15:53 2019, max compression
+gzip compressed data, was "dist/async-worker-0.9.0rc2.tar", last modified: Sun Feb 17 17:14:02 2019, max compression
```

## Comparing `async-worker-0.9.0rc1.tar` & `async-worker-0.9.0rc2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/
--rw-r--r--   0 diogo      (501) staff       (20)      428 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/PKG-INFO
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/asyncworker/
--rw-r--r--   0 diogo      (501) staff       (20)      545 2019-02-10 19:35:41.000000 async-worker-0.9.0rc1/asyncworker/options.py
--rw-r--r--   0 diogo      (501) staff       (20)     1763 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/time.py
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/asyncworker/sse/
--rw-r--r--   0 diogo      (501) staff       (20)        0 2018-11-30 11:52:06.000000 async-worker-0.9.0rc1/asyncworker/sse/__init__.py
--rw-r--r--   0 diogo      (501) staff       (20)      199 2018-11-30 11:52:06.000000 async-worker-0.9.0rc1/asyncworker/sse/message.py
--rw-r--r--   0 diogo      (501) staff       (20)     4086 2019-01-05 12:59:50.000000 async-worker-0.9.0rc1/asyncworker/sse/consumer.py
--rw-r--r--   0 diogo      (501) staff       (20)      624 2018-12-19 01:44:12.000000 async-worker-0.9.0rc1/asyncworker/sse/app.py
--rw-r--r--   0 diogo      (501) staff       (20)      863 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/bucket.py
--rw-r--r--   0 diogo      (501) staff       (20)      524 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/conf.py
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/asyncworker/signals/
--rw-r--r--   0 diogo      (501) staff       (20)        0 2018-11-30 11:52:06.000000 async-worker-0.9.0rc1/asyncworker/signals/__init__.py
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/asyncworker/signals/handlers/
--rw-r--r--   0 diogo      (501) staff       (20)        0 2018-11-30 11:52:06.000000 async-worker-0.9.0rc1/asyncworker/signals/handlers/__init__.py
--rw-r--r--   0 diogo      (501) staff       (20)      770 2019-01-05 12:59:50.000000 async-worker-0.9.0rc1/asyncworker/signals/handlers/sse.py
--rw-r--r--   0 diogo      (501) staff       (20)     1039 2019-01-05 12:59:50.000000 async-worker-0.9.0rc1/asyncworker/signals/handlers/rabbitmq.py
--rw-r--r--   0 diogo      (501) staff       (20)     1027 2019-02-10 19:35:41.000000 async-worker-0.9.0rc1/asyncworker/signals/handlers/http.py
--rw-r--r--   0 diogo      (501) staff       (20)      291 2018-12-19 01:44:12.000000 async-worker-0.9.0rc1/asyncworker/signals/handlers/base.py
--rw-r--r--   0 diogo      (501) staff       (20)     1058 2018-12-19 01:44:12.000000 async-worker-0.9.0rc1/asyncworker/signals/base.py
--rw-r--r--   0 diogo      (501) staff       (20)      610 2018-12-21 00:46:32.000000 async-worker-0.9.0rc1/asyncworker/__init__.py
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/asyncworker/rabbitmq/
--rw-r--r--   0 diogo      (501) staff       (20)       51 2018-12-19 01:44:12.000000 async-worker-0.9.0rc1/asyncworker/rabbitmq/__init__.py
--rw-r--r--   0 diogo      (501) staff       (20)     1427 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/rabbitmq/message.py
--rw-r--r--   0 diogo      (501) staff       (20)     1741 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/rabbitmq/connection.py
--rw-r--r--   0 diogo      (501) staff       (20)     7000 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/consumer.py
--rw-r--r--   0 diogo      (501) staff       (20)     1944 2018-12-19 01:44:12.000000 async-worker-0.9.0rc1/asyncworker/utils.py
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/asyncworker/easyqueue/
--rw-r--r--   0 diogo      (501) staff       (20)    11091 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/easyqueue/queue.py
--rw-r--r--   0 diogo      (501) staff       (20)        0 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/easyqueue/__init__.py
--rw-r--r--   0 diogo      (501) staff       (20)     2121 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/asyncworker/easyqueue/message.py
--rw-r--r--   0 diogo      (501) staff       (20)     1970 2019-02-10 20:59:46.000000 async-worker-0.9.0rc1/asyncworker/easyqueue/connection.py
--rw-r--r--   0 diogo      (501) staff       (20)      407 2019-02-10 20:59:46.000000 async-worker-0.9.0rc1/asyncworker/easyqueue/exceptions.py
--rw-r--r--   0 diogo      (501) staff       (20)     4562 2019-01-05 12:59:50.000000 async-worker-0.9.0rc1/asyncworker/base.py
--rw-r--r--   0 diogo      (501) staff       (20)     1895 2018-12-21 00:46:32.000000 async-worker-0.9.0rc1/asyncworker/task_runners.py
--rw-r--r--   0 diogo      (501) staff       (20)     3126 2019-02-10 19:35:41.000000 async-worker-0.9.0rc1/asyncworker/routes.py
-drwxr-xr-x   0 diogo      (501) staff       (20)        0 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/async_worker.egg-info/
--rw-r--r--   0 diogo      (501) staff       (20)      428 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/async_worker.egg-info/PKG-INFO
--rw-r--r--   0 diogo      (501) staff       (20)     1049 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/async_worker.egg-info/SOURCES.txt
--rw-r--r--   0 diogo      (501) staff       (20)       86 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/async_worker.egg-info/requires.txt
--rw-r--r--   0 diogo      (501) staff       (20)       12 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/async_worker.egg-info/top_level.txt
--rw-r--r--   0 diogo      (501) staff       (20)        1 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/async_worker.egg-info/dependency_links.txt
--rw-r--r--   0 diogo      (501) staff       (20)    17478 2019-02-17 16:14:01.000000 async-worker-0.9.0rc1/README.md
--rw-r--r--   0 diogo      (501) staff       (20)      904 2019-02-17 16:14:36.000000 async-worker-0.9.0rc1/setup.py
--rw-r--r--   0 diogo      (501) staff       (20)       38 2019-02-17 16:15:53.000000 async-worker-0.9.0rc1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17478 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/asyncworker/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7000 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/consumer.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/asyncworker/rabbitmq/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1741 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/rabbitmq/connection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1427 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/rabbitmq/message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/rabbitmq/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1895 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/task_runners.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/asyncworker/sse/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4086 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/sse/consumer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/sse/message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/sse/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      624 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/sse/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3126 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/routes.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/asyncworker/easyqueue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11091 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/easyqueue/queue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      407 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/easyqueue/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1970 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/easyqueue/connection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2121 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/easyqueue/message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/easyqueue/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1763 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/time.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      524 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1944 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/asyncworker/signals/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/asyncworker/signals/handlers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1039 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/signals/handlers/rabbitmq.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1027 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/signals/handlers/http.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      770 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/signals/handlers/sse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      291 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/signals/handlers/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/signals/handlers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1058 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/signals/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/signals/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      863 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/bucket.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4562 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/options.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/asyncworker/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/async_worker.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/async_worker.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/async_worker.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/async_worker.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/async_worker.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       90 2019-02-17 17:14:02.000000 async-worker-0.9.0rc2/async_worker.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      908 2019-02-17 17:12:27.000000 async-worker-0.9.0rc2/setup.py
```

### Comparing `async-worker-0.9.0rc1/asyncworker/options.py` & `async-worker-0.9.0rc2/asyncworker/options.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/time.py` & `async-worker-0.9.0rc2/asyncworker/time.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/sse/consumer.py` & `async-worker-0.9.0rc2/asyncworker/sse/consumer.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/sse/app.py` & `async-worker-0.9.0rc2/asyncworker/sse/app.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/bucket.py` & `async-worker-0.9.0rc2/asyncworker/bucket.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/conf.py` & `async-worker-0.9.0rc2/asyncworker/conf.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/signals/handlers/sse.py` & `async-worker-0.9.0rc2/asyncworker/signals/handlers/sse.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/signals/handlers/rabbitmq.py` & `async-worker-0.9.0rc2/asyncworker/signals/handlers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/signals/handlers/http.py` & `async-worker-0.9.0rc2/asyncworker/signals/handlers/http.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/signals/base.py` & `async-worker-0.9.0rc2/asyncworker/signals/base.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/__init__.py` & `async-worker-0.9.0rc2/asyncworker/__init__.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/rabbitmq/message.py` & `async-worker-0.9.0rc2/asyncworker/rabbitmq/message.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/rabbitmq/connection.py` & `async-worker-0.9.0rc2/asyncworker/rabbitmq/connection.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/consumer.py` & `async-worker-0.9.0rc2/asyncworker/consumer.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/utils.py` & `async-worker-0.9.0rc2/asyncworker/utils.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/easyqueue/queue.py` & `async-worker-0.9.0rc2/asyncworker/easyqueue/queue.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/easyqueue/message.py` & `async-worker-0.9.0rc2/asyncworker/easyqueue/message.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/easyqueue/connection.py` & `async-worker-0.9.0rc2/asyncworker/easyqueue/connection.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/base.py` & `async-worker-0.9.0rc2/asyncworker/base.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/task_runners.py` & `async-worker-0.9.0rc2/asyncworker/task_runners.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/asyncworker/routes.py` & `async-worker-0.9.0rc2/asyncworker/routes.py`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/async_worker.egg-info/SOURCES.txt` & `async-worker-0.9.0rc2/async_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/README.md` & `async-worker-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `async-worker-0.9.0rc1/setup.py` & `async-worker-0.9.0rc2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from setuptools import setup, find_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="async-worker",
-    version="0.9.0-rc1",
+    version="0.9.0-rc2",
     description="Microframework para escrever consumers para RabbitMQ",
     long_description="Microframework para escrever consumers para RabbitMQ",
     url="https://github.com/B2W-BIT/async-worker",
     # Author details
     author="Dalton Barreto",
     author_email="daltonmatos@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     install_requires=[
         "aioamqp==0.12.0",
-        "aiologger==0.3.0",
+        "aiologger>=0.4.0-rc1",
         "pydantic==0.14",
         "cached-property==1.5.1",
         "aiohttp==3.4.4",
     ],
     entry_points={},
 )
```

