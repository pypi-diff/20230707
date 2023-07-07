# Comparing `tmp/subaligner-0.3.3.tar.gz` & `tmp/subaligner-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subaligner-0.3.3.tar", last modified: Fri Jun  9 18:01:02 2023, max compression
+gzip compressed data, was "dist/subaligner-0.3.4.tar", last modified: Fri Jul  7 08:03:08 2023, max compression
```

## Comparing `subaligner-0.3.3.tar` & `subaligner-0.3.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.260026 subaligner-0.3.3/
--rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.3/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.3/MANIFEST.in
--rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 18:01:02.259467 subaligner-0.3.3/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     9247 2023-04-15 17:31:09.000000 subaligner-0.3.3/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.176880 subaligner-0.3.3/bin/
--rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.3/bin/subaligner
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.3/bin/subaligner_1pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.3/bin/subaligner_2pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.3/bin/subaligner_batch
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.3/bin/subaligner_convert
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.3/bin/subaligner_train
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.3/bin/subaligner_tune
--rw-r--r--   0 macbook    (501) staff       (20)     1185 2023-06-09 08:34:37.000000 subaligner-0.3.3/requirements.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-09 18:01:02.260151 subaligner-0.3.3/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     3748 2023-06-08 23:47:15.000000 subaligner-0.3.3/setup.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.197970 subaligner-0.3.3/subaligner/
--rw-r--r--   0 macbook    (501) staff       (20)      258 2023-03-11 16:33:37.000000 subaligner-0.3.3/subaligner/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.3/subaligner/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)       64 2023-06-09 17:58:20.000000 subaligner-0.3.3/subaligner/_version.py
--rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/embedder.py
--rw-r--r--   0 macbook    (501) staff       (20)      511 2023-03-11 23:58:14.000000 subaligner-0.3.3/subaligner/exception.py
--rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/hparam_tuner.py
--rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/hyperparameters.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.231693 subaligner-0.3.3/subaligner/lib/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/lib/language.py
--rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/lib/to_srt.py
--rw-r--r--   0 macbook    (501) staff       (20)      709 2023-03-19 19:33:51.000000 subaligner-0.3.3/subaligner/llm.py
--rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)    18286 2023-03-17 01:31:21.000000 subaligner-0.3.3/subaligner/media_helper.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.164770 subaligner-0.3.3/subaligner/models/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.165377 subaligner-0.3.3/subaligner/models/training/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.233276 subaligner-0.3.3/subaligner/models/training/config/
--rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/config/hyperparameters.json
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.234957 subaligner-0.3.3/subaligner/models/training/model/
--rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/model/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/model/model.hdf5
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.247728 subaligner-0.3.3/subaligner/models/training/weights/
--rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/weights/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/models/training/weights/weights.hdf5
--rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/network.py
--rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/singleton.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.254200 subaligner-0.3.3/subaligner/subaligner_1pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_1pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/subaligner_1pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.255055 subaligner-0.3.3/subaligner/subaligner_2pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_2pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/subaligner_2pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.256216 subaligner-0.3.3/subaligner/subaligner_batch/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_batch/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.3/subaligner/subaligner_batch/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.257204 subaligner-0.3.3/subaligner/subaligner_convert/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_convert/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.3/subaligner/subaligner_convert/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.258139 subaligner-0.3.3/subaligner/subaligner_train/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_train/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.3/subaligner/subaligner_train/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.258912 subaligner-0.3.3/subaligner/subaligner_tune/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_tune/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.3/subaligner/subaligner_tune/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-04-15 16:48:57.000000 subaligner-0.3.3/subaligner/subtitle.py
--rw-r--r--   0 macbook    (501) staff       (20)    15876 2023-06-06 00:57:05.000000 subaligner-0.3.3/subaligner/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     4695 2023-06-09 19:42:27.000000 subaligner-0.3.3/subaligner/transcriber.py
--rw-r--r--   0 macbook    (501) staff       (20)    12182 2023-06-06 09:49:57.000000 subaligner-0.3.3/subaligner/translator.py
--rw-r--r--   0 macbook    (501) staff       (20)    33741 2023-03-17 02:05:09.000000 subaligner-0.3.3/subaligner/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 18:01:02.228454 subaligner-0.3.3/subaligner.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1628 2023-06-09 18:01:02.000000 subaligner-0.3.3/subaligner.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      424 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)     2015 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-06-09 18:01:01.000000 subaligner-0.3.3/subaligner.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.810333 subaligner-0.3.4/
+-rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.4/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.4/MANIFEST.in
+-rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-07-07 08:03:08.809193 subaligner-0.3.4/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     9247 2023-04-15 17:31:09.000000 subaligner-0.3.4/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.618817 subaligner-0.3.4/bin/
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.4/bin/subaligner
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.4/bin/subaligner_1pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.4/bin/subaligner_2pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.4/bin/subaligner_batch
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.4/bin/subaligner_convert
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.4/bin/subaligner_train
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.4/bin/subaligner_tune
+-rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-07-05 22:41:18.000000 subaligner-0.3.4/requirements.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-07-07 08:03:08.810556 subaligner-0.3.4/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     4084 2023-07-05 22:53:21.000000 subaligner-0.3.4/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.675208 subaligner-0.3.4/subaligner/
+-rw-r--r--   0 macbook    (501) staff       (20)      258 2023-03-11 16:33:37.000000 subaligner-0.3.4/subaligner/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.4/subaligner/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)       64 2023-07-05 22:45:57.000000 subaligner-0.3.4/subaligner/_version.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/embedder.py
+-rw-r--r--   0 macbook    (501) staff       (20)      511 2023-03-11 23:58:14.000000 subaligner-0.3.4/subaligner/exception.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/hparam_tuner.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/hyperparameters.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.729303 subaligner-0.3.4/subaligner/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/lib/language.py
+-rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/lib/to_srt.py
+-rw-r--r--   0 macbook    (501) staff       (20)      709 2023-03-19 19:33:51.000000 subaligner-0.3.4/subaligner/llm.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)    18286 2023-03-17 01:31:21.000000 subaligner-0.3.4/subaligner/media_helper.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.603186 subaligner-0.3.4/subaligner/models/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.603803 subaligner-0.3.4/subaligner/models/training/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.735510 subaligner-0.3.4/subaligner/models/training/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/models/training/config/hyperparameters.json
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.738092 subaligner-0.3.4/subaligner/models/training/model/
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/models/training/model/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/models/training/model/model.hdf5
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.772463 subaligner-0.3.4/subaligner/models/training/weights/
+-rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/models/training/weights/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/models/training/weights/weights.hdf5
+-rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/network.py
+-rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 19:10:53.000000 subaligner-0.3.4/subaligner/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/singleton.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.781762 subaligner-0.3.4/subaligner/subaligner_1pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/subaligner_1pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.4/subaligner/subaligner_1pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.782790 subaligner-0.3.4/subaligner/subaligner_2pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/subaligner_2pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.4/subaligner/subaligner_2pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.784901 subaligner-0.3.4/subaligner/subaligner_batch/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/subaligner_batch/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.4/subaligner/subaligner_batch/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.803907 subaligner-0.3.4/subaligner/subaligner_convert/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/subaligner_convert/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.4/subaligner/subaligner_convert/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.806434 subaligner-0.3.4/subaligner/subaligner_train/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/subaligner_train/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.4/subaligner/subaligner_train/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.808034 subaligner-0.3.4/subaligner/subaligner_tune/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/subaligner_tune/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.4/subaligner/subaligner_tune/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-04-15 16:48:57.000000 subaligner-0.3.4/subaligner/subtitle.py
+-rw-r--r--   0 macbook    (501) staff       (20)    15876 2023-06-06 00:57:05.000000 subaligner-0.3.4/subaligner/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4792 2023-06-18 11:51:47.000000 subaligner-0.3.4/subaligner/transcriber.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12182 2023-06-06 09:49:57.000000 subaligner-0.3.4/subaligner/translator.py
+-rw-r--r--   0 macbook    (501) staff       (20)    33741 2023-03-17 02:05:09.000000 subaligner-0.3.4/subaligner/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-07 08:03:08.726668 subaligner-0.3.4/subaligner.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-07-07 08:03:08.000000 subaligner-0.3.4/subaligner.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1628 2023-07-07 08:03:08.000000 subaligner-0.3.4/subaligner.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-07-07 08:03:08.000000 subaligner-0.3.4/subaligner.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      424 2023-07-07 08:03:08.000000 subaligner-0.3.4/subaligner.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)     1975 2023-07-07 08:03:08.000000 subaligner-0.3.4/subaligner.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-07-07 08:03:08.000000 subaligner-0.3.4/subaligner.egg-info/top_level.txt
```

### Comparing `subaligner-0.3.3/LICENSE` & `subaligner-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/PKG-INFO` & `subaligner-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subaligner
-Version: 0.3.3
+Version: 0.3.4
 Summary: Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.
 Home-page: https://subaligner.readthedocs.io/en/latest/
 Author: Xi Bai
 Author-email: xi.bai.ed@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `subaligner-0.3.3/README.md` & `subaligner-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/bin/subaligner` & `subaligner-0.3.4/bin/subaligner`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/bin/subaligner_1pass` & `subaligner-0.3.4/bin/subaligner_1pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/bin/subaligner_2pass` & `subaligner-0.3.4/bin/subaligner_2pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/bin/subaligner_batch` & `subaligner-0.3.4/bin/subaligner_batch`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/bin/subaligner_convert` & `subaligner-0.3.4/bin/subaligner_convert`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/bin/subaligner_train` & `subaligner-0.3.4/bin/subaligner_train`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/bin/subaligner_tune` & `subaligner-0.3.4/bin/subaligner_tune`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/requirements.txt` & `subaligner-0.3.4/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -49,16 +49,14 @@
 pydotplus==2.0.2
 pyprof2calltree==1.4.3
 pysrt==1.1.1
 pysubs2<=1.4.2
 pystack-debugger==0.8.0
 pytz==2018.4
 PyYAML>=4.2b1
