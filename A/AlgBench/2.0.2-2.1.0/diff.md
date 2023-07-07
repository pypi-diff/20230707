# Comparing `tmp/AlgBench-2.0.2.tar.gz` & `tmp/AlgBench-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgBench-2.0.2.tar", last modified: Sat Jul  1 20:32:57 2023, max compression
+gzip compressed data, was "AlgBench-2.1.0.tar", last modified: Fri Jul  7 17:00:06 2023, max compression
```

## Comparing `AlgBench-2.0.2.tar` & `AlgBench-2.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.331591 AlgBench-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.339591 AlgBench-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 20:32:45.000000 AlgBench-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-07-01 20:32:57.355591 AlgBench-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23814 2023-07-01 20:32:45.000000 AlgBench-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.343591 AlgBench-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/algbench.db.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/algbench.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/algbench.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.331591 AlgBench-2.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-01 20:32:45.000000 AlgBench-2.0.2/examples/graph_coloring/00_generate_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/01_instances.zip
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/02_run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/algbench.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/env_info/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/results/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
--rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/04_check_results.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/05_process_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/06_simplified_results.json.zip
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/07_analyze_mean.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1072992 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/08_analyze_runtime.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   397344 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/09_analyze_quality.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-01 20:32:46.000000 AlgBench-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:32:46.000000 AlgBench-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:32:57.355591 AlgBench-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.335591 AlgBench-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.351591 AlgBench-2.0.2/src/AlgBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/src/algbench/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/benchmark_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/src/algbench/db/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/nfs_json_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/nfs_json_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/nfs_json_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/stream_with_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/src/algbench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-01 20:32:46.000000 AlgBench-2.0.2/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-01 20:32:46.000000 AlgBench-2.0.2/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.888727 AlgBench-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.876726 AlgBench-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.880726 AlgBench-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 16:59:53.000000 AlgBench-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-07 17:00:06.888727 AlgBench-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24004 2023-07-07 16:59:53.000000 AlgBench-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.880726 AlgBench-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/algbench.db.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/algbench.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/algbench.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.876726 AlgBench-2.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/00_generate_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/01_instances.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/02_run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/algbench.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/env_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/04_check_results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/05_process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/06_simplified_results.json.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/07_analyze_mean.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1072992 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/08_analyze_runtime.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   397344 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/09_analyze_quality.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-07 16:59:53.000000 AlgBench-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 16:59:53.000000 AlgBench-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:00:06.888727 AlgBench-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.876726 AlgBench-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/AlgBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/algbench/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/benchmark_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/algbench/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/nfs_json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/nfs_json_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/nfs_json_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/algbench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-07 16:59:53.000000 AlgBench-2.1.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 16:59:53.000000 AlgBench-2.1.0/tests/test_logger.py
```

### Comparing `AlgBench-2.0.2/.github/workflows/pytest.yml` & `AlgBench-2.1.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/.github/workflows/release.yml` & `AlgBench-2.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/.gitignore` & `AlgBench-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/.pre-commit-config.yaml` & `AlgBench-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/.readthedocs.yaml` & `AlgBench-2.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/LICENSE` & `AlgBench-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/PKG-INFO` & `AlgBench-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 2.0.2
+Version: 2.1.0
 Summary: Util for benchmarking algorithms.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/AlgBench
 Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -635,14 +635,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
    Additionally, you can now capture loggers of the Python logging framework and save them to the database.
    This is especially useful if you use a library that uses the logging framework. Prefere ``logging`` over ``print`` for logging information.
 -  **1.1.0** Some changes for efficiency turned out to be less robust in
    case of, e.g., keyboard interrupt. Fixed that.
 -  **1.0.0** Changing the database layout, making it more efficient
```

### Comparing `AlgBench-2.0.2/README.rst` & `AlgBench-2.1.0/src/AlgBench.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: AlgBench
+Version: 2.1.0
+Summary: Util for benchmarking algorithms.
+Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
+Project-URL: Homepage, https://github.com/d-krupke/AlgBench
+Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 AlgBench: A Python-util to run benchmarks for the empirical evaluation of algorithms.
 =====================================================================================
 
 .. image:: https://img.shields.io/pypi/v/algbench.svg
    :target: https://pypi.python.org/pypi/algbench
 
 .. image:: https://img.shields.io/pypi/pyversions/algbench.svg
@@ -621,14 +635,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
    Additionally, you can now capture loggers of the Python logging framework and save them to the database.
    This is especially useful if you use a library that uses the logging framework. Prefere ``logging`` over ``print`` for logging information.
 -  **1.1.0** Some changes for efficiency turned out to be less robust in
    case of, e.g., keyboard interrupt. Fixed that.
 -  **1.0.0** Changing the database layout, making it more efficient
```

### Comparing `AlgBench-2.0.2/docs/Makefile` & `AlgBench-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/docs/algbench.db.rst` & `AlgBench-2.1.0/docs/algbench.db.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/docs/algbench.rst` & `AlgBench-2.1.0/docs/algbench.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/docs/conf.py` & `AlgBench-2.1.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,23 @@
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
 ]
