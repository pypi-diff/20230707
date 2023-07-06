# Comparing `tmp/neon-utils-1.6.0.tar.gz` & `tmp/neon-utils-1.6.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-utils-1.6.0.tar", last modified: Thu Jun 29 17:07:13 2023, max compression
+gzip compressed data, was "neon-utils-1.6.1a1.tar", last modified: Thu Jul  6 22:46:53 2023, max compression
```

## Comparing `neon-utils-1.6.0.tar` & `neon-utils-1.6.1a1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.266245 neon-utils-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 17:07:09.000000 neon-utils-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-29 17:07:13.262245 neon-utils-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 17:07:09.000000 neon-utils-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/authentication_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68558 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/default_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/default_configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/default_configurations/default_user_conf.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/language_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/location_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/messagebus_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/mq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/packaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/process_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.254244 neon-utils-1.6.0/neon_utils/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/res/snd/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/snd/acknowledge.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   428660 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/snd/loaded.wav
--rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/snd/start_listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.254244 neon-utils-1.6.0/neon_utils/res/text/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/res/text/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/stop.voc
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/res/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/ui/neon_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/signal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/neon_utils/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/common_message_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/common_play_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/common_query_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/instructor_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/kiosk_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/mycroft_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/neon_fallback_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/neon_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/skill_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/socket_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/validator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/web_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:07:13.266245 neon-utils-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-29 17:07:09.000000 neon-utils-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/authentication_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/cache_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    63829 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/configuration_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/file_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/language_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/location_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/log_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/message_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/messagebus_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/metric_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/mq_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    55268 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/neon_skill_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/net_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/packaging_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/parse_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/search_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/signal_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/skills/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/skills/test_skill/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/skills/test_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/skills/test_skill/settingsmeta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/socket_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/user_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/valid_skill/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/valid_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/validator_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/web_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.475878 neon-utils-1.6.1a1/neon_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/authentication_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68558 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.475878 neon-utils-1.6.1a1/neon_utils/default_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/default_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/default_configurations/default_user_conf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/language_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/location_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/messagebus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/mq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/packaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/process_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.471878 neon-utils-1.6.1a1/neon_utils/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.475878 neon-utils-1.6.1a1/neon_utils/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/snd/acknowledge.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   428660 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/snd/loaded.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/snd/start_listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.471878 neon-utils-1.6.1a1/neon_utils/res/text/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.475878 neon-utils-1.6.1a1/neon_utils/res/text/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/text/en-us/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/text/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/text/en-us/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/text/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.475878 neon-utils-1.6.1a1/neon_utils/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/res/ui/neon_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/signal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/neon_utils/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/common_message_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/common_play_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/common_query_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/instructor_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/kiosk_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16284 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/mycroft_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/neon_fallback_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/neon_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/skills/skill_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/socket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/validator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/neon_utils/web_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.475878 neon-utils-1.6.1a1/neon_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-06 22:46:53.000000 neon-utils-1.6.1a1/neon_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-06 22:46:53.000000 neon-utils-1.6.1a1/neon_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:46:53.000000 neon-utils-1.6.1a1/neon_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 22:46:53.000000 neon-utils-1.6.1a1/neon_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-06 22:46:53.000000 neon-utils-1.6.1a1/neon_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 22:46:53.000000 neon-utils-1.6.1a1/neon_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/authentication_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/cache_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63829 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/configuration_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/file_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/language_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/location_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/log_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/message_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/messagebus_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/metric_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/mq_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55268 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/neon_skill_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/net_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/packaging_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/parse_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/search_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/signal_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/tests/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/skills/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/tests/skills/test_skill/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/skills/test_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/skills/test_skill/settingsmeta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/socket_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/user_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:46:53.479878 neon-utils-1.6.1a1/tests/valid_skill/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/valid_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/validator_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-06 22:46:49.000000 neon-utils-1.6.1a1/tests/web_util_tests.py
```

### Comparing `neon-utils-1.6.0/LICENSE.md` & `neon-utils-1.6.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/PKG-INFO` & `neon-utils-1.6.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.6.0
+Version: 1.6.1a1
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.6.0/neon_utils/__init__.py` & `neon-utils-1.6.1a1/neon_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/authentication_utils.py` & `neon-utils-1.6.1a1/neon_utils/authentication_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/cache_utils.py` & `neon-utils-1.6.1a1/neon_utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/configuration_utils.py` & `neon-utils-1.6.1a1/neon_utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/decorators.py` & `neon-utils-1.6.1a1/neon_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/default_configurations/__init__.py` & `neon-utils-1.6.1a1/neon_utils/default_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/default_configurations/default_user_conf.yml` & `neon-utils-1.6.1a1/neon_utils/default_configurations/default_user_conf.yml`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/file_utils.py` & `neon-utils-1.6.1a1/neon_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/language_utils.py` & `neon-utils-1.6.1a1/neon_utils/language_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/location_utils.py` & `neon-utils-1.6.1a1/neon_utils/location_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/log_utils.py` & `neon-utils-1.6.1a1/neon_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/logger.py` & `neon-utils-1.6.1a1/neon_utils/logger.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/message_utils.py` & `neon-utils-1.6.1a1/neon_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/messagebus_utils.py` & `neon-utils-1.6.1a1/neon_utils/messagebus_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/metrics_utils.py` & `neon-utils-1.6.1a1/neon_utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/mq_utils.py` & `neon-utils-1.6.1a1/neon_utils/mq_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/net_utils.py` & `neon-utils-1.6.1a1/neon_utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/packaging_utils.py` & `neon-utils-1.6.1a1/neon_utils/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/parse_utils.py` & `neon-utils-1.6.1a1/neon_utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/process_utils.py` & `neon-utils-1.6.1a1/neon_utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/res/snd/acknowledge.mp3` & `neon-utils-1.6.1a1/neon_utils/res/snd/acknowledge.mp3`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/res/snd/loaded.wav` & `neon-utils-1.6.1a1/neon_utils/res/snd/loaded.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/res/snd/start_listening.wav` & `neon-utils-1.6.1a1/neon_utils/res/snd/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/res/ui/neon_logo.png` & `neon-utils-1.6.1a1/neon_utils/res/ui/neon_logo.png`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/search_utils.py` & `neon-utils-1.6.1a1/neon_utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/signal_utils.py` & `neon-utils-1.6.1a1/neon_utils/signal_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/__init__.py` & `neon-utils-1.6.1a1/neon_utils/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/common_message_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/common_message_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/common_play_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/common_play_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/common_query_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/common_query_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/instructor_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/instructor_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/kiosk_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/kiosk_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/mycroft_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/mycroft_skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,24 @@
 from typing import Optional
 from json_database import JsonStorage
 from ovos_bus_client.message import Message
 from ovos_workshop.skills.mycroft_skill import MycroftSkill
 from ovos_utils.skills.settings import get_local_settings
 
 from neon_utils.signal_utils import wait_for_signal_clear, check_for_signal
-from neon_utils.skills.skill_gui import SkillGUI
 from neon_utils.logger import LOG
 from neon_utils.message_utils import get_message_user, dig_for_message, resolve_message
 from neon_utils.configuration_utils import dict_update_keys, \
     parse_skill_default_settings, get_mycroft_compatible_location
 from neon_utils.user_utils import get_user_prefs
 
 
 class PatchedMycroftSkill(MycroftSkill):
     def __init__(self, name=None, bus=None, *args, **kwargs):
         MycroftSkill.__init__(self, name, bus, *args, **kwargs)
-        self.gui = SkillGUI(self)
         # TODO: Should below defaults be global config?
         # allow skills to specify timeout overrides per-skill
         self._speak_timeout = 30
         self._get_response_timeout = 15  # 10 for listener, 5 for STT, then timeout
 
     @property
     def location(self):
@@ -78,20 +76,16 @@
                 self.settings.store()
             else:
                 with open(self._settings_path, "w+") as f:
                     json.dump(self.settings, f, indent=4)
         self._initial_settings = dict(self.settings)
 
     def _init_settings_manager(self):
-        try:
-            from ovos_workshop.settings import SkillSettingsManager
-            self.settings_manager = SkillSettingsManager(self)
-        except ImportError:
-            super()._init_settings_manager()
-
+        from ovos_workshop.settings import SkillSettingsManager
+        self.settings_manager = SkillSettingsManager(self)
 
     def _read_default_settings(self):
         yaml_path = os.path.join(self.root_dir, "settingsmeta.yml")
         json_path = os.path.join(self.root_dir, "settingsmeta.json")
         if os.path.isfile(yaml_path):
             with open(yaml_path) as f:
                 self.settings_meta = yaml.safe_load(f) or dict()
```

