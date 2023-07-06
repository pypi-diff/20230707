# Comparing `tmp/neuro-flow-22.8.1.tar.gz` & `tmp/neuro-flow-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-flow-22.8.1.tar", last modified: Fri Aug  5 10:15:26 2022, max compression
+gzip compressed data, was "neuro-flow-23.7.0.tar", last modified: Thu Jul  6 23:04:37 2023, max compression
```

## Comparing `neuro-flow-22.8.1.tar` & `neuro-flow-23.7.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:15:26.618602 neuro-flow-22.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-08-05 10:15:26.618602 neuro-flow-22.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-08-05 10:15:26.622602 neuro-flow-22.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:15:26.610602 neuro-flow-22.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:15:26.614602 neuro-flow-22.8.1/src/neuro_flow/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12922 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/ast.py
--rw-r--r--   0 runner    (1001) docker     (121)    49122 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/batch_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    30083 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/batch_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:15:26.618602 neuro-flow-22.8.1/src/neuro_flow/cli/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11307 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)    11963 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/click_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/file_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/images.py
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/live.py
--rw-r--r--   0 runner    (1001) docker     (121)     5879 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/root.py
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/colored_topo_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)    13704 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)    90880 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    46118 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)     7573 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/expr_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)    24864 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/live_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)    48945 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:15:26.618602 neuro-flow-22.8.1/src/neuro_flow/storage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36672 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/storage/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    12291 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    18844 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/storage/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2022-08-05 10:14:47.000000 neuro-flow-22.8.1/src/neuro_flow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 10:15:26.618602 neuro-flow-22.8.1/src/neuro_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-08-05 10:15:26.000000 neuro-flow-22.8.1/src/neuro_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-08-05 10:15:26.000000 neuro-flow-22.8.1/src/neuro_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 10:15:26.000000 neuro-flow-22.8.1/src/neuro_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-05 10:15:26.000000 neuro-flow-22.8.1/src/neuro_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 10:14:58.000000 neuro-flow-22.8.1/src/neuro_flow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-05 10:15:26.000000 neuro-flow-22.8.1/src/neuro_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-05 10:15:26.000000 neuro-flow-22.8.1/src/neuro_flow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:37.502023 neuro-flow-23.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-06 23:04:37.502023 neuro-flow-23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-06 23:04:37.502023 neuro-flow-23.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:37.490023 neuro-flow-23.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:37.494023 neuro-flow-23.7.0/src/neuro_flow/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47524 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/batch_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/batch_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:37.498023 neuro-flow-23.7.0/src/neuro_flow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/click_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/file_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/colored_topo_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13704 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91408 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46118 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/expr_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23426 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/live_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49145 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:37.498023 neuro-flow-23.7.0/src/neuro_flow/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37416 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/storage/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12756 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/storage/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-06 23:03:56.000000 neuro-flow-23.7.0/src/neuro_flow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:37.498023 neuro-flow-23.7.0/src/neuro_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-06 23:04:37.000000 neuro-flow-23.7.0/src/neuro_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-06 23:04:37.000000 neuro-flow-23.7.0/src/neuro_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:04:37.000000 neuro-flow-23.7.0/src/neuro_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 23:04:37.000000 neuro-flow-23.7.0/src/neuro_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:04:07.000000 neuro-flow-23.7.0/src/neuro_flow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-06 23:04:37.000000 neuro-flow-23.7.0/src/neuro_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 23:04:37.000000 neuro-flow-23.7.0/src/neuro_flow.egg-info/top_level.txt
```

### Comparing `neuro-flow-22.8.1/LICENSE` & `neuro-flow-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/PKG-INFO` & `neuro-flow-23.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: neuro-flow
-Version: 22.8.1
+Version: 23.7.0
 Summary: Pipelines system for neu.ro
 Home-page: https://github.com/neuro-inc/neuro-flow
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Getting started
 
 `neuro-flow` is a tool that simplifies daily jobs on the Neu.ro platform.
```

### Comparing `neuro-flow-22.8.1/README.md` & `neuro-flow-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/setup.cfg` & `neuro-flow-23.7.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Neu.ro Team
 author_email = team@neu.ro
 license = Apache 2
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Intended Audience :: Information Technology
 	Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -25,24 +26,24 @@
 	License :: OSI Approved :: Apache Software License
 
 [options]
 package_dir = 
 	=src
 packages = find:
 zip_safe = False
-python_requires = >=3.7.0
+python_requires = >=3.8.0
 include_package_data = True
 install_requires = 
-	neuro-cli>=21.11.4
+	neuro-cli>=23.7.0
 	pyyaml>=5.4
 	funcparserlib>=1.0.0
 	humanize>=0.5.1
-	neuro-extras>=21.11.5
+	neuro-extras>=23.7.0
 	graphviz>=0.14
-	yarl>=1.7,<1.8
+	yarl>=1.7
 	multidict>=5.0,<6.0
 	rich>=10.0.1
 	typing-extensions>=3.10
 	click>=8.0
 
 [options.packages.find]
 where = src
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/ast.py` & `neuro-flow-23.7.0/src/neuro_flow/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     life_span: OptTimeDeltaExpr
     # TODO: maybe add extra key->value mapping for additional cache keys later
 
 
 @dataclass(frozen=True)
 class Project(Base):
     id: SimpleIdExpr
