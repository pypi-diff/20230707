# Comparing `tmp/neuralhydrology-1.7.0.tar.gz` & `tmp/neuralhydrology-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralhydrology-1.7.0.tar", last modified: Wed May 17 12:27:12 2023, max compression
+gzip compressed data, was "neuralhydrology-1.8.0.tar", last modified: Fri Jul  7 11:06:08 2023, max compression
```

## Comparing `neuralhydrology-1.7.0.tar` & `neuralhydrology-1.8.0.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.620346 neuralhydrology-1.7.0/neuralhydrology/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.624346 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/basedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsaus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelscl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/caravan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/genericdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/hourlycamelsus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/lamah.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.624346 neuralhydrology-1.7.0/neuralhydrology/datautils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/climateindices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/dischargeinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/pet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.624346 neuralhydrology-1.7.0/neuralhydrology/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    26358 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/neuralhydrology/modelzoo/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/arlstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/cudalstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/customlstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/ealstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/embcudalstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/fc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/gru.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/inputlayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/mclstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/mtslstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/odelstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/nh_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/nh_run_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/neuralhydrology/training/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/basetrainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/neuralhydrology/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/configutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/nh_results_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/ratingcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    30861 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/samplingutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.620346 neuralhydrology-1.7.0/neuralhydrology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:27:12.632346 neuralhydrology-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_config_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_custom_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_mclstm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.938261 neuralhydrology-1.8.0/neuralhydrology/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.942261 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45263 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/basedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsaus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelscl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/caravan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/genericdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/hourlycamelsus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/lamah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.942261 neuralhydrology-1.8.0/neuralhydrology/datautils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/climateindices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/dischargeinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/pet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.942261 neuralhydrology-1.8.0/neuralhydrology/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28418 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/neuralhydrology/modelzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/arlstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/cudalstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/customlstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/ealstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/embcudalstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/gru.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10145 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/handoff_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/inputlayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/mclstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/mtslstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/multihead_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/odelstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/sequential_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/stacked_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/nh_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/nh_run_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/neuralhydrology/training/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/basetrainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/neuralhydrology/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29390 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/configutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/nh_results_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/ratingcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32397 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/samplingutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.938261 neuralhydrology-1.8.0/neuralhydrology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_config_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_custom_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_mclstm.py
```

### Comparing `neuralhydrology-1.7.0/LICENSE` & `neuralhydrology-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/PKG-INFO` & `neuralhydrology-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralhydrology
-Version: 1.7.0
+Version: 1.8.0
 Summary: Library for training deep learning models with environmental focus
 Home-page: https://neuralhydrology.readthedocs.io
 Author: Frederik Kratzert, Daniel Klotz, Martin Gauch
 Author-email: neuralhydrology@googlegroups.com
 Project-URL: Documentation, https://neuralhydrology.readthedocs.io
 Project-URL: Source, https://github.com/neuralhydrology/neuralhydrology
 Project-URL: Research Blog, https://neuralhydrology.github.io/
```

### Comparing `neuralhydrology-1.7.0/README.md` & `neuralhydrology-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/__init__.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/basedataset.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/basedataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,14 +78,26 @@
         if period in ["validation", "test"]:
             if not scaler:
                 raise ValueError("During evaluation of validation or test period, scaler dictionary has to be passed")
 
             if cfg.use_basin_id_encoding and not id_to_int:
                 raise ValueError("For basin id embedding, the id_to_int dictionary has to be passed anything but train")
 
+        if self.cfg.timestep_counter:
+            if not self.cfg.forecast_inputs:
+                raise ValueError('Timestep counter only works for forecast data.')
+            if cfg.forecast_overlap:
+                overlap_zeros = torch.zeros((cfg.forecast_overlap, 1))
+                forecast_counter = torch.Tensor(range(1, cfg.forecast_seq_length - cfg.forecast_overlap + 1)).unsqueeze(-1)
+                self.forecast_counter = torch.concatenate([overlap_zeros, forecast_counter], dim=0)
+                self.hindcast_counter = torch.zeros((cfg.seq_length - cfg.forecast_seq_length + cfg.forecast_overlap, 1))
+            else:
+                self.forecast_counter = torch.Tensor(range(1, cfg.forecast_seq_length + 1)).unsqueeze(-1)
+                self.hindcast_counter = torch.zeros((cfg.seq_length - cfg.forecast_seq_length, 1))
+            
         if basin is None:
             self.basins = utils.load_basin_file(getattr(cfg, f"{period}_basin_file"))
         else:
             self.basins = [basin]
         self.additional_features = additional_features
         self.id_to_int = id_to_int
         self.scaler = scaler
@@ -102,14 +114,16 @@
         self._initialize_frequency_configuration()
 
         # during training we log data processing with progress bars, but not during validation/testing
         self._disable_pbar = cfg.verbose == 0 or not self.is_train
 
         # initialize class attributes that are filled in the data loading functions
         self._x_d = {}
+        self._x_h = {}
+        self._x_f = {}
         self._x_s = {}
         self._attributes = {}
         self._y = {}
         self._per_basin_target_stds = {}
         self._dates = {}
         self.start_and_end_dates = {}
         self.num_samples = 0
@@ -140,27 +154,47 @@
         basin, indices = self.lookup_table[item]
 
         sample = {}
         for freq, seq_len, idx in zip(self.frequencies, self.seq_len, indices):
             # if there's just one frequency, don't use suffixes.
             freq_suffix = '' if len(self.frequencies) == 1 else f'_{freq}'
             # slice until idx + 1 because slice-end is excluding
-            sample[f'x_d{freq_suffix}'] = self._x_d[basin][freq][idx - seq_len + 1:idx + 1]
-            sample[f'y{freq_suffix}'] = self._y[basin][freq][idx - seq_len + 1:idx + 1]
-            sample[f'date{freq_suffix}'] = self._dates[basin][freq][idx - seq_len + 1:idx + 1]
+            hindcast_start_idx = idx + 1 - seq_len
+            global_end_idx = idx + 1
+            if self._x_d:
+                sample[f'x_d{freq_suffix}'] = self._x_d[basin][freq][hindcast_start_idx:global_end_idx]
+            elif self._x_h:
+                hindcast_end_idx = idx + 1 - self.cfg.forecast_seq_length
+                forecast_start_idx = idx + 1 - self.cfg.forecast_seq_length
+                if self.cfg.forecast_overlap and self.cfg.forecast_overlap > 0:
+                    hindcast_end_idx += self.cfg.forecast_overlap
+                sample[f'x_h{freq_suffix}'] = self._x_h[basin][freq][hindcast_start_idx:hindcast_end_idx]
+                sample[f'x_f{freq_suffix}'] = self._x_f[basin][freq][forecast_start_idx:global_end_idx]
+            else:
+                raise ValueError('Data must include x_d or x_h.')
+
+            sample[f'y{freq_suffix}'] = self._y[basin][freq][hindcast_start_idx:global_end_idx]
+            sample[f'date{freq_suffix}'] = self._dates[basin][freq][hindcast_start_idx:global_end_idx]
 
             # check for static inputs
             static_inputs = []
             if self._attributes:
                 static_inputs.append(self._attributes[basin])
             if self._x_s:
                 static_inputs.append(self._x_s[basin][freq][idx])
             if static_inputs:
                 sample[f'x_s{freq_suffix}'] = torch.cat(static_inputs, dim=-1)
 
