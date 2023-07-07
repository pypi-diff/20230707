# Comparing `tmp/python-graphblas-2023.5.0.tar.gz` & `tmp/python-graphblas-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-graphblas-2023.5.0.tar", last modified: Wed May  3 15:17:55 2023, max compression
+gzip compressed data, was "python-graphblas-2023.7.0.tar", last modified: Fri Jul  7 21:05:48 2023, max compression
```

## Comparing `python-graphblas-2023.5.0.tar` & `python-graphblas-2023.7.0.tar`

### file list

```diff
@@ -1,128 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26264 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.565513 python-graphblas-2023.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.565513 python-graphblas-2023.5.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/docs/_static/img/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/docs/_static/img/draw-example.png
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/docs/_static/img/logo-name-medium.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/docs/_static/img/repr-matrix.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/agg/
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/agg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/agg/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/binary/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/binary/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/binary/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/core/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/agg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/automethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30152 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/infix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/infixmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    15867 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)   140889 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/core/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/agg.py
--rw-r--r--   0 runner    (1001) docker     (123)    17765 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    36090 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/indexunary.py
--rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/monoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/semiring.py
--rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/unary.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    39703 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/core/ss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)   158708 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/prefix_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    59191 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    83507 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/graphblas.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/indexunary/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/indexunary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/io/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_awkward.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_matrixmarket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/monoid/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/monoid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/monoid/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/op/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/op/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/op/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/select/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/select/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/semiring/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/semiring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/semiring/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/semiring/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/ss/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/ss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/ss/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/graphblas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle1-vanilla.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle2-vanilla.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle2.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle3-vanilla.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle3.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_auto_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_external_init.py
--rw-r--r--   0 runner    (1001) docker     (123)   187980 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_infix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)   151341 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_numpyops.py
--rw-r--r--   0 runner    (1001) docker     (123)    54654 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_operator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_prefix_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_resolving.py
--rw-r--r--   0 runner    (1001) docker     (123)    19247 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_ss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    88452 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/graphblas/unary/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/unary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/unary/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/unary/ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    16813 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/python_graphblas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26264 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.936422 python-graphblas-2023.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-07 21:05:48.936422 python-graphblas-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.920422 python-graphblas-2023.7.0/graphblas/
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.920422 python-graphblas-2023.7.0/graphblas/agg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/agg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/agg/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.920422 python-graphblas-2023.7.0/graphblas/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/binary/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/binary/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.924422 python-graphblas-2023.7.0/graphblas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/automethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30152 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/infix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/infixmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141041 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.924422 python-graphblas-2023.7.0/graphblas/core/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36112 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/indexunary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/monoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21706 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/semiring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/operator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39707 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/core/ss/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/indexunary.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158921 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/prefix_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59298 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/ss/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83796 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/core/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/dtypes/ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/graphblas.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/indexunary/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/indexunary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/indexunary/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/_awkward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/_matrixmarket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/io/_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/monoid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/monoid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/monoid/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/monoid/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/op/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/op/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/op/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/select/
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/select/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/semiring/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/semiring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/semiring/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/semiring/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.928422 python-graphblas-2023.7.0/graphblas/ss/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/ss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/ss/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.932422 python-graphblas-2023.7.0/graphblas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/pickle1-vanilla.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/pickle1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/pickle2-vanilla.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/pickle2.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/pickle3-vanilla.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/pickle3.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_auto_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_external_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187980 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_infix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151343 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_numpyops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55008 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_operator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_prefix_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_resolving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19247 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_ss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_ssjit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88800 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/tests/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.932422 python-graphblas-2023.7.0/graphblas/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/unary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/unary/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/unary/ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/graphblas/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:05:48.936422 python-graphblas-2023.7.0/python_graphblas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-07 21:05:48.000000 python-graphblas-2023.7.0/python_graphblas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-07 21:05:48.000000 python-graphblas-2023.7.0/python_graphblas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:05:48.000000 python-graphblas-2023.7.0/python_graphblas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 21:05:48.000000 python-graphblas-2023.7.0/python_graphblas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 21:05:48.000000 python-graphblas-2023.7.0/python_graphblas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:05:48.936422 python-graphblas-2023.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:05:31.000000 python-graphblas-2023.7.0/setup.py
```

### Comparing `python-graphblas-2023.5.0/LICENSE` & `python-graphblas-2023.7.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2020 Anaconda, Inc
+   Copyright 2020-2023 Anaconda, Inc. and contributors
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `python-graphblas-2023.5.0/PKG-INFO` & `python-graphblas-2023.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-graphblas
-Version: 2023.5.0
+Version: 2023.7.0
 Summary: Python library for GraphBLAS: high-performance sparse linear algebra for scalable graph analytics
 Author: Jim Kitchen, Python-graphblas contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>, Sultan Orazbayev <contact@econpoint.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -189,15 +189,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright 2020 Anaconda, Inc
+           Copyright 2020-2023 Anaconda, Inc. and contributors
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
@@ -244,15 +244,15 @@
 Provides-Extra: viz
 Provides-Extra: datashade
 Provides-Extra: test
 Provides-Extra: default
 Provides-Extra: all
 License-File: LICENSE
 
-![Python-graphblas](docs/_static/img/logo-name-medium.svg)
+![Python-graphblas](https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/logo-name-medium.svg)
 
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/python-graphblas.svg)](https://anaconda.org/conda-forge/python-graphblas)
 [![pypi](https://img.shields.io/pypi/v/python-graphblas.svg)](https://pypi.python.org/pypi/python-graphblas/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)](https://pypi.python.org/pypi/python-graphblas/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/python-graphblas/blob/main/LICENSE)
 <br>
 [![Tests](https://github.com/python-graphblas/python-graphblas/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/python-graphblas/actions)
@@ -274,16 +274,16 @@
 - **Source:** [https://github.com/python-graphblas/python-graphblas](https://github.com/python-graphblas/python-graphblas)
 - **Bug reports:** [https://github.com/python-graphblas/python-graphblas/issues](https://github.com/python-graphblas/python-graphblas/issues)
 - **Github discussions:** [https://github.com/python-graphblas/python-graphblas/discussions](https://github.com/python-graphblas/python-graphblas/discussions)
 - **Weekly community call:** [https://github.com/python-graphblas/python-graphblas/issues/247](https://github.com/python-graphblas/python-graphblas/issues/247)
 - **Chat via Discord:** [https://discord.com/invite/vur45CbwMz](https://discord.com/invite/vur45CbwMz) in the [#graphblas channel](https://discord.com/channels/786703927705862175/1024732940233605190)
 
 <p float="left">
-  <img src="docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
-  <img src="docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
+  <img src="https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
+  <img src="https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
 </p>
 
 ## Install
 Install the latest version of Python-graphblas via conda:
 ```
 $ conda install -c conda-forge python-graphblas
 ```
@@ -422,16 +422,17 @@
 ```
 ## Initialization
 There is a mechanism to initialize `graphblas` with a context prior to use. This allows for setting the backend to
 use as well as the blocking/non-blocking mode. If the context is not initialized, a default initialization will
 be performed automatically.
 ```python
 import graphblas as gb
+
 # Context initialization must happen before any other imports
-gb.init('suitesparse', blocking=True)
+gb.init("suitesparse", blocking=True)
 
 # Now we can import other items from graphblas
 from graphblas import binary, semiring
 from graphblas import Matrix, Vector, Scalar
 ```
 ## Performant User Defined Functions
 Python-graphblas requires `numba` which enables compiling user-defined Python functions to native C for use in GraphBLAS.
@@ -441,30 +442,46 @@
 from graphblas import unary
 
 def force_odd_func(x):
     if x % 2 == 0:
         return x + 1
     return x
 
-unary.register_new('force_odd', force_odd_func)
+unary.register_new("force_odd", force_odd_func)
 
 v = Vector.from_coo([0, 1, 3], [1, 2, 3])
 w = v.apply(unary.force_odd).new()
 w  # indexes=[0, 1, 3], values=[1, 3, 3]
 ```
 Similar methods exist for BinaryOp, Monoid, and Semiring.
 
+## Relation to other network analysis libraries
+Python-graphblas aims to provide an efficient and consistent expression
+of graph operations using linear algebra. This allows the development of
+high-performance implementations of existing and new graph algorithms
+(also see [`graphblas-algorithms`](https://github.com/python-graphblas/graphblas-algorithms)).
+
+While end-to-end analysis can be done using `python-graphblas`, users
+might find that other libraries in the Python ecosystem provide a more
+convenient high-level interface for data pre-processing and transformation
+(e.g. `pandas`, `scipy.sparse`), visualization (e.g. `networkx`, `igraph`),
+interactive exploration and analysis (e.g. `networkx`, `igraph`) or for
+algorithms that are not (yet) implemented in `graphblas-algorithms` (e.g.
+`networkx`, `igraph`, `scipy.sparse.csgraph`). To facilitate communication with
+other libraries, `graphblas.io` contains multiple connectors, see the
+following section.
+
 ## Import/Export connectors to the Python ecosystem
 `graphblas.io` contains functions for converting to and from:
 ```python
 import graphblas as gb
 
 # scipy.sparse matrices
 A = gb.io.from_scipy_sparse(m)
-m = gb.io.to_scipy_sparse(m, format='csr')
+m = gb.io.to_scipy_sparse(m, format="csr")
 
 # networkx graphs
 A = gb.io.from_networkx(g)
 g = gb.io.to_networkx(A)
 
 # numpy arrays can use `from_dense` and `to_dense` on Vector and Matrix
 v = gb.Vector.from_dense(m)
