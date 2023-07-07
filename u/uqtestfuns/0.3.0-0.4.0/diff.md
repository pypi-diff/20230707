# Comparing `tmp/uqtestfuns-0.3.0.tar.gz` & `tmp/uqtestfuns-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uqtestfuns-0.3.0.tar", last modified: Mon Jul  3 15:36:51 2023, max compression
+gzip compressed data, was "uqtestfuns-0.4.0.tar", last modified: Fri Jul  7 16:23:49 2023, max compression
```

## Comparing `uqtestfuns-0.3.0.tar` & `uqtestfuns-0.4.0.tar`

### file list

```diff
@@ -1,76 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9012 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.476695 uqtestfuns-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns/
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns/core/
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (122)     8331 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/probabilistic_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     6077 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.484695 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5984 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (122)     6845 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6394 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py
--rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py
--rw-r--r--   0 runner    (1001) docker     (122)     9350 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py
--rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3875 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun.py
--rw-r--r--   0 runner    (1001) docker     (122)    15916 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun_abc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/global_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     8816 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.484695 uqtestfuns-0.3.0/src/uqtestfuns/meta/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    12619 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/metaspec.py
--rw-r--r--   0 runner    (1001) docker     (122)     7364 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/uqmetatestfun.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3321 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ackley.py
--rw-r--r--   0 runner    (1001) docker     (122)     4792 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/borehole.py
--rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/bratley1992.py
--rw-r--r--   0 runner    (1001) docker     (122)     3753 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/cantilever_beam_2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/circular_pipe_crack.py
--rw-r--r--   0 runner    (1001) docker     (122)    10303 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/damped_oscillator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/flood.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/forrester.py
--rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/four_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/franke.py
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/gayton_hat.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/gramacy2007.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/hyper_sphere.py
--rw-r--r--   0 runner    (1001) docker     (122)     3668 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ishigami.py
--rw-r--r--   0 runner    (1001) docker     (122)     7421 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/mclain.py
--rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/oakley2002.py
--rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/otl_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/piston.py
--rw-r--r--   0 runner    (1001) docker     (122)     9619 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sobol_g.py
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/speed_reducer_shaft.py
--rw-r--r--   0 runner    (1001) docker     (122)     7550 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sulfur.py
--rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/welch1992.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/wing_weight.py
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2767 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/tests/test_list_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.527137 uqtestfuns-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11010 2023-07-07 16:23:49.527137 uqtestfuns-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9885 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     2657 2023-07-07 16:23:49.527137 uqtestfuns-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.511136 uqtestfuns-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.511136 uqtestfuns-0.4.0/src/uqtestfuns/
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.515136 uqtestfuns-0.4.0/src/uqtestfuns/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.515136 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/probabilistic_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6564 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.519136 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5984 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6845 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6394 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9350 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3875 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/uqtestfun.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15502 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/uqtestfun_abc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/global_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8816 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.519136 uqtestfuns-0.4.0/src/uqtestfuns/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/meta/basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12619 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/meta/metaspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7364 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/meta/uqmetatestfun.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.527137 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3321 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/ackley.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4792 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/borehole.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/bratley1992.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3753 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/cantilever_beam_2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/circular_pipe_crack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/convex_fail_domain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/damped_cosine.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10303 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/damped_oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/flood.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/forrester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/four_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/franke.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/gayton_hat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/gramacy2007.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/hyper_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3668 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/ishigami.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7421 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/mclain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/oakley2002.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/otl_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/piston.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2634 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/rs_circular_bar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/rs_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9619 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/sobol_g.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/speed_reducer_shaft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7550 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/sulfur.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/webster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/welch1992.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/test_functions/wing_weight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/src/uqtestfuns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.515136 uqtestfuns-0.4.0/src/uqtestfuns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11010 2023-07-07 16:23:49.000000 uqtestfuns-0.4.0/src/uqtestfuns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-07-07 16:23:49.000000 uqtestfuns-0.4.0/src/uqtestfuns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 16:23:49.000000 uqtestfuns-0.4.0/src/uqtestfuns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-07 16:23:49.000000 uqtestfuns-0.4.0/src/uqtestfuns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-07 16:23:49.000000 uqtestfuns-0.4.0/src/uqtestfuns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 16:23:49.527137 uqtestfuns-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-07-07 16:23:37.000000 uqtestfuns-0.4.0/tests/test_list_functions.py
```

### Comparing `uqtestfuns-0.3.0/LICENSE` & `uqtestfuns-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/PKG-INFO` & `uqtestfuns-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,52 @@
-Metadata-Version: 2.1
-Name: uqtestfuns
-Version: 0.3.0
-Summary: A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
-Home-page: https://github.com/damar-wicaksono/uqtestfuns
-Author: Damar Wicaksono
-Author-email: damar.wicaksono@outlook.com
-License: MIT
-Platform: ANY
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: all
-License-File: LICENSE
-
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8109901-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8109901)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8125015-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8125015)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
-[![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
+[![PyPI](https://img.shields.io/pypi/v/uqtestfuns?style=flat-square)](https://pypi.org/project/uqtestfuns/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
 |  [`dev`](https://github.com/damar-wicaksono/uqtestfuns/tree/dev) (latest)  | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=dev&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/dev?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/dev) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=latest&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=latest)    |
 
 <!--One paragraph description-->
 UQTestFuns is an open-source Python3 library of test functions commonly used
-within the uncertainty quantification (UQ) community.
-The package aims to provide:
+within the applied uncertainty quantification (UQ) community.
+Specifically, the package provides:
 
-- a _lightweight implementation_ (with minimal dependencies) of
-  many test functions available in the UQ literature
-- a _single entry point_ (combining models and their probabilistic input
-  specification) to a wide range of test functions
-- an opportunity for an _open-source contribution_ where new test functions and
-  reference results are posted.
+- an implementation _with minimal dependencies_ (i.e., NumPy and SciPy) and
+  _a common interface_ of many test functions available in the UQ literature
+- a _single entry point_ collecting test functions _and_ their probabilistic
+  input specifications in a single Python package
+- an _opportunity for an open-source contribution_, supporting
+  the implementation of new test functions or posting reference results.
 
 In short, UQTestFuns is an homage
 to the [Virtual Library of Simulation Experiments (VLSE)](https://www.sfu.ca/~ssurjano/).
 
 ## Usage
 
 UQTestFuns includes several commonly used test functions in the UQ community.
 To list the available functions:
 
 ```python-repl
 >>> import uqtestfuns as uqtf
 >>> uqtf.list_functions()
- No.      Constructor       Spatial Dimension          Application          Description
------  ------------------  -------------------  --------------------------  ----------------------------------------------------------------------------
-  1         Ackley()                M           optimization, metamodeling  Ackley function from Ackley (1987)
-  2        Borehole()               8           metamodeling, sensitivity   Borehole function from Harper and Gupta (1983)
-  3    DampedOscillator()           8           metamodeling, sensitivity   Damped oscillator model from Igusa and Der Kiureghian (1985)
-  4         Flood()                 8           metamodeling, sensitivity   Flood model from Iooss and Lemaître (2015)
-  5        Ishigami()               3                  sensitivity          Ishigami function from Ishigami and Homma (1991)
+No.            Constructor            Dimension                Application                Description
+-----  -----------------------------  -----------  --------------------------------------  ----------------------------------------------------------------------------
+  1              Ackley()                  M             optimization, metamodeling        Optimization test function from Ackley (1987)
+  2             Borehole()                 8             metamodeling, sensitivity         Borehole function from Harper and Gupta (1983)
+  3           Bratley1992a()               M              integration, sensitivity         Integration test function #1 from Bratley et al. (1992)
+  4           Bratley1992b()               M              integration, sensitivity         Integration test function #2 from Bratley et al. (1992)
+  5           Bratley1992c()               M              integration, sensitivity         Integration test function #3 from Bratley et al. (1992)
+  6           Bratley1992d()               M              integration, sensitivity         Integration test function #4 from Bratley et al. (1992)
+  7         CantileverBeam2D()             2                    reliability                Cantilever beam reliability problem from Rajashekhar and Ellington (1993)
+  8         CircularPipeCrack()            2                    reliability                Circular pipe under bending moment from Verma et al. (2015)
 ...
 ```
 
 Consider the Borehole function, a test function commonly used for metamodeling
 and sensitivity analysis purposes; to create an instance of this test function:
 
 ```python-repl
@@ -177,11 +154,15 @@
 with tax funds on the basis of the budget approved
 by the Saxony State Parliament.
 
 UQTestFuns is currently maintained by:
 
 - Damar Wicaksono ([HZDR/CASUS](https://www.casus.science/))
 
+with scientific supervision from:
+
+- Michael Hecht ([HZDR/CASUS](https://www.casus.science/))
+
 ## License
 
 <!--License-->
 UQTestFuns is released under the [MIT License](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uqtestfuns-0.3.0/README.md` & `uqtestfuns-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,80 @@
+Metadata-Version: 2.1
+Name: uqtestfuns
+Version: 0.4.0
+Summary: A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
+Home-page: https://github.com/damar-wicaksono/uqtestfuns
+Author: Damar Wicaksono
+Author-email: damar.wicaksono@outlook.com
+License: MIT
+Platform: ANY
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: all
+License-File: LICENSE
+
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8109901-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8109901)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8125015-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8125015)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
-[![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
+[![PyPI](https://img.shields.io/pypi/v/uqtestfuns?style=flat-square)](https://pypi.org/project/uqtestfuns/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
 |  [`dev`](https://github.com/damar-wicaksono/uqtestfuns/tree/dev) (latest)  | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=dev&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/dev?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/dev) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=latest&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=latest)    |
 
 <!--One paragraph description-->
 UQTestFuns is an open-source Python3 library of test functions commonly used
-within the uncertainty quantification (UQ) community.
-The package aims to provide:
+within the applied uncertainty quantification (UQ) community.
+Specifically, the package provides:
 
-- a _lightweight implementation_ (with minimal dependencies) of
-  many test functions available in the UQ literature
-- a _single entry point_ (combining models and their probabilistic input
-  specification) to a wide range of test functions
-- an opportunity for an _open-source contribution_ where new test functions and
-  reference results are posted.
+- an implementation _with minimal dependencies_ (i.e., NumPy and SciPy) and
+  _a common interface_ of many test functions available in the UQ literature
+- a _single entry point_ collecting test functions _and_ their probabilistic
+  input specifications in a single Python package
+- an _opportunity for an open-source contribution_, supporting
+  the implementation of new test functions or posting reference results.
 
 In short, UQTestFuns is an homage
 to the [Virtual Library of Simulation Experiments (VLSE)](https://www.sfu.ca/~ssurjano/).
 
 ## Usage
 
 UQTestFuns includes several commonly used test functions in the UQ community.
 To list the available functions:
 
 ```python-repl
 >>> import uqtestfuns as uqtf
 >>> uqtf.list_functions()
- No.      Constructor       Spatial Dimension          Application          Description
------  ------------------  -------------------  --------------------------  ----------------------------------------------------------------------------
-  1         Ackley()                M           optimization, metamodeling  Ackley function from Ackley (1987)
-  2        Borehole()               8           metamodeling, sensitivity   Borehole function from Harper and Gupta (1983)
-  3    DampedOscillator()           8           metamodeling, sensitivity   Damped oscillator model from Igusa and Der Kiureghian (1985)
-  4         Flood()                 8           metamodeling, sensitivity   Flood model from Iooss and Lemaître (2015)
-  5        Ishigami()               3                  sensitivity          Ishigami function from Ishigami and Homma (1991)
+No.            Constructor            Dimension                Application                Description
+-----  -----------------------------  -----------  --------------------------------------  ----------------------------------------------------------------------------
+  1              Ackley()                  M             optimization, metamodeling        Optimization test function from Ackley (1987)
+  2             Borehole()                 8             metamodeling, sensitivity         Borehole function from Harper and Gupta (1983)
+  3           Bratley1992a()               M              integration, sensitivity         Integration test function #1 from Bratley et al. (1992)
+  4           Bratley1992b()               M              integration, sensitivity         Integration test function #2 from Bratley et al. (1992)
+  5           Bratley1992c()               M              integration, sensitivity         Integration test function #3 from Bratley et al. (1992)
+  6           Bratley1992d()               M              integration, sensitivity         Integration test function #4 from Bratley et al. (1992)
+  7         CantileverBeam2D()             2                    reliability                Cantilever beam reliability problem from Rajashekhar and Ellington (1993)
+  8         CircularPipeCrack()            2                    reliability                Circular pipe under bending moment from Verma et al. (2015)
 ...
 ```
 
 Consider the Borehole function, a test function commonly used for metamodeling
 and sensitivity analysis purposes; to create an instance of this test function:
 
 ```python-repl
@@ -150,11 +182,15 @@
 with tax funds on the basis of the budget approved
 by the Saxony State Parliament.
 
 UQTestFuns is currently maintained by:
 
 - Damar Wicaksono ([HZDR/CASUS](https://www.casus.science/))
 
+with scientific supervision from:
+
+- Michael Hecht ([HZDR/CASUS](https://www.casus.science/))
+
 ## License
 
 <!--License-->
 UQTestFuns is released under the [MIT License](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uqtestfuns-0.3.0/setup.cfg` & `uqtestfuns-0.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uqtestfuns
-version = 0.3.0
+version = 0.4.0
 url = https://github.com/damar-wicaksono/uqtestfuns
 author = Damar Wicaksono
 author_email = damar.wicaksono@outlook.com
 description = A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 long_description = file: README.md
 long_description_content_type = text/markdown
 platform = ANY
@@ -14,14 +14,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Mathematics
 	Topic :: Software Development :: Libraries :: Python Modules
 	Intended Audience :: Science/Research
 
 [options]
 package_dir = 
@@ -80,14 +81,15 @@
 [tox:tox]
 isolated_build = True
 envlist = 
 	py37
 	py38
 	py39
 	py310
+	py311
 
 [testenv]
 deps = 
 	pytest
 	pytest-cov
 	pytest-randomly
 	numpy>=1.13.3
```

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/__init__.py` & `uqtestfuns-0.4.0/src/uqtestfuns/__init__.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/input_spec.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/input_spec.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/probabilistic_input.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/probabilistic_input.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,14 +109,27 @@
             for idx_dim, marginal in enumerate(self.marginals):
                 xx[:, idx_dim] = marginal.icdf(xx[:, idx_dim])
         else:
             raise ValueError("Copulas are not currently supported!")
 
         return xx
 
+    def reset_rng(self, rng_seed: Optional[int]) -> None:
+        """Reset the random number generator.
+
+        Parameters
+        ----------
+        rng_seed : int, optional.
+            The seed used to initialize the pseudo-random number generator.
+            If not specified, the value is taken from the system entropy.
+        """
+        rng = np.random.default_rng(rng_seed)
+        object.__setattr__(self, "_rng", rng)
+        object.__setattr__(self, "rng_seed", rng_seed)
+
     def pdf(self, xx: np.ndarray) -> np.ndarray:
         """Get the PDF value of the distribution on a set of values.
 
         Parameters
         ----------
         xx : np.ndarray
             Sample values (realizations) from a distribution.
```

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distribution.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,27 @@
 
         xx = self._rng.random(sample_size)  # type: ignore
 
         return get_icdf_values(
             xx, self.distribution, self.parameters, self.lower, self.upper
         )
 
+    def reset_rng(self, rng_seed: Optional[int]) -> None:
+        """Reset the random number generator.
+
+        Parameters
+        ----------
+        rng_seed : int, optional.
+            The seed used to initialize the pseudo-random number generator.
+            If not specified, the value is taken from the system entropy.
+        """
+        rng = np.random.default_rng(rng_seed)
+        object.__setattr__(self, "_rng", rng)
+        object.__setattr__(self, "rng_seed", rng_seed)
+
     def pdf(self, xx: Union[float, np.ndarray]) -> ARRAY_FLOAT:
         """Compute the PDF of the distribution on a set of values."""
         # TODO: check if you put a scalar inside
         # Convert input to an np.array
         xx = np.asarray(xx)
 
         return get_pdf_values(
```

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/utils.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/prob_input/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/uqtestfun.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun_abc.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/uqtestfun_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,19 +189,14 @@
         The selection of parameters set; this is used when there are multiple
         sets of parameters available in the literature.
         This is a keyword only parameter.
     name : str, optional
         The name of the UQ test function.
         If not given, `None` is used as name.
         This is a keyword only parameter.
-    rng_seed_prob_input : int, optional
-        The seed number for the pseudo-random number generator of the
-        corresponding `ProbInput`; if not given, `None` is used
-        (taken from the system entropy).
-        This is a keyword only parameter.
 
     Notes
     -----
     - A published UQ test function includes a couple of additional metadata,
       namely tags and description.
 
     Raises
@@ -219,15 +214,14 @@
     def __init__(
         self,
         *,
         spatial_dimension: Optional[int] = None,
         prob_input_selection: Optional[str] = None,
         parameters_selection: Optional[str] = None,
         name: Optional[str] = None,
-        rng_seed_prob_input: Optional[int] = None,
     ):
         # --- Create a probabilistic input model
         # Select the probabilistic input model
         available_inputs = self.available_inputs
         if not prob_input_selection:
             prob_input_selection = self.default_input
         if prob_input_selection not in available_inputs:
@@ -245,20 +239,17 @@
             spatial_dimension = DEFAULT_DIMENSION
 
         # Create a ProbInput instance
         if isinstance(prob_input_spec, ProbInputSpecVarDim):
             prob_input = ProbInput.from_spec(
                 prob_input_spec,
                 spatial_dimension=spatial_dimension,
-                rng_seed=rng_seed_prob_input,
             )
         else:
-            prob_input = ProbInput.from_spec(
-                prob_input_spec, rng_seed=rng_seed_prob_input
-            )
+            prob_input = ProbInput.from_spec(prob_input_spec)
 
         # --- Select the parameters set, when applicable
         available_parameters = self.available_parameters
         if available_parameters is not None:
             if not parameters_selection:
                 parameters_selection = self.default_parameters
             if parameters_selection not in available_parameters:
```

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/core/utils.py` & `uqtestfuns-0.4.0/src/uqtestfuns/core/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/helpers.py` & `uqtestfuns-0.4.0/src/uqtestfuns/helpers.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/meta/basis_functions.py` & `uqtestfuns-0.4.0/src/uqtestfuns/meta/basis_functions.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/meta/metaspec.py` & `uqtestfuns-0.4.0/src/uqtestfuns/meta/metaspec.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/meta/uqmetatestfun.py` & `uqtestfuns-0.4.0/src/uqtestfuns/meta/uqmetatestfun.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/__init__.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 The init for the 'test_functions' subpackage of UQTestFuns.
 """
 from .ackley import Ackley
 from .borehole import Borehole
 from .bratley1992 import Bratley1992a, Bratley1992b, Bratley1992c, Bratley1992d
 from .cantilever_beam_2d import CantileverBeam2D
 from .circular_pipe_crack import CircularPipeCrack
+from .convex_fail_domain import ConvexFailDomain
+from .damped_cosine import DampedCosine
 from .damped_oscillator import DampedOscillator, DampedOscillatorReliability
 from .flood import Flood
 from .forrester import Forrester2008
 from .four_branch import FourBranch
 from .franke import Franke1, Franke2, Franke3, Franke4, Franke5, Franke6
 from .gayton_hat import GaytonHat
 from .gramacy2007 import Gramacy1DSine
 from .hyper_sphere import HyperSphere
 from .ishigami import Ishigami
 from .oakley2002 import Oakley1D
 from .otl_circuit import OTLCircuit
 from .mclain import McLainS1, McLainS2, McLainS3, McLainS4, McLainS5
 from .piston import Piston
+from .rs_circular_bar import RSCircularBar
+from .rs_quadratic import RSQuadratic
 from .sobol_g import SobolG
 from .speed_reducer_shaft import SpeedReducerShaft
 from .sulfur import Sulfur
+from .webster import Webster2D
 from .welch1992 import Welch1992
 from .wing_weight import WingWeight
 
 # NOTE: Import the new test function implementation class from its respective
 # module manually here and update the list below.
 
 __all__ = [
@@ -33,14 +38,16 @@
     "Borehole",
     "Bratley1992a",
     "Bratley1992b",
     "Bratley1992c",
     "Bratley1992d",
     "CantileverBeam2D",
     "CircularPipeCrack",
+    "ConvexFailDomain",
+    "DampedCosine",
     "DampedOscillator",
     "DampedOscillatorReliability",
     "Flood",
     "Forrester2008",
     "FourBranch",
     "Franke1",
     "Franke2",
@@ -56,13 +63,16 @@
     "OTLCircuit",
     "McLainS1",
     "McLainS2",
     "McLainS3",
     "McLainS4",
     "McLainS5",
     "Piston",
+    "RSCircularBar",
+    "RSQuadratic",
     "SobolG",
     "SpeedReducerShaft",
     "Sulfur",
+    "Webster2D",
     "Welch1992",
     "WingWeight",
 ]
```

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ackley.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/ackley.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/borehole.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/borehole.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/bratley1992.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/bratley1992.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/cantilever_beam_2d.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/cantilever_beam_2d.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/circular_pipe_crack.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/circular_pipe_crack.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/damped_oscillator.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/damped_oscillator.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/flood.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/flood.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/forrester.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/forrester.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/four_branch.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/four_branch.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/franke.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/franke.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/gayton_hat.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/gayton_hat.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/gramacy2007.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/gramacy2007.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/hyper_sphere.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/hyper_sphere.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ishigami.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/ishigami.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/mclain.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/mclain.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/oakley2002.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/oakley2002.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/otl_circuit.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/otl_circuit.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/piston.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/piston.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sobol_g.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/sobol_g.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/speed_reducer_shaft.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/speed_reducer_shaft.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sulfur.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/sulfur.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/utils.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/welch1992.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/welch1992.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/wing_weight.py` & `uqtestfuns-0.4.0/src/uqtestfuns/test_functions/wing_weight.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns/utils.py` & `uqtestfuns-0.4.0/src/uqtestfuns/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns.egg-info/PKG-INFO` & `uqtestfuns-0.4.0/src/uqtestfuns.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 Metadata-Version: 2.1
 Name: uqtestfuns
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 Home-page: https://github.com/damar-wicaksono/uqtestfuns
 Author: Damar Wicaksono
 Author-email: damar.wicaksono@outlook.com
 License: MIT
 Platform: ANY
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8109901-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8109901)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8125015-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8125015)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
-[![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
+[![PyPI](https://img.shields.io/pypi/v/uqtestfuns?style=flat-square)](https://pypi.org/project/uqtestfuns/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
 |  [`dev`](https://github.com/damar-wicaksono/uqtestfuns/tree/dev) (latest)  | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=dev&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/dev?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/dev) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=latest&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=latest)    |
 
 <!--One paragraph description-->
 UQTestFuns is an open-source Python3 library of test functions commonly used
-within the uncertainty quantification (UQ) community.
-The package aims to provide:
+within the applied uncertainty quantification (UQ) community.
+Specifically, the package provides:
 
-- a _lightweight implementation_ (with minimal dependencies) of
-  many test functions available in the UQ literature
-- a _single entry point_ (combining models and their probabilistic input
-  specification) to a wide range of test functions
-- an opportunity for an _open-source contribution_ where new test functions and
-  reference results are posted.
+- an implementation _with minimal dependencies_ (i.e., NumPy and SciPy) and
+  _a common interface_ of many test functions available in the UQ literature
+- a _single entry point_ collecting test functions _and_ their probabilistic
+  input specifications in a single Python package
+- an _opportunity for an open-source contribution_, supporting
+  the implementation of new test functions or posting reference results.
 
 In short, UQTestFuns is an homage
 to the [Virtual Library of Simulation Experiments (VLSE)](https://www.sfu.ca/~ssurjano/).
 
 ## Usage
 
 UQTestFuns includes several commonly used test functions in the UQ community.
 To list the available functions:
 
 ```python-repl
 >>> import uqtestfuns as uqtf
 >>> uqtf.list_functions()
- No.      Constructor       Spatial Dimension          Application          Description
------  ------------------  -------------------  --------------------------  ----------------------------------------------------------------------------
-  1         Ackley()                M           optimization, metamodeling  Ackley function from Ackley (1987)
-  2        Borehole()               8           metamodeling, sensitivity   Borehole function from Harper and Gupta (1983)
-  3    DampedOscillator()           8           metamodeling, sensitivity   Damped oscillator model from Igusa and Der Kiureghian (1985)
-  4         Flood()                 8           metamodeling, sensitivity   Flood model from Iooss and Lemaître (2015)
-  5        Ishigami()               3                  sensitivity          Ishigami function from Ishigami and Homma (1991)
+No.            Constructor            Dimension                Application                Description
+-----  -----------------------------  -----------  --------------------------------------  ----------------------------------------------------------------------------
+  1              Ackley()                  M             optimization, metamodeling        Optimization test function from Ackley (1987)
+  2             Borehole()                 8             metamodeling, sensitivity         Borehole function from Harper and Gupta (1983)
+  3           Bratley1992a()               M              integration, sensitivity         Integration test function #1 from Bratley et al. (1992)
+  4           Bratley1992b()               M              integration, sensitivity         Integration test function #2 from Bratley et al. (1992)
+  5           Bratley1992c()               M              integration, sensitivity         Integration test function #3 from Bratley et al. (1992)
+  6           Bratley1992d()               M              integration, sensitivity         Integration test function #4 from Bratley et al. (1992)
+  7         CantileverBeam2D()             2                    reliability                Cantilever beam reliability problem from Rajashekhar and Ellington (1993)
+  8         CircularPipeCrack()            2                    reliability                Circular pipe under bending moment from Verma et al. (2015)
 ...
 ```
 
 Consider the Borehole function, a test function commonly used for metamodeling
 and sensitivity analysis purposes; to create an instance of this test function:
 
 ```python-repl
@@ -177,11 +182,15 @@
 with tax funds on the basis of the budget approved
 by the Saxony State Parliament.
 
 UQTestFuns is currently maintained by:
 
 - Damar Wicaksono ([HZDR/CASUS](https://www.casus.science/))
 
+with scientific supervision from:
+
+- Michael Hecht ([HZDR/CASUS](https://www.casus.science/))
+
 ## License
 
 <!--License-->
 UQTestFuns is released under the [MIT License](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uqtestfuns-0.3.0/src/uqtestfuns.egg-info/SOURCES.txt` & `uqtestfuns-0.4.0/src/uqtestfuns.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,27 +39,32 @@
 src/uqtestfuns/meta/uqmetatestfun.py
 src/uqtestfuns/test_functions/__init__.py
 src/uqtestfuns/test_functions/ackley.py
 src/uqtestfuns/test_functions/borehole.py
 src/uqtestfuns/test_functions/bratley1992.py
 src/uqtestfuns/test_functions/cantilever_beam_2d.py
 src/uqtestfuns/test_functions/circular_pipe_crack.py
+src/uqtestfuns/test_functions/convex_fail_domain.py
+src/uqtestfuns/test_functions/damped_cosine.py
 src/uqtestfuns/test_functions/damped_oscillator.py
 src/uqtestfuns/test_functions/flood.py
 src/uqtestfuns/test_functions/forrester.py
 src/uqtestfuns/test_functions/four_branch.py
 src/uqtestfuns/test_functions/franke.py
 src/uqtestfuns/test_functions/gayton_hat.py
 src/uqtestfuns/test_functions/gramacy2007.py
 src/uqtestfuns/test_functions/hyper_sphere.py
 src/uqtestfuns/test_functions/ishigami.py
 src/uqtestfuns/test_functions/mclain.py
 src/uqtestfuns/test_functions/oakley2002.py
 src/uqtestfuns/test_functions/otl_circuit.py
 src/uqtestfuns/test_functions/piston.py
+src/uqtestfuns/test_functions/rs_circular_bar.py
+src/uqtestfuns/test_functions/rs_quadratic.py
 src/uqtestfuns/test_functions/sobol_g.py
 src/uqtestfuns/test_functions/speed_reducer_shaft.py
 src/uqtestfuns/test_functions/sulfur.py
 src/uqtestfuns/test_functions/utils.py
+src/uqtestfuns/test_functions/webster.py
 src/uqtestfuns/test_functions/welch1992.py
 src/uqtestfuns/test_functions/wing_weight.py
 tests/test_list_functions.py
```

### Comparing `uqtestfuns-0.3.0/tests/test_list_functions.py` & `uqtestfuns-0.4.0/tests/test_list_functions.py`

 * *Files identical despite different names*

