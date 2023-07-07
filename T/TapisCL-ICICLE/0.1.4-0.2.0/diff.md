# Comparing `tmp/TapisCL-ICICLE-0.1.4.tar.gz` & `tmp/TapisCL-ICICLE-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.1.4.tar", last modified: Fri Jun 23 18:50:46 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.2.0.tar", last modified: Fri Jul  7 17:08:30 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.1.4.tar` & `TapisCL-ICICLE-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.176371 TapisCL-ICICLE-0.1.4/
--rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    44548 2023-06-23 18:50:46.176371 TapisCL-ICICLE-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/README.md
--rw-rw-rw-   0        0        0     1178 2023-06-23 18:49:57.000000 TapisCL-ICICLE-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 18:50:46.176371 TapisCL-ICICLE-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:45.907452 TapisCL-ICICLE-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:45.994994 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      417 2023-06-23 17:45:33.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.013548 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     8996 2023-06-23 18:46:38.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.083949 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.094318 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     5788 2023-06-23 17:07:16.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.108935 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/systemCommands.py
--rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.128298 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0     7982 2023-06-23 17:46:27.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/serviceCheck.py
--rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.141727 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.160917 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.174222 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44548 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1677 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.933509 TapisCL-ICICLE-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    44922 2023-07-07 17:08:30.932509 TapisCL-ICICLE-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3015 2023-06-27 20:45:47.000000 TapisCL-ICICLE-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1178 2023-07-07 17:07:13.000000 TapisCL-ICICLE-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:08:30.933509 TapisCL-ICICLE-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.103918 TapisCL-ICICLE-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.156532 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-06-28 16:15:55.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.208282 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0    10068 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0    10189 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.442478 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0    10762 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.503334 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     7175 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    17471 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0    10393 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2190 2023-06-30 23:43:06.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     1616 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-07-03 18:52:39.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    11359 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     6205 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/jobCommands.py
+-rw-rw-rw-   0        0        0     9081 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.565368 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-06-30 18:18:14.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     4010 2023-07-07 16:41:01.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    20776 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/systemCommands.py
+-rw-rw-rw-   0        0        0     8018 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.629637 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    11007 2023-07-07 17:05:35.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0    10202 2023-07-07 16:36:44.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0     2044 2023-07-07 17:02:35.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/server/userFileManager.py
+-rw-rw-rw-   0        0        0      290 2023-07-03 18:17:51.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.732514 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4439 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.906643 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     1961 2023-07-06 18:19:25.000000 TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:08:30.929986 TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44922 2023-07-07 17:08:30.000000 TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2023-07-07 17:08:30.000000 TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:08:30.000000 TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-07 17:08:30.000000 TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-07-07 17:08:30.000000 TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-07 17:08:30.000000 TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-27 23:09:19.000000 TapisCL-ICICLE-0.2.0/src/__init__.py
```

### Comparing `TapisCL-ICICLE-0.1.4/LICENSE` & `TapisCL-ICICLE-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.4/PKG-INFO` & `TapisCL-ICICLE-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.4
+Version: 0.2.0
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -704,26 +704,23 @@
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 #### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
-2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
-3. enter your username and password when prompted
+2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be icicle.tapis.io
+3. the application will then prompt you to choose your authentication method, password, federated, or device code. Which ones are avaiable depends on the tenant in question. If you choose either the 2nd or 3rd option, you will be asked to create a session password to authenticate secure operations.
 4. if all went well the console should open. You can run `help` to see command options
-5. to exit the application, run `exit`
+5. to exit the application, run `exit`. To shut it down, run `shutdown`. The server automatically shuts down after 25 minutes of inactivity
 
 #### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
-`python -m TapisCLICICLE pods -c help`
+`python -m TapisCLICICLE help -v`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
-**Scripting**
-
-Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
-
 ### Known Issues
 Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
+The application has known compatibility issues with the WSL vpn due to its reliance on sockets. If you intend to use the application with WSL turn off your VPN. If the application doesnt work and you have a VPN on, turn it off just to make sure.
```

### Comparing `TapisCL-ICICLE-0.1.4/README.md` & `TapisCL-ICICLE-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -14,26 +14,23 @@
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 #### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
-2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
-3. enter your username and password when prompted
+2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be icicle.tapis.io
+3. the application will then prompt you to choose your authentication method, password, federated, or device code. Which ones are avaiable depends on the tenant in question. If you choose either the 2nd or 3rd option, you will be asked to create a session password to authenticate secure operations.
 4. if all went well the console should open. You can run `help` to see command options
-5. to exit the application, run `exit`
+5. to exit the application, run `exit`. To shut it down, run `shutdown`. The server automatically shuts down after 25 minutes of inactivity
 
 #### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
-`python -m TapisCLICICLE pods -c help`
+`python -m TapisCLICICLE help -v`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
-**Scripting**
-
-Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
-
 ### Known Issues
 Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
+The application has known compatibility issues with the WSL vpn due to its reliance on sockets. If you intend to use the application with WSL turn off your VPN. If the application doesnt work and you have a VPN on, turn it off just to make sure.
```

### Comparing `TapisCL-ICICLE-0.1.4/pyproject.toml` & `TapisCL-ICICLE-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.1.4"
+version = "0.2.0"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/client/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,38 @@
 import socket
 import argparse
 import sys
 import os
 import time
 import traceback
 import subprocess
+import pprint
 
 import pyfiglet
 from blessed import Terminal
 
 if __name__ != "__main__":
     from . import handlers
     from ..socketopts import socketOpts, schemas
     from ..commands import decorators
-    from ..utilities import killableThread
+    from ..utilities import killableThread, exceptions
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(f"{__file__}")))
 server_path = os.path.join(__location__, r'../serverRun.py')
+
+ENTRANCE_MESSAGE = \
+"""
+Welcome to TapisCLICICLE
+The server takes a bit of time to start. Please Wait.
+If you have VPN enabled and startup fails, disable your VPN
+If issues persist, try restarting your computer.
+If you find any issues, please create a new issue here: https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/issues
+"""
     
 
 class ClientSideConnection(socketOpts.ClientSocketOpts, handlers.Handlers):
     def __init__(self, connection, debug=False):
         super().__init__("client", debug=debug)
         self.connection = connection
     
@@ -36,49 +46,59 @@
     """
     Receive user input, either direct from bash environment or from the custom interface, then parse these commands and send them to the server to be executed. 
     """
     def __init__(self, IP: str, PORT: int):
         super().__init__()
 
         self.term = Terminal()
+        print(f"{self.term.color_rgb(0, 0, 255)}{ENTRANCE_MESSAGE}{self.term.normal}")
         self.ip, self.port = IP, PORT
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM) 
 
         # set up argparse
         self.parser = None
 
         setup_message = schemas.ResponseData(request_content={'setup_success':True})
         try:
             self.username, self.url = self.connect()
             self.connection.send(setup_message)
+        except ConnectionAbortedError:
+            print("Server timed out during authentication. Try again")
+            sys.exit(0)
         except (KeyboardInterrupt, Exception) as e:
             error_str = traceback.format_exc()
             if self.debug:
                 print(error_str)
             print(e)
             setup_message.error = str(e)
             setup_message.request_content['setup_success'] = False
             self.connection.send(setup_message)
-            os._exit(0)
+            sys.exit(0)
 
         self.pwd = ""
         self.current_system = ""
 
     def parser_error(self, args):
         print(f"Ignoring unrecognized arguments: {args}")
     
     def configure_parser(self, arguments):
         parser = argparse.ArgumentParser(description="Command Line Argument Parser", exit_on_error=False, usage=argparse.SUPPRESS, add_help=False, conflict_handler='resolve')
         parser.add_argument('command_selection')
-        parser.add_argument('positionals', nargs='*', default='default1')
+        parser.add_argument('positionals', nargs='*')
         parser.error = self.parser_error
-
+        
         for arg_name, arg in arguments.items():
+            if arg['action'] == 'store_true':
+                default = False
+            elif arg['action'] == 'store_false':
+                default = True
+            else:
+                default = None
             parser.add_argument(f"-{arg['truncated_arg']}", arg['full_arg'],
-                                action=arg['action'])
+                                action=arg['action'], default=default)
         return parser
 
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
         """
         if 'win' in sys.platform:
@@ -92,38 +112,38 @@
         start the local server through the client
         """
         startup_flag = False
         timeout_time = time.time() + 30 # server setup timeout. If expires, there is a problem!
         while True:
             if time.time() > timeout_time: # connection timeout condition
                 sys.stdout.write("\r[-] Connection timeout")
-                os._exit(0)
+                sys.exit(0)
             try:
                 self.connection.connect((self.ip, self.port)) 
                 self.connection = ClientSideConnection(self.connection, debug=self.debug)
                 if startup_flag:
                     startup.kill()
                 break
             except Exception as e:
                 if not startup_flag:
-                    startup = killableThread.KillableThread(target=self.initialize_server) # run the server setup on a separate thread
+                    startup = killableThread.KillableThread(target=self.initialize_server, daemon=True) # run the server setup on a separate thread
                     startup.start() 
                     startup_flag = True # set the flag to true so the thread runs only once
                     continue
 
     def auth(self):
         while True:
             server_auth_request: schemas.AuthRequest = self.connection.receive()
             if not server_auth_request.message and not server_auth_request.request_content:
                 self.print_response(server_auth_request.error)
                 sys.exit(0)
             elif server_auth_request.auth_request_type == "success":
                 self.print_response(server_auth_request.message)
                 return server_auth_request.message['username'], server_auth_request.message['url']
-            form_response, repeat = self.universal_message_handler(server_auth_request, self.term)
+            form_response = self.universal_message_handler(server_auth_request, self.term)
             if not form_response:
                 break
             client_response_request = schemas.AuthRequest(auth_request_type=server_auth_request.auth_request_type, request_content=form_response)
             self.connection.send(client_response_request)
         
     def connect(self):
         """
@@ -148,58 +168,65 @@
         self.connection.send(command_request)
         while True:
             command_response = self.connection.receive()
             if isinstance(command_response, schemas.ResponseData):
                 self.url, self.username = command_response.url, command_response.active_username
                 self.pwd, self.current_system = command_response.pwd, command_response.system
                 if command_response.exit_status:
-                    print("Exit initiated")
-                    os._exit(0)
-            handled_response, repeat = self.universal_message_handler(command_response, self.term)
+                    raise exceptions.Shutdown()
+            handled_response = self.universal_message_handler(command_response, self.term)
             if not handled_response:
                 break
             handled_response = schemas.FormResponse(request_content=handled_response)
             self.connection.send(handled_response)
 
     def terminal_cli(self):
         try:
             kwargs = self.parser.parse_args()
-        except:
-            print("Invalid Arguments")
-            os._exit(0)
-        kwargs = vars(kwargs)
-        self.interface(kwargs)
-        os._exit(0)
+            kwargs = vars(kwargs)
+            self.interface(kwargs)
+        except Exception as e:
+            print(e)
+        finally:
+            sys.exit(0)
 
     def cli_window(self):
         title = pyfiglet.figlet_format("-----------\nTapisCLICICLE\n-----------", font="slant") # print the title when CLI is accessed
         print(title)
-        print(r"""If you find any issues, please create a new issue here: https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/issues
-                Enter 'exit' to exit the client
+        print(r"""Enter 'exit' to exit the client
                 Enter 'shutdown' to shut down the client and server
                 Enter 'Help' to show command options""")
         while True:
             try:
                 time.sleep(0.01)
                 kwargs: dict = vars(self.parser.parse_args(str(input(f"[{self.username}@{self.url}][{self.current_system}]{self.pwd} ")).split(" ")))
                 self.interface(kwargs)
             except KeyboardInterrupt:
                 continue
+            except exceptions.Shutdown:
+                print("Server shutdown, exiting")
+                kwargs = vars(self.parser.parse_args(['shutdown']))
+                response_message = schemas.CommandData(request_content=kwargs)
+                self.connection.send(response_message)
+                self.connection.close()
+                break
             except (ConnectionAbortedError, ConnectionResetError):
                 print("Server shutdown, exiting")
-                os._exit(0)
+                self.connection.close()
+                break
             except (TypeError, argparse.ArgumentError, argparse.ArgumentTypeError) as e:
                 print(e)
                 error_str = traceback.format_exc()
                 print(error_str)
                 print("Invalid command")
             except Exception as e:
                 error_str = traceback.format_exc()
                 if self.debug:
                     print(error_str)
+                print(e)
                 error_message = schemas.ResponseData(error=str(e))
                 self.connection.send(error_message)
         
 
     def main(self):
         if len(sys.argv) > 1: # checks if any command line arguments were provided. Does not open CLI
             self.terminal_cli()
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/client/handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from getpass import getpass
 import os
 import json
 
 from prompt_toolkit.validation import Validator, ValidationError
+from prompt_toolkit.completion import word_completer, WordCompleter
 from prompt_toolkit import prompt
 from blessed import Terminal
 
 if __name__ != "__main__":
     from ..socketopts import schemas
 
 
@@ -34,45 +35,34 @@
                 self.print_response(data, depth=depth+1)
         elif isinstance(input_data, (int, str)):
             print(input_data)
         if depth == 0:
             print("\n")
 
 