+# For including __iniit__ docstrings
+autodoc_default_options = {
+    'members': True,
+    'member-order': 'bysource',
+    'special-members': '__init__',
+    'undoc-members': True,
+    'exclude-members': '__weakref__'
+}
+
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `AlgBench-2.0.2/docs/make.bat` & `AlgBench-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/00_generate_instances.py` & `AlgBench-2.1.0/examples/graph_coloring/00_generate_instances.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/02_run_benchmark.py` & `AlgBench-2.1.0/examples/graph_coloring/02_run_benchmark.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/02b_run_benchmark_with_slurminade.py` & `AlgBench-2.1.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/04_check_results.ipynb` & `AlgBench-2.1.0/examples/graph_coloring/04_check_results.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/05_process_results.py` & `AlgBench-2.1.0/examples/graph_coloring/05_process_results.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/07_analyze_mean.ipynb` & `AlgBench-2.1.0/examples/graph_coloring/07_analyze_mean.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/08_analyze_runtime.ipynb` & `AlgBench-2.1.0/examples/graph_coloring/08_analyze_runtime.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/09_analyze_quality.ipynb` & `AlgBench-2.1.0/examples/graph_coloring/09_analyze_quality.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/README.md` & `AlgBench-2.1.0/examples/graph_coloring/README.md`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/examples/graph_coloring/_utils/__init__.py` & `AlgBench-2.1.0/examples/graph_coloring/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/pyproject.toml` & `AlgBench-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/AlgBench.egg-info/PKG-INFO` & `AlgBench-2.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: AlgBench
-Version: 2.0.2
-Summary: Util for benchmarking algorithms.
-Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
-Project-URL: Homepage, https://github.com/d-krupke/AlgBench
-Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 AlgBench: A Python-util to run benchmarks for the empirical evaluation of algorithms.
 =====================================================================================
 
 .. image:: https://img.shields.io/pypi/v/algbench.svg
    :target: https://pypi.python.org/pypi/algbench
 
 .. image:: https://img.shields.io/pypi/pyversions/algbench.svg
@@ -635,14 +621,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
    Additionally, you can now capture loggers of the Python logging framework and save them to the database.
    This is especially useful if you use a library that uses the logging framework. Prefere ``logging`` over ``print`` for logging information.
 -  **1.1.0** Some changes for efficiency turned out to be less robust in
    case of, e.g., keyboard interrupt. Fixed that.
 -  **1.0.0** Changing the database layout, making it more efficient
```

### Comparing `AlgBench-2.0.2/src/AlgBench.egg-info/SOURCES.txt` & `AlgBench-2.1.0/src/AlgBench.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 examples/graph_coloring/_utils/__init__.py
 src/AlgBench.egg-info/PKG-INFO
 src/AlgBench.egg-info/SOURCES.txt
 src/AlgBench.egg-info/dependency_links.txt
 src/AlgBench.egg-info/requires.txt
 src/AlgBench.egg-info/top_level.txt
 src/algbench/__init__.py
+src/algbench/_stream_utils.py
 src/algbench/benchmark.py
 src/algbench/benchmark_db.py
 src/algbench/environment.py
 src/algbench/fingerprint.py
 src/algbench/log_capture.py
 src/algbench/pandas.py
-src/algbench/stream_with_time.py
 src/algbench/db/__init__.py
 src/algbench/db/json_serializer.py
 src/algbench/db/nfs_json_dict.py
 src/algbench/db/nfs_json_list.py
 src/algbench/db/nfs_json_set.py
 src/algbench/utils/__init__.py
 src/algbench/utils/timer.py
```

### Comparing `AlgBench-2.0.2/src/algbench/__init__.py` & `AlgBench-2.1.0/src/algbench/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/benchmark.py` & `AlgBench-2.1.0/src/algbench/benchmark.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,83 @@
 import datetime
 import inspect
 import io
 import logging
 import traceback
 import typing
+import sys
 from contextlib import ExitStack, redirect_stderr, redirect_stdout
 
 import yaml
 
 from .benchmark_db import BenchmarkDb
 from .db.json_serializer import to_json
 from .fingerprint import fingerprint
 from .log_capture import JsonLogCapture, JsonLogHandler
-from .stream_with_time import StreamWithTime
+from ._stream_utils import StreamWithTime, PrintingStringIO, NotSavingIO
 from .utils import Timer
 
 
 class Benchmark:
     """
     This is the heart of the library. It allows to run, save, and load
     a benchmark.
 
     The function `add` will run a configuration, if it is not
     already in the database. You can also split this into `check` and
     `run`. This may be advised if you want to distribute the execution.
 
     The following functions are thread-safe:
+
     - exists
     - run
     - add
     - insert
     - front
     - capture_logger
     - unlink_logger
     - __iter__
 
     Don't call any of the other functions while the benchmark is
     running. It could lead to data loss.
     """
 
