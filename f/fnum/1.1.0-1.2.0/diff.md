# Comparing `tmp/fnum-1.1.0-py3-none-any.whl.zip` & `tmp/fnum-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5600 bytes, number of entries: 11
--rw-r--r--  2.0 unx     4010 b- defN 23-Jul-07 09:52 fnum/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-07 09:52 fnum/__main__.py
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-07 09:52 fnum/cli.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-07 09:52 fnum/exceptions.py
--rw-r--r--  2.0 unx     1896 b- defN 23-Jul-07 09:52 fnum/metadata.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1027 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/RECORD
-11 files, 10825 bytes uncompressed, 4226 bytes compressed:  61.0%
+Zip file size: 5746 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     4361 b- defN 23-Jul-07 19:43 fnum/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-07 19:43 fnum/__main__.py
+-rw-r--r--  2.0 unx     1969 b- defN 23-Jul-07 19:43 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-07 19:43 fnum/exceptions.py
+-rw-r--r--  2.0 unx     2086 b- defN 23-Jul-07 19:43 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 19:43 fnum-1.2.0.dist-info/RECORD
+11 files, 11548 bytes uncompressed, 4372 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: fnum/exceptions.py
 Comment: 
 
 Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.1.0.dist-info/LICENSE
+Filename: fnum-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.1.0.dist-info/METADATA
+Filename: fnum-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.1.0.dist-info/WHEEL
+Filename: fnum-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.1.0.dist-info/entry_points.txt
+Filename: fnum-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.1.0.dist-info/top_level.txt
+Filename: fnum-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.1.0.dist-info/RECORD
+Filename: fnum-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1,18 +1,19 @@
 from pathlib import Path
 from contextlib import contextmanager
+from imeta import ImageMetadata
 
 from .exceptions import FnumException
 from .metadata import FnumMetadata, FnumMax
 
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 
-def number_files(dirpath, suffixes, progressbar=None):
+def number_files(dirpath, suffixes, progressbar=None, include_imeta=False):
     dirpath = Path(dirpath)
 
     try:
         metadata = FnumMetadata.from_file(dirpath)
         regen_meta = False
     except FileNotFoundError:
         metadata = FnumMetadata.get_default()
@@ -63,14 +64,21 @@
             original_index = tuple(metadata.originals.values()).index(filepath.name)
             original_key = tuple(metadata.originals.keys())[original_index]
             metadata.originals[original_key] = newpath.name
         except ValueError:
             metadata.originals[filepath.name] = newpath.name
 
         filepath.rename(newpath)
+        if include_imeta:
+            metapath = Path(ImageMetadata.for_image(str(filepath)))
+            newmetapath = metapath.parents[0] / f"{newpath.stem}{metapath.suffix}"
+            try:
+                metapath.rename(newmetapath)
+            except FileNotFoundError:
+                pass
 
     for filenum in range(num, nummax + 1):
         possible_names = tuple(dirpath / f"{filenum}{suffix}" for suffix in suffixes)
         used_suffixes = tuple(
             filepath for filepath in possible_names if filepath.exists()
         )
         if len(used_suffixes) > 1:
```

## fnum/__main__.py

```diff
@@ -1,4 +1,4 @@
 from .cli import cli
 
-if __name__ == "__main__":
-    cli()
+
+cli()
```

## fnum/cli.py

```diff
@@ -3,15 +3,15 @@
 
 from . import __version__, number_files
 from .exceptions import FnumException
 
 
 @click.command(
     help="""
-Renames files in a directory to be named using sequential integers starting with 1.\n
+Renames files in a directory using sequential integers.\n
 Suffixes is a comma separated list of file extensions to rename (eg. .jpg,.gif).\n
 Dirpath is a directory to rename files in.
 """,
     context_settings={
         "help_option_names": ["-h", "--help"],
     },
 )
@@ -32,20 +32,30 @@
     help="""
 Writes a file named fnum.metadata.yaml containing data about what was changed.\n
 Max is the highest number used in a filename.\n
 Order contains a list of filenames in the order they were added. Newly added files are added to the end of the list when the command is run multiple times.\n
 Originals maps the original filenames to what they were renamed to.
     """,
 )
+@click.option(
+    "--include-imeta/--no-include-imeta",
+    default=False,
+    help="""
+Also rename image metadata files generated by imeta.
+    """,
+)
 def cli(**kwargs):
     dirpath = kwargs["dirpath"]
     suffixes = kwargs["suffixes"].split(",")
     try:
         metadata = number_files(
-            dirpath=dirpath, suffixes=suffixes, progressbar=click.progressbar
+            dirpath=dirpath,
+            suffixes=suffixes,
+            progressbar=click.progressbar,
+            include_imeta=kwargs["include_imeta"],
         )
     except FnumException as e:
         click.echo(str(e))
         sys.exit(1)
 
     if kwargs["write_max"]:
         metadata.get_max().to_file(dirpath)
```

## fnum/metadata.py

```diff
@@ -31,14 +31,21 @@
                 "max": None,
             }
         )
 
     def get_max(self):
         return FnumMax(self.max)
 
+    def contains(self, filename):
+        return (
+            filename in self.order
+            or filename in self.originals
+            or filename in self.originals.values()
+        )
+
     def __iter__(self):
         data = OrderedDict()
         for field in self._FIELDS:
             data[field] = getattr(self, field)
         for key in self._raw_data.keys():
             if key not in data:
                 data[key] = self._raw_data[key]
```

## Comparing `fnum-1.1.0.dist-info/LICENSE` & `fnum-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.1.0.dist-info/METADATA` & `fnum-1.2.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.1.0
-Summary: Renames files in a directory to be named using sequential integers starting with 1
-Author-email: Matt Wisniewski <fnum@mattw.life>
+Version: 1.2.0
+Summary: Renames files in a directory using sequential integers
+Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
-Project-URL: homepage, https://github.com/polishmatt/fnum
+Project-URL: homepage, https://github.com/healthycrowd/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
@@ -19,8 +19,9 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8.0
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: pyyaml
+Requires-Dist: imeta (~=1.1)
```