-def cast_int(data):
-    return int(data)
-
-def cast_string(data):
-    return str(data)
-
-
 class ParserTypeLenEnforcer:
-        type_map = {'int':cast_int, 'string':cast_string}
         def __init__(self, name: str=str(), size: tuple=(0, 0), data_type: str='string', choices: list=list()):
             self.arg_name = name
-            self.update_data_type(data_type)
+            self.data_type = data_type
             self.lower_size_limit, self.upper_size_limit = size
             self.choices = choices
 
-        def update_data_type(self, d_type_str):
-            try:
-                self.data_type = self.type_map[d_type_str]
-            except KeyError:
-                self.data_type = None
-
         def update_constraints(self, name=None, data_type=None, choices=None, size_limit=None, **kwargs):
             self.arg_name = name
-            self.data_type = self.update_data_type(data_type)
+            self.data_type = data_type
             self.choices = choices
             self.lower_size_limit, self.upper_size_limit = size_limit
 
         def __call__(self, data):
             if self.data_type:
                 try:
-                    self.data_type(data)
+                    if self.data_type == 'string':
+                        str(data)
+                    elif self.data_type == 'int':
+                        int(data)
                 except Exception as e:
                     raise ValidationError(message=str(e) + self.data_type, cursor_position=0)
             if self.data_type == int:
                 if not data >= self.lower_size_limit or not data < self.upper_size_limit:
                     raise ValidationError(message=f"The input for the argument {self.arg_name} must be in the range ({self.lower_size_limit}, {self.upper_size_limit}). Got value {data}", cursor_position=0)
             elif self.data_type == str:
                 if not len(data) >= self.lower_size_limit or not len(data) < self.upper_size_limit:
@@ -104,89 +94,129 @@
         line = ''
         while line != 'exit': 
             line = str(input("> "))
             if line != 'exit':
                 expression += line
         return expression
     
-    def confirmation_handler(self):
-        print("are you sure?")
+    def confirmation_handler(self, argument):
+        print(argument['name'])
         while True:
             decision = str(input("(y/n)"))
             if decision == 'y':
                 decision = True
                 break
             elif decision == 'n':
                 decision = False
                 break
             else:
                 print("Enter valid response")
         return decision
     
+    def input_dict_handler(self, term: Terminal, attrs: dict):
+        mode = 'create'
+        answer = dict()
+        default_name = attrs['data_type']['name']
+        with term.fullscreen():
+            print(f"You are now entering data for {attrs['name']}")
+            while True:
+                print(f"{term.clear}{attrs['name']}\nreserved names: create, delete, exit (enter these for special action)\n{answer}\nmode: {mode}")
+                attrs['data_type']['name'] = default_name
+                name = str(input(f"enter the name for the instance of your {attrs['data_type']['name']}: "))
+                if name.lower() in ('delete', 'create'):
+                    mode = name
+                    continue
+                if name.lower() == 'exit':
+                    return answer
+                if mode == 'create':
+                    mode = 'create'
+                    attrs['data_type']['name'] = name
+                    sub_answer = self.form_handler({name:attrs['data_type']}, term)
+                    answer.update(**sub_answer)
+                elif mode == 'delete':
+                    mode = 'delete'
+                    try:
+                        answer.pop(name)
+                    except KeyError:
+                        pass
+
+    def input_list(self, term: Terminal, attrs: dict):
+        answer = []
+        with term.fullscreen():
+            print(f"You are now entering data for {attrs['name']}")
+            while True:
+                presentable_dict = {str(index+1):value for index, value in enumerate(answer)}
+                print(f"{term.clear}{attrs['name']}\nreserved names: exit, new (enter these for special action). Enter index of an existing variable name to delete it\n{presentable_dict}")
+                decision = input("Enter 'new' or 'exit': ")
+                if decision.lower() == 'exit':
+                    return answer
+                elif decision.lower() == 'new':
+                    pass
+                elif decision.isdigit():
+                    try:
+                        answer.pop(int(decision)-1)
+                    except IndexError:
+                        continue
+                    continue
+                else:
+                    continue
+                sub_answer = self.form_handler({str(len(answer)+1):attrs['data_type']}, term)
+                index, value = list(sub_answer.items())[0]
+                answer.append(value)
+    
     def form_handler(self, form_request: dict, term: Terminal):
         response = dict()
-        repeat = False
         for field, attrs in form_request.items():
-            while True:
-                arg_type = attrs['arg_type']
-                self.validator.enforcer.update_constraints(**attrs)
-                try:
-                    match arg_type:
-                        case 'secure':
-                            answer = prompt(f"{attrs['name']}: ", validator=self.validator, is_password=True)
-                        case 'expression':
-                            with term.fullscreen():
-                                print(f"Enter expression input for the {attrs['name']} argument.")
-                                answer = self.__expression_input()
-                        case 'form':
-                            answer = self.form_handler(attrs['arguments_list'], term)
-                        case 'input_list':
-                            repeat = True
-                            answer = []
-                            with term.fullscreen():
-                                print(f"You are now entering data for the {attrs['args']} field")
-                                while repeat:
-                                    sub_answer, repeat = self.form_handler(attrs['data_type'], term)
-                                    answer.append(sub_answer)
-                        case 'input_dict':
-                            repeat = True
-                            answer = dict()
-                            with term.fullscreen():
-                                print(f"You are now entering data for the {attrs['args']} field")
-                                while repeat:
-                                    name = str(input(f"enter the {attrs['data_type']['name']} for the instance of {attrs['name']}"))
-                                    sub_answer, repeat = self.form_handler(attrs['data_type'], term)
-                                    answer[name] = sub_answer
-                        case 'str_input':
-                            answer = prompt(f"{attrs['name']}: ", validator=self.validator)
-                        case 'confirmation':
-                            answer = self.confirmation_handler()
-                        case 'silent':
-                            continue
-                        case _:
-                            raise AttributeError(f"There is not argument type {arg_type}")
-                    response[field] = answer
-                    break
-                except KeyboardInterrupt:
-                    raise RuntimeError('Form cancelled, command execution stopped')
-                except Exception as e:
-                    with open(saved_command, 'w') as f:
-                        f.write(json.dumps(response))
-                        print(f"Argument input failure, command data written to file {saved_command}")
-                        raise e
-        return response, repeat
+            arg_type = attrs['arg_type']
+            self.validator.enforcer.update_constraints(**attrs)
+            try:
+                match arg_type:
+                    case 'secure':
+                        answer = prompt(f"{attrs['name']}: ", validator=self.validator, is_password=True)
+                    case 'expression':
+                        with term.fullscreen():
+                            print(f"Enter expression input for the {attrs['name']} argument.")
+                            answer = self.__expression_input()
+                    case 'form':
+                        answer = self.form_handler(attrs['arguments_list'], term)
+                    case 'input_list':
+                        answer = self.input_list(term, attrs)
+                    case 'input_dict':
+                        answer = self.input_dict_handler(term, attrs)
+                    case 'str_input':
+                        completer = None
+                        if 'description' in attrs and attrs['description']:
+                            print(attrs['description'])
+                        if 'choices' in attrs and attrs['choices']:
+                            completer = WordCompleter(attrs['choices'])
+                        answer = prompt(f"{attrs['name']}: ", validator=self.validator, wrap_lines=True, completer=completer)
+                    case 'confirmation':
+                        answer = self.confirmation_handler(attrs)
+                    case 'silent':
+                        continue
+                    case _:
+                        raise AttributeError(f"There is not argument type {arg_type}")
+                response[field] = answer
+            except KeyboardInterrupt:
+                raise RuntimeError('Form cancelled, command execution stopped')
+            except Exception as e:
+                with open(saved_command, 'a') as f:
+                    f.write(json.dumps(response))
+                    print(f"Argument input failure, command data written to file {saved_command}")
+                    raise e
+        return response
     
     def universal_message_handler(self, message: schemas.BaseSchema, term: Terminal):
         self.print_response(message.message)
         if message.error:
             self.print_response(message.error)
         if message.request_content:
-            filled_form, repeat = self.form_handler(message.request_content, term)
-            return filled_form, repeat
-        return None, None
+            filled_form = self.form_handler(message.request_content, term)
+            return filled_form
+        return None
         
     def environment_cli_response_stream_handler(self, response):
         if response.schema_type == 'ResponseData' and response.exit_status: # if the command was a shutdown or exit, close the program
             self.print_response(response.response_message)
             os._exit(0)
         elif response.schema_type == 'ResponseData':
             if response.active_username:
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 import abc
 
 
 ALLOWED_ARG_TYPES = typing.Literal['silent', 'secure', 'expression', 'input_list', 'input_dict', 'form', 'str_input', 'confirmation']
-ALLOWED_DATA_TYPES = typing.Literal['string', 'int']
+ALLOWED_DATA_TYPES = typing.Literal['string', 'int', 'bool']
 ALLOWED_ACTIONS = typing.Literal['store', 'store_true', 'store_false']
 
 
 class DynamicChoiceList(abc.ABC):
     @abc.abstractmethod
     def __call__(self, tapis_instance):
         pass
@@ -21,19 +21,23 @@
 
 def cast_int(data):
     return int(data)
 
 def cast_string(data):
     return str(data)
 
+def cast_bool(data):
+    return bool(data)
+
 
 class Argument(AbstractArgument):
     type_map = {
         'int':cast_int,
-        'string':cast_string
+        'string':cast_string,
+        'bool':cast_bool
     }
     def __init__(self, argument: str,
                  data_type: ALLOWED_DATA_TYPES | typing.Type[AbstractArgument] = 'string',
                  arg_type: ALLOWED_ARG_TYPES | typing.Literal['standard']='standard',
                  choices: list | typing.Type[DynamicChoiceList] | None=None, 
                  action: typing.Literal['store', 'store_true', 'store_false']="store", 
                  description: str="",
@@ -42,14 +46,18 @@
                  size_limit: tuple=(0,4096)):
         if arg_type not in typing.get_args(ALLOWED_ARG_TYPES) and arg_type != 'standard':
             raise ValueError(f"The arg type parameter in the argument {self.__class__.__name__} must be in the list {ALLOWED_ARG_TYPES}. Got arg type {arg_type}")
         if data_type not in typing.get_args(ALLOWED_DATA_TYPES) and not issubclass(data_type.__class__, AbstractArgument):
             raise ValueError(f"The data type argument provided to the argument {self.__class__.__name__} must be in the list {ALLOWED_DATA_TYPES}, or must be a subclass of AbstractArgument")
         if action not in typing.get_args(ALLOWED_ACTIONS):
             raise ValueError(f"Action {action} not in the list {ALLOWED_ACTIONS}, in argument {self.__class__.__name__}")
+        if arg_type in ('input_list', 'input_dict') and isinstance(data_type, Argument) and data_type.arg_type == 'standard':
+            data_type.arg_type = 'str_input'
+        if action != 'store':
+            data_type = 'bool'
         self.argument = argument
         self.arg_type = arg_type
         self.data_type = data_type
         self.choices = choices
         if self.arg_type != 'standard':
             action = 'store_true'
         self.action = action
@@ -59,26 +67,33 @@
         self.size_limit=size_limit
 
         self.truncated_arg = None
         self.full_arg = f"--{self.argument}"
 
     def verify_standard_value(self, value):
         if self.arg_type == "standard":
-            print(type(self.size_limit))
+            #print(f"ARGUMENT NAME: {self.argument}\nARGUMENT VALUE: {value}\n")
+            if value == None and self.default_value:
+                value = self.default_value
+                return value
+            elif not value:
+                return value
             min_, max_ = self.size_limit
             try:
                 value = self.type_map[self.data_type](value)
             except:
                 raise ValueError(f"The argument {self.argument} requires a datatype {self.data_type}")
             if type(value) == int:
                 if value >= max_ or value < min_:
                     raise ValueError(f"The argument {self.argument} must be a value in the range {self.size_limit}")
-            elif type(value) == str and len(value) >= max_ or len(value) < min_:
+            elif type(value) == str and (len(value) >= max_ or len(value) < min_):
                 raise ValueError(f"The argument {self.argument} must be between the sizes {self.size_limit}")
             elif self.choices and value not in self.choices:
+                print(value)
+                print(self.choices)
                 raise ValueError(f"The value for argument {self.argument} must be in the list {self.choices}")
             elif value == None and self.default_value:
                 value = self.default_value
         return value
 
     def json(self):
         json = {
@@ -90,56 +105,77 @@
             'description':self.description,
             'positional':self.positional,
             'default_value':self.default_value,
             'size_limit':self.size_limit,
             'truncated_arg':self.truncated_arg,
             'full_arg':self.full_arg
         }
-        if self.data_type in ('string', 'int'):
+        if self.data_type in ('string', 'int', 'bool'):
             json['data_type'] = self.data_type
         else:
             json['data_type'] = self.data_type.json()
         return json
     
     def help_message(self):
         help = {"name":self.argument,
-                    "description":f"{self.description}"}
-        if self.action == 'store':
-            help['syntax'] = f"{self.truncated_arg}/{self.full_arg} <{self.argument}>"
-        elif self.positional:
+                "description":f"{self.description}"}
+        if self.choices:
+            help['choices'] = self.choices
+        if self.positional:
             help['syntax'] = f"<{self.argument}>"
