# Comparing `tmp/challengeutils-4.2.0.tar.gz` & `tmp/challengeutils-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challengeutils-4.2.0.tar", last modified: Fri Mar 17 13:07:05 2023, max compression
+gzip compressed data, was "challengeutils-4.2.1.tar", last modified: Fri Jul  7 01:10:55 2023, max compression
```

## Comparing `challengeutils-4.2.0.tar` & `challengeutils-4.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:07:05.850770 challengeutils-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-03-17 13:06:55.000000 challengeutils-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-03-17 13:07:05.850770 challengeutils-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-17 13:06:55.000000 challengeutils-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:07:05.846770 challengeutils-4.2.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-03-17 13:06:55.000000 challengeutils-4.2.0/bin/runqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:07:05.846770 challengeutils-4.2.0/challengeutils/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30138 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    26682 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/cheat_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/createchallenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    14464 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/discussion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/dockertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/evaluation_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/mirrorwiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/submission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:07:05.846770 challengeutils-4.2.0/challengeutils/synapseservices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/synapseservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/synapseservices/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/synapseservices/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/synapseservices/discussion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-03-17 13:06:55.000000 challengeutils-4.2.0/challengeutils/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:07:05.846770 challengeutils-4.2.0/challengeutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-03-17 13:07:05.000000 challengeutils-4.2.0/challengeutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-17 13:07:05.000000 challengeutils-4.2.0/challengeutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:07:05.000000 challengeutils-4.2.0/challengeutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-17 13:07:05.000000 challengeutils-4.2.0/challengeutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:07:05.000000 challengeutils-4.2.0/challengeutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-17 13:07:05.000000 challengeutils-4.2.0/challengeutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 13:07:05.000000 challengeutils-4.2.0/challengeutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 13:06:55.000000 challengeutils-4.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:07:05.846770 challengeutils-4.2.0/scoring_harness/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:06:55.000000 challengeutils-4.2.0/scoring_harness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-03-17 13:06:55.000000 challengeutils-4.2.0/scoring_harness/base_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-17 13:06:55.000000 challengeutils-4.2.0/scoring_harness/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-17 13:06:55.000000 challengeutils-4.2.0/scoring_harness/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-03-17 13:06:55.000000 challengeutils-4.2.0/scoring_harness/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-17 13:06:55.000000 challengeutils-4.2.0/scoring_harness/queue_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-17 13:06:55.000000 challengeutils-4.2.0/scoring_harness/queue_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-17 13:07:05.850770 challengeutils-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-17 13:06:55.000000 challengeutils-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:07:05.850770 challengeutils-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/evaluation_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_cheatdetection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_createchallenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_discussion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_dockertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_evaluation_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_mirrorwiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-03-17 13:06:55.000000 challengeutils-4.2.0/tests/test_wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:55.861020 challengeutils-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-07 01:10:44.000000 challengeutils-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-07 01:10:55.861020 challengeutils-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-07 01:10:44.000000 challengeutils-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:55.853020 challengeutils-4.2.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-07 01:10:44.000000 challengeutils-4.2.1/bin/runqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:55.857020 challengeutils-4.2.1/challengeutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30138 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26682 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/cheat_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/createchallenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14464 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/discussion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/dockertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/evaluation_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/mirrorwiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/submission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:55.857020 challengeutils-4.2.1/challengeutils/synapseservices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/synapseservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/synapseservices/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/synapseservices/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/synapseservices/discussion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-07-07 01:10:44.000000 challengeutils-4.2.1/challengeutils/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:55.857020 challengeutils-4.2.1/challengeutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-07 01:10:55.000000 challengeutils-4.2.1/challengeutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-07 01:10:55.000000 challengeutils-4.2.1/challengeutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:10:55.000000 challengeutils-4.2.1/challengeutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 01:10:55.000000 challengeutils-4.2.1/challengeutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:10:55.000000 challengeutils-4.2.1/challengeutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 01:10:55.000000 challengeutils-4.2.1/challengeutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 01:10:55.000000 challengeutils-4.2.1/challengeutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 01:10:44.000000 challengeutils-4.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:55.857020 challengeutils-4.2.1/scoring_harness/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:44.000000 challengeutils-4.2.1/scoring_harness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-07 01:10:44.000000 challengeutils-4.2.1/scoring_harness/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 01:10:44.000000 challengeutils-4.2.1/scoring_harness/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-07 01:10:44.000000 challengeutils-4.2.1/scoring_harness/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-07 01:10:44.000000 challengeutils-4.2.1/scoring_harness/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-07 01:10:44.000000 challengeutils-4.2.1/scoring_harness/queue_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-07 01:10:44.000000 challengeutils-4.2.1/scoring_harness/queue_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-07 01:10:55.861020 challengeutils-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-07 01:10:44.000000 challengeutils-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:55.861020 challengeutils-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/evaluation_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_cheatdetection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_createchallenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_discussion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_dockertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_evaluation_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_mirrorwiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-07 01:10:44.000000 challengeutils-4.2.1/tests/test_wiki.py
```

### Comparing `challengeutils-4.2.0/LICENSE` & `challengeutils-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/PKG-INFO` & `challengeutils-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: challengeutils
-Version: 4.2.0
+Version: 4.2.1
 Summary: Challenge utility functions
 Home-page: https://github.com/Sage-Bionetworks/challengeutils
 Author: Thomas Yu
 Author-email: thomas.yu@sagebionetworks.org
 License: Apache
 Project-URL: Bug Tracker, https://github.com/Sage-Bionetworks/challengeutils/issues
 Project-URL: Source Code, https://github.com/Sage-Bionetworks/challengeutil
