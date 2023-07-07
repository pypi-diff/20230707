# Comparing `tmp/pyjd-1.0.2.tar.gz` & `tmp/pyjd-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjd-1.0.2.tar", last modified: Fri Jul  7 06:16:50 2023, max compression
+gzip compressed data, was "pyjd-1.0.3.tar", last modified: Fri Jul  7 06:34:40 2023, max compression
```

## Comparing `pyjd-1.0.2.tar` & `pyjd-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:16:50.427722 pyjd-1.0.2/
--rw-r--r--   0 philipp    (501) staff       (20)     7652 2023-07-07 06:01:35.000000 pyjd-1.0.2/LICENSE
--rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:16:50.427591 pyjd-1.0.2/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      890 2023-07-07 06:01:35.000000 pyjd-1.0.2/README.md
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:16:50.426755 pyjd-1.0.2/pyjd/
--rw-r--r--   0 philipp    (501) staff       (20)      301 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     6933 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/accounts.py
--rw-r--r--   0 philipp    (501) staff       (20)     2951 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/captcha.py
--rw-r--r--   0 philipp    (501) staff       (20)     6110 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/config.py
--rw-r--r--   0 philipp    (501) staff       (20)     2023 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/content.py
--rw-r--r--   0 philipp    (501) staff       (20)      849 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/device.py
--rw-r--r--   0 philipp    (501) staff       (20)     1289 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/direct_connection_helper.py
--rw-r--r--   0 philipp    (501) staff       (20)      873 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/direct_connector.py
--rw-r--r--   0 philipp    (501) staff       (20)    13669 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/downloads.py
--rw-r--r--   0 philipp    (501) staff       (20)     7315 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/events.py
--rw-r--r--   0 philipp    (501) staff       (20)     2476 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/extensions.py
--rw-r--r--   0 philipp    (501) staff       (20)     1769 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/jd_device.py
--rw-r--r--   0 philipp    (501) staff       (20)    18966 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/jd_types.py
--rw-r--r--   0 philipp    (501) staff       (20)    11978 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/linkgrabber.py
--rw-r--r--   0 philipp    (501) staff       (20)      987 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/log.py
--rw-r--r--   0 philipp    (501) staff       (20)     6021 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/myjd_connection_helper.py
--rw-r--r--   0 philipp    (501) staff       (20)    15537 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/myjd_connector.py
--rw-r--r--   0 philipp    (501) staff       (20)     2060 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/plugins.py
--rw-r--r--   0 philipp    (501) staff       (20)      529 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/polling.py
--rw-r--r--   0 philipp    (501) staff       (20)     1449 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/system.py
--rw-r--r--   0 philipp    (501) staff       (20)     3017 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/toolbar.py
--rw-r--r--   0 philipp    (501) staff       (20)     1085 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/ui.py
--rw-r--r--   0 philipp    (501) staff       (20)      846 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/update.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:16:50.427273 pyjd-1.0.2/pyjd.egg-info/
--rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      554 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/SOURCES.txt
--rw-r--r--   0 philipp    (501) staff       (20)        1 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/dependency_links.txt
--rw-r--r--   0 philipp    (501) staff       (20)        5 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/top_level.txt
--rw-r--r--   0 philipp    (501) staff       (20)       38 2023-07-07 06:16:50.427765 pyjd-1.0.2/setup.cfg
--rw-r--r--   0 philipp    (501) staff       (20)      986 2023-07-07 06:16:19.000000 pyjd-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:40.322980 pyjd-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-07 06:34:32.000000 pyjd-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 06:34:40.322980 pyjd-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-07 06:34:32.000000 pyjd-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:40.322980 pyjd-1.0.3/pyjd/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/direct_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/direct_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/jd_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/jd_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/linkgrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/myjd_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/myjd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:40.322980 pyjd-1.0.3/pyjd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:34:40.322980 pyjd-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-07 06:34:32.000000 pyjd-1.0.3/setup.py
```

### Comparing `pyjd-1.0.2/LICENSE` & `pyjd-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/PKG-INFO` & `pyjd-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.2/README.md` & `pyjd-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/accounts.py` & `pyjd-1.0.3/pyjd/accounts.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/captcha.py` & `pyjd-1.0.3/pyjd/captcha.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/config.py` & `pyjd-1.0.3/pyjd/config.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/content.py` & `pyjd-1.0.3/pyjd/content.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/device.py` & `pyjd-1.0.3/pyjd/device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/direct_connection_helper.py` & `pyjd-1.0.3/pyjd/direct_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/direct_connector.py` & `pyjd-1.0.3/pyjd/direct_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/downloads.py` & `pyjd-1.0.3/pyjd/downloads.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/events.py` & `pyjd-1.0.3/pyjd/events.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/extensions.py` & `pyjd-1.0.3/pyjd/extensions.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/jd_device.py` & `pyjd-1.0.3/pyjd/jd_device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/jd_types.py` & `pyjd-1.0.3/pyjd/jd_types.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/linkgrabber.py` & `pyjd-1.0.3/pyjd/linkgrabber.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/log.py` & `pyjd-1.0.3/pyjd/log.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/myjd_connection_helper.py` & `pyjd-1.0.3/pyjd/myjd_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/myjd_connector.py` & `pyjd-1.0.3/pyjd/myjd_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/plugins.py` & `pyjd-1.0.3/pyjd/plugins.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/polling.py` & `pyjd-1.0.3/pyjd/polling.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/system.py` & `pyjd-1.0.3/pyjd/system.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/toolbar.py` & `pyjd-1.0.3/pyjd/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/ui.py` & `pyjd-1.0.3/pyjd/ui.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd/update.py` & `pyjd-1.0.3/pyjd/update.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/pyjd.egg-info/PKG-INFO` & `pyjd-1.0.3/pyjd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.2/pyjd.egg-info/SOURCES.txt` & `pyjd-1.0.3/pyjd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.2/setup.py` & `pyjd-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="pyjd",
-    version="1.0.2",
+    version="1.0.3",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
     description=("A wapper for the JDownloader API"),
     license="GPLv3",
     keywords="api jdownloader",
     url="https://git.sr.ht/~pglaum/pyjd-api",
     packages=["pyjd"],
```

