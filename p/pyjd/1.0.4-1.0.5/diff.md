# Comparing `tmp/pyjd-1.0.4.tar.gz` & `tmp/pyjd-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjd-1.0.4.tar", last modified: Fri Jul  7 07:41:29 2023, max compression
+gzip compressed data, was "pyjd-1.0.5.tar", last modified: Fri Jul  7 08:03:02 2023, max compression
```

## Comparing `pyjd-1.0.4.tar` & `pyjd-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:41:29.003286 pyjd-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-07 07:41:17.000000 pyjd-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 07:41:28.999286 pyjd-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 07:41:17.000000 pyjd-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:41:28.999286 pyjd-1.0.4/pyjd/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/content.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/direct_connection_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/direct_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/jd_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/jd_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/linkgrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/myjd_connection_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/myjd_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:41:28.999286 pyjd-1.0.4/pyjd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:41:29.003286 pyjd-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-07 07:41:17.000000 pyjd-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:03:02.559521 pyjd-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-07 08:02:54.000000 pyjd-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 08:03:02.559521 pyjd-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 08:02:54.000000 pyjd-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:03:02.555521 pyjd-1.0.5/pyjd/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/direct_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/direct_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/jd_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/jd_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/linkgrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/myjd_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/myjd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 08:02:54.000000 pyjd-1.0.5/pyjd/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:03:02.559521 pyjd-1.0.5/pyjd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 08:03:02.000000 pyjd-1.0.5/pyjd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:03:02.000000 pyjd-1.0.5/pyjd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:03:02.000000 pyjd-1.0.5/pyjd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 08:03:02.000000 pyjd-1.0.5/pyjd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 08:03:02.000000 pyjd-1.0.5/pyjd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:03:02.559521 pyjd-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-07 08:02:54.000000 pyjd-1.0.5/setup.py
```

### Comparing `pyjd-1.0.4/LICENSE` & `pyjd-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/PKG-INFO` & `pyjd-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.4/README.md` & `pyjd-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/accounts.py` & `pyjd-1.0.5/pyjd/accounts.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/captcha.py` & `pyjd-1.0.5/pyjd/captcha.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/config.py` & `pyjd-1.0.5/pyjd/config.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/content.py` & `pyjd-1.0.5/pyjd/content.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/device.py` & `pyjd-1.0.5/pyjd/device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/direct_connection_helper.py` & `pyjd-1.0.5/pyjd/direct_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/direct_connector.py` & `pyjd-1.0.5/pyjd/direct_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/downloads.py` & `pyjd-1.0.5/pyjd/downloads.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/events.py` & `pyjd-1.0.5/pyjd/events.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/extensions.py` & `pyjd-1.0.5/pyjd/extensions.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/jd_device.py` & `pyjd-1.0.5/pyjd/jd_device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/jd_types.py` & `pyjd-1.0.5/pyjd/jd_types.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/linkgrabber.py` & `pyjd-1.0.5/pyjd/linkgrabber.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/log.py` & `pyjd-1.0.5/pyjd/log.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/myjd_connection_helper.py` & `pyjd-1.0.5/pyjd/myjd_connection_helper.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/myjd_connector.py` & `pyjd-1.0.5/pyjd/myjd_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/plugins.py` & `pyjd-1.0.5/pyjd/plugins.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/polling.py` & `pyjd-1.0.5/pyjd/polling.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/system.py` & `pyjd-1.0.5/pyjd/system.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/toolbar.py` & `pyjd-1.0.5/pyjd/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/ui.py` & `pyjd-1.0.5/pyjd/ui.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd/update.py` & `pyjd-1.0.5/pyjd/update.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.4/pyjd.egg-info/PKG-INFO` & `pyjd-1.0.5/pyjd.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.4/pyjd.egg-info/SOURCES.txt` & `pyjd-1.0.5/pyjd.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 pyjd/system.py
 pyjd/toolbar.py
 pyjd/ui.py
 pyjd/update.py
 pyjd.egg-info/PKG-INFO
 pyjd.egg-info/SOURCES.txt
 pyjd.egg-info/dependency_links.txt
+pyjd.egg-info/requires.txt
 pyjd.egg-info/top_level.txt
```

### Comparing `pyjd-1.0.4/setup.py` & `pyjd-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="pyjd",
-    version="1.0.4",
+    version="1.0.5",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
     description=("A wapper for the JDownloader API"),
     license="GPLv3",
     keywords="api jdownloader",
     url="https://git.sr.ht/~pglaum/pyjd-api",
     packages=["pyjd"],
-    install_required=["requests", "pydantic===1.10.10", "pycryptodome"],
+    install_requires=["requests", "pydantic===1.10.10", "pycryptodome"],
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
```