+            if self.cfg.timestep_counter:
+                if self._x_d:
+                    torch.concatenate([sample[f'x_d{freq_suffix}'], self.hindcast_counter], dim=-1)
+                else:
+                    torch.concatenate([sample[f'x_h{freq_suffix}'], self.hindcast_counter], dim=-1)
+                    torch.concatenate([sample[f'x_f{freq_suffix}'], self.forecast_counter], dim=-1)
+
         if self._per_basin_target_stds:
             sample['per_basin_target_stds'] = self._per_basin_target_stds[basin]
         if self.id_to_int:
             sample['x_one_hot'] = torch.nn.functional.one_hot(torch.tensor(self.id_to_int[basin]),
                                                               num_classes=len(self.id_to_int)).to(torch.float32)
 
         return sample
@@ -228,14 +262,21 @@
 
     def _duplicate_features(self, df: pd.DataFrame) -> pd.DataFrame:
         for feature, n_duplicates in self.cfg.duplicate_features.items():
             for n in range(1, n_duplicates + 1):
                 df[f"{feature}_copy{n}"] = df[feature]
 
         return df
+    
+    def _add_missing_targets(self, df: pd.DataFrame) -> pd.DataFrame:
+        for var in self.cfg.target_variables:
+            if var not in df.columns:
+                df[var] = np.nan
+
+        return df
 
     def _add_lagged_features(self, df: pd.DataFrame) -> pd.DataFrame:
 
         # check that all autoregressive inputs are contained in the list of shifted variables
         self._check_autoregressive_inputs()
 
         # create the shifted varaibles, as requested
@@ -287,14 +328,18 @@
                 LOGGER.info("Loading basin data into xarray data set.")
             for basin in tqdm(self.basins, disable=self._disable_pbar, file=sys.stdout):
                 df = self._load_basin_data(basin)
 
                 # add columns from dataframes passed as additional data files
                 df = pd.concat([df, *[d[basin] for d in self.additional_features]], axis=1)
 
+                # if target variables are missing for basin, add empty column to still allow predictions to be made
+                if not self.is_train:
+                    df = self._add_missing_targets(df)
+
                 # check if any feature should be duplicated
                 df = self._duplicate_features(df)
 
                 # check if a shifted copy of a feature should be added
                 df = self._add_lagged_features(df)
 
                 # remove unnecessary columns
@@ -477,14 +522,15 @@
         basins_without_samples = []
         basin_coordinates = xr["basin"].values.tolist()
         for basin in tqdm(basin_coordinates, file=sys.stdout, disable=self._disable_pbar):
 
             # store data of each frequency as numpy array of shape [time steps, features] and dates as numpy array of
             # shape (time steps,)
             x_d, x_s, y, dates = {}, {}, {}, {}
+            x_d_column_names = []
 
             # keys: frequencies, values: array mapping each lowest-frequency
             # sample to its corresponding sample in this frequency
             frequency_maps = {}
             lowest_freq = utils.sort_frequencies(self.frequencies)[0]
 
             # converting from xarray to pandas DataFrame because resampling is much faster in pandas.
@@ -497,14 +543,15 @@
                     dynamic_cols = self.cfg.mass_inputs + self.cfg.dynamic_inputs[freq]
 
                 df_resampled = df_native[dynamic_cols + self.cfg.target_variables + self.cfg.evolving_attributes +
                                          self.cfg.autoregressive_inputs].resample(freq).mean()
 
                 # pull all of the data that needs to be validated
                 x_d[freq] = df_resampled[dynamic_cols].values
+                x_d_column_names = dynamic_cols
                 y[freq] = df_resampled[self.cfg.target_variables].values
                 if self.cfg.evolving_attributes:
                     x_s[freq] = df_resampled[self.cfg.evolving_attributes].values
 
                 # Add dates of the (resampled) data to the dates dict
                 dates[freq] = df_resampled.index.to_numpy()
 
@@ -542,23 +589,32 @@
 
             # Concatenate autoregressive columns to dynamic inputs *after* validation, so as to not remove
             # samples with missing autoregressive inputs.
             # AR inputs must go at the end of the df/array (this is assumed by the AR model).
             if self.cfg.autoregressive_inputs:
                 for freq in self.frequencies:
                     x_d[freq] = np.concatenate([x_d[freq], df_resampled[self.cfg.autoregressive_inputs].values], axis=1)
+                x_d_column_names += self.cfg.autoregressive_inputs
 
             valid_samples = np.argwhere(flag == 1)
             for f in valid_samples:
                 # store pointer to basin and the sample's index in each frequency
                 lookup.append((basin, [frequency_maps[freq][int(f)] for freq in self.frequencies]))
 
             # only store data if this basin has at least one valid sample in the given period
             if valid_samples.size > 0:
