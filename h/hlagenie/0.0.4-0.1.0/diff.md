# Comparing `tmp/hlagenie-0.0.4.tar.gz` & `tmp/hlagenie-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlagenie-0.0.4.tar", last modified: Thu Jul  6 23:14:05 2023, max compression
+gzip compressed data, was "hlagenie-0.1.0.tar", last modified: Fri Jul  7 00:21:43 2023, max compression
```

## Comparing `hlagenie-0.0.4.tar` & `hlagenie-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:14:05.596488 hlagenie-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 23:13:53.000000 hlagenie-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 23:13:53.000000 hlagenie-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-06 23:14:05.596488 hlagenie-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-06 23:13:53.000000 hlagenie-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:14:05.592488 hlagenie-0.0.4/hlagenie/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/genie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-06 23:13:53.000000 hlagenie-0.0.4/hlagenie/smart_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:14:05.596488 hlagenie-0.0.4/hlagenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 23:14:05.000000 hlagenie-0.0.4/hlagenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 23:13:53.000000 hlagenie-0.0.4/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-06 23:13:53.000000 hlagenie-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 23:14:05.596488 hlagenie-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-06 23:13:53.000000 hlagenie-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.288255 hlagenie-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 00:21:29.000000 hlagenie-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 00:21:29.000000 hlagenie-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-07 00:21:43.288255 hlagenie-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-07 00:21:29.000000 hlagenie-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.284255 hlagenie-0.1.0/hlagenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/genie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 00:21:29.000000 hlagenie-0.1.0/hlagenie/smart_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.284255 hlagenie-0.1.0/hlagenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 00:21:43.000000 hlagenie-0.1.0/hlagenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 00:21:29.000000 hlagenie-0.1.0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 00:21:29.000000 hlagenie-0.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:21:43.288255 hlagenie-0.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 00:21:29.000000 hlagenie-0.1.0/scripts/hlagenie
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-07 00:21:43.288255 hlagenie-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 00:21:29.000000 hlagenie-0.1.0/setup.py
```

### Comparing `hlagenie-0.0.4/LICENSE` & `hlagenie-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.4/PKG-INFO` & `hlagenie-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlagenie
-Version: 0.0.4
+Version: 0.1.0
 Summary: Sequence handing for HLA with Python
 Home-page: https://github.com/gbiagini/hlagenie
 Author: Giovanni Biagini
 Author-email: dbiagini@tulane.edu
 License: LGPL 3.0
 Keywords: hlagenie
 Classifier: Development Status :: 3 - Alpha
@@ -36,14 +36,19 @@
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
+  - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
+    - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
+    - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
+    - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
+    - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -161,7 +166,52 @@
 #### Get the extracellular domain sequence of an allele
 
 The `getXRD` function takes as input an allele name and returns the extracellular domain sequence of that allele.
 
 ```python
 genie.getXRD("A*01:01")
 ```
+
+### Using `hlagenie` from the command line
+
+Some command-line functions are now available.
+
+- Retrieval of specific amino acid positions
+- Retrieval of ARD sequence
+- Retrieval of XRD sequence
+- Retrieval of mature protein sequence
+
+Note that the gapped sequences can be retrieved for any of the following by passing the `--gapped` flag.
+
+#### Retrieval of specific amino acid positions
+
+Calling `hlagenie` from the command line with an allele name and space-delimited list of positions will allow you to retrieve the amino acid at those positions.
+
+```bash
+hlagenie -a "A*01:01" -p 1 2 3 4 5 # returns 1G_2S_3H_4S_5M
+```
+
+#### Retrieval of ARD sequence
+
+Calling `hlagenie` from the command line with an allele name and the `--ard` flag will allow you to retrieve the ARD sequence of that allele.
+
+```bash
+hlagenie -a "A*01:01" --ard
+```
+
+#### Retrieval of XRD sequence
+
+Calling `hlagenie` from the command line with an allele name and the `--xrd` flag will allow you to retrieve the XRD sequence of that allele.
+
+```bash
+hlagene -a "A*01:01" --xrd
+```
+
+#### Retrieval of mature protein sequence
+
+Calling `hlagenie` from the command line with only an allele name will allow you to retrieve the mature protein sequence of that allele.
+
+```bash
+
+hlagenie -a "A*01:01"
+```
+
```

### Comparing `hlagenie-0.0.4/README.md` & `hlagenie-0.1.0/hlagenie.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: hlagenie
+Version: 0.1.0
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
 
