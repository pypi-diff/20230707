# Comparing `tmp/mxmake-1.0a1.tar.gz` & `tmp/mxmake-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxmake-1.0a1.tar", last modified: Fri May  5 06:49:45 2023, max compression
+gzip compressed data, was "mxmake-1.0a2.tar", last modified: Fri Jul  7 08:49:19 2023, max compression
```

## Comparing `mxmake-1.0a1.tar` & `mxmake-1.0a2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3155 2023-05-05 06:46:53.000000 mxmake-1.0a1/CHANGES.md
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1320 2023-01-31 23:41:42.000000 mxmake-1.0a1/LICENSE.md
--rw-r--r--   0 rnix      (1000) rnix      (1000)      133 2023-05-05 06:46:08.000000 mxmake-1.0a1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7066 2023-05-05 06:49:45.769435 mxmake-1.0a1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1359 2023-01-31 23:41:42.000000 mxmake-1.0a1/README.md
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2254 2023-05-05 06:46:28.000000 mxmake-1.0a1/pyproject.toml
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-05 06:49:45.769435 mxmake-1.0a1/setup.cfg
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/
--rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2022-05-19 08:58:33.000000 mxmake-1.0a1/src/mxmake/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2131 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/hook.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7162 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/main.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2200 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/parser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1410 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/sphinxext.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/templates/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2057 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/templates/Makefile
--rw-r--r--   0 rnix      (1000) rnix      (1000)       82 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/templates/additional_sources_targets.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)      521 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/templates/dependencies.md
--rw-r--r--   0 rnix      (1000) rnix      (1000)      389 2022-06-10 06:32:06.000000 mxmake-1.0a1/src/mxmake/templates/env.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      380 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/templates/mx.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/pytest-run-coverage.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      180 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/pytest-run-tests.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      173 2022-05-19 09:05:03.000000 mxmake-1.0a1/src/mxmake/templates/script.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      843 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/templates/topics.md
--rw-r--r--   0 rnix      (1000) rnix      (1000)      677 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/zope-testrunner-run-coverage.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      212 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/zope-testrunner-run-tests.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12231 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2759 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/testing/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      745 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      687 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/test_hook.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2619 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/tests/test_parser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    26046 2023-05-05 06:23:39.000000 mxmake-1.0a1/src/mxmake/tests/test_templates.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11073 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/test_topics.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      953 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/test_utils.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/topics/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/applications/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1083 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/applications/cookiecutter.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)       76 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/topics/applications/metadata.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1177 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/topics/applications/twisted.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1969 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/applications/zest-releaser.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3362 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/applications/zope.mk
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/core/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2048 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/core/base.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/core/metadata.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3537 2023-05-05 06:20:53.000000 mxmake-1.0a1/src/mxmake/topics/core/mxenv.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1960 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/core/mxfiles.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1407 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/core/packages.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)      994 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/core/sources.mk
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/docs/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      910 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/topics/docs/jsdoc.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/docs/metadata.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1839 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/topics/docs/sphinx.mk
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/i18n/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2106 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/i18n/gettext.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1525 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/i18n/lingua.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)       83 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/i18n/metadata.ini
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/js/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      763 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/js/karma.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-02-06 10:28:34.000000 mxmake-1.0a1/src/mxmake/topics/js/metadata.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2351 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/js/npm.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)      666 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/js/rollup.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1084 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/topics/js/scss.mk
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/ldap/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       63 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/ldap/metadata.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2197 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/ldap/openldap.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1307 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/ldap/python-ldap.mk
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/qa/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1253 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/black.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1478 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/qa/coverage.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1251 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/isort.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)       58 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/qa/metadata.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1245 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/mypy.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1592 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/topics/qa/test.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1467 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/zpretty.mk
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/system/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      752 2023-02-06 10:28:34.000000 mxmake-1.0a1/src/mxmake/topics/system/dependencies.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)       65 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/system/metadata.ini
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9529 2023-05-05 06:05:05.000000 mxmake-1.0a1/src/mxmake/topics.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      831 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/utils.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7066 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2295 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      314 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-05-19 09:22:24.000000 mxmake-1.0a1/src/mxmake.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)      128 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        7 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/top_level.txt
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.441553 mxmake-1.0a2/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     3513 2023-07-07 08:48:48.000000 mxmake-1.0a2/CHANGES.md
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1320 2023-04-28 08:45:02.000000 mxmake-1.0a2/LICENSE.md
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      133 2023-06-14 12:27:46.000000 mxmake-1.0a2/MANIFEST.in
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     7426 2023-07-07 08:49:19.437554 mxmake-1.0a2/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1359 2023-04-28 08:45:02.000000 mxmake-1.0a2/README.md
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2254 2023-07-07 08:49:04.000000 mxmake-1.0a2/pyproject.toml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       38 2023-07-07 08:49:19.441553 mxmake-1.0a2/setup.cfg
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.429554 mxmake-1.0a2/src/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.433554 mxmake-1.0a2/src/mxmake/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2022-05-24 15:39:25.000000 mxmake-1.0a2/src/mxmake/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2269 2023-07-07 08:42:27.000000 mxmake-1.0a2/src/mxmake/hook.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     7162 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/main.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2200 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/parser.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1410 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/sphinxext.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.433554 mxmake-1.0a2/src/mxmake/templates/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2057 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/templates/Makefile
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       82 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/additional_sources_targets.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      521 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/dependencies.md
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      389 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/env.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      380 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/mx.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      111 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/templates/pip.conf
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      627 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/pytest-run-coverage.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      180 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/pytest-run-tests.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      173 2022-05-24 15:39:25.000000 mxmake-1.0a2/src/mxmake/templates/script.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      843 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/topics.md
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      677 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/zope-testrunner-run-coverage.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      212 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/templates/zope-testrunner-run-tests.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)    12947 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/templates.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.433554 mxmake-1.0a2/src/mxmake/testing/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2759 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/testing/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.433554 mxmake-1.0a2/src/mxmake/tests/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      745 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/tests/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      687 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/tests/test_hook.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2619 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/tests/test_parser.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)    27404 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/tests/test_templates.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)    11073 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/tests/test_topics.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      953 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/tests/test_utils.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.429554 mxmake-1.0a2/src/mxmake/topics/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/applications/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1083 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/applications/cookiecutter.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       76 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/applications/metadata.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1177 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/applications/twisted.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1969 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/topics/applications/zest-releaser.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     3362 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/applications/zope.mk
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/core/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2048 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/topics/core/base.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       62 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/core/metadata.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     3613 2023-07-07 08:42:27.000000 mxmake-1.0a2/src/mxmake/topics/core/mxenv.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2055 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/topics/core/mxfiles.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1407 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/core/packages.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1012 2023-07-07 08:42:27.000000 mxmake-1.0a2/src/mxmake/topics/core/sources.mk
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/docs/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      910 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/docs/jsdoc.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       62 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/docs/metadata.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1839 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/docs/sphinx.mk
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/i18n/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2122 2023-07-07 08:42:27.000000 mxmake-1.0a2/src/mxmake/topics/i18n/gettext.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1525 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/i18n/lingua.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       83 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/i18n/metadata.ini
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/js/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      763 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/js/karma.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       74 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/js/metadata.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2351 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/js/npm.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      666 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/js/rollup.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1084 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/js/scss.mk
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/ldap/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       63 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/ldap/metadata.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2197 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/topics/ldap/openldap.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1307 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/topics/ldap/python-ldap.mk
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/qa/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1253 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/qa/black.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1478 2023-06-14 12:27:46.000000 mxmake-1.0a2/src/mxmake/topics/qa/coverage.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1251 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/qa/isort.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       58 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/qa/metadata.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1245 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/qa/mypy.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1592 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/qa/test.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1467 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/qa/zpretty.mk
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.437554 mxmake-1.0a2/src/mxmake/topics/system/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      752 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/system/dependencies.mk
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       65 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics/system/metadata.ini
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     9529 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/topics.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      831 2023-04-28 08:45:02.000000 mxmake-1.0a2/src/mxmake/utils.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-07 08:49:19.433554 mxmake-1.0a2/src/mxmake.egg-info/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     7426 2023-07-07 08:49:19.000000 mxmake-1.0a2/src/mxmake.egg-info/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2325 2023-07-07 08:49:19.000000 mxmake-1.0a2/src/mxmake.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-07-07 08:49:19.000000 mxmake-1.0a2/src/mxmake.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      314 2023-07-07 08:49:19.000000 mxmake-1.0a2/src/mxmake.egg-info/entry_points.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-01-25 19:28:58.000000 mxmake-1.0a2/src/mxmake.egg-info/not-zip-safe
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      128 2023-07-07 08:49:19.000000 mxmake-1.0a2/src/mxmake.egg-info/requires.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        7 2023-07-07 08:49:19.000000 mxmake-1.0a2/src/mxmake.egg-info/top_level.txt
```

### Comparing `mxmake-1.0a1/CHANGES.md` & `mxmake-1.0a2/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 # Changelog
 