```

### Comparing `challengeutils-4.2.0/README.md` & `challengeutils-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/bin/runqueue.py` & `challengeutils-4.2.1/bin/runqueue.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/__main__.py` & `challengeutils-4.2.1/challengeutils/__main__.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/annotations.py` & `challengeutils-4.2.1/challengeutils/annotations.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/challenge.py` & `challengeutils-4.2.1/challengeutils/challenge.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/cheat_detection.py` & `challengeutils-4.2.1/challengeutils/cheat_detection.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/createchallenge.py` & `challengeutils-4.2.1/challengeutils/createchallenge.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/discussion.py` & `challengeutils-4.2.1/challengeutils/discussion.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/dockertools.py` & `challengeutils-4.2.1/challengeutils/dockertools.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/evaluation_queue.py` & `challengeutils-4.2.1/challengeutils/evaluation_queue.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/mirrorwiki.py` & `challengeutils-4.2.1/challengeutils/mirrorwiki.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/permissions.py` & `challengeutils-4.2.1/challengeutils/permissions.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/submission.py` & `challengeutils-4.2.1/challengeutils/submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,26 +99,22 @@
 
     Returns:
         submission_errors (str) - error messages ("" if none found)
         submission_status (str) - "VALIDATED"/"INVALID"
     """
     writeup = syn.getSubmission(submission)
     errors = []
-
     type_error = _validate_ent_type(writeup)
     if type_error:
         errors.append(type_error)
-
     contents_error = _validate_project_id(writeup, challenge)
     if contents_error:
         errors.append(contents_error)
-
     permissions_error = _check_project_permissions(syn, writeup, public, admin)
     errors.extend(permissions_error)
-
     status = "INVALID" if errors else "VALIDATED"
     return {"submission_errors": "\n".join(errors), "submission_status": status}
 
 
 def archive_project(syn, submission, admin):
     """
     Make a copy (archive) of the Project submission.
@@ -138,89 +134,79 @@
     archived = synapseutils.copy(syn, writeup.entityId, archive.id)
     return {"archived": archived.get(writeup.entityId)}
 
 
 # TODO: move to utils module
 def _validate_ent_type(submission):
     """Check entity type of submission."""
-
     try:
         if not isinstance(submission.entity, entity.Project):
             ent_type = re.search(r"entity\.(.*?)'", str(type(submission.entity))).group(
                 1
             )
             return f"Submission should be a Synapse project, not a {ent_type}."
     except AttributeError:
         return "Unknown entity type; please submit a Synapse project."
     else:
         return ""
 
 
 def _validate_project_id(proj, challenge):
     """Check that submission is not the Challenge site."""
-
     return (
         "Submission should not be the Challenge site."
         if proj.entityId == challenge
         else ""
     )
 
 
 def _validate_public_permissions(syn, proj):
     """Ensure project is shared with the public."""
-
     error = "Your project is not publicly available."
-
     try:
         # Remove error message if the project is accessible by the public.
-        syn_users_perms = syn.getPermissions(proj.entityId, AUTHENTICATED_USERS)
         public_perms = syn.getPermissions(proj.entityId)
-        if (
-            "READ" in syn_users_perms and "DOWNLOAD" in syn_users_perms
-        ) and "READ" in public_perms:
+        if "READ" in public_perms:
             error = ""
-
     except SynapseHTTPError as e:
         # Raise exception message if error is not a permissions error.
         if e.response.status_code != 403:
             raise e
-
     return error
 
 
 def _validate_admin_permissions(syn, proj, admin):
     """Ensure project is shared with the given admin."""
-
     error = (
         "Project is private; please update its sharing settings."
         f" Writeup should be shared with {admin}."
     )
     try:
-        # Remove error message if admin has read and download permissions.
+        # Remove error message if admin has read and download permissions
+        # OR if the project is publicly availably.
         admin_perms = syn.getPermissions(proj.entityId, admin)
-        if "READ" in admin_perms and "DOWNLOAD" in admin_perms:
+        public_perms = syn.getPermissions(proj.entityId)
+        if "READ" in public_perms or (
+            "READ" in admin_perms and "DOWNLOAD" in admin_perms
+        ):
             error = ""
