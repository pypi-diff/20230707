# Comparing `tmp/word-search-generator-3.4.0.tar.gz` & `tmp/word-search-generator-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "word-search-generator-3.4.0.tar", last modified: Mon Jun 26 22:02:28 2023, max compression
+gzip compressed data, was "word-search-generator-3.4.1.tar", last modified: Thu Jul  6 21:48:12 2023, max compression
```

## Comparing `word-search-generator-3.4.0.tar` & `word-search-generator-3.4.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.193896 word-search-generator-3.4.0/
--rw-r--r--   0 jbd        (501) staff       (20)       51 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/.flake8
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.178699 word-search-generator-3.4.0/.github/
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.183230 word-search-generator-3.4.0/.github/workflows/
--rw-r--r--   0 jbd        (501) staff       (20)      623 2022-10-24 16:01:30.000000 word-search-generator-3.4.0/.github/workflows/tests.yml
--rw-r--r--   0 jbd        (501) staff       (20)     1978 2023-03-13 16:13:15.000000 word-search-generator-3.4.0/.gitignore
--rw-r--r--   0 jbd        (501) staff       (20)      961 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/.pre-commit-config.yaml
--rw-r--r--   0 jbd        (501) staff       (20)    15126 2023-06-26 21:43:27.000000 word-search-generator-3.4.0/CHANGLOG.md
--rw-r--r--   0 jbd        (501) staff       (20)     1077 2021-08-08 03:10:36.000000 word-search-generator-3.4.0/LICENSE
--rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-06-26 22:02:28.193714 word-search-generator-3.4.0/PKG-INFO
--rw-r--r--   0 jbd        (501) staff       (20)     6954 2023-03-16 21:28:47.000000 word-search-generator-3.4.0/README.md
--rw-r--r--   0 jbd        (501) staff       (20)      514 2023-06-03 05:23:36.000000 word-search-generator-3.4.0/TODO.md
--rw-r--r--   0 jbd        (501) staff       (20)     2650 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/pyproject.toml
--rw-r--r--   0 jbd        (501) staff       (20)      157 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/requirements-dev.txt
--rw-r--r--   0 jbd        (501) staff       (20)       38 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/requirements.txt
--rwxr--r--   0 jbd        (501) staff       (20)     1384 2023-05-11 17:36:26.000000 word-search-generator-3.4.0/run
--rw-r--r--   0 jbd        (501) staff       (20)       38 2023-06-26 22:02:28.193939 word-search-generator-3.4.0/setup.cfg
--rw-r--r--   0 jbd        (501) staff       (20)       38 2021-09-14 03:36:29.000000 word-search-generator-3.4.0/setup.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.178901 word-search-generator-3.4.0/src/
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.185405 word-search-generator-3.4.0/src/word_search_generator/
--rw-r--r--   0 jbd        (501) staff       (20)    22392 2023-06-26 21:44:11.000000 word-search-generator-3.4.0/src/word_search_generator/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)      119 2022-11-29 21:17:05.000000 word-search-generator-3.4.0/src/word_search_generator/__main__.py
--rw-r--r--   0 jbd        (501) staff       (20)     8004 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/src/word_search_generator/cli.py
--rw-r--r--   0 jbd        (501) staff       (20)     1547 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/src/word_search_generator/config.py
--rw-r--r--   0 jbd        (501) staff       (20)     6360 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/src/word_search_generator/export.py
--rw-r--r--   0 jbd        (501) staff       (20)     7889 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/src/word_search_generator/generate.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.188415 word-search-generator-3.4.0/src/word_search_generator/mask/
--rw-r--r--   0 jbd        (501) staff       (20)    11610 2023-03-13 18:38:34.000000 word-search-generator-3.4.0/src/word_search_generator/mask/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)     4202 2023-03-13 18:38:37.000000 word-search-generator-3.4.0/src/word_search_generator/mask/bitmap.py
--rw-r--r--   0 jbd        (501) staff       (20)     3694 2023-03-13 18:39:21.000000 word-search-generator-3.4.0/src/word_search_generator/mask/ellipse.py
--rw-r--r--   0 jbd        (501) staff       (20)    14385 2023-03-14 02:51:02.000000 word-search-generator-3.4.0/src/word_search_generator/mask/polygon.py
--rw-r--r--   0 jbd        (501) staff       (20)    13001 2023-06-03 04:37:19.000000 word-search-generator-3.4.0/src/word_search_generator/mask/shapes.py
--rw-r--r--   0 jbd        (501) staff       (20)        0 2021-09-14 03:56:24.000000 word-search-generator-3.4.0/src/word_search_generator/py.typed
--rw-r--r--   0 jbd        (501) staff       (20)    24390 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/src/word_search_generator/utils.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.188784 word-search-generator-3.4.0/src/word_search_generator/word/
--rw-r--r--   0 jbd        (501) staff       (20)     6881 2023-06-03 04:16:37.000000 word-search-generator-3.4.0/src/word_search_generator/word/__init__.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.186834 word-search-generator-3.4.0/src/word_search_generator.egg-info/
--rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/PKG-INFO
--rw-r--r--   0 jbd        (501) staff       (20)     1450 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/SOURCES.txt
--rw-r--r--   0 jbd        (501) staff       (20)        1 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/dependency_links.txt
--rw-r--r--   0 jbd        (501) staff       (20)       63 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/entry_points.txt
--rw-r--r--   0 jbd        (501) staff       (20)      180 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/requires.txt
--rw-r--r--   0 jbd        (501) staff       (20)       22 2023-06-26 22:02:28.000000 word-search-generator-3.4.0/src/word_search_generator.egg-info/top_level.txt
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.191289 word-search-generator-3.4.0/tests/
--rw-r--r--   0 jbd        (501) staff       (20)    15028 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/tests/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)    15204 2023-03-16 18:23:55.000000 word-search-generator-3.4.0/tests/test_Mask.py
--rw-r--r--   0 jbd        (501) staff       (20)     1188 2022-12-01 03:07:29.000000 word-search-generator-3.4.0/tests/test_Word.py
--rw-r--r--   0 jbd        (501) staff       (20)    13819 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/tests/test_WordSearch.py
--rw-r--r--   0 jbd        (501) staff       (20)     5897 2023-06-26 21:42:46.000000 word-search-generator-3.4.0/tests/test_cli.py
--rw-r--r--   0 jbd        (501) staff       (20)     8797 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/tests/test_export.py
--rw-r--r--   0 jbd        (501) staff       (20)     2932 2023-06-15 03:54:37.000000 word-search-generator-3.4.0/tests/test_generate.py
--rw-r--r--   0 jbd        (501) staff       (20)     1317 2023-03-16 18:06:21.000000 word-search-generator-3.4.0/tests/test_shapes.py
--rw-r--r--   0 jbd        (501) staff       (20)     2392 2022-12-31 04:21:53.000000 word-search-generator-3.4.0/tests/test_utils.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.191771 word-search-generator-3.4.0/tools/
--rw-r--r--   0 jbd        (501) staff       (20)      385 2023-03-16 18:09:17.000000 word-search-generator-3.4.0/tools/build_masks_output_dict.py
--rw-r--r--   0 jbd        (501) staff       (20)     1125 2023-01-03 03:25:46.000000 word-search-generator-3.4.0/tools/pdf_layout_testing.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-06-26 22:02:28.193327 word-search-generator-3.4.0/tools/sample_word_lists/
--rw-r--r--   0 jbd        (501) staff       (20)       76 2021-08-12 01:43:53.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-10.txt
--rw-r--r--   0 jbd        (501) staff       (20)      173 2021-08-12 01:42:41.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-25.txt
--rw-r--r--   0 jbd        (501) staff       (20)       43 2021-08-12 01:41:55.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-5.txt
--rw-r--r--   0 jbd        (501) staff       (20)      369 2021-08-12 01:43:03.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-50.txt
--rw-r--r--   0 jbd        (501) staff       (20)       83 2021-08-12 02:00:51.000000 word-search-generator-3.4.0/tools/sample_word_lists/words-junk.txt
--rw-r--r--   0 jbd        (501) staff       (20)      523 2023-03-06 05:02:24.000000 word-search-generator-3.4.0/tox.ini
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.166936 word-search-generator-3.4.1/
+-rw-r--r--   0 jbd        (501) staff       (20)       51 2023-03-06 05:02:24.000000 word-search-generator-3.4.1/.flake8
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.157366 word-search-generator-3.4.1/.github/
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.160375 word-search-generator-3.4.1/.github/workflows/
+-rw-r--r--   0 jbd        (501) staff       (20)      623 2022-10-24 16:01:30.000000 word-search-generator-3.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 jbd        (501) staff       (20)     1978 2023-03-13 16:13:15.000000 word-search-generator-3.4.1/.gitignore
+-rw-r--r--   0 jbd        (501) staff       (20)      961 2023-03-06 05:02:24.000000 word-search-generator-3.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 jbd        (501) staff       (20)    15190 2023-07-06 21:45:29.000000 word-search-generator-3.4.1/CHANGLOG.md
+-rw-r--r--   0 jbd        (501) staff       (20)     1077 2021-08-08 03:10:36.000000 word-search-generator-3.4.1/LICENSE
+-rw-r--r--   0 jbd        (501) staff       (20)     8294 2023-07-06 21:48:12.166741 word-search-generator-3.4.1/PKG-INFO
+-rw-r--r--   0 jbd        (501) staff       (20)     6954 2023-03-16 21:28:47.000000 word-search-generator-3.4.1/README.md
+-rw-r--r--   0 jbd        (501) staff       (20)      514 2023-06-03 05:23:36.000000 word-search-generator-3.4.1/TODO.md
+-rw-r--r--   0 jbd        (501) staff       (20)     2877 2023-07-06 21:47:07.000000 word-search-generator-3.4.1/pyproject.toml
+-rw-r--r--   0 jbd        (501) staff       (20)      157 2023-07-06 17:46:20.000000 word-search-generator-3.4.1/requirements-dev.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2023-07-06 17:46:20.000000 word-search-generator-3.4.1/requirements.txt
+-rwxr--r--   0 jbd        (501) staff       (20)     1384 2023-05-11 17:36:26.000000 word-search-generator-3.4.1/run
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2023-07-06 21:48:12.166977 word-search-generator-3.4.1/setup.cfg
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2021-09-14 03:36:29.000000 word-search-generator-3.4.1/setup.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.157570 word-search-generator-3.4.1/src/
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.161746 word-search-generator-3.4.1/src/word_search_generator/
+-rw-r--r--   0 jbd        (501) staff       (20)    22392 2023-07-06 21:44:32.000000 word-search-generator-3.4.1/src/word_search_generator/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)      119 2022-11-29 21:17:05.000000 word-search-generator-3.4.1/src/word_search_generator/__main__.py
+-rw-r--r--   0 jbd        (501) staff       (20)     8004 2023-07-06 17:46:20.000000 word-search-generator-3.4.1/src/word_search_generator/cli.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1547 2023-06-15 03:54:37.000000 word-search-generator-3.4.1/src/word_search_generator/config.py
+-rw-r--r--   0 jbd        (501) staff       (20)     6519 2023-07-06 21:34:53.000000 word-search-generator-3.4.1/src/word_search_generator/export.py
+-rw-r--r--   0 jbd        (501) staff       (20)     7889 2023-06-15 03:54:37.000000 word-search-generator-3.4.1/src/word_search_generator/generate.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.163833 word-search-generator-3.4.1/src/word_search_generator/mask/
+-rw-r--r--   0 jbd        (501) staff       (20)    11610 2023-03-13 18:38:34.000000 word-search-generator-3.4.1/src/word_search_generator/mask/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)     4202 2023-03-13 18:38:37.000000 word-search-generator-3.4.1/src/word_search_generator/mask/bitmap.py
+-rw-r--r--   0 jbd        (501) staff       (20)     3694 2023-03-13 18:39:21.000000 word-search-generator-3.4.1/src/word_search_generator/mask/ellipse.py
+-rw-r--r--   0 jbd        (501) staff       (20)    14385 2023-03-14 02:51:02.000000 word-search-generator-3.4.1/src/word_search_generator/mask/polygon.py
+-rw-r--r--   0 jbd        (501) staff       (20)    13001 2023-06-03 04:37:19.000000 word-search-generator-3.4.1/src/word_search_generator/mask/shapes.py
+-rw-r--r--   0 jbd        (501) staff       (20)        0 2021-09-14 03:56:24.000000 word-search-generator-3.4.1/src/word_search_generator/py.typed
+-rw-r--r--   0 jbd        (501) staff       (20)    24390 2023-07-06 18:16:15.000000 word-search-generator-3.4.1/src/word_search_generator/utils.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.163962 word-search-generator-3.4.1/src/word_search_generator/word/
+-rw-r--r--   0 jbd        (501) staff       (20)     6881 2023-06-03 04:16:37.000000 word-search-generator-3.4.1/src/word_search_generator/word/__init__.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.162705 word-search-generator-3.4.1/src/word_search_generator.egg-info/
+-rw-r--r--   0 jbd        (501) staff       (20)     8294 2023-07-06 21:48:12.000000 word-search-generator-3.4.1/src/word_search_generator.egg-info/PKG-INFO
+-rw-r--r--   0 jbd        (501) staff       (20)     1450 2023-07-06 21:48:12.000000 word-search-generator-3.4.1/src/word_search_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 jbd        (501) staff       (20)        1 2023-07-06 21:48:12.000000 word-search-generator-3.4.1/src/word_search_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       63 2023-07-06 21:48:12.000000 word-search-generator-3.4.1/src/word_search_generator.egg-info/entry_points.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      180 2023-07-06 21:48:12.000000 word-search-generator-3.4.1/src/word_search_generator.egg-info/requires.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       22 2023-07-06 21:48:12.000000 word-search-generator-3.4.1/src/word_search_generator.egg-info/top_level.txt
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.165025 word-search-generator-3.4.1/tests/
+-rw-r--r--   0 jbd        (501) staff       (20)    15028 2023-06-15 03:54:37.000000 word-search-generator-3.4.1/tests/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)    15204 2023-03-16 18:23:55.000000 word-search-generator-3.4.1/tests/test_Mask.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1188 2022-12-01 03:07:29.000000 word-search-generator-3.4.1/tests/test_Word.py
+-rw-r--r--   0 jbd        (501) staff       (20)    13819 2023-06-15 03:54:37.000000 word-search-generator-3.4.1/tests/test_WordSearch.py
+-rw-r--r--   0 jbd        (501) staff       (20)     5897 2023-07-06 17:46:20.000000 word-search-generator-3.4.1/tests/test_cli.py
+-rw-r--r--   0 jbd        (501) staff       (20)     8797 2023-03-06 05:02:24.000000 word-search-generator-3.4.1/tests/test_export.py
+-rw-r--r--   0 jbd        (501) staff       (20)     2932 2023-06-15 03:54:37.000000 word-search-generator-3.4.1/tests/test_generate.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1317 2023-03-16 18:06:21.000000 word-search-generator-3.4.1/tests/test_shapes.py
+-rw-r--r--   0 jbd        (501) staff       (20)     2392 2022-12-31 04:21:53.000000 word-search-generator-3.4.1/tests/test_utils.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.165246 word-search-generator-3.4.1/tools/
+-rw-r--r--   0 jbd        (501) staff       (20)      385 2023-03-16 18:09:17.000000 word-search-generator-3.4.1/tools/build_masks_output_dict.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1125 2023-01-03 03:25:46.000000 word-search-generator-3.4.1/tools/pdf_layout_testing.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-07-06 21:48:12.166388 word-search-generator-3.4.1/tools/sample_word_lists/
+-rw-r--r--   0 jbd        (501) staff       (20)       76 2021-08-12 01:43:53.000000 word-search-generator-3.4.1/tools/sample_word_lists/words-10.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      173 2021-08-12 01:42:41.000000 word-search-generator-3.4.1/tools/sample_word_lists/words-25.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       43 2021-08-12 01:41:55.000000 word-search-generator-3.4.1/tools/sample_word_lists/words-5.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      369 2021-08-12 01:43:03.000000 word-search-generator-3.4.1/tools/sample_word_lists/words-50.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       83 2021-08-12 02:00:51.000000 word-search-generator-3.4.1/tools/sample_word_lists/words-junk.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      523 2023-03-06 05:02:24.000000 word-search-generator-3.4.1/tox.ini
```

### Comparing `word-search-generator-3.4.0/.github/workflows/tests.yml` & `word-search-generator-3.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/.gitignore` & `word-search-generator-3.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/.pre-commit-config.yaml` & `word-search-generator-3.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/CHANGLOG.md` & `word-search-generator-3.4.1/CHANGLOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.4.1]
+
+### Fixed
+- Solution highlighting on exported PDFs
+
 ## [3.4.0]
 
 ### Fixed
 - `Word.offset_coordinates()`
 - Secret words correctly obey their directional constraints (by duck57). Fixes issue #42.
 
 ### Changed