+    project_name: SimpleOptStrExpr  # project name can contain "-"
     owner: SimpleOptStrExpr  # user name can contain "-"
     role: SimpleOptStrExpr
 
     images: Optional[Mapping[str, "Image"]] = field(metadata={"allow_none": True})
     volumes: Optional[Mapping[str, "Volume"]] = field(metadata={"allow_none": True})
     defaults: Optional["BatchFlowDefaults"] = field(metadata={"allow_none": True})
     mixins: Optional[Mapping[str, "ExecUnitMixin"]] = field(
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/batch_executor.py` & `neuro-flow-23.7.0/src/neuro_flow/batch_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import asyncio
 import logging
 import os
 import shlex
+import sys
 import textwrap
 from collections import defaultdict
 from contextlib import asynccontextmanager
 from datetime import datetime, timedelta, timezone
 from neuro_sdk import (
-    Action,
-    AuthorizationError,
     Client,
     DiskVolume,
     EnvParseResult,
     HTTPPort,
-    IllegalArgumentError,
     JobDescription,
     JobRestartPolicy,
     JobStatus,
-    Permission,
     Preset,
     RemoteImage,
     ResourceNotFound,
     SecretFile,
     Tag,
     Volume,
     VolumeParseResult,
@@ -446,20 +443,14 @@
         self, env: Sequence[str], env_file: Sequence[str] = ()
     ) -> EnvParseResult:
         return self._client.parse.envs(env, env_file)
 
     def parse_volumes(self, volume: Sequence[str]) -> VolumeParseResult:
         return self._client.parse.volumes(volume)
 
-    async def user_add(self, role_name: str) -> None:
-        await self._client.users.add(role_name)
-
-    async def user_share(self, user: str, permission: Permission) -> Permission:
-        return await self._client.users.share(user, permission)
-
 
 class BatchExecutor:
     transient_progress: bool = False
     run_builder_job: Callable[..., Awaitable[str]] = staticmethod(  # type: ignore
         start_image_build
     )
 
@@ -496,15 +487,14 @@
         self._bake_storage = bake_storage
         self._graphs: Graph[RunningBatchBase[BaseBatchContext]] = Graph(
             flow.graph, flow
         )
         self._tasks_mgr = BakeTasksManager()
         self._is_cancelling = False
         self._project_role = project_role
-        self._is_projet_role_created = False
 
         self._run_builder_job = self.run_builder_job
 
         # A note about default value:
         # AS: I have no idea what timeout is better;
         # too short value bombards servers,
         # too long timeout makes the waiting longer than expected
@@ -1154,15 +1144,14 @@
             name=task.name,
             tags=list(task.tags),
             description=task.title,
             life_span=task.life_span,
             schedule_timeout=task.schedule_timeout,
             pass_config=bool(task.pass_config),
         )
-        await self._add_resource(job.uri)
         return await self._create_task(
             yaml_id=full_id,
             raw_id=job.id,
             status=TaskStatusItem(
                 when=job.history.created_at or datetime.now(timezone.utc),
                 status=TaskStatus.PENDING,
             ),
@@ -1229,46 +1218,14 @@
                     await image_storage.update(
                         status=ImageStatus.BUILD_FAILED,
                     )
                     self._progress.log(
                         "Image", fmt_id(image.ref), "is", ImageStatus.BUILD_FAILED
                     )
 
-    async def _create_project_role(self, project_role: str) -> None:
-        if self._is_projet_role_created:
-            return
-        log.debug(f"BatchExecutor: creating project role {project_role}")
-        try:
-            await self._client.user_add(project_role)
-        except AuthorizationError:
-            log.debug(
-                f"BatchExecutor: AuthorizationError for create"
-                f" project role {project_role}"
-            )
-            pass
-            # We have no permissions to create role --
-            # assume that this is shared project and
-            # current user is not the owner
-        except IllegalArgumentError as e:
-            if "already exists" not in str(e):
-                raise
-        self._is_projet_role_created = True
-
-    async def _add_resource(self, uri: URL) -> None:
-        log.debug(f"BatchExecutor: adding resource {uri}")
-        project_role = self._project_role
-        if project_role is None:
-            return
-        await self._create_project_role(project_role)
-        permission = Permission(uri, Action.WRITE)
-        try:
-            await self._client.user_share(project_role, permission)
-        except ValueError:
-            self._progress.log(f"[red]Cannot share [b]{uri!s}[/b]")
-
 
 class LocalsBatchExecutor(BatchExecutor):
     transient_progress = True
 
     @classmethod
     @asynccontextmanager
     async def create(
@@ -1297,16 +1254,17 @@
     async def _process_local(self, full_id: FullID) -> None:
         local = await self._get_local(full_id)
         task = await self._create_task(
             yaml_id=full_id,
             status=TaskStatus.PENDING,
             raw_id=None,
         )
+        posix = False if sys.platform == "win32" else True
         subprocess = await asyncio.create_subprocess_exec(
-            *shlex.split(local.cmd),
+            *shlex.split(local.cmd, posix=posix),
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             cwd=self._top_flow.workspace,
         )
         (stdout_data, stderr_data) = await subprocess.communicate()
         async with CmdProcessor() as proc:
             async for line in proc.feed_chunk(stdout_data):
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/batch_runner.py` & `neuro-flow-23.7.0/src/neuro_flow/batch_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,18 +207,24 @@
                         dockerfile=image.dockerfile,
                         ast=flow.get_image_ast(image.id),
                     )
                 )
 
     errors = []
     for ref, images in _tmp.items():
+        # checks rendered paths are the same (for local actions)
         contexts_differ = len({it.context for it in images}) > 1
         dockerfiles_differ = len({it.dockerfile for it in images}) > 1
         if contexts_differ or dockerfiles_differ:
