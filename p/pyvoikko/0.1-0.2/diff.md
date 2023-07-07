# Comparing `tmp/pyvoikko-0.1.tar.gz` & `tmp/pyvoikko-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoikko-0.1.tar", last modified: Thu Jul  6 22:26:35 2023, max compression
+gzip compressed data, was "pyvoikko-0.2.tar", last modified: Fri Jul  7 11:10:04 2023, max compression
```

## Comparing `pyvoikko-0.1.tar` & `pyvoikko-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 22:26:35.386964 pyvoikko-0.1/
--rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-06 21:40:03.000000 pyvoikko-0.1/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-06 22:26:35.387012 pyvoikko-0.1/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1098 2023-07-06 22:23:41.000000 pyvoikko-0.1/README.md
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:43.000000 pyvoikko-0.1/pyproject.toml
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 22:26:35.385720 pyvoikko-0.1/pyvoikko/
--rw-r--r--   0 iikka      (501) staff       (20)      558 2023-07-06 21:49:07.000000 pyvoikko-0.1/pyvoikko/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)     5129 2023-07-06 22:19:12.000000 pyvoikko-0.1/pyvoikko/analysis.py
--rw-r--r--   0 iikka      (501) staff       (20)     2010 2023-07-06 21:59:47.000000 pyvoikko-0.1/pyvoikko/constants.py
--rw-r--r--   0 iikka      (501) staff       (20)  1071442 2023-07-06 20:45:08.000000 pyvoikko-0.1/pyvoikko/voikko.kfst
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 22:26:35.386811 pyvoikko-0.1/pyvoikko.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-06 22:26:35.000000 pyvoikko-0.1/pyvoikko.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)      286 2023-07-06 22:26:35.000000 pyvoikko-0.1/pyvoikko.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-06 22:26:35.000000 pyvoikko-0.1/pyvoikko.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-06 22:26:35.000000 pyvoikko-0.1/pyvoikko.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        9 2023-07-06 22:26:35.000000 pyvoikko-0.1/pyvoikko.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)      816 2023-07-06 22:26:35.387220 pyvoikko-0.1/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 11:10:04.816772 pyvoikko-0.2/
+-rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-06 21:40:03.000000 pyvoikko-0.2/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-07 11:10:04.816811 pyvoikko-0.2/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1098 2023-07-06 22:23:41.000000 pyvoikko-0.2/README.md
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:43.000000 pyvoikko-0.2/pyproject.toml
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 11:10:04.815564 pyvoikko-0.2/pyvoikko/
+-rw-r--r--   0 iikka      (501) staff       (20)      594 2023-07-07 10:42:45.000000 pyvoikko-0.2/pyvoikko/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)     5161 2023-07-07 10:42:55.000000 pyvoikko-0.2/pyvoikko/analysis.py
+-rw-r--r--   0 iikka      (501) staff       (20)     2010 2023-07-06 21:59:47.000000 pyvoikko-0.2/pyvoikko/constants.py
+-rw-r--r--   0 iikka      (501) staff       (20)  1071442 2023-07-06 20:45:08.000000 pyvoikko-0.2/pyvoikko/voikko.kfst
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 11:10:04.816668 pyvoikko-0.2/pyvoikko.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)      286 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        9 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)      816 2023-07-07 11:10:04.817015 pyvoikko-0.2/setup.cfg
```

### Comparing `pyvoikko-0.1/LICENSE` & `pyvoikko-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.1/PKG-INFO` & `pyvoikko-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyvoikko
-Version: 0.1
+Version: 0.2
 Summary: A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyVoikko
 
 PyVoikko is an implementation of Voikko, a free and open source morphological analyzer for Finnish.
 It aims to reimplement the Voikko library in pure Python, so that it can be used in environments in which native libraries like libvoikko cannot be installed.
```

### Comparing `pyvoikko-0.1/README.md` & `pyvoikko-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.1/pyvoikko/__init__.py` & `pyvoikko-0.2/pyvoikko/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os.path
 
 from kfst import FST
 
 from .analysis import VoikkoAnalysis
 
 SCRIPT_DIR = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `pyvoikko-0.1/pyvoikko/analysis.py` & `pyvoikko-0.2/pyvoikko/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 from typing import NamedTuple
 
 from .constants import MAPS, FIELD_NAMES
 
 class VoikkoAnalysis(NamedTuple):
     """
@@ -28,15 +30,15 @@
     """
 
     FORM: str
     BASEFORM: str
     CLASS: str
     FSTOUTPUT: str
     INFO_FLAGS: list[str]
-    
+
     # Verb attributes
     MOOD: str | None = None
     NEGATIVE: str | None = None
     PERSON: str | None = None
     TENSE: str | None = None
 
     # Noun attributes
```

### Comparing `pyvoikko-0.1/pyvoikko/constants.py` & `pyvoikko-0.2/pyvoikko/constants.py`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.1/pyvoikko/voikko.kfst` & `pyvoikko-0.2/pyvoikko/voikko.kfst`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.1/pyvoikko.egg-info/PKG-INFO` & `pyvoikko-0.2/pyvoikko.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyvoikko
-Version: 0.1
+Version: 0.2
 Summary: A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyVoikko
 
 PyVoikko is an implementation of Voikko, a free and open source morphological analyzer for Finnish.
 It aims to reimplement the Voikko library in pure Python, so that it can be used in environments in which native libraries like libvoikko cannot be installed.
```

### Comparing `pyvoikko-0.1/setup.cfg` & `pyvoikko-0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyvoikko
-version = 0.1
+version = 0.2
 author = Iikka Hauhio
 author_email = iikka.hauhio@helsinki.fi
 description = A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = finnish nlp morphology
 license = GNU GPLv3
@@ -16,15 +16,15 @@
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 
 [options]
 packages = pyvoikko
-python_requires = >=3.9
+python_requires = >=3.8
 install_requires = 
 	kfst
 
 [options.package_data]
 pyvoikko = *.kfst
 
 [egg_info]
```