```

### Comparing `word-search-generator-3.4.0/LICENSE` & `word-search-generator-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/PKG-INFO` & `word-search-generator-3.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: word-search-generator
-Version: 3.4.0
+Version: 3.4.1
 Summary: Make awesome Word Search puzzles
 Author-email: Josh Duncan <joshbduncan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/joshbduncan/word-search-generator
 Project-URL: documentation, https://github.com/joshbduncan/word-search-generator/wiki
 Project-URL: repository, https://github.com/joshbduncan/word-search-generator.git
 Project-URL: changelog, https://github.com/joshbduncan/word-search-generator/blob/main/CHANGLOG.md
@@ -12,14 +12,19 @@
 Keywords: puzzles,games,word-search
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `word-search-generator-3.4.0/README.md` & `word-search-generator-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/TODO.md` & `word-search-generator-3.4.1/TODO.md`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/pyproject.toml` & `word-search-generator-3.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 classifiers = [
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Games/Entertainment :: Puzzle Games",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = [
     "fpdf2==2.4.2",
     "typing_extensions==4.4.0",
 ]
 dynamic = ["version"]
```

### Comparing `word-search-generator-3.4.0/run` & `word-search-generator-3.4.1/run`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/__init__.py` & `word-search-generator-3.4.1/src/word_search_generator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Generate Word Search puzzles with Python.
     -----------
     :copyright: (c) 2021 Josh Duncan.
     :license: MIT, see LICENSE for more details.
 """
 
 __app_name__ = "word-search"
-__version__ = "3.4.0"
+__version__ = "3.4.1"
 
 
 import json
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Set
 
 from . import export, generate, utils
```

