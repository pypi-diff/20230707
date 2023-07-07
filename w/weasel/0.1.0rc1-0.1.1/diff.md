# Comparing `tmp/weasel-0.1.0rc1.tar.gz` & `tmp/weasel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasel-0.1.0rc1.tar", last modified: Mon Jun  5 16:25:14 2023, max compression
+gzip compressed data, was "weasel-0.1.1.tar", last modified: Fri Jul  7 07:38:14 2023, max compression
```

## Comparing `weasel-0.1.0rc1.tar` & `weasel-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:14.142004 weasel-0.1.0rc1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)     4048 2023-06-05 16:25:14.142004 weasel-0.1.0rc1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3014 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      403 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1379 2023-06-05 16:25:14.142004 weasel-0.1.0rc1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:14.134003 weasel-0.1.0rc1/weasel/
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/about.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:14.138003 weasel-0.1.0rc1/weasel/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)      272 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8231 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/assets.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4757 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/clone.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5160 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/document.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8460 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/dvc.py
--rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2934 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/pull.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2764 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/push.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7967 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/remote_storage.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14748 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/cli/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/errors.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4627 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:14.138003 weasel-0.1.0rc1/weasel/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:14.138003 weasel-0.1.0rc1/weasel/tests/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6698 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/cli/test_cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5928 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/cli/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1908 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/cli/test_document.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/cli/test_remote.py
--rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/test_schemas.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5222 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/test_validation.py
--rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:14.142004 weasel-0.1.0rc1/weasel/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/commands.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5778 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)      595 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2796 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/filesystem.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2232 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/frozen.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6419 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/git.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1380 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/hashing.py
--rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/logging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      587 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/modules.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1294 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/remote.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3221 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/validation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2098 2023-06-05 16:25:01.000000 weasel-0.1.0rc1/weasel/util/versions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 16:25:14.138003 weasel-0.1.0rc1/weasel.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     4048 2023-06-05 16:25:14.000000 weasel-0.1.0rc1/weasel.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1117 2023-06-05 16:25:14.000000 weasel-0.1.0rc1/weasel.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 16:25:14.000000 weasel-0.1.0rc1/weasel.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-06-05 16:25:14.000000 weasel-0.1.0rc1/weasel.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-06-05 16:25:14.000000 weasel-0.1.0rc1/weasel.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-06-05 16:25:14.000000 weasel-0.1.0rc1/weasel.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.092214 weasel-0.1.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-07-07 07:38:04.000000 weasel-0.1.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     4055 2023-07-07 07:38:14.092214 weasel-0.1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3024 2023-07-07 07:38:04.000000 weasel-0.1.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      403 2023-07-07 07:38:04.000000 weasel-0.1.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1374 2023-07-07 07:38:14.092214 weasel-0.1.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-07 07:38:04.000000 weasel-0.1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.084215 weasel-0.1.1/weasel/
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/about.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)      272 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8231 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/assets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4757 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5160 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/document.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8460 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/dvc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2934 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/pull.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2764 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/push.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7967 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/remote_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14748 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4627 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel/tests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6698 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5928 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1908 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_document.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_remote.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/test_schemas.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5222 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/test_validation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.092214 weasel-0.1.1/weasel/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5778 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      595 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2796 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2232 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/frozen.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6419 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/git.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1380 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/hashing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      587 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/modules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1294 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/remote.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3221 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/validation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2098 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/versions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4055 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1117 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       42 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/top_level.txt
```

### Comparing `weasel-0.1.0rc1/LICENSE` & `weasel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/PKG-INFO` & `weasel-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel
-Version: 0.1.0rc1
+Version: 0.1.1
 Summary: Weasel: A small and easy workflow system
 Home-page: https://github.com/explosion/weasel/
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/weasel/releases
 Project-URL: Source, https://github.com/explosion/weasel/
