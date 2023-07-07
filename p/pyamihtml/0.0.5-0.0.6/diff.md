# Comparing `tmp/pyamihtml-0.0.5.tar.gz` & `tmp/pyamihtml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyamihtml-0.0.5.tar", last modified: Tue Jul  4 16:19:08 2023, max compression
+gzip compressed data, was "dist/pyamihtml-0.0.6.tar", last modified: Fri Jul  7 09:25:21 2023, max compression
```

## Comparing `pyamihtml-0.0.5.tar` & `pyamihtml-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 16:19:08.378072 pyamihtml-0.0.5/
--rw-r--r--   0 pm286      (503) staff       (20)     5420 2022-09-21 21:52:33.000000 pyamihtml-0.0.5/CONFIG.md
--rw-r--r--   0 pm286      (503) staff       (20)    11357 2021-08-20 16:43:32.000000 pyamihtml-0.0.5/LICENSE
--rw-r--r--   0 pm286      (503) staff       (20)      159 2022-09-21 21:52:33.000000 pyamihtml-0.0.5/MANIFEST.in
--rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-04 16:19:08.377945 pyamihtml-0.0.5/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)     8963 2023-05-24 09:30:50.000000 pyamihtml-0.0.5/README.md
--rw-r--r--   0 pm286      (503) staff       (20)     1800 2021-09-04 09:10:40.000000 pyamihtml-0.0.5/config.ini.master
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 16:19:08.372186 pyamihtml-0.0.5/pyamihtml/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2021-08-20 16:43:32.000000 pyamihtml-0.0.5/pyamihtml/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     5168 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/pyamihtml/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)    10020 2023-07-03 08:18:38.000000 pyamihtml-0.0.5/pyamihtml/ami_config.py
--rw-r--r--   0 pm286      (503) staff       (20)   156540 2023-07-01 22:53:26.000000 pyamihtml-0.0.5/pyamihtml/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    10529 2023-07-01 20:43:25.000000 pyamihtml-0.0.5/pyamihtml/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     2634 2023-07-04 15:23:49.000000 pyamihtml-0.0.5/pyamihtml/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)   103045 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/pyamihtml/ami_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)     3192 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/pyamihtml/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10585 2023-06-27 08:49:50.000000 pyamihtml-0.0.5/pyamihtml/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    19684 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/pyamihtml/bbox_copy.py
--rw-r--r--   0 pm286      (503) staff       (20)    15062 2023-07-04 10:08:02.000000 pyamihtml-0.0.5/pyamihtml/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    52982 2023-07-01 19:02:25.000000 pyamihtml-0.0.5/pyamihtml/ipcc.py
--rw-r--r--   0 pm286      (503) staff       (20)    44047 2023-07-04 16:17:49.000000 pyamihtml-0.0.5/pyamihtml/pyamix.py
--rw-r--r--   0 pm286      (503) staff       (20)    25940 2023-07-01 12:42:42.000000 pyamihtml-0.0.5/pyamihtml/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    33891 2023-07-04 15:51:32.000000 pyamihtml-0.0.5/pyamihtml/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    27429 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/pyamihtml/xml_lib.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 16:19:08.373170 pyamihtml-0.0.5/pyamihtml.egg-info/
--rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-04 16:19:08.000000 pyamihtml-0.0.5/pyamihtml.egg-info/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)      942 2023-07-04 16:19:08.000000 pyamihtml-0.0.5/pyamihtml.egg-info/SOURCES.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-04 16:19:08.000000 pyamihtml-0.0.5/pyamihtml.egg-info/dependency_links.txt
--rw-r--r--   0 pm286      (503) staff       (20)       53 2023-07-04 16:19:08.000000 pyamihtml-0.0.5/pyamihtml.egg-info/entry_points.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2023-06-30 07:44:44.000000 pyamihtml-0.0.5/pyamihtml.egg-info/not-zip-safe
--rw-r--r--   0 pm286      (503) staff       (20)       64 2023-07-04 16:19:08.000000 pyamihtml-0.0.5/pyamihtml.egg-info/requires.txt
--rw-r--r--   0 pm286      (503) staff       (20)       10 2023-07-04 16:19:08.000000 pyamihtml-0.0.5/pyamihtml.egg-info/top_level.txt
--rw-r--r--   0 pm286      (503) staff       (20)      511 2023-01-08 16:25:37.000000 pyamihtml-0.0.5/requirements.txt
--rw-r--r--   0 pm286      (503) staff       (20)       38 2023-07-04 16:19:08.378109 pyamihtml-0.0.5/setup.cfg
--rw-r--r--   0 pm286      (503) staff       (20)     2264 2023-07-04 16:17:16.000000 pyamihtml-0.0.5/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 16:19:08.377655 pyamihtml-0.0.5/test/
--rw-r--r--   0 pm286      (503) staff       (20)     7530 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)      775 2022-10-29 09:43:23.000000 pyamihtml-0.0.5/test/test_experiment.py
--rw-r--r--   0 pm286      (503) staff       (20)     4194 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)     8874 2021-11-24 22:01:19.000000 pyamihtml-0.0.5/test/test_gui.py
--rw-r--r--   0 pm286      (503) staff       (20)   106191 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    14031 2023-07-04 15:23:49.000000 pyamihtml-0.0.5/test/test_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-01 20:28:05.000000 pyamihtml-0.0.5/test/test_ipcc.py
--rw-r--r--   0 pm286      (503) staff       (20)      439 2023-07-01 20:50:25.000000 pyamihtml-0.0.5/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    79214 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)     8530 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_pyamix.py
--rw-r--r--   0 pm286      (503) staff       (20)     1071 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)      299 2022-08-26 08:16:11.000000 pyamihtml-0.0.5/test/test_text.py
--rw-r--r--   0 pm286      (503) staff       (20)     7591 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    34807 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)      663 2023-06-30 07:32:29.000000 pyamihtml-0.0.5/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-07 09:25:21.118125 pyamihtml-0.0.6/
+-rw-r--r--   0 pm286      (503) staff       (20)     5420 2022-09-21 21:52:33.000000 pyamihtml-0.0.6/CONFIG.md
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2021-08-20 16:43:32.000000 pyamihtml-0.0.6/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)      159 2022-09-21 21:52:33.000000 pyamihtml-0.0.6/MANIFEST.in
+-rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-07 09:25:21.117977 pyamihtml-0.0.6/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)     8963 2023-05-24 09:30:50.000000 pyamihtml-0.0.6/README.md
+-rw-r--r--   0 pm286      (503) staff       (20)     1800 2021-09-04 09:10:40.000000 pyamihtml-0.0.6/config.ini.master
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-07 09:25:21.112001 pyamihtml-0.0.6/pyamihtml/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2021-08-20 16:43:32.000000 pyamihtml-0.0.6/pyamihtml/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5168 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/pyamihtml/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10020 2023-07-03 08:18:38.000000 pyamihtml-0.0.6/pyamihtml/ami_config.py
+-rw-r--r--   0 pm286      (503) staff       (20)   156540 2023-07-01 22:53:26.000000 pyamihtml-0.0.6/pyamihtml/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10529 2023-07-01 20:43:25.000000 pyamihtml-0.0.6/pyamihtml/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     6723 2023-07-05 17:36:18.000000 pyamihtml-0.0.6/pyamihtml/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)   103045 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/pyamihtml/ami_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     3192 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/pyamihtml/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10585 2023-06-27 08:49:50.000000 pyamihtml-0.0.6/pyamihtml/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19684 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/pyamihtml/bbox_copy.py
+-rw-r--r--   0 pm286      (503) staff       (20)    15062 2023-07-04 10:08:02.000000 pyamihtml-0.0.6/pyamihtml/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    53018 2023-07-06 08:56:21.000000 pyamihtml-0.0.6/pyamihtml/ipcc.py
+-rw-r--r--   0 pm286      (503) staff       (20)    44047 2023-07-07 09:24:13.000000 pyamihtml-0.0.6/pyamihtml/pyamix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    25940 2023-07-01 12:42:42.000000 pyamihtml-0.0.6/pyamihtml/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    33891 2023-07-04 15:51:32.000000 pyamihtml-0.0.6/pyamihtml/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27429 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/pyamihtml/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-07 09:25:21.113062 pyamihtml-0.0.6/pyamihtml.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-07 09:25:21.000000 pyamihtml-0.0.6/pyamihtml.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      942 2023-07-07 09:25:21.000000 pyamihtml-0.0.6/pyamihtml.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-07 09:25:21.000000 pyamihtml-0.0.6/pyamihtml.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       53 2023-07-07 09:25:21.000000 pyamihtml-0.0.6/pyamihtml.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2023-06-30 07:44:44.000000 pyamihtml-0.0.6/pyamihtml.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)       64 2023-07-07 09:25:21.000000 pyamihtml-0.0.6/pyamihtml.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       10 2023-07-07 09:25:21.000000 pyamihtml-0.0.6/pyamihtml.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)      511 2023-01-08 16:25:37.000000 pyamihtml-0.0.6/requirements.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2023-07-07 09:25:21.118159 pyamihtml-0.0.6/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     2264 2023-07-07 09:24:13.000000 pyamihtml-0.0.6/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-07 09:25:21.117692 pyamihtml-0.0.6/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     7530 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)      775 2022-10-29 09:43:23.000000 pyamihtml-0.0.6/test/test_experiment.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4194 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8874 2021-11-24 22:01:19.000000 pyamihtml-0.0.6/test/test_gui.py
+-rw-r--r--   0 pm286      (503) staff       (20)   106191 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    15153 2023-07-05 17:37:02.000000 pyamihtml-0.0.6/test/test_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-01 20:28:05.000000 pyamihtml-0.0.6/test/test_ipcc.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1216 2023-07-05 17:28:26.000000 pyamihtml-0.0.6/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    79214 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8530 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_pyamix.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1071 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)      299 2022-08-26 08:16:11.000000 pyamihtml-0.0.6/test/test_text.py
+-rw-r--r--   0 pm286      (503) staff       (20)     7591 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    34807 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)      663 2023-06-30 07:32:29.000000 pyamihtml-0.0.6/test/test_xml.py
```

### Comparing `pyamihtml-0.0.5/CONFIG.md` & `pyamihtml-0.0.6/CONFIG.md`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/LICENSE` & `pyamihtml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/PKG-INFO` & `pyamihtml-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamihtml
-Version: 0.0.5
+Version: 0.0.6
 Summary: pdf2html converter
 Home-page: https://github.com/petermr/pyamihtml
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Platform: UNKNOWN
```

