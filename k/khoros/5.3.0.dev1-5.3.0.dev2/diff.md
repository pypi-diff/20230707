# Comparing `tmp/khoros-5.3.0.dev1.tar.gz` & `tmp/khoros-5.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khoros-5.3.0.dev1.tar", last modified: Thu Jul  6 19:41:58 2023, max compression
+gzip compressed data, was "khoros-5.3.0.dev2.tar", last modified: Fri Jul  7 19:37:54 2023, max compression
```

## Comparing `khoros-5.3.0.dev1.tar` & `khoros-5.3.0.dev2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.652542 khoros-5.3.0.dev1/
--rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.3.0.dev1/LICENSE
--rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-06 19:41:58.651457 khoros-5.3.0.dev1/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)    15696 2023-01-02 17:40:43.000000 khoros-5.3.0.dev1/README.md
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.580067 khoros-5.3.0.dev1/khoros/
--rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    73826 2023-06-14 20:24:00.000000 khoros-5.3.0.dev1/khoros/api.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11891 2023-06-14 19:57:43.000000 khoros-5.3.0.dev1/khoros/auth.py
--rw-r--r--   0 shurtj     (501) staff       (20)    14989 2023-06-14 19:56:42.000000 khoros-5.3.0.dev1/khoros/bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)   278016 2023-06-06 21:08:56.000000 khoros-5.3.0.dev1/khoros/core.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.587945 khoros-5.3.0.dev1/khoros/errors/
--rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.3.0.dev1/khoros/errors/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/errors/exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11117 2023-06-14 20:26:29.000000 khoros-5.3.0.dev1/khoros/errors/handlers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.3.0.dev1/khoros/errors/translations.py
--rw-r--r--   0 shurtj     (501) staff       (20)    23051 2023-06-06 21:11:32.000000 khoros-5.3.0.dev1/khoros/liql.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.601598 khoros-5.3.0.dev1/khoros/objects/
--rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.3.0.dev1/khoros/objects/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.3.0.dev1/khoros/objects/albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/objects/archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.3.0.dev1/khoros/objects/attachments.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/objects/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)      519 2021-10-11 04:30:21.000000 khoros-5.3.0.dev1/khoros/objects/labels.py
--rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.3.0.dev1/khoros/objects/messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/objects/roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.3.0.dev1/khoros/objects/settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.3.0.dev1/khoros/objects/subscriptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/objects/tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)    61692 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/objects/users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/saml.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.612649 khoros-5.3.0.dev1/khoros/structures/
--rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/structures/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.3.0.dev1/khoros/structures/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)    32351 2023-06-05 22:07:05.000000 khoros-5.3.0.dev1/khoros/structures/boards.py
--rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.3.0.dev1/khoros/structures/categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/structures/communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/structures/grouphubs.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.3.0.dev1/khoros/structures/nodes.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.615466 khoros-5.3.0.dev1/khoros/studio/
--rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.3.0.dev1/khoros/studio/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2845 2023-06-14 20:27:59.000000 khoros-5.3.0.dev1/khoros/studio/base.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.622828 khoros-5.3.0.dev1/khoros/utils/
--rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.3.0.dev1/khoros/utils/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/environment.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/helper.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/log_utils.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.650153 khoros-5.3.0.dev1/khoros/utils/tests/
--rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.3.0.dev1/khoros/utils/tests/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/resources.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_board_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_error_handling.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_grouphub_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_helper_file.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_http_headers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_library_import.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_liql.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_mentions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    13752 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_node_id_extract.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_ssl_verify.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_studio.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8450 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_version.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3790 2023-06-02 20:52:17.000000 khoros-5.3.0.dev1/khoros/utils/version.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.583883 khoros-5.3.0.dev1/khoros.egg-info/
--rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/SOURCES.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/dependency_links.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/requires.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/top_level.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      917 2023-06-20 13:43:52.000000 khoros-5.3.0.dev1/pyproject.toml
--rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-07-06 19:41:58.652755 khoros-5.3.0.dev1/setup.cfg
--rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.3.0.dev1/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.508592 khoros-5.3.0.dev2/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.3.0.dev2/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-07 19:37:54.508036 khoros-5.3.0.dev2/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)    15696 2023-01-02 17:40:43.000000 khoros-5.3.0.dev2/README.md
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.450049 khoros-5.3.0.dev2/khoros/
+-rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    73826 2023-06-14 20:24:00.000000 khoros-5.3.0.dev2/khoros/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11891 2023-06-14 19:57:43.000000 khoros-5.3.0.dev2/khoros/auth.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    14989 2023-06-14 19:56:42.000000 khoros-5.3.0.dev2/khoros/bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)   279262 2023-07-06 21:23:27.000000 khoros-5.3.0.dev2/khoros/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.455194 khoros-5.3.0.dev2/khoros/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.3.0.dev2/khoros/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11117 2023-06-14 20:26:29.000000 khoros-5.3.0.dev2/khoros/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.3.0.dev2/khoros/errors/translations.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    23051 2023-06-06 21:11:32.000000 khoros-5.3.0.dev2/khoros/liql.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.465203 khoros-5.3.0.dev2/khoros/objects/
+-rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.3.0.dev2/khoros/objects/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.3.0.dev2/khoros/objects/albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/objects/archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.3.0.dev2/khoros/objects/attachments.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/objects/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1508 2023-07-06 21:05:48.000000 khoros-5.3.0.dev2/khoros/objects/labels.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.3.0.dev2/khoros/objects/messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/objects/roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.3.0.dev2/khoros/objects/settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.3.0.dev2/khoros/objects/subscriptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/objects/tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    61692 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/objects/users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/saml.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.473961 khoros-5.3.0.dev2/khoros/structures/
+-rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/structures/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.3.0.dev2/khoros/structures/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    32351 2023-06-05 22:07:05.000000 khoros-5.3.0.dev2/khoros/structures/boards.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.3.0.dev2/khoros/structures/categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/structures/communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/structures/grouphubs.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.3.0.dev2/khoros/structures/nodes.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.477786 khoros-5.3.0.dev2/khoros/studio/
+-rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.3.0.dev2/khoros/studio/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2845 2023-06-14 20:27:59.000000 khoros-5.3.0.dev2/khoros/studio/base.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.483737 khoros-5.3.0.dev2/khoros/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.3.0.dev2/khoros/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/environment.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/helper.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/log_utils.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.506892 khoros-5.3.0.dev2/khoros/utils/tests/
+-rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.3.0.dev2/khoros/utils/tests/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/resources.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_board_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_error_handling.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_grouphub_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_helper_file.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_http_headers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_library_import.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_liql.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_mentions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    13752 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_node_id_extract.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_ssl_verify.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_studio.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     8450 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_version.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3790 2023-07-07 14:06:27.000000 khoros-5.3.0.dev2/khoros/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.452211 khoros-5.3.0.dev2/khoros.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/top_level.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      917 2023-07-07 14:06:40.000000 khoros-5.3.0.dev2/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-07-07 19:37:54.508756 khoros-5.3.0.dev2/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.3.0.dev2/setup.py
```

### Comparing `khoros-5.3.0.dev1/LICENSE` & `khoros-5.3.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/PKG-INFO` & `khoros-5.3.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.3.0.dev1
+Version: 5.3.0.dev2
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev1 Summary: Useful tools
+Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev2 Summary: Useful tools
 and utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
