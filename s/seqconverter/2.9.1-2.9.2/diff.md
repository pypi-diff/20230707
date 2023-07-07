# Comparing `tmp/seqconverter-2.9.1.tar.gz` & `tmp/seqconverter-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqconverter-2.9.1.tar", last modified: Thu Mar 30 07:59:20 2023, max compression
+gzip compressed data, was "seqconverter-2.9.2.tar", last modified: Mon Jul  3 12:57:59 2023, max compression
```

## Comparing `seqconverter-2.9.1.tar` & `seqconverter-2.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-03-30 07:59:20.661372 seqconverter-2.9.1/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2021-11-29 16:03:18.000000 seqconverter-2.9.1/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)    13728 2023-03-30 07:59:20.661437 seqconverter-2.9.1/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)    13212 2023-03-30 07:58:09.000000 seqconverter-2.9.1/README.md
--rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 seqconverter-2.9.1/pyproject.toml
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-03-30 07:59:20.661260 seqconverter-2.9.1/seqconverter.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)    13728 2023-03-30 07:59:20.000000 seqconverter-2.9.1/seqconverter.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      276 2023-03-30 07:59:20.000000 seqconverter-2.9.1/seqconverter.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2023-03-30 07:59:20.000000 seqconverter-2.9.1/seqconverter.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       51 2023-03-30 07:59:20.000000 seqconverter-2.9.1/seqconverter.egg-info/entry_points.txt
--rw-r--r--   0 agpe       (502) staff       (20)       26 2023-03-30 07:59:20.000000 seqconverter-2.9.1/seqconverter.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)       13 2023-03-30 07:59:20.000000 seqconverter-2.9.1/seqconverter.egg-info/top_level.txt
--rwxr-xr-x   0 agpe       (502) staff       (20)    35993 2023-03-29 07:50:56.000000 seqconverter-2.9.1/seqconverter.py
--rw-r--r--   0 agpe       (502) staff       (20)      711 2023-03-30 07:59:20.661734 seqconverter-2.9.1/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-03 12:57:59.505326 seqconverter-2.9.2/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2021-11-29 16:03:18.000000 seqconverter-2.9.2/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)    13728 2023-07-03 12:57:59.505386 seqconverter-2.9.2/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)    13212 2023-07-03 12:56:18.000000 seqconverter-2.9.2/README.md
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 seqconverter-2.9.2/pyproject.toml
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-03 12:57:59.505202 seqconverter-2.9.2/seqconverter.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)    13728 2023-07-03 12:57:59.000000 seqconverter-2.9.2/seqconverter.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      276 2023-07-03 12:57:59.000000 seqconverter-2.9.2/seqconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2023-07-03 12:57:59.000000 seqconverter-2.9.2/seqconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       51 2023-07-03 12:57:59.000000 seqconverter-2.9.2/seqconverter.egg-info/entry_points.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       26 2023-07-03 12:57:59.000000 seqconverter-2.9.2/seqconverter.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       13 2023-07-03 12:57:59.000000 seqconverter-2.9.2/seqconverter.egg-info/top_level.txt
+-rwxr-xr-x   0 agpe       (502) staff       (20)    35993 2023-03-29 07:50:56.000000 seqconverter-2.9.2/seqconverter.py
+-rw-r--r--   0 agpe       (502) staff       (20)      711 2023-07-03 12:57:59.505663 seqconverter-2.9.2/setup.cfg
```

### Comparing `seqconverter-2.9.1/LICENSE` & `seqconverter-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seqconverter-2.9.1/PKG-INFO` & `seqconverter-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: seqconverter
-Version: 2.9.1
+Version: 2.9.2
 Summary: Reads and writes sequence files in various formats. Performs manipulations on sequences
 Home-page: https://github.com/agormp/seqconverter
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # seqconverter
 
-![](https://img.shields.io/badge/version-2.9.1-blue)
+![](https://img.shields.io/badge/version-2.9.2-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/seqconverter?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/seqconverter)
 
 The command-line program `seqconverter` can read and write text files containing aligned or unaligned DNA or protein sequences. The program understands most standard and some non-standard formats (fasta, Nexus, Phylip, Clustal, Stockholm, tab, raw, Genbank, How). The program can perform various manipulations on the sequences.
 
 ## Availability
 
 The seqconverter source code is available on GitHub: https://github.com/agormp/seqconverter. The executable can be installed from PyPI: https://pypi.org/project/seqconverter/
```

### Comparing `seqconverter-2.9.1/README.md` & `seqconverter-2.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # seqconverter
 
-![](https://img.shields.io/badge/version-2.9.1-blue)
+![](https://img.shields.io/badge/version-2.9.2-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/seqconverter?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/seqconverter)
 
 The command-line program `seqconverter` can read and write text files containing aligned or unaligned DNA or protein sequences. The program understands most standard and some non-standard formats (fasta, Nexus, Phylip, Clustal, Stockholm, tab, raw, Genbank, How). The program can perform various manipulations on the sequences.
 
 ## Availability
 
 The seqconverter source code is available on GitHub: https://github.com/agormp/seqconverter. The executable can be installed from PyPI: https://pypi.org/project/seqconverter/
```

### Comparing `seqconverter-2.9.1/seqconverter.egg-info/PKG-INFO` & `seqconverter-2.9.2/seqconverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: seqconverter
-Version: 2.9.1
+Version: 2.9.2
 Summary: Reads and writes sequence files in various formats. Performs manipulations on sequences
 Home-page: https://github.com/agormp/seqconverter
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # seqconverter
 
-![](https://img.shields.io/badge/version-2.9.1-blue)
+![](https://img.shields.io/badge/version-2.9.2-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/seqconverter?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/seqconverter)
 
 The command-line program `seqconverter` can read and write text files containing aligned or unaligned DNA or protein sequences. The program understands most standard and some non-standard formats (fasta, Nexus, Phylip, Clustal, Stockholm, tab, raw, Genbank, How). The program can perform various manipulations on the sequences.
 
 ## Availability
 
 The seqconverter source code is available on GitHub: https://github.com/agormp/seqconverter. The executable can be installed from PyPI: https://pypi.org/project/seqconverter/
```

### Comparing `seqconverter-2.9.1/seqconverter.py` & `seqconverter-2.9.2/seqconverter.py`

 * *Files identical despite different names*

