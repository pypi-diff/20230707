# Comparing `tmp/pycompile-0.1.6.tar.gz` & `tmp/pycompile-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompile-0.1.6.tar", max compression
+gzip compressed data, was "pycompile-0.1.7.tar", max compression
```

## Comparing `pycompile-0.1.6.tar` & `pycompile-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1074 2023-06-27 15:15:48.888388 pycompile-0.1.6/LICENSE
--rw-r--r--   0        0        0     9925 2023-06-27 15:15:48.892389 pycompile-0.1.6/README.md
--rw-r--r--   0        0        0     1565 2023-06-27 15:15:48.900389 pycompile-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      307 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/__init__.py
--rw-r--r--   0        0        0     7131 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/benchmark.py
--rw-r--r--   0        0        0        0 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/__init__.py
--rw-r--r--   0        0        0     2489 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/benchmark_cmd.py
--rw-r--r--   0        0        0     2352 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/compile_cmd.py
--rw-r--r--   0        0        0     1666 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/dry_run_cmd.py
--rw-r--r--   0        0        0      693 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/entrypoint.py
--rw-r--r--   0        0        0     2682 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/compiler_handler.py
--rw-r--r--   0        0        0        0 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/examples_benchmark.py
--rw-r--r--   0        0        0      145 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/fib.py
--rw-r--r--   0        0        0      128 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/harmonic.py
--rw-r--r--   0        0        0      441 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/sum.py
--rw-r--r--   0        0        0       97 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/test_examples.py
--rw-r--r--   0        0        0     4531 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/file_handler.py
--rw-r--r--   0        0        0     2989 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/helpers.py
--rw-r--r--   0        0        0     1341 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/logging_setup.py
--rw-r--r--   0        0        0     3209 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/wrappers.py
--rw-r--r--   0        0        0    10660 1970-01-01 00:00:00.000000 pycompile-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-07 16:50:17.956671 pycompile-0.1.7/LICENSE
+-rw-r--r--   0        0        0    10555 2023-07-07 16:50:17.956671 pycompile-0.1.7/README.md
+-rw-r--r--   0        0        0     1581 2023-07-07 16:50:17.968671 pycompile-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      515 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/__init__.py
+-rw-r--r--   0        0        0     7161 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/benchmark.py
+-rw-r--r--   0        0        0        0 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/__init__.py
+-rw-r--r--   0        0        0     2583 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/benchmark_cmd.py
+-rw-r--r--   0        0        0     2365 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/compile_cmd.py
+-rw-r--r--   0        0        0     1721 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/dry_run_cmd.py
+-rw-r--r--   0        0        0      701 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/entrypoint.py
+-rw-r--r--   0        0        0     2886 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/compiler_handler.py
+-rw-r--r--   0        0        0        0 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/examples_benchmark.py
+-rw-r--r--   0        0        0      145 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/fib.py
+-rw-r--r--   0        0        0      128 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/harmonic.py
+-rw-r--r--   0        0        0      441 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/sum.py
+-rw-r--r--   0        0        0       97 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/test_examples.py
+-rw-r--r--   0        0        0     4692 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/file_handler.py
+-rw-r--r--   0        0        0     2888 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/helpers.py
+-rw-r--r--   0        0        0     1341 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/logging_setup.py
+-rw-r--r--   0        0        0     3284 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/wrappers.py
+-rw-r--r--   0        0        0    11242 1970-01-01 00:00:00.000000 pycompile-0.1.7/PKG-INFO
```

### Comparing `pycompile-0.1.6/LICENSE` & `pycompile-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.6/README.md` & `pycompile-0.1.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,47 +9,49 @@
    |_|    |___/                    |_|
    
 """
 ```
 A CLI tool for compiling python source code using [Cython](https://cython.org/)  or
 [Nuitka](https://nuitka.net/).
 
+![PyPI](https://img.shields.io/pypi/v/pycompile)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pycompile)
+![PyPI - License](https://img.shields.io/pypi/l/pycompile)
+[![Tests](https://github.com/iplitharas/pycompile/actions/workflows/test.yaml/badge.svg)](https://github.com/iplitharas/pycompile/actions/workflows/test.yaml)
+![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycompile)
+
 
 ### Latest docs 📝
 [here](https://iplitharas.github.io/pycompile/)
 
 ## Table of contents
-1. [Local-development 💻](#local-development)
+1. [installation 🔨](#installation)
 2. [compile](#compile)
 3. [benchmark](#benchmark)
 4. [dry run](#dry-run)
+5. [Local-development 💻🏭](#local-development)
 
 
-
-### Local-development
-For local development run the following command
+### Installation 
 ```bash
-make setup-local-dev
-```
-All available `make` commands
-```bash
-make help
+pip install pycompile
 ```
 
 ### Compile
 
-| Syntax                 | Description                                                   |
-|------------------------|---------------------------------------------------------------|
-| `--input-path PATH`    | by default it will exclude any `test` and `__init__.py` files |
-| `--clean-source`       | Deletes the sources files.                                    |
-| `--keep-builds`        | Keeps the temp build files.                                   |
-| `--clean-executables`  | Deletes the shared objects (`.so`) files.                     |
-| `--engine`             | Can be `cython` or `nuitka`.                                  |
-| `--exclude-glob-paths` | Glob file patterns for excluding specific files.              |
-| `--verbose`            | Increase log messages.                                        |
+| Syntax               | Description                                               |
+|----------------------|-----------------------------------------------------------|
+| --input-path PATH    | by default it excludes any `test` and `__init__.py` files |
+| --clean-source       | Deletes the sources files.                                |
+| --keep-builds        | Keeps the temp build files.                               |
+| --clean-executables  | Deletes the shared objects (`.so`) files.                 |
+| --engine             | Can be `cython` or `nuitka`.                              |
+| --exclude-glob-paths | Glob file patterns for excluding specific files.          |
+| --verbose            | Increase log messages.                                    |
 
 ```bash
 pycompile -i your_python_files --clean-source --engine nuitka 
 ```
 
 By default, the [Cython](https://cython.org/) is being used as the default
 compiler. 
@@ -74,35 +76,50 @@
     ├── fib.cpython-310-darwin.so                      
     ├── test_fib.py                   
 ```
 
 ### Benchmark
 
 
-| Syntax                        | Description                                                   |
-|-------------------------------|---------------------------------------------------------------|
-| `--input-path PATH`           | by default it will exclude any `test` and `__init__.py` files |
-| `--engine`                    | Can be `cython`, `nuitka`, `all` or `none`.                   |
-| `--type`                      | Can be `memory` , `cpy`, or `both`                            |
-| `--verbose`                   | Increase log messages.                                        |
-| `--profile_func_pattern TEXT` | function name pattern for profiling defaults to `benchmark`   |
+| Syntax                      | Description                                                 |
+|-----------------------------|-------------------------------------------------------------|
+| --input-path PATH           | by default it excludes any `test` and `__init__.py` files   |
+| --engine                    | Can be `cython`, `nuitka`, `all` or `none`.                 |
+| --type                      | Can be `memory` , `cpy`, or `both`                          |
+| --verbose                   | Increase log messages.                                      |
+| --profile_func_pattern TEXT | function name pattern for profiling defaults to `benchmark` |
 
-For running a benchmark on  the `examples` use the following command:
+For running a benchmark on  the `input-path` use the following command:
 ```bash
-pycompile benchmark -i src/examples -vvv --engine cython
+pycompile benchmark -i src/examples -vvv
 ```
 which by default will start a `memory` and a `cpu` benchmark, starting with 
 `python` and then with `cython` and `nuitka`
 > The python package must have a `test_module.py` because both benchmark types are invoked 
 > with `pytest` runs
 
-For **memory profiling** the script will decorate all the functions in `main.py` 
+* For **memory profiling** the script will decorate all the functions in `benchmark.py` 
   with the `profile` decorator from `memory-profiler`. This is not optimal memory profiling, 
   because we don't actually `profile` the function itself, instead we profile the `caller` but it's necessary
   if we want to `profile` also the compiled code.
+  Use the `profile_func_pattern` to specify the function to be profiled in different module for example 
+  if `main` is the entrypoint under `main.py` use `--profile_func_pattern main`.
+
+Hence, the following structure are required for the `benchmark` subcommand.
+
+* For **cpu profiling** the same approached is being used, but instead of decorating the `calling functions` 
+  it `decorates` the test cases with the `benchmark` from `pytest-benchmark`.
+
+
+```text
+ module
+    ├── sample_funcs.py                        # implementation
+    ├── main.py                                # entrypoint with a `main` function, during compilation will be excluded
+    ├── test_sample_funcs.py                   # test cases
+```
 
 **Memory benchmark** using:`3.10.9 (main, Feb  2 2023, 12:59:36) [Clang 14.0.0 (clang-1400.0.29.202)`
 ```text
 Line #    Mem usage    Increment  Occurrences   Line Contents
 =============================================================
      7     49.4 MiB     49.4 MiB           1   @profile
      8                                         def samples_benchmark():
@@ -142,17 +159,14 @@
     12    225.1 MiB     38.6 MiB           1       sum_numbers()
     13    225.1 MiB      0.0 MiB           1       sum_strings()
 ```
 ```text
 3.45s call     test_examples.py::test_examples
 ```
 
-For **cpu profiling** the same approached is being used, but instead of decorating the `calling functions` 
- it `decorates` the test cases with the `benchmark` from `pytest-benchmark`.
-
 **CPU benchmark** using:`3.10.9 (main, Feb  2 2023, 12:59:36) [Clang 14.0.0 (clang-1400.0.29.202)]`
 ```text
 ------------------------------------------- benchmark: 1 tests ------------------------------------------
 Name (time in s)        Min     Max    Mean  StdDev  Median     IQR  Outliers     OPS  Rounds  Iterations
 ---------------------------------------------------------------------------------------------------------
 test_examples        3.9257  4.0640  3.9731  0.0605  3.9387  0.0917       1;0  0.2517       5           1
 ---------------------------------------------------------------------------------------------------------
@@ -189,37 +203,38 @@
 Legend:
   Outliers: 1 Standard Deviation from Mean; 1.5 IQR (InterQuartile Range) from 1st Quartile and 3rd Quartile.
   OPS: Operations Per Second, computed as 1 / Mean
 ===================================================================================================================
 24.02s call     test_examples.py::test_examples
 ```
 
-Hence, the following structure are required for the `benchmark` subcommand.
-
-```text
- module
-    ├── sample_funcs.py                        # implementation
-    ├── main.py                                # entrypoint
-    ├── test_sample_funcs.py                   # test cases
-```
-
 
 ![benchmark_cython_python.gif](data/benchmark_cython_python.gif)
 
 
 ### Dry run 
 
-| Syntax                 | Description                                                   |
-|------------------------|---------------------------------------------------------------|
-| `--input-path PATH`    | by default it will exclude any `test` and `__init__.py` files |
-| `--exclude-glob-paths` | Glob file patterns for excluding specific files.              |
-| `--verbose`            | Increase log messages.                                        |
+| Syntax               | Description                                               |
+|----------------------|-----------------------------------------------------------|
+| --input-path PATH    | by default it excludes any `test` and `__init__.py` files |
+| --exclude-glob-paths | Glob file patterns for excluding specific files.          |
+| --verbose            | Increase log messages.                                    |
 
 ```bash
 pycompile dry_run -i ./src
 ```
 
 ![dry_run.gif](data/dry_run.gif)
 
 
+### Local-development
+For local development run the following command
+```bash
+make setup-local-dev
+```
+All available `make` commands
+```bash
+make help
+```
+
+
 
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycompile)
```

### Comparing `pycompile-0.1.6/pyproject.toml` & `pycompile-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pycompile"
-version = "0.1.6"
+version = "0.1.7"
 description = "A CLI tool for compiling python"
 authors = ["iplitharas <johnplitharas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src" }
 ]
 
 [tool.poetry.dependencies]
-python = ">3.8"                       # MIT
+python = ">=3.10"                     # MIT
 click = "^8.1.3"                      # BSD-3-Clause
 tqdm = "^4.64.1"                      # MIT
 cython = "^0.29.33"                   # Apache
 nuitka = "^1.4.8"                     # Apache 2.0
 pytest-benchmark = "^4.0.0"           # BSD-2-Clause
 memory-profiler = "^0.61.0"           # BSD
 
@@ -51,14 +51,17 @@
 line_length = 80
 skip = [".gitignore", ".dockerignore" ,".env"]
 
 
 [tool.mypy]
 python_version = "3.10"
 strict_optional = true
+strict = true
+
+
```

### Comparing `pycompile-0.1.6/src/benchmark.py` & `pycompile-0.1.7/src/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from src.compiler_handler import CompilerHandler
 from src.file_handler import FileHandler
 from src.helpers import Colors, copy_files, decorate_functions, run_pytest
 
 logger = logging.getLogger(__name__)
 
 
-class Benchmark:  # pylint: disable=invalid-name
+class Benchmark:
     """
     Runs a benchmarks (memory, cpu)  with (``python``, ``Cython``, ``Nuitka``)
     on ``input_path``  files using the:
 
     * ``benchmark`` pytest fixture from ``pytest-benchmark`` framework
 
     *  ``@profile`` decorator from ``memory-profiler``.
