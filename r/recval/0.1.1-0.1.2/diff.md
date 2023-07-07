# Comparing `tmp/recval-0.1.1.tar.gz` & `tmp/recval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recval-0.1.1.tar", max compression
+gzip compressed data, was "recval-0.1.2.tar", max compression
```

## Comparing `recval-0.1.1.tar` & `recval-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1072 2023-02-06 11:39:53.263554 recval-0.1.1/LICENSE
--rw-r--r--   0        0        0     1209 2023-02-06 11:39:53.263554 recval-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/__init__.py
--rw-r--r--   0        0        0      453 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/constants.py
--rw-r--r--   0        0        0      625 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/decorators.py
--rw-r--r--   0        0        0     6481 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/evaluator.py
--rw-r--r--   0        0        0       94 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/metrics/__init__.py
--rw-r--r--   0        0        0     2270 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/metrics/accuracy.py
--rw-r--r--   0        0        0      779 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/metrics/factory.py
--rw-r--r--   0        0        0     1770 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/metrics/metric_interface.py
--rw-r--r--   0        0        0     2861 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/metrics/metrics.py
--rw-r--r--   0        0        0     1999 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/metrics/metrics_utils.py
--rw-r--r--   0        0        0     2506 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/metrics/ranking.py
--rw-r--r--   0        0        0     2923 2023-02-06 11:39:53.263554 recval-0.1.1/src/recval/utils.py
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 recval-0.1.1/setup.py
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 recval-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-07 12:16:40.924595 recval-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1208 2023-07-07 12:16:40.924595 recval-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/__init__.py
+-rw-r--r--   0        0        0      453 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/constants.py
+-rw-r--r--   0        0        0      625 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/decorators.py
+-rw-r--r--   0        0        0     6481 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/evaluator.py
+-rw-r--r--   0        0        0       94 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/metrics/__init__.py
+-rw-r--r--   0        0        0     2270 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/metrics/accuracy.py
+-rw-r--r--   0        0        0      779 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/metrics/factory.py
+-rw-r--r--   0        0        0     1770 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/metrics/metric_interface.py
+-rw-r--r--   0        0        0     2861 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/metrics/metrics.py
+-rw-r--r--   0        0        0     1999 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/metrics/metrics_utils.py
+-rw-r--r--   0        0        0     2506 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/metrics/ranking.py
+-rw-r--r--   0        0        0     2923 2023-07-07 12:16:40.924595 recval-0.1.2/src/recval/utils.py
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 recval-0.1.2/setup.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 recval-0.1.2/PKG-INFO
```

### Comparing `recval-0.1.1/LICENSE` & `recval-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/pyproject.toml` & `recval-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "recval"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Edoardo D'Amico <damicoedoardo95@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numba = "^0.56.4"
 numpy = "^1.23.5"
-pandas = "^1.5.2"
+pandas = "2.0.3"
 pytest-xdist = "^3.1.0"
 strenum = "^0.4.9"
 toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 isort = "^5.9.3"
```

### Comparing `recval-0.1.1/src/recval/decorators.py` & `recval-0.1.2/src/recval/decorators.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/evaluator.py` & `recval-0.1.2/src/recval/evaluator.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/metrics/accuracy.py` & `recval-0.1.2/src/recval/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/metrics/factory.py` & `recval-0.1.2/src/recval/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/metrics/metric_interface.py` & `recval-0.1.2/src/recval/metrics/metric_interface.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/metrics/metrics.py` & `recval-0.1.2/src/recval/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/metrics/metrics_utils.py` & `recval-0.1.2/src/recval/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/metrics/ranking.py` & `recval-0.1.2/src/recval/metrics/ranking.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/src/recval/utils.py` & `recval-0.1.2/src/recval/utils.py`

 * *Files identical despite different names*

### Comparing `recval-0.1.1/setup.py` & `recval-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numba>=0.56.4,<0.57.0',
  'numpy>=1.23.5,<2.0.0',
- 'pandas>=1.5.2,<2.0.0',
+ 'pandas==2.0.3',
  'pytest-xdist>=3.1.0,<4.0.0',
  'strenum>=0.4.9,<0.5.0',
  'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'recval',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': 'None',
     'author': "Edoardo D'Amico",
     'author_email': 'damicoedoardo95@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `recval-0.1.1/PKG-INFO` & `recval-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: recval
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Edoardo D'Amico
 Author-email: damicoedoardo95@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas (==2.0.3)
 Requires-Dist: pytest-xdist (>=3.1.0,<4.0.0)
 Requires-Dist: strenum (>=0.4.9,<0.5.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

