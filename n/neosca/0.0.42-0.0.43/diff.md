# Comparing `tmp/neosca-0.0.42.tar.gz` & `tmp/neosca-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosca-0.0.42.tar", last modified: Sat Apr 29 14:19:10 2023, max compression
+gzip compressed data, was "neosca-0.0.43.tar", last modified: Fri Jul  7 08:35:04 2023, max compression
```

## Comparing `neosca-0.0.42.tar` & `neosca-0.0.43.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-04-29 14:19:10.551722 neosca-0.0.42/
--rw-r--r--   0 tan       (1000) tan       (1000)    18092 2023-04-05 18:36:09.000000 neosca-0.0.42/LICENSE.txt
--rw-r--r--   0 tan       (1000) tan       (1000)      106 2023-04-05 18:36:09.000000 neosca-0.0.42/MANIFEST.in
--rw-r--r--   0 tan       (1000) tan       (1000)    15625 2023-04-29 14:19:10.551722 neosca-0.0.42/PKG-INFO
--rw-r--r--   0 tan       (1000) tan       (1000)    14776 2023-04-29 14:17:28.000000 neosca-0.0.42/README.md
-drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-04-29 14:19:10.551722 neosca-0.0.42/neosca/
--rw-r--r--   0 tan       (1000) tan       (1000)       93 2023-04-29 14:17:28.000000 neosca-0.0.42/neosca/__init__.py
--rw-r--r--   0 tan       (1000) tan       (1000)       62 2023-04-05 18:36:09.000000 neosca-0.0.42/neosca/__main__.py
--rw-r--r--   0 tan       (1000) tan       (1000)    17121 2023-04-28 21:18:36.000000 neosca-0.0.42/neosca/depends_installer.py
--rw-r--r--   0 tan       (1000) tan       (1000)     3539 2023-04-29 14:17:25.000000 neosca-0.0.42/neosca/io.py
--rw-r--r--   0 tan       (1000) tan       (1000)    24224 2023-04-29 14:17:25.000000 neosca-0.0.42/neosca/main.py
--rw-r--r--   0 tan       (1000) tan       (1000)     7287 2023-04-29 14:17:25.000000 neosca-0.0.42/neosca/neosca.py
--rw-r--r--   0 tan       (1000) tan       (1000)     6005 2023-04-28 21:18:36.000000 neosca-0.0.42/neosca/parser.py
--rw-r--r--   0 tan       (1000) tan       (1000)     4854 2023-04-28 21:18:36.000000 neosca-0.0.42/neosca/querier.py
--rw-r--r--   0 tan       (1000) tan       (1000)     9877 2023-04-28 21:18:36.000000 neosca-0.0.42/neosca/structure_counter.py
--rw-r--r--   0 tan       (1000) tan       (1000)      316 2023-04-28 21:18:36.000000 neosca-0.0.42/neosca/util.py
--rw-r--r--   0 tan       (1000) tan       (1000)     5319 2023-04-28 21:18:36.000000 neosca-0.0.42/neosca/util_env.py
--rw-r--r--   0 tan       (1000) tan       (1000)      414 2023-04-18 15:44:34.000000 neosca-0.0.42/neosca/util_platform_info.py
--rw-r--r--   0 tan       (1000) tan       (1000)     1650 2023-04-18 15:44:34.000000 neosca-0.0.42/neosca/util_print.py
-drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-04-29 14:19:10.551722 neosca-0.0.42/neosca.egg-info/
--rw-r--r--   0 tan       (1000) tan       (1000)    15625 2023-04-29 14:19:10.000000 neosca-0.0.42/neosca.egg-info/PKG-INFO
--rw-r--r--   0 tan       (1000) tan       (1000)      621 2023-04-29 14:19:10.000000 neosca-0.0.42/neosca.egg-info/SOURCES.txt
--rw-r--r--   0 tan       (1000) tan       (1000)        1 2023-04-29 14:19:10.000000 neosca-0.0.42/neosca.egg-info/dependency_links.txt
--rw-r--r--   0 tan       (1000) tan       (1000)       37 2023-04-29 14:19:10.000000 neosca-0.0.42/neosca.egg-info/entry_points.txt
--rw-r--r--   0 tan       (1000) tan       (1000)       26 2023-04-29 14:19:10.000000 neosca-0.0.42/neosca.egg-info/requires.txt
--rw-r--r--   0 tan       (1000) tan       (1000)        7 2023-04-29 14:19:10.000000 neosca-0.0.42/neosca.egg-info/top_level.txt
--rw-r--r--   0 tan       (1000) tan       (1000)       38 2023-04-29 14:19:10.551722 neosca-0.0.42/setup.cfg
--rw-r--r--   0 tan       (1000) tan       (1000)     1491 2023-04-29 14:17:28.000000 neosca-0.0.42/setup.py
-drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-04-29 14:19:10.551722 neosca-0.0.42/tests/
--rw-r--r--   0 tan       (1000) tan       (1000)     4977 2023-04-18 15:44:34.000000 neosca-0.0.42/tests/test_cmdline.py
--rw-r--r--   0 tan       (1000) tan       (1000)      568 2023-04-18 15:44:34.000000 neosca-0.0.42/tests/test_main.py
--rw-r--r--   0 tan       (1000) tan       (1000)     4523 2023-04-28 21:18:36.000000 neosca-0.0.42/tests/test_parser.py
--rw-r--r--   0 tan       (1000) tan       (1000)      931 2023-04-28 21:18:36.000000 neosca-0.0.42/tests/test_querier.py
--rw-r--r--   0 tan       (1000) tan       (1000)     5470 2023-04-18 15:44:34.000000 neosca-0.0.42/tests/test_structure_counter.py
--rw-r--r--   0 tan       (1000) tan       (1000)      467 2023-04-18 15:44:34.000000 neosca-0.0.42/tests/test_util_env.py
+drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-07-07 08:35:04.058194 neosca-0.0.43/
+-rw-r--r--   0 tan       (1000) tan       (1000)    18092 2023-06-17 06:06:55.000000 neosca-0.0.43/LICENSE.txt
+-rw-r--r--   0 tan       (1000) tan       (1000)      106 2023-07-03 12:01:28.000000 neosca-0.0.43/MANIFEST.in
+-rw-r--r--   0 tan       (1000) tan       (1000)    16024 2023-07-07 08:35:04.058194 neosca-0.0.43/PKG-INFO
+-rw-r--r--   0 tan       (1000) tan       (1000)    15175 2023-07-07 08:29:52.000000 neosca-0.0.43/README.md
+drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-07-07 08:35:04.058194 neosca-0.0.43/neosca/
+-rw-r--r--   0 tan       (1000) tan       (1000)       50 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/__init__.py
+-rw-r--r--   0 tan       (1000) tan       (1000)       62 2023-06-17 06:06:55.000000 neosca-0.0.43/neosca/__main__.py
+-rw-r--r--   0 tan       (1000) tan       (1000)       70 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/about.py
+-rw-r--r--   0 tan       (1000) tan       (1000)    17386 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/depends_installer.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     4768 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/io.py
+-rw-r--r--   0 tan       (1000) tan       (1000)    25513 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/main.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     7702 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/neosca.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     6010 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/parser.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     4969 2023-07-07 07:37:48.000000 neosca-0.0.43/neosca/querier.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     6777 2023-07-07 07:37:48.000000 neosca-0.0.43/neosca/structure_counter.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     4050 2023-07-07 07:37:48.000000 neosca-0.0.43/neosca/structure_data.py
+-rw-r--r--   0 tan       (1000) tan       (1000)      316 2023-06-17 06:06:55.000000 neosca-0.0.43/neosca/util.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     5343 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/util_env.py
+-rw-r--r--   0 tan       (1000) tan       (1000)      623 2023-07-07 08:24:33.000000 neosca-0.0.43/neosca/util_platform_info.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     1650 2023-06-17 06:06:55.000000 neosca-0.0.43/neosca/util_print.py
+drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-07-07 08:35:04.058194 neosca-0.0.43/neosca.egg-info/
+-rw-r--r--   0 tan       (1000) tan       (1000)    16024 2023-07-07 08:35:04.000000 neosca-0.0.43/neosca.egg-info/PKG-INFO
+-rw-r--r--   0 tan       (1000) tan       (1000)      662 2023-07-07 08:35:04.000000 neosca-0.0.43/neosca.egg-info/SOURCES.txt
+-rw-r--r--   0 tan       (1000) tan       (1000)        1 2023-07-07 08:35:04.000000 neosca-0.0.43/neosca.egg-info/dependency_links.txt
+-rw-r--r--   0 tan       (1000) tan       (1000)       37 2023-07-07 08:35:04.000000 neosca-0.0.43/neosca.egg-info/entry_points.txt
+-rw-r--r--   0 tan       (1000) tan       (1000)       26 2023-07-07 08:35:04.000000 neosca-0.0.43/neosca.egg-info/requires.txt
+-rw-r--r--   0 tan       (1000) tan       (1000)        7 2023-07-07 08:35:04.000000 neosca-0.0.43/neosca.egg-info/top_level.txt
+-rw-r--r--   0 tan       (1000) tan       (1000)       38 2023-07-07 08:35:04.058194 neosca-0.0.43/setup.cfg
+-rw-r--r--   0 tan       (1000) tan       (1000)     1287 2023-07-07 08:24:33.000000 neosca-0.0.43/setup.py
+drwxr-xr-x   0 tan       (1000) tan       (1000)        0 2023-07-07 08:35:04.058194 neosca-0.0.43/tests/
+-rw-r--r--   0 tan       (1000) tan       (1000)     4977 2023-07-07 07:37:48.000000 neosca-0.0.43/tests/test_cmdline.py
+-rw-r--r--   0 tan       (1000) tan       (1000)      568 2023-06-17 06:06:55.000000 neosca-0.0.43/tests/test_main.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     4523 2023-06-17 06:06:55.000000 neosca-0.0.43/tests/test_parser.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     1013 2023-07-07 07:37:48.000000 neosca-0.0.43/tests/test_querier.py
+-rw-r--r--   0 tan       (1000) tan       (1000)     4633 2023-07-07 07:37:48.000000 neosca-0.0.43/tests/test_structure_counter.py
+-rw-r--r--   0 tan       (1000) tan       (1000)      467 2023-06-17 06:06:55.000000 neosca-0.0.43/tests/test_util_env.py
```

### Comparing `neosca-0.0.42/LICENSE.txt` & `neosca-0.0.43/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neosca-0.0.42/PKG-INFO` & `neosca-0.0.43/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neosca
-Version: 0.0.42
+Version: 0.0.43
 Summary: Another syntactic complexity analyzer of written English language samples
 Home-page: https://github.com/tanloong/neosca
