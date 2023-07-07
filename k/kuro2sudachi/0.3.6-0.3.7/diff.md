# Comparing `tmp/kuro2sudachi-0.3.6.tar.gz` & `tmp/kuro2sudachi-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuro2sudachi-0.3.6.tar", max compression
+gzip compressed data, was "kuro2sudachi-0.3.7.tar", max compression
```

## Comparing `kuro2sudachi-0.3.6.tar` & `kuro2sudachi-0.3.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     3535 2021-06-06 09:08:54.137396 kuro2sudachi-0.3.6/README.md
--rw-r--r--   0        0        0      634 2021-06-29 04:22:57.280810 kuro2sudachi-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2021-01-18 09:48:45.840749 kuro2sudachi-0.3.6/src/kuro2sudachi/__init__.py
--rw-r--r--   0        0        0     6476 2021-06-29 04:21:49.810805 kuro2sudachi-0.3.6/src/kuro2sudachi/core.py
--rw-r--r--   0        0        0     2736 2021-01-18 13:58:40.771596 kuro2sudachi-0.3.6/src/kuro2sudachi/normalizer.py
--rw-r--r--   0        0        0     5426 2021-04-17 05:56:39.867538 kuro2sudachi-0.3.6/src/kuro2sudachi/rewrite.def
--rw-r--r--   0        0        0     4574 2021-06-29 04:23:30.424184 kuro2sudachi-0.3.6/setup.py
--rw-r--r--   0        0        0     4321 2021-06-29 04:23:30.424574 kuro2sudachi-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     2904 2023-06-26 15:47:20.263852 kuro2sudachi-0.3.7/README.md
+-rw-r--r--   0        0        0      659 2023-07-07 12:03:17.498785 kuro2sudachi-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.3.7/src/kuro2sudachi/__init__.py
+-rw-r--r--   0        0        0     6492 2023-07-07 11:56:16.740436 kuro2sudachi-0.3.7/src/kuro2sudachi/core.py
+-rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.3.7/src/kuro2sudachi/normalizer.py
+-rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.3.7/src/kuro2sudachi/rewrite.def
+-rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 kuro2sudachi-0.3.7/PKG-INFO
```

### Comparing `kuro2sudachi-0.3.6/README.md` & `kuro2sudachi-0.3.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 $ cat kuromoji_dict.txt
 融合たんぱく質,融合たんぱく質,融合たんぱく質,名詞
 発作性心房細動,発作性心房細動,発作性心房細動,名詞
 
 $ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c convert_config.json --ignore
 
 $ cat sudachi_user_dict.txt
-融合たんぱく質,4786,4786,5000,融合たんぱく質,名詞,普通名詞,一般,*,*,*,,融合たんぱく質,*,C,"融合,名詞,普通名詞,サ変可能,*,*,*,ユウゴウ/たんぱく,名詞,普通名詞,一般,*,*,*,タンパク/質,接尾辞,名詞的,一般,*,*,*,シツ","融合,名詞,普通名詞,サ変可能,*,*,*,ユウゴウ/たんぱく質,名詞,普通名詞,一般,*,*,*,タンパクシツ",*
-発作性心房細動,4786,4786,5000,発作性心房細動,名詞,普通名詞,一般,*,*,*,,発作性心房細動,*,C,"発作,名詞,普通名詞,一般,*,*,*,ホッサ/性,接尾辞,名詞的,一般,*,*,*,セイ/心房,名詞,普通名詞,一般,*,*,*,シンボウ/細動,名詞,普通名詞,一般,*,*,*,サイドウ","発作,名詞,普通名詞,一般,*,*,*,ホッサ/性,接尾辞,名詞的,一般,*,*,*,セイ/心房,名詞,普通名詞,一般,*,*,*,シンボウ/細動,名詞,普通名詞,一般,*,*,*,サイドウ",*
+融合たんぱく質,4786,4786,5000,融合たんぱく質,名詞,普通名詞,一般,*,*,*,,融合たんぱく質,*,C,*,660881/810248,*
+発作性心房細動,4786,4786,5000,発作性心房細動,名詞,普通名詞,一般,*,*,*,,発作性心房細動,*,C,584006/434835/428494/619020,2756385/428494/619020,*
 ```
 
 ## Splitting Words defined by kuromoji
 
 Currently, the CLI does not support word splitting defined by kuromoji. Therefore, the split representation of kuromoji is ignored.
 
 ```
```

### Comparing `kuro2sudachi-0.3.6/pyproject.toml` & `kuro2sudachi-0.3.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "kuro2sudachi"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["po3rin"]
 repository = "http://github.com/po3rin/kuro2sudachi"
 homepage = "http://github.com/po3rin/kuro2sudachi"
 readme = "README.md"
 license = "Apache-2.0"
 include = ["rewrite.def"]
 
 [tool.poetry.scripts]
 kuro2sudachi = "kuro2sudachi.core:cli"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.11"
 jaconv = "^0.2.4"
-importlib-metadata = "^3.7.3"
+importlib-metadata = "^6.7.0"
 sudachipy = "^0.5.2"
-sudachidict_full = "^20210608"
-SudachiDict-core = "^20210608"
+sudachidict-core = "^20230110"
+sudachidict-full = "^20230110"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
 pytest = "^6.2.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `kuro2sudachi-0.3.6/src/kuro2sudachi/core.py` & `kuro2sudachi-0.3.7/src/kuro2sudachi/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,23 @@
     "--rewrite_def",
     default=os.path.dirname(os.path.abspath(__file__)) + "/rewrite.def",
     help="rewrite text file path",
 )
 parser.add_argument(
     "--rm_already_exist",
     action="store_true",
-    help="remove words system dict already exist"
+    help="remove words system dict already exist",
 )
 parser.add_argument("-r", "--sudachi_setting", help="the setting file in JSON format")
 parser.add_argument("-s", "--sudachi_dict_type", help="sudachidict type")
