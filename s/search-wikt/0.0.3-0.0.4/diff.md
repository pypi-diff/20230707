# Comparing `tmp/search_wikt-0.0.3.tar.gz` & `tmp/search_wikt-0.0.4.tar.gz`

## Comparing `search_wikt-0.0.3.tar` & `search_wikt-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 search_wikt-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 search_wikt-0.0.3/src/search_wikt/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 search_wikt-0.0.3/src/search_wikt/__main__.py
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 search_wikt-0.0.3/src/search_wikt/core.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 search_wikt-0.0.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 search_wikt-0.0.3/LICENSE
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 search_wikt-0.0.3/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 search_wikt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 search_wikt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 search_wikt-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 search_wikt-0.0.4/src/search_wikt/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 search_wikt-0.0.4/src/search_wikt/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 search_wikt-0.0.4/src/search_wikt/core/__init__.py
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 search_wikt-0.0.4/src/search_wikt/core/core.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 search_wikt-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 search_wikt-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 search_wikt-0.0.4/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 search_wikt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 search_wikt-0.0.4/PKG-INFO
```

### Comparing `search_wikt-0.0.3/src/search_wikt/core.py` & `search_wikt-0.0.4/src/search_wikt/core/core.py`

 * *Files identical despite different names*

### Comparing `search_wikt-0.0.3/LICENSE` & `search_wikt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `search_wikt-0.0.3/README.md` & `search_wikt-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ### Search Wiktionary
 
 A simple command-line tool for searching English Wiktionary using Wiktionary Parser ([click](https://github.com/Suyash458/WiktionaryParser)).
 
 Wiktionary definitions are licensed under CC BY-SA 4.0. Visit wiktionary at wiktionary.org ([click](wiktionary.org)).
-
 #### Installation
 To install, type:
 ```
 pip install search_wikt
 ```
 To run the program, type:
 ```
```

### Comparing `search_wikt-0.0.3/pyproject.toml` & `search_wikt-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "search_wikt"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="lauramvx", email="lesbianhouse@gmx.com" },
 ]
 description = "A simple command-line tool for searching Wiktionary."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `search_wikt-0.0.3/PKG-INFO` & `search_wikt-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search_wikt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple command-line tool for searching Wiktionary.
 Author-email: lauramvx <lesbianhouse@gmx.com>
 License-File: LICENSE
 Keywords: CLI,Wiktionary,dictionary,etymology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,14 @@
 Description-Content-Type: text/markdown
 
 ### Search Wiktionary
 
 A simple command-line tool for searching English Wiktionary using Wiktionary Parser ([click](https://github.com/Suyash458/WiktionaryParser)).
 
 Wiktionary definitions are licensed under CC BY-SA 4.0. Visit wiktionary at wiktionary.org ([click](wiktionary.org)).
-
 #### Installation
 To install, type:
 ```
 pip install search_wikt
 ```
 To run the program, type:
 ```
```

