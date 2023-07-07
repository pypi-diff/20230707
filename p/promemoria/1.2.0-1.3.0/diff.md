# Comparing `tmp/promemoria-1.2.0.tar.gz` & `tmp/promemoria-1.3.0.tar.gz`

## Comparing `promemoria-1.2.0.tar` & `promemoria-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 promemoria-1.2.0/.gitattributes
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 promemoria-1.2.0/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/__main__.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/files.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/git.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/help.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/reminders.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/utilities.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 promemoria-1.2.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 promemoria-1.2.0/LICENSE
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 promemoria-1.2.0/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 promemoria-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 promemoria-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 promemoria-1.3.0/.gitattributes
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 promemoria-1.3.0/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 promemoria-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 promemoria-1.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 promemoria-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 promemoria-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 promemoria-1.3.0/src/promemoria/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 promemoria-1.3.0/src/promemoria/__main__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 promemoria-1.3.0/src/promemoria/files.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 promemoria-1.3.0/src/promemoria/git.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 promemoria-1.3.0/src/promemoria/help.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 promemoria-1.3.0/src/promemoria/reminders.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 promemoria-1.3.0/src/promemoria/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 promemoria-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 promemoria-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 promemoria-1.3.0/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 promemoria-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 promemoria-1.3.0/PKG-INFO
```

### Comparing `promemoria-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `promemoria-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `promemoria-1.2.0/.github/workflows/python-publish.yml` & `promemoria-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `promemoria-1.2.0/src/promemoria/files.py` & `promemoria-1.3.0/src/promemoria/files.py`

 * *Files identical despite different names*

### Comparing `promemoria-1.2.0/src/promemoria/git.py` & `promemoria-1.3.0/src/promemoria/git.py`

 * *Files identical despite different names*

### Comparing `promemoria-1.2.0/src/promemoria/reminders.py` & `promemoria-1.3.0/src/promemoria/reminders.py`

 * *Files identical despite different names*

### Comparing `promemoria-1.2.0/src/promemoria/utilities.py` & `promemoria-1.3.0/src/promemoria/utilities.py`

 * *Files identical despite different names*

### Comparing `promemoria-1.2.0/LICENSE` & `promemoria-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promemoria-1.2.0/README.md` & `promemoria-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 **promemoria** is a Python based tool to help you stay organized and on top of your tasks! Quickly *create reminders in the shell* with the ability to *set a title, description, priority and date* to make sure you never forget anything.
 
 ## Main features
 
 - Create and manage reminders directly from the shell.
 - Import the latest *Issues* and *Pull Requests* as reminders from a public GitHub repository. ![New feature](https://img.shields.io/badge/new-green)
+- Automatically checks for expired reminders when opening a new shell. ![New feature](https://img.shields.io/badge/new-green)
 
 ## Installation
 
 **promemoria** can be installed from [PyPI](https://pypi.org) by:
 
 ```
 python3 -m pip install --upgrade promemoria
@@ -71,14 +72,24 @@
 
 promemoria gh Imports issues and pull requests from GitHub
     -r public repo, string [user/repo].
     -u user, string.
     --pulls Imports pull requests instead of issues.
 ```
 
+## Expired reminders check
+
+The automatic check can be enabled by issuing the following command[^4]:
+
+[^4]: Linux and macOS only, bash and zsh only.
+
+```
+promemoria-check enable
+```
+
 ## Examples
 
 ### Quickly check your reminders
 
 ```
 promemoria
 ```
@@ -116,17 +127,17 @@
 
 ### Import from a GitHub repository
 
 ```
 promemoria gh -r "python/cpython" -u "sobolevn"
 ```
 
-which results[^4] in:
+which results[^5] in:
 
-[^4]: An example from the official [Python](https://github.com/python/cpython) repository.
+[^5]: An example from the official [Python](https://github.com/python/cpython) repository.
 
 ```
 [promemoria]
 
 Imported 1 issue(s).
 ____________________
 
@@ -136,17 +147,17 @@
 
 ### Toggling a reminder
 
 ```
 promemoria toggle -i 1
 ````
 
-which results[^2][^5] in:
+which results[^2][^6] in:
 
-[^5]: The mark changes and the title gets dimmed.
+[^6]: The mark changes and the title gets dimmed.
 
 ```
 [promemoria]
 
 You toggled a reminder.
 -----------------------
```

### Comparing `promemoria-1.2.0/pyproject.toml` & `promemoria-1.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "promemoria"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools", "requests"]
@@ -16,11 +16,12 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 promemoria = "promemoria:main"
+promemoria-check = "promemoria:checker"
 
 [project.urls]
 "Homepage" = "https://github.com/diantonioandrea/promemoria"
 "Bug Tracker" = "https://github.com/diantonioandrea/promemoria/issues"
```

### Comparing `promemoria-1.2.0/PKG-INFO` & `promemoria-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promemoria
-Version: 1.2.0
+Version: 1.3.0
 Project-URL: Homepage, https://github.com/diantonioandrea/promemoria
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/promemoria/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,15 @@
 
 **promemoria** is a Python based tool to help you stay organized and on top of your tasks! Quickly *create reminders in the shell* with the ability to *set a title, description, priority and date* to make sure you never forget anything.
 
 ## Main features
 
 - Create and manage reminders directly from the shell.
 - Import the latest *Issues* and *Pull Requests* as reminders from a public GitHub repository. ![New feature](https://img.shields.io/badge/new-green)
+- Automatically checks for expired reminders when opening a new shell. ![New feature](https://img.shields.io/badge/new-green)
 
 ## Installation
 
 **promemoria** can be installed from [PyPI](https://pypi.org) by:
 
 ```
 python3 -m pip install --upgrade promemoria
@@ -87,14 +88,24 @@
 
 promemoria gh Imports issues and pull requests from GitHub
     -r public repo, string [user/repo].
     -u user, string.
     --pulls Imports pull requests instead of issues.
 ```
 
+## Expired reminders check
+
+The automatic check can be enabled by issuing the following command[^4]:
+
+[^4]: Linux and macOS only, bash and zsh only.
+
+```
+promemoria-check enable
+```
+
 ## Examples
 
 ### Quickly check your reminders
 
 ```
 promemoria
 ```
@@ -132,17 +143,17 @@
 
 ### Import from a GitHub repository
 
 ```
 promemoria gh -r "python/cpython" -u "sobolevn"
 ```
 
-which results[^4] in:
+which results[^5] in:
 
-[^4]: An example from the official [Python](https://github.com/python/cpython) repository.
+[^5]: An example from the official [Python](https://github.com/python/cpython) repository.
 
 ```
 [promemoria]
 
 Imported 1 issue(s).
 ____________________
 
@@ -152,17 +163,17 @@
 
 ### Toggling a reminder
 
 ```
 promemoria toggle -i 1
 ````
 
-which results[^2][^5] in:
+which results[^2][^6] in:
 
-[^5]: The mark changes and the title gets dimmed.
+[^6]: The mark changes and the title gets dimmed.
 
 ```
 [promemoria]
 
 You toggled a reminder.
 -----------------------
```

