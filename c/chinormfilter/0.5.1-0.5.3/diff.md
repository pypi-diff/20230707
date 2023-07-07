# Comparing `tmp/chinormfilter-0.5.1.tar.gz` & `tmp/chinormfilter-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chinormfilter-0.5.1.tar", max compression
+gzip compressed data, was "chinormfilter-0.5.3.tar", max compression
```

## Comparing `chinormfilter-0.5.1.tar` & `chinormfilter-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2021-04-09 16:02:56.291644 chinormfilter-0.5.1/LICENSE
--rw-r--r--   0        0        0      886 2021-04-13 12:04:51.567351 chinormfilter-0.5.1/README.md
--rw-r--r--   0        0        0       22 2021-04-09 16:17:59.560310 chinormfilter-0.5.1/chinormfilter/__init__.py
--rw-r--r--   0        0        0     1722 2021-04-09 15:05:31.759916 chinormfilter-0.5.1/chinormfilter/cli.py
--rw-r--r--   0        0        0      584 2021-06-18 06:03:13.818353 chinormfilter-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1741 2021-06-18 06:06:53.046640 chinormfilter-0.5.1/setup.py
--rw-r--r--   0        0        0     1619 2021-06-18 06:06:53.047531 chinormfilter-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 12:42:20.418731 chinormfilter-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1087 2023-07-07 12:42:20.418908 chinormfilter-0.5.3/README.md
+-rw-r--r--   0        0        0       22 2023-07-07 12:50:23.831975 chinormfilter-0.5.3/chinormfilter/__init__.py
+-rw-r--r--   0        0        0     1743 2023-07-07 12:50:01.209525 chinormfilter-0.5.3/chinormfilter/cli.py
+-rw-r--r--   0        0        0      643 2023-07-07 12:50:21.195525 chinormfilter-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 chinormfilter-0.5.3/PKG-INFO
```

### Comparing `chinormfilter-0.5.1/LICENSE` & `chinormfilter-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chinormfilter-0.5.1/README.md` & `chinormfilter-0.5.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # chinormfilter
 
 [![PyPi version](https://img.shields.io/pypi/v/chinormfilter.svg)](https://pypi.python.org/pypi/chinormfilter/)
 ![PyTest](https://github.com/po3rin/chinormfilter/workflows/PyTest/badge.svg)
 [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-390/)
 ![](https://img.shields.io/pypi/l/chinormfilter)
 
-Filter synonym files written in lucene format to avoid duplication with Sudachi normalization. Mainly used when migrating to sudachi analyzer.
+Filter synonym written in lucene format to avoid duplication with Sudachi normalization. Mainly used when migrating to sudachi analyzer.
 
 ## Usage
 
 ```sh
 $ chinormfilter tests/test.txt -o out.txt
 ```
 
@@ -24,9 +24,23 @@
 
 ↓ filter
 
 レナリドミド,レナリドマイド
 tlc => tlc,全肺気量
 ```
 
+### Specify system dict
+
+```sh
+$ chinormfilter tests/test.txt -s full -o out.txt
+```
+
+### Use Custom Dict
+
+Specify dict via sudachi.json
+
+```sh
+$ chinormfilter tests/test.txt -s sudachi.json -o out.txt
+```
+
 ## TODO
 - [ ] custom dict test
```

### Comparing `chinormfilter-0.5.1/chinormfilter/cli.py` & `chinormfilter-0.5.3/chinormfilter/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,38 +9,37 @@
 
 parser = argparse.ArgumentParser(
     description="Filter synonym files written in lucene format to avoid duplication with Sudachi normalization"
 )
 
 parser.add_argument("file", help="lucene synonym file path")
 parser.add_argument("-o", "--out", help="output path")
-parser.add_argument(
-    "-r", "--sudachi_setting", help="the setting file in JSON format"
-)
-parser.add_argument(
-    "-s", "--sudachi_dict_type", help="sudachidict type"
-)
+parser.add_argument("-r", "--sudachi_setting", help="the setting file in JSON format")
+parser.add_argument("-s", "--sudachi_dict_type", help="sudachidict type")
 
 
 class Filter:
     def __init__(self, sudachi_setting=None, dict_type="core"):
         self.tokenizer = dictionary.Dictionary(
-            dict_type=dict_type, config_path=sudachi_setting).create()
+            dict_type=dict_type, config_path=sudachi_setting
+        ).create()
 
     def duplicated(self, line: str) -> bool:
-        words = [l.strip() for l in re.split(',|=>', line)]
+        words = [l.strip() for l in re.split(",|=>", line)]
 
         normalized = []
         for w in words:
             n = ""
             for t in self.tokenizer.tokenize(w, mode):
                 n += t.normalized_form()
             normalized.append(n)
 
-        return all([t == normalized[0] for t in normalized[1:]]) if normalized else False
+        return (
+            all([t == normalized[0] for t in normalized[1:]]) if normalized else False
+        )
 
 
 def cli() -> str:
     args = parser.parse_args()
     out = open(args.out, "wt")
     sudachi_setting = args.sudachi_setting
     sudachi_dict_type = args.sudachi_dict_type
```

### Comparing `chinormfilter-0.5.1/PKG-INFO` & `chinormfilter-0.5.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: chinormfilter
-Version: 0.5.1
+Version: 0.5.3
 Summary: 
 Home-page: http://github.com/po3rin/chinormfilter
 License: Apache-2.0
 Author: po3rin
 Author-email: abctail30@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: sudachidict_core (>=20210608,<20210609)
-Requires-Dist: sudachidict_full (>=20210608,<20210609)
-Requires-Dist: sudachipy (>=0.5.2,<0.6.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: sudachidict-core (>=20230110,<20230111)
+Requires-Dist: sudachidict-full (>=20230110,<20230111)
+Requires-Dist: sudachipy (>=0.6.7,<0.7.0)
 Project-URL: Repository, http://github.com/po3rin/chinormfilter
 Description-Content-Type: text/markdown
 
 # chinormfilter
 
 [![PyPi version](https://img.shields.io/pypi/v/chinormfilter.svg)](https://pypi.python.org/pypi/chinormfilter/)
 ![PyTest](https://github.com/po3rin/chinormfilter/workflows/PyTest/badge.svg)
 [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-390/)
 ![](https://img.shields.io/pypi/l/chinormfilter)
 
-Filter synonym files written in lucene format to avoid duplication with Sudachi normalization. Mainly used when migrating to sudachi analyzer.
+Filter synonym written in lucene format to avoid duplication with Sudachi normalization. Mainly used when migrating to sudachi analyzer.
 
 ## Usage
 
 ```sh
 $ chinormfilter tests/test.txt -o out.txt
 ```
 
@@ -44,10 +42,24 @@
 
 ↓ filter
 
 レナリドミド,レナリドマイド
 tlc => tlc,全肺気量
 ```
 
+### Specify system dict
+
+```sh
+$ chinormfilter tests/test.txt -s full -o out.txt
+```
+
+### Use Custom Dict
+
+Specify dict via sudachi.json
+
+```sh
+$ chinormfilter tests/test.txt -s sudachi.json -o out.txt
+```
+
 ## TODO
 - [ ] custom dict test
```

