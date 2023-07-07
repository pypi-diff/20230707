# Comparing `tmp/gen3_util-0.0.2rc6.tar.gz` & `tmp/gen3_util-0.0.2rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.2rc6.tar", last modified: Thu Jun 22 17:06:11 2023, max compression
+gzip compressed data, was "gen3_util-0.0.2rc7.tar", last modified: Thu Jul  6 19:58:29 2023, max compression
```

## Comparing `gen3_util-0.0.2rc6.tar` & `gen3_util-0.0.2rc7.tar`

### file list

```diff
@@ -1,71 +1,79 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.202558 gen3_util-0.0.2rc6/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc6/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-22 17:06:11.202393 gen3_util-0.0.2rc6/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     6374 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.136662 gen3_util-0.0.2rc6/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.158931 gen3_util-0.0.2rc6/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/access/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.161379 gen3_util-0.0.2rc6/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.167312 gen3_util-0.0.2rc6/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4469 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.187335 gen3_util-0.0.2rc6/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4119 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.189243 gen3_util-0.0.2rc6/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.194244 gen3_util-0.0.2rc6/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.196817 gen3_util-0.0.2rc6/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.198287 gen3_util-0.0.2rc6/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-22 16:34:30.000000 gen3_util-0.0.2rc6/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-22 17:04:30.000000 gen3_util-0.0.2rc6/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.154913 gen3_util-0.0.2rc6/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-22 17:06:11.202607 gen3_util-0.0.2rc6/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-06-22 17:05:57.000000 gen3_util-0.0.2rc6/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.130195 gen3_util-0.0.2rc6/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.200055 gen3_util-0.0.2rc6/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2055 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.202131 gen3_util-0.0.2rc6/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.394527 gen3_util-0.0.2rc7/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc7/LICENSE
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8535 2023-07-06 19:58:29.394237 gen3_util-0.0.2rc7/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     7850 2023-07-06 01:19:54.000000 gen3_util-0.0.2rc7/README.md
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.355831 gen3_util-0.0.2rc7/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       71 2023-07-05 18:55:42.000000 gen3_util-0.0.2rc7/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.372647 gen3_util-0.0.2rc7/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2321 2023-06-30 14:28:04.000000 gen3_util-0.0.2rc7/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3973 2023-07-06 19:12:10.000000 gen3_util-0.0.2rc7/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.374182 gen3_util-0.0.2rc7/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-06-30 18:19:19.000000 gen3_util-0.0.2rc7/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5679 2023-07-01 13:38:21.000000 gen3_util-0.0.2rc7/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.375849 gen3_util-0.0.2rc7/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      629 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc7/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.376788 gen3_util-0.0.2rc7/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4637 2023-06-30 14:47:36.000000 gen3_util-0.0.2rc7/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc7/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.377156 gen3_util-0.0.2rc7/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5428 2023-07-06 00:58:23.000000 gen3_util-0.0.2rc7/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.378443 gen3_util-0.0.2rc7/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2824 2023-06-29 20:12:33.000000 gen3_util-0.0.2rc7/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      433 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.383083 gen3_util-0.0.2rc7/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      938 2023-06-28 20:40:29.000000 gen3_util-0.0.2rc7/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    12907 2023-06-29 18:03:19.000000 gen3_util-0.0.2rc7/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.386524 gen3_util-0.0.2rc7/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4117 2023-07-05 18:55:47.000000 gen3_util-0.0.2rc7/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2256 2023-07-01 13:41:32.000000 gen3_util-0.0.2rc7/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      323 2023-06-29 20:10:18.000000 gen3_util-0.0.2rc7/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    10062 2023-07-06 01:11:29.000000 gen3_util-0.0.2rc7/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      329 2023-06-29 19:48:08.000000 gen3_util-0.0.2rc7/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3858 2023-06-29 20:12:21.000000 gen3_util-0.0.2rc7/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.388146 gen3_util-0.0.2rc7/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2769 2023-07-01 13:37:39.000000 gen3_util-0.0.2rc7/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.2rc7/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      793 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc7/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.370593 gen3_util-0.0.2rc7/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8535 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1687 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       53 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      128 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       16 2023-07-06 19:58:29.000000 gen3_util-0.0.2rc7/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2023-07-06 19:58:29.394590 gen3_util-0.0.2rc7/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5580 2023-07-06 19:56:56.000000 gen3_util-0.0.2rc7/setup.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.350122 gen3_util-0.0.2rc7/tests/
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.390632 gen3_util-0.0.2rc7/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      270 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3931 2023-07-06 19:09:19.000000 gen3_util-0.0.2rc7/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      454 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      243 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc7/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2089 2023-06-29 20:23:35.000000 gen3_util-0.0.2rc7/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2443 2023-06-29 20:10:37.000000 gen3_util-0.0.2rc7/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1237 2023-06-29 19:02:47.000000 gen3_util-0.0.2rc7/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.393202 gen3_util-0.0.2rc7/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.393569 gen3_util-0.0.2rc7/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 00:58:23.000000 gen3_util-0.0.2rc7/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-06 19:58:29.393782 gen3_util-0.0.2rc7/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1450 2023-07-06 01:18:25.000000 gen3_util-0.0.2rc7/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3380 2023-06-29 20:22:33.000000 gen3_util-0.0.2rc7/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc7/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2699 2023-07-06 01:20:50.000000 gen3_util-0.0.2rc7/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc7/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.2rc6/LICENSE` & `gen3_util-0.0.2rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/PKG-INFO` & `gen3_util-0.0.2rc7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: gen3_util
-Version: 0.0.2rc6
-Summary: Commons utilities
-Home-page: https://github.com/ACED-IDP/gen3_util
-Author: Ellrott Lab
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
-Project-URL: Source, https://github.com/ACED-IDP/gen3_util
-Keywords: gen3 bioinformatics
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # Gen3 Utilities
 
 Utilities to manage Gen3 schemas, projects and submissions.
 
 ## Installation
 