-parser.add_argument("-m", "--merge_dict", help="A dictionary for split registration of words that are not in the system dictionary. Must be specified as a user dictionary in sudachi's configuration file (json).")
+parser.add_argument(
+    "-m",
+    "--merge_dict",
+    help="A dictionary for split registration of words that are not in the system dictionary. Must be specified as a user dictionary in sudachi's configuration file (json).",
+)
 parser.add_argument(
     "--ignore",
     action="store_true",
     help="ignore invalid format line / unsupported pos error / oov error in splitted word",
 )
 
 default_setting = {
@@ -148,26 +152,25 @@
     def split_info(self, normalized: str, udm: list[str], mode: any) -> str:
         word_ids = []
         oov = []
         for m in self.tokenizer.tokenize(normalized, mode):
             if ",".join(m.part_of_speech()) == "名詞,数詞,*,*,*,*":
                 return "*"
 
-            if m.is_oov() or m.dictionary_id()==-1:
+            if m.is_oov() or m.dictionary_id() == -1:
                 oov.append(m.surface())
                 continue
 
             word_ids.append(str(m.word_id()))
 
         if len(oov) > 0:
             raise OOVError(f"split word has out of vocab: {oov} in {normalized}")
 
         return "/".join(word_ids)
 
-
     def split(self, normalized: str, udm: list[str]) -> str:
         try:
             unit_div_info = []
             if "A" in udm:
                 info = self.split_info(normalized, udm, tokenizer.Tokenizer.SplitMode.A)
                 unit_div_info.append(info)
             else:
@@ -200,15 +203,15 @@
         sudachi_setting=sudachi_setting,
         dict_type=sudachi_dict_type,
         rm=rm,
     )
 
     with fileinput.input(files=merge_dict) as merged:
         for line in merged:
-            line = line.replace("\n" , "")
+            line = line.replace("\n", "")
             out.write(f"{line}\n")
 
     with fileinput.input(files=args.file) as input:
         for line in input:
             line = line.strip()
             if line == "":
                 continue
```

### Comparing `kuro2sudachi-0.3.6/src/kuro2sudachi/normalizer.py` & `kuro2sudachi-0.3.7/src/kuro2sudachi/normalizer.py`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.3.6/src/kuro2sudachi/rewrite.def` & `kuro2sudachi-0.3.7/src/kuro2sudachi/rewrite.def`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.3.6/PKG-INFO` & `kuro2sudachi-0.3.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: kuro2sudachi
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Home-page: http://github.com/po3rin/kuro2sudachi
 License: Apache-2.0
 Author: po3rin
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: SudachiDict-core (>=20210608,<20210609)
-Requires-Dist: importlib-metadata (>=3.7.3,<4.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib-metadata (>=6.7.0,<7.0.0)
 Requires-Dist: jaconv (>=0.2.4,<0.3.0)
-Requires-Dist: sudachidict_full (>=20210608,<20210609)
+Requires-Dist: sudachidict-core (>=20230110,<20230111)
+Requires-Dist: sudachidict-full (>=20230110,<20230111)
 Requires-Dist: sudachipy (>=0.5.2,<0.6.0)
 Project-URL: Repository, http://github.com/po3rin/kuro2sudachi
 Description-Content-Type: text/markdown
 
 # kuro2sudachi
 
 [![PyPi version](https://img.shields.io/pypi/v/kuro2sudachi.svg)](https://pypi.python.org/pypi/kuro2sudachi/)
@@ -96,16 +94,16 @@
 $ cat kuromoji_dict.txt
 融合たんぱく質,融合たんぱく質,融合たんぱく質,名詞
 発作性心房細動,発作性心房細動,発作性心房細動,名詞
 
 $ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c convert_config.json --ignore
 
 $ cat sudachi_user_dict.txt
-融合たんぱく質,4786,4786,5000,融合たんぱく質,名詞,普通名詞,一般,*,*,*,,融合たんぱく質,*,C,"融合,名詞,普通名詞,サ変可能,*,*,*,ユウゴウ/たんぱく,名詞,普通名詞,一般,*,*,*,タンパク/質,接尾辞,名詞的,一般,*,*,*,シツ","融合,名詞,普通名詞,サ変可能,*,*,*,ユウゴウ/たんぱく質,名詞,普通名詞,一般,*,*,*,タンパクシツ",*
-発作性心房細動,4786,4786,5000,発作性心房細動,名詞,普通名詞,一般,*,*,*,,発作性心房細動,*,C,"発作,名詞,普通名詞,一般,*,*,*,ホッサ/性,接尾辞,名詞的,一般,*,*,*,セイ/心房,名詞,普通名詞,一般,*,*,*,シンボウ/細動,名詞,普通名詞,一般,*,*,*,サイドウ","発作,名詞,普通名詞,一般,*,*,*,ホッサ/性,接尾辞,名詞的,一般,*,*,*,セイ/心房,名詞,普通名詞,一般,*,*,*,シンボウ/細動,名詞,普通名詞,一般,*,*,*,サイドウ",*
+融合たんぱく質,4786,4786,5000,融合たんぱく質,名詞,普通名詞,一般,*,*,*,,融合たんぱく質,*,C,*,660881/810248,*
+発作性心房細動,4786,4786,5000,発作性心房細動,名詞,普通名詞,一般,*,*,*,,発作性心房細動,*,C,584006/434835/428494/619020,2756385/428494/619020,*
 ```
 
 ## Splitting Words defined by kuromoji
 
 Currently, the CLI does not support word splitting defined by kuromoji. Therefore, the split representation of kuromoji is ignored.
 
 ```
```

