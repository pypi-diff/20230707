# Comparing `tmp/zit-0.0.2a8.tar.gz` & `tmp/zit-0.0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zit-0.0.2a8.tar", max compression
+gzip compressed data, was "zit-0.0.2a9.tar", max compression
```

## Comparing `zit-0.0.2a8.tar` & `zit-0.0.2a9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      986 2023-07-07 05:50:41.559582 zit-0.0.2a8/pyproject.toml
--rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.2a8/zit/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.2a8/zit/auth.py
--rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.2a8/zit/config.py
--rw-r--r--   0        0        0     8180 2023-07-04 08:17:13.827602 zit-0.0.2a8/zit/dashboard.py
--rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.2a8/zit/dataset/__init__.py
--rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.2a8/zit/dataset/build.py
--rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.2a8/zit/dataset/classification.py
--rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.2a8/zit/dataset/convert.py
--rw-r--r--   0        0        0     1363 2023-07-03 13:39:04.584358 zit-0.0.2a8/zit/dataset/detection.py
--rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.2a8/zit/dataset/factory.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.2a8/zit/dataset/keypoints.py
--rw-r--r--   0        0        0    15732 2023-06-18 22:35:18.479099 zit-0.0.2a8/zit/dataset/manager.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.2a8/zit/dataset/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.2a8/zit/dataset/segmentation.py
--rw-r--r--   0        0        0    10862 2023-07-07 05:43:26.259723 zit-0.0.2a8/zit/formula.py
--rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.2a8/zit/main.py
--rw-r--r--   0        0        0      670 2023-06-28 06:34:04.531830 zit-0.0.2a8/zit/routes/__init__.py
--rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.2a8/zit/routes/dataset/annotations.py
--rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.2a8/zit/routes/dataset/categories.py
--rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.2a8/zit/routes/dataset/images.py
--rw-r--r--   0        0        0     2126 2023-06-28 09:53:59.159211 zit-0.0.2a8/zit/routes/dataset/queries.py
--rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.2a8/zit/utils.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 zit-0.0.2a8/setup.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 zit-0.0.2a8/PKG-INFO
+-rw-r--r--   0        0        0      986 2023-07-07 09:10:40.605729 zit-0.0.2a9/pyproject.toml
+-rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.2a9/zit/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.2a9/zit/auth.py
+-rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.2a9/zit/config.py
+-rw-r--r--   0        0        0     8184 2023-07-07 09:09:33.325754 zit-0.0.2a9/zit/dashboard.py
+-rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.2a9/zit/dataset/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.2a9/zit/dataset/build.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.2a9/zit/dataset/classification.py
+-rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.2a9/zit/dataset/convert.py
+-rw-r--r--   0        0        0     1363 2023-07-03 13:39:04.584358 zit-0.0.2a9/zit/dataset/detection.py
+-rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.2a9/zit/dataset/factory.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.2a9/zit/dataset/keypoints.py
+-rw-r--r--   0        0        0    15732 2023-06-18 22:35:18.479099 zit-0.0.2a9/zit/dataset/manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.2a9/zit/dataset/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.2a9/zit/dataset/segmentation.py
+-rw-r--r--   0        0        0    10862 2023-07-07 05:43:26.259723 zit-0.0.2a9/zit/formula.py
+-rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.2a9/zit/main.py
+-rw-r--r--   0        0        0      670 2023-06-28 06:34:04.531830 zit-0.0.2a9/zit/routes/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.2a9/zit/routes/dataset/annotations.py
+-rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.2a9/zit/routes/dataset/categories.py
+-rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.2a9/zit/routes/dataset/images.py
+-rw-r--r--   0        0        0     2126 2023-06-28 09:53:59.159211 zit-0.0.2a9/zit/routes/dataset/queries.py
+-rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.2a9/zit/utils.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 zit-0.0.2a9/setup.py
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 zit-0.0.2a9/PKG-INFO
```

### Comparing `zit-0.0.2a8/pyproject.toml` & `zit-0.0.2a9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zit"
-version = "0.0.2a8"
+version = "0.0.2a9"
 description = "ZitySpace CLI tool"
 authors = ["Rui Zheng <rui@zityspace.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = "^6.0"
@@ -46,10 +46,10 @@
 
 [tool.isort]
 profile = "black"
 skip = ["dist"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.2a8"
+version = "0.0.2a9"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
```

### Comparing `zit-0.0.2a8/zit/auth.py` & `zit-0.0.2a9/zit/auth.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/config.py` & `zit-0.0.2a9/zit/config.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/dashboard.py` & `zit-0.0.2a9/zit/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
 def check_and_install_poetry():
     try:
         # Check if poetry is already installed
         run_subprocess(["poetry", "--version"], cwd=None, capture_stdout=False)
         logger.info("Poetry is already installed.")
-    except SubprocessError:
+    except FileNotFoundError:
         yes = typer.prompt("Poetry not found. Do you want to install it?", type=bool)
         if not yes:
             logger.info('Please install poetry manually and re-run "zit dashboard install".')
 
         # Check the Python version
         major_version = sys.version_info.major
         minor_version = sys.version_info.minor
@@ -106,15 +106,15 @@
     if not has_npm():
         logger.info('NPM is not installed. Please install Node.js and NPM manually and re-run "zit dashboard install".')
         return
 
     try:
         run_subprocess(["pnpm", "--version"], cwd=None, capture_stdout=False)
         logger.info("pnpm is already installed.")
-    except SubprocessError:
+    except FileNotFoundError:
         logger.info("pnpm not found. Installing pnpm...")
         install_command = "npm install -g pnpm"
 
         try:
             run_subprocess(install_command, cwd=None, shell=True)
             logger.info("pnpm has been installed successfully.")
         except SubprocessError as e:
```

### Comparing `zit-0.0.2a8/zit/dataset/convert.py` & `zit-0.0.2a9/zit/dataset/convert.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/dataset/detection.py` & `zit-0.0.2a9/zit/dataset/detection.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/dataset/manager.py` & `zit-0.0.2a9/zit/dataset/manager.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/formula.py` & `zit-0.0.2a9/zit/formula.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/main.py` & `zit-0.0.2a9/zit/main.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/routes/__init__.py` & `zit-0.0.2a9/zit/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/routes/dataset/annotations.py` & `zit-0.0.2a9/zit/routes/dataset/annotations.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/routes/dataset/categories.py` & `zit-0.0.2a9/zit/routes/dataset/categories.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/routes/dataset/images.py` & `zit-0.0.2a9/zit/routes/dataset/images.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/zit/routes/dataset/queries.py` & `zit-0.0.2a9/zit/routes/dataset/queries.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a8/setup.py` & `zit-0.0.2a9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'websocket-client>=1.5.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['zit = zit.main:app']}
 
 setup_kwargs = {
     'name': 'zit',
-    'version': '0.0.2a8',
+    'version': '0.0.2a9',
     'description': 'ZitySpace CLI tool',
     'long_description': 'None',
     'author': 'Rui Zheng',
     'author_email': 'rui@zityspace.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zit-0.0.2a8/PKG-INFO` & `zit-0.0.2a9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zit
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: ZitySpace CLI tool
 License: MIT
 Author: Rui Zheng
 Author-email: rui@zityspace.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

