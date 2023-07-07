# Comparing `tmp/flightanalysis-0.1.8.tar.gz` & `tmp/flightanalysis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightanalysis-0.1.8.tar", last modified: Fri Jun 16 08:50:57 2023, max compression
+gzip compressed data, was "flightanalysis-0.1.9.tar", last modified: Mon Jun 19 18:10:01 2023, max compression
```

## Comparing `flightanalysis-0.1.8.tar` & `flightanalysis-0.1.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.281992 flightanalysis-0.1.8/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/LICENSE
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-06-14 11:48:20.000000 flightanalysis-0.1.8/MANIFEST.in
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-16 08:50:57.281992 flightanalysis-0.1.8/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      370 2023-06-16 08:49:31.000000 flightanalysis-0.1.8/flightanalysis/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/analysis/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      127 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/analysis/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/flightanalysis/analysis/aircraft_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5479 2023-06-15 09:42:28.000000 flightanalysis-0.1.8/flightanalysis/analysis/analysis.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/base/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       83 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/base/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2574 2023-06-14 16:19:59.000000 flightanalysis-0.1.8/flightanalysis/base/collection.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.8/flightanalysis/base/constructs.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/flightanalysis/base/numpy_encoder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5436 2023-06-14 15:42:22.000000 flightanalysis-0.1.8/flightanalysis/base/table.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/controls/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       24 2023-06-15 09:38:45.000000 flightanalysis-0.1.8/flightanalysis/controls/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.8/flightanalysis/controls/controls.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/criteria/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1541 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/criteria/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2434 2023-06-14 16:18:29.000000 flightanalysis-0.1.8/flightanalysis/criteria/combination.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1417 2023-06-14 16:16:38.000000 flightanalysis-0.1.8/flightanalysis/criteria/comparison.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2228 2023-06-14 16:17:13.000000 flightanalysis-0.1.8/flightanalysis/criteria/continuous.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/flightanalysis/criteria/results.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1532 2023-06-14 16:16:58.000000 flightanalysis-0.1.8/flightanalysis/criteria/single.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      293 2023-06-14 12:08:11.000000 flightanalysis-0.1.8/flightanalysis/data/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.8/flightanalysis/data/f25.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    70404 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/data/p23.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.8/flightanalysis/data/p25.json
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/environment/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/flightanalysis/environment/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1226 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/environment/environment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4252 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/environment/wind.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.8/flightanalysis/fc_json.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/flightline/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       40 2023-06-15 09:39:44.000000 flightanalysis-0.1.8/flightanalysis/flightline/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.8/flightanalysis/flightline/flightline.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/model/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      109 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/model/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      828 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/model/coefficients.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/flightanalysis/model/constants.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1113 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/model/flow.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/flightanalysis/model/model.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/schedule/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.8/flightanalysis/schedule/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis/schedule/definition/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      691 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/collectors.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/element_builders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/element_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_builder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_info.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6222 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_parameters.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/operation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.8/flightanalysis/schedule/definition/schedule_definition.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.281992 flightanalysis-0.1.8/flightanalysis/schedule/elements/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7343 2023-06-15 15:25:25.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2307 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/autorotation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3372 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/line.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/loop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2421 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/nose_drop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1958 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/pitch_break.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1557 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/recovery.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.8/flightanalysis/schedule/elements/stall_turn.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4156 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/schedule/manoeuvre.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.8/flightanalysis/schedule/schedule.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.281992 flightanalysis-0.1.8/flightanalysis/state/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       27 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/state/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    22499 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/flightanalysis/state/state.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.277992 flightanalysis-0.1.8/flightanalysis.egg-info/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-16 08:50:57.000000 flightanalysis-0.1.8/flightanalysis.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2528 2023-06-16 08:50:57.000000 flightanalysis-0.1.8/flightanalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-16 08:50:57.000000 flightanalysis-0.1.8/flightanalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-16 08:50:57.000000 flightanalysis-0.1.8/flightanalysis.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-16 08:50:57.000000 flightanalysis-0.1.8/flightanalysis.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      446 2023-06-16 08:50:57.281992 flightanalysis-0.1.8/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.1.8/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:50:57.281992 flightanalysis-0.1.8/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      196 2023-06-16 08:25:50.000000 flightanalysis-0.1.8/tests/test_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/tests/test_controls.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/tests/test_data.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.8/tests/test_fc_json.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.8/tests/test_flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.797786 flightanalysis-0.1.9/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-06-14 11:48:20.000000 flightanalysis-0.1.9/MANIFEST.in
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-19 18:10:01.797786 flightanalysis-0.1.9/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.777785 flightanalysis-0.1.9/flightanalysis/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      370 2023-06-16 08:49:31.000000 flightanalysis-0.1.9/flightanalysis/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.781785 flightanalysis-0.1.9/flightanalysis/analysis/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      127 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/analysis/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/flightanalysis/analysis/aircraft_analysis.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4484 2023-06-19 18:08:35.000000 flightanalysis-0.1.9/flightanalysis/analysis/analysis.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.781785 flightanalysis-0.1.9/flightanalysis/base/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       83 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/base/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2574 2023-06-14 16:19:59.000000 flightanalysis-0.1.9/flightanalysis/base/collection.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.9/flightanalysis/base/constructs.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/flightanalysis/base/numpy_encoder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5436 2023-06-14 15:42:22.000000 flightanalysis-0.1.9/flightanalysis/base/table.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.785786 flightanalysis-0.1.9/flightanalysis/controls/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       24 2023-06-15 09:38:45.000000 flightanalysis-0.1.9/flightanalysis/controls/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.9/flightanalysis/controls/controls.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.785786 flightanalysis-0.1.9/flightanalysis/criteria/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1541 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/criteria/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2434 2023-06-14 16:18:29.000000 flightanalysis-0.1.9/flightanalysis/criteria/combination.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1417 2023-06-14 16:16:38.000000 flightanalysis-0.1.9/flightanalysis/criteria/comparison.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2228 2023-06-14 16:17:13.000000 flightanalysis-0.1.9/flightanalysis/criteria/continuous.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/flightanalysis/criteria/results.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1532 2023-06-14 16:16:58.000000 flightanalysis-0.1.9/flightanalysis/criteria/single.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.789785 flightanalysis-0.1.9/flightanalysis/data/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      293 2023-06-14 12:08:11.000000 flightanalysis-0.1.9/flightanalysis/data/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.9/flightanalysis/data/f25.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    70404 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/data/p23.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.9/flightanalysis/data/p25.json
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.789785 flightanalysis-0.1.9/flightanalysis/environment/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/flightanalysis/environment/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1226 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/environment/environment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4252 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/environment/wind.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.9/flightanalysis/fc_json.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.789785 flightanalysis-0.1.9/flightanalysis/flightline/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       40 2023-06-15 09:39:44.000000 flightanalysis-0.1.9/flightanalysis/flightline/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.9/flightanalysis/flightline/flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.789785 flightanalysis-0.1.9/flightanalysis/model/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      109 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/model/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      828 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/model/coefficients.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/flightanalysis/model/constants.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1113 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/model/flow.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/flightanalysis/model/model.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.793786 flightanalysis-0.1.9/flightanalysis/schedule/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.9/flightanalysis/schedule/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.793786 flightanalysis-0.1.9/flightanalysis/schedule/definition/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      691 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/collectors.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/element_builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/element_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_builder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_info.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6222 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_parameters.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/operation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.9/flightanalysis/schedule/definition/schedule_definition.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.793786 flightanalysis-0.1.9/flightanalysis/schedule/elements/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7343 2023-06-15 15:25:25.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2307 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/autorotation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3372 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/line.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/loop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2421 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/nose_drop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1958 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/pitch_break.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1557 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/recovery.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.9/flightanalysis/schedule/elements/stall_turn.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4156 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/schedule/manoeuvre.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.9/flightanalysis/schedule/schedule.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.793786 flightanalysis-0.1.9/flightanalysis/state/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       27 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/state/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    22499 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/flightanalysis/state/state.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.781785 flightanalysis-0.1.9/flightanalysis.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-19 18:10:01.000000 flightanalysis-0.1.9/flightanalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2528 2023-06-19 18:10:01.000000 flightanalysis-0.1.9/flightanalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-19 18:10:01.000000 flightanalysis-0.1.9/flightanalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-19 18:10:01.000000 flightanalysis-0.1.9/flightanalysis.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-19 18:10:01.000000 flightanalysis-0.1.9/flightanalysis.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      446 2023-06-19 18:10:01.797786 flightanalysis-0.1.9/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.1.9/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-19 18:10:01.797786 flightanalysis-0.1.9/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      196 2023-06-16 08:25:50.000000 flightanalysis-0.1.9/tests/test_analysis.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/tests/test_controls.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/tests/test_data.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.9/tests/test_fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.9/tests/test_flightline.py
```

### Comparing `flightanalysis-0.1.8/LICENSE` & `flightanalysis-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/PKG-INFO` & `flightanalysis-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightanalysis-0.1.8/README.md` & `flightanalysis-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/analysis/aircraft_analysis.py` & `flightanalysis-0.1.9/flightanalysis/analysis/aircraft_analysis.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/analysis/analysis.py` & `flightanalysis-0.1.9/flightanalysis/analysis/analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,23 +16,14 @@
     def __init__(self, mdef: ManDef, aligned: State, intended: Manoeuvre, intended_template: State, corrected: Manoeuvre, corrected_template: State):
         self.mdef = mdef
         self.aligned = aligned
         self.intended = intended
         self.intended_template = intended_template
         self.corrected = corrected
         self.corrected_template = corrected_template
