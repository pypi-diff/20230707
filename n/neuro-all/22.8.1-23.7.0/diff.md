# Comparing `tmp/neuro-all-22.8.1.tar.gz` & `tmp/neuro_all-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-all-22.8.1.tar", max compression
+gzip compressed data, was "neuro_all-23.7.0.tar", max compression
```

## Comparing `neuro-all-22.8.1.tar` & `neuro_all-23.7.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11357 2022-08-05 11:10:03.149533 neuro-all-22.8.1/LICENSE
--rw-r--r--   0        0        0      107 2022-08-05 11:10:03.149533 neuro-all-22.8.1/README.md
--rw-r--r--   0        0        0      462 2022-08-05 11:10:03.149533 neuro-all-22.8.1/neuro_all/__init__.py
--rw-r--r--   0        0        0     1659 2022-08-05 11:10:03.149533 neuro-all-22.8.1/pyproject.toml
--rw-r--r--   0        0        0     1244 2022-08-05 11:10:11.880074 neuro-all-22.8.1/setup.py
--rw-r--r--   0        0        0     1398 2022-08-05 11:10:11.880465 neuro-all-22.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 23:26:30.096095 neuro_all-23.7.0/LICENSE
+-rw-r--r--   0        0        0      107 2023-07-06 23:26:30.096095 neuro_all-23.7.0/README.md
+-rw-r--r--   0        0        0      462 2023-07-06 23:26:30.100096 neuro_all-23.7.0/neuro_all/__init__.py
+-rw-r--r--   0        0        0     1659 2023-07-06 23:26:30.100096 neuro_all-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 neuro_all-23.7.0/PKG-INFO
```

### Comparing `neuro-all-22.8.1/LICENSE` & `neuro_all-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-all-22.8.1/pyproject.toml` & `neuro_all-23.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neuro-all"
-version = "22.8.1"
+version = "23.7.0"
 description = "Combo package for installing all neu.ro command line tools by 'pipx install neuro-all' command"
 authors = ["Neu.ro Team <team@neu.ro>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://neu.ro"
 repository = "https://github.com/neuro-inc/neuro-all"
 keywords = [
@@ -38,21 +38,21 @@
 [tool.poetry.scripts]
 neuro = "neuro_cli.main:main"
 docker-credential-neuro = "neuro_cli.docker_credential_helper:main"
 neuro-extras = "neuro_extras:main"
 neuro-flow = "neuro_flow.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
-neuro-cli = "22.7.1"
-neuro-extras = "22.2.2"
-neuro-flow = "22.8.1"
-certifi = "2022.6.15"
+python = "^3.8.0"
+neuro-cli = "23.7.0"
+neuro-extras = "23.7.0"
+neuro-flow = "23.7.0"
+certifi = "2022.12.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "7.1.2"
-pre-commit = "^2.20.0"
+pytest = "7.2.1"
+pre-commit = "^2.21.0"
 click = "^8.1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `neuro-all-22.8.1/PKG-INFO` & `neuro_all-23.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: neuro-all
-Version: 22.8.1
+Version: 23.7.0
 Summary: Combo package for installing all neu.ro command line tools by 'pipx install neuro-all' command
 Home-page: https://neu.ro
 License: Apache-2.0
 Keywords: neu.ro,mlops
 Author: Neu.ro Team
 Author-email: team@neu.ro
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Dist: certifi (==2022.6.15)
-Requires-Dist: neuro-cli (==22.7.1)
-Requires-Dist: neuro-extras (==22.2.2)
-Requires-Dist: neuro-flow (==22.8.1)
+Requires-Dist: certifi (==2022.12.7)
+Requires-Dist: neuro-cli (==23.7.0)
+Requires-Dist: neuro-extras (==23.7.0)
+Requires-Dist: neuro-flow (==23.7.0)
 Project-URL: Repository, https://github.com/neuro-inc/neuro-all
 Description-Content-Type: text/markdown
 
 # neuro-all
 Combo package for installing all neu.ro command line tools by `pipx install neuro-all` command
```