@@ -17,14 +36,19 @@
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
+  - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
+    - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
+    - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
+    - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
+    - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -141,8 +165,53 @@
 
 #### Get the extracellular domain sequence of an allele
 
 The `getXRD` function takes as input an allele name and returns the extracellular domain sequence of that allele.
 
 ```python
 genie.getXRD("A*01:01")
-```
+```
+
+### Using `hlagenie` from the command line
+
+Some command-line functions are now available.
+
+- Retrieval of specific amino acid positions
+- Retrieval of ARD sequence
+- Retrieval of XRD sequence
+- Retrieval of mature protein sequence
+
+Note that the gapped sequences can be retrieved for any of the following by passing the `--gapped` flag.
+
+#### Retrieval of specific amino acid positions
+
+Calling `hlagenie` from the command line with an allele name and space-delimited list of positions will allow you to retrieve the amino acid at those positions.
+
+```bash
+hlagenie -a "A*01:01" -p 1 2 3 4 5 # returns 1G_2S_3H_4S_5M
+```
+
+#### Retrieval of ARD sequence
+
+Calling `hlagenie` from the command line with an allele name and the `--ard` flag will allow you to retrieve the ARD sequence of that allele.
+
+```bash
+hlagenie -a "A*01:01" --ard
+```
+
+#### Retrieval of XRD sequence
+
+Calling `hlagenie` from the command line with an allele name and the `--xrd` flag will allow you to retrieve the XRD sequence of that allele.
+
+```bash
+hlagene -a "A*01:01" --xrd
+```
+
+#### Retrieval of mature protein sequence
+
+Calling `hlagenie` from the command line with only an allele name will allow you to retrieve the mature protein sequence of that allele.
+
+```bash
+
+hlagenie -a "A*01:01"
+```
+
```

### Comparing `hlagenie-0.0.4/hlagenie/data_repository.py` & `hlagenie-0.1.0/hlagenie/data_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -225,15 +225,18 @@
     :param db_conn: The database connection object
     :param seqs: dictionary of sequences to get reference sequence
     :return: dictionary of ARD ending positions
     """
 
     # check if the table exists so as to not rebuild if unnecessary
     if db.table_exists(db_conn, "gapped_ard"):
-        return db.load_dict(db_conn, "gapped_ard", ("locus", "ard_end"))
+        ard_ends = db.load_dict(db_conn, "gapped_ard", ("locus", "ard_end"))
+        # convert the values to integers
+        ard_ends = dict(map(lambda x: (x[0], int(x[1])), ard_ends.items()))
+        return ard_ends
 
     # initialize dictionary to store ard positions
     ard_ends = {}
 
     # iterate through loci
     for locus in config["loci"]:
         # get the reference allele
@@ -245,15 +248,15 @@
         # get the reference sequence
         ref_seq = seqs[ref_allele]
 
         # get the end coordinates based on reference sequence
         end_coords = coordinate_end(ref_seq, regex)
 
         # add to dictionary
-        ard_ends[locus] = end_coords
+        ard_ends[locus] = int(end_coords)
 
     # save the dictionary to the database
     db.save_dict(db_conn, "gapped_ard", ard_ends, ("locus", "ard_end"))
 
     return ard_ends
 
 
@@ -264,15 +267,18 @@
     :param db_conn: The database connection object
     :param seqs: dictionary of sequences to get reference sequence
     :return: dictionary of XRD ending positions
     """
 
     # check if the table exists so as to not rebuild if unnecessary
     if db.table_exists(db_conn, "gapped_xrd"):
-        return db.load_dict(db_conn, "gapped_xrd", ("locus", "xrd_end"))
+        xrd_ends = db.load_dict(db_conn, "gapped_xrd", ("locus", "xrd_end"))
+        # convert the values to integers
+        xrd_ends = dict(map(lambda x: (x[0], int(x[1])), xrd_ends.items()))
+        return xrd_ends
 
     # initialize dictionary to store ard positions
     xrd_ends = {}
 
     # iterate through loci
     for locus in config["loci"]:
         # get the reference allele