+## 1.0a2 (2023-07-07)
+
+- Add support for `pip.conf` file.
+
+- Fixes #18: VENV_CREATE is ignored.
+
+- Fix error when new source package gets added to `mx.ini` in
+  `Hook.generate_additional_sources_targets`.
+
+- Add `PROJECT_CONFIG` as the dependency target of `SOURCES_TARGET` to make
+  sure the target runs when a new source package gets added to `mx.ini`.
+
 ## 1.0a1 (2023-05-05)
 
 - Add `zest-releaser` domain to `applications` topic.
 
 - Support custom makefile include.
 
-- Support `pytest` as test runner and make it default if not configured
+- Support `pytest` as a test runner and make it default if not configured
   otherwise.
 
 - Add `RUN_TARGET` setting to `base` domain and generate `run` target in
   `Makefile`.
 
 - Create `twisted` domain in `applications` topic.
```

### Comparing `mxmake-1.0a1/LICENSE.md` & `mxmake-1.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/PKG-INFO` & `mxmake-1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mxmake
-Version: 1.0a1
+Version: 1.0a2
 Summary: Generates a Python project-specific Makefile by using an extensible library of configurable Makefile snippets.
 Author-email: MX Stack Developers <dev@bluedynamics.com>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://github.com/mxstack/mxmake
