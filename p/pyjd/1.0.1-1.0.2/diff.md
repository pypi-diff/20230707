# Comparing `tmp/pyjd-1.0.1.tar.gz` & `tmp/pyjd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjd-1.0.1.tar", last modified: Fri Jul  7 06:11:11 2023, max compression
+gzip compressed data, was "pyjd-1.0.2.tar", last modified: Fri Jul  7 06:16:50 2023, max compression
```

## Comparing `pyjd-1.0.1.tar` & `pyjd-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:11:11.498665 pyjd-1.0.1/
--rw-r--r--   0 philipp    (501) staff       (20)     7652 2023-07-07 06:01:35.000000 pyjd-1.0.1/LICENSE
--rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:11:11.498530 pyjd-1.0.1/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      890 2023-07-07 06:01:35.000000 pyjd-1.0.1/README.md
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:11:11.497808 pyjd-1.0.1/pyjd/
--rw-r--r--   0 philipp    (501) staff       (20)      301 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     6933 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/accounts.py
--rw-r--r--   0 philipp    (501) staff       (20)     2951 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/captcha.py
--rw-r--r--   0 philipp    (501) staff       (20)     6110 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/config.py
--rw-r--r--   0 philipp    (501) staff       (20)     2023 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/content.py
--rw-r--r--   0 philipp    (501) staff       (20)      849 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/device.py
--rw-r--r--   0 philipp    (501) staff       (20)     1289 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/direct_connection_helper.py
--rw-r--r--   0 philipp    (501) staff       (20)      873 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/direct_connector.py
--rw-r--r--   0 philipp    (501) staff       (20)    13669 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/downloads.py
--rw-r--r--   0 philipp    (501) staff       (20)     7315 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/events.py
--rw-r--r--   0 philipp    (501) staff       (20)     2476 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/extensions.py
--rw-r--r--   0 philipp    (501) staff       (20)     1769 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/jd_device.py
--rw-r--r--   0 philipp    (501) staff       (20)    18966 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/jd_types.py
--rw-r--r--   0 philipp    (501) staff       (20)    11978 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/linkgrabber.py
--rw-r--r--   0 philipp    (501) staff       (20)      987 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/log.py
--rw-r--r--   0 philipp    (501) staff       (20)     6021 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/myjd_connection_helper.py
--rw-r--r--   0 philipp    (501) staff       (20)    15537 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/myjd_connector.py
--rw-r--r--   0 philipp    (501) staff       (20)     2060 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/plugins.py
--rw-r--r--   0 philipp    (501) staff       (20)      529 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/polling.py
--rw-r--r--   0 philipp    (501) staff       (20)     1449 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/system.py
--rw-r--r--   0 philipp    (501) staff       (20)     3017 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/toolbar.py
--rw-r--r--   0 philipp    (501) staff       (20)     1085 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/ui.py
--rw-r--r--   0 philipp    (501) staff       (20)      846 2023-07-07 06:01:35.000000 pyjd-1.0.1/pyjd/update.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:11:11.498330 pyjd-1.0.1/pyjd.egg-info/
--rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      554 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/SOURCES.txt
--rw-r--r--   0 philipp    (501) staff       (20)        1 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/dependency_links.txt
--rw-r--r--   0 philipp    (501) staff       (20)        5 2023-07-07 06:11:11.000000 pyjd-1.0.1/pyjd.egg-info/top_level.txt
--rw-r--r--   0 philipp    (501) staff       (20)       38 2023-07-07 06:11:11.498704 pyjd-1.0.1/setup.cfg
--rw-r--r--   0 philipp    (501) staff       (20)      958 2023-07-07 06:10:11.000000 pyjd-1.0.1/setup.py
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:16:50.427722 pyjd-1.0.2/
+-rw-r--r--   0 philipp    (501) staff       (20)     7652 2023-07-07 06:01:35.000000 pyjd-1.0.2/LICENSE
+-rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:16:50.427591 pyjd-1.0.2/PKG-INFO
+-rw-r--r--   0 philipp    (501) staff       (20)      890 2023-07-07 06:01:35.000000 pyjd-1.0.2/README.md
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:16:50.426755 pyjd-1.0.2/pyjd/
+-rw-r--r--   0 philipp    (501) staff       (20)      301 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/__init__.py
+-rw-r--r--   0 philipp    (501) staff       (20)     6933 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/accounts.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2951 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/captcha.py
+-rw-r--r--   0 philipp    (501) staff       (20)     6110 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/config.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2023 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/content.py
+-rw-r--r--   0 philipp    (501) staff       (20)      849 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/device.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1289 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/direct_connection_helper.py
+-rw-r--r--   0 philipp    (501) staff       (20)      873 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/direct_connector.py
+-rw-r--r--   0 philipp    (501) staff       (20)    13669 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/downloads.py
+-rw-r--r--   0 philipp    (501) staff       (20)     7315 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/events.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2476 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/extensions.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1769 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/jd_device.py
+-rw-r--r--   0 philipp    (501) staff       (20)    18966 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/jd_types.py
+-rw-r--r--   0 philipp    (501) staff       (20)    11978 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/linkgrabber.py
+-rw-r--r--   0 philipp    (501) staff       (20)      987 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/log.py
+-rw-r--r--   0 philipp    (501) staff       (20)     6021 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/myjd_connection_helper.py
+-rw-r--r--   0 philipp    (501) staff       (20)    15537 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/myjd_connector.py
+-rw-r--r--   0 philipp    (501) staff       (20)     2060 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/plugins.py
+-rw-r--r--   0 philipp    (501) staff       (20)      529 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/polling.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1449 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/system.py
+-rw-r--r--   0 philipp    (501) staff       (20)     3017 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/toolbar.py
+-rw-r--r--   0 philipp    (501) staff       (20)     1085 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/ui.py
+-rw-r--r--   0 philipp    (501) staff       (20)      846 2023-07-07 06:01:35.000000 pyjd-1.0.2/pyjd/update.py
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-07 06:16:50.427273 pyjd-1.0.2/pyjd.egg-info/
+-rw-r--r--   0 philipp    (501) staff       (20)     1350 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/PKG-INFO
+-rw-r--r--   0 philipp    (501) staff       (20)      554 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/SOURCES.txt
+-rw-r--r--   0 philipp    (501) staff       (20)        1 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/dependency_links.txt
+-rw-r--r--   0 philipp    (501) staff       (20)        5 2023-07-07 06:16:50.000000 pyjd-1.0.2/pyjd.egg-info/top_level.txt
+-rw-r--r--   0 philipp    (501) staff       (20)       38 2023-07-07 06:16:50.427765 pyjd-1.0.2/setup.cfg
+-rw-r--r--   0 philipp    (501) staff       (20)      986 2023-07-07 06:16:19.000000 pyjd-1.0.2/setup.py
```

### Comparing `pyjd-1.0.1/LICENSE` & `pyjd-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/PKG-INFO` & `pyjd-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.1/README.md` & `pyjd-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/accounts.py` & `pyjd-1.0.2/pyjd/accounts.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/captcha.py` & `pyjd-1.0.2/pyjd/captcha.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/config.py` & `pyjd-1.0.2/pyjd/config.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/content.py` & `pyjd-1.0.2/pyjd/content.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/device.py` & `pyjd-1.0.2/pyjd/device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/direct_connection_helper.py` & `pyjd-1.0.2/pyjd/direct_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/direct_connector.py` & `pyjd-1.0.2/pyjd/direct_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/downloads.py` & `pyjd-1.0.2/pyjd/downloads.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/events.py` & `pyjd-1.0.2/pyjd/events.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/extensions.py` & `pyjd-1.0.2/pyjd/extensions.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/jd_device.py` & `pyjd-1.0.2/pyjd/jd_device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/jd_types.py` & `pyjd-1.0.2/pyjd/jd_types.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/linkgrabber.py` & `pyjd-1.0.2/pyjd/linkgrabber.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/log.py` & `pyjd-1.0.2/pyjd/log.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/myjd_connection_helper.py` & `pyjd-1.0.2/pyjd/myjd_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/myjd_connector.py` & `pyjd-1.0.2/pyjd/myjd_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/plugins.py` & `pyjd-1.0.2/pyjd/plugins.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/polling.py` & `pyjd-1.0.2/pyjd/polling.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/system.py` & `pyjd-1.0.2/pyjd/system.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/toolbar.py` & `pyjd-1.0.2/pyjd/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/ui.py` & `pyjd-1.0.2/pyjd/ui.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd/update.py` & `pyjd-1.0.2/pyjd/update.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/pyjd.egg-info/PKG-INFO` & `pyjd-1.0.2/pyjd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.1/pyjd.egg-info/SOURCES.txt` & `pyjd-1.0.2/pyjd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.1/setup.py` & `pyjd-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="pyjd",
-    version="1.0.1",
+    version="1.0.2",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
     description=("A wapper for the JDownloader API"),
     license="GPLv3",
     keywords="api jdownloader",
     url="https://git.sr.ht/~pglaum/pyjd-api",
     packages=["pyjd"],
-    install_required=["requests"],
+    install_required=["requests", "pydantic", "pycryptodome"],
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
```