-
     except SynapseHTTPError as e:
         # Raise exception message if error is not a permissions error.
         if e.response.status_code != 403:
             raise e
-
     return error
 
 
 def _check_project_permissions(syn, submission, public, admin):
     """Check the submission sharing settings."""
-
     errors = []
     if public:
         public_error = _validate_public_permissions(syn, submission)
         if public_error:
             errors.append(public_error)
-
     if not public and admin is not None:
         admin_error = _validate_admin_permissions(syn, submission, admin)
         if admin_error:
             errors.append(admin_error)
     return errors
```

### Comparing `challengeutils-4.2.0/challengeutils/synapseservices/base_service.py` & `challengeutils-4.2.1/challengeutils/synapseservices/base_service.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/synapseservices/challenge.py` & `challengeutils-4.2.1/challengeutils/synapseservices/challenge.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/synapseservices/discussion.py` & `challengeutils-4.2.1/challengeutils/synapseservices/discussion.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/teams.py` & `challengeutils-4.2.1/challengeutils/teams.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/utils.py` & `challengeutils-4.2.1/challengeutils/utils.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils/wiki.py` & `challengeutils-4.2.1/challengeutils/wiki.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/challengeutils.egg-info/PKG-INFO` & `challengeutils-4.2.1/challengeutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: challengeutils
-Version: 4.2.0
+Version: 4.2.1
 Summary: Challenge utility functions
 Home-page: https://github.com/Sage-Bionetworks/challengeutils
 Author: Thomas Yu
 Author-email: thomas.yu@sagebionetworks.org
 License: Apache
 Project-URL: Bug Tracker, https://github.com/Sage-Bionetworks/challengeutils/issues
 Project-URL: Source Code, https://github.com/Sage-Bionetworks/challengeutil
```

### Comparing `challengeutils-4.2.0/challengeutils.egg-info/SOURCES.txt` & `challengeutils-4.2.1/challengeutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/scoring_harness/base_processor.py` & `challengeutils-4.2.1/scoring_harness/base_processor.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/scoring_harness/lock.py` & `challengeutils-4.2.1/scoring_harness/lock.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/scoring_harness/messages.py` & `challengeutils-4.2.1/scoring_harness/messages.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/scoring_harness/queue_scorer.py` & `challengeutils-4.2.1/scoring_harness/queue_scorer.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/scoring_harness/queue_validator.py` & `challengeutils-4.2.1/scoring_harness/queue_validator.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/setup.cfg` & `challengeutils-4.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/evaluation_queue.py` & `challengeutils-4.2.1/tests/evaluation_queue.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_annotations.py` & `challengeutils-4.2.1/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_challenge.py` & `challengeutils-4.2.1/tests/test_challenge.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_cheatdetection.py` & `challengeutils-4.2.1/tests/test_cheatdetection.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_createchallenge.py` & `challengeutils-4.2.1/tests/test_createchallenge.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_discussion.py` & `challengeutils-4.2.1/tests/test_discussion.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_dockertools.py` & `challengeutils-4.2.1/tests/test_dockertools.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_evaluation_queue.py` & `challengeutils-4.2.1/tests/test_evaluation_queue.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_mirrorwiki.py` & `challengeutils-4.2.1/tests/test_mirrorwiki.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_permissions.py` & `challengeutils-4.2.1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_processor.py` & `challengeutils-4.2.1/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_scorer.py` & `challengeutils-4.2.1/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_submission.py` & `challengeutils-4.2.1/tests/test_submission.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """Tests sharing settings for an admin.
 
     One call to check for permissions expected.
     """
     admin = "me"
     with patch.object(SYN, "getPermissions") as patch_perms:
         errors = submission._validate_admin_permissions(SYN, PROJ, admin=admin)
-        patch_perms.assert_called_once()
+        assert patch_perms.call_count == 2
 
         message = (
             "Project is private; please update its sharing settings."
             f" Writeup should be shared with {admin}."
         )
         assert errors == message
 
@@ -82,15 +82,15 @@
     """Tests sharing settings to the public.
 
     Two calls to check for permissions expected (one for all Synapse
     users, another for the public).
     """
     with patch.object(SYN, "getPermissions") as patch_perms:
         errors = submission._validate_public_permissions(SYN, PROJ)
-        assert patch_perms.call_count == 2
+        patch_perms.assert_called_once()
         assert errors == "Your project is not publicly available."
 
 
 @pytest.mark.parametrize(
     "public, admin, output",
     [
         (True, None, "Your project is not publicly available."),
```

### Comparing `challengeutils-4.2.0/tests/test_teams.py` & `challengeutils-4.2.1/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_utils.py` & `challengeutils-4.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_validator.py` & `challengeutils-4.2.1/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `challengeutils-4.2.0/tests/test_wiki.py` & `challengeutils-4.2.1/tests/test_wiki.py`

 * *Files identical despite different names*

