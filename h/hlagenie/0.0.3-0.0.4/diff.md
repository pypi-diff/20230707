# Comparing `tmp/hlagenie-0.0.3.tar.gz` & `tmp/hlagenie-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlagenie-0.0.3.tar", last modified: Wed Jul  5 19:42:39 2023, max compression
+gzip compressed data, was "hlagenie-0.0.4.tar", last modified: Thu Jul  6 23:14:05 2023, max compression
```

## Comparing `hlagenie-0.0.3.tar` & `hlagenie-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:42:39.149740 hlagenie-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 19:42:29.000000 hlagenie-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-05 19:42:29.000000 hlagenie-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-05 19:42:39.149740 hlagenie-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-05 19:42:29.000000 hlagenie-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:42:39.145740 hlagenie-0.0.3/hlagenie/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/genie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/smart_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:42:39.149740 hlagenie-0.0.3/hlagenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:42:38.000000 hlagenie-0.0.3/hlagenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 19:42:29.000000 hlagenie-0.0.3/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 19:42:29.000000 hlagenie-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 19:42:39.149740 hlagenie-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-05 19:42:29.000000 hlagenie-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:14:05.596488 hlagenie-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 23:13:53.000000 hlagenie-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 23:13:53.000000 hlagenie-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-06 23:14:05.596488 hlagenie-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-06 23:13:53.000000 hlagenie-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:14:05.592488 hlagenie-0.0.4/hlagenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/genie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/smart_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:14:05.596488 hlagenie-0.0.4/hlagenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 23:13:53.000000 hlagenie-0.0.4/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-06 23:13:53.000000 hlagenie-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 23:14:05.596488 hlagenie-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-06 23:13:53.000000 hlagenie-0.0.4/setup.py
```

### Comparing `hlagenie-0.0.3/LICENSE` & `hlagenie-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.3/PKG-INFO` & `hlagenie-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: hlagenie
-Version: 0.0.3
-Summary: Sequence handing for HLA with Python
-Home-page: https://github.com/gbiagini/hlagenie
-Author: Giovanni Biagini
-Author-email: dbiagini@tulane.edu
-License: LGPL 3.0
-Keywords: hlagenie
-Classifier: Development Status :: 2 - Pre-Alpha
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
 