-                self._x_d[basin] = {freq: torch.from_numpy(_x_d.astype(np.float32)) for freq, _x_d in x_d.items()}
+                if self.cfg.forecast_inputs:
+                    if not self.cfg.hindcast_inputs:
+                        raise ValueError('Hindcast inputs must be provided if forecast inputs are provided.')
+                    hindcast_indexes = [idx for idx, variable in enumerate(x_d_column_names) if variable in self.cfg.hindcast_inputs]
+                    forecast_indexes = [idx for idx, variable in enumerate(x_d_column_names) if variable in self.cfg.forecast_inputs]
+                    self._x_h[basin] = {freq: torch.from_numpy(_x_d[:, hindcast_indexes].astype(np.float32)) for freq, _x_d in x_d.items()}
+                    self._x_f[basin] = {freq: torch.from_numpy(_x_d[:, forecast_indexes].astype(np.float32)) for freq, _x_d in x_d.items()}
+                else:
+                    self._x_d[basin] = {freq: torch.from_numpy(_x_d.astype(np.float32)) for freq, _x_d in x_d.items()}
                 self._y[basin] = {freq: torch.from_numpy(_y.astype(np.float32)) for freq, _y in y.items()}
                 if x_s:
                     self._x_s[basin] = {freq: torch.from_numpy(_x_s.astype(np.float32)) for freq, _x_s in x_s.items()}
                 self._dates[basin] = dates
             else:
                 basins_without_samples.append(basin)
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsaus.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsaus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsbr.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsbr.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelscl.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelscl.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsgb.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsgb.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsus.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/caravan.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/caravan.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/genericdataset.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/genericdataset.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/hourlycamelsus.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/hourlycamelsus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/lamah.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/lamah.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/template.py` & `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/template.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datautils/climateindices.py` & `neuralhydrology-1.8.0/neuralhydrology/datautils/climateindices.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datautils/dischargeinput.py` & `neuralhydrology-1.8.0/neuralhydrology/datautils/dischargeinput.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datautils/pet.py` & `neuralhydrology-1.8.0/neuralhydrology/datautils/pet.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/datautils/utils.py` & `neuralhydrology-1.8.0/neuralhydrology/datautils/utils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/evaluation/__init__.py` & `neuralhydrology-1.8.0/neuralhydrology/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/evaluation/evaluate.py` & `neuralhydrology-1.8.0/neuralhydrology/evaluation/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     epoch : int, optional
         Define a specific epoch to evaluate. By default, the weights of the last epoch are used.
     period : {'train', 'validation', 'test'}, optional
         The period to evaluate, by default 'test'.
 
     """
     tester = get_tester(cfg=cfg, run_dir=run_dir, period=period, init_model=True)
-    tester.evaluate(epoch=epoch, save_results=True, metrics=cfg.metrics)
+    tester.evaluate(epoch=epoch, save_results=True, save_all_output=cfg.save_all_output, metrics=cfg.metrics)
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/evaluation/metrics.py` & `neuralhydrology-1.8.0/neuralhydrology/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/evaluation/plots.py` & `neuralhydrology-1.8.0/neuralhydrology/evaluation/plots.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/evaluation/signatures.py` & `neuralhydrology-1.8.0/neuralhydrology/evaluation/signatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         "slope_fdc": slope_fdc(da),
         "stream_elas": stream_elas(da, prcp, datetime_coord=datetime_coord),
         "runoff_ratio": runoff_ratio(da, prcp, datetime_coord=datetime_coord)
     }
     return results
 
 
-def calculate_signatures(da: DataArray, signatures: List[str], datetime_coord: str = None,
+def calculate_signatures(da: DataArray,
+                         signatures: List[str],
+                         datetime_coord: str = None,
                          prcp: DataArray = None) -> Dict[str, float]:
     """Calculate the specified signatures with default values.
 
     Parameters
     ----------
     da : DataArray
         Array of discharge values for which the signatures will be calculated.
@@ -595,16 +597,16 @@
     # sort discharge by descending order
     fdc = da.sortby(da, ascending=False)
 
     # get idx of lower and upper quantile
     idx_lower = np.round(lower_quantile * len(fdc)).astype(int)
     idx_upper = np.round(upper_quantile * len(fdc)).astype(int)
 
-    value = (np.log(fdc[idx_lower].values +
-                    1e-8)) - np.log(fdc[idx_upper].values + 1e-8) / (upper_quantile - lower_quantile)
+    value = (np.log(fdc[idx_lower].values + 1e-8) - np.log(fdc[idx_upper].values + 1e-8)) / (upper_quantile -
+                                                                                             lower_quantile)
 
     return value
 
 
 def runoff_ratio(da: DataArray, prcp: DataArray, datetime_coord: str = None) -> float:
     """Calculate runoff ratio.
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/evaluation/tester.py` & `neuralhydrology-1.8.0/neuralhydrology/evaluation/tester.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import pickle
 import random
 import re
 import sys
 from collections import defaultdict
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from pandas.tseries.frequencies import to_offset
 import torch
 import xarray
 from torch.utils.data import DataLoader
@@ -60,14 +60,16 @@
 
         # determine device
         self._set_device()
 
         if self.init_model:
             self.model = get_model(cfg).to(self.device)
 
+        self._disable_pbar = cfg.verbose == 0
+
         # pre-initialize variables, defined in class methods
         self.basins = None
         self.scaler = None
         self.id_to_int = {}
         self.additional_features = []
 
         # placeholder to store cached validation data
@@ -141,25 +143,28 @@
                          id_to_int=self.id_to_int,
                          scaler=self.scaler)
         return ds
 
     def evaluate(self,
                  epoch: int = None,
                  save_results: bool = True,
+                 save_all_output: bool = False,
                  metrics: Union[list, dict] = [],
                  model: torch.nn.Module = None,
                  experiment_logger: Logger = None) -> dict:
         """Evaluate the model.
         
         Parameters
         ----------
         epoch : int, optional
             Define a specific epoch to evaluate. By default, the weights of the last epoch are used.
         save_results : bool, optional
             If True, stores the evaluation results in the run directory. By default, True.
+        save_all_output : bool, optional
+            If True, stores all of the model output in the run directory. By default, False.
         metrics : Union[list, dict], optional
             List of metrics to compute during evaluation. Can also be a dict that specifies per-target metrics
         model : torch.nn.Module, optional
             If a model is passed, this is used for validation.
         experiment_logger : Logger, optional
             Logger can be passed during training to log metrics
 
@@ -185,16 +190,17 @@
         # force model to train-mode when doing mc-dropout evaluation
         if self.cfg.mc_dropout:
             model.train()
         else:
             model.eval()
 
         results = defaultdict(dict)
+        all_output = {basin: None for basin in basins}
 
-        pbar = tqdm(basins, file=sys.stdout)
+        pbar = tqdm(basins, file=sys.stdout, disable=self._disable_pbar)
         pbar.set_description('# Validation' if self.period == "validation" else "# Evaluation")
 
         for basin in pbar:
 
             if self.cfg.cache_validation_data and basin in self.cached_datasets.keys():
                 ds = self.cached_datasets[basin]
             else:
@@ -204,15 +210,15 @@
                     # skip basin
                     continue
                 if self.cfg.cache_validation_data and self.period == "validation":
                     self.cached_datasets[basin] = ds
 
             loader = DataLoader(ds, batch_size=self.cfg.batch_size, num_workers=0, collate_fn=ds.collate_fn)
 
-            y_hat, y, dates, all_losses = self._evaluate(model, loader, ds.frequencies)
+            y_hat, y, dates, all_losses, all_output[basin] = self._evaluate(model, loader, ds.frequencies, save_all_output)
 
             # log loss of this basin plus number of samples in the logger to compute epoch aggregates later
             if experiment_logger is not None:
                 experiment_logger.log_step(**{k: (v, len(loader)) for k, v in all_losses.items()})
 
             predict_last_n = self.cfg.predict_last_n
             seq_length = self.cfg.seq_length
