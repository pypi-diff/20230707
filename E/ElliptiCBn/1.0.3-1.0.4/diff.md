# Comparing `tmp/ElliptiCBn-1.0.3.tar.gz` & `tmp/ElliptiCBn-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElliptiCBn-1.0.3.tar", last modified: Fri Jul  7 21:47:01 2023, max compression
+gzip compressed data, was "ElliptiCBn-1.0.4.tar", last modified: Fri Jul  7 21:50:46 2023, max compression
```

## Comparing `ElliptiCBn-1.0.3.tar` & `ElliptiCBn-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.310042 ElliptiCBn-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.292633 ElliptiCBn-1.0.3/ElliptiC/
--rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.3/ElliptiC/ElliptiC.py
--rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.3/ElliptiC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.308041 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/
--rw-rw-rw-   0        0        0     5423 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 21:47:01.000000 ElliptiCBn-1.0.3/ElliptiCBn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     5423 2023-07-07 21:47:01.310042 ElliptiCBn-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-07-07 21:46:15.000000 ElliptiCBn-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 21:47:01.309044 ElliptiCBn-1.0.3/bin/
--rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.3/bin/ElliptiC
--rw-rw-rw-   0        0        0      780 2023-07-07 21:46:29.000000 ElliptiCBn-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 21:47:01.310042 ElliptiCBn-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-07-07 21:46:41.000000 ElliptiCBn-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.789797 ElliptiCBn-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.774150 ElliptiCBn-1.0.4/ElliptiC/
+-rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.4/ElliptiC/ElliptiC.py
+-rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.4/ElliptiC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.786804 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/
+-rw-rw-rw-   0        0        0     5393 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5393 2023-07-07 21:50:46.789797 ElliptiCBn-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4621 2023-07-07 21:49:44.000000 ElliptiCBn-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.788798 ElliptiCBn-1.0.4/bin/
+-rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.4/bin/ElliptiC
+-rw-rw-rw-   0        0        0      780 2023-07-07 21:50:19.000000 ElliptiCBn-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 21:50:46.790799 ElliptiCBn-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-07-07 21:50:08.000000 ElliptiCBn-1.0.4/setup.py
```

### Comparing `ElliptiCBn-1.0.3/ElliptiC/ElliptiC.py` & `ElliptiCBn-1.0.4/ElliptiC/ElliptiC.py`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.3/ElliptiCBn.egg-info/PKG-INFO` & `ElliptiCBn-1.0.4/ElliptiCBn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElliptiCBn
-Version: 1.0.3
+Version: 1.0.4
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
-![](https://github.com/mshavlik/ElliptiC/raw/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png)
+![](https://github.com/tensorbored/kds/raw/master/docs/_static/readme_lift.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
 ![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/folder_test.png?token=GHSAT0AAAAAACEFKZS2QDGUHV7PEO7TBJTYZFIQXHQ)
 
 <br />
```

### Comparing `ElliptiCBn-1.0.3/LICENSE` & `ElliptiCBn-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.3/PKG-INFO` & `ElliptiCBn-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElliptiCBn
-Version: 1.0.3
+Version: 1.0.4
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
-![](https://github.com/mshavlik/ElliptiC/raw/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png)
+![](https://github.com/tensorbored/kds/raw/master/docs/_static/readme_lift.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
 ![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/folder_test.png?token=GHSAT0AAAAAACEFKZS2QDGUHV7PEO7TBJTYZFIQXHQ)
 
 <br />
```

### Comparing `ElliptiCBn-1.0.3/README.md` & `ElliptiCBn-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 <br />
 
 ## How to run the analysis
 ### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
 
 **To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
 (NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://github.com/mshavlik/ElliptiC/raw/862682bad75f3521ff466b526dcaef7738487db8/images/single_file.png)
+![](https://github.com/tensorbored/kds/raw/master/docs/_static/readme_lift.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
 ![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/folder_test.png?token=GHSAT0AAAAAACEFKZS2QDGUHV7PEO7TBJTYZFIQXHQ)
 
 <br />
```

### Comparing `ElliptiCBn-1.0.3/bin/ElliptiC` & `ElliptiCBn-1.0.4/bin/ElliptiC`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.3/pyproject.toml` & `ElliptiCBn-1.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ElliptiCBn"
-version = "1.0.3"
+version = "1.0.4"
 authors = [{name="Michael Shavlik", email="mshavlik@uoregon.edu"}]
 description = "Python package for analyzing Cucurbituril crystal structures automatically"
 readme = "README.md"
 requires-python = ">=3.7.0"
 classifiers = [
                   "Development Status :: 3 - Alpha",
                   "Intended Audience :: Science/Research",
```

### Comparing `ElliptiCBn-1.0.3/setup.py` & `ElliptiCBn-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 #Package meta-data
 DESCRIPTION= \
 """ Python package for analyzing CBn crystal structures automatically. """
 URL = "https://github.com/harmslab/ElliptiC"  # temp URL
 EMAIL = "mshavlik@uoregon.edu"
 AUTHOR = "Michael Shavlik"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import README for description
 with io.open(os.path.join(here,'README.md'),encoding='utf-8') as f:
     full_description = '\n' + f.read()
 
     
 # Now the part where we do setup
 setup(
     name='ElliptiCBn',
-    version='1.0.3',
+    version='1.0.4',
     author=AUTHOR,
     author_email=EMAIL,
     description=DESCRIPTION,
     long_description=full_description,
     url=URL,
     license='MIT',
     packages=['ElliptiC'],
```