@@ -34,14 +15,16 @@
     - [Accessing amino acid sequence dictionaries for HLA alleles](#accessing-amino-acid-sequence-dictionaries-for-hla-alleles)
     - [Retrieve amino acid position from mature protein sequence](#retrieve-amino-acid-position-from-mature-protein-sequence)
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
+    - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
+    - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -94,28 +77,28 @@
 ```python
 genie.seqs # mature protein sequences
 genie.full_seqs # full protein sequences
 ```
 
 #### Retrieve amino acid position from mature protein sequence
 
-To get a given amino acid position from a given HLA allele, you can use the `getAAposition` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
+To get a given amino acid position from a given HLA allele, you can use the `getAA` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
 
 For this and following functions, if a three- or four-field allele name is passed, a call is made to `py-ard` to reduce to the two-field level.
 
 ```python
-genie.getAAposition("A*01:01",1) # returns "G"
+genie.getAA("A*01:01",1) # returns "G"
 ```
 
 #### Retrieve amino acid substring from mature protein sequence
 
-To get a given amino acid substring from a given HLA allele, you can use the `getAAsubstring` function. This function is 1-indexed as well and is inclusive of the start and end positions.
+To get a given amino acid substring from a given HLA allele, you can use the `getPeptide` function. This function is 1-indexed as well and is inclusive of the start and end positions.
 
 ```python
-genie.getAAsubstring("A*01:01",1,10) # returns "GSHSMRYFFT"
+genie.getPeptide("A*01:01",1,10) # returns "GSHSMRYFFT"
 ```
 
 #### Retrieve epitope from mature protein sequence
 
 If you pass an allele name and a list of positions to the `getEpitope` function, `hlagenie` will return a formatted epitope string.
 
 ```python
@@ -143,7 +126,23 @@
 #### Count the number of amino acid mismatches between donor and recipient at a given position given the alleles
 
 The `countAAMismatchesAllele` function takes as input four alleles and an amino acid position. The input order is: Donor Allele 1, Donor Allele 2, Recipient Allele 1, Recipient Allele 2, amino acid position. The function returns the number of mismatches between the donor and recipient at that position, adjusting for donor homozygosity.
 
 ```python
 genie.countAAMismatchesAllele("A*02:01","A*02:01","A*01:01","A*01:01", 44) # returns 1
 ```
+
+#### Get the antigen recognition domain sequence of an allele
+
+The `getARD` function takes as input an allele name and returns the antigen recognition domain sequence of that allele.
+
+```python
+genie.getARD("A*01:01")
+```
+
+#### Get the extracellular domain sequence of an allele
+
+The `getXRD` function takes as input an allele name and returns the extracellular domain sequence of that allele.
+
+```python
+genie.getXRD("A*01:01")
+```
```

### Comparing `hlagenie-0.0.3/README.md` & `hlagenie-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: hlagenie
+Version: 0.0.4
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
 
 Heavily inspired by and dependent on the [pyARD](https://www.github.com/nmdp-bioinformatics/py-ard) package. The `HLAGenie` package strives to streamline and standardize the bulk handling of HLA sequence data and provide functions to simplify matching analysis.
 
@@ -15,14 +34,16 @@
     - [Accessing amino acid sequence dictionaries for HLA alleles](#accessing-amino-acid-sequence-dictionaries-for-hla-alleles)
     - [Retrieve amino acid position from mature protein sequence](#retrieve-amino-acid-position-from-mature-protein-sequence)
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
+    - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
+    - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -75,28 +96,28 @@
 ```python
 genie.seqs # mature protein sequences
 genie.full_seqs # full protein sequences
 ```
 
 #### Retrieve amino acid position from mature protein sequence
 
-To get a given amino acid position from a given HLA allele, you can use the `getAAposition` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
+To get a given amino acid position from a given HLA allele, you can use the `getAA` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
 
 For this and following functions, if a three- or four-field allele name is passed, a call is made to `py-ard` to reduce to the two-field level.
 
 ```python
-genie.getAAposition("A*01:01",1) # returns "G"
+genie.getAA("A*01:01",1) # returns "G"
 ```
 
 #### Retrieve amino acid substring from mature protein sequence
 
-To get a given amino acid substring from a given HLA allele, you can use the `getAAsubstring` function. This function is 1-indexed as well and is inclusive of the start and end positions.
+To get a given amino acid substring from a given HLA allele, you can use the `getPeptide` function. This function is 1-indexed as well and is inclusive of the start and end positions.
 
 ```python
-genie.getAAsubstring("A*01:01",1,10) # returns "GSHSMRYFFT"
+genie.getPeptide("A*01:01",1,10) # returns "GSHSMRYFFT"
 ```
 
 #### Retrieve epitope from mature protein sequence
 
 If you pass an allele name and a list of positions to the `getEpitope` function, `hlagenie` will return a formatted epitope string.
 
 ```python
@@ -123,8 +144,24 @@
 
 #### Count the number of amino acid mismatches between donor and recipient at a given position given the alleles
 
 The `countAAMismatchesAllele` function takes as input four alleles and an amino acid position. The input order is: Donor Allele 1, Donor Allele 2, Recipient Allele 1, Recipient Allele 2, amino acid position. The function returns the number of mismatches between the donor and recipient at that position, adjusting for donor homozygosity.
 
 ```python
 genie.countAAMismatchesAllele("A*02:01","A*02:01","A*01:01","A*01:01", 44) # returns 1
-```
+```
+
+#### Get the antigen recognition domain sequence of an allele
+
+The `getARD` function takes as input an allele name and returns the antigen recognition domain sequence of that allele.
+
+```python
+genie.getARD("A*01:01")
+```
+
+#### Get the extracellular domain sequence of an allele
+
+The `getXRD` function takes as input an allele name and returns the extracellular domain sequence of that allele.
+
+```python
+genie.getXRD("A*01:01")
+```
```

### Comparing `hlagenie-0.0.3/hlagenie/db.py` & `hlagenie-0.0.4/hlagenie/db.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.3/hlagenie/genie.py` & `hlagenie-0.0.4/hlagenie/genie.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,33 +34,37 @@
 
         # load sequence data from database
         if ungap:
             self.full_seqs = dr.generate_ungapped_tables(
                 self.db_connection, imgt_version
             )
             self.seqs = dr.generate_ungapped_mature_tables(self.db_connection)
+            self.ards = dr.generate_ungapped_ard_table(self.db_connection, self.seqs)
+            self.xrds = dr.generate_ungapped_xrd_table(self.db_connection, self.seqs)
         else:
             self.full_seqs = dr.generate_gapped_tables(self.db_connection, imgt_version)
             self.seqs = dr.generated_gapped_mature_tables(self.db_connection)
+            self.ards = dr.generate_gapped_ard_table(self.db_connection, self.seqs)
+            self.xrds = dr.generate_gapped_xrd_table(self.db_connection, self.seqs)
 
-    def getAAposition(self, allele, position):
+    def getAA(self, allele, position):
         """
         Get the amino acid at a specific position in an allele
 
         :param allele: The allele to get the amino acid from
         :param position: The position to get the amino acid from
         """
 
         if allele.count(":") > 1:
             allele = self.ard.redux(allele, "U2")
 
         # get the amino acid at the specified position
         return self.seqs[allele][position - 1]
 
-    def getAAsubstring(self, allele, start, stop):
+    def getPeptide(self, allele, start, stop):
         """
         Get the amino acid substring from a specified position to another specified position
 
         :param allele: The allele to get the amino acid substring from
         :param start: The position to start the substring
         :param stop: The position to end the substring
         """
@@ -98,16 +102,16 @@
 
         if allele1.count(":") > 1:
             allele1 = self.ard.redux(allele1, "U2")
         if allele2.count(":") > 1:
             allele2 = self.ard.redux(allele2, "U2")
 
         # get the amino acid at the specified position for each allele
-        aa1 = self.getAAposition(allele1, position)
-        aa2 = self.getAAposition(allele2, position)
+        aa1 = self.getAA(allele1, position)
+        aa2 = self.getAA(allele2, position)
 
         # check if the amino acids are the same
         return not (aa1 == aa2)
 
     def countAAMismatchesAllele(
         self, allele1donor, allele2donor, allele1recip, allele2recip, position
     ):
@@ -131,18 +135,18 @@
 
         # check if donor is homozygous
         donor_homozygous = False
         if allele1donor == allele2donor:
             donor_homozygous = True
 
         # get amino acids at specified position
-        aa1_donor = self.getAAposition(allele1donor, position)
-        aa2_donor = self.getAAposition(allele2donor, position)
-        aa1_recip = self.getAAposition(allele1recip, position)
-        aa2_recip = self.getAAposition(allele2recip, position)
+        aa1_donor = self.getAA(allele1donor, position)
+        aa2_donor = self.getAA(allele2donor, position)
+        aa1_recip = self.getAA(allele1recip, position)
+        aa2_recip = self.getAA(allele2recip, position)
 
         # count mismatches between donor and recipient
         mm_count = self.countAAMismatches(aa1_donor, aa2_donor, aa1_recip, aa2_recip)
 
         # adjust if donor is homozygous, due to mismatch being same AA
         if (mm_count == 2) and (donor_homozygous):
             mm_count = 1
@@ -164,7 +168,43 @@
         mm_count = 0
         if (aa1_donor != aa1_recip) and (aa1_donor != aa2_recip):
             mm_count += 1
         if (aa2_donor != aa2_recip) and (aa2_donor != aa1_recip):
             mm_count += 1
 
         return mm_count
+
+    def getARD(self, allele):
+        """
+        Get the ARD sequence of an allele
+
+        :param allele: The allele to get the ARD sequence from
+        :return: The ARD sequence
+        """
+
+        # reduce to two field if greater than two field
+        if allele.count(":") > 1:
+            allele = self.ard.redux(allele, "U2")
+
+        # get locus
+        locus = allele.split("*")[0]
+
+        # get the ARD sequence
+        return self.seqs[allele][: self.ards[locus]]
+
+    def getXRD(self, allele):
+        """
+        Get the XRD sequence of an allele
+
+        :param allele: The allele to get the XRD sequence from
+        :return: The XRD sequence
+        """
+
+        # reduce to two field if greater than two field
+        if allele.count(":") > 1:
+            allele = self.ard.redux(allele, "U2")
+
+        # get locus
+        locus = allele.split("*")[0]
+
+        # get the ARD sequence
+        return self.seqs[allele][: self.xrds[locus]]
```

### Comparing `hlagenie-0.0.3/hlagenie/load.py` & `hlagenie-0.0.4/hlagenie/load.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.3/hlagenie/misc.py` & `hlagenie-0.0.4/hlagenie/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,7 +97,27 @@
     # find match
     match = re.search(regex, sequence)
 
     # if match is found, return start coordinate
     start = match.start()
 
     return start
+
+
+def coordinate_end(sequence: str, regex: str):
+    """
+    Find the end coordinates of either the ARD or XRD based on a regular expression
+
+    :param regex: regex for identifying the end of a domain
+    :param sequence: reference sequence
+    :return: end coordinates of the domain
+    """
+
+    import re  # for regex matching
+
+    # find match
+    match = re.search(regex, sequence)
+
+    # if match is found, return end coordinate
+    end = match.span()[1]
+
+    return end
```

### Comparing `hlagenie-0.0.3/hlagenie/smart_sort.py` & `hlagenie-0.0.4/hlagenie/smart_sort.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.3/hlagenie.egg-info/PKG-INFO` & `hlagenie-0.0.4/hlagenie.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Provides: hlagenie
 Description-Content-Type: text/markdown
@@ -34,14 +34,16 @@
     - [Accessing amino acid sequence dictionaries for HLA alleles](#accessing-amino-acid-sequence-dictionaries-for-hla-alleles)
     - [Retrieve amino acid position from mature protein sequence](#retrieve-amino-acid-position-from-mature-protein-sequence)
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
+    - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
+    - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -94,28 +96,28 @@
 ```python
 genie.seqs # mature protein sequences
 genie.full_seqs # full protein sequences
 ```
 
 #### Retrieve amino acid position from mature protein sequence
 
-To get a given amino acid position from a given HLA allele, you can use the `getAAposition` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
+To get a given amino acid position from a given HLA allele, you can use the `getAA` function. This function is 1-indexed to match standard IMGT/HLA database nomenclature.
 
 For this and following functions, if a three- or four-field allele name is passed, a call is made to `py-ard` to reduce to the two-field level.
 
 ```python
-genie.getAAposition("A*01:01",1) # returns "G"
+genie.getAA("A*01:01",1) # returns "G"
 ```
 
 #### Retrieve amino acid substring from mature protein sequence
 
-To get a given amino acid substring from a given HLA allele, you can use the `getAAsubstring` function. This function is 1-indexed as well and is inclusive of the start and end positions.
+To get a given amino acid substring from a given HLA allele, you can use the `getPeptide` function. This function is 1-indexed as well and is inclusive of the start and end positions.
 
 ```python
-genie.getAAsubstring("A*01:01",1,10) # returns "GSHSMRYFFT"
+genie.getPeptide("A*01:01",1,10) # returns "GSHSMRYFFT"
 ```
 
 #### Retrieve epitope from mature protein sequence
 
 If you pass an allele name and a list of positions to the `getEpitope` function, `hlagenie` will return a formatted epitope string.
 
 ```python
@@ -143,7 +145,23 @@
 #### Count the number of amino acid mismatches between donor and recipient at a given position given the alleles
 
 The `countAAMismatchesAllele` function takes as input four alleles and an amino acid position. The input order is: Donor Allele 1, Donor Allele 2, Recipient Allele 1, Recipient Allele 2, amino acid position. The function returns the number of mismatches between the donor and recipient at that position, adjusting for donor homozygosity.
 
 ```python
 genie.countAAMismatchesAllele("A*02:01","A*02:01","A*01:01","A*01:01", 44) # returns 1
 ```
+
+#### Get the antigen recognition domain sequence of an allele
+
+The `getARD` function takes as input an allele name and returns the antigen recognition domain sequence of that allele.
+
+```python
+genie.getARD("A*01:01")
+```
+
+#### Get the extracellular domain sequence of an allele
+
+The `getXRD` function takes as input an allele name and returns the extracellular domain sequence of that allele.
+
+```python
+genie.getXRD("A*01:01")
+```
```

### Comparing `hlagenie-0.0.3/setup.py` & `hlagenie-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="hlagenie",
-    version="0.0.3",
+    version="0.0.4",
     description="Sequence handing for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Giovanni Biagini",
     author_email="dbiagini@tulane.edu",
     url="https://github.com/gbiagini/hlagenie",
     packages=[
@@ -26,15 +26,15 @@
     provides=["hlagenie"],
     scripts=[],
     install_requires=requirements,
     license="LGPL 3.0",
     zip_safe=False,
     keywords="hlagenie",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.11",
     ],
     test_suite="tests",
```

