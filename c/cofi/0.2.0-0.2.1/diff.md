# Comparing `tmp/cofi-0.2.0.tar.gz` & `tmp/cofi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofi-0.2.0.tar", last modified: Mon Jun  5 06:30:40 2023, max compression
+gzip compressed data, was "cofi-0.2.1.tar", last modified: Fri Jul  7 03:56:03 2023, max compression
```

## Comparing `cofi-0.2.0.tar` & `cofi-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.125372 cofi-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-05 06:30:22.000000 cofi-0.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-05 06:30:40.125372 cofi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-05 06:30:22.000000 cofi-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-05 06:30:23.000000 cofi-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:30:40.125372 cofi-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.117371 cofi-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67472 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_base_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_base_inference_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_cofi_simple_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_emcee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_pytorch_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_scipy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_scipy_opt_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_scipy_opt_min.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/_reg_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/_reg_lp_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/_reg_model_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.125372 cofi-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_for_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_for_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_inversion_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.918507 cofi-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 03:55:49.000000 cofi-0.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-07 03:56:03.918507 cofi-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-07 03:55:49.000000 cofi-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-07 03:55:49.000000 cofi-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 03:56:03.918507 cofi-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.910507 cofi-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67472 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_base_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_base_inference_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_cofi_simple_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_pytorch_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_scipy_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_scipy_opt_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_scipy_opt_min.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/_reg_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/_reg_lp_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/_reg_model_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.918507 cofi-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_for_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_for_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_inversion_result.py
```

### Comparing `cofi-0.2.0/LICENCE` & `cofi-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/PKG-INFO` & `cofi-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `cofi-0.2.0/README.md` & `cofi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/pyproject.toml` & `cofi-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/__init__.py` & `cofi-0.2.1/src/cofi/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/_base_problem.py` & `cofi-0.2.1/src/cofi/_base_problem.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/_exceptions.py` & `cofi-0.2.1/src/cofi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/_inversion.py` & `cofi-0.2.1/src/cofi/_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/_inversion_options.py` & `cofi-0.2.1/src/cofi/_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/tools/__init__.py` & `cofi-0.2.1/src/cofi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/tools/_base_inference_tool.py` & `cofi-0.2.1/src/cofi/tools/_base_inference_tool.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/tools/_emcee.py` & `cofi-0.2.1/src/cofi/tools/_emcee.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/tools/_pytorch_optim.py` & `cofi-0.2.1/src/cofi/tools/_pytorch_optim.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/tools/_scipy_lstsq.py` & `cofi-0.2.1/src/cofi/tools/_scipy_lstsq.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/tools/_scipy_opt_lstsq.py` & `cofi-0.2.1/src/cofi/tools/_scipy_opt_lstsq.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/tools/_scipy_opt_min.py` & `cofi-0.2.1/src/cofi/tools/_scipy_opt_min.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/utils/__init__.py` & `cofi-0.2.1/src/cofi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/utils/_reg_base.py` & `cofi-0.2.1/src/cofi/utils/_reg_base.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/utils/_reg_lp_norm.py` & `cofi-0.2.1/src/cofi/utils/_reg_lp_norm.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi/utils/_reg_model_cov.py` & `cofi-0.2.1/src/cofi/utils/_reg_model_cov.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/src/cofi.egg-info/PKG-INFO` & `cofi-0.2.1/src/cofi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `cofi-0.2.0/src/cofi.egg-info/SOURCES.txt` & `cofi-0.2.1/src/cofi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/tests/test_base_problem_basics.py` & `cofi-0.2.1/tests/test_base_problem_basics.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/tests/test_base_problem_for_optimization.py` & `cofi-0.2.1/tests/test_base_problem_for_optimization.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/tests/test_base_problem_for_sampling.py` & `cofi-0.2.1/tests/test_base_problem_for_sampling.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/tests/test_base_problem_misc.py` & `cofi-0.2.1/tests/test_base_problem_misc.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/tests/test_inversion.py` & `cofi-0.2.1/tests/test_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/tests/test_inversion_options.py` & `cofi-0.2.1/tests/test_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.0/tests/test_inversion_result.py` & `cofi-0.2.1/tests/test_inversion_result.py`

 * *Files identical despite different names*