### Comparing `pyamihtml-0.0.5/README.md` & `pyamihtml-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/config.ini.master` & `pyamihtml-0.0.6/config.ini.master`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ami_bib.py` & `pyamihtml-0.0.6/pyamihtml/ami_bib.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ami_config.py` & `pyamihtml-0.0.6/pyamihtml/ami_config.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ami_html.py` & `pyamihtml-0.0.6/pyamihtml/ami_html.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ami_integrate.py` & `pyamihtml-0.0.6/pyamihtml/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ami_pdf.py` & `pyamihtml-0.0.6/pyamihtml/ami_pdf.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ami_svg.py` & `pyamihtml-0.0.6/pyamihtml/ami_svg.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ami_util.py` & `pyamihtml-0.0.6/pyamihtml/ami_util.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/bbox_copy.py` & `pyamihtml-0.0.6/pyamihtml/bbox_copy.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/file_lib.py` & `pyamihtml-0.0.6/pyamihtml/file_lib.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/ipcc.py` & `pyamihtml-0.0.6/pyamihtml/ipcc.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         return href_as
 
 
 class IPCCArgs(AbstractArgs):
     INPUT = "input"
     INFORMAT = "informat"
     OPERATION = "operation"
-    KWARGS = "otherargs"
+    KWARGS = "kwords"
     OUTDIR = "outdir"
     SECTIONS = "sections"
     VAR = "var"
 
     PDF2HTML = "pdf2html"
     AUTHORS = "authors"
 
