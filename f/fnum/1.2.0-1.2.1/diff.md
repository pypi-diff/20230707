# Comparing `tmp/fnum-1.2.0-py3-none-any.whl.zip` & `tmp/fnum-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5746 bytes, number of entries: 11
--rw-r--r--  2.0 unx     4361 b- defN 23-Jul-07 19:43 fnum/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-07 19:43 fnum/__main__.py
--rw-r--r--  2.0 unx     1969 b- defN 23-Jul-07 19:43 fnum/cli.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-07 19:43 fnum/exceptions.py
--rw-r--r--  2.0 unx     2086 b- defN 23-Jul-07 19:43 fnum/metadata.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1038 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/RECORD
-11 files, 11548 bytes uncompressed, 4372 bytes compressed:  62.1%
+Zip file size: 5747 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     4363 b- defN 23-Jul-07 21:09 fnum/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-07 21:09 fnum/__main__.py
+-rw-r--r--  2.0 unx     1969 b- defN 23-Jul-07 21:09 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-07 21:09 fnum/exceptions.py
+-rw-r--r--  2.0 unx     2086 b- defN 23-Jul-07 21:09 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/RECORD
+11 files, 11550 bytes uncompressed, 4373 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: fnum/exceptions.py
 Comment: 
 
 Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.2.0.dist-info/LICENSE
+Filename: fnum-1.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.2.0.dist-info/METADATA
+Filename: fnum-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.2.0.dist-info/WHEEL
+Filename: fnum-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.2.0.dist-info/entry_points.txt
+Filename: fnum-1.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.2.0.dist-info/top_level.txt
+Filename: fnum-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.2.0.dist-info/RECORD
+Filename: fnum-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -2,15 +2,15 @@
 from contextlib import contextmanager
 from imeta import ImageMetadata
 
 from .exceptions import FnumException
 from .metadata import FnumMetadata, FnumMax
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 def number_files(dirpath, suffixes, progressbar=None, include_imeta=False):
     dirpath = Path(dirpath)
 
     try:
         metadata = FnumMetadata.from_file(dirpath)
@@ -112,15 +112,15 @@
 
     # Find new files
     files = list(dirpath.iterdir())
     if not progressbar:
 
         @contextmanager
         def noop_progressbar(*args, **kwargs):
-            yield files
+            yield args[0]
 
         progressbar = noop_progressbar
     with progressbar(files, length=len(files), label="Processing files") as bar:
         for filepath in bar:
             if not filepath.is_file() or filepath.suffix not in suffixes:
                 continue
```

## Comparing `fnum-1.2.0.dist-info/LICENSE` & `fnum-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.2.0.dist-info/METADATA` & `fnum-1.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.2.0
+Version: 1.2.1
 Summary: Renames files in a directory using sequential integers
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

## Comparing `fnum-1.2.0.dist-info/RECORD` & `fnum-1.2.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-fnum/__init__.py,sha256=x44EBjgTFHJYCDWDmSuxt3Kgs8A0AFC_OTAcTlBagVc,4361
+fnum/__init__.py,sha256=6SxEgzLCTZFYl80ZLV-hMD58-tbSslsZJF7VjpfJr5w,4363
 fnum/__main__.py,sha256=VNXCcgJ6hm4LbZBeOMBPCzuFTICAcX2m_2ThvsGiB2M,29
 fnum/cli.py,sha256=PciKbMofZDWJSLG42VW4B64KG5SxLWLxFbupp-ZR0Oo,1969
 fnum/exceptions.py,sha256=LYhcKutJUeBI2IYzIfH22L6tvt5rMz3zJSEjvoEkyAE,41
 fnum/metadata.py,sha256=pDxyFmS6NkbgINs3lsrcWQ5SSxyoos-jBF0xfXPBh7Q,2086
-fnum-1.2.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
-fnum-1.2.0.dist-info/METADATA,sha256=1jqpf-gBlV66JVGi_qRmwTydB6hwiYkt6FHhpSs1HyQ,1038
-fnum-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fnum-1.2.0.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
-fnum-1.2.0.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
-fnum-1.2.0.dist-info/RECORD,,
+fnum-1.2.1.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
+fnum-1.2.1.dist-info/METADATA,sha256=0oucHfXMuZW06bOA1qBWnixrbXL8l654QjcrYK76mcM,1038
+fnum-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fnum-1.2.1.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
+fnum-1.2.1.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
+fnum-1.2.1.dist-info/RECORD,,
```

