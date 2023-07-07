# Comparing `tmp/flask_management-0.1.4.tar.gz` & `tmp/flask_management-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_management-0.1.4.tar", max compression
+gzip compressed data, was "flask_management-0.1.5.tar", max compression
```

## Comparing `flask_management-0.1.4.tar` & `flask_management-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-05-15 07:20:16.429166 flask_management-0.1.4/LICENSE
--rw-r--r--   0        0        0      186 2023-05-15 08:04:24.922081 flask_management-0.1.4/README.md
--rw-r--r--   0        0        0       45 2023-05-15 07:20:44.714318 flask_management-0.1.4/flask_management/__main__.py
--rw-r--r--   0        0        0      659 2023-05-15 07:20:44.699986 flask_management-0.1.4/flask_management/constants.py
--rw-r--r--   0        0        0     1102 2023-05-15 07:20:44.703599 flask_management-0.1.4/flask_management/context.py
--rw-r--r--   0        0        0     1318 2023-05-15 08:09:53.291424 flask_management-0.1.4/flask_management/main.py
--rw-r--r--   0        0        0        0 2023-05-15 07:20:44.704460 flask_management-0.1.4/flask_management/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 07:20:44.705010 flask_management-0.1.4/flask_management/templates/project/__init__.py
--rw-r--r--   0        0        0      344 2023-05-15 07:20:44.705440 flask_management-0.1.4/flask_management/templates/project/cookiecutter.json
--rw-r--r--   0        0        0     2058 2023-05-15 07:20:44.712954 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore
--rw-r--r--   0        0        0       25 2023-05-15 07:20:44.712191 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/README.md
--rw-r--r--   0        0        0      702 2023-05-17 07:36:14.503897 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml
--rw-r--r--   0        0        0      283 2023-05-15 07:20:44.713408 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-15 07:20:44.711861 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/tests/__init__.py
--rw-r--r--   0        0        0      418 2023-05-15 07:20:44.708330 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/__init__.py
--rw-r--r--   0        0        0      206 2023-05-15 07:20:44.706995 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/app_settings.py
--rw-r--r--   0        0        0      163 2023-05-15 08:09:53.286874 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/__init__.py
--rw-r--r--   0        0        0      120 2023-05-15 07:20:44.709994 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/api.py
--rw-r--r--   0        0        0      278 2023-05-15 07:20:44.710804 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/ext.py
--rw-r--r--   0        0        0      414 2023-05-15 07:20:44.707497 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/models.py
--rw-r--r--   0        0        0      216 2023-05-15 07:20:44.706410 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/signals.py
--rw-r--r--   0        0        0       78 2023-05-15 07:20:44.712473 flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.env }}
--rw-r--r--   0        0        0      673 2023-05-17 07:36:53.851084 flask_management-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 flask_management-0.1.4/setup.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 flask_management-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 07:20:16.429166 flask_management-0.1.5/LICENSE
+-rw-r--r--   0        0        0      300 2023-07-07 06:18:16.501228 flask_management-0.1.5/README.md
+-rw-r--r--   0        0        0       45 2023-05-15 07:20:44.714318 flask_management-0.1.5/flask_management/__main__.py
+-rw-r--r--   0        0        0      659 2023-05-15 07:20:44.699986 flask_management-0.1.5/flask_management/constants.py
+-rw-r--r--   0        0        0     1102 2023-05-15 07:20:44.703599 flask_management-0.1.5/flask_management/context.py
+-rw-r--r--   0        0        0     1318 2023-05-15 08:09:53.291424 flask_management-0.1.5/flask_management/main.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:20:44.704460 flask_management-0.1.5/flask_management/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:20:44.705010 flask_management-0.1.5/flask_management/templates/project/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-15 07:20:44.705440 flask_management-0.1.5/flask_management/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0     2058 2023-05-15 07:20:44.712954 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore
+-rw-r--r--   0        0        0       25 2023-05-15 07:20:44.712191 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/README.md
+-rw-r--r--   0        0        0      702 2023-05-17 07:36:14.503897 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-05-15 07:20:44.713408 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-15 07:20:44.711861 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/tests/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-15 07:20:44.708330 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-15 07:20:44.706995 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/app_settings.py
+-rw-r--r--   0        0        0      163 2023-05-15 08:09:53.286874 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-15 07:20:44.709994 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/book/api.py
+-rw-r--r--   0        0        0      278 2023-05-15 07:20:44.710804 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/ext.py
+-rw-r--r--   0        0        0      414 2023-05-15 07:20:44.707497 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/models.py
+-rw-r--r--   0        0        0      216 2023-05-15 07:20:44.706410 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.app_name }}/signals.py
+-rw-r--r--   0        0        0       78 2023-05-15 07:20:44.712473 flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/{{ cookiecutter.env }}
+-rw-r--r--   0        0        0      673 2023-07-07 06:18:47.622598 flask_management-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 flask_management-0.1.5/PKG-INFO
```

### Comparing `flask_management-0.1.4/LICENSE` & `flask_management-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.4/flask_management/constants.py` & `flask_management-0.1.5/flask_management/constants.py`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.4/flask_management/context.py` & `flask_management-0.1.5/flask_management/context.py`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.4/flask_management/main.py` & `flask_management-0.1.5/flask_management/main.py`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore` & `flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.4/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml` & `flask_management-0.1.5/flask_management/templates/project/{{ cookiecutter.folder_name }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_management-0.1.4/pyproject.toml` & `flask_management-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-management"
-version = "0.1.4"
+version = "0.1.5"
 description = "create the flask project quickly."
 authors = ["huangsong <huangsong@leyantech.com>"]
 readme = "README.md"
 packages = [{ include = "flask_management" }]
 homepage = "https://github.com/ponytailer/flask-management"
 
 [[tool.poetry.source]]
```

### Comparing `flask_management-0.1.4/PKG-INFO` & `flask_management-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-management
-Version: 0.1.4
+Version: 0.1.5
 Summary: create the flask project quickly.
 Home-page: https://github.com/ponytailer/flask-management
 Author: huangsong
 Author-email: huangsong@leyantech.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,14 +14,17 @@
 Requires-Dist: cookiecutter (>=1.7.2)
 Requires-Dist: pydantic[email] (>=1.7.2)
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # flask-management
 
+![flask-management Actions](https://api.meercode.io/badge/ponytailer/flask-management?type=ci-score&lastDay=14)
+
 ## How to use :
 
 - simple command: `flaskapi your-project-name`
 
 - choose your python version: `flaskapi your-project-name --python 3.7`
 
 Inspired by `manage-fastapi`
+
```

