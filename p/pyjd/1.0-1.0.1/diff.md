# Comparing `tmp/pyjd-1.0.tar.gz` & `tmp/pyjd-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjd-1.0.tar", last modified: Fri Jul  7 06:08:44 2023, max compression
+gzip compressed data, was "pyjd-1.0.1.tar", last modified: Fri Jul  7 06:11:11 2023, max compression
```

## Comparing `pyjd-1.0.tar` & `pyjd-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:08:44.507785 pyjd-1.0/
--rw-r--r--   0 philipp    (501) staff       (20)     7652 2023-07-07 06:01:35.000000 pyjd-1.0/LICENSE
--rw-r--r--   0 philipp    (501) staff       (20)     1361 2023-07-07 06:08:44.507653 pyjd-1.0/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      890 2023-07-07 06:01:35.000000 pyjd-1.0/README.md
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:08:44.506952 pyjd-1.0/pyjd/
--rw-r--r--   0 philipp    (501) staff       (20)      301 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     6933 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/accounts.py
--rw-r--r--   0 philipp    (501) staff       (20)     2951 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/captcha.py
--rw-r--r--   0 philipp    (501) staff       (20)     6110 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/config.py
--rw-r--r--   0 philipp    (501) staff       (20)     2023 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/content.py
--rw-r--r--   0 philipp    (501) staff       (20)      849 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/device.py
--rw-r--r--   0 philipp    (501) staff       (20)     1289 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/direct_connection_helper.py
--rw-r--r--   0 philipp    (501) staff       (20)      873 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/direct_connector.py
--rw-r--r--   0 philipp    (501) staff       (20)    13669 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/downloads.py
--rw-r--r--   0 philipp    (501) staff       (20)     7315 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/events.py
--rw-r--r--   0 philipp    (501) staff       (20)     2476 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/extensions.py
--rw-r--r--   0 philipp    (501) staff       (20)     1769 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/jd_device.py
--rw-r--r--   0 philipp    (501) staff       (20)    18966 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/jd_types.py
--rw-r--r--   0 philipp    (501) staff       (20)    11978 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/linkgrabber.py
--rw-r--r--   0 philipp    (501) staff       (20)      987 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/log.py
--rw-r--r--   0 philipp    (501) staff       (20)     6021 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/myjd_connection_helper.py
--rw-r--r--   0 philipp    (501) staff       (20)    15537 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/myjd_connector.py
--rw-r--r--   0 philipp    (501) staff       (20)     2060 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/plugins.py
--rw-r--r--   0 philipp    (501) staff       (20)      529 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/polling.py
--rw-r--r--   0 philipp    (501) staff       (20)     1449 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/system.py
--rw-r--r--   0 philipp    (501) staff       (20)     3017 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/toolbar.py
--rw-r--r--   0 philipp    (501) staff       (20)     1085 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/ui.py
--rw-r--r--   0 philipp    (501) staff       (20)      846 2023-07-07 06:01:35.000000 pyjd-1.0/pyjd/update.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:08:44.507479 pyjd-1.0/pyjd.egg-info/
--rw-r--r--   0 philipp    (501) staff       (20)     1361 2023-07-07 06:08:44.000000 pyjd-1.0/pyjd.egg-info/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      554 2023-07-07 06:08:44.000000 pyjd-1.0/pyjd.egg-info/SOURCES.txt
--rw-r--r--   0 philipp    (501) staff       (20)        1 2023-07-07 06:08:44.000000 pyjd-1.0/pyjd.egg-info/dependency_links.txt
--rw-r--r--   0 philipp    (501) staff       (20)        5 2023-07-07 06:08:44.000000 pyjd-1.0/pyjd.egg-info/top_level.txt
--rw-r--r--   0 philipp    (501) staff       (20)       38 2023-07-07 06:08:44.507825 pyjd-1.0/setup.cfg
--rw-r--r--   0 philipp    (501) staff       (20)      969 2023-07-07 06:07:47.000000 pyjd-1.0/setup.py
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:11:11.498665 pyjd-1.0.1/
+-rw-r--r--   0 philipp    (501) staff       (20)     7652 2023-07-07 06:01:35.000000 pyjd-1.0.1/LICENSE
+-rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:11:11.498530 pyjd-1.0.1/PKG-INFO
+-rw-r--r--   0 philipp    (501) staff       (20)      890 2023-07-07 06:01:35.000000 pyjd-1.0.1/README.md
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:11:11.497808 pyjd-1.0.1/pyjd/
+-rw-r--r--   0 philipp    (501) staff       (20)      301 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/__init__.py
+-rw-r--r--   0 philipp    (501) staff       (20)     6933 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/accounts.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2951 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/captcha.py
+-rw-r--r--   0 philipp    (501) staff       (20)     6110 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/config.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2023 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/content.py
+-rw-r--r--   0 philipp    (501) staff       (20)      849 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/device.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1289 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/direct_connection_helper.py
+-rw-r--r--   0 philipp    (501) staff       (20)      873 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/direct_connector.py
+-rw-r--r--   0 philipp    (501) staff       (20)    13669 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/downloads.py
+-rw-r--r--   0 philipp    (501) staff       (20)     7315 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/events.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2476 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/extensions.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1769 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/jd_device.py
+-rw-r--r--   0 philipp    (501) staff       (20)    18966 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/jd_types.py
+-rw-r--r--   0 philipp    (501) staff       (20)    11978 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/linkgrabber.py
+-rw-r--r--   0 philipp    (501) staff       (20)      987 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/log.py
+-rw-r--r--   0 philipp    (501) staff       (20)     6021 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/myjd_connection_helper.py
+-rw-r--r--   0 philipp    (501) staff       (20)    15537 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/myjd_connector.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2060 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/plugins.py
+-rw-r--r--   0 philipp    (501) staff       (20)      529 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/polling.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1449 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/system.py
+-rw-r--r--   0 philipp    (501) staff       (20)     3017 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/toolbar.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1085 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/ui.py
+-rw-r--r--   0 philipp    (501) staff       (20)      846 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/update.py
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:11:11.498330 pyjd-1.0.1/pyjd.egg-info/
+-rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/PKG-INFO
+-rw-r--r--   0 philipp    (501) staff       (20)      554 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/SOURCES.txt
+-rw-r--r--   0 philipp    (501) staff       (20)        1 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/dependency_links.txt
+-rw-r--r--   0 philipp    (501) staff       (20)        5 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/top_level.txt
+-rw-r--r--   0 philipp    (501) staff       (20)       38 2023-07-07 06:11:11.498704 pyjd-1.0.1/setup.cfg
+-rw-r--r--   0 philipp    (501) staff       (20)      958 2023-07-07 06:10:11.000000 pyjd-1.0.1/setup.py
```

### Comparing `pyjd-1.0/LICENSE` & `pyjd-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/PKG-INFO` & `pyjd-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0
-Summary: A wapper for the JDownloader (deprecated) API
+Version: 1.0.1
+Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjd-1.0/README.md` & `pyjd-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/accounts.py` & `pyjd-1.0.1/pyjd/accounts.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/captcha.py` & `pyjd-1.0.1/pyjd/captcha.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/config.py` & `pyjd-1.0.1/pyjd/config.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/content.py` & `pyjd-1.0.1/pyjd/content.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/device.py` & `pyjd-1.0.1/pyjd/device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/direct_connection_helper.py` & `pyjd-1.0.1/pyjd/direct_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/direct_connector.py` & `pyjd-1.0.1/pyjd/direct_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/downloads.py` & `pyjd-1.0.1/pyjd/downloads.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/events.py` & `pyjd-1.0.1/pyjd/events.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/extensions.py` & `pyjd-1.0.1/pyjd/extensions.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/jd_device.py` & `pyjd-1.0.1/pyjd/jd_device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/jd_types.py` & `pyjd-1.0.1/pyjd/jd_types.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/linkgrabber.py` & `pyjd-1.0.1/pyjd/linkgrabber.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/log.py` & `pyjd-1.0.1/pyjd/log.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/myjd_connection_helper.py` & `pyjd-1.0.1/pyjd/myjd_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/myjd_connector.py` & `pyjd-1.0.1/pyjd/myjd_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/plugins.py` & `pyjd-1.0.1/pyjd/plugins.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/polling.py` & `pyjd-1.0.1/pyjd/polling.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/system.py` & `pyjd-1.0.1/pyjd/system.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/toolbar.py` & `pyjd-1.0.1/pyjd/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/ui.py` & `pyjd-1.0.1/pyjd/ui.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd/update.py` & `pyjd-1.0.1/pyjd/update.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/pyjd.egg-info/PKG-INFO` & `pyjd-1.0.1/pyjd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0
-Summary: A wapper for the JDownloader (deprecated) API
+Version: 1.0.1
+Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjd-1.0/pyjd.egg-info/SOURCES.txt` & `pyjd-1.0.1/pyjd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjd-1.0/setup.py` & `pyjd-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="pyjd",
-    version="1.0",
+    version="1.0.1",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
-    description=("A wapper for the JDownloader (deprecated) API"),
+    description=("A wapper for the JDownloader API"),
     license="GPLv3",
     keywords="api jdownloader",
     url="https://git.sr.ht/~pglaum/pyjd-api",
     packages=["pyjd"],
     install_required=["requests"],
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

