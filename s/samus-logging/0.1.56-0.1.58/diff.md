# Comparing `tmp/samus-logging-0.1.56.tar.gz` & `tmp/samus-logging-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.56.tar", last modified: Fri Jul  7 20:26:24 2023, max compression
+gzip compressed data, was "samus-logging-0.1.58.tar", last modified: Fri Jul  7 20:40:19 2023, max compression
```

## Comparing `samus-logging-0.1.56.tar` & `samus-logging-0.1.58.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:26:24.541233 samus-logging-0.1.56/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.56/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:26:24.537233 samus-logging-0.1.56/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:21.000000 samus-logging-0.1.56/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:26:24.537233 samus-logging-0.1.56/samus_logging/
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:26:24.537233 samus-logging-0.1.56/samus_logging/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:26:24.000000 samus-logging-0.1.56/samus_logging/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      280 2023-07-07 20:26:24.000000 samus-logging-0.1.56/samus_logging/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:26:24.000000 samus-logging-0.1.56/samus_logging/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-07 20:26:24.000000 samus-logging-0.1.56/samus_logging/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:26:24.000000 samus-logging-0.1.56/samus_logging/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-07 20:26:24.541233 samus-logging-0.1.56/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)      999 2023-07-07 20:26:17.000000 samus-logging-0.1.56/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:40:19.249009 samus-logging-0.1.58/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.58/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:40:19.249009 samus-logging-0.1.58/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:21.000000 samus-logging-0.1.58/README.md
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:40:19.249009 samus-logging-0.1.58/samus_logging/
+-rw-rw-r--   0 samu      (1000) samu      (1000)       54 2023-07-07 20:37:42.000000 samus-logging-0.1.58/samus_logging/__init__.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)      277 2023-06-28 16:49:59.000000 samus-logging-0.1.58/samus_logging/level_filter.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)     4559 2023-07-07 20:13:43.000000 samus-logging-0.1.58/samus_logging/samus_logging.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:40:19.249009 samus-logging-0.1.58/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:40:19.000000 samus-logging-0.1.58/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-07 20:40:19.000000 samus-logging-0.1.58/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:40:19.000000 samus-logging-0.1.58/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-07 20:40:19.000000 samus-logging-0.1.58/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-07 20:40:19.000000 samus-logging-0.1.58/samus_logging.egg-info/top_level.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-07 20:40:19.249009 samus-logging-0.1.58/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)      975 2023-07-07 20:39:48.000000 samus-logging-0.1.58/setup.py
```

### Comparing `samus-logging-0.1.56/setup.py` & `samus-logging-0.1.58/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     return None
 
 
 setup(
     name='samus-logging',
     version=read_file(f'VERSION'),
     python_requires='>=3.10',
-    package_dir={'': 'samus_logging'},
-    packages=find_packages(where='samus_logging'),
+    package_dir={'': '.'},
+    packages=find_packages(where='.'),
     install_requires=[],
     extras_require={'dev': ['twine==4.0.2']},
 
     # license='',
     description='A minimal Logging-controller.',
     long_description=read_file('README.md'),
     author='Samu Rabin',
```