### Comparing `word-search-generator-3.4.0/src/word_search_generator/cli.py` & `word-search-generator-3.4.1/src/word_search_generator/cli.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/config.py` & `word-search-generator-3.4.1/src/word_search_generator/config.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/export.py` & `word-search-generator-3.4.1/src/word_search_generator/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,25 +139,29 @@
     # to ensure all words and the puzzle key fit on one page
     info_font_size = config.pdf_font_size_XL - (
         len(ws.words) - config.min_puzzle_words
     ) * (6 / (config.max_puzzle_words - config.min_puzzle_words))
     pdf.set_font_size(font_size)
 
     # draw the puzzle
-    placed_words_coordinates = {
-        coord
-        for coords in [
-            word.offset_coordinates(ws.bounding_box) for word in ws.placed_words
-        ]
-        for coord in coords  # type: ignore
-    }  # type: ignore
-    for r, row in enumerate(ws.cropped_puzzle):
-        for c, char in enumerate(row):
+    if solution:
+        placed_words_coordinates = {
+            coord
+            for coords in [
+                word.offset_coordinates(ws.bounding_box) for word in ws.placed_words
+            ]
+            for coord in coords  # type: ignore
+        }  # type: ignore
+    else:
+        placed_words_coordinates = {}  # type: ignore
+    print(f"{placed_words_coordinates=}")
+    for y, row in enumerate(ws.cropped_puzzle):
+        for x, char in enumerate(row):
             # draw a border around correct letters if solution was requested