@@ -328,16 +334,27 @@
         # a non-existing basin
         results = dict(results)
 
         if (self.period == "validation") and (self.cfg.log_n_figures > 0) and (experiment_logger
                                                                                is not None) and results:
             self._create_and_log_figures(results, experiment_logger, epoch)
 
+        # save model output to file, if requested
+        results_to_save = None
+        states_to_save = None
         if save_results:
-            self._save_results(results, epoch)
+            results_to_save = results
+        if save_all_output:
+            states_to_save = all_output
+        if save_results or save_all_output:
+            self._save_results(
+                results=results_to_save, 
+                states=states_to_save,
+                epoch=epoch
+            )
 
         return results
 
     def _create_and_log_figures(self, results: dict, experiment_logger: Logger, epoch: int):
         basins = list(results.keys())
         random.shuffle(basins)
         for target_var in self.cfg.target_variables:
@@ -353,36 +370,49 @@
                         sim = xarray.where(sim < 0, 0, sim)
                     figures.append(
                         self._get_plots(
                             obs, sim, title=f"{target_var} - Basin {basins[i]} - Epoch {epoch} - Frequency {freq}")[0])
                 # make sure the preamble is a valid file name
                 experiment_logger.log_figures(figures, freq, preamble=re.sub(r"[^A-Za-z0-9\._\-]+", "", target_var))
 
-    def _save_results(self, results: dict, epoch: int = None):
+    def _save_results(self, results: Optional[dict], states: Optional[dict] = None, epoch: int = None):
         """Store results in various formats to disk.
         
         Developer note: We cannot store the time series data (the xarray objects) as netCDF file but have to use
         pickle as a wrapper. The reason is that netCDF files have special constraints on the characters/symbols that can
         be used as variable names. However, for convenience we will store metrics, if calculated, in a separate csv-file.
         """
         # use name of weight file as part of the result folder name
         weight_file = self._get_weight_file(epoch=epoch)
 
-        # store all results packed as pickle file
-        result_file = self.run_dir / self.period / weight_file.stem / f"{self.period}_results.p"
-        result_file.parent.mkdir(parents=True, exist_ok=True)
-        with result_file.open("wb") as fp:
-            pickle.dump(results, fp)
+        # make sure the parent directory exists
+        parent_directory = self.run_dir / self.period / weight_file.stem
+        parent_directory.mkdir(parents=True, exist_ok=True)
 
+        # save metrics any time this funciton is called, as long as they exist
         if self.cfg.metrics:
             df = self._metrics_to_dataframe(results)
-            file_name = self.run_dir / self.period / weight_file.stem / f"{self.period}_metrics.csv"
-            df.to_csv(file_name)
+            metrics_file = parent_directory / f"{self.period}_metrics.csv"
+            df.to_csv(metrics_file)
+            LOGGER.info(f"Stored metrics at {metrics_file}")
+
+        # store all results packed as pickle file
+        if results is not None:
+            result_file = parent_directory / f"{self.period}_results.p"
+            with result_file.open("wb") as fp:
+                pickle.dump(results, fp)
+            LOGGER.info(f"Stored results at {result_file}")
+
+        # store all model output packed as pickle file
+        if states is not None:
+            result_file = parent_directory / f"{self.period}_all_output.p"
+            with result_file.open("wb") as fp:
+                pickle.dump(states, fp)
+            LOGGER.info(f"Stored states at {result_file}")
 
-        LOGGER.info(f"Stored results at {result_file}")
 
     def _metrics_to_dataframe(self, results: dict) -> pd.DataFrame:
         """Extract all metric values from result dictionary and convert to pandas.DataFrame
 
         Parameters
         ----------
         results: dict
@@ -404,31 +434,38 @@
                         metrics_dict[basin][metric] = np.nan
 
         df = pd.DataFrame.from_dict(metrics_dict, orient="index")
         df.index.name = "basin"
 
         return df
 
-    def _evaluate(self, model: BaseModel, loader: DataLoader, frequencies: List[str]):
+    def _evaluate(self, model: BaseModel, loader: DataLoader, frequencies: List[str], save_all_output: bool = False):
         """Evaluate model"""
         predict_last_n = self.cfg.predict_last_n
         if isinstance(predict_last_n, int):
             predict_last_n = {frequencies[0]: predict_last_n}  # if predict_last_n is int, there's only one frequency
 
-        preds, obs, dates = {}, {}, {}
+        preds, obs, dates, all_output = {}, {}, {}, {}
         losses = []
         with torch.no_grad():
             for data in loader:
 
                 for key in data:
                     if not key.startswith('date'):
                         data[key] = data[key].to(self.device)
                 data = model.pre_model_hook(data, is_train=False)
                 predictions, loss = self._get_predictions_and_loss(model, data)
 
+                if all_output:
+                    for key, value in predictions.items():
+                        if value is not None and type(value) != dict:
+                            all_output[key].append(value.detach().cpu().numpy()) 
+                elif save_all_output:
+                    all_output = {key: [value.detach().cpu().numpy()] for key, value in predictions.items() if value is not None and type(value) != dict}
+
                 for freq in frequencies:
                     if predict_last_n[freq] == 0:
                         continue  # no predictions for this frequency
                     freq_key = '' if len(frequencies) == 1 else f'_{freq}'
                     y_hat_sub, y_sub = self._subset_targets(model, data, predictions, predict_last_n[freq], freq_key)
                     # Date subsetting is universal across all models and thus happens here.
                     date_sub = data[f'date{freq_key}'][:, -predict_last_n[freq]:]
@@ -444,23 +481,28 @@
 
                 losses.append(loss)
 
             for freq in preds.keys():
                 preds[freq] = preds[freq].numpy()
                 obs[freq] = obs[freq].numpy()
 
+        # concatenate all output variables (currently a dict-of-dicts) into a single-level dict
+        for key, list_of_data in all_output.items():
+            all_output[key] = np.concatenate(list_of_data, 0)
+            
         # set to NaN explicitly if all losses are NaN to avoid RuntimeWarning
         mean_losses = {}
         if len(losses) == 0:
             mean_losses['loss'] = np.nan
         else:
             for loss_name in losses[0].keys():
                 loss_values = [loss[loss_name] for loss in losses]
                 mean_losses[loss_name] = np.nanmean(loss_values) if not np.all(np.isnan(loss_values)) else np.nan
-        return preds, obs, dates, mean_losses
+        
+        return preds, obs, dates, mean_losses, all_output
 
     def _get_predictions_and_loss(self, model: BaseModel, data: Dict[str, torch.Tensor]) -> Tuple[torch.Tensor, float]:
         predictions = model(data)
         _, all_losses = self.loss_obj(predictions, data)
         return predictions, {k: v.item() for k, v in all_losses.items()}
 
     def _subset_targets(self, model: BaseModel, data: Dict[str, torch.Tensor], predictions: np.ndarray,
@@ -553,7 +595,8 @@
         for i, var in enumerate(self.cfg.target_variables):
             data[f"{var}_obs"] = (('date', 'time_step'), y[:, :, i])
             data[f"{var}_sim"] = (('date', 'time_step', 'samples'), y_hat[:, :, i, :])
         return data
 
     def _get_plots(self, qobs: np.ndarray, qsim: np.ndarray, title: str):
         return plots.uncertainty_plot(qobs, qsim, title)
+
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/evaluation/utils.py` & `neuralhydrology-1.8.0/neuralhydrology/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/__init__.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,39 @@
 import torch.nn as nn
 
 from neuralhydrology.modelzoo.arlstm import ARLSTM
 from neuralhydrology.modelzoo.cudalstm import CudaLSTM
 from neuralhydrology.modelzoo.customlstm import CustomLSTM
 from neuralhydrology.modelzoo.ealstm import EALSTM
 from neuralhydrology.modelzoo.embcudalstm import EmbCudaLSTM
+from neuralhydrology.modelzoo.handoff_forecast_lstm import HandoffForecastLSTM
 from neuralhydrology.modelzoo.gru import GRU
 from neuralhydrology.modelzoo.mclstm import MCLSTM
 from neuralhydrology.modelzoo.mtslstm import MTSLSTM
+from neuralhydrology.modelzoo.multihead_forecast_lstm import MultiHeadForecastLSTM
 from neuralhydrology.modelzoo.odelstm import ODELSTM
+from neuralhydrology.modelzoo.sequential_forecast_lstm import SequentialForecastLSTM
+from neuralhydrology.modelzoo.stacked_forecast_lstm import StackedForecastLSTM
 from neuralhydrology.modelzoo.transformer import Transformer
 from neuralhydrology.utils.config import Config
 
-SINGLE_FREQ_MODELS = ["cudalstm", "ealstm", "customlstm", "embcudalstm", "gru", "transformer", "mclstm", "arlstm"]
+SINGLE_FREQ_MODELS = [
+    "cudalstm", 
+    "ealstm", 
+    "customlstm", 
+    "embcudalstm", 
+    "gru", 
+    "transformer", 
+    "mclstm", 
+    "arlstm",
+    "handoff_forecast_lstm",
+    "sequential_forecast_lstm",
+    "multihead_forecast_lstm",
+    "stacked_forecast_lstm"
+]
 AUTOREGRESSIVE_MODELS = ['arlstm']
 
 
 def get_model(cfg: Config) -> nn.Module:
     """Get model object, depending on the run configuration.
     
     Parameters