@@ -284,15 +290,15 @@
         # get the reference sequence
         ref_seq = seqs[ref_allele]
 
         # get the end coordinates based on reference sequence
         end_coords = coordinate_end(ref_seq, regex)
 
         # add to dictionary
-        xrd_ends[locus] = end_coords
+        xrd_ends[locus] = int(end_coords)
 
     # save the dictionary to the database
     db.save_dict(db_conn, "gapped_xrd", xrd_ends, ("locus", "xrd_end"))
 
     return xrd_ends
 
 
@@ -303,15 +309,18 @@
     :param db_conn: The database connection object
     :param seqs: dictionary of sequences to get reference sequence
     :return: dictionary of ARD ending positions
     """
 
     # check if the table exists so as to not rebuild if unnecessary
     if db.table_exists(db_conn, "ungapped_ard"):
-        return db.load_dict(db_conn, "ungapped_ard", ("locus", "ard_end"))
+        ard_ends = db.load_dict(db_conn, "ungapped_ard", ("locus", "ard_end"))
+        # convert the values to integers
+        ard_ends = dict(map(lambda x: (x[0], int(x[1])), ard_ends.items()))
+        return ard_ends
 
     # initialize dictionary to store ard positions
     ard_ends = {}
 
     # iterate through loci
     for locus in config["loci"]:
         # get the reference allele
@@ -323,15 +332,15 @@
         # get the reference sequence
         ref_seq = seqs[ref_allele]
 
         # get the end coordinates based on reference sequence
         end_coords = coordinate_end(ref_seq, regex)
 
         # add to dictionary
-        ard_ends[locus] = end_coords
+        ard_ends[locus] = int(end_coords)
 
     # save the dictionary to the database
     db.save_dict(db_conn, "ungapped_ard", ard_ends, ("locus", "ard_end"))
 
     return ard_ends
 
 
@@ -342,15 +351,18 @@
     :param db_conn: The database connection object
     :param seqs: dictionary of sequences to get reference sequence
     :return: dictionary of XRD ending positions
     """
 
     # check if the table exists so as to not rebuild if unnecessary
     if db.table_exists(db_conn, "ungapped_xrd"):
-        return db.load_dict(db_conn, "ungapped_xrd", ("locus", "xrd_end"))
+        xrd_ends = db.load_dict(db_conn, "ungapped_xrd", ("locus", "xrd_end"))
+        # convert the values to integers
+        xrd_ends = dict(map(lambda x: (x[0], int(x[1])), xrd_ends.items()))
+        return xrd_ends
 
     # initialize dictionary to store ard positions
     xrd_ends = {}
 
     # iterate through loci
     for locus in config["loci"]:
         # get the reference allele
@@ -362,13 +374,13 @@
         # get the reference sequence
         ref_seq = seqs[ref_allele]
 
         # get the end coordinates based on reference sequence
         end_coords = coordinate_end(ref_seq, regex)
 
         # add to dictionary
-        xrd_ends[locus] = end_coords
+        xrd_ends[locus] = int(end_coords)
 
     # save the dictionary to the database
     db.save_dict(db_conn, "ungapped_xrd", xrd_ends, ("locus", "xrd_end"))
 
     return xrd_ends
```

### Comparing `hlagenie-0.0.4/hlagenie/db.py` & `hlagenie-0.1.0/hlagenie/db.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.4/hlagenie/genie.py` & `hlagenie-0.1.0/hlagenie/genie.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 self.db_connection, imgt_version
             )
             self.seqs = dr.generate_ungapped_mature_tables(self.db_connection)
             self.ards = dr.generate_ungapped_ard_table(self.db_connection, self.seqs)
             self.xrds = dr.generate_ungapped_xrd_table(self.db_connection, self.seqs)
         else:
             self.full_seqs = dr.generate_gapped_tables(self.db_connection, imgt_version)
