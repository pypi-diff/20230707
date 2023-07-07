# Comparing `tmp/hlagenie-0.2.1.tar.gz` & `tmp/hlagenie-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlagenie-0.2.1.tar", last modified: Fri Jul  7 18:13:07 2023, max compression
+gzip compressed data, was "hlagenie-0.2.2.tar", last modified: Fri Jul  7 19:50:36 2023, max compression
```

## Comparing `hlagenie-0.2.1.tar` & `hlagenie-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:13:07.697279 hlagenie-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 18:12:57.000000 hlagenie-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 18:12:57.000000 hlagenie-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-07 18:13:07.697279 hlagenie-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-07 18:12:57.000000 hlagenie-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:13:07.693279 hlagenie-0.2.1/hlagenie/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/genie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 18:12:57.000000 hlagenie-0.2.1/hlagenie/smart_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:13:07.697279 hlagenie-0.2.1/hlagenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-07 18:13:07.000000 hlagenie-0.2.1/hlagenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 18:13:07.000000 hlagenie-0.2.1/hlagenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:13:07.000000 hlagenie-0.2.1/hlagenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:13:07.000000 hlagenie-0.2.1/hlagenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 18:13:07.000000 hlagenie-0.2.1/hlagenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 18:13:07.000000 hlagenie-0.2.1/hlagenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 18:12:57.000000 hlagenie-0.2.1/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 18:12:57.000000 hlagenie-0.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:13:07.697279 hlagenie-0.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 18:12:57.000000 hlagenie-0.2.1/scripts/hlagenie
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-07 18:12:57.000000 hlagenie-0.2.1/scripts/hlagenie-match
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-07 18:13:07.697279 hlagenie-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 18:12:57.000000 hlagenie-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 19:50:26.000000 hlagenie-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 19:50:26.000000 hlagenie-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-07 19:50:36.008402 hlagenie-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-07 19:50:26.000000 hlagenie-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/hlagenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/genie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 19:50:26.000000 hlagenie-0.2.2/hlagenie/smart_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/hlagenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 19:50:36.000000 hlagenie-0.2.2/hlagenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 19:50:35.000000 hlagenie-0.2.2/hlagenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 19:50:26.000000 hlagenie-0.2.2/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 19:50:26.000000 hlagenie-0.2.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:50:36.008402 hlagenie-0.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 19:50:26.000000 hlagenie-0.2.2/scripts/hlagenie
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-07 19:50:26.000000 hlagenie-0.2.2/scripts/hlagenie-match
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-07 19:50:36.008402 hlagenie-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 19:50:26.000000 hlagenie-0.2.2/setup.py
```

### Comparing `hlagenie-0.2.1/LICENSE` & `hlagenie-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/PKG-INFO` & `hlagenie-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,13 @@
-Metadata-Version: 2.1
-Name: hlagenie
-Version: 0.2.1
-Summary: Sequence handing for HLA with Python
-Home-page: https://github.com/gbiagini/hlagenie
-Author: Giovanni Biagini
-Author-email: dbiagini@tulane.edu
-License: LGPL 3.0
-Keywords: hlagenie
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.11
-Provides: hlagenie
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HLAGenie
 Python package for dealing with HLA sequence data
 
 ![hlagenie_logo.png](images/hlagenie_logo.png)
 
