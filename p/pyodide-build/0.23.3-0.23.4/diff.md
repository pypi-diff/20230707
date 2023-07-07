# Comparing `tmp/pyodide-build-0.23.3.tar.gz` & `tmp/pyodide-build-0.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-build-0.23.3.tar", last modified: Sun Jun 18 02:24:12 2023, max compression
+gzip compressed data, was "pyodide-build-0.23.4.tar", last modified: Fri Jul  7 07:32:14 2023, max compression
```

## Comparing `pyodide-build-0.23.3.tar` & `pyodide-build-0.23.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.486356 pyodide-build-0.23.3/pyodide_build/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/_f2c_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/_py_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27665 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/buildall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30522 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/buildpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/build_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/create_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/py_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/create_pypa_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/create_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/install_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8595 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/mkpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/out_of_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/pypabuild.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20853 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/pywasmcross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/pyzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tests/replace_so_abi_tags_test_package/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/tests/replace_so_abi_tags_test_package/mypkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/tests/replace_so_abi_tags_test_package/mypkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tools/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/Platform/
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/tools/pyo3_config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.119787 pyodide-build-0.23.4/pyodide_build/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/_f2c_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/_py_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27665 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/buildall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30522 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/buildpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.123787 pyodide-build-0.23.4/pyodide_build/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/build_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/create_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/py_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/cli/xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/create_pypa_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/create_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/install_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8595 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/mkpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/pyodide_build/out_of_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/out_of_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/out_of_tree/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/out_of_tree/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/out_of_tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/out_of_tree/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/pypabuild.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20853 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/pywasmcross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/pyzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.107787 pyodide-build-0.23.4/pyodide_build/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.107787 pyodide-build-0.23.4/pyodide_build/tests/replace_so_abi_tags_test_package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/pyodide_build/tests/replace_so_abi_tags_test_package/mypkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/tests/replace_so_abi_tags_test_package/mypkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/pyodide_build/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.111787 pyodide-build-0.23.4/pyodide_build/tools/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.111787 pyodide-build-0.23.4/pyodide_build/tools/cmake/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/pyodide_build/tools/cmake/Modules/Platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyodide_build/tools/pyo3_config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/pyodide_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-07 07:32:14.000000 pyodide-build-0.23.4/pyodide_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-07 07:32:14.000000 pyodide-build-0.23.4/pyodide_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:32:14.000000 pyodide-build-0.23.4/pyodide_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 07:32:14.000000 pyodide-build-0.23.4/pyodide_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-07 07:32:14.000000 pyodide-build-0.23.4/pyodide_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 07:32:14.000000 pyodide-build-0.23.4/pyodide_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-07 07:32:14.127788 pyodide-build-0.23.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 07:31:57.000000 pyodide-build-0.23.4/setup.py
```

### Comparing `pyodide-build-0.23.3/LICENSE` & `pyodide-build-0.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/PKG-INFO` & `pyodide-build-0.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-build
-Version: 0.23.3
+Version: 0.23.4
 Summary: "Tools for building Pyodide"
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyodide-build-0.23.3/pyodide_build/__main__.py` & `pyodide-build-0.23.4/pyodide_build/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/_f2c_fixes.py` & `pyodide-build-0.23.4/pyodide_build/_f2c_fixes.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/_py_compile.py` & `pyodide-build-0.23.4/pyodide_build/_py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/buildall.py` & `pyodide-build-0.23.4/pyodide_build/buildall.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/buildpkg.py` & `pyodide-build-0.23.4/pyodide_build/buildpkg.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/cli/build.py` & `pyodide-build-0.23.4/pyodide_build/cli/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 import re
 import shutil
 import sys
 import tempfile
 from pathlib import Path
-from typing import Optional
+from typing import Optional, cast, get_args
 from urllib.parse import urlparse
 
 import requests
 import typer
 
 from .. import common
+from ..io import _BuildSpecExports, _ExportTypes
+from ..logger import logger
 from ..out_of_tree import build
 from ..out_of_tree.pypi import (
     build_dependencies_for_wheel,
     build_wheels_from_pypi_requirements,
     fetch_pypi_package,
 )
 from ..out_of_tree.utils import initialize_pyodide_root
 
 