@@ -354,34 +354,44 @@
         if self.parser is None:
             self.parser = argparse.ArgumentParser()
         self.parser.description = textwrap.dedent(
             'Manage and search IPCC resources and other climate stuff. \n'
             '----------------------------------------------------------\n'
             'see pyamihtml/IPCC.md'
             '\nExamples:\n'
-            f'parse foo.pdf and create default HTML'
-            f'  * IPCC --input foo.pdf\n'
+            'help'
+            ''
+            'parse foo.pdf and create default HTML'
+            f'  pyamihtml IPCC --input foo.pdf\n'
+            f''
 
         )
         self.parser.formatter_class = argparse.RawDescriptionHelpFormatter
+        INPUT_HELP = f"input from:\n" \
+                     f"   file/s single, multiple, and glob/wildcard (experimental)\n" \
+                     f"   directories (needs {self.INFORMAT})\n" \
+                     f"   URL/s (must start with 'https:); provide {self.OUTDIR} for output' \n"
         self.parser.add_argument(f"--{IPCCArgs.INPUT}", nargs="+",
-                                 help="read one or more resources. file/listof files/globs/URLs")
+                                 help=INPUT_HELP)
 
+        INFORM_HELP = "input format/s; experimental"
         self.parser.add_argument(f"--{IPCCArgs.INFORMAT}", nargs="+", default="PDF",
-                                 help="input format/s")
+                                 help=INFORM_HELP)
         self.parser.add_argument(f"--{IPCCArgs.OPERATION}", nargs="?", const="all",
                                  choices=(IPCCArgs.PDF2HTML, IPCCArgs.AUTHORS),
-                                 help="operation to perform", default=IPCCArgs.PDF2HTML)
+                                 help="operation to perform; default pdf2html", default=IPCCArgs.PDF2HTML)
         self.parser.add_argument(f"--{IPCCArgs.KWARGS}", nargs="*",
                                  help="space-separated list of colon_separated keyword-value pairs, format kw1:val1 kw2:val2;\nif empty list gives help")
 
