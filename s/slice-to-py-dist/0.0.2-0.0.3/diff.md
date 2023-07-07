# Comparing `tmp/slice_to_py_dist-0.0.2.tar.gz` & `tmp/slice_to_py_dist-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slice_to_py_dist-0.0.2.tar", max compression
+gzip compressed data, was "slice_to_py_dist-0.0.3.tar", max compression
```

## Comparing `slice_to_py_dist-0.0.2.tar` & `slice_to_py_dist-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1099 2023-07-07 04:51:53.375211 slice_to_py_dist-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6375 2023-07-07 04:37:53.628479 slice_to_py_dist-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-04 04:30:11.675500 slice_to_py_dist-0.0.2/slice_to_py_dist/__init__.py
--rw-r--r--   0        0        0     3083 2023-07-06 04:56:29.003197 slice_to_py_dist-0.0.2/slice_to_py_dist/__main__.py
--rw-r--r--   0        0        0     4628 2023-07-07 04:49:40.793768 slice_to_py_dist-0.0.2/slice_to_py_dist/build_sdist.py
--rw-r--r--   0        0        0     2453 2023-07-06 04:10:24.467371 slice_to_py_dist-0.0.2/slice_to_py_dist/custom_build_backend/backend.py
--rw-r--r--   0        0        0      235 2023-07-05 05:00:12.037048 slice_to_py_dist-0.0.2/slice_to_py_dist/types.py
--rw-r--r--   0        0        0      852 2023-07-06 03:54:13.948132 slice_to_py_dist-0.0.2/slice_to_py_dist/utils.py
--rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 slice_to_py_dist-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-07 07:26:26.664954 slice_to_py_dist-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6376 2023-07-07 06:27:18.737532 slice_to_py_dist-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 04:30:11.675500 slice_to_py_dist-0.0.3/slice_to_py_dist/__init__.py
+-rw-r--r--   0        0        0     3083 2023-07-06 04:56:29.003197 slice_to_py_dist-0.0.3/slice_to_py_dist/__main__.py
+-rw-r--r--   0        0        0     4548 2023-07-07 06:10:58.974792 slice_to_py_dist-0.0.3/slice_to_py_dist/build_sdist.py
+-rw-r--r--   0        0        0     2419 2023-07-07 06:10:58.971815 slice_to_py_dist-0.0.3/slice_to_py_dist/custom_build_backend/backend.py
+-rw-r--r--   0        0        0      235 2023-07-05 05:00:12.037048 slice_to_py_dist-0.0.3/slice_to_py_dist/types.py
+-rw-r--r--   0        0        0      852 2023-07-06 03:54:13.948132 slice_to_py_dist-0.0.3/slice_to_py_dist/utils.py
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 slice_to_py_dist-0.0.3/PKG-INFO
```

### Comparing `slice_to_py_dist-0.0.2/pyproject.toml` & `slice_to_py_dist-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slice_to_py_dist"
-version = "0.0.2"
+version = "0.0.3"
 description = "Put a set of ZeroC/ICE slice files (.ice) into python distribution package."
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 configargparse = "^1.5.5"
```

### Comparing `slice_to_py_dist-0.0.2/README.md` & `slice_to_py_dist-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ## Пример
 Для примера будет использоваться каталог `tests/funnycat/data`, который содержит:
 - подкаталог `slice` со Slice файлами,
 - конфигурационный файл `config.toml`.
 
 Установка `slice_to_py_dist` и запуск для упаковки Slice файлов в sdist пакет:
 ```
-$ python -m venv .venv
+$ python3 -m venv .venv
 $ source .venv/bin/activate
 (.venv) $ pip install slice_to_py_dist
 
 (.venv) $ datadir=tests/funnycat/data
 (.venv) $ python -m slice_to_py_dist -c $datadir/config.toml --slice-source-dir $datadir/slice
 ```
 (Опции, указанные в конфигурационном файле, могут быть указаны и в командной строке. И наоборот,
```

### Comparing `slice_to_py_dist-0.0.2/slice_to_py_dist/__main__.py` & `slice_to_py_dist-0.0.3/slice_to_py_dist/__main__.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.0.2/slice_to_py_dist/build_sdist.py` & `slice_to_py_dist-0.0.3/slice_to_py_dist/build_sdist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import os
 import shutil
 import subprocess
 import tempfile
 from pathlib import Path
 from typing import List
 
@@ -103,19 +104,18 @@
     with tempfile.TemporaryDirectory() as build_dir:
         build_dir = Path(build_dir)
 
         print("Preparing temporary build directory...")
         prepare_build_dir(build_dir, Path(slice_source_dir), slice_storage_package, dist_info)
 
         print("Building the sdist package...")
-        args = "python -m build --sdist".split()
-        shell = True  # Required to select an interpreter related to the venv
-        completed = subprocess.run(args, shell=shell, cwd=build_dir, check=False)
+        args = f"{sys.executable} -m build --sdist".split()
+        completed = subprocess.run(args, cwd=build_dir, check=False)
         if completed.returncode != 0:
-            raise SliceToPyDistError(f"'python -m build --sdist' failed with code {completed.returncode}")
+            raise SliceToPyDistError(f"Command {args} failed with code {completed.returncode}")
 
         print("Copying the newly built sdist to the current directory...")
         dist_dir = build_dir / "dist"
         dist_files = [p.relative_to(dist_dir) for p in dist_dir.glob("*.tar.gz")]
         if len(dist_files) == 0:
             raise SliceToPyDistError(f"Can't find newly built sdist files under {dist_dir.absolute()}")
         for rel_path in dist_files:
```

### Comparing `slice_to_py_dist-0.0.2/slice_to_py_dist/custom_build_backend/backend.py` & `slice_to_py_dist-0.0.3/slice_to_py_dist/custom_build_backend/backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import os
 import subprocess
 from pathlib import Path
 from typing import List, Mapping, Optional, Union
 
 from setuptools import build_meta as orig_build_meta
 
@@ -43,19 +44,19 @@
     slice_pkg_dir = Path(".") / slice_storage_pkg_name
     slice_files_rel_paths = [p.relative_to(slice_pkg_dir) for p in slice_pkg_dir.glob(f"**/*{SLICE_SUFFIX}")]
     subprocess_cwd = slice_pkg_dir
     subprocess_output_dir = ".."
 
     # Use --underscore option to permit underscores in the Slice:
     # https://forums.zeroc.com/discussion/5923/slice-illegal-underscore-in-identifier
-    args: List[str] = f"python -m slice2py --underscore -I. --output-dir {subprocess_output_dir}".split()
+    args: List[str] = f"{sys.executable} -m slice2py --underscore -I. --output-dir {subprocess_output_dir}".split()
     args += [str(rel_path) for rel_path in slice_files_rel_paths]
-    completed = subprocess.run(args, capture_output=True, cwd=subprocess_cwd, check=False)
+    completed = subprocess.run(args, cwd=subprocess_cwd, check=False)
     if completed.returncode != 0:
-        raise BackendError(f"slice2py failed with code {completed.returncode}, stderr is: {completed.stderr.decode()}")
+        raise BackendError(f"Command {args} failed with code {completed.returncode}")
 
     # Call original setuptools function.
     return orig_build_meta.build_wheel(
         wheel_directory,
         config_settings=config_settings,
         metadata_directory=metadata_directory,
     )
```

### Comparing `slice_to_py_dist-0.0.2/slice_to_py_dist/utils.py` & `slice_to_py_dist-0.0.3/slice_to_py_dist/utils.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.0.2/PKG-INFO` & `slice_to_py_dist-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slice-to-py-dist
-Version: 0.0.2
+Version: 0.0.3
 Summary: Put a set of ZeroC/ICE slice files (.ice) into python distribution package.
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,15 +41,15 @@
 ## Пример
 Для примера будет использоваться каталог `tests/funnycat/data`, который содержит:
 - подкаталог `slice` со Slice файлами,
 - конфигурационный файл `config.toml`.
 
 Установка `slice_to_py_dist` и запуск для упаковки Slice файлов в sdist пакет:
 ```
-$ python -m venv .venv
+$ python3 -m venv .venv
 $ source .venv/bin/activate
 (.venv) $ pip install slice_to_py_dist
 
 (.venv) $ datadir=tests/funnycat/data
 (.venv) $ python -m slice_to_py_dist -c $datadir/config.toml --slice-source-dir $datadir/slice
 ```
 (Опции, указанные в конфигурационном файле, могут быть указаны и в командной строке. И наоборот,
```

