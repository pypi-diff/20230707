# Comparing `tmp/zhinst-23.2.4.tar.gz` & `tmp/zhinst-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhinst-23.2.4.tar", last modified: Wed Apr  5 16:47:57 2023, max compression
+gzip compressed data, was "zhinst-23.6.0.tar", last modified: Fri Jul  7 14:56:24 2023, max compression
```

## Comparing `zhinst-23.2.4.tar` & `zhinst-23.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:47:57.507916 zhinst-23.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:47:57.507916 zhinst-23.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:47:57.507916 zhinst-23.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-05 16:47:43.000000 zhinst-23.2.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-05 16:47:43.000000 zhinst-23.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-05 16:47:43.000000 zhinst-23.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-05 16:47:57.507916 zhinst-23.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-05 16:47:43.000000 zhinst-23.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:47:57.507916 zhinst-23.2.4/build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-05 16:47:43.000000 zhinst-23.2.4/build_tools/test_wheels.sh
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-05 16:47:43.000000 zhinst-23.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-05 16:47:57.511916 zhinst-23.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:47:57.507916 zhinst-23.2.4/zhinst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-05 16:47:57.000000 zhinst-23.2.4/zhinst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-05 16:47:57.000000 zhinst-23.2.4/zhinst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:47:57.000000 zhinst-23.2.4/zhinst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-05 16:47:57.000000 zhinst-23.2.4/zhinst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 16:47:57.000000 zhinst-23.2.4/zhinst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:56:24.620290 zhinst-23.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:56:24.616290 zhinst-23.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:56:24.620290 zhinst-23.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-07 14:56:06.000000 zhinst-23.6.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-07 14:56:06.000000 zhinst-23.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-07 14:56:06.000000 zhinst-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 14:56:24.620290 zhinst-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-07 14:56:06.000000 zhinst-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:56:24.620290 zhinst-23.6.0/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-07 14:56:06.000000 zhinst-23.6.0/build_tools/test_wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-07 14:56:06.000000 zhinst-23.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-07 14:56:24.620290 zhinst-23.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:56:24.620290 zhinst-23.6.0/zhinst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 14:56:24.000000 zhinst-23.6.0/zhinst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-07 14:56:24.000000 zhinst-23.6.0/zhinst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:56:24.000000 zhinst-23.6.0/zhinst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 14:56:24.000000 zhinst-23.6.0/zhinst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 14:56:24.000000 zhinst-23.6.0/zhinst.egg-info/top_level.txt
```

### Comparing `zhinst-23.2.4/.github/workflows/publish.yml` & `zhinst-23.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `zhinst-23.2.4/LICENSE` & `zhinst-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhinst-23.2.4/PKG-INFO` & `zhinst-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhinst
-Version: 23.2.4
+Version: 23.6.0
 Summary: Zurich Instruments Python API
 Author: Zurich Instrument
 Author-email: info@zhinst.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `zhinst-23.2.4/README.md` & `zhinst-23.6.0/README.md`

 * *Files identical despite different names*

### Comparing `zhinst-23.2.4/setup.cfg` & `zhinst-23.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	Topic :: Scientific/Engineering
 	Intended Audience :: Science/Research
 
 [options]
 python_requires = >=3.7
 use_scm_version = True
 install_requires = 
-	zhinst.core == 23.2.42414
-	zhinst.utils == 0.3.1
-	zhinst.toolkit == 0.5.3
+	zhinst.core == 23.6.45428
+	zhinst.utils == 0.3.2
+	zhinst.toolkit == 0.6.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `zhinst-23.2.4/zhinst.egg-info/PKG-INFO` & `zhinst-23.6.0/zhinst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhinst
-Version: 23.2.4
+Version: 23.6.0
 Summary: Zurich Instruments Python API
 Author: Zurich Instrument
 Author-email: info@zhinst.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