+        OUTDIR_HELP = "output directory, required for URL input. If not given, autogenerated from file names"
         self.parser.add_argument(f"--{IPCCArgs.OUTDIR}", nargs=1,
-                                 help="output directory, required for URL input. If not given, autogenerated from file names")
-        self.parser.add_argument(f"--{IPCCArgs.VAR}", nargs=2,
-                                 help="set environment variable (name value)")
+                                 help=OUTDIR_HELP)
+        #
+        # self.parser.add_argument(f"--{IPCCArgs.VAR}", nargs=2,
+        #                          help="set environment variable (name value)")
         return self.parser
 
     # class ProjectArgs:
     def process_args(self):
         """runs parsed args
         :return:
 
@@ -455,27 +465,14 @@
     def get_outdir(self):
         outdir = self.arg_dict.get(IPCCArgs.OUTDIR)
         return outdir
 
     def get_author_roles(self):
         pass
 
-    # def get_xxx(entry):
-    #     anchors = entry.xpath(f"{H_A}")
-    #     # if len(anchors) != 1:
-    #     #     continue
-    #     anchor0 = anchors[0]
-    #     id = anchor0.get(A_ID)
-    #     print(f">?>{id}")
-    #     spans = entry.xpath(f"{H_SPAN}")
-    #     text = " ".join(spans[1:])
-    #     href_as = entry.xpath(f"{H_SPAN}/{H_A}")
-    #     return href_as
-
-
 class IPCCSections:
 
     @classmethod
     def get_ipcc_regexes(cls, front_back="Table of Contents|Frequently Asked Questions|Executive Summary|References"):
         """
         :param front_back: common section headings (not numbered)
         :return: (section_regex_dict, section_regexes) to manage regexes (largely for IPCC).
```

### Comparing `pyamihtml-0.0.5/pyamihtml/pyamix.py` & `pyamihtml-0.0.6/pyamihtml/pyamix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1129,15 +1129,15 @@
 
     def version(self):
         """
         reads setup.py and extracts line of form version='0.0.29'
         This is still a mess. We need to set the version once somewhere.
         """
 
-        version = '0.0.5' # 2023-07-03
+        version = '0.0.6' # 2023-07-03
         if False: # this fails - it gets the python distrib
             with open(Path(Path(__file__).parent.parent, "setup.py"), "r") as f:
                 setup_lines = f.readlines()
                 for line in setup_lines:
                     match = re.match("\s*version\s*=\s*\'\s*(\d+\.\d+\.\d+)\s*\'\s*,", line)
                     if match:
                         version = match.group(1)