-
-        self.pos_error = self.aligned.pos - self.corrected_template.pos
-        self.roll_error = Quaternion.body_axis_rates(self.aligned.att, self.corrected_template.att).x
-
-        #TODO factor by visibility, replace abs here with something cleverer. Add some logic to the arbitrary fudge factors
-        self.pos_dg = np.cumsum(abs(self.pos_error) * self.aligned.dt / 500)
-        self.roll_dg = np.cumsum(np.abs(self.roll_error) * self.aligned.dt / 40)
-
-        self.score = 10 - self.pos_dg[-1] - self.roll_dg[-1]
     
     def to_dict(self):
         return dict(
             mdef = self.mdef.to_dict(),
             aligned = self.aligned.to_dict(),
             intended = self.intended.to_dict(),
             intended_template = self.intended_template.to_dict(),
@@ -85,74 +76,53 @@
         mdef.mps.update_defaults(intended)       
 
         corr = Manoeuvre(intended.entry_line, mdef._create().elements, mdef.info.short_name)
         corr_tp = corr.create_template(itrans, aligned)
         
         return ManoeuvreAnalysis(mdef, aligned, intended, int_tp, corr, corr_tp)
 
-
-
-
     def plot_3d(self, **kwargs):
         fig = plotsec(self.aligned, color="red", **kwargs)
         return plotsec(self.corrected_template, color="green", fig=fig, **kwargs)
 
-    def plot_dg(self):
-        import plotly.graph_objects as go
-
-        fig = go.Figure()
-
-        fig.add_trace(go.Line(y=self.pos_dg))
-        fig.add_trace(go.Line(y=self.roll_dg , yaxis="y2"))
-        fig.update_layout(
-            yaxis=dict(
-                title="position error"
-            ), 
-            yaxis2=dict(title="roll error",
-                overlaying="y",
-                side="right",)
-        )
-        fig.show()
 
 class ScheduleAnalysis(Collection):
     VType=ManoeuvreAnalysis
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def summary_df(self):
-        return pd.DataFrame(
-            [[an.mdef.info.short_name, an.mdef.info.k, an.score] for an in self], 
-            columns=["name", "k", "score"]
-        )
-
-    def total_score(self):
-        df = self.summary_df()
-        return sum(df.k * df.score)
-
 
 if __name__ == "__main__":
     with open("examples/data/manual_F3A_P23_22_05_31_00000350.json", "r") as f:
         data = load(f)
 
 
     flight = Flight.from_fc_json(data)
     box = Box.from_fcjson_parmameters(data["parameters"])
     state = State.from_flight(flight, box).splitter_labels(data["mans"])
     sdef = get_schedule_definition(data["parameters"]["schedule"][1])
 
-    analyses: List[ManoeuvreAnalysis] = []
+    analyses = ScheduleAnalysis()
 
     for mid in range(17):
-        analyses.append(ManoeuvreAnalysis.build(sdef[mid], state.get_meid(mid+1)))
+        analyses.add(ManoeuvreAnalysis.build(sdef[mid], state.get_meid(mid+1)))
 
-    df = pd.DataFrame([[an.mdef.info.short_name, an.score, an.mdef.info.k] for an in analyses], columns=["name", "score", "k"])
+    scores = []
+
+    for ma in analyses:
+        scores.append(dict(
+            name=ma.mdef.info.name,
+            k=ma.mdef.info.k,
+            pos_dg=np.sum(abs(ma.aligned.pos - ma.corrected_template.pos) * ma.aligned.dt / 500),
+            roll_dg = np.sum(np.abs(Quaternion.body_axis_rates(ma.aligned.att, ma.corrected_template.att).x) * ma.aligned.dt / 40)
+        ))
+
+    scores = pd.DataFrame(scores)
+    scores["score"] = 10 - scores.pos_dg - scores.roll_dg
     if "scores" in data:
-        df["manual_scores"] = data["scores"][1:-1]
+        scores["manual_scores"] = data["scores"][1:-1]
         
-    print(df)
-    print(f"total = {sum(df.score * df.k)}")
-    pass
+    print(scores)
+    print(f"total = {sum(scores.score * scores.k)}")
+
```

### Comparing `flightanalysis-0.1.8/flightanalysis/base/collection.py` & `flightanalysis-0.1.9/flightanalysis/base/collection.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/base/constructs.py` & `flightanalysis-0.1.9/flightanalysis/base/constructs.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/base/table.py` & `flightanalysis-0.1.9/flightanalysis/base/table.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/controls/controls.py` & `flightanalysis-0.1.9/flightanalysis/controls/controls.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/criteria/__init__.py` & `flightanalysis-0.1.9/flightanalysis/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/criteria/combination.py` & `flightanalysis-0.1.9/flightanalysis/criteria/combination.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/criteria/comparison.py` & `flightanalysis-0.1.9/flightanalysis/criteria/comparison.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/criteria/continuous.py` & `flightanalysis-0.1.9/flightanalysis/criteria/continuous.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/criteria/results.py` & `flightanalysis-0.1.9/flightanalysis/criteria/results.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/criteria/single.py` & `flightanalysis-0.1.9/flightanalysis/criteria/single.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/data/f25.json` & `flightanalysis-0.1.9/flightanalysis/data/f25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/data/p23.json` & `flightanalysis-0.1.9/flightanalysis/data/p23.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/data/p25.json` & `flightanalysis-0.1.9/flightanalysis/data/p25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/environment/environment.py` & `flightanalysis-0.1.9/flightanalysis/environment/environment.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/environment/wind.py` & `flightanalysis-0.1.9/flightanalysis/environment/wind.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/flightline/flightline.py` & `flightanalysis-0.1.9/flightanalysis/flightline/flightline.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/model/coefficients.py` & `flightanalysis-0.1.9/flightanalysis/model/coefficients.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/model/flow.py` & `flightanalysis-0.1.9/flightanalysis/model/flow.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/model/model.py` & `flightanalysis-0.1.9/flightanalysis/model/model.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/__init__.py` & `flightanalysis-0.1.9/flightanalysis/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/__init__.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/collectors.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/collectors.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/element_builders.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/element_builders.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/element_definition.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/element_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_builder.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_builder.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_definition.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_info.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_info.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/manoeuvre_parameters.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/manoeuvre_parameters.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/operation.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/operation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/definition/schedule_definition.py` & `flightanalysis-0.1.9/flightanalysis/schedule/definition/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/__init__.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/autorotation.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/autorotation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/line.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/line.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/loop.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/loop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/nose_drop.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/nose_drop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/pitch_break.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/pitch_break.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/recovery.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/recovery.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/elements/stall_turn.py` & `flightanalysis-0.1.9/flightanalysis/schedule/elements/stall_turn.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/manoeuvre.py` & `flightanalysis-0.1.9/flightanalysis/schedule/manoeuvre.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/schedule/schedule.py` & `flightanalysis-0.1.9/flightanalysis/schedule/schedule.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis/state/state.py` & `flightanalysis-0.1.9/flightanalysis/state/state.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/flightanalysis.egg-info/PKG-INFO` & `flightanalysis-0.1.9/flightanalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightanalysis-0.1.8/flightanalysis.egg-info/SOURCES.txt` & `flightanalysis-0.1.9/flightanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/setup.py` & `flightanalysis-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/tests/test_fc_json.py` & `flightanalysis-0.1.9/tests/test_fc_json.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.8/tests/test_flightline.py` & `flightanalysis-0.1.9/tests/test_flightline.py`

 * *Files identical despite different names*