-        elif self.action != 'store':
+        elif self.action == 'store':
+            help['syntax'] = f"{self.truncated_arg}/{self.full_arg} <{self.argument}>"
+        else:
             help['syntax'] = f"{self.truncated_arg}/{self.full_arg}"
+            if self.arg_type != 'standard':
+                help['syntax'] = help['syntax'] + " (f)"
         return help
     
     def check_for_copy_data(self):
         return {
             'name':self.argument,
             'action':self.action,
         }
     
     def str(self):
         help_str = f"{self.truncated_arg}/{self.full_arg} "
         if self.positional:
-            help_str = f"{self.argument} "
+            help_str = f"<{self.argument}> "
         elif self.action == 'store':
             help_str += f"<{self.argument}> "
+        if self.arg_type != 'standard':
+            help_str += ' (f)'
         return help_str
 
 
 class Form(Argument):
     def __init__(self, form_name, arguments_list):
         super().__init__(form_name, arg_type='form')
         for argument in arguments_list:
             if argument.arg_type == 'standard':
                 argument.arg_type = 'str_input'
         self.arguments_list = {argument.argument:argument for argument in arguments_list}
 
     def json(self):
-        return {argument_name:argument.json() for argument_name, argument in self.arguments_list.items()}
+        fields = {argument_name:argument.json() for argument_name, argument in self.arguments_list.items()}
+        json = {
+            'name':self.argument,
+            'arg_type':self.arg_type,
+            'data_type':self.data_type,
+            'choices':self.choices,
+            'action':self.action,
+            'description':self.description,
+            'positional':self.positional,
+            'default_value':self.default_value,
+            'size_limit':self.size_limit,
+            'truncated_arg':self.truncated_arg,
+            'full_arg':self.full_arg,
+            'arguments_list':fields
+        }
+        return json
     
 
 class RequestHandler:
     def handle_requests(self, request):
         pass
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,27 @@
 import inspect
 import abc
 import ast
 import json
 from typing import Type
 import typing
 from abc import abstractmethod, ABC
+import os
+from pprint import pprint
 
 from commands import decorators # I finally understand. Imported at the top level by serverRun, so it can only see packages from that vantage point
 from utilities import exceptions
 from commands.arguments.argument import Argument, DynamicChoiceList, ALLOWED_ARG_TYPES
 from socketopts import schemas
+from commands import dataFormatters
+
+
+__location__ = os.path.realpath(
+    os.path.join(os.getcwd(), os.path.dirname(f"{__file__}")))
+saved_command = os.path.join(__location__, r'entered_command.json')
 
 
 def get_kwargs(function):
     sig = inspect.signature(function)
     keyword_args = [param.name for param in sig.parameters.values() if param.default != inspect.Parameter.empty]
     return keyword_args
 
@@ -95,61 +103,77 @@
     
     def dict(self):
         return self.arguments
 
 
 class BaseCommand(ABC, HelpStringRetriever, metaclass=CommandMetaClass):
     decorator = None
-    return_formatter = None
+    return_fields: list = []
     command_opt: list = None
     supports_config_file: bool = False
     required_arguments: list[Argument] | dict = list()
     optional_arguments: list[Argument] | dict = list()
     def __init__(self):
         self.t = None
         self.username = None
         self.password = None
         self.server = None
         self.arguments = dict()
+        self.return_formatter: dataFormatters.BaseDataFormatter = dataFormatters.BaseDataFormatter(self.return_fields)
+        self.default_commands()
+        if self.supports_config_file:
+            self.optional_arguments.append(Argument('file'))
         if isinstance(self.required_arguments, list):
             self.required_arguments = {argument.argument:argument for argument in self.required_arguments}
-            self.required_arguments['connection'] = Argument('connection', arg_type='silent')
             self.arguments.update(**self.required_arguments)
         if isinstance(self.optional_arguments, list):  
             self.optional_arguments = {argument.argument:argument for argument in self.optional_arguments}
             self.arguments.update(**self.optional_arguments)
         self.positional_arguments = [arg_name for arg_name, arg in self.required_arguments.items() if arg.positional]
         self.form_arguments = [arg_name for arg_name, arg in self.arguments.items() if arg.arg_type not in  ('standard', 'silent')]
         self.help: dict[dict[str, list[dict[str, str]]]] = dict()
 
-        self.command_execution_sequence = [self.verify_argument_rules_followed]
+        self.command_execution_sequence = []
         if self.supports_config_file:
             self.command_execution_sequence.append(self.handle_config_file)
-        if self.form_arguments:
-            self.command_execution_sequence.append(self.handle_form_input)
         if self.positional_arguments:
             self.command_execution_sequence.append(self.check_for_positionals)
         if self.command_opt:
             self.command_execution_sequence.append(self.handle_arg_opts)
+        self.command_execution_sequence.append(self.verify_argument_rules_followed)
+        if self.form_arguments:
+            self.command_execution_sequence.append(self.handle_form_input)
+        self.command_execution_sequence.append(self.verify_argument_rules_followed)
         self.command_execution_sequence.append(self.filter_kwargs)
 
+    def default_commands(self):
+        default_commands = [Argument('connection', arg_type='silent'),
+                            Argument('verbose', arg_type='silent'),
+                            Argument('help', arg_type='silent'),
+                            Argument('positionals', arg_type='silent')]
+        
+        for command in default_commands:
+            self.required_arguments.append(command)
+
     async def verify_argument_rules_followed(self, kwargs):
-        for name, value in kwargs.items():
-            if name in self.optional_arguments and value and name not in self.form_arguments:
-                kwargs[name] = self.optional_arguments[name].verify_standard_value(value)
-            elif name in self.required_arguments:
-                kwargs[name] = self.required_arguments[name].verify_standard_value(value)
+        print("ACTIVATED THE ARGUMENT RULES TESTER")
+        for name, value in self.arguments.items():
+            if name in self.required_arguments and kwargs[name] == None:
+                raise Exception(f"The argument {name} is required by the command {self.__class__.__name__}")
+            elif name in kwargs and name in self.required_arguments and name not in self.form_arguments:
+                kwargs[name] = self.required_arguments[name].verify_standard_value(kwargs[name])
+            elif name in kwargs and name in self.optional_arguments and name not in self.form_arguments:
+                kwargs[name] = self.optional_arguments[name].verify_standard_value(kwargs[name])
         return kwargs
 
     async def filter_kwargs(self, kwargs):
         filtered_kwargs = dict()
         for arg, value in kwargs.items():
-            if arg in self.arguments and value != None:
-                if (self.arguments[arg].arg_type in typing.get_args(ALLOWED_ARG_TYPES) and kwargs[arg]) or self.arguments[arg].arg_type == 'standard':
-                    filtered_kwargs[arg] = value
+            if arg in self.arguments and value or arg in self.required_arguments or (value == False and arg in self.arguments and self.arguments[arg].arg_type == 'standard'):
+                filtered_kwargs[arg] = value
         return filtered_kwargs
 
     async def handle_config_file(self, kwargs):
         if kwargs['file']:
             with open(kwargs['file'], 'r') as f:
                 kwargs = json.loads(f.read)
         return kwargs
@@ -157,15 +181,14 @@
     async def handle_form_input(self, kwargs):
         for arg_name in self.form_arguments:
             if kwargs[arg_name] or arg_name in self.required_arguments:
                 request = schemas.FormRequest(request_content={arg_name:self.arguments[arg_name] for arg_name in self.form_arguments if kwargs[arg_name] or arg_name in self.required_arguments})
                 await kwargs['connection'].send(request)
                 response: schemas.FormResponse = await kwargs['connection'].receive()
                 kwargs.update(**response.request_content)
-        print(kwargs)
         return kwargs
     
     async def handle_arg_opts(self, kwargs):
         for opt in self.command_opt:
             kwargs = opt(kwargs)
         return kwargs
     
@@ -213,35 +236,51 @@
         else:
             help_dict.update(**{
                 "Syntax":f"{self.__class__.__name__}",
                 "Required Arguments":self.help['required']['verbose'],
                 "Optional Arguments":self.help['optional']['verbose']})
         return help_dict
     
+    def brief_help(self):
+        return {"Command":self.__class__.__name__,
+                "Description":self.help_string_retriever()}
+    
     @abstractmethod
     async def run(self, *args, **kwargs):
         pass
 
     async def __call__(self, **kwargs):
-        command = kwargs.pop('command_selection')
-
+        pprint(kwargs)
         if self.decorator:
-            return_value = await self.decorator(input_command=self, **kwargs)
-        
-        verbose = kwargs.pop('verbose')
-        help = kwargs.pop('help')
+            try:
+                return_value = await self.decorator(input_command=self, **kwargs)
+            except (ValueError, exceptions.NoConfirmationError) as e:
+                return f"Command execution failed due to {e}"
 
-        if help:
-            return self.__get_help(verbose=verbose)
+        if kwargs['help']:
+            return self.__get_help(verbose=kwargs['verbose'])
         for handler in self.command_execution_sequence:
+            print(f"EXECUTING: {handler.__name__}")
             kwargs = await handler(kwargs)
+            pprint(f"{kwargs}\n")
         else:
-            return_value = await self.run(**kwargs)
+            try:
+                return_value = await self.run(**kwargs)
+            except exceptions.Shutdown as e:
+                raise e
+            except Exception as e:
+                with open(saved_command, 'a') as f:
+                    kwargs.pop('connection')
+                    f.write(json.dumps(kwargs))
+                    print(f"Argument input failure, command data written to file {saved_command}")
+                    raise e
         if self.return_formatter:
-            return_value = self.return_formatter(return_value, verbose)
+            return_value = self.return_formatter(return_value, kwargs['verbose'])
+        else:
+            return_value = str(return_value)
         return return_value
     
 
 class BaseQuery(BaseCommand):
     def get_pod_credentials(self, id):
         uname, pword = self.t.pods.get_pod_credentials(pod_id=id).user_username, self.t.pods.get_pod_credentials(pod_id=id).user_password
         return uname, pword
@@ -253,35 +292,27 @@
 
 class CommandMapMetaClass(type):
     def __new__(cls, name, bases, attrs):
         instance = super().__new__(cls, name, bases, attrs)
         if name not in ('CommandMapMetaClass', 'BaseCommandMap'):
             instance.__check_commands_are_proper_type(name, attrs)
             instance.__check_command_name(name, attrs)
-            instance.__check_data_formatter(name, attrs)
             instance.__special_command_opts(name, attrs)
         return instance
     
     def __check_commands_are_proper_type(self, name, attrs):
         commands = attrs['command_map']
         if not commands:
             raise AttributeError(f"The command group {name} has no commands!")
-        for command_name, command in commands.items():
-            if not issubclass(command.__class__, BaseCommand):
-                raise AttributeError(f"The command {command_name} was not passed to the {name} as a class, but as an object. Ensure you do not instantiate commands when defining the class")
             
     def __check_command_name(self, name, attrs):
         commands = attrs['command_map']
         for command_name, command in commands.items():
             if command_name != command.__class__.__name__:
                 raise AttributeError(f"The command {command_name} in the command map {name} is a different name from its corresponding command class, {command.__class__.__name__}")
-            
-    def __check_data_formatter(self, name, attrs):
-        if 'data_formatter' not in list(attrs.keys()):
-            print(f"WARNING: The command map {name} has no data formatter. If any commands have non json-serializable return values, command execution will fail! These must be handled by a formatter")
 
     def __special_command_opts(self, name, attrs):
         if 'command_opt' in list(attrs.keys()):
             if type(attrs['command_opt']) != list:
                 raise TypeError(f"The command_opt attribute for the command group {name} must be a list!")
             for command_name, command in attrs['command_map'].items():
                 if not command.command_opt:
@@ -297,37 +328,35 @@
         'verbose':Argument('verbose', action='store_true'),
         'file':Argument('file')
     }
 
 
 class BaseCommandMap(CommandContainer, HelpStringRetriever, metaclass=CommandMapMetaClass):
     command_map: dict[str, Type[BaseCommand]] = None
-    data_formatter = None
     command_opt = None
     def __init__(self):
         self.brief_help = self.__brief_help_gen()
         self.verbose_help = self.__help_gen()
         for name, command in self.command_map.items():
-            command.return_formatter = self.data_formatter
             self.aggregate_command_map.update({name:command})
             if command.required_arguments or command.optional_arguments:
                 self.__contribute_to_arguments(command)
 
     def __contribute_to_arguments(self, command):
         arg_dict = {**command.required_arguments, **command.optional_arguments}
         for name, arg in arg_dict.items():
             if name not in self.arguments:
                 self.arguments[name] = arg
             elif self.arguments[name].check_for_copy_data() != arg.check_for_copy_data():
                 raise ValueError(f"Found two instances of the argument {arg.argument} that had different attributes.\n\n{command.__class__.__name__}: {arg.check_for_copy_data()}\n\nvs\n\n{self.arguments[name].check_for_copy_data()}")
 
     def __help_gen(self):
-        verbose_help = dict()
+        verbose_help = list()
         for command in self.command_map.values():
