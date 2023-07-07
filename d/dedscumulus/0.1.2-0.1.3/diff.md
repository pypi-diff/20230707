# Comparing `tmp/dedscumulus-0.1.2.tar.gz` & `tmp/dedscumulus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedscumulus-0.1.2.tar", last modified: Thu Jun  8 19:36:38 2023, max compression
+gzip compressed data, was "dedscumulus-0.1.3.tar", last modified: Fri Jul  7 09:23:53 2023, max compression
```

## Comparing `dedscumulus-0.1.2.tar` & `dedscumulus-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 19:36:38.595858 dedscumulus-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 dedscumulus-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      566 2023-06-08 19:36:38.596859 dedscumulus-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-04-21 00:56:16.000000 dedscumulus-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 19:36:38.549133 dedscumulus-0.1.2/dedscumulus/
--rw-rw-rw-   0        0        0      465 2023-04-21 13:58:35.000000 dedscumulus-0.1.2/dedscumulus/RequestHandler.py
--rw-rw-rw-   0        0        0    14284 2023-04-25 13:13:55.000000 dedscumulus-0.1.2/dedscumulus/SharePointHandler.py
--rw-rw-rw-   0        0        0     2250 2023-02-20 20:06:50.000000 dedscumulus-0.1.2/dedscumulus/TableLogHandler.py
--rw-rw-rw-   0        0        0        0 2022-05-17 10:12:58.000000 dedscumulus-0.1.2/dedscumulus/__init__.py
--rw-rw-rw-   0        0        0     8815 2023-02-21 02:51:22.000000 dedscumulus-0.1.2/dedscumulus/brzGlobal.py
--rw-rw-rw-   0        0        0     6485 2023-06-08 19:34:55.000000 dedscumulus-0.1.2/dedscumulus/gbtGlobal.py
--rw-rw-rw-   0        0        0    14664 2023-05-15 11:03:56.000000 dedscumulus-0.1.2/dedscumulus/mstAst.py
--rw-rw-rw-   0        0        0      824 2023-04-21 13:55:52.000000 dedscumulus-0.1.2/dedscumulus/mstLog.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:36:38.584086 dedscumulus-0.1.2/dedscumulus.egg-info/
--rw-rw-rw-   0        0        0      566 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-04-21 01:29:23.000000 dedscumulus-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-06-08 19:36:38.601193 dedscumulus-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      661 2023-06-08 19:35:53.000000 dedscumulus-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:23:53.691159 dedscumulus-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 dedscumulus-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-07-07 09:23:53.691824 dedscumulus-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-04-21 00:56:16.000000 dedscumulus-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 09:23:53.653472 dedscumulus-0.1.3/dedscumulus/
+-rw-rw-rw-   0        0        0      465 2023-04-21 13:58:35.000000 dedscumulus-0.1.3/dedscumulus/RequestHandler.py
+-rw-rw-rw-   0        0        0    14284 2023-04-25 13:13:55.000000 dedscumulus-0.1.3/dedscumulus/SharePointHandler.py
+-rw-rw-rw-   0        0        0     2250 2023-02-20 20:06:50.000000 dedscumulus-0.1.3/dedscumulus/TableLogHandler.py
+-rw-rw-rw-   0        0        0        0 2022-05-17 10:12:58.000000 dedscumulus-0.1.3/dedscumulus/__init__.py
+-rw-rw-rw-   0        0        0     8815 2023-02-21 02:51:22.000000 dedscumulus-0.1.3/dedscumulus/brzGlobal.py
+-rw-rw-rw-   0        0        0     6485 2023-06-08 19:34:55.000000 dedscumulus-0.1.3/dedscumulus/gbtGlobal.py
+-rw-rw-rw-   0        0        0    14664 2023-05-15 11:03:56.000000 dedscumulus-0.1.3/dedscumulus/mstAst.py
+-rw-rw-rw-   0        0        0      824 2023-04-21 13:55:52.000000 dedscumulus-0.1.3/dedscumulus/mstLog.py
+-rw-rw-rw-   0        0        0     2992 2023-07-07 09:20:56.000000 dedscumulus-0.1.3/dedscumulus/s3eGlobal.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:23:53.684992 dedscumulus-0.1.3/dedscumulus.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-07-07 09:23:53.000000 dedscumulus-0.1.3/dedscumulus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-07-07 09:23:53.000000 dedscumulus-0.1.3/dedscumulus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 09:23:53.000000 dedscumulus-0.1.3/dedscumulus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 09:23:53.000000 dedscumulus-0.1.3/dedscumulus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-04-21 01:29:23.000000 dedscumulus-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-07-07 09:23:53.693824 dedscumulus-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      661 2023-07-07 09:23:25.000000 dedscumulus-0.1.3/setup.py
```

### Comparing `dedscumulus-0.1.2/LICENSE` & `dedscumulus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.2/PKG-INFO` & `dedscumulus-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 License: UNKNOWN
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Platform: UNKNOWN
```

### Comparing `dedscumulus-0.1.2/dedscumulus/SharePointHandler.py` & `dedscumulus-0.1.3/dedscumulus/SharePointHandler.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.2/dedscumulus/TableLogHandler.py` & `dedscumulus-0.1.3/dedscumulus/TableLogHandler.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.2/dedscumulus/brzGlobal.py` & `dedscumulus-0.1.3/dedscumulus/brzGlobal.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.2/dedscumulus/gbtGlobal.py` & `dedscumulus-0.1.3/dedscumulus/gbtGlobal.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.2/dedscumulus/mstAst.py` & `dedscumulus-0.1.3/dedscumulus/mstAst.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.2/dedscumulus/mstLog.py` & `dedscumulus-0.1.3/dedscumulus/mstLog.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.2/dedscumulus.egg-info/PKG-INFO` & `dedscumulus-0.1.3/dedscumulus.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 License: UNKNOWN
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Platform: UNKNOWN
```

### Comparing `dedscumulus-0.1.2/setup.cfg` & `dedscumulus-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6564 7363 756d 756c 7573 0d0a   = dedscumulus..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 320d  version = 0.1.2.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 330d  version = 0.1.3.
 00000030: 0a61 7574 686f 7220 3d20 4261 7957 6120  .author = BayWa 
 00000040: 722e 652e 2044 6174 6120 5365 7276 6963  r.e. Data Servic
 00000050: 6573 2047 6d62 480d 0a61 7574 686f 725f  es GmbH..author_
 00000060: 656d 6169 6c20 3d20 6e6f 2d72 6570 6c79  email = no-reply
 00000070: 4062 6179 7761 2d72 652e 636f 6d0d 0a64  @baywa-re.com..d
 00000080: 6573 6372 6970 7469 6f6e 203d 204b 6572  escription = Ker
 00000090: 6e65 6c20 6675 6e63 7469 6f6e 7320 666f  nel functions fo
```

### Comparing `dedscumulus-0.1.2/setup.py` & `dedscumulus-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
      name='dedscumulus',  
-     version='0.1.2',
+     version='0.1.3',
      author="BayWa r.e. Data Services GmbH",
      author_email="no-reply@baywa-re.com",
      description="Kernel functions for Cumulus",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/nino-baywa/dedscumulus",
      classifiers=[
```