-            if solution and (r, c) in placed_words_coordinates:
+            if solution and (x + 1, y + 1) in placed_words_coordinates:
                 pdf.set_text_color(255, 0, 0)
                 pdf.multi_cell(gsize, gsize, char, align="C", ln=3)
                 pdf.set_text_color(0, 0, 0)
             else:
                 pdf.multi_cell(gsize, gsize, char, align="C", ln=3)
         pdf.ln(gsize)
     pdf.ln(0.25)
```

### Comparing `word-search-generator-3.4.0/src/word_search_generator/generate.py` & `word-search-generator-3.4.1/src/word_search_generator/generate.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/mask/__init__.py` & `word-search-generator-3.4.1/src/word_search_generator/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/mask/bitmap.py` & `word-search-generator-3.4.1/src/word_search_generator/mask/bitmap.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/mask/ellipse.py` & `word-search-generator-3.4.1/src/word_search_generator/mask/ellipse.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/mask/polygon.py` & `word-search-generator-3.4.1/src/word_search_generator/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/mask/shapes.py` & `word-search-generator-3.4.1/src/word_search_generator/mask/shapes.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/utils.py` & `word-search-generator-3.4.1/src/word_search_generator/utils.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator/word/__init__.py` & `word-search-generator-3.4.1/src/word_search_generator/word/__init__.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/src/word_search_generator.egg-info/PKG-INFO` & `word-search-generator-3.4.1/src/word_search_generator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: word-search-generator
-Version: 3.4.0
+Version: 3.4.1
 Summary: Make awesome Word Search puzzles
 Author-email: Josh Duncan <joshbduncan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/joshbduncan/word-search-generator
 Project-URL: documentation, https://github.com/joshbduncan/word-search-generator/wiki
 Project-URL: repository, https://github.com/joshbduncan/word-search-generator.git
 Project-URL: changelog, https://github.com/joshbduncan/word-search-generator/blob/main/CHANGLOG.md
@@ -12,14 +12,19 @@
 Keywords: puzzles,games,word-search
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `word-search-generator-3.4.0/src/word_search_generator.egg-info/SOURCES.txt` & `word-search-generator-3.4.1/src/word_search_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/__init__.py` & `word-search-generator-3.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_Mask.py` & `word-search-generator-3.4.1/tests/test_Mask.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_Word.py` & `word-search-generator-3.4.1/tests/test_Word.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_WordSearch.py` & `word-search-generator-3.4.1/tests/test_WordSearch.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_cli.py` & `word-search-generator-3.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_export.py` & `word-search-generator-3.4.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_generate.py` & `word-search-generator-3.4.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_shapes.py` & `word-search-generator-3.4.1/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tests/test_utils.py` & `word-search-generator-3.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tools/pdf_layout_testing.py` & `word-search-generator-3.4.1/tools/pdf_layout_testing.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.4.0/tox.ini` & `word-search-generator-3.4.1/tox.ini`

 * *Files identical despite different names*