-Heavily inspired by and dependent on the [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
+Heavily inspired by and dependent on the fantastic [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
 
 ## Table of Contents
 - [Installation](#installation)
   - [Install from PyPI](#install-from-pypi)
   - [Install from source](#install-from-source)
 - [Using HLAGenie](#using-hlagenie)
   - [Using `hlagenie` from Python](#using-hlagenie-from-python)
@@ -43,14 +24,16 @@
   - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
     - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
     - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
     - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
     - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
     - [Checking if positions are mismatched between two alleles](#checking-if-positions-are-mismatched-between-two-alleles)
     - [Counting mismatches between donor and recipient given two sets of alleles](#counting-mismatches-between-donor-and-recipient-given-two-sets-of-alleles)
+- [Feature requests](#feature-requests)
+- [Contributing](#contributing)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -266,7 +249,17 @@
 
 Alternatively, you can use the `--ard` or `--xrd` flags to get the mismatches between the donor and recipient at the ARD or XRD level, respectively.
 
 ```bash
 hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --ard # returns 24
 hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --xrd # returns 29
 ```
+
+## Feature requests
+
+If you have a feature request, please feel free to open a new discussion in the [Ideas](https://github.com/gbiagini/hlagenie/discussions/categories/ideas) page of the Discussions tab. Doing so allows for a more open discussion of the feature and allows others to chime in with their thoughts.
+
+## Contributing
+
+Contributions are welcome. Please feel free to open a pull request with your changes. If you are unsure of how to do this, please feel free to open a discussion in the [Q&A](https://github.com/gbiagini/hlagenie/discussions/categories/q-a). If you are interested in contributing but are unsure of where to start, please check out the [Issues](https://github.com/gbiagini/hlagenie/issues) tab.
+
+Bug reporting is also welcome in the [Issues](https://github.com/gbiagini/hlagenie/issues) tab. Please include as much information as possible, including the version of `hlagenie` you are using, the version of Python you are using, and the operating system you are using. If you are able to provide a minimal reproducible example, that would be very helpful.
```

### Comparing `hlagenie-0.2.1/README.md` & `hlagenie-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,32 @@
+Metadata-Version: 2.1
+Name: hlagenie
+Version: 0.2.2
+Summary: Sequence handing for HLA with Python
+Home-page: https://github.com/gbiagini/hlagenie
+Author: Giovanni Biagini
+Author-email: dbiagini@tulane.edu
+License: LGPL 3.0
+Keywords: hlagenie
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.11
+Provides: hlagenie
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # HLAGenie
 Python package for dealing with HLA sequence data
 
 ![hlagenie_logo.png](images/hlagenie_logo.png)
 
-Heavily inspired by and dependent on the [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
+Heavily inspired by and dependent on the fantastic [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
 
 ## Table of Contents
 - [Installation](#installation)
   - [Install from PyPI](#install-from-pypi)
   - [Install from source](#install-from-source)
 - [Using HLAGenie](#using-hlagenie)
   - [Using `hlagenie` from Python](#using-hlagenie-from-python)
@@ -24,14 +43,16 @@
   - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
     - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
     - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
     - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
     - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
     - [Checking if positions are mismatched between two alleles](#checking-if-positions-are-mismatched-between-two-alleles)
     - [Counting mismatches between donor and recipient given two sets of alleles](#counting-mismatches-between-donor-and-recipient-given-two-sets-of-alleles)
+- [Feature requests](#feature-requests)
+- [Contributing](#contributing)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -246,8 +267,18 @@
 ```
 
 Alternatively, you can use the `--ard` or `--xrd` flags to get the mismatches between the donor and recipient at the ARD or XRD level, respectively.
 
 ```bash
 hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --ard # returns 24
 hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --xrd # returns 29
-```
+```
+
+## Feature requests
+
+If you have a feature request, please feel free to open a new discussion in the [Ideas](https://github.com/gbiagini/hlagenie/discussions/categories/ideas) page of the Discussions tab. Doing so allows for a more open discussion of the feature and allows others to chime in with their thoughts.
+
+## Contributing
+
+Contributions are welcome. Please feel free to open a pull request with your changes. If you are unsure of how to do this, please feel free to open a discussion in the [Q&A](https://github.com/gbiagini/hlagenie/discussions/categories/q-a). If you are interested in contributing but are unsure of where to start, please check out the [Issues](https://github.com/gbiagini/hlagenie/issues) tab.
+
+Bug reporting is also welcome in the [Issues](https://github.com/gbiagini/hlagenie/issues) tab. Please include as much information as possible, including the version of `hlagenie` you are using, the version of Python you are using, and the operating system you are using. If you are able to provide a minimal reproducible example, that would be very helpful.
```

### Comparing `hlagenie-0.2.1/hlagenie/data_repository.py` & `hlagenie-0.2.2/hlagenie/data_repository.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/hlagenie/db.py` & `hlagenie-0.2.2/hlagenie/db.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/hlagenie/genie.py` & `hlagenie-0.2.2/hlagenie/genie.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/hlagenie/load.py` & `hlagenie-0.2.2/hlagenie/load.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/hlagenie/misc.py` & `hlagenie-0.2.2/hlagenie/misc.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/hlagenie/smart_sort.py` & `hlagenie-0.2.2/hlagenie/smart_sort.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/hlagenie.egg-info/PKG-INFO` & `hlagenie-0.2.2/hlagenie.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 License-File: LICENSE
 
 # HLAGenie
 Python package for dealing with HLA sequence data
 
 ![hlagenie_logo.png](images/hlagenie_logo.png)
 
-Heavily inspired by and dependent on the [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
+Heavily inspired by and dependent on the fantastic [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
 
 ## Table of Contents
 - [Installation](#installation)
   - [Install from PyPI](#install-from-pypi)
   - [Install from source](#install-from-source)
 - [Using HLAGenie](#using-hlagenie)
   - [Using `hlagenie` from Python](#using-hlagenie-from-python)
@@ -43,14 +43,16 @@
   - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
     - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
     - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
     - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
     - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
     - [Checking if positions are mismatched between two alleles](#checking-if-positions-are-mismatched-between-two-alleles)
     - [Counting mismatches between donor and recipient given two sets of alleles](#counting-mismatches-between-donor-and-recipient-given-two-sets-of-alleles)
+- [Feature requests](#feature-requests)
+- [Contributing](#contributing)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -266,7 +268,17 @@
 
 Alternatively, you can use the `--ard` or `--xrd` flags to get the mismatches between the donor and recipient at the ARD or XRD level, respectively.
 
 ```bash
 hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --ard # returns 24
 hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --xrd # returns 29
 ```
+
+## Feature requests
+
+If you have a feature request, please feel free to open a new discussion in the [Ideas](https://github.com/gbiagini/hlagenie/discussions/categories/ideas) page of the Discussions tab. Doing so allows for a more open discussion of the feature and allows others to chime in with their thoughts.
+
+## Contributing
+
+Contributions are welcome. Please feel free to open a pull request with your changes. If you are unsure of how to do this, please feel free to open a discussion in the [Q&A](https://github.com/gbiagini/hlagenie/discussions/categories/q-a). If you are interested in contributing but are unsure of where to start, please check out the [Issues](https://github.com/gbiagini/hlagenie/issues) tab.
+
+Bug reporting is also welcome in the [Issues](https://github.com/gbiagini/hlagenie/issues) tab. Please include as much information as possible, including the version of `hlagenie` you are using, the version of Python you are using, and the operating system you are using. If you are able to provide a minimal reproducible example, that would be very helpful.
```

### Comparing `hlagenie-0.2.1/scripts/hlagenie` & `hlagenie-0.2.2/scripts/hlagenie`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/scripts/hlagenie-match` & `hlagenie-0.2.2/scripts/hlagenie-match`

 * *Files identical despite different names*

### Comparing `hlagenie-0.2.1/setup.py` & `hlagenie-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="hlagenie",
-    version="0.2.1",
+    version="0.2.2",
     description="Sequence handing for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Giovanni Biagini",
     author_email="dbiagini@tulane.edu",
     url="https://github.com/gbiagini/hlagenie",
     packages=[
```

