# Comparing `tmp/nuclia-1.1.0.tar.gz` & `tmp/nuclia-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.1.0.tar", last modified: Wed Jul  5 15:13:26 2023, max compression
+gzip compressed data, was "nuclia-1.1.1.tar", last modified: Fri Jul  7 07:14:08 2023, max compression
```

## Comparing `nuclia-1.1.0.tar` & `nuclia-1.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.636134 nuclia-1.1.0/
--rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-05 15:13:25.000000 nuclia-1.1.0/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-05 15:13:25.000000 nuclia-1.1.0/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)      479 2023-07-05 15:13:25.000000 nuclia-1.1.0/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-05 15:13:25.000000 nuclia-1.1.0/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-05 15:13:25.000000 nuclia-1.1.0/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-05 15:13:25.000000 nuclia-1.1.0/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-05 15:13:26.636398 nuclia-1.1.0/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-05 15:13:25.000000 nuclia-1.1.0/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-05 15:13:25.000000 nuclia-1.1.0/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-05 15:13:25.000000 nuclia-1.1.0/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.620929 nuclia-1.1.0/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/AUTH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/CONVERSATION.md
--rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/DEFAULT.md
--rw-r--r--   0 ebr        (501) staff       (20)      648 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/SEARCH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1993 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/UPLOAD.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.622733 nuclia-1.1.0/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      303 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.626142 nuclia-1.1.0/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1280 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     2971 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.627652 nuclia-1.1.0/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)     6040 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/nua_responses.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.632790 nuclia-1.1.0/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     1341 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/nuas.py
--rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)     8910 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.635230 nuclia-1.1.0/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.635669 nuclia-1.1.0/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/fixtures.py
--rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)      682 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/test_predict.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.625066 nuclia-1.1.0/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1222 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-05 15:13:25.000000 nuclia-1.1.0/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-05 15:13:26.637172 nuclia-1.1.0/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-05 15:13:25.000000 nuclia-1.1.0/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-05 15:13:25.000000 nuclia-1.1.0/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.024874 nuclia-1.1.1/
+-rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-07 07:14:07.000000 nuclia-1.1.1/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-07 07:14:07.000000 nuclia-1.1.1/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)      545 2023-07-07 07:14:07.000000 nuclia-1.1.1/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-07 07:14:07.000000 nuclia-1.1.1/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-07 07:14:07.000000 nuclia-1.1.1/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-07 07:14:07.000000 nuclia-1.1.1/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-07 07:14:08.025019 nuclia-1.1.1/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-07 07:14:07.000000 nuclia-1.1.1/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-07 07:14:07.000000 nuclia-1.1.1/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-07 07:14:07.000000 nuclia-1.1.1/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.013309 nuclia-1.1.1/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/AUTH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/CONVERSATION.md
+-rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/DEFAULT.md
+-rw-r--r--   0 ebr        (501) staff       (20)      648 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/SEARCH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1993 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/UPLOAD.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.014692 nuclia-1.1.1/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      303 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.017279 nuclia-1.1.1/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1280 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3040 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.018792 nuclia-1.1.1/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6040 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/nua_responses.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.022465 nuclia-1.1.1/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1341 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/nuas.py
+-rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8910 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.024303 nuclia-1.1.1/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.024587 nuclia-1.1.1/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/fixtures.py
+-rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)      682 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/test_predict.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.016583 nuclia-1.1.1/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1222 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-07 07:14:07.000000 nuclia-1.1.1/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-07 07:14:08.025607 nuclia-1.1.1/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-07 07:14:07.000000 nuclia-1.1.1/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-07 07:14:07.000000 nuclia-1.1.1/test-requirements.txt
```

### Comparing `nuclia-1.1.0/LICENSE` & `nuclia-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/PKG-INFO` & `nuclia-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.0/README.md` & `nuclia-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/docs/AUTH.md` & `nuclia-1.1.1/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/docs/CONVERSATION.md` & `nuclia-1.1.1/docs/CONVERSATION.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/docs/DEFAULT.md` & `nuclia-1.1.1/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/docs/README.md` & `nuclia-1.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/docs/SEARCH.md` & `nuclia-1.1.1/docs/SEARCH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/docs/UPLOAD.md` & `nuclia-1.1.1/docs/UPLOAD.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/cli/run.py` & `nuclia-1.1.1/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/cli/utils.py` & `nuclia-1.1.1/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/config.py` & `nuclia-1.1.1/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/data.py` & `nuclia-1.1.1/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/decorators.py` & `nuclia-1.1.1/nuclia/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,16 +60,17 @@
                         environment=Environment.CLOUD,
                         url=kb_obj.url,
                         api_key=kb_obj.token,
                         region=kb_obj.region,
                     )
 
         elif url.find("nuclia.cloud") >= 0:
+            region = url.split(".")[0].split("/")[-1]
             ndb = NucliaDBClient(
-                environment=Environment.CLOUD, url=url, api_key=api_key
+                environment=Environment.CLOUD, url=url, api_key=api_key, region=region
             )
         else:
             ndb = NucliaDBClient(environment=Environment.OSS, url=url)
         kwargs["ndb"] = ndb
         return func(*args, **kwargs)
 
     return wrapper_checkout_kb
```

### Comparing `nuclia-1.1.0/nuclia/lib/kb.py` & `nuclia-1.1.1/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/lib/nua.py` & `nuclia-1.1.1/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/sdk/auth.py` & `nuclia-1.1.1/nuclia/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/sdk/kb.py` & `nuclia-1.1.1/nuclia/sdk/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/sdk/kbs.py` & `nuclia-1.1.1/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/sdk/nuas.py` & `nuclia-1.1.1/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/sdk/search.py` & `nuclia-1.1.1/nuclia/sdk/search.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/sdk/upload.py` & `nuclia-1.1.1/nuclia/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/tests/fixtures.py` & `nuclia-1.1.1/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia/tests/test_conversation.py` & `nuclia-1.1.1/nuclia/tests/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/nuclia.egg-info/PKG-INFO` & `nuclia-1.1.1/nuclia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.0/nuclia.egg-info/SOURCES.txt` & `nuclia-1.1.1/nuclia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.0/setup.py` & `nuclia-1.1.1/setup.py`

 * *Files identical despite different names*