```

### Comparing `python-graphblas-2023.5.0/README.md` & `python-graphblas-2023.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Python-graphblas](docs/_static/img/logo-name-medium.svg)
+![Python-graphblas](https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/logo-name-medium.svg)
 
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/python-graphblas.svg)](https://anaconda.org/conda-forge/python-graphblas)
 [![pypi](https://img.shields.io/pypi/v/python-graphblas.svg)](https://pypi.python.org/pypi/python-graphblas/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)](https://pypi.python.org/pypi/python-graphblas/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/python-graphblas/blob/main/LICENSE)
 <br>
 [![Tests](https://github.com/python-graphblas/python-graphblas/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/python-graphblas/actions)
@@ -24,16 +24,16 @@
 - **Source:** [https://github.com/python-graphblas/python-graphblas](https://github.com/python-graphblas/python-graphblas)
 - **Bug reports:** [https://github.com/python-graphblas/python-graphblas/issues](https://github.com/python-graphblas/python-graphblas/issues)
 - **Github discussions:** [https://github.com/python-graphblas/python-graphblas/discussions](https://github.com/python-graphblas/python-graphblas/discussions)
 - **Weekly community call:** [https://github.com/python-graphblas/python-graphblas/issues/247](https://github.com/python-graphblas/python-graphblas/issues/247)
 - **Chat via Discord:** [https://discord.com/invite/vur45CbwMz](https://discord.com/invite/vur45CbwMz) in the [#graphblas channel](https://discord.com/channels/786703927705862175/1024732940233605190)
 
 <p float="left">
-  <img src="docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
-  <img src="docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
+  <img src="https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
+  <img src="https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
 </p>
 
 ## Install
 Install the latest version of Python-graphblas via conda:
 ```
 $ conda install -c conda-forge python-graphblas
 ```
@@ -172,16 +172,17 @@
 ```
 ## Initialization
 There is a mechanism to initialize `graphblas` with a context prior to use. This allows for setting the backend to
 use as well as the blocking/non-blocking mode. If the context is not initialized, a default initialization will
 be performed automatically.
 ```python
 import graphblas as gb
+
 # Context initialization must happen before any other imports
-gb.init('suitesparse', blocking=True)
+gb.init("suitesparse", blocking=True)
 
 # Now we can import other items from graphblas
 from graphblas import binary, semiring
 from graphblas import Matrix, Vector, Scalar
 ```
 ## Performant User Defined Functions
 Python-graphblas requires `numba` which enables compiling user-defined Python functions to native C for use in GraphBLAS.
@@ -191,30 +192,46 @@
 from graphblas import unary
 
 def force_odd_func(x):
     if x % 2 == 0:
         return x + 1
     return x
 
-unary.register_new('force_odd', force_odd_func)
+unary.register_new("force_odd", force_odd_func)
 
 v = Vector.from_coo([0, 1, 3], [1, 2, 3])
 w = v.apply(unary.force_odd).new()
 w  # indexes=[0, 1, 3], values=[1, 3, 3]
 ```
 Similar methods exist for BinaryOp, Monoid, and Semiring.
 
+## Relation to other network analysis libraries
+Python-graphblas aims to provide an efficient and consistent expression
+of graph operations using linear algebra. This allows the development of
+high-performance implementations of existing and new graph algorithms
+(also see [`graphblas-algorithms`](https://github.com/python-graphblas/graphblas-algorithms)).
+
+While end-to-end analysis can be done using `python-graphblas`, users
+might find that other libraries in the Python ecosystem provide a more
+convenient high-level interface for data pre-processing and transformation
+(e.g. `pandas`, `scipy.sparse`), visualization (e.g. `networkx`, `igraph`),
+interactive exploration and analysis (e.g. `networkx`, `igraph`) or for
+algorithms that are not (yet) implemented in `graphblas-algorithms` (e.g.
+`networkx`, `igraph`, `scipy.sparse.csgraph`). To facilitate communication with
+other libraries, `graphblas.io` contains multiple connectors, see the
+following section.
+
 ## Import/Export connectors to the Python ecosystem
 `graphblas.io` contains functions for converting to and from:
 ```python
 import graphblas as gb
 
 # scipy.sparse matrices
 A = gb.io.from_scipy_sparse(m)
-m = gb.io.to_scipy_sparse(m, format='csr')
+m = gb.io.to_scipy_sparse(m, format="csr")
 
 # networkx graphs
 A = gb.io.from_networkx(g)
 g = gb.io.to_networkx(A)
 
 # numpy arrays can use `from_dense` and `to_dense` on Vector and Matrix
 v = gb.Vector.from_dense(m)
```

### Comparing `python-graphblas-2023.5.0/graphblas/__init__.py` & `python-graphblas-2023.7.0/graphblas/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/agg/__init__.py` & `python-graphblas-2023.7.0/graphblas/agg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""`graphblas.agg` is an experimental module for exploring Aggregators.
+"""``graphblas.agg`` is an experimental module for exploring Aggregators.
 
 Aggregators may be used in reduce methods:
     - Matrix.reduce_rowwise
     - Matrix.reduce_columnwise
     - Matrix.reduce_scalar
     - Vector.reduce
 
@@ -55,17 +55,17 @@
     # These don't work with Matrix.reduce_scalar
     - ss.first_index
     - ss.last_index
     - ss.argmin
     - ss.argmax
 
 .. deprecated:: 2023.1.0
-    Aggregators `first`, `last`, `first_index`, `last_index`, `argmin`, and `argmax` are
-    deprecated in the `agg` namespace such as `agg.first`. Use them from `agg.ss` namespace
-    instead such as `agg.ss.first`. Will be removed in version 2023.9.0 or later.
+    Aggregators ``first``, ``last``, ``first_index``, ``last_index``, ``argmin``, and ``argmax``
+    are deprecated in the ``agg`` namespace such as ``agg.first``. Use them from ``agg.ss``
+    namespace instead such as ``agg.ss.first``. Will be removed in version 2023.9.0 or later.
 
 # Possible aggregators:
 #   - absolute_deviation, sum(abs(x - mean(x))),  sum_absminus(x, mean(x))
 #   - mean_absolute_deviation, absolute_deviation / count
 #   - argmini, argminj, argmaxi, argmaxj
 #   - firsti, firstj, lasti, lastj
 #   - lxnor monoid: even number of true
```

### Comparing `python-graphblas-2023.5.0/graphblas/binary/__init__.py` & `python-graphblas-2023.7.0/graphblas/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/binary/numpy.py` & `python-graphblas-2023.7.0/graphblas/binary/numpy.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/agg.py` & `python-graphblas-2023.7.0/graphblas/core/agg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """graphblas.core.agg namespace is deprecated; please use graphblas.core.operator.agg instead.
 
 .. deprecated:: 2023.3.0
-`graphblas.core.agg` will be removed in a future release.
-Use `graphblas.core.operator.agg` instead.
+``graphblas.core.agg`` will be removed in a future release.
+Use ``graphblas.core.operator.agg`` instead.
 Will be removed in version 2023.11.0 or later.
 
 """
 import warnings
 
 from .operator.agg import *  # pylint: disable=wildcard-import,unused-wildcard-import
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/automethods.py` & `python-graphblas-2023.7.0/graphblas/core/automethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Define functions to use as property methods on expressions.
 
-These will automatically compute the value and avoid the need for `.new()`.
+These will automatically compute the value and avoid the need for ``.new()``.
 
 To automatically create the functions, run:
 
 $ python -m graphblas.core.automethods
 
 """
 from .. import config
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/base.py` & `python-graphblas-2023.7.0/graphblas/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
                 # Simple assignment (w << v)
                 if self._is_scalar:
                     if accum is not None:
                         self(**opts) << self.ewise_add(expr, accum)
                         return
                     if opts:
                         # Ignore opts for now
-                        descriptor_lookup(**opts)
+                        desc = descriptor_lookup(**opts)
                     self.value = expr
                     return
 
                 # Two choices here: apply identity `expr = expr.apply(identity)`, or assign.
                 # Choose assign for now, since it works better for iso-valued objects.
                 # Perhaps we should benchmark to see which is faster and has less Python overhead.
                 self(mask=mask, accum=accum, replace=replace, input_mask=input_mask, **opts)[
@@ -367,15 +367,15 @@
                     expr = expr._to_expr()
                 elif accum is not None:
                     self(**opts) << self.ewise_add(expr, accum)
                     return
                 else:
                     if opts:
                         # Ignore opts for now
-                        descriptor_lookup(**opts)
+                        desc = descriptor_lookup(**opts)
                     self.value = expr
                     return
             else:
                 from .infix import InfixExprBase
                 from .matrix import Matrix, MatrixExpression, TransposedMatrix
 
                 if type(expr) is TransposedMatrix and type(self) is Matrix:
@@ -567,15 +567,15 @@
         if (
             mask is None
             and self._value is not None
             and (dtype is None or self._value.dtype == dtype)
         ):
             if opts:
                 # Ignore opts for now
-                descriptor_lookup(**opts)
+                desc = descriptor_lookup(**opts)  # noqa: F841 (keep desc in scope for context)
             if self._is_scalar and self._value._is_cscalar != is_cscalar:
                 return self._value.dup(is_cscalar=is_cscalar, name=name)
             rv = self._value
             if name is not None:
                 rv.name = name
             self._value = None
             return rv
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/descriptor.py` & `python-graphblas-2023.7.0/graphblas/core/descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.gb_obj = gb_obj
         self.name = f"Desc_{next(Descriptor._name_counter)}" if name is None else name
         self.output_replace = output_replace
         self.mask_complement = mask_complement
         self.mask_structure = mask_structure
         self.transpose_first = transpose_first
         self.transpose_second = transpose_second
+        self._context = None  # Used by SuiteSparse:GraphBLAS 8
 
     @property
     def _carg(self):
         return self.gb_obj[0]
 
     def __del__(self):
         gb_obj = getattr(self, "gb_obj", None)
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/expr.py` & `python-graphblas-2023.7.0/graphblas/core/expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,15 +417,15 @@
 
     def _setitem(self, resolved_indexes, obj, *, is_submask):
         # Occurs when user calls C(params)[index] = expr
         if resolved_indexes.is_single_element and not self.kwargs:
             # Fast path using assignElement
             if self.opts:
                 # Ignore opts for now
-                descriptor_lookup(**self.opts)
+                desc = descriptor_lookup(**self.opts)  # noqa: F841 (keep desc in scope for context)
             self.parent._assign_element(resolved_indexes, obj)
         else:
             mask = self.kwargs.get("mask")
             replace = self.kwargs.get("replace", False)
             expr, alt_mask = self.parent._prep_for_assign(
                 resolved_indexes,
                 obj,
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/formatting.py` & `python-graphblas-2023.7.0/graphblas/core/formatting.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/infix.py` & `python-graphblas-2023.7.0/graphblas/core/infix.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/infixmethods.py` & `python-graphblas-2023.7.0/graphblas/core/infixmethods.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/mask.py` & `python-graphblas-2023.7.0/graphblas/core/mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,35 +31,35 @@
     def _carg(self):
         return self.parent.gb_obj[0]
 
     def new(self, dtype=None, *, complement=False, mask=None, name=None, **opts):
         """Return a new object with True values determined by the mask(s).
 
         By default, the result is True wherever the mask(s) would have been applied,
-        and empty otherwise.  If `complement` is True, then these are switched:
+        and empty otherwise.  If ``complement`` is True, then these are switched:
         the result is empty where the mask(s) would have been applied, and True otherwise.
 
         In other words, these are equivalent if complement is False (and mask keyword is None):
 
         >>> C(self) << expr
         >>> C(result.S) << expr  # equivalent when complement is False
 
         And these are equivalent if complement is True (and mask keyword is None):
 
         >>> C(self) << expr
         >>> C(~result.S) << expr  # equivalent when complement is True
 
-        This can also efficiently merge two masks by using the `mask=` argument.
+        This can also efficiently merge two masks by using the ``mask=`` argument.
         This is equivalent to the following (but uses more efficient recipes):
 
         >>> val = Matrix(...)
         >>> val(self) << True
         >>> val(mask, replace=True) << val
 
-        If `complement=` argument is True, then the *complement* will be returned.
+        If ``complement=`` argument is True, then the *complement* will be returned.
         This is equivalent to the following (but uses more efficient recipes):
 
         >>> val = Matrix(...)
         >>> val(~self) << True
         >>> val(~mask) << True
 
         """
@@ -79,15 +79,15 @@
         d = _COMPLEMENT_MASKS if complement else _COMBINE_MASKS
         func = d[type(self), type(mask)]
         return func(self, mask, dtype, name, opts)
 
     def __and__(self, other, **opts):
         """Return the intersection of two masks as a new mask.
 
-        `new_mask = mask1 & mask2` is equivalent to the following:
+        ``new_mask = mask1 & mask2`` is equivalent to the following:
 
         >>> val = Matrix(bool, nrows, ncols)
         >>> val(mask1) << True
         >>> val(mask2, replace=True) << val
         >>> new_mask = val.S
 
         This uses faster recipes than the above for all combinations of input mask types,
@@ -105,15 +105,15 @@
         return StructuralMask(val)
 
     __rand__ = __and__
 
     def __or__(self, other, **opts):
         """Return the union of two masks as a new mask.
 
-        `new_mask = mask1 | mask2` is equivalent to the following:
+        ``new_mask = mask1 | mask2`` is equivalent to the following:
 
         >>> val = Matrix(bool, nrows, ncols)
         >>> val(mask1) << True
         >>> val(mask2) << True
         >>> new_mask = val.S
 
         This uses faster recipes than the above for all combinations of input mask types,
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/matrix.py` & `python-graphblas-2023.7.0/graphblas/core/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
             Absolute tolerance.
         check_dtype : bool
             If True, also checks that dtypes match
 
         Returns
         -------
         bool
-            Whether all values of the Matrix are close to the values in `other`.
+            Whether all values of the Matrix are close to the values in ``other``.
         """
         other = self._expect_type(
             other, (Matrix, TransposedMatrix), within="isclose", argname="other"
         )
         if check_dtype and self.dtype != other.dtype:
             return False
         if self._nrows != other._nrows:
@@ -444,27 +444,27 @@
         self._ncols = ncols.value
 
     def to_values(self, dtype=None, *, rows=True, columns=True, values=True, sort=True):
         """Extract the indices and values as a 3-tuple of numpy arrays
         corresponding to the COO format of the Matrix.
 
         .. deprecated:: 2022.11.0
-            `Matrix.to_values` will be removed in a future release.
-            Use `Matrix.to_coo` instead. Will be removed in version 2023.9.0 or later
+            ``Matrix.to_values`` will be removed in a future release.
+            Use ``Matrix.to_coo`` instead. Will be removed in version 2023.9.0 or later
 
         Parameters
         ----------
         dtype :
             Requested dtype for the output values array.
         rows : bool, default=True
-            Whether to return rows; will return `None` for rows if `False`
-        columns  :bool, default=True
-            Whether to return columns; will return `None` for columns if `False`
+            Whether to return rows; will return ``None`` for rows if ``False``
+        columns : bool, default=True
+            Whether to return columns; will return ``None`` for columns if ``False``
         values : bool, default=True
-            Whether to return values; will return `None` for values if `False`
+            Whether to return values; will return ``None`` for values if ``False``
         sort : bool, default=True
             Whether to require sorted indices.
             If internally stored rowwise, the sorting will be first by rows, then by column.
             If internally stored columnwise, the sorting will be first by column, then by row.
 
         Returns
         -------
@@ -484,19 +484,19 @@
         corresponding to the COO format of the Matrix.
 
         Parameters
         ----------
         dtype :
             Requested dtype for the output values array.
         rows : bool, default=True
-            Whether to return rows; will return `None` for rows if `False`
+            Whether to return rows; will return ``None`` for rows if ``False``
         columns  :bool, default=True
-            Whether to return columns; will return `None` for columns if `False`
+            Whether to return columns; will return ``None`` for columns if ``False``
         values : bool, default=True
-            Whether to return values; will return `None` for values if `False`
+            Whether to return values; will return ``None`` for values if ``False``
         sort : bool, default=True
             Whether to require sorted indices.
             If internally stored rowwise, the sorting will be first by rows, then by column.
             If internally stored columnwise, the sorting will be first by column, then by row.
 
         See Also
         --------
@@ -555,15 +555,15 @@
         This calls ``to_coo`` then transforms the data into an edgelist.
 
         Parameters
         ----------
         dtype :
             Requested dtype for the output values array.
         values : bool, default=True
-            Whether to return values; will return `None` for values if `False`
+            Whether to return values; will return ``None`` for values if ``False``
         sort : bool, default=True
             Whether to require sorted indices.
             If internally stored rowwise, the sorting will be first by rows, then by column.
             If internally stored columnwise, the sorting will be first by column, then by row.
 
         See Also
         --------
@@ -581,15 +581,15 @@
 
     def build(self, rows, columns, values, *, dup_op=None, clear=False, nrows=None, ncols=None):
         """Rarely used method to insert values into an existing Matrix.
 
         The typical use case is to create a new Matrix and insert values
         at the same time using :meth:`from_coo`.
 
-        All the arguments are used identically in :meth:`from_coo`, except for `clear`, which
+        All the arguments are used identically in :meth:`from_coo`, except for ``clear``, which
         indicates whether to clear the Matrix prior to adding the new values.
         """
         # TODO: accept `dtype` keyword to match the dtype of `values`?
         rows = ints_to_numpy_buffer(rows, np.uint64, name="row indices")
         columns = ints_to_numpy_buffer(columns, np.uint64, name="column indices")
         values, dtype = values_to_numpy_buffer(values, self.dtype)
         n = values.shape[0]
@@ -661,15 +661,15 @@
                 dtype = self.dtype
             rv = Matrix(dtype, nrows=self._nrows, ncols=self._ncols, name=name)
             if not clear:
                 rv(mask=mask, **opts)[...] = self
         else:
             if opts:
                 # Ignore opts for now
-                descriptor_lookup(**opts)
+                desc = descriptor_lookup(**opts)  # noqa: F841 (keep desc in scope for context)
             new_mat = ffi_new("GrB_Matrix*")
             rv = Matrix._from_obj(new_mat, self.dtype, self._nrows, self._ncols, name=name)
             call("GrB_Matrix_dup", [_Pointer(rv), self])
         return rv
 
     def diag(self, k=0, dtype=None, *, name=None, **opts):
         """Return a Vector built from the diagonal values of the Matrix.
@@ -777,16 +777,16 @@
         ncols=None,
         dup_op=None,
         name=None,
     ):
         """Create a new Matrix from row and column indices and values.
 
         .. deprecated:: 2022.11.0
-            `Matrix.from_values` will be removed in a future release.
-            Use `Matrix.from_coo` instead. Will be removed in version 2023.9.0 or later
+            ``Matrix.from_values`` will be removed in a future release.
+            Use ``Matrix.from_coo`` instead. Will be removed in version 2023.9.0 or later
 
         Parameters
         ----------
         rows : list or np.ndarray
             Row indices.
         columns : list or np.ndarray
             Column indices.
@@ -1082,15 +1082,15 @@
         inferred as ``nrows = len(indptr) - 1``.
 
         This always copies data. For zero-copy import with move semantics, see Matrix.ss.import_csr
 
         Parameters
         ----------
         indptr : list or np.ndarray
-            Pointers for each row into col_indices and values; `indptr.size == nrows + 1`.
+            Pointers for each row into col_indices and values; ``indptr.size == nrows + 1``.
         col_indices : list or np.ndarray
             Column indices.
         values : list or np.ndarray or scalar, default 1.0
             List of values. If a scalar is provided, all values will be set to this single value.
         dtype :
             Data type of the Matrix. If not provided, the values will be inspected
             to choose an appropriate dtype.
@@ -1129,15 +1129,15 @@
         inferred as ``ncols = len(indptr) - 1``.
 
         This always copies data. For zero-copy import with move semantics, see Matrix.ss.import_csc
 
         Parameters
         ----------
         indptr : list or np.ndarray
-            Pointers for each column into row_indices and values; `indptr.size == ncols + 1`.
+            Pointers for each column into row_indices and values; ``indptr.size == ncols + 1``.
         col_indices : list or np.ndarray
             Column indices.
         values : list or np.ndarray or scalar, default 1.0
             List of values. If a scalar is provided, all values will be set to this single value.
         dtype :
             Data type of the Matrix. If not provided, the values will be inspected
             to choose an appropriate dtype.
@@ -2703,15 +2703,15 @@
         rowidx, colidx = resolved_indexes.indices
         if self._is_transposed:
             rowidx, colidx = colidx, rowidx
         if result is None:
             result = Scalar(dtype, is_cscalar=is_cscalar, name=name)
         if opts:
             # Ignore opts for now
-            descriptor_lookup(**opts)
+            desc = descriptor_lookup(**opts)  # noqa: F841 (keep desc in scope for context)
         if is_cscalar:
             dtype_name = "UDT" if dtype._is_udt else dtype.name
             if (
                 call(
                     f"GrB_Matrix_extractElement_{dtype_name}",
                     [_Pointer(result), self, rowidx.index, colidx.index],
                 )
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/__init__.py` & `python-graphblas-2023.7.0/graphblas/core/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/agg.py` & `python-graphblas-2023.7.0/graphblas/core/operator/agg.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/base.py` & `python-graphblas-2023.7.0/graphblas/core/operator/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
                 break
         return rv
 
     @classmethod
     def _initialize(cls, include_in_ops=True):
         """
         include_in_ops determines whether the operators are included in the
-        `gb.ops` namespace in addition to the defined module.
+        ``gb.ops`` namespace in addition to the defined module.
         """
         if cls._initialized:  # pragma: no cover (safety)
             return
         # Read in the parse configs
         trim_from_front = cls._parse_config.get("trim_from_front", 0)
         delete_exact = cls._parse_config.get("delete_exact")
         num_underscores = cls._parse_config["num_underscores"]
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/binary.py` & `python-graphblas-2023.7.0/graphblas/core/operator/binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     INT16,
     INT32,
     INT64,
     UINT8,
     UINT16,
     UINT32,
     UINT64,
-    _sample_values,
     _supports_complex,
     lookup_dtype,
 )
 from ...exceptions import UdfParseError, check_status_carg
 from .. import _has_numba, _supports_udfs, ffi, lib
+from ..dtypes import _sample_values
 from ..expr import InfixExprBase
 from .base import (
     _SS_OPERATORS,
     OpBase,
     ParameterizedUdf,
     TypedOpBase,
     _call_op,
@@ -502,15 +502,15 @@
                         new_binary,
                         binary_wrapper.cffi,
                         ret_type.gb_obj,
                         type_.gb_obj,
                         type_.gb_obj,
                     ),
                     "BinaryOp",
-                    new_binary,
+                    new_binary[0],
                 )
                 op = TypedUserBinaryOp(new_type_obj, name, type_, ret_type, new_binary[0])
                 new_type_obj._add(op)
                 success = True
                 return_types[type_] = ret_type
         if success or is_udt:
             return new_type_obj
@@ -607,15 +607,15 @@
         binary_wrapper = numba.cfunc(wrapper_sig, nopython=True)(binary_wrapper)
         new_binary = ffi_new("GrB_BinaryOp*")
         check_status_carg(
             lib.GrB_BinaryOp_new(
                 new_binary, binary_wrapper.cffi, ret_type._carg, dtype._carg, dtype2._carg
             ),
             "BinaryOp",
-            new_binary,
+            new_binary[0],
         )
         op = TypedUserBinaryOp(
             self,
             self.name,
             dtype,
             ret_type,
             new_binary[0],
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/indexunary.py` & `python-graphblas-2023.7.0/graphblas/core/operator/indexunary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import inspect
 import re
 from types import FunctionType
 
 from ... import _STANDARD_OPERATOR_NAMES, indexunary, select
-from ...dtypes import BOOL, FP64, INT8, INT64, UINT64, _sample_values, lookup_dtype
+from ...dtypes import BOOL, FP64, INT8, INT64, UINT64, lookup_dtype
 from ...exceptions import UdfParseError, check_status_carg
 from .. import _has_numba, ffi, lib
+from ..dtypes import _sample_values
 from .base import OpBase, ParameterizedUdf, TypedOpBase, _call_op, _deserialize_parameterized
 
 if _has_numba:
     import numba
 
     from .base import _get_udt_wrapper
 ffi_new = ffi.new
@@ -189,15 +190,15 @@
                         new_indexunary,
                         indexunary_wrapper.cffi,
                         ret_type.gb_obj,
                         type_.gb_obj,
                         type_.gb_obj,
                     ),
                     "IndexUnaryOp",
-                    new_indexunary,
+                    new_indexunary[0],
                 )
                 op = cls._typed_user_class(new_type_obj, name, type_, ret_type, new_indexunary[0])
                 new_type_obj._add(op)
                 success = True
                 return_types[type_] = ret_type
         if success or is_udt:
             return new_type_obj
@@ -221,15 +222,15 @@
         indexunary_wrapper = numba.cfunc(wrapper_sig, nopython=True)(indexunary_wrapper)
         new_indexunary = ffi_new("GrB_IndexUnaryOp*")
         check_status_carg(
             lib.GrB_IndexUnaryOp_new(
                 new_indexunary, indexunary_wrapper.cffi, ret_type._carg, dtype._carg, dtype2._carg
             ),
             "IndexUnaryOp",
-            new_indexunary,
+            new_indexunary[0],
         )
         op = TypedUserIndexUnaryOp(
             self,
             self.name,
             dtype,
             ret_type,
             new_indexunary[0],
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/monoid.py` & `python-graphblas-2023.7.0/graphblas/core/operator/monoid.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/select.py` & `python-graphblas-2023.7.0/graphblas/core/operator/select.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/semiring.py` & `python-graphblas-2023.7.0/graphblas/core/operator/semiring.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
                 or monoid.coercions.get(binary_out, binary_out) != binary_out
             ):
                 continue
             new_semiring = ffi_new("GrB_Semiring*")
             check_status_carg(
                 lib.GrB_Semiring_new(new_semiring, monoid[binary_out].gb_obj, binary_func.gb_obj),
                 "Semiring",
-                new_semiring,
+                new_semiring[0],
             )
             ret_type = monoid[binary_out].return_type
             op = TypedUserSemiring(
                 new_type_obj,
                 name,
                 binary_in,
                 ret_type,
@@ -250,15 +250,15 @@
         if dtypes in self._udt_types:
             return self._udt_ops[dtypes]
         binaryop = self.binaryop._compile_udt(dtype, dtype2)
         monoid = self.monoid[binaryop.return_type]
         ret_type = monoid.return_type
         new_semiring = ffi_new("GrB_Semiring*")
         status = lib.GrB_Semiring_new(new_semiring, monoid.gb_obj, binaryop.gb_obj)
-        check_status_carg(status, "Semiring", new_semiring)
+        check_status_carg(status, "Semiring", new_semiring[0])
         op = TypedUserSemiring(
             new_semiring,
             self.name,
             dtype,
             ret_type,
             new_semiring[0],
             monoid,
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/unary.py` & `python-graphblas-2023.7.0/graphblas/core/operator/unary.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     INT16,
     INT32,
     INT64,
     UINT8,
     UINT16,
     UINT32,
     UINT64,
-    _sample_values,
     _supports_complex,
     lookup_dtype,
 )
 from ...exceptions import UdfParseError, check_status_carg
 from .. import _has_numba, ffi, lib
+from ..dtypes import _sample_values
 from ..utils import output_type
 from .base import (
     _SS_OPERATORS,
     OpBase,
     ParameterizedUdf,
     TypedOpBase,
     _deserialize_parameterized,
@@ -235,15 +235,15 @@
                 unary_wrapper = numba.cfunc(wrapper_sig, nopython=True)(unary_wrapper)
                 new_unary = ffi_new("GrB_UnaryOp*")
                 check_status_carg(
                     lib.GrB_UnaryOp_new(
                         new_unary, unary_wrapper.cffi, ret_type.gb_obj, type_.gb_obj
                     ),
                     "UnaryOp",
-                    new_unary,
+                    new_unary[0],
                 )
                 op = TypedUserUnaryOp(new_type_obj, name, type_, ret_type, new_unary[0])
                 new_type_obj._add(op)
                 success = True
                 return_types[type_] = ret_type
         if success or is_udt:
             return new_type_obj
@@ -260,15 +260,15 @@
 
         unary_wrapper, wrapper_sig = _get_udt_wrapper(numba_func, ret_type, dtype)
         unary_wrapper = numba.cfunc(wrapper_sig, nopython=True)(unary_wrapper)
         new_unary = ffi_new("GrB_UnaryOp*")
         check_status_carg(
             lib.GrB_UnaryOp_new(new_unary, unary_wrapper.cffi, ret_type._carg, dtype._carg),
             "UnaryOp",
-            new_unary,
+            new_unary[0],
         )
         op = TypedUserUnaryOp(self, self.name, dtype, ret_type, new_unary[0])
         self._udt_types[dtype] = ret_type
         self._udt_ops[dtype] = op
         return op
 
     @classmethod
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/operator/utils.py` & `python-graphblas-2023.7.0/graphblas/core/operator/utils.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/recorder.py` & `python-graphblas-2023.7.0/graphblas/core/recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         return f"{'M' if c == 'M' else c.lower()}_temp"
     return name
 
 
 class Recorder:
     """Record GraphBLAS C calls.
 
-    The recorder can use `.start()` and `.stop()` to enable/disable recording,
+    The recorder can use ``.start()`` and ``.stop()`` to enable/disable recording,
     or it can be used as a context manager.
 
     For example,
 
     >>> with Recorder() as rec:
     ...     C = A.mxm(B).new()
     >>> rec.data[0]
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/scalar.py` & `python-graphblas-2023.7.0/graphblas/core/scalar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1052,15 +1052,15 @@
         return Scalar.from_value(scalar, dtype, is_cscalar=is_cscalar, name="")
     if scalar._is_cscalar != is_cscalar or dtype is not None and scalar.dtype != dtype:
         return scalar.dup(dtype, is_cscalar=is_cscalar, name=scalar.name)
     return scalar
 
 
 def _dict_to_record(np_type, d):
-    """Converts e.g. `{"x": 1, "y": 2.3}` to `(1, 2.3)`."""
+    """Converts e.g. ``{"x": 1, "y": 2.3}`` to ``(1, 2.3)``."""
     rv = []
     for name, (dtype, _) in np_type.fields.items():
         val = d[name]
         if dtype.names is not None and isinstance(val, dict):
             rv.append(_dict_to_record(dtype, val))
         else:
             rv.append(val)
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/slice.py` & `python-graphblas-2023.7.0/graphblas/core/slice.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/ss/config.py` & `python-graphblas-2023.7.0/graphblas/core/ss/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 class BaseConfig(MutableMapping):
     _initialized = False
     # Subclasses should redefine these
     _get_function = None
     _set_function = None
+    _context_get_function = "GxB_Context_get"
+    _context_set_function = "GxB_Context_set"
+    _context_keys = set()
     _null_valid = {}
     _options = {}
     _defaults = {}
     # We add reverse lookups for _enumerations and _bitwise in __init__
     _bitwise = {}
     _enumerations = {}
     _read_only = set()
@@ -24,15 +27,15 @@
         "int",
         "int32_t",
         "GrB_Desc_Value",
         "GrB_Mode",
         "GxB_Format_Value",
     }
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, context=None):
         cls = type(self)
         if not cls._initialized:
             cls._reverse_enumerations = {}
             for key, d in self._enumerations.items():
                 cls._reverse_enumerations[key] = rd = {}
                 for k, v in list(d.items()):
                     if v not in d:
@@ -47,37 +50,46 @@
                     if v not in d:  # pragma: no branch (safety)
                         d[v] = v
                     rd[v] = k
                     if k not in rd:  # pragma: no branch (safety)
                         rd[k] = k
             cls._initialized = True
         self._parent = parent
+        self._context = context
 
     def __delitem__(self, key):
         raise TypeError("Configuration options can't be deleted.")
 
     def __getitem__(self, key):
         key = key.lower()
         if key not in self._options:
             raise KeyError(key)
         key_obj, ctype = self._options[key]
         is_bool = ctype == "bool"
+        if is_context := (key in self._context_keys):
+            get_function_base = self._context_get_function
+        else:
+            get_function_base = self._get_function
         if ctype in self._int32_ctypes:
             ctype = "int32_t"
-            get_function_name = f"{self._get_function}_INT32"
+            get_function_name = f"{get_function_base}_INT32"
         elif ctype.startswith("int64_t"):
-            get_function_name = f"{self._get_function}_INT64"
+            get_function_name = f"{get_function_base}_INT64"
         elif ctype.startswith("double"):
-            get_function_name = f"{self._get_function}_FP64"
+            get_function_name = f"{get_function_base}_FP64"
+        elif ctype.startswith("char"):
+            get_function_name = f"{get_function_base}_CHAR"
         else:  # pragma: no cover (sanity)
             raise ValueError(ctype)
         get_function = getattr(lib, get_function_name)
         is_array = "[" in ctype
         val_ptr = ffi.new(ctype if is_array else f"{ctype}*")
-        if self._parent is None:
+        if is_context:
+            info = get_function(self._context._carg, key_obj, val_ptr)
+        elif self._parent is None:
             info = get_function(key_obj, val_ptr)
         else:
             info = get_function(self._parent._carg, key_obj, val_ptr)
         if info == lib.GrB_SUCCESS:  # pragma: no branch (safety)
             if is_array:
                 return list(val_ptr)
             if key in self._reverse_enumerations:
@@ -89,33 +101,41 @@
                 rv = set()
                 for k, v in self._bitwise[key].items():
                     if isinstance(k, str) and val & v and bin(v).count("1") == 1:
                         rv.add(k)
                 return rv
             if is_bool:
                 return bool(val_ptr[0])
+            if ctype.startswith("char"):
+                return ffi.string(val_ptr[0]).decode()
             return val_ptr[0]
         raise _error_code_lookup[info](f"Failed to get info for {key!r}")  # pragma: no cover
 
     def __setitem__(self, key, val):
         key = key.lower()
         if key not in self._options:
             raise KeyError(key)
         if key in self._read_only:
             raise ValueError(f"Config option {key!r} is read-only")
         key_obj, ctype = self._options[key]
+        if is_context := (key in self._context_keys):
+            set_function_base = self._context_set_function
+        else:
+            set_function_base = self._set_function
         if ctype in self._int32_ctypes:
             ctype = "int32_t"
-            set_function_name = f"{self._set_function}_INT32"
+            set_function_name = f"{set_function_base}_INT32"
         elif ctype == "double":
-            set_function_name = f"{self._set_function}_FP64"
+            set_function_name = f"{set_function_base}_FP64"
         elif ctype.startswith("int64_t["):
-            set_function_name = f"{self._set_function}_INT64_ARRAY"
+            set_function_name = f"{set_function_base}_INT64_ARRAY"
         elif ctype.startswith("double["):
-            set_function_name = f"{self._set_function}_FP64_ARRAY"
+            set_function_name = f"{set_function_base}_FP64_ARRAY"
+        elif ctype.startswith("char"):
+            set_function_name = f"{set_function_base}_CHAR"
         else:  # pragma: no cover (sanity)
             raise ValueError(ctype)
         set_function = getattr(lib, set_function_name)
         if val is None:
             pass
         elif key in self._enumerations:
             if isinstance(val, str):
@@ -150,17 +170,27 @@
             vals, dtype = values_to_numpy_buffer(val, dtype.np_type)
             if int(size) != vals.size:
                 raise ValueError(
                     f"Wrong number of elements when setting {key!r} config.  "
                     f"expected {size}, got {vals.size}: {val}"
                 )
             val_obj = ffi.from_buffer(ctype, vals)
+        elif ctype.startswith("char"):
+            val_obj = ffi.new("char[]", val.encode())
         else:
             val_obj = ffi.cast(ctype, val)
-        if self._parent is None:
+        if is_context:
+            if self._context is None:
+                from .context import Context
+
+                self._context = Context(engage=False)
+                self._context._engage()  # Disengage when context goes out of scope
+                self._parent._context = self._context  # Set context to descriptor
+            info = set_function(self._context._carg, key_obj, val_obj)
+        elif self._parent is None:
             info = set_function(key_obj, val_obj)
         else:
             info = set_function(self._parent._carg, key_obj, val_obj)
         if info != lib.GrB_SUCCESS:
             if self._parent is not None:  # pragma: no branch (safety)
                 check_status(info, self._parent)
             raise _error_code_lookup[info](  # pragma: no cover (safety)
@@ -170,11 +200,16 @@
     def __iter__(self):
         return iter(sorted(self._options))
 
     def __len__(self):
         return len(self._options)
 
     def __repr__(self):
-        return "{" + ",\n ".join(f"{k!r}: {v!r}" for k, v in self.items()) + "}"
+        return (
+            type(self).__name__
+            + "({"
+            + ",\n ".join(f"{k!r}: {v!r}" for k, v in self.items())
+            + "})"
+        )
 
     def _ipython_key_completions_(self):  # pragma: no cover (ipython)
         return list(self)
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/ss/descriptor.py` & `python-graphblas-2023.7.0/graphblas/core/ss/descriptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ...exceptions import check_status, check_status_carg
 from .. import ffi, lib
 from ..descriptor import Descriptor
+from . import _IS_SSGB7
 from .config import BaseConfig
 
 ffi_new = ffi.new
 
 _str_to_compression = {
     "none": lib.GxB_COMPRESSION_NONE,
     "default": lib.GxB_COMPRESSION_DEFAULT,
@@ -14,29 +15,43 @@
 }
 
 
 # It would be great if we could make Descriptor class more like this
 class _DescriptorConfig(BaseConfig):
     _get_function = "GxB_Desc_get"
     _set_function = "GxB_Desc_set"
+    if not _IS_SSGB7:
+        _context_keys = {"chunk", "gpu_id", "nthreads"}
     _options = {
         # GrB
         "output_replace": (lib.GrB_OUTP, "GrB_Desc_Value"),
         "mask_complement": (lib.GrB_MASK, "GrB_Desc_Value"),
         "mask_structure": (lib.GrB_MASK, "GrB_Desc_Value"),
         "transpose_first": (lib.GrB_INP0, "GrB_Desc_Value"),
         "transpose_second": (lib.GrB_INP1, "GrB_Desc_Value"),
         # GxB
-        "nthreads": (lib.GxB_DESCRIPTOR_NTHREADS, "int"),
-        "chunk": (lib.GxB_DESCRIPTOR_CHUNK, "double"),
         "axb_method": (lib.GxB_AxB_METHOD, "GrB_Desc_Value"),
         "sort": (lib.GxB_SORT, "int"),
         "secure_import": (lib.GxB_IMPORT, "int"),
-        # "gpu_control": (GxB_DESCRIPTOR_GPU_CONTROL, "GrB_Desc_Value"),  # Coming soon...
     }
+    if _IS_SSGB7:
+        _options.update(
+            {
+                "nthreads": (lib.GxB_DESCRIPTOR_NTHREADS, "int"),
+                "chunk": (lib.GxB_DESCRIPTOR_CHUNK, "double"),
+            }
+        )
+    else:
+        _options.update(
+            {
+                "chunk": (lib.GxB_CONTEXT_CHUNK, "double"),
+                "gpu_id": (lib.GxB_CONTEXT_GPU_ID, "int"),
+                "nthreads": (lib.GxB_CONTEXT_NTHREADS, "int"),
+            }
+        )
     _enumerations = {
         # GrB
         "output_replace": {
             True: lib.GrB_REPLACE,
             False: False,
         },
         "mask_complement": {
@@ -67,18 +82,14 @@
             True: lib.GxB_SECURE_IMPORT,
             False: False,
         },
         "sort": {
             False: False,
             True: lib.GxB_SORT,
         },
-        # "gpu_control": {  # Coming soon...
-        #     "always": lib.GxB_GPU_ALWAYS,
-        #     "never": lib.GxB_GPU_NEVER,
-        # },
     }
     _defaults = {
         # GrB
         "output_replace": False,
         "mask_complement": False,
         "mask_structure": False,
         "transpose_first": False,
@@ -86,15 +97,16 @@
         # GxB
         "nthreads": 0,
         "chunk": 0,
         "axb_method": "default",
         "sort": False,
         "secure_import": False,
     }
-    _count = 0
+    if not _IS_SSGB7:
+        _defaults["gpu_id"] = -1
 
     def __init__(self):
         gb_obj = ffi_new("GrB_Descriptor*")
         check_status_carg(lib.GrB_Descriptor_new(gb_obj), "Descriptor", gb_obj[0])
         parent = Descriptor(gb_obj)
         initialized = self._initialized
         super().__init__(parent)
@@ -128,15 +140,15 @@
         If not set, use nthreads from global config ``gb.ss.config["nthreads"]``
     chunk : double
     axb_method : str, {"gustavson", "dot", "hash", "saxpy", "default"}
         A hint for which matrix multiply method to use
     sort : bool, default False
         A hint for whether methods may return a "jumbled" matrix
     secure_import : bool, default False
-        Whether to trust the data for `import` and `pack` functions.
+        Whether to trust the data for ``import`` and ``pack`` functions.
         When True, checks are performed to ensure input data is valid.
     compression : str, {"none", "default", "lz4", "lz4hc", "zstd"}
         Whether and how to compress the data for serialization.
         The default is "zstd" with ``compression_level=1``
     compression_level : int
         1-9 for "lz4hc" compression: (1) is the fastest, (9) is the most compact (default 1).
         1-19 for "zstd" compression: (1) is the fastest, (19) is the most compact (default 1).
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/ss/matrix.py` & `python-graphblas-2023.7.0/graphblas/core/ss/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 import numpy as np
 from suitesparse_graphblas.utils import claim_buffer, claim_buffer_2d, unclaim_buffer
 
 import graphblas as gb
 
 from ... import binary, monoid
-from ...dtypes import _INDEX, BOOL, INT64, UINT64, _string_to_dtype, lookup_dtype
+from ...dtypes import _INDEX, BOOL, INT64, UINT64, lookup_dtype
 from ...exceptions import _error_code_lookup, check_status, check_status_carg
 from .. import NULL, _has_numba, ffi, lib
 from ..base import call
+from ..dtypes import _string_to_dtype
 from ..operator import get_typed_op
 from ..scalar import Scalar, _as_scalar, _scalar_index
 from ..utils import (
     _CArray,
     _MatrixArray,
     _Pointer,
     get_order,
@@ -59,15 +60,15 @@
     else:
         dtype = lookup_dtype(dtype)
     rows, cols, vals = zip(*itertools.islice(matrix.ss.iteritems(), n))
     return np.array(rows, np.uint64), np.array(cols, np.uint64), np.array(vals, dtype.np_type)
 
 
 def _concat_mn(tiles, *, is_matrix=None):
-    """Argument checking for `Matrix.ss.concat` and returns number of tiles in each dimension."""
+    """Argument checking for ``Matrix.ss.concat`` and returns number of tiles in each dimension."""
     from ..matrix import Matrix, TransposedMatrix
     from ..vector import Vector
 
     valid_types = (Matrix, TransposedMatrix, Vector, Scalar)
     if not isinstance(tiles, (list, tuple)):
         raise TypeError(f"tiles argument must be list or tuple; got: {type(tiles)}")
     if not tiles:
@@ -257,16 +258,16 @@
         Existing entries in the Matrix are discarded.
 
         Parameters
         ----------
         vector : Vector
             Create a diagonal from this Vector.
         k : int, default 0
-            Diagonal in question.  Use `k>0` for diagonals above the main diagonal,
-            and `k<0` for diagonals below the main diagonal.
+            Diagonal in question.  Use ``k>0`` for diagonals above the main diagonal,
+            and ``k<0`` for diagonals below the main diagonal.
 
         See Also
         --------
         Matrix.diag
         Vector.diag
 
         """
@@ -278,28 +279,28 @@
             [self._parent, vector, _as_scalar(k, INT64, is_cscalar=True), get_descriptor(**opts)],
         )
 
     def split(self, chunks, *, name=None, **opts):
         """
         GxB_Matrix_split.
 
-        Split a Matrix into a 2D array of sub-matrices according to `chunks`.
+        Split a Matrix into a 2D array of sub-matrices according to ``chunks``.
 
         This performs the opposite operation as ``concat``.
 
-        `chunks` is short for "chunksizes" and indicates the chunk sizes for each dimension.
-        `chunks` may be a single integer, or a length 2 tuple or list.  Example chunks:
+        ``chunks`` is short for "chunksizes" and indicates the chunk sizes for each dimension.
+        ``chunks`` may be a single integer, or a length 2 tuple or list.  Example chunks:
 
         - ``chunks=10``
             - Split each dimension into chunks of size 10 (the last chunk may be smaller).
         - ``chunks=(10, 20)``
             - Split rows into chunks of size 10 and columns into chunks of size 20.
         - ``chunks=(None, [5, 10])``
             - Don't split rows into chunks, and split columns into two chunks of size 5 and 10.
-        ` ``chunks=(10, [20, None])``
+        - ``chunks=(10, [20, None])``
             - Split columns into two chunks of size 20 and ``ncols - 20``
 
         See Also
         --------
         Matrix.ss.concat
         graphblas.ss.concat
         """
@@ -362,17 +363,17 @@
 
     def concat(self, tiles, **opts):
         """
         GxB_Matrix_concat.
 
         Concatenate a 2D list of Matrix objects into the current Matrix.
         Any existing values in the current Matrix will be discarded.
-        To concatenate into a new Matrix, use `graphblas.ss.concat`.
+        To concatenate into a new Matrix, use ``graphblas.ss.concat``.
 
-        Vectors may be used as `Nx1` Matrix objects.
+        Vectors may be used as ``Nx1`` Matrix objects.
 
         This performs the opposite operation as ``split``.
 
         See Also
         --------
         Matrix.ss.split
         graphblas.ss.concat
@@ -538,16 +539,16 @@
     def export(self, format=None, *, sort=False, give_ownership=False, raw=False, **opts):
         """
         GxB_Matrix_export_xxx.
 
         Parameters
         ----------
         format : str, optional
-            If `format` is not specified, this method exports in the currently stored format.
-            To control the export format, set `format` to one of:
+            If ``format`` is not specified, this method exports in the currently stored format.
+            To control the export format, set ``format`` to one of:
                 - "csr"
                 - "csc"
                 - "hypercsr"
                 - "hypercsc"
                 - "bitmapr"
                 - "bitmapc"
                 - "fullr"
@@ -574,15 +575,15 @@
             If False, arrays may be trimmed to be the expected size, and 2d arrays are
             returned when format is "bitmapr", "bitmapc", "fullr", or "fullc".
             It may make sense to choose ``raw=True`` if one wants to use the data to perform
             a zero-copy import back to SuiteSparse.
 
         Returns
         -------
-        dict; keys depend on `format` and `raw` arguments (see below).
+        dict; keys depend on ``format`` and ``raw`` arguments (see below).
 
         See Also
         --------
         Matrix.to_coo
         Matrix.ss.import_any
 
         Return values
@@ -728,18 +729,18 @@
             opts=opts,
         )
 
     def unpack(self, format=None, *, sort=False, raw=False, **opts):
         """
         GxB_Matrix_unpack_xxx.
 
-        `unpack` is like `export`, except that the Matrix remains valid but empty.
-        `pack_*` methods are the opposite of `unpack`.
+        ``unpack`` is like ``export``, except that the Matrix remains valid but empty.
+        ``pack_*`` methods are the opposite of ``unpack``.
 
-        See `Matrix.ss.export` documentation for more details.
+        See ``Matrix.ss.export`` documentation for more details.
         """
         return self._export(
             format, sort=sort, raw=raw, give_ownership=True, method="unpack", opts=opts
         )
 
     def _export(self, format=None, *, sort=False, give_ownership=False, raw=False, method, opts):
         if format is None:
@@ -1189,15 +1190,15 @@
         nrows : int
         ncols : int
         indptr : array-like
         values : array-like
         col_indices : array-like
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_cols : bool, default False
             Indicate whether the values in "col_indices" are sorted.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
@@ -1206,15 +1207,15 @@
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "csr" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -1255,18 +1256,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_CSR.
 
-        `pack_csr` is like `import_csr` except it "packs" data into an
+        ``pack_csr`` is like ``import_csr`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("csr")``
 
-        See `Matrix.ss.import_csr` documentation for more details.
+        See ``Matrix.ss.import_csr`` documentation for more details.
         """
         return self._import_csr(
             indptr=indptr,
             values=values,
             col_indices=col_indices,
             is_iso=is_iso,
             sorted_cols=sorted_cols,
@@ -1379,15 +1380,15 @@
         nrows : int
         ncols : int
         indptr : array-like
         values : array-like
         row_indices : array-like
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_rows : bool, default False
             Indicate whether the values in "row_indices" are sorted.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
@@ -1396,15 +1397,15 @@
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "csc" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -1445,18 +1446,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_CSC.
 
-        `pack_csc` is like `import_csc` except it "packs" data into an
+        ``pack_csc`` is like ``import_csc`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("csc")``
 
-        See `Matrix.ss.import_csc` documentation for more details.
+        See ``Matrix.ss.import_csc`` documentation for more details.
         """
         return self._import_csc(
             indptr=indptr,
             values=values,
             row_indices=row_indices,
             is_iso=is_iso,
             sorted_rows=sorted_rows,
@@ -1575,15 +1576,15 @@
         values : array-like
         col_indices : array-like
         nvec : int, optional
             The number of elements in "rows" to use.
             If not specified, will be set to ``len(rows)``.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_cols : bool, default False
             Indicate whether the values in "col_indices" are sorted.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
@@ -1592,15 +1593,15 @@
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "hypercsr" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -1645,18 +1646,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_HyperCSR.
 
-        `pack_hypercsr` is like `import_hypercsr` except it "packs" data into an
+        ``pack_hypercsr`` is like ``import_hypercsr`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("hypercsr")``
 
-        See `Matrix.ss.import_hypercsr` documentation for more details.
+        See ``Matrix.ss.import_hypercsr`` documentation for more details.
         """
         return self._import_hypercsr(
             rows=rows,
             indptr=indptr,
             values=values,
             col_indices=col_indices,
             nvec=nvec,
@@ -1799,15 +1800,15 @@
         values : array-like
         row_indices : array-like
         nvec : int, optional
             The number of elements in "cols" to use.
             If not specified, will be set to ``len(cols)``.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_rows : bool, default False
             Indicate whether the values in "row_indices" are sorted.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
@@ -1816,15 +1817,15 @@
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "hypercsc" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -1869,18 +1870,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_HyperCSC.
 
-        `pack_hypercsc` is like `import_hypercsc` except it "packs" data into an
+        ``pack_hypercsc`` is like ``import_hypercsc`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("hypercsc")``
 
-        See `Matrix.ss.import_hypercsc` documentation for more details.
+        See ``Matrix.ss.import_hypercsc`` documentation for more details.
         """
         return self._import_hypercsc(
             cols=cols,
             indptr=indptr,
             values=values,
             row_indices=row_indices,
             nvec=nvec,
@@ -2024,30 +2025,30 @@
             The number of rows for the Matrix.
             If not provided, will be inferred from values or bitmap if either is 2d.
         ncols : int
             The number of columns for the Matrix.
             If not provided, will be inferred from values or bitmap if either is 2d.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
                 - have the correct dtype (bool for bitmap)
                 - own its own data
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "bitmapr" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -2086,18 +2087,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_BitmapR.
 
-        `pack_bitmapr` is like `import_bitmapr` except it "packs" data into an
+        ``pack_bitmapr`` is like ``import_bitmapr`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("bitmapr")``
 
-        See `Matrix.ss.import_bitmapr` documentation for more details.
+        See ``Matrix.ss.import_bitmapr`` documentation for more details.
         """
         return self._import_bitmapr(
             bitmap=bitmap,
             values=values,
             nvals=nvals,
             is_iso=is_iso,
             take_ownership=take_ownership,
@@ -2217,30 +2218,30 @@
             The number of rows for the Matrix.
             If not provided, will be inferred from values or bitmap if either is 2d.
         ncols : int
             The number of columns for the Matrix.
             If not provided, will be inferred from values or bitmap if either is 2d.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be FORTRAN contiguous
                 - have the correct dtype (bool for bitmap)
                 - own its own data
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "bitmapc" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -2279,18 +2280,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_BitmapC.
 
-        `pack_bitmapc` is like `import_bitmapc` except it "packs" data into an
+        ``pack_bitmapc`` is like ``import_bitmapc`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("bitmapc")``
 
-        See `Matrix.ss.import_bitmapc` documentation for more details.
+        See ``Matrix.ss.import_bitmapc`` documentation for more details.
         """
         return self._import_bitmapc(
             bitmap=bitmap,
             values=values,
             nvals=nvals,
             is_iso=is_iso,
             take_ownership=take_ownership,
@@ -2403,30 +2404,30 @@
             The number of rows for the Matrix.
             If not provided, will be inferred from values if it is 2d.
         ncols : int
             The number of columns for the Matrix.
             If not provided, will be inferred from values if it is 2d.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
                 - have the correct dtype
                 - own its own data
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "fullr" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -2461,18 +2462,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_FullR.
 
-        `pack_fullr` is like `import_fullr` except it "packs" data into an
+        ``pack_fullr`` is like ``import_fullr`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("fullr")``
 
-        See `Matrix.ss.import_fullr` documentation for more details.
+        See ``Matrix.ss.import_fullr`` documentation for more details.
         """
         return self._import_fullr(
             values=values,
             is_iso=is_iso,
             take_ownership=take_ownership,
             secure_import=secure_import,
             format=format,
@@ -2562,30 +2563,30 @@
             The number of rows for the Matrix.
             If not provided, will be inferred from values if it is 2d.
         ncols : int
             The number of columns for the Matrix.
             If not provided, will be inferred from values if it is 2d.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be FORTRAN contiguous
                 - have the correct dtype
                 - own its own data
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "fullc" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -2620,18 +2621,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_FullC.
 
-        `pack_fullc` is like `import_fullc` except it "packs" data into an
+        ``pack_fullc`` is like ``import_fullc`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("fullc")``
 
-        See `Matrix.ss.import_fullc` documentation for more details.
+        See ``Matrix.ss.import_fullc`` documentation for more details.
         """
         return self._import_fullc(
             values=values,
             is_iso=is_iso,
             take_ownership=take_ownership,
             secure_import=secure_import,
             format=format,
@@ -2723,24 +2724,24 @@
         values : array-like
         nrows : int
             The number of rows for the Matrix.
         ncols : int
             The number of columns for the Matrix.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_rows : bool, default False
             True if rows are sorted or when (cols, rows) are sorted lexicographically
         sorted_cols : bool, default False
             True if cols are sorted or when (rows, cols) are sorted lexicographically
         take_ownership : bool, default False
             Ignored.  Zero-copy is not possible for "coo" format.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "coo" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -2783,18 +2784,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GrB_Matrix_build_XXX and GxB_Matrix_build_Scalar.
 
-        `pack_coo` is like `import_coo` except it "packs" data into an
+        ``pack_coo`` is like ``import_coo`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("coo")``
 
-        See `Matrix.ss.import_coo` documentation for more details.
+        See ``Matrix.ss.import_coo`` documentation for more details.
         """
         return self._import_coo(
             nrows=self._parent._nrows,
             ncols=self._parent._ncols,
             rows=rows,
             cols=cols,
             values=values,
@@ -2910,15 +2911,15 @@
         values : array-like
         nrows : int
             The number of rows for the Matrix.
         ncols : int
             The number of columns for the Matrix.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_cols : bool, default False
             True indicates indices are sorted by column, then row.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
@@ -2928,15 +2929,15 @@
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
             For "coor", ownership of "rows" will never change.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "coor" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -2979,18 +2980,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_CSR.
 
-        `pack_coor` is like `import_coor` except it "packs" data into an
+        ``pack_coor`` is like ``import_coor`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("coor")``
 
-        See `Matrix.ss.import_coor` documentation for more details.
+        See ``Matrix.ss.import_coor`` documentation for more details.
         """
         return self._import_coor(
             rows=rows,
             cols=cols,
             nrows=self._parent._nrows,
             values=values,
             is_iso=is_iso,
@@ -3079,15 +3080,15 @@
         values : array-like
         nrows : int
             The number of rows for the Matrix.
         ncols : int
             The number of columns for the Matrix.
         is_iso : bool, default False
             Is the Matrix iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_rows : bool, default False
             True indicates indices are sorted by column, then row.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
@@ -3097,15 +3098,15 @@
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
             For "cooc", ownership of "cols" will never change.
         dtype : dtype, optional
             dtype of the new Matrix.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "cooc" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Matrix.
 
         Returns
@@ -3148,18 +3149,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_CSC.
 
-        `pack_cooc` is like `import_cooc` except it "packs" data into an
+        ``pack_cooc`` is like ``import_cooc`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack("cooc")``
 
-        See `Matrix.ss.import_cooc` documentation for more details.
+        See ``Matrix.ss.import_cooc`` documentation for more details.
         """
         return self._import_cooc(
             ncols=self._parent._ncols,
             rows=rows,
             cols=cols,
             values=values,
             is_iso=is_iso,
@@ -3251,15 +3252,15 @@
         nvals=None,  # optional
         **opts,
     ):
         """
         GxB_Matrix_import_xxx.
 
         Dispatch to appropriate import method inferred from inputs.
-        See the other import functions and `Matrix.ss.export`` for details.
+        See the other import functions and ``Matrix.ss.export`` for details.
 
         Returns
         -------
         Matrix
 
         See Also
         --------
@@ -3348,18 +3349,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Matrix_pack_xxx.
 
-        `pack_any` is like `import_any` except it "packs" data into an
+        ``pack_any`` is like ``import_any`` except it "packs" data into an
         existing Matrix.  This is the opposite of ``unpack()``
 
-        See `Matrix.ss.import_any` documentation for more details.
+        See ``Matrix.ss.import_any`` documentation for more details.
         """
         return self._import_any(
             values=values,
             is_iso=is_iso,
             take_ownership=take_ownership,
             secure_import=secure_import,
             format=format,
@@ -3697,16 +3698,16 @@
     @wrapdoc(head)
     def head(self, n=10, dtype=None, *, sort=False):
         return head(self._parent, n, dtype, sort=sort)
 
     def scan(self, op=monoid.plus, order="rowwise", *, name=None, **opts):
         """Perform a prefix scan across rows (default) or columns with the given monoid.
 
-        For example, use `monoid.plus` (the default) to perform a cumulative sum,
-        and `monoid.times` for cumulative product.  Works with any monoid.
+        For example, use ``monoid.plus`` (the default) to perform a cumulative sum,
+        and ``monoid.times`` for cumulative product.  Works with any monoid.
 
         Returns
         -------
         Matrix
         """
         order = get_order(order)
         parent = self._parent
@@ -3714,20 +3715,20 @@
             parent = parent.T
         return prefix_scan(parent, op, name=name, within="scan", **opts)
 
     def scan_columnwise(self, op=monoid.plus, *, name=None, **opts):
         """Perform a prefix scan across columns with the given monoid.
 
         .. deprecated:: 2022.11.1
-            `Matrix.ss.scan_columnwise` will be removed in a future release.
-            Use `Matrix.ss.scan(order="columnwise")` instead.
+            ``Matrix.ss.scan_columnwise`` will be removed in a future release.
+            Use ``Matrix.ss.scan(order="columnwise")`` instead.
             Will be removed in version 2023.7.0 or later
 
-        For example, use `monoid.plus` (the default) to perform a cumulative sum,
-        and `monoid.times` for cumulative product.  Works with any monoid.
+        For example, use ``monoid.plus`` (the default) to perform a cumulative sum,
+        and ``monoid.times`` for cumulative product.  Works with any monoid.
 
         Returns
         -------
         Matrix
         """
         warnings.warn(
             "`Matrix.ss.scan_columnwise` is deprecated; "
@@ -3737,20 +3738,20 @@
         )
         return prefix_scan(self._parent.T, op, name=name, within="scan_columnwise", **opts)
 
     def scan_rowwise(self, op=monoid.plus, *, name=None, **opts):
         """Perform a prefix scan across rows with the given monoid.
 
         .. deprecated:: 2022.11.1
-            `Matrix.ss.scan_rowwise` will be removed in a future release.
-            Use `Matrix.ss.scan` instead.
+            ``Matrix.ss.scan_rowwise`` will be removed in a future release.
+            Use ``Matrix.ss.scan`` instead.
             Will be removed in version 2023.7.0 or later
 
-        For example, use `monoid.plus` (the default) to perform a cumulative sum,
-        and `monoid.times` for cumulative product.  Works with any monoid.
+        For example, use ``monoid.plus`` (the default) to perform a cumulative sum,
+        and ``monoid.times`` for cumulative product.  Works with any monoid.
 
         Returns
         -------
         Matrix
         """
         warnings.warn(
             "`Matrix.ss.scan_rowwise` is deprecated; please use `Matrix.ss.scan` instead.",
@@ -3900,16 +3901,16 @@
             k, fmt, indices, sort_axis, choose_func, is_random, do_sort, name
         )
 
     def selectk_rowwise(self, how, k, *, name=None):  # pragma: no cover (deprecated)
         """Select (up to) k elements from each row.
 
         .. deprecated:: 2022.11.1
-            `Matrix.ss.selectk_rowwise` will be removed in a future release.
-            Use `Matrix.ss.selectk` instead.
+            ``Matrix.ss.selectk_rowwise`` will be removed in a future release.
+            Use ``Matrix.ss.selectk`` instead.
             Will be removed in version 2023.7.0 or later
 
         Parameters
         ----------
         how : str
             "random": choose k elements with equal probability
             "first": choose the first k elements
@@ -3946,16 +3947,16 @@
             k, fmt, indices, sort_axis, choose_func, is_random, do_sort, name
         )
 
     def selectk_columnwise(self, how, k, *, name=None):  # pragma: no cover (deprecated)
         """Select (up to) k elements from each column.
 
         .. deprecated:: 2022.11.1
-            `Matrix.ss.selectk_columnwise` will be removed in a future release.
-            Use `Matrix.ss.selectk(order="columnwise")` instead.
+            ``Matrix.ss.selectk_columnwise`` will be removed in a future release.
+            Use ``Matrix.ss.selectk(order="columnwise")`` instead.
             Will be removed in version 2023.7.0 or later
 
         Parameters
         ----------
         how : str
             - "random": choose elements with equal probability
             - "first": choose the first k elements
@@ -4212,31 +4213,31 @@
             name=name,
         )
 
     def sort(self, op=binary.lt, order="rowwise", *, values=True, permutation=True, **opts):
         """GxB_Matrix_sort to sort values along the rows (default) or columns of the Matrix.
 
         Sorting moves all the elements to the left (if rowwise) or top (if columnwise) just
-        like `compactify`. The returned matrices will be the same shape as the input Matrix.
+        like ``compactify``. The returned matrices will be the same shape as the input Matrix.
 
         Parameters
         ----------
         op : :class:`~graphblas.core.operator.BinaryOp`, optional
             Binary operator with a bool return type used to sort the values.
-            For example, `binary.lt` (the default) sorts the smallest elements first.
+            For example, ``binary.lt`` (the default) sorts the smallest elements first.
             Ties are broken according to indices (smaller first).
         order : {"rowwise", "columnwise"}, optional
             Whether to sort rowwise or columnwise. Rowwise shifts all values to the left,
             and columnwise shifts all values to the top. The default is "rowwise".
         values : bool, default=True
-            Whether to return values; will return `None` for values if `False`.
+            Whether to return values; will return ``None`` for values if ``False``.
         permutation : bool, default=True
             Whether to compute the permutation Matrix that has the original column
             indices (if rowwise) or row indices (if columnwise) of the sorted values.
-            Will return None if `False`.
+            Will return None if ``False``.
         nthreads : int, optional
             The maximum number of threads to use for this operation.
             None, 0 or negative nthreads means to use the default number of threads.
 
         Returns
         -------
         Matrix : Values
@@ -4297,15 +4298,15 @@
             Level 1 is the fastest and largest, and is the default for "zstd" compression.
             Level 9 is the default when using "lz4hc" compression.
         nthreads : int, optional
             The maximum number of threads to use when serializing the Matrix.
             None, 0 or negative nthreads means to use the default number of threads.
 
         For best performance, this function returns a numpy array with uint8 dtype.
-        Use `Matrix.ss.deserialize(blob)` to create a Matrix from the result of serialization
+        Use ``Matrix.ss.deserialize(blob)`` to create a Matrix from the result of serialization
 
         This method is intended to support all serialization options from SuiteSparse:GraphBLAS.
 
         *Warning*: Behavior of serializing UDTs is experimental and may change in a future release.
         """
         desc = get_descriptor(compression=compression, compression_level=level, **opts)
         blob_handle = ffi_new("void**")
@@ -4323,15 +4324,15 @@
         return claim_buffer(ffi, blob_handle[0], blob_size_handle[0], np.dtype(np.uint8))
 
     @classmethod
     def deserialize(cls, data, dtype=None, *, name=None, **opts):
         """Deserialize a Matrix from bytes, buffer, or numpy array using GxB_Matrix_deserialize.
 
         The data should have been previously serialized with a compatible version of
-        SuiteSparse:GraphBLAS.  For example, from the result of `data = matrix.ss.serialize()`.
+        SuiteSparse:GraphBLAS.  For example, from the result of ``data = matrix.ss.serialize()``.
 
         Examples
         --------
         >>> data = matrix.serialize()
         >>> new_matrix = Matrix.ss.deserialize(data)
         >>> new_matrix.isequal(matrix)
         True
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/ss/prefix_scan.py` & `python-graphblas-2023.7.0/graphblas/core/ss/prefix_scan.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/core/ss/vector.py` & `python-graphblas-2023.7.0/graphblas/core/ss/vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 import numpy as np
 from suitesparse_graphblas.utils import claim_buffer, unclaim_buffer
 
 import graphblas as gb
 
 from ... import binary, monoid
-from ...dtypes import _INDEX, INT64, UINT64, _string_to_dtype, lookup_dtype
+from ...dtypes import _INDEX, INT64, UINT64, lookup_dtype
 from ...exceptions import _error_code_lookup, check_status, check_status_carg
 from .. import NULL, ffi, lib
 from ..base import call
+from ..dtypes import _string_to_dtype
 from ..operator import get_typed_op
 from ..scalar import Scalar, _as_scalar
 from ..utils import (
     _CArray,
     _MatrixArray,
     ints_to_numpy_buffer,
     normalize_chunks,
@@ -151,16 +152,16 @@
         Existing entries in the Vector are discarded.
 
         Parameters
         ----------
         matrix : Matrix or TransposedMatrix
             Extract a diagonal from this matrix.
         k : int, default 0
-            Diagonal in question.  Use `k>0` for diagonals above the main diagonal,
-            and `k<0` for diagonals below the main diagonal.
+            Diagonal in question.  Use ``k>0`` for diagonals above the main diagonal,
+            and ``k<0`` for diagonals below the main diagonal.
 
         See Also
         --------
         Matrix.diag
         Vector.diag
 
         """
@@ -181,20 +182,20 @@
             [self._parent, matrix, _as_scalar(k, INT64, is_cscalar=True), get_descriptor(**opts)],
         )
 
     def split(self, chunks, *, name=None, **opts):
         """
         GxB_Matrix_split.
 
-        Split a Vector into a 1D array of sub-vectors according to `chunks`.
+        Split a Vector into a 1D array of sub-vectors according to ``chunks``.
 
         This performs the opposite operation as ``concat``.
 
-        `chunks` is short for "chunksizes" and indicates the chunk sizes.
-        `chunks` may be a single integer, or a tuple or list.  Example chunks:
+        ``chunks`` is short for "chunksizes" and indicates the chunk sizes.
+        ``chunks`` may be a single integer, or a tuple or list.  Example chunks:
 
         - ``chunks=10``
             - Split vector into chunks of size 10 (the last chunk may be smaller).
         - ``chunks=[5, 10]``
             - Split vector into two chunks of size 5 and 10.
 
         See Also
@@ -249,15 +250,15 @@
 
     def concat(self, tiles, **opts):
         """
         GxB_Matrix_concat.
 
         Concatenate a 1D list of Vector objects into the current Vector.
         Any existing values in the current Vector will be discarded.
-        To concatenate into a new Vector, use `graphblas.ss.concat`.
+        To concatenate into a new Vector, use ``graphblas.ss.concat``.
 
         This performs the opposite operation as ``split``.
 
         See Also
         --------
         Vector.ss.split
         graphblas.ss.concat
@@ -411,16 +412,16 @@
     def export(self, format=None, *, sort=False, give_ownership=False, raw=False, **opts):
         """
         GxB_Vextor_export_xxx.
 
         Parameters
         ----------
         format : str or None, default None
-            If `format` is not specified, this method exports in the currently stored format.
-            To control the export format, set `format` to one of:
+            If ``format`` is not specified, this method exports in the currently stored format.
+            To control the export format, set ``format`` to one of:
                 - "sparse"
                 - "bitmap"
                 - "full"
         sort : bool, default False
             Whether to sort indices if the format is "sparse"
         give_ownership : bool, default False
             Perform a zero-copy data transfer to Python if possible.  This gives ownership of
@@ -430,23 +431,23 @@
             If True, always return array the same size as returned by SuiteSparse.
             If False, arrays may be trimmed to be the expected size.
             It may make sense to choose ``raw=True`` if one wants to use the data to perform
             a zero-copy import back to SuiteSparse.
 
         Returns
         -------
-        dict; keys depend on `format` and `raw` arguments (see below).
+        dict; keys depend on ``format`` and ``raw`` arguments (see below).
 
         See Also
         --------
         Vector.to_coo
         Vector.ss.import_any
 
         Return values
-            - Note: for `raw=True`, arrays may be larger than specified.
+            - Note: for ``raw=True``, arrays may be larger than specified.
             - "sparse" format
                 - indices : ndarray(dtype=uint64, size=nvals)
                 - values : ndarray(size=nvals)
                 - sorted_index : bool
                     - True if the values in "indices" are sorted
                 - size : int
                 - nvals : int, only present if raw == True
@@ -477,18 +478,18 @@
             opts=opts,
         )
 
     def unpack(self, format=None, *, sort=False, raw=False, **opts):
         """
         GxB_Vector_unpack_xxx.
 
-        `unpack` is like `export`, except that the Vector remains valid but empty.
-        `pack_*` methods are the opposite of `unpack`.
+        ``unpack`` is like ``export``, except that the Vector remains valid but empty.
+        ``pack_*`` methods are the opposite of ``unpack``.
 
-        See `Vector.ss.export` documentation for more details.
+        See ``Vector.ss.export`` documentation for more details.
         """
         return self._export(
             format=format, sort=sort, give_ownership=True, raw=raw, method="unpack", opts=opts
         )
 
     def _export(self, format=None, *, sort=False, give_ownership=False, raw=False, method, opts):
         if give_ownership:
@@ -654,15 +655,15 @@
         nvals=None,  # optional
         **opts,
     ):
         """
         GxB_Vector_import_xxx.
 
         Dispatch to appropriate import method inferred from inputs.
-        See the other import functions and `Vector.ss.export`` for details.
+        See the other import functions and ``Vector.ss.export`` for details.
 
         Returns
         -------
         Vector
 
         See Also
         --------
@@ -720,18 +721,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Vector_pack_xxx.
 
-        `pack_any` is like `import_any` except it "packs" data into an
+        ``pack_any`` is like ``import_any`` except it "packs" data into an
         existing Vector.  This is the opposite of ``unpack()``
 
-        See `Vector.ss.import_any` documentation for more details.
+        See ``Vector.ss.import_any`` documentation for more details.
         """
         return self._import_any(
             values=values,
             is_iso=is_iso,
             take_ownership=take_ownership,
             secure_import=secure_import,
             format=format,
@@ -854,15 +855,15 @@
         indices : array-like
         values : array-like
         nvals : int, optional
             The number of elements in "values" to use.
             If not specified, will be set to ``len(values)``.
         is_iso : bool, default False
             Is the Vector iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         sorted_index : bool, default False
             Indicate whether the values in "col_indices" are sorted.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
@@ -871,15 +872,15 @@
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Vector.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "sparse" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Vector.
 
         Returns
@@ -918,18 +919,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Vector_pack_CSC.
 
-        `pack_sparse` is like `import_sparse` except it "packs" data into an
+        ``pack_sparse`` is like ``import_sparse`` except it "packs" data into an
         existing Vector.  This is the opposite of ``unpack("sparse")``
 
-        See `Vector.ss.import_sparse` documentation for more details.
+        See ``Vector.ss.import_sparse`` documentation for more details.
         """
         return self._import_sparse(
             indices=indices,
             values=values,
             nvals=nvals,
             is_iso=is_iso,
             sorted_index=sorted_index,
@@ -1041,30 +1042,30 @@
         nvals : int, optional
             The number of True elements in the bitmap for this Vector.
         size : int, optional
             The size of the new Vector.
             If not specified, it will be set to the size of values.
         is_iso : bool, default False
             Is the Vector iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
                 - have the correct dtype (bool for bitmap)
                 - own its own data
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Vector.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "bitmap" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Vector.
 
         Returns
@@ -1101,18 +1102,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Vector_pack_Bitmap.
 
-        `pack_bitmap` is like `import_bitmap` except it "packs" data into an
+        ``pack_bitmap`` is like ``import_bitmap`` except it "packs" data into an
         existing Vector.  This is the opposite of ``unpack("bitmap")``
 
-        See `Vector.ss.import_bitmap` documentation for more details.
+        See ``Vector.ss.import_bitmap`` documentation for more details.
         """
         return self._import_bitmap(
             bitmap=bitmap,
             values=values,
             nvals=nvals,
             is_iso=is_iso,
             take_ownership=take_ownership,
@@ -1222,30 +1223,30 @@
         ----------
         values : array-like
         size : int, optional
             The size of the new Vector.
             If not specified, it will be set to the size of values.
         is_iso : bool, default False
             Is the Vector iso-valued (meaning all the same value)?
-            If true, then `values` should be a length 1 array.
+            If true, then ``values`` should be a length 1 array.
         take_ownership : bool, default False
             If True, perform a zero-copy data transfer from input numpy arrays
             to GraphBLAS if possible.  To give ownership of the underlying
             memory buffers to GraphBLAS, the arrays must:
                 - be C contiguous
                 - have the correct dtype (bool for bitmap)
                 - own its own data
                 - be writeable
             If all of these conditions are not met, then the data will be
             copied and the original array will be unmodified.  If zero copy
             to GraphBLAS is successful, then the array will be modified to be
             read-only and will no longer own the data.
         dtype : dtype, optional
             dtype of the new Vector.
-            If not specified, this will be inferred from `values`.
+            If not specified, this will be inferred from ``values``.
         format : str, optional
             Must be "full" or None.  This is included to be compatible with
             the dict returned from exporting.
         name : str, optional
             Name of the new Vector.
 
         Returns
@@ -1278,18 +1279,18 @@
         dtype=None,
         name=None,
         **opts,
     ):
         """
         GxB_Vector_pack_Full.
 
-        `pack_full` is like `import_full` except it "packs" data into an
+        ``pack_full`` is like ``import_full`` except it "packs" data into an
         existing Vector.  This is the opposite of ``unpack("full")``
 
-        See `Vector.ss.import_full` documentation for more details.
+        See ``Vector.ss.import_full`` documentation for more details.
         """
         return self._import_full(
             values=values,
             is_iso=is_iso,
             take_ownership=take_ownership,
             secure_import=secure_import,
             format=format,
@@ -1360,16 +1361,16 @@
     @wrapdoc(head)
     def head(self, n=10, dtype=None, *, sort=False):
         return head(self._parent, n, dtype, sort=sort)
 
     def scan(self, op=monoid.plus, *, name=None, **opts):
         """Perform a prefix scan with the given monoid.
 
-        For example, use `monoid.plus` (the default) to perform a cumulative sum,
-        and `monoid.times` for cumulative product.  Works with any monoid.
+        For example, use ``monoid.plus`` (the default) to perform a cumulative sum,
+        and ``monoid.times`` for cumulative product.  Works with any monoid.
 
         Returns
         -------
         Scalar
         """
         return prefix_scan(self._parent, op, name=name, within="scan", **opts)
 
@@ -1557,28 +1558,28 @@
             take_ownership=True,
             name=name,
         )
 
     def sort(self, op=binary.lt, *, values=True, permutation=True, **opts):
         """GxB_Vector_sort to sort values of the Vector.
 
-        Sorting moves all the elements to the left just like `compactify`.
+        Sorting moves all the elements to the left just like ``compactify``.
         The returned vectors will be the same size as the input Vector.
 
         Parameters
         ----------
         op : :class:`~graphblas.core.operator.BinaryOp`, optional
             Binary operator with a bool return type used to sort the values.
-            For example, `binary.lt` (the default) sorts the smallest elements first.
+            For example, ``binary.lt`` (the default) sorts the smallest elements first.
             Ties are broken according to indices (smaller first).
         values : bool, default=True
-            Whether to return values; will return `None` for values if `False`.
+            Whether to return values; will return ``None`` for values if ``False``.
         permutation : bool, default=True
             Whether to compute the permutation Vector that has the original indices of the
-            sorted values. Will return None if `False`.
+            sorted values. Will return None if ``False``.
         nthreads : int, optional
             The maximum number of threads to use for this operation.
             None, 0 or negative nthreads means to use the default number of threads.
 
         Returns
         -------
         Vector : values
@@ -1638,15 +1639,15 @@
             Level 1 is the fastest and largest, and is the default for "zstd" compression.
             Level 9 is the default when using "lz4hc" compression.
         nthreads : int, optional
             The maximum number of threads to use when serializing the Vector.
             None, 0 or negative nthreads means to use the default number of threads.
 
         For best performance, this function returns a numpy array with uint8 dtype.
-        Use `Vector.ss.deserialize(blob)` to create a Vector from the result of serialization·
+        Use ``Vector.ss.deserialize(blob)`` to create a Vector from the result of serialization·
 
         This method is intended to support all serialization options from SuiteSparse:GraphBLAS.
 
         *Warning*: Behavior of serializing UDTs is experimental and may change in a future release.
         """
         desc = get_descriptor(compression=compression, compression_level=level, **opts)
         blob_handle = ffi_new("void**")
@@ -1664,15 +1665,15 @@
         return claim_buffer(ffi, blob_handle[0], blob_size_handle[0], np.dtype(np.uint8))
 
     @classmethod
     def deserialize(cls, data, dtype=None, *, name=None, **opts):
         """Deserialize a Vector from bytes, buffer, or numpy array using GxB_Vector_deserialize.
 
         The data should have been previously serialized with a compatible version of
-        SuiteSparse:GraphBLAS.  For example, from the result of `data = vector.ss.serialize()`.
+        SuiteSparse:GraphBLAS.  For example, from the result of ``data = vector.ss.serialize()``.
 
         Examples
         --------
         >>> data = vector.serialize()
         >>> new_vector = Vector.ss.deserialize(data)
         >>> new_vector.isequal(vector)
         True
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/utils.py` & `python-graphblas-2023.7.0/graphblas/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             return getattr(lib, ext_name)
         except AttributeError:  # pragma: no cover (sanity)
             pass
         raise  # pragma: no cover (sanity)
 
 
 def wrapdoc(func_with_doc):
-    """Decorator to copy `__doc__` from a function onto the wrapped function."""
+    """Decorator to copy ``__doc__`` from a function onto the wrapped function."""
 
     def inner(func_wo_doc):
         func_wo_doc.__doc__ = func_with_doc.__doc__
         return func_wo_doc
 
     return inner
 
@@ -155,15 +155,15 @@
     raise ValueError(
         f"Bad value for order: {order!r}.  "
         'Expected "rowwise", "columnwise", "rows", "columns", "C", or "F"'
     )
 
 
 def normalize_chunks(chunks, shape):
-    """Normalize chunks argument for use by `Matrix.ss.split`.
+    """Normalize chunks argument for use by ``Matrix.ss.split``.
 
     Examples
     --------
     >>> shape = (10, 20)
     >>> normalize_chunks(10, shape)
     [(10,), (10, 10)]
     >>> normalize_chunks((10, 10), shape)
@@ -245,25 +245,25 @@
                 f"  Got: {type(chunk)}"
             )
         chunksizes.append(cur_chunks)
     return chunksizes
 
 
 def ensure_type(x, types):
-    """Try to ensure `x` is one of the given types, computing if necessary.
+    """Try to ensure ``x`` is one of the given types, computing if necessary.
 
-    `types` must be a type or a tuple of types as used in `isinstance`.
+    ``types`` must be a type or a tuple of types as used in ``isinstance``.
 
-    For example, if `types` is a Vector, then a Vector input will be returned,
-    and a `VectorExpression` input will be computed and returned as a Vector.
+    For example, if ``types`` is a Vector, then a Vector input will be returned,
+    and a ``VectorExpression`` input will be computed and returned as a Vector.
 
     TypeError will be raised if the input is not or can't be converted to types.
 
-    This function ignores `graphblas.config["autocompute"]`; it always computes
-    if the return type will match `types`.
+    This function ignores ``graphblas.config["autocompute"]``; it always computes
+    if the return type will match ``types``.
     """
     if isinstance(x, types):
         return x
     if isinstance(types, tuple):
         if output_type(x) in types:
             return x.new()
     elif output_type(x) is types:
@@ -354,14 +354,15 @@
 
 def _autogenerate_code(
     filepath,
     text,
     specializer=None,
     begin="# Begin auto-generated code",
     end="# End auto-generated code",
+    callblack=True,
 ):
     """Super low-tech auto-code generation used by automethods.py and infixmethods.py."""
     with filepath.open() as f:  # pragma: no branch (flaky)
         orig_text = f.read()
     if specializer:
         begin = f"{begin}: {specializer}"
         end = f"{end}: {specializer}"
@@ -380,11 +381,12 @@
     new_text = orig_text
     for start, stop in reversed(boundaries):
         new_text = f"{new_text[:start]}{begin}{text}{new_text[stop:]}"
     with filepath.open("w") as f:  # pragma: no branch (flaky)
         f.write(new_text)
     import subprocess
 
-    try:
-        subprocess.check_call(["black", filepath])
-    except FileNotFoundError:  # pragma: no cover (safety)
-        pass  # It's okay if `black` isn't installed; pre-commit hooks will do linting
+    if callblack:
+        try:
+            subprocess.check_call(["black", filepath])
+        except FileNotFoundError:  # pragma: no cover (safety)
+            pass  # It's okay if `black` isn't installed; pre-commit hooks will do linting
```

### Comparing `python-graphblas-2023.5.0/graphblas/core/vector.py` & `python-graphblas-2023.7.0/graphblas/core/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,25 +449,25 @@
         call("GrB_Vector_resize", [self, size])
         self._size = size.value
 
     def to_values(self, dtype=None, *, indices=True, values=True, sort=True):
         """Extract the indices and values as a 2-tuple of numpy arrays.
 
         .. deprecated:: 2022.11.0
-            `Vector.to_values` will be removed in a future release.
-            Use `Vector.to_coo` instead. Will be removed in version 2023.9.0 or later
+            ``Vector.to_values`` will be removed in a future release.
+            Use ``Vector.to_coo`` instead. Will be removed in version 2023.9.0 or later
 
         Parameters
         ----------
         dtype :
             Requested dtype for the output values array.
         indices :bool, default=True
-            Whether to return indices; will return `None` for indices if `False`
+            Whether to return indices; will return ``None`` for indices if ``False``
         values : bool, default=True
-            Whether to return values; will return `None` for values if `False`
+            Whether to return values; will return ``None`` for values if ``False``
         sort : bool, default=True
             Whether to require sorted indices.
 
         Returns
         -------
         np.ndarray[dtype=uint64] : Indices
         np.ndarray : Values
@@ -483,17 +483,17 @@
         """Extract the indices and values as a 2-tuple of numpy arrays.
 
         Parameters
         ----------
         dtype :
             Requested dtype for the output values array.
         indices :bool, default=True
-            Whether to return indices; will return `None` for indices if `False`
+            Whether to return indices; will return ``None`` for indices if ``False``
         values : bool, default=True
-            Whether to return values; will return `None` for values if `False`
+            Whether to return values; will return ``None`` for values if ``False``
         sort : bool, default=True
             Whether to require sorted indices.
 
         See Also
         --------
         to_dense
         to_dict
@@ -535,15 +535,15 @@
             c_values if values else None,
         )
 
     def build(self, indices, values, *, dup_op=None, clear=False, size=None):
         """Rarely used method to insert values into an existing Vector. The typical use case
         is to create a new Vector and insert values at the same time using :meth:`from_coo`.
 
-        All the arguments are used identically in :meth:`from_coo`, except for `clear`, which
+        All the arguments are used identically in :meth:`from_coo`, except for ``clear``, which
         indicates whether to clear the Vector prior to adding the new values.
         """
         # TODO: accept `dtype` keyword to match the dtype of `values`?
         indices = ints_to_numpy_buffer(indices, np.uint64, name="indices")
         values, dtype = values_to_numpy_buffer(values, self.dtype)
         n = values.shape[0]
         if indices.size != n:
@@ -608,15 +608,15 @@
                 dtype = self.dtype
             rv = Vector(dtype, size=self._size, name=name)
             if not clear:
                 rv(mask=mask, **opts)[...] = self
         else:
             if opts:
                 # Ignore opts for now
-                descriptor_lookup(**opts)
+                desc = descriptor_lookup(**opts)  # noqa: F841 (keep desc in scope for context)
             rv = Vector._from_obj(ffi_new("GrB_Vector*"), self.dtype, self._size, name=name)
             call("GrB_Vector_dup", [_Pointer(rv), self])
         return rv
 
     def diag(self, k=0, *, name=None):
         """Return a Matrix with values on the diagonal built from the Vector.
 
@@ -691,16 +691,16 @@
         )
 
     @classmethod
     def from_values(cls, indices, values, dtype=None, *, size=None, dup_op=None, name=None):
         """Create a new Vector from indices and values.
 
         .. deprecated:: 2022.11.0
-            `Vector.from_values` will be removed in a future release.
-            Use `Vector.from_coo` instead. Will be removed in version 2023.9.0 or later
+            ``Vector.from_values`` will be removed in a future release.
+            Use ``Vector.from_coo`` instead. Will be removed in version 2023.9.0 or later
 
         Parameters
         ----------
         indices : list or np.ndarray
             Vector indices.
         values : list or np.ndarray or scalar
             List of values. If a scalar is provided, all values will be set to this single value.
@@ -1753,15 +1753,15 @@
         else:
             dtype = lookup_dtype(dtype)
         idx = resolved_indexes.indices[0]
         if result is None:
             result = Scalar(dtype, is_cscalar=is_cscalar, name=name)
         if opts:
             # Ignore opts for now
-            descriptor_lookup(**opts)
+            desc = descriptor_lookup(**opts)  # noqa: F841 (keep desc in scope for context)
         if is_cscalar:
             dtype_name = "UDT" if dtype._is_udt else dtype.name
             if (
                 call(f"GrB_Vector_extractElement_{dtype_name}", [_Pointer(result), self, idx.index])
                 is not NoValue
             ):
                 result._empty = False
@@ -2173,14 +2173,17 @@
         return (self._size,)
 
     @wrapdoc(Vector.dup)
     def dup(self, dtype=None, *, clear=False, mask=None, name=None, **opts):
         if clear:
             if dtype is None:
                 dtype = self.dtype
+            if opts:
+                # Ignore opts for now
+                desc = descriptor_lookup(**opts)  # noqa: F841 (keep desc in scope for context)
             return self.output_type(dtype, *self.shape, name=name)
         return self.new(dtype, mask=mask, name=name, **opts)
 
     # Begin auto-generated code: Vector
     _get_value = automethods._get_value
     S = wrapdoc(Vector.S)(property(automethods.S))
     V = wrapdoc(Vector.V)(property(automethods.V))
```

### Comparing `python-graphblas-2023.5.0/graphblas/dtypes.py` & `python-graphblas-2023.7.0/graphblas/core/dtypes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-import warnings as _warnings
+import warnings
 
-import numpy as _np
-from numpy import find_common_type as _find_common_type
-from numpy import promote_types as _promote_types
-
-from . import backend
-from .core import NULL as _NULL
-from .core import _has_numba
-from .core import ffi as _ffi
-from .core import lib as _lib
+import numpy as np
+from numpy import promote_types, result_type
+
+from .. import backend, dtypes
+from ..core import NULL, _has_numba, ffi, lib
 
 if _has_numba:
-    import numba as _numba
+    import numba
 
 # Default assumption unless FC32/FC64 are found in lib
-_supports_complex = hasattr(_lib, "GrB_FC64") or hasattr(_lib, "GxB_FC64")
+_supports_complex = hasattr(lib, "GrB_FC64") or hasattr(lib, "GxB_FC64")
 
 
 class DataType:
     __slots__ = "name", "gb_obj", "gb_name", "c_type", "numba_type", "np_type", "__weakref__"
 
     def __init__(self, name, gb_obj, gb_name, c_type, numba_type, np_type):
         self.name = name
         self.gb_obj = gb_obj
         self.gb_name = gb_name
         self.c_type = c_type
         self.numba_type = numba_type
-        self.np_type = _np.dtype(np_type)
+        self.np_type = np.dtype(np_type) if np_type is not None else None
 
     def __repr__(self):
         return self.name
 
     def __eq__(self, other):
         try:
             return self is lookup_dtype(other)
@@ -58,15 +54,15 @@
 
     @property
     def _carg(self):
         return self.gb_obj[0] if self.gb_name is None else self.gb_obj
 
     @property
     def _is_anonymous(self):
-        return globals().get(self.name) is not self
+        return getattr(dtypes, self.name, None) is not self
 
     @property
     def _is_udt(self):
         return self.gb_name is None
 
     @staticmethod
     def _deserialize(name, dtype, is_anonymous):
@@ -76,236 +72,238 @@
             return _registry[name]
         return register_new(name, dtype)
 
 
 def register_new(name, dtype):
     if not name.isidentifier():
         raise ValueError(f"`name` argument must be a valid Python identifier; got: {name!r}")
-    if name in _registry or name in globals():
+    if name in _registry or hasattr(dtypes, name):
         raise ValueError(f"{name!r} name for dtype is unavailable")
     rv = register_anonymous(dtype, name)
     _registry[name] = rv
-    globals()[name] = rv
+    setattr(dtypes, name, rv)
     return rv
 
 
 def register_anonymous(dtype, name=None):
     try:
-        dtype = _np.dtype(dtype)
+        dtype = np.dtype(dtype)
     except TypeError:
         if isinstance(dtype, dict):
             # Allow dtypes such as `{'x': int, 'y': float}` for convenience
-            dtype = _np.dtype([(key, lookup_dtype(val).np_type) for key, val in dtype.items()])
+            dtype = np.dtype(
+                [(key, lookup_dtype(val).np_type) for key, val in dtype.items()], align=True
+            )
         elif isinstance(dtype, str) and "[" in dtype and dtype.endswith("]"):
             # Allow dtypes such as `"INT64[3, 4]"` for convenience
             base_dtype, shape = dtype.split("[", 1)
             base_dtype = lookup_dtype(base_dtype)
-            shape = _np.lib.format.safe_eval(f"[{shape}")
-            dtype = _np.dtype((base_dtype.np_type, shape))
+            shape = np.lib.format.safe_eval(f"[{shape}")
+            dtype = np.dtype((base_dtype.np_type, shape))
         else:
             raise
     if dtype in _registry:
         # Always use the same object, but use the latest name
         rv = _registry[dtype]
         if name is not None:
             if rv.gb_name is not None and name != rv.gb_name:
                 raise ValueError("dtype must not be a builtin type")
             rv.name = name  # Rename an existing object (a little weird, but okay)
         return rv
     if dtype.hasobject:
         raise ValueError("dtype must not allow Python objects")
 
-    from .exceptions import check_status_carg
+    from ..exceptions import check_status_carg
 
-    gb_obj = _ffi.new("GrB_Type*")
+    gb_obj = ffi.new("GrB_Type*")
     if backend == "suitesparse":
         # We name this so that we can serialize and deserialize UDTs
         # We don't yet have C definitions
         np_repr = _dtype_to_string(dtype).encode()
-        if len(np_repr) > _lib.GxB_MAX_NAME_LEN:
+        if len(np_repr) > lib.GxB_MAX_NAME_LEN:
             msg = (
                 f"UDT repr is too large to serialize ({len(repr(dtype).encode())} > "
-                f"{_lib.GxB_MAX_NAME_LEN})."
+                f"{lib.GxB_MAX_NAME_LEN})."
             )
             if name is not None:
-                np_repr = name.encode()[: _lib.GxB_MAX_NAME_LEN]
+                np_repr = name.encode()[: lib.GxB_MAX_NAME_LEN]
             else:
-                np_repr = np_repr[: _lib.GxB_MAX_NAME_LEN]
-            _warnings.warn(
+                np_repr = np_repr[: lib.GxB_MAX_NAME_LEN]
+            warnings.warn(
                 f"{msg}.  It will use the following name, "
                 f"and the dtype may need to be specified when deserializing: {np_repr}",
                 stacklevel=2,
             )
-        status = _lib.GxB_Type_new(gb_obj, dtype.itemsize, np_repr, _NULL)
+        status = lib.GxB_Type_new(gb_obj, dtype.itemsize, np_repr, NULL)
     else:
-        status = _lib.GrB_Type_new(gb_obj, dtype.itemsize)
+        status = lib.GrB_Type_new(gb_obj, dtype.itemsize)
     check_status_carg(status, "Type", gb_obj[0])
 
     # For now, let's use "opaque" unsigned bytes for the c type.
     if name is None:
         name = _default_name(dtype)
-    numba_type = _numba.typeof(dtype).dtype if _has_numba else None
+    numba_type = numba.typeof(dtype).dtype if _has_numba else None
     rv = DataType(name, gb_obj, None, f"uint8_t[{dtype.itemsize}]", numba_type, dtype)
     _registry[gb_obj] = rv
     _registry[dtype] = rv
     if _has_numba:
         _registry[numba_type] = rv
         _registry[numba_type.name] = rv
     return rv
 
 
 BOOL = DataType(
     "BOOL",
-    _lib.GrB_BOOL,
+    lib.GrB_BOOL,
     "GrB_BOOL",
     "_Bool",
-    _numba.types.bool_ if _has_numba else None,
-    _np.bool_,
+    numba.types.bool_ if _has_numba else None,
+    np.bool_,
 )
 INT8 = DataType(
-    "INT8", _lib.GrB_INT8, "GrB_INT8", "int8_t", _numba.types.int8 if _has_numba else None, _np.int8
+    "INT8", lib.GrB_INT8, "GrB_INT8", "int8_t", numba.types.int8 if _has_numba else None, np.int8
 )
 UINT8 = DataType(
     "UINT8",
-    _lib.GrB_UINT8,
+    lib.GrB_UINT8,
     "GrB_UINT8",
     "uint8_t",
-    _numba.types.uint8 if _has_numba else None,
-    _np.uint8,
+    numba.types.uint8 if _has_numba else None,
+    np.uint8,
 )
 INT16 = DataType(
     "INT16",
-    _lib.GrB_INT16,
+    lib.GrB_INT16,
     "GrB_INT16",
     "int16_t",
-    _numba.types.int16 if _has_numba else None,
-    _np.int16,
+    numba.types.int16 if _has_numba else None,
+    np.int16,
 )
 UINT16 = DataType(
     "UINT16",
-    _lib.GrB_UINT16,
+    lib.GrB_UINT16,
     "GrB_UINT16",
     "uint16_t",
-    _numba.types.uint16 if _has_numba else None,
-    _np.uint16,
+    numba.types.uint16 if _has_numba else None,
+    np.uint16,
 )
 INT32 = DataType(
     "INT32",
-    _lib.GrB_INT32,
+    lib.GrB_INT32,
     "GrB_INT32",
     "int32_t",
-    _numba.types.int32 if _has_numba else None,
-    _np.int32,
+    numba.types.int32 if _has_numba else None,
+    np.int32,
 )
 UINT32 = DataType(
     "UINT32",
-    _lib.GrB_UINT32,
+    lib.GrB_UINT32,
     "GrB_UINT32",
     "uint32_t",
-    _numba.types.uint32 if _has_numba else None,
-    _np.uint32,
+    numba.types.uint32 if _has_numba else None,
+    np.uint32,
 )
 INT64 = DataType(
     "INT64",
-    _lib.GrB_INT64,
+    lib.GrB_INT64,
     "GrB_INT64",
     "int64_t",
-    _numba.types.int64 if _has_numba else None,
-    _np.int64,
+    numba.types.int64 if _has_numba else None,
+    np.int64,
 )
 # _Index (like UINT64) is for internal use only and shouldn't be exposed to the user
 _INDEX = DataType(
     "UINT64",
-    _lib.GrB_UINT64,
+    lib.GrB_UINT64,
     "GrB_Index",
     "GrB_Index",
-    _numba.types.uint64 if _has_numba else None,
-    _np.uint64,
+    numba.types.uint64 if _has_numba else None,
+    np.uint64,
 )
 UINT64 = DataType(
     "UINT64",
-    _lib.GrB_UINT64,
+    lib.GrB_UINT64,
     "GrB_UINT64",
     "uint64_t",
-    _numba.types.uint64 if _has_numba else None,
-    _np.uint64,
+    numba.types.uint64 if _has_numba else None,
+    np.uint64,
 )
 FP32 = DataType(
     "FP32",
-    _lib.GrB_FP32,
+    lib.GrB_FP32,
     "GrB_FP32",
     "float",
-    _numba.types.float32 if _has_numba else None,
-    _np.float32,
+    numba.types.float32 if _has_numba else None,
+    np.float32,
 )
 FP64 = DataType(
     "FP64",
-    _lib.GrB_FP64,
+    lib.GrB_FP64,
     "GrB_FP64",
     "double",
-    _numba.types.float64 if _has_numba else None,
-    _np.float64,
+    numba.types.float64 if _has_numba else None,
+    np.float64,
 )
 
-if _supports_complex and hasattr(_lib, "GxB_FC32"):
+if _supports_complex and hasattr(lib, "GxB_FC32"):
     FC32 = DataType(
         "FC32",
-        _lib.GxB_FC32,
+        lib.GxB_FC32,
         "GxB_FC32",
         "float _Complex",
-        _numba.types.complex64 if _has_numba else None,
-        _np.complex64,
+        numba.types.complex64 if _has_numba else None,
+        np.complex64,
     )
-if _supports_complex and hasattr(_lib, "GrB_FC32"):  # pragma: no cover (unused)
+if _supports_complex and hasattr(lib, "GrB_FC32"):  # pragma: no cover (unused)
     FC32 = DataType(
         "FC32",
-        _lib.GrB_FC32,
+        lib.GrB_FC32,
         "GrB_FC32",
         "float _Complex",
-        _numba.types.complex64 if _has_numba else None,
-        _np.complex64,
+        numba.types.complex64 if _has_numba else None,
+        np.complex64,
     )
-if _supports_complex and hasattr(_lib, "GxB_FC64"):
+if _supports_complex and hasattr(lib, "GxB_FC64"):
     FC64 = DataType(
         "FC64",
-        _lib.GxB_FC64,
+        lib.GxB_FC64,
         "GxB_FC64",
         "double _Complex",
-        _numba.types.complex128 if _has_numba else None,
-        _np.complex128,
+        numba.types.complex128 if _has_numba else None,
+        np.complex128,
     )
-if _supports_complex and hasattr(_lib, "GrB_FC64"):  # pragma: no cover (unused)
+if _supports_complex and hasattr(lib, "GrB_FC64"):  # pragma: no cover (unused)
     FC64 = DataType(
         "FC64",
-        _lib.GrB_FC64,
+        lib.GrB_FC64,
         "GrB_FC64",
         "double _Complex",
-        _numba.types.complex128 if _has_numba else None,
-        _np.complex128,
+        numba.types.complex128 if _has_numba else None,
+        np.complex128,
     )
 
 # Used for testing user-defined functions
 _sample_values = {
-    INT8: _np.int8(1),
-    UINT8: _np.uint8(1),
-    INT16: _np.int16(1),
-    UINT16: _np.uint16(1),
-    INT32: _np.int32(1),
-    UINT32: _np.uint32(1),
-    INT64: _np.int64(1),
-    UINT64: _np.uint64(1),
-    FP32: _np.float32(0.5),
-    FP64: _np.float64(0.5),
-    BOOL: _np.bool_(True),
+    INT8: np.int8(1),
+    UINT8: np.uint8(1),
+    INT16: np.int16(1),
+    UINT16: np.uint16(1),
+    INT32: np.int32(1),
+    UINT32: np.uint32(1),
+    INT64: np.int64(1),
+    UINT64: np.uint64(1),
+    FP32: np.float32(0.5),
+    FP64: np.float64(0.5),
+    BOOL: np.bool_(True),
 }
 if _supports_complex:
     _sample_values.update(
         {
-            FC32: _np.complex64(complex(0, 0.5)),
-            FC64: _np.complex128(complex(0, 0.5)),
+            FC32: np.complex64(complex(0, 0.5)),
+            FC64: np.complex128(complex(0, 0.5)),
         }
     )
 
 # Create register to easily lookup types by name, gb_obj, or c_type
 _registry = {}
 _dtypes_to_register = [
     BOOL,
@@ -385,27 +383,19 @@
     unify(INT8, UINT16) -> INT32
     unify(BOOL, UINT16) -> UINT16
     unify(FP32, INT32) -> FP64
     """
     if type1 is type2:
         return type1
     if is_left_scalar:
-        scalar_types = [type1.np_type]
-        array_types = []
-    elif not is_right_scalar:
-        # Using `promote_types` is faster than `find_common_type`
-        return lookup_dtype(_promote_types(type1.np_type, type2.np_type))
-    else:
-        scalar_types = []
-        array_types = [type1.np_type]
-    if is_right_scalar:
-        scalar_types.append(type2.np_type)
-    else:
-        array_types.append(type2.np_type)
-    return lookup_dtype(_find_common_type(array_types, scalar_types))
+        if not is_right_scalar:
+            return lookup_dtype(result_type(np.array(0, type1.np_type), type2.np_type))
+    elif is_right_scalar:
+        return lookup_dtype(result_type(type1.np_type, np.array(0, type2.np_type)))
+    return lookup_dtype(promote_types(type1.np_type, type2.np_type))
 
 
 def _default_name(dtype):
     if dtype in _registry:
         dt = _registry[dtype]
         if not dt._is_udt:
             return dt.name
@@ -427,37 +417,37 @@
     This is useful when serializing UDT.  To recreate the dtype, do:
 
     >>> s = _dtype_to_string(dtype)
     >>> new_dtype = _string_to_dtype(s)
     >>> dtype == new_dtype
     True
     """
-    if isinstance(dtype, _np.dtype) and dtype not in _registry:
+    if isinstance(dtype, np.dtype) and dtype not in _registry:
         np_type = dtype
     else:
         dtype = lookup_dtype(dtype)
         if not dtype._is_udt:
             return dtype.name
         np_type = dtype.np_type
     s = str(np_type)
     try:
-        if _np.dtype(_np.lib.format.safe_eval(s)) == np_type:  # pragma: no branch (safety)
+        if np.dtype(np.lib.format.safe_eval(s)) == np_type:  # pragma: no branch (safety)
             return s
     except Exception:
         pass
-    if _np.dtype(np_type.str) != np_type:  # pragma: no cover (safety)
+    if np.dtype(np_type.str) != np_type:  # pragma: no cover (safety)
         raise ValueError(f"Unable to reliably convert dtype to string and back: {dtype}")
     return repr(np_type.str)
 
 
 def _string_to_dtype(s):
     """Convert a string back to a dtype.
 
     >>> _string_to_dtype(_dtype_to_string(dtype)) == dtype
     True
     """
     try:
         return lookup_dtype(s)
     except Exception:
         pass
-    np_type = _np.dtype(_np.lib.format.safe_eval(s))
+    np_type = np.dtype(np.lib.format.safe_eval(s))
     return lookup_dtype(np_type)
```

### Comparing `python-graphblas-2023.5.0/graphblas/exceptions.py` & `python-graphblas-2023.7.0/graphblas/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/io/_awkward.py` & `python-graphblas-2023.7.0/graphblas/io/_awkward.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,66 +3,14 @@
 from ..core.matrix import Matrix
 from ..core.utils import output_type
 from ..core.vector import Vector
 
 _AwkwardDoublyCompressedMatrix = None
 
 
-def from_awkward(A, *, name=None):
-    """Create a Matrix or Vector from an Awkward Array.
-
-    The Awkward Array must have top-level parameters: format, shape
-
-    The Awkward Array must have top-level attributes based on format:
-    - vec/csr/csc: values, indices
-    - hypercsr/hypercsc: values, indices, offset_labels
-
-    Parameters
-    ----------
-    A : awkward.Array
-        Awkward Array with values and indices
-    name : str, optional
-        Name of resulting Matrix or Vector
-
-    Returns
-    -------
-    Vector or Matrix
-    """
-    params = A.layout.parameters
-    if missing := {"format", "shape"} - params.keys():
-        raise ValueError(f"Missing parameters: {missing}")
-    format = params["format"]
-    shape = params["shape"]
-
-    if len(shape) == 1:
-        if format != "vec":
-            raise ValueError(f"Invalid format for Vector: {format}")
-        return Vector.from_coo(
-            A.indices.layout.data, A.values.layout.data, size=shape[0], name=name
-        )
-    nrows, ncols = shape
-    values = A.values.layout.content.data
-    indptr = A.values.layout.offsets.data
-    if format == "csr":
-        cols = A.indices.layout.content.data
-        return Matrix.from_csr(indptr, cols, values, ncols=ncols, name=name)
-    if format == "csc":
-        rows = A.indices.layout.content.data
-        return Matrix.from_csc(indptr, rows, values, nrows=nrows, name=name)
-    if format == "hypercsr":
-        rows = A.offset_labels.layout.data
-        cols = A.indices.layout.content.data
-        return Matrix.from_dcsr(rows, indptr, cols, values, nrows=nrows, ncols=ncols, name=name)
-    if format == "hypercsc":
-        cols = A.offset_labels.layout.data
-        rows = A.indices.layout.content.data
-        return Matrix.from_dcsc(cols, indptr, rows, values, nrows=nrows, ncols=ncols, name=name)
-    raise ValueError(f"Invalid format for Matrix: {format}")
-
-
 def to_awkward(A, format=None):
     """Create an Awkward Array from a GraphBLAS Matrix.
 
     Parameters
     ----------
     A : Matrix or Vector
         GraphBLAS object to be converted
@@ -175,7 +123,65 @@
 
     ret = ak.from_buffers(form, size, d)
     ret = ak.with_parameter(ret, "format", format)
     ret = ak.with_parameter(ret, "shape", list(A.shape))
     if classname:
         ret = ak.with_name(ret, classname)
     return ret
+
+
+def from_awkward(A, *, name=None):
+    """Create a Matrix or Vector from an Awkward Array.
+
+    The Awkward Array must have top-level parameters: format, shape
+
+    The Awkward Array must have top-level attributes based on format:
+    - vec/csr/csc: values, indices
+    - hypercsr/hypercsc: values, indices, offset_labels
+
+    Parameters
+    ----------
+    A : awkward.Array
+        Awkward Array with values and indices
+    name : str, optional
+        Name of resulting Matrix or Vector
+
+    Returns
+    -------
+    Vector or Matrix
+
+    Note: the intended purpose of this function is to facilitate
+    conversion of an `awkward-array` that was created via `to_awkward`
+    function. If attempting to convert an arbitrary `awkward-array`,
+    make sure that the top-level attributes and parameters contain
+    the expected values.
+    """
+    params = A.layout.parameters
+    if missing := {"format", "shape"} - params.keys():
+        raise ValueError(f"Missing parameters: {missing}")
+    format = params["format"]
+    shape = params["shape"]
+
+    if len(shape) == 1:
+        if format != "vec":
+            raise ValueError(f"Invalid format for Vector: {format}")
+        return Vector.from_coo(
+            A.indices.layout.data, A.values.layout.data, size=shape[0], name=name
+        )
+    nrows, ncols = shape
+    values = A.values.layout.content.data
+    indptr = A.values.layout.offsets.data
+    if format == "csr":
+        cols = A.indices.layout.content.data
+        return Matrix.from_csr(indptr, cols, values, ncols=ncols, name=name)
+    if format == "csc":
+        rows = A.indices.layout.content.data
+        return Matrix.from_csc(indptr, rows, values, nrows=nrows, name=name)
+    if format == "hypercsr":
+        rows = A.offset_labels.layout.data
+        cols = A.indices.layout.content.data
+        return Matrix.from_dcsr(rows, indptr, cols, values, nrows=nrows, ncols=ncols, name=name)
+    if format == "hypercsc":
+        cols = A.offset_labels.layout.data
+        rows = A.indices.layout.content.data
+        return Matrix.from_dcsc(cols, indptr, rows, values, nrows=nrows, ncols=ncols, name=name)
+    raise ValueError(f"Invalid format for Matrix: {format}")
```

### Comparing `python-graphblas-2023.5.0/graphblas/io/_matrixmarket.py` & `python-graphblas-2023.7.0/graphblas/io/_matrixmarket.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     Returns
     -------
     :class:`~graphblas.Matrix`
     """
     try:
         # scipy is currently needed for *all* engines
         from scipy.io import mmread
-        from scipy.sparse import isspmatrix_coo
     except ImportError:  # pragma: no cover (import)
         raise ImportError("scipy is required to read Matrix Market files") from None
     engine = engine.lower()
     if engine in {"auto", "fmm", "fast_matrix_market"}:
         try:
             from fast_matrix_market import mmread  # noqa: F811
         except ImportError:  # pragma: no cover (import)
@@ -50,15 +49,15 @@
                     f'using the "{engine}" engine'
                 ) from None
     elif engine != "scipy":
         raise ValueError(
             f'Bad engine value: {engine!r}. Must be "auto", "scipy", "fmm", or "fast_matrix_market"'
         )
     array = mmread(source, **kwargs)
-    if isspmatrix_coo(array):
+    if getattr(array, "format", None) == "coo":
         nrows, ncols = array.shape
         return Matrix.from_coo(
             array.row, array.col, array.data, nrows=nrows, ncols=ncols, dup_op=dup_op, name=name
         )
     return Matrix.from_dense(array, name=name)
 
 
@@ -101,29 +100,39 @@
         # scipy is currently needed for *all* engines
         from scipy.io import mmwrite
     except ImportError:  # pragma: no cover (import)
         raise ImportError("scipy is required to write Matrix Market files") from None
     engine = engine.lower()
     if engine in {"auto", "fmm", "fast_matrix_market"}:
         try:
-            from fast_matrix_market import mmwrite  # noqa: F811
+            from fast_matrix_market import __version__, mmwrite  # noqa: F811
         except ImportError:  # pragma: no cover (import)
             if engine != "auto":
                 raise ImportError(
                     "fast_matrix_market is required to write Matrix Market files "
                     f'using the "{engine}" engine'
                 ) from None
+        else:
+            import scipy as sp
+
+            engine = "fast_matrix_market"
     elif engine != "scipy":
         raise ValueError(
             f'Bad engine value: {engine!r}. Must be "auto", "scipy", "fmm", or "fast_matrix_market"'
         )
     if backend == "suitesparse" and matrix.ss.format in {"fullr", "fullc"}:
         array = matrix.ss.export()["values"]
     else:
         array = to_scipy_sparse(matrix, format="coo")
+        if engine == "fast_matrix_market" and __version__ < "1.7." and sp.__version__ > "1.11.":
+            # 2023-06-25: scipy 1.11.0 added `sparray` and changed e.g. `ss.isspmatrix_coo`.
+            # fast_matrix_market updated to handle this in version 1.7.0
+            # Also, it looks like fast_matrix_market has special writers for csr and csc;
+            # should we see if using those are faster?
+            array = sp.sparse.coo_matrix(array)  # FLAKY COVERAGE
     mmwrite(
         target,
         array,
         comment=comment,
         field=field,
         precision=precision,
         symmetry=symmetry,
```

### Comparing `python-graphblas-2023.5.0/graphblas/io/_networkx.py` & `python-graphblas-2023.7.0/graphblas/io/_networkx.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/io/_numpy.py` & `python-graphblas-2023.7.0/graphblas/io/_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from ._scipy import from_scipy_sparse, to_scipy_sparse
 
 
 def from_numpy(m):  # pragma: no cover (deprecated)
     """Create a sparse Vector or Matrix from a dense numpy array.
 
     .. deprecated:: 2023.2.0
-        `from_numpy` will be removed in a future release.
-        Use `Vector.from_dense` or `Matrix.from_dense` instead.
+        ``from_numpy`` will be removed in a future release.
+        Use ``Vector.from_dense`` or ``Matrix.from_dense`` instead.
         Will be removed in version 2023.10.0 or later
 
     A value of 0 is considered as "missing".
 
-    - m.ndim == 1 returns a `Vector`
-    - m.ndim == 2 returns a `Matrix`
+    - m.ndim == 1 returns a ``Vector``
+    - m.ndim == 2 returns a ``Matrix``
     - m.ndim > 2 raises an error
 
     dtype is inferred from m.dtype
 
     Parameters
     ----------
     m : np.ndarray
@@ -61,16 +61,16 @@
     return from_scipy_sparse(A)
 
 
 def to_numpy(m):  # pragma: no cover (deprecated)
     """Create a dense numpy array from a sparse Vector or Matrix.
 
     .. deprecated:: 2023.2.0
-        `to_numpy` will be removed in a future release.
-        Use `Vector.to_dense` or `Matrix.to_dense` instead.
+        ``to_numpy`` will be removed in a future release.
+        Use ``Vector.to_dense`` or ``Matrix.to_dense`` instead.
         Will be removed in version 2023.10.0 or later
 
     Missing values will become 0 in the output.
 
     numpy dtype will match the GraphBLAS dtype
 
     Parameters
```

### Comparing `python-graphblas-2023.5.0/graphblas/io/_scipy.py` & `python-graphblas-2023.7.0/graphblas/io/_scipy.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/io/_sparse.py` & `python-graphblas-2023.7.0/graphblas/io/_sparse.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/monoid/numpy.py` & `python-graphblas-2023.7.0/graphblas/monoid/numpy.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/op/__init__.py` & `python-graphblas-2023.7.0/graphblas/op/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/op/numpy.py` & `python-graphblas-2023.7.0/graphblas/op/numpy.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/select/__init__.py` & `python-graphblas-2023.7.0/graphblas/select/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,35 @@
 # boolean and they default to `select` when called, rather than
 # `apply`).
 _delayed = {}
 _binary_to_select = {}
 
 
 def __dir__():
-    return globals().keys() | _delayed.keys()
+    return globals().keys() | _delayed.keys() | {"ss"}
 
 
 def __getattr__(key):
     if key in _delayed:
         func, kwargs = _delayed.pop(key)
         rv = func(**kwargs)
         globals()[key] = rv
         return rv
+    if key == "ss":
+        from .. import backend
+
+        if backend != "suitesparse":
+            raise AttributeError(
+                f'module {__name__!r} only has attribute "ss" when backend is "suitesparse"'
+            )
+        from importlib import import_module
+
+        ss = import_module(".ss", __name__)
+        globals()["ss"] = ss
+        return ss
     raise AttributeError(f"module {__name__!r} has no attribute {key!r}")
 
 
 def _resolve_expr(expr, callname, opname):
     from ..core.base import BaseExpression
 
     if not isinstance(expr, BaseExpression):
@@ -53,17 +65,17 @@
         else:  # e.g., suitesparse-vanilla
             tensor = tensor[0].new()
             thunk = thunk[0].new()
     return globals()[method](tensor, thunk)
 
 
 def _match_expr(parent, expr):
-    """Match expressions to rewrite `A.select(A < 5)` into select expression.
+    """Match expressions to rewrite ``A.select(A < 5)`` into select expression.
 
-    The argument must match the parent, so this _won't_ be rewritten: `A.select(B < 5)`
+    The argument must match the parent, so this _won't_ be rewritten: ``A.select(B < 5)``
     """
     args = expr.args
     op = expr.op
     if (
         expr.method_name == "apply"
         and len(args) == 2
         and op.parent in _binary_to_select
@@ -79,57 +91,57 @@
     """
     An advanced select method which allows for easily expressing
     value comparison logic.
 
     Example usage:
     >>> gb.select.value(A > 0)
 
-    The example will dispatch to `gb.select.valuegt(A, 0)`
+    The example will dispatch to ``gb.select.valuegt(A, 0)``
     while being nicer to read.
     """
     return _resolve_expr(expr, "value", "value")
 
 
 def row(expr):
     """
     An advanced select method which allows for easily expressing
     Matrix row index comparison logic.
 
     Example usage:
     >>> gb.select.row(A <= 5)
 
-    The example will dispatch to `gb.select.rowle(A, 5)`
+    The example will dispatch to ``gb.select.rowle(A, 5)``
     while being potentially nicer to read.
     """
     return _resolve_expr(expr, "row", "row")
 
 
 def column(expr):
     """
     An advanced select method which allows for easily expressing
     Matrix column index comparison logic.
 
     Example usage:
     >>> gb.select.column(A <= 5)
 
-    The example will dispatch to `gb.select.colle(A, 5)`
+    The example will dispatch to ``gb.select.colle(A, 5)``
     while being potentially nicer to read.
     """
     return _resolve_expr(expr, "column", "col")
 
 
 def index(expr):
     """
     An advanced select method which allows for easily expressing
     Vector index comparison logic.
 
     Example usage:
     >>> gb.select.index(v <= 5)
 
-    The example will dispatch to `gb.select.indexle(v, 5)`
+    The example will dispatch to ``gb.select.indexle(v, 5)``
     while being potentially nicer to read.
     """
     return _resolve_expr(expr, "index", "index")
 
 
 from ..core import operator  # noqa: E402 isort:skip
```

### Comparing `python-graphblas-2023.5.0/graphblas/semiring/__init__.py` & `python-graphblas-2023.7.0/graphblas/semiring/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/semiring/numpy.py` & `python-graphblas-2023.7.0/graphblas/semiring/numpy.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/ss/_core.py` & `python-graphblas-2023.7.0/graphblas/ss/_core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from collections.abc import Mapping
 
 from ..core import ffi, lib
 from ..core.base import _expect_type
+from ..core.descriptor import lookup as descriptor_lookup
 from ..core.matrix import Matrix, TransposedMatrix
 from ..core.scalar import _as_scalar
+from ..core.ss import _IS_SSGB7
 from ..core.ss.config import BaseConfig
 from ..core.ss.matrix import _concat_mn
 from ..core.vector import Vector
 from ..dtypes import INT64
 from ..exceptions import _error_code_lookup
 
 
 class _graphblas_ss:
-    """Used in `_expect_type`."""
+    """Used in ``_expect_type``."""
 
 
 _graphblas_ss.__name__ = "graphblas.ss"
 _graphblas_ss = _graphblas_ss()
 
 
 def diag(x, k=0, dtype=None, *, name=None, **opts):
@@ -29,16 +31,16 @@
 
     Parameters
     ----------
     x : Vector or Matrix
         The Vector to assign to the diagonal, or the Matrix from which to
         extract the diagonal.
     k : int, default 0
-        Diagonal in question.  Use `k>0` for diagonals above the main diagonal,
-        and `k<0` for diagonals below the main diagonal.
+        Diagonal in question.  Use ``k>0`` for diagonals above the main diagonal,
+        and ``k<0`` for diagonals below the main diagonal.
 
     See Also
     --------
     Vector.diag
     Matrix.diag
     Vector.ss.build_diag
     Matrix.ss.build_diag
@@ -48,14 +50,17 @@
         _graphblas_ss, x, (Matrix, TransposedMatrix, Vector), within="diag", argname="x"
     )
     k = _as_scalar(k, INT64, is_cscalar=True)
     if dtype is None:
         dtype = x.dtype
     typ = type(x)
     if typ is Vector:
+        if opts:
+            # Ignore opts for now
+            desc = descriptor_lookup(**opts)  # noqa: F841 (keep desc in scope for context)
         size = x._size + abs(k.value)
         rv = Matrix(dtype, nrows=size, ncols=size, name=name)
         rv.ss.build_diag(x, k)
     else:
         if k.value < 0:
             size = max(0, min(x._nrows + k.value, x._ncols))
         else:
@@ -67,17 +72,17 @@
 
 def concat(tiles, dtype=None, *, name=None, **opts):
     """
     GxB_Matrix_concat.
 
     Concatenate a 2D list of Matrix objects into a new Matrix, or a 1D list of
     Vector objects into a new Vector.  To concatenate into existing objects,
-    use ``Matrix.ss.concat`` or `Vector.ss.concat`.
+    use ``Matrix.ss.concat`` or ``Vector.ss.concat``.
 
-    Vectors may be used as `Nx1` Matrix objects when creating a new Matrix.
+    Vectors may be used as ``Nx1`` Matrix objects when creating a new Matrix.
 
     This performs the opposite operation as ``split``.
 
     See Also
     --------
     Matrix.ss.split
     Matrix.ss.concat
@@ -116,62 +121,105 @@
     bitmap_switch : List[double]
         Threshold that determines when to switch to bitmap format
     nthreads : int
         Maximum number of OpenMP threads to use
     memory_pool : List[int]
     burble : bool
         Enable diagnostic printing from SuiteSparse:GraphBLAS
-    print_1based: bool
+    print_1based : bool
     gpu_control : str, {"always", "never"}
+        Only available for SuiteSparse:GraphBLAS 7
+        **GPU support is a work in progress--not recommended to use**
     gpu_chunk : double
+        Only available for SuiteSparse:GraphBLAS 7
+        **GPU support is a work in progress--not recommended to use**
+    gpu_id : int
+        Which GPU to use; default is -1, which means do not run on the GPU.
+        Only available for SuiteSparse:GraphBLAS 8
+        **GPU support is a work in progress--not recommended to use**
 
     Setting values to None restores the default value for most configurations.
     """
 
     _get_function = "GxB_Global_Option_get"
     _set_function = "GxB_Global_Option_set"
+    if not _IS_SSGB7:
+        _context_keys = {"chunk", "gpu_id", "nthreads"}
     _null_valid = {"bitmap_switch"}
     _options = {
         # Matrix/Vector format
         "hyper_switch": (lib.GxB_HYPER_SWITCH, "double"),
         "bitmap_switch": (lib.GxB_BITMAP_SWITCH, f"double[{lib.GxB_NBITMAP_SWITCH}]"),
         "format": (lib.GxB_FORMAT, "GxB_Format_Value"),
         # OpenMP control
         "nthreads": (lib.GxB_GLOBAL_NTHREADS, "int"),
         "chunk": (lib.GxB_GLOBAL_CHUNK, "double"),
         # Memory pool control
         "memory_pool": (lib.GxB_MEMORY_POOL, "int64_t[64]"),
         # Diagnostics (skipping "printf" and "flush" for now)
         "burble": (lib.GxB_BURBLE, "bool"),
         "print_1based": (lib.GxB_PRINT_1BASED, "bool"),
-        # CUDA GPU control
-        "gpu_control": (lib.GxB_GLOBAL_GPU_CONTROL, "GrB_Desc_Value"),
-        "gpu_chunk": (lib.GxB_GLOBAL_GPU_CHUNK, "double"),
     }
+    if _IS_SSGB7:
+        _options.update(
+            {
+                "gpu_control": (lib.GxB_GLOBAL_GPU_CONTROL, "GrB_Desc_Value"),
+                "gpu_chunk": (lib.GxB_GLOBAL_GPU_CHUNK, "double"),
+            }
+        )
+    else:
+        _options.update(
+            {
+                # JIT control
+                "jit_c_control": (lib.GxB_JIT_C_CONTROL, "int"),
+                "jit_use_cmake": (lib.GxB_JIT_USE_CMAKE, "bool"),
+                "jit_c_compiler_name": (lib.GxB_JIT_C_COMPILER_NAME, "char*"),
+                "jit_c_compiler_flags": (lib.GxB_JIT_C_COMPILER_FLAGS, "char*"),
+                "jit_c_linker_flags": (lib.GxB_JIT_C_LINKER_FLAGS, "char*"),
+                "jit_c_libraries": (lib.GxB_JIT_C_LIBRARIES, "char*"),
+                "jit_c_cmake_libs": (lib.GxB_JIT_C_CMAKE_LIBS, "char*"),
+                "jit_c_preface": (lib.GxB_JIT_C_PREFACE, "char*"),
+                "jit_error_log": (lib.GxB_JIT_ERROR_LOG, "char*"),
+                "jit_cache_path": (lib.GxB_JIT_CACHE_PATH, "char*"),
+                # CUDA GPU control
+                "gpu_id": (lib.GxB_GLOBAL_GPU_ID, "int"),
+            }
+        )
     # Values to restore defaults
     _defaults = {
         "hyper_switch": lib.GxB_HYPER_DEFAULT,
         "bitmap_switch": None,
         "format": lib.GxB_FORMAT_DEFAULT,
         "nthreads": 0,
         "chunk": 0,
         "burble": 0,
         "print_1based": 0,
     }
+    if not _IS_SSGB7:
+        _defaults["gpu_id"] = -1  # -1 means no GPU
     _enumerations = {
         "format": {
             "by_row": lib.GxB_BY_ROW,
             "by_col": lib.GxB_BY_COL,
             # "no_format": lib.GxB_NO_FORMAT,  # Used by iterators; not valid here
         },
-        "gpu_control": {
+    }
+    if _IS_SSGB7:
+        _enumerations["gpu_control"] = {
             "always": lib.GxB_GPU_ALWAYS,
             "never": lib.GxB_GPU_NEVER,
-        },
-    }
+        }
+    else:
+        _enumerations["jit_c_control"] = {
+            "off": lib.GxB_JIT_OFF,
+            "pause": lib.GxB_JIT_PAUSE,
+            "run": lib.GxB_JIT_RUN,
+            "load": lib.GxB_JIT_LOAD,
+            "on": lib.GxB_JIT_ON,
+        }
 
 
 class About(Mapping):
     _modes = {
         lib.GrB_NONBLOCKING: "nonblocking",
         lib.GrB_BLOCKING: "blocking",
         lib.GxB_NONBLOCKING_GPU: "nonblocking_gpu",
@@ -250,8 +298,14 @@
         )
 
     __repr__ = GlobalConfig.__repr__
     _ipython_key_completions_ = GlobalConfig._ipython_key_completions_
 
 
 about = About()
-config = GlobalConfig()
+if _IS_SSGB7:
+    config = GlobalConfig()
+else:
+    # Context was introduced in SuiteSparse:GraphBLAS 8.0
+    from ..core.ss.context import global_context
+
+    config = GlobalConfig(context=global_context)
```

### Comparing `python-graphblas-2023.5.0/graphblas/tests/conftest.py` & `python-graphblas-2023.7.0/graphblas/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import atexit
+import contextlib
 import functools
 import itertools
 import platform
 from pathlib import Path
 
 import numpy as np
 import pytest
@@ -14,34 +15,39 @@
 orig_semirings = set()
 
 pypy = platform.python_implementation() == "PyPy"
 
 
 def pytest_configure(config):
     rng = np.random.default_rng()
-    randomly = config.getoption("--randomly", False)
+    randomly = config.getoption("--randomly", None)
+    if randomly is None:  # pragma: no cover
+        options_unavailable = True
+        randomly = True
+        config.addinivalue_line("markers", "slow: Skipped unless --runslow passed")
+    else:
+        options_unavailable = False
     backend = config.getoption("--backend", None)
     if backend is None:
         if randomly:
             backend = "suitesparse" if rng.random() < 0.5 else "suitesparse-vanilla"
         else:
             backend = "suitesparse"
-    blocking = config.getoption("--blocking", True)
+    blocking = config.getoption("--blocking", None)
     if blocking is None:  # pragma: no branch
         blocking = rng.random() < 0.5 if randomly else True
     record = config.getoption("--record", False)
     if record is None:  # pragma: no branch
         record = rng.random() < 0.5 if randomly else False
-    mapnumpy = config.getoption("--mapnumpy", False)
+    mapnumpy = config.getoption("--mapnumpy", None)
     if mapnumpy is None:
         mapnumpy = rng.random() < 0.5 if randomly else False
-    runslow = config.getoption("--runslow", False)
+    runslow = config.getoption("--runslow", None)
     if runslow is None:
-        # Add a small amount of randomization to be safer
-        runslow = rng.random() < 0.05 if randomly else False
+        runslow = options_unavailable
     config.runslow = runslow
 
     gb.config.set(autocompute=False, mapnumpy=mapnumpy)
 
     gb.init(backend, blocking=blocking)
     print(
         f"Running tests with {backend!r} backend, blocking={blocking}, "
@@ -105,14 +111,35 @@
     except ImportError:
         return
     icecream.install()
     # icecream.ic.disable()  # This disables icecream; do ic.enable() to re-enable
     return icecream.ic
 
 
+@contextlib.contextmanager
+def burble():  # pragma: no cover (debug)
+    """Show the burble diagnostics within a context."""
+    if gb.backend != "suitesparse":
+        yield
+        return
+    prev = gb.ss.config["burble"]
+    gb.ss.config["burble"] = True
+    try:
+        yield
+    finally:
+        gb.ss.config["burble"] = prev
+
+
+@pytest.fixture(scope="session")
+def burble_all():  # pragma: no cover (debug)
+    """Show the burble diagnostics for the entire test."""
+    with burble():
+        yield burble
+
+
 def autocompute(func):
     @functools.wraps(func)
     def inner(*args, **kwargs):
         with gb.config.set(autocompute=True):
             return func(*args, **kwargs)
 
     return inner
```

### Comparing `python-graphblas-2023.5.0/graphblas/tests/pickle1-vanilla.pkl` & `python-graphblas-2023.7.0/graphblas/tests/pickle1-vanilla.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/pickle1.pkl` & `python-graphblas-2023.7.0/graphblas/tests/pickle1.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/pickle2-vanilla.pkl` & `python-graphblas-2023.7.0/graphblas/tests/pickle2-vanilla.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/pickle2.pkl` & `python-graphblas-2023.7.0/graphblas/tests/pickle2.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/pickle3-vanilla.pkl` & `python-graphblas-2023.7.0/graphblas/tests/pickle3-vanilla.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/pickle3.pkl` & `python-graphblas-2023.7.0/graphblas/tests/pickle3.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_core.py` & `python-graphblas-2023.7.0/graphblas/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,11 +79,14 @@
     pkgs = [f"graphblas.{x}" for x in setuptools.find_packages(str(path))]
     pkgs.append("graphblas")
     pkgs.sort()
     pyproject = path.parent / "pyproject.toml"
     if not pyproject.exists():  # pragma: no cover (safety)
         pytest.skip("Did not find pyproject.toml")
     with pyproject.open("rb") as f:
-        pkgs2 = sorted(tomli.load(f)["tool"]["setuptools"]["packages"])
+        cfg = tomli.load(f)
+    if cfg.get("project", {}).get("name") != "python-graphblas":  # pragma: no cover (safety)
+        pytest.skip("Did not find correct pyproject.toml")
+    pkgs2 = sorted(cfg["tool"]["setuptools"]["packages"])
     assert (
         pkgs == pkgs2
     ), "If there are extra items on the left, add them to pyproject.toml:tool.setuptools.packages"
```

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_descriptor.py` & `python-graphblas-2023.7.0/graphblas/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_dtype.py` & `python-graphblas-2023.7.0/graphblas/tests/test_dtype.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import string
 import sys
 
 import numpy as np
 import pytest
 
 import graphblas as gb
-from graphblas import dtypes
+from graphblas import core, dtypes
 from graphblas.core import lib
 from graphblas.dtypes import lookup_dtype
 
 suitesparse = gb.backend == "suitesparse"
 is_win = sys.platform.startswith("win")
 
 all_dtypes = [
@@ -119,29 +119,29 @@
     with pytest.raises(TypeError):
         assert dtypes.BOOL == object()
     with pytest.raises(TypeError):
         assert object() != dtypes.BOOL
 
 
 def test_dtypes_match_numpy():
-    for key, val in dtypes._registry.items():
+    for key, val in core.dtypes._registry.items():
         try:
             if key is int or (isinstance(key, str) and key == "int"):
                 # For win64, numpy treats int as int32, not int64
                 # graphblas won't allow this craziness
                 npval = np.int64
             else:
                 npval = np.dtype(key)
         except Exception:
             continue
         assert dtypes.lookup_dtype(npval) == val, f"{key} of type {type(key)}"
 
 
 def test_pickle():
-    for val in dtypes._registry.values():
+    for val in core.dtypes._registry.values():
         s = pickle.dumps(val)
         val2 = pickle.loads(s)
         if val._is_udt:  # pragma: no cover
             assert val.np_type == val2.np_type
             assert val.name == val2.name
         else:
             assert val == val2
@@ -201,15 +201,15 @@
     rng = np.random.default_rng()
     n = rng.integers(10, 64, endpoint=True)
     np_type = np.dtype(f"({n},)int16")
     assert lookup_dtype(np_type).np_type == np_type
 
 
 def test_default_names():
-    from graphblas.dtypes import _default_name
+    from graphblas.core.dtypes import _default_name
 
     assert _default_name(np.dtype([("x", np.int32), ("y", np.float64)], align=True)) == (
         "{'x': INT32, 'y': FP64}"
     )
     assert _default_name(np.dtype("(29,)uint8")) == "UINT8[29]"
     assert _default_name(np.dtype("(3,4)bool")) == "BOOL[3, 4]"
     assert _default_name(np.dtype((np.dtype("(5,)float64"), (6,)))) == "FP64[5][6]"
@@ -226,17 +226,17 @@
     for c in string.ascii_letters:
         try:
             dtype = np.dtype(c)
             types.append(dtype)
         except Exception:
             pass
     for dtype in types:
-        s = dtypes._dtype_to_string(dtype)
+        s = core.dtypes._dtype_to_string(dtype)
         try:
-            dtype2 = dtypes._string_to_dtype(s)
+            dtype2 = core.dtypes._string_to_dtype(s)
         except Exception:
             with pytest.raises(ValueError, match="Unknown dtype"):
                 lookup_dtype(dtype)
         else:
             assert dtype == dtype2
 
 
@@ -249,7 +249,24 @@
         assert dtypes._supports_complex
         return
 
     import suitesparse_graphblas as ssgb
     from packaging.version import parse
 
     assert dtypes._supports_complex == (parse(ssgb.__version__) >= parse("7.4.3.1"))
+
+
+def test_has_ss_attribute():
+    if suitesparse:
+        assert dtypes.ss is not None
+    else:
+        with pytest.raises(AttributeError):
+            dtypes.ss
+
+
+def test_dir():
+    must_have = {"DataType", "lookup_dtype", "register_anonymous", "register_new", "ss", "unify"}
+    must_have.update({"FP32", "FP64", "INT8", "INT16", "INT32", "INT64"})
+    must_have.update({"BOOL", "UINT8", "UINT16", "UINT32", "UINT64"})
+    if dtypes._supports_complex:
+        must_have.update({"FC32", "FC64"})
+    assert set(dir(dtypes)) & must_have == must_have
```

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_formatting.py` & `python-graphblas-2023.7.0/graphblas/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_infix.py` & `python-graphblas-2023.7.0/graphblas/tests/test_infix.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_io.py` & `python-graphblas-2023.7.0/graphblas/tests/test_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,26 +55,32 @@
     v = Vector.from_dense(a, 0)
     assert v.isequal(gb.Vector.from_coo([1, 2], [2.0, 4.1]), check_dtype=True)
     a2 = v.to_dense(0)
     np.testing.assert_array_equal(a, a2)
 
     csr = gb.io.to_scipy_sparse(v, "csr")
     assert csr.nnz == 2
-    assert ss.isspmatrix_csr(csr)
+    # 2023-06-25: scipy 1.11.0 added `sparray` and changed e.g. `ss.isspmatrix_csr`
+    assert isinstance(csr, getattr(ss, "sparray", ss.spmatrix))
+    assert csr.format == "csr"
     np.testing.assert_array_equal(csr.toarray(), np.array([[0.0, 2.0, 4.1]]))
 
     csc = gb.io.to_scipy_sparse(v, "csc")
     assert csc.nnz == 2
-    assert ss.isspmatrix_csc(csc)
+    # 2023-06-25: scipy 1.11.0 added `sparray` and changed e.g. `ss.isspmatrix_csc`
+    assert isinstance(csc, getattr(ss, "sparray", ss.spmatrix))
+    assert csc.format == "csc"
     np.testing.assert_array_equal(csc.toarray(), np.array([[0.0, 2.0, 4.1]]).T)
 
     # default to csr-like
     coo = gb.io.to_scipy_sparse(v, "coo")
     assert coo.shape == csr.shape
-    assert ss.isspmatrix_coo(coo)
+    # 2023-06-25: scipy 1.11.0 added `sparray` and changed e.g. `ss.isspmatrix_coo`
+    assert isinstance(coo, getattr(ss, "sparray", ss.spmatrix))
+    assert coo.format == "coo"
     assert coo.nnz == 2
     np.testing.assert_array_equal(coo.toarray(), np.array([[0.0, 2.0, 4.1]]))
 
 
 @pytest.mark.skipif("not ss")
 @pytest.mark.parametrize("a", [np.array([7, 0]), np.array([0, 0]), np.array([])])
 def test_vector_to_from_numpy_correct_size(a):
@@ -95,15 +101,17 @@
     M = Matrix.from_dense(a, 0)
     assert M.isequal(gb.Matrix.from_coo([0, 1, 1], [0, 0, 1], [1.0, 2.0, 3.7]), check_dtype=True)
     a2 = M.to_dense(0)
     np.testing.assert_array_equal(a, a2)
 
     for format in ["csr", "csc", "coo"]:
         sparse = gb.io.to_scipy_sparse(M, format)
-        assert getattr(ss, f"isspmatrix_{format}")(sparse)
+        # 2023-06-25: scipy 1.11.0 added `sparray` and changed e.g. `ss.isspmatrix_csr`
+        assert isinstance(sparse, getattr(ss, "sparray", ss.spmatrix))
+        assert sparse.format == format
         assert sparse.nnz == 3
         np.testing.assert_array_equal(sparse.toarray(), a)
         M2 = gb.io.from_scipy_sparse(sparse)
         assert M.isequal(M2, check_dtype=True)
 
     with pytest.raises(ValueError, match="Invalid format"):
         gb.io.to_scipy_sparse(M, "bad format")
@@ -163,15 +171,19 @@
 
 
 @pytest.mark.skipif("not ss")
 @pytest.mark.parametrize("engine", ["auto", "scipy", "fmm"])
 def test_mmread_mmwrite(engine):
     if engine == "fmm" and fmm is None:  # pragma: no cover (import)
         pytest.skip("needs fast_matrix_market")
-    from scipy.io.tests import test_mmio
+    try:
+        from scipy.io.tests import test_mmio
+    except ImportError:
+        # Test files are mysteriously missing from some conda-forge builds
+        pytest.skip("scipy.io.tests.test_mmio unavailable :(")
 
     p31 = 2**31
     p63 = 2**63
     m31 = -p31
     m63 = -p63
     p311 = p31 - 1
     p312 = p31 - 2
@@ -361,14 +373,15 @@
                     assert sa.nnz == M.nvals
                 assert sa.shape == M.shape
                 sa2 = gb.io.to_scipy_sparse(M, fmt)
                 assert (sa != sa2).nnz == 0
 
 
 @pytest.mark.skipif("not ak")
+@pytest.mark.xfail(np.__version__[:5] == "1.25.", reason="awkward bug with numpy 1.25")
 def test_awkward_roundtrip():
     # Vector
     v = gb.Vector.from_coo([1, 3, 5], [20, 21, -5], size=22)
     for dtype in ["int16", "float32", "bool"]:
         v1 = v.dup(dtype=dtype)
         kv = gb.io.to_awkward(v1)
         assert isinstance(kv, ak.Array)
@@ -382,14 +395,15 @@
             km = gb.io.to_awkward(m1, format=format)
             assert isinstance(km, ak.Array)
             m2 = gb.io.from_awkward(km)
             assert m2.isequal(m1)
 
 
 @pytest.mark.skipif("not ak")
+@pytest.mark.xfail(np.__version__[:5] == "1.25.", reason="awkward bug with numpy 1.25")
 def test_awkward_iso_roundtrip():
     # Vector
     v = gb.Vector.from_coo([1, 3, 5], [20, 20, 20], size=22)
     if suitesparse:
         assert v.ss.is_iso
     kv = gb.io.to_awkward(v)
     assert isinstance(kv, ak.Array)
@@ -425,27 +439,29 @@
     with pytest.raises(ValueError, match="Invalid format for Matrix"):
         gb.io.to_awkward(m, format="dcsr")
     with pytest.raises(TypeError):
         gb.io.to_awkward(gb.Scalar.from_value(5))
 
 
 @pytest.mark.skipif("not sparse")
+@pytest.mark.slow
 def test_vector_to_from_pydata_sparse():
     coords = np.array([0, 1, 2, 3, 4], dtype="int64")
     data = np.array([10, 20, 30, 40, 50], dtype="int64")
     s = sparse.COO(coords, data, shape=(5,))
     v = gb.io.from_pydata_sparse(s)
     assert v.isequal(gb.Vector.from_coo(coords, data, dtype=dtypes.INT64), check_dtype=True)
 
     t = gb.io.to_pydata_sparse(v)
     assert t.shape == s.shape
     assert (t == s).all()
 
 
 @pytest.mark.skipif("not sparse")
+@pytest.mark.slow
 def test_matrix_to_from_pydata_sparse():
     coords = np.array([[0, 1, 2, 3, 4], [0, 1, 2, 3, 4]], dtype="int64")
     data = np.array([10, 20, 30, 40, 50], dtype="int64")
     s = sparse.COO(coords, data, shape=(5, 5))
     v = gb.io.from_pydata_sparse(s)
     assert v.isequal(gb.Matrix.from_coo(*coords, data, dtype=dtypes.INT64), check_dtype=False)
```

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_mask.py` & `python-graphblas-2023.7.0/graphblas/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_matrix.py` & `python-graphblas-2023.7.0/graphblas/tests/test_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -4294,15 +4294,15 @@
         C2 = (A @ A).new(nthreads=4, axb_method="dot", sort=True)
         assert C1.isequal(C2)
         C2 = (A @ A).new(Nthreads=4, AxB_method="dot", sort=True)
         assert C1.isequal(C2)
         A(nthreads=4, axb_method="dot", sort=True) << A @ A
         assert A.isequal(C2)
         # Bad option should show list of valid options
-        with pytest.raises(ValueError, match="nthreads"):
+        with pytest.raises(ValueError, match="axb_method"):
             C1(bad_opt=True) << A
         with pytest.raises(ValueError, match="Duplicate descriptor"):
             (A @ A).new(nthreads=4, Nthreads=5)
         with pytest.raises(ValueError, match="escriptor"):
             A[0, 0].new(bad_opt=True)
         A[0, 0].new(nthreads=4, sort=None)  # ignored, but okay
         with pytest.raises(ValueError, match="escriptor"):
```

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_numpyops.py` & `python-graphblas-2023.7.0/graphblas/tests/test_numpyops.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_op.py` & `python-graphblas-2023.7.0/graphblas/tests/test_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     del unary.plus_one["INT8"]
     assert "INT8" not in unary.plus_one
     assert INT8 not in unary.plus_one.types
     with pytest.raises(TypeError, match="UDF argument must be a function"):
         UnaryOp.register_new("bad", object())
     assert not hasattr(unary, "bad")
     with pytest.raises(UdfParseError, match="Unable to parse function using Numba"):
-        UnaryOp.register_new("bad", lambda x: v)
+        UnaryOp.register_new("bad", lambda x: v)  # pragma: no branch (numba)
 
 
 @pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_unaryop_parameterized():
     def plus_x(x=0):
         def inner(val):
@@ -1002,15 +1002,15 @@
         sr = get_semiring(monoid.plus, binary.numpy.copysign)
         assert sr.monoid is monoid.plus
         assert sr.binaryop is binary.numpy.copysign
 
 
 def test_create_semiring():
     # stress test / sanity check
-    monoid_names = {x for x in dir(monoid) if not x.startswith("_")}
+    monoid_names = {x for x in dir(monoid) if not x.startswith("_") and x != "ss"}
     binary_names = {x for x in dir(binary) if not x.startswith("_") and x != "ss"}
     for monoid_name, binary_name in itertools.product(monoid_names, binary_names):
         cur_monoid = getattr(monoid, monoid_name)
         if not isinstance(cur_monoid, Monoid):
             continue
         cur_binary = (
             getattr(binary, binary_name)
@@ -1429,20 +1429,32 @@
         gb.op.secondj
     with pytest.warns(DeprecationWarning, match="please use"):
         gb.agg.argmin
     with pytest.warns(DeprecationWarning, match="please use"):
         import graphblas.core.agg  # noqa: F401
 
 
+@pytest.mark.slow
 def test_is_idempotent():
     assert monoid.min.is_idempotent
     assert monoid.max[int].is_idempotent
     assert monoid.lor.is_idempotent
     assert monoid.band.is_idempotent
     if shouldhave(monoid.numpy, "gcd"):
         assert monoid.numpy.gcd.is_idempotent
     assert not monoid.plus.is_idempotent
     assert not monoid.times[float].is_idempotent
     if config["mapnumpy"] or shouldhave(monoid.numpy, "equal"):
         assert not monoid.numpy.equal.is_idempotent
     with pytest.raises(AttributeError):
         binary.min.is_idempotent
+
+
+def test_ops_have_ss():
+    modules = [unary, binary, monoid, semiring, indexunary, select, op]
+    if suitesparse:
+        for mod in modules:
+            assert mod.ss is not None
+    else:
+        for mod in modules:
+            with pytest.raises(AttributeError):
+                mod.ss
```

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_operator_types.py` & `python-graphblas-2023.7.0/graphblas/tests/test_operator_types.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_pickle.py` & `python-graphblas-2023.7.0/graphblas/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_prefix_scan.py` & `python-graphblas-2023.7.0/graphblas/tests/test_prefix_scan.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_recorder.py` & `python-graphblas-2023.7.0/graphblas/tests/test_recorder.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_resolving.py` & `python-graphblas-2023.7.0/graphblas/tests/test_resolving.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_scalar.py` & `python-graphblas-2023.7.0/graphblas/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_ss_utils.py` & `python-graphblas-2023.7.0/graphblas/tests/test_ss_utils.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/tests/test_vector.py` & `python-graphblas-2023.7.0/graphblas/tests/test_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -854,15 +854,15 @@
     result = v.select(select.register_anonymous(iin, parameterized=True)(2), 2).new()
     assert result.isequal(expected)
     delattr(indexunary, "ii")
     delattr(select, "ii")
     delattr(indexunary, "iin")
     delattr(select, "iin")
     with pytest.raises(UdfParseError, match="Unable to parse function using Numba"):
-        indexunary.register_new("bad", lambda x, row, col, thunk: result)
+        indexunary.register_new("bad", lambda x, row, col, thunk: result)  # pragma: no branch
 
 
 def test_reduce(v):
     s = v.reduce(monoid.plus).new()
     assert s == 4
     assert s.dtype == dtypes.INT64
     assert v.reduce(binary.plus).new() == 4
@@ -1428,15 +1428,15 @@
     expected = Vector.from_coo([0, 1], [20, 10])
     for dtype in ["int8", "uint8", "int16", "uint16", "int32", "uint32"]:
         s1 = Scalar.from_value(1, dtype=dtype)
         assert v[s1].new() == 20
         s0 = Scalar.from_value(0, dtype=dtype)
         w = v[[s1, s0]].new()
         assert w.isequal(expected)
-    for dtype in ["bool", "fp32", "fp64"] + ["fc32", "fc64"] if dtypes._supports_complex else []:
+    for dtype in ["bool", "fp32", "fp64"] + (["fc32", "fc64"] if dtypes._supports_complex else []):
         s = Scalar.from_value(1, dtype=dtype)
         with pytest.raises(TypeError, match="An integer is required for indexing"):
             v[s]
 
 
 @autocompute
 def test_diag(v):
@@ -1444,22 +1444,22 @@
     for k in range(-5, 5):
         size = v.size + abs(k)
         rows = indices + max(0, -k)
         cols = indices + max(0, k)
         expected = Matrix.from_coo(rows, cols, values, nrows=size, ncols=size, dtype=v.dtype)
         # Construct diagonal matrix A
         if suitesparse:
-            A = gb.ss.diag(v, k=k)
+            A = gb.ss.diag(v, k=k, nthreads=2)
             assert expected.isequal(A)
         A = v.diag(k)
         assert expected.isequal(A)
 
         # Extract diagonal from A
         if suitesparse:
-            w = gb.ss.diag(A, Scalar.from_value(k))
+            w = gb.ss.diag(A, Scalar.from_value(k), nthreads=2)
             assert v.isequal(w)
             assert w.dtype == "INT64"
 
             w = gb.ss.diag(A.T, -k, dtype=float)
             assert v.isequal(w)
             assert w.dtype == "FP64"
         w = A.diag(Scalar.from_value(k))
@@ -1733,14 +1733,21 @@
     result = v[:].dup(float, clear=True)
     assert result.isequal(v.dup(float, clear=True), check_dtype=True)
     b = v.dup(bool)
     result = (b | b).dup()
     assert result.isequal(b)
     result = (b | b).dup(clear=True)
     assert result.isequal(b.dup(clear=True))
+    result = v[:5].dup()
+    assert result.isequal(v[:5].new())
+    if suitesparse:
+        result = v[:5].dup(nthreads=2)
+        assert result.isequal(v[:5].new())
+        result = v[:5].dup(clear=True, nthreads=2)
+        assert result.isequal(Vector(v.dtype, size=5))
 
 
 @pytest.mark.skipif("not suitesparse")
 def test_ss_random(v):
     r1 = Vector.from_coo([1], [1], size=v.size)
     r2 = Vector.from_coo([3], [1], size=v.size)
     r3 = Vector.from_coo([4], [2], size=v.size)
@@ -2421,15 +2428,15 @@
     assert result.isequal(expected)
     result = v.ewise_add(v, lambda x, y: x + y).new()  # pragma: no branch (numba)
     assert result.isequal(expected)
     # Should we also allow lambdas for monoids with assumed identity of 0?
     # with pytest.raises(TypeError):
     v.ewise_add(v, lambda x, y: x + y)  # pragma: no branch (numba)
     with pytest.raises(TypeError):
-        v.inner(v, lambda x, y: x + y)
+        v.inner(v, lambda x, y: x + y)  # pragma: no branch (numba)
 
 
 def test_get(v):
     assert compute(v.get(0)) is None
     assert v.get(0, "mittens") == "mittens"
     assert v.get(1) == 1
     assert v.get(1, "mittens") == 1
```

### Comparing `python-graphblas-2023.5.0/graphblas/unary/__init__.py` & `python-graphblas-2023.7.0/graphblas/unary/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/unary/numpy.py` & `python-graphblas-2023.7.0/graphblas/unary/numpy.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.5.0/graphblas/viz.py` & `python-graphblas-2023.7.0/graphblas/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
             val = globals()[name]
         else:
             try:
                 val = _import_module(_LAZY_IMPORTS[name])
             except ImportError:
                 modname = _LAZY_IMPORTS[name].split(".")[0]
                 raise ImportError(f"`{within}` requires {modname} to be installed") from None
-            finally:
-                globals()[name] = val
+            globals()[name] = val
         rv.append(val)
     if is_string:
         return rv[0]
     return rv
 
 
 def draw(m):  # pragma: no cover
@@ -63,15 +62,15 @@
     edge_labels = {(i, j): d["weight"] for i, j, d in g.edges(data=True)}
     nx.draw_networkx(g, pos, node_color="red", node_size=500)
     nx.draw_networkx_edge_labels(g, pos, edge_labels=edge_labels)
     plt.show()
 
 
 def spy(M, *, centered=False, show=True, figure=None, axes=None, figsize=None, **kwargs):
-    """Plot the sparsity pattern of a Matrix using `matplotlib.spy`.
+    """Plot the sparsity pattern of a Matrix using ``matplotlib.spy``.
 
     See:
     - https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.spy.html
     - https://matplotlib.org/stable/gallery/images_contours_and_fields/spy_demos.html
 
     By default, this function automatically calculates markersize to properly tile
     the sparsity pattern.  That is, the square plotted for a visible element abuts
@@ -102,16 +101,16 @@
         axes.set_yticks(axes.get_yticks()[1:-1] - 0.5, axes.get_yticklabels()[1:-1])
     return axes.figure
 
 
 def datashade(M, agg="count", *, width=None, height=None, opts_kwargs=None, **kwargs):
     """Interactive plot of the sparsity pattern of a Matrix using hvplot and datashader.
 
-    The `datashader` library rasterizes large data into a 2d grid of pixels.  Each pixel
-    may contain multiple data points, which are combined by an aggregator (`agg="count"`).
+    The ``datashader`` library rasterizes large data into a 2d grid of pixels.  Each pixel
+    may contain multiple data points, which are combined by an aggregator (``agg="count"``).
     Common aggregators are "count", "sum", "mean", "min", and "max".  See full list here:
     - https://datashader.org/api.html#reductions
 
     Multiple aggregators may be given to create a grid of linked plots.  For example,
 
     >>> datashade(A, agg=[["count", "sum"], ["min", "max"]])
```

### Comparing `python-graphblas-2023.5.0/pyproject.toml` & `python-graphblas-2023.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 packages = [
     "graphblas",
     "graphblas.agg",
     "graphblas.binary",
     "graphblas.core",
     "graphblas.core.operator",
     "graphblas.core.ss",
+    "graphblas.dtypes",
     "graphblas.indexunary",
     "graphblas.io",
     "graphblas.monoid",
     "graphblas.op",
     "graphblas.semiring",
     "graphblas.select",
     "graphblas.ss",
@@ -164,38 +165,51 @@
 skip_gitignore = true
 float_to_top = true
 default_section = "THIRDPARTY"
 known_first_party = "graphblas"
 line_length = 100
 
 [tool.pytest.ini_options]
+minversion = "6.0"
 testpaths = "graphblas/tests"
-xfail_strict = true
+xfail_strict = false  # 2023-07-23: awkward and numpy 1.25 sometimes conflict
+addopts = [
+    "--strict-config",  # Force error if config is mispelled
+    "--strict-markers",  # Force error if marker is mispelled (must be defined in config)
+    "-ra",  # Print summary of all fails/errors
+]
 markers = [
     "slow: Skipped unless --runslow passed",
 ]
+log_cli_level = "info"
 filterwarnings = [
     # See: https://docs.python.org/3/library/warnings.html#describing-warning-filters
     # and: https://docs.pytest.org/en/7.2.x/how-to/capture-warnings.html#controlling-warnings
     "error",
+
     # sparse 0.14.0 (2022-02-24) began raising this warning; it has been reported and fixed upstream.
     "ignore:coords should be an ndarray. This will raise a ValueError:DeprecationWarning:sparse._coo.core",
 
     # setuptools v67.3.0 deprecated `pkg_resources.declare_namespace` on 13 Feb 2023. See:
     # https://setuptools.pypa.io/en/latest/history.html#v67-3-0
     # MAINT: check if this is still necessary in 2025
     "ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning:pkg_resources",
-    # And this deprecation warning was added in setuptools v67.5.0 (8 Mar 2023). See:
+
+    # This deprecation warning was added in setuptools v67.5.0 (8 Mar 2023). See:
     # https://setuptools.pypa.io/en/latest/history.html#v67-5-0
-    "ignore:pkg_resources is deprecated as an API:DeprecationWarning:pkg_resources",
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning:",
 
     # sre_parse deprecated in 3.11; this is triggered by awkward 0.10
     "ignore:module 'sre_parse' is deprecated:DeprecationWarning:",
     "ignore:module 'sre_constants' is deprecated:DeprecationWarning:",
 
+    # numpy 1.25.0 (2023-06-17) deprecated `np.find_common_type`; many other dependencies use it.
+    # See if we can remove this filter in 2025.
+    "ignore:np.find_common_type is deprecated:DeprecationWarning:",
+
     # pypy gives this warning
     "ignore:can't resolve package from __spec__ or __package__:ImportWarning:",
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["graphblas"]
@@ -294,25 +308,30 @@
     "PLE0605",  # Invalid format for `__all__`, must be `tuple` or `list` (Note: broken in v0.0.237)
 
     # Maybe consider
     # "SIM300",  # Yoda conditions are discouraged, use ... instead (Note: we're not this picky)
     # "SIM401",  # Use dict.get ... instead of if-else-block (Note: if-else better for coverage and sometimes clearer)
     "TRY004",  # Prefer `TypeError` exception for invalid type (Note: good advice, but not worth the nuisance)
     "TRY200",  # Use `raise from` to specify exception cause (Note: sometimes okay to raise original exception)
+    "RUF012",  # Mutable class attributes should be annotated with `typing.ClassVar` (Note: no annotations yet)
+    "PERF401",  # Use a list comprehension to create a transformed list (Note: poorly implemented atm)
 
     # Intentionally ignored
     "COM812",  # Trailing comma missing
     "D203",  # 1 blank line required before class docstring (Note: conflicts with D211, which is preferred)
     "D400",  # First line should end with a period (Note: prefer D415, which also allows "?" and "!")
     "N801",  # Class name ... should use CapWords convention (Note:we have a few exceptions to this)
     "N802",  # Function name ... should be lowercase
     "N803",  # Argument name ... should be lowercase (Maybe okay--except in tests)
     "N806",  # Variable ... in function should be lowercase
     "N807",  # Function name should not start and end with `__`
     "N818",  # Exception name ... should be named with an Error suffix (Note: good advice)
+    "PERF203",  # `try`-`except` within a loop incurs performance overhead (Note: too strict)
+    "PLC0205",  # Class `__slots__` should be a non-string iterable (Note: string is fine)
+    "PLR0124", # Name compared with itself, consider replacing `x == x` (Note: too strict)
     "PLR0911",  # Too many return statements
     "PLR0912",  # Too many branches
     "PLR0913",  # Too many arguments to function call
     "PLR0915",  # Too many statements
     "PLR2004",  # Magic number used in comparison, consider replacing magic with a constant variable
     "PLW0603",  # Using the global statement to update ... is discouraged (Note: yeah, discouraged, but too strict)
     "PLW2901",  # Outer for loop variable ... overwritten by inner assignment target (Note: good advice, but too strict)
@@ -338,14 +357,16 @@
     "EM",  # flake8-errmsg (Perhaps nicer, but too much work)
     "ICN",  # flake8-import-conventions (Doesn't allow "_" prefix such as `_np`)
     "PYI",  # flake8-pyi (We don't have stub files yet)
     "SLF",  # flake8-self (We can use our own private variables--sheesh!)
     "TID",  # flake8-tidy-imports (Rely on isort and our own judgement)
     "TCH",  # flake8-type-checking (Note: figure out type checking later)
     "ARG",  # flake8-unused-arguments (Sometimes helpful, but too strict)
+    "TD",  # flake8-todos (Maybe okay to add some of these)
+    "FIX",  # flake8-fixme (like flake8-todos)
     "ERA",  # eradicate (We like code in comments!)
     "PD",  # pandas-vet (Intended for scripts that use pandas, not libraries)
 ]
 
 [tool.ruff.per-file-ignores]
 "graphblas/core/agg.py" = ["F401", "F403"]  # Deprecated
 "graphblas/core/operator/base.py" = ["S102"]  # exec is used for UDF
```

### Comparing `python-graphblas-2023.5.0/python_graphblas.egg-info/PKG-INFO` & `python-graphblas-2023.7.0/python_graphblas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-graphblas
-Version: 2023.5.0
+Version: 2023.7.0
 Summary: Python library for GraphBLAS: high-performance sparse linear algebra for scalable graph analytics
 Author: Jim Kitchen, Python-graphblas contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>, Sultan Orazbayev <contact@econpoint.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -189,15 +189,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright 2020 Anaconda, Inc
+           Copyright 2020-2023 Anaconda, Inc. and contributors
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
@@ -244,15 +244,15 @@
 Provides-Extra: viz
 Provides-Extra: datashade
 Provides-Extra: test
 Provides-Extra: default
 Provides-Extra: all
 License-File: LICENSE
 
-![Python-graphblas](docs/_static/img/logo-name-medium.svg)
+![Python-graphblas](https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/logo-name-medium.svg)
 
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/python-graphblas.svg)](https://anaconda.org/conda-forge/python-graphblas)
 [![pypi](https://img.shields.io/pypi/v/python-graphblas.svg)](https://pypi.python.org/pypi/python-graphblas/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)](https://pypi.python.org/pypi/python-graphblas/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/python-graphblas/blob/main/LICENSE)
 <br>
 [![Tests](https://github.com/python-graphblas/python-graphblas/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/python-graphblas/actions)
@@ -274,16 +274,16 @@
 - **Source:** [https://github.com/python-graphblas/python-graphblas](https://github.com/python-graphblas/python-graphblas)
 - **Bug reports:** [https://github.com/python-graphblas/python-graphblas/issues](https://github.com/python-graphblas/python-graphblas/issues)
 - **Github discussions:** [https://github.com/python-graphblas/python-graphblas/discussions](https://github.com/python-graphblas/python-graphblas/discussions)
 - **Weekly community call:** [https://github.com/python-graphblas/python-graphblas/issues/247](https://github.com/python-graphblas/python-graphblas/issues/247)
 - **Chat via Discord:** [https://discord.com/invite/vur45CbwMz](https://discord.com/invite/vur45CbwMz) in the [#graphblas channel](https://discord.com/channels/786703927705862175/1024732940233605190)
 
 <p float="left">
-  <img src="docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
-  <img src="docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
+  <img src="https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
+  <img src="https://raw.githubusercontent.com/python-graphblas/python-graphblas/main/docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
 </p>
 
 ## Install
 Install the latest version of Python-graphblas via conda:
 ```
 $ conda install -c conda-forge python-graphblas
 ```
@@ -422,16 +422,17 @@
 ```
 ## Initialization
 There is a mechanism to initialize `graphblas` with a context prior to use. This allows for setting the backend to
 use as well as the blocking/non-blocking mode. If the context is not initialized, a default initialization will
 be performed automatically.
 ```python
 import graphblas as gb
+
 # Context initialization must happen before any other imports
-gb.init('suitesparse', blocking=True)
+gb.init("suitesparse", blocking=True)
 
 # Now we can import other items from graphblas
 from graphblas import binary, semiring
 from graphblas import Matrix, Vector, Scalar
 ```
 ## Performant User Defined Functions
 Python-graphblas requires `numba` which enables compiling user-defined Python functions to native C for use in GraphBLAS.
@@ -441,30 +442,46 @@
 from graphblas import unary
 
 def force_odd_func(x):
     if x % 2 == 0:
         return x + 1
     return x
 
-unary.register_new('force_odd', force_odd_func)
+unary.register_new("force_odd", force_odd_func)
 
 v = Vector.from_coo([0, 1, 3], [1, 2, 3])
 w = v.apply(unary.force_odd).new()
 w  # indexes=[0, 1, 3], values=[1, 3, 3]
 ```
 Similar methods exist for BinaryOp, Monoid, and Semiring.
 
+## Relation to other network analysis libraries
+Python-graphblas aims to provide an efficient and consistent expression
+of graph operations using linear algebra. This allows the development of
+high-performance implementations of existing and new graph algorithms
+(also see [`graphblas-algorithms`](https://github.com/python-graphblas/graphblas-algorithms)).
+
+While end-to-end analysis can be done using `python-graphblas`, users
+might find that other libraries in the Python ecosystem provide a more
+convenient high-level interface for data pre-processing and transformation
+(e.g. `pandas`, `scipy.sparse`), visualization (e.g. `networkx`, `igraph`),
+interactive exploration and analysis (e.g. `networkx`, `igraph`) or for
+algorithms that are not (yet) implemented in `graphblas-algorithms` (e.g.
+`networkx`, `igraph`, `scipy.sparse.csgraph`). To facilitate communication with
+other libraries, `graphblas.io` contains multiple connectors, see the
+following section.
+
 ## Import/Export connectors to the Python ecosystem
 `graphblas.io` contains functions for converting to and from:
 ```python
 import graphblas as gb
 
 # scipy.sparse matrices
 A = gb.io.from_scipy_sparse(m)
-m = gb.io.to_scipy_sparse(m, format='csr')
+m = gb.io.to_scipy_sparse(m, format="csr")
 
 # networkx graphs
 A = gb.io.from_networkx(g)
 g = gb.io.to_networkx(A)
 
 # numpy arrays can use `from_dense` and `to_dense` on Vector and Matrix
 v = gb.Vector.from_dense(m)
```

### Comparing `python-graphblas-2023.5.0/python_graphblas.egg-info/SOURCES.txt` & `python-graphblas-2023.7.0/python_graphblas.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 LICENSE
 MANIFEST.in
 README.md
+conftest.py
 pyproject.toml
 setup.py
-docs/_static/img/draw-example.png
-docs/_static/img/logo-name-medium.svg
-docs/_static/img/repr-matrix.png
 graphblas/__init__.py
-graphblas/dtypes.py
 graphblas/exceptions.py
 graphblas/graphblas.yaml
 graphblas/viz.py
 graphblas/agg/__init__.py
 graphblas/agg/ss.py
 graphblas/binary/__init__.py
 graphblas/binary/numpy.py
 graphblas/binary/ss.py
 graphblas/core/__init__.py
 graphblas/core/agg.py
 graphblas/core/automethods.py
 graphblas/core/base.py
 graphblas/core/descriptor.py
+graphblas/core/dtypes.py
 graphblas/core/expr.py
 graphblas/core/formatting.py
 graphblas/core/infix.py
 graphblas/core/infixmethods.py
 graphblas/core/mask.py
 graphblas/core/matrix.py
 graphblas/core/recorder.py
@@ -39,34 +37,45 @@
 graphblas/core/operator/indexunary.py
 graphblas/core/operator/monoid.py
 graphblas/core/operator/select.py
 graphblas/core/operator/semiring.py
 graphblas/core/operator/unary.py
 graphblas/core/operator/utils.py
 graphblas/core/ss/__init__.py
+graphblas/core/ss/binary.py
 graphblas/core/ss/config.py
+graphblas/core/ss/context.py
 graphblas/core/ss/descriptor.py
+graphblas/core/ss/dtypes.py
+graphblas/core/ss/indexunary.py
 graphblas/core/ss/matrix.py
 graphblas/core/ss/prefix_scan.py
+graphblas/core/ss/select.py
+graphblas/core/ss/unary.py
 graphblas/core/ss/vector.py
+graphblas/dtypes/__init__.py
+graphblas/dtypes/ss.py
 graphblas/indexunary/__init__.py
+graphblas/indexunary/ss.py
 graphblas/io/__init__.py
 graphblas/io/_awkward.py
 graphblas/io/_matrixmarket.py
 graphblas/io/_networkx.py
 graphblas/io/_numpy.py
 graphblas/io/_scipy.py
 graphblas/io/_sparse.py
 graphblas/io/_viz.py
 graphblas/monoid/__init__.py
 graphblas/monoid/numpy.py
+graphblas/monoid/ss.py
 graphblas/op/__init__.py
 graphblas/op/numpy.py
 graphblas/op/ss.py
 graphblas/select/__init__.py
+graphblas/select/ss.py
 graphblas/semiring/__init__.py
 graphblas/semiring/numpy.py
 graphblas/semiring/ss.py
 graphblas/ss/__init__.py
 graphblas/ss/_core.py
 graphblas/tests/__init__.py
 graphblas/tests/conftest.py
@@ -91,14 +100,15 @@
 graphblas/tests/test_operator_types.py
 graphblas/tests/test_pickle.py
 graphblas/tests/test_prefix_scan.py
 graphblas/tests/test_recorder.py
 graphblas/tests/test_resolving.py
 graphblas/tests/test_scalar.py
 graphblas/tests/test_ss_utils.py
+graphblas/tests/test_ssjit.py
 graphblas/tests/test_vector.py
 graphblas/unary/__init__.py
 graphblas/unary/numpy.py
 graphblas/unary/ss.py
 python_graphblas.egg-info/PKG-INFO
 python_graphblas.egg-info/SOURCES.txt
 python_graphblas.egg-info/dependency_links.txt
```

### Comparing `python-graphblas-2023.5.0/python_graphblas.egg-info/requires.txt` & `python-graphblas-2023.7.0/python_graphblas.egg-info/requires.txt`

 * *Files identical despite different names*