@@ -132,40 +112,113 @@
       region: us-east-1
 endpoint: https://aced-training.compbio.ohsu.edu
 msg: OK
 
 
 ```
 
+> I need to create a project
 
-> I want to create a simple project with a set of files
+```text
+$ gen3_util projects touch aced-MyExperiment
+projects:
+  aced-MyExperiment:
+    exists: true
+messages:
+- Created program:aced Program is updated!
 
 ```
-$ gen3_util meta  import dir tests/fixtures/dir_to_study/ tmp/foo --project_id aced-Alcoholism
-msg: OK
+
+> I need to assign default policies to that project
+
+```text
+$ gen3_util projects add policies aced-MyExperiment
+msg: Approve these requests to assign default policies to aced-MyExperiment
+commands:
+- gen3_util access update 24f047d7-0e7c-43c6-bab6-61e2d385c71a SIGNED
+- gen3_util access update 293c6cd1-7ab7-420f-bafb-34319589eac4 SIGNED
+
+```
+
+> I need to add a user to that project
+
+```text
+$ gen3_util projects add user aced-MyExperiment linus.pauling@osu.edu
+msg: Approve these requests to add linus.pauling@osu.edu to aced-MyExperiment
+commands:
+- gen3_util access update 293c6cd1-7ab7-420f-bafb-34319589eac4 SIGNED
+
+```
+
+> Before proceeding, I need to sign those equests
+```text
+gen3_util access update xxxxxx SIGNED
+```
+
+```text
+
+> I want to create a simple project structure with a set of files
+
+```
+$ gen3_util meta  import dir tests/fixtures/dir_to_study/ tmp/foo --project_id aced-MyExperiment
 summary:
+  ResearchStudy:
+    count: 1
   DocumentReference:
     count: 5
     size: 6013814
+msg: OK
+
+```
+
+> I want need to do something a bit more complex, for example, I want to create a project structure with a set of files, but I need to specify the `Patient` and `Specimen` based on the path of the file.
+
+```text
+gen3_util meta  import dir tests/fixtures/dir_to_study_with_meta/ tmp/foometa --project_id aced-foometa --plugin_path ./tests/unit/plugins
+
+tests/fixtures/dir_to_study_with_meta/
+├── file-2.csv
+├── p1
+│   ├── s1
+│   │   └── file-3.pdf
+│   ├── s2
+│   │   └── file-4.tsv
+│   └── s3
+│       └── file-5
+└── p2
+    └── s4
+        └── file-1.txt
+
+Will produce the following meta data:
+
+summary:
   ResearchStudy:
     count: 1
+  Patient:
+    count: 2
+  Specimen:
+    count: 4
+  DocumentReference:
+    count: 5
+    size: 6013814
+
 ```
 
-> I need to upload those files to the instance
+For more see [test_meta_plugin](./tests/unit/meta/test_plugins.py)
+
+
+
+> I need to upload the meta data about those files to the instance
 
 ```
-$ gen3_util files cp --ignore_state --project_id aced-Alcoholism tmp/foo/DocumentReference.ndjson  bucket://aced-ohsu
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████| 5.74M/5.74M [00:03<00:00, 1.71MB/s, elapsed=0:00:02.056022, file=6f8101]
-errors: []
-incomplete: []
-info:
-- Wrote state to ~/.gen3/gen3-util-state/state.ndjson
-msg: OK
+$gen3_util meta cp tmp/foo bucket://aced-development-ohsu-data-bucket --project_id aced-MyExperiment
+msg: Uploaded /var/folders/2c/hffqqtr94nv64tjy0xrl38r89k1sty/T/tmpacozhhoo/_aced-MyExperiment_meta.zip
 ```
 
