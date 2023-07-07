# Comparing `tmp/modernmetric-1.0.0.tar.gz` & `tmp/modernmetric-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernmetric-1.0.0.tar", last modified: Sat Jun 24 14:04:05 2023, max compression
+gzip compressed data, was "modernmetric-1.0.2.tar", last modified: Fri Jul  7 18:29:54 2023, max compression
```

## Comparing `modernmetric-1.0.0.tar` & `modernmetric-1.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.917190 modernmetric-1.0.0/
--rw-r--r--   0 jason     (1000) jason     (1000)     1486 2023-06-24 13:59:39.000000 modernmetric-1.0.0/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)       59 2023-03-27 09:12:10.000000 modernmetric-1.0.0/MANIFEST.in
--rw-r--r--   0 jason     (1000) jason     (1000)     1019 2023-06-24 14:04:05.917190 modernmetric-1.0.0/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     6981 2023-06-24 13:58:02.000000 modernmetric-1.0.0/README.md
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.907190 modernmetric-1.0.0/modernmetric/
--rw-r--r--   0 jason     (1000) jason     (1000)       18 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4393 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/__main__.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.907190 modernmetric-1.0.0/modernmetric/cls/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)      722 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/base.py
--rw-r--r--   0 jason     (1000) jason     (1000)      278 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/base_calc.py
--rw-r--r--   0 jason     (1000) jason     (1000)      284 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/base_stats.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.917190 modernmetric-1.0.0/modernmetric/cls/calc/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/calc/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     3380 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/calc/halstead.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1968 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/calc/maintenance.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2195 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/calc/pylint.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4632 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/calc/tiobe.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.917190 modernmetric-1.0.0/modernmetric/cls/importer/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/importer/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1061 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/importer/base.py
--rw-r--r--   0 jason     (1000) jason     (1000)      375 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/importer/filtered.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.917190 modernmetric-1.0.0/modernmetric/cls/importer/mods/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/importer/mods/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)      535 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/importer/mods/csv.py
--rw-r--r--   0 jason     (1000) jason     (1000)      687 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/importer/mods/json.py
--rw-r--r--   0 jason     (1000) jason     (1000)      556 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/importer/pick.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.917190 modernmetric-1.0.0/modernmetric/cls/metric/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/metric/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1715 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/metric/comments.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1682 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/metric/cyclomatic.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4258 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/metric/fanout.py
--rw-r--r--   0 jason     (1000) jason     (1000)      908 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/metric/loc.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2395 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/metric/operands.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1584 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/metric/operators.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2118 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/modules.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.917190 modernmetric-1.0.0/modernmetric/cls/stats/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 modernmetric-1.0.0/modernmetric/cls/stats/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1358 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/cls/stats/stats.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1683 2023-06-24 13:54:21.000000 modernmetric-1.0.0/modernmetric/fp.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-24 14:04:05.907190 modernmetric-1.0.0/modernmetric.egg-info/
--rw-r--r--   0 jason     (1000) jason     (1000)     1019 2023-06-24 14:04:05.000000 modernmetric-1.0.0/modernmetric.egg-info/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     1232 2023-06-24 14:04:05.000000 modernmetric-1.0.0/modernmetric.egg-info/SOURCES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-06-24 14:04:05.000000 modernmetric-1.0.0/modernmetric.egg-info/dependency_links.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       60 2023-06-24 14:04:05.000000 modernmetric-1.0.0/modernmetric.egg-info/entry_points.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-06-24 14:04:05.000000 modernmetric-1.0.0/modernmetric.egg-info/requires.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       13 2023-06-24 14:04:05.000000 modernmetric-1.0.0/modernmetric.egg-info/top_level.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-06-09 19:24:40.000000 modernmetric-1.0.0/requirements.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-06-24 14:04:05.917190 modernmetric-1.0.0/setup.cfg
--rw-r--r--   0 jason     (1000) jason     (1000)     1770 2023-06-24 14:00:17.000000 modernmetric-1.0.0/setup.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.095144 modernmetric-1.0.2/
+-rw-r--r--   0 jason     (1000) jason     (1000)     1486 2023-07-07 18:20:19.000000 modernmetric-1.0.2/LICENSE
+-rw-r--r--   0 jason     (1000) jason     (1000)       59 2023-03-27 09:12:10.000000 modernmetric-1.0.2/MANIFEST.in
+-rw-r--r--   0 jason     (1000) jason     (1000)     1019 2023-07-07 18:29:54.095144 modernmetric-1.0.2/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)     7340 2023-07-07 18:20:19.000000 modernmetric-1.0.2/README.md
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.085144 modernmetric-1.0.2/modernmetric/
+-rw-r--r--   0 jason     (1000) jason     (1000)       18 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     4946 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/__main__.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.085144 modernmetric-1.0.2/modernmetric/cls/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      722 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/base.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      278 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/base_calc.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      284 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/base_stats.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.085144 modernmetric-1.0.2/modernmetric/cls/calc/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/calc/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     3380 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/calc/halstead.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1968 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/calc/maintenance.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     2195 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/calc/pylint.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     4632 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/calc/tiobe.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.085144 modernmetric-1.0.2/modernmetric/cls/importer/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/importer/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1061 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/importer/base.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      375 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/importer/filtered.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.095144 modernmetric-1.0.2/modernmetric/cls/importer/mods/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/importer/mods/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      535 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/importer/mods/csv.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      687 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/importer/mods/json.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      556 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/importer/pick.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.095144 modernmetric-1.0.2/modernmetric/cls/metric/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/metric/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1715 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/metric/comments.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1682 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/metric/cyclomatic.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     4258 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/metric/fanout.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      908 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/metric/loc.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     2395 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/metric/operands.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1584 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/metric/operators.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     2118 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/modules.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.095144 modernmetric-1.0.2/modernmetric/cls/stats/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/stats/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1358 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/cls/stats/stats.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1683 2023-07-07 18:20:19.000000 modernmetric-1.0.2/modernmetric/fp.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-07-07 18:29:54.085144 modernmetric-1.0.2/modernmetric.egg-info/
+-rw-r--r--   0 jason     (1000) jason     (1000)     1019 2023-07-07 18:29:54.000000 modernmetric-1.0.2/modernmetric.egg-info/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)     1232 2023-07-07 18:29:54.000000 modernmetric-1.0.2/modernmetric.egg-info/SOURCES.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-07-07 18:29:54.000000 modernmetric-1.0.2/modernmetric.egg-info/dependency_links.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       60 2023-07-07 18:29:54.000000 modernmetric-1.0.2/modernmetric.egg-info/entry_points.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-07-07 18:29:54.000000 modernmetric-1.0.2/modernmetric.egg-info/requires.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       13 2023-07-07 18:29:54.000000 modernmetric-1.0.2/modernmetric.egg-info/top_level.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-06-09 19:24:40.000000 modernmetric-1.0.2/requirements.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-07-07 18:29:54.095144 modernmetric-1.0.2/setup.cfg
+-rw-r--r--   0 jason     (1000) jason     (1000)     1770 2023-07-07 18:20:36.000000 modernmetric-1.0.2/setup.py
```

### Comparing `modernmetric-1.0.0/LICENSE` & `modernmetric-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/PKG-INFO` & `modernmetric-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmetric
-Version: 1.0.0
+Version: 1.0.2
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/startupos/multimetric
 Author: Jason Nichols
 Author-email: jason@startupos.dev
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `modernmetric-1.0.0/README.md` & `modernmetric-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -49,23 +49,33 @@
 usage: modernmetric [-h] [--warn_compiler WARN_COMPILER]
                    [--warn_duplication WARN_DUPLICATION]
                    [--warn_functional WARN_FUNCTIONAL]
                    [--warn_standard WARN_STANDARD]
                    [--warn_security WARN_SECURITY] [--coverage COVERAGE]
                    [--bugpredict {old,new}]
                    [--maintindex {sei,classic,microsoft}]
+                   [--file=path_to_filelist]
+                   AND/OR
                    files [files ...]
 
 Calculate code metrics in various languages
 
 positional arguments:
   files                 Files to parse
 
 optional arguments:
   -h, --help            show this help message and exit
+  --file=path_to_filelist
+                    Path to JSON filelist to scan. Format is:
+                    [
+                        {
+                            "name": "test.c",
+                            "path": "../testfiles/test.c"
+                        }
+                    ]
   --warn_compiler WARN_COMPILER
                         File(s) holding information about compiler warnings
   --warn_duplication WARN_DUPLICATION
                         File(s) holding information about code duplications
   --warn_functional WARN_FUNCTIONAL
                         File(s) holding information about static code analysis findings
   --warn_standard WARN_STANDARD
```

