# Comparing `tmp/aichat-cli-0.4.9.tar.gz` & `tmp/aichat-cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aichat-cli-0.4.9.tar", last modified: Mon Jun 19 19:10:46 2023, max compression
+gzip compressed data, was "aichat-cli-0.5.0.tar", last modified: Fri Jul  7 17:19:59 2023, max compression
```

## Comparing `aichat-cli-0.4.9.tar` & `aichat-cli-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 19:10:46.432538 aichat-cli-0.4.9/
--rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.9/LICENSE
--rw-rw-rw-   0        0        0     5240 2023-06-19 19:10:46.431538 aichat-cli-0.4.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 19:10:46.430541 aichat-cli-0.4.9/aichat_cli.egg-info/
--rw-rw-rw-   0        0        0     5240 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:10:46.000000 aichat-cli-0.4.9/aichat_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 19:10:46.433540 aichat-cli-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-06-19 19:10:24.000000 aichat-cli-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:19:59.100624 aichat-cli-0.5.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5240 2023-07-07 17:19:59.099620 aichat-cli-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 17:19:59.098613 aichat-cli-0.5.0/aichat_cli.egg-info/
+-rw-rw-rw-   0        0        0     5240 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:19:59.000000 aichat-cli-0.5.0/aichat_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:19:59.100624 aichat-cli-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-07-07 17:19:38.000000 aichat-cli-0.5.0/setup.py
```

### Comparing `aichat-cli-0.4.9/LICENSE` & `aichat-cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aichat-cli-0.4.9/PKG-INFO` & `aichat-cli-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.9
+Version: 0.5.0
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `aichat-cli-0.4.9/aichat_cli.egg-info/PKG-INFO` & `aichat-cli-0.5.0/aichat_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.9
+Version: 0.5.0
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `aichat-cli-0.4.9/setup.py` & `aichat-cli-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="aichat-cli",
-    version="0.4.9",
+    version="0.5.0",
     author="TheLime1",
     license="GPLv3",
     description="A CLI app that allows you to have interactive conversations with different AI bots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