-            self.seqs = dr.generated_gapped_mature_tables(self.db_connection)
+            self.seqs = dr.generate_gapped_mature_tables(self.db_connection)
             self.ards = dr.generate_gapped_ard_table(self.db_connection, self.seqs)
             self.xrds = dr.generate_gapped_xrd_table(self.db_connection, self.seqs)
 
     def getAA(self, allele, position):
         """
         Get the amino acid at a specific position in an allele
```

### Comparing `hlagenie-0.0.4/hlagenie/load.py` & `hlagenie-0.1.0/hlagenie/load.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.4/hlagenie/misc.py` & `hlagenie-0.1.0/hlagenie/misc.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.4/hlagenie/smart_sort.py` & `hlagenie-0.1.0/hlagenie/smart_sort.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.4/hlagenie.egg-info/PKG-INFO` & `hlagenie-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: hlagenie
-Version: 0.0.4
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
 
@@ -36,14 +17,19 @@
     - [Retrieve amino acid substring from mature protein sequence](#retrieve-amino-acid-substring-from-mature-protein-sequence)
     - [Retrieve epitope from mature protein sequence](#retrieve-epitope-from-mature-protein-sequence)
     - [Check if two alleles have a mismatch at a given position](#check-if-two-alleles-have-a-mismatch-at-a-given-position)
     - [Count the number of amino acid mismatches at a position between donor and recipient](#count-the-number-of-amino-acid-mismatches-at-a-position-between-donor-and-recipient)
     - [Count the number of amino acid mismatches between donor and recipient at a given position given the alleles](#count-the-number-of-amino-acid-mismatches-between-donor-and-recipient-at-a-given-position-given-the-alleles)
     - [Get the antigen recognition domain sequence of an allele](#get-the-antigen-recognition-domain-sequence-of-an-allele)
     - [Get the extracellular domain sequence of an allele](#get-the-extracellular-domain-sequence-of-an-allele)
+  - [Using `hlagenie` from the command line](#using-hlagenie-from-the-command-line)
+    - [Retrieval of specific amino acid positions](#retrieval-of-specific-amino-acid-positions)
+    - [Retrieval of ARD sequence](#retrieval-of-ard-sequence)
+    - [Retrieval of XRD sequence](#retrieval-of-xrd-sequence)
+    - [Retrieval of mature protein sequence](#retrieval-of-mature-protein-sequence)
 
 ## Installation
 
 ### Install from PyPI
 
 ``` pip install hlagenie ```
 
@@ -161,7 +147,52 @@
 #### Get the extracellular domain sequence of an allele
 
 The `getXRD` function takes as input an allele name and returns the extracellular domain sequence of that allele.
 
 ```python
 genie.getXRD("A*01:01")
 ```
+
+### Using `hlagenie` from the command line
+
+Some command-line functions are now available.
+
+- Retrieval of specific amino acid positions
+- Retrieval of ARD sequence
+- Retrieval of XRD sequence
+- Retrieval of mature protein sequence
+
+Note that the gapped sequences can be retrieved for any of the following by passing the `--gapped` flag.
+
+#### Retrieval of specific amino acid positions
+
+Calling `hlagenie` from the command line with an allele name and space-delimited list of positions will allow you to retrieve the amino acid at those positions.
+
+```bash
+hlagenie -a "A*01:01" -p 1 2 3 4 5 # returns 1G_2S_3H_4S_5M
+```
+
+#### Retrieval of ARD sequence
+
+Calling `hlagenie` from the command line with an allele name and the `--ard` flag will allow you to retrieve the ARD sequence of that allele.
+
+```bash
+hlagenie -a "A*01:01" --ard
+```
+
+#### Retrieval of XRD sequence
+
+Calling `hlagenie` from the command line with an allele name and the `--xrd` flag will allow you to retrieve the XRD sequence of that allele.
+
+```bash
+hlagene -a "A*01:01" --xrd
+```
+
+#### Retrieval of mature protein sequence
+
+Calling `hlagenie` from the command line with only an allele name will allow you to retrieve the mature protein sequence of that allele.
+
+```bash
+
+hlagenie -a "A*01:01"
+```
+
```

### Comparing `hlagenie-0.0.4/setup.py` & `hlagenie-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,28 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="hlagenie",
-    version="0.0.4",
+    version="0.1.0",
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
-    scripts=[],
+    scripts=[
+        "scripts/hlagenie",
+    ],
     install_requires=requirements,
     license="LGPL 3.0",
     zip_safe=False,
     keywords="hlagenie",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
```

