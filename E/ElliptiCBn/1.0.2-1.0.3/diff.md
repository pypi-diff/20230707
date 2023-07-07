# Comparing `tmp/ElliptiCBn-1.0.2.tar.gz` & `tmp/ElliptiCBn-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElliptiCBn-1.0.2.tar", last modified: Fri Jul  7 21:41:11 2023, max compression
+gzip compressed data, was "ElliptiCBn-1.0.3.tar", last modified: Fri Jul  7 21:47:01 2023, max compression
```

## Comparing `ElliptiCBn-1.0.2.tar` & `ElliptiCBn-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 21:41:11.946002 ElliptiCBn-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-07 21:41:11.897903 ElliptiCBn-1.0.2/ElliptiC/
--rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.2/ElliptiC/ElliptiC.py
--rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.2/ElliptiC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 21:41:11.942002 ElliptiCBn-1.0.2/ElliptiCBn.egg-info/
--rw-rw-rw-   0        0        0     5483 2023-07-07 21:41:11.000000 ElliptiCBn-1.0.2/ElliptiCBn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-07-07 21:41:11.000000 ElliptiCBn-1.0.2/ElliptiCBn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 21:41:11.000000 ElliptiCBn-1.0.2/ElliptiCBn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 21:41:11.000000 ElliptiCBn-1.0.2/ElliptiCBn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     5483 2023-07-07 21:41:11.945011 ElliptiCBn-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4711 2023-07-07 21:39:58.000000 ElliptiCBn-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 21:41:11.943000 ElliptiCBn-1.0.2/bin/
--rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.2/bin/ElliptiC
--rw-rw-rw-   0        0        0      780 2023-07-07 21:40:17.000000 ElliptiCBn-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 21:41:11.946002 ElliptiCBn-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-07-07 21:40:49.000000 ElliptiCBn-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.310042 ElliptiCBn-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.292633 ElliptiCBn-1.0.3/ElliptiC/
+-rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.3/ElliptiC/ElliptiC.py
+-rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.3/ElliptiC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.308041 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/
+-rw-rw-rw-   0        0        0     5423 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5423 2023-07-07 21:47:01.310042 ElliptiCBn-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-07-07 21:46:15.000000 ElliptiCBn-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.309044 ElliptiCBn-1.0.3/bin/
+-rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.3/bin/ElliptiC
+-rw-rw-rw-   0        0        0      780 2023-07-07 21:46:29.000000 ElliptiCBn-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 21:47:01.310042 ElliptiCBn-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-07-07 21:46:41.000000 ElliptiCBn-1.0.3/setup.py
```

### Comparing `ElliptiCBn-1.0.2/ElliptiC/ElliptiC.py` & `ElliptiCBn-1.0.3/ElliptiC/ElliptiC.py`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.2/ElliptiCBn.egg-info/PKG-INFO` & `ElliptiCBn-1.0.3/ElliptiCBn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElliptiCBn
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for analyzing Cucurbituril crystal structures automatically
 Home-page: https://github.com/harmslab/ElliptiC
 Author: Michael Shavlik
 Author-email: Michael Shavlik <mshavlik@uoregon.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/harmslab/ElliptiC
 Keywords: CBn; Crystal structure
@@ -36,15 +36,15 @@
 <br />
 
 ## How to run the analysis
 ### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
 
 **To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
 (NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png?token=GHSAT0AAAAAACEFKZS3MXIFKPDAKMXL7LWYZFIQYAA)
+![](https://github.com/mshavlik/ElliptiC/raw/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
 ![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/folder_test.png?token=GHSAT0AAAAAACEFKZS2QDGUHV7PEO7TBJTYZFIQXHQ)
 
 <br />
```

### Comparing `ElliptiCBn-1.0.2/LICENSE` & `ElliptiCBn-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.2/PKG-INFO` & `ElliptiCBn-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElliptiCBn
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for analyzing Cucurbituril crystal structures automatically
 Home-page: https://github.com/harmslab/ElliptiC
 Author: Michael Shavlik
 Author-email: Michael Shavlik <mshavlik@uoregon.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/harmslab/ElliptiC
 Keywords: CBn; Crystal structure
@@ -36,15 +36,15 @@
 <br />
 
 ## How to run the analysis
 ### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
 
 **To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
 (NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png?token=GHSAT0AAAAAACEFKZS3MXIFKPDAKMXL7LWYZFIQYAA)
+![](https://github.com/mshavlik/ElliptiC/raw/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
 ![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/folder_test.png?token=GHSAT0AAAAAACEFKZS2QDGUHV7PEO7TBJTYZFIQXHQ)
 
 <br />
```

### Comparing `ElliptiCBn-1.0.2/README.md` & `ElliptiCBn-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 <br />
 
 ## How to run the analysis
 ### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
 
 **To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
 (NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png?token=GHSAT0AAAAAACEFKZS3MXIFKPDAKMXL7LWYZFIQYAA)
+![](https://github.com/mshavlik/ElliptiC/raw/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
 ![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/folder_test.png?token=GHSAT0AAAAAACEFKZS2QDGUHV7PEO7TBJTYZFIQXHQ)
 
 <br />
```

### Comparing `ElliptiCBn-1.0.2/bin/ElliptiC` & `ElliptiCBn-1.0.3/bin/ElliptiC`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.2/pyproject.toml` & `ElliptiCBn-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ElliptiCBn"
-version = "1.0.2"
+version = "1.0.3"
 authors = [{name="Michael Shavlik", email="mshavlik@uoregon.edu"}]
 description = "Python package for analyzing Cucurbituril crystal structures automatically"
 readme = "README.md"
 requires-python = ">=3.7.0"
 classifiers = [
                   "Development Status :: 3 - Alpha",
                   "Intended Audience :: Science/Research",
```

### Comparing `ElliptiCBn-1.0.2/setup.py` & `ElliptiCBn-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 #Package meta-data
 DESCRIPTION= \
 """ Python package for analyzing CBn crystal structures automatically. """
 URL = "https://github.com/harmslab/ElliptiC"  # temp URL
 EMAIL = "mshavlik@uoregon.edu"
 AUTHOR = "Michael Shavlik"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import README for description
 with io.open(os.path.join(here,'README.md'),encoding='utf-8') as f:
     full_description = '\n' + f.read()
 
     
 # Now the part where we do setup
 setup(
     name='ElliptiCBn',
-    version='1.0.2',
+    version='1.0.3',
     author=AUTHOR,
     author_email=EMAIL,
     description=DESCRIPTION,
     long_description=full_description,
     url=URL,
     license='MIT',
     packages=['ElliptiC'],
```