+
 > I need to request or manage access to a project
 
 ```
 $ gen3_util access
 Usage: gen3_util access [OPTIONS] COMMAND [ARGS]...
 
   Manage access requests.
@@ -177,14 +230,18 @@
   touch   Create a request for read access.
   update  Update the request's approval workflow.
   ls      List current user's requests.
   cat     Show details of a specific request.
 
 ```
 
+
+
+
+
 ## Development Setup
 
 ```
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
@@ -261,9 +318,7 @@
 
 # this could be maintained as so: export $(cat .env | xargs)
 
 rm -r dist/
 python3  setup.py sdist bdist_wheel
 twine upload dist/*
 ```
-
-
```

### Comparing `gen3_util-0.0.2rc6/gen3_util/access/__init__.py` & `gen3_util-0.0.2rc7/gen3_util/access/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 from gen3.auth import Gen3Auth
+from requests import HTTPError
 
 from gen3_util.config import ensure_auth, Config
 
 
 def _ensure_auth(auth, config):
     """Create auth from config, if we don't have one already."""
     if not auth:
@@ -12,35 +13,47 @@
     return auth
 
 
 def get_requests(config: Config = None, auth: Gen3Auth = None, mine: bool = False) -> dict:
     """Fetch information about the user."""
     auth = _ensure_auth(auth, config)
     if mine:
+        # returns a list of dicts
+        # https://github.com/uc-cdis/requestor/blob/master/src/requestor/routes/query.py#L200
         return auth.curl('/requestor/request/user').json()
     else:
+        # returns a list of dicts
+        # https://github.com/uc-cdis/requestor/blob/master/src/requestor/routes/query.py#L158
         return auth.curl('/requestor/request').json()
 
 
 def get_request(config: Config = None, auth: Gen3Auth = None, request_id: str = None):
     """Get a specific request"""
     assert request_id, "required"
     auth = _ensure_auth(auth, config)
+    # returns a dict
+    # https://github.com/uc-cdis/requestor/blob/master/src/requestor/routes/query.py#L235
     return auth.curl(f'/requestor/request/{request_id}').json()
 
 
-def create_request(config: Config = None, auth: Gen3Auth = None, resource_path: str = None):
+def create_request(config: Config = None, auth: Gen3Auth = None, request: dict = None):
     """Get a specific request"""
-    assert resource_path, "required"
     auth = _ensure_auth(auth, config)
-    request = {'resource_path': resource_path, "username": "foo@bar.com"}  # , 'policy_id': 'aced_reader'
+    one_of = ['policy_id', 'resource_paths', 'resource_path']
+    assert any([k in request for k in one_of]), (f"one of {one_of} required", request)
     response = requests.post(
         auth.endpoint + "/" + 'requestor/request', json=request, auth=auth
     )
-    response.raise_for_status()
+    try:
+        response.raise_for_status()
+    except HTTPError as e:
+        print(e)
+        print(response.text)
+        raise e
+
     return response.json()
 
 
 def update_request(config: Config = None, auth: Gen3Auth = None, request_id: str = None, status: str = None):
     """Update a specific request"""
     assert request_id, "required"
     assert status, "required"
```

### Comparing `gen3_util-0.0.2rc6/gen3_util/access/cli.py` & `gen3_util-0.0.2rc7/gen3_util/projects/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,87 @@
 import click
 
-from gen3_util.access.requestor import ls, cat, touch, update
+from gen3_util.access.requestor import add_policies, add_user
 from gen3_util.cli import CLIOutput
 from gen3_util.cli import NaturalOrderGroup
-from gen3_util.config import Config
+from gen3_util.config import Config, ensure_auth
+from gen3_util.projects.creator import touch
+from gen3_util.projects.lister import ls
+from gen3_util.projects.remover import rm
 
 
-@click.group(name='access', cls=NaturalOrderGroup)
+@click.group(name='projects', cls=NaturalOrderGroup)
 @click.pass_obj
-def access_group(config: Config):
-    """Manage access requests."""
+def project_group(config: Config):
+    """Manage Gen3 projects."""
     pass
 
 
-@access_group.command(name="touch")
-@click.argument('user_name')
-@click.argument('resource_path')
+@project_group.command(name="ping")
 @click.pass_obj
