# Comparing `tmp/fnum-1.0.3-py3-none-any.whl.zip` & `tmp/fnum-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 16169 bytes, number of entries: 10
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 04:33 fnum/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-06 04:33 fnum/__main__.py
--rw-r--r--  2.0 unx     2699 b- defN 23-Jul-06 04:33 fnum/actions.py
--rw-r--r--  2.0 unx     1793 b- defN 23-Jul-06 04:33 fnum/cli.py
--rw-r--r--  2.0 unx    35141 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1055 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      745 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/RECORD
-10 files, 41649 bytes uncompressed, 14909 bytes compressed:  64.2%
+Zip file size: 5600 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     4010 b- defN 23-Jul-07 09:52 fnum/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-07 09:52 fnum/__main__.py
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jul-07 09:52 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-07 09:52 fnum/exceptions.py
+-rw-r--r--  2.0 unx     1896 b- defN 23-Jul-07 09:52 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1027 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 09:52 fnum-1.1.0.dist-info/RECORD
+11 files, 10825 bytes uncompressed, 4226 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: fnum/__init__.py
 Comment: 
 
 Filename: fnum/__main__.py
 Comment: 
 
-Filename: fnum/actions.py
+Filename: fnum/cli.py
 Comment: 
 
-Filename: fnum/cli.py
+Filename: fnum/exceptions.py
+Comment: 
+
+Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.0.3.dist-info/LICENSE
+Filename: fnum-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.0.3.dist-info/METADATA
+Filename: fnum-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.0.3.dist-info/WHEEL
+Filename: fnum-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.0.3.dist-info/entry_points.txt
+Filename: fnum-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.0.3.dist-info/top_level.txt
+Filename: fnum-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.0.3.dist-info/RECORD
+Filename: fnum-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1 +1,129 @@
-__version__ = "1.0.3"
+from pathlib import Path
+from contextlib import contextmanager
+
+from .exceptions import FnumException
+from .metadata import FnumMetadata, FnumMax
+
+
+__version__ = "1.1.0"
+
+
+def number_files(dirpath, suffixes, progressbar=None):
+    dirpath = Path(dirpath)
+
+    try:
+        metadata = FnumMetadata.from_file(dirpath)
+        regen_meta = False
+    except FileNotFoundError:
+        metadata = FnumMetadata.get_default()
+        regen_meta = True
+
+    num = 1
+
+    def numpath(suffix):
+        return dirpath / (str(num) + suffix)
+
+    # Find what files we already have in order
+    while used_suffixes := tuple(
+        suffix for suffix in suffixes if numpath(suffix).exists()
+    ):
+        if len(used_suffixes) > 1:
+            raise FnumException(
+                f"Unexpectedly found multiple existing files with number {num}"
+            )
+        if regen_meta:
+            filepath = numpath(used_suffixes[0])
+            metadata.order.append(filepath.name)
+            metadata.originals[filepath.name] = filepath.name
+        num += 1
+
+    # Shift down existing ordered files so new ones are added at the end
+    nummax = num - 1
+    for filepath in dirpath.iterdir():
+        if not filepath.is_file() or filepath.suffix not in suffixes:
+            continue
+
+        try:
+            filenum = int(filepath.stem)
+        except ValueError:
+            continue
+
+        if filenum > nummax:
+            nummax = filenum
+
+    def move_file(filepath):
+        newpath = numpath(filepath.suffix)
+
+        try:
+            order_index = metadata.order.index(filepath.name)
+            metadata.order[order_index] = newpath.name
+        except ValueError:
+            metadata.order.append(newpath.name)
+        try:
+            original_index = tuple(metadata.originals.values()).index(filepath.name)
+            original_key = tuple(metadata.originals.keys())[original_index]
+            metadata.originals[original_key] = newpath.name
+        except ValueError:
+            metadata.originals[filepath.name] = newpath.name
+
+        filepath.rename(newpath)
+
+    for filenum in range(num, nummax + 1):
+        possible_names = tuple(dirpath / f"{filenum}{suffix}" for suffix in suffixes)
+        used_suffixes = tuple(
+            filepath for filepath in possible_names if filepath.exists()
+        )
+        if len(used_suffixes) > 1:
+            raise FnumException(
+                f"Unexpectedly found multiple existing files with number {filenum}"
+            )
+
+        if not used_suffixes:
+            for filepath in possible_names:
+                name = filepath.name
+                if name in metadata.order or name in metadata.originals.values():
+                    try:
+                        metadata.order.remove(name)
+                    except ValueError:
+                        pass
+                    try:
+                        original_index = tuple(metadata.originals.values()).index(name)
+                        original_key = tuple(metadata.originals.keys())[original_index]
+                        del metadata.originals[original_key]
+                    except ValueError:
+                        pass
+
+                    break
+            continue
+
+        filepath = used_suffixes[0]
+        move_file(filepath)
+        num += 1
+        if int(filepath.stem) == nummax:
+            break
+
+    # Find new files
+    files = list(dirpath.iterdir())
+    if not progressbar:
+
+        @contextmanager
+        def noop_progressbar(*args, **kwargs):
+            yield files
+
+        progressbar = noop_progressbar
+    with progressbar(files, length=len(files), label="Processing files") as bar:
+        for filepath in bar:
+            if not filepath.is_file() or filepath.suffix not in suffixes:
+                continue
+
+            try:
+                if int(filepath.stem) <= num:
+                    continue
+            except ValueError:
+                pass
+
+            move_file(filepath)
+            num += 1
+
+    metadata.max = num - 1
+    return metadata
```

## fnum/cli.py

```diff
@@ -1,12 +1,12 @@
 import sys
 import click
 
-from .actions import number_files, write_max, write_metadata, FnumException
-from . import __version__
+from . import __version__, number_files
+from .exceptions import FnumException
 
 
 @click.command(
     help="""
 Renames files in a directory to be named using sequential integers starting with 1.\n
 Suffixes is a comma separated list of file extensions to rename (eg. .jpg,.gif).\n
 Dirpath is a directory to rename files in.
@@ -44,10 +44,10 @@
             dirpath=dirpath, suffixes=suffixes, progressbar=click.progressbar
         )
     except FnumException as e:
         click.echo(str(e))
         sys.exit(1)
 
     if kwargs["write_max"]:
-        write_max(dirpath, metadata)
+        metadata.get_max().to_file(dirpath)
     if kwargs["write_metadata"]:
-        write_metadata(dirpath, metadata)
+        metadata.to_file(dirpath)
```

## Comparing `fnum-1.0.3.dist-info/METADATA` & `fnum-1.1.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.0.3
+Version: 1.1.0
 Summary: Renames files in a directory to be named using sequential integers starting with 1
 Author-email: Matt Wisniewski <fnum@mattw.life>
-License: GPLv3
+License: MIT
 Project-URL: homepage, https://github.com/polishmatt/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