### Comparing `modernmetric-1.0.0/modernmetric/__main__.py` & `modernmetric-1.0.2/modernmetric/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import argparse
 import json
 import os
 import textwrap
 import multiprocessing as mp
 
-
 from modernmetric.cls.importer.pick import importer_pick
 from modernmetric.cls.modules import get_additional_parser_args
 from modernmetric.cls.modules import get_modules_calculated
 from modernmetric.cls.modules import get_modules_metrics
 from modernmetric.cls.modules import get_modules_stats
 from modernmetric.fp import file_process
 
+
 def ArgParser():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawTextHelpFormatter,
         prog="modernmetric", description='Calculate code metrics in various languages',
         epilog=textwrap.dedent("""
         Currently you could import files of the following types for --warn_* or --coverage
 
@@ -35,14 +35,15 @@
 
         json: JSON file
              <file>: {
                  "content": <content>,
                  "severity": <severity>
              }
         """))
+
     parser.add_argument(
         "--warn_compiler",
         default=None,
         help="File(s) holding information about compiler warnings")
     parser.add_argument(
         "--warn_duplication",
         default=None,
@@ -74,16 +75,31 @@
         default=1,
         help="Run x jobs in parallel")
     parser.add_argument(
         "--ignore_lexer_errors",
         default=True,
         help="Ignore unparseable files")
     get_additional_parser_args(parser)
