# Comparing `tmp/ott-jax-0.4.1.tar.gz` & `tmp/ott-jax-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ott-jax-0.4.1.tar", last modified: Tue Jun 20 14:15:35 2023, max compression
+gzip compressed data, was "ott-jax-0.4.2.tar", last modified: Thu Jul  6 22:25:50 2023, max compression
```

## Comparing `ott-jax-0.4.1.tar` & `ott-jax-0.4.2.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.305106 ott-jax-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 14:14:33.000000 ott-jax-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 14:14:33.000000 ott-jax-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-06-20 14:15:35.305106 ott-jax-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-20 14:14:33.000000 ott-jax-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 14:14:33.000000 ott-jax-0.4.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-20 14:14:33.000000 ott-jax-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:15:35.305106 ott-jax-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 14:14:33.000000 ott-jax-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.269105 ott-jax-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.277105 ott-jax-0.4.1/src/ott/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29464 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/epsilon_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32238 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/low_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/initializers/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/linear/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/linear/initializers_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/initializers/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/nn/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.285106 ott-jax-0.4.1/src/ott/initializers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/quadratic/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.285106 ott-jax-0.4.1/src/ott/math/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/fixed_point_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/matrix_square_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/unbalanced_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.285106 ott-jax-0.4.1/src/ott/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/problems/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/barycenter_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/linear_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/potentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/problems/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/nn/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/problems/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.293106 ott-jax-0.4.1/src/ott/solvers/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/continuous_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/discrete_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/implicit_differentiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/lineax_implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    46962 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.293106 ott-jax-0.4.1/src/ott/solvers/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/conjugate_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/neuraldual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.297106 ott-jax-0.4.1/src/ott/solvers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19738 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/quadratic/gromov_wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/was_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.297106 ott-jax-0.4.1/src/ott/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.301106 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/scale_tril.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/k_means.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/segment_sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/sinkhorn_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/soft_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.301106 ott-jax-0.4.1/src/ott_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-20 14:15:35.000000 ott-jax-0.4.1/src/ott_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.612058 ott-jax-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 22:24:34.000000 ott-jax-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 22:24:34.000000 ott-jax-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-06 22:25:50.612058 ott-jax-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-06 22:24:34.000000 ott-jax-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 22:24:34.000000 ott-jax-0.4.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-06 22:24:34.000000 ott-jax-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:25:50.612058 ott-jax-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 22:24:34.000000 ott-jax-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.588058 ott-jax-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/epsilon_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32238 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/low_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/initializers/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/linear/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/linear/initializers_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/initializers/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/nn/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/initializers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/quadratic/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/fixed_point_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/matrix_square_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/unbalanced_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/problems/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/barycenter_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/linear_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/potentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/problems/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/nn/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.600058 ott-jax-0.4.2/src/ott/problems/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.600058 ott-jax-0.4.2/src/ott/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.600058 ott-jax-0.4.2/src/ott/solvers/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/continuous_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/discrete_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/implicit_differentiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/lineax_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/lr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51767 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.604058 ott-jax-0.4.2/src/ott/solvers/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/conjugate_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/neuraldual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.604058 ott-jax-0.4.2/src/ott/solvers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19738 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/quadratic/gromov_wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/was_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.608058 ott-jax-0.4.2/src/ott/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.608058 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/scale_tril.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/k_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/map_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/segment_sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/sinkhorn_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/soft_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.612058 ott-jax-0.4.2/src/ott_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/top_level.txt
```

### Comparing `ott-jax-0.4.1/.gitignore` & `ott-jax-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/.pre-commit-config.yaml` & `ott-jax-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/LICENSE` & `ott-jax-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/PKG-INFO` & `ott-jax-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.1
+Version: 0.4.2
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -246,15 +246,15 @@
 ## What is OTT-JAX?
 A ``JAX`` powered library to compute optimal transport at scale and on accelerators, ``OTT-JAX`` includes the fastest
 implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling, momentum, acceleration, initializations) and extensions (low-rank, entropic maps). They can be used directly between two datasets, or within more advanced problems
 (Gromov-Wasserstein, barycenters). Some of ``JAX`` features, including
 [JIT](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Using-jit-to-speed-up-functions),
 [auto-vectorization](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Auto-vectorization-with-vmap) and
 [implicit differentiation](https://jax.readthedocs.io/en/latest/notebooks/Custom_derivative_rules_for_Python_code.html)
-work towards the goal of having end-to-end differentiable outputs. OTT-JAX is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
+work towards the goal of having end-to-end differentiable outputs. ``OTT-JAX`` is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
 
 ## Installation
 Install ``OTT-JAX`` from [PyPI](https://pypi.org/project/ott-jax/) as:
 ```bash
 pip install ott-jax
 ```
 or with ``conda`` via [conda-forge](https://anaconda.org/conda-forge/ott-jax) as:
```

### Comparing `ott-jax-0.4.1/README.md` & `ott-jax-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ## What is OTT-JAX?
 A ``JAX`` powered library to compute optimal transport at scale and on accelerators, ``OTT-JAX`` includes the fastest
 implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling, momentum, acceleration, initializations) and extensions (low-rank, entropic maps). They can be used directly between two datasets, or within more advanced problems
 (Gromov-Wasserstein, barycenters). Some of ``JAX`` features, including
 [JIT](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Using-jit-to-speed-up-functions),
 [auto-vectorization](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Auto-vectorization-with-vmap) and
 [implicit differentiation](https://jax.readthedocs.io/en/latest/notebooks/Custom_derivative_rules_for_Python_code.html)
-work towards the goal of having end-to-end differentiable outputs. OTT-JAX is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
+work towards the goal of having end-to-end differentiable outputs. ``OTT-JAX`` is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
 
 ## Installation
 Install ``OTT-JAX`` from [PyPI](https://pypi.org/project/ott-jax/) as:
 ```bash
 pip install ott-jax
 ```
 or with ``conda`` via [conda-forge](https://anaconda.org/conda-forge/ott-jax) as:
```

### Comparing `ott-jax-0.4.1/pyproject.toml` & `ott-jax-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 authors = [
     {name = "OTT team", email = "optimal.transport.tools@gmail.com"}
 ]
 dependencies = [
     "jax>=0.1.67",
     "jaxlib>=0.1.47",
     "jaxopt>=0.5.5",
-    # https://github.com/google/jax/discussions/9951#discussioncomment-3017784
-    "numpy>=1.18.4, !=1.23.0",
+    # numba/numpy compatibility issue
+    "numpy>=1.18.4, !=1.25.0",
     "flax>=0.5.2",
     "optax>=0.1.1",
     "lineax>=0.0.1; python_version >= '3.9'"
 ]
 keywords = [
     "optimal transport",
     "gromov wasserstein",
@@ -236,15 +236,15 @@
         python -m build --sdist --wheel --outdir {tox_root}{/}dist{/} {posargs:}
         twine check {tox_root}{/}dist{/}*
     commands_post =
         python -c 'import pathlib; print(f"Package is under:", pathlib.Path("{tox_root}") / "dist")'
 
     [testenv:format-references]
     description = Format references.bib.
-    deps =
+    skip_install = true
     allowlist_externals = biber
     commands = biber --tool --output_file={tox_root}{/}docs{/}references.bib --nolog \
         --output_align --output_indent=2 --output_fieldcase=lower \
         --output_legacy_dates --output-field-replace=journaltitle:journal,thesis:phdthesis,institution:school \
         {tox_root}{/}docs{/}references.bib
 """
```

### Comparing `ott-jax-0.4.1/setup.py` & `ott-jax-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/__init__.py` & `ott-jax-0.4.2/src/ott/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/_version.py` & `ott-jax-0.4.2/src/ott/_version.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/geometry/__init__.py` & `ott-jax-0.4.2/src/ott/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/geometry/costs.py` & `ott-jax-0.4.2/src/ott/geometry/costs.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 import abc
 import functools
 import math
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
+import jaxopt
 import numpy as np
 
 from ott.math import fixed_point_loop, matrix_square_root
 from ott.math import utils as mu
 
 __all__ = [
     "PNormP",
     "SqPNorm",
     "Euclidean",
     "SqEuclidean",
     "Cosine",
     "ElasticL1",
+    "ElasticL2",
     "ElasticSTVS",
     "ElasticSqKOverlap",
     "Bures",
     "UnbalancedBures",
     "SoftDTW",
 ]
 
@@ -43,16 +45,15 @@
   """Base class for all costs.
 
   Cost functions evaluate a function on a pair of inputs. For convenience,
   that function is split into two norms -- evaluated on each input separately --
   followed by a pairwise cost that involves both inputs, as in:
 
   .. math::
-
-    c(x,y) = norm(x) + norm(y) + pairwise(x,y)
+    c(x, y) = norm(x) + norm(y) + pairwise(x, y)
 
   If the :attr:`norm` function is not implemented, that value is handled as
   :math:`0`, and only :func:`pairwise` is used.
   """
 
   # no norm function created by default.
   norm: Optional[Callable[[jnp.ndarray], Union[float, jnp.ndarray]]] = None
@@ -108,15 +109,14 @@
       :math:`x`/:math:`y`.
     """
     cost = self.pairwise(x, y)
     if self.norm is None:
       return cost
     return cost + self.norm(x) + self.norm(y)
 
-  # TODO(michalk8): unused
   def all_pairs(self, x: jnp.ndarray, y: jnp.ndarray) -> jnp.ndarray:
     """Compute matrix of all pairwise costs, including the :attr:`norms <norm>`.
 
     Args:
       x: Array of shape ``[n, ...]``.
       y: Array of shape ``[m, ...]``.
 
@@ -150,30 +150,36 @@
 class TICost(CostFn):
   """Base class for translation invariant (TI) costs.
 
   Such costs are defined using a function :math:`h`, mapping vectors to
   real-values, to be used as:
 
   .. math::
-
-    c(x,y) = h(z), z := x-y.
+    c(x, y) = h(z), z := x - y.
 
   If that cost function is used to form an Entropic map using the
   :cite:`brenier:91` theorem, then the user should ensure :math:`h` is
   strictly convex, as well as provide the Legendre transform of :math:`h`,
   whose gradient is necessarily the inverse of the gradient of :math:`h`.
   """
 
   @abc.abstractmethod
   def h(self, z: jnp.ndarray) -> float:
-    """TI function acting on difference of :math:`x-y` to output cost."""
+    """TI function acting on difference of :math:`x-y` to output cost.
+
+    Args:
+      z: Array of shape ``[d,]``.
+
+    Returns:
+      The cost.
+    """
 
   def h_legendre(self, z: jnp.ndarray) -> float:
     """Legendre transform of :func:`h` when it is convex."""
-    raise NotImplementedError("`h_legendre` not implemented.")
+    raise NotImplementedError("Legendre transform of `h` is not implemented.")
 
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Compute cost as evaluation of :func:`h` on :math:`x-y`."""
     return self.h(x - y)
 
 
 @jax.tree_util.register_pytree_node_class
@@ -291,140 +297,299 @@
 
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Cosine distance between vectors, denominator regularized with ridge."""
     ridge = self._ridge
     x_norm = jnp.linalg.norm(x, axis=-1)
     y_norm = jnp.linalg.norm(y, axis=-1)
     cosine_similarity = jnp.vdot(x, y) / (x_norm * y_norm + ridge)
-    cosine_distance = 1.0 - cosine_similarity
-    # similarity is in [-1, 1], clip because of numerical imprecision
-    return jnp.clip(cosine_distance, 0., 2.)
+    return 1.0 - cosine_similarity
 
   @classmethod
   def _padder(cls, dim: int) -> jnp.ndarray:
     return jnp.ones((1, dim))
 
 
 class RegTICost(TICost, abc.ABC):
   r"""Base class for regularized translation-invariant costs.
 
   .. math::
-
-    \frac{1}{2} \|\cdot\|_2^2 + reg\left(\cdot\right)
+    \frac{1}{2} \|\cdot\|_2^2 + \text{scaling_reg} reg\left(\cdot\right)
 
   where :func:`reg` is the regularization function.
+
+  Args:
+    scaling_reg: Strength of the :meth:`regularization <reg>`.
+    matrix: :math:`p \times d` projection matrix with **orthogonal rows**.
+    orthogonal: Whether to regularize in the orthogonal complement
+      to promote displacements in the span of ``matrix``.
   """
 
+  def __init__(
+      self,
+      scaling_reg: float = 1.0,
+      matrix: Optional[jnp.ndarray] = None,
+      orthogonal: bool = False,
+  ):
+    super().__init__()
+    self.scaling_reg = scaling_reg
+    self.matrix = matrix
+    self.orthogonal = orthogonal
+
   @abc.abstractmethod
-  def reg(self, z: jnp.ndarray) -> float:
+  def _reg(self, z: jnp.ndarray) -> float:
     """Regularization function."""
 
-  def prox_reg(self, z: jnp.ndarray) -> jnp.ndarray:
-    """Proximal operator of :func:`reg`."""
+  def _reg_stiefel_orth(self, z: jnp.ndarray) -> float:
+    raise NotImplementedError(
+        "Regularization in the orthogonal "
+        "subspace is not implemented."
+    )
+
+  def reg(self, z: jnp.ndarray) -> float:
+    """Regularization function.
+
+    Args:
+      z: Array of shape ``[d,]``.
+
+    Returns:
+      The regularization value.
+    """
+    if self.matrix is None:
+      return self._reg(z)
+    if self.orthogonal:
+      return self._reg_stiefel_orth(z)
+    return self._reg(self.matrix @ z)
+
+  def prox_reg(self, z: jnp.ndarray, tau: float = 1.0) -> jnp.ndarray:
+    """Proximal operator of :meth:`reg`.
+
+    Args:
+      z: Array of shape ``[d,]``.
+      tau: Positive weight.
+
+    Returns:
+      The prox of ``z``.
+    """
+    if self.matrix is None:
+      return self._prox_reg(z, tau)
+    if self.orthogonal:
+      # regularization in the orthogonal subspace
+      return self._prox_reg_stiefel_orth(z, tau)
+    return self._prox_reg_stiefel(z, tau)
+
+  def _prox_reg(self, z: jnp.ndarray, tau: float = 1.0) -> jnp.ndarray:
     raise NotImplementedError("Proximal operator is not implemented.")
 
+  def _prox_reg_stiefel_orth(
+      self, z: jnp.ndarray, tau: float = 1.0
+  ) -> jnp.ndarray:
+
+    def orth(x: jnp.ndarray) -> jnp.ndarray:
+      return x - self.matrix.T @ (self.matrix @ x)
+
+    # assumes `matrix` has orthogonal rows
+    tmp = orth(z)
+    return z - orth(tmp - self._prox_reg(tmp, tau))
+
+  def _prox_reg_stiefel(self, z: jnp.ndarray, tau: float) -> jnp.ndarray:
+    # assumes `matrix` has orthogonal rows
+    tmp = self.matrix @ z
+    return z - self.matrix.T @ (tmp - self._prox_reg(tmp, tau))
+
+  def prox_legendre_reg(self, z: jnp.ndarray, tau: float = 1.0) -> jnp.ndarray:
+    r"""Proximal operator of the Legendre transform of :meth:`reg`.
+
+    Uses Moreau's decomposition:
+
+    .. math::
+        x = \text{prox}_{\tau f} \left(x\right) +
+        \tau \text{prox}_{\frac{1}{\tau} f^*} \left(\frac{x}{\tau}\right)
+
+    Args:
+      z: Array of shape ``[d,]``.
+      tau: Positive weight.
+
+    Returns:
+      The prox of ``z``.
+    """
+    return z - tau * self.prox_reg(z / tau, 1.0 / tau)
+
   def h(self, z: jnp.ndarray) -> float:  # noqa: D102
-    return 0.5 * jnp.linalg.norm(z, ord=2) ** 2 + self.reg(z)
+    out = 0.5 * jnp.linalg.norm(z, ord=2) ** 2
+    return out + self.scaling_reg * self.reg(z)
 
   def h_legendre(self, z: jnp.ndarray) -> float:  # noqa: D102
     q = jax.lax.stop_gradient(self.prox_reg(z))
     return jnp.sum(q * z) - self.h(q)
 
+  def h_transform(self, f: Callable[[jnp.ndarray], float],
+                  **kwargs: Any) -> Callable[[jnp.ndarray], float]:
+    r"""Compute the h-transform of a concave function.
+
+    Return a callable :math:`f_h` defined as:
+
+    .. math::
+      f_h(x) = \min_y h(x - y) - f(y)
+
+    This is equivalent, up to a change of variables, :math:`z = x - y`, to
+    define
+
+    .. math::
+      \min_z h(z) - f(x - z). \\
+      \min_z h(z) + \tilde{f}(z, x).
+
+    where :math:`\tilde{f}(z, x) := -f(x - z)`.
+
+    This is solved using proximal gradient descent, which requires having
+    access to the prox of :math:`\text{scaling_h} \cdot h` and not only to that
+    of :meth:`h`. Given the properties of :meth:`h`, the prox is obtained by
+    rescaling the output of the prox of a suitable scaling of :meth:`prox_reg`.
+
+    Args:
+      f: Concave function.
+      kwargs: Keyword arguments for :class:`~jaxopt.ProximalGradient`.
+
+    Returns:
+      The h-transform of ``f``.
+    """
+
+    def minus_f(z: jnp.ndarray, x: jnp.ndarray) -> float:
+      return -f(x - z)
+
+    def prox(
+        x: jnp.ndarray, scaling_reg: float, scaling_h: float
+    ) -> jnp.ndarray:
+      # https://web.stanford.edu/~boyd/papers/pdf/prox_algs.pdf 2.2.
+      tmp = 1.0 / (1.0 + scaling_h)
+      tau = scaling_reg * scaling_h * tmp
+      return self.prox_reg(x * tmp, tau)
+
+    def f_h(x: jnp.ndarray) -> float:
+      pg = jaxopt.ProximalGradient(fun=minus_f, prox=prox, **kwargs)
+      pg_run = pg.run(x, self.scaling_reg, x=x)
+      pg_sol = jax.lax.stop_gradient(pg_run.params)
+      return self.h(pg_sol) + minus_f(pg_sol, x)
+
+    return f_h
+
+  def tree_flatten(self):  # noqa: D102
+    return (self.scaling_reg, self.matrix), {"orthogonal": self.orthogonal}
+
+  @classmethod
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    return cls(*children, **aux_data)
+
 
 @jax.tree_util.register_pytree_node_class
 class ElasticL1(RegTICost):
   r"""Cost inspired by elastic net :cite:`zou:05` regularization.
 
   .. math::
-
-    \frac{1}{2} \|\cdot\|_2^2 + \gamma \|\cdot\|_1
+    \frac{1}{2} \|\cdot\|_2^2 + \text{scaling_reg} \|\text{matrix} \cdot\|_1
 
   Args:
-    gamma: Strength of the :math:`\|\cdot\|_1` regularization, :math:`\ge 0`.
+    scaling_reg: Strength of the :meth:`regularization <reg>`.
+    matrix: :math:`p \times d` projection matrix with **orthogonal rows**.
+    orthogonal: Whether to regularize in the orthogonal complement
+      to promote displacements in the span of ``matrix``.
   """
 
-  def __init__(self, gamma: float = 1.0):
-    super().__init__()
-    self.gamma = gamma
+  def _reg(self, z: jnp.ndarray) -> float:  # noqa: D102
+    return jnp.linalg.norm(z, ord=1)
 
-  def reg(self, z: jnp.ndarray) -> float:  # noqa: D102
-    return self.gamma * jnp.linalg.norm(z, ord=1)
+  def _prox_reg(self, z: jnp.ndarray, tau: float = 1.0) -> jnp.ndarray:
+    return jnp.sign(z) * jax.nn.relu(jnp.abs(z) - tau * self.scaling_reg)
 
-  def prox_reg(self, z: jnp.ndarray) -> float:  # noqa: D102
-    return jnp.sign(z) * jax.nn.relu(jnp.abs(z) - self.gamma)
 
-  def tree_flatten(self):  # noqa: D102
-    return (self.gamma,), None
+@jax.tree_util.register_pytree_node_class
+class ElasticL2(RegTICost):
+  r"""Cost with L2 regularization.
 
-  @classmethod
-  def tree_unflatten(cls, aux_data, children):  # noqa: D102
-    del aux_data
-    return cls(*children)
+  .. math::
+    \frac{1}{2} \|\cdot\|_2^2 + \text{scaling_reg} \|\text{matrix} \cdot\|_2^2
+
+  Args:
+    scaling_reg: Strength of the :meth:`regularization <reg>`.
+    matrix: :math:`p \times d` projection matrix with **orthogonal rows**.
+    orthogonal: Whether to regularize in the orthogonal complement
+      to promote displacements in the span of ``matrix``.
+  """
+
+  def _reg(self, z: jnp.ndarray) -> float:  # noqa: D102
+    return 0.5 * jnp.sum(z ** 2)
+
+  def _reg_stiefel_orth(self, z: jnp.ndarray) -> float:
+    # Pythagorean identity
+    return self._reg(z) - self._reg(self.matrix @ z)
+
+  def _prox_reg(self, z: jnp.ndarray, tau: float = 1.0) -> jnp.ndarray:
+    return z / (1.0 + tau * self.scaling_reg)
+
+  def _prox_reg_stiefel_orth(
+      self, z: jnp.ndarray, tau: float = 1.0
+  ) -> jnp.ndarray:
+    out = z + tau * self.scaling_reg * self.matrix.T @ (self.matrix @ z)
+    return self._prox_reg(out, tau)
 
 
 @jax.tree_util.register_pytree_node_class
 class ElasticSTVS(RegTICost):
   r"""Cost with soft thresholding operator with vanishing shrinkage (STVS)
   :cite:`schreck:15` regularization.
 
   .. math::
-
-    \frac{1}{2} \|\cdot\|_2^2 + \gamma^2\mathbf{1}_d^T\left(\sigma(\cdot) -
+    \frac{1}{2} \|\cdot\|_2^2 + \text{scaling_reg}^2\mathbf{1}_d^T\left(\sigma(\cdot) -
     \frac{1}{2} \exp\left(-2\sigma(\cdot)\right) + \frac{1}{2}\right)
 
-  where :math:`\sigma(\cdot) := \text{asinh}\left(\frac{\cdot}{2\gamma}\right)`
+  where :math:`\sigma(\cdot) := \text{asinh}\left(\frac{\cdot}
+  {2\text{scaling_reg}}\right)`
 
   Args:
-    gamma: Strength of the STVS regularization, :math:`> 0`.
-  """  # noqa
-
-  def __init__(self, gamma: float = 1.0):
-    super().__init__()
-    self.gamma = gamma
+    scaling_reg: Strength of the :meth:`regularization <reg>`.
+    matrix: :math:`p \times d` projection matrix with **orthogonal rows**.
+    orthogonal: Whether to regularize in the orthogonal complement
+      to promote displacements in the span of ``matrix``.
+  """  # noqa: D205,E501
 
-  def reg(self, z: jnp.ndarray) -> float:  # noqa: D102
-    u = jnp.arcsinh(jnp.abs(z) / (2 * self.gamma))
+  def _reg(self, z: jnp.ndarray) -> float:  # noqa: D102
+    u = jnp.arcsinh(jnp.abs(z) / (2 * self.scaling_reg))
     out = u - 0.5 * jnp.exp(-2.0 * u)
-    return (self.gamma ** 2) * jnp.sum(out + 0.5)  # make positive
-
-  def prox_reg(self, z: jnp.ndarray) -> float:  # noqa: D102
-    return jax.nn.relu(1 - (self.gamma / (jnp.abs(z) + 1e-12)) ** 2) * z
-
-  def tree_flatten(self):  # noqa: D102
-    return (self.gamma,), None
-
-  @classmethod
-  def tree_unflatten(cls, aux_data, children):  # noqa: D102
-    del aux_data
-    return cls(*children)
+    # Lemma 2.1 of `schreck:15`;
+    # don't use `self.scaling_reg ** 2` because it's included in `h`
+    return self.scaling_reg * jnp.sum(out + 0.5)  # make positive
+
+  def _prox_reg(  # noqa: D102
+      self, z: jnp.ndarray, tau: float = 1.0
+  ) -> jnp.ndarray:
+    tmp = 1.0 - (self.scaling_reg * tau / (jnp.abs(z) + 1e-12)) ** 2
+    return jax.nn.relu(tmp) * z
 
 
 @jax.tree_util.register_pytree_node_class
 class ElasticSqKOverlap(RegTICost):
   r"""Cost with squared k-overlap norm regularization :cite:`argyriou:12`.
 
   .. math::
-
-    \frac{1}{2} \|\cdot\|_2^2 + \frac{1}{2} \gamma \|\cdot\|_{ovk}^2
+    \frac{1}{2} \|\cdot\|_2^2 + \frac{1}{2} \text{scaling_reg} \|\cdot\|_{ovk}^2
 
   where :math:`\|\cdot\|_{ovk}^2` is the squared k-overlap norm,
   see def. 2.1 of :cite:`argyriou:12`.
 
   Args:
     k: Number of groups. Must be in ``[0, d)`` where :math:`d` is the
       dimensionality of the data.
-    gamma: Strength of the squared k-overlap norm regularization, :math:`> 0`.
+    args: Positional arguments for :class:`~ott.geometry.costs.RegTICost`.
+    kwargs: Keyword arguments for :class:`~ott.geometry.costs.RegTICost`.
   """
 
-  def __init__(self, k: int, gamma: float = 1.0):
-    super().__init__()
+  def __init__(self, k: int, *args, **kwargs: Any):
+    super().__init__(*args, **kwargs)
     self.k = k
-    self.gamma = gamma
 
-  def reg(self, z: jnp.ndarray) -> float:  # noqa: D102
+  def _reg(self, z: jnp.ndarray) -> float:  # noqa: D102
     # Prop 2.1 in :cite:`argyriou:12`
     k = self.k
     top_w = jax.lax.top_k(jnp.abs(z), k)[0]  # Fetch largest k values
     top_w = jnp.flip(top_w)  # Sort k-largest from smallest to largest
     # sum (dim - k) smallest values
     sum_bottom = jnp.sum(jnp.abs(z)) - jnp.sum(top_w)
     cumsum_top = jnp.cumsum(top_w)
@@ -435,17 +600,17 @@
     lower_bound = cesaro - top_w >= 0
     # Last upper bound is always True.
     upper_bound = jnp.concatenate(((top_w[1:] - cesaro[:-1] > 0),
                                    jnp.array((True,))))
     r = jnp.argmax(lower_bound * upper_bound)
     s = jnp.sum(jnp.where(jnp.arange(k) < k - r - 1, jnp.flip(top_w) ** 2, 0))
 
-    return 0.5 * self.gamma * (s + (r + 1) * cesaro[r] ** 2)
+    return 0.5 * (s + (r + 1) * cesaro[r] ** 2)
 
-  def prox_reg(self, z: jnp.ndarray) -> float:  # noqa: D102
+  def prox_reg(self, z: jnp.ndarray, tau: float = 1.0) -> float:  # noqa: D102
 
     @functools.partial(jax.vmap, in_axes=[0, None, None])
     def find_indices(r: int, l: jnp.ndarray,
                      z: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
 
       @functools.partial(jax.vmap, in_axes=[None, 0, None])
       def inner(r: int, l: int,
@@ -462,16 +627,17 @@
         cond2_right = jnp.logical_or(l == d, res >= z[l])
         cond2 = jnp.logical_and(cond2_left, cond2_right)
 
         return res, cond1 & cond2
 
       return inner(r, l, z)
 
+    del tau  # this case is not handled and currently not needed
     # Alg. 1 of :cite:`argyriou:12`
-    k, d, beta = self.k, z.shape[-1], 1.0 / self.gamma
+    k, d, beta = self.k, z.shape[-1], 1.0 / self.scaling_reg
 
     ixs = jnp.arange(d)
     z, sgn = jnp.abs(z), jnp.sign(z)
     z_ixs = jnp.argsort(z)[::-1]
     z_sorted = z[z_ixs]
 
     # (k, d - k + 1)
@@ -483,19 +649,21 @@
     q2 = (z_sorted - T) * jnp.logical_and((k - r - 1) <= ixs, ixs < (l + k))
     q = q1 + q2
 
     # change sign and reorder
     return sgn * q[jnp.argsort(z_ixs.astype(float))]
 
   def tree_flatten(self):  # noqa: D102
-    return (self.gamma,), {"k": self.k}
+    children, aux_data = super().tree_flatten()
+    return children, (self.k, aux_data)
 
   @classmethod
   def tree_unflatten(cls, aux_data, children):  # noqa: D102
-    return cls(**aux_data, gamma=children[0])
+    k, aux_data = aux_data
+    return cls(k, *children, **aux_data)
 
 
 @jax.tree_util.register_pytree_node_class
 class Bures(CostFn):
   """Bures distance between a pair of (mean, covariance matrix).
 
   Args:
```

### Comparing `ott-jax-0.4.1/src/ott/geometry/epsilon_scheduler.py` & `ott-jax-0.4.2/src/ott/geometry/epsilon_scheduler.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/geometry/geometry.py` & `ott-jax-0.4.2/src/ott/geometry/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
   Args:
     cost_matrix: Cost matrix of shape ``[n, m]``.
     kernel_matrix: Kernel matrix of shape ``[n, m]``.
     epsilon: Regularization parameter. If ``scale_epsilon = None`` and either
       ``relative_epsilon = True`` or ``relative_epsilon = None`` and
       ``epsilon = None`` in :class:`~ott.geometry.epsilon_scheduler.Epsilon`
-      is used, ``scale_epsilon`` the is :attr:`mean_cost_matrix`. If
+      is used, ``scale_epsilon`` is the :attr:`mean_cost_matrix`. If
       ``epsilon = None``, use :math:`0.05`.
     relative_epsilon: when `False`, the parameter ``epsilon`` specifies the
       value of the entropic regularization parameter. When `True`, ``epsilon``
       refers to a fraction of the :attr:`mean_cost_matrix`, which is computed
       adaptively from data.
     scale_cost: option to rescale the cost matrix. Implemented scalings are
       'median', 'mean' and 'max_cost'. Alternatively, a float factor can be
```

### Comparing `ott-jax-0.4.1/src/ott/geometry/graph.py` & `ott-jax-0.4.2/src/ott/geometry/graph.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/geometry/grid.py` & `ott-jax-0.4.2/src/ott/geometry/grid.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/geometry/low_rank.py` & `ott-jax-0.4.2/src/ott/geometry/low_rank.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/geometry/pointcloud.py` & `ott-jax-0.4.2/src/ott/geometry/pointcloud.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/geometry/segment.py` & `ott-jax-0.4.2/src/ott/geometry/segment.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/__init__.py` & `ott-jax-0.4.2/src/ott/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/linear/__init__.py` & `ott-jax-0.4.2/src/ott/initializers/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/linear/initializers.py` & `ott-jax-0.4.2/src/ott/initializers/linear/initializers.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/linear/initializers_lr.py` & `ott-jax-0.4.2/src/ott/initializers/linear/initializers_lr.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/nn/__init__.py` & `ott-jax-0.4.2/src/ott/initializers/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/nn/initializers.py` & `ott-jax-0.4.2/src/ott/initializers/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/quadratic/__init__.py` & `ott-jax-0.4.2/src/ott/initializers/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/initializers/quadratic/initializers.py` & `ott-jax-0.4.2/src/ott/initializers/quadratic/initializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,15 +188,21 @@
     Returns:
       The initial geometry used to initialize a linear problem.
     """
     from ott.solvers.linear import sinkhorn_lr
 
     q, r, g = self._linear_lr_initializer(quad_prob, **kwargs)
     tmp_out = sinkhorn_lr.LRSinkhornOutput(
-        q=q, r=r, g=g, costs=None, errors=None, ot_prob=None
+        q=q,
+        r=r,
+        g=g,
+        costs=None,
+        errors=None,
+        ot_prob=None,
+        epsilon=None,
     )
 
     return quad_prob.update_lr_geom(tmp_out)
 
   @property
   def rank(self) -> int:
     """Rank of the transport matrix factorization."""
```

### Comparing `ott-jax-0.4.1/src/ott/math/__init__.py` & `ott-jax-0.4.2/src/ott/math/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/math/fixed_point_loop.py` & `ott-jax-0.4.2/src/ott/math/fixed_point_loop.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,39 +23,39 @@
 def fixpoint_iter(
     cond_fn: Callable[[int, Any, Any], bool],
     body_fn: Callable[[Any, Any, Any, Any], Any], min_iterations: int,
     max_iterations: int, inner_iterations: int, constants: Any, state: Any
 ):
   """Implementation of a fixed point loop.
 
-  This fixed point loop iterator applies body_fn to a tuple
-  (iteration, constants, state, compute_error) to output a new state, using
+  This fixed point loop iterator applies ``body_fn`` to a tuple
+  ``(iteration, constants, state, compute_error)`` to output a new state, using
   context provided in iteration and constants.
 
-  body_fn is iterated (inner_iterations -1) times, and one last time with the
-  compute_error flag indicating that additional computational effort can be
-  spent on recalculating the latest error (errors are stored as the first
-  element of the state tuple).
-
-  upon termination of these inner_iterations, the loop is continued if iteration
-  is smaller than min_iterations, stopped if equal/larger than max_iterations,
-  and interrupted if cond_fn returns False.
+  ``body_fn`` is iterated (inner_iterations -1) times, and one last time with
+  the ``compute_error`` flag to ``True``, indicating that additional
+  computational effort can be spent on recalculating the latest error
+  (``errors`` are stored as the first element of the state tuple).
+
+  upon termination of these ``inner_iterations``, the loop is continued if
+  iteration is smaller than ``min_iterations``, stopped if equal/larger than
+  ``max_iterations``, and interrupted if ``cond_fn`` returns False.
 
   Args:
     cond_fn : termination condition function
     body_fn : body loop instructions
     min_iterations : lower bound on the total amount of fixed point iterations
     max_iterations : upper bound on the total amount of fixed point iterations
-    inner_iterations : number of iterations body_fn will be executed
-      successively before calling cond_fn.
+    inner_iterations : number of iterations ``body_fn`` will be executed
+      successively before calling ``cond_fn``.
     constants : constant (during loop) parameters passed on to body
     state : state variable
 
   Returns:
-    outputs state returned by body_fn upon termination.
+    outputs state returned by ``body_fn`` upon termination.
   """  # noqa: D401
   # If number of minimal iterations matches maximal number, force a scan instead
   # of a while loop.
 
   force_scan = (min_iterations == max_iterations)
 
   compute_error_flags = jnp.arange(inner_iterations) == inner_iterations - 1
```

### Comparing `ott-jax-0.4.1/src/ott/math/matrix_square_root.py` & `ott-jax-0.4.2/src/ott/math/matrix_square_root.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/math/unbalanced_functions.py` & `ott-jax-0.4.2/src/ott/math/unbalanced_functions.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/math/utils.py` & `ott-jax-0.4.2/src/ott/math/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,64 +8,56 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Optional
 
 import jax
-import jax.experimental.sparse as jesp
 import jax.numpy as jnp
 import jax.scipy as jsp
 
 if TYPE_CHECKING:
   from ott.geometry import costs
 
 __all__ = [
-    "safe_log", "kl", "js", "sparse_scale", "logsumexp", "softmin",
+    "safe_log", "kl", "gen_kl", "js", "logsumexp", "softmin",
     "barycentric_projection"
 ]
 
-# TODO(michalk8): move to typing.py when refactoring types
-Sparse_t = Union[jesp.CSR, jesp.CSC, jesp.COO, jesp.BCOO]
-
 
 def safe_log(  # noqa: D103
     x: jnp.ndarray,
     *,
     eps: Optional[float] = None
 ) -> jnp.ndarray:
   if eps is None:
     eps = jnp.finfo(x.dtype).tiny
   return jnp.where(x > 0., jnp.log(x), jnp.log(eps))
 
 
 # TODO(michalk8): add axis argument
 def kl(p: jnp.ndarray, q: jnp.ndarray) -> float:
-  """Kullback-Leilbler divergence."""
+  """Kullback-Leibler divergence."""
   return jnp.vdot(p, (safe_log(p) - safe_log(q)))
 
 
+def gen_kl(p: jnp.ndarray, q: jnp.ndarray) -> float:
+  """Generalized Kullback-Leibler divergence."""
+  return jnp.vdot(p, (safe_log(p) - safe_log(q))) + jnp.sum(q) - jnp.sum(p)
+
+
 # TODO(michalk8): add axis argument
-def js(p: jnp.ndarray, q: jnp.ndarray, *, c: float = 0.5) -> float:
+def js(p: jnp.ndarray, q: jnp.ndarray, c: float = 0.5) -> float:
   """Jensen-Shannon divergence."""
   return c * (kl(p, q) + kl(q, p))
 
 
-def sparse_scale(c: float, mat: Sparse_t) -> Sparse_t:
-  """Scale a sparse matrix by a constant."""
-  if isinstance(mat, jesp.BCOO):
-    # most feature complete, defer to original impl.
-    return c * mat
-  (data, *children), aux_data = mat.tree_flatten()
-  return type(mat).tree_unflatten(aux_data, [c * data] + children)
-
-
 @functools.partial(jax.custom_jvp, nondiff_argnums=(1, 2, 4))
 def logsumexp(  # noqa: D103
     mat, axis=None, keepdims=False, b=None, return_sign=False
 ):
   return jax.scipy.special.logsumexp(
       mat, axis=axis, keepdims=keepdims, b=b, return_sign=return_sign
   )
```

### Comparing `ott-jax-0.4.1/src/ott/problems/__init__.py` & `ott-jax-0.4.2/src/ott/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/linear/__init__.py` & `ott-jax-0.4.2/src/ott/problems/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/linear/barycenter_problem.py` & `ott-jax-0.4.2/src/ott/problems/linear/barycenter_problem.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/linear/linear_problem.py` & `ott-jax-0.4.2/src/ott/problems/linear/linear_problem.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/linear/potentials.py` & `ott-jax-0.4.2/src/ott/problems/linear/potentials.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/nn/__init__.py` & `ott-jax-0.4.2/src/ott/problems/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/nn/dataset.py` & `ott-jax-0.4.2/src/ott/problems/nn/dataset.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/quadratic/__init__.py` & `ott-jax-0.4.2/src/ott/problems/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/quadratic/gw_barycenter.py` & `ott-jax-0.4.2/src/ott/problems/quadratic/gw_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_costs.py` & `ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_costs.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_problem.py` & `ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_problem.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/__init__.py` & `ott-jax-0.4.2/src/ott/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/__init__.py` & `ott-jax-0.4.2/src/ott/solvers/nn/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,16 +7,8 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from . import (
-    acceleration,
-    continuous_barycenter,
-    discrete_barycenter,
-    implicit_differentiation,
-    sinkhorn,
-    sinkhorn_lr,
-)
+from . import conjugate_solvers, layers, losses, models, neuraldual
```

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/acceleration.py` & `ott-jax-0.4.2/src/ott/solvers/linear/acceleration.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/continuous_barycenter.py` & `ott-jax-0.4.2/src/ott/solvers/linear/continuous_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/discrete_barycenter.py` & `ott-jax-0.4.2/src/ott/solvers/linear/discrete_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/implicit_differentiation.py` & `ott-jax-0.4.2/src/ott/solvers/linear/implicit_differentiation.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/lineax_implicit.py` & `ott-jax-0.4.2/src/ott/solvers/linear/lineax_implicit.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn.py` & `ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     Sequence,
     Tuple,
     Union,
 )
 
 import jax
 import jax.numpy as jnp
+import jax.scipy as jsp
 import numpy as np
 from jax.experimental import host_callback
 
 from ott import utils
 from ott.geometry import geometry
 from ott.initializers.linear import initializers as init_lib
 from ott.math import fixed_point_loop
@@ -252,24 +253,24 @@
   """
   supp_a = ot_prob.a > 0
   supp_b = ot_prob.b > 0
   fa = ot_prob.geom.potential_from_scaling(ot_prob.a)
   if ot_prob.tau_a == 1.0:
     div_a = jnp.sum(jnp.where(supp_a, ot_prob.a * (f - fa), 0.0))
   else:
-    rho_a = ot_prob.epsilon * (ot_prob.tau_a / (1 - ot_prob.tau_a))
+    rho_a = uf.rho(ot_prob.epsilon, ot_prob.tau_a)
     div_a = -jnp.sum(
         jnp.where(supp_a, ot_prob.a * uf.phi_star(-(f - fa), rho_a), 0.0)
     )
 
   gb = ot_prob.geom.potential_from_scaling(ot_prob.b)
   if ot_prob.tau_b == 1.0:
     div_b = jnp.sum(jnp.where(supp_b, ot_prob.b * (g - gb), 0.0))
   else:
-    rho_b = ot_prob.epsilon * (ot_prob.tau_b / (1 - ot_prob.tau_b))
+    rho_b = uf.rho(ot_prob.epsilon, ot_prob.tau_b)
     div_b = -jnp.sum(
         jnp.where(supp_b, ot_prob.b * uf.phi_star(-(g - gb), rho_b), 0.0)
     )
 
   # Using https://arxiv.org/pdf/1910.12958.pdf (24)
   if lse_mode:
     total_sum = jnp.sum(ot_prob.geom.marginal_from_potentials(f, g))
@@ -279,21 +280,55 @@
     total_sum = jnp.sum(ot_prob.geom.marginal_from_scalings(u, v))
   return div_a + div_b + ot_prob.epsilon * (
       jnp.sum(ot_prob.a) * jnp.sum(ot_prob.b) - total_sum
   )
 
 
 class SinkhornOutput(NamedTuple):
-  """Implements the problems.Transport interface, for a Sinkhorn solution."""
+  """Holds the output of a Sinkhorn solver applied to a problem.
+
+  Objects of this class contain both solutions and problem definition of a
+  regularized OT problem, along several methods that can be used to access its
+  content, to, for instance, materialize an OT matrix or apply it to a vector
+  (without having to materialize it when not needed).
+
+  Args:
+    f: dual variables vector of size ``ot.prob.shape[0]`` returned by Sinkhorn
+    g: dual variables vector of size ``ot.prob.shape[1]`` returned by Sinkhorn
+    errors: vector or errors, along iterations. This vector is of size
+      ``max_iterations // inner_iterations`` where those were the parameters
+      passed on to the :class:`ott.solvers.linear.sinkhorn.Sinkhorn` solver.
+      For each entry indexed at ``i``, ``errors[i]`` can be either a real
+      nonnegative value (meaning the algorithm recorded that error at the
+      ``i * inner_iterations`` iteration), a ``jnp.inf`` value (meaning the
+      algorithm computed that iteration but did not compute its error, because,
+      for instance, ``i < min_iterations // inner_iterations``), or a ``-1``,
+      meaning that execution was terminated before that iteration, because the
+      criterion was found to be smaller than ``threshold``.
+    reg_ot_cost: the regularized optimal transport cost. By default this is
+      the linear contribution + KL term. See
+      :meth:`ott.solvers.linear.sinkhorn.SinkhornOutput.ent_reg_cost`,
+      :meth:`ott.solvers.linear.sinkhorn.SinkhornOutput.primal_cost` and
+      :meth:`ott.solvers.linear.sinkhorn.SinkhornOutput.dual_cost` for other
+      objective values.
+    ot_prob: stores the definition of the OT problem, including geometry,
+      marginals, unbalanced regularizers, etc.
+    threshold: convergence threshold used to control the termination of the
+      algorithm.
+    converged: whether the output corresponds to a solution whose error is
+      below the convergence threshold.
+  """
 
   f: Optional[jnp.ndarray] = None
   g: Optional[jnp.ndarray] = None
   errors: Optional[jnp.ndarray] = None
   reg_ot_cost: Optional[float] = None
   ot_prob: Optional[linear_problem.LinearProblem] = None
+  threshold: Optional[jnp.ndarray] = None
+  converged: Optional[bool] = None
 
   def set(self, **kwargs: Any) -> "SinkhornOutput":
     """Return a copy of self, with potential overwrites."""
     return self._replace(**kwargs)
 
   def set_cost(  # noqa: D102
       self, ot_prob: linear_problem.LinearProblem, lse_mode: bool,
@@ -301,25 +336,68 @@
   ) -> "SinkhornOutput":
     f = jax.lax.stop_gradient(self.f) if use_danskin else self.f
     g = jax.lax.stop_gradient(self.g) if use_danskin else self.g
     return self.set(reg_ot_cost=ent_reg_cost(f, g, ot_prob, lse_mode))
 
   @property
   def dual_cost(self) -> jnp.ndarray:
-    """Return transport cost in dual form of current solution."""
+    """Return dual transport cost, without considering regularizer."""
     a, b = self.ot_prob.a, self.ot_prob.b
     dual_cost = jnp.sum(jnp.where(a > 0.0, a * self.f, 0))
     dual_cost += jnp.sum(jnp.where(b > 0.0, b * self.g, 0))
     return dual_cost
 
   @property
   def primal_cost(self) -> float:
-    """Return transport cost of current solution at geometry."""
+    """Return transport cost of current transport solution at geometry."""
     return self.transport_cost_at_geom(other_geom=self.geom)
 
+  @property
+  def ent_reg_cost(self) -> float:
+    r"""Entropy regularized cost.
+
+    This outputs
+    .. math::
+
+      \langle P^{\star},C\rangle - \varepsilon H(P^{\star}) +
+      \rho_a\text{KL}(P^{\star} 1|a) + \rho_b\text{KL}(1^T P^{\star}|b),
+
+    where :math:`P^{\star}, a, b` is the coupling returned by the
+    :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` and the two marginal weight
+    vectors; :math:`\rho_a=\varepsilon \tau_a / (1-\tau_a)` and
+    :math:`\rho_b=\varepsilon \tau_b / (1-\tau_b)` are obtained when the problem
+    is unbalanced from parameters ``tau_a`` and ``tau_b``. Note that the last
+    two terms vanish in the balanced case, when ``tau_a==tau_b==1``.
+    """
+    ent_a = jnp.sum(jsp.special.entr(self.ot_prob.a))
+    ent_b = jnp.sum(jsp.special.entr(self.ot_prob.b))
+    return self.reg_ot_cost - self.geom.epsilon * (ent_a + ent_b)
+
+  @property
+  def kl_reg_cost(self) -> float:
+    r"""KL regularized OT transport cost.
+
+    This outputs
+    .. math::
+
+      \langle P^{\star}, C \rangle + \varepsilon KL(P^{\star},ab^T) +
+      \rho_a\text{KL}(P^{\star} 1|a) + \rho_b\text{KL}(1^T P^{\star}|b),
+
+    where :math:`P^{\star}, a, b` are the coupling returned by the
+    :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` algorithm and the two
+    marginal weight vectors, respectively, and
+    :math:`\rho_a=\varepsilon \tau_a / (1-\tau_a)` and
+    :math:`\rho_b=\varepsilon \tau_b / (1-\tau_b)` are obtained when the problem
+    is unbalanced from parameters ``tau_a`` and ``tau_b``. Note that the last
+    two terms vanish in the balanced case, when ``tau_a==tau_b==1``. This
+    quantity coincides with :attr:`reg_ot_cost`, which is computed using
+    dual variables.
+    """
+    return self.reg_ot_cost
+
   def transport_cost_at_geom(
       self, other_geom: geometry.Geometry
   ) -> jnp.ndarray:
     r"""Return bare transport cost of current solution at any geometry.
 
     In order to compute cost, we check first if the geometry can be converted
     to a low-rank cost geometry in order to speed up computations, without
@@ -356,22 +434,14 @@
   def b(self) -> jnp.ndarray:  # noqa: D102
     return self.ot_prob.b
 
   @property
   def linear_output(self) -> bool:  # noqa: D102
     return True
 
-  @property
-  def converged(self) -> bool:  # noqa: D102
-    if self.errors is None:
-      return False
-    return jnp.logical_and(
-        jnp.any(self.errors == -1), jnp.all(jnp.isfinite(self.errors))
-    )
-
   # TODO(michalk8): this should be always present
   @property
   def n_iters(self) -> int:  # noqa: D102
     if self.errors is None:
       return -1
     return jnp.sum(self.errors > -1)
 
@@ -477,15 +547,16 @@
     where :math:`KL` is the generalized Kullback-Leibler divergence.
 
     The very same primal problem can also be written using a kernel :math:`K`
     instead of a cost :math:`C` as well:
 
     .. math::
 
-      \arg\min_{P} \varepsilon KL(P|K) + \rho_a \text{KL}(P\mathbf{1}_m | a) +
+      \arg\min_{P} \varepsilon \text{KL}(P|K)
+      + \rho_a \text{KL}(P\mathbf{1}_m | a) +
       \rho_b \text{KL}(P^T \mathbf{1}_n | b)
 
     The *original* OT problem taught in linear programming courses is recovered
     by using the formulation above relying on the cost :math:`C`, and letting
     :math:`\varepsilon \rightarrow 0`, and :math:`\rho_a, \rho_b \rightarrow
     \infty`.
     In that case the entropy disappears, whereas the :math:`KL` regularization
@@ -494,42 +565,44 @@
     toolbox, which focuses exclusively on the case :math:`\varepsilon > 0`.
 
     The *balanced* regularized OT problem is recovered for finite
     :math:`\varepsilon > 0` but letting :math:`\rho_a, \rho_b \rightarrow
     \infty`. This problem can be shown to be equivalent to a matrix scaling
     problem, which can be solved using the Sinkhorn fixed-point algorithm.
     To handle the case :math:`\rho_a, \rho_b \rightarrow \infty`, the
-    ``sinkhorn`` function uses parameters :math:`tau\_a := \rho_a /
-    (\varepsilon + \rho_a)` and :math:`tau\_b := \rho_b / (\varepsilon +
-    \rho_b)` instead. Setting either of these parameters to 1 corresponds to
-    setting the corresponding :math:`\rho_a, \rho_b` to :math:`\infty`.
-
-    The Sinkhorn algorithm solves the reg-OT problem by seeking optimal `f`, `g`
-    potentials (or alternatively their parameterization as positive scalings
-    `u`, `v`), rather than solving the primal problem in :math:`P`.
-    This is mostly for efficiency (potentials and scalings have a ``n + m``
-    memory footprint, rather than ``n m`` required to store `P`). This is also
-    because both problems are, in fact, equivalent, since the optimal transport
-    math:`P^*` can be recovered from optimal potentials :math:`f^*`, :math:`g^*`
-    or scalings :math:`u^*`, :math:`v^*`, using the geometry's cost or kernel
+    ``sinkhorn`` function uses parameters ``tau_a`` and ``tau_b`` equal
+    respectively to :math:`\rho_a /(\varepsilon + \rho_a)` and
+    :math:`\rho_b / (\varepsilon + \rho_b)` instead. Setting either of these
+    parameters to 1 corresponds to setting the corresponding
+    :math:`\rho_a, \rho_b` to :math:`\infty`.
+
+    The Sinkhorn algorithm solves the reg-OT problem by seeking optimal
+    :math:`f`, :math:`g` potentials (or alternatively their parameterization
+    as positive scaling vectors :math:`u`, :math:`v`), rather than solving the
+    primal problem in :math:`P`. This is mostly for efficiency (potentials and
+    scalings have a ``n + m`` memory footprint, rather than ``n m`` required
+    to store `P`). This is also because both problems are, in fact, equivalent,
+    since the optimal transport :math:`P^{\star}` can be recovered from
+    optimal potentials :math:`f^{\star}`, :math:`g^{\star}` or scaling
+    :math:`u^{\star}`, :math:`v^{\star}`, using the geometry's cost or kernel
     matrix respectively:
 
     .. math::
 
-      P^* = \exp\left(\frac{f^*\mathbf{1}_m^T + \mathbf{1}_n g^{*T} -
-      C}{\varepsilon}\right) \text{ or } P^* = \text{diag}(u^*) K
-      \text{diag}(v^*)
-
-    By default, the Sinkhorn algorithm solves this dual problem in `f, g` or
-    `u, v` using block coordinate ascent, i.e. devising an update for each `f`
-    and `g` (resp. `u` and `v`) that cancels their respective gradients, one at
-    a time. These two iterations are repeated ``inner_iterations`` times, after
-    which the norm of these gradients will be evaluated and compared with the
-    ``threshold`` value. The iterations are then repeated as long as that error
-    exceeds ``threshold``.
+      P^{\star} = \exp\left(\frac{f^{\star}\mathbf{1}_m^T + \mathbf{1}_n g^{*T}-
+      C}{\varepsilon}\right) \text{ or } P^{\star} = \text{diag}(u^{\star}) K
+      \text{diag}(v^{\star})
+
+    By default, the Sinkhorn algorithm solves this dual problem in :math:`f, g`
+    or :math:`u, v` using block coordinate ascent, i.e. devising an update for
+    each :math:`f` and :math:`g` (resp. :math:`u` and :math:`v`) that cancels
+    their respective gradients, one at a time. These two iterations are repeated
+    ``inner_iterations`` times, after which the norm of these gradients will be
+    evaluated and compared with the ``threshold`` value. The iterations are then
+    repeated as long as that error exceeds ``threshold``.
 
   Note on Sinkhorn updates:
     The boolean flag ``lse_mode`` sets whether the algorithm is run in either:
 
     - log-sum-exp mode (``lse_mode=True``), in which case it is directly
       defined in terms of updates to `f` and `g`, using log-sum-exp
       computations. This requires access to the cost matrix :math:`C`, as it is
@@ -573,17 +646,18 @@
     updated simultaneously. Note that setting that choice to ``True`` requires
     using some form of averaging (e.g. ``momentum=0.5``). Without this, and on
     its own ``parallel_dual_updates`` won't work.
 
   Differentiation:
     The optimal solutions ``f`` and ``g`` and the optimal objective
     (``reg_ot_cost``) outputted by the Sinkhorn algorithm can be differentiated
-    w.r.t. relevant inputs ``geom``, ``a`` and ``b`` using, by default, implicit
-    differentiation of the optimality conditions (``implicit_diff``
-    not equal to ``None``). This choice has two consequences.
+    w.r.t. relevant inputs ``geom``, ``a`` and ``b``. In the default setting,
+    implicit differentiation of the optimality conditions (``implicit_diff``
+    not equal to ``None``), this has two consequences, treating ``f`` and ``g``
+    differently from ``reg_ot_cost``.
 
     - The termination criterion used to stop Sinkhorn (cancellation of
       gradient of objective w.r.t. ``f_u`` and ``g_v``) is used to differentiate
       ``f`` and ``g``, given a change in the inputs. These changes are computed
       by solving a linear system. The arguments starting with
       ``implicit_solver_*`` allow to define the linear solver that is used, and
       to control for two types or regularization (we have observed that,
@@ -655,15 +729,15 @@
     threshold: tolerance used to stop the Sinkhorn iterations. This is
       typically the deviation between a target marginal and the marginal of the
       current primal solution when either or both tau_a and tau_b are 1.0
       (balanced or semi-balanced problem), or the relative change between two
       successive solutions in the unbalanced case.
     norm_error: power used to define p-norm of error for marginal/target.
     inner_iterations: the Sinkhorn error is not recomputed at each
-      iteration but every inner_num_iter instead.
+      iteration but every ``inner_iterations`` instead.
     min_iterations: the minimum number of Sinkhorn iterations carried
       out before the error is computed and monitored.
     max_iterations: the maximum number of Sinkhorn iterations. If
       ``max_iterations`` is equal to ``min_iterations``, Sinkhorn iterations are
       run by default using a :func:`jax.lax.scan` loop rather than a custom,
       unroll-able :func:`jax.lax.while_loop` that monitors convergence.
       In that case the error is not monitored and the ``converged``
@@ -680,15 +754,17 @@
       to achieve faster convergence. Only used when ``lse_mode = True`` and
       ``tau_a < 1`` and ``tau_b < 1``.
     use_danskin: when ``True``, it is assumed the entropy regularized cost
       is evaluated using optimal potentials that are frozen, i.e. whose
       gradients have been stopped. This is useful when carrying out first order
       differentiation, and is only valid (as with ``implicit_differentiation``)
       when the algorithm has converged with a low tolerance.
-    initializer: how to compute the initial potentials/scalings.
+    initializer: how to compute the initial potentials/scalings. This refers to
+      a few possible classes implemented following the template in
+      :class:`~ott.initializers.linear.SinkhornInitializer`.
     progress_fn: callback function which gets called during the Sinkhorn
       iterations, so the user can display the error at each iteration,
       e.g., using a progress bar. See :func:`~ott.utils.default_progress_fn`
       for a basic implementation.
     kwargs_init: keyword arguments when creating the initializer.
   """
 
@@ -890,15 +966,18 @@
       state = self.kernel_step(ot_prob, state, iteration)
 
     if self.anderson:
       state = self.anderson.update_history(state, ot_prob, self.lse_mode)
 
     # re-computes error if compute_error is True, else set it to inf.
     err = jax.lax.cond(
-        jnp.logical_and(compute_error, iteration >= self.min_iterations),
+        jnp.logical_or(
+            iteration == self.max_iterations - 1,
+            jnp.logical_and(compute_error, iteration >= self.min_iterations)
+        ),
         lambda state, prob: state.solution_error(
             prob,
             self.norm_error,
             lse_mode=self.lse_mode,
             parallel_dual_updates=self.parallel_dual_updates,
             recenter=self.recenter_potentials
         )[0],
@@ -984,15 +1063,35 @@
     geom = ot_prob.geom
 
     f = state.fu if self.lse_mode else geom.potential_from_scaling(state.fu)
     g = state.gv if self.lse_mode else geom.potential_from_scaling(state.gv)
     if self.recenter_potentials:
       f, g = state.recenter(f, g, ot_prob=ot_prob)
 
-    return SinkhornOutput(f=f, g=g, errors=state.errors[:, 0])
+    # By convention, the algorithm is said to have converged if the algorithm
+    # has not nan'ed during iterations (notice some errors might be infinite,
+    # this convention is used when the error is not recomputed), and if the
+    # last recorded error is lower than the threshold. Note that this will be
+    # the case if either the algorithm terminated earlier (in which case the
+    # last state.errors[-1] = -1 by convention) or if the algorithm carried out
+    # the maximal number of iterations and its last recorded error (at -1
+    # position) is lower than the threshold.
+
+    converged = jnp.logical_and(
+        jnp.logical_not(jnp.any(jnp.isnan(state.errors))),
+        state.errors[-1] < self.threshold
+    )[0]
+
+    return SinkhornOutput(
+        f=f,
+        g=g,
+        errors=state.errors[:, 0],
+        threshold=jnp.array(self.threshold),
+        converged=converged
+    )
 
   @property
   def norm_error(self) -> Tuple[int, ...]:
     """Powers used to compute the p-norm between marginal/target."""
     # To change momentum adaptively, one needs errors in ||.||_1 norm.
     # In that case, we add this exponent to the list of errors to compute,
     # notably if that was not the error requested by the user.
```

### Comparing `ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn_lr.py` & `ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn_lr.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,48 +30,57 @@
 from jax.experimental import host_callback
 
 from ott.geometry import geometry, low_rank, pointcloud
 from ott.initializers.linear import initializers_lr as init_lib
 from ott.math import fixed_point_loop
 from ott.math import utils as mu
 from ott.problems.linear import linear_problem
-from ott.solvers.linear import sinkhorn
+from ott.solvers.linear import lr_utils, sinkhorn
 
 __all__ = ["LRSinkhorn", "LRSinkhornOutput"]
 
 ProgressCallbackFn_t = Callable[
     [Tuple[np.ndarray, np.ndarray, np.ndarray, "LRSinkhornState"]], None]
 
 
 class LRSinkhornState(NamedTuple):
   """State of the Low Rank Sinkhorn algorithm."""
-
   q: jnp.ndarray
   r: jnp.ndarray
   g: jnp.ndarray
   gamma: float
   costs: jnp.ndarray
   errors: jnp.ndarray
   crossed_threshold: bool
 
   def compute_error(  # noqa: D102
       self, previous_state: "LRSinkhornState"
   ) -> float:
-    err_1 = mu.js(self.q, previous_state.q, c=1.)
-    err_2 = mu.js(self.r, previous_state.r, c=1.)
-    err_3 = mu.js(self.g, previous_state.g, c=1.)
+    err_q = mu.js(self.q, previous_state.q, c=1.0)
+    err_r = mu.js(self.r, previous_state.r, c=1.0)
+    err_g = mu.js(self.g, previous_state.g, c=1.0)
 
-    return ((1. / self.gamma) ** 2) * (err_1 + err_2 + err_3)
+    return ((1.0 / self.gamma) ** 2) * (err_q + err_r + err_g)
 
   def reg_ot_cost(  # noqa: D102
       self,
       ot_prob: linear_problem.LinearProblem,
+      *,
+      epsilon: float,
       use_danskin: bool = False
   ) -> float:
-    return compute_reg_ot_cost(self.q, self.r, self.g, ot_prob, use_danskin)
+    """For LR Sinkhorn, this defaults to the primal cost of LR solution."""
+    return compute_reg_ot_cost(
+        self.q,
+        self.r,
+        self.g,
+        ot_prob,
+        epsilon=epsilon,
+        use_danskin=use_danskin
+    )
 
   def solution_error(  # noqa: D102
       self, ot_prob: linear_problem.LinearProblem, norm_error: Tuple[int, ...]
   ) -> jnp.ndarray:
     return solution_error(self.q, self.r, ot_prob, norm_error)
 
   def set(self, **kwargs: Any) -> "LRSinkhornState":
@@ -80,33 +89,50 @@
 
 
 def compute_reg_ot_cost(
     q: jnp.ndarray,
     r: jnp.ndarray,
     g: jnp.ndarray,
     ot_prob: linear_problem.LinearProblem,
+    epsilon: float,
     use_danskin: bool = False
 ) -> float:
-  """Compute the regularized OT cost.
+  """Compute the regularized OT cost, here the primal cost of the LR solution.
 
   Args:
     q: first factor of solution
     r: second factor of solution
     g: weights of solution
     ot_prob: linear problem
+    epsilon: Entropic regularization.
     use_danskin: if True, use Danskin's theorem :cite:`danskin:67,bertsekas:71`
       to avoid computing the gradient of the cost function.
 
   Returns:
-    regularized OT cost
+    regularized OT cost, the (primal) transport cost of the low-rank solution.
   """
+
+  def ent(x: jnp.ndarray) -> float:
+    # generalized entropy
+    return jnp.sum(jsp.special.entr(x) + x)
+
+  tau_a, tau_b = ot_prob.tau_a, ot_prob.tau_b
+
   q = jax.lax.stop_gradient(q) if use_danskin else q
   r = jax.lax.stop_gradient(r) if use_danskin else r
   g = jax.lax.stop_gradient(g) if use_danskin else g
-  return jnp.sum(ot_prob.geom.apply_cost(r, axis=1) * q * (1. / g)[None, :])
+
+  cost = jnp.sum(ot_prob.geom.apply_cost(r, axis=1) * q * (1.0 / g)[None, :])
+  cost -= epsilon * (ent(q) + ent(r) + ent(g))
+  if tau_a != 1.0:
+    cost += tau_a / (1.0 - tau_a) * mu.gen_kl(jnp.sum(q, axis=1), ot_prob.a)
+  if tau_b != 1.0:
+    cost += tau_b / (1.0 - tau_b) * mu.gen_kl(jnp.sum(r, axis=1), ot_prob.b)
+
+  return cost
 
 
 def solution_error(
     q: jnp.ndarray, r: jnp.ndarray, ot_prob: linear_problem.LinearProblem,
     norm_error: Tuple[int, ...]
 ) -> jnp.ndarray:
   """Compute solution error.
@@ -145,14 +171,15 @@
   r: jnp.ndarray
   g: jnp.ndarray
   costs: jnp.ndarray
   # TODO(michalk8): must be called `errors`, because of `store_inner_errors`
   # in future, enforce via class hierarchy
   errors: jnp.ndarray
   ot_prob: linear_problem.LinearProblem
+  epsilon: float
   # TODO(michalk8): Optional is an artifact of the current impl., refactor
   reg_ot_cost: Optional[float] = None
 
   def set(self, **kwargs: Any) -> "LRSinkhornOutput":
     """Return a copy of self, with potential overwrites."""
     return self._replace(**kwargs)
 
@@ -166,15 +193,22 @@
     return self.set(reg_ot_cost=self.compute_reg_ot_cost(ot_prob, use_danskin))
 
   def compute_reg_ot_cost(  # noqa: D102
       self,
       ot_prob: linear_problem.LinearProblem,
       use_danskin: bool = False,
   ) -> float:
-    return compute_reg_ot_cost(self.q, self.r, self.g, ot_prob, use_danskin)
+    return compute_reg_ot_cost(
+        self.q,
+        self.r,
+        self.g,
+        ot_prob,
+        epsilon=self.epsilon,
+        use_danskin=use_danskin
+    )
 
   @property
   def linear(self) -> bool:  # noqa: D102
     return isinstance(self.ot_prob, linear_problem.LinearProblem)
 
   @property
   def geom(self) -> geometry.Geometry:  # noqa: D102
@@ -258,28 +292,29 @@
       factors. Valid options are `'random'`, `'rank2'`, `'k-means'`, and
       `'generalized-k-means`. If `None`,
       :class:`~ott.initializers.linear.initializers_lr.KMeansInitializer`
       is used when the linear problem's geometry is
       :class:`~ott.geometry.pointcloud.PointCloud` or
       :class:`~ott.geometry.low_rank.LRCGeometry`. Otherwise, use
       :class:`~ott.initializers.linear.initializers_lr.RandomInitializer`.
-
-    lse_mode: Whether to run computations in lse or kernel mode. At the moment,
-      only ``lse_mode = True`` is implemented.
+    lse_mode: Whether to run computations in lse or kernel mode.
     inner_iterations: Number of inner iterations used by the algorithm before
       re-evaluating progress.
     use_danskin: Use Danskin theorem to evaluate gradient of objective w.r.t.
       input parameters. Only `True` handled at this moment.
     implicit_diff: Whether to use implicit differentiation. Currently, only
       ``implicit_diff = False`` is implemented.
     progress_fn: callback function which gets called during the Sinkhorn
       iterations, so the user can display the error at each iteration,
       e.g., using a progress bar. See :func:`~ott.utils.default_progress_fn`
       for a basic implementation.
-    kwargs_dys: Keyword arguments passed to :meth:`dykstra_update`.
+    kwargs_dys: Keyword arguments passed to :meth:`dykstra_update_lse`,
+      :meth:`dykstra_update_kernel` or one of the functions defined in
+      :mod:`ott.solvers.linear`, depending on whether the problem
+      is balanced and on the ``lse_mode``.
     kwargs_init: Keyword arguments for
       :class:`~ott.initializers.linear.initializers_lr.LRInitializer`.
     kwargs: Keyword arguments for
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn`.
   """
 
   def __init__(
@@ -339,20 +374,19 @@
         Any `None` values will be initialized using the initializer.
       rng: Random key for seeding.
       kwargs: Additional arguments when calling the initializer.
 
     Returns:
       The low-rank Sinkhorn output.
     """
-    assert ot_prob.is_balanced, "Unbalanced case is not implemented."
     initializer = self.create_initializer(ot_prob)
     init = initializer(ot_prob, *init, rng=rng, **kwargs)
     return run(ot_prob, self, init)
 
-  def _lr_costs(
+  def _get_costs(
       self,
       ot_prob: linear_problem.LinearProblem,
       state: LRSinkhornState,
   ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray, float]:
     log_q, log_r, log_g = (
         mu.safe_log(state.q), mu.safe_log(state.r), mu.safe_log(state.g)
     )
@@ -372,52 +406,24 @@
       norm_q = jnp.max(jnp.abs(grad_q)) ** 2
       norm_r = jnp.max(jnp.abs(grad_r)) ** 2
       norm_g = jnp.max(jnp.abs(grad_g)) ** 2
       gamma = self.gamma / jnp.max(jnp.array([norm_q, norm_r, norm_g]))
     else:
       gamma = self.gamma
 
-    c_q = grad_q - (1. / gamma) * log_q
-    c_r = grad_r - (1. / gamma) * log_r
-    h = -grad_g + (1. / gamma) * log_g
-    return c_q, c_r, h, gamma
+    eps_factor = 1.0 / (self.epsilon * gamma + 1.0)
+    gamma *= eps_factor
 
-  def _lr_kernels(
-      self,
-      ot_prob: linear_problem.LinearProblem,
-      state: LRSinkhornState,
-  ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray, float]:
-    log_q, log_r, log_g = (
-        mu.safe_log(state.q), mu.safe_log(state.r), mu.safe_log(state.g)
-    )
+    c_q = -gamma * grad_q + eps_factor * log_q
+    c_r = -gamma * grad_r + eps_factor * log_r
+    c_g = -gamma * grad_g + eps_factor * log_g
 
-    grad_q = ot_prob.geom.apply_cost(state.r, axis=1) / state.g[None, :]
-    grad_r = ot_prob.geom.apply_cost(state.q) / state.g[None, :]
-    diag_qcr = jnp.sum(
-        state.q * ot_prob.geom.apply_cost(state.r, axis=1), axis=0
-    )
-    grad_g = -diag_qcr / (state.g ** 2)
-    if self.is_entropic:
-      grad_q += self.epsilon * log_q
-      grad_r += self.epsilon * log_r
-      grad_g += self.epsilon * log_g
-
-    if self.gamma_rescale:
-      norm_q = jnp.max(jnp.abs(grad_q)) ** 2
-      norm_r = jnp.max(jnp.abs(grad_r)) ** 2
-      norm_g = jnp.max(jnp.abs(grad_g)) ** 2
-      gamma = self.gamma / jnp.max(jnp.array([norm_q, norm_r, norm_g]))
-    else:
-      gamma = self.gamma
-
-    k_q = jnp.exp((-gamma) * (grad_q - (1. / gamma) * log_q))
-    k_r = jnp.exp((-gamma) * (grad_r - (1. / gamma) * log_r))
-    k_g = jnp.exp((-gamma) * (grad_g - (1. / gamma) * log_g))
-    return k_q, k_r, k_g, gamma
+    return c_q, c_r, c_g, gamma
 
+  # TODO(michalk8): move to `lr_utils` when refactoring this
   def dykstra_update_lse(
       self,
       c_q: jnp.ndarray,
       c_r: jnp.ndarray,
       h: jnp.ndarray,
       gamma: float,
       ot_prob: linear_problem.LinearProblem,
@@ -629,29 +635,43 @@
     return recompute_couplings(u1, v1_old, k_q, u2, v2_old, k_r, g_old)
 
   def lse_step(
       self, ot_prob: linear_problem.LinearProblem, state: LRSinkhornState,
       iteration: int
   ) -> LRSinkhornState:
     """LR Sinkhorn LSE update."""
-    c_q, c_r, h, gamma = self._lr_costs(ot_prob, state)
-    q, r, g = self.dykstra_update_lse(
-        c_q, c_r, h, gamma, ot_prob, **self.kwargs_dys
-    )
+    c_q, c_r, c_g, gamma = self._get_costs(ot_prob, state)
+
+    if ot_prob.is_balanced:
+      c_q, c_r, h = c_q / -gamma, c_r / -gamma, c_g / gamma
+      q, r, g = self.dykstra_update_lse(
+          c_q, c_r, h, gamma, ot_prob, **self.kwargs_dys
+      )
+    else:
+      q, r, g = lr_utils.unbalanced_dykstra_lse(
+          c_q, c_r, c_g, gamma, ot_prob, **self.kwargs_dys
+      )
     return state.set(q=q, g=g, r=r, gamma=gamma)
 
   def kernel_step(
       self, ot_prob: linear_problem.LinearProblem, state: LRSinkhornState,
       iteration: int
   ) -> LRSinkhornState:
     """LR Sinkhorn Kernel update."""
-    k_q, k_r, k_g, gamma = self._lr_kernels(ot_prob, state)
-    q, r, g = self.dykstra_update_kernel(
-        k_q, k_r, k_g, gamma, ot_prob, **self.kwargs_dys
-    )
+    c_q, c_r, c_g, gamma = self._get_costs(ot_prob, state)
+    c_q, c_r, c_g = jnp.exp(c_q), jnp.exp(c_r), jnp.exp(c_g)
+
+    if ot_prob.is_balanced:
+      q, r, g = self.dykstra_update_kernel(
+          c_q, c_r, c_g, gamma, ot_prob, **self.kwargs_dys
+      )
+    else:
+      q, r, g = lr_utils.unbalanced_dykstra_kernel(
+          c_q, c_r, c_g, gamma, ot_prob, **self.kwargs_dys
+      )
     return state.set(q=q, g=g, r=r, gamma=gamma)
 
   def one_iteration(
       self, ot_prob: linear_problem.LinearProblem, state: LRSinkhornState,
       iteration: int, compute_error: bool
   ) -> LRSinkhornState:
     """Carries out one low-rank Sinkhorn iteration.
@@ -676,15 +696,16 @@
       state = self.lse_step(ot_prob, state, iteration)
     else:
       state = self.kernel_step(ot_prob, state, iteration)
 
     # re-computes error if compute_error is True, else set it to inf.
     cost = jax.lax.cond(
         jnp.logical_and(compute_error, iteration >= self.min_iterations),
-        lambda: state.reg_ot_cost(ot_prob), lambda: jnp.inf
+        lambda: state.reg_ot_cost(ot_prob, epsilon=self.epsilon),
+        lambda: jnp.inf
     )
     error = state.compute_error(previous_state)
     crossed_threshold = jnp.logical_or(
         state.crossed_threshold,
         jnp.logical_and(
             state.errors[it - 1] >= self.threshold, error < self.threshold
         )
@@ -774,14 +795,15 @@
     return LRSinkhornOutput(
         q=state.q,
         r=state.r,
         g=state.g,
         ot_prob=ot_prob,
         costs=state.costs,
         errors=state.errors,
+        epsilon=self.epsilon,
     )
 
   def _converged(self, state: LRSinkhornState, iteration: int) -> bool:
 
     def conv_crossed(prev_err: float, curr_err: float) -> bool:
       return jnp.logical_and(
           prev_err < self.threshold, curr_err < self.threshold
```

### Comparing `ott-jax-0.4.1/src/ott/solvers/nn/__init__.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import conjugate_solvers, layers, models, neuraldual
+from . import fit_gmm_pair, gaussian, gaussian_mixture, gaussian_mixture_pair
```

### Comparing `ott-jax-0.4.1/src/ott/solvers/nn/conjugate_solvers.py` & `ott-jax-0.4.2/src/ott/solvers/nn/conjugate_solvers.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/nn/layers.py` & `ott-jax-0.4.2/src/ott/solvers/nn/layers.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/nn/models.py` & `ott-jax-0.4.2/src/ott/solvers/nn/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,19 @@
 
 class ModelBase(abc.ABC, nn.Module):
   """Base class for the neural solver models."""
 
   @property
   @abc.abstractmethod
   def is_potential(self) -> bool:
-    """Indicates if the module defines the potential's value or the gradient.
+    """Indicates if the module implements a potential value or a vector field.
 
     Returns:
-      ``True`` if the module defines the potential's value, ``False``
-      if it defines the gradient.
+      ``True`` if the module defines a potential, ``False`` if it defines a
+       vector field.
     """
 
   def potential_value_fn(
       self,
       params: frozen_dict.FrozenDict[str, jnp.ndarray],
       other_potential_value_fn: Optional[PotentialValueFn_t] = None,
   ) -> PotentialValueFn_t:
@@ -85,15 +85,16 @@
 
     Args:
       params: parameters of the module
       other_potential_value_fn: function giving the value of the other
         potential. Only needed when :attr:`is_potential` is ``False``.
 
     Returns:
-      A function that can be evaluated to obtain the potential's value
+      A function that can be evaluated to obtain a potential value, or a linear
+      interpolation of a potential.
     """
     if self.is_potential:
       return lambda x: self.apply({"params": params}, x)
 
     assert other_potential_value_fn is not None, \
         "The value of the gradient-based potential depends " \
         "on the value of the other potential."
@@ -109,15 +110,15 @@
 
     return value_fn
 
   def potential_gradient_fn(
       self,
       params: frozen_dict.FrozenDict[str, jnp.ndarray],
   ) -> PotentialGradientFn_t:
-    """Return a function giving the gradient of the potential.
+    """Return a function returning a vector or the gradient of the potential.
 
     Args:
       params: parameters of the module
 
     Returns:
       A function that can be evaluated to obtain the potential's gradient
     """
@@ -298,15 +299,15 @@
       z = jnp.add(self.w_zs[i](z), self.w_xs[i + 1](x))
       z = self.act_fn(z)
     z += self.pos_def_potential(x)
     return z.squeeze()
 
 
 class MLP(ModelBase):
-  """A non-convex MLP.
+  """A generic, typically not-convex (w.r.t input) MLP.
 
   Args:
     dim_hidden: sequence specifying size of hidden dimensions. The output
       dimension of the last layer is automatically set to 1 if
       :attr:`is_potential` is ``True``, or the dimension of the input otherwise
     is_potential: Model the potential if ``True``, otherwise
       model the gradient of the potential
```

### Comparing `ott-jax-0.4.1/src/ott/solvers/nn/neuraldual.py` & `ott-jax-0.4.2/src/ott/solvers/nn/neuraldual.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/quadratic/__init__.py` & `ott-jax-0.4.2/src/ott/solvers/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/quadratic/gromov_wasserstein.py` & `ott-jax-0.4.2/src/ott/solvers/quadratic/gromov_wasserstein.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/quadratic/gw_barycenter.py` & `ott-jax-0.4.2/src/ott/solvers/quadratic/gw_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/solvers/was_solver.py` & `ott-jax-0.4.2/src/ott/solvers/was_solver.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/__init__.py` & `ott-jax-0.4.2/src/ott/solvers/linear/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,8 +7,17 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import gaussian_mixture, k_means, plot, sinkhorn_divergence, soft_sort
+
+from . import (
+    acceleration,
+    continuous_barycenter,
+    discrete_barycenter,
+    implicit_differentiation,
+    lr_utils,
+    sinkhorn,
+    sinkhorn_lr,
+)
```

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm_pair.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm_pair.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/linalg.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/linalg.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/probabilities.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/probabilities.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/scale_tril.py` & `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/scale_tril.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/k_means.py` & `ott-jax-0.4.2/src/ott/tools/k_means.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/plot.py` & `ott-jax-0.4.2/src/ott/tools/plot.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/segment_sinkhorn.py` & `ott-jax-0.4.2/src/ott/tools/segment_sinkhorn.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/tools/sinkhorn_divergence.py` & `ott-jax-0.4.2/src/ott/tools/sinkhorn_divergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,19 @@
     implicit_diff = kwargs.get("implicit_diff", None)
     if implicit_diff is not None:
       kwargs_symmetric["implicit_diff"] = implicit_diff.replace(symmetric=True)
 
   out_xy = sinkhorn.solve(geometry_xy, a, b, **kwargs)
   out_xx = sinkhorn.solve(geometry_xx, a, a, **kwargs_symmetric)
   if geometry_yy is None:
-    out_yy = sinkhorn.SinkhornOutput(errors=jnp.array([]), reg_ot_cost=0.0)
+    # Create dummy output, corresponds to scenario where static_b is True.
+    # This choice ensures that `converged`` of this dummy output is True.
+    out_yy = sinkhorn.SinkhornOutput(
+        errors=jnp.array([-jnp.inf]), reg_ot_cost=0.0, threshold=0.0
+    )
   else:
     out_yy = sinkhorn.solve(geometry_yy, b, b, **kwargs_symmetric)
 
   div = (
       out_xy.reg_ot_cost - 0.5 * (out_xx.reg_ot_cost + out_yy.reg_ot_cost) +
       0.5 * geometry_xy.epsilon * (jnp.sum(a) - jnp.sum(b)) ** 2
   )
```

### Comparing `ott-jax-0.4.1/src/ott/tools/soft_sort.py` & `ott-jax-0.4.2/src/ott/tools/soft_sort.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,67 +8,67 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Union
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from ott.geometry import pointcloud
 from ott.problems.linear import linear_problem
 from ott.solvers.linear import sinkhorn
 
 __all__ = ["sort", "ranks", "quantile"]
 
 
 def transport_for_sort(
     inputs: jnp.ndarray,
-    weights: jnp.ndarray,
-    target_weights: jnp.ndarray,
+    weights: Optional[jnp.ndarray] = None,
+    target_weights: Optional[jnp.ndarray] = None,
     squashing_fun: Optional[Callable[[jnp.ndarray], jnp.ndarray]] = None,
     epsilon: float = 1e-2,
     **kwargs: Any,
 ) -> sinkhorn.SinkhornOutput:
   r"""Solve reg. OT, from inputs to a weighted family of increasing values.
 
   Args:
-    inputs: jnp.ndarray[num_points]. Must be one dimensional.
-    weights: jnp.ndarray[num_points]. Weight vector `a` for input values.
-    target_weights: jnp.ndarray[num_targets]: Weight vector of the target
+    inputs: Array[num_points]. Must be one dimensional.
+    weights: Array[num_points]. Weight vector `a` for input values.
+    target_weights: Array[num_targets]: Weight vector of the target
       measure. It may be of different size than `weights`.
     squashing_fun: function taking an array to squash all its entries in [0,1].
       sigmoid of whitened values by default. Can be set to be the identity by
       passing ``squashing_fun = lambda x : x`` instead.
     epsilon: the regularization parameter.
     kwargs: keyword arguments for
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn`.
 
   Returns:
-    A jnp.ndarray<float> num_points x num_target transport matrix, from all
-    inputs onto the sorted target.
+    A :class:`~ott.solvers.linear.sinkhorn.SinkhornOutput` object.
   """
   shape = inputs.shape
   if len(shape) > 2 or (len(shape) == 2 and shape[1] != 1):
     raise ValueError(
         f"Shape ({shape}) not supported. The input should be one-dimensional."
     )
 
   x = jnp.expand_dims(jnp.squeeze(inputs), axis=1)
   if squashing_fun is None:
     squashing_fun = lambda z: jax.nn.sigmoid((z - jnp.mean(z)) /
                                              (jnp.std(z) + 1e-10))
   x = squashing_fun(x)
+
   a = jnp.squeeze(weights)
   b = jnp.squeeze(target_weights)
-  num_targets = b.shape[0]
+  num_targets = inputs.shape[0] if b is None else b.shape[0]
   y = jnp.linspace(0.0, 1.0, num_targets)[:, jnp.newaxis]
 
   geom = pointcloud.PointCloud(x, y, epsilon=epsilon)
   prob = linear_problem.LinearProblem(geom, a=a, b=b)
 
   solver = sinkhorn.Sinkhorn(**kwargs)
 
@@ -76,23 +76,23 @@
 
 
 def apply_on_axis(op, inputs, axis, *args, **kwargs: Any) -> jnp.ndarray:
   """Apply a differentiable operator on a given axis of the input.
 
   Args:
     op: a differentiable operator (can be ranks, quantile, etc.)
-    inputs: jnp.ndarray<float> of any shape.
+    inputs: Array of any shape.
     axis: the axis (int) or tuple of ints on which to apply the operator. If
       several axes are passed the operator, those are merged as a single
       dimension.
     args: other positional arguments to the operator.
     kwargs: other positional arguments to the operator.
 
   Returns:
-    A jnp.ndarray holding the output of the differentiable operator on the given
+    An Array holding the output of the differentiable operator on the given
     axis.
   """
   op_inner = functools.partial(op, **kwargs)
   axis = (axis,) if isinstance(axis, int) else axis
   num_points = np.prod(np.array(inputs.shape)[(axis,)])
   permutation = np.arange(len(inputs.shape))
   axis = tuple(permutation[a] for a in axis)
@@ -120,15 +120,19 @@
   if 0 < topk < num_points:
     start_index = 1
     b = jnp.concatenate([
         jnp.array([(num_points - topk) / num_points]),
         jnp.ones(topk, dtype=inputs.dtype) / num_points
     ])
   else:
-    num_targets = num_points if num_targets is None else num_targets
+    # Use the "sorting" initializer if default uniform weights of same size.
+    if num_targets is None or num_targets == num_points:
+      num_targets = num_points
+      # use sorting initializer in this case.
+      kwargs.setdefault("initializer", "sorting")
     start_index = 0
     b = jnp.ones((num_targets,)) / num_targets
   ot = transport_for_sort(inputs, a, b, **kwargs)
   out = 1.0 / b * ot.apply(inputs, axis=0)
   return out[start_index:]
 
 
@@ -137,36 +141,58 @@
     axis: int = -1,
     topk: int = -1,
     num_targets: Optional[int] = None,
     **kwargs: Any,
 ) -> jnp.ndarray:
   r"""Apply the soft sort operator on a given axis of the input.
 
+  For instance:
+
+  .. code-block:: python
+
+    x = jax.random.uniform(rng, (100,))
+    x_sorted = sort(x)
+
+
+  will output sorted convex-combinations of values contained in ``x``, that are
+  differentiable approximations to the sorted vector of entries in ``x``.
+  These can be compared with the values produced by :func:`jax.numpy.sort`,
+
+  .. code-block:: python
+
+    x_sorted = jax.numpy.sort(x)
+
+
   Args:
-    inputs: jnp.ndarray<float> of any shape.
-    axis: the axis on which to apply the operator.
+    inputs: Array of any shape.
+    axis: the axis on which to apply the soft-sorting operator.
     topk: if set to a positive value, the returned vector will only contain
-      the top-k values. This also reduces the complexity of soft sorting.
-    num_targets: if top-k is not specified, num_targets defines the number of
-      (composite) sorted values computed from the inputs (each value is a convex
-      combination of values recorded in the inputs, provided in increasing
-      order). If not specified, ``num_targets`` is set by default to be the size
-      of the slices of the input that are sorted, i.e. the number of composite
-      sorted values is equal to that of the inputs that are sorted.
+      the top-k values. This also reduces the complexity of soft-sorting, since
+      the number of target points to which the slice of the ``inputs`` tensor
+      will be mapped to will be equal to ``topk+1``.
+    num_targets: if ``topk`` is not specified, ``num_targets`` defines the
+      number of (composite) sorted values computed from the inputs (each value
+      is a convex combination of values recorded in the inputs, provided in
+      increasing order). If neither ``topk`` nor ``num_targets`` are specified,
+      ``num_targets`` defaults to the size of the slices of the input that are
+      sorted, i.e. ``inputs.shape[axis]``, and the number of composite sorted
+      values is equal to the slice of the inputs that are sorted.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
-      ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
-      solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
-      that defines the ground cost function to transport from ``inputs`` to the
-      ``num_targets`` target values (squared Euclidean distance by default, see
-      ``pointcloud.py`` for more details); ``epsilon`` values as well as other
-      parameters to shape the ``sinkhorn`` algorithm.
+      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+      to solve the optimal transport problem;
+      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+      cost function to transport from ``inputs`` to the ``num_targets`` target
+      values ; ``epsilon`` regularization
+      parameter. Remaining ``kwargs`` are passed on to defined the
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
-    A jnp.ndarray of the same shape as the input with soft sorted values on the
+    An Array of the same shape as the input with soft-sorted values on the
     given axis.
   """
   return apply_on_axis(_sort, inputs, axis, topk, num_targets, **kwargs)
 
 
 def _ranks(inputs: jnp.ndarray, num_targets, **kwargs: Any) -> jnp.ndarray:
   """Apply the soft ranks operator on a one dimensional array."""
@@ -183,86 +209,181 @@
     inputs: jnp.ndarray,
     axis: int = -1,
     num_targets: Optional[int] = None,
     **kwargs: Any,
 ) -> jnp.ndarray:
   r"""Apply the soft rank operator on input tensor.
 
+  For instance:
+
+  .. code-block:: python
+
+    x = jax.random.uniform(rng, (100,))
+    x_ranks = ranks(x)
+
+  will output fractional values, between 0 and 1, that are differentiable
+  approximations to the normalized ranks of entries in ``x``. These should be
+  compared to the non-differentiable rank vectors, namely the normalized inverse
+  permutation produced by :func:`jax.numpy.argsort`, which can be obtained as:
+
+  .. code-block:: python
+
+    x_ranks = jax.numpy.argsort(jax.numpy.argsort(x)) / x.shape[0]
+
   Args:
-    inputs: a jnp.ndarray<float> of any shape.
-    axis: the axis on which to apply the soft ranks operator.
-    num_targets: num_targets defines the number of targets used to compute a
-      composite ranks for each value in ``inputs``: that soft rank will be a
-      convex combination of values in [0,...,``(num_targets-2)/num_targets``,1]
-      specified by the optimal transport between values in ``inputs`` towards
-      those values. If not specified, ``num_targets`` is set by default to be
-      the size of the slices of the input that are sorted.
+    inputs: Array of any shape.
+    axis: the axis on which to apply the soft-sorting operator.
+    topk: if set to a positive value, the returned vector will only contain
+      the top-k values. This also reduces the complexity of soft-sorting, since
+      the number of target points to which the slice of the ``inputs`` tensor
+      will be mapped to will be equal to ``topk+1``.
+    num_targets: if ``topk`` is not specified, ``num_targets`` defines the
+      number of (composite) sorted values computed from the inputs (each value
+      is a convex combination of values recorded in the inputs, provided in
+      increasing order). If neither ``topk`` nor ``num_targets`` are specified,
+      ``num_targets`` defaults to the size of the slices of the input that are
+      sorted, i.e. ``inputs.shape[axis]``, and the number of composite sorted
+      values is equal to the slice of the inputs that are sorted.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
-      ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
-      solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
-      that defines the ground cost function to transport from ``inputs`` to the
-      ``num_targets`` target values (squared Euclidean distance by default, see
-      ``pointcloud.py`` for more details); ``epsilon`` values as well as other
-      parameters to shape the ``sinkhorn`` algorithm.
+      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+      to solve the optimal transport problem;
+      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+      cost function to transport from ``inputs`` to the ``num_targets`` target
+      values ; ``epsilon`` regularization
+      parameter. Remaining ``kwargs`` are passed on to defined the
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
-    A jnp.ndarray<float> of the same shape as inputs, with the ranks.
+    An Array of the same shape as the input with soft-rank values
+    normalized to be in :math:`[0,1]`, replacing the original ones.
+
   """
   return apply_on_axis(_ranks, inputs, axis, num_targets, **kwargs)
 
 
 def quantile(
     inputs: jnp.ndarray,
+    q: jnp.ndarray,
     axis: int = -1,
-    level: float = 0.5,
-    weight: float = 0.05,
+    weight: Optional[Union[float, jnp.ndarray]] = None,
     **kwargs: Any,
 ) -> jnp.ndarray:
-  r"""Apply the soft quantile operator on the input tensor.
+  r"""Apply the soft quantiles operator on the input tensor.
 
   For instance:
 
-  x = jax.random.uniform(rng, (1000,))
-  q = quantile(x, level=0.5, weight=0.01)
+  .. code-block:: python
+
+    x = jax.random.uniform(rng, (100,))
+    x_quantiles = quantiles(x, q=jnp.array([0.2, 0.8]))
+
+  ``x_quantiles`` will hold an approximation to the 20 and 80 percentiles in
+  ``x``, computed as a convex combination (a weighted mean, with weights summing
+  to 1) of all values in ``x`` (and not, as for standard quantiles, the
+  values ``x_sorted[20]`` and ``x_sorted[80]`` if ``x_sorted=jnp.sort(x)``).
+  These values offer a trade-off between accuracy (closeness to the true
+  percentiles) and gradient (the Jacobian of ``x_quantiles`` w.r.t ``x`` will
+  impact all values listed in ``x``, not just those indexed at 20 and 80).
+
+  The non-differentiable version is given by :func:`jax.numpy.quantile`, e.g.
+
+  .. code-block:: python
+
+    x_quantiles = jax.numpy.quantile(x, q=jnp.array([0.2, 0.8]))
 
-  Then q will be computed as a mean over the 10 median points of x.
-  Therefore, there is a trade-off between accuracy and gradient.
 
   Args:
-   inputs: a jnp.ndarray<float> of any shape.
+   inputs: an Array of any shape.
+   q: values of the quantile level to be computed, e.g. [0.5] for median.
+     These values should all lie in :math:`[0,1]`.
    axis: the axis on which to apply the operator.
-   level: the value of the quantile level to be computed. 0.5 for median.
-   weight: the weight of the quantile in the transport problem.
+   weight: the weight assigned to each quantile target value in the OT problem.
+    This weight should be small, typically of the order of ``1/n``, where ``n``
+    is the size of ``x``. Note: Since the size of ``q`` times ``weight``
+    must be strictly smaller than ``1``, in order to leave enough mass to set
+    other target values in the transport problem, the algorithm might ensure
+    this by setting, when needed, a lower value.
    kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
-      ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
-      solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
-      that defines the ground cost function to transport from ``inputs`` to the
-      ``num_targets`` target values (squared Euclidean distance by default, see
-      ``pointcloud.py`` for more details); ``epsilon`` values as well as other
-      parameters to shape the ``sinkhorn`` algorithm.
+      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+      to solve the optimal transport problem;
+      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+      cost function to transport from ``inputs`` to the ``num_targets`` target
+      values ; ``epsilon`` regularization
+      parameter. Remaining ``kwargs`` are passed on to defined the
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
-    A jnp.ndarray, which has the same shape as the input, except on the give
-    axis on which the dimension is 1.
+    An Array, which has the same shape as ``inputs``, except on the ``axis``
+    that is passed, which has size ``q.shape[0]``, to collect soft-quantile
+    values.
   """
 
   def _quantile(
-      inputs: jnp.ndarray, level: float, weight: float, **kwargs
+      inputs: jnp.ndarray, q: float, weight: float, **kwargs
   ) -> jnp.ndarray:
-    # TODO(cuturi,oliviert) option to compute several quantiles at once
     num_points = inputs.shape[0]
+    q = jnp.array([0.2, 0.5, 0.8]) if q is None else jnp.atleast_1d(q)
+    num_quantiles = q.shape[0]
     a = jnp.ones((num_points,)) / num_points
-    b = jnp.array([level - weight / 2, weight, 1.0 - weight / 2 - level])
-    ot = transport_for_sort(inputs, a, b, **kwargs)
-    out = 1.0 / b * ot.apply(jnp.squeeze(inputs), axis=0)
-    return out[1:2]
+    idx = jnp.argsort(q)
+    q = q[idx]
+
+    extended_q = jnp.concatenate([jnp.array([0.0]), q, jnp.array([1.0])])
+    filler_weights = extended_q[1:] - extended_q[:-1]
+    safe_weight = 0.5 * jnp.concatenate([
+        jnp.array([1.0 / num_quantiles]), filler_weights
+    ])
+    if weight is None:
+      # Populate with other options.
+      safe_weight = jnp.concatenate([
+          safe_weight,
+          jnp.array(
+              [.02]
+          ),  # reasonable mass per quantile for a small number of points
+          jnp.array(
+              [1.5 / num_points]
+          ),  # this means each quantile would be ~ assigned 1.5 points.
+      ])
+    else:
+      safe_weight = jnp.concatenate([safe_weight, jnp.atleast_1d(weight)])
+    weight = jnp.min(safe_weight)
+    weights = jnp.ones(filler_weights.shape) * weight
+
+    # Takes into account quantile_width in the definition of weights
+    shift = -jnp.ones(filler_weights.shape)
+    shift = shift + 0.5 * (
+        jax.nn.one_hot(0, num_quantiles + 1) +
+        jax.nn.one_hot(num_quantiles, num_quantiles + 1)
+    )
+    filler_weights = filler_weights + weights * shift
 
-  return apply_on_axis(_quantile, inputs, axis, level, weight, **kwargs)
+    # Adds one more value to have tensors of the same shape to interleave them.
+    quantile_weights = jnp.ones(num_quantiles + 1) * weights
+
+    # Interleaves the filler_weights with the quantile weights.
+    weights = jnp.reshape(
+        jnp.stack([filler_weights, quantile_weights], axis=1), (-1,)
+    )[:-1]
+
+    ot = transport_for_sort(inputs, a, weights, **kwargs)
+    out = 1.0 / weights * ot.apply(jnp.squeeze(inputs), axis=0)
+
+    # Recover odd indices corresponding to the desired quantiles.
+    odds = jnp.concatenate([
+        jnp.zeros((num_quantiles + 1, 1), dtype=bool),
+        jnp.ones((num_quantiles + 1, 1), dtype=bool)
+    ],
+                           axis=1).ravel()[:-1]
+    return out[odds][idx]
+
+  return apply_on_axis(_quantile, inputs, axis, q, weight, **kwargs)
 
 
 def _quantile_normalization(
     inputs: jnp.ndarray, targets: jnp.ndarray, weights: float, **kwargs: Any
 ) -> jnp.ndarray:
   """Apply soft quantile normalization on a one dimensional array."""
   num_points = inputs.shape[0]
@@ -276,36 +397,43 @@
     targets: jnp.ndarray,
     weights: Optional[jnp.ndarray] = None,
     axis: int = -1,
     **kwargs
 ) -> jnp.ndarray:
   r"""Renormalize inputs so that its quantiles match those of targets/weights.
 
-  The idea of quantile normalization is to map the inputs to values so that the
-  distribution of transformed values matches the distribution of target values.
-  In a sense, we want to keep the inputs in the same order, but apply the values
-  of the target.
+  Quantile normalization rearranges the values in inputs to values that match
+  the distribution of values described in the discrete distribution ``targets``
+  weighted by ``weights``. This transformation preserves the order of values
+  in ``inputs`` along the specified ``axis``.
 
   Args:
-    inputs: the inputs array of any shape.
-    targets: the target values of dimension 1. The targets must be sorted.
-    weights: if set, the weights or the target.
-    axis: the axis along which to apply the transformation on the inputs.
+    inputs: array of any shape whose values will be changed to match those in
+      ``targets``.
+    targets: sorted array (in ascending order) of dimension 1 describing a
+      discrete distribution. Note: the ``targets`` values must be provided as
+      a sorted vector.
+    weights: vector of nonnegative weights, summing to :math:`1`, of the same
+      size as ``targets``. When not set, this defaults to the uniform
+      distribution.
+    axis: the axis along which the quantile transformation is applied.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
-      ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
-      solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
-      that defines the ground cost function to transport from ``inputs`` to the
-      ``num_targets`` target values (squared Euclidean distance by default, see
-      ``pointcloud.py`` for more details); ``epsilon`` values as well as other
-      parameters to shape the ``sinkhorn`` algorithm.
+      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+      to solve the optimal transport problem;
+      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+      cost function to transport from ``inputs`` to the ``num_targets`` target
+      values ; ``epsilon`` regularization
+      parameter. Remaining ``kwargs`` are passed on to defined the
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
-    A jnp.ndarray, which has the same shape as the input, except on the give
-    axis on which the dimension is 1.
+    An array, which has the same shape as the input, except on the give axis on
+    which the dimension is 1.
 
   Raises:
     A ValueError in case the weights and the targets are both set and not of
     compatible shapes.
   """
   if weights is not None and weights.shape != targets.shape:
     raise ValueError(
@@ -333,29 +461,31 @@
   ``batch`` if ``topk`` is set to -1, as by default) composite vectors of size
   ``dim`` that will be convex combinations of all vectors, ranked from smallest
   to largest criterion. Composite vectors with the largest indices will contain
   convex combinations of those vectors with highest criterion, vectors with
   smaller indices will contain combinations of vectors with smaller criterion.
 
   Args:
-    inputs: the inputs as a jnp.ndarray[batch, dim].
+    inputs: Array of size [batch, dim].
     criterion: the values according to which to sort the inputs. It has shape
       [batch, 1].
     topk: The number of outputs to keep.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
-      ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
-      solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
-      that defines the ground cost function to transport from ``inputs`` to the
-      ``num_targets`` target values (squared Euclidean distance by default, see
-      ``pointcloud.py`` for more details); ``epsilon`` values as well as other
-      parameters to shape the ``sinkhorn`` algorithm.
+      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+      to solve the optimal transport problem;
+      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+      cost function to transport from ``inputs`` to the ``num_targets`` target
+      values ; ``epsilon`` regularization
+      parameter. Remaining ``kwargs`` are passed on to defined the
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
-    A jnp.ndarray[batch | topk, dim].
+    An Array of size [batch | topk, dim].
   """
   num_points = criterion.shape[0]
   weights = jnp.ones(num_points, dtype=criterion.dtype) / num_points
   if 0 < topk < num_points:
     start_index = 1
     target_weights = jnp.concatenate([
         jnp.array([(num_points - topk) / num_points]),
@@ -370,21 +500,19 @@
       lambda x: (1.0 / target_weights * ot.apply(x, axis=0))[start_index:],
       in_axes=(1,),
       out_axes=1
   )
   return sort_fn(inputs)
 
 
-def _quantize(
-    inputs: jnp.ndarray, num_levels: int, **kwargs: Any
-) -> jnp.ndarray:
+def _quantize(inputs: jnp.ndarray, num_q: int, **kwargs: Any) -> jnp.ndarray:
   """Apply the soft quantization operator on a one dimensional array."""
   num_points = inputs.shape[0]
   a = jnp.ones((num_points,)) / num_points
-  b = jnp.ones((num_levels,)) / num_levels
+  b = jnp.ones((num_q,)) / num_q
   ot = transport_for_sort(inputs, a, b, **kwargs)
   return 1.0 / a * ot.apply(1.0 / b * ot.apply(inputs), axis=1)
 
 
 def quantize(
     inputs: jnp.ndarray,
     num_levels: int = 10,
@@ -402,23 +530,26 @@
   values using the transportation matrix. As the regularization parameter
   ``epsilon`` of regularized optimal transport goes to 0, this operator recovers
   the expected behavior of quantization, namely each value in ``inputs`` is
   assigned a single level. When using ``epsilon>0`` the behavior is similar but
   differentiable.
 
   Args:
-    inputs: the inputs as a jnp.ndarray[batch, dim].
-    num_levels: number of levels available to quantize the signal.
+    inputs: an Array of size [batch, dim].
+    num_levels: number of quantiles available to quantize the signal.
     axis: axis along which quantization is carried out.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
-      ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
-      solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
-      that defines the ground cost function to transport from ``inputs`` to the
-      ``num_targets`` target values (squared Euclidean distance by default, see
-      ``pointcloud.py`` for more details); ``epsilon`` values as well as other
-      parameters to shape the ``sinkhorn`` algorithm.
+      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+      to solve the optimal transport problem;
+      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+      cost function to transport from ``inputs`` to the ``num_targets`` target
+      values ; ``epsilon`` regularization
+      parameter. Remaining ``kwargs`` are passed on to defined the
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
+
 
   Returns:
-    A jnp.ndarray of the same size as ``inputs``.
+    An Array of the same size as ``inputs``.
   """
   return apply_on_axis(_quantize, inputs, axis, num_levels, **kwargs)
```

### Comparing `ott-jax-0.4.1/src/ott/types.py` & `ott-jax-0.4.2/src/ott/types.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott/utils.py` & `ott-jax-0.4.2/src/ott/utils.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.1/src/ott_jax.egg-info/PKG-INFO` & `ott-jax-0.4.2/src/ott_jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.1
+Version: 0.4.2
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -246,15 +246,15 @@
 ## What is OTT-JAX?
 A ``JAX`` powered library to compute optimal transport at scale and on accelerators, ``OTT-JAX`` includes the fastest
 implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling, momentum, acceleration, initializations) and extensions (low-rank, entropic maps). They can be used directly between two datasets, or within more advanced problems
 (Gromov-Wasserstein, barycenters). Some of ``JAX`` features, including
 [JIT](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Using-jit-to-speed-up-functions),
 [auto-vectorization](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Auto-vectorization-with-vmap) and
 [implicit differentiation](https://jax.readthedocs.io/en/latest/notebooks/Custom_derivative_rules_for_Python_code.html)
-work towards the goal of having end-to-end differentiable outputs. OTT-JAX is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
+work towards the goal of having end-to-end differentiable outputs. ``OTT-JAX`` is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
 
 ## Installation
 Install ``OTT-JAX`` from [PyPI](https://pypi.org/project/ott-jax/) as:
 ```bash
 pip install ott-jax
 ```
 or with ``conda`` via [conda-forge](https://anaconda.org/conda-forge/ott-jax) as:
```

### Comparing `ott-jax-0.4.1/src/ott_jax.egg-info/SOURCES.txt` & `ott-jax-0.4.2/src/ott_jax.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,29 @@
 src/ott/solvers/was_solver.py
 src/ott/solvers/linear/__init__.py
 src/ott/solvers/linear/acceleration.py
 src/ott/solvers/linear/continuous_barycenter.py
 src/ott/solvers/linear/discrete_barycenter.py
 src/ott/solvers/linear/implicit_differentiation.py
 src/ott/solvers/linear/lineax_implicit.py
+src/ott/solvers/linear/lr_utils.py
 src/ott/solvers/linear/sinkhorn.py
 src/ott/solvers/linear/sinkhorn_lr.py
 src/ott/solvers/nn/__init__.py
 src/ott/solvers/nn/conjugate_solvers.py
 src/ott/solvers/nn/layers.py
+src/ott/solvers/nn/losses.py
 src/ott/solvers/nn/models.py
 src/ott/solvers/nn/neuraldual.py
 src/ott/solvers/quadratic/__init__.py
 src/ott/solvers/quadratic/gromov_wasserstein.py
 src/ott/solvers/quadratic/gw_barycenter.py
 src/ott/tools/__init__.py
 src/ott/tools/k_means.py
+src/ott/tools/map_estimator.py
 src/ott/tools/plot.py
 src/ott/tools/segment_sinkhorn.py
 src/ott/tools/sinkhorn_divergence.py
 src/ott/tools/soft_sort.py
 src/ott/tools/gaussian_mixture/__init__.py
 src/ott/tools/gaussian_mixture/fit_gmm.py
 src/ott/tools/gaussian_mixture/fit_gmm_pair.py
```

### Comparing `ott-jax-0.4.1/src/ott_jax.egg-info/requires.txt` & `ott-jax-0.4.2/src/ott_jax.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 jax>=0.1.67
 jaxlib>=0.1.47
 jaxopt>=0.5.5
-numpy!=1.23.0,>=1.18.4
+numpy!=1.25.0,>=1.18.4
 flax>=0.5.2
 optax>=0.1.1
 
 [:python_version >= "3.9"]
 lineax>=0.0.1
 
 [dev]
```