-Project-URL: Documentation, https://mxmake.readthedocs.io
+Project-URL: Documentation, https://mxstack.github.io/mxmake
 Project-URL: Bug Reports, https://github.com/mxstack/mxmake/issues
-Project-URL: Source, https://github.com/mxstack/mxmake/
+Project-URL: Source, https://github.com/mxstack/mxmake
 Keywords: development,deployment,environment
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -53,21 +53,33 @@
 Contributors
 ============
 
 - Robert Niederreiter
 - Jens Klein
 # Changelog
 
+## 1.0a2 (2023-07-07)
+
+- Add support for `pip.conf` file.
+
+- Fixes #18: VENV_CREATE is ignored.
+
+- Fix error when new source package gets added to `mx.ini` in
+  `Hook.generate_additional_sources_targets`.
+
+- Add `PROJECT_CONFIG` as the dependency target of `SOURCES_TARGET` to make
+  sure the target runs when a new source package gets added to `mx.ini`.
+
 ## 1.0a1 (2023-05-05)
 
 - Add `zest-releaser` domain to `applications` topic.
 
 - Support custom makefile include.
 
-- Support `pytest` as test runner and make it default if not configured
+- Support `pytest` as a test runner and make it default if not configured
   otherwise.
 
 - Add `RUN_TARGET` setting to `base` domain and generate `run` target in
   `Makefile`.
 
 - Create `twisted` domain in `applications` topic.
```

### Comparing `mxmake-1.0a1/README.md` & `mxmake-1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/pyproject.toml` & `mxmake-1.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "mxmake"
 description = "Generates a Python project-specific Makefile by using an extensible library of configurable Makefile snippets."
