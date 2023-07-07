# Comparing `tmp/pyhard-2.1.8.tar.gz` & `tmp/pyhard-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhard-2.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyhard-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyhard-2.1.8.tar` & `pyhard-2.2.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0     8692 2023-07-04 03:21:03.698911 pyhard-2.1.8/README.md
--rw-r--r--   0        0        0     1297 2023-07-04 03:21:03.768911 pyhard-2.1.8/pyhard/__init__.py
--rw-r--r--   0        0        0       66 2023-07-04 03:21:03.768911 pyhard-2.1.8/pyhard/__main__.py
--rw-r--r--   0        0        0    37751 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/app.py
--rw-r--r--   0        0        0    19119 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/base.py
--rw-r--r--   0        0        0    12128 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/classification.py
--rw-r--r--   0        0        0    20574 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/cli.py
--rw-r--r--   0        0        0     5199 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/conf/config.yaml
--rw-r--r--   0        0        0     3469 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/conf/config_old.yaml
--rw-r--r--   0        0        0      703 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/conf/options.json
--rw-r--r--   0        0        0    12210 2023-07-04 03:21:03.769911 pyhard-2.1.8/pyhard/context.py
--rw-r--r--   0        0        0    64554 2023-07-04 03:21:03.770911 pyhard-2.1.8/pyhard/data/2normals/2normals.pdf
--rw-r--r--   0        0        0    39390 2023-07-04 03:21:03.770911 pyhard-2.1.8/pyhard/data/2normals/coordinates.csv
--rw-r--r--   0        0        0    39209 2023-07-04 03:21:03.770911 pyhard-2.1.8/pyhard/data/2normals/data.csv
--rw-r--r--   0        0        0   242683 2023-07-04 03:21:03.771911 pyhard-2.1.8/pyhard/data/2normals/feature_process.csv
--rw-r--r--   0        0        0   168248 2023-07-04 03:21:03.772911 pyhard-2.1.8/pyhard/data/2normals/feature_raw.csv
--rw-r--r--   0        0        0   328455 2023-07-04 03:21:03.773911 pyhard-2.1.8/pyhard/data/2normals/metadata.csv
--rw-r--r--   0        0        0      598 2023-07-04 03:21:03.773911 pyhard-2.1.8/pyhard/data/2normals/options.json
--rw-r--r--   0        0        0    64659 2023-07-04 03:21:03.774911 pyhard-2.1.8/pyhard/data/2normalsSd030/2normals030.pdf
--rw-r--r--   0        0        0    39624 2023-07-04 03:21:03.774911 pyhard-2.1.8/pyhard/data/2normalsSd030/coordinates.csv
--rw-r--r--   0        0        0    38990 2023-07-04 03:21:03.774911 pyhard-2.1.8/pyhard/data/2normalsSd030/data.csv
--rw-r--r--   0        0        0   130100 2023-07-04 03:21:03.775911 pyhard-2.1.8/pyhard/data/2normalsSd030/feature_process.csv
--rw-r--r--   0        0        0    94130 2023-07-04 03:21:03.775911 pyhard-2.1.8/pyhard/data/2normalsSd030/feature_raw.csv
--rw-r--r--   0        0        0   284473 2023-07-04 03:21:03.776911 pyhard-2.1.8/pyhard/data/2normalsSd030/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-04 03:21:03.776911 pyhard-2.1.8/pyhard/data/2normalsSd030/options.json
--rw-r--r--   0        0        0    64807 2023-07-04 03:21:03.777911 pyhard-2.1.8/pyhard/data/2normalsSd045/2normals045.pdf
--rw-r--r--   0        0        0    39780 2023-07-04 03:21:03.777911 pyhard-2.1.8/pyhard/data/2normalsSd045/coordinates.csv
--rw-r--r--   0        0        0    39157 2023-07-04 03:21:03.777911 pyhard-2.1.8/pyhard/data/2normalsSd045/data.csv
--rw-r--r--   0        0        0   178828 2023-07-04 03:21:03.778911 pyhard-2.1.8/pyhard/data/2normalsSd045/feature_process.csv
--rw-r--r--   0        0        0   131886 2023-07-04 03:21:03.778911 pyhard-2.1.8/pyhard/data/2normalsSd045/feature_raw.csv
--rw-r--r--   0        0        0   318453 2023-07-04 03:21:03.780911 pyhard-2.1.8/pyhard/data/2normalsSd045/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-04 03:21:03.780911 pyhard-2.1.8/pyhard/data/2normalsSd045/options.json
--rw-r--r--   0        0        0    15846 2023-07-04 03:21:03.780911 pyhard-2.1.8/pyhard/data/circle/circle.png
--rw-r--r--   0        0        0    39346 2023-07-04 03:21:03.780911 pyhard-2.1.8/pyhard/data/circle/coordinates.csv
--rw-r--r--   0        0        0    40231 2023-07-04 03:21:03.781911 pyhard-2.1.8/pyhard/data/circle/data.csv
--rw-r--r--   0        0        0   226405 2023-07-04 03:21:03.782911 pyhard-2.1.8/pyhard/data/circle/feature_process.csv
--rw-r--r--   0        0        0   145447 2023-07-04 03:21:03.783911 pyhard-2.1.8/pyhard/data/circle/feature_raw.csv
--rw-r--r--   0        0        0   320526 2023-07-04 03:21:03.784911 pyhard-2.1.8/pyhard/data/circle/metadata.csv
--rw-r--r--   0        0        0      595 2023-07-04 03:21:03.784911 pyhard-2.1.8/pyhard/data/circle/options.json
--rw-r--r--   0        0        0    40190 2023-07-04 03:21:03.784911 pyhard-2.1.8/pyhard/data/easy/coordinates.csv
--rw-r--r--   0        0        0    40952 2023-07-04 03:21:03.785911 pyhard-2.1.8/pyhard/data/easy/data.csv
--rw-r--r--   0        0        0   147238 2023-07-04 03:21:03.785911 pyhard-2.1.8/pyhard/data/easy/feature_process.csv
--rw-r--r--   0        0        0    54473 2023-07-04 03:21:03.785911 pyhard-2.1.8/pyhard/data/easy/feature_raw_color.csv
--rw-r--r--   0        0        0   282881 2023-07-04 03:21:03.787911 pyhard-2.1.8/pyhard/data/easy/metadata.csv
--rw-r--r--   0        0        0      595 2023-07-04 03:21:03.787911 pyhard-2.1.8/pyhard/data/easy/options.json
--rw-r--r--   0        0        0    39957 2023-07-04 03:21:03.787911 pyhard-2.1.8/pyhard/data/easy2/coordinates.csv
--rw-r--r--   0        0        0    40817 2023-07-04 03:21:03.787911 pyhard-2.1.8/pyhard/data/easy2/data.csv
--rw-r--r--   0        0        0    42676 2023-07-04 03:21:03.787911 pyhard-2.1.8/pyhard/data/easy2/easy2.png
--rw-r--r--   0        0        0   285261 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/easy2/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/easy2/options.json
--rw-r--r--   0        0        0      190 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/easy2/projection_matrix.csv
--rw-r--r--   0        0        0     5787 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/iris/coordinates.csv
--rw-r--r--   0        0        0     3877 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/iris/data.csv
--rw-r--r--   0        0        0    42802 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/iris/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/iris/options.json
--rw-r--r--   0        0        0    39716 2023-07-04 03:21:03.789911 pyhard-2.1.8/pyhard/data/mix/coordinates.csv
--rw-r--r--   0        0        0    40903 2023-07-04 03:21:03.790911 pyhard-2.1.8/pyhard/data/mix/data.csv
--rw-r--r--   0        0        0   193499 2023-07-04 03:21:03.790911 pyhard-2.1.8/pyhard/data/mix/feature_process.csv
--rw-r--r--   0        0        0   144369 2023-07-04 03:21:03.791911 pyhard-2.1.8/pyhard/data/mix/feature_raw.csv
--rw-r--r--   0        0        0   296920 2023-07-04 03:21:03.792911 pyhard-2.1.8/pyhard/data/mix/metadata.csv
--rw-r--r--   0        0        0    66400 2023-07-04 03:21:03.792911 pyhard-2.1.8/pyhard/data/mix/mix.png
--rw-r--r--   0        0        0      597 2023-07-04 03:21:03.792911 pyhard-2.1.8/pyhard/data/mix/options.json
--rw-r--r--   0        0        0    39233 2023-07-04 03:21:03.793911 pyhard-2.1.8/pyhard/data/overlap/coordinates.csv
--rw-r--r--   0        0        0    39752 2023-07-04 03:21:03.793911 pyhard-2.1.8/pyhard/data/overlap/data.csv
--rw-r--r--   0        0        0   321095 2023-07-04 03:21:03.794911 pyhard-2.1.8/pyhard/data/overlap/metadata.csv
--rw-r--r--   0        0        0      598 2023-07-04 03:21:03.794911 pyhard-2.1.8/pyhard/data/overlap/options.json
--rw-r--r--   0        0        0    13099 2023-07-04 03:21:03.794911 pyhard-2.1.8/pyhard/data/overlap/overlap.png
--rw-r--r--   0        0        0    39995 2023-07-04 03:21:03.795911 pyhard-2.1.8/pyhard/data/separate/coordinates.csv
--rw-r--r--   0        0        0    42167 2023-07-04 03:21:03.795911 pyhard-2.1.8/pyhard/data/separate/data.csv
--rw-r--r--   0        0        0   177556 2023-07-04 03:21:03.795911 pyhard-2.1.8/pyhard/data/separate/feature_process.csv
--rw-r--r--   0        0        0   113525 2023-07-04 03:21:03.796911 pyhard-2.1.8/pyhard/data/separate/feature_raw.csv
--rw-r--r--   0        0        0   287283 2023-07-04 03:21:03.797911 pyhard-2.1.8/pyhard/data/separate/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-04 03:21:03.797911 pyhard-2.1.8/pyhard/data/separate/options.json
--rw-r--r--   0        0        0    29361 2023-07-04 03:21:03.797911 pyhard-2.1.8/pyhard/data/wine/algorithm_bin.csv
--rw-r--r--   0        0        0   226327 2023-07-04 03:21:03.798911 pyhard-2.1.8/pyhard/data/wine/algorithm_process.csv
--rw-r--r--   0        0        0   218520 2023-07-04 03:21:03.799911 pyhard-2.1.8/pyhard/data/wine/algorithm_raw.csv
--rw-r--r--   0        0        0    10101 2023-07-04 03:21:03.799911 pyhard-2.1.8/pyhard/data/wine/beta_easy.csv
--rw-r--r--   0        0        0     4375 2023-07-04 03:21:03.799911 pyhard-2.1.8/pyhard/data/wine/config.yaml
--rw-r--r--   0        0        0    69563 2023-07-04 03:21:03.799911 pyhard-2.1.8/pyhard/data/wine/coordinates.csv
--rw-r--r--   0        0        0   100951 2023-07-04 03:21:03.800911 pyhard-2.1.8/pyhard/data/wine/data.csv
--rw-r--r--   0        0        0   163688 2023-07-04 03:21:03.801911 pyhard-2.1.8/pyhard/data/wine/feature_process.csv
--rw-r--r--   0        0        0   163380 2023-07-04 03:21:03.801911 pyhard-2.1.8/pyhard/data/wine/feature_raw.csv
--rw-r--r--   0        0        0       12 2023-07-04 03:21:03.801911 pyhard-2.1.8/pyhard/data/wine/footprint_bagging_best.csv
--rw-r--r--   0        0        0     1634 2023-07-04 03:21:03.801911 pyhard-2.1.8/pyhard/data/wine/footprint_bagging_good.csv
--rw-r--r--   0        0        0      174 2023-07-04 03:21:03.801911 pyhard-2.1.8/pyhard/data/wine/footprint_gradient_boosting_best.csv
--rw-r--r--   0        0        0     1726 2023-07-04 03:21:03.801911 pyhard-2.1.8/pyhard/data/wine/footprint_gradient_boosting_good.csv
--rw-r--r--   0        0        0      720 2023-07-04 03:21:03.801911 pyhard-2.1.8/pyhard/data/wine/footprint_instance_easiness_good.csv
--rw-r--r--   0        0        0       12 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_logistic_regression_best.csv
--rw-r--r--   0        0        0     1696 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_logistic_regression_good.csv
--rw-r--r--   0        0        0       12 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_mlp_best.csv
--rw-r--r--   0        0        0     1663 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_mlp_good.csv
--rw-r--r--   0        0        0      893 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_performance.csv
--rw-r--r--   0        0        0     2760 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_random_forest_best.csv
--rw-r--r--   0        0        0     1903 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_random_forest_good.csv
--rw-r--r--   0        0        0      259 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_svc_linear_best.csv
--rw-r--r--   0        0        0     1434 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_svc_linear_good.csv
--rw-r--r--   0        0        0       12 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_svc_rbf_best.csv
--rw-r--r--   0        0        0     1516 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/footprint_svc_rbf_good.csv
--rw-r--r--   0        0        0    10103 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/good_algos.csv
--rw-r--r--   0        0        0    37458 2023-07-04 03:21:03.802911 pyhard-2.1.8/pyhard/data/wine/ih.csv
--rw-r--r--   0        0        0   317680 2023-07-04 03:21:03.803911 pyhard-2.1.8/pyhard/data/wine/metadata.csv
--rw-r--r--   0        0        0   522841 2023-07-04 03:21:03.805911 pyhard-2.1.8/pyhard/data/wine/metadata_full.csv
--rw-r--r--   0        0        0   409402 2023-07-04 03:21:03.807911 pyhard-2.1.8/pyhard/data/wine/model.pkl
--rw-r--r--   0        0        0      790 2023-07-04 03:21:03.807911 pyhard-2.1.8/pyhard/data/wine/options.json
--rw-r--r--   0        0        0    10105 2023-07-04 03:21:03.807911 pyhard-2.1.8/pyhard/data/wine/portfolio.csv
--rw-r--r--   0        0        0      231 2023-07-04 03:21:03.807911 pyhard-2.1.8/pyhard/data/wine/projection_matrix.csv
--rw-r--r--   0        0        0    40143 2023-07-04 03:21:03.808911 pyhard-2.1.8/pyhard/data/xor/coordinates.csv
--rw-r--r--   0        0        0    40214 2023-07-04 03:21:03.808911 pyhard-2.1.8/pyhard/data/xor/data.csv
--rw-r--r--   0        0        0   272866 2023-07-04 03:21:03.809911 pyhard-2.1.8/pyhard/data/xor/metadata.csv
--rw-r--r--   0        0        0      598 2023-07-04 03:21:03.809911 pyhard-2.1.8/pyhard/data/xor/options.json
--rw-r--r--   0        0        0      196 2023-07-04 03:21:03.809911 pyhard-2.1.8/pyhard/data/xor/projection_matrix.csv
--rw-r--r--   0        0        0    65163 2023-07-04 03:21:03.809911 pyhard-2.1.8/pyhard/data/xor/xor.pdf
--rw-r--r--   0        0        0     7659 2023-07-04 03:21:03.809911 pyhard-2.1.8/pyhard/feature_selection.py
--rw-r--r--   0        0        0    10144 2023-07-04 03:21:03.811911 pyhard-2.1.8/pyhard/hpo.py
--rw-r--r--   0        0        0    10847 2023-07-04 03:21:03.811911 pyhard-2.1.8/pyhard/integrator.py
--rw-r--r--   0        0        0    43027 2023-07-04 03:21:03.811911 pyhard-2.1.8/pyhard/measures.py
--rw-r--r--   0        0        0     3787 2023-07-04 03:21:03.811911 pyhard-2.1.8/pyhard/metrics.py
--rw-r--r--   0        0        0   157445 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/midia/blobs.svg
--rw-r--r--   0        0        0    11042 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/regression.py
--rw-r--r--   0        0        0     4123 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/structures.py
--rw-r--r--   0        0        0        0 2023-07-04 03:21:03.843911 pyhard-2.1.8/pyhard/thirdparty/__init__.py
--rwxr-xr-x   0        0        0    10787 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/thirdparty/entropy_estimators.py
--rw-r--r--   0        0        0     4948 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/thirdparty/rank_aggregation.py
--rw-r--r--   0        0        0    21966 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/thirdparty/skfeature.py
--rw-r--r--   0        0        0     5221 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/utils.py
--rw-r--r--   0        0        0     2359 2023-07-04 03:21:03.812911 pyhard-2.1.8/pyhard/validator.py
--rw-r--r--   0        0        0    38600 2023-07-04 03:21:03.813911 pyhard-2.1.8/pyhard/visualization.py
--rw-r--r--   0        0        0     1574 2023-07-04 03:21:03.813911 pyhard-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    10244 1970-01-01 00:00:00.000000 pyhard-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     8692 2023-07-07 15:38:37.949955 pyhard-2.2.0/README.md
+-rw-r--r--   0        0        0     1297 2023-07-07 15:38:38.023956 pyhard-2.2.0/pyhard/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-07 15:38:38.023956 pyhard-2.2.0/pyhard/__main__.py
+-rw-r--r--   0        0        0    38272 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/app.py
+-rw-r--r--   0        0        0    19119 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/base.py
+-rw-r--r--   0        0        0    12613 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/classification.py
+-rw-r--r--   0        0        0    20574 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/cli.py
+-rw-r--r--   0        0        0     5199 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/conf/config.yaml
+-rw-r--r--   0        0        0     3469 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/conf/config_old.yaml
+-rw-r--r--   0        0        0      703 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/conf/options.json
+-rw-r--r--   0        0        0    12210 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/context.py
+-rw-r--r--   0        0        0    64554 2023-07-07 15:38:38.025956 pyhard-2.2.0/pyhard/data/2normals/2normals.pdf
+-rw-r--r--   0        0        0    39390 2023-07-07 15:38:38.025956 pyhard-2.2.0/pyhard/data/2normals/coordinates.csv
+-rw-r--r--   0        0        0    39209 2023-07-07 15:38:38.025956 pyhard-2.2.0/pyhard/data/2normals/data.csv
+-rw-r--r--   0        0        0   242683 2023-07-07 15:38:38.026956 pyhard-2.2.0/pyhard/data/2normals/feature_process.csv
+-rw-r--r--   0        0        0   168248 2023-07-07 15:38:38.027956 pyhard-2.2.0/pyhard/data/2normals/feature_raw.csv
+-rw-r--r--   0        0        0   328455 2023-07-07 15:38:38.028956 pyhard-2.2.0/pyhard/data/2normals/metadata.csv
+-rw-r--r--   0        0        0      598 2023-07-07 15:38:38.028956 pyhard-2.2.0/pyhard/data/2normals/options.json
+-rw-r--r--   0        0        0    64659 2023-07-07 15:38:38.028956 pyhard-2.2.0/pyhard/data/2normalsSd030/2normals030.pdf
+-rw-r--r--   0        0        0    39624 2023-07-07 15:38:38.029956 pyhard-2.2.0/pyhard/data/2normalsSd030/coordinates.csv
+-rw-r--r--   0        0        0    38990 2023-07-07 15:38:38.029956 pyhard-2.2.0/pyhard/data/2normalsSd030/data.csv
+-rw-r--r--   0        0        0   130100 2023-07-07 15:38:38.029956 pyhard-2.2.0/pyhard/data/2normalsSd030/feature_process.csv
+-rw-r--r--   0        0        0    94130 2023-07-07 15:38:38.030956 pyhard-2.2.0/pyhard/data/2normalsSd030/feature_raw.csv
+-rw-r--r--   0        0        0   284473 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd030/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd030/options.json
+-rw-r--r--   0        0        0    64807 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd045/2normals045.pdf
+-rw-r--r--   0        0        0    39780 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd045/coordinates.csv
+-rw-r--r--   0        0        0    39157 2023-07-07 15:38:38.032956 pyhard-2.2.0/pyhard/data/2normalsSd045/data.csv
+-rw-r--r--   0        0        0   178828 2023-07-07 15:38:38.032956 pyhard-2.2.0/pyhard/data/2normalsSd045/feature_process.csv
+-rw-r--r--   0        0        0   131886 2023-07-07 15:38:38.033956 pyhard-2.2.0/pyhard/data/2normalsSd045/feature_raw.csv
+-rw-r--r--   0        0        0   318453 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/2normalsSd045/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/2normalsSd045/options.json
+-rw-r--r--   0        0        0    15846 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/circle/circle.png
+-rw-r--r--   0        0        0    39346 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/circle/coordinates.csv
+-rw-r--r--   0        0        0    40231 2023-07-07 15:38:38.035956 pyhard-2.2.0/pyhard/data/circle/data.csv
+-rw-r--r--   0        0        0   226405 2023-07-07 15:38:38.035956 pyhard-2.2.0/pyhard/data/circle/feature_process.csv
+-rw-r--r--   0        0        0   145447 2023-07-07 15:38:38.036956 pyhard-2.2.0/pyhard/data/circle/feature_raw.csv
+-rw-r--r--   0        0        0   320526 2023-07-07 15:38:38.037956 pyhard-2.2.0/pyhard/data/circle/metadata.csv
+-rw-r--r--   0        0        0      595 2023-07-07 15:38:38.037956 pyhard-2.2.0/pyhard/data/circle/options.json
+-rw-r--r--   0        0        0    40190 2023-07-07 15:38:38.038956 pyhard-2.2.0/pyhard/data/easy/coordinates.csv
+-rw-r--r--   0        0        0    40952 2023-07-07 15:38:38.038956 pyhard-2.2.0/pyhard/data/easy/data.csv
+-rw-r--r--   0        0        0   147238 2023-07-07 15:38:38.038956 pyhard-2.2.0/pyhard/data/easy/feature_process.csv
+-rw-r--r--   0        0        0    54473 2023-07-07 15:38:38.039956 pyhard-2.2.0/pyhard/data/easy/feature_raw_color.csv
+-rw-r--r--   0        0        0   282881 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy/metadata.csv
+-rw-r--r--   0        0        0      595 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy/options.json
+-rw-r--r--   0        0        0    39957 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy2/coordinates.csv
+-rw-r--r--   0        0        0    40817 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy2/data.csv
+-rw-r--r--   0        0        0    42676 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy2/easy2.png
+-rw-r--r--   0        0        0   285261 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/easy2/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/easy2/options.json
+-rw-r--r--   0        0        0      190 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/easy2/projection_matrix.csv
+-rw-r--r--   0        0        0     5787 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/coordinates.csv
+-rw-r--r--   0        0        0     3877 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/data.csv
+-rw-r--r--   0        0        0    42802 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/options.json
+-rw-r--r--   0        0        0    39716 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/mix/coordinates.csv
+-rw-r--r--   0        0        0    40903 2023-07-07 15:38:38.043956 pyhard-2.2.0/pyhard/data/mix/data.csv
+-rw-r--r--   0        0        0   193499 2023-07-07 15:38:38.043956 pyhard-2.2.0/pyhard/data/mix/feature_process.csv
+-rw-r--r--   0        0        0   144369 2023-07-07 15:38:38.044956 pyhard-2.2.0/pyhard/data/mix/feature_raw.csv
+-rw-r--r--   0        0        0   296920 2023-07-07 15:38:38.045956 pyhard-2.2.0/pyhard/data/mix/metadata.csv
+-rw-r--r--   0        0        0    66400 2023-07-07 15:38:38.045956 pyhard-2.2.0/pyhard/data/mix/mix.png
+-rw-r--r--   0        0        0      597 2023-07-07 15:38:38.045956 pyhard-2.2.0/pyhard/data/mix/options.json
+-rw-r--r--   0        0        0    39233 2023-07-07 15:38:38.046956 pyhard-2.2.0/pyhard/data/overlap/coordinates.csv
+-rw-r--r--   0        0        0    39752 2023-07-07 15:38:38.046956 pyhard-2.2.0/pyhard/data/overlap/data.csv
+-rw-r--r--   0        0        0   321095 2023-07-07 15:38:38.047956 pyhard-2.2.0/pyhard/data/overlap/metadata.csv
+-rw-r--r--   0        0        0      598 2023-07-07 15:38:38.047956 pyhard-2.2.0/pyhard/data/overlap/options.json
+-rw-r--r--   0        0        0    13099 2023-07-07 15:38:38.047956 pyhard-2.2.0/pyhard/data/overlap/overlap.png
+-rw-r--r--   0        0        0    39995 2023-07-07 15:38:38.048956 pyhard-2.2.0/pyhard/data/separate/coordinates.csv
+-rw-r--r--   0        0        0    42167 2023-07-07 15:38:38.048956 pyhard-2.2.0/pyhard/data/separate/data.csv
+-rw-r--r--   0        0        0   177556 2023-07-07 15:38:38.049956 pyhard-2.2.0/pyhard/data/separate/feature_process.csv
+-rw-r--r--   0        0        0   113525 2023-07-07 15:38:38.049956 pyhard-2.2.0/pyhard/data/separate/feature_raw.csv
+-rw-r--r--   0        0        0   287283 2023-07-07 15:38:38.050956 pyhard-2.2.0/pyhard/data/separate/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-07 15:38:38.050956 pyhard-2.2.0/pyhard/data/separate/options.json
+-rw-r--r--   0        0        0    29361 2023-07-07 15:38:38.050956 pyhard-2.2.0/pyhard/data/wine/algorithm_bin.csv
+-rw-r--r--   0        0        0   226327 2023-07-07 15:38:38.051956 pyhard-2.2.0/pyhard/data/wine/algorithm_process.csv
+-rw-r--r--   0        0        0   218520 2023-07-07 15:38:38.052956 pyhard-2.2.0/pyhard/data/wine/algorithm_raw.csv
+-rw-r--r--   0        0        0    10101 2023-07-07 15:38:38.052956 pyhard-2.2.0/pyhard/data/wine/beta_easy.csv
+-rw-r--r--   0        0        0     4375 2023-07-07 15:38:38.052956 pyhard-2.2.0/pyhard/data/wine/config.yaml
+-rw-r--r--   0        0        0    69563 2023-07-07 15:38:38.053956 pyhard-2.2.0/pyhard/data/wine/coordinates.csv
+-rw-r--r--   0        0        0   100951 2023-07-07 15:38:38.053956 pyhard-2.2.0/pyhard/data/wine/data.csv
+-rw-r--r--   0        0        0   163688 2023-07-07 15:38:38.054956 pyhard-2.2.0/pyhard/data/wine/feature_process.csv
+-rw-r--r--   0        0        0   163380 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/feature_raw.csv
+-rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_bagging_best.csv
+-rw-r--r--   0        0        0     1634 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_bagging_good.csv
+-rw-r--r--   0        0        0      174 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_gradient_boosting_best.csv
+-rw-r--r--   0        0        0     1726 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_gradient_boosting_good.csv
+-rw-r--r--   0        0        0      720 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_instance_easiness_good.csv
+-rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_logistic_regression_best.csv
+-rw-r--r--   0        0        0     1696 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_logistic_regression_good.csv
+-rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_mlp_best.csv
+-rw-r--r--   0        0        0     1663 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_mlp_good.csv
+-rw-r--r--   0        0        0      893 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_performance.csv
+-rw-r--r--   0        0        0     2760 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_best.csv
+-rw-r--r--   0        0        0     1903 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_good.csv
+-rw-r--r--   0        0        0      259 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_linear_best.csv
+-rw-r--r--   0        0        0     1434 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_linear_good.csv
+-rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_rbf_best.csv
+-rw-r--r--   0        0        0     1516 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_rbf_good.csv
+-rw-r--r--   0        0        0    10103 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/good_algos.csv
+-rw-r--r--   0        0        0    37458 2023-07-07 15:38:38.056956 pyhard-2.2.0/pyhard/data/wine/ih.csv
+-rw-r--r--   0        0        0   317680 2023-07-07 15:38:38.057956 pyhard-2.2.0/pyhard/data/wine/metadata.csv
+-rw-r--r--   0        0        0   522841 2023-07-07 15:38:38.059956 pyhard-2.2.0/pyhard/data/wine/metadata_full.csv
+-rw-r--r--   0        0        0   409402 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/model.pkl
+-rw-r--r--   0        0        0      790 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/options.json
+-rw-r--r--   0        0        0    10105 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/portfolio.csv
+-rw-r--r--   0        0        0      231 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/projection_matrix.csv
+-rw-r--r--   0        0        0    40143 2023-07-07 15:38:38.062956 pyhard-2.2.0/pyhard/data/xor/coordinates.csv
+-rw-r--r--   0        0        0    40214 2023-07-07 15:38:38.062956 pyhard-2.2.0/pyhard/data/xor/data.csv
+-rw-r--r--   0        0        0   272866 2023-07-07 15:38:38.063956 pyhard-2.2.0/pyhard/data/xor/metadata.csv
+-rw-r--r--   0        0        0      598 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/data/xor/options.json
+-rw-r--r--   0        0        0      196 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/data/xor/projection_matrix.csv
+-rw-r--r--   0        0        0    65163 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/data/xor/xor.pdf
+-rw-r--r--   0        0        0     7659 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/feature_selection.py
+-rw-r--r--   0        0        0    10144 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/hpo.py
+-rw-r--r--   0        0        0    10847 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/integrator.py
+-rw-r--r--   0        0        0    43485 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/measures.py
+-rw-r--r--   0        0        0     3787 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/metrics.py
+-rw-r--r--   0        0        0   157445 2023-07-07 15:38:38.067956 pyhard-2.2.0/pyhard/midia/blobs.svg
+-rw-r--r--   0        0        0    11042 2023-07-07 15:38:38.067956 pyhard-2.2.0/pyhard/regression.py
+-rw-r--r--   0        0        0     4123 2023-07-07 15:38:38.067956 pyhard-2.2.0/pyhard/structures.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:38:38.104956 pyhard-2.2.0/pyhard/thirdparty/__init__.py
+-rwxr-xr-x   0        0        0    10787 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/thirdparty/entropy_estimators.py
+-rw-r--r--   0        0        0     4948 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/thirdparty/rank_aggregation.py
+-rw-r--r--   0        0        0    21966 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/thirdparty/skfeature.py
+-rw-r--r--   0        0        0     5221 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/utils.py
+-rw-r--r--   0        0        0     2359 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/validator.py
+-rw-r--r--   0        0        0    38600 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/visualization.py
+-rw-r--r--   0        0        0     1587 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10287 1970-01-01 00:00:00.000000 pyhard-2.2.0/PKG-INFO
```

### Comparing `pyhard-2.1.8/README.md` & `pyhard-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/__init__.py` & `pyhard-2.2.0/pyhard/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from pathlib import Path
 from typing import Union
 
 
