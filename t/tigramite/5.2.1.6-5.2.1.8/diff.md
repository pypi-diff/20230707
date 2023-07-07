# Comparing `tmp/tigramite-5.2.1.6.tar.gz` & `tmp/tigramite-5.2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigramite-5.2.1.6.tar", last modified: Fri Jun  2 16:50:51 2023, max compression
+gzip compressed data, was "tigramite-5.2.1.8.tar", last modified: Fri Jun  2 17:04:44 2023, max compression
```

## Comparing `tigramite-5.2.1.6.tar` & `tigramite-5.2.1.8.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/PKG-INFO
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8006 2023-06-02 16:50:38.000000 tigramite-5.2.1.6/README.md
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       79 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/setup.cfg
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3150 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/setup.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.766601 tigramite-5.2.1.6/tests/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     5485 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_construct_array.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    38249 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_independence_tests.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3894 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_models.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    26762 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_pcmci_calculations.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17546 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_pcmci_construction.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13375 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_var_process.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.770601 tigramite-5.2.1.6/tigramite/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   103626 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/causal_effects.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    65916 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/data_processing.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/tigramite/independence_tests/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    43660 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/LBFGS.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17895 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/cmiknn.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    10905 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/cmisymb.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    23994 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/gpdc.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    31189 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/gpdc_torch.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     6459 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/gsquared.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41951 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/independence_tests_base.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    62833 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/oracle_conditional_independence.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     9979 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/parcorr.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12267 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/parcorr_mult.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17975 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/parcorr_wls.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13647 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/regressionCI.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13402 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/robust_parcorr.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   170551 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/lpcmci.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    77764 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/models.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   169431 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/pcmci.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41334 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/pcmci_base.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   164901 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/plotting.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/tigramite/toymodels/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/toymodels/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41858 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/toymodels/structural_causal_processes.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12722 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/toymodels/surrogate_generator.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.770601 tigramite-5.2.1.6/tigramite.egg-info/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/PKG-INFO
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     1298 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/SOURCES.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        1 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/dependency_links.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)      428 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/requires.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       10 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/top_level.txt
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:44.206861 tigramite-5.2.1.8/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-06-02 17:04:44.206861 tigramite-5.2.1.8/PKG-INFO
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8006 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/README.md
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       79 2023-06-02 17:04:44.210861 tigramite-5.2.1.8/setup.cfg
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3150 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/setup.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:44.202861 tigramite-5.2.1.8/tests/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     5485 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tests/test_construct_array.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    38249 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tests/test_independence_tests.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3894 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tests/test_models.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    26762 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tests/test_pcmci_calculations.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17546 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tests/test_pcmci_construction.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13375 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tests/test_var_process.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:44.206861 tigramite-5.2.1.8/tigramite/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   103626 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/causal_effects.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    65916 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/data_processing.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:44.206861 tigramite-5.2.1.8/tigramite/independence_tests/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    43660 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/LBFGS.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17895 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/cmiknn.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    10905 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/cmisymb.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    23994 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/gpdc.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    31189 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/gpdc_torch.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     6459 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/gsquared.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41951 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/independence_tests_base.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    62833 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/oracle_conditional_independence.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     9979 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/parcorr.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12267 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/parcorr_mult.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17975 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/parcorr_wls.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13647 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/regressionCI.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13402 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/independence_tests/robust_parcorr.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   170551 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/lpcmci.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    77764 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/models.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   169431 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/pcmci.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41334 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/pcmci_base.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   164901 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/plotting.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    19278 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/rpcmci.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:44.206861 tigramite-5.2.1.8/tigramite/toymodels/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/toymodels/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41858 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/toymodels/structural_causal_processes.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12722 2023-06-02 17:04:32.000000 tigramite-5.2.1.8/tigramite/toymodels/surrogate_generator.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 17:04:44.206861 tigramite-5.2.1.8/tigramite.egg-info/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-06-02 17:04:44.000000 tigramite-5.2.1.8/tigramite.egg-info/PKG-INFO
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     1318 2023-06-02 17:04:44.000000 tigramite-5.2.1.8/tigramite.egg-info/SOURCES.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        1 2023-06-02 17:04:44.000000 tigramite-5.2.1.8/tigramite.egg-info/dependency_links.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)      428 2023-06-02 17:04:44.000000 tigramite-5.2.1.8/tigramite.egg-info/requires.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       10 2023-06-02 17:04:44.000000 tigramite-5.2.1.8/tigramite.egg-info/top_level.txt
```

### Comparing `tigramite-5.2.1.6/PKG-INFO` & `tigramite-5.2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigramite
-Version: 5.2.1.6
+Version: 5.2.1.8
 Summary: Tigramite causal inference for time series
 Home-page: https://github.com/jakobrunge/tigramite/
 Author: Jakob Runge
 Author-email: jakob@jakob-runge.com
 License: GNU General Public License v3.0
 Keywords: causal inference,causal discovery,prediction,time series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tigramite-5.2.1.6/README.md` & `tigramite-5.2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/setup.py` & `tigramite-5.2.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 # Use a custom build to handle numpy.include_dirs() when building
 CMDCLASS = {"build_ext": UseNumpyHeadersBuildExt}
 
 # Run the setup
 setup(
     name="tigramite",
-    version="5.2.1.6",
+    version="5.2.1.8",
     packages=["tigramite", "tigramite.independence_tests", "tigramite.toymodels"],
     license="GNU General Public License v3.0",
     description="Tigramite causal inference for time series",
     author="Jakob Runge",
     author_email="jakob@jakob-runge.com",
     url="https://github.com/jakobrunge/tigramite/",
     long_description=long_description,
```

### Comparing `tigramite-5.2.1.6/tests/test_construct_array.py` & `tigramite-5.2.1.8/tests/test_construct_array.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tests/test_independence_tests.py` & `tigramite-5.2.1.8/tests/test_independence_tests.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tests/test_models.py` & `tigramite-5.2.1.8/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tests/test_pcmci_calculations.py` & `tigramite-5.2.1.8/tests/test_pcmci_calculations.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tests/test_pcmci_construction.py` & `tigramite-5.2.1.8/tests/test_pcmci_construction.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tests/test_var_process.py` & `tigramite-5.2.1.8/tests/test_var_process.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/causal_effects.py` & `tigramite-5.2.1.8/tigramite/causal_effects.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/data_processing.py` & `tigramite-5.2.1.8/tigramite/data_processing.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/LBFGS.py` & `tigramite-5.2.1.8/tigramite/independence_tests/LBFGS.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/cmiknn.py` & `tigramite-5.2.1.8/tigramite/independence_tests/cmiknn.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/cmisymb.py` & `tigramite-5.2.1.8/tigramite/independence_tests/cmisymb.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/gpdc.py` & `tigramite-5.2.1.8/tigramite/independence_tests/gpdc.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/gpdc_torch.py` & `tigramite-5.2.1.8/tigramite/independence_tests/gpdc_torch.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/gsquared.py` & `tigramite-5.2.1.8/tigramite/independence_tests/gsquared.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/independence_tests_base.py` & `tigramite-5.2.1.8/tigramite/independence_tests/independence_tests_base.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/oracle_conditional_independence.py` & `tigramite-5.2.1.8/tigramite/independence_tests/oracle_conditional_independence.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/parcorr.py` & `tigramite-5.2.1.8/tigramite/independence_tests/parcorr.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/parcorr_mult.py` & `tigramite-5.2.1.8/tigramite/independence_tests/parcorr_mult.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/parcorr_wls.py` & `tigramite-5.2.1.8/tigramite/independence_tests/parcorr_wls.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/regressionCI.py` & `tigramite-5.2.1.8/tigramite/independence_tests/regressionCI.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/independence_tests/robust_parcorr.py` & `tigramite-5.2.1.8/tigramite/independence_tests/robust_parcorr.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/lpcmci.py` & `tigramite-5.2.1.8/tigramite/lpcmci.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/models.py` & `tigramite-5.2.1.8/tigramite/models.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/pcmci.py` & `tigramite-5.2.1.8/tigramite/pcmci.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/pcmci_base.py` & `tigramite-5.2.1.8/tigramite/pcmci_base.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/plotting.py` & `tigramite-5.2.1.8/tigramite/plotting.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/toymodels/structural_causal_processes.py` & `tigramite-5.2.1.8/tigramite/toymodels/structural_causal_processes.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite/toymodels/surrogate_generator.py` & `tigramite-5.2.1.8/tigramite/toymodels/surrogate_generator.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.1.6/tigramite.egg-info/PKG-INFO` & `tigramite-5.2.1.8/tigramite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigramite
-Version: 5.2.1.6
+Version: 5.2.1.8
 Summary: Tigramite causal inference for time series
 Home-page: https://github.com/jakobrunge/tigramite/
 Author: Jakob Runge
 Author-email: jakob@jakob-runge.com
 License: GNU General Public License v3.0
 Keywords: causal inference,causal discovery,prediction,time series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tigramite-5.2.1.6/tigramite.egg-info/SOURCES.txt` & `tigramite-5.2.1.8/tigramite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 tigramite/causal_effects.py
 tigramite/data_processing.py
 tigramite/lpcmci.py
 tigramite/models.py
 tigramite/pcmci.py
 tigramite/pcmci_base.py
 tigramite/plotting.py
+tigramite/rpcmci.py
 tigramite.egg-info/PKG-INFO
 tigramite.egg-info/SOURCES.txt
 tigramite.egg-info/dependency_links.txt
 tigramite.egg-info/requires.txt
 tigramite.egg-info/top_level.txt
 tigramite/independence_tests/LBFGS.py
 tigramite/independence_tests/__init__.py
```