+def convert_exports(exports: str) -> _BuildSpecExports:
+    if "," in exports:
+        return [x.strip() for x in exports.split(",") if x.strip()]
+    possible_exports = get_args(_ExportTypes)
+    if exports in possible_exports:
+        return cast(_ExportTypes, exports)
+    logger.stderr(
+        f"Expected exports to be one of "
+        '"pyinit", "requested", "whole_archive", '
+        "or a comma separated list of symbols to export. "
+        f'Got "{exports}".'
+    )
+    sys.exit(1)
+
+
 def pypi(
     package: str,
     output_directory: Path,
     exports: str = typer.Option(
         "requested",
+        envvar="PYODIDE_BUILD_EXPORTS",
         help="Which symbols should be exported when linking .so files?",
     ),
     ctx: typer.Context = typer.Context,
 ) -> Path:
     """Fetch a wheel from pypi, or build from source if none available."""
     initialize_pyodide_root()
     common.check_emscripten_version()
@@ -40,15 +58,17 @@
         if not package_path.is_dir():
             # a pure-python wheel has been downloaded - just copy to dist folder
             dest_file = output_directory / package_path.name
             shutil.copyfile(str(package_path), output_directory / package_path.name)
             print(f"Successfully fetched: {package_path.name}")
             return dest_file
 
-        built_wheel = build.run(srcdir, output_directory, exports, backend_flags)
+        built_wheel = build.run(
+            srcdir, output_directory, convert_exports(exports), backend_flags
+        )
         return built_wheel
 
 
 def download_url(url: str, output_directory: Path) -> str:
     with requests.get(url, stream=True) as response:
         urlpath = Path(urlparse(response.url).path)
         if urlpath.suffix == ".gz":
@@ -61,14 +81,15 @@
 
 
 def url(
     package_url: str,
     output_directory: Path,
     exports: str = typer.Option(
         "requested",
+        envvar="PYODIDE_BUILD_EXPORTS",
         help="Which symbols should be exported when linking .so files?",
     ),
     ctx: typer.Context = typer.Context,
 ) -> Path:
     """Fetch a wheel or build sdist from url."""
     initialize_pyodide_root()
     common.check_emscripten_version()
@@ -82,40 +103,47 @@
 
         builddir = tmppath / "build"
         shutil.unpack_archive(tmppath / filename, builddir)
         files = list(builddir.iterdir())
         if len(files) == 1 and files[0].is_dir():
             # unzipped into subfolder
             builddir = files[0]
-        wheel_path = build.run(builddir, output_directory, exports, backend_flags)
+        wheel_path = build.run(
+            builddir, output_directory, convert_exports(exports), backend_flags
+        )
         return wheel_path
 
 
 def source(
     source_location: Path,
     output_directory: Path,
     exports: str = typer.Option(
         "requested",
+        envvar="PYODIDE_BUILD_EXPORTS",
         help="Which symbols should be exported when linking .so files?",
     ),
     ctx: typer.Context = typer.Context,
 ) -> Path:
     """Use pypa/build to build a Python package from source"""
     initialize_pyodide_root()
     common.check_emscripten_version()
     backend_flags = ctx.args
-    built_wheel = build.run(source_location, output_directory, exports, backend_flags)
+    built_wheel = build.run(
+        source_location, output_directory, convert_exports(exports), backend_flags
+    )
     return built_wheel
 
 
 # simple 'pyodide build' command
 def main(
     source_location: "Optional[str]" = typer.Argument(
         "",
-        help="Build source, can be source folder, pypi version specification, or url to a source dist archive or wheel file. If this is blank, it will build the current directory.",
+        help="Build source, can be source folder, pypi version specification, "
+        "or url to a source dist archive or wheel file. If this is blank, it "
+        "will build the current directory.",
     ),
     output_directory: str = typer.Option(
         "",
         "--outdir",
         "-o",
         help="which directory should the output be placed into?",
     ),
@@ -124,26 +152,28 @@
         "",
         "--requirements",
         "-r",
         help="Build a list of package requirements from a requirements.txt file",
     ),
     exports: str = typer.Option(
         "requested",
+        envvar="PYODIDE_BUILD_EXPORTS",
         help="Which symbols should be exported when linking .so files?",
     ),
     build_dependencies: bool = typer.Option(
         False, help="Fetch non-pyodide dependencies from pypi and build them too."
     ),
     output_lockfile: str = typer.Option(
         "",
         help="Output list of resolved dependencies to a file in requirements.txt format",
     ),
     skip_dependency: list[str] = typer.Option(
         [],
-        help="Skip building or resolving a single dependency. Use multiple times or provide a comma separated list to skip multiple dependencies.",
+        help="Skip building or resolving a single dependency. "
+        "Use multiple times or provide a comma separated list to skip multiple dependencies.",
     ),
     compression_level: int = typer.Option(
         6, help="Compression level to use for the created zip file"
     ),
     ctx: typer.Context = typer.Context,
 ) -> None:
     """Use pypa/build to build a Python package from source, pypi or url."""
