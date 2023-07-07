# Comparing `tmp/gen3_util-0.0.2rc7.tar.gz` & `tmp/gen3_util-0.0.2rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.2rc7.tar", last modified: Thu Jul  6 19:58:29 2023, max compression
+gzip compressed data, was "gen3_util-0.0.2rc8.tar", last modified: Fri Jul  7 00:12:28 2023, max compression
```

## Comparing `gen3_util-0.0.2rc7.tar` & `gen3_util-0.0.2rc8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.394527 gen3_util-0.0.2rc7/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc7/LICENSE
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8535 2023-07-06 19:58:29.394237 gen3_util-0.0.2rc7/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     7850 2023-07-06 01:19:54.000000 gen3_util-0.0.2rc7/README.md
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.355831 gen3_util-0.0.2rc7/gen3_util/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       71 2023-07-05 18:55:42.000000 gen3_util-0.0.2rc7/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.372647 gen3_util-0.0.2rc7/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2321 2023-06-30 14:28:04.000000 gen3_util-0.0.2rc7/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3973 2023-07-06 19:12:10.000000 gen3_util-0.0.2rc7/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.374182 gen3_util-0.0.2rc7/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-06-30 18:19:19.000000 gen3_util-0.0.2rc7/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5679 2023-07-01 13:38:21.000000 gen3_util-0.0.2rc7/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.375849 gen3_util-0.0.2rc7/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      629 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc7/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.376788 gen3_util-0.0.2rc7/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4637 2023-06-30 14:47:36.000000 gen3_util-0.0.2rc7/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc7/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.377156 gen3_util-0.0.2rc7/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5428 2023-07-06 00:58:23.000000 gen3_util-0.0.2rc7/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.378443 gen3_util-0.0.2rc7/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2824 2023-06-29 20:12:33.000000 gen3_util-0.0.2rc7/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      433 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.383083 gen3_util-0.0.2rc7/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      938 2023-06-28 20:40:29.000000 gen3_util-0.0.2rc7/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    12907 2023-06-29 18:03:19.000000 gen3_util-0.0.2rc7/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.386524 gen3_util-0.0.2rc7/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4117 2023-07-05 18:55:47.000000 gen3_util-0.0.2rc7/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2256 2023-07-01 13:41:32.000000 gen3_util-0.0.2rc7/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      323 2023-06-29 20:10:18.000000 gen3_util-0.0.2rc7/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    10062 2023-07-06 01:11:29.000000 gen3_util-0.0.2rc7/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      329 2023-06-29 19:48:08.000000 gen3_util-0.0.2rc7/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3858 2023-06-29 20:12:21.000000 gen3_util-0.0.2rc7/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.388146 gen3_util-0.0.2rc7/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2769 2023-07-01 13:37:39.000000 gen3_util-0.0.2rc7/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.2rc7/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      793 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.370593 gen3_util-0.0.2rc7/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8535 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1687 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       53 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      128 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       16 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2023-07-06 19:58:29.394590 gen3_util-0.0.2rc7/setup.cfg
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5580 2023-07-06 19:56:56.000000 gen3_util-0.0.2rc7/setup.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.350122 gen3_util-0.0.2rc7/tests/
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.390632 gen3_util-0.0.2rc7/tests/integration/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      270 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3931 2023-07-06 19:09:19.000000 gen3_util-0.0.2rc7/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      454 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      243 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2089 2023-06-29 20:23:35.000000 gen3_util-0.0.2rc7/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2443 2023-06-29 20:10:37.000000 gen3_util-0.0.2rc7/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1237 2023-06-29 19:02:47.000000 gen3_util-0.0.2rc7/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.393202 gen3_util-0.0.2rc7/tests/unit/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.393569 gen3_util-0.0.2rc7/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 00:58:23.000000 gen3_util-0.0.2rc7/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.393782 gen3_util-0.0.2rc7/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1450 2023-07-06 01:18:25.000000 gen3_util-0.0.2rc7/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3380 2023-06-29 20:22:33.000000 gen3_util-0.0.2rc7/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2699 2023-07-06 01:20:50.000000 gen3_util-0.0.2rc7/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.526396 gen3_util-0.0.2rc8/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc8/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8535 2023-07-07 00:12:28.526097 gen3_util-0.0.2rc8/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7850 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.491322 gen3_util-0.0.2rc8/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-07-05 18:55:42.000000 gen3_util-0.0.2rc8/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.504439 gen3_util-0.0.2rc8/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4281 2023-07-07 00:08:11.000000 gen3_util-0.0.2rc8/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.504777 gen3_util-0.0.2rc8/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5679 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.513570 gen3_util-0.0.2rc8/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc8/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.514270 gen3_util-0.0.2rc8/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc8/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.514706 gen3_util-0.0.2rc8/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5262 2023-07-07 00:02:54.000000 gen3_util-0.0.2rc8/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.516560 gen3_util-0.0.2rc8/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.518264 gen3_util-0.0.2rc8/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      938 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12907 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.520153 gen3_util-0.0.2rc8/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      323 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    10101 2023-07-07 00:02:54.000000 gen3_util-0.0.2rc8/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3293 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.521392 gen3_util-0.0.2rc8/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.2rc8/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.499854 gen3_util-0.0.2rc8/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8535 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1687 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-07 00:12:28.526458 gen3_util-0.0.2rc8/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-07-07 00:12:04.000000 gen3_util-0.0.2rc8/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.489219 gen3_util-0.0.2rc8/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.523177 gen3_util-0.0.2rc8/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      270 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4358 2023-07-07 00:10:58.000000 gen3_util-0.0.2rc8/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      454 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      243 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2443 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.525204 gen3_util-0.0.2rc8/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.525549 gen3_util-0.0.2rc8/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.525751 gen3_util-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2699 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.2rc7/LICENSE` & `gen3_util-0.0.2rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/PKG-INFO` & `gen3_util-0.0.2rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.2rc7
+Version: 0.0.2rc8
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.2rc7/README.md` & `gen3_util-0.0.2rc8/README.md`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/access/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/access/cli.py` & `gen3_util-0.0.2rc8/gen3_util/access/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,38 +14,43 @@
 def access_group(config: Config):
     """Manage access requests."""
     pass
 
 
 @access_group.command(name="touch")
 @click.argument('user_name')
-@click.argument('project_id')
+@click.option('--project_id', show_default=True, default=None, help='add a project id ex: --project_id aced-Alcoholism')
+@click.option('--resource_path',  show_default=True, default=None, help='add resource paths ex: --resource_path /programs/aced/projects/Alcoholism')
 @click.option('--roles', show_default=True, default=None, help='Add comma-delimited role permissions to the access request, ex: --roles "storage_writer,file_uploader"')
 @click.pass_obj
-def access_touch(config: Config,  user_name: str, project_id: str, roles: str):
+def access_touch(config: Config,  user_name: str, project_id: str, resource_path: str, roles: str):
     """Create a request for read access.
 
     \b
     USER_NAME (str): user's email
     PROJECT_ID or RESOURCE_PATH: <program-name>-<project-name> or /resource/path
 
     """
     msgs = validate_email(user_name)
     assert msgs == [], f"Invalid email address: {user_name} {msgs}"
 
     msgs = validate_project_id(project_id)
     # assert msgs == [], f"Invalid project id: {project_id} {msgs}"
-    resource_path = None
+
     if len(msgs) == 0:
-        resource_path = project_id
-        project_id = None
+        resource_path = to_resource_path(project_id)
+    else:
+        resource_path = project_id  # assume resource path passed
 
-    assert resource_path, "required"
     assert user_name, "required"
-    resource_path = to_resource_path(project_id, resource_path)
+
+    assert (project_id or resource_path), "required"
+
+    resource_path = to_resource_path(project_id)
+
     request = {"username": user_name, "resource_path": resource_path}
     if roles is not None:
         roles = list(map(str, roles.split(',')))
         request.update({"role_ids": roles})
 
     with CLIOutput(config=config) as output:
         output.update(create_request(config=config, request=request))
```

