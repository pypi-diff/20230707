# Comparing `tmp/embykeeper-2.2.7.tar.gz` & `tmp/embykeeper-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.2.7.tar", last modified: Thu Jun 29 12:10:41 2023, max compression
+gzip compressed data, was "embykeeper-2.2.9.tar", last modified: Fri Jul  7 10:39:51 2023, max compression
```

## Comparing `embykeeper-2.2.7.tar` & `embykeeper-2.2.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 12:10:31.000000 embykeeper-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 12:10:31.000000 embykeeper-2.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23854 2023-06-29 12:10:41.581615 embykeeper-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22905 2023-06-29 12:10:31.000000 embykeeper-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23854 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-29 12:10:31.000000 embykeeper-2.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:10:41.581615 embykeeper-2.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-29 12:10:31.000000 embykeeper-2.2.7/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.889610 embykeeper-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 10:39:41.000000 embykeeper-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 10:39:41.000000 embykeeper-2.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-07 10:39:51.889610 embykeeper-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-07-07 10:39:41.000000 embykeeper-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.881610 embykeeper-2.2.9/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.881610 embykeeper-2.2.9/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.889610 embykeeper-2.2.9/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-07 10:39:41.000000 embykeeper-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:39:51.889610 embykeeper-2.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.889610 embykeeper-2.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-07 10:39:41.000000 embykeeper-2.2.9/tests/test_cli.py
```

### Comparing `embykeeper-2.2.7/LICENSE` & `embykeeper-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/PKG-INFO` & `embykeeper-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.7
+Version: 2.2.9
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -83,22 +83,14 @@
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
 ### 在线部署
 
-#### Railway
-
-Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
-
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
-
-请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
-
 #### Render.com
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.7 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.9 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -87,22 +87,15 @@
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
-å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
-æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
-(https://railway.app/button.svg)](https://railway.app/new/template/
-WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
-06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
-5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
-é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+å¨çº¿é¨ç½² #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
 å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
```

### Comparing `embykeeper-2.2.7/README.md` & `embykeeper-2.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,14 @@
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
 ### 在线部署
 
-#### Railway
-
-Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
-
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
-
-请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
-
 #### Render.com
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
```

#### html2text {}

```diff
@@ -75,22 +75,15 @@
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
-å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
-æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
-(https://railway.app/button.svg)](https://railway.app/new/template/
-WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
-06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
-5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
-é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+å¨çº¿é¨ç½² #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
 å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
```

### Comparing `embykeeper-2.2.7/embykeeper/cli.py` & `embykeeper-2.2.9/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/data.py` & `embykeeper-2.2.9/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/embywatcher/emby.py` & `embykeeper-2.2.9/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/embywatcher/main.py` & `embykeeper-2.2.9/embykeeper/embywatcher/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 def is_ok(co):
     if isinstance(co, tuple):
         co, *_ = co
     if 200 <= co < 300:
         return True
 
 
-async def get_latest(emby: Emby, n=10):
-    items = await emby.get_items(["Movie", "Episode"], limit=n, sort="DateCreated", ascending=False)
-    i: Union[Movie, Episode]
-    for i in items:
-        yield i
+async def get_latest(emby: Emby):
+    while True:
+        items = await emby.get_items(["Movie", "Episode"], limit=10, sort="DateCreated", ascending=False)
+        i: Union[Movie, Episode]
+        for i in items:
+            yield i
 
 
 async def set_played(obj: EmbyObject):
     c: Connector = obj.connector
     return is_ok(await c.post(f"/Users/{{UserId}}/PlayedItems/{obj.id}"))
 
 
@@ -65,15 +66,18 @@
     except asyncio.CancelledError:
         pass
 
 
 async def play(obj: EmbyObject, time=10, progress=1000):
     c: Connector = obj.connector
     # 检查
-    if obj.object_dict.get("RunTimeTicks") < max(progress, time) * 10000000:
+    totalticks = obj.object_dict.get("RunTimeTicks")
+    if not totalticks:
+        raise PlayError("无法获取视频长度")
+    if totalticks < max(progress, time) * 10000000:
         raise PlayError("视频长度低于观看进度所需")
     # 获取播放源
     resp = await c.postJson(f"/Items/{obj.id}/PlaybackInfo", isPlayBack=True, AutoOpenLiveStream=True)
     if not resp["MediaSources"]:
         raise PlayError("无视频源")
     else:
         play_session_id = resp["PlaySessionId"]
```

### Comparing `embykeeper-2.2.7/embykeeper/log.py` & `embykeeper-2.2.9/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/settings.py` & `embykeeper-2.2.9/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/base.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.2.9/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/link.py` & `embykeeper-2.2.9/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/log.py` & `embykeeper-2.2.9/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/main.py` & `embykeeper-2.2.9/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/messager/base.py` & `embykeeper-2.2.9/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/messager/common.py` & `embykeeper-2.2.9/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.2.9/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/telechecker/tele.py` & `embykeeper-2.2.9/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper/utils.py` & `embykeeper-2.2.9/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.2.9/embykeeper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.7
+Version: 2.2.9
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -83,22 +83,14 @@
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
 ### 在线部署
 
-#### Railway
-
-Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
-
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
-
-请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
-
 #### Render.com
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.7 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.9 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -87,22 +87,15 @@
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
-å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
-æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
-(https://railway.app/button.svg)](https://railway.app/new/template/
-WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
-06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
-5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
-é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+å¨çº¿é¨ç½² #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
 å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
```

### Comparing `embykeeper-2.2.7/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.2.9/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/app.py` & `embykeeper-2.2.9/embykeeperweb/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -207,15 +207,20 @@
             app.config["fd"] = None
             app.config["pid"] = None
             app.config["hist"] = ""
             logger.debug(f"Embykeeper stopped.")
 
 
 @cli.command(context_settings={"ignore_unknown_options": True, "allow_extra_args": True})
-def run(ctx: typer.Context, port: int = 1818, host: str = "0.0.0.0", debug: bool = False):
+def run(
+    ctx: typer.Context,
+    port: int = typer.Option(1818, envvar="PORT", show_envvar=False),
+    host: str = "0.0.0.0",
+    debug: bool = False,
+):
     app.config["args"] = ctx.args
     logger.info(f"Embykeeper webserver started at {host}:{port}.")
     socketio.run(app, port=port, host=host, debug=debug)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/404.html` & `embykeeper-2.2.9/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.2.9/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.2.9/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.2.9/embykeeperweb/templates/assets/js/console.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.2.9/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/console.html` & `embykeeper-2.2.9/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/embykeeperweb/templates/login.html` & `embykeeper-2.2.9/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.7/pyproject.toml` & `embykeeper-2.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.2.7"
+version = "2.2.9"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
```

### Comparing `embykeeper-2.2.7/tests/test_cli.py` & `embykeeper-2.2.9/tests/test_cli.py`

 * *Files identical despite different names*