```

### Comparing `khoros-5.3.0.dev1/README.md` & `khoros-5.3.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/__init__.py` & `khoros-5.3.0.dev2/khoros/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/api.py` & `khoros-5.3.0.dev2/khoros/api.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/auth.py` & `khoros-5.3.0.dev2/khoros/auth.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/bulk_data.py` & `khoros-5.3.0.dev2/khoros/bulk_data.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/core.py` & `khoros-5.3.0.dev2/khoros/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 :Module:            khoros.core
 :Synopsis:          Collection of core functions and tools to work with the Khoros Community APIs
 :Usage:             ``import khoros.core`` *(Imported by default in primary package)*
 :Example:           ``khoros = Khoros(helper='helper.yml')``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     06 Jun 2023
+:Modified Date:     06 Jul 2023
 """
 
 import sys
 import copy
 import logging
 import warnings
 
@@ -298,14 +298,15 @@
         self.albums = self._import_album_class()
         self.archives = self._import_archives_class()
         self.boards = self._import_board_class()
         self.bulk_data = self._import_bulk_data_class()
         self.categories = self._import_category_class()
         self.communities = self._import_community_class()
         self.grouphubs = self._import_grouphub_class()
+        self.labels = self._import_label_class()
         self.messages = self._import_message_class()
         self.nodes = self._import_node_class()
         self.roles = self._import_role_class()
         self.saml = self._import_saml_class()
         self.settings = self._import_settings_class()
         self.studio = self._import_studio_class()
         self.subscriptions = self._import_subscription_class()
@@ -574,14 +575,21 @@
         """This method allows the :py:class:`khoros.core.Khoros.GroupHub` inner class to be utilized in the
         core object.
 
         .. versionadded:: 2.6.0
         """
         return Khoros.GroupHub(self)
 
+    def _import_label_class(self):
+        """This method allows the :py:class:`khoros.core.Khoros.Label` inner class to be utilized in the core object.
+
+        .. versionadded:: 5.3.0
+        """
+        return Khoros.Label(self)
+
     def _import_message_class(self):
         """This method allows the :py:class:`khoros.core.Khoros.Message` inner class to be utilized in the core object.
 
         .. versionadded:: 2.3.0
         """
         return Khoros.Message(self)
 
@@ -2814,14 +2822,36 @@
                      :py:exc:`khoros.errors.exceptions.PUTRequestError`
             """
             return structures_module.grouphubs.update_title(self.khoros_object, new_title, group_hub_id,
                                                             group_hub_url, full_response, return_id, return_url,
                                                             return_api_url, return_http_code, return_status,
                                                             return_error_messages, split_errors)
 