@@ -61,11 +78,19 @@
         model = MTSLSTM(cfg=cfg)
     elif cfg.model.lower() == "odelstm":
         model = ODELSTM(cfg=cfg)
     elif cfg.model.lower() == "mclstm":
         model = MCLSTM(cfg=cfg)
     elif cfg.model.lower() == "transformer":
         model = Transformer(cfg=cfg)
+    elif cfg.model.lower() == "handoff_forecast_lstm":
+        model = HandoffForecastLSTM(cfg=cfg)
+    elif cfg.model.lower() == "multihead_forecast_lstm":
+        model = MultiHeadForecastLSTM(cfg=cfg)
+    elif cfg.model.lower() == "sequential_forecast_lstm":
+        model = SequentialForecastLSTM(cfg=cfg)
+    elif cfg.model.lower() == "stacked_forecast_lstm":
+        model = StackedForecastLSTM(cfg=cfg)
     else:
         raise NotImplementedError(f"{cfg.model} not implemented or not linked in `get_model()`")
 
     return model
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/arlstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/arlstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/basemodel.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/basemodel.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/cudalstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/cudalstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/customlstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/customlstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/ealstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/ealstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/embcudalstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/embcudalstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/fc.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/fc.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/gru.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/gru.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/head.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/head.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/inputlayer.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/inputlayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch.nn as nn
 
 from neuralhydrology.modelzoo.fc import FC
 from neuralhydrology.utils.config import Config
 
 LOGGER = logging.getLogger(__name__)
 
+_EMBEDDING_TYPES = ['full_model', 'hindcast', 'forecast']
 
 class InputLayer(nn.Module):
     """Input layer to preprocess static and dynamic inputs.
 
     This module provides optional embedding of dynamic and static inputs. If ``dynamic_embeddings`` or
     ``static_embeddings`` are specified as dictionaries in the config, a fully-connected embedding network will be
     prepended to the timeseries model. The dictionaries have the following keys:
@@ -29,24 +30,37 @@
 
     Parameters
     ----------
     cfg : Config
         The run configuration
     """
 
-    def __init__(self, cfg: Config):
+    def __init__(self, cfg: Config, embedding_type: str = 'full_model'):
         super(InputLayer, self).__init__()
 
-        if isinstance(cfg.dynamic_inputs, dict):
-            frequencies = list(cfg.dynamic_inputs.keys())
+        if embedding_type not in _EMBEDDING_TYPES:
+            raise ValueError(
+                f'Embedding type {embedding_type} is not recognized. '
+                f'Must be one of: {_EMBEDDING_TYPES}.'
+            )
+        self.embedding_type = embedding_type
+        if embedding_type == 'full_model':
+            dynamic_inputs = cfg.dynamic_inputs
+        elif embedding_type == 'forecast':
+            dynamic_inputs = cfg.forecast_inputs
+        elif embedding_type == 'hindcast':
+            dynamic_inputs = cfg.hindcast_inputs
+            
+        if isinstance(dynamic_inputs, dict):
+            frequencies = list(dynamic_inputs.keys())
             if len(frequencies) > 1:
                 raise ValueError('InputLayer only supports single-frequency data')
-            dynamics_input_size = len(cfg.dynamic_inputs[frequencies[0]])
+            dynamics_input_size = len(dynamic_inputs[frequencies[0]])
         else:
-            dynamics_input_size = len(cfg.dynamic_inputs)
+            dynamics_input_size = len(dynamic_inputs)
 
         self._num_autoregression_inputs = 0
         if cfg.autoregressive_inputs:
             self._num_autoregression_inputs = len(cfg.autoregressive_inputs)
 
         statics_input_size = len(cfg.static_attributes + cfg.hydroatlas_attributes + cfg.evolving_attributes)
         if cfg.use_basin_id_encoding:
@@ -125,15 +139,21 @@
         Returns
         -------
         Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]
             If `concatenate_output` is True, a single tensor is returned. Else, a tuple with one tensor of dynamic
             inputs and one tensor of static inputs.
         """
         # transpose to [seq_length, batch_size, n_features]
-        x_d = data['x_d'].transpose(0, 1)
+        if self.embedding_type == 'full_model':
+            data_type = 'x_d'
+        elif self.embedding_type == 'forecast':
+            data_type = 'x_f'
+        elif self.embedding_type == 'hindcast':
+            data_type = 'x_h'
+        x_d = data[data_type].transpose(0, 1)
 
         if 'x_s' in data and 'x_one_hot' in data:
             x_s = torch.cat([data['x_s'], data['x_one_hot']], dim=-1)
         elif 'x_s' in data:
             x_s = data['x_s']
         elif 'x_one_hot' in data:
             x_s = data['x_one_hot']
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/mclstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/mclstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/mtslstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/mtslstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/odelstm.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/odelstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/template.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/template.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/modelzoo/transformer.py` & `neuralhydrology-1.8.0/neuralhydrology/modelzoo/transformer.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/nh_run.py` & `neuralhydrology-1.8.0/neuralhydrology/nh_run.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/nh_run_scheduler.py` & `neuralhydrology-1.8.0/neuralhydrology/nh_run_scheduler.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/training/__init__.py` & `neuralhydrology-1.8.0/neuralhydrology/training/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,11 +93,13 @@
         if isinstance(reg_item, str):
             reg_name = reg_item
             reg_weight = 1.0
         else:
             reg_name, reg_weight = reg_item
         if reg_name == "tie_frequencies":
             regularization_modules.append(regularization.TiedFrequencyMSERegularization(cfg=cfg, weight=reg_weight))
+        elif reg_name == "forecast_overlap":
+            regularization_modules.append(regularization.ForecastOverlapMSERegularization(cfg=cfg, weight=reg_weight))
         else:
             raise NotImplementedError(f"{reg_name} not implemented or not linked in `get_regularization_obj()`.")
 
     return regularization_modules
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/training/basetrainer.py` & `neuralhydrology-1.8.0/neuralhydrology/training/basetrainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         self.loader = None
         self.validator = None
         self.noise_sampler_y = None
         self._target_mean = None
         self._target_std = None
         self._scaler = {}
         self._allow_subsequent_nan_losses = cfg.allow_subsequent_nan_losses
+        self._disable_pbar = cfg.verbose == 0
 
         # load train basin list and add number of basins to the config
         self.basins = load_basin_file(cfg.train_basin_file)
         self.cfg.number_of_basins = len(self.basins)
 
         # check at which epoch the training starts
         self._epoch = self._get_start_epoch_number()
@@ -217,14 +218,15 @@
 
             if epoch % self.cfg.save_weights_every == 0:
                 self._save_weights_and_optimizer(epoch)
 
             if (self.validator is not None) and (epoch % self.cfg.validate_every == 0):
                 self.validator.evaluate(epoch=epoch,
                                         save_results=self.cfg.save_validation_results,
+                                        save_all_output=self.cfg.save_all_output,
                                         metrics=self.cfg.metrics,
                                         model=self.model,
                                         experiment_logger=self.experiment_logger.valid())
 
                 valid_metrics = self.experiment_logger.summarise()
                 print_msg = f"Epoch {epoch} average validation loss: {valid_metrics['avg_total_loss']:.5f}"
                 if self.cfg.metrics:
@@ -269,15 +271,15 @@
         torch.save(self.optimizer.state_dict(), str(optimizer_path))
 
     def _train_epoch(self, epoch: int):
         self.model.train()
         self.experiment_logger.train()
 
         # process bar handle
-        pbar = tqdm(self.loader, file=sys.stdout)
+        pbar = tqdm(self.loader, file=sys.stdout, disable=self._disable_pbar)
         pbar.set_description(f'# Epoch {epoch}')
 
         # Iterate in batches over training set
         nan_count = 0
         for data in pbar:
 
             for key in data.keys():
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/training/logger.py` & `neuralhydrology-1.8.0/neuralhydrology/training/logger.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/training/loss.py` & `neuralhydrology-1.8.0/neuralhydrology/training/loss.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/training/regularization.py` & `neuralhydrology-1.8.0/neuralhydrology/training/regularization.py`

 * *Files 20% similar despite different names*

```diff
@@ -107,7 +107,49 @@
             freq_pred = prediction[f'y_hat_{freq}']
             mean_freq_pred = freq_pred.view(freq_pred.shape[0], freq_pred.shape[1] // frequency_factor,
                                             frequency_factor, -1).mean(dim=2)
             lower_freq_pred = prediction[f'y_hat_{self._frequencies[idx - 1]}'][:, -mean_freq_pred.shape[1]:]
             loss = loss + torch.mean((lower_freq_pred - mean_freq_pred)**2)
 
         return loss
+
+class ForecastOverlapMSERegularization(BaseRegularization):
+    """Squared error regularization for penalizing differences between hindcast and forecast models.
+
+    Parameters
+    ----------
+    cfg : Config
+        The run configuration.
+    """
+
+    def forward(self, prediction: Dict[str, torch.Tensor], ground_truth: Dict[str, torch.Tensor],
+                *args) -> torch.Tensor:
+        """Calculate the squared difference between hindcast and forecast model during overlap.
+
+        Does not work with multi-frequency models.
+
+        Parameters
+        ----------
+        prediction : Dict[str, torch.Tensor]
+            Dictionary containing ``y_hindcast_overlap}`` and ``y_forecast_overlap``.
+        ground_truth : Dict[str, torch.Tensor]
+            Dictionary continaing ``y_{frequency}`` for !one! frequency.
+
+        Returns
+        -------
+        torch.Tensor
+            The sum of mean squared deviations between overlapping portions of hindcast and forecast models.
+
+        Raises
+        ------
+        ValueError if y_hindcast_overlap or y_forecast_overlap is not present in model output.
+        """
+        loss = 0
+        if 'y_hindcast_overlap' not in prediction or not prediction['y_hindcast_overlap']:
+            raise ValueError('y_hindcast_overlap is not present in the model output.')
+        if 'y_forecast_overlap' not in prediction or not prediction['y_forecast_overlap']:
+            raise ValueError('y_forecast_overlap is not present in the model output.')
+        for key in prediction['y_hindcast_overlap']:
+            hindcast = prediction['y_hindcast_overlap'][key]
+            forecast = prediction['y_forecast_overlap'][key]
+            loss += torch.mean((hindcast - forecast)**2)
+        return loss
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/training/train.py` & `neuralhydrology-1.8.0/neuralhydrology/training/train.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/utils/config.py` & `neuralhydrology-1.8.0/neuralhydrology/utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,14 +194,22 @@
                     cfg[key] = temp_list
                 else:
                     cfg[key] = pd.to_datetime(val, format='%d/%m/%Y')
 
             else:
                 pass
 
+        # Check forecast sequence length.
+        if cfg.get('forecast_seq_length'):
+            if cfg['forecast_seq_length'] >= cfg['seq_length']:
+                raise ValueError('Forecast sequence length must be < sequence length.')
+            if cfg.get('forecast_overlap'):
+                if cfg['forecast_overlap'] > cfg['forecast_seq_length']:
+                    raise ValueError('Forecast overlap must be <= forecast_seq_length.')
+
         # Check autoregressive inputs.
         if 'autoregressive_inputs' in cfg:
             if len(cfg['autoregressive_inputs']) > 1:
                 raise ValueError('Currently only one autoregressive input is supported.')
             if cfg['autoregressive_inputs'] and len(cfg['target_variables']) > 1:
                 raise ValueError('Autoregressive models currently only support a single target variable.')
             if not cfg['autoregressive_inputs'][0].startswith(cfg['target_variables'][0]):
@@ -244,14 +252,18 @@
         self._cfg["base_run_dir"] = folder
 
     @property
     def batch_size(self) -> int:
         return self._get_value_verbose("batch_size")
 
     @property
+    def bidirectional_stacked_forecast_lstm(self) -> bool:
+        return self._cfg.get("bidirectional_stacked_forecast_lstm", False)
+
+    @property
     def cache_validation_data(self) -> bool:
         return self._cfg.get("cache_validation_data", True)
 
     @property
     def checkpoint_path(self) -> Path:
         return self._cfg.get("checkpoint_path", None)
 
@@ -305,15 +317,15 @@
             raise RuntimeError(f"Unsupported type {type(duplicate_features)} for 'duplicate_features' argument.")
 
     @property
     def dynamic_inputs(self) -> Union[List[str], Dict[str, List[str]]]:
         return self._get_value_verbose("dynamic_inputs")
 
     @property
-    def dynamics_embedding(self) -> bool:
+    def dynamics_embedding(self) -> dict:
         embedding_spec = self._cfg.get("dynamics_embedding", None)
 
         if embedding_spec is None:
             return None
         return self._get_embedding_spec(embedding_spec)
 
     @property
@@ -346,33 +358,73 @@
             return [finetune_modules]
         elif isinstance(finetune_modules, dict) or isinstance(finetune_modules, list):
             return finetune_modules
         else:
             raise ValueError(f"Unknown data type {type(finetune_modules)} for 'finetune_modules' argument.")
 
     @property
+    def forecast_network(self) -> dict:
+        embedding_spec = self._cfg.get("forecast_network", None)
+
+        if embedding_spec is None:
+            return None
+        return self._get_embedding_spec(embedding_spec)
+
+    @property
+    def forecast_hidden_size(self) -> int:
+        return self._cfg.get("forecast_hidden_size", self.hidden_size)
+
+    @property
+    def forecast_inputs(self) -> List[str]:
+        return self._cfg.get("forecast_inputs", [])
+
+    @property
+    def forecast_overlap(self) -> int:
+        return self._cfg.get("forecast_overlap", None)
+
+    @property
+    def forecast_seq_length(self) -> int:
+        return self._cfg.get("forecast_seq_length", None)
+
+    @property
     def forcings(self) -> List[str]:
         return self._as_default_list(self._get_value_verbose("forcings"))
 
     @property
     def save_git_diff(self) -> bool:
         return self._cfg.get('save_git_diff', False)
 
     @property
+    def state_handoff_network(self) -> dict:
+        embedding_spec = self._cfg.get("state_handoff_network", None)
+
+        if embedding_spec is None:
+            return None
+        return self._get_embedding_spec(embedding_spec)
+
+    @property
     def head(self) -> str:
         if self.model == "mclstm":
             return ''
         else:
             return self._get_value_verbose("head")
 
     @property
+    def hindcast_inputs(self) -> List[str]:
+        return self._cfg.get("hindcast_inputs", [])
+
+    @property
     def hidden_size(self) -> Union[int, Dict[str, int]]:
         return self._get_value_verbose("hidden_size")
 
     @property
+    def hindcast_hidden_size(self) -> Union[int, Dict[str, int]]:
+        return self._cfg.get("hindcast_hidden_size", self.hidden_size)
+
+    @property
     def hydroatlas_attributes(self) -> List[str]:
         return self._as_default_list(self._cfg.get("hydroatlas_attributes", []))
 
     @property
     def img_log_dir(self) -> Path:
         return self._cfg.get("img_log_dir", None)
 
@@ -556,14 +608,18 @@
         self._cfg["run_dir"] = folder
 
     @property
     def save_train_data(self) -> bool:
         return self._cfg.get("save_train_data", False)
 
     @property
+    def save_all_output(self) -> bool:
+        return self._cfg.get('save_all_output', False)
+
+    @property
     def save_validation_results(self) -> bool:
         return self._cfg.get("save_validation_results", False)
 
     @property
     def save_weights_every(self) -> int:
         return self._cfg.get("save_weights_every", 1)
 
@@ -618,15 +674,15 @@
             warnings.warn("'camels_attributes' will be deprecated. Use 'static_attributes' in the future",
                           FutureWarning)
             return self._as_default_list(self._cfg["camels_attributes"])
         else:
             return []
 
     @property
-    def statics_embedding(self) -> bool:
+    def statics_embedding(self) -> dict:
         embedding_spec = self._cfg.get("statics_embedding", None)
 
         if embedding_spec is None:
             return None
         return self._get_embedding_spec(embedding_spec)
 
     @property
@@ -667,14 +723,18 @@
         return self._get_value_verbose("test_end_date")
 
     @property
     def test_start_date(self) -> pd.Timestamp:
         return self._get_value_verbose("test_start_date")
 
     @property
+    def timestep_counter(self) -> bool:
+        return self._cfg.get("timestep_counter", False)
+        
+    @property
     def train_basin_file(self) -> Path:
         return self._get_value_verbose("train_basin_file")
 
     @property
     def train_data_file(self) -> Path:
         return self._cfg.get("train_data_file", None)
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology/utils/configutils.py` & `neuralhydrology-1.8.0/neuralhydrology/utils/configutils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/utils/logging_utils.py` & `neuralhydrology-1.8.0/neuralhydrology/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/utils/nh_results_ensemble.py` & `neuralhydrology-1.8.0/neuralhydrology/utils/nh_results_ensemble.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/utils/ratingcurve.py` & `neuralhydrology-1.8.0/neuralhydrology/utils/ratingcurve.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/neuralhydrology/utils/samplingutils.py` & `neuralhydrology-1.8.0/neuralhydrology/utils/samplingutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,17 +138,25 @@
         # make model checks:
         cfg = model.cfg
         if not cfg.head.lower() == head.lower():
             raise NotImplementedError(f"{head} sampling not supported for the {cfg.head} head!")
 
         dropout_modules = [model.dropout.p]
 
-        # Multi-Timescale models don't have an embedding_net
+        # Certain models don't have embedding_net(s)
         implied_statics_embedding, implied_dynamics_embedding = None, None
-        if cfg.model.lower() not in ['mtslstm', 'odelstm']:
+        if hasattr(model, 'forecast_embedding_net'):
+            implied_forecast_statics_embedding = model.forecast_embedding_net.statics_embedding_p_dropout
+            implied_forecast_dynamics_embedding = model.forecast_embedding_net.dynamics_embedding_p_dropout
+            dropout_modules += [implied_forecast_statics_embedding, implied_forecast_dynamics_embedding]
+        if hasattr(model, 'hindcast_embedding_net'):
+            implied_hindcast_statics_embedding = model.hindcast_embedding_net.statics_embedding_p_dropout
+            implied_hindcast_dynamics_embedding = model.hindcast_embedding_net.dynamics_embedding_p_dropout
+            dropout_modules += [implied_hindcast_statics_embedding, implied_hindcast_dynamics_embedding]
+        if hasattr(model, 'embedding_net'):
             implied_statics_embedding = model.embedding_net.statics_embedding_p_dropout
             implied_dynamics_embedding = model.embedding_net.dynamics_embedding_p_dropout
             dropout_modules += [implied_statics_embedding, implied_dynamics_embedding]
         # account for transformer
         implied_transformer_dropout = None
         if cfg.model.lower() == 'transfomer':
             implied_transformer_dropout = cfg.transformer_dropout
@@ -158,22 +166,30 @@
         # check lower bound dropout:
         if cfg.mc_dropout and max_implied_dropout <= 0.0:
             raise RuntimeError(f"""{cfg.model} with `mc_dropout` activated requires a dropout rate larger than 0.0
                                The current implied dropout-rates are:
                                   - model: {cfg.output_dropout}
                                   - statics_embedding: {implied_statics_embedding}
                                   - dynamics_embedding: {implied_dynamics_embedding}