-requests<3.0.0
-requests-oauthlib==1.3.0
 rsa==4.7
 scipy<=1.8.1
 scikit-learn<1.2.0
 setuptools>=41.0.0
 six~=1.15.0
 tblib==1.3.2
 tensorflow>=1.15.5,<2.13
```

### Comparing `subaligner-0.3.3/setup.py` & `subaligner-0.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import os
+import platform
 
 from setuptools import setup
 
 with open(os.path.join(os.getcwd(), "subaligner", "_version.py")) as f:
     exec(f.read())
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
+if platform.machine() == "arm64":
+    with open("requirements-aarch64.txt") as requirements_file:
+        requirements = requirements_file.read().splitlines()[::-1]
+else:
+    with open("requirements.txt") as requirements_file:
+        requirements = requirements_file.read().splitlines()[::-1]
+
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()[::-1]
 
 with open("requirements-stretch.txt") as stretch_requirements_file:
     stretch_requirements = stretch_requirements_file.read().splitlines()[::-1]
 
 with open("requirements-site.txt") as docs_requirements_file:
@@ -48,14 +56,15 @@
       ],
       license="MIT",
       url="https://subaligner.readthedocs.io/en/latest/",
       description="Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.",
       long_description=readme + "\n\n",
       long_description_content_type='text/markdown',
       python_requires=">=3.8",