-            errors.append(ImageRefNotUniqueError(ref, images))
+            # if rendered paths do not match, we might be dealing with github action
+            # and should compare ast defs
+            ast_contexts_differ = len({it.ast.context for it in images}) > 1
+            ast_dockerfiles_differ = len({it.ast.dockerfile for it in images}) > 1
+            if ast_contexts_differ or ast_dockerfiles_differ:
+                errors.append(ImageRefNotUniqueError(ref, images))
     if errors:
         raise MultiError(errors)
 
 
 async def build_graphs(
     top_flow: RunningBatchFlow,
 ) -> Mapping[FullID, Mapping[FullID, AbstractSet[FullID]]]:
@@ -343,16 +349,21 @@
     async def close(self) -> None:
         if self._config_loader is not None:
             await self._config_loader.close()
 
     async def __aenter__(self) -> "BatchRunner":
         self._config_loader = BatchLocalCL(self._config_dir, self._client)
         self._project = await setup_project_ctx(EMPTY_ROOT, self._config_loader)
+        project_name = (
+            self._project.project_name or self._client.config.project_name_or_raise
+        )
         project = await self._storage.get_or_create_project(
-            self._project.id, owner=self._project.owner
+            self._project.id,
+            owner=self._project.owner,
+            project_name=project_name,
         )
         self._project_storage = self._storage.project(id=project.id)
         return self
 
     async def __aexit__(
         self,
         exc_typ: Optional[Type[BaseException]],
@@ -411,15 +422,15 @@
         )
         bake_storage = self.storage.bake(id=bake.id)
         config_meta = await self.config_loader.collect_configs(batch_name, bake_storage)
         await bake_storage.create_attempt(number=1, configs_meta=config_meta)
 
         self._console.log(
             f"Bake [b]{bake.name or bake.id}[/b] of "
-            f"project [b]{self.project_id}[/b] is created"
+            f"flow [b]{self.project_id}[/b] is created"
         )
         self._console.log("Uploading image contexts/dockerfiles...")
         await upload_image_data(flow, self._run_neuro_cli, bake_storage)
 
         return bake, flow
 
     # Next function is also used in tests:
@@ -467,14 +478,16 @@
             await self.process(bake.id)
         else:
             self._console.log(f"[bright_black]Starting remote executor")
             if flow.life_span:
                 life_span = fmt_timedelta(flow.life_span)
             else:
                 life_span = "7d"
+            # TODO: Update tags `project` -> `flow` and `flow` -> `batch`
+            # After performing the corresponding changes in web app upfront.
             run_args = [
                 "run",
                 "--pass-config",
                 f"--volume=storage:.flow/logs/{bake.id}/:/root/.neuro/logs"
                 f"--life-span={life_span}",
                 f"--tag=project:{self.project_id}",
                 f"--tag=flow:{bake.batch}",
@@ -572,23 +585,22 @@
         *,
         attempt_no: int = -1,
         output: Optional[LocalPath] = None,
         save_dot: bool = False,
         save_pdf: bool = False,
         view_pdf: bool = False,
     ) -> None:
-
         bake_storage = self.storage.bake(id=bake_id)
         try:
             bake = await bake_storage.get()
         except ResourceNotFound:
             self._console.print("[yellow]Bake not found")
             self._console.print(
-                f"Please make sure that the bake [b]{bake_id}[/b] and "
-                f"project [b]{self.project_id}[/b] are correct."
+                f"Please make sure that the bake ID [b]{bake_id}[/b] and "
+                f"flow [b]{self.project_id}[/b] are correct."
             )
             exit(1)
             assert False, "unreachable"
 
         attempt_storage = bake_storage.attempt(number=attempt_no)
         attempt = await attempt_storage.get()
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/batch.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/batch.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/click_types.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/click_types.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/completion.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/completion.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/file_logging.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/file_logging.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/flow.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/flow.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/images.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/images.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/live.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/live.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,21 +151,21 @@
                 raise click.BadArgumentUsage(
                     "Suffix is not supported when killing ALL jobs"
                 )
             await runner.kill_all()
 
 
 @click.command()
-@argument("project_ids", type=PROJECT, nargs=-1, required=True)
+@argument("flow_ids", type=PROJECT, nargs=-1, required=True)
 @wrap_async()