-Author: TAN Long
+Author: Long Tan
 Author-email: tanloong@foxmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
@@ -100,15 +100,15 @@
 
 <!-- vim-markdown-toc -->
 
 ## Highlights
 
 * Cross-platform compatibility: Windows, macOS, and Linux
 * Flexible command-line options to serve various needs
-* Supports reading docx files
+* Supports reading txt/docx/odt files
 
 ## Install
 
 ### Install NeoSCA
 
 To install NeoSCA, you need to have [Python](https://www.python.org/) 3.7 or later installed on your system. You can check if you already have Python installed by running the following command in your terminal:
 
@@ -156,15 +156,15 @@
 To analyze a single file, use the command `nsca` followed by the file path.
 
 ```sh
 nsca ./samples/sample1.txt
 nsca ./samples/sample1.docx
 ```
 
-When working on docx files, tables, figures, images, and other unrelated elements (except for headers and footers, which will be automatically ignored) should be manually removed before they are analyzed.
+Tables, figures, images, and other unrelated elements (except for headers and footers, which will be automatically ignored) should be manually removed before docx/odt files are analyzed.
 
 After running the above command, a `result.csv` file will be generated in the current directory. You can specify a different output filename using `-o/--output-file`.
 
 ```sh
 nsca ./samples/sample1.txt -o sample1.csv
 # frequency output: ./sample1.csv
 ```
@@ -237,15 +237,15 @@
 It is for text with hard line breaks and a blank line between paragraphs.
 
 #### Select a Subset of Measures
 
 NeoSCA by default outputs values of all of the available measures. You can use `--select` to only analyze measures that you are interested in. To see a full list of available measures, use `nsca --list`.
 
 ```sh
-nsca --select VP T DC_C -- sample1.txt
+nsca --select VP T DC/C -- sample1.txt
 ```
 
 To avoid the program taking input filenames as a selected measure and raising an error, use `--` to separate them from the measures. All arguments after `--` will be considered input filenames. Make sure to specify arguments except for input filenames at the left side of `--`.
 
 #### Combine Subfiles
 
 Use `-c`/`--combine-subfiles` to add up frequencies of the 9 syntactic structures of subfiles and compute values of the 14 syntactic complexity indices for the imaginary parent file. You can use this option multiple times to combine different lists of subfiles respectively. The `--` should be used to separate input filenames from input subfile-names.
@@ -319,14 +319,22 @@
 ```sh
 nsca samples/sample1.txt --no-query
 # parsed trees: samples/sample1.parsed
 nsca --text 'This is a test.' --no-query
 # parsed trees: ./cmdline_text.parsed
 ```
 
+#### Parse trees as input
+
+By default, the program expects raw text as input that will be parsed before querying. If you already have parsed input files, use `--no-parse` to indicate that the program should skip the parsing step and proceed directly to querying. When this flag is set, the is_skip_querying and reserve_parsed are automatically set as False.
+
+```sh
+nsca samples/sample1.parsed --no-parse
+```
+
 #### List Output Fields
 
 Use `--list` to print a list of all the available output fields.
 
 <details>
 
 <summary>
@@ -369,40 +377,40 @@
 
 <summary>
 BibTeX
 </summary>
 
 ```BibTeX
 @misc{tan2022neosca,
-title        = {NeoSCA: A Rewrite of L2 Syntactic Complexity Analyzer, version 0.0.42},
+title        = {NeoSCA: A Rewrite of L2 Syntactic Complexity Analyzer, version 0.0.43},
 author       = {Long Tan},
 howpublished = {\url{https://github.com/tanloong/neosca}},
 year         = {2022}
 }
 ```
 
 </details>
 
 <details>
 
 <summary>
 APA (7th edition)
 </summary>
 
-<pre>Tan, L. (2022). <i>NeoSCA</i> (version 0.0.42) [Computer software]. Github. https://github.com/tanloong/neosca</pre>
+<pre>Tan, L. (2022). <i>NeoSCA</i> (version 0.0.43) [Computer software]. Github. https://github.com/tanloong/neosca</pre>
 
 </details>
 
 <details>
 
 <summary>
 MLA (9th edition)
 </summary>
 
-<pre>Tan, Long. <i>NeoSCA</i>. version 0.0.42, GitHub, 2022, https://github.com/tanloong/neosca.</pre>
+<pre>Tan, Long. <i>NeoSCA</i>. version 0.0.43, GitHub, 2022, https://github.com/tanloong/neosca.</pre>
 
 </details>
 
 Also, you need to cite Xiaofei's article describing L2SCA.
 
 <details>
```

### Comparing `neosca-0.0.42/README.md` & `neosca-0.0.43/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 <!-- vim-markdown-toc -->
 
 ## Highlights
 
 * Cross-platform compatibility: Windows, macOS, and Linux
 * Flexible command-line options to serve various needs
-* Supports reading docx files
+* Supports reading txt/docx/odt files
 
 ## Install
 
 ### Install NeoSCA
 
 To install NeoSCA, you need to have [Python](https://www.python.org/) 3.7 or later installed on your system. You can check if you already have Python installed by running the following command in your terminal:
 
@@ -135,15 +135,15 @@
 To analyze a single file, use the command `nsca` followed by the file path.
 
 ```sh
 nsca ./samples/sample1.txt
 nsca ./samples/sample1.docx
 ```
 
-When working on docx files, tables, figures, images, and other unrelated elements (except for headers and footers, which will be automatically ignored) should be manually removed before they are analyzed.
+Tables, figures, images, and other unrelated elements (except for headers and footers, which will be automatically ignored) should be manually removed before docx/odt files are analyzed.
 
 After running the above command, a `result.csv` file will be generated in the current directory. You can specify a different output filename using `-o/--output-file`.
 
 ```sh
 nsca ./samples/sample1.txt -o sample1.csv
 # frequency output: ./sample1.csv
 ```
@@ -216,15 +216,15 @@
 It is for text with hard line breaks and a blank line between paragraphs.
 
 #### Select a Subset of Measures
 
 NeoSCA by default outputs values of all of the available measures. You can use `--select` to only analyze measures that you are interested in. To see a full list of available measures, use `nsca --list`.
 
 ```sh
-nsca --select VP T DC_C -- sample1.txt
+nsca --select VP T DC/C -- sample1.txt
 ```
 
 To avoid the program taking input filenames as a selected measure and raising an error, use `--` to separate them from the measures. All arguments after `--` will be considered input filenames. Make sure to specify arguments except for input filenames at the left side of `--`.
 
 #### Combine Subfiles
 
 Use `-c`/`--combine-subfiles` to add up frequencies of the 9 syntactic structures of subfiles and compute values of the 14 syntactic complexity indices for the imaginary parent file. You can use this option multiple times to combine different lists of subfiles respectively. The `--` should be used to separate input filenames from input subfile-names.
@@ -298,14 +298,22 @@
 ```sh
 nsca samples/sample1.txt --no-query
 # parsed trees: samples/sample1.parsed
 nsca --text 'This is a test.' --no-query
 # parsed trees: ./cmdline_text.parsed
 ```
 
+#### Parse trees as input
+
+By default, the program expects raw text as input that will be parsed before querying. If you already have parsed input files, use `--no-parse` to indicate that the program should skip the parsing step and proceed directly to querying. When this flag is set, the is_skip_querying and reserve_parsed are automatically set as False.
+
+```sh
+nsca samples/sample1.parsed --no-parse
+```
+
 #### List Output Fields
 
 Use `--list` to print a list of all the available output fields.
 
 <details>
 
 <summary>
@@ -348,40 +356,40 @@
 
 <summary>
 BibTeX
 </summary>
 
 ```BibTeX
 @misc{tan2022neosca,
-title        = {NeoSCA: A Rewrite of L2 Syntactic Complexity Analyzer, version 0.0.42},
+title        = {NeoSCA: A Rewrite of L2 Syntactic Complexity Analyzer, version 0.0.43},
 author       = {Long Tan},
 howpublished = {\url{https://github.com/tanloong/neosca}},
 year         = {2022}
 }
 ```
 
 </details>
 
 <details>
 
 <summary>
 APA (7th edition)
 </summary>
 
-<pre>Tan, L. (2022). <i>NeoSCA</i> (version 0.0.42) [Computer software]. Github. https://github.com/tanloong/neosca</pre>
+<pre>Tan, L. (2022). <i>NeoSCA</i> (version 0.0.43) [Computer software]. Github. https://github.com/tanloong/neosca</pre>
 
 </details>
 
 <details>
 
 <summary>
 MLA (9th edition)
 </summary>
 
-<pre>Tan, Long. <i>NeoSCA</i>. version 0.0.42, GitHub, 2022, https://github.com/tanloong/neosca.</pre>
+<pre>Tan, Long. <i>NeoSCA</i>. version 0.0.43, GitHub, 2022, https://github.com/tanloong/neosca.</pre>
 
 </details>
 
 Also, you need to cite Xiaofei's article describing L2SCA.
 
 <details>
```

### Comparing `neosca-0.0.42/neosca/depends_installer.py` & `neosca-0.0.43/neosca/depends_installer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,24 @@
 
 from .util import SCAProcedureResult
 from .util_platform_info import IS_DARWIN, IS_WINDOWS
 from .util_platform_info import USER_SOFTWARE_DIR
 from .util_print import same_line_print
 from .util_print import get_yes_or_no
 
+if IS_DARWIN:
+    import ssl
+
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
 _UNPACK200 = "unpack200.exe" if IS_WINDOWS else "unpack200"
 _UNPACK200_ARGS = '-r -v -l ""' if IS_WINDOWS else ""
 
 OS = "windows" if IS_WINDOWS else "mac" if IS_DARWIN else platform
 ARCH = "x64" if maxsize > 2**32 else "x32"
 
 _TAR = ".tar"
@@ -82,15 +92,15 @@
             return sucess, err_msg
         else:
             version = err_msg  # type:ignore
         self.is_use_chinese_jdk_mirror = get_yes_or_no(
             "Do you want to download Java from a Chinese mirror site? If you are inside of"
             " China, you may want to use this for a faster network connection."
         )
-        if self.is_use_chinese_jdk_mirror in ("n", "N"):
+        if self.is_use_chinese_jdk_mirror in ("n", "N", "no", "No"):
             return True, self._URL_JAVA_TEMPLATE.format(version, operating_system, arch, impl)
         else:
             index_url = self._URL_JAVA_TEMPLATE_CHINA.format(version, arch, operating_system)
             req = urllib.request.Request(index_url, headers=self.headers)
             response = urllib.request.urlopen(req)
             content = response.read().decode("utf-8")
             match = re.search(r'"([^"]+\.(?:zip|tar\.gz|tar|7z))"', content)
@@ -300,15 +310,15 @@
         if is_assume_yes:
             is_install = "y"
         else:
             is_install = get_yes_or_no(
                 f"It seems that {name} has not been installed, because {reason_dict[name]}. Do"
                 " you want to let NeoSCA install it for you?"
             )
-        if is_install in ("n", "N"):
+        if is_install in ("n", "N", "no", "No"):
             manual_install_prompt_dict = {
                 JAVA: (
                     f"You will have to install {JAVA} manually.\n\n1. To install it, visit"
                     " https://www.java.com/en/download/manual.jsp. Note that when mixing 64 bit"
                     " Python with 32 bit Java or vice versa the program will crash, so make"
                     " sure that you install a Java with the same bitness of your Python.\n2."
                     " Set an environment variable JAVA_HOME to the path of the unzipped"
```

### Comparing `neosca-0.0.42/neosca/io.py` & `neosca-0.0.43/neosca/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,123 @@
 #!/usr/bin/env python3
 # -*- coding=utf-8 -*-
 
 try:
-    from xml.etree.cElementTree import XML
+    from xml.etree.cElementTree import XML, fromstring
 except ImportError:
-    from xml.etree.ElementTree import XML
+    from xml.etree.ElementTree import XML, fromstring
 import logging
 import os
 import sys
-from typing import Optional
+from typing import ByteString, Optional, Union
 import zipfile
 
 from charset_normalizer import detect
 
 from .util import SCAProcedureResult
 
-WORD_NAMESPACE = "{http://schemas.openxmlformats.org/wordprocessingml/2006/main}"
-PARA = WORD_NAMESPACE + "p"
-TEXT = WORD_NAMESPACE + "t"
-
 
 class SCAIO:
-    def __init__(self) -> None:
+    DOCX_NAMESPACE = "{http://schemas.openxmlformats.org/wordprocessingml/2006/main}"
+    DOCX_PARA = DOCX_NAMESPACE + "p"
+    DOCX_TEXT = DOCX_NAMESPACE + "t"
+
+    ODT_NAMESPACE = ".//{urn:oasis:names:tc:opendocument:xmlns:text:1.0}"
+    ODT_PARA = ODT_NAMESPACE + "p"
+
+    def __init__(self):
+        self.ext_read_map = {
+            ".txt": self.read_txt,
+            ".docx": self.read_docx,
+            ".odt": self.read_odt,
+        }
         self.previous_encoding = "utf-8"
 
-    def read_docx(self, path) -> str:
+    def read_docx(self, path: str) -> str:
         """
         Take the path of a docx file as argument, return the text in unicode.
-        This approach does not extract text from tables, headers, and footers.
+        This approach does not extract text from headers and footers.
 
         https://etienned.github.io/posts/extract-text-from-word-docx-simply/
         """
-        document = zipfile.ZipFile(path)
-        xml_content = document.read("word/document.xml")
-        document.close()
+        with zipfile.ZipFile(path) as zip_file:
+            xml_content = zip_file.read("word/document.xml")
         tree = XML(xml_content)
 
         paragraphs = []
-        for paragraph in tree.iter(PARA):
-            text = "".join(node.text for node in paragraph.iter(TEXT) if node.text)
+        for paragraph in tree.iter(self.DOCX_PARA):
+            text = "".join(node.text for node in paragraph.iter(self.DOCX_TEXT) if node.text)
             paragraphs.append(text)
         return "\n".join(paragraphs)
 
+    def read_odt(self, path: str) -> str:
+        with zipfile.ZipFile(path) as zip_file:
+            xml_content = zip_file.read("content.xml")
+        root = fromstring(xml_content)
+        paragraphs = root.findall(self.ODT_PARA)
+        return "\n".join("".join(node.itertext()) for node in paragraphs)
+
+    def _read_txt(
+        self, path: str, mode: str, encoding: Optional[str] = None
+    ) -> Union[str, ByteString]:
+        try:
+            with open(path, mode=mode, encoding=encoding) as f:
+                content = f.read()
+        # input file existence has already been checked before running (main.py: verified_ifile_list),
+        # here check it again in case users remove input files during runtime
+        except FileNotFoundError:
+            logging.critical(f"{path} does not exist.")
+            sys.exit(1)
+        else:
+            return content
+
     def read_txt(self, path: str, is_guess_encoding=True) -> str:
         if not is_guess_encoding:
-            with open(path, "r", encoding="utf-8") as f:
-                content = f.read()
+            content = self._read_txt(path, "r", "utf-8")
         else:
             try:
                 logging.info(
                     f"Attempting to read {path} with {self.previous_encoding} encoding..."
                 )
-                with open(path, "r", encoding=self.previous_encoding) as f:  # type:ignore
-                    content = f.read()
+                content = self._read_txt(path, "r", self.previous_encoding)  # type:ignore
             except ValueError:
                 logging.info(f"Attempt failed. Reading {path} in binary mode...")
-                with open(path, "rb") as f:
-                    bytes_ = f.read()
+                bytes_ = self._read_txt(path, "rb")
                 logging.info("Guessing the encoding of the byte string...")
-                encoding = detect(bytes_)["encoding"]
+                encoding = detect(bytes_)["encoding"]  # type:ignore
+
                 if encoding is not None:
                     logging.info(f"Decoding the byte string with {encoding} encoding...")
                     content = bytes_.decode(encoding=encoding)  # type:ignore
                     self.previous_encoding = encoding  # type:ignore
                 else:
-                    logging.critical(f"Cannot detect encoding for {path}.")
+                    logging.critical(f"{path} is of unsupported file type.")
                     sys.exit(1)
-        return content
+        return content  # type:ignore
 
     def read_file(self, path: str) -> str:
         _, ext = os.path.splitext(path)
-
-        if ext == ".txt":
-            return self.read_txt(path)
-        elif ext == ".docx":
-            return self.read_docx(path)
-        else:
-            raise ValueError("Unexpected file type. Only txt and docx files are supported.")
-
-
-def try_write(filename: str, content: Optional[str]) -> SCAProcedureResult:
-    if not os.path.exists(filename):
-        return True, None
-    try:
-        with open(filename, "w", encoding="utf-8") as f:
-            if content is not None:
-                f.write(content)
+        if ext not in self.ext_read_map:
+            ext = (  # assume files with other extensions as .txt files; throw an error from within read_txt() if not so
+                ".txt"
+            )
+        return self.ext_read_map[ext](path)  # type:ignore
+
+    @classmethod
+    def try_write(cls, filename: str, content: Optional[str]) -> SCAProcedureResult:
+        if not os.path.exists(filename):
             return True, None
-    except PermissionError:
-        return (
-            False,
-            (
-                f"PermissionError: can not write to {filename}, because it is already"
-                f" in use by another process.\n\n1. Ensure that {filename} is closed,"
-                " or \n2. Specify another output filename through the `-o` option,"
-                f" e.g. nsca input.txt -o {filename.replace('.csv', '-2.csv')}"
-            ),
-        )
+        try:
+            with open(filename, "w", encoding="utf-8") as f:
+                if content is not None:
+                    f.write(content)
+                return True, None
+        except PermissionError:
+            return (
+                False,
+                (
+                    f"PermissionError: can not write to {filename}, because it is already"
+                    f" in use by another process.\n\n1. Ensure that {filename} is closed,"
+                    " or \n2. Specify another output filename through the `-o` option,"
+                    f" e.g. nsca input.txt -o {filename.replace('.csv', '-2.csv')}"
+                ),
+            )
```

### Comparing `neosca-0.0.42/neosca/main.py` & `neosca-0.0.43/neosca/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import argparse
 import glob
 import logging
 import os
 import sys
-from typing import List, Optional
+from typing import Callable, List, Optional
 
-from . import __version__
-from .io import try_write
+from .about import __version__
+from .io import SCAIO
 from .util import SCAProcedureResult
 from .util_env import getenv
 from .util_env import setenv
 from .util_env import search_java_home
 from .util_print import color_print
 
 
 class SCAUI:
     def __init__(self) -> None:
-        self.supported_ifile_types = ["txt", "docx"]
+        self.supported_ifile_types = [".txt", ".docx", ".odt"]
         self.cwd = os.getcwd()
         self.args_parser: argparse.ArgumentParser = self.create_args_parser()
         self.options: argparse.Namespace = argparse.Namespace()
 
         self.JAVA_HOME = "JAVA_HOME"
         self.STANFORD_PARSER_HOME = "STANFORD_PARSER_HOME"
         self.STANFORD_TREGEX_HOME = "STANFORD_TREGEX_HOME"
@@ -81,26 +81,26 @@
                 ' "always" means to treat a newline as a sentence break, but there still may be'
                 ' more than one sentences per line. "two" means to take two or more consecutive'
                 " newlines as a sentence break, and is for text with hard line breaks and a"
                 ' blank line between paragraphs. The default is "never".'
             ),
         )
         args_parser.add_argument(
-            "-c",
             "--combine-files",
+            "-c",
             metavar="<subfile>",
             dest="subfile_lists",
             action="append",
             default=None,
             nargs="+",
             help="Combine frequency output of multiple files.",
         )
         args_parser.add_argument(
-            "-t",
             "--text",
+            "-t",
             metavar="<text>",
             default=None,
             help="Pass text through the command line.",
         )
         args_parser.add_argument(
             "--ftype",
             dest="ifile_types",
@@ -116,16 +116,16 @@
             "--pretokenized",
             dest="is_pretokenized",
             action="store_true",
             default=False,
             help="Assume that the text has already been tokenized.",
         )
         args_parser.add_argument(
-            "-o",
             "--output-file",
+            "-o",
             metavar="<filename>",
             dest="ofile_freq",
             default=None,
             help='Specify an output file. The default is "result.csv".',
         )
         args_parser.add_argument(
             "--output-format",
@@ -154,57 +154,71 @@
                 "DC",
                 "CT",
                 "CP",
                 "CN",
                 "MLS",
                 "MLT",
                 "MLC",
-                "C_S",
-                "VP_T",
-                "C_T",
-                "DC_C",
-                "DC_T",
-                "T_S",
-                "CT_T",
-                "CP_T",
-                "CP_C",
-                "CN_T",
-                "CN_C",
+                "C/S",
+                "VP/T",
+                "C/T",
+                "DC/C",
+                "DC/T",
+                "T/S",
+                "CT/T",
+                "CP/T",
+                "CP/C",
+                "CN/T",
+                "CN/C",
             ],
             default=None,
             nargs="+",
             help=(
                 "Select only some of the measures to analyze. The full list of measures include"
-                ' "W", "S", "VP", "C", "T", "DC", "CT", "CP", "CN", "MLS", "MLT", "MLC", "C_S",'
-                ' "VP_T", "C_T", "DC_C", "DC_T", "T_S", "CT_T", "CP_T", "CP_C", "CN_T", and'
-                ' "CN_C".'
+                ' "W", "S", "VP", "C", "T", "DC", "CT", "CP", "CN", "MLS", "MLT", "MLC", "C/S",'
+                ' "VP/T", "C/T", "DC/C", "DC/T", "T/S", "CT/T", "CP/T", "CP/C", "CN/T", and'
+                ' "CN/C".'
             ),
         )
         args_parser.add_argument(
-            "-p",
             "--reserve-parsed",
+            "-p",
             dest="is_reserve_parsed",
             action="store_true",
             default=False,
-            help="Reserve the parsed trees produced by the Stanford Parser.",
+            help="Reserve the parse trees produced by the Stanford Parser.",
         )
         args_parser.add_argument(
-            "-m",
             "--reserve-matched",
+            "-m",
             dest="is_reserve_matched",
             default=False,
             action="store_true",
             help="Reserve the matched subtrees produced by the Stanford Tregex.",
         )
         args_parser.add_argument(
+            "--no-parse",
+            dest="is_skip_parsing",
+            action="store_true",
+            default=False,
+            help=(
+                "Assume input as parse trees. By default, the program expects"
+                " raw text as input that will be parsed before querying. If you"
+                " already have parsed input files, use this flag to indicate that"
+                " the program should skip the parsing step and proceed directly"
+                " to querying. When this flag is set, the is_skip_querying and"
+                " reserve_parsed are automatically set as False."
+            ),
+        )
+        args_parser.add_argument(
             "--no-query",
             dest="is_skip_querying",
             action="store_true",
             default=False,
-            help="Parse the input files, save the parsed trees and exit.",
+            help="Parse the input files, save the parse trees and exit.",
         )
         args_parser.add_argument(
             "--quiet",
             dest="is_quiet",
             action="store_true",
             default=False,
             help="Stop NeoSCA from print anything except for final results.",
@@ -246,15 +260,15 @@
     Analyze files ranging from sample101.txt to sample200.txt.
 10. nsca sample10[1-9].txt sample1[1-9][0-9].txt sample200.txt --expand-wildcards
     Expand the specified wildcards and exit.
 11. nsca sample1.txt --max-length 100
     Only analyze sentences with lengths shorter than or equal to 100.
 12. nsca sample1.txt --newline-break always
     Consider newlines as sentence breaks.
-13. nsca --select VP T DC_C -- sample1.txt
+13. nsca --select VP T DC/C -- sample1.txt
     Select a subset of measures to analyze. Use -- to separate input
     filenames from the selected measures, or otherwise the program will take
     "sample1.txt" as a measure and then raise an error. Arguments other than
     input filenames should be specified at the left side of --.
 14. nsca -c sample1-sub1.txt sample1-sub2.txt
     Add up frequencies of the 9 syntactic structures of the subfiles and compute
     values of the 14 syntactic complexity indices for the imaginary parent file.
@@ -262,14 +276,18 @@
     Combine all the ".txt" files within the "samples/" directory
 16. nsca -c sample1-sub*.txt
     Wildcards are supported for -c.
 17. nsca -c sample1-sub*.txt -c sample2-sub*.txt
     Use multiple -c to combine different lists of subfiles respectively.
 18. nsca -c sample1-sub*.txt -c sample2-sub*.txt -- sample[3-9].txt
     Use -- to separate input filenames from names of the subfiles.
+19. nsca sample1.txt --no-query
+    Parse the input files, save the parsed trees and exit.
+20. nsca sample1.parsed --no-parse
+    Assume input as parse trees. Skip the parsing step and proceed directly to querying.
 
 Contact:
 1. https://github.com/tanloong/neosca/issues
 2. tanloong@foxmail.com
 """
         return args_parser
 
@@ -283,14 +301,17 @@
             options, ifile_list = self.args_parser.parse_known_args(argv[1:])
         if options.is_quiet:
             logging.basicConfig(format="%(message)s", level=logging.CRITICAL)
         else:
             logging.basicConfig(format="%(message)s", level=logging.INFO)
         if options.is_skip_querying:
             options.is_reserve_parsed = True
+        if options.is_skip_parsing:
+            options.is_skip_querying = False
+            options.is_reserve_parsed = False
 
         if options.text is not None:
             if ifile_list:
                 return False, "Unexpected argument(s):\n\n{}".format("\n".join(ifile_list))
             logging.info(f"Command-line text: {options.text}")
             verified_ifile_list = None
         else:
@@ -367,14 +388,15 @@
             "newline_break": options.newline_break,
             "max_length": options.max_length,
             "selected_measures": options.selected_measures,
             "is_reserve_parsed": options.is_reserve_parsed,
             "is_reserve_matched": options.is_reserve_matched,
             "is_stdout": options.is_stdout,
             "is_skip_querying": options.is_skip_querying,
+            "is_skip_parsing": options.is_skip_parsing,
             "is_pretokenized": options.is_pretokenized,
         }
         self.options = options
         return True, None
 
     def check_java(self) -> SCAProcedureResult:
         java_home = getenv(self.JAVA_HOME)
@@ -393,19 +415,19 @@
                 else:
                     java_home = err_msg
             java_bin = os.path.join(java_home, "bin")  # type:ignore
             path_orig = os.getenv("PATH", "")
             setenv(
                 "JAVA_HOME",
                 [java_home],  # type:ignore
-                refresh=True,
+                is_refresh=True,
                 is_quiet=self.options.is_quiet,
             )
             setenv(
-                "PATH", [java_bin], refresh=False, is_quiet=self.options.is_quiet
+                "PATH", [java_bin], is_refresh=False, is_quiet=self.options.is_quiet
             )  # type:ignore
             os.environ["JAVA_HOME"] = java_home  # type:ignore
             os.environ["PATH"] = java_bin + os.pathsep + path_orig  # type:ignore
         elif not self.options.is_quiet:
             color_print("OKGREEN", "ok", prefix="Java has already been installed. ")
         return True, None
 
@@ -422,15 +444,15 @@
             if not sucess:
                 return sucess, err_msg
             else:
                 stanford_parser_home = err_msg
                 setenv(
                     self.STANFORD_PARSER_HOME,
                     [stanford_parser_home],  # type:ignore
-                    refresh=True,
+                    is_refresh=True,
                     is_quiet=self.options.is_quiet,
                 )
                 self.options.stanford_parser_home = stanford_parser_home  # type:ignore
         elif not self.options.is_quiet:
             color_print("OKGREEN", "ok", prefix="Stanford Parser has already been installed. ")
         self.init_kwargs.update({"stanford_parser_home": self.options.stanford_parser_home})
         return True, None
@@ -448,15 +470,15 @@
             if not sucess:
                 return sucess, err_msg
             else:
                 stanford_tregex_home = err_msg
                 setenv(
                     self.STANFORD_TREGEX_HOME,
                     [stanford_tregex_home],  # type:ignore
-                    refresh=True,
+                    is_refresh=True,
                     is_quiet=self.options.is_quiet,
                 )
                 self.options.stanford_tregex_home = stanford_tregex_home  # type:ignore
         elif not self.options.is_quiet:
             color_print("OKGREEN", "ok", prefix="Stanford Tregex has already been installed. ")
         self.init_kwargs.update({"stanford_tregex_home": self.options.stanford_tregex_home})
         return True, None
@@ -500,62 +522,62 @@
                     prefix=f"{msg_num}. Frequency output was saved to ",
                     postfix=".",
                 )
             if self.options.is_reserve_parsed:
                 if self.verified_ifile_list or self.verified_subfile_lists:
                     msg_num += 1
                     logging.info(
-                        f"{msg_num}. Parsed trees were saved corresponding to input files,"
+                        f"{msg_num}. parse trees were saved corresponding to input files,"
                         ' with the same name but a ".parsed" extension.'
                     )
                 elif self.options.text is not None:
                     msg_num += 1
                     color_print(
                         "OKGREEN",
                         f"{self.cwd}{os.sep}cmdline_text.parsed",
-                        prefix=f"{msg_num}. Parsed trees were saved to ",
+                        prefix=f"{msg_num}. parse trees were saved to ",
                         postfix=".",
                     )
             if self.options.is_reserve_matched:
                 msg_num += 1
                 color_print(
                     "OKGREEN",
                     f"{os.path.abspath(self.odir_matched)}",
                     prefix=f"{msg_num}. Matched subtrees were saved to ",
                     postfix=".",
                 )
         if msg_num > 0:
             logging.info("Done.")
 
-    def run_tmpl(func):  # type: ignore
+    def run_tmpl(func: Callable):  # type:ignore
         def wrapper(self, *args, **kwargs):
             sucess, err_msg = self.check_python()
             if not sucess:
                 return sucess, err_msg
             sucess, err_msg = self.check_depends()
             if not sucess:
                 return sucess, err_msg
             if not self.options.is_stdout:
-                sucess, err_msg = try_write(self.options.ofile_freq, None)
+                sucess, err_msg = SCAIO.try_write(self.options.ofile_freq, None)
                 if not sucess:
                     return sucess, err_msg
             func(self, *args, **kwargs)  # type: ignore
             self.exit_routine()
             return True, None
 
         return wrapper
 
-    @run_tmpl  # type: ignore
+    @run_tmpl
     def run_on_text(self) -> None:
         from .neosca import NeoSCA
 
         analyzer = NeoSCA(**self.init_kwargs)
         analyzer.run_on_text(self.options.text)
 
-    @run_tmpl  # type: ignore
+    @run_tmpl
     def run_on_ifiles(self) -> None:
         from .neosca import NeoSCA
 
         analyzer = NeoSCA(**self.init_kwargs)
         analyzer.run_on_ifiles(self.verified_ifile_list)
         for subfiles in self.verified_subfile_lists:
             analyzer.run_on_ifiles(subfiles, is_combine=True)
@@ -581,23 +603,28 @@
         from .structure_counter import StructureCounter
 
         for structure in StructureCounter().structures_to_report:
             print(f"{structure.name}: {structure.desc}")
         return True, None
 
     def expand_wildcards(self) -> SCAProcedureResult:
+        is_not_found = True
         if self.verified_ifile_list:
+            is_not_found = False
             print("Input files:")
-            for ifile in sorted(self.verified_ifile_list):
-                print(f" {ifile}")
+            for i, ifile in enumerate(self.verified_ifile_list, 1):
+                print(f" {i}. {ifile}")
         if self.verified_subfile_lists:
-            for i, subfiles in enumerate(self.verified_subfile_lists):
-                print(f"Input subfile list {i+1}:")
-                for subfile in subfiles:
-                    print(f" {subfile}")
+            is_not_found = False
+            for i, subfiles in enumerate(self.verified_subfile_lists, 1):
+                print(f"Input subfile list {i}:")
+                for j, subfile in enumerate(subfiles, 1):
+                    print(f" {j}. {subfile}")
+        if is_not_found:
+            print("0 files and subfiles are found.")
         return True, None
 
     def show_version(self) -> SCAProcedureResult:
         print(__version__)
         return True, None
```

### Comparing `neosca-0.0.42/neosca/neosca.py` & `neosca-0.0.43/neosca/neosca.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,28 +21,30 @@
         newline_break: str = "never",
         max_length: Optional[int] = None,
         selected_measures: Optional[Set[str]] = None,
         is_reserve_parsed: bool = False,
         is_reserve_matched: bool = False,
         is_stdout: bool = False,
         is_skip_querying: bool = False,
+        is_skip_parsing: bool = False,
         is_pretokenized: bool = False,
         is_verbose: bool = True,
     ) -> None:
         self.ofile_freq = ofile_freq
         self.oformat_freq = oformat_freq
         self.classpaths = unite_classpaths(stanford_parser_home, stanford_tregex_home)
         self.odir_matched = odir_matched
         self.newline_break = newline_break
         self.max_length = max_length
         self.selected_measures = selected_measures
         self.is_reserve_parsed = is_reserve_parsed
         self.is_reserve_matched = is_reserve_matched
         self.is_stdout = is_stdout
         self.is_skip_querying = is_skip_querying
+        self.is_skip_parsing = is_skip_parsing
         self.is_pretokenized = is_pretokenized
         self.is_verbose = is_verbose
         self.counter_lists: List[StructureCounter] = []
         self.io = SCAIO()
 
         self.is_stanford_parser_initialized = False
         self.is_stanford_tregex_initialized = False
@@ -56,66 +58,74 @@
         if not self.is_stanford_parser_initialized:
             self.parser = StanfordParser(
                 classpaths=self.classpaths,
                 is_verbose=self.is_verbose,
             )
             self.is_stanford_parser_initialized = True
 
-    def _is_skip_parsing(self, ofile_parsed: str, ifile: str) -> bool:
-        """See whether a parsed file already exists"""
-        is_skip_parsing = False
+    def has_parse_file(self, ofile_parsed: str, ifile: str) -> bool:
+        """Check is a parse file already exists before parsing"""
+        has_parse_file = False
         is_exist = os.path.exists(ofile_parsed)
         if is_exist:
             is_not_empty = os.path.getsize(ofile_parsed) > 0
             is_parsed_newer_than_input = os.path.getmtime(ofile_parsed) > os.path.getmtime(ifile)
             if is_not_empty and is_parsed_newer_than_input:
-                is_skip_parsing = True
-        return is_skip_parsing
+                has_parse_file = True
+        return has_parse_file
 
     def query_against_trees(self, trees: str, counter: StructureCounter) -> StructureCounter:
         self.ensure_stanford_tregex_initialized()
         counter = self.tregex.query(
             counter,
             trees,
             is_reserve_matched=self.is_reserve_matched,
             odir_matched=self.odir_matched,
             is_stdout=self.is_stdout,
         )
         return counter
 
     def parse_text(self, text: str, ofile_parsed="cmdline_text.parsed") -> str:
+        if self.is_skip_parsing:  # assume input as parse trees
+            return text
+
         self.ensure_stanford_parser_initialized()
         trees = self.parser.parse(
             text,
             max_length=self.max_length,
             newline_break=self.newline_break,
             is_pretokenized=self.is_pretokenized,
             is_reserve_parsed=self.is_reserve_parsed,
             ofile_parsed=ofile_parsed,
             is_stdout=self.is_stdout,
         )
         return trees
 
     def run_on_text(self, text: str, ifile: str = "cmdline_text") -> None:
-        trees = self.parse_text(text)
+        trees: str = self.parse_text(text)
         if not self.is_skip_querying:
             counter = StructureCounter(ifile, selected_measures=self.selected_measures)
             counter = self.query_against_trees(trees, counter)
             self.counter_lists.append(counter)
             self.write_freq_output()
 
     def parse_ifile(self, ifile: str) -> str:
         """Parse a single file"""
+        if self.is_skip_parsing:
+            # assume input as parse trees
+            return self.io.read_txt(ifile, is_guess_encoding=False)
+
         ofile_parsed = os.path.splitext(ifile)[0] + ".parsed"
-        is_skip_parsing = self._is_skip_parsing(ofile_parsed=ofile_parsed, ifile=ifile)
-        if is_skip_parsing:
+        has_parse_file = self.has_parse_file(ofile_parsed=ofile_parsed, ifile=ifile)
+        if has_parse_file:
             logging.info(
                 f"[Parser] Parsing skipped: {ofile_parsed} already"
                 f" exists, and is non-empty and newer than {ifile}."
             )
+            # parse file are always (1) plain text, and (2) of utf-8 encoding
             return self.io.read_txt(ofile_parsed, is_guess_encoding=False)
         text = self.io.read_file(ifile)
         try:
             trees = self.parse_text(text, ofile_parsed)
         except KeyboardInterrupt:
             if os.path.exists(ofile_parsed):
                 os.remove(ofile_parsed)
@@ -131,45 +141,45 @@
     def run_on_ifiles(self, ifiles, is_combine=False) -> None:
         if not ifiles:
             return None
         total = len(ifiles)
         if not self.is_skip_querying:
             if is_combine:
                 parent_counter = StructureCounter(selected_measures=self.selected_measures)
-                for i, ifile in enumerate(ifiles):
-                    logging.info(f'[NeoSCA] Processing "{ifile}" ({i+1}/{total})...')
+                for i, ifile in enumerate(ifiles, 1):
+                    logging.info(f'[NeoSCA] Processing "{ifile}" ({i}/{total})...')
                     child_counter = self.parse_ifile_and_query(ifile)
                     parent_counter += child_counter
                 self.counter_lists.append(parent_counter)
             else:
-                for i, ifile in enumerate(ifiles):
-                    logging.info(f'[NeoSCA] Processing "{ifile}" ({i+1}/{total})...')
+                for i, ifile in enumerate(ifiles, 1):
+                    logging.info(f'[NeoSCA] Processing "{ifile}" ({i}/{total})...')
                     counter = self.parse_ifile_and_query(ifile)
                     self.counter_lists.append(counter)
             self.write_freq_output()
         else:
-            for i, ifile in enumerate(ifiles):
-                logging.info(f'[NeoSCA] Processing "{ifile}" ({i+1}/{total})...')
+            for i, ifile in enumerate(ifiles, 1):
+                logging.info(f'[NeoSCA] Processing "{ifile}" ({i}/{total})...')
                 self.parse_ifile(ifile)
 
     def get_freq_output(self, format_: str) -> str:
         assert format_ in ("csv", "json")
         if format_ == "csv":
             freq_output = self.counter_lists[0].fields
             for counter in self.counter_lists:
-                freq_dict = counter.get_freqs()
+                freq_dict = counter.get_all_freqs()
                 if "," in freq_dict["Filename"]:
                     freq_dict["Filename"] = '"' + freq_dict["Filename"] + '"'
                 freq_output += "\n" + ",".join(str(freq) for freq in freq_dict.values())
         else:
             import json
 
             final_freq_dict: Dict[str, List[Dict]] = {"Files": []}
             for counter in self.counter_lists:
-                freq_dict = counter.get_freqs()
+                freq_dict = counter.get_all_freqs()
                 final_freq_dict["Files"].append(freq_dict)
             freq_output = json.dumps(final_freq_dict)
         return freq_output
 
     def write_freq_output(self) -> None:
         freq_output = self.get_freq_output(self.oformat_freq)
         if not self.is_stdout:
```

### Comparing `neosca-0.0.42/neosca/parser.py` & `neosca-0.0.43/neosca/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             trees = self.parse_text(text, max_length, is_pretokenized)
         else:
             if newline_break == "always":
                 paragraphs = list(filter(None, text.split("\n")))
             else:
                 import re
 
-                paragraphs = re.split(r"(?:\r?\n){2,}", text)
+                paragraphs = re.split(r"(?:\r\n|\n|\r){2,}", text)
             trees = "\n".join(
                 self.parse_text(paragraph, max_length, is_pretokenized)
                 for paragraph in paragraphs
             )
         if is_reserve_parsed:
             if not is_stdout:
                 with open(ofile_parsed, "w", encoding="utf-8") as f:
```

### Comparing `neosca-0.0.42/neosca/querier.py` & `neosca-0.0.43/neosca/querier.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,20 +73,22 @@
         trees: str,
         is_reserve_matched: bool = False,
         odir_matched: str = "",
         is_stdout: bool = False,
     ):
         for structure in counter.structures_to_query:
             logging.info(f'[Tregex] Querying "{structure.desc}"...')
+            s_name = structure.name
             if structure.name == "W":
-                structure.freq = len(re.findall(r"\([A-Z]+\$? [^()—–-]+\)", trees))
+                freq = len(re.findall(r"\([A-Z]+\$? [^()—–-]+\)", trees))
+                counter.set_freq(s_name, freq)
                 continue
-            structure.freq, structure.matches = self.query_pattern(
-                structure.name, structure.pattern, trees
-            )
+            freq, matches = self.query_pattern(structure.name, structure.pattern, trees)
+            counter.set_freq(s_name, freq)
+            counter.set_matches(s_name, matches)
         if is_reserve_matched:  # pragma: no cover
             self.write_match_output(counter, odir_matched, is_stdout)
         return counter
 
     def write_match_output(
         self, counter: StructureCounter, odir_matched: str = "", is_stdout: bool = False
     ) -> None:  # pragma: no cover
```

### Comparing `neosca-0.0.42/neosca/structure_counter.py` & `neosca-0.0.43/neosca/structure_counter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,212 +1,114 @@
 from collections import OrderedDict
-from typing import Optional, Sequence, Set, Union
+from typing import Dict, List, Optional, Set, Union
+
+from .structure_data import data
 
 
 class Structure:
     def __init__(
         self,
         name: str,
         desc: str,
         pattern: str = "",
-        matches: Optional[list] = None,
+        *,
         requirements: Optional[list] = None,
     ) -> None:
         """
         :param name: name of the structure
         :param desc: description of the structure
         :param pattern: Tregex pattern
-        :param matches: matched subtrees by Tregex
         :param requirements: a list of structure names that current instance of Structure requires. Note that the elements come from the initial StructureCounter.structures_to_query, thus CN_T requires ["CN1", "CN2", "CN3", "T1", "T2"] instead of ["CN", "T"]
         """
         self.name = name
         self.desc = desc
         self.pattern = pattern
-        if matches is None:
-            self.matches = []
-        else:  # pragma: no cover
-            self.matches = matches
         if requirements is None:
             self.requirements = []
         else:
             self.requirements = requirements
         self.freq: Union[float, int] = 0
+        self.matches: list = []
 
     def __repr__(self) -> str:  # pragma: no cover
         return (
             f"name: {self.name} ({self.desc})\nrequirements: {self.requirements}\npattern:"
             f" {self.pattern}\nmatches: {self.matches}\nfrequency: {self.freq}"
         )
 
-    def __truediv__(self, other) -> Union[float, int]:
-        return round(self.freq / other.freq, 4) if other.freq else 0
-
 
 class StructureCounter:
     def __init__(self, ifile="", selected_measures: Optional[Set[str]] = None) -> None:
         self.ifile = ifile
         if selected_measures is None:
             self.selected_measures = set()
         else:
             self.selected_measures = selected_measures
-        self.W = Structure("W", "words")
-        self.S = Structure("S", "sentences", "ROOT")
-        self.VP1 = Structure("VP1", "regular verb phrases", "VP > S|SINV|SQ")
-        self.VP2 = Structure(
-            "VP2",
-            "verb phrases in inverted yes/no questions or in wh-questions",
-            "MD|VBZ|VBP|VBD > (SQ !< VP)",
-        )
-        self.C1 = Structure(
-            "C1",
-            "regular clauses",
-            (
-                "S|SINV|SQ "
-                "[> ROOT <, (VP <# VB) | <# MD|VBZ|VBP|VBD | < "
-                "(VP [<# MD|VBP|VBZ|VBD | < CC < (VP <# MD|VBP|VBZ|VBD)])]"
-            ),
-        )
-        self.C2 = Structure(
-            "C2",
-            "fragment clauses",
-            (
-                "FRAG > ROOT !<< "
-                "(S|SINV|SQ [> ROOT <, (VP <# VB) | <# MD|VBZ|VBP|VBD | < "
-                "(VP [<# MD|VBP|VBZ|VBD | < CC < "
-                "(VP <# MD|VBP|VBZ|VBD)])])"
-            ),
-        )
-        self.T1 = Structure(
-            "T1",
-            "regular T-units",
-            "S|SBARQ|SINV|SQ > ROOT | [$-- S|SBARQ|SINV|SQ !>> SBAR|VP]",
-        )
-        self.T2 = Structure(
-            "T2",
-            "fragment T-units",
-            "FRAG > ROOT !<< (S|SBARQ|SINV|SQ > ROOT | [$-- S|SBARQ|SINV|SQ !>> SBAR|VP])",
-        )
-        self.CN1 = Structure(
-            "CN1",
-            "complex nominals, type 1",
-            "NP !> NP [<< JJ|POS|PP|S|VBG | << (NP $++ NP !$+ CC)]",
-        )
-        self.CN2 = Structure(
-            "CN2",
-            "complex nominals, type 2",
-            "SBAR [<# WHNP | <# (IN < That|that|For|for) | <, S] & [$+ VP | > VP]",
-        )
-        self.CN3 = Structure("CN3", "complex nominals, type 3", "S < (VP <# VBG|TO) $+ VP")
-        self.DC = Structure(
-            "DC",
-            "dependent clauses",
-            (
-                "SBAR < "
-                "(S|SINV|SQ "
-                "[> ROOT <, (VP <# VB) | <# MD|VBZ|VBP|VBD | < "
-                "(VP [<# MD|VBP|VBZ|VBD | < CC < (VP <# MD|VBP|VBZ|VBD)])])"
-            ),
-        )
-        self.CT = Structure(
-            "CT",
-            "complex T-units",
-            (
-                "S|SBARQ|SINV|SQ [> ROOT | [$-- S|SBARQ|SINV|SQ !>> SBAR|VP]] << "
-                "(SBAR < (S|SINV|SQ "
-                "[> ROOT <, (VP <# VB) | <# MD|VBZ|VBP|VBD | < "
-                "(VP [<# MD|VBP|VBZ|VBD | < CC < "
-                "(VP <# MD|VBP|VBZ|VBD)])]))"
-            ),
-        )
-        self.CP = Structure("CP", "coordinate phrases", "ADJP|ADVP|NP|VP < CC")
 
-        self.VP = Structure("VP", "verb phrases", requirements=["VP1", "VP2"])
-        self.C = Structure("C", "clauses", requirements=["C1", "C2"])
-        self.T = Structure("T", "T-units", requirements=["T1", "T2"])
-        self.CN = Structure("CN", "complex nominals", requirements=["CN1", "CN2", "CN3"])
-
-        self.MLS = Structure("MLS", "mean length of sentence", requirements=["W", "S"])
-        self.MLT = Structure("MLT", "mean length of T-unit", requirements=["W", "T1", "T2"])
-        self.MLC = Structure("MLC", "mean length of clause", requirements=["W", "C1"])
-        self.C_S = Structure("C_S", "clauses per sentence", requirements=["C1", "S"])
-        self.VP_T = Structure(
-            "VP_T", "verb phrases per T-unit", requirements=["VP1", "T1", "T2"]
-        )
-        self.C_T = Structure("C_T", "clauses per T-unit", requirements=["C1", "T1", "T2"])
-        self.DC_C = Structure("DC_C", "dependent clauses per clause", requirements=["DC", "C1"])
-        self.DC_T = Structure(
-            "DC_T", "dependent clauses per T-unit", requirements=["DC", "T1", "T2"]
-        )
-        self.T_S = Structure("T_S", "T-units per sentence", requirements=["T1", "T2", "S"])
-        self.CT_T = Structure("CT_T", "complex T-unit ratio", requirements=["CT", "T1", "T2"])
-        self.CP_T = Structure(
-            "CP_T", "coordinate phrases per T-unit", requirements=["CP", "T1", "T2"]
-        )
-        self.CP_C = Structure("CP_C", "coordinate phrases per clause", requirements=["CP", "C1"])
-        self.CN_T = Structure(
-            "CN_T", "complex nominals per T-unit", requirements=["CN1", "CN2", "CN3", "T1", "T2"]
-        )
-        self.CN_C = Structure(
-            "CN_C", "complex nominals per clause", requirements=["CN1", "CN2", "CN3", "C1"]
-        )
-
-        self.structures_to_query: Sequence[Structure] = (
-            self.W,
-            self.S,
-            self.VP1,
-            self.VP2,
-            self.C1,
-            self.C2,
-            self.T1,
-            self.T2,
-            self.CN1,
-            self.CN2,
-            self.CN3,
-            self.DC,
-            self.CT,
-            self.CP,
-        )
-        self.structures_to_report: Sequence[Structure] = (
-            self.W,
-            self.S,
-            self.VP,
-            self.C,
-            self.T,
-            self.DC,
-            self.CT,
-            self.CP,
-            self.CN,
-            self.MLS,
-            self.MLT,
-            self.MLC,
-            self.C_S,
-            self.VP_T,
-            self.C_T,
-            self.DC_C,
-            self.DC_T,
-            self.T_S,
-            self.CT_T,
-            self.CP_T,
-            self.CP_C,
-            self.CN_T,
-            self.CN_C,
-        )
+        self.structures: Dict[str, Structure] = {}
+        for args, kwargs in data:
+            self.structures[args[0]] = Structure(*args, **kwargs)
+
+        self.structures_to_query: List[Structure] = [
+            self.structures[key]
+            for key in (
+                "W",
+                "S",
+                "VP1",
+                "VP2",
+                "C1",
+                "C2",
+                "T1",
+                "T2",
+                "CN1",
+                "CN2",
+                "CN3",
+                "DC",
+                "CT",
+                "CP",
+            )
+        ]
+
+        self.structures_to_report: List[Structure] = [
+            self.structures[key]
+            for key in (
+                "W",
+                "S",
+                "VP",
+                "C",
+                "T",
+                "DC",
+                "CT",
+                "CP",
+                "CN",
+                "MLS",
+                "MLT",
+                "MLC",
+                "C/S",
+                "VP/T",
+                "C/T",
+                "DC/C",
+                "DC/T",
+                "T/S",
+                "CT/T",
+                "CP/T",
+                "CP/C",
+                "CN/T",
+                "CN/C",
+            )
+        ]
 
         self.parse_selected_measures()
-        self.fields = "Filename," + ",".join(
-            (structure.name for structure in self.structures_to_report)
-        ).replace("_", "/")
+        self.fields = "Filename," + ",".join((s.name for s in self.structures_to_report))
 
     def parse_selected_measures(self):
         if len(self.selected_measures) > 0:
-            self.structures_to_report = [
-                structure
-                for structure in self.structures_to_report
-                if structure.name in self.selected_measures
-            ]
+            self.structures_to_report = list(
+                filter(lambda s: s.name in self.selected_measures, self.structures_to_report)
+            )
             selected_measures_extended = self.selected_measures.copy()
             for structure in self.structures_to_report:
                 for name in structure.requirements:
                     if name not in self.selected_measures:
                         selected_measures_extended.add(name)
             self.structures_to_query = [
                 structure
@@ -214,46 +116,79 @@
                 if structure.name in selected_measures_extended
             ]
 
     def update_freqs(self) -> None:
         """
         Update frequencies of complex nominals, clauses, verb phrases, and T-units
         """
-        self.VP.freq = self.VP1.freq + self.VP2.freq
-        self.C.freq = self.C1.freq + self.C2.freq
-        self.T.freq = self.T1.freq + self.T2.freq
-        self.CN.freq = self.CN1.freq + self.CN2.freq + self.CN3.freq
+        for s_name in ("VP", "C", "T", "CN"):
+            self.structures[s_name].freq = sum(
+                self.structures[requirement_name].freq
+                for requirement_name in self.structures[s_name].requirements
+            )
 
     def compute_14_indicies(self) -> None:
         """
         Compute the 14 syntactic complexity indices
         """
-        self.MLS.freq = self.W / self.S
-        self.MLT.freq = self.W / self.T
-        self.MLC.freq = self.W / self.C1
-        self.C_S.freq = self.C1 / self.S
-        self.VP_T.freq = self.VP1 / self.T
-        self.C_T.freq = self.C1 / self.T
-        self.DC_C.freq = self.DC / self.C1
-        self.DC_T.freq = self.DC / self.T
-        self.T_S.freq = self.T / self.S
-        self.CT_T.freq = self.CT / self.T
-        self.CP_T.freq = self.CP / self.T
-        self.CP_C.freq = self.CP / self.C1
-        self.CN_T.freq = self.CN / self.T
-        self.CN_C.freq = self.CN / self.C1
+        for s_name, dividend, divisor in (
+            ("MLS", "W", "S"),
+            ("MLT", "W", "T"),
+            ("MLC", "W", "C1"),
+            ("C/S", "C1", "S"),
+            ("VP/T", "VP1", "T"),
+            ("C/T", "C1", "T"),
+            ("DC/C", "DC", "C1"),
+            ("DC/T", "DC", "T"),
+            ("T/S", "T", "S"),
+            ("CT/T", "CT", "T"),
+            ("CP/T", "CP", "T"),
+            ("CP/C", "CP", "C1"),
+            ("CN/T", "CN", "T"),
+            ("CN/C", "CN", "C1"),
+        ):
+            divident_freq, divisor_freq = (
+                self.structures[dividend].freq,
+                self.structures[divisor].freq,
+            )
+            self.structures[s_name].freq = (
+                round(divident_freq / divisor_freq, 4) if divisor_freq else 0
+            )
+
+    def set_freq(self, structure_name: str, freq: int) -> None:
+        if structure_name not in self.structures:
+            raise ValueError(f"{structure_name} not counted")
+        elif not isinstance(freq, int) or freq < 0:
+            raise ValueError("freq should be a non-negative integer")
+        else:
+            self.structures[structure_name].freq = freq
+
+    def set_matches(self, structure_name: str, matches: list) -> None:
+        if structure_name not in self.structures:
+            raise ValueError(f"{structure_name} not counted")
+        elif not isinstance(matches, list):
+            raise ValueError("matches should be a list object")
+        else:
+            self.structures[structure_name].matches = matches
+
+    def get_freq(self, structure_name: str) -> Union[float, int]:
+        if structure_name not in self.structures:
+            raise ValueError(f"{structure_name} not counted")
+        return self.structures[structure_name].freq
 
-    def get_freqs(self) -> dict:
+    def get_all_freqs(self) -> dict:
         self.update_freqs()
         self.compute_14_indicies()
         freq_dict = OrderedDict({"Filename": self.ifile})
         for structure in self.structures_to_report:
             freq_dict[structure.name] = str(structure.freq)
         return freq_dict
 
     def __add__(self, other: "StructureCounter") -> "StructureCounter":
         new_ifile = self.ifile + "+" + other.ifile if self.ifile else other.ifile
-        selected_measures = self.selected_measures | other.selected_measures
-        new = StructureCounter(new_ifile, selected_measures=selected_measures)
-        for structure in new.structures_to_query:
-            exec("new.{0}.freq = self.{0}.freq + other.{0}.freq".format(structure.name))
+        new_selected_measures = self.selected_measures | other.selected_measures
+        new = StructureCounter(new_ifile, selected_measures=new_selected_measures)
+        for s in new.structures_to_query:
+            s_name = s.name
+            freq = self.get_freq(s_name) + other.get_freq(s_name)
+            new.set_freq(s_name, freq)  # type: ignore
         return new
```

### Comparing `neosca-0.0.42/neosca/util_env.py` & `neosca-0.0.43/neosca/util_env.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import os
 from typing import List, Optional
 
 from .util_platform_info import IS_DARWIN, IS_LINUX, IS_WINDOWS
 from .util_print import color_print
 
 
-def _setenv_windows(env_var: str, paths: List[str], refresh: bool = False) -> None:
+def _setenv_windows(env_var: str, paths: List[str], is_refresh: bool = False) -> None:
     import winreg  # Allows access to the windows registry
     import ctypes  # Allows interface with low-level C API's
 
     with winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER) as root:  # type:ignore
         # Get the current user registry
         with winreg.OpenKey(root, "Environment", 0, winreg.KEY_ALL_ACCESS) as key:  # type:ignore
             # Go to the environment key
-            if refresh or os.environ.get(env_var) is None:
+            if is_refresh or os.environ.get(env_var) is None:
                 new_value = ";".join(paths)
             else:
                 existing_value = os.environ.get(env_var)
                 new_value = existing_value + ";" + ";".join(paths)  # type:ignore
                 # Takes the current path value and appends the new program path
             winreg.SetValueEx(key, env_var, 0, winreg.REG_EXPAND_SZ, new_value)  # type:ignore
             # Updated the path with the updated path
@@ -40,15 +40,15 @@
             "Environment",
             SMTO_ABORTIFHUNG,
             5000,
             ctypes.byref(result),
         )
 
 
-def _setenv_unix(env_var: str, paths: List[str], refresh: bool = False) -> None:
+def _setenv_unix(env_var: str, paths: List[str], is_refresh: bool = False) -> None:
     shell = os.environ.get("SHELL")
     if shell is None:
         logging.warning(
             "Failed to permanently append {path} to {env_var}.\nReason: can't detect current"
             " shell."
         )
     else:
@@ -74,20 +74,20 @@
             if not os.path.isfile(rcfile):
                 configs = []
             else:
                 with open(rcfile, "r", encoding="utf-8") as f:
                     configs = [line.strip() for line in f.readlines()]
             new_config = (
                 f"export {env_var}={new_paths}"
-                if refresh
+                if is_refresh
                 else f"export {env_var}=${env_var}:{new_paths}"
             )
             duplicated_config_index = []
             for i, config in enumerate(configs):
-                if refresh:
+                if is_refresh:
                     if config.startswith(f"export {env_var}"):
                         duplicated_config_index.append(i)
                 else:
                     if config == new_config:
                         duplicated_config_index.append(i)
             for i in duplicated_config_index:
                 del configs[i]
@@ -96,21 +96,21 @@
             else:
                 configs.append(new_config)
             with open(rcfile, "w", encoding="utf-8") as f:
                 f.write("\n".join(configs))
 
 
 def setenv(
-    env_var: str, paths: List[str], refresh: bool = False, is_quiet: bool = False
+    env_var: str, paths: List[str], is_refresh: bool = False, is_quiet: bool = False
 ) -> None:
     assert any((IS_WINDOWS, IS_DARWIN, IS_LINUX))
     if IS_WINDOWS:
-        _setenv_windows(env_var, paths, refresh)
+        _setenv_windows(env_var, paths, is_refresh)
     else:
-        _setenv_unix(env_var, paths, refresh)
+        _setenv_unix(env_var, paths, is_refresh)
     if not is_quiet:
         color_print(
             "OKGREEN",
             env_var,
             prefix="Added the following path(s) to ",
             postfix=":\n" + "\n".join(paths),
         )
```

### Comparing `neosca-0.0.42/neosca/util_print.py` & `neosca-0.0.43/neosca/util_print.py`

 * *Files identical despite different names*

### Comparing `neosca-0.0.42/neosca.egg-info/PKG-INFO` & `neosca-0.0.43/neosca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neosca
-Version: 0.0.42
+Version: 0.0.43
 Summary: Another syntactic complexity analyzer of written English language samples
 Home-page: https://github.com/tanloong/neosca
-Author: TAN Long
+Author: Long Tan
 Author-email: tanloong@foxmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
@@ -100,15 +100,15 @@
 
 <!-- vim-markdown-toc -->
 
 ## Highlights
 
 * Cross-platform compatibility: Windows, macOS, and Linux
 * Flexible command-line options to serve various needs
-* Supports reading docx files
+* Supports reading txt/docx/odt files
 
 ## Install
 
 ### Install NeoSCA
 
 To install NeoSCA, you need to have [Python](https://www.python.org/) 3.7 or later installed on your system. You can check if you already have Python installed by running the following command in your terminal:
 
@@ -156,15 +156,15 @@
 To analyze a single file, use the command `nsca` followed by the file path.
 
 ```sh
 nsca ./samples/sample1.txt
 nsca ./samples/sample1.docx
 ```
 
-When working on docx files, tables, figures, images, and other unrelated elements (except for headers and footers, which will be automatically ignored) should be manually removed before they are analyzed.
+Tables, figures, images, and other unrelated elements (except for headers and footers, which will be automatically ignored) should be manually removed before docx/odt files are analyzed.
 
 After running the above command, a `result.csv` file will be generated in the current directory. You can specify a different output filename using `-o/--output-file`.
 
 ```sh
 nsca ./samples/sample1.txt -o sample1.csv
 # frequency output: ./sample1.csv
 ```
@@ -237,15 +237,15 @@
 It is for text with hard line breaks and a blank line between paragraphs.
 
 #### Select a Subset of Measures
 
 NeoSCA by default outputs values of all of the available measures. You can use `--select` to only analyze measures that you are interested in. To see a full list of available measures, use `nsca --list`.
 
 ```sh
-nsca --select VP T DC_C -- sample1.txt
+nsca --select VP T DC/C -- sample1.txt
 ```
 
 To avoid the program taking input filenames as a selected measure and raising an error, use `--` to separate them from the measures. All arguments after `--` will be considered input filenames. Make sure to specify arguments except for input filenames at the left side of `--`.
 
 #### Combine Subfiles
 
 Use `-c`/`--combine-subfiles` to add up frequencies of the 9 syntactic structures of subfiles and compute values of the 14 syntactic complexity indices for the imaginary parent file. You can use this option multiple times to combine different lists of subfiles respectively. The `--` should be used to separate input filenames from input subfile-names.
@@ -319,14 +319,22 @@
 ```sh
 nsca samples/sample1.txt --no-query
 # parsed trees: samples/sample1.parsed
 nsca --text 'This is a test.' --no-query
 # parsed trees: ./cmdline_text.parsed
 ```
 
+#### Parse trees as input
+
+By default, the program expects raw text as input that will be parsed before querying. If you already have parsed input files, use `--no-parse` to indicate that the program should skip the parsing step and proceed directly to querying. When this flag is set, the is_skip_querying and reserve_parsed are automatically set as False.
+
+```sh
+nsca samples/sample1.parsed --no-parse
+```
+
 #### List Output Fields
 
 Use `--list` to print a list of all the available output fields.
 
 <details>
 
 <summary>
@@ -369,40 +377,40 @@
 
 <summary>
 BibTeX
 </summary>
 
 ```BibTeX
 @misc{tan2022neosca,
-title        = {NeoSCA: A Rewrite of L2 Syntactic Complexity Analyzer, version 0.0.42},
+title        = {NeoSCA: A Rewrite of L2 Syntactic Complexity Analyzer, version 0.0.43},
 author       = {Long Tan},
 howpublished = {\url{https://github.com/tanloong/neosca}},
 year         = {2022}
 }
 ```
 
 </details>
 
 <details>
 
 <summary>
 APA (7th edition)
 </summary>
 
-<pre>Tan, L. (2022). <i>NeoSCA</i> (version 0.0.42) [Computer software]. Github. https://github.com/tanloong/neosca</pre>
+<pre>Tan, L. (2022). <i>NeoSCA</i> (version 0.0.43) [Computer software]. Github. https://github.com/tanloong/neosca</pre>
 
 </details>
 
 <details>
 
 <summary>
 MLA (9th edition)
 </summary>
 
-<pre>Tan, Long. <i>NeoSCA</i>. version 0.0.42, GitHub, 2022, https://github.com/tanloong/neosca.</pre>
+<pre>Tan, Long. <i>NeoSCA</i>. version 0.0.43, GitHub, 2022, https://github.com/tanloong/neosca.</pre>
 
 </details>
 
 Also, you need to cite Xiaofei's article describing L2SCA.
 
 <details>
```

### Comparing `neosca-0.0.42/neosca.egg-info/SOURCES.txt` & `neosca-0.0.43/neosca.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 neosca/__init__.py
 neosca/__main__.py
+neosca/about.py
 neosca/depends_installer.py
 neosca/io.py
 neosca/main.py
 neosca/neosca.py
 neosca/parser.py
 neosca/querier.py
 neosca/structure_counter.py
+neosca/structure_data.py
 neosca/util.py
 neosca/util_env.py
 neosca/util_platform_info.py
 neosca/util_print.py
 neosca.egg-info/PKG-INFO
 neosca.egg-info/SOURCES.txt
 neosca.egg-info/dependency_links.txt
```

### Comparing `neosca-0.0.42/tests/test_cmdline.py` & `neosca-0.0.43/tests/test_cmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         )
 
     def test_list_fields(self):
         result = self.template(
             ["python", "-m", "neosca", "--list"], text=None, expected_output_file=None
         )
         result_stdout = result.stdout.decode("utf-8")
-        ncorrect_lines = len(re.findall(r"^[A-Z_]+: .*$", result_stdout, re.MULTILINE))
+        ncorrect_lines = len(re.findall(r"^[A-Z/]+: .*$", result_stdout, re.MULTILINE))
         self.assertEqual(result_stdout.count("\n"), 23)
         self.assertEqual(ncorrect_lines, 23)
 
     def test_show_version(self):
         result = self.template(
             ["python", "-m", "neosca", "--version"], text=None, expected_output_file=None
         )
```

### Comparing `neosca-0.0.42/tests/test_main.py` & `neosca-0.0.43/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `neosca-0.0.42/tests/test_parser.py` & `neosca-0.0.43/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `neosca-0.0.42/tests/test_querier.py` & `neosca-0.0.43/tests/test_querier.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 class TestStanfordTregex(BaseTmpl):
     def setUp(self):
         self.counter = StructureCounter()
         self.tregex = StanfordTregex(classpaths=classpaths)
         return super().setUp()
 
     def test_query(self):
-        structures = self.tregex.query(self.counter, tree)
-        structures.update_freqs()
-        self.assertEqual(1, structures.S.freq)
-        self.assertEqual(2, structures.VP.freq)
-        self.assertEqual(1, structures.C.freq)
-        self.assertEqual(1, structures.T.freq)
-        self.assertEqual(0, structures.DC.freq)
-        self.assertEqual(0, structures.CT.freq)
-        self.assertEqual(0, structures.CP.freq)
-        self.assertEqual(1, structures.CN.freq)
+        counter = self.tregex.query(self.counter, tree)
+        counter.update_freqs()
+        self.assertEqual(1, counter.structures["S"].freq)
+        self.assertEqual(2, counter.structures["VP"].freq)
+        self.assertEqual(1, counter.structures["C"].freq)
+        self.assertEqual(1, counter.structures["T"].freq)
+        self.assertEqual(0, counter.structures["DC"].freq)
+        self.assertEqual(0, counter.structures["CT"].freq)
+        self.assertEqual(0, counter.structures["CP"].freq)
+        self.assertEqual(1, counter.structures["CN"].freq)
```