+      wheel=True,
       package_dir={"subaligner": "subaligner"},
       packages=[
           "subaligner",
           "subaligner.lib",
           "subaligner.subaligner_1pass",
           "subaligner.subaligner_2pass",
           "subaligner.subaligner_batch",
@@ -88,8 +97,9 @@
               "subaligner=subaligner.__main__:main",
               "subaligner_1pass=subaligner.subaligner_1pass.__main__:main",
               "subaligner_2pass=subaligner.subaligner_2pass.__main__:main",
               "subaligner_batch=subaligner.subaligner_batch.__main__:main",
               "subaligner_convert=subaligner.subaligner_convert.__main__:main",
               "subaligner_train=subaligner.subaligner_train.__main__:main",
               "subaligner_tune=subaligner.subaligner_tune.__main__:main",
-          ]})
+          ]
+      })
```

### Comparing `subaligner-0.3.3/subaligner/__main__.py` & `subaligner-0.3.4/subaligner/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/embedder.py` & `subaligner-0.3.4/subaligner/embedder.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/hparam_tuner.py` & `subaligner-0.3.4/subaligner/hparam_tuner.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/hyperparameters.py` & `subaligner-0.3.4/subaligner/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/lib/language.py` & `subaligner-0.3.4/subaligner/lib/language.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/lib/to_srt.py` & `subaligner-0.3.4/subaligner/lib/to_srt.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/llm.py` & `subaligner-0.3.4/subaligner/llm.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/logger.py` & `subaligner-0.3.4/subaligner/logger.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/media_helper.py` & `subaligner-0.3.4/subaligner/media_helper.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/models/training/config/hyperparameters.json` & `subaligner-0.3.4/subaligner/models/training/config/hyperparameters.json`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/models/training/model/model.hdf5` & `subaligner-0.3.4/subaligner/models/training/model/model.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/models/training/weights/weights.hdf5` & `subaligner-0.3.4/subaligner/models/training/weights/weights.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/network.py` & `subaligner-0.3.4/subaligner/network.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/predictor.py` & `subaligner-0.3.4/subaligner/predictor.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/subaligner_1pass/__main__.py` & `subaligner-0.3.4/subaligner/subaligner_1pass/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/subaligner_2pass/__main__.py` & `subaligner-0.3.4/subaligner/subaligner_2pass/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/subaligner_batch/__main__.py` & `subaligner-0.3.4/subaligner/subaligner_batch/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/subaligner_convert/__main__.py` & `subaligner-0.3.4/subaligner/subaligner_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/subaligner_train/__main__.py` & `subaligner-0.3.4/subaligner/subaligner_train/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/subaligner_tune/__main__.py` & `subaligner-0.3.4/subaligner/subaligner_tune/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/subtitle.py` & `subaligner-0.3.4/subaligner/subtitle.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/trainer.py` & `subaligner-0.3.4/subaligner/trainer.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/transcriber.py` & `subaligner-0.3.4/subaligner/transcriber.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,17 @@
         if self.__recipe == "whisper":
             lang = Utils.get_iso_639_alpha_2(language_code)
             if lang not in LANGUAGES:
                 raise TranscriptionException(f'"{language_code}" is not supported by {self.__recipe} ({self.__flavour})')
             audio_file_path = self.__media_helper.extract_audio(video_file_path, True, 16000)
             try:
                 audio = whisper.load_audio(audio_file_path)
-                self.__LOGGER.debug("Start transcribing the audio...")
-                result = self.__model.transcribe(audio, task="transcribe", language=LANGUAGES[lang])
+                self.__LOGGER.info("Start transcribing the audio...")
+                verbose = False if Logger.VERBOSE and not Logger.QUIET else None
+                result = self.__model.transcribe(audio, task="transcribe", language=LANGUAGES[lang], verbose=verbose)
                 self.__LOGGER.info("Finished transcribing the audio")
                 srt_str = ""
                 for i, segment in enumerate(result["segments"], start=1):
                     srt_str += f"{i}\n" \
                                f"{Utils.format_timestamp(segment['start'])} --> {Utils.format_timestamp(segment['end'])}\n" \
                                f"{segment['text'].strip().replace('-->', '->')}\n" \
                                "\n"
```