-    def __init__(self, path: str, save_output_with_time: bool = True) -> None:
+    def __init__(self, path: str, save_output: bool = True, hide_output: bool = True, save_output_with_time: bool = True) -> None:
         """
         Just specify the path of where to put the
         database and everything else happens magically.
         Make sure not to use the same path for different
         databases, as they will get mixed.
 
         :param path: The path to the database.
+        :param save_output: If true, all output (stdout and stderr) will be
+            saved. If set to false, the output will be discarded. This is
+            useful if you have a lot of output and don't want to waste disk
+            space. However, you will not be able to see the output of the
+            algorithm afterwards. Note that the output can only be saved if
+            the code aquires the Python sys.stdout and sys.stderr streams
+            during the execution, as the corresponding streams are replaced
+            by the benchmark. Normal ``print`` statements do so, but
+            ``logging.StreamHandler`` does not. For the latter, use
+            ``Benchmark.capture_logger``.
+        :param hide_output: If true, all output (stdout and stderr) will be
+            hidden. This is useful if you have a lot of output and don't want
+            to clutter your console. However, you will not be able to see the
+            output of the algorithm while it is running. Code the aquired handles
+            to the Python sys.stdout and sys.stderr streams earlier will still be
+            able to print to the console, as they circumvent the replacement.
         :param save_output_with_time: If true, all output (stdout and stderr)
             will be saved with the time it was written. This gives you more
             insights on the runtime of the algorithm, but also increases the
-            size of the database.
+            size of the database. This option is ignored if `save_output` is
+            set to false.
         """
         self._db = BenchmarkDb(path)
+        self._save_output = save_output
+        self._hide_output = hide_output
         self._save_output_with_time = save_output_with_time
         self._log_captures = {}
 
     def capture_logger(self, logger_name: str, level=logging.NOTSET):
         """
         Capture the logs of a logger of the Python logging module.
         This allows you to precisely control which logs you want to
@@ -110,35 +131,39 @@
 
         Caveat: This function may have false negatives. i.e., says that it
         does not exist despite it existing (only for fresh data).
         """
         fingp, _ = self._get_arg_data(func, args, kwargs)
         return self._db.contains_fingerprint(fingp)
 
-    def _get_stream_obj(self):
+    def _get_stream_obj(self, forward_stream):
+        if not self._save_output:
+            # This wrapper just adds a ``getvalue`` method to the stream,
+            # so it can be used drop-in for StringIO.
+            return NotSavingIO(forward_stream)
         if self._save_output_with_time:
             # SteamWithTime is a wrapper around StringIO.
             # It stores the time of each line.
             # getvalue() returns a list of tuples (time, line).
-            return StreamWithTime()
+            return StreamWithTime(forward_stream)
         else:
-            return io.StringIO()
+            return PrintingStringIO(forward_stream)
 
     def run(self, func: typing.Callable, *args, **kwargs):
         """
         Will add the function call with the arguments
         to the benchmark.
 
         The output of stdout and stderr will be captured and stored,
         but not printed to the console.
         """
         fingp, arg_data = self._get_arg_data(func, args, kwargs)
         try:
-            stdout = self._get_stream_obj()
-            stderr = self._get_stream_obj()
+            stdout = self._get_stream_obj(sys.stdout if not self._hide_output else None)
+            stderr = self._get_stream_obj(sys.stderr if not self._hide_output else None)
             with ExitStack() as logging_stack:
                 log_handler = JsonLogHandler()
                 for logger_name, level in self._log_captures.items():
                     logging_stack.enter_context(
                         JsonLogCapture(logger_name, level, log_handler)
                     )
                 with redirect_stdout(stdout), redirect_stderr(stderr):
```

### Comparing `AlgBench-2.0.2/src/algbench/benchmark_db.py` & `AlgBench-2.1.0/src/algbench/benchmark_db.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/db/json_serializer.py` & `AlgBench-2.1.0/src/algbench/db/json_serializer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/db/nfs_json_dict.py` & `AlgBench-2.1.0/src/algbench/db/nfs_json_dict.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/db/nfs_json_list.py` & `AlgBench-2.1.0/src/algbench/db/nfs_json_list.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/db/nfs_json_set.py` & `AlgBench-2.1.0/src/algbench/db/nfs_json_set.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/environment.py` & `AlgBench-2.1.0/src/algbench/environment.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/log_capture.py` & `AlgBench-2.1.0/src/algbench/log_capture.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/pandas.py` & `AlgBench-2.1.0/src/algbench/pandas.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/src/algbench/utils/timer.py` & `AlgBench-2.1.0/src/algbench/utils/timer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/tests/test_basics.py` & `AlgBench-2.1.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.2/tests/test_logger.py` & `AlgBench-2.1.0/tests/test_logger.py`

 * *Files identical despite different names*