-    parser.add_argument("files", nargs='+', help="Files to parse")
+
+    parser.add_argument('--file', type=str, help='Path to the JSON file list of file paths')
+    parser.add_argument('files', metavar='file', type=str, nargs='*', help='List of file paths')
+
     RUNARGS = parser.parse_args()
+
+    file_paths = RUNARGS.files
+    input_file = RUNARGS.file
+
+    if not file_paths and not input_file: # No file passed in, read filelist from command line
+        raise Exception("No filelist provided. Provide path to file list with --file=<path>")
+    if input_file:
+        with open(input_file) as file:
+            data = json.load(file)
+            for file in data:
+                RUNARGS.files.append(file["path"])
+
     # Turn all paths to abs-paths right here
     RUNARGS.files = [os.path.abspath(x) for x in RUNARGS.files]
     return RUNARGS
 
 def main():
     _args = ArgParser()
     _result = {"files": {}, "overall": {}}
```

### Comparing `modernmetric-1.0.0/modernmetric/cls/base.py` & `modernmetric-1.0.2/modernmetric/cls/base.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/calc/halstead.py` & `modernmetric-1.0.2/modernmetric/cls/calc/halstead.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/calc/maintenance.py` & `modernmetric-1.0.2/modernmetric/cls/calc/maintenance.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/calc/pylint.py` & `modernmetric-1.0.2/modernmetric/cls/calc/pylint.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/calc/tiobe.py` & `modernmetric-1.0.2/modernmetric/cls/calc/tiobe.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/importer/base.py` & `modernmetric-1.0.2/modernmetric/cls/importer/base.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/importer/mods/csv.py` & `modernmetric-1.0.2/modernmetric/cls/importer/mods/csv.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/importer/mods/json.py` & `modernmetric-1.0.2/modernmetric/cls/importer/mods/json.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/importer/pick.py` & `modernmetric-1.0.2/modernmetric/cls/importer/pick.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/metric/comments.py` & `modernmetric-1.0.2/modernmetric/cls/metric/comments.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/metric/cyclomatic.py` & `modernmetric-1.0.2/modernmetric/cls/metric/cyclomatic.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/metric/fanout.py` & `modernmetric-1.0.2/modernmetric/cls/metric/fanout.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/metric/loc.py` & `modernmetric-1.0.2/modernmetric/cls/metric/loc.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/metric/operands.py` & `modernmetric-1.0.2/modernmetric/cls/metric/operands.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/metric/operators.py` & `modernmetric-1.0.2/modernmetric/cls/metric/operators.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/modules.py` & `modernmetric-1.0.2/modernmetric/cls/modules.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/cls/stats/stats.py` & `modernmetric-1.0.2/modernmetric/cls/stats/stats.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric/fp.py` & `modernmetric-1.0.2/modernmetric/fp.py`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/modernmetric.egg-info/PKG-INFO` & `modernmetric-1.0.2/modernmetric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmetric
-Version: 1.0.0
+Version: 1.0.2
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/startupos/multimetric
 Author: Jason Nichols
 Author-email: jason@startupos.dev
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `modernmetric-1.0.0/modernmetric.egg-info/SOURCES.txt` & `modernmetric-1.0.2/modernmetric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modernmetric-1.0.0/setup.py` & `modernmetric-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="modernmetric",
-    version="1.0.0",
+    version="1.0.2",
     author="Jason Nichols",
     author_email="jason@startupos.dev",
     description="Calculate code metrics in various languages",
     long_description=_long_description,
     long_description_content_type=_long_description_content_type,
     url="https://github.com/startupos/multimetric",
     packages=setuptools.find_packages(),
```