### Comparing `gen3_util-0.0.2rc7/gen3_util/access/requestor.py` & `gen3_util-0.0.2rc8/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/buckets/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/buckets/cli.py` & `gen3_util-0.0.2rc8/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/cli/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/cli/cli.py` & `gen3_util-0.0.2rc8/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/common/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/common/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,17 +167,12 @@
         from email_validator import validate_email as email_validator_validate, EmailNotValidError
         email_validator_validate(email)
     except EmailNotValidError as e:
         msgs.append(f"{email} is not a valid email address. {e}")
     return msgs
 
 
-def to_resource_path(project_id, resource_path):
+def to_resource_path(project_id):
     """Canonical conversion of project_id to resource path."""
 
-    assert not (resource_path and project_id), "Please choose either project_id or resource_path"
-
-    if resource_path:
-        return resource_path
-
     _ = project_id.split('-')
     return f"/programs/{_[0]}/projects/{_[1]}"
```

### Comparing `gen3_util-0.0.2rc7/gen3_util/config/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/files/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/files/cli.py` & `gen3_util-0.0.2rc8/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/files/downloader.py` & `gen3_util-0.0.2rc8/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/files/uploader.py` & `gen3_util-0.0.2rc8/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/meta/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/meta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 def _has_entries(_: ParseResult):
     """FHIR types Bundles List have entries"""
     if _.resource is None:
         return False
     return _.resource.resource_type in ["Bundle", "List"] and _.resource.entry is not None
 
 