@@ -59,15 +59,15 @@
     * this way of **memory profiling** isn't accurate (because we don't profile the
       actual python functions), and neither we can do for compiled code
       with python *profiling tools*, but it could be an indicator.
 
     * The ``test files`` are needed to be able to execute the functions with the right arguments.
     """
 
-    def __init__(self, input_path):
+    def __init__(self, input_path: Path):
         self.input_path = input_path
 
     @staticmethod
     def _compile(
         compiler: CompilerWrapper, temp_dir: Path, prof_func_name: str
     ) -> None:
         additional_exclude_patterns = [f"*{prof_func_name}.py"]
@@ -94,16 +94,18 @@
             Colors.RESET,
             test_files,
         )
 
     @staticmethod
     def mem_bench(input_path: Path, prof_func_name: str, engine: str) -> None:
         """
-        decorate all the function from the `examples path` marked as `benchmark`
-        with `@profile` decorator from `memory_profiler`
+        decorate all the function(s) from the ``input_path`` where their name match
+        the ``prof_func_name`` pattern,
+        with the ``@profile`` decorator from ``memory_profiler``.
+
         Finally, invoke pytest within.
         """
         logger.info(
             "%s Memory benchmark using:`%s` %s",
             Colors.CYAN,
             engine,
             Colors.RESET,
@@ -120,16 +122,17 @@
                 func_name_pattern=prof_func_name,
             )
             run_pytest(directory=temp_dir)
 
     @staticmethod
     def cpu_bench(input_path: Path, engine: str) -> None:
         """