-def access_touch(config: Config,  user_name: str, resource_path: str):
-    """Create a request for read access.
+def ping(config: Config):
+    """Test connectivity to Gen3 endpoint."""
+    with CLIOutput(config=config) as output:
+        auth = ensure_auth(config.gen3.refresh_file, validate=True)
+        output.update({'endpoint': auth.endpoint, 'username': auth.curl('/user/user').json()['username']})
 
-    \b
-    user_name (str): user's email
-    resource_path (str): /programs/XXX/project/YYY
 
-    """
+@project_group.command(name="ls")
+@click.pass_obj
+def project_ls(config: Config):
+    """List all projects user has access to."""
     with CLIOutput(config=config) as output:
-        output.update(touch(config, resource_path))
+        output.update(ls(config))
 
 
-@access_group.command(name="update")
-@click.argument('request_id')
-@click.argument('status')
+@project_group.command(name="touch")
+@click.argument('project_id', required=False)
+@click.option('--all/--no-all', '-a', 'all_', help='Create all configured projects', is_flag=True, default=False)
 @click.pass_obj
-def access_update(config: Config, request_id: str, status: str):
-    """Update the request's approval workflow.
-
-    \b
-    request_id (str): uuid of an existing request
-    status (str): new status see {ALLOWED_REQUEST_STATUSES}
+def project_touch(config: Config, project_id: str, all_: bool):
+    """Create a project
+    PROJECT_ID: <program-name>-<project-name>
     """
     with CLIOutput(config=config) as output:
-        output.update(update(config, request_id, status))
+        output.update(touch(config, project_id, all_))
 
 
-@access_group.command(name="ls")
-@click.option('--mine',  is_flag=True, show_default=True, default=False, help="List current user's requests. Otherwise, list all the requests the current user has access to see.")
+@project_group.command(name="rm")
+@click.argument('project_id')
 @click.pass_obj
-def access_ls(config: Config, mine: bool):
-    """List current user's requests."""
+def project_rm(config: Config, project_id: str):
+    """Remove project.
+    PROJECT_ID: <program-name>-<project-name>
+    """
     with CLIOutput(config=config) as output:
-        output.update(ls(config, mine))
+        output.update(rm(config, project_id))
+
+
+@project_group.group(name="add")
+def project_add():
+    """Add policies and users to a project."""
+    pass
 
 
-@access_group.command(name="cat")
-@click.argument('request_id')
+@project_add.command(name="user")
+@click.argument('project_id')
+@click.argument('user_name')
+@click.option('--write/--no-write', '-a', help='Give user write privileges', is_flag=True, default=False)
 @click.pass_obj