-version = "1.0a1"
+version = "1.0a2"
 keywords = ["development", "deployment", "environment"]
 authors = [
   {name = "MX Stack Developers", email = "dev@bluedynamics.com" }
 ]
 requires-python = ">=3.7"
 license = { text = "BSD 2-Clause License" }
 classifiers = [
@@ -34,17 +34,17 @@
     "types-pkg-resources",
 ]
 docs = ["Sphinx", "sphinxcontrib-mermaid"]
 test = ["zope.testrunner"]
 
 [project.urls]
 Homepage = "https://github.com/mxstack/mxmake"
-Documentation = "https://mxmake.readthedocs.io"
+Documentation = "https://mxstack.github.io/mxmake"
 "Bug Reports" = "https://github.com/mxstack/mxmake/issues"
-Source = "https://github.com/mxstack/mxmake/"
+Source = "https://github.com/mxstack/mxmake"
 
 [project.scripts]
 mxmake = "mxmake.main:main"
 
 [project.entry-points.mxdev]
 hook = "mxmake.hook:Hook"
 
@@ -82,9 +82,7 @@
 profile = "black"
 force_alphabetical_sort = true
 force_single_line = true
 lines_after_imports = 2
 
 [tool.mypy]
 ignore_missing_imports = true
-
-
```

### Comparing `mxmake-1.0a1/src/mxmake/hook.py` & `mxmake-1.0a2/src/mxmake/hook.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 
     def generate_additional_sources_targets(self, state: mxdev.State):
         config = state.configuration
         additional_sources_targets = []
         sources_folder = config.settings.get("default-target", "sources")
         for package_name in config.packages:
             source_folder = os.path.join(sources_folder, package_name)
+            # case new source package has been added to mx.ini
+            if not os.path.exists(source_folder):
+                continue
             for child in os.listdir(source_folder):
                 if child in ADDITIONAL_SOURCES_TARGETS:
                     additional_sources_targets.append(
                         os.path.join(source_folder, child)
                     )
         if not additional_sources_targets:
             return
```

### Comparing `mxmake-1.0a1/src/mxmake/main.py` & `mxmake-1.0a2/src/mxmake/main.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/parser.py` & `mxmake-1.0a2/src/mxmake/parser.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/sphinxext.py` & `mxmake-1.0a2/src/mxmake/sphinxext.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/templates/Makefile` & `mxmake-1.0a2/src/mxmake/templates/Makefile`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/templates/dependencies.md` & `mxmake-1.0a2/src/mxmake/templates/dependencies.md`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/templates/pytest-run-coverage.sh` & `mxmake-1.0a2/src/mxmake/templates/pytest-run-coverage.sh`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/templates/topics.md` & `mxmake-1.0a2/src/mxmake/templates/topics.md`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/templates/zope-testrunner-run-coverage.sh` & `mxmake-1.0a2/src/mxmake/templates/zope-testrunner-run-coverage.sh`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/templates.py` & `mxmake-1.0a2/src/mxmake/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,40 @@
         variables = super().template_variables
         variables["sourcepaths"] = self.package_paths(ns_name("source-path"))
         variables["omitpaths"] = self.package_paths(ns_name("omit-path"))
         return variables
 
 
 ##############################################################################
+# pip config template
+##############################################################################
+
+
+@template("pip-conf")
+class PipConf(MxIniBoundTemplate):
+    description: str = "Pip config"
+    target_name: str = "pip.conf"
+    template_name: str = "pip.conf"
+
+    @property
+    def target_folder(self) -> str:
+        return mxmake_files()
+
+    @property
+    def template_variables(self) -> typing.Dict[str, typing.Any]:
+        return dict(
+            find_links=[
+                link.strip()
+                for link in self.settings.get("find-links", "").split("\n")
+                if link.strip()
+            ]
+        )
+
+
+##############################################################################
 # makefile template
 ##############################################################################
 
 
 @template("makefile")
 class Makefile(Template):
     description: str = "Makefile"
```