-def directory_reader(directory_path: [str, pathlib.Path],
+def directory_reader(directory_path: str,
                      recurse: bool = True,
                      validate: bool = False) -> Iterator[ParseResult]:
 
     """Extract FHIR resources from directory
 
     Read any type of json file, return itemized resources by iterating through Bundles and Lists
     """
```

### Comparing `gen3_util-0.0.2rc7/gen3_util/meta/cli.py` & `gen3_util-0.0.2rc8/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/meta/importer.py` & `gen3_util-0.0.2rc8/gen3_util/meta/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 def _extract_fhir_resources(file, input_path, plugin_path) -> list[Resource]:
     """Parse other resources from file."""
     plugins = _discover_plugins(plugin_path=plugin_path)
 
     if plugin_path:
-        assert len(plugins) > 0, f"No plugins found in {plugin_path}."
+        assert len(plugins) > 0, f"No plugins found in {plugin_path}"
     assert input_path, "No input path provided."
 
     resources = []
 
     for plugin in plugins:
         patient_identifier = plugin.extract_patient_identifier(path=str(file))
         specimen_identifier = plugin.extract_specimen_identifier(path=str(file))
@@ -140,15 +140,15 @@
                 continue
             stat = file.stat()
             modified = datetime.fromtimestamp(stat.st_mtime, tz=timezone.utc)
             mime, encoding = mimetypes.guess_type(file)
             if not mime:
                 mime = _magic.from_file(file)
 
-            resources = _extract_fhir_resources(file, input_path, plugin_path)
+            resources = _extract_fhir_resources(str(file).replace(remove_path_prefix, '', 1), input_path, plugin_path)
             subject_reference = f"ResearchStudy/{research_study['id']}"  # Who/what is the subject of the document
 
             for resource in resources:
 
                 if resource.resource_type == 'Patient':
                     subject_reference = f"Patient/{resource.id}"
```

### Comparing `gen3_util-0.0.2rc7/gen3_util/meta/uploader.py` & `gen3_util-0.0.2rc8/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/meta/validator.py` & `gen3_util-0.0.2rc8/gen3_util/meta/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,18 @@
     return orig_reference_dict(self, *args, **kwargs)
 
 
 def validate(config: Config, directory_path: pathlib.Path) -> ValidateDirectoryResult:
     """Check FHIR data, accumulate results."""
     exceptions = []
     resources = defaultdict(int)
+    print("DIRECTORY PATH: ", directory_path)
     for parse_result in directory_reader(directory_path):
-        # print('parse_result', parse_result)
+        print('parse_result', parse_result)
+
         if parse_result.exception:
             exceptions.append(parse_result)
         else:
             resources[parse_result.resource.resource_type] += 1
     return ValidateDirectoryResult(resources={'summary': dict(resources)}, exceptions=exceptions)
```

### Comparing `gen3_util-0.0.2rc7/gen3_util/projects/__init__.py` & `gen3_util-0.0.2rc8/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/projects/cli.py` & `gen3_util-0.0.2rc8/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/projects/creator.py` & `gen3_util-0.0.2rc8/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/projects/lister.py` & `gen3_util-0.0.2rc8/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util/projects/remover.py` & `gen3_util-0.0.2rc8/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.2rc8/gen3_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-util
-Version: 0.0.2rc7
+Version: 0.0.2rc8
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.2rc7/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.2rc8/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/setup.py` & `gen3_util-0.0.2rc8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2-rc7',  # Required
+    version='0.0.2-rc8',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.2rc7/tests/integration/test_access.py` & `gen3_util-0.0.2rc8/tests/unit/test_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,100 @@
-import json
-
 from click.testing import CliRunner
 from gen3_util.cli.cli import cli
 
 
-def test_access_ls(caplog):
-    """Ensure we can ls access."""
+def test_default_command(caplog):
+    """Ensure it prints version if no other command"""
     runner = CliRunner()
-    result = runner.invoke(cli, ['access', 'ls'])
+    result = runner.invoke(cli)
     assert result.exit_code == 0
-    expected_strings = ['OK']
-    for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
+    expected = ['Version']
+    for _ in expected:
+        assert _ in result.output, f"Should have printed expected={_} actual={result.output}"
 
 
-def test_access_touch_read_only():
-    """Ensure we can add a user with default read-only access."""
+def test_any_command(caplog):
+    """Ensure it does not print version if command provided"""
     runner = CliRunner()
-    result = runner.invoke(cli, 'access touch bar@foo.com aced-Alcoholism'.split())
-    print(result.output)
+    result = runner.invoke(cli, ['config'])
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
-    for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
+    un_expected_strings = ['Version']
+    for expected_string in un_expected_strings:
+        assert expected_string not in result.output, "only print version if nothing else to do"
 
 
-def test_access_touch_roles():
-    """Ensure we can add a user with specific roles."""
+def test_help(caplog):
+    """Ensure it prints command groups"""
     runner = CliRunner()
-    result = runner.invoke(cli, 'access touch bar@foo.com aced-Alcoholism --roles storage_writer,file_uploader'.split())
+    result = runner.invoke(cli, ['--help'])
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
+    print(result.output)
+    expected_strings = """
+        projects  Manage Gen3 projects.
+        buckets   Manage Gen3 buckets.
+        meta      Manage meta data.
+        files     Manage file transfers.
+        access    Manage access requests.
+        config    Configure this utility.
+        """.split()
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
+        assert expected_string in result.output, f"Should have printed {expected_string}"
 
 
-def test_access_touch_bad_email():
-    """Ensure we catch invalid email."""
+def test_projects(caplog):
+    """Ensure it prints project"""
     runner = CliRunner()
-    result = runner.invoke(cli, 'access touch barfoo.com aced-Alcoholism --roles storage_writer,file_uploader'.split())
-    assert result.exit_code != 0
-
-
-def test_access_touch_bad_project_id():
-    """Ensure we catch invalid email."""
-    runner = CliRunner()
-    result = runner.invoke(cli, 'access touch bar@foo.com aced-Alcoholism-XXX --roles storage_writer,file_uploader'.split())
-    assert result.exit_code != 0
+    result = runner.invoke(cli, ['projects', '--help'])
+    assert result.exit_code == 0
+    print(result.output)
+    expected_strings = """
+      ls     List all projects.
+      touch  Create a project
+      rm     Remove project.
+    """.split()
+    for expected_string in expected_strings:
+        assert expected_string in result.output, f"Should have printed {expected_string}"
 
 
-def test_access_workflow():
+def test_meta(caplog):
+    """Ensure it prints meta"""
     runner = CliRunner()
-    result = runner.invoke(cli, '--format json access touch bar@foo.com aced-MCF10A'.split())
+    result = runner.invoke(cli, ['meta', '--help'])
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
+    print(result.output)
+    expected_strings = """
+      cp        Copy meta to/from the project bucket.
+      ls        Query buckets from submitted metadata.
+      rm        Remove meta from a project.
+      import    Import study from directory listing.
+      validate  Validate FHIR data in DIRECTORY.
+    """.split()
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['request_id'], "Missing request id"
-    request_id = request['request_id']
-    assert request['status'] == 'DRAFT', f"unexpected status {request['status']}"
+        assert expected_string in result.output, f"Should have printed {expected_string}"
 
-    print(f'--format json access access update {request_id} SUBMITTED')
-    result = runner.invoke(cli, f'--format json access update {request_id} SUBMITTED'.split())
-    assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
-    for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['status'] == 'SUBMITTED', f"unexpected status {request['status']}"
 
-    result = runner.invoke(cli, f'--format json access update {request_id} APPROVED'.split())
+def test_file(caplog):
+    """Ensure it prints file"""
+    runner = CliRunner()
+    result = runner.invoke(cli, ['files', '--help'])
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
+    print(result.output)
+    expected_strings = """
+      ls  List files in a project.
+      cp  Copy files to/from the project bucket.
+      rm  Remove files from a project.
+    """.split()
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['status'] == 'APPROVED', f"unexpected status {request['status']}"
+        assert expected_string in result.output, f"Should have printed {expected_string}"
+
 
-    result = runner.invoke(cli, f'--format json access update {request_id} SIGNED'.split())
+def test_config(caplog):
+    """Ensure it prints file"""
+    runner = CliRunner()
+    result = runner.invoke(cli, ['config', '--help'])
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
+    print(result.output)
+    expected_strings = """
+      ls  Show defaults.
+    """.split()
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['status'] == 'SIGNED', f"unexpected status {request['status']}"
+        assert expected_string in result.output, f"Should have printed {expected_string}"
```

### Comparing `gen3_util-0.0.2rc7/tests/integration/test_files.py` & `gen3_util-0.0.2rc8/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/integration/test_meta.py` & `gen3_util-0.0.2rc8/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/integration/test_project.py` & `gen3_util-0.0.2rc8/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_util-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.2rc8/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/unit/test_config.py` & `gen3_util-0.0.2rc8/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/unit/test_files.py` & `gen3_util-0.0.2rc8/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/unit/test_meta.py` & `gen3_util-0.0.2rc8/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc7/tests/unit/test_validate_directory.py` & `gen3_util-0.0.2rc8/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