-def access_cat(config: Config, request_id: str):
-    """Show details of a specific request.
+def project_add_user(config: Config, user_name: str, project_id: str, write: bool):
+    """Add user to project.
+    PROJECT_ID: <program-name>-<project-name>
+    USER_NAME: user's email
+    """
+    with CLIOutput(config=config) as output:
+        output.update(add_user(config, project_id, user_name, write))
+
 
-    \b
-    request_id (str): uuid of an existing request
+@project_add.command(name="policies")
+@click.argument('project_id')
+@click.pass_obj
+def project_add_policies(config: Config, project_id: str):
+    """Add default policies to project.
+    PROJECT_ID: <program-name>-<project-name>
     """
     with CLIOutput(config=config) as output:
-        output.update(cat(config, request_id))
+        output.update(add_policies(config, project_id))
```

### Comparing `gen3_util-0.0.2rc6/gen3_util/buckets/__init__.py` & `gen3_util-0.0.2rc7/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/buckets/cli.py` & `gen3_util-0.0.2rc7/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/cli/__init__.py` & `gen3_util-0.0.2rc7/gen3_util/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,25 +80,27 @@
         return self.commands.keys()
 
 
 class CommandOutput(object):
     """Output object for commands."""
     def __init__(self):
         self.obj = None
+        self.exit_code = 0
 
     def update(self, obj):
         """Update output with obj."""
         self.obj = obj
 
 
 class CLIOutput:
     """Ensure output, exceptions and exit code are returned to user consistently."""
-    def __init__(self, config: Config):
+    def __init__(self, config: Config, exit_on_error: bool = True):
         self.output = CommandOutput()
         self.config = config
+        self.exit_on_error = exit_on_error
 
     def __enter__(self):
         return self.output
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         rc = 0
         _ = {}
@@ -119,8 +121,10 @@
         prune = []
         for k, v in _.items():
             if not v:
                 prune.append(k)
         for k in prune:
             del _[k]
         print_formatted(self.config, _)
-        exit(rc)
+        self.output.exit_code = rc
+        if self.exit_on_error:
+            exit(rc)
```

### Comparing `gen3_util-0.0.2rc6/gen3_util/cli/cli.py` & `gen3_util-0.0.2rc7/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/common/__init__.py` & `gen3_util-0.0.2rc7/gen3_util/common/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,15 +33,19 @@
         for l_ in jsonfile.readlines():
             yield orjson.loads(l_)
 
 
 def read_json_file(path: str) -> Iterator[dict]:
     """Read ndjson file, load json line by line."""
     with _file_opener(path) as jsonfile:
-        yield orjson.loads(jsonfile.read())
+        try:
+            yield orjson.loads(jsonfile.read())
+        except orjson.JSONDecodeError as e:
+            logging.error(f"Error reading {path}: {e}")
+            raise
 
 
 def read_json(path: str) -> Iterator[dict]:
     """Read json or ndjson from file or zip."""
     if is_ndjson(path):
         _reader = read_ndjson_file
     else:
@@ -136,7 +140,44 @@
     def emit(self, name: str) -> TextIO:
         """Maintain a hash of open files."""
         if name not in self.emitters:
             self.emitters[name] = open(self.output_path / f"{name}.ndjson", self.file_mode)
             if self.verbose:
                 self.logger.info(f"opened {self.emitters[name].name}")
         return self.emitters[name]
+
+
+def validate_project_id(project_id) -> list[str]:
+    """Ensure that the project_id is valid"""
+    msgs = []
+    if not project_id:
+        msgs.append("project_id is missing")
+    if not project_id.count('-') == 1:
+        msgs.append(f"{project_id} should have a single '-' delimiter.")
+    return msgs
+
+
+def validate_email(email) -> list[str]:
+    """Ensure that the email is valid"""
+    msgs = []
+    if not email:
+        msgs.append("email is missing")
+    if not email.count('@') == 1:
+        msgs.append(f"{email} should have a single '@' delimiter.")
+    try:
+        from email_validator import validate_email as email_validator_validate, EmailNotValidError
+        email_validator_validate(email)
+    except EmailNotValidError as e:
+        msgs.append(f"{email} is not a valid email address. {e}")
+    return msgs
+
+
+def to_resource_path(project_id, resource_path):
+    """Canonical conversion of project_id to resource path."""
+
+    assert not (resource_path and project_id), "Please choose either project_id or resource_path"
+
+    if resource_path:
+        return resource_path
+
+    _ = project_id.split('-')
+    return f"/programs/{_[0]}/projects/{_[1]}"
```

### Comparing `gen3_util-0.0.2rc6/gen3_util/files/__init__.py` & `gen3_util-0.0.2rc7/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/files/cli.py` & `gen3_util-0.0.2rc7/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/files/downloader.py` & `gen3_util-0.0.2rc7/gen3_util/files/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     url = urlparse(from_)
     assert url.scheme, f"{from_} does not appear to be a url"
     return from_, to_
 
 
 def cp(config: Config, from_: str, to_: str):
     """Copy files from bucket to local file system."""
-    from_, to_ = _validate_parameters(from_, to_)
-    print_formatted(config, {'msg': 'file download progress goes here'})
+    # from_, to_ = _validate_parameters(from_, to_)
+    print_formatted(config, {'msg': 'Please use "gen3 file download-single OBJECT_ID"'})
```

### Comparing `gen3_util-0.0.2rc6/gen3_util/files/uploader.py` & `gen3_util-0.0.2rc7/gen3_util/files/uploader.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 from dataclasses import dataclass
 from multiprocessing import Pool
 from time import sleep
 from typing import List
 from urllib.parse import urlparse, ParseResult
 
 import requests
-from gen3_util.common import read_ndjson_file
-from gen3.file import Gen3File
-from gen3.index import Gen3Index
 from orjson import orjson
 from pydantic import BaseModel
 from tqdm import tqdm
 
-from gen3_util.config import Config, ensure_auth
+from gen3_util.common import read_ndjson_file
+from gen3_util.config import Config, gen3_services
 from gen3_util.files import assert_valid_project_id, assert_valid_bucket
 
 logger = logging.getLogger(__name__)
 
 
 def _upload_file_to_signed_url(file_name, md5sum, metadata, signed_url):
     """Upload file """
@@ -39,24 +37,25 @@
         # SYNC
         response = requests.put(signed_url, data=fp)
         response_text = response.text
         assert response.status_code == 200, (signed_url, response_text)
 
 
 def _update_indexd(attachment, bucket_name, document_reference, duplicate_check, index_client, md5sum, object_name,
-                   program, project):
+                   program, project, metadata=None):
     hashes = {'md5': md5sum}
     assert 'id' in document_reference, document_reference
     guid = document_reference['id']
-    metadata = {
-        **{
-            'datanode_type': 'DocumentReference',
-            'datanode_object_id': guid
-        },
-        **hashes}
+    if metadata is None:
+        metadata = {
+            **{
+                'datanode_type': 'DocumentReference',
+                'datanode_object_id': guid
+            },
+            **hashes}
     # SYNC
     existing_record = None
     s3_url = f"s3://{bucket_name}/{guid}/{object_name}"
     if duplicate_check:
         try:
             existing_record = index_client.get_record(guid=document_reference["id"])
         except Exception: # noqa
@@ -108,22 +107,14 @@
     assert len(md5_extension) == 1, "Missing MD5 extension."
     md5sum = md5_extension[0]['valueString']
     source_path_extension = [_ for _ in attachment['extension'] if
                              _['url'] == "http://aced-idp.org/fhir/StructureDefinition/source_path"]
     return attachment, md5sum, source_path_extension
 
 
-def _gen3_services(config: Config) -> (Gen3File, Gen3Index):
-    """Create Gen3 Services."""
-    auth = ensure_auth(config.gen3.refresh_file)
-    file_client = Gen3File(auth_provider=auth)
-    index_client = Gen3Index(auth_provider=auth)
-    return file_client, index_client
-
-
 def _validate_parameters(from_: str, to_: str) -> (pathlib.Path, ParseResult):
     url = urlparse(to_)
     assert url.scheme, f"{to_} does not appear to be a url"
 
     assert len(urlparse(from_).scheme) == 0, f"{from_} appears to be an url. url to url cp not supported"
 
     from_ = pathlib.Path(from_)
@@ -156,18 +147,16 @@
 def _upload_document_reference(config: Config, document_reference: dict, bucket_name: str,
                                program: str, project: str, duplicate_check: bool,
                                source_path: str) -> UploadResult:
     """Write a single document reference to indexd and upload file."""
 
     try:
         start = datetime.datetime.now()
-        # print(('starting', document_reference['id'], start.isoformat()))
 
-        file_client, index_client = _gen3_services(config=config)
-        # print("Connected to gen3")
+        file_client, index_client, user = gen3_services(config=config)
 
         attachment, md5sum, source_path_extension = _extract_extensions(document_reference)
 
         source_path = _extract_source_path(attachment, source_path, source_path_extension)
 
         file_name = source_path.lstrip('./').lstrip('file:///')
         object_name = attachment['url'].lstrip('./').lstrip('file:///')
```

### Comparing `gen3_util-0.0.2rc6/gen3_util/meta/__init__.py` & `gen3_util-0.0.2rc7/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/meta/validator.py` & `gen3_util-0.0.2rc7/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/projects/__init__.py` & `gen3_util-0.0.2rc7/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/projects/creator.py` & `gen3_util-0.0.2rc7/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/projects/lister.py` & `gen3_util-0.0.2rc7/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util/projects/remover.py` & `gen3_util-0.0.2rc7/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.2rc7/gen3_util.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 gen3_util.egg-info/dependency_links.txt
 gen3_util.egg-info/entry_points.txt
 gen3_util.egg-info/requires.txt
 gen3_util.egg-info/top_level.txt
 gen3_util/access/__init__.py
 gen3_util/access/cli.py
 gen3_util/access/requestor.py
+gen3_util/access/policies/__init__.py
 gen3_util/buckets/__init__.py
 gen3_util/buckets/cli.py
 gen3_util/buckets/lister.py
 gen3_util/cli/__init__.py
 gen3_util/cli/cli.py
 gen3_util/common/__init__.py
 gen3_util/config/__init__.py
@@ -39,17 +40,21 @@
 gen3_util/projects/creator.py
 gen3_util/projects/lister.py
 gen3_util/projects/remover.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/test_access.py
 tests/integration/test_buckets.py
+tests/integration/test_config.py
 tests/integration/test_files.py
+tests/integration/test_meta.py
 tests/integration/test_project.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_cli.py
 tests/unit/test_coding_conventions.py
 tests/unit/test_config.py
 tests/unit/test_files.py
 tests/unit/test_meta.py
-tests/unit/test_validate_directory.py
+tests/unit/test_validate_directory.py
+tests/unit/plugins/__init__.py
+tests/unit/plugins/gen3_util_plugin_foo/__init__.py
```

### Comparing `gen3_util-0.0.2rc6/setup.py` & `gen3_util-0.0.2rc7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2-rc6',  # Required
+    version='0.0.2-rc7',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.2rc6/tests/integration/test_access.py` & `gen3_util-0.0.2rc7/tests/integration/test_meta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 import json
+import pathlib
 
 from click.testing import CliRunner
+
 from gen3_util.cli.cli import cli
 
 
-def test_access_ls(caplog):
-    """Ensure we can ls access."""
+def import_from_directory():
+    params = 'meta  import dir tests/fixtures/dir_to_study/ tmp/foo --project_id aced-foo'.split()
     runner = CliRunner()
-    result = runner.invoke(cli, ['access', 'ls'])
+    result = runner.invoke(cli, params)
+    print(result.output)
     assert result.exit_code == 0
-    expected_strings = ['OK']
+    expected_strings = ['DocumentReference', "size: 6013814", 'ResearchStudy', "count: 1"]
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-
+        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
 
-# def test_access_touch():
-#     """Ensure we detect missing input path."""
-#     runner = CliRunner()
-#     result = runner.invoke(cli, 'access touch bar@foo.com /programs/aced/project/MCF10A'.split())
-#     assert result.exit_code == 0
-#     expected_strings = ['OK', 'request_id']
-#     for expected_string in expected_strings:
-#         assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
+    result = runner.invoke(cli, 'meta validate tmp/foo'.split())
+    print(result.output)
+    assert result.exit_code == 0
+    expected_strings = ["msg: OK"]
+    for expected_string in expected_strings:
+        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
 
 
-def test_access_workflow():
+def ls():
+    params = '--format json meta ls'.split()
     runner = CliRunner()
-    result = runner.invoke(cli, '--format json access touch bar@foo.com /programs/aced/project/MCF10A'.split())
+    result = runner.invoke(cli, params)
+    print(result.output)
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
+    expected_strings = ['"msg": "OK"', "is_metadata", "file_name"]
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['request_id'], "Missing request id"
-    request_id = request['request_id']
-    assert request['status'] == 'DRAFT', f"unexpected status {request['status']}"
+        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
+    return json.loads(result.output)
 
-    print(f'--format json access access update {request_id} SUBMITTED')
-    result = runner.invoke(cli, f'--format json access update {request_id} SUBMITTED'.split())
-    assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
-    for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['status'] == 'SUBMITTED', f"unexpected status {request['status']}"
 
-    result = runner.invoke(cli, f'--format json access update {request_id} APPROVED'.split())
+def cp_upload(data_bucket):
+    params = f'--format json meta cp tmp/foo/extractions bucket://{data_bucket} --project_id aced-foo --ignore_state'.split()
+    runner = CliRunner()
+    result = runner.invoke(cli, params)
+    print(result.output)
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
+    expected_strings = ['Uploaded']
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['status'] == 'APPROVED', f"unexpected status {request['status']}"
+        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
+
 
-    result = runner.invoke(cli, f'--format json access update {request_id} SIGNED'.split())
+def cp_download(did):
+    params = f'--format json meta cp {did} tmp/foo/'.split()
+    runner = CliRunner()
+    result = runner.invoke(cli, params)
+    print(result.output)
     assert result.exit_code == 0
-    expected_strings = ['OK', 'request_id']
+    expected_strings = ['Downloaded']
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"Did not find {expected_string} in {expected_strings}"
-    request = json.loads(result.output)['request']
-    assert request['status'] == 'SIGNED', f"unexpected status {request['status']}"
+        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
+
+
+def test_workflow(data_bucket):
+    import_from_directory()
+    cp_upload(data_bucket)
+    records = ls()['records']
+    for _ in records:
+        cp_download(_['did'])
+        stat = pathlib.Path(f"tmp/foo/{_['file_name']}").stat()
+        assert stat.st_size == _['size']
```

### Comparing `gen3_util-0.0.2rc6/tests/integration/test_files.py` & `gen3_util-0.0.2rc7/tests/integration/test_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 
 from click.testing import CliRunner
 
 from gen3_util.cli.cli import cli
 
 
-def test_files_upload_bad_source(caplog):
+def test_files_upload_bad_source(caplog, data_bucket):
     """Ensure we detect missing input path."""
     runner = CliRunner()
-    result = runner.invoke(cli, ['files', 'cp', '--project_id', 'prog-proj', 'foo', 'bucket://bar'])
+    result = runner.invoke(cli, ['files', 'cp', '--project_id', 'prog-proj', 'foo', f'bucket://{data_bucket}'])
     assert result.exit_code == 1
     expected_strings = ['foo does not exist']
     for expected_string in expected_strings:
         assert expected_string in result.output, "Did not find project does not exist error"
 
 
-def test_files_upload(caplog):
+def test_files_upload(caplog, data_bucket):
     """Ensure we upload files from generated DocumentReferences to existing project."""
 
     runner = CliRunner()
 
     params = 'meta  import dir tests/fixtures/dir_to_study/ tmp/Alcoholism --project_id aced-Alcoholism'.split()
     result = runner.invoke(cli, params)
     print(result.output)
     assert result.exit_code == 0, "Could not create project from directory"
 
-    result = runner.invoke(cli, ['files', 'cp', '--project_id', 'aced-foo', 'tmp/Alcoholism', 'bucket://bar'])
+    result = runner.invoke(cli, ['files', 'cp', '--project_id', 'aced-XXXX', 'tmp/Alcoholism', 'bucket://bar'])
     assert result.exit_code == 1
     print(result.output)
-    expected_strings = ['aced-foo does not exist']
+    expected_strings = ['aced-XXXX does not exist']
     for expected_string in expected_strings:
         assert expected_string in result.output, "Did not find project does not exist error"
 
     result = runner.invoke(cli, ['files', 'cp', '--project_id', 'aced-Alcoholism', 'tmp/Alcoholism', 'bucket://bar'])
     assert result.exit_code == 1
     print(result.output)
     expected_strings = ['bar not in configured buckets']
     for expected_string in expected_strings:
         assert expected_string in result.output, "Did not find bucket does not exist error"
 
     result = runner.invoke(cli, ['files', 'cp', '--project_id', 'aced-Alcoholism', '--ignore_state',
-                                 'tmp/Alcoholism/DocumentReference.ndjson', 'bucket://aced-ohsu-staging'])
+                                 'tmp/Alcoholism/DocumentReference.ndjson', "bucket://"+data_bucket])
     assert result.exit_code == 0
     print(result.output)
     expected_strings = ['OK']
     for expected_string in expected_strings:
         assert expected_string in result.output, "Did not find OK message"
```

### Comparing `gen3_util-0.0.2rc6/tests/integration/test_project.py` & `gen3_util-0.0.2rc7/tests/integration/test_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def test_project_ping(caplog):
     """Ensure we can retrieve connected message."""
     runner = CliRunner()
     result = runner.invoke(cli, ['projects', 'ping'])
     assert result.exit_code == 0
-    expected_strings = ['OK', 'http']
+    expected_strings = ['OK', 'http', 'username']
     for expected_string in expected_strings:
         assert expected_string in result.output, "Did not find connected message."
 
 
 def test_project_bad_ping(caplog):
     """Ensure we can descriptive error."""
     runner = CliRunner(mix_stderr=False)
```

### Comparing `gen3_util-0.0.2rc6/tests/unit/test_cli.py` & `gen3_util-0.0.2rc7/tests/unit/test_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 def test_help(caplog):
     """Ensure it prints command groups"""
     runner = CliRunner()
     result = runner.invoke(cli, ['--help'])
     assert result.exit_code == 0
     print(result.output)
     expected_strings = """
