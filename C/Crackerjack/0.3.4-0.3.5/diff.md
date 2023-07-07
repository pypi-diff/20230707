# Comparing `tmp/crackerjack-0.3.4.tar.gz` & `tmp/crackerjack-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.4.tar", last modified: Mon Jul  3 01:09:59 2023, max compression
+gzip compressed data, was "crackerjack-0.3.5.tar", last modified: Fri Jul  7 13:14:10 2023, max compression
```

## Comparing `crackerjack-0.3.4.tar` & `crackerjack-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.4/LICENSE
--rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-07-03 01:09:19.930137 crackerjack-0.3.4/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      229 2023-07-03 01:09:19.880908 crackerjack-0.3.4/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-07-03 01:09:19.914538 crackerjack-0.3.4/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2917 2023-07-03 01:09:19.898753 crackerjack-0.3.4/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.4/crackerjack/.pyanalyze-report.json
--rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.4/crackerjack/.pyanalyze-report.md
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.4/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.4/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.4/crackerjack/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.4/crackerjack/__main__.py
--rw-r--r--   0        0        0     6145 2023-06-19 10:49:19.257226 crackerjack-0.3.4/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1657 2023-07-03 01:09:20.698148 crackerjack-0.3.4/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2008 2023-07-03 01:09:59.734847 crackerjack-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 crackerjack-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.5/LICENSE
+-rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 13:13:51.723700 crackerjack-0.3.5/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      229 2023-07-07 13:13:51.674755 crackerjack-0.3.5/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-07-07 13:13:51.707759 crackerjack-0.3.5/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2917 2023-07-07 13:13:51.692103 crackerjack-0.3.5/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.5/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.5/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.5/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.5/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.5/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.5/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6145 2023-06-19 10:49:19.257226 crackerjack-0.3.5/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1659 2023-07-07 13:13:52.445350 crackerjack-0.3.5/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2010 2023-07-07 13:14:10.111259 crackerjack-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.5/PKG-INFO
```

### Comparing `crackerjack-0.3.4/LICENSE` & `crackerjack-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.4/README.md` & `crackerjack-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.4/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.5/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.4/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.5/crackerjack/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         name: check-added-large-files
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.275
+    rev: v0.0.277
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
     rev: v2.6.2
     hooks:
       - id: creosote
         args: [--paths, "crackerjack", --exclude-deps, "pdm-bump", "tomli-w"]
@@ -83,15 +83,15 @@
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.275
+    rev: v0.0.277
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
```

### Comparing `crackerjack-0.3.4/crackerjack/.pyanalyze-report.json` & `crackerjack-0.3.5/crackerjack/.pyanalyze-report.json`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.4/crackerjack/.pyanalyze-report.md` & `crackerjack-0.3.5/crackerjack/.pyanalyze-report.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.4/crackerjack/crackerjack.py` & `crackerjack-0.3.5/crackerjack/crackerjack.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.4/crackerjack/pyproject.toml` & `crackerjack-0.3.5/crackerjack/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.4"
+version = "0.3.5"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -58,18 +58,18 @@
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "click>=8.1.3",
+    "click>=8.1.4",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
-    "pydantic>=2.0",
+    "pydantic>=2.0.2",
     "inflection>=0.5.1",
     "acb>=0.1.10",
     "tomli-w>=1.0.0",
     "pdm-bump>=0.7.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
```

### Comparing `crackerjack-0.3.4/pyproject.toml` & `crackerjack-0.3.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.4"
+version = "0.3.5"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -77,18 +77,18 @@
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "click>=8.1.3",
+    "click>=8.1.4",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
-    "pydantic>=2.0",
+    "pydantic>=2.0.2",
     "inflection>=0.5.1",
     "acb>=0.1.10",
     "tomli-w>=1.0.0",
     "pdm-bump>=0.7.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
```

### Comparing `crackerjack-0.3.4/PKG-INFO` & `crackerjack-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.3.4
+Version: 0.3.5
 Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://github.com/lesleslie/crackerjack
 Project-URL: Documentation, https://github.com/lesleslie/crackerjack
 Project-URL: Repository, https://github.com/lesleslie/crackerjack
 Requires-Python: >=3.11
-Requires-Dist: click>=8.1.3
+Requires-Dist: click>=8.1.4
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: aioconsole>=0.6.1
-Requires-Dist: pydantic>=2.0
+Requires-Dist: pydantic>=2.0.2
 Requires-Dist: inflection>=0.5.1
 Requires-Dist: acb>=0.1.10
 Requires-Dist: tomli-w>=1.0.0
 Requires-Dist: pdm-bump>=0.7.1
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
```

