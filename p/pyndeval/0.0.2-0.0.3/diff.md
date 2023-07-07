# Comparing `tmp/pyndeval-0.0.2.tar.gz` & `tmp/pyndeval-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyndeval-0.0.2.tar", last modified: Fri Oct  8 15:02:11 2021, max compression
+gzip compressed data, was "pyndeval-0.0.3.tar", last modified: Fri Jul  7 09:40:40 2023, max compression
```

## Comparing `pyndeval-0.0.2.tar` & `pyndeval-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 15:02:11.776035 pyndeval-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-10-08 15:02:00.000000 pyndeval-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2021-10-08 15:02:11.776035 pyndeval-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2021-10-08 15:02:00.000000 pyndeval-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 15:02:11.776035 pyndeval-0.0.2/pyndeval/
--rw-r--r--   0 runner    (1001) docker     (121)     5924 2021-10-08 15:02:00.000000 pyndeval-0.0.2/pyndeval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 15:02:11.776035 pyndeval-0.0.2/pyndeval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2021-10-08 15:02:11.000000 pyndeval-0.0.2/pyndeval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-10-08 15:02:11.000000 pyndeval-0.0.2/pyndeval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-08 15:02:11.000000 pyndeval-0.0.2/pyndeval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-08 15:02:11.000000 pyndeval-0.0.2/pyndeval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-08 15:02:11.776035 pyndeval-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-10-08 15:02:00.000000 pyndeval-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 15:02:11.776035 pyndeval-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (121)    39592 2021-10-08 15:02:00.000000 pyndeval-0.0.2/src/ndeval.c
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2021-10-08 15:02:00.000000 pyndeval-0.0.2/src/pyndeval.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:40:40.365718 pyndeval-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 09:40:25.000000 pyndeval-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-07 09:40:40.365718 pyndeval-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-07 09:40:25.000000 pyndeval-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:40:40.361718 pyndeval-0.0.3/pyndeval/
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-07 09:40:25.000000 pyndeval-0.0.3/pyndeval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:40:40.361718 pyndeval-0.0.3/pyndeval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-07 09:40:40.000000 pyndeval-0.0.3/pyndeval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-07 09:40:40.000000 pyndeval-0.0.3/pyndeval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:40:40.000000 pyndeval-0.0.3/pyndeval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 09:40:40.000000 pyndeval-0.0.3/pyndeval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:40:40.365718 pyndeval-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-07 09:40:25.000000 pyndeval-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:40:40.365718 pyndeval-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    39593 2023-07-07 09:40:25.000000 pyndeval-0.0.3/src/ndeval.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-07 09:40:25.000000 pyndeval-0.0.3/src/pyndeval.c
```

### Comparing `pyndeval-0.0.2/PKG-INFO` & `pyndeval-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: pyndeval
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interface to ndeval.c
 Home-page: https://github.com/seanmacavaney/pyndeval
 Author: Sean MacAvaney
 Author-email: sean.macavaney@glasgow.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # pyndeval
 
 A python interface to TREC's `ndeval.c`, used for computing diversity retrieval metrics.
 
 ## Getting Started
 
+From pip:
+
 ```bash
+pip install pyndeval
+```
+
+Or install from source:
+
+```bash
+git clone https://github.com/seanmacavaney/pyndeval.git
+cd pyndeval
 python setup.py install
 ```
 
 ## Usage
 
 ```python
 import pyndeval
@@ -109,9 +117,7 @@
 
 ```python
 for result in pyndeval.ndeval_iter(qrels, run):
   {"query_id": "0", ...}
 for result in ev.evaluate_iter(run):
   {"query_id": "0", ...}
 ```
-
-
```

### Comparing `pyndeval-0.0.2/README.md` & `pyndeval-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # pyndeval
 
 A python interface to TREC's `ndeval.c`, used for computing diversity retrieval metrics.
 
 ## Getting Started
 
+From pip:
+
+```bash
+pip install pyndeval
+```
+
+Or install from source:
+
 ```bash
+git clone https://github.com/seanmacavaney/pyndeval.git
+cd pyndeval
 python setup.py install
 ```
 
 ## Usage
 
 ```python
 import pyndeval
```

### Comparing `pyndeval-0.0.2/pyndeval/__init__.py` & `pyndeval-0.0.3/pyndeval/__init__.py`

 * *Files identical despite different names*

### Comparing `pyndeval-0.0.2/pyndeval.egg-info/PKG-INFO` & `pyndeval-0.0.3/pyndeval.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: pyndeval
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interface to ndeval.c
 Home-page: https://github.com/seanmacavaney/pyndeval
 Author: Sean MacAvaney
 Author-email: sean.macavaney@glasgow.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # pyndeval
 
 A python interface to TREC's `ndeval.c`, used for computing diversity retrieval metrics.
 
 ## Getting Started
 
+From pip:
+
 ```bash
+pip install pyndeval
+```
+
+Or install from source:
+
+```bash
+git clone https://github.com/seanmacavaney/pyndeval.git
+cd pyndeval
 python setup.py install
 ```
 
 ## Usage
 
 ```python
 import pyndeval
@@ -109,9 +117,7 @@
 
 ```python
 for result in pyndeval.ndeval_iter(qrels, run):
   {"query_id": "0", ...}
 for result in ev.evaluate_iter(run):
   {"query_id": "0", ...}
 ```
-
-
```

### Comparing `pyndeval-0.0.2/setup.py` & `pyndeval-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyndeval",
-    version="0.0.2",
+    version="0.0.3",
     author="Sean MacAvaney",
     author_email="sean.macavaney@glasgow.ac.uk",
     description="Interface to ndeval.c",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/seanmacavaney/pyndeval",
     include_package_data = True,
```

### Comparing `pyndeval-0.0.2/src/ndeval.c` & `pyndeval-0.0.3/src/ndeval.c`

 * *Files 0% similar despite different names*

```diff
@@ -1432,15 +1432,15 @@
     if (argc >= 2 && strcmp ("-version", argv[1]) == 0)
       {
   printf ("%s: %s\n", programName, version);
   exit (0);
       }
     else if (argc >= 2 && strcmp ("-help", argv[1]) == 0)
       {
-  printf (helpText);
+//  print(helpText);
   exit (0);
       }
     else if (argc >= 5 && strcmp ("-alpha", argv[1]) == 0)
       {
   sscanf (argv[2], "%lf", &alpha);
   if (alpha < 0.0 || alpha > 1.0)
     usage();
@@ -1517,8 +1517,8 @@
   if (cFlag)
     actualTopics = qTopics;
   outputMeasures (rrl, rTopics, actualTopics, runid, cFlag, aFlag, brl, riskAlpha,
       (riskAlphaStr == NULL? riskAlphaDefString : riskAlphaStr),
       bTopics, brunid);
 
   return 0;
-}
+}
```

### Comparing `pyndeval-0.0.2/src/pyndeval.c` & `pyndeval-0.0.3/src/pyndeval.c`

 * *Files identical despite different names*