@@ -187,15 +217,17 @@
                 reqs.append(x)
         try:
             build_wheels_from_pypi_requirements(
                 reqs,
                 outpath,
                 build_dependencies,
                 skip_dependency,
-                exports,
+                # TODO: should we really use same "exports" value for all of our
+                # dependencies? Not sure this makes sense...
+                convert_exports(exports),
                 ctx.args,
                 output_lockfile=output_lockfile,
             )
         except BaseException as e:
             import traceback
 
             print("Failed building multiple wheels:", traceback.format_exc())
@@ -222,15 +254,17 @@
     # now build deps for wheel
     if build_dependencies:
         try:
             build_dependencies_for_wheel(
                 wheel,
                 extras,
                 skip_dependency,
-                exports,
+                # TODO: should we really use same "exports" value for all of our
+                # dependencies? Not sure this makes sense...
+                convert_exports(exports),
                 ctx.args,
                 output_lockfile=output_lockfile,
                 compression_level=compression_level,
             )
         except BaseException as e:
             import traceback
```

### Comparing `pyodide-build-0.23.3/pyodide_build/cli/build_recipes.py` & `pyodide-build-0.23.4/pyodide_build/cli/build_recipes.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/cli/config.py` & `pyodide-build-0.23.4/pyodide_build/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/cli/create_zipfile.py` & `pyodide-build-0.23.4/pyodide_build/cli/create_zipfile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/cli/py_compile.py` & `pyodide-build-0.23.4/pyodide_build/cli/py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/cli/skeleton.py` & `pyodide-build-0.23.4/pyodide_build/cli/skeleton.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/cli/xbuildenv.py` & `pyodide-build-0.23.4/pyodide_build/cli/xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/common.py` & `pyodide-build-0.23.4/pyodide_build/common.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/create_pypa_index.py` & `pyodide-build-0.23.4/pyodide_build/create_pypa_index.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/create_xbuildenv.py` & `pyodide-build-0.23.4/pyodide_build/create_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/install_xbuildenv.py` & `pyodide-build-0.23.4/pyodide_build/install_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/io.py` & `pyodide-build-0.23.4/pyodide_build/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,22 +71,23 @@
                 "If source is a wheel, 'source/patches' and 'source/extras' "
                 "keys are not allowed"
             )
 
         return values
 
 
-_BuildSpecExports = Literal["pyinit", "requested", "whole_archive"]
+_ExportTypes = Literal["pyinit", "requested", "whole_archive"]
+_BuildSpecExports = _ExportTypes | list[str]
 _BuildSpecTypes = Literal[
     "package", "static_library", "shared_library", "cpython_module"
 ]
 
 
 class _BuildSpec(BaseModel):
-    exports: _BuildSpecExports | list[_BuildSpecExports] = "pyinit"
+    exports: _BuildSpecExports = "pyinit"
     backend_flags: str = Field("", alias="backend-flags")
     cflags: str = ""
     cxxflags: str = ""
     ldflags: str = ""
     package_type: _BuildSpecTypes = Field("package", alias="type")
     cross_script: str | None = Field(None, alias="cross-script")
     script: str | None = None
```

### Comparing `pyodide-build-0.23.3/pyodide_build/logger.py` & `pyodide-build-0.23.4/pyodide_build/logger.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/mkpkg.py` & `pyodide-build-0.23.4/pyodide_build/mkpkg.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/out_of_tree/build.py` & `pyodide-build-0.23.4/pyodide_build/out_of_tree/build.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 from pathlib import Path
-from typing import Any
 
 from .. import common, pypabuild