### Comparing `subaligner-0.3.3/subaligner/translator.py` & `subaligner-0.3.4/subaligner/translator.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner/utils.py` & `subaligner-0.3.4/subaligner/utils.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner.egg-info/PKG-INFO` & `subaligner-0.3.4/subaligner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subaligner
-Version: 0.3.3
+Version: 0.3.4
 Summary: Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.
 Home-page: https://subaligner.readthedocs.io/en/latest/
 Author: Xi Bai
 Author-email: xi.bai.ed@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `subaligner-0.3.3/subaligner.egg-info/SOURCES.txt` & `subaligner-0.3.4/subaligner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.3/subaligner.egg-info/requires.txt` & `subaligner-0.3.4/subaligner.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 tensorflow<2.13,>=1.15.5
 tblib==1.3.2
 six~=1.15.0
 setuptools>=41.0.0
 scikit-learn<1.2.0
 scipy<=1.8.1
 rsa==4.7
-requests-oauthlib==1.3.0
-requests<3.0.0
 PyYAML>=4.2b1
 pytz==2018.4
 pystack-debugger==0.8.0
 pysubs2<=1.4.2
 pysrt==1.1.1
 pyprof2calltree==1.4.3
 pydotplus==2.0.2
@@ -85,41 +83,41 @@
 snakeviz==2.1.0
 twine<4.0.0
 pycodestyle==2.5.0
 tox~=3.23.0
 coverage==5.5
 mock==4.0.3
 aeneas~=1.7.3.0
-openai-whisper==20230124
+openai-whisper==20230314
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
 docutils~=0.17.0
 sphinx-rtd-theme==0.5.0
 sphinx==3.3.1
 
 [docs]
 docutils~=0.17.0
 sphinx-rtd-theme==0.5.0
 sphinx==3.3.1
 
 [harmony]
 aeneas~=1.7.3.0
-openai-whisper==20230124
+openai-whisper==20230314
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
 
 [llm]
-openai-whisper==20230124
+openai-whisper==20230314
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
 
 [stretch]
 aeneas~=1.7.3.0
 
 [translation]
-openai-whisper==20230124
+openai-whisper==20230314
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
```