-async def delete_project(
+async def delete_flow(
     root: Root,
-    project_ids: Sequence[str],
+    flow_ids: Sequence[str],
 ) -> None:
-    """Completely remove project with all related entities"""
+    """Completely remove flow with all related entities"""
     async with AsyncExitStack() as stack:
         client = await stack.enter_async_context(neuro_sdk.get())
         storage: Storage = await stack.enter_async_context(ApiStorage(client))
-        for project_id in project_ids:
-            await storage.project(yaml_id=project_id).delete()
+        for flow_id in flow_ids:
+            await storage.project(yaml_id=flow_id).delete()
             if root.verbosity >= 0:
-                root.console.print(f"Project '{project_id}' was successfully removed.")
+                root.console.print(f"Flow '{flow_id}' was successfully removed.")
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/main.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
 # Live commands
 cli.add_command(live.run)
 cli.add_command(live.ps)
 cli.add_command(live.logs)
 cli.add_command(live.status)
 cli.add_command(live.kill)
-cli.add_command(live.delete_project)
+cli.add_command(live.delete_flow)
 
 # Batch commands
 cli.add_command(batch.bake)
 cli.add_command(batch.execute)
 cli.add_command(batch.bakes)
 cli.add_command(batch.show)
 cli.add_command(batch.inspect)
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/storage.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/storage.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/cli/utils.py` & `neuro-flow-23.7.0/src/neuro_flow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/colored_topo_sorter.py` & `neuro-flow-23.7.0/src/neuro_flow/colored_topo_sorter.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/commands.py` & `neuro-flow-23.7.0/src/neuro_flow/commands.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/config_loader.py` & `neuro-flow-23.7.0/src/neuro_flow/config_loader.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/context.py` & `neuro-flow-23.7.0/src/neuro_flow/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,20 @@
     pass
 
 
 class UnknownTask(KeyError):
     pass
 
 
+PROJECT_ROLE_DEPRECATED_MSG = (
+    "Flow roles are deprecated and will be ignored. "
+    "To grant access to the flow and its artifacts, please add users "
+    "to the corresponding project using `neuro admin add-project-user`."
+)
+
 # ...Ctx types, they define parts that can be available in expressions
 
 
 EnvCtx = Annotated[Mapping[str, str], "EnvCtx"]
 TagsCtx = Annotated[AbstractSet[str], "TagsCtx"]
 VolumesCtx = Annotated[Mapping[str, "VolumeCtx"], "VolumesCtx"]
 ImagesCtx = Annotated[Mapping[str, "ImageCtx"], "ImagesCtx"]
@@ -91,14 +97,15 @@
 StateCtx = Annotated[Mapping[str, str], "StateCtx"]
 MatrixCtx = Annotated[Mapping[str, LiteralT], "MatrixCtx"]
 
 
 @dataclass(frozen=True)
 class ProjectCtx:
     id: str
+    project_name: str
     owner: Optional[str] = None
     role: Optional[str] = None
 
 
 @dataclass(frozen=True)
 class FlowCtx:
     flow_id: str
@@ -740,19 +747,26 @@
 
 async def setup_project_ctx(
     ctx: RootABC,
     config_loader: ConfigLoader,
 ) -> ProjectCtx:
     ast_project = await config_loader.fetch_project()
     project_id = await ast_project.id.eval(ctx)
+    project_name = await ast_project.project_name.eval(ctx)
+    # TODO (y.s.): Should we deprecate project_owner?
     project_owner = await ast_project.owner.eval(ctx)
     project_role = await ast_project.role.eval(ctx)
-    if project_role is None and project_owner is not None:
-        project_role = f"{project_owner}/projects/{sanitize_name(project_id)}"
-    return ProjectCtx(id=project_id, owner=project_owner, role=project_role)
+    if project_role:
+        log.warning(PROJECT_ROLE_DEPRECATED_MSG)
+    project_role = None
+    if not project_name:
+        project_name = config_loader.client.config.project_name_or_raise
+    return ProjectCtx(
+        id=project_id, owner=project_owner, role=project_role, project_name=project_name
+    )
 
 
 async def setup_flow_ctx(
     ctx: RootABC,
     ast_flow: ast.BaseFlow,
     config_name: str,
     config_loader: ConfigLoader,
@@ -1248,40 +1262,40 @@
         ...
 
 
 _MergeTarget = TypeVar("_MergeTarget", bound=SupportsAstMerge)
 
 
 async def merge_asts(child: _MergeTarget, parent: SupportsAstMerge) -> _MergeTarget:
-    child_fields = {f.name for f in dataclasses.fields(child)}
+    child_fields = {f.name for f in dataclasses.fields(child)}  # type: ignore
     for field in parent._specified_fields:
         if field == "mixins" or field not in child_fields:
             continue
         field_present = field in child._specified_fields
         child_value = getattr(child, field)
         parent_value = getattr(parent, field)
         merge_supported = isinstance(parent_value, BaseSequenceExpr) or isinstance(
             parent_value, BaseMappingExpr
         )
         if not field_present or (child_value is None and merge_supported):
             child = replace(
                 child,
                 **{field: parent_value},
                 _specified_fields=child._specified_fields | {field},
-            )
+            )  # type: ignore
         elif isinstance(parent_value, BaseSequenceExpr):
             assert isinstance(child_value, BaseSequenceExpr)
             child = replace(
                 child, **{field: ConcatSequenceExpr(child_value, parent_value)}
-            )
+            )  # type: ignore
         elif isinstance(parent_value, BaseMappingExpr):
             assert isinstance(child_value, BaseMappingExpr)
             child = replace(
                 child, **{field: MergeMappingsExpr(child_value, parent_value)}
-            )
+            )  # type: ignore
     return child
 
 
 class MixinApplyTarget(Protocol):
     @property
     def mixins(self) -> Optional[Sequence[StrExpr]]:
         ...
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/expr.py` & `neuro-flow-23.7.0/src/neuro_flow/expr.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/expr_validation.py` & `neuro-flow-23.7.0/src/neuro_flow/expr_validation.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow/live_runner.py` & `neuro-flow-23.7.0/src/neuro_flow/live_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,15 @@
 
 import asyncio
 import click
 import datetime
 import secrets
 import shlex
 import sys
-from neuro_sdk import (
-    Action,
-    AuthorizationError,
-    Client,
-    IllegalArgumentError,
-    JobDescription,
-    JobStatus,
-    Permission,
-    ResourceNotFound,
-)
+from neuro_sdk import Client, JobDescription, JobStatus, ResourceNotFound
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from types import TracebackType
 from typing import (
     AbstractSet,
     AsyncContextManager,
@@ -27,15 +18,14 @@
     Iterable,
     List,
     Mapping,
     Optional,
     Tuple,
     Type,
 )