-        decorate all the test functions from the `examples path`
-        with the `@benchmark_wrapper` decorator
+        decorate all the test functions from the ``input_path``
+        with the ``@benchmark_wrapper`` decorator.
+
         Finally, invoke pytest within.
         """
         logger.info(
             "%s CPU benchmark using:`%s` %s",
             Colors.CYAN,
             engine,
             Colors.RESET,
```

### Comparing `pycompile-0.1.6/src/cli/benchmark_cmd.py` & `pycompile-0.1.7/src/cli/benchmark_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 import logging
 import sys
 from pathlib import Path
 from typing import Sequence
 
 import click
 
-from src import CompilerCommands, CythonWrapper, NuitkaWrapper, setup_logging
+from src import (
+    CompilerCommands,
+    CompilerWrapper,
+    CythonWrapper,
+    NuitkaWrapper,
+    setup_logging,
+)
 from src.benchmark import Benchmark
 from src.helpers import Colors
 
 logger = logging.getLogger(__name__)
 
 
 @click.command(name="benchmark")
@@ -51,29 +57,33 @@
     "will be decorated with `@profile` from: "
     "`memory-profiler`, in addition their module needs to follow  "
     "the pattern (`something_prof_func_name.py` to be excluded from compilation).",
     type=str,
 )
 @click.option("-v", "--verbose", count=True, help="verbose level")
 def benchmark_cmd(
-    input_path: Path, engine: str, bench_type, prof_func_name, verbose: int
-):
+    input_path: Path,
+    engine: str,
+    bench_type: str,
+    prof_func_name: str,
+    verbose: int,
+) -> None:
     """
     Run a memory and cpu benchmark.
     """
     setup_logging(verbose)
     input_path = Path(input_path)
     if not input_path.is_dir():
         print(
             f"{Colors.FAIL} Benchmark input path: `{input_path}` needs to "
             f"be a directory, exiting...{Colors.RESET}"
         )
         sys.exit(1)
     benc = Benchmark(input_path=input_path)
-    compilers: Sequence = []
+    compilers: Sequence[CompilerWrapper] = []
     match engine:
         case "cython":
             compilers = [CythonWrapper(cmd=CompilerCommands.cython_bench)]
         case "nuitka":
             compilers = [NuitkaWrapper(cmd=CompilerCommands.nuitka_bench)]
         case "both":
             compilers = [
```

### Comparing `pycompile-0.1.6/src/cli/compile_cmd.py` & `pycompile-0.1.7/src/cli/compile_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,20 +66,20 @@
     flag_value=True,
     default=False,
     help="Clean final executables (.so) files",
 )
 def compile_cmd(  # pylint: disable=R0913
     input_path: Path,
     exclude_glob_paths: list[str],
-    verbose,
+    verbose: int,
     engine: str,
     clean_source: bool,
     keep_builds: bool,
     clean_executables: bool,
-):
+) -> None:
     """
     Compile the python files using `cython` or `nuitka`.
     """
     setup_logging(verbose)
 
     dir_files = FileHandler(
         input_path=input_path,
```

### Comparing `pycompile-0.1.6/src/cli/dry_run_cmd.py` & `pycompile-0.1.7/src/cli/dry_run_cmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     required=False,
     multiple=True,
     type=str,
     default=FileHandler("..").exclude_patterns,  # type: ignore[arg-type]
     help="glob files patterns of the files to be excluded, example: **/ignore_this_module.py",
 )
 @click.option("-v", "--verbose", count=True, help="verbose level")
-def dry_run_cmd(input_path: Path, exclude_glob_paths: list[str], verbose: int):
+def dry_run_cmd(
+    input_path: Path, exclude_glob_paths: list[str], verbose: int
+) -> None:
     """
     Perform a dry run.
     """
     setup_logging(verbose)
     file_handler = FileHandler(
         input_path=input_path, additional_exclude_patterns=exclude_glob_paths
     )
@@ -48,15 +50,17 @@
         return
 
     for dir_name, files in dir_files.items():
         print(f"{Colors.CYAN} {dir_name} {Colors.RESET}")
         render_files(files, is_last=False)
 
 
-def render_files(files, indent="", is_last=True):
+def render_files(
+    files: list[Path], indent: str = "", is_last: bool = True
+) -> None:
     """
     Render the output in a human-readable format.
     """
     branch = "└── " if is_last else "├── "
     indent += "    "
     for file in files:
         print(f"{indent[:-1]}{branch}{file.name}")
```

### Comparing `pycompile-0.1.6/src/cli/entrypoint.py` & `pycompile-0.1.7/src/cli/entrypoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from src.cli.compile_cmd import compile_cmd
 from src.cli.dry_run_cmd import dry_run_cmd
 
 logger = logging.getLogger(__name__)
 
 
 @click.group()
-def main():
+def main() -> None:
     r"""
                                           _ _
     _ __  _   _  ___ ___  _ __ ___  _ __ (_) | ___
    | '_ \| | | |/ __/ _ \| '_ ` _ \| '_ \| | |/ _ \
    | |_) | |_| | (_| (_) | | | | | | |_) | | |  __/
    | .__/ \__, |\___\___/|_| |_| |_| .__/|_|_|\___|
    |_|    |___/                    |_|
```