+from ..io import _BuildSpecExports
 
 
-def run(srcdir: Path, outdir: Path, exports: Any, args: list[str]) -> Path:
+def run(
+    srcdir: Path, outdir: Path, exports: _BuildSpecExports, args: list[str]
+) -> Path:
     outdir = outdir.resolve()
     cflags = common.get_make_flag("SIDE_MODULE_CFLAGS")
     cflags += f" {os.environ.get('CFLAGS', '')}"
     cxxflags = common.get_make_flag("SIDE_MODULE_CXXFLAGS")
     cxxflags += f" {os.environ.get('CXXFLAGS', '')}"
     ldflags = common.get_make_flag("SIDE_MODULE_LDFLAGS")
     ldflags += f" {os.environ.get('LDFLAGS', '')}"
```

### Comparing `pyodide-build-0.23.3/pyodide_build/out_of_tree/pypi.py` & `pyodide-build-0.23.4/pyodide_build/out_of_tree/pypi.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from resolvelib import BaseReporter, Resolver
 from resolvelib.providers import AbstractProvider
 from unearth.evaluator import TargetPython
 from unearth.finder import PackageFinder
 
 from .. import common
 from ..common import repack_zip_archive
+from ..io import _BuildSpecExports
 from ..logger import logger
 from . import build
 
 _PYPI_INDEX = ["https://pypi.org/simple/"]
 _PYPI_TRUSTED_HOSTS = ["pypi.org"]
 
 
@@ -231,15 +232,15 @@
     # If we didn't find the metadata, return an empty dict
     return EmailMessage()
 
 
 class PyPIProvider(APBase):
     BUILD_FLAGS: list[str] = []
     BUILD_SKIP: list[str] = []
-    BUILD_EXPORTS: str = ""
+    BUILD_EXPORTS: _BuildSpecExports = []
 
     def __init__(self, build_dependencies: bool):
         self.build_dependencies = build_dependencies
 
     def identify(self, requirement_or_candidate):
         base = canonicalize_name(requirement_or_candidate.name)
         return base
@@ -372,15 +373,15 @@
 
 
 def build_wheels_from_pypi_requirements(
     reqs: list[str],
     target_folder: Path,
     build_dependencies: bool,
     skip_dependency: list[str],
-    exports: str,
+    exports: _BuildSpecExports,
     build_flags: list[str],
     output_lockfile: str | None,
 ) -> None:
     """
     Given a list of package requirements, build or fetch them. If build_dependencies is true, then
     package dependencies will be built or fetched also.
     """
