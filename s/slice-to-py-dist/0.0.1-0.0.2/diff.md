# Comparing `tmp/slice_to_py_dist-0.0.1.tar.gz` & `tmp/slice_to_py_dist-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slice_to_py_dist-0.0.1.tar", max compression
+gzip compressed data, was "slice_to_py_dist-0.0.2.tar", max compression
```

## Comparing `slice_to_py_dist-0.0.1.tar` & `slice_to_py_dist-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1099 2023-07-06 03:31:07.198116 slice_to_py_dist-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6279 2023-07-07 02:59:42.360299 slice_to_py_dist-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-04 04:30:11.675500 slice_to_py_dist-0.0.1/slice_to_py_dist/__init__.py
--rw-r--r--   0        0        0     3083 2023-07-06 04:56:29.003197 slice_to_py_dist-0.0.1/slice_to_py_dist/__main__.py
--rw-r--r--   0        0        0     4708 2023-07-06 04:27:26.959220 slice_to_py_dist-0.0.1/slice_to_py_dist/build_sdist.py
--rw-r--r--   0        0        0     2453 2023-07-06 04:10:24.467371 slice_to_py_dist-0.0.1/slice_to_py_dist/custom_build_backend/backend.py
--rw-r--r--   0        0        0      235 2023-07-05 05:00:12.037048 slice_to_py_dist-0.0.1/slice_to_py_dist/types.py
--rw-r--r--   0        0        0      852 2023-07-06 03:54:13.948132 slice_to_py_dist-0.0.1/slice_to_py_dist/utils.py
--rw-r--r--   0        0        0     6924 1970-01-01 00:00:00.000000 slice_to_py_dist-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-07 04:51:53.375211 slice_to_py_dist-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6375 2023-07-07 04:37:53.628479 slice_to_py_dist-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 04:30:11.675500 slice_to_py_dist-0.0.2/slice_to_py_dist/__init__.py
+-rw-r--r--   0        0        0     3083 2023-07-06 04:56:29.003197 slice_to_py_dist-0.0.2/slice_to_py_dist/__main__.py
+-rw-r--r--   0        0        0     4628 2023-07-07 04:49:40.793768 slice_to_py_dist-0.0.2/slice_to_py_dist/build_sdist.py
+-rw-r--r--   0        0        0     2453 2023-07-06 04:10:24.467371 slice_to_py_dist-0.0.2/slice_to_py_dist/custom_build_backend/backend.py
+-rw-r--r--   0        0        0      235 2023-07-05 05:00:12.037048 slice_to_py_dist-0.0.2/slice_to_py_dist/types.py
+-rw-r--r--   0        0        0      852 2023-07-06 03:54:13.948132 slice_to_py_dist-0.0.2/slice_to_py_dist/utils.py
+-rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 slice_to_py_dist-0.0.2/PKG-INFO
```

### Comparing `slice_to_py_dist-0.0.1/pyproject.toml` & `slice_to_py_dist-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slice_to_py_dist"
-version = "0.0.1"
+version = "0.0.2"
 description = "Put a set of ZeroC/ICE slice files (.ice) into python distribution package."
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 configargparse = "^1.5.5"
```

### Comparing `slice_to_py_dist-0.0.1/README.md` & `slice_to_py_dist-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,35 +17,34 @@
 соответствующие модулям верхнего уровня в Slice описаниях. Эти импортируемые python-пакеты и будут
 установлены в целевом python-окружении.
 
 Запуск компиляции Slice файлов на этапе установки sdist-пакета производится из специализированного
 бэкенда сборки (*build-backend*), который добавляется в sdist-пакет при его формировании. Бэкенд
 сборки использует технологию *in-tree backend* (см. ссылки).
 
-## Установка
-```
-python -m venv .venv
-.venv/bin/python -m pip install slice_to_py_dist
-```
-
 ## Пример
 Для примера будет использоваться каталог `tests/funnycat/data`, который содержит:
 - подкаталог `slice` со Slice файлами,
 - конфигурационный файл `config.toml`.
 
-Упаковка Slice файлов в sdist пакет:
+Установка `slice_to_py_dist` и запуск для упаковки Slice файлов в sdist пакет:
 ```
-datadir=tests/funnycat/data
-.venv/bin/python -m slice_to_py_dist -c $datadir/config.toml --slice-source-dir $datadir/slice
+$ python -m venv .venv
+$ source .venv/bin/activate
+(.venv) $ pip install slice_to_py_dist
+
+(.venv) $ datadir=tests/funnycat/data
+(.venv) $ python -m slice_to_py_dist -c $datadir/config.toml --slice-source-dir $datadir/slice
 ```
 (Опции, указанные в конфигурационном файле, могут быть указаны и в командной строке. И наоборот,
 опция `--slice-source-dir` также может быть указана в конфигурационном файле. Для разбора опций
 используется pypi-пакет configargparse).
 
-После выполнения команды должен появиться sdist пакет, например `funnycat-0.0.2.tar.gz`.
+После выполнения команды в текущем каталоге должен появиться sdist пакет, например
+`funnycat-0.0.2.tar.gz`.
 
 При установке sdist пакета в целевом python-окружении выполняется компиляция Slice файлов и
 появляются следующие импортируемые python-пакеты:
 - `FunnyCat`
 - `FunnyCatSupport`
 - `funnycat_gen`
 - `funnycat_slice`