-__version__ = "2.1.8"
+__version__ = "2.2.0"
 
 
 def get_seed() -> Union[int, None]:
     seed = os.environ.get("PYHARD_SEED")
     if seed is None:
         return seed
     else:
```

### Comparing `pyhard-2.1.8/pyhard/app.py` & `pyhard-2.2.0/pyhard/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,45 +552,52 @@
             df_selection = df_full[mask].copy()
             df_selection.loc[:, output_col] = df_selection[output_col].apply(lambda x: str(x))
             classes = df_selection[output_col].unique().tolist()
             classes.sort()
             category_orders = {output_col: classes}
             fig = None
 
+            df_full['Group'] = 'All instances'
+            df_selection['Group'] = 'Selected instances'
+            df_groups = pd.concat([df_selection, df_full])
+
             if dist_type == 'Histogram':
                 fig = px.histogram(
-                    df_selection,
+                    df_groups,
                     x=var,
                     color=output_col,
+                    facet_col="Group",
                     category_orders=category_orders
                 )
+                fig.update_layout(barmode='overlay')
+                fig.update_traces(opacity=0.7)
             elif dist_type == 'Bar':
-                df_count = df_selection[[var, output_col]].value_counts()
+                df_count = df_groups[[var, output_col, 'Group']].value_counts()
                 df_count.name = 'count'
                 df_count = df_count.to_frame().reset_index()