@@ -396,15 +397,15 @@
     )
 
 
 def build_dependencies_for_wheel(
     wheel: Path,
     extras: list[str],
     skip_dependency: list[str],
-    exports: str,
+    exports: _BuildSpecExports,
     build_flags: list[str],
     output_lockfile: str | None,
     compression_level: int = 6,
 ) -> None:
     """Extract dependencies from this wheel and build pypi dependencies
     for each one in ./dist/
```

### Comparing `pyodide-build-0.23.3/pyodide_build/out_of_tree/utils.py` & `pyodide-build-0.23.4/pyodide_build/out_of_tree/utils.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/out_of_tree/venv.py` & `pyodide-build-0.23.4/pyodide_build/out_of_tree/venv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/pypabuild.py` & `pyodide-build-0.23.4/pyodide_build/pypabuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     env: dict[str, str],
     *,
     pkgname: str,
     cflags: str,
     cxxflags: str,
     ldflags: str,
     target_install_dir: str,
-    exports: _BuildSpecExports | list[_BuildSpecExports],
+    exports: _BuildSpecExports,
 ) -> Iterator[dict[str, str]]:
     """
     Returns a dict of environment variables that should be used when building
     a package with pypa/build.
     """
 
     kwargs = dict(
```

### Comparing `pyodide-build-0.23.3/pyodide_build/pywasmcross.py` & `pyodide-build-0.23.4/pyodide_build/pywasmcross.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/pyzip.py` & `pyodide-build-0.23.4/pyodide_build/pyzip.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/recipe.py` & `pyodide-build-0.23.4/pyodide_build/recipe.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/serve.py` & `pyodide-build-0.23.4/pyodide_build/serve.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake` & `pyodide-build-0.23.4/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,36 @@
   message(FATAL_ERROR "Failed to find emscripten root directory with command \"em-config EMSCRIPTEN_ROOT\"! Process returned with error code ${_emcache_result}.")
 endif()
 
 file(TO_CMAKE_PATH "${_emconfig_output}" _emcache_output)
 set(EMSCRIPTEN_CMAKE_TOOLCHAIN_FILE "${_emconfig_output}/cmake/Modules/Platform/Emscripten.cmake" CACHE FILEPATH "Path to Emscripten CMake toolchain file.")
 include("${EMSCRIPTEN_CMAKE_TOOLCHAIN_FILE}")
 
+# From Emscripten 3.1.33, CACHE property was removed from these variables,
+# so it is not possible to overwrite them by -D<var>=<value>.
+# See: https://github.com/emscripten-core/emscripten/pull/18764
+# But we need to do it, so set them again here...
+unset(CMAKE_C_COMPILER)
+unset(CMAKE_CXX_COMPILER)
+unset(CMAKE_AR)
+unset(CMAKE_RANLIB)
+unset(CMAKE_C_COMPILER_AR)
+unset(CMAKE_CXX_COMPILER_AR)
+unset(CMAKE_C_COMPILER_RANLIB)
+unset(CMAKE_CXX_COMPILER_RANLIB)
+
+set(CMAKE_C_COMPILER "${EMSCRIPTEN_ROOT_PATH}/emcc${EMCC_SUFFIX}" CACHE FILEPATH "Emscripten emcc")
+set(CMAKE_CXX_COMPILER "${EMSCRIPTEN_ROOT_PATH}/em++${EMCC_SUFFIX}" CACHE FILEPATH "Emscripten em++")
+set(CMAKE_AR "${EMSCRIPTEN_ROOT_PATH}/emar${EMCC_SUFFIX}" CACHE FILEPATH "Emscripten ar")
+set(CMAKE_RANLIB "${EMSCRIPTEN_ROOT_PATH}/emranlib${EMCC_SUFFIX}" CACHE FILEPATH "Emscripten ranlib")
+set(CMAKE_C_COMPILER_AR "${CMAKE_AR}" CACHE FILEPATH "Emscripten ar")
+set(CMAKE_CXX_COMPILER_AR "${CMAKE_AR}" CACHE FILEPATH "Emscripten ar")
+set(CMAKE_C_COMPILER_RANLIB "${CMAKE_RANLIB}" CACHE FILEPATH "Emscripten ranlib")
+set(CMAKE_CXX_COMPILER_RANLIB "${CMAKE_RANLIB}" CACHE FILEPATH "Emscripten ranlib")
+
 # Note: this is False in original Emscripten toolchain,
 #       however we always want to allow build shared libs
 #       (See also: https://github.com/emscripten-core/emscripten/pull/16281)
 set_property(GLOBAL PROPERTY TARGET_SUPPORTS_SHARED_LIBS TRUE)
 
 # CMakeSystemSpecificInformation.cmake tries to include a Toolchain file from ${CMAKE_MODULE_PATH}/Platform/{CMAKE_SYSTEM_NAME}.cmake.
 # So in order to prevent CMake from loading the original Emscripten toolchain file, we need to prepend our own toolchain file.
```

### Comparing `pyodide-build-0.23.3/pyodide_build.egg-info/PKG-INFO` & `pyodide-build-0.23.4/pyodide_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-build
-Version: 0.23.3
+Version: 0.23.4
 Summary: "Tools for building Pyodide"
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyodide-build-0.23.3/pyodide_build.egg-info/SOURCES.txt` & `pyodide-build-0.23.4/pyodide_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.3/setup.cfg` & `pyodide-build-0.23.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	cython<3.0
 	ruamel.yaml
 	packaging
 	wheel
 	tomli
 	build==0.7.0
 	virtualenv
-	pydantic>=1.10.2
+	pydantic>=1.10.2,<2
 	pyodide-cli~=0.2.1
 	cmake>=3.24
 	unearth~=0.6
 	requests
 	types-requests
 	typer
 	auditwheel-emscripten~=0.0.9
```