-            verbose_help.update({command.__class__.__name__:command.help})
+            verbose_help.append(command.brief_help())
         return verbose_help
     
     def __brief_help_gen(self):
         brief_help = {
             'group':self.__class__.__name__,
             'description':self.help_string_retriever(),
             'instruction':f"enter {self.__class__.__name__} to retrieve list of commands"
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/commandMap.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,92 @@
 if __name__ != "__main__":
-    from . import systemCommands, volumeCommands, serverCommands, appCommands, podCommands, fileCommands, dataFormatters, baseCommand
+    from . import systemCommands, volumeCommands, serverCommands, appCommands, podCommands, fileCommands, dataFormatters, baseCommand, jobCommands
     from .query import postgres, neo4j
     from utilities import exceptions
     from commands.arguments.argument import Argument
     from commands.commandOpts import CHECK_EXPLICIT_ID
 
 
 class Systems(baseCommand.BaseCommandMap):
     """
     @help: run operations on Tapis systems
     """
-    data_formatter = dataFormatters.DataFormatters.system_formatter
     command_map = {
         'get_systems':systemCommands.get_systems(), # since initialization of commands is separate from __init__, you dont need to specify these as classes anymore
         'get_system_info':systemCommands.get_system_info(),
         'get_scheduler_profiles':systemCommands.get_scheduler_profiles(),
+        'submit_system_credentials':systemCommands.submit_system_credentials(),
         'verify_pki_keys':systemCommands.verify_pki_keys(),
-        'create_child_system':systemCommands.create_child_system(),
         'create_system':systemCommands.create_system(),
         'update_system':systemCommands.update_system(),
-        'is_enabled':systemCommands.is_enabled(),
+        'is_system_enabled':systemCommands.is_system_enabled(),
         'enable_system':systemCommands.enable_system(),
         'disable_system':systemCommands.disable_system(),
         'system':systemCommands.system(),
         'exit_system':systemCommands.exit_system(),
         'delete_system':systemCommands.delete_system(),
-        'undelete_system':systemCommands.undelete_system()
+        'undelete_system':systemCommands.undelete_system(),
+        'create_child_system':systemCommands.create_child_system(),
+        'unlink_child_system':systemCommands.unlink_child_system(),
+        'unlink_children':systemCommands.unlink_children(),
+        'get_user_perms':systemCommands.get_user_perms(),
+        'grant_user_perms':systemCommands.grant_user_perms(),
+        'revoke_user_perms':systemCommands.revoke_user_perms(),
     }
 
 
-class Server(baseCommand.BaseCommandMap):
+class General(baseCommand.BaseCommandMap):
     """
     @help: run config operations on the 
     """
-    data_formatter = dataFormatters.DataFormatters.server_formatter
     command_map = {
+        'get_tenants':serverCommands.get_tenants(),
+        'get_tenant':serverCommands.get_tenant(),
         'whoami':serverCommands.whoami(),
+        'user':serverCommands.user(),
         'whereami':serverCommands.whereami(),
         'exit':serverCommands.exit(),
         'shutdown':serverCommands.shutdown(),
         "get_args":serverCommands.get_args(),
-        'switch_service':serverCommands.switch_service()
+        'switch_service_to':serverCommands.switch_service_to(),
+        'manpages':serverCommands.manpages()
     }
 
 
 class Pods(baseCommand.BaseCommandMap):
     """
     @help: run operations on tapis pods
     """
-    data_formatter = dataFormatters.DataFormatters.pod_formatter
     command_map = {
         'get_pods':podCommands.get_pods(),
         'get_pod':podCommands.get_pod(),
         'create_pod':podCommands.create_pod(),
         'update_pod':podCommands.update_pod(),
         'start_pod':podCommands.start_pod(),
         'restart_pod':podCommands.restart_pod(),
         'delete_pod':podCommands.delete_pod(),
         'set_pod_perms':podCommands.set_pod_perms(),
         'stop_pod':podCommands.stop_pod(),
         'delete_pod_perms':podCommands.delete_pod_perms(),
-        'get_perms':podCommands.get_perms(),
+        'get_pod_perms':podCommands.get_pod_perms(),
         'copy_pod_password':podCommands.copy_pod_password(),
         'get_pod_logs':podCommands.get_pod_logs(),
     }
 
 
 class Volumes(baseCommand.BaseCommandMap):
     """
     @help: run operations on tapis volumes and snapshots
     """
     command_map = {
         'get_volumes':volumeCommands.get_volumes(),
         'create_volume':volumeCommands.create_volume(),
         'get_volume':volumeCommands.get_volume(),
         'volume':volumeCommands.volume(),
+        'exit_volume':volumeCommands.exit_volume(),
         'update_volume':volumeCommands.update_volume(),
         'delete_volume':volumeCommands.delete_volume(),
         'dir':volumeCommands.dir(),
         'upload_volume':volumeCommands.upload_volume(),
         'set_volume_permission':volumeCommands.set_volume_permission(),
         'get_volume_permissions':volumeCommands.get_volume_permissions(),
         'delete_volume_permission':volumeCommands.delete_volume_permission(),
@@ -94,44 +102,75 @@
 class Files(baseCommand.BaseCommandMap):
     """
     @help: run operations on tapis files
     """
     command_map = {
         'ls':fileCommands.ls(),
         'cd':fileCommands.cd(),
+        'pwd':fileCommands.pwd(),
         'showme':fileCommands.showme(),
         'cat':fileCommands.cat(),
         'mkdir':fileCommands.mkdir(),
         'mv':fileCommands.mv(),
         'cp':fileCommands.cp(),
         'rm':fileCommands.rm(),
-        'get_recent_transfers':fileCommands.get_recent_transfers(),
+        #'get_recent_transfers':fileCommands.get_recent_transfers(),
         'create_postit':fileCommands.create_postit(),
         'list_postits':fileCommands.list_postits(),
         'get_postit':fileCommands.get_postit(),
         'delete_postit':fileCommands.delete_postit(),
         'redeem_postit':fileCommands.redeem_postit(),
         'upload':fileCommands.upload(),
         'download':fileCommands.download(),
     }
 
 
 class Apps(baseCommand.BaseCommandMap):
     """
     @help: Run operations on tapis apps
     """
-    data_formatter = dataFormatters.DataFormatters.app_formatter
     command_map = {
         'create_app':appCommands.create_app(),
+        'update_app':appCommands.update_app(),
         'get_apps':appCommands.get_apps(),
         'delete_app':appCommands.delete_app(),
         'get_app':appCommands.get_app(),
-        'run_job':appCommands.run_job(),
-        'get_job_status':appCommands.get_job_status(),
-        'download_job_output':appCommands.download_job_output(),
+        'assign_default_job_attributes':appCommands.assign_default_job_attributes(),
+        'is_app_enabled':appCommands.is_app_enabled(),
+        'enable_app':appCommands.enable_app(),
+        'disable_app':appCommands.disable_app(),
+        'undelete_app':appCommands.undelete_app(),
+        'get_app_history':appCommands.get_app_history(),
+        'get_app_user_perms':appCommands.get_app_user_perms(),
+        'grant_app_user_perms':appCommands.grant_app_user_perms(),
+        'revoke_app_user_perms':appCommands.revoke_app_user_perms()
+    }
+
+
+class Jobs(baseCommand.BaseCommandMap):
+    """
+    @help: run jobs on a tapis system
+    """
+    command_map = {
+        'hide_job':jobCommands.hide_job(),
+        'unhide_job':jobCommands.unhide_job(),
+        'cancel_job':jobCommands.cancel_job(),
+        'get_job':jobCommands.get_job(),
+        'get_job_history':jobCommands.get_job_history(),
+        'get_jobs':jobCommands.get_jobs(),
+        'download_job_output':jobCommands.download_job_output(),
+        'get_job_status':jobCommands.get_job_status(),
+        'resubmit_job':jobCommands.resubmit_job(),
+        'submit_job':jobCommands.submit_job(),
+        'share_job':jobCommands.share_job(),
+        'get_job_share':jobCommands.get_job_share(),
+        'delete_job_share':jobCommands.delete_job_share(),
+        'subscribe_to_job':jobCommands.subscribe_to_job(),
+        'get_subscriptions':jobCommands.get_subscriptions(),
+        'delete_subscriptions':jobCommands.delete_subscriptions()
     }
 
 
 class Query(baseCommand.BaseCommandMap):
     """
     @help: run integrated query CLIs
     """
@@ -145,30 +184,34 @@
     def generate_truncated_arguments(self, arg_dict: dict) -> dict:
         truncation_dict = dict()
         for argument_name in arg_dict.keys():
             truncated_argument = self.__generate_truncated_argument(argument_name, truncation_dict)
             truncation_dict[argument_name] = truncated_argument
         return truncation_dict
             
-    def __generate_truncated_argument(self, argument, truncated_arguments_dict, attempt=1):
-        if argument[attempt-1] in ('_', '-'):
-            attempt += 1
-        truncated_argument = argument[:attempt]
-        if truncated_argument in list(truncated_arguments_dict.values()):
-            return self.__generate_truncated_argument(argument, truncated_arguments_dict, attempt=attempt+1)
-        return truncated_argument
+    def __generate_truncated_argument(self, argument, truncated_arguments_dict, attempts=1):
+        if argument[attempts-1] in ('_', '-'):
+            argument += 1
+        abbreviation = argument[:attempts]
+        for index, letter in enumerate(argument):
+            if letter.isupper() or not (argument[index-1].isnumeric() or argument[index-1].isalpha()):
+                abbreviation += letter.lower()
+
+        if abbreviation.lower() in list(truncated_arguments_dict.values()):
+            abbreviation = self.__generate_truncated_argument(argument, truncated_arguments_dict, attempts=attempts+1)
+        return abbreviation.lower()
     
 
 class AggregateCommandMap(baseCommand.CommandContainer, ArgsGenerator):
     groups = {
         'Systems': Systems(),
-        'Server': Server(),
+        'General': General(),
         'Pods': Pods(),
         'Files': Files(),
-        #'Apps': Apps(),
+        'Apps': Apps(),
         'Query': Query(),
         'Volumes':Volumes()
     }
     def __init__(self):
         truncated_arguments = self.generate_truncated_arguments(self.arguments)
         for command in self.aggregate_command_map.values():
             command.update_args_with_truncated(truncated_arguments)
@@ -188,21 +231,21 @@
 
     async def run_command(self, connection, command_data: dict):
         """
         process and run command based on received kwargs
         """
         command_name = command_data['command_selection']
 
-        if command_name in list(self.aggregate_command_map.keys()):
+        if command_name in self.aggregate_command_map:
             command = self.aggregate_command_map[command_name]
-            if command.supports_config_file and 'file' in list(command_data.keys()) and command_data['file']:
-                command_data = {'file':command_data['file']}
-
             command_data['connection'] = connection
-            command_data['server'] = self
-            return await command(**command_data)
-        elif command_name in list(self.groups.keys()):
+            kwargs = dict()
+            for argument, value in command_data.items():
+                if argument in command.arguments:
+                    kwargs[argument] = value
+            return await command(**kwargs)
+        elif command_name in self.groups:
             return self.groups[command_name]()
         elif command_name == "help":
             return self.help
         else:
             raise exceptions.CommandNotFoundError(command_name)
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,60 +8,68 @@
 
 class ls(baseCommand.BaseCommand):
     """
     @help: list the files on a system 
     """
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
         Argument('file_path', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs) -> str: # lists files available on a tapis account
         file_list = self.t.files.listFiles(systemId=kwargs['systemId'], path=kwargs['file_path'])
         file_list_truncated = [f"{file.type} - {file.nativePermissions} ---- {file.name}" for file in file_list]
         return file_list_truncated
     
 
 class cd(baseCommand.BaseCommand):
     """
     @help: change the directory
     """
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
         Argument('file_path', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs):
         self.t.files.listFiles(systemId=kwargs['systemId'], path=kwargs['file_path'])
         kwargs['connection'].pwd = kwargs['file_path']
         return kwargs['connection'].pwd
+    
 
+class pwd(baseCommand.BaseCommand):
+    """
+    @help: get the current directory
+    """
+    async def run(self, *args, **kwargs):
+        return kwargs['connection'].pwd
 
 class showme(baseCommand.BaseCommand):
     """
     @help: display file metadata
     """
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
+    return_fields = ['absolutePath', 'uid', 'size', 'perms']
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
         Argument('file_path', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs):
-        return_data = str(self.t.files.getStatInfo(systemId=kwargs['systemId'], path=kwargs['file_path']))
+        return_data = self.t.files.getStatInfo(systemId=kwargs['systemId'], path=kwargs['file_path'])
         return return_data
     
 
 class cat(baseCommand.BaseCommand):
     """
     @help: display small files directly to the terminal
     """
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
-        Argument('file_path', positional=True)
+        Argument('file_path', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs):
         size = self.t.files.getStatInfo(systemId=kwargs['systemId'], path=kwargs['file_path']).size
         if size <= 4000:
             file_info = self.t.files.getContents(systemId=kwargs['systemId'],
                                 path=kwargs['file_path'])
         else:
@@ -71,136 +79,154 @@
 
 class mkdir(baseCommand.BaseCommand):
     """
     @help: create a new directory at the selected path
     """
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
-        Argument('file_path', positional=True)
+        Argument('file_path', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs):
         self.t.files.mkdir(systemId=kwargs['systemId'], path=kwargs['file_path'])
         return f"Successfully created file at {kwargs['file_path']}"
     
 
 class mv(baseCommand.BaseCommand):
     """
     @help: move a file from a source directory to a destination directory within a system's file structure
     """
     command_opt = [commandOpts.CHECK_PWD(('source_file', 'destination_file')), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
-        Argument('source_file'),
+        Argument('source_file', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True),
         Argument('desination_file')
     ]
     async def run(self, destination_file: str, *args, **kwargs):
         self.t.files.moveCopy(systemId=kwargs['systemId'], path=kwargs['source_file'], operation="MOVE", newPath=destination_file)
         return f"File moved successfully to {destination_file}"
     
 
 class cp(baseCommand.BaseCommand):
     """
     @help: copy a file from a source directory to another directory
     """
     command_opt = [commandOpts.CHECK_PWD(('source_file', 'destination_file')), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
-        Argument('source_file'),
+        Argument('source_file', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True),
         Argument('destination_file')
     ]
     async def run(self, *args, **kwargs):
         self.t.files.moveCopy(systemId=kwargs['systemId'], path=kwargs['source_file'], operation="COPY", newPath=kwargs['destination_file'])
         return f"File copied successfully to {kwargs['destination_file']}"
     
 
 class rm(baseCommand.BaseCommand):
     """
     @help: delete a selected file
     """
     decorator=decorators.NeedsConfirmation()
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
-        Argument('file_path', positional=True)
+        Argument('file_path', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs):
         self.t.delete(systemId=kwargs['systemId'], path=kwargs['file_path'])
         return f"file {kwargs['file_path']} successfully deleted"
     
 
 class get_recent_transfers(baseCommand.BaseCommand):
     """
     @help: return a list of recent file transfers
     """
+    return_fields = ['id', 'username', 'status', 'estimatedTotalBytes']
     async def run(self, *args, **kwargs):
         recent_transfers = self.t.files.getRecentTransferTasks()
-        return str(recent_transfers)
+        return recent_transfers
+    
+
+class create_transfer_task(baseCommand.BaseCommand):
+    """
+    @help: create a task to transfer files between systems. The two system types must be the same
+    """
+    required_arguments = [
+        Argument('source_file_path', positional=True),
+        Argument('source_system_id', positional=True),
+        Argument('destination_system_id'),
+        Argument('destination_file_path')
+    ]
+    async def run(self, *args, **kwargs):
+        pass
     
 
 class create_postit(baseCommand.BaseCommand):
     """
     @help: create a postit to easily share file with other users
     """
+    return_fields = ['postitId', 'systemId', 'path', 'redeemUrl']
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId', size_limit=(1, 80)),
-        Argument('file_path', positional=True)
+        Argument('file_path', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     optional_arguments = [
         Argument('allowed_uses', data_type='int'),
         Argument('expiration_time', data_type='int')
     ]
     async def run(self, *args, **kwargs):
         self.t.files.createPostIt(systemId=kwargs['systemId'], path=kwargs['file_path'], allowedUses=kwargs['allowed_uses'], validSeconds=kwargs['expiration_time'])
         return f"created a postit for the file {kwargs['file_path']}"
     
 
 class list_postits(baseCommand.BaseCommand):
     """
     @help: list all postits
     """
+    return_fields = ['postitId', 'systemId', 'path', 'redeemUrl']
     optional_arguments = [
         Argument('owned_or_all', choices=['ALL', 'OWNED'])
     ]
     async def run(self, *args, **kwargs):
         postit_list = str(self.t.files.listPostIts(listType=kwargs['owned_or_all']))
         return postit_list
     
 
 class get_postit(baseCommand.BaseCommand):
     """
     @help: get a specific postit information based on postit id
     """
+    return_fields = ['postitId', 'systemId', 'path', 'redeemUrl']
     required_arguments = [
-        Argument('postitId'),
+        Argument('postitId', positional=True),
     ]
     async def run(self, *args, **kwargs):
         postit = str(self.t.files.getPostIt(postitId=kwargs['postitId']))
         return postit
     
 
 class delete_postit(baseCommand.BaseCommand):
     """
     @help: get a specific postit information based on postit kwargs['systemId']
     """
     required_arguments = [
-        Argument('postitId'),
+        Argument('postitId', positional=True),
     ]
     async def run(self, *args, **kwargs):
         postit = str(self.t.files.deletePostIt(postitId=kwargs['postitId']))
         return f"Successfully deleted postit {kwargs['postitId']}"
     
 
 class redeem_postit(baseCommand.BaseCommand):
     """
     @help: redeem a postit and download posted file. Downloads to browser
     """
     required_arguments = [
-        Argument('postitId'),
+        Argument('postitId', positional=True),
     ]
     async def run(self, *args, **kwargs):
         self.t.files.redeemPostIt(postitId=kwargs['postitId'])
         return f"Downloading postit {kwargs['postitId']}, check browser"
 
     
 class upload(baseCommand.BaseCommand):
@@ -208,18 +234,17 @@
     @help: upload a file to the system 
     the source and destination files must both be in the file argument, respectively, separated by a comma
     @todo: make it so that this doesnt need to take both source and destination files, but have it so it retrieves the current file location on the tapis system
     and sets that file location to be the upload point. Do the same for downloads but in reverse
     """
     command_opt = [commandOpts.CHECK_PWD(('destination_file',))]
     required_arguments = [
-        Argument('source_file'),
+        Argument('source_file', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True),
         Argument('destination_file'),
-        Argument('systemId', size_limit=(1, 80)),
-        Argument('connection', arg_type='silent')
     ]
     async def run(self, *args, **kwargs) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
         if not kwargs['destination_file']:
             kwargs['destination_file'] = kwargs['connection'].pwd
         self.t.upload(system_id=kwargs['systemId'],
                 source_file_path=kwargs['source_file'],
                 dest_file_path=kwargs['destination_file'])
@@ -229,17 +254,17 @@
 class download(baseCommand.BaseCommand):
     """
     @help: download a file from the system
     the source and destination files must both be in the file argument, respectively, separated by a comma
     """
     command_opt = [commandOpts.CHECK_PWD(('source_file',))]
     required_arguments = [
-        Argument('source_file'),
+        Argument('source_file', positional=True),
+        Argument('systemId', size_limit=(1, 80), positional=True),
         Argument('destination_file'),
-        Argument('systemId', size_limit=(1, 80)),
         Argument('connection', arg_type='silent')
     ]
     async def run(self, *args, **kwargs) -> str: # download a remote file using tapis, operates basically the same as upload
         if not kwargs["source_file"]:
             kwargs["source_file"] = kwargs['connection'].pwd
         file_info = self.t.files.getContents(systemId=kwargs['systemId'],
                             path=kwargs["source_file"])
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,10 +21,8 @@
         return_value = graph.run(kwargs['expression'])
         print(type(return_value))
         if str(return_value) == '(No data)' and 'create' in kwargs['expression'].lower(): # if no data is returned (mostly if something is created) then just say 'success'
             return f'[+][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
         elif str(return_value) == '(No data)':
             return f'[-][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
 
-        print(return_value)
-        print(type(return_value))
-        return str(f'[+][{kwargs["id"]}] {return_value}')
+        return return_value
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,38 +5,62 @@
 
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from utilities import exceptions
     from commands.arguments.argument import Argument
 
 
-class switch_service(baseCommand.BaseCommand):
+class get_tenants(baseCommand.BaseCommand):
+    """
+    @help: get a list of available tenants to authenticate with
+    """
+    async def run(self, *args, **kwargs):
+        return_data = dict()
+        tenants = self.t.tenants.list_tenants()
+        for tenant in tenants:
+            return_data[tenant.tenant_id] = {'uri':tenant.base_url.split('//')[1], 'owner':tenant.owner, 'description':tenant.description}
+        return return_data
+    
+
+class get_tenant(baseCommand.BaseCommand):
+    """
+    @help: get a specific tenant
+    """
+    required_arguments = [
+        Argument('tenant_id', positional=True)
+    ]
+    async def run(self, *args, **kwargs):
+        tenant = self.t.tenants.get_tenant(**kwargs)
+        return {'uri':tenant.base_url.split('//')[1], 'owner':tenant.owner, 'description':tenant.description}
+    
+    
+class switch_service_to(baseCommand.BaseCommand):
     """
     @help: switch the connected tapis service
     @todo: upgrade to federated auth
     """
     required_arguments=[
-        Argument('link', size_limit=(0, 80)),
+        Argument('tenant_uri', size_limit=(0, 80), positional=True),
         Argument('auth', choices=['password', 'device_code', 'federated']),
-        Argument('connection', arg_type='silent')
     ]
-    async def run(self, *args, **kwargs):  # link is the baseURL
+    async def run(self, *args, **kwargs):  # tenant_uri is the baseURL
         auth = kwargs['auth']
-        link = kwargs['link']
+        tenant_uri = kwargs['tenant_uri']
         self.server.auth_type = auth
         if auth == "password":
-            results = await self.server.password_grant(link, kwargs['connection'])
+            results = await self.server.password_grant(tenant_uri, kwargs['connection'])
         elif auth == "device_code":
-            results = await self.server.device_code_grant(link, kwargs['connection'])
+            results = await self.server.device_code_grant(tenant_uri, kwargs['connection'])
         elif auth == "federated":
-            results = await self.server.federated_grant(link, kwargs['connection'])
+            results = await self.server.federated_grant(tenant_uri, kwargs['connection'])
         else:
             results = None
         self.server.configure_decorators(self.server.username, self.server.password)
         self.server.update_credentials(self.server.t, self.server.username, self.server.password)
+        self.server.available_services = self.server.service_checker.check_services(self.server.t)
         return results
       
 
 class exit(baseCommand.BaseCommand):
     """
     @help: exit the CLI without shutting down the service
     """
@@ -44,35 +68,52 @@
         raise exceptions.Exit
     
 
 class shutdown(baseCommand.BaseCommand):
     """
     @help: exit the CLI and shutdown the service
     """
-    decorator = decorators.NeedsConfirmation()
     async def run(self, *args, **kwargs):
         raise exceptions.Shutdown
     
     
 class whoami(baseCommand.BaseCommand):
     """
     @help: returns the username of the current user
     """
     async def run(self, *args, **kwargs) -> str:
         user_info = self.t.authenticator.get_userinfo()
         return user_info
     
 
+class user(baseCommand.BaseCommand):
+    """
+    @help: returns the username of the selected user
+    """
+    required_arguments = [
+        Argument('username', positional=True)
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.authenticator.get_profile(**kwargs)
+
 class get_args(baseCommand.BaseCommand):
     """
     @help: get the list of possible arguments 
     """
     async def run(self, *args, **kwargs):
         return self.server.arguments
     
 
 class whereami(baseCommand.BaseCommand):
     """
     @help: get the URI of current tapis tenant
     """
     async def run(self, *args, **kwargs):
-        return self.server.url
+        return self.server.url
+    
+
+class manpages(baseCommand.BaseCommand):
+    """
+    @help: get a link to the application manpages
+    """
+    async def run(self, *args, **kwargs):
+        return "Please see https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE for manpages (will add actual manpages later)"
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/systemCommands.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class system(baseCommand.BaseCommand):
     """
     @help: set the system to run operations on by default. Running this will put you "in" the system so that you dont have to specify system ID for each command
     """
     required_arguments=[
-        Argument('systemId', size_limit=(1, 80)),
+        Argument('systemId', size_limit=(1, 80), positional=True),
     ]
     async def run(self, *args, **kwargs):
         system_info = self.t.systems.getSystem(systemId=kwargs['systemId'])
         kwargs['connection'].system = kwargs['systemId']
         kwargs['connection'].pwd = system_info.rootDir
         return f"successfully entered the system {kwargs['connection'].system}"
 
@@ -48,39 +48,45 @@
     
 
 class get_systems(baseCommand.BaseCommand):
     """
     @help: Gets and returns the list of systems the current Tapis service and account have access to
     @doc: this is an example of the doc segment of the docstring. not included in help message
     """
+    return_fields = ['id', 'systemType', 'host', 'enabled']
+    optional_arguments = [
+        Argument('listType', choices=['OWNED', 'SHARED_PUBLIC', 'ALL'])
+    ]
     async def run(self, *args, **kwargs):
-        systems = self.t.systems.getSystems()
+        systems = self.t.systems.getSystems(**kwargs)
         return systems
     
 
 class get_system_info(baseCommand.BaseCommand):
     """
     @help: get information on a selected system
     """
+    return_fields = ['id', 'systemType', 'host', 'enabled']
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments=[
-        Argument('systemId', size_limit=(1, 80))
+        Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs): 
         system_info = self.t.systems.getSystem(systemId=kwargs['systemId'])
         return system_info
     
 
 class verify_pki_keys(baseCommand.BaseCommand):
     """
     @help: upload system credentials to a system. Must generate keys first using 'ssh-keygen -m PEM -f id_rsa', and format with, 'awk -v ORS='\\n' '1' <private_key_name>
     file argument must contain the path to the private and public keys respectively, separated by a ','
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId'),
+        Argument('systemId', positional=True),
         Argument('private_key_path'),
         Argument('public_key_path')
     ]
     async def run(self, *args, **kwargs): # get information about a system given its ID
         with open(kwargs['private_key_path'], 'r') as f:
             private_key = f.read()
 
@@ -113,31 +119,31 @@
     """
     @help: create a system. Must have a properly configured system file.
     see the template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/system-config.json
     this command will automatically create and upload the ssh keys
     """
     supports_config_file=True
     required_arguments=[
-        Argument('systemId', size_limit=(1, 80)),
+        Argument('id', size_limit=(1, 80), positional=True),
         Argument('systemType', choices=["LINUX", "S3", "IRODS", "GLOBUS"], description=
                                     """LINUX is a standard linux kernel
                                     S3 refers to an AWS S3 Bucket
                                     IRODS refers to an IRODS data management system
                                     GLOBUS refers to a GLOBUS file system"""),
         Argument('host', size_limit=(1, 256), description="In the case of Linux this is the hostname or IP of the HPC system you want to connect to. For S3, this is the AWS bucket URL"),
         Argument('defaultAuthnMethod', choices=['PASSWORD', "PKI_KEYS", "ACCESS_KEY", "TOKEN", "CERT"], description=
                                     """Depending on your systemType, you will be restricted to certain options.
                                     Linux: PASSWORD, PKI_KEYS
                                     S3: ACCESS_KEY
                                     GLOBUS: TOKEN
                                     IRODS: TOKEN
                                     In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
-        Argument('canExec', action='store_true'),
     ]
     optional_arguments=[
+        Argument('canExec', action='store_true', default_value=False),
         Argument('description', arg_type='str_input', size_limit=(0, 2048)),
         Argument('owner'),
         Argument('enabled', action='store_true'),
         Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
         Argument('bucketName'),
         Argument('rootDir', default_value='/', size_limit=(0, 4096)),
         Argument('port', data_type='int'),
@@ -196,116 +202,146 @@
                 Argument('datatype', choices=['STRING', 'INTEGER', 
                                               'BOOLEAN', 'NUMBER', 
                                               'TIMESTAMP']),
                 Argument('precedence', data_type='int'),
                 Argument('value')
             ]
         )),
-        Argument('tags', arg_type='input_list'),
+        Argument('tags', arg_type='input_list', data_type=Argument('tag', arg_type='str_input')),
         Argument('notes', arg_type='str_input'),
         Argument('importRefId')
     ]
     def __init__(self):
         super().__init__()
         self.sys_auth_map = {"LINUX":{"PASSWORD":self.password_auth, "PKI_KEYS":self.pki_keys_auth}, 
                              "S3":{"ACCESS_KEY":self.access_key_auth}, "GLOBUS":{"TOKEN":self.token_auth}, 
                              "IRODS":{"TOKEN":self.token_auth}}
 
     async def password_auth(self, **kwargs):
-        userName = self.username
-        if self.server.auth_type == 'password':
-            password = self.password
-        else:
-            request = schemas.FormRequest(request_content={"password":Argument('password', arg_type='secure')},
-                                          message=f"Please enter the credentials you entered on the web portal {self.server.url}")
-            await kwargs['connection'].send(request)
-            response = await kwargs['connection'].receive()
-            response_content = response.request_content
-            password = response_content['password']
+        request = schemas.FormRequest(request_content={'username':Argument('username', arg_type='str_input'), "password":Argument('password', arg_type='secure')},
+                                        message={'message':f"Enter your credentials to the select host specified in the system creation"})
+        await kwargs['connection'].send(request)
+        response = await kwargs['connection'].receive()
+        response_content = response.request_content
+        password = response_content['password']
+        loginUserName = response_content['username']
         cred_return_value = self.t.systems.createUserCredential(systemId=kwargs['id'],
-                            userName=userName,
+                            userName=self.username,
+                            loginUser=loginUserName,
                             password=password)
         return cred_return_value
     
     async def token_auth(self, **kwargs):
         session_details = self.systems.getGlobusAuthUrl()
-        request = schemas.FormRequest(message=f"travel to the url {session_details.url} if the page doesnt open on its own, and enter your credentials. Then paste the code displayed to this app",
+        request = schemas.FormRequest(message={"message":f"travel to the url {session_details.url} if the page doesnt open on its own, and enter your credentials. Then paste the code displayed to this app"},
                                       request_content={'Auth_code':Argument('code', arg_type='str_input')})
         webbrowser.open(session_details.url)
         await kwargs['connection'].send(request)
         response = await kwargs['connection'].receive()
         auth_code = response.request_content['Auth_code']
         token_info = self.t.systems.generateGlobusTokens(systemId=kwargs['id'], userName=self.username, authCode=auth_code, sessionId=session_details.sessionId)
-        return str(token_info)
+        cred_return_value = self.t.systems.createUserCredential(systemId=kwargs['id'],
+                                                                userName=self.username,
+                            accessToken=token_info.access_token,
+                            refreshToken=token_info.refresh_token)
+        return cred_return_value
     
     async def access_key_auth(self, **kwargs):
-        request = schemas.FormRequest(message=f"Retrieve the access key and access secret from your S3 bucket",
+        request = schemas.FormRequest(message={"message":f"Retrieve the access key and access secret from your S3 bucket"},
                                       request_content={'access_key':Argument('access_key', arg_type='str_input'), 'access_secret':Argument('access_secret', arg_type='secure')})
         await kwargs['connection'].send(request)
         response = await kwargs['connection'].receive()
         cred_return_value = self.t.systems.createUserCredential(systemId=kwargs['id'],
+                                                                userName=self.username,
                             accessKey=response.request_content['access_key'],
                             password=response.request_content['access_secret'])
         return cred_return_value
     
     async def pki_keys_auth(self, **kwargs):
-        request = schemas.FormRequest(message=
+        request = schemas.FormRequest(message= {"message":
                                       f"""Follow these steps to manually register PKI keys with the system
                                       1. ssh into the host you are creating your system on, {kwargs['host']}
                                       2. navigate into the .ssh folder of the host. If there are not pre-generated keys, run ssh-keygen -t rsa -b 4096 -m PEM
                                       3. format both key files using cat $privateKeyFile | awk -v ORS='\\n' '1'. Both keys must be in single line format
                                       4. ensure the private key is not in openSSH format (that is it has the begin and end headers)
                                       5. download both to your local machine using scp
                                       6. run the verify_pki_keys command and submit the system id {kwargs['id']} and the file path of the public and private keys
-                                      7. you should be able to access the system now""",
+                                      7. you should be able to access the system now"""},
                                       request_content={"continue":Argument("continue", arg_type='confirmation')})
         await kwargs['connection'].send(request)
         await kwargs['connection'].receive()
         return None        
+    
+    async def authenticate(self, kwargs):
+        return await self.sys_auth_map[kwargs['systemType']][kwargs['defaultAuthnMethod']](**kwargs)
 
     async def run(self, *args, **kwargs) -> str: # create a tapius system. Takes a path to a json file with all system information, as well as an ID
-        system_creation_info = self.t.systems.createSystem(**kwargs)
+        return_info = dict()
+        return_info['system_creation_info'] = self.t.systems.createSystem(**kwargs)
         if kwargs['defaultAuthnMethod'] not in self.sys_auth_map[kwargs['systemType']]:
             raise ValueError(f"The system type {kwargs['systemType']} does not support {kwargs['defaultAuthnMethod']} authentication.")
         else:
-            auth_result = self.sys_auth_map[kwargs['systemType']]['defaultAuthnMethod'](**kwargs)
-        return system_creation_info
+            try:
+                return_info['auth_result'] = await self.sys_auth_map[kwargs['systemType']][kwargs['defaultAuthnMethod']](**kwargs)
+            except Exception as e:
+                return_info['auth_result'] = f"Authentication for the system {kwargs['id']} failed, maybe you entered something wrong? run the submit_system_credentials command"
+        return return_info
+    
+
+class submit_system_credentials(create_system):
+    """
+    @help: manually submit system credentials
+    """
+    supports_config_file = False
+    required_arguments = [
+        Argument('id', positional=True)
+    ]
+    optional_arguments = []
+    async def run(self, *args, **kwargs):
+        system_info = self.t.systems.getSystem(systemId=kwargs['id'])
+        kwargs['systemType'] = system_info.systemType
+        kwargs['defaultAuthnMethod'] = system_info.defaultAuthnMethod
+        return_info = await self.authenticate(kwargs)
+        return return_info
     
 
 class update_system(create_system):
     """
     @help: update a system with new information
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
+    required_arguments = [
+        Argument('systemId', size_limit=(1, 80), positional=True)
+    ]
     async def run(self, *args, **kwargs):
-        result = self.t.putSystem(**kwargs)
+        result = self.t.systems.putSystem(**kwargs)
         return result
     
 
-class is_enabled(baseCommand.BaseCommand):
+class is_system_enabled(baseCommand.BaseCommand):
     """
     @help: check to see if a system is enabled
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
-        Argument('systemId')
+        Argument('systemId', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.systems.isEnabled(**kwargs)
 
 
-class enable_system(is_enabled):
+class enable_system(is_system_enabled):
     """
     @help: enable a system
     """
     async def run(self, *args, **kwargs):
         return self.t.systems.enableSystem(**kwargs)
     
 
-class disable_system(is_enabled):
+class disable_system(is_system_enabled):
     """
     @help: disable a system
     """
     decorator=decorators.NeedsConfirmation()
     async def run(self, *args, **kwargs):
         return self.t.systems.disableSystem(**kwargs)
     
@@ -313,32 +349,99 @@
 class delete_system(baseCommand.BaseCommand):
     """
     @help: delete the selected system
     """
     decorator=decorators.NeedsConfirmation()
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments=[
-        Argument('systemId', size_limit=(1, 80)),
+        Argument('systemId', size_limit=(1, 80), positional=True),
     ]
     async def run(self, *args, **kwargs) -> str:
         kwargs['connection'].system = ''
         kwargs['connection'].pwd = ''
         return_value = self.t.systems.deleteSystem(systemId=kwargs['systemId'])
         return return_value
     
 
 class undelete_system(baseCommand.BaseCommand):
     """
     @help: undo deletion
     """
     required_arguments=[
-        Argument('systemId', size_limit=(1, 80)),
+        Argument('systemId', size_limit=(1, 80), positional=True),
     ]
     async def run(self, *args, **kwargs):
         return self.t.systems.undelete(**kwargs)
 
 class create_child_system(baseCommand.BaseCommand):
     """
     @help: create a child system which inherits majority attributes from parent
     """
+    required_arguments = [
+        Argument('parentId', positional=True),
+        Argument('rootDir')
+    ]
+    optional_arguments = [
+        Argument('effectiveUserId', default_value=r"${apiUserId}")
+    ]
     async def run(self, *args, **kwargs):
-        return "UNFINISHED FEATURE"
+        return self.t.systems.createChildSystem(**kwargs)
+    
+
+class unlink_child_system(baseCommand.BaseCommand):
+    """
+    @help: make a child system stand alone, so that updates to parent system will not transfer to this child system
+    """
+    required_arguments = [
+        Argument('parentId', positional=True)
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.systems.unlinkFromParent(**kwargs)
+    
+
+class unlink_children(baseCommand.BaseCommand):
+    """
+    @help: unlink an array of child systems from their parent system. Requires parent system permissions
+    """
+    required_arguments = [
+        Argument('parentId', positional=True),
+        Argument('childSystemIds', arg_type='input_list', data_type=Argument('systemId', size_limit=(1, 80)))
+    ]
+    async def run(self, *args, **kwargs):
+        parent_id = kwargs.pop('parentId')
+        kwargs['parentSystemId'] = parent_id
+        return self.t.systems.unlinkChildren(**kwargs)
+    
+
+class get_user_perms(baseCommand.BaseCommand):
+    """
+    @help: list perms for the user on a select system
+    """
+    required_arguments = [
+        Argument('systemId'),
+        Argument('userName')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.systems.getUserPerms(**kwargs)
+    
+
+class grant_user_perms(baseCommand.BaseCommand):
+    """
+    @help: assign a perm for a user on the select system
+    """
+    required_arguments = [
+        Argument('systemId'),
+        Argument('userName'),
+        Argument('permissions', arg_type='input_list', data_type=Argument('permission', choices=['READ', 'MODIFY', 'EXECUTE'], arg_type='str_input'))
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.grantUserPerms(**kwargs)
+    
+
+class revoke_user_perms(grant_user_perms):
+    """
+    @help: delete user permissions
+    """
+    async def run(self, *args, **kwargs):
+        return self.t.revokeUserPerms(**kwargs)
+    
+
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class create_volume(baseCommand.BaseCommand):
     """
     @help: create a new volume on which to store files to be used by Tapis pods. This allows several pods to share the same persistent files
     """
     supports_config_file=True
     required_arguments = [
-        Argument('volume_id')
+        Argument('volume_id', positional=True)
     ]
     optional_arguments = [
         Argument('description', arg_type='str_input'),
         Argument('size_limit', data_type='int', default_value=1024)
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.create_volume(**kwargs)
@@ -34,35 +34,49 @@
 
 class get_volume(baseCommand.BaseCommand):
     """
     @help: get information on a specific volume
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('volume_id')
+        Argument('volume_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.get_volume(**kwargs)
     
 
 class volume(baseCommand.BaseCommand):
     """
     @help: enter the volume to interact with its files more directly
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('volume_id')
+        Argument('volume_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         volume_info = self.t.pods.get_volume(volume_id=kwargs['volume_id'])
-        kwargs['connection'].system = volume_info
+        kwargs['connection'].system = volume_info.volume_id
         kwargs['connection'].pwd = "/"
         return f"successfully entered the volume {kwargs['connection'].system}"
     
 
+class exit_volume(baseCommand.BaseCommand):
+    """
+    @help: exit the volume you are currently in 
+    """
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id', positional=True)
+    ]
+    async def run(self, *args, **kwargs):
+        kwargs['connection'].system = ""
+        kwargs['connection'].pwd = ""
+        return f"successfully exited the volume {kwargs['volume_id']}"
+    
+
 class update_volume(create_volume):
     """
     @help: update a volume's information
     """
     supports_config_file=True
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     async def run(self, *args, **kwargs):
@@ -72,53 +86,53 @@
 class delete_volume(baseCommand.BaseCommand):
     """
     @help: delete a volume
     """
     decorator=decorators.NeedsConfirmation()
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('volume_id')
+        Argument('volume_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.delete_volume_files(**kwargs)
 
 
 class dir(baseCommand.BaseCommand):
     """
     @help: list all files in the selected volume
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('volume_id')
+        Argument('volume_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.list_volume_files(**kwargs)
     
 
 class upload_volume(baseCommand.BaseCommand):
     """
     @help: upload a file from your local machine to the volume
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id'), commandOpts.CHECK_PWD('path',)]
     required_arguments = [
-        Argument('volume_id'),
+        Argument('volume_id', positional=True),
         Argument('path'),
         Argument('file')
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.upload_to_volume(**kwargs)
     
 
 class set_volume_permission(baseCommand.BaseCommand):
     """
     @help: set the permission for a user on a volume
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('volume_id'),
+        Argument('volume_id', positional=True),
         Argument('username'),
         Argument('level')
     ]
     async def run(self, *args, **kwargs):
         user = kwargs.pop('username')
         kwargs['user'] = user
         return self.t.pods.set_volume_permission(**kwargs)
@@ -126,27 +140,27 @@
 
 class get_volume_permissions(baseCommand.BaseCommand):
     """
     @help: set the permission for a user on a volume
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('volume_id'),
+        Argument('volume_id', positional=True),
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.get_volume_permission(**kwargs)
     
 
 class delete_volume_permission(baseCommand.BaseCommand):
     """
     @help: delete the persmission for a user on a volume
     """
     decorator=decorators.NeedsConfirmation()
     required_arguments = [
-        Argument('volume_id'),
+        Argument('volume_id', positional=True),
         Argument('username'),
         Argument('level')
     ]
     async def run(self, *args, **kwargs):
         user = kwargs.pop('username')
         kwargs['user'] = user
         return self.t.pods.delete_volume_permission(**kwargs)
@@ -163,61 +177,73 @@
 class create_snapshot(baseCommand.BaseCommand):
     """
     @help: create a backup of the volume selected or specific files in the volume
     """
     supports_config_file=True
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('source_volume_id'), commandOpts.CHECK_PWD(('source_volume_path', 'destination_path'))]
     required_arguments = [
-        Argument('snapshot_id'),
-        Argument('source_volume_id'),
+        Argument('snapshot_id', positional=True),
+        Argument('source_volume_id', positional=True),
         Argument('source_volume_path')
     ]
     optional_arguments = [
         Argument('destination_path', description="Required if your snapshot is of a single file"),
         Argument('description', arg_type='str_input'),
         Argument('size_limit', data_type='int', description='maximum size in megabytes of the snapshot'),
         Argument('cron'),
         Argument('retention_policy')
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.create_snapshot(**kwargs)
     
 
 class get_snapshot(baseCommand.BaseCommand):
+    """
+    @help: get snapshot information
+    """
     required_arguments = [
-        Argument('snapshot_id')
+        Argument('snapshot_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.get_snapshot(**kwargs)
     
 
 class update_snapshot(baseCommand.BaseCommand):
+    """
+    @help: update snapshot information
+    """
     supports_config_file=True
     required_arguments = [
-        Argument('snapshot_id')
+        Argument('snapshot_id', positional=True)
     ]
     optional_arguments = [
         Argument('description', arg_type='str_input'),
         Argument('size_limit', data_type='int'),
         Argument('cron'),
         Argument('retention_policy')
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.update_snapshot(**kwargs)
     
 
 class delete_snapshot(baseCommand.BaseCommand):
+    """
+    @help: delete snapshot information
+    """
     decorator=decorators.NeedsConfirmation()
     required_arguments = [
-        Argument('snapshot_id')
+        Argument('snapshot_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.delete_snapshot(**kwargs)
     
 
 class list_snapshot_files(baseCommand.BaseCommand):
+    """
+    @help: list the files in a snapshot
+    """
     required_arguments = [
-        Argument('snapshot_id')
+        Argument('snapshot_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.list_snapshot_files(**kwargs)
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/server/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,40 @@
 import traceback
 
 
 from tapipy.tapis import Tapis
 from tapipy import tapis
 from federatedTenantAuthAPI.get import get_client_code
 import requests
+import pyperclip
 
 
 from socketopts import schemas
 from utilities import exceptions
 from commands.arguments import argument
 
 
 
 class ServerSideAuth:
     def create_token_device_grant(link, device_code, client_id):
         response = requests.post(f"https://{link}/v3/oauth2/tokens", json={"grant_type":"device_code", "device_code":device_code, "client_id":client_id})
         parsed_data = json.loads(response.content.decode())
         return parsed_data['result']['access_token']['access_token'], parsed_data['result']['refresh_token']['refresh_token']
     
+    def get_tenant_uris(self):
+        if not self.t:
+            t = Tapis('https://tacc.tapis.io')
+        else:
+            t = self.t
+        tenants = t.tenants.list_tenants()
+        uri_list = list()
+        for tenant in tenants:
+            uri_list.append(tenant.base_url.split("//")[1])
+        return uri_list
+    
     async def password_grant(self, link: str, connection):
         start = time.time()
         username_password_request = schemas.AuthRequest(auth_request_type='password',
                                                         request_content={"username":argument.Argument('username', size_limit=(1, 100), arg_type='str_input'), "password":argument.Argument('password', arg_type='secure')},
                                                         message={"message":"enter your TACC username and password"})
         for attempt in range(1, 4):
             await connection.send(username_password_request)
@@ -67,39 +79,41 @@
     
     async def device_code_grant(self, link: str, connection):
         start = time.time()
         self.t = Tapis(f"https://{link}", resource_set='dev')
         client_id = get_client_code(link)
         if not client_id:
             raise exceptions.NoTenantClient(link)
-        print(client_id)
         authentication_information = self.t.authenticator.generate_device_code(client_id=client_id)
         payload = schemas.AuthRequest(auth_request_type='device_code',
-                                      message={"message":"Go to the URL if it doesnt open automatically and enter the user code to authenticate. Then click y when you enter the code", 
+                                      message={"message":"Go to the URL if it doesnt open automatically and enter the user code to authenticate. Then click y when you enter the code\nUser code copied to clipboard", 
                                                "url":authentication_information.verification_uri, 
                                                "user_code": authentication_information.user_code},
-                                      request_content={'entered_confirm':argument.Argument('entered_confirm', arg_type='confirmation')})
+                                      request_content={'Entered User Code':argument.Argument('Entered User Code', arg_type='confirmation')})
         await connection.send(payload)
+        pyperclip.copy(authentication_information.user_code)
         webbrowser.open(authentication_information.verification_uri)
         confirmation = await connection.receive()
-        if not confirmation.request_content['entered_confirm']:
+        if not confirmation.request_content['Entered User Code']:
             raise RuntimeError(f"User indicated that device code auth failed") # get rid of this feature and switch to polling
         start_time = time.time()
         while True:
             try:
                 access_info = self.t.authenticator.create_token(grant_type="device_code", device_code=authentication_information.device_code, client_id=client_id)
                 break
-            except:
+            except Exception as e:
+                print(e)
                 time.sleep(1)
-                if time.time() - start_time > 500:
-                    raise Exception("Timeout while polling for authenticator token")
+                if time.time() - start_time > 60:
+                    raise RuntimeError("Timeout while polling for authenticator token")
 
         self.t = Tapis(f"https://{link}",
                        access_token=access_info.access_token.access_token,
-                       refresh_token=access_info.refresh_token.refresh_token)
+                       refresh_token=access_info.refresh_token.refresh_token,
+                       resource_set="dev")
         
         self.username = self.t.authenticator.get_userinfo().username
         self.url = link
         self.access_token = self.t.access_token
 
         self.logger.info(f"initiated in {time.time()-start}")
 
@@ -110,46 +124,46 @@
         auth_link = rf"https://{link}/v3/oauth2/webapp"
         payload = schemas.AuthRequest(auth_request_type='federated',
                                       message={
                                           "message":"Go to the URL if it doesnt open and enter your account information. Then enter the user code to this application",
                                           "url":auth_link
                                             }, 
                                       request_content={
-                                          "user_code":argument.Argument('user_code', arg_type='str_input')
+                                          "access_token":argument.Argument('access_token', arg_type='str_input')
                                           })
         await connection.send(payload)
         webbrowser.open(auth_link)
         response_code_message: schemas.AuthRequest = await connection.receive()
         
         self.t = Tapis(f"https://{link}",
-                       access_token=response_code_message.request_content['user_code'].strip())
+                       access_token=response_code_message.request_content['access_token'].strip())
 
         self.username = self.t.authenticator.get_userinfo().username
         self.url = link
         self.access_token = self.t.access_token
 
         self.logger.info(f"initiated in {time.time()-start}")
 
         return f"Successfully initialized tapis service on {self.url}"
 
     async def auth_startup(self, connection):
-        session_auth_type_request = schemas.AuthRequest(request_content={"uri":argument.Argument('uri', arg_type='str_input'), "auth_type":argument.Argument('auth_type', choices=['password', 'device_code', 'federated'], arg_type='str_input')},
+        session_auth_type_request = schemas.AuthRequest(request_content={"Tenant URI":argument.Argument('Tenant URI', arg_type='str_input', choices=self.get_tenant_uris()), "auth_type":argument.Argument('auth_type', choices=['password', 'device_code', 'federated'], arg_type='str_input')},
                                                         auth_request_type="requested",
                                                         message={"message":"Enter the URI of the Tapis tenant you wish to connect to, then select your auth type from the options below",
                                                                  "grant options":['password', 'device_code', 'federated']})
         while True:
             try:
                 await connection.send(session_auth_type_request)
                 session_auth_type_response: schemas.FormResponse = await connection.receive()
                 auth_type = session_auth_type_response.request_content['auth_type']
                 if auth_type not in ('password', 'device_code', 'federated'):
                     raise exceptions.InvalidCredentialsReceived()
                 self.auth_type = auth_type
-                link = session_auth_type_response.request_content['uri']
-                self.t = Tapis(f"https://{link}", resource_set='dev')
+                link = session_auth_type_response.request_content['Tenant URI']
+                self.t = Tapis(f"https://{link}")#, resource_set='dev')
                 break
             except exceptions.InvalidCredentialsReceived:
                 session_auth_type_request.error = "Invalid auth type received"
             except tapis.errors.BaseTapyException:
                 session_auth_type_request.error = "Invalid tenant URI received, try again"
 
         if auth_type != "password":
@@ -165,26 +179,29 @@
                 session_password_request.error = "The password provided was too short, the password must be at least 6 characters!!!"
         
         while True:
             try:
                 if auth_type == "federated":
                     await self.federated_grant(link, connection)
                 elif auth_type == "device_code":
+                    connection.set_status_device_authenticating()
                     await self.device_code_grant(link, connection)
+                    connection.set_status_closed()
                 else:
                     await self.password_grant(link, connection)
                 break
-            except (exceptions.ClientSideError, exceptions.InvalidCredentialsReceived, exceptions.NoTenantClient) as e:
+            except (exceptions.ClientSideError, exceptions.InvalidCredentialsReceived, exceptions.NoTenantClient, RuntimeError) as e:
                 raise e
             except Exception as e:
                 error_str = traceback.format_exc()
                 print(error_str)
                 continue
         success_message = schemas.AuthRequest(auth_request_type="success", message={
             "message":f"Successfully authenticated with {auth_type} authentication",
             "username":self.username,
             "url":link})
         self.configure_decorators(self.username, self.password)
         self.update_credentials(self.t, self.username, self.password)
+        self.available_services = self.service_checker.check_services(self.t)
         await connection.send(success_message)
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/server/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,142 @@
-import sys
 import time
 import socket
-import os
 import asyncio
 import traceback
 
 from tapipy.tapis import Tapis
 
 if __name__ != "__main__":
     from commands import commandMap, decorators
     from utilities import logger, exceptions
     from socketopts import schemas, socketOpts
     from server import auth
 else:
     import commands.commandMap as commandMap
 
 
+class ServiceChecker:
+    def __init__(self, available_services: list):
+        self.available_services = available_services
+
+    def check_services(self, t):
+        tenant = t.tenants.get_tenant(tenant_id=t.tenant_id)
+        site_id = tenant.site_id
+        supported_services = t.tenants.get_site(site_id=site_id).services
+        filtered_supported_services = [service for service in supported_services if service in self.available_services]
+        return filtered_supported_services
+
+
 class ServerConnection(socketOpts.ServerSocketOpts):
     """
     connection object to wrap around async reader and writer to make work easier
     """
-    def __init__(self, name, reader, writer, debug=False):
+    def __init__(self, name, reader, writer, connection_list, debug=False):
         super().__init__(name, debug=debug)
         self.name = name
-        self.reader = reader
-        self.writer = writer
+        self.connection_list: list = connection_list
+        self.reader: asyncio.StreamReader = reader
+        self.writer: asyncio.StreamWriter = writer
+        self.task: asyncio.Task = None
+        self.status = "CLOSED"
+        self.shutdown_message = schemas.ResponseData(message={'message':'Shutdown initiated, closing'}, exit_status=1)
+
+    def set_status_device_authenticating(self):
+        self.status = 'DEVICE_CODE_AUTH'
+
+    def set_status_closed(self):
+        self.status = 'CLOSED'
+
+    def set_task(self, task: asyncio.Task):
+        self.task = task
+        self.status == 'OPEN'
 
     async def close(self):
-        self.writer.close()
-        await self.writer.wait_closed()
-        
-
-class TaskCallback:
-    def __init__(self, logger, task: asyncio.Task, task_list: list):
-        self.task_list = task_list
-        self.logger, self.task = logger, task
-
-    def __call__(self, result):
-        self.task_list.remove(self.task)
-        print(result)
-        result = self.task.result()
-        self.logger.info(result)
+        self.logger.info('ATTEMPTING TO CLOSE')
+        if self.status == 'OPEN':
+            self.task.cancel()
+            self.logger.info(self.task.result())
+            await self.send(self.shutdown_message)
+            self.writer.close()
+            await self.writer.wait_closed()
+            self.status = 'CLOSED'
+            self.connection_list.remove(self)
+        elif self.status == 'DEVICE_CODE_AUTH':
+            await self.send(schemas.AuthRequest(error='cancelled authentication during device_code grant', auth_request_type='device_code'))
+            self.writer.close()
+            await self.writer.wait_closed()
+        else:
+            self.writer.close()
+            await self.writer.wait_closed()
+        self.logger.info('SUCCESSFULLY CLOSED')
 
 
 class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup, auth.ServerSideAuth):
     """
     Receives commands from the client and executes Tapis operations
     """
-    SESSION_TIME = 1200
+    SESSION_TIME = 5000
     debug=False
     def __init__(self, IP: str, PORT: int):
         super().__init__()
         self.initial = True
+        self.running = True
 
         self.t = None
         self.url = None
         self.access_token = None
         self.username = None
         self.password = None
         self.auth_type = None
 
+        self.service_checker = ServiceChecker(available_services=list(self.groups.keys()))
+        self.available_services = []
+
         self.__name__ = "Server"
         self.initialize_logger(self.__name__)
         # setting up socket server
         self.ip, self.port = IP, PORT
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.sock.setblocking(False)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.bind((self.ip, self.port))
         self.sock.listen(1)
+
         self.end_time = time.time() + self.SESSION_TIME # start the countdown on the timeout
 
-        self.task_list: list[asyncio.Task] = []
+        self.connections_list: list[ServerConnection] = []
 
         self.server = None
         self.num_connections = 0
 
         self.logger.info('initialization complete')
 
-    def cancel_tasks(self):
-        for task in self.task_list:
-            task.cancel()
+    async def close_connections(self):
+        for connection in self.connections_list:
+            await connection.close()
+
+    async def close(self):
+        await self.close_connections()
+        self.server.close()
+        raise exceptions.Shutdown()
+
+    async def check_timeout(self):
+        while self.running:
+            if time.time() >= self.end_time:
+                self.logger.info("Timeout, shutting down")
+                self.running = False
+                return 'server timed out'
+            await asyncio.sleep(3)
+    
+    async def check_shutdown(self):
+        while self.running:
+            await asyncio.sleep(3)
+        await self.close()
+        self.logger.info("The server shutdown.")
+        return None
 
     async def handshake(self, connection):
         self.logger.info("Handshake starting")
         if self.initial:  # if this is the first time in the session that the cli is connecting
             startup_data = schemas.StartupData(initial = self.initial)
             await connection.send(startup_data)
             await self.auth_startup(connection)
@@ -95,19 +147,17 @@
         self.logger.info("Final connection data sent")
 
     async def accept(self, reader, writer):
         """
         accept connection request and initialize communication with the client
         """  
         self.num_connections += 1
-        connection = ServerConnection(f"CON-{self.num_connections}", reader=reader, writer=writer, debug=self.debug)
-        self.timeout_handler()
-        ip, port= writer.transport.get_extra_info('socket').getsockname()
-        if ip != socket.gethostbyname(socket.gethostname()):
-            raise exceptions.UnauthorizedAccessError(ip)
+        self.end_time = time.time() + self.SESSION_TIME
+        connection = ServerConnection(f"CON-{self.num_connections}", reader=reader, writer=writer, connection_list=self.connections_list, debug=self.debug)
+        ip, port = writer.transport.get_extra_info('socket').getsockname()
         self.logger.info("Received connection request")
         try:
             await self.handshake(connection)
         except exceptions.InvalidCredentialsReceived as e:
             self.logger.warning("invalid credentials entered too many times. Cancelling request")
             await connection.close()
             return
@@ -125,75 +175,69 @@
         setup_response: schemas.ResponseData = await connection.receive()
         if not setup_response.request_content['setup_success']:
             self.logger.warning(f"The setup of the connection {connection.name} failed")
             return
 
         loop = asyncio.get_event_loop()
         task: asyncio.Task = loop.create_task(self.receive_and_execute(connection))
-        callback = TaskCallback(self.logger, task, self.task_list)
-        task.add_done_callback(callback)
-        self.task_list.append(task)
-
-    def timeout_handler(self):  
-        """
-        checks if the timeout has been exceeded
-        """
-        if time.time() > self.end_time: 
-            raise exceptions.TimeoutError
+        connection.set_task(task)
+        self.connections_list.append(connection)
 
-    async def receive_and_execute(self, connection):
+    async def receive_and_execute(self, connection: ServerConnection):
         """
         receive and process commands
         """
-        while True:
+        self.logger.info(f"{connection.name} is now running")
+        while self.running:
             try:
                 message = await connection.receive()
-                self.timeout_handler()  
+                if not self.running:
+                    raise exceptions.Shutdown
                 kwargs = message.request_content
                 result = await self.run_command(connection, kwargs)
                 response = schemas.ResponseData(message={"message":result}, url=self.url, active_username=self.username)
                 self.end_time = time.time() + self.SESSION_TIME 
                 await connection.send(response)
                 self.logger.info(message.schema_type)
             except exceptions.ClientSideError as e:
                 self.logger.warning(e)
                 continue
             except (exceptions.TimeoutError, exceptions.Shutdown) as e:
                 error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 self.logger.warning(str(e))
-                self.cancel_tasks()
-                self.server.close()
-                loop = asyncio.get_event_loop()
-                loop.stop()
-                loop.close()
-                sys.exit(0)
+                self.running = False
+                return 'shutdown initiated, closing'
             except exceptions.Exit as e:
                 self.logger.info("user exit initiated")
                 error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 await connection.close()
                 return
-                #self.accept()  # wait for CLI to reconnect
             except OSError:
                 self.logger.info("connection was lost, waiting to reconnect")
                 await connection.close()
+            except asyncio.CancelledError:
+                return 'task was cancelled'
             except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived, Exception) as e:
                 error_str = traceback.format_exc()
                 error_response = schemas.ResponseData(error=str(e), url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 self.logger.warning(f"{error_str}")
     
     async def main(self):
         self.server = await asyncio.start_server(self.accept, sock=self.sock)
         try:
             async with self.server:
-                await self.server.serve_forever()
-        except KeyboardInterrupt:
-            self.server.close()
-            self.cancel_tasks()
-            sys.exit(0)
+                result = await asyncio.gather(self.server.serve_forever(), self.check_timeout(), self.check_shutdown(), return_exceptions=True)#, self.check_timeout(), return_exceptions=True)
+                self.logger.info(str(result))
+        except (KeyboardInterrupt, exceptions.Shutdown):
+            self.running = False
 
 
 if __name__ == '__main__':
-    server = Server(socket.gethostbyname(socket.gethostname()), 30000)
-    asyncio.run(server.main())
+    loop = asyncio.get_event_loop()
+    server = Server(socket.gethostbyname('127.0.0.1', 30000)) 
+    try:
+        asyncio.run(server.main())
+    finally:
+        loop.close()
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import typing
+from pprint import pformat
 
 import pydantic
 
 
 try:
     from socketopts import schemas
     from utilities import logger, exceptions
@@ -31,17 +32,17 @@
         self.initialize_logger(f"{name} LOGGER")
         self.debug_state = debug
 
     def debug(self, operation: typing.Literal["SENDING", "RECEIVED", "WAITING"], message: str | typing.Type[schemas.BaseSchema]):
         if self.debug_state:
             if not isinstance(message, str):
                 self.logger.info(f"""{operation}: {message.schema_type}
-                                    MESSAGE CONTENT:{message.request_content}
-                                    MESSAGE: {message.message}
-                                    ERROR: {message.error}""")
+                                    MESSAGE CONTENT:{pformat(message.request_content)}
+                                    MESSAGE: {pformat(message.message)}
+                                    ERROR: {pformat(message.error)}""")
             else:
                 self.logger.info(message)
 
 
 class ClientSocketOpts(BaseSocketOpts):
     """
     synchronous sockets to be used by clients
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.2.0/src/TapisCLICICLE/utilities/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,8 +35,22 @@
         self.logger.setLevel(logging.INFO)
         stream_handler = logging.StreamHandler(stream=sys.stdout)
         stream_handler.setLevel(logging.INFO)
         stream_format = logging.Formatter(
             '%(name)s - %(levelname)s - %(message)s')
         stream_handler.setFormatter(stream_format)
         self.logger.addHandler(stream_handler)
+        self.logger.disabled = False
+
+
+class ServiceLogger:
+    def __init__(self, name, log_path):
+        self.logger = logging.getLogger(name)
+        self.logger.setLevel(logging.INFO)
+        file_handler = file_handler = logging.FileHandler(
+            log_path, mode='a')
+        file_handler.setLevel(logging.INFO)
+        file_format = logging.Formatter(
+            '%(name)s - %(levelname)s - %(message)s')
+        file_handler.setFormatter(file_format)
+        self.logger.addHandler(file_handler)
         self.logger.disabled = False
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.4
+Version: 0.2.0
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -704,26 +704,23 @@
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 #### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
-2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
-3. enter your username and password when prompted
+2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be icicle.tapis.io
+3. the application will then prompt you to choose your authentication method, password, federated, or device code. Which ones are avaiable depends on the tenant in question. If you choose either the 2nd or 3rd option, you will be asked to create a session password to authenticate secure operations.
 4. if all went well the console should open. You can run `help` to see command options
-5. to exit the application, run `exit`
+5. to exit the application, run `exit`. To shut it down, run `shutdown`. The server automatically shuts down after 25 minutes of inactivity
 
 #### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
-`python -m TapisCLICICLE pods -c help`
+`python -m TapisCLICICLE help -v`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
-**Scripting**
-
-Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
-
 ### Known Issues
 Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
+The application has known compatibility issues with the WSL vpn due to its reliance on sockets. If you intend to use the application with WSL turn off your VPN. If the application doesnt work and you have a VPN on, turn it off just to make sure.
```

### Comparing `TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.2.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 src/TapisCLICICLE/commands/appCommands.py
 src/TapisCLICICLE/commands/baseCommand.py
 src/TapisCLICICLE/commands/commandMap.py
 src/TapisCLICICLE/commands/commandOpts.py
 src/TapisCLICICLE/commands/dataFormatters.py
 src/TapisCLICICLE/commands/decorators.py
 src/TapisCLICICLE/commands/fileCommands.py
+src/TapisCLICICLE/commands/jobCommands.py
 src/TapisCLICICLE/commands/podCommands.py
 src/TapisCLICICLE/commands/serverCommands.py
 src/TapisCLICICLE/commands/systemCommands.py
 src/TapisCLICICLE/commands/volumeCommands.py
 src/TapisCLICICLE/commands/arguments/__init__.py
 src/TapisCLICICLE/commands/arguments/argument.py
 src/TapisCLICICLE/commands/query/__init__.py
 src/TapisCLICICLE/commands/query/neo4j.py
 src/TapisCLICICLE/commands/query/postgres.py
 src/TapisCLICICLE/server/__init__.py
 src/TapisCLICICLE/server/auth.py
 src/TapisCLICICLE/server/server.py
-src/TapisCLICICLE/server/serviceCheck.py
+src/TapisCLICICLE/server/userFileManager.py
 src/TapisCLICICLE/socketopts/__init__.py
 src/TapisCLICICLE/socketopts/schemas.py
 src/TapisCLICICLE/socketopts/socketOpts.py
 src/TapisCLICICLE/utilities/__init__.py
 src/TapisCLICICLE/utilities/exceptions.py
 src/TapisCLICICLE/utilities/killableThread.py
 src/TapisCLICICLE/utilities/logger.py
```