### Comparing `mxmake-1.0a1/src/mxmake/testing/__init__.py` & `mxmake-1.0a2/src/mxmake/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/tests/__init__.py` & `mxmake-1.0a2/src/mxmake/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/tests/test_hook.py` & `mxmake-1.0a2/src/mxmake/tests/test_hook.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/tests/test_parser.py` & `mxmake-1.0a2/src/mxmake/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/tests/test_templates.py` & `mxmake-1.0a2/src/mxmake/tests/test_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.assertEqual(
             templates.template._registry,
             {
                 "additional_sources_targets": templates.AdditionalSourcesTargets,
                 "dependencies.md": templates.Dependencies,
                 "makefile": templates.Makefile,
                 "mx.ini": templates.MxIni,
+                "pip-conf": templates.PipConf,
                 "run-coverage": templates.CoverageScript,
                 "run-tests": templates.TestScript,
                 "topics.md": templates.Topics,
             },
         )
 
     @testing.template_directory()
@@ -468,14 +469,52 @@
 
                 exit 0
                 """,
                 f.read(),
             )
 
     @testing.template_directory()
+    def test_PipConf(self, tempdir):
+        config_file = io.StringIO()
+        config_file.write(
+            "[settings]\n"
+            "\n"
+            "[mxmake-pip-conf]\n"
+            "find-links =\n"
+            "    file:///path/to/folder\n"
+            "    https://tld.com/\n"
+        )
+        config_file.seek(0)
+
+        configuration = mxdev.Configuration(config_file, hooks=[hook.Hook()])
+        factory = templates.template.lookup("pip-conf")
+        template = factory(configuration, templates.get_template_environment())
+
+        self.assertEqual(template.description, "Pip config")
+        self.assertEqual(template.target_folder, utils.mxmake_files())
+        self.assertEqual(template.target_name, "pip.conf")
+        self.assertEqual(template.template_name, "pip.conf")
+        self.assertEqual(
+            template.template_variables,
+            {"find_links": ["file:///path/to/folder", "https://tld.com/"]},
+        )
+
+        template.write()
+        with open(os.path.join(tempdir, "pip.conf")) as f:
+            self.checkOutput(
+                """
+                [global]
+                find-links =
+                    file:///path/to/folder
+                    https://tld.com/
+                """,
+                f.read(),
+            )
+
+    @testing.template_directory()
     def test_AdditionalSourcesTargets(self, tempdir):
         factory = templates.template.lookup("additional_sources_targets")
         template = factory(["a", "b"], templates.get_template_environment())
         template.write()
 
         path = os.path.join(tempdir, "additional_sources_targets.mk")
         with open(path) as f:
```

### Comparing `mxmake-1.0a1/src/mxmake/tests/test_topics.py` & `mxmake-1.0a2/src/mxmake/tests/test_topics.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/tests/test_utils.py` & `mxmake-1.0a2/src/mxmake/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/applications/cookiecutter.mk` & `mxmake-1.0a2/src/mxmake/topics/applications/cookiecutter.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/applications/twisted.mk` & `mxmake-1.0a2/src/mxmake/topics/applications/twisted.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/applications/zest-releaser.mk` & `mxmake-1.0a2/src/mxmake/topics/applications/zest-releaser.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/applications/zope.mk` & `mxmake-1.0a2/src/mxmake/topics/applications/zope.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/core/base.mk` & `mxmake-1.0a2/src/mxmake/topics/core/base.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/core/mxenv.mk` & `mxmake-1.0a2/src/mxmake/topics/core/mxenv.mk`

 * *Files 4% similar despite different names*

```diff
@@ -82,17 +82,19 @@
 else
 MXENV_PATH=
 endif
 
 MXENV_TARGET:=$(SENTINEL_FOLDER)/mxenv.sentinel
 $(MXENV_TARGET): $(SENTINEL)
 ifeq ("$(VENV_ENABLED)", "true")
+ifeq ("$(VENV_CREATE)", "true")
 	@echo "Setup Python Virtual Environment under '$(VENV_FOLDER)'"
 	@$(PYTHON_BIN) -m venv $(VENV_FOLDER)
 endif
+endif
 	@$(MXENV_PATH)pip install -U pip setuptools wheel
 	@$(MXENV_PATH)pip install -U $(MXDEV)
 	@$(MXENV_PATH)pip install -U $(MXMAKE)
 	@touch $(MXENV_TARGET)
 
 .PHONY: mxenv
 mxenv: $(MXENV_TARGET)
@@ -100,15 +102,17 @@
 .PHONY: mxenv-dirty
 mxenv-dirty:
 	@rm -f $(MXENV_TARGET)
 
 .PHONY: mxenv-clean
 mxenv-clean: mxenv-dirty
 ifeq ("$(VENV_ENABLED)", "true")
+ifeq ("$(VENV_CREATE)", "true")
 	@rm -rf $(VENV_FOLDER)
+endif
 else
 	@$(MXENV_PATH)pip uninstall -y $(MXDEV)
 	@$(MXENV_PATH)pip uninstall -y $(MXMAKE)
 endif
 
 INSTALL_TARGETS+=mxenv
 DIRTY_TARGETS+=mxenv-dirty
```

### Comparing `mxmake-1.0a1/src/mxmake/topics/core/mxfiles.mk` & `mxmake-1.0a2/src/mxmake/topics/core/mxfiles.mk`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 FILES_TARGET:=requirements-mxdev.txt
 $(FILES_TARGET): $(PROJECT_CONFIG) $(MXENV_TARGET) $(SOURCES_TARGET) $(LOCAL_PACKAGE_FILES)
 	@echo "Create project files"
 	@mkdir -p $(MXMAKE_FILES)
 	$(call set_mxfiles_env,$(MXENV_PATH),$(MXMAKE_FILES))
 	@$(MXENV_PATH)mxdev -n -c $(PROJECT_CONFIG)
 	$(call unset_mxfiles_env,$(MXENV_PATH),$(MXMAKE_FILES))
+	@test -e $(MXMAKE_FILES)/pip.conf && cp $(MXMAKE_FILES)/pip.conf $(VENV_FOLDER)/pip.conf || :
 	@touch $(FILES_TARGET)
 
 .PHONY: mxfiles
 mxfiles: $(FILES_TARGET)
 
 .PHONY: mxfiles-dirty
 mxfiles-dirty:
```

### Comparing `mxmake-1.0a1/src/mxmake/topics/core/packages.mk` & `mxmake-1.0a2/src/mxmake/topics/core/packages.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/core/sources.mk` & `mxmake-1.0a2/src/mxmake/topics/core/sources.mk`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #:description = Removes sources folder.
 
 ##############################################################################
 # sources
 ##############################################################################
 
 SOURCES_TARGET:=$(SENTINEL_FOLDER)/sources.sentinel
-$(SOURCES_TARGET): $(MXENV_TARGET)
+$(SOURCES_TARGET): $(PROJECT_CONFIG) $(MXENV_TARGET)
 	@echo "Checkout project sources"
 	@$(MXENV_PATH)mxdev -o -c $(PROJECT_CONFIG)
 	@touch $(SOURCES_TARGET)
 
 .PHONY: sources
 sources: $(SOURCES_TARGET)
```

### Comparing `mxmake-1.0a1/src/mxmake/topics/docs/jsdoc.mk` & `mxmake-1.0a2/src/mxmake/topics/docs/jsdoc.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/docs/sphinx.mk` & `mxmake-1.0a2/src/mxmake/topics/docs/sphinx.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/i18n/gettext.mk` & `mxmake-1.0a2/src/mxmake/topics/i18n/gettext.mk`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #:default = locale
 #:
 #:[setting.GETTEXT_DOMAIN]
 #:description = Translation domain to use.
 #:default =
 #:
 #:[setting.GETTEXT_LANGUAGES]
-#:description = List of language identifiers.
+#:description = Space separated list of language identifiers.
 #:default =
 
 ##############################################################################
 # gettext
 ##############################################################################
 
 # case `system.dependencies` domain is included
```

### Comparing `mxmake-1.0a1/src/mxmake/topics/i18n/lingua.mk` & `mxmake-1.0a2/src/mxmake/topics/i18n/lingua.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/js/karma.mk` & `mxmake-1.0a2/src/mxmake/topics/js/karma.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/js/npm.mk` & `mxmake-1.0a2/src/mxmake/topics/js/npm.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/js/rollup.mk` & `mxmake-1.0a2/src/mxmake/topics/js/rollup.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/js/scss.mk` & `mxmake-1.0a2/src/mxmake/topics/js/scss.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/ldap/openldap.mk` & `mxmake-1.0a2/src/mxmake/topics/ldap/openldap.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/ldap/python-ldap.mk` & `mxmake-1.0a2/src/mxmake/topics/ldap/python-ldap.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/qa/black.mk` & `mxmake-1.0a2/src/mxmake/topics/qa/black.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/qa/coverage.mk` & `mxmake-1.0a2/src/mxmake/topics/qa/coverage.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/qa/isort.mk` & `mxmake-1.0a2/src/mxmake/topics/qa/isort.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/qa/mypy.mk` & `mxmake-1.0a2/src/mxmake/topics/qa/mypy.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/qa/test.mk` & `mxmake-1.0a2/src/mxmake/topics/qa/test.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/qa/zpretty.mk` & `mxmake-1.0a2/src/mxmake/topics/qa/zpretty.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics/system/dependencies.mk` & `mxmake-1.0a2/src/mxmake/topics/system/dependencies.mk`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/topics.py` & `mxmake-1.0a2/src/mxmake/topics.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake/utils.py` & `mxmake-1.0a2/src/mxmake/utils.py`

 * *Files identical despite different names*

### Comparing `mxmake-1.0a1/src/mxmake.egg-info/PKG-INFO` & `mxmake-1.0a2/src/mxmake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mxmake
-Version: 1.0a1
+Version: 1.0a2
 Summary: Generates a Python project-specific Makefile by using an extensible library of configurable Makefile snippets.
 Author-email: MX Stack Developers <dev@bluedynamics.com>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://github.com/mxstack/mxmake
-Project-URL: Documentation, https://mxmake.readthedocs.io
+Project-URL: Documentation, https://mxstack.github.io/mxmake
 Project-URL: Bug Reports, https://github.com/mxstack/mxmake/issues
-Project-URL: Source, https://github.com/mxstack/mxmake/
+Project-URL: Source, https://github.com/mxstack/mxmake
 Keywords: development,deployment,environment
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -53,21 +53,33 @@
 Contributors
 ============
 
 - Robert Niederreiter
 - Jens Klein
 # Changelog
 
+## 1.0a2 (2023-07-07)
+
+- Add support for `pip.conf` file.
+
+- Fixes #18: VENV_CREATE is ignored.
+
+- Fix error when new source package gets added to `mx.ini` in
+  `Hook.generate_additional_sources_targets`.
+
+- Add `PROJECT_CONFIG` as the dependency target of `SOURCES_TARGET` to make
+  sure the target runs when a new source package gets added to `mx.ini`.
+
 ## 1.0a1 (2023-05-05)
 
 - Add `zest-releaser` domain to `applications` topic.
 
 - Support custom makefile include.
 
-- Support `pytest` as test runner and make it default if not configured
+- Support `pytest` as a test runner and make it default if not configured
   otherwise.
 
 - Add `RUN_TARGET` setting to `base` domain and generate `run` target in
   `Makefile`.
 
 - Create `twisted` domain in `applications` topic.
```

### Comparing `mxmake-1.0a1/src/mxmake.egg-info/SOURCES.txt` & `mxmake-1.0a2/src/mxmake.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/mxmake.egg-info/requires.txt
 src/mxmake.egg-info/top_level.txt
 src/mxmake/templates/Makefile
 src/mxmake/templates/additional_sources_targets.mk
 src/mxmake/templates/dependencies.md
 src/mxmake/templates/env.sh
 src/mxmake/templates/mx.ini
+src/mxmake/templates/pip.conf
 src/mxmake/templates/pytest-run-coverage.sh
 src/mxmake/templates/pytest-run-tests.sh
 src/mxmake/templates/script.sh
 src/mxmake/templates/topics.md
 src/mxmake/templates/zope-testrunner-run-coverage.sh
 src/mxmake/templates/zope-testrunner-run-tests.sh
 src/mxmake/testing/__init__.py
```