### Comparing `neon-utils-1.6.0/neon_utils/skills/neon_fallback_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/neon_fallback_skill.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,15 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.skills.neon_skill import NeonSkill
 from ovos_workshop.skills.ovos import OVOSSkill
 from ovos_utils.intents import IntentLayers
 from ovos_workshop.skills.layers import IntentLayers
-try:
-    from ovos_workshop.skills.fallback import FallbackSkillV1 as FallbackSkill
-except ImportError:
-    from ovos_workshop.skills.fallback import FallbackSkill
+from ovos_workshop.skills.fallback import FallbackSkillV1 as FallbackSkill
 
 
 class NeonFallbackSkill(FallbackSkill, NeonSkill, OVOSSkill):
     """
     Class that extends the NeonSkill and FallbackSkill classes to provide
     NeonSkill functionality to any Fallback skill subclassing this class.
     """
```

### Comparing `neon-utils-1.6.0/neon_utils/skills/neon_skill.py` & `neon-utils-1.6.1a1/neon_utils/skills/neon_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/skills/skill_gui.py` & `neon-utils-1.6.1a1/neon_utils/skills/skill_gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from os.path import join
-from neon_utils.logger import LOG
+from ovos_utils.log import LOG, log_deprecation
 from neon_utils.file_utils import resolve_neon_resource_file
