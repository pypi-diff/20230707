# Comparing `tmp/autopio-0.1.0.tar.gz` & `tmp/autopio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopio-0.1.0.tar", last modified: Thu Jul  6 17:08:42 2023, max compression
+gzip compressed data, was "autopio-0.1.2.tar", last modified: Fri Jul  7 09:53:07 2023, max compression
```

## Comparing `autopio-0.1.0.tar` & `autopio-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:08:42.828410 autopio-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 17:08:28.000000 autopio-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 17:08:42.828410 autopio-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 17:08:28.000000 autopio-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:08:42.828410 autopio-0.1.0/autopio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:08:28.000000 autopio-0.1.0/autopio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:08:42.828410 autopio-0.1.0/autopio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 17:08:42.000000 autopio-0.1.0/autopio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 17:08:42.000000 autopio-0.1.0/autopio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:08:42.000000 autopio-0.1.0/autopio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 17:08:42.000000 autopio-0.1.0/autopio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 17:08:42.000000 autopio-0.1.0/autopio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-06 17:08:28.000000 autopio-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 17:08:28.000000 autopio-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 17:08:28.000000 autopio-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:08:42.828410 autopio-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:53:07.461714 autopio-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-07 09:52:55.000000 autopio-0.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:53:07.461714 autopio-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:53:07.461714 autopio-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-07 09:52:55.000000 autopio-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 09:52:55.000000 autopio-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 09:52:55.000000 autopio-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-07 09:53:07.461714 autopio-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 09:52:55.000000 autopio-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:53:07.461714 autopio-0.1.2/autopio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:52:55.000000 autopio-0.1.2/autopio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:53:07.461714 autopio-0.1.2/autopio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-07 09:53:07.000000 autopio-0.1.2/autopio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-07 09:53:07.000000 autopio-0.1.2/autopio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:53:07.000000 autopio-0.1.2/autopio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 09:53:07.000000 autopio-0.1.2/autopio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 09:53:07.000000 autopio-0.1.2/autopio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-07 09:52:55.000000 autopio-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:53:07.461714 autopio-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:53:07.461714 autopio-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:52:55.000000 autopio-0.1.2/tests/__init__.py
```

### Comparing `autopio-0.1.0/LICENSE` & `autopio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autopio-0.1.0/PKG-INFO` & `autopio-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopio
-Version: 0.1.0
+Version: 0.1.2
 Summary: A simple CLI tool to improve the development of PlatformIO configuration files
 Author-email: Daniil Kalamin <dakalamin@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Daniil Kalamin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://pypi.org/project/autopio
 Project-URL: Repository, https://github.com/autopio/autopio
-Keywords: CLI,PlatformIO,pio,config,embedded,tool
+Keywords: CLI,config,embedded,pio,PlatformIO
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: tests
 License-File: LICENSE
 
 # AutoPIO
 
 A simple CLI tool to improve the development of PlatformIO configuration files
 
 [![PyPI - Python][python-badge]][python-link]
```

### Comparing `autopio-0.1.0/README.md` & `autopio-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `autopio-0.1.0/autopio.egg-info/PKG-INFO` & `autopio-0.1.2/autopio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopio
-Version: 0.1.0
+Version: 0.1.2
 Summary: A simple CLI tool to improve the development of PlatformIO configuration files
 Author-email: Daniil Kalamin <dakalamin@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Daniil Kalamin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://pypi.org/project/autopio
 Project-URL: Repository, https://github.com/autopio/autopio
-Keywords: CLI,PlatformIO,pio,config,embedded,tool
+Keywords: CLI,config,embedded,pio,PlatformIO
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: tests
 License-File: LICENSE
 
 # AutoPIO
 
 A simple CLI tool to improve the development of PlatformIO configuration files
 
 [![PyPI - Python][python-badge]][python-link]
```