+                                  - statics_forecast_embedding: {implied_forecast_statics_embedding}
+                                  - dynamics_forecast_embedding: {implied_forecast_dynamics_embedding}
+                                  - statics_hindcast_embedding: {implied_hindcast_statics_embedding}
+                                  - dynamics_hindcast_embedding: {implied_hindcast_dynamics_embedding}
                                   - transformer: {implied_transformer_dropout}""")
         # check upper bound dropout:
         if cfg.mc_dropout and max_implied_dropout >= 1.0:
             raise RuntimeError(f"""The maximal dropout-rate is 1. Please check your dropout-settings:
                                The current implied dropout-rates are:
                                   - model: {cfg.output_dropout}
                                   - statics_embedding: {implied_statics_embedding}
                                   - dynamics_embedding: {implied_dynamics_embedding}
+                                  - statics_forecast_embedding: {implied_forecast_statics_embedding}
+                                  - dynamics_forecast_embedding: {implied_forecast_dynamics_embedding}
+                                  - statics_hindcast_embedding: {implied_hindcast_statics_embedding}
+                                  - dynamics_hindcast_embedding: {implied_hindcast_dynamics_embedding}
                                   - transformer: {implied_transformer_dropout}""")
 
         # assign setup properties:
         self.cfg = cfg
         self.device = next(model.parameters()).device
         self.number_of_targets = len(cfg.target_variables)
         self.mc_dropout = cfg.mc_dropout
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology.egg-info/PKG-INFO` & `neuralhydrology-1.8.0/neuralhydrology.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralhydrology
-Version: 1.7.0
+Version: 1.8.0
 Summary: Library for training deep learning models with environmental focus
 Home-page: https://neuralhydrology.readthedocs.io
 Author: Frederik Kratzert, Daniel Klotz, Martin Gauch
 Author-email: neuralhydrology@googlegroups.com
 Project-URL: Documentation, https://neuralhydrology.readthedocs.io
 Project-URL: Source, https://github.com/neuralhydrology/neuralhydrology
 Project-URL: Research Blog, https://neuralhydrology.github.io/
```

### Comparing `neuralhydrology-1.7.0/neuralhydrology.egg-info/SOURCES.txt` & `neuralhydrology-1.8.0/neuralhydrology.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,23 @@
 neuralhydrology/modelzoo/basemodel.py
 neuralhydrology/modelzoo/cudalstm.py
 neuralhydrology/modelzoo/customlstm.py
 neuralhydrology/modelzoo/ealstm.py
 neuralhydrology/modelzoo/embcudalstm.py
 neuralhydrology/modelzoo/fc.py
 neuralhydrology/modelzoo/gru.py
+neuralhydrology/modelzoo/handoff_forecast_lstm.py
 neuralhydrology/modelzoo/head.py
 neuralhydrology/modelzoo/inputlayer.py
 neuralhydrology/modelzoo/mclstm.py
 neuralhydrology/modelzoo/mtslstm.py
+neuralhydrology/modelzoo/multihead_forecast_lstm.py
 neuralhydrology/modelzoo/odelstm.py
+neuralhydrology/modelzoo/sequential_forecast_lstm.py
+neuralhydrology/modelzoo/stacked_forecast_lstm.py
 neuralhydrology/modelzoo/template.py
 neuralhydrology/modelzoo/transformer.py
 neuralhydrology/training/__init__.py
 neuralhydrology/training/basetrainer.py
 neuralhydrology/training/logger.py
 neuralhydrology/training/loss.py
 neuralhydrology/training/regularization.py
```

### Comparing `neuralhydrology-1.7.0/setup.py` & `neuralhydrology-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/test/test_config_runs.py` & `neuralhydrology-1.8.0/test/test_config_runs.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/test/test_custom_lstm.py` & `neuralhydrology-1.8.0/test/test_custom_lstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/test/test_datautils.py` & `neuralhydrology-1.8.0/test/test_datautils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.7.0/test/test_mclstm.py` & `neuralhydrology-1.8.0/test/test_mclstm.py`

 * *Files identical despite different names*

