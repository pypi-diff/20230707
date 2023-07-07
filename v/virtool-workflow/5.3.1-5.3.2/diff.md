# Comparing `tmp/virtool_workflow-5.3.1.tar.gz` & `tmp/virtool_workflow-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtool_workflow-5.3.1.tar", max compression
+gzip compressed data, was "virtool_workflow-5.3.2.tar", max compression
```

## Comparing `virtool_workflow-5.3.1.tar` & `virtool_workflow-5.3.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1097 2023-07-05 20:22:12.764709 virtool_workflow-5.3.1/LICENSE
--rw-r--r--   0        0        0     3874 2023-07-05 20:22:12.764709 virtool_workflow-5.3.1/README.md
--rw-r--r--   0        0        0     1094 2023-07-05 20:22:39.040563 virtool_workflow-5.3.1/pyproject.toml
--rw-r--r--   0        0        0      370 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/__init__.py
--rw-r--r--   0        0        0      126 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/__init__.py
--rw-r--r--   0        0        0      795 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/analysis.py
--rw-r--r--   0        0        0     7127 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/fastqc.py
--rw-r--r--   0        0        0      405 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/fixtures.py
--rw-r--r--   0        0        0     2148 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/hmms.py
--rw-r--r--   0        0        0     1079 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/indexes.py
--rw-r--r--   0        0        0     1355 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/reads.py
--rw-r--r--   0        0        0      717 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/sample.py
--rw-r--r--   0        0        0     4082 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/skewer.py
--rw-r--r--   0        0        0      549 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/subtractions.py
--rw-r--r--   0        0        0     1978 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/trimming.py
--rw-r--r--   0        0        0      992 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/__init__.py
--rw-r--r--   0        0        0     4789 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/analysis.py
--rw-r--r--   0        0        0     1528 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/client.py
--rw-r--r--   0        0        0     2476 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/errors.py
--rw-r--r--   0        0        0     2106 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/hmm.py
--rw-r--r--   0        0        0     3616 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/indexes.py
--rw-r--r--   0        0        0     4248 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/jobs.py
--rw-r--r--   0        0        0     3168 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/samples.py
--rw-r--r--   0        0        0     4016 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/subtractions.py
--rw-r--r--   0        0        0     1861 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/uploads.py
--rw-r--r--   0        0        0     3769 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/utils.py
--rw-r--r--   0        0        0     1510 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/builtin_fixtures.py
--rw-r--r--   0        0        0     1392 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/cli.py
--rw-r--r--   0        0        0        0 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/__init__.py
--rw-r--r--   0        0        0     1117 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/analysis.py
--rw-r--r--   0        0        0      376 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/files.py
--rw-r--r--   0        0        0     6565 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/indexes.py
--rw-r--r--   0        0        0      240 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/jobs.py
--rw-r--r--   0        0        0      864 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/samples.py
--rw-r--r--   0        0        0     1500 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/subtractions.py
--rw-r--r--   0        0        0     1697 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/decorators.py
--rw-r--r--   0        0        0      230 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/errors.py
--rw-r--r--   0        0        0     2647 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/hooks.py
--rw-r--r--   0        0        0        0 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/__init__.py
--rw-r--r--   0        0        0     2937 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/discovery.py
--rw-r--r--   0        0        0      138 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/events.py
--rw-r--r--   0        0        0     3561 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/executor.py
--rw-r--r--   0        0        0     4389 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/hook.py
--rw-r--r--   0        0        0     2504 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/providers.py
--rw-r--r--   0        0        0     1566 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/redis.py
--rw-r--r--   0        0        0     5618 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/run.py
--rw-r--r--   0        0        0     4636 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/run_subprocess.py
--rw-r--r--   0        0        0      684 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/sentry.py
--rw-r--r--   0        0        0      203 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/states.py
--rw-r--r--   0        0        0     2437 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/step.py
--rw-r--r--   0        0        0      432 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/runtime/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/testing/__init__.py
--rw-r--r--   0        0        0     1609 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/testing/fixtures.py
--rw-r--r--   0        0        0      752 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/workflow.py
--rw-r--r--   0        0        0     4774 1970-01-01 00:00:00.000000 virtool_workflow-5.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-07-07 03:22:20.264675 virtool_workflow-5.3.2/LICENSE
+-rw-r--r--   0        0        0     3874 2023-07-07 03:22:20.264675 virtool_workflow-5.3.2/README.md
+-rw-r--r--   0        0        0     1095 2023-07-07 03:22:42.693182 virtool_workflow-5.3.2/pyproject.toml
+-rw-r--r--   0        0        0      370 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/__init__.py
+-rw-r--r--   0        0        0      795 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/analysis.py
+-rw-r--r--   0        0        0     7127 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/fastqc.py
+-rw-r--r--   0        0        0      405 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/fixtures.py
+-rw-r--r--   0        0        0     2148 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/hmms.py
+-rw-r--r--   0        0        0     1079 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/indexes.py
+-rw-r--r--   0        0        0     1355 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/reads.py
+-rw-r--r--   0        0        0      717 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/sample.py
+-rw-r--r--   0        0        0     4082 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/skewer.py
+-rw-r--r--   0        0        0      549 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/subtractions.py
+-rw-r--r--   0        0        0     1978 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/trimming.py
+-rw-r--r--   0        0        0      992 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/analysis/utils.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/__init__.py
+-rw-r--r--   0        0        0     4789 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/analysis.py
+-rw-r--r--   0        0        0     1528 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/client.py
+-rw-r--r--   0        0        0     2476 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/errors.py
+-rw-r--r--   0        0        0     2106 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/hmm.py
+-rw-r--r--   0        0        0     3616 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/indexes.py
+-rw-r--r--   0        0        0     4248 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/jobs.py
+-rw-r--r--   0        0        0     3168 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/samples.py
+-rw-r--r--   0        0        0     4016 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/subtractions.py
+-rw-r--r--   0        0        0     1861 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/uploads.py
+-rw-r--r--   0        0        0     3769 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/api/utils.py
+-rw-r--r--   0        0        0     1510 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/builtin_fixtures.py
+-rw-r--r--   0        0        0     1392 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/cli.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/data_model/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/data_model/analysis.py
+-rw-r--r--   0        0        0      376 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/data_model/files.py
+-rw-r--r--   0        0        0     6565 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/data_model/indexes.py
+-rw-r--r--   0        0        0      240 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/data_model/jobs.py
+-rw-r--r--   0        0        0      864 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/data_model/samples.py
+-rw-r--r--   0        0        0     1500 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/data_model/subtractions.py
+-rw-r--r--   0        0        0     1697 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/decorators.py
+-rw-r--r--   0        0        0      230 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/errors.py
+-rw-r--r--   0        0        0     2647 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/hooks.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/__init__.py
+-rw-r--r--   0        0        0     2937 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/discovery.py
+-rw-r--r--   0        0        0      138 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/events.py
+-rw-r--r--   0        0        0     3561 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/executor.py
+-rw-r--r--   0        0        0     4389 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/hook.py
+-rw-r--r--   0        0        0     2504 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/providers.py
+-rw-r--r--   0        0        0     1566 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/redis.py
+-rw-r--r--   0        0        0     5618 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/run.py
+-rw-r--r--   0        0        0     4636 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/run_subprocess.py
+-rw-r--r--   0        0        0      684 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/sentry.py
+-rw-r--r--   0        0        0      203 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/states.py
+-rw-r--r--   0        0        0     2437 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/step.py
+-rw-r--r--   0        0        0      432 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/runtime/utils.py
+-rw-r--r--   0        0        0        0 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/testing/__init__.py
+-rw-r--r--   0        0        0     1609 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/testing/fixtures.py
+-rw-r--r--   0        0        0      752 2023-07-07 03:22:21.032756 virtool_workflow-5.3.2/virtool_workflow/workflow.py
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 virtool_workflow-5.3.2/PKG-INFO
```

### Comparing `virtool_workflow-5.3.1/LICENSE` & `virtool_workflow-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/README.md` & `virtool_workflow-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/pyproject.toml` & `virtool_workflow-5.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virtool-workflow"
-version = "5.3.1"
+version = "5.3.2"
 description = "A framework for developing bioinformatics workflows for Virtool."
 authors = ["Ian Boyes", "Blake Smith", "Ryan Fang"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/virtool/virtool-workflow"
 classifiers = [
     "Topic :: Software Development :: Libraries",
@@ -15,15 +15,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.0.0"
 aiohttp = "^3.8.1"
 aiofiles = "^0.7.0"
-virtool-core = "^3.0.0"
+virtool-core = "^4.13.0"
 aioredis = "1.3.1"
 sentry-sdk = "^1.5.7"
 pyfixtures = "^1.0.0"
 
 [tool.poetry.scripts]
 run-workflow = "virtool_workflow.cli:cli_main"
 
@@ -33,13 +33,13 @@
 pytest-regressions = "^2.4.1"
 pytest-docker-compose = "^3.2.1"
 pytest-mock = "^3.10.0"
 pre-commit = "^2.18.1"
 pytest = "^6.2.2"
 pytest-asyncio = "^0.17.0"
 pytest-aiohttp = "^0.3.0"
-motor = "^2.5.1"
+motor = "^3.1.2"
 black = "^22.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/analysis.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/fastqc.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/fastqc.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/hmms.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/hmms.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/indexes.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/indexes.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/reads.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/reads.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/sample.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/sample.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/skewer.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/skewer.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/subtractions.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/subtractions.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/trimming.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/trimming.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/analysis/utils.py` & `virtool_workflow-5.3.2/virtool_workflow/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/analysis.py` & `virtool_workflow-5.3.2/virtool_workflow/api/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/client.py` & `virtool_workflow-5.3.2/virtool_workflow/api/client.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/errors.py` & `virtool_workflow-5.3.2/virtool_workflow/api/errors.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/hmm.py` & `virtool_workflow-5.3.2/virtool_workflow/api/hmm.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/indexes.py` & `virtool_workflow-5.3.2/virtool_workflow/api/indexes.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/jobs.py` & `virtool_workflow-5.3.2/virtool_workflow/api/jobs.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/samples.py` & `virtool_workflow-5.3.2/virtool_workflow/api/samples.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/subtractions.py` & `virtool_workflow-5.3.2/virtool_workflow/api/subtractions.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/uploads.py` & `virtool_workflow-5.3.2/virtool_workflow/api/uploads.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/api/utils.py` & `virtool_workflow-5.3.2/virtool_workflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/builtin_fixtures.py` & `virtool_workflow-5.3.2/virtool_workflow/builtin_fixtures.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/cli.py` & `virtool_workflow-5.3.2/virtool_workflow/cli.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/data_model/analysis.py` & `virtool_workflow-5.3.2/virtool_workflow/data_model/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/data_model/indexes.py` & `virtool_workflow-5.3.2/virtool_workflow/data_model/indexes.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/data_model/samples.py` & `virtool_workflow-5.3.2/virtool_workflow/data_model/samples.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/data_model/subtractions.py` & `virtool_workflow-5.3.2/virtool_workflow/data_model/subtractions.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/decorators.py` & `virtool_workflow-5.3.2/virtool_workflow/decorators.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/hooks.py` & `virtool_workflow-5.3.2/virtool_workflow/hooks.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/discovery.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/discovery.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/executor.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/executor.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/hook.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/hook.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/providers.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/providers.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/redis.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/redis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/run.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/run.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/run_subprocess.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/run_subprocess.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/sentry.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/runtime/step.py` & `virtool_workflow-5.3.2/virtool_workflow/runtime/step.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/testing/fixtures.py` & `virtool_workflow-5.3.2/virtool_workflow/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/virtool_workflow/workflow.py` & `virtool_workflow-5.3.2/virtool_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.1/PKG-INFO` & `virtool_workflow-5.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtool-workflow
-Version: 5.3.1
+Version: 5.3.2
 Summary: A framework for developing bioinformatics workflows for Virtool.
 Home-page: https://github.com/virtool/virtool-workflow
 License: MIT
 Author: Ian Boyes
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiofiles (>=0.7.0,<0.8.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: aioredis (==1.3.1)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: pyfixtures (>=1.0.0,<2.0.0)
 Requires-Dist: sentry-sdk (>=1.5.7,<2.0.0)
-Requires-Dist: virtool-core (>=3.0.0,<4.0.0)
+Requires-Dist: virtool-core (>=4.13.0,<5.0.0)
 Project-URL: Repository, https://github.com/virtool/virtool-workflow
 Description-Content-Type: text/markdown
 
 # Virtool Workflow
 
 ![Tests](https://github.com/virtool/virtool-workflow/workflows/Tests/badge.svg?branch=master)
 [![PyPI version](https://badge.fury.io/py/virtool-workflow.svg)](https://badge.fury.io/py/virtool-workflow)
```