-from mycroft.enclosure.gui import SkillGUI as _SkillGUI
+from ovos_workshop.skills.base import SkillGUI as _SkillGUI
 
 
 class SkillGUI(_SkillGUI):
     def __init__(self, skill):
+        log_deprecation("Implement ovos_utils.gui.GUIInterface directly",
+                        "2.0.0")
         super().__init__(skill)
         self.serving_http = skill.config_core["skills"].get(
             "run_gui_file_server", False)
 
     def _pages2uri(self, page_names):
         # Convert pages to full reference
         page_urls = []
```

### Comparing `neon-utils-1.6.0/neon_utils/socket_utils.py` & `neon-utils-1.6.1a1/neon_utils/socket_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/user_utils.py` & `neon-utils-1.6.1a1/neon_utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils/validator_utils.py` & `neon-utils-1.6.1a1/neon_utils/validator_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils import LOG
 from lingua_franca import parse, set_default_lang
 
-from mycroft.skills.core import MycroftSkill
+from ovos_workshop.skills.mycroft_skill import MycroftSkill
 
 
 def numeric_confirmation_validator(confirmation_num: str, lang: str = "en"):
     """
     Returns a validator method that returns true if the confirmation_num is in the passed string.
      The confirmation_num must be the only number in the utterance (something 123 != 1 something 123).
     :param confirmation_num: number to locate in utterance
```

### Comparing `neon-utils-1.6.0/neon_utils/web_utils.py` & `neon-utils-1.6.1a1/neon_utils/web_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils.egg-info/PKG-INFO` & `neon-utils-1.6.1a1/neon_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.6.0
+Version: 1.6.1a1
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.6.0/neon_utils.egg-info/SOURCES.txt` & `neon-utils-1.6.1a1/neon_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/neon_utils.egg-info/requires.txt` & `neon-utils-1.6.1a1/neon_utils.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ovos-bus-client~=0.0.3
 combo-lock~=0.2
 pendulum~=2.1
 timezonefinder~=5.2
 nltk~=3.5
 pyyaml<7.0,>=5.4
 ovos-lingua-franca~=0.4
-ovos_utils~=0.0.34
+ovos_utils>=0.0.35a6,~=0.0.34
 geopy~=2.1
 ovos-config~=0.0.9
-ovos-workshop~=0.0.11
+ovos-workshop>=0.0.12a34,~=0.0.11
 
 [audio]
 soundfile~=0.10
 librosa<0.10,~=0.8
 pydub~=0.25
 
 [configuration]
```

### Comparing `neon-utils-1.6.0/setup.py` & `neon-utils-1.6.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/__init__.py` & `neon-utils-1.6.1a1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/authentication_util_tests.py` & `neon-utils-1.6.1a1/tests/authentication_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/cache_util_tests.py` & `neon-utils-1.6.1a1/tests/cache_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/configuration_util_tests.py` & `neon-utils-1.6.1a1/tests/configuration_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/file_util_tests.py` & `neon-utils-1.6.1a1/tests/file_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/language_util_tests.py` & `neon-utils-1.6.1a1/tests/language_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/location_util_tests.py` & `neon-utils-1.6.1a1/tests/location_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/log_util_tests.py` & `neon-utils-1.6.1a1/tests/log_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/message_util_tests.py` & `neon-utils-1.6.1a1/tests/message_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/messagebus_util_tests.py` & `neon-utils-1.6.1a1/tests/messagebus_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/metric_util_tests.py` & `neon-utils-1.6.1a1/tests/metric_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/mq_util_tests.py` & `neon-utils-1.6.1a1/tests/mq_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/neon_skill_tests.py` & `neon-utils-1.6.1a1/tests/neon_skill_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/net_util_tests.py` & `neon-utils-1.6.1a1/tests/net_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/packaging_util_tests.py` & `neon-utils-1.6.1a1/tests/packaging_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/parse_util_tests.py` & `neon-utils-1.6.1a1/tests/parse_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/search_util_tests.py` & `neon-utils-1.6.1a1/tests/search_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/signal_util_tests.py` & `neon-utils-1.6.1a1/tests/signal_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/skills/__init__.py` & `neon-utils-1.6.1a1/tests/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/skills/test_skill/__init__.py` & `neon-utils-1.6.1a1/tests/skills/test_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/socket_utils_tests.py` & `neon-utils-1.6.1a1/tests/socket_utils_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/user_util_tests.py` & `neon-utils-1.6.1a1/tests/user_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/valid_skill/__init__.py` & `neon-utils-1.6.1a1/tests/valid_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/validator_util_tests.py` & `neon-utils-1.6.1a1/tests/validator_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.6.0/tests/web_util_tests.py` & `neon-utils-1.6.1a1/tests/web_util_tests.py`

 * *Files identical despite different names*