-      projects  Manage Gen3 projects.
-      meta      Manage meta data.
-      files     Manage file buckets.
-      config    Configure this utility.
-    """.split()
+        projects  Manage Gen3 projects.
+        buckets   Manage Gen3 buckets.
+        meta      Manage meta data.
+        files     Manage file transfers.
+        access    Manage access requests.
+        config    Configure this utility.
+        """.split()
     for expected_string in expected_strings:
         assert expected_string in result.output, f"Should have printed {expected_string}"
 
 
 def test_projects(caplog):
     """Ensure it prints project"""
     runner = CliRunner()
@@ -56,18 +58,19 @@
 def test_meta(caplog):
     """Ensure it prints meta"""
     runner = CliRunner()
     result = runner.invoke(cli, ['meta', '--help'])
     assert result.exit_code == 0
     print(result.output)
     expected_strings = """
-      ls        List meta in a project.
-      validate  Copy meta to/from the project bucket.
       cp        Copy meta to/from the project bucket.
+      ls        Query buckets from submitted metadata.
       rm        Remove meta from a project.
+      import    Import study from directory listing.
+      validate  Validate FHIR data in DIRECTORY.
     """.split()
     for expected_string in expected_strings:
         assert expected_string in result.output, f"Should have printed {expected_string}"
 
 
 def test_file(caplog):
     """Ensure it prints file"""
```

### Comparing `gen3_util-0.0.2rc6/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.2rc7/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/tests/unit/test_config.py` & `gen3_util-0.0.2rc7/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/tests/unit/test_files.py` & `gen3_util-0.0.2rc7/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc6/tests/unit/test_validate_directory.py` & `gen3_util-0.0.2rc7/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

