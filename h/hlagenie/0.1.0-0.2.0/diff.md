# Comparing `tmp/hlagenie-0.1.0.tar.gz` & `tmp/hlagenie-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlagenie-0.1.0.tar", last modified: Fri Jul  7 00:21:43 2023, max compression
+gzip compressed data, was "hlagenie-0.2.0.tar", last modified: Fri Jul  7 18:00:07 2023, max compression
```

## Comparing `hlagenie-0.1.0.tar` & `hlagenie-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.288255 hlagenie-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 00:21:29.000000 hlagenie-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 00:21:29.000000 hlagenie-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-07 00:21:43.288255 hlagenie-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-07 00:21:29.000000 hlagenie-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.284255 hlagenie-0.1.0/hlagenie/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/genie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/smart_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.284255 hlagenie-0.1.0/hlagenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 00:21:29.000000 hlagenie-0.1.0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 00:21:29.000000 hlagenie-0.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.288255 hlagenie-0.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 00:21:29.000000 hlagenie-0.1.0/scripts/hlagenie
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-07 00:21:43.288255 hlagenie-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 00:21:29.000000 hlagenie-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:07.504537 hlagenie-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 17:59:55.000000 hlagenie-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 17:59:55.000000 hlagenie-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-07 18:00:07.504537 hlagenie-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-07 17:59:55.000000 hlagenie-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:07.504537 hlagenie-0.2.0/hlagenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/genie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 17:59:55.000000 hlagenie-0.2.0/hlagenie/smart_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:07.504537 hlagenie-0.2.0/hlagenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-07 18:00:07.000000 hlagenie-0.2.0/hlagenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 18:00:07.000000 hlagenie-0.2.0/hlagenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:00:07.000000 hlagenie-0.2.0/hlagenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:00:07.000000 hlagenie-0.2.0/hlagenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 18:00:07.000000 hlagenie-0.2.0/hlagenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 18:00:07.000000 hlagenie-0.2.0/hlagenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 17:59:55.000000 hlagenie-0.2.0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 17:59:55.000000 hlagenie-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:07.504537 hlagenie-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 17:59:55.000000 hlagenie-0.2.0/scripts/hlagenie
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-07 17:59:55.000000 hlagenie-0.2.0/scripts/hlagenie-match
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-07 18:00:07.508537 hlagenie-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 17:59:55.000000 hlagenie-0.2.0/setup.py
```

### Comparing `hlagenie-0.1.0/LICENSE` & `hlagenie-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hlagenie-0.1.0/PKG-INFO` & `hlagenie-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: hlagenie
-Version: 0.1.0
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
 
 Heavily inspired by and dependent on the [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
 
@@ -41,14 +22,16 @@
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
   - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
     - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
     - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
     - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
     - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
+    - [Checking if positions are mismatched between two alleles](#checking-if-positions-are-mismatched-between-two-alleles)
+    - [Counting mismatches between donor and recipient given two sets of alleles](#counting-mismatches-between-donor-and-recipient-given-two-sets-of-alleles)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -211,7 +194,46 @@
 Calling `hlagenie` from the command line with only an allele name will allow you to retrieve the mature protein sequence of that allele.
 
 ```bash
 
 hlagenie -a "A*01:01"
 ```
 
+#### Checking if positions are mismatched between two alleles
+
+Calling `hlagenie-match` from the command line with two allele names and a position will allow you to check if the two alleles have a mismatch at that position. This is based on the mature protein sequence of the alleles. This uses the gapped sequences by default to best assess matching.
+
+```bash
+hlagenie-match --allele1 "A*01:01" --allele2 "A*01:02" --positions 1 # returns Matched
+```
+
+Supplying a space-delimited list of positions will provide a count of mismatches between the alleles.
+
+```bash
+hlagenie-match --allele1 "A*01:01" --allele2 "A*01:02" --positions 1 2 3 4 5 # returns 0
+```
+
+Calling `hlagenie-match` from the command line with two allele names and no specified positions will allow you to count the total number of mismatches between the two alleles.
+
+```bash
+hlagenie-match --allele1 "A*01:01" --allele2 "A*01:02" # returns 2
+```
+
+#### Counting mismatches between donor and recipient given two sets of alleles
+
+Calling `hlagenie-match` from the command line with a recipient haplotype and a donor haplotype and a set of positions will allow you to retrieve the number of mismatches between the donor and recipient at those positions. This is based on the mature protein sequence of the alleles. This uses the gapped sequences by default to best assess matching. This value is adjusted for donor homozygosity.
+
+```bash
+hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --positions 1 2 3 4 5 # returns 0
+```
+
+This can also be done with a single position.
+
+```bash
+hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --positions 1 # returns 0
+```
+
+Supplying no positions gets the total number of mismatches between the donor and recipient, adjusted for donor homozygosity.
+
+```bash
+hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" # returns 32
+```
```

### Comparing `hlagenie-0.1.0/hlagenie/data_repository.py` & `hlagenie-0.2.0/hlagenie/data_repository.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.1.0/hlagenie/db.py` & `hlagenie-0.2.0/hlagenie/db.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.1.0/hlagenie/genie.py` & `hlagenie-0.2.0/hlagenie/genie.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.1.0/hlagenie/load.py` & `hlagenie-0.2.0/hlagenie/load.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.1.0/hlagenie/misc.py` & `hlagenie-0.2.0/hlagenie/misc.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.1.0/hlagenie/smart_sort.py` & `hlagenie-0.2.0/hlagenie/smart_sort.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.1.0/hlagenie.egg-info/PKG-INFO` & `hlagenie-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.1.0
+Version: 0.2.0
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
 Classifier: Development Status :: 3 - Alpha
@@ -41,14 +41,16 @@
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
   - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
     - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
     - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
     - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
     - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
+    - [Checking if positions are mismatched between two alleles](#checking-if-positions-are-mismatched-between-two-alleles)
+    - [Counting mismatches between donor and recipient given two sets of alleles](#counting-mismatches-between-donor-and-recipient-given-two-sets-of-alleles)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -211,7 +213,46 @@
 Calling `hlagenie` from the command line with only an allele name will allow you to retrieve the mature protein sequence of that allele.
 
 ```bash
 
 hlagenie -a "A*01:01"
 ```
 
+#### Checking if positions are mismatched between two alleles
+
+Calling `hlagenie-match` from the command line with two allele names and a position will allow you to check if the two alleles have a mismatch at that position. This is based on the mature protein sequence of the alleles. This uses the gapped sequences by default to best assess matching.
+
+```bash
+hlagenie-match --allele1 "A*01:01" --allele2 "A*01:02" --positions 1 # returns Matched
+```
+
+Supplying a space-delimited list of positions will provide a count of mismatches between the alleles.
+
+```bash
+hlagenie-match --allele1 "A*01:01" --allele2 "A*01:02" --positions 1 2 3 4 5 # returns 0
+```
+
+Calling `hlagenie-match` from the command line with two allele names and no specified positions will allow you to count the total number of mismatches between the two alleles.
+
+```bash
+hlagenie-match --allele1 "A*01:01" --allele2 "A*01:02" # returns 2
+```
+
+#### Counting mismatches between donor and recipient given two sets of alleles
+
+Calling `hlagenie-match` from the command line with a recipient haplotype and a donor haplotype and a set of positions will allow you to retrieve the number of mismatches between the donor and recipient at those positions. This is based on the mature protein sequence of the alleles. This uses the gapped sequences by default to best assess matching. This value is adjusted for donor homozygosity.
+
+```bash
+hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --positions 1 2 3 4 5 # returns 0
+```
+
+This can also be done with a single position.
+
+```bash
+hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" --positions 1 # returns 0
+```
+
+Supplying no positions gets the total number of mismatches between the donor and recipient, adjusted for donor homozygosity.
+
+```bash
+hlagenie-match --recip-haplo "A*01:01+A*01:02" --donor-haplo "A*02:01+A*01:02" # returns 32
+```
```

### Comparing `hlagenie-0.1.0/scripts/hlagenie` & `hlagenie-0.2.0/scripts/hlagenie`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 import argparse
 import sys
 import pyard
 import hlagenie
 from hlagenie.misc import get_imgt_version
```

### Comparing `hlagenie-0.1.0/setup.py` & `hlagenie-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,28 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="hlagenie",
-    version="0.1.0",
+    version="0.2.0",
     description="Sequence handing for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Giovanni Biagini",
     author_email="dbiagini@tulane.edu",
     url="https://github.com/gbiagini/hlagenie",
     packages=[
         "hlagenie",
     ],
     provides=["hlagenie"],
     scripts=[
         "scripts/hlagenie",
+        "scripts/hlagenie-match",
     ],
     install_requires=requirements,
     license="LGPL 3.0",
     zip_safe=False,
     keywords="hlagenie",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

