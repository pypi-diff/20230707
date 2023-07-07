# Comparing `tmp/tt_terminal_translator-0.1.4.tar.gz` & `tmp/tt_terminal_translator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tt_terminal_translator-0.1.4.tar", max compression
+gzip compressed data, was "tt_terminal_translator-0.1.5.tar", max compression
```

## Comparing `tt_terminal_translator-0.1.4.tar` & `tt_terminal_translator-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.4/LICENSE
--rw-r--r--   0        0        0     1895 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.4/README.md
--rw-r--r--   0        0        0     1777 2023-05-22 23:04:34.025626 tt_terminal_translator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2439 2023-05-06 03:14:32.129998 tt_terminal_translator-0.1.4/src/terminal_translator/config.py
--rw-r--r--   0        0        0     2517 2023-05-06 03:14:41.539958 tt_terminal_translator-0.1.4/src/terminal_translator/main.py
--rw-r--r--   0        0        0      359 2023-05-06 03:29:43.733677 tt_terminal_translator-0.1.4/src/terminal_translator/version.py
--rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-07 00:13:37.022649 tt_terminal_translator-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1895 2023-07-07 00:13:37.022649 tt_terminal_translator-0.1.5/README.md
+-rw-r--r--   0        0        0     1777 2023-07-07 00:15:28.772930 tt_terminal_translator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2439 2023-07-07 00:13:37.029316 tt_terminal_translator-0.1.5/src/terminal_translator/config.py
+-rw-r--r--   0        0        0     2517 2023-07-07 00:13:37.029316 tt_terminal_translator-0.1.5/src/terminal_translator/main.py
+-rw-r--r--   0        0        0      359 2023-07-07 00:13:37.029316 tt_terminal_translator-0.1.5/src/terminal_translator/version.py
+-rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.5/PKG-INFO
```

### Comparing `tt_terminal_translator-0.1.4/LICENSE` & `tt_terminal_translator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.4/README.md` & `tt_terminal_translator-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.4/pyproject.toml` & `tt_terminal_translator-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tt-terminal-translator"
-version = "0.1.4"
+version = "0.1.5"
 description = "Terminal Translator is a translation CLI that uses the Google Cloud API. "
 authors = ["gbPagano <guilhermebpagano@gmail.com>"]
 readme = "README.md"
 packages = [{include = "terminal_translator", from = "src"}]
 classifiers = [  
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tt_terminal_translator-0.1.4/src/terminal_translator/config.py` & `tt_terminal_translator-0.1.5/src/terminal_translator/config.py`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.4/src/terminal_translator/main.py` & `tt_terminal_translator-0.1.5/src/terminal_translator/main.py`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.4/PKG-INFO` & `tt_terminal_translator-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: tt-terminal-translator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Terminal Translator is a translation CLI that uses the Google Cloud API. 
 Author: gbPagano
 Author-email: guilhermebpagano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: google-cloud-translate (>=3.11.0,<4.0.0)
 Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