-from yarl import URL
 
 from .config_loader import LiveLocalCL
 from .context import ImageCtx, JobMeta, RunningLiveFlow, UnknownJob, VolumeCtx
 from .parser import ConfigDir
 from .storage.base import ProjectStorage, Storage
 from .types import TaskStatus
 from .utils import (
@@ -71,15 +61,14 @@
         self._config_dir = config_dir
         self._console = console
         self._config_loader: Optional[LiveLocalCL] = None
         self._flow: Optional[RunningLiveFlow] = None
         self._client = client
         self._storage = storage
         self._project_storage: Optional[ProjectStorage] = None
-        self._is_projet_role_created = False
         self._run_neuro_cli = make_cmd_exec(
             "neuro", global_options=encode_global_options(global_options)
         )
         self._run_extras_cli = make_cmd_exec("neuro-extras")
         self._dry_run = dry_run
 
     async def init_flow(self) -> None:
@@ -91,16 +80,22 @@
                 self._config_loader, dry_run=self._dry_run
             )
         except Exception:
             await self._config_loader.close()
             raise
 
     async def init_project_storage(self) -> None:
+        project_name = self.flow.project.project_name
+        if not project_name:
+            project_name = self._client.config.project_name_or_raise
+
         project = await self._storage.get_or_create_project(
-            self.flow.project.id, owner=self.flow.project.owner
+            self.flow.project.id,
+            owner=self.flow.project.owner,
+            project_name=project_name,
         )
         self._project_storage = self._storage.project(id=project.id)
 
     async def close(self) -> None:
         if self._config_loader is not None:
             await self._config_loader.close()
 
@@ -164,39 +159,45 @@
             days=7
         )
         if meta.multi and not suffix:
             async for job in self.client.jobs.list(
                 tags=meta.tags,
                 reverse=True,
                 statuses=(JobStatus.PENDING, JobStatus.RUNNING),
+                project_names=[self.flow.project.project_name],
+                org_names=[self.client.config.org_name],
             ):
                 found = True
                 yield job
             async for job in self.client.jobs.list(
                 tags=meta.tags,
                 reverse=True,
                 statuses=(
                     JobStatus.SUSPENDED,
                     JobStatus.SUCCEEDED,
                     JobStatus.FAILED,
                     JobStatus.CANCELLED,
                 ),
                 since=since,
+                project_names=[self.flow.project.project_name],
+                org_names=[self.client.config.org_name],
             ):
                 found = True
                 yield job
         else:
             tags = list(meta.tags)
             if meta.multi and suffix:
                 tags.append(f"multi:{suffix}")
             async for job in self.client.jobs.list(
                 tags=tags,
                 reverse=True,
                 limit=1,
                 statuses=(JobStatus.PENDING, JobStatus.RUNNING),
+                project_names=[self.flow.project.project_name],
+                org_names=[self.client.config.org_name],
             ):
                 found = True
                 yield job
                 return
             async for job in self.client.jobs.list(
                 tags=tags,
                 reverse=True,
@@ -204,14 +205,16 @@
                 statuses=(
                     JobStatus.SUSPENDED,
                     JobStatus.SUCCEEDED,
                     JobStatus.FAILED,
                     JobStatus.CANCELLED,
                 ),
                 since=since,
+                project_names=[self.flow.project.project_name],
+                org_names=[self.client.config.org_name],
             ):
                 found = True
                 yield job
                 return
         if not found:
             raise ResourceNotFound
 
@@ -401,15 +404,15 @@
                 name = name.replace("--", "-")
         run_args.append(f"--name={name}")
         if job.preset is not None:
             run_args.append(f"--preset={job.preset}")
         if job.schedule_timeout is not None:
             run_args.append(f"--schedule-timeout={int(job.schedule_timeout)}s")
         if job.http_port is not None:
-            run_args.append(f"--http={job.http_port}")
+            run_args.append(f"--http-port={job.http_port}")
         if job.http_auth is not None:
             if job.http_auth:
                 run_args.append(f"--http-auth")
             else:
                 run_args.append(f"--no-http-auth")
         if job.entrypoint:
             run_args.append(f"--entrypoint={job.entrypoint}")
@@ -427,18 +430,14 @@
             run_args.append(f"--browse")
         if job.detach:
             run_args.append(f"--detach")
         for pf in job.port_forward:
             run_args.append(f"--port-forward={pf}")
         if job.pass_config:
             run_args.append(f"--pass-config")
-        project_role = self._flow.project.role
-        if project_role is not None:
-            await self._create_project_role(project_role)
-            run_args.append(f"--share={project_role}")
 
         run_args.append(job.image)
 
         run_args.extend(["--"])
         if job.cmd:
             run_args.extend(shlex.split(job.cmd))
 
@@ -558,19 +557,14 @@
             "cp",
             "--recursive",
             "--update",
             "--no-target-directory",
             str(volume_ctx.full_local_path),
             str(volume_ctx.remote),
         )