```

### Comparing `slice_to_py_dist-0.0.1/slice_to_py_dist/__main__.py` & `slice_to_py_dist-0.0.2/slice_to_py_dist/__main__.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.0.1/slice_to_py_dist/build_sdist.py` & `slice_to_py_dist-0.0.2/slice_to_py_dist/build_sdist.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     build_dir: Path, slice_source_dir: Path, slice_storage_package: str, dist_info: DistPackageInfo
 ) -> None:
     # Find input slice files.
     slice_source_dir = expand_path(slice_source_dir)
     slice_files = find_slice_files(slice_source_dir)
     print(f"Found {len(slice_files)} slice files in {str(slice_source_dir)}")
 
-    # Copy the directory of the custom build backend, also find backend module in it.
+    # Copy the directory of the custom build backend, also check backend module in it.
     backend_dir_src = Path(__file__).parent / BACKEND_DIR
     backend_module = backend_dir_src / BACKEND_MODULE
     if not backend_module.exists():
         raise SliceToPyDistError(f"prepare_build_dir: missing the module: {backend_module}")
     backend_dir_dest = build_dir / BACKEND_DIR
     shutil.copytree(backend_dir_src, backend_dir_dest)
 
@@ -99,28 +99,25 @@
         )
 
 
 def build_sdist(slice_source_dir: str, slice_storage_package: str, dist_info: DistPackageInfo) -> None:
     with tempfile.TemporaryDirectory() as build_dir:
         build_dir = Path(build_dir)
 
+        print("Preparing temporary build directory...")
         prepare_build_dir(build_dir, Path(slice_source_dir), slice_storage_package, dist_info)
 
-        # Build the sdist package.
+        print("Building the sdist package...")
         args = "python -m build --sdist".split()
         shell = True  # Required to select an interpreter related to the venv
-        completed = subprocess.run(args, shell=shell, capture_output=True, cwd=build_dir, check=False)
+        completed = subprocess.run(args, shell=shell, cwd=build_dir, check=False)
         if completed.returncode != 0:
-            raise SliceToPyDistError(
-                f"build --sdist failed with code {completed.returncode}\n"
-                f"stdout is:\n{completed.stdout.decode()}\n"
-                f"stderr is:\n{completed.stderr.decode()}"
-            )
+            raise SliceToPyDistError(f"'python -m build --sdist' failed with code {completed.returncode}")
 
-        # Copy the newly built sdist to the current directory.
+        print("Copying the newly built sdist to the current directory...")
         dist_dir = build_dir / "dist"
         dist_files = [p.relative_to(dist_dir) for p in dist_dir.glob("*.tar.gz")]
         if len(dist_files) == 0:
             raise SliceToPyDistError(f"Can't find newly built sdist files under {dist_dir.absolute()}")
         for rel_path in dist_files:
             print(rel_path)
             shutil.copyfile(dist_dir / rel_path, Path(".") / rel_path)
```

### Comparing `slice_to_py_dist-0.0.1/slice_to_py_dist/custom_build_backend/backend.py` & `slice_to_py_dist-0.0.2/slice_to_py_dist/custom_build_backend/backend.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.0.1/slice_to_py_dist/utils.py` & `slice_to_py_dist-0.0.2/slice_to_py_dist/utils.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.0.1/PKG-INFO` & `slice_to_py_dist-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slice-to-py-dist
-Version: 0.0.1
+Version: 0.0.2
 Summary: Put a set of ZeroC/ICE slice files (.ice) into python distribution package.
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -34,35 +34,34 @@
 соответствующие модулям верхнего уровня в Slice описаниях. Эти импортируемые python-пакеты и будут
 установлены в целевом python-окружении.
 
 Запуск компиляции Slice файлов на этапе установки sdist-пакета производится из специализированного
 бэкенда сборки (*build-backend*), который добавляется в sdist-пакет при его формировании. Бэкенд
 сборки использует технологию *in-tree backend* (см. ссылки).
 
-## Установка
-```
-python -m venv .venv
-.venv/bin/python -m pip install slice_to_py_dist
-```
-
 ## Пример
 Для примера будет использоваться каталог `tests/funnycat/data`, который содержит:
 - подкаталог `slice` со Slice файлами,
 - конфигурационный файл `config.toml`.
 
-Упаковка Slice файлов в sdist пакет:
+Установка `slice_to_py_dist` и запуск для упаковки Slice файлов в sdist пакет:
 ```
-datadir=tests/funnycat/data
-.venv/bin/python -m slice_to_py_dist -c $datadir/config.toml --slice-source-dir $datadir/slice
+$ python -m venv .venv
+$ source .venv/bin/activate
+(.venv) $ pip install slice_to_py_dist
+
+(.venv) $ datadir=tests/funnycat/data
+(.venv) $ python -m slice_to_py_dist -c $datadir/config.toml --slice-source-dir $datadir/slice
 ```
 (Опции, указанные в конфигурационном файле, могут быть указаны и в командной строке. И наоборот,
 опция `--slice-source-dir` также может быть указана в конфигурационном файле. Для разбора опций
 используется pypi-пакет configargparse).
 
-После выполнения команды должен появиться sdist пакет, например `funnycat-0.0.2.tar.gz`.
+После выполнения команды в текущем каталоге должен появиться sdist пакет, например
+`funnycat-0.0.2.tar.gz`.
 
 При установке sdist пакета в целевом python-окружении выполняется компиляция Slice файлов и
 появляются следующие импортируемые python-пакеты:
 - `FunnyCat`
 - `FunnyCatSupport`
 - `funnycat_gen`
 - `funnycat_slice`
```

