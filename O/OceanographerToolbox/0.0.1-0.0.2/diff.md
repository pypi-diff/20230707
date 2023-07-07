# Comparing `tmp/OceanographerToolbox-0.0.1.tar.gz` & `tmp/OceanographerToolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OceanographerToolbox-0.0.1.tar", last modified: Fri Jul  7 21:26:43 2023, max compression
+gzip compressed data, was "OceanographerToolbox-0.0.2.tar", last modified: Fri Jul  7 21:46:57 2023, max compression
```

## Comparing `OceanographerToolbox-0.0.1.tar` & `OceanographerToolbox-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 21:26:43.829466 OceanographerToolbox-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 OceanographerToolbox-0.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-07 21:26:43.827475 OceanographerToolbox-0.0.1/OceanographerToolbox.egg-info/
--rw-rw-rw-   0        0        0      540 2023-07-07 21:26:43.000000 OceanographerToolbox-0.0.1/OceanographerToolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-07 21:26:43.000000 OceanographerToolbox-0.0.1/OceanographerToolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 21:26:43.000000 OceanographerToolbox-0.0.1/OceanographerToolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 21:26:43.000000 OceanographerToolbox-0.0.1/OceanographerToolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      540 2023-07-07 21:26:43.828511 OceanographerToolbox-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-07-07 18:08:28.000000 OceanographerToolbox-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 21:26:43.829466 OceanographerToolbox-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-07-07 18:18:21.000000 OceanographerToolbox-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 21:46:57.744908 OceanographerToolbox-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 OceanographerToolbox-0.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-07 21:46:57.742945 OceanographerToolbox-0.0.2/OceanographerToolbox.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-07-07 21:46:57.000000 OceanographerToolbox-0.0.2/OceanographerToolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-07 21:46:57.000000 OceanographerToolbox-0.0.2/OceanographerToolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 21:46:57.000000 OceanographerToolbox-0.0.2/OceanographerToolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 21:46:57.000000 OceanographerToolbox-0.0.2/OceanographerToolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      523 2023-07-07 21:46:57.743876 OceanographerToolbox-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-07-07 18:08:28.000000 OceanographerToolbox-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 21:46:57.744908 OceanographerToolbox-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-07-07 21:45:35.000000 OceanographerToolbox-0.0.2/setup.py
```

### Comparing `OceanographerToolbox-0.0.1/LICENSE` & `OceanographerToolbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OceanographerToolbox-0.0.1/OceanographerToolbox.egg-info/PKG-INFO` & `OceanographerToolbox-0.0.2/OceanographerToolbox.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OceanographerToolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page: https://github.com/andrewtbanks/OceanographerToolbox
 Author: Andy Banks
-Author-email: anba@dhigroup.com
+Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OceanographerToolbox
```

### Comparing `OceanographerToolbox-0.0.1/PKG-INFO` & `OceanographerToolbox-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OceanographerToolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page: https://github.com/andrewtbanks/OceanographerToolbox
 Author: Andy Banks
-Author-email: anba@dhigroup.com
+Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OceanographerToolbox
```

### Comparing `OceanographerToolbox-0.0.1/setup.py` & `OceanographerToolbox-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OceanographerToolbox",
-    version="0.0.1",
+    version="0.0.2",
     author="Andy Banks",
-    author_email="anba@dhigroup.com",
+    author_email="",
     description="Toolbox for importing and plotting ADCP and CTD data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andrewtbanks/OceanographerToolbox",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