-        uri = self._client.parse.normalize_uri(
-            volume_ctx.remote,
-            allowed_schemes=("storage",),
-        )
-        await self._add_resource(uri)
 
     async def download(self, volume: str) -> None:
         volume_ctx = await self.find_volume(volume)
         await self._run_neuro_cli(
             "cp",
             "--recursive",
             "--update",
@@ -604,19 +598,14 @@
                 volume_ctx = await self.find_volume(volume.id)
                 self._console.print(f"Create volume [b]{volume.id}[/b]")
                 await self._run_neuro_cli(
                     "mkdir",
                     "--parents",
                     str(volume_ctx.remote),
                 )
-                uri = self._client.parse.normalize_uri(
-                    volume_ctx.remote,
-                    allowed_schemes=("storage",),
-                )
-                await self._add_resource(uri)
 
     # images subsystem
 
     async def find_image(self, image: str) -> ImageCtx:
         image_ctx = self.flow.images.get(image)
         if image_ctx is None:
             self._console.print(f"[red]Unknown image [b]{image}[/b]")
@@ -647,48 +636,12 @@
         if force_overwrite or image_ctx.force_rebuild:
             cmd.append("--force-overwrite")
         if image_ctx.build_preset is not None:
             cmd.append(f"--preset={image_ctx.build_preset}")
         cmd.append(str(image_ctx.context))
         cmd.append(str(image_ctx.ref))
         await self._run_extras_cli("image", "build", *cmd)
-        image_ref = self._client.parse.remote_image(image_ctx.ref)
-        image_ref = dataclasses.replace(image_ref, tag=None)
-        await self._add_resource(URL(str(image_ref)))
 
     async def build_all(self, force_overwrite: bool) -> None:
         for image, image_ctx in self.flow.images.items():
             if image_ctx.context is not None:
                 await self.build(image, force_overwrite=force_overwrite)
-
-    async def _create_project_role(self, project_role: str) -> None:
-        if self._is_projet_role_created:
-            return
-        try:
-            await self._client.users.add(project_role)
-        except AuthorizationError:
-            pass
-            # We have no permissions to create role --
-            # assume that this is shared project and
-            # current user is not the owner
-        except IllegalArgumentError as e:
-            if "already exists" not in str(e):
-                raise
-        self._is_projet_role_created = True
-
-    async def _add_storage_resource(self, uri: URL) -> None:
-        uri = self._client.parse.normalize_uri(
-            uri,
-            allowed_schemes=("storage",),
-        )
-
-    async def _add_resource(self, uri: URL) -> None:
-        assert self._flow is not None
-        project_role = self._flow.project.role
-        if project_role is None:
-            return
-        await self._create_project_role(project_role)
-        permission = Permission(uri, Action.WRITE)
-        try:
-            await self._client.users.share(project_role, permission)
-        except ValueError:
-            self._console.print(f"[red]Cannot share [b]{uri!s}[/b]")
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/parser.py` & `neuro-flow-23.7.0/src/neuro_flow/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1494,14 +1494,15 @@
         Composer.__init__(self)
         BaseConstructor.__init__(self)
         BaseResolver.__init__(self)
 
 
 PROJECT = {
     "id": SimpleIdExpr,
+    "project_name": SimpleOptStrExpr,
     "owner": SimpleOptStrExpr,
     "role": SimpleOptStrExpr,
     "images": None,
     "volumes": None,
     "defaults": None,
     "mixins": None,
 }
@@ -1607,14 +1608,19 @@
         _start=Pos(0, 0, LocalPath("<default>")),
         _end=Pos(0, 0, LocalPath("<default>")),
         id=SimpleIdExpr(
             Pos(0, 0, LocalPath("<default>")),
             Pos(0, 0, LocalPath("<default>")),
             project_id,
         ),
+        project_name=SimpleOptStrExpr(
+            Pos(0, 0, LocalPath("<default>")),
+            Pos(0, 0, LocalPath("<default>")),
+            None,
+        ),
         owner=SimpleOptStrExpr(
             Pos(0, 0, LocalPath("<default>")),
             Pos(0, 0, LocalPath("<default>")),
             None,
         ),
         role=SimpleOptStrExpr(
             Pos(0, 0, LocalPath("<default>")),
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/storage/api.py` & `neuro-flow-23.7.0/src/neuro_flow/storage/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 def _parse_project_payload(data: Mapping[str, Any]) -> Project:
     return Project(
         id=data["id"],
         yaml_id=data["name"],
         owner=data["owner"],
         cluster=data["cluster"],
         org_name=data["org_name"],
+        project_name=data["project_name"],
     )
 
 
 def _parse_live_job_payload(data: Mapping[str, Any]) -> LiveJob:
     return LiveJob(
         id=data["id"],
         yaml_id=data["yaml_id"],
@@ -337,71 +338,88 @@
         self._raw_client = RawApiClient(client)
 
     def with_retry_read(self) -> Storage:
         return ApiStorage(
             self._client, _raw_client=RetryingReadRawApiClient(self._client)
         )
 
-    def check_can_create_for_owner(self, owner: str) -> None:
-        if owner != self._client.config.username:
+    def check_can_create_for_project_name(self, project_name: str) -> None:
+        if project_name != self._client.config.project_name_or_raise:
             raise ValueError(
-                f"Cannot create project with owner '{owner}' that is"
-                f" different from current user '{self._client.config.username}'."
+                f"Cannot create flow within project '{project_name}' that is"
+                f" different from current project '{self._client.config.project_name}'."
             )
 
     async def close(self) -> None:
         pass
 
     def project(
         self,
         *,
         id: Optional[str] = None,
+        project_name: Optional[str] = None,
         owner: Optional[str] = None,
         yaml_id: Optional[str] = None,
         cluster: Optional[str] = None,
         org_name: Optional[str] = None,
     ) -> "ProjectStorage":
         cluster = cluster or self._cluster_name
         org_name = org_name or self._org_name
         owner = owner or self._client.config.username
+        project_name = project_name or self._client.config.project_name_or_raise
+
         if id:
             return ApiProjectStorage(self._raw_client, id=id)
         else:
             assert yaml_id
             return ApiProjectStorage(
                 self._raw_client,
                 args=dict(
-                    yaml_id=yaml_id, cluster=cluster, org_name=org_name, owner=owner
+                    yaml_id=yaml_id,
+                    cluster=cluster,
+                    org_name=org_name,
+                    owner=owner,
+                    project_name=project_name,
                 ),
             )
 
     async def create_project(
         self,
         yaml_id: str,
+        project_name: str,
         cluster: Optional[str] = None,
         org_name: Optional[str] = None,
     ) -> Project:
         return await self._raw_client.create(
             "flow/projects",
             data={
                 "name": yaml_id,
+                "project_name": project_name,
                 "cluster": cluster or self._cluster_name,
                 "org_name": org_name or self._org_name,
             },
             mapper=_parse_project_payload,
         )
 
     def list_projects(
-        self, name: Optional[str] = None, cluster: Optional[str] = None
+        self,
+        name: Optional[str] = None,
+        cluster: Optional[str] = None,
+        project_name: Optional[str] = None,
+        org_name: Optional[str] = None,
     ) -> AsyncIterator[Project]:
         params = []
         if name is not None:
             params += [("name", name)]
         if cluster is not None:
             params += [("cluster", cluster)]
+        if project_name is not None:
+            params += [("project_name", project_name)]
+        if org_name is not None:
+            params += [("org_name", org_name)]
         return self._raw_client.list("flow/projects", _parse_project_payload, params)
 
     def bake(self, *, id: str) -> "BakeStorage":
         return ApiBakeStorage(self._raw_client, id=id)
 
 
 E = TypeVar("E")
@@ -426,14 +444,15 @@
 
 
 class ProjectInitArgs(TypedDict):
     yaml_id: str
     cluster: str
     org_name: Optional[str]
     owner: str
+    project_name: str
 
 
 class ApiProjectStorage(DeferredIdMixin[Project, ProjectInitArgs], ProjectStorage):
     @overload
     def __init__(self, raw_client: RawApiClient, *, id: str):
         pass
 
@@ -458,14 +477,15 @@
         self._args = args
 
     async def _retrieve_id(self, args: ProjectInitArgs) -> Tuple[str, Project]:
         params = {
             "name": args["yaml_id"],
             "cluster": args["cluster"],
             "owner": args["owner"],
+            "project_name": args["project_name"],
         }
         org_name = args.get("org_name")
         if org_name:
             params["org_name"] = org_name
         project = await self._raw_client.get(
             "flow/projects/by_name", _parse_project_payload, params=params
         )
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/storage/base.py` & `neuro-flow-23.7.0/src/neuro_flow/storage/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 @dataclass(frozen=True)
 class Project:
     id: str
     yaml_id: str
     owner: str
     cluster: str
     org_name: str
+    project_name: str  # in platform scope, not neuro-flow
 
 
 @dataclass(frozen=True)
 class LiveJob:
     id: str
     yaml_id: str
     project_id: str
@@ -160,15 +161,15 @@
         self,
         exc_typ: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         await self.close()
 
-    def check_can_create_for_owner(self, owner: str) -> None:
+    def check_can_create_for_project_name(self, project_name: str) -> None:
         pass
 
     @abc.abstractmethod
     def with_retry_read(self) -> "Storage":
         pass
 
     @abc.abstractmethod
@@ -180,63 +181,77 @@
         pass
 
     @overload
     def project(
         self,
         *,
         yaml_id: str,
+        project_name: Optional[str] = None,
         owner: Optional[str] = None,
         cluster: Optional[str] = None,
         org_name: Optional[str] = None,
     ) -> "ProjectStorage":
         pass
 
     @abc.abstractmethod
     def project(
         self,
         *,
         id: Optional[str] = None,
         yaml_id: Optional[str] = None,
+        project_name: Optional[str] = None,
         cluster: Optional[str] = None,
         org_name: Optional[str] = None,
         owner: Optional[str] = None,
     ) -> "ProjectStorage":
         pass
 
     @abc.abstractmethod
     def bake(self, *, id: str) -> "BakeStorage":
         pass
 
     @abc.abstractmethod
     async def create_project(
-        self, yaml_id: str, cluster: Optional[str] = None
+        self,
+        yaml_id: str,
+        project_name: str,
+        cluster: Optional[str] = None,
+        org_name: Optional[str] = None,
     ) -> Project:
         pass
 
     @abc.abstractmethod
     def list_projects(
-        self, name: Optional[str] = None, cluster: Optional[str] = None
+        self,
+        name: Optional[str] = None,
+        cluster: Optional[str] = None,
+        project_name: Optional[str] = None,
+        org_name: Optional[str] = None,
     ) -> AsyncIterator[Project]:
         pass
 
     async def get_or_create_project(
         self,
         yaml_id: str,
+        project_name: str,
         cluster: Optional[str] = None,
         org_name: Optional[str] = None,
         owner: Optional[str] = None,
     ) -> Project:
         try:
             return await self.project(
-                yaml_id=yaml_id, cluster=cluster, org_name=org_name, owner=owner
+                yaml_id=yaml_id,
+                cluster=cluster,
+                org_name=org_name,
+                owner=owner,
+                project_name=project_name,
             ).get()
         except ResourceNotFound:
-            if owner is not None:
-                self.check_can_create_for_owner(owner)
-            return await self.create_project(yaml_id, cluster)
+            self.check_can_create_for_project_name(project_name)
+            return await self.create_project(yaml_id, project_name, cluster, org_name)
 
 
 class ProjectStorage(abc.ABC):
     @abc.abstractmethod
     async def get(self) -> Project:
         pass
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/storage/in_memory.py` & `neuro-flow-23.7.0/src/neuro_flow/storage/in_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,76 +65,91 @@
 
 class InMemoryStorage(Storage):
     def __init__(
         self,
         owner: str = "in_memory_owner",
         cluster: str = "in_memory_cluster",
         org_name: str = "in_memory_org",
+        project_name: str = "in_memory_project",
     ):
         self._owner = owner
         self._cluster = cluster
         self._org_name = org_name
+        self._project_name = project_name
         self._db = InMemoryDB()
 
     def with_retry_read(self) -> "Storage":
         return self  # In memory read cannot fail
 
     async def close(self) -> None:
         pass
 
     def project(
         self,
         *,
         id: Optional[str] = None,
+        project_name: Optional[str] = None,
         yaml_id: Optional[str] = None,
         cluster: Optional[str] = None,
         org_name: Optional[str] = None,
         owner: Optional[str] = None,
     ) -> "ProjectStorage":
         if id:
             return InMemoryProjectStorage(id, self._db)
         cluster = cluster or self._cluster
         org_name = org_name or self._org_name
+        project_name = project_name or self._project_name
         for project in self._db.projects.values():
             if (
                 project.yaml_id == yaml_id
                 and project.cluster == cluster
                 and project.org_name == org_name
                 and (owner is None or project.owner == owner)
+                and project.project_name == project_name
             ):
                 return InMemoryProjectStorage(project.id, self._db)
         return InMemoryProjectStorage("fake-id", self._db)
 
     def bake(self, *, id: str) -> "BakeStorage":
         return InMemoryBakeStorage(id, self._db)
 
     async def create_project(
         self,
         yaml_id: str,
+        project_name: str,
         cluster: Optional[str] = None,
         org_name: Optional[str] = None,
     ) -> Project:
         project = Project(
             id=_make_id(),
+            project_name=project_name,
             yaml_id=yaml_id,
             cluster=cluster or self._cluster,
             owner=self._owner,
             org_name=org_name or self._org_name,
         )
         self._db.projects[project.id] = project
         return project
 
     async def list_projects(
-        self, name: Optional[str] = None, cluster: Optional[str] = None
+        self,
+        name: Optional[str] = None,
+        cluster: Optional[str] = None,
+        project_name: Optional[str] = None,
+        org_name: Optional[str] = None,
     ) -> AsyncIterator[Project]:
         for project in self._db.projects.values():
             if name and project.yaml_id != name:
                 continue
             if cluster and project.cluster != cluster:
                 continue
+            if project_name and project.project_name != project_name:
+                continue
+            if org_name and project.org_name != org_name:
+                continue
             yield project
 
 
 class InMemoryProjectStorage(ProjectStorage):
     def __init__(self, project_id: str, db: InMemoryDB) -> None:
         self._project_id = project_id
         self._db = db
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/tokenizer.py` & `neuro-flow-23.7.0/src/neuro_flow/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
     def __str__(self) -> str:
         s = "cannot tokenize data"
         return f'{s}: {self.place.line},{self.place.col}: "{self.msg}"'
 
 
 class Tokenizer:
-
     TOKENS = [
         ("LTMPL", r"\$\{\{"),
         ("RTMPL", r"\}\}"),
         ("LTMPL2", r"\$\[\["),
         ("RTMPL2", r"\]\]"),
         ("SPACE", r"[ \t]+"),
         ("NONE", r"None"),
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/types.py` & `neuro-flow-23.7.0/src/neuro_flow/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return cls.instance
 
 
 class TaskStatus(str, enum.Enum):
     # Almost copy of neuro_sdk.JobStatus, but adds new SKIPPED state
 
     def __rich__(self) -> str:
-        return f"[{COLORS[self]}]{self}"
+        return f"[{COLORS[self]}]{self.value}"
 
     UNKNOWN = "unknown"
     PENDING = "pending"
     RUNNING = "running"
     SUCCEEDED = "succeeded"
     FAILED = "failed"
     CANCELLED = "cancelled"
@@ -84,15 +84,15 @@
     PENDING = "pending"
     BUILDING = "building"
     BUILT = "built"
     BUILD_FAILED = "build_failed"
     CACHED = "cached"
 
     def __rich__(self) -> str:
-        return f"[{IMAGE_STATUS_COLORS[self]}]{self}"
+        return f"[{IMAGE_STATUS_COLORS[self]}]{self.value}"
 
 
 IMAGE_STATUS_COLORS = {
     ImageStatus.PENDING: "cyan",
     ImageStatus.BUILDING: "blue",
     ImageStatus.BUILT: "green",
     ImageStatus.BUILD_FAILED: "red",
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow/utils.py` & `neuro-flow-23.7.0/src/neuro_flow/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-flow-22.8.1/src/neuro_flow.egg-info/PKG-INFO` & `neuro-flow-23.7.0/src/neuro_flow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: neuro-flow
-Version: 22.8.1
+Version: 23.7.0
 Summary: Pipelines system for neu.ro
 Home-page: https://github.com/neuro-inc/neuro-flow
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Getting started
 
 `neuro-flow` is a tool that simplifies daily jobs on the Neu.ro platform.
```

### Comparing `neuro-flow-22.8.1/src/neuro_flow.egg-info/SOURCES.txt` & `neuro-flow-23.7.0/src/neuro_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

