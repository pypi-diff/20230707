# Comparing `tmp/golfy-1.4.0.tar.gz` & `tmp/golfy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.4.0.tar", last modified: Thu Jul  6 20:44:31 2023, max compression
+gzip compressed data, was "golfy-1.4.1.tar", last modified: Thu Jul  6 20:51:55 2023, max compression
```

## Comparing `golfy-1.4.0.tar` & `golfy-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.997751 golfy-1.4.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.4.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     1872 2023-07-06 20:44:31.997600 golfy-1.4.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1146 2023-07-06 20:37:45.000000 golfy-1.4.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.996271 golfy-1.4.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      289 2023-07-04 03:33:07.000000 golfy-1.4.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5494 2023-07-06 20:32:53.000000 golfy-1.4.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     6396 2023-07-03 19:39:52.000000 golfy-1.4.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-06 20:20:26.000000 golfy-1.4.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     3163 2023-07-06 20:21:28.000000 golfy-1.4.0/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.4.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)      335 2023-07-03 19:34:38.000000 golfy-1.4.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.4.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.997064 golfy-1.4.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     1872 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      370 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      734 2023-07-06 20:42:37.000000 golfy-1.4.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-06 20:44:31.997792 golfy-1.4.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.997416 golfy-1.4.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.4.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      234 2023-07-03 19:40:32.000000 golfy-1.4.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.4.0/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:51:55.629541 golfy-1.4.1/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.4.1/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-06 20:51:55.629419 golfy-1.4.1/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.4.1/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:51:55.628461 golfy-1.4.1/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      289 2023-07-04 03:33:07.000000 golfy-1.4.1/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5492 2023-07-06 20:50:21.000000 golfy-1.4.1/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6396 2023-07-03 19:39:52.000000 golfy-1.4.1/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-06 20:20:26.000000 golfy-1.4.1/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3163 2023-07-06 20:21:28.000000 golfy-1.4.1/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.4.1/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)      335 2023-07-03 19:34:38.000000 golfy-1.4.1/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.4.1/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:51:55.628894 golfy-1.4.1/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-06 20:51:55.000000 golfy-1.4.1/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      370 2023-07-06 20:51:55.000000 golfy-1.4.1/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-06 20:51:55.000000 golfy-1.4.1/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-06 20:51:55.000000 golfy-1.4.1/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      734 2023-07-06 20:51:30.000000 golfy-1.4.1/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-06 20:51:55.629573 golfy-1.4.1/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:51:55.629272 golfy-1.4.1/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.4.1/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      234 2023-07-03 19:40:32.000000 golfy-1.4.1/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.4.1/tests/test_optimize.py
```

### Comparing `golfy-1.4.0/LICENSE` & `golfy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.4.0/PKG-INFO` & `golfy-1.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.4.0
+Version: 1.4.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
@@ -56,11 +56,13 @@
 
 ```python
 from golfy.deconvolution import create_linear_system, solve_linear_system
 
 # s is a golfy.Solution object containing the mapping of peptides to pools
 # counts is a dictionary from (replicate, pool) index pairs to ELISpot counts or activity values
 linear_system = create_linear_system(s, counts)
-#
-solution = solve_linear_system(linear_system)
-print(solution.high_confidence_hits)
+
+# result type has an array of individual peptide activity estimates (result.activity_per_peptide)
+# and a set of high confidence hit peptides (result.high_confidence_peptides)
+result = solve_linear_system(linear_system)
+print(result.high_confidence_hits)
 ```
```

### Comparing `golfy-1.4.0/README.md` & `golfy-1.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -39,11 +39,13 @@
 
 ```python
 from golfy.deconvolution import create_linear_system, solve_linear_system
 
 # s is a golfy.Solution object containing the mapping of peptides to pools
 # counts is a dictionary from (replicate, pool) index pairs to ELISpot counts or activity values
 linear_system = create_linear_system(s, counts)
-#
-solution = solve_linear_system(linear_system)
-print(solution.high_confidence_hits)
+
+# result type has an array of individual peptide activity estimates (result.activity_per_peptide)
+# and a set of high confidence hit peptides (result.high_confidence_peptides)
+result = solve_linear_system(linear_system)
+print(result.high_confidence_hits)
 ```
```

### Comparing `golfy-1.4.0/golfy/deconvolution.py` & `golfy-1.4.1/golfy/deconvolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         pool_tuple_to_idx=pool_tuple_to_idx,
         idx_to_pool_tuple=idx_to_pool_tuple,
     )
 
 
 @dataclass
 class DeconvolutionResult:
-    activity_per_peptides: np.ndarray
+    activity_per_peptide: np.ndarray
     prob_hit_per_peptide: np.ndarray
     high_confidence_hits: set[Peptide]
 
 
 def solve_linear_system(
     linear_system: LinearSystem,
     min_peptide_activity: float = 1.0,
@@ -169,11 +169,11 @@
         frac_hit += (x > min_peptide_activity).astype(float)
 
     avg_activity /= len(loo_indices)
     frac_hit /= len(loo_indices)
     high_confidence_hits = set(np.where(frac_hit > 0.5)[0])
 
     return DeconvolutionResult(
-        activity_per_peptides=avg_activity,
+        activity_per_peptide=avg_activity,
         prob_hit_per_peptide=frac_hit,
         high_confidence_hits=high_confidence_hits,
     )
```

### Comparing `golfy-1.4.0/golfy/initialization.py` & `golfy-1.4.1/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.4.0/golfy/optimization.py` & `golfy-1.4.1/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.4.0/golfy/solution.py` & `golfy-1.4.1/golfy/solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.4.0/golfy/validity.py` & `golfy-1.4.1/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.4.0/golfy.egg-info/PKG-INFO` & `golfy-1.4.1/golfy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.4.0
+Version: 1.4.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
@@ -56,11 +56,13 @@
 
 ```python
 from golfy.deconvolution import create_linear_system, solve_linear_system
 
 # s is a golfy.Solution object containing the mapping of peptides to pools
 # counts is a dictionary from (replicate, pool) index pairs to ELISpot counts or activity values
 linear_system = create_linear_system(s, counts)
-#
-solution = solve_linear_system(linear_system)
-print(solution.high_confidence_hits)
+
+# result type has an array of individual peptide activity estimates (result.activity_per_peptide)
+# and a set of high confidence hit peptides (result.high_confidence_peptides)
+result = solve_linear_system(linear_system)
+print(result.high_confidence_hits)
 ```
```

### Comparing `golfy-1.4.0/pyproject.toml` & `golfy-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'Environment :: Console',
     'Operating System :: OS Independent',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: Apache Software License',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 readme = "README.md"
-version = "1.4.0"  
+version = "1.4.1"  
 
 [tool.setuptools]
 packages = ["golfy"]
 
 [project.urls]
 "Homepage" = "https://github.com/pirl-unc/golfy"
 "Bug Tracker" = "https://github.com/pirl-unc/golfy"
```

### Comparing `golfy-1.4.0/tests/test_deconvolution.py` & `golfy-1.4.1/tests/test_deconvolution.py`

 * *Files identical despite different names*

