# Comparing `tmp/samus-logging-0.1.54.tar.gz` & `tmp/samus-logging-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.54.tar", last modified: Fri Jul  7 20:18:29 2023, max compression
+gzip compressed data, was "samus-logging-0.1.55.tar", last modified: Fri Jul  7 20:22:10 2023, max compression
```

## Comparing `samus-logging-0.1.54.tar` & `samus-logging-0.1.55.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:18:29.134263 samus-logging-0.1.54/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.54/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:18:29.134263 samus-logging-0.1.54/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:21.000000 samus-logging-0.1.54/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:18:29.134263 samus-logging-0.1.54/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:18:29.000000 samus-logging-0.1.54/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      210 2023-07-07 20:18:29.000000 samus-logging-0.1.54/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:18:29.000000 samus-logging-0.1.54/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-07 20:18:29.000000 samus-logging-0.1.54/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:18:29.000000 samus-logging-0.1.54/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-07 20:18:29.134263 samus-logging-0.1.54/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)      978 2023-07-07 19:59:08.000000 samus-logging-0.1.54/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:22:10.544255 samus-logging-0.1.55/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.55/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:22:10.544255 samus-logging-0.1.55/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:21.000000 samus-logging-0.1.55/README.md
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-07 20:22:10.544255 samus-logging-0.1.55/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)      981 2023-07-07 20:22:05.000000 samus-logging-0.1.55/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:22:10.544255 samus-logging-0.1.55/test/
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:22:10.544255 samus-logging-0.1.55/test/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:22:10.000000 samus-logging-0.1.55/test/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      235 2023-07-07 20:22:10.000000 samus-logging-0.1.55/test/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:22:10.000000 samus-logging-0.1.55/test/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-07 20:22:10.000000 samus-logging-0.1.55/test/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:22:10.000000 samus-logging-0.1.55/test/samus_logging.egg-info/top_level.txt
```

### Comparing `samus-logging-0.1.54/setup.py` & `samus-logging-0.1.55/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return None
 
 
 setup(
     name='samus-logging',
     version=read_file(f'VERSION'),
     python_requires='>=3.10',
-    package_dir={'': '.'},
+    package_dir={'': 'test'},
     packages=find_packages(where='test'),
     install_requires=[],
     extras_require={'dev': ['twine==4.0.2']},
 
     # license='',
     description='A minimal Logging-controller.',
     long_description=read_file('README.md'),
```