### Comparing `pycompile-0.1.6/src/compiler_handler.py` & `pycompile-0.1.7/src/compiler_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 from src.wrappers import CompilerWrapper
 
 logger = logging.getLogger(__name__)
 
 
 class CompilerHandler:
     """
-     CompilerHandler is responsible for compiling all the `.py` files using
-    `Cython` or `Nuitka`
+    CompilerHandler is responsible for compiling all the ``.py`` files using
+    ``Cython`` or ``Nuitka``
+    example usage::
+        compiler_handler = CompilerHandler(files=dir_files,compiler=compiler,
+                            clean_source=True,keep_builds=True)
+        compiler_handler.start()
     """
 
     def __init__(
         self,
         files: dict[str, list[Path]],
         compiler: CompilerWrapper,
         clean_source: bool = False,
@@ -61,16 +65,16 @@
         """
         for directory, _ in self.files.items():
             for executable in Path(directory).glob(pattern="*.so"):
                 executable.unlink(missing_ok=True)
 
     def start(self) -> None:
         """
-        For each `.py` file runs the compiler command
-        to build the final executable `.so`
+        For each ``.py`` file runs the compiler command
+        to build the final executable ``.so``
         """
         total_iterations = sum(len(files) for files in self.files.values())
         for directory, dir_files in tqdm(
             self.files.items(),
             total=total_iterations,
             ascii=True,
             desc=f"{Colors.CYAN}Compiling using: `{self.compiler}`{Colors.RESET}",
```

### Comparing `pycompile-0.1.6/src/file_handler.py` & `pycompile-0.1.7/src/file_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
 FileHandler implementation
-Note:
-`glob patterns`: `**`:   Recursively matches zero or more directories
-                         that fall under the current directory.
-                 `*` :   On Unix, will match everything except slashes.
-                         On Windows, it will avoid matching backslashes as well as slashes.
+glob patterns ::
+    **:   Recursively matches zero or more directories
+          that fall under the current directory.
+    * :   On Unix, will match everything except slashes.
+          On Windows, it will avoid matching backslashes as well as slashes.
 """
 import logging
 from collections import defaultdict
 from pathlib import Path
 from typing import Generator, Optional
 
 from src.helpers import Colors
 
 logger = logging.getLogger(__name__)
 
 
 class FileHandler:
     """
-    FileHandler is responsible for finding all the `.py` files  given
-    any `input_path`.
-    example usage: FileHandler("./my_module).start()
+    FileHandler is responsible for finding all the ``.py`` files within
+    the  ``input_path``.
+    example usage::
+       dir_files = FileHandler("./my_module").start()
     """
 
     def __init__(
         self,
         input_path: Path,
         additional_exclude_patterns: Optional[list[str]] = None,
     ):
         """
-        By default, all the `test` files and any `__init__` files are excluded
-        :param `input_path`: Should be a valid file/directory path.
-        :param `additional_exclude_patterns`: Any optional additional glob patterns.
+        By default, all the ``test`` files and any ``__init__`` files are excluded.
+
+        :param input_path: Should be a valid file/directory path.
+        :param additional_exclude_patterns: Any optional additional glob patterns.
         """
         self.input_path = input_path
-        self.exclude_patterns = additional_exclude_patterns
+        self.exclude_patterns = additional_exclude_patterns or []
 
     @property
     def input_path(self) -> Path:
         """
         Current `input path`
         """
         return self._input_path
@@ -47,34 +49,37 @@
     def input_path(self, path: Path | str) -> None:
         if Path(path).exists():
             self._input_path = Path(path)
         else:
             raise ValueError(f"Path: {Path(path)} doesn't exist...")
 
     @property
-    def exclude_patterns(self):
+    def exclude_patterns(self) -> list[str]:
         """
         Current glob exclude patterns
         """
         return self._exclude_patterns
 
     @exclude_patterns.setter
-    def exclude_patterns(self, additional_exclude_patterns: list[str] | None):
+    def exclude_patterns(
+        self, additional_exclude_patterns: list[str] | None
+    ) -> None:
         self._exclude_patterns = [
             "**/test**",
             "**/__init__.py",
         ]
 
         if additional_exclude_patterns:
             self._exclude_patterns.extend(additional_exclude_patterns)
 
     def start(self) -> dict[str, list[Path]]:
         """
-        For the given `input path` collect all valid `.py` files based on
-        the `exclude_patterns`
+        For the given ``input path`` collect all valid ``.py`` files based on
+        the ``exclude_patterns``
+
         :return: a dictionary for valid files within each directory.
         """
 
         files = defaultdict(list[Path])  # type: ignore[var-annotated]
         excluded_files = list(self._filter_files())
         logger.debug(
             "%sExcluded files: %s%s",
@@ -117,20 +122,23 @@
         else:
             for sub_dir in self.input_path.iterdir():
                 if sub_dir.is_dir():
                     yield from sub_dir.rglob(pattern="**/*.py")
 
             yield from self.input_path.glob(pattern="*.py")
 
-    def collect_with_pattern(self, pattern: str):
+    def collect_with_pattern(self, pattern: str) -> Generator[Path, None, None]:
         """
-        Collects all python files from the `input_path` where they mach
-        the `pattern`
+        Collects all python files within the ``input_path`` where they mach
+        the ``pattern``
 
+        :param pattern: str containing glob patters
+        :return: A Generator of file paths.
         """
+
         if not self.input_path.is_dir():
             yield self.input_path
         else:
             yield from (
                 file for file in self._collect_files() if file.match(pattern)
             )
```

### Comparing `pycompile-0.1.6/src/helpers.py` & `pycompile-0.1.7/src/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 """
-implementations for
-`change_dir` context manager,
-`copy_files` context manager,
-`decorate_functions`,
-`run_pytest`,
-and `run_sub_process` helper function.
+pycompile helper functions.
 """
 import ast
 import os
 import re
 import shutil
 import subprocess
 import tempfile
@@ -17,15 +12,19 @@
 from pathlib import Path
 from typing import Generator, Iterable
 
 import pytest
 
 
 @dataclass(frozen=True)
-class Colors:  # pylint: disable=missing-class-docstring
+class Colors:
+    """
+    pycompile colors
+    """
+
     HEADER = "\033[95m"
     BLUE = "\033[94m"
     CYAN = "\033[96m"
     GREEN = "\033[92m"
     WARNING = "\033[93m"
     FAIL = "\033[91m"
     RESET = "\033[0m"
@@ -45,15 +44,15 @@
         os.chdir(file_path)
         yield
     finally:
         os.chdir(current_path)
 
 
 @contextmanager
-def copy_files(from_dir: Path):
+def copy_files(from_dir: Path) -> Generator[Path, None, None]:
     """
     Copies all files at a temp directory.
     """
     with tempfile.TemporaryDirectory() as temp_dir:
         shutil.copytree(from_dir, temp_dir, dirs_exist_ok=True)
         yield Path(temp_dir)
```

### Comparing `pycompile-0.1.6/src/logging_setup.py` & `pycompile-0.1.7/src/logging_setup.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.6/src/wrappers.py` & `pycompile-0.1.7/src/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,29 @@
     nuitka = "python -m nuitka --module {}"
     nuitka_bench = "python -m nuitka --quiet --module {} 2>/dev/null"
 
 
 class CompilerWrapper(ABC):  # pylint: disable=missing-class-docstring
     @property
     @abstractmethod
-    def cmd(self):  # pylint: disable=missing-function-docstring
+    def cmd(self) -> str:  # pylint: disable=missing-function-docstring
         raise NotImplementedError("Each compiler should have a command!")
 
     @cmd.setter
-    def cmd(self, new_cmd: str):  # pylint: disable=missing-function-docstring
+    def cmd(
+        self, new_cmd: str
+    ) -> None:  # pylint: disable=missing-function-docstring
         raise NotImplementedError(
             "Each compiler should be able to set the command!"
         )
 
     @abstractmethod
-    def cleanup(
+    def cleanup(  # pylint: disable=missing-function-docstring
         self, file_path: Path
-    ):  # pylint: disable=missing-function-docstring
+    ) -> None:
         raise NotImplementedError("Each compiler should clean it's mess!")
 
 
 class CythonWrapper(CompilerWrapper):
     """
     Cython is a programming language, a superset of the Python programming language,
     designed to give C-like performance with code that is written mostly in Python with optional
@@ -43,19 +45,19 @@
     https://cython.org/
     """
 
     def __init__(self, cmd: str = CompilerCommands.cython):
         self.cmd = cmd
 
     @property
-    def cmd(self):
+    def cmd(self) -> str:
         return self._cmd
 
     @cmd.setter
-    def cmd(self, new_cmd: str):
+    def cmd(self, new_cmd: str) -> None:
         self._cmd = new_cmd
 
     def cleanup(self, file_path: Path) -> None:
         """
         Deletes the `build`directory.
         """
         build_path = file_path.parent / "build"
@@ -80,22 +82,22 @@
     https://nuitka.net/
     """
 
     def __init__(self, cmd: str = CompilerCommands.nuitka):
         self.cmd = cmd
 
     @property
-    def cmd(self):
+    def cmd(self) -> str:
         return self._cmd
 
     @cmd.setter
-    def cmd(self, new_cmd: str):
+    def cmd(self, new_cmd: str) -> None:
         self._cmd = new_cmd
 
-    def cleanup(self, file_path: Path):
+    def cleanup(self, file_path: Path) -> None:
         """
         Deletes the `build`directory alongside with the `file.pyi` temp file.
         """
         build_path = file_path.with_suffix(".build")
         if build_path.exists():
             shutil.rmtree(build_path)
         pyi_extension = file_path.with_suffix(".pyi")
```

### Comparing `pycompile-0.1.6/PKG-INFO` & `pycompile-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pycompile
-Version: 0.1.6
+Version: 0.1.7
 Summary: A CLI tool for compiling python
 License: MIT
 Author: iplitharas
 Author-email: johnplitharas@gmail.com
-Requires-Python: >3.8
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cython (>=0.29.33,<0.30.0)
 Requires-Dist: memory-profiler (>=0.61.0,<0.62.0)
 Requires-Dist: nuitka (>=1.4.8,<2.0.0)
 Requires-Dist: pytest-benchmark (>=4.0.0,<5.0.0)
@@ -30,47 +29,49 @@
    |_|    |___/                    |_|
    
 """
 ```
 A CLI tool for compiling python source code using [Cython](https://cython.org/)  or
 [Nuitka](https://nuitka.net/).
 
+![PyPI](https://img.shields.io/pypi/v/pycompile)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pycompile)
+![PyPI - License](https://img.shields.io/pypi/l/pycompile)
+[![Tests](https://github.com/iplitharas/pycompile/actions/workflows/test.yaml/badge.svg)](https://github.com/iplitharas/pycompile/actions/workflows/test.yaml)
+![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycompile)
+
 
 ### Latest docs 📝
 [here](https://iplitharas.github.io/pycompile/)
 
 ## Table of contents
-1. [Local-development 💻](#local-development)
+1. [installation 🔨](#installation)
 2. [compile](#compile)
 3. [benchmark](#benchmark)
 4. [dry run](#dry-run)
+5. [Local-development 💻🏭](#local-development)
 
 
-
-### Local-development
-For local development run the following command
+### Installation 
 ```bash
-make setup-local-dev
-```
-All available `make` commands
-```bash
-make help
+pip install pycompile
 ```
 
 ### Compile
 
-| Syntax                 | Description                                                   |
-|------------------------|---------------------------------------------------------------|
-| `--input-path PATH`    | by default it will exclude any `test` and `__init__.py` files |
-| `--clean-source`       | Deletes the sources files.                                    |
-| `--keep-builds`        | Keeps the temp build files.                                   |
-| `--clean-executables`  | Deletes the shared objects (`.so`) files.                     |
-| `--engine`             | Can be `cython` or `nuitka`.                                  |
-| `--exclude-glob-paths` | Glob file patterns for excluding specific files.              |
-| `--verbose`            | Increase log messages.                                        |
+| Syntax               | Description                                               |
+|----------------------|-----------------------------------------------------------|
+| --input-path PATH    | by default it excludes any `test` and `__init__.py` files |
+| --clean-source       | Deletes the sources files.                                |
+| --keep-builds        | Keeps the temp build files.                               |
+| --clean-executables  | Deletes the shared objects (`.so`) files.                 |
+| --engine             | Can be `cython` or `nuitka`.                              |
+| --exclude-glob-paths | Glob file patterns for excluding specific files.          |
+| --verbose            | Increase log messages.                                    |
 
 ```bash
 pycompile -i your_python_files --clean-source --engine nuitka 
 ```
 
 By default, the [Cython](https://cython.org/) is being used as the default
 compiler. 
@@ -95,35 +96,50 @@
     ├── fib.cpython-310-darwin.so                      
     ├── test_fib.py                   
 ```
 
 ### Benchmark
 
 
-| Syntax                        | Description                                                   |
-|-------------------------------|---------------------------------------------------------------|
-| `--input-path PATH`           | by default it will exclude any `test` and `__init__.py` files |
-| `--engine`                    | Can be `cython`, `nuitka`, `all` or `none`.                   |
-| `--type`                      | Can be `memory` , `cpy`, or `both`                            |
-| `--verbose`                   | Increase log messages.                                        |
-| `--profile_func_pattern TEXT` | function name pattern for profiling defaults to `benchmark`   |
+| Syntax                      | Description                                                 |
+|-----------------------------|-------------------------------------------------------------|
+| --input-path PATH           | by default it excludes any `test` and `__init__.py` files   |
+| --engine                    | Can be `cython`, `nuitka`, `all` or `none`.                 |
+| --type                      | Can be `memory` , `cpy`, or `both`                          |
+| --verbose                   | Increase log messages.                                      |
+| --profile_func_pattern TEXT | function name pattern for profiling defaults to `benchmark` |
 
-For running a benchmark on  the `examples` use the following command:
+For running a benchmark on  the `input-path` use the following command:
 ```bash
-pycompile benchmark -i src/examples -vvv --engine cython
+pycompile benchmark -i src/examples -vvv
 ```
 which by default will start a `memory` and a `cpu` benchmark, starting with 
 `python` and then with `cython` and `nuitka`
 > The python package must have a `test_module.py` because both benchmark types are invoked 
 > with `pytest` runs
 
-For **memory profiling** the script will decorate all the functions in `main.py` 
+* For **memory profiling** the script will decorate all the functions in `benchmark.py` 
   with the `profile` decorator from `memory-profiler`. This is not optimal memory profiling, 
   because we don't actually `profile` the function itself, instead we profile the `caller` but it's necessary
   if we want to `profile` also the compiled code.
+  Use the `profile_func_pattern` to specify the function to be profiled in different module for example 
+  if `main` is the entrypoint under `main.py` use `--profile_func_pattern main`.
+
+Hence, the following structure are required for the `benchmark` subcommand.
+
+* For **cpu profiling** the same approached is being used, but instead of decorating the `calling functions` 
+  it `decorates` the test cases with the `benchmark` from `pytest-benchmark`.
+
+
+```text
+ module
+    ├── sample_funcs.py                        # implementation
+    ├── main.py                                # entrypoint with a `main` function, during compilation will be excluded
+    ├── test_sample_funcs.py                   # test cases
+```
 
 **Memory benchmark** using:`3.10.9 (main, Feb  2 2023, 12:59:36) [Clang 14.0.0 (clang-1400.0.29.202)`
 ```text
 Line #    Mem usage    Increment  Occurrences   Line Contents
 =============================================================
      7     49.4 MiB     49.4 MiB           1   @profile
      8                                         def samples_benchmark():
@@ -163,17 +179,14 @@
     12    225.1 MiB     38.6 MiB           1       sum_numbers()
     13    225.1 MiB      0.0 MiB           1       sum_strings()
 ```
 ```text
 3.45s call     test_examples.py::test_examples
 ```
 
-For **cpu profiling** the same approached is being used, but instead of decorating the `calling functions` 
- it `decorates` the test cases with the `benchmark` from `pytest-benchmark`.
-
 **CPU benchmark** using:`3.10.9 (main, Feb  2 2023, 12:59:36) [Clang 14.0.0 (clang-1400.0.29.202)]`
 ```text
 ------------------------------------------- benchmark: 1 tests ------------------------------------------
 Name (time in s)        Min     Max    Mean  StdDev  Median     IQR  Outliers     OPS  Rounds  Iterations
 ---------------------------------------------------------------------------------------------------------
 test_examples        3.9257  4.0640  3.9731  0.0605  3.9387  0.0917       1;0  0.2517       5           1
 ---------------------------------------------------------------------------------------------------------
@@ -210,38 +223,39 @@
 Legend:
   Outliers: 1 Standard Deviation from Mean; 1.5 IQR (InterQuartile Range) from 1st Quartile and 3rd Quartile.
   OPS: Operations Per Second, computed as 1 / Mean
 ===================================================================================================================
 24.02s call     test_examples.py::test_examples
 ```
 
-Hence, the following structure are required for the `benchmark` subcommand.
-
-```text
- module
-    ├── sample_funcs.py                        # implementation
-    ├── main.py                                # entrypoint
-    ├── test_sample_funcs.py                   # test cases
-```
-
 
 ![benchmark_cython_python.gif](data/benchmark_cython_python.gif)
 
 
 ### Dry run 
 
-| Syntax                 | Description                                                   |
-|------------------------|---------------------------------------------------------------|
-| `--input-path PATH`    | by default it will exclude any `test` and `__init__.py` files |
-| `--exclude-glob-paths` | Glob file patterns for excluding specific files.              |
-| `--verbose`            | Increase log messages.                                        |
+| Syntax               | Description                                               |
+|----------------------|-----------------------------------------------------------|
+| --input-path PATH    | by default it excludes any `test` and `__init__.py` files |
+| --exclude-glob-paths | Glob file patterns for excluding specific files.          |
+| --verbose            | Increase log messages.                                    |
 
 ```bash
 pycompile dry_run -i ./src
 ```
 
 ![dry_run.gif](data/dry_run.gif)
 
 
+### Local-development
+For local development run the following command
+```bash
+make setup-local-dev
+```
+All available `make` commands
+```bash
+make help
+```
+
+
 
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycompile)
```