```

### Comparing `pyamihtml-0.0.5/pyamihtml/util.py` & `pyamihtml-0.0.6/pyamihtml/util.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/wikimedia.py` & `pyamihtml-0.0.6/pyamihtml/wikimedia.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml/xml_lib.py` & `pyamihtml-0.0.6/pyamihtml/xml_lib.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/pyamihtml.egg-info/PKG-INFO` & `pyamihtml-0.0.6/pyamihtml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamihtml
-Version: 0.0.5
+Version: 0.0.6
 Summary: pdf2html converter
 Home-page: https://github.com/petermr/pyamihtml
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Platform: UNKNOWN
```

### Comparing `pyamihtml-0.0.5/pyamihtml.egg-info/SOURCES.txt` & `pyamihtml-0.0.6/pyamihtml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/setup.py` & `pyamihtml-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
  # 'backports',
 
 ]
 
 setup(
     name='pyamihtml',
     url='https://github.com/petermr/pyamihtml',
-    version='0.0.5',
+    version='0.0.6',
     description='pdf2html converter',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `pyamihtml-0.0.5/test/test_all.py` & `pyamihtml-0.0.6/test/test_all.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_experiment.py` & `pyamihtml-0.0.6/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_file.py` & `pyamihtml-0.0.6/test/test_file.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_gui.py` & `pyamihtml-0.0.6/test/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_html.py` & `pyamihtml-0.0.6/test/test_html.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_integrate.py` & `pyamihtml-0.0.6/test/test_integrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from urllib import request
 
 import lxml
 import pandas as pd
 import pdfplumber
 import pyvis
 import requests
+from sklearn.cluster import AgglomerativeClustering, KMeans
+from sklearn.feature_extraction.text import TfidfVectorizer
+from sklearn.metrics.pairwise import cosine_similarity
 
 from pyamihtml.ami_integrate import HtmlGenerator
 # from pyamihtml.ami_html import HtmlStyle
 # from pyamihtml.ami_integrate import HtmlGenerator
 # from pyamihtml.file_lib import FileLib
 # from pyamihtml.ipcc import IPCCSections, IPCCCommand
 from pyamihtml.ami_nlp import AmiNLP
@@ -349,7 +352,32 @@
             csv_path = Path(AR6_DIR, report, "annexes", "html", "glossary", "links.csv")
             if not(csv_path.exists()):
                 logger.error(f"file does not exist {csv_path}")
                 continue
             ami_nlp = AmiNLP()
             ami_nlp.find_text_similarities(csv_path, maxt=1000, min_sim=0.25, omit_dict=omit_dict)
 
+    def test_distance_matrix(self):
+        """
+        """
+
+        omit_dict = {
+            A_TEXT: 'See |see ',
+            T_TEXT: 'See |see ',
+        }
+        duplicates = [A_TEXT]
+        n_clusters = 25
+        random_state = 42
+        for report in REPORTS:
+            csv_path = Path(AR6_DIR, report, "annexes", "html", "glossary", "links.csv")
+            print(f"\n==========================={report}========================")
+
+            if not(csv_path.exists()):
+                logger.error(f"file does not exist {csv_path}")
+                continue
+            ami_nlp = AmiNLP()
+            ami_nlp.read_csv_remove_duplicates_and_unwanted_values(csv_path, omit_dict, duplicates=duplicates)
+            texts = ami_nlp.data[A_TEXT]
+            print(f"texts: ++++++ {len(texts)} ++++++ {texts}")
+            ami_nlp.calculate_distance_matrices(texts, omit_dict=omit_dict, n_clusters=n_clusters, random_state=random_state)
+
+
```

### Comparing `pyamihtml-0.0.5/test/test_pdf.py` & `pyamihtml-0.0.6/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_pyamix.py` & `pyamihtml-0.0.6/test/test_pyamix.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_svg.py` & `pyamihtml-0.0.6/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_util.py` & `pyamihtml-0.0.6/test/test_util.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_wikidata.py` & `pyamihtml-0.0.6/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.5/test/test_xml.py` & `pyamihtml-0.0.6/test/test_xml.py`

 * *Files identical despite different names*

