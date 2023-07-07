# Comparing `tmp/prismstudio-1.1.5.tar.gz` & `tmp/prismstudio-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-1.1.5.tar", last modified: Thu Jul  6 01:27:24 2023, max compression
+gzip compressed data, was "prismstudio-1.1.6.tar", last modified: Fri Jul  7 03:19:31 2023, max compression
```

## Comparing `prismstudio-1.1.5.tar` & `prismstudio-1.1.6.tar`

### file list

```diff
@@ -1,63 +1,89 @@
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.010098 prismstudio-1.1.5/
--rw-rw-r--   0 prism     (1000) prism     (1000)      392 2023-07-06 01:27:24.010098 prismstudio-1.1.5/PKG-INFO
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.006097 prismstudio-1.1.5/prism/
--rw-rw-r--   0 prism     (1000) prism     (1000)     4630 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.006097 prismstudio-1.1.5/prism/_common/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1059 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_common/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15651 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_common/config.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    48951 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_common/const.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.006097 prismstudio-1.1.5/prism/_core/
--rw-rw-r--   0 prism     (1000) prism     (1000)     2419 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.010098 prismstudio-1.1.5/prism/_core/_data/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1075 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   165243 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/estimate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    34215 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/event.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   283107 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/financial.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    53787 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/index.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   484407 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/industry.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   152627 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/market.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    28511 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/precalculated.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    17575 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_data/securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    67035 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_fn.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.010098 prismstudio-1.1.5/prism/_core/_req_builder/
--rw-rw-r--   0 prism     (1000) prism     (1000)     8355 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     8147 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_auth.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    89231 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_dataquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     9611 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_dbinfo.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    31711 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_exportdata.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    18951 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_gui.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    67399 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_job.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    21663 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_list.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    59387 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_portfolio.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    19031 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    99491 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_task.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    43783 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_taskquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    93991 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/_universe.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    39475 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/_req_builder/preference.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    40035 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_core/ols.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.010098 prismstudio-1.1.5/prism/_prismcomponent/
--rw-rw-r--   0 prism     (1000) prism     (1000)     2391 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_prismcomponent/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    32207 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_prismcomponent/abstract_prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   123835 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_prismcomponent/datacomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   802319 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_prismcomponent/prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    75355 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_prismcomponent/taskcomponent.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.010098 prismstudio-1.1.5/prism/_utils/
--rw-rw-r--   0 prism     (1000) prism     (1000)     3563 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    13915 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/auth_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    27659 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/exceptions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    14479 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/loader.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    21259 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/prismcomponent_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    22599 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/req_builder_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    53595 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/validate_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    35783 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/_utils/validate_utils_refactored.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.010098 prismstudio-1.1.5/prism/pytransform/
--rw-rw-r--   0 prism     (1000) prism     (1000)    13587 2023-06-18 11:30:13.000000 prismstudio-1.1.5/prism/pytransform/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)  1198080 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prism/pytransform/_pytransform.so
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-06 01:27:24.010098 prismstudio-1.1.5/prismstudio.egg-info/
--rw-rw-r--   0 prism     (1000) prism     (1000)      392 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prismstudio.egg-info/PKG-INFO
--rw-rw-r--   0 prism     (1000) prism     (1000)     1639 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prismstudio.egg-info/SOURCES.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prismstudio.egg-info/dependency_links.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      256 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prismstudio.egg-info/requires.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)        6 2023-07-06 01:27:23.000000 prismstudio-1.1.5/prismstudio.egg-info/top_level.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-06 01:27:24.010098 prismstudio-1.1.5/setup.cfg
--rw-rw-r--   0 prism     (1000) prism     (1000)     1299 2023-07-06 01:27:23.000000 prismstudio-1.1.5/setup.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.443140 prismstudio-1.1.6/
+-rw-rw-r--   0 prism     (1000) prism     (1000)    23016 2023-07-07 02:52:00.000000 prismstudio-1.1.6/LICENSE.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)      440 2023-07-07 03:19:31.443140 prismstudio-1.1.6/PKG-INFO
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.439140 prismstudio-1.1.6/prism/
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1177 2023-07-07 02:42:51.000000 prismstudio-1.1.6/prism/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.439140 prismstudio-1.1.6/prism/_common/
+-rw-rw-r--   0 prism     (1000) prism     (1000)       35 2023-07-07 03:19:28.000000 prismstudio-1.1.6/prism/_common/.env
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_common/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3449 2023-07-07 03:06:42.000000 prismstudio-1.1.6/prism/_common/config.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    10161 2023-06-14 16:37:45.000000 prismstudio-1.1.6/prism/_common/const.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.439140 prismstudio-1.1.6/prism/_core/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      251 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.439140 prismstudio-1.1.6/prism/_core/_data/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_data/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    41177 2023-06-16 00:01:45.000000 prismstudio-1.1.6/prism/_core/_data/estimate.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7950 2023-06-16 00:01:45.000000 prismstudio-1.1.6/prism/_core/_data/event.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    70720 2023-06-30 07:00:13.000000 prismstudio-1.1.6/prism/_core/_data/financial.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    12859 2023-06-27 09:00:21.000000 prismstudio-1.1.6/prism/_core/_data/index.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)   121051 2023-06-16 00:01:45.000000 prismstudio-1.1.6/prism/_core/_data/industry.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    36768 2023-07-07 02:42:51.000000 prismstudio-1.1.6/prism/_core/_data/market.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     6446 2023-06-16 00:01:45.000000 prismstudio-1.1.6/prism/_core/_data/precalculated.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3840 2023-06-14 16:37:45.000000 prismstudio-1.1.6/prism/_core/_data/securitymaster.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15625 2023-06-15 23:39:09.000000 prismstudio-1.1.6/prism/_core/_fn.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.439140 prismstudio-1.1.6/prism/_core/_req_builder/
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1458 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1450 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/_auth.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    22657 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/_dataquery.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2058 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/_dbinfo.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7633 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/_exportdata.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3633 2023-06-15 23:39:09.000000 prismstudio-1.1.6/prism/_core/_req_builder/_gui.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15003 2023-06-14 16:37:45.000000 prismstudio-1.1.6/prism/_core/_req_builder/_job.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     4582 2023-06-14 16:37:45.000000 prismstudio-1.1.6/prism/_core/_req_builder/_list.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15321 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/_portfolio.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     4295 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/_securitymaster.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    25699 2023-06-15 23:39:09.000000 prismstudio-1.1.6/prism/_core/_req_builder/_task.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    10877 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/_taskquery.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    24533 2023-06-14 16:37:45.000000 prismstudio-1.1.6/prism/_core/_req_builder/_universe.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     8696 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/_req_builder/preference.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     9606 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_core/ols.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.439140 prismstudio-1.1.6/prism/_prismcomponent/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      353 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_prismcomponent/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7323 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_prismcomponent/abstract_prismcomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    14370 2023-06-14 16:37:45.000000 prismstudio-1.1.6/prism/_prismcomponent/datacomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)   185597 2023-06-15 23:39:09.000000 prismstudio-1.1.6/prism/_prismcomponent/prismcomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    21567 2023-07-07 02:42:51.000000 prismstudio-1.1.6/prism/_prismcomponent/taskcomponent.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.443140 prismstudio-1.1.6/prism/_utils/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      480 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2248 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/auth_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3629 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/exceptions.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2028 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/loader.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3706 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/prismcomponent_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     5532 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/req_builder_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    14289 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/validate_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7232 2023-06-12 06:52:36.000000 prismstudio-1.1.6/prism/_utils/validate_utils_refactored.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1438 2023-07-07 02:42:51.000000 prismstudio-1.1.6/prism/_utils/version.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.443140 prismstudio-1.1.6/prismstudio.egg-info/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      440 2023-07-07 03:19:31.000000 prismstudio-1.1.6/prismstudio.egg-info/PKG-INFO
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3022 2023-07-07 03:19:31.000000 prismstudio-1.1.6/prismstudio.egg-info/SOURCES.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-07 03:19:31.000000 prismstudio-1.1.6/prismstudio.egg-info/dependency_links.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)      256 2023-07-07 03:19:31.000000 prismstudio-1.1.6/prismstudio.egg-info/requires.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)       12 2023-07-07 03:19:31.000000 prismstudio-1.1.6/prismstudio.egg-info/top_level.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)       91 2023-06-12 06:52:36.000000 prismstudio-1.1.6/pyproject.toml
+-rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-07 03:19:31.443140 prismstudio-1.1.6/setup.cfg
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1341 2023-07-07 03:02:32.000000 prismstudio-1.1.6/setup.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.443140 prismstudio-1.1.6/tests/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.443140 prismstudio-1.1.6/tests/test_util/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.443140 prismstudio-1.1.6/tests/test_util/test__validate_args/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2200 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_common_functions.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1539 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_fillna.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-07 03:19:31.443140 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     5990 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2004 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2719 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1615 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2304 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1946 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2302 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_07_method.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     6448 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3854 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1717 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1118 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_11_base.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1792 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)      889 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_13_setting.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)      956 2023-06-12 06:52:36.000000 prismstudio-1.1.6/tests/test_util/test__validate_args/test_params/test_param_14_settings.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1770 2023-07-07 02:42:51.000000 prismstudio-1.1.6/tests/test_util/test_version.py
```

### Comparing `prismstudio-1.1.5/setup.py` & `prismstudio-1.1.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
-from setuptools import setup, find_packages
 from glob import glob
+from dotenv import dotenv_values
+from setuptools import setup, find_packages
+
 
 env = os.environ['ENV_STATE']
 name = "prismstudio"
+version = dotenv_values("prism/_common/.env").get("VERSION", "")
 
-datafiles = [("pyarmor_transform", glob("prism/pytransform/*"))]
+datafiles = [("prism/_common", ["prism/_common/.env"])]
 if env == 'dev' or env == 'stg' or env == 'demo':
     name = name + '-' + env
-    datafiles.append(("prism/_common", glob("prism/_common/.env")))
 
 setup(
     name=name,
-    version="1.1.5",
+    version=version,
     description="Python Extension for PrismStudio",
     author="Prism39",
     author_email="jmp@prism39.com",
     url="https://www.prism39.com",
     packages=find_packages(),
-    platforms="nt",
+    license="Prism39 End User License",
     python_requires=">=3.8",
     data_files=datafiles,
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
```

