# Comparing `tmp/w3bstream_client_python-0.4.3.tar.gz` & `tmp/w3bstream_client_python-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-0.4.3.tar", last modified: Mon Jul  3 17:51:39 2023, max compression
+gzip compressed data, was "w3bstream_client_python-0.4.4.tar", last modified: Fri Jul  7 18:19:58 2023, max compression
```

## Comparing `w3bstream_client_python-0.4.3.tar` & `w3bstream_client_python-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-03 17:51:39.019818 w3bstream_client_python-0.4.3/
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.3/.gitignore
--rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.3/LICENSE
--rw-r--r--   0 haaai     (1000) haaai     (1000)      855 2023-07-03 17:51:39.019818 w3bstream_client_python-0.4.3/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      679 2023-06-30 21:10:19.000000 w3bstream_client_python-0.4.3/README.md
--rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-03 17:50:56.000000 w3bstream_client_python-0.4.3/pyproject.toml
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-03 17:51:39.019818 w3bstream_client_python-0.4.3/setup.cfg
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-03 17:51:39.019818 w3bstream_client_python-0.4.3/src/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-03 17:26:30.000000 w3bstream_client_python-0.4.3/src/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3852 2023-07-03 17:26:30.000000 w3bstream_client_python-0.4.3/src/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-03 17:51:39.019818 w3bstream_client_python-0.4.3/src/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      855 2023-07-03 17:51:39.000000 w3bstream_client_python-0.4.3/src/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      327 2023-07-03 17:51:39.000000 w3bstream_client_python-0.4.3/src/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-03 17:51:39.000000 w3bstream_client_python-0.4.3/src/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-03 17:51:39.000000 w3bstream_client_python-0.4.3/src/w3bstream_client_python.egg-info/requires.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       16 2023-07-03 17:51:39.000000 w3bstream_client_python-0.4.3/src/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.4/.gitignore
+-rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.4/LICENSE
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      810 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      634 2023-07-07 16:58:52.000000 w3bstream_client_python-0.4.4/README.md
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-07 18:19:43.000000 w3bstream_client_python-0.4.4/pyproject.toml
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/setup.cfg
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.482362 w3bstream_client_python-0.4.4/src/
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.482362 w3bstream_client_python-0.4.4/src/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-07 17:50:45.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3852 2023-07-07 16:58:52.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      810 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/requires.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream_client_python-0.4.3/.gitignore` & `w3bstream_client_python-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.3/LICENSE` & `w3bstream_client_python-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.3/README.md` & `w3bstream_client_python-0.4.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 The Python Client for W3bstream integration on server
 
 ## Getting started
 
 Install `w3bstream-client-python` via `pip3`
 ``` shell
 pip3 install w3bstream-client-python
-pip3 install typeguard
-pip3 install requests
 ```
 
 
 ## Example Code
 
 ### Publish Event Synchronously
```

### Comparing `w3bstream_client_python-0.4.3/src/client.py` & `w3bstream_client_python-0.4.4/src/w3bstream_client_python/client.py`

 * *Files identical despite different names*