+    class Label(object):
+        """This class includes methods for interacting with labels."""
+        def __init__(self, khoros_object):
+            """This method initializes the :py:class:`khoros.core.Khoros.Label` inner class object.
+
+            :param khoros_object: The core :py:class:`khoros.Khoros` object
+            :type khoros_object: class[khoros.Khoros]
+            """
+            self.khoros_object = khoros_object
+
+        def get_labels_for_message(self, message_id):
+            """This method retrieves the labels associated with a specific message.
+
+            .. versionadded:: 5.3.0
+
+            :param message_id: The ID associated with the message to query
+            :type message_id: str, int
+            :returns: A list of strings for the labels
+            :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+            """
+            return objects_module.labels.get_labels_for_message(self.khoros_object, message_id)
+
     class Message(object):
         """This class includes methods for interacting with messages."""
         def __init__(self, khoros_object):
             """This method initializes the :py:class:`khoros.core.Khoros.Message` inner class object.
 
             :param khoros_object: The core :py:class:`khoros.Khoros` object
             :type khoros_object: class[khoros.Khoros]
```

### Comparing `khoros-5.3.0.dev1/khoros/errors/__init__.py` & `khoros-5.3.0.dev2/khoros/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/errors/exceptions.py` & `khoros-5.3.0.dev2/khoros/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/errors/handlers.py` & `khoros-5.3.0.dev2/khoros/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/errors/translations.py` & `khoros-5.3.0.dev2/khoros/errors/translations.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/liql.py` & `khoros-5.3.0.dev2/khoros/liql.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/__init__.py` & `khoros-5.3.0.dev2/khoros/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/albums.py` & `khoros-5.3.0.dev2/khoros/objects/albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/archives.py` & `khoros-5.3.0.dev2/khoros/objects/archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/attachments.py` & `khoros-5.3.0.dev2/khoros/objects/attachments.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/base.py` & `khoros-5.3.0.dev2/khoros/objects/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/messages.py` & `khoros-5.3.0.dev2/khoros/objects/messages.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/roles.py` & `khoros-5.3.0.dev2/khoros/objects/roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/settings.py` & `khoros-5.3.0.dev2/khoros/objects/settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/subscriptions.py` & `khoros-5.3.0.dev2/khoros/objects/subscriptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/tags.py` & `khoros-5.3.0.dev2/khoros/objects/tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/objects/users.py` & `khoros-5.3.0.dev2/khoros/objects/users.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/saml.py` & `khoros-5.3.0.dev2/khoros/saml.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/structures/__init__.py` & `khoros-5.3.0.dev2/khoros/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/structures/base.py` & `khoros-5.3.0.dev2/khoros/structures/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/structures/boards.py` & `khoros-5.3.0.dev2/khoros/structures/boards.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/structures/categories.py` & `khoros-5.3.0.dev2/khoros/structures/categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/structures/communities.py` & `khoros-5.3.0.dev2/khoros/structures/communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/structures/grouphubs.py` & `khoros-5.3.0.dev2/khoros/structures/grouphubs.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/structures/nodes.py` & `khoros-5.3.0.dev2/khoros/structures/nodes.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/studio/base.py` & `khoros-5.3.0.dev2/khoros/studio/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/core_utils.py` & `khoros-5.3.0.dev2/khoros/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/environment.py` & `khoros-5.3.0.dev2/khoros/utils/environment.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/helper.py` & `khoros-5.3.0.dev2/khoros/utils/helper.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/log_utils.py` & `khoros-5.3.0.dev2/khoros/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/resources.py` & `khoros-5.3.0.dev2/khoros/utils/tests/resources.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_albums.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_archives.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_board_creation.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_board_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_bulk_data.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_bulk_data.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_categories.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_communities.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_core_utils.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_error_handling.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_exceptions.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_grouphub_creation.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_grouphub_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_helper_file.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_helper_file.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_http_headers.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_library_import.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_library_import.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_liql.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_liql.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_mentions.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_messages.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_node_id_extract.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_node_id_extract.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_roles.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_settings.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_ssl_verify.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_ssl_verify.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_studio.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_tags.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_users.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/tests/test_version.py` & `khoros-5.3.0.dev2/khoros/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/khoros/utils/version.py` & `khoros-5.3.0.dev2/khoros/utils/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 """
 :Module:            khoros.utils.version
 :Synopsis:          This simple script contains the package version
 :Usage:             ``from .utils import version``
 :Example:           ``__version__ = version.get_full_version()``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     02 Jun 2023
+:Modified Date:     07 Jul 2023
 """
 
 import json
 import urllib.request
 
 from . import log_utils
 
 # Define special and global variables
-__version__ = "5.3.0dev1"
+__version__ = "5.3.0dev2"
 latest_version_reported = False
 logger = log_utils.initialize_logging(__name__)
 
 
 def get_full_version():
     """This function returns the current full version of the khoros package."""
     return __version__
```

### Comparing `khoros-5.3.0.dev1/khoros.egg-info/PKG-INFO` & `khoros-5.3.0.dev2/khoros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.3.0.dev1
+Version: 5.3.0.dev2
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev1 Summary: Useful tools
+Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev2 Summary: Useful tools
 and utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
```

### Comparing `khoros-5.3.0.dev1/khoros.egg-info/SOURCES.txt` & `khoros-5.3.0.dev2/khoros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev1/pyproject.toml` & `khoros-5.3.0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "khoros"
-version = "5.3.0dev1"
+version = "5.3.0dev2"
 description = "Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment."
 authors = ["Jeff Shurtliff <jeff.shurtliff@rsa.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `khoros-5.3.0.dev1/setup.py` & `khoros-5.3.0.dev2/setup.py`

 * *Files identical despite different names*

