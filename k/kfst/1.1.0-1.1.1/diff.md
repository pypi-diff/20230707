# Comparing `tmp/kfst-1.1.0.tar.gz` & `tmp/kfst-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfst-1.1.0.tar", last modified: Thu Jul  6 21:09:07 2023, max compression
+gzip compressed data, was "kfst-1.1.1.tar", last modified: Fri Jul  7 10:32:48 2023, max compression
```

## Comparing `kfst-1.1.0.tar` & `kfst-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:09:07.316405 kfst-1.1.0/
--rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.1.0/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-06 21:09:07.316444 kfst-1.1.0/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1456 2023-07-06 13:42:57.000000 kfst-1.1.0/README.md
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:09:07.315817 kfst-1.1.0/kfst/
--rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.1.0/kfst/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)      495 2023-07-06 13:08:58.000000 kfst-1.1.0/kfst/convert.py
--rw-r--r--   0 iikka      (501) staff       (20)    17180 2023-07-06 20:44:56.000000 kfst-1.1.0/kfst/transducer.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:09:07.316330 kfst-1.1.0/kfst.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)      233 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-06 21:09:07.000000 kfst-1.1.0/kfst.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.1.0/pyproject.toml
--rw-r--r--   0 iikka      (501) staff       (20)      708 2023-07-06 21:09:07.316630 kfst-1.1.0/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:32:48.381470 kfst-1.1.1/
+-rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.1.1/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-07 10:32:48.381527 kfst-1.1.1/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1456 2023-07-06 13:42:57.000000 kfst-1.1.1/README.md
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:32:48.380401 kfst-1.1.1/kfst/
+-rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.1.1/kfst/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)     1211 2023-07-07 10:30:22.000000 kfst-1.1.1/kfst/convert.py
+-rw-r--r--   0 iikka      (501) staff       (20)    17216 2023-07-07 10:26:55.000000 kfst-1.1.1/kfst/transducer.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:32:48.381333 kfst-1.1.1/kfst.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)      233 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.1.1/pyproject.toml
+-rw-r--r--   0 iikka      (501) staff       (20)      708 2023-07-07 10:32:48.381769 kfst-1.1.1/setup.cfg
```

### Comparing `kfst-1.1.0/LICENSE` & `kfst-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kfst-1.1.0/PKG-INFO` & `kfst-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.1.0
+Version: 1.1.1
 Summary: A pure-python finite state transducer library
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KFST
 
 KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files and its own binary format.
 In addition to standard features, it also supports flag diacritics.
```

### Comparing `kfst-1.1.0/README.md` & `kfst-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kfst-1.1.0/kfst/__init__.py` & `kfst-1.1.1/kfst/__init__.py`

 * *Files identical despite different names*

### Comparing `kfst-1.1.0/kfst/transducer.py` & `kfst-1.1.1/kfst/transducer.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with KFST. If not, see <https://www.gnu.org/licenses/>. 
 
+from __future__ import annotations
+
 import argparse
 import lzma
 import re
 import struct
 from collections import defaultdict
 from pathlib import Path
 from typing import NamedTuple
```

### Comparing `kfst-1.1.0/kfst.egg-info/PKG-INFO` & `kfst-1.1.1/kfst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.1.0
+Version: 1.1.1
 Summary: A pure-python finite state transducer library
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KFST
 
 KFST is a finite state transducer library written in pure Python. It supports reading transducers from [AT&T tabular format](https://github.com/hfst/hfst/blob/master/doc/transducer-representations-formats.rst) files and its own binary format.
 In addition to standard features, it also supports flag diacritics.
```