@@ -33,15 +33,15 @@
 serving your custom pipelines. You can start off by cloning a pre-defined
 project template, adjust it to fit your needs, load in your data, train a
 pipeline, export it as a Python package, upload your outputs to a remote storage
 and share your results with your team. Weasel can be used via the
 [`weasel`](https://github.com/explosion/weasel/blob/main/docs/cli.md) command and we provide templates in our
 [`projects`](https://github.com/explosion/projects) repo.
 
-![Illustration of project workflow and commands](https://github.com/explosion/weasel/blob/main/docs/assets/images/projects.svg)
+![Illustration of project workflow and commands](https://raw.githubusercontent.com/explosion/weasel/main/docs/assets/images/projects.svg)
 
 ## 💡 Example: Get started with a project template
 
 The easiest way to get started is to clone a project template and run it – for
 example, this [end-to-end template](https://github.com/explosion/projects/tree/v3/pipelines/tagger_parser_ud)
 that lets you train a spaCy **part-of-speech
 tagger** and **dependency parser** on a Universal Dependencies treebank.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: weasel Version: 0.1.0rc1 Summary: Weasel: A small
-and easy workflow system Home-page: https://github.com/explosion/weasel/
-Author: Explosion Author-email: contact@explosion.ai License: MIT Project-URL:
-Release notes, https://github.com/explosion/weasel/releases Project-URL:
-Source, https://github.com/explosion/weasel/ Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Metadata-Version: 2.1 Name: weasel Version: 0.1.1 Summary: Weasel: A small and
+easy workflow system Home-page: https://github.com/explosion/weasel/ Author:
+Explosion Author-email: contact@explosion.ai License: MIT Project-URL: Release
+notes, https://github.com/explosion/weasel/releases Project-URL: Source, https:
+//github.com/explosion/weasel/ Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering Description-Content-
 Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/img/
@@ -17,19 +17,19 @@
 orchestrate training, packaging and serving your custom pipelines. You can
 start off by cloning a pre-defined project template, adjust it to fit your
 needs, load in your data, train a pipeline, export it as a Python package,
 upload your outputs to a remote storage and share your results with your team.
 Weasel can be used via the [`weasel`](https://github.com/explosion/weasel/blob/
 main/docs/cli.md) command and we provide templates in our [`projects`](https://
 github.com/explosion/projects) repo. ![Illustration of project workflow and
-commands](https://github.com/explosion/weasel/blob/main/docs/assets/images/
-projects.svg) ## ð¡ Example: Get started with a project template The easiest
-way to get started is to clone a project template and run it âÂ for example,
-this [end-to-end template](https://github.com/explosion/projects/tree/v3/
-pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
+commands](https://raw.githubusercontent.com/explosion/weasel/main/docs/assets/
+images/projects.svg) ## ð¡ Example: Get started with a project template The
+easiest way to get started is to clone a project template and run it âÂ for
+example, this [end-to-end template](https://github.com/explosion/projects/tree/
+v3/pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
 tagger** and **dependency parser** on a Universal Dependencies treebank.
 ```shell python -m weasel clone pipelines/tagger_parser_ud ``` > **Note** > >
 Our [`projects`](https://github.com/explosion/projects) repo includes various >
 project templates for different NLP tasks, models, workflows and integrations >
 that you can clone and run. The easiest way to get started is to pick a >
 template, clone it and start modifying it! ## ð Documentation Get started
 with the documentation: - [Learn how to create a Weasel workflow](https://
```

### Comparing `weasel-0.1.0rc1/README.md` & `weasel-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 serving your custom pipelines. You can start off by cloning a pre-defined
 project template, adjust it to fit your needs, load in your data, train a
 pipeline, export it as a Python package, upload your outputs to a remote storage
 and share your results with your team. Weasel can be used via the
 [`weasel`](https://github.com/explosion/weasel/blob/main/docs/cli.md) command and we provide templates in our
 [`projects`](https://github.com/explosion/projects) repo.
 
-![Illustration of project workflow and commands](https://github.com/explosion/weasel/blob/main/docs/assets/images/projects.svg)
+![Illustration of project workflow and commands](https://raw.githubusercontent.com/explosion/weasel/main/docs/assets/images/projects.svg)
 
 ## 💡 Example: Get started with a project template
 
 The easiest way to get started is to clone a project template and run it – for
 example, this [end-to-end template](https://github.com/explosion/projects/tree/v3/pipelines/tagger_parser_ud)
 that lets you train a spaCy **part-of-speech
 tagger** and **dependency parser** on a Universal Dependencies treebank.
```

#### html2text {}

```diff
@@ -3,37 +3,37 @@
 **use cases and domains**, and orchestrate training, packaging and serving your
 custom pipelines. You can start off by cloning a pre-defined project template,
 adjust it to fit your needs, load in your data, train a pipeline, export it as
 a Python package, upload your outputs to a remote storage and share your
 results with your team. Weasel can be used via the [`weasel`](https://
 github.com/explosion/weasel/blob/main/docs/cli.md) command and we provide
 templates in our [`projects`](https://github.com/explosion/projects) repo. !
-[Illustration of project workflow and commands](https://github.com/explosion/
-weasel/blob/main/docs/assets/images/projects.svg) ## ð¡ Example: Get started
-with a project template The easiest way to get started is to clone a project
-template and run it âÂ for example, this [end-to-end template](https://
-github.com/explosion/projects/tree/v3/pipelines/tagger_parser_ud) that lets you
-train a spaCy **part-of-speech tagger** and **dependency parser** on a
-Universal Dependencies treebank. ```shell python -m weasel clone pipelines/
-tagger_parser_ud ``` > **Note** > > Our [`projects`](https://github.com/
-explosion/projects) repo includes various > project templates for different NLP
-tasks, models, workflows and integrations > that you can clone and run. The
-easiest way to get started is to pick a > template, clone it and start
-modifying it! ## ð Documentation Get started with the documentation: -
-[Learn how to create a Weasel workflow](https://github.com/explosion/weasel/
-blob/main/docs/tutorial/workflow.md) - [Working with directory and assets]
-(https://github.com/explosion/weasel/blob/main/docs/tutorial/directory-and-
-assets.md) - [Running custom scripts](https://github.com/explosion/weasel/blob/
-main/docs/tutorial/custom-scripts.md) - [Using remote storage](https://
-github.com/explosion/weasel/blob/main/docs/tutorial/remote-storage.md) -
-[Weasel integrations](https://github.com/explosion/weasel/blob/main/docs/
-tutorial/integrations.md) - [Command line interface description](https://
-github.com/explosion/weasel/blob/main/docs/cli.md) ## Migrating from spaCy
-Projects Weasel is a standalone replacement for spaCy Projects. There are a few
-backward incompatibilities that you should be aware of: - The
+[Illustration of project workflow and commands](https://
+raw.githubusercontent.com/explosion/weasel/main/docs/assets/images/
+projects.svg) ## ð¡ Example: Get started with a project template The easiest
+way to get started is to clone a project template and run it âÂ for example,
+this [end-to-end template](https://github.com/explosion/projects/tree/v3/
+pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
+tagger** and **dependency parser** on a Universal Dependencies treebank.
+```shell python -m weasel clone pipelines/tagger_parser_ud ``` > **Note** > >
+Our [`projects`](https://github.com/explosion/projects) repo includes various >
+project templates for different NLP tasks, models, workflows and integrations >
+that you can clone and run. The easiest way to get started is to pick a >
+template, clone it and start modifying it! ## ð Documentation Get started
+with the documentation: - [Learn how to create a Weasel workflow](https://
+github.com/explosion/weasel/blob/main/docs/tutorial/workflow.md) - [Working
+with directory and assets](https://github.com/explosion/weasel/blob/main/docs/
+tutorial/directory-and-assets.md) - [Running custom scripts](https://
+github.com/explosion/weasel/blob/main/docs/tutorial/custom-scripts.md) - [Using
+remote storage](https://github.com/explosion/weasel/blob/main/docs/tutorial/
+remote-storage.md) - [Weasel integrations](https://github.com/explosion/weasel/
+blob/main/docs/tutorial/integrations.md) - [Command line interface description]
+(https://github.com/explosion/weasel/blob/main/docs/cli.md) ## Migrating from
+spaCy Projects Weasel is a standalone replacement for spaCy Projects. There are
+a few backward incompatibilities that you should be aware of: - The
 `SPACY_CONFIG_OVERRIDES` environment variable is no longer checked. You can set
 configuration overrides using `WEASEL_CONFIG_OVERRIDES`. - Support for the
 `spacy_version` configuration key has been dropped. - Support for
 `SPACY_PROJECT_USE_GIT_VERSION` environment variable has been dropped. - Error
 codes are now Weasel-specific, and do not follow spaCy error codes. Weasel
 checks for the first three incompatibilities and will issue a warning if you're
 using it with spaCy-specific configuration options.
```

### Comparing `weasel-0.1.0rc1/setup.cfg` & `weasel-0.1.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weasel
-version = 0.1.0rc1
+version = 0.1.1
 description = Weasel: A small and easy workflow system
 url = https://github.com/explosion/weasel/
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -36,15 +36,15 @@
 	typer>=0.3.0,<0.8.0
 	pathy>=0.10.0
 	requests>=2.13.0,<3.0.0
 	pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0
 
 [options.entry_points]
 console_scripts = 
-	weasel = weasel._util:app
+	weasel = weasel.cli:app
 
 [mypy]
 ignore_missing_imports = True
 no_implicit_optional = True
 plugins = pydantic.mypy
 allow_redefinition = True
```

### Comparing `weasel-0.1.0rc1/weasel/cli/assets.py` & `weasel-0.1.1/weasel/cli/assets.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/cli/clone.py` & `weasel-0.1.1/weasel/cli/clone.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/cli/document.py` & `weasel-0.1.1/weasel/cli/document.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/cli/dvc.py` & `weasel-0.1.1/weasel/cli/dvc.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/cli/pull.py` & `weasel-0.1.1/weasel/cli/pull.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/cli/push.py` & `weasel-0.1.1/weasel/cli/push.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/cli/remote_storage.py` & `weasel-0.1.1/weasel/cli/remote_storage.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/cli/run.py` & `weasel-0.1.1/weasel/cli/run.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/errors.py` & `weasel-0.1.1/weasel/errors.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/schemas.py` & `weasel-0.1.1/weasel/schemas.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/tests/cli/test_cli.py` & `weasel-0.1.1/weasel/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/tests/cli/test_cli_app.py` & `weasel-0.1.1/weasel/tests/cli/test_cli_app.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/tests/cli/test_document.py` & `weasel-0.1.1/weasel/tests/cli/test_document.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/tests/cli/test_remote.py` & `weasel-0.1.1/weasel/tests/cli/test_remote.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/tests/test_schemas.py` & `weasel-0.1.1/weasel/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/tests/test_validation.py` & `weasel-0.1.1/weasel/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/tests/util.py` & `weasel-0.1.1/weasel/tests/util.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/__init__.py` & `weasel-0.1.1/weasel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/commands.py` & `weasel-0.1.1/weasel/util/commands.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/config.py` & `weasel-0.1.1/weasel/util/config.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/environment.py` & `weasel-0.1.1/weasel/util/environment.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/filesystem.py` & `weasel-0.1.1/weasel/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/frozen.py` & `weasel-0.1.1/weasel/util/frozen.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/git.py` & `weasel-0.1.1/weasel/util/git.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/hashing.py` & `weasel-0.1.1/weasel/util/hashing.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/modules.py` & `weasel-0.1.1/weasel/util/modules.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/remote.py` & `weasel-0.1.1/weasel/util/remote.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/validation.py` & `weasel-0.1.1/weasel/util/validation.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel/util/versions.py` & `weasel-0.1.1/weasel/util/versions.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.0rc1/weasel.egg-info/PKG-INFO` & `weasel-0.1.1/weasel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel
-Version: 0.1.0rc1
+Version: 0.1.1
 Summary: Weasel: A small and easy workflow system
 Home-page: https://github.com/explosion/weasel/
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/weasel/releases
 Project-URL: Source, https://github.com/explosion/weasel/
@@ -33,15 +33,15 @@
 serving your custom pipelines. You can start off by cloning a pre-defined
 project template, adjust it to fit your needs, load in your data, train a
 pipeline, export it as a Python package, upload your outputs to a remote storage
 and share your results with your team. Weasel can be used via the
 [`weasel`](https://github.com/explosion/weasel/blob/main/docs/cli.md) command and we provide templates in our
 [`projects`](https://github.com/explosion/projects) repo.
 
-![Illustration of project workflow and commands](https://github.com/explosion/weasel/blob/main/docs/assets/images/projects.svg)
+![Illustration of project workflow and commands](https://raw.githubusercontent.com/explosion/weasel/main/docs/assets/images/projects.svg)
 
 ## 💡 Example: Get started with a project template
 
 The easiest way to get started is to clone a project template and run it – for
 example, this [end-to-end template](https://github.com/explosion/projects/tree/v3/pipelines/tagger_parser_ud)
 that lets you train a spaCy **part-of-speech
 tagger** and **dependency parser** on a Universal Dependencies treebank.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: weasel Version: 0.1.0rc1 Summary: Weasel: A small
-and easy workflow system Home-page: https://github.com/explosion/weasel/
-Author: Explosion Author-email: contact@explosion.ai License: MIT Project-URL:
-Release notes, https://github.com/explosion/weasel/releases Project-URL:
-Source, https://github.com/explosion/weasel/ Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Metadata-Version: 2.1 Name: weasel Version: 0.1.1 Summary: Weasel: A small and
+easy workflow system Home-page: https://github.com/explosion/weasel/ Author:
+Explosion Author-email: contact@explosion.ai License: MIT Project-URL: Release
+notes, https://github.com/explosion/weasel/releases Project-URL: Source, https:
+//github.com/explosion/weasel/ Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering Description-Content-
 Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/img/
@@ -17,19 +17,19 @@
 orchestrate training, packaging and serving your custom pipelines. You can
 start off by cloning a pre-defined project template, adjust it to fit your
 needs, load in your data, train a pipeline, export it as a Python package,
 upload your outputs to a remote storage and share your results with your team.
 Weasel can be used via the [`weasel`](https://github.com/explosion/weasel/blob/
 main/docs/cli.md) command and we provide templates in our [`projects`](https://
 github.com/explosion/projects) repo. ![Illustration of project workflow and
-commands](https://github.com/explosion/weasel/blob/main/docs/assets/images/
-projects.svg) ## ð¡ Example: Get started with a project template The easiest
-way to get started is to clone a project template and run it âÂ for example,
-this [end-to-end template](https://github.com/explosion/projects/tree/v3/
-pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
+commands](https://raw.githubusercontent.com/explosion/weasel/main/docs/assets/
+images/projects.svg) ## ð¡ Example: Get started with a project template The
+easiest way to get started is to clone a project template and run it âÂ for
+example, this [end-to-end template](https://github.com/explosion/projects/tree/
+v3/pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
 tagger** and **dependency parser** on a Universal Dependencies treebank.
 ```shell python -m weasel clone pipelines/tagger_parser_ud ``` > **Note** > >
 Our [`projects`](https://github.com/explosion/projects) repo includes various >
 project templates for different NLP tasks, models, workflows and integrations >
 that you can clone and run. The easiest way to get started is to pick a >
 template, clone it and start modifying it! ## ð Documentation Get started
 with the documentation: - [Learn how to create a Weasel workflow](https://
```

### Comparing `weasel-0.1.0rc1/weasel.egg-info/SOURCES.txt` & `weasel-0.1.1/weasel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