+
                 fig = px.bar(
                     df_count,
                     x=var,
                     y="count",
                     color=output_col,
+                    facet_col="Group",
                     category_orders=category_orders
                 )
             elif dist_type == 'Box':
-                df_full['Group'] = 'All instances'
-                df_selection['Group'] = 'Selected instances'
                 fig = px.box(
-                    pd.concat([df_selection, df_full]),
+                    df_groups,
                     x='Group',
                     y=var,
                     color=output_col,
                     category_orders=category_orders
                 )
 
             fig.update_layout(
-                margin=dict(l=0, r=0, t=20, b=10),
+                margin=dict(l=0, r=0, t=50, b=10),
                 paper_bgcolor='rgba(0,0,0,0)',
                 modebar={'bgcolor': 'rgba(255,255,255,0)'},
                 font_family="'Source Sans Pro', verdana, arial",
                 legend_font_size=14,
                 font_size=16
             )
             fig.layout.autosize = True
@@ -699,15 +706,21 @@
                 ),
                 coloraxis={'colorscale': coolwarm_cmap}
             )
             # fig_plotly.update_traces(marker=dict(size=7))
             fig_plotly.layout.autosize = True
             return pn.Column(
                 pn.Spacer(),
-                pn.pane.Plotly(fig_plotly, aspect_ratio=2),
+                pn.Row(pn.pane.Plotly(fig_plotly, aspect_ratio=2)),
+                pn.Spacer(height=20),
+                "## Descriptive statistics of the filtered data",
+                pn.Row(pn.pane.DataFrame(
+                    df_all.loc[~background, self.feat_cols + self.meta_cols].describe().T,
+                    sizing_mode="stretch_both"
+                )),
                 sizing_mode="stretch_width"
             )
 
         def download_data():
             return BytesIO(self.explorer_data.to_csv().encode())
 
         button_download = pn.widgets.FileDownload(
```

### Comparing `pyhard-2.1.8/pyhard/base.py` & `pyhard-2.2.0/pyhard/base.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/classification.py` & `pyhard-2.2.0/pyhard/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import time
 import warnings
 from typing import Any, Dict, List, Optional, Union, Type, Tuple
 
 import hyperopt
 import numpy as np
 import pandas as pd
+from imblearn.over_sampling import SMOTE
 from sklearn.base import ClassifierMixin, RegressorMixin
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.dummy import DummyClassifier
 from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier, BaggingClassifier
 from sklearn.exceptions import ConvergenceWarning
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import StratifiedKFold
@@ -26,14 +27,15 @@
 from sklearn.preprocessing import StandardScaler
 from sklearn.svm import SVC, LinearSVC
 
 from . import metrics, get_seed
 from .base import LearnersPool
 from .hpo import find_best_params
 from .metrics import loss_threshold
+from .validator import are_classes_balanced
 
 
 _clf_dict = {
     'svc_linear': LinearSVC,
     'svc_rbf': SVC,
     'random_forest': RandomForestClassifier,
     'gradient_boosting': GradientBoostingClassifier,
@@ -159,32 +161,42 @@
             kwargs = {**kwargs, **{'random_state': seed}}
 
         if verbose:
             self.logger.setLevel(logging.DEBUG)
 
         kf = StratifiedKFold(n_splits=n_folds, shuffle=True, random_state=seed)
 
+        imbalanced = not are_classes_balanced(pd.Series(self.y))
+
         score = np.zeros((self.N, n_iter))
         proba = np.zeros((self.N, n_iter))
         start = time.time()
 
         self.logger.info("Estimating instance performance...")
         if not hyper_param_optm:
             self.logger.debug(f"Training classifier with default parameters {kwargs}")
         for i in range(n_iter):
             k = 0
             accuracy = 0
             for train_index, test_index in kf.split(self.X, self.y):
                 k += 1
                 self.logger.info(f"Evaluating testing fold #{k}")
 
-                scaler = StandardScaler()
-                X_train = scaler.fit_transform(self.X[train_index, :])
+                X_train_ = self.X[train_index, :]
                 y_train = self.y[train_index]
-                X_test = scaler.transform(self.X[test_index, :])
+                X_test_ = self.X[test_index, :]
+
+                if imbalanced:
+                    self.logger.info("Over-sampling training fold with SMOTE")
+                    X_train_, y_train = SMOTE().fit_resample(X_train_, y_train)
+
+                self.logger.debug("Normalizing values with standard scaler")
+                scaler = StandardScaler()
+                X_train = scaler.fit_transform(X_train_)
+                X_test = scaler.transform(X_test_)
 
                 if hyper_param_optm:
                     self.logger.info("Optimizing classifier hyper-parameters")
                     best_params = find_best_params(
                         alias=hpo_name,
                         predictor=algo,
                         fixed_params=kwargs,
@@ -197,15 +209,15 @@
                     clf = algo(**best_params)
                 else:
                     clf = algo(**kwargs)
 
                 # clf = clf.fit(X_train, y_train)
                 self.logger.info("Calibrating probabilities")
                 calibrated_clf = CalibratedClassifierCV(
-                    base_estimator=clf,
+                    estimator=clf,
                     method='sigmoid',
                     cv=3,
                     ensemble=False,
                     n_jobs=None
                 )
                 calibrated_clf.fit(X_train, y_train)
```

### Comparing `pyhard-2.1.8/pyhard/cli.py` & `pyhard-2.2.0/pyhard/cli.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/conf/config.yaml` & `pyhard-2.2.0/pyhard/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/conf/config_old.yaml` & `pyhard-2.2.0/pyhard/conf/config_old.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/conf/options.json` & `pyhard-2.2.0/pyhard/conf/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/context.py` & `pyhard-2.2.0/pyhard/context.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normals/2normals.pdf` & `pyhard-2.2.0/pyhard/data/2normals/2normals.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normals/coordinates.csv` & `pyhard-2.2.0/pyhard/data/2normals/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normals/data.csv` & `pyhard-2.2.0/pyhard/data/2normals/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normals/feature_process.csv` & `pyhard-2.2.0/pyhard/data/2normals/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normals/feature_raw.csv` & `pyhard-2.2.0/pyhard/data/2normals/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normals/metadata.csv` & `pyhard-2.2.0/pyhard/data/2normals/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normals/options.json` & `pyhard-2.2.0/pyhard/data/2normals/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd030/2normals030.pdf` & `pyhard-2.2.0/pyhard/data/2normalsSd030/2normals030.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd030/coordinates.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd030/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd030/data.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd030/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd030/feature_process.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd030/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd030/feature_raw.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd030/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd030/metadata.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd030/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd030/options.json` & `pyhard-2.2.0/pyhard/data/2normalsSd030/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd045/2normals045.pdf` & `pyhard-2.2.0/pyhard/data/2normalsSd045/2normals045.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd045/coordinates.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd045/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd045/data.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd045/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd045/feature_process.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd045/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd045/feature_raw.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd045/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd045/metadata.csv` & `pyhard-2.2.0/pyhard/data/2normalsSd045/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/2normalsSd045/options.json` & `pyhard-2.2.0/pyhard/data/2normalsSd045/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/circle/circle.png` & `pyhard-2.2.0/pyhard/data/circle/circle.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/circle/coordinates.csv` & `pyhard-2.2.0/pyhard/data/circle/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/circle/data.csv` & `pyhard-2.2.0/pyhard/data/circle/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/circle/feature_process.csv` & `pyhard-2.2.0/pyhard/data/circle/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/circle/feature_raw.csv` & `pyhard-2.2.0/pyhard/data/circle/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/circle/metadata.csv` & `pyhard-2.2.0/pyhard/data/circle/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/circle/options.json` & `pyhard-2.2.0/pyhard/data/circle/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy/coordinates.csv` & `pyhard-2.2.0/pyhard/data/easy/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy/data.csv` & `pyhard-2.2.0/pyhard/data/easy/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy/feature_process.csv` & `pyhard-2.2.0/pyhard/data/easy/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy/feature_raw_color.csv` & `pyhard-2.2.0/pyhard/data/easy/feature_raw_color.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy/metadata.csv` & `pyhard-2.2.0/pyhard/data/easy/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy/options.json` & `pyhard-2.2.0/pyhard/data/easy/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy2/coordinates.csv` & `pyhard-2.2.0/pyhard/data/easy2/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy2/data.csv` & `pyhard-2.2.0/pyhard/data/easy2/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy2/easy2.png` & `pyhard-2.2.0/pyhard/data/easy2/easy2.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy2/metadata.csv` & `pyhard-2.2.0/pyhard/data/easy2/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/easy2/options.json` & `pyhard-2.2.0/pyhard/data/easy2/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/iris/coordinates.csv` & `pyhard-2.2.0/pyhard/data/iris/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/iris/data.csv` & `pyhard-2.2.0/pyhard/data/iris/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/iris/metadata.csv` & `pyhard-2.2.0/pyhard/data/iris/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/iris/options.json` & `pyhard-2.2.0/pyhard/data/iris/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/mix/coordinates.csv` & `pyhard-2.2.0/pyhard/data/mix/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/mix/data.csv` & `pyhard-2.2.0/pyhard/data/mix/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/mix/feature_process.csv` & `pyhard-2.2.0/pyhard/data/mix/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/mix/feature_raw.csv` & `pyhard-2.2.0/pyhard/data/mix/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/mix/metadata.csv` & `pyhard-2.2.0/pyhard/data/mix/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/mix/mix.png` & `pyhard-2.2.0/pyhard/data/mix/mix.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/mix/options.json` & `pyhard-2.2.0/pyhard/data/mix/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/overlap/coordinates.csv` & `pyhard-2.2.0/pyhard/data/overlap/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/overlap/data.csv` & `pyhard-2.2.0/pyhard/data/overlap/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/overlap/metadata.csv` & `pyhard-2.2.0/pyhard/data/overlap/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/overlap/options.json` & `pyhard-2.2.0/pyhard/data/overlap/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/overlap/overlap.png` & `pyhard-2.2.0/pyhard/data/overlap/overlap.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/separate/coordinates.csv` & `pyhard-2.2.0/pyhard/data/separate/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/separate/data.csv` & `pyhard-2.2.0/pyhard/data/separate/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/separate/feature_process.csv` & `pyhard-2.2.0/pyhard/data/separate/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/separate/feature_raw.csv` & `pyhard-2.2.0/pyhard/data/separate/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/separate/metadata.csv` & `pyhard-2.2.0/pyhard/data/separate/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/separate/options.json` & `pyhard-2.2.0/pyhard/data/separate/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/algorithm_bin.csv` & `pyhard-2.2.0/pyhard/data/wine/algorithm_bin.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/algorithm_process.csv` & `pyhard-2.2.0/pyhard/data/wine/algorithm_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/algorithm_raw.csv` & `pyhard-2.2.0/pyhard/data/wine/algorithm_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/beta_easy.csv` & `pyhard-2.2.0/pyhard/data/wine/beta_easy.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/config.yaml` & `pyhard-2.2.0/pyhard/data/wine/config.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/coordinates.csv` & `pyhard-2.2.0/pyhard/data/wine/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/data.csv` & `pyhard-2.2.0/pyhard/data/wine/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/feature_process.csv` & `pyhard-2.2.0/pyhard/data/wine/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/feature_raw.csv` & `pyhard-2.2.0/pyhard/data/wine/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_bagging_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_bagging_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_gradient_boosting_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_gradient_boosting_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_instance_easiness_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_instance_easiness_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_logistic_regression_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_logistic_regression_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_mlp_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_mlp_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_performance.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_performance.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_random_forest_best.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_best.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_random_forest_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_svc_linear_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_svc_linear_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/footprint_svc_rbf_good.csv` & `pyhard-2.2.0/pyhard/data/wine/footprint_svc_rbf_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/good_algos.csv` & `pyhard-2.2.0/pyhard/data/wine/good_algos.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/ih.csv` & `pyhard-2.2.0/pyhard/data/wine/ih.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/metadata.csv` & `pyhard-2.2.0/pyhard/data/wine/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/metadata_full.csv` & `pyhard-2.2.0/pyhard/data/wine/metadata_full.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/model.pkl` & `pyhard-2.2.0/pyhard/data/wine/model.pkl`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/options.json` & `pyhard-2.2.0/pyhard/data/wine/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/wine/portfolio.csv` & `pyhard-2.2.0/pyhard/data/wine/portfolio.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/xor/coordinates.csv` & `pyhard-2.2.0/pyhard/data/xor/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/xor/data.csv` & `pyhard-2.2.0/pyhard/data/xor/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/xor/metadata.csv` & `pyhard-2.2.0/pyhard/data/xor/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/xor/options.json` & `pyhard-2.2.0/pyhard/data/xor/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/data/xor/xor.pdf` & `pyhard-2.2.0/pyhard/data/xor/xor.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/feature_selection.py` & `pyhard-2.2.0/pyhard/feature_selection.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/hpo.py` & `pyhard-2.2.0/pyhard/hpo.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/integrator.py` & `pyhard-2.2.0/pyhard/integrator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/measures.py` & `pyhard-2.2.0/pyhard/measures.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,16 +208,21 @@
         self.dtc_pruned = self.dtc_pruned.fit(self.X.values, self.y.values)
 
         # Naive Bayes classifier
         n_c = self.y.nunique()
         priors = np.ones((n_c,)) / n_c
 
         nb = GaussianNB(priors=priors)
-        self.calibrated_nb = CalibratedClassifierCV(base_estimator=nb, method='sigmoid',
-                                                    cv=3, ensemble=False, n_jobs=-1)
+        self.calibrated_nb = CalibratedClassifierCV(
+            estimator=nb,
+            method='sigmoid',
+            cv=3,
+            ensemble=False,
+            n_jobs=-1
+        )
         self.calibrated_nb.fit(self.X, self.y)
 
         # Gower distance matrix
         # self.dist_matrix_gower = gower.gower_matrix(self.X.values.copy())
         self.dist_matrix_gower = gower_distance(self.X)
         delta = np.diag(-np.ones(self.dist_matrix_gower.shape[0]))
         self.indices_gower = np.argsort(self.dist_matrix_gower + delta, axis=1)
@@ -862,15 +867,15 @@
         Returns:
             array-like: Absolute error after linear fit values per instance.
         """
         lr = LinearRegression(fit_intercept=False)
         lr.fit(self.X_scaled, self.y_scaled)
         y_pred = lr.predict(self.X_scaled)
         L1 = np.abs(self.y_scaled - y_pred)
-        L1_normalized = 1 - 1/(1 + L1)
+        L1_normalized = 1 - 1 / (1 + L1)
         return L1_normalized
 
     def output_distribution(self) -> np.ndarray:
         r"""
         As in :math:`N_1` for classification, first a MST is generated from input data. Next :math:`S_1` monitors
         whether the instances joined in the MST have similar output values. An instance :math:`\mathbf x_i` can have
         multiple neighbors in the MST. So, take the average of the differences between their outputs:
@@ -935,35 +940,47 @@
         aux[1:] += d1
         aux[:-1] += d2
         aux[1:-1] *= 1 / 2
         S2[idx] = aux
 
         return 1 - 1 / (1 + S2)
 
-    def error_nn_regressor(self) -> np.ndarray:
+    def error_nn_regressor(self, n_neighbors: int = 5) -> np.ndarray:
         r"""
         Calculates the squared error (SE) of a *1-nearest neighbor regressor* (NN), using *leave-one-out*. The 1-NN
         regressor looks for the training example :math:`\mathbf x_i` most similar to the new example in the input space
         and assigns to it the same output :math:`y_i`.
 
         .. math::
 
             S_3(\mathbf x_i) = (NN(\mathbf x_i)-y_i)^2
 
         where :math:`NN(\mathbf x_i)` represents the 1-nearest neighbor prediction for :math:`\mathbf x_i`. Larger
         values are observed for harder instances.
 
+        Args:
+            n_neighbors (int): number of neighbors
+
         Returns:
             array-like: Squared error of 1-nearest neighbor values per instance.
         """
-        nn = NearestNeighbors(n_neighbors=1, metric='precomputed').fit(self.dist_matrix_gower)
+        nn = NearestNeighbors(n_neighbors=n_neighbors, metric='precomputed').fit(self.dist_matrix_gower)
         nn_arr = nn.kneighbors_graph(mode='distance').toarray()
         _, neighs = np.nonzero(nn_arr)
-        S3 = (self.y_scaled[neighs] - self.y_scaled) ** 2
 
+        nn_y_avg_scaled = np.array(list())
+
+        # Iterates over the neighbors and gets the average of y
+        for idx in range(0, len(neighs), n_neighbors):
+            nn_y_avg_scaled = \
+                np.append(
+                    nn_y_avg_scaled,
+                    np.mean(self.y_scaled[neighs[idx:idx + n_neighbors]])
+                )
+        S3 = (nn_y_avg_scaled - self.y_scaled) ** 2
         return 1 - np.exp(-S3 / S3.std())
 
     def feature_outlier(self) -> np.ndarray:
         IQR = iqr(self.X_scaled, axis=0)
         Q1 = np.quantile(self.X_scaled, 0.25, axis=0)
         Q3 = np.quantile(self.X_scaled, 0.75, axis=0)
         lbound = Q1 - 1.5 * IQR
```

### Comparing `pyhard-2.1.8/pyhard/metrics.py` & `pyhard-2.2.0/pyhard/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/midia/blobs.svg` & `pyhard-2.2.0/pyhard/midia/blobs.svg`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/regression.py` & `pyhard-2.2.0/pyhard/regression.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/structures.py` & `pyhard-2.2.0/pyhard/structures.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/thirdparty/entropy_estimators.py` & `pyhard-2.2.0/pyhard/thirdparty/entropy_estimators.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/thirdparty/rank_aggregation.py` & `pyhard-2.2.0/pyhard/thirdparty/rank_aggregation.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/thirdparty/skfeature.py` & `pyhard-2.2.0/pyhard/thirdparty/skfeature.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/utils.py` & `pyhard-2.2.0/pyhard/utils.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/validator.py` & `pyhard-2.2.0/pyhard/validator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyhard/visualization.py` & `pyhard-2.2.0/pyhard/visualization.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.8/pyproject.toml` & `pyhard-2.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -12,53 +12,53 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Intended Audience :: Science/Research"
 ]
 dynamic = ["version"]
 dependencies = [
-    'pandas>=1.3.0',
-    'scikit-learn>=1.0.1',
-    'numpy>=1.18.4',
-    'PyYAML>=5.3',
-    'scipy>=1.4.1',
-    'panel~=0.14.1',
-    'param>=1.12.2',
-    'bokeh>=2.4.3',
-    'holoviews>=1.15.0',
-    'matplotlib>=3.2.2',
-    'plotly>=5.9.0',
-    'plotting>=0.0.7',
-    'shapely~=1.8.0',
-    'hyperopt>=0.2.4',
-    'pyispace>=0.3.4',
-    'deprecation>=2.1.0',
-    'joblib>=1.0.0',
-    'ncafs>=0.2',
-    'typer>=0.4.1',
-    'packaging>=21.0',
-    'requests>=2.27.0'
+    "pandas>=1.3.0",
+    "scikit-learn>=1.2.0, <1.3.0",
+    "imbalanced-learn>=0.10.0",
+    "numpy>=1.18.4",
+    "PyYAML>=5.3",
+    "scipy>=1.4.1",
+    "panel~=0.14.1",
+    "param>=1.12.2",
+    "bokeh>=2.4.3",
+    "holoviews>=1.15.0",
+    "matplotlib>=3.2.2",
+    "plotly>=5.9.0",
+    "plotting>=0.0.7",
+    "shapely~=1.8.0",
+    "hyperopt>=0.2.4",
+    "pyispace>=0.3.4",
+    "deprecation>=2.1.0",
+    "joblib>=1.0.0",
+    "ncafs>=0.2",
+    "typer>=0.4.1",
+    "packaging>=21.0",
+    "requests>=2.27.0"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "plotly>=5.6",
     "sphinx",
     "sphinx_rtd_theme",
+    "pytest",
     "notebook>=6.4",
     "jupyterlab>=3.5.3"
 ]
 
 [project.scripts]
 pyhard = "pyhard.cli:cli"
 
 [project.urls]
-Documentation = "https://ita-ml.gitlab.io/pyhard/"
-Repository = "https://gitlab.com/ita-ml/pyhard"
+documentation = "https://ita-ml.gitlab.io/pyhard/"
+repository = "https://gitlab.com/ita-ml/pyhard"
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [tool.flit.sdist]
-# include = ["docs/"]
 exclude = ["docs/", "experiments/", "notebooks/", "pyhard/tests/", ".pytest_cache/", "pyhard/graphene/"]
```

### Comparing `pyhard-2.1.8/PKG-INFO` & `pyhard-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyhard
-Version: 2.1.8
+Version: 2.2.0
 Summary: Analyze, explore and visualize instance hardness within datasets
 Author-email: Pedro Paiva <paiva@ita.br>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Dist: pandas>=1.3.0
-Requires-Dist: scikit-learn>=1.0.1
+Requires-Dist: scikit-learn>=1.2.0, <1.3.0
+Requires-Dist: imbalanced-learn>=0.10.0
 Requires-Dist: numpy>=1.18.4
 Requires-Dist: PyYAML>=5.3
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: panel~=0.14.1
 Requires-Dist: param>=1.12.2
 Requires-Dist: bokeh>=2.4.3
 Requires-Dist: holoviews>=1.15.0
@@ -28,21 +29,21 @@
 Requires-Dist: pyispace>=0.3.4
 Requires-Dist: deprecation>=2.1.0
 Requires-Dist: joblib>=1.0.0
 Requires-Dist: ncafs>=0.2
 Requires-Dist: typer>=0.4.1
 Requires-Dist: packaging>=21.0
 Requires-Dist: requests>=2.27.0
-Requires-Dist: plotly>=5.6 ; extra == "dev"
 Requires-Dist: sphinx ; extra == "dev"
 Requires-Dist: sphinx_rtd_theme ; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: notebook>=6.4 ; extra == "dev"
 Requires-Dist: jupyterlab>=3.5.3 ; extra == "dev"
-Project-URL: Documentation, https://ita-ml.gitlab.io/pyhard/
-Project-URL: Repository, https://gitlab.com/ita-ml/pyhard
+Project-URL: documentation, https://ita-ml.gitlab.io/pyhard/
+Project-URL: repository, https://gitlab.com/ita-ml/pyhard
 Provides-Extra: dev
 
 <!--
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/ita-ml%2Finstance-hardness/binder?filepath=notebooks%2F)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://en.wikipedia.org/wiki/MIT_License)
 -->
```

