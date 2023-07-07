# Comparing `tmp/intake-esm-2023.6.14.tar.gz` & `tmp/intake-esm-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-esm-2023.6.14.tar", last modified: Wed Jun 14 13:17:29 2023, max compression
+gzip compressed data, was "intake-esm-2023.7.7.tar", last modified: Fri Jul  7 12:55:29 2023, max compression
```

## Comparing `intake-esm-2023.6.14.tar` & `intake-esm-2023.7.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.023198 intake-esm-2023.6.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.011198 intake-esm-2023.6.14/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.015198 intake-esm-2023.6.14/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.015198 intake-esm-2023.6.14/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/.prettierrc.toml
--rw-r--r--   0 runner    (1001) docker     (123)    51400 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-14 13:17:29.023198 intake-esm-2023.6.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.015198 intake-esm-2023.6.14/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.003198 intake-esm-2023.6.14/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.015198 intake-esm-2023.6.14/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    22404 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/_static/images/NSF_4-Color_bitmap_Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/_static/images/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.015198 intake-esm-2023.6.14/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/catalogs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.019198 intake-esm-2023.6.14/docs/source/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/build-a-catalog-from-timeseries-files.md
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/define-and-use-derived-variable-registry.md
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/install-intake-esm.md
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/modify-catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/multi-variable-catalog.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/multi-variable-catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/understand-keys-and-how-to-change-them.md
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.019198 intake-esm-2023.6.14/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/reference/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/reference/cmip_ap.md
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/reference/esm-catalog-spec.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/reference/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.019198 intake-esm-2023.6.14/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/docs/source/tutorials/loading-cmip6-data.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.023198 intake-esm-2023.6.14/intake_esm/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15495 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    33791 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/intake_esm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.023198 intake-esm-2023.6.14/intake_esm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-14 13:17:28.000000 intake-esm-2023.6.14/intake_esm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-14 13:17:28.000000 intake-esm-2023.6.14/intake_esm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:17:28.000000 intake-esm-2023.6.14/intake_esm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 13:17:28.000000 intake-esm-2023.6.14/intake_esm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:17:28.000000 intake-esm-2023.6.14/intake_esm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 13:17:28.000000 intake-esm-2023.6.14/intake_esm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 13:17:28.000000 intake-esm-2023.6.14/intake_esm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:17:29.023198 intake-esm-2023.6.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:17:29.023198 intake-esm-2023.6.14/tutorial-catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/tutorial-catalogs/AWS-CESM2-LENS.json
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/tutorial-catalogs/AWS-CMIP6.json
--rw-r--r--   0 runner    (1001) docker     (123)   108734 2023-06-14 13:17:08.000000 intake-esm-2023.6.14/tutorial-catalogs/GOOGLE-CMIP6.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.605468 intake-esm-2023.7.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.593467 intake-esm-2023.7.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.593467 intake-esm-2023.7.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.593467 intake-esm-2023.7.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    51400 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-07 12:55:29.605468 intake-esm-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.593467 intake-esm-2023.7.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.589467 intake-esm-2023.7.7/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.593467 intake-esm-2023.7.7/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    22404 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/_static/images/NSF_4-Color_bitmap_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/_static/images/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.593467 intake-esm-2023.7.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/catalogs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.597468 intake-esm-2023.7.7/docs/source/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/build-a-catalog-from-timeseries-files.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/define-and-use-derived-variable-registry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/install-intake-esm.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/modify-catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/multi-variable-catalog.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/multi-variable-catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/understand-keys-and-how-to-change-them.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.597468 intake-esm-2023.7.7/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/reference/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/reference/cmip_ap.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/reference/esm-catalog-spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/reference/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.597468 intake-esm-2023.7.7/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/docs/source/tutorials/loading-cmip6-data.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.601468 intake-esm-2023.7.7/intake_esm/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34111 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/intake_esm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.605468 intake-esm-2023.7.7/intake_esm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-07 12:55:29.000000 intake-esm-2023.7.7/intake_esm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-07 12:55:29.000000 intake-esm-2023.7.7/intake_esm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:55:29.000000 intake-esm-2023.7.7/intake_esm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 12:55:29.000000 intake-esm-2023.7.7/intake_esm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:55:28.000000 intake-esm-2023.7.7/intake_esm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 12:55:29.000000 intake-esm-2023.7.7/intake_esm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 12:55:29.000000 intake-esm-2023.7.7/intake_esm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:55:29.605468 intake-esm-2023.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:29.605468 intake-esm-2023.7.7/tutorial-catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/tutorial-catalogs/AWS-CESM2-LENS.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/tutorial-catalogs/AWS-CMIP6.json
+-rw-r--r--   0 runner    (1001) docker     (123)   108734 2023-07-07 12:55:09.000000 intake-esm-2023.7.7/tutorial-catalogs/GOOGLE-CMIP6.json
```

### Comparing `intake-esm-2023.6.14/.github/ISSUE_TEMPLATE/bug_report.md` & `intake-esm-2023.7.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/.github/ISSUE_TEMPLATE/feature_request.md` & `intake-esm-2023.7.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/.github/pull_request_template.md` & `intake-esm-2023.7.7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/.github/workflows/ci.yaml` & `intake-esm-2023.7.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/.github/workflows/pypi.yml` & `intake-esm-2023.7.7/.github/workflows/pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -24,12 +24,12 @@
           git clean -xdf
           git restore -SW .
           python -m build --sdist --wheel .
       - name: Test the artifacts
         run: |
           python -m twine check dist/*
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           user: ${{ secrets.PYPI_USERNAME }}
           password: ${{ secrets.PYPI_PASSWORD }}
           verbose: true
```

### Comparing `intake-esm-2023.6.14/.gitignore` & `intake-esm-2023.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/.pre-commit-config.yaml` & `intake-esm-2023.7.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/CHANGELOG.md` & `intake-esm-2023.7.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/CONTRIBUTING.md` & `intake-esm-2023.7.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/LICENSE` & `intake-esm-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/Makefile` & `intake-esm-2023.7.7/Makefile`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/PKG-INFO` & `intake-esm-2023.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-esm
-Version: 2023.6.14
+Version: 2023.7.7
 Summary: An intake plugin for parsing an Earth System Model (ESM) catalog and loading netCDF files and/or Zarr stores into Xarray datasets.
 Home-page: https://intake-esm.readthedocs.io
 Maintainer: NCAR XDev Team
 Maintainer-email: xdev@ucar.edu
 License: Apache 2.0
 Project-URL: Documentation, https://intake-esm.readthedocs.io
 Project-URL: Source, https://github.com/intake/intake-esm
```

### Comparing `intake-esm-2023.6.14/README.md` & `intake-esm-2023.7.7/README.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/Makefile` & `intake-esm-2023.7.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/_static/images/NSF_4-Color_bitmap_Logo.png` & `intake-esm-2023.7.7/docs/_static/images/NSF_4-Color_bitmap_Logo.png`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/_static/images/nsf.png` & `intake-esm-2023.7.7/docs/_static/images/nsf.png`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/make.bat` & `intake-esm-2023.7.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/catalogs.yaml` & `intake-esm-2023.7.7/docs/source/catalogs.yaml`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/conf.py` & `intake-esm-2023.7.7/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,26 @@
     'sphinx.ext.intersphinx',
     'sphinx.ext.extlinks',
     'sphinx.ext.intersphinx',
     'sphinx.ext.napoleon',
     'myst_nb',
     'sphinxext.opengraph',
     'sphinx_copybutton',
-    'sphinxcontrib.autodoc_pydantic',
     'sphinx_design',
 ]
 
 
 # MyST config
 myst_enable_extensions = ['amsmath', 'colon_fence', 'deflist', 'html_image']
 myst_url_schemes = ['http', 'https', 'mailto']
 
 # sphinx-copybutton configurations
 copybutton_prompt_text = r'>>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: '
 copybutton_prompt_is_regexp = True
 
-autodoc_pydantic_model_show_json = True
-autodoc_pydantic_model_show_config = False
-
 nb_execution_mode = 'cache'
 nb_execution_timeout = 600
 nb_execution_raise_on_error = True
 
 extlinks = {
     'issue': ('https://github.com/intake/intake-esm/issues/%s', 'GH#'),
     'pr': ('https://github.com/intake/intake-esm/pull/%s', 'GH#'),
```

### Comparing `intake-esm-2023.6.14/docs/source/how-to/build-a-catalog-from-timeseries-files.md` & `intake-esm-2023.7.7/docs/source/how-to/build-a-catalog-from-timeseries-files.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/define-and-use-derived-variable-registry.md` & `intake-esm-2023.7.7/docs/source/how-to/define-and-use-derived-variable-registry.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md` & `intake-esm-2023.7.7/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md` & `intake-esm-2023.7.7/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/install-intake-esm.md` & `intake-esm-2023.7.7/docs/source/how-to/install-intake-esm.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/modify-catalog.md` & `intake-esm-2023.7.7/docs/source/how-to/modify-catalog.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/multi-variable-catalog.csv` & `intake-esm-2023.7.7/docs/source/how-to/multi-variable-catalog.csv`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/multi-variable-catalog.json` & `intake-esm-2023.7.7/docs/source/how-to/multi-variable-catalog.json`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/understand-keys-and-how-to-change-them.md` & `intake-esm-2023.7.7/docs/source/how-to/understand-keys-and-how-to-change-them.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md` & `intake-esm-2023.7.7/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/index.md` & `intake-esm-2023.7.7/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/reference/cmip_ap.md` & `intake-esm-2023.7.7/docs/source/reference/cmip_ap.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/reference/esm-catalog-spec.md` & `intake-esm-2023.7.7/docs/source/reference/esm-catalog-spec.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/reference/faq.md` & `intake-esm-2023.7.7/docs/source/reference/faq.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/docs/source/tutorials/loading-cmip6-data.md` & `intake-esm-2023.7.7/docs/source/tutorials/loading-cmip6-data.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/intake_esm/__init__.py` & `intake-esm-2023.7.7/intake_esm/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/intake_esm/_search.py` & `intake-esm-2023.7.7/intake_esm/_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         )
         column_has_iterables = column in columns_with_iterables
         for value in values:
             if column_has_iterables:
                 mask = df[column].str.contains(value, regex=False)
             elif column_is_stringtype and is_pattern(value):
                 mask = df[column].str.contains(value, regex=True, case=True, flags=0)
+            elif pd.isna(value):
+                mask = df[column].isnull()
             else:
                 mask = df[column] == value
             local_mask = local_mask | mask
         global_mask = global_mask & local_mask
     results = df.loc[global_mask]
     return results.reset_index(drop=True)
```

### Comparing `intake-esm-2023.6.14/intake_esm/cat.py` & `intake-esm-2023.7.7/intake_esm/cat.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import typing
 
 import fsspec
 import pandas as pd
 import pydantic
 import tlz
+from pydantic import ConfigDict
 
 from ._search import search, search_apply_require_all_on
 
 
 def _allnan_or_nonan(df, column: str) -> bool:
     """Check if all values in a column are NaN or not NaN
 
@@ -36,116 +37,102 @@
 
 
 class AggregationType(str, enum.Enum):
     join_new = 'join_new'
     join_existing = 'join_existing'
     union = 'union'
 
-    class Config:
-        validate_all = True
-        validate_assignment = True
+    model_config = ConfigDict(validate_default=True, validate_assignment=True)
 
 
 class DataFormat(str, enum.Enum):
     netcdf = 'netcdf'
     zarr = 'zarr'
     reference = 'reference'
     opendap = 'opendap'
 
-    class Config:
-        validate_all = True
-        validate_assignment = True
+    model_config = ConfigDict(validate_default=True, validate_assignment=True)
 
 
 class Attribute(pydantic.BaseModel):
     column_name: pydantic.StrictStr
     vocabulary: pydantic.StrictStr = ''
 
-    class Config:
-        validate_all = True
-        validate_assignment = True
+    model_config = ConfigDict(validate_default=True, validate_assignment=True)
 
 
 class Assets(pydantic.BaseModel):
     column_name: pydantic.StrictStr
-    format: typing.Optional[DataFormat]
-    format_column_name: typing.Optional[pydantic.StrictStr]
+    format: typing.Optional[DataFormat] = None
+    format_column_name: typing.Optional[pydantic.StrictStr] = None
 
-    class Config:
-        validate_all = True
-        validate_assignment = True
-
-    @pydantic.root_validator
-    def _validate_data_format(cls, values):
-        data_format, format_column_name = values.get('format'), values.get('format_column_name')
+    model_config = ConfigDict(validate_default=True, validate_assignment=True)
+
+    @pydantic.model_validator(mode='after')
+    def _validate_data_format(cls, model):
+        data_format, format_column_name = model.format, model.format_column_name
         if data_format is not None and format_column_name is not None:
             raise ValueError('Cannot set both format and format_column_name')
         elif data_format is None and format_column_name is None:
             raise ValueError('Must set one of format or format_column_name')
-        return values
+        return model
 
 
 class Aggregation(pydantic.BaseModel):
     type: AggregationType
     attribute_name: pydantic.StrictStr
-    options: typing.Optional[dict] = {}
+    options: dict = {}
 
-    class Config:
-        validate_all = True
-        validate_assignment = True
+    model_config = ConfigDict(validate_default=True, validate_assignment=True)
 
 
 class AggregationControl(pydantic.BaseModel):
     variable_column_name: pydantic.StrictStr
     groupby_attrs: list[pydantic.StrictStr]
     aggregations: list[Aggregation] = []
 
-    class Config:
-        validate_all = True
-        validate_assignment = True
+    model_config = ConfigDict(validate_default=True, validate_assignment=True)
 
 
 class ESMCatalogModel(pydantic.BaseModel):
     """
     Pydantic model for the ESM data catalog defined in https://git.io/JBWoW
     """
 
     esmcat_version: pydantic.StrictStr
     attributes: list[Attribute]
     assets: Assets
     aggregation_control: typing.Optional[AggregationControl] = None
-    id: typing.Optional[str] = ''
+    id: str = ''
     catalog_dict: typing.Optional[list[dict]] = None
-    catalog_file: pydantic.StrictStr = None
-    description: pydantic.StrictStr = None
-    title: pydantic.StrictStr = None
+    catalog_file: typing.Optional[pydantic.StrictStr] = None
+    description: typing.Optional[pydantic.StrictStr] = None
+    title: typing.Optional[pydantic.StrictStr] = None
     last_updated: typing.Optional[typing.Union[datetime.datetime, datetime.date]] = None
-    _df: typing.Optional[pd.DataFrame] = pydantic.PrivateAttr()
+    _df: pd.DataFrame = pydantic.PrivateAttr()
 
-    class Config:
-        arbitrary_types_allowed = True
-        underscore_attrs_are_private = True
-        validate_all = True
-        validate_assignment = True
-
-    @pydantic.root_validator
-    def validate_catalog(cls, values):
-        catalog_dict, catalog_file = values.get('catalog_dict'), values.get('catalog_file')
+    model_config = ConfigDict(
+        arbitrary_types_allowed=True, validate_default=True, validate_assignment=True
+    )
+
+    @pydantic.model_validator(mode='after')
+    def validate_catalog(cls, model):
+        catalog_dict, catalog_file = model.catalog_dict, model.catalog_file
         if catalog_dict is not None and catalog_file is not None:
             raise ValueError('catalog_dict and catalog_file cannot be set at the same time')
 
-        return values
+        return model
 
     @classmethod
     def from_dict(cls, data: dict) -> 'ESMCatalogModel':
         esmcat = data['esmcat']
         df = data['df']
         if 'last_updated' not in esmcat:
             esmcat['last_updated'] = None
-        cat = cls.parse_obj(esmcat)
+        cat = cls.model_validate(esmcat)
         cat._df = df
         return cat
 
     def save(
         self,
         name: str,
         *,
@@ -250,15 +237,15 @@
         json_file = str(json_file)  # We accept Path, but fsspec doesn't.
         _mapper = fsspec.get_mapper(json_file, **storage_options)
 
         with fsspec.open(json_file, **storage_options) as fobj:
             data = json.loads(fobj.read())
             if 'last_updated' not in data:
                 data['last_updated'] = None
-            cat = cls.parse_obj(data)
+            cat = cls.model_validate(data)
             if cat.catalog_file:
                 if _mapper.fs.exists(cat.catalog_file):
                     csv_path = cat.catalog_file
                 else:
                     csv_path = f'{os.path.dirname(_mapper.root)}/{cat.catalog_file}'
                 cat.catalog_file = csv_path
                 df = pd.read_csv(
@@ -413,36 +400,36 @@
 
 
 class QueryModel(pydantic.BaseModel):
     """A Pydantic model to represent a query to be executed against a catalog."""
 
     query: dict[pydantic.StrictStr, typing.Union[typing.Any, list[typing.Any]]]
     columns: list[str]
-    require_all_on: typing.Union[str, list[typing.Any]] = None
+    require_all_on: typing.Optional[typing.Union[str, list[typing.Any]]] = None
 
-    class Config:
-        validate_all = True
-        validate_assignment = True
-
-    @pydantic.root_validator(pre=False)
-    def validate_query(cls, values):
-        query = values.get('query', {})
-        columns = values.get('columns')
-        require_all_on = values.get('require_all_on', [])
+    # TODO: Seem to be unable to modify fields in model_validator with
+    # validate_assignment=True since it leads to recursion
+    model_config = ConfigDict(validate_default=True, validate_assignment=False)
+
+    @pydantic.model_validator(mode='after')
+    def validate_query(cls, model):
+        query = model.query
+        columns = model.columns
+        require_all_on = model.require_all_on
 
         if query:
             for key in query:
                 if key not in columns:
                     raise ValueError(f'Column {key} not in columns {columns}')
         if isinstance(require_all_on, str):
-            values['require_all_on'] = [require_all_on]
+            model.require_all_on = [require_all_on]
         if require_all_on is not None:
-            for key in values['require_all_on']:
+            for key in model.require_all_on:
                 if key not in columns:
                     raise ValueError(f'Column {key} not in columns {columns}')
         _query = query.copy()
         for key, value in _query.items():
-            if isinstance(value, (str, int, float, bool)):
+            if isinstance(value, (str, int, float, bool)) or value is None or value is pd.NA:
                 _query[key] = [value]
 
-        values['query'] = _query
-        return values
+        model.query = _query
+        return model
```

### Comparing `intake-esm-2023.6.14/intake_esm/core.py` & `intake-esm-2023.7.7/intake_esm/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,15 +325,19 @@
         ]
         return sorted(list(self.__dict__.keys()) + rv)
 
     def _ipython_key_completions_(self):
         return self.__dir__()
 
     @pydantic.validate_arguments
-    def search(self, require_all_on: typing.Union[str, list[str]] = None, **query: typing.Any):
+    def search(
+        self,
+        require_all_on: typing.Optional[typing.Union[str, list[str]]] = None,
+        **query: typing.Any,
+    ):
         """Search for entries in the catalog.
 
         Parameters
         ----------
         require_all_on : list, str, optional
             A dataframe column or a list of dataframe columns across
             which all entries must satisfy the query criteria.
@@ -439,19 +443,19 @@
             cat.derivedcat = self.derivedcat
         return cat
 
     @pydantic.validate_arguments
     def serialize(
         self,
         name: pydantic.StrictStr,
-        directory: typing.Union[pydantic.DirectoryPath, pydantic.StrictStr] = None,
+        directory: typing.Optional[typing.Union[pydantic.DirectoryPath, pydantic.StrictStr]] = None,
         catalog_type: str = 'dict',
-        to_csv_kwargs: dict[typing.Any, typing.Any] = None,
-        json_dump_kwargs: dict[typing.Any, typing.Any] = None,
-        storage_options: dict[str, typing.Any] = None,
+        to_csv_kwargs: typing.Optional[dict[typing.Any, typing.Any]] = None,
+        json_dump_kwargs: typing.Optional[dict[typing.Any, typing.Any]] = None,
+        storage_options: typing.Optional[dict[str, typing.Any]] = None,
     ) -> None:
         """Serialize catalog to corresponding json and csv files.
 
         Parameters
         ----------
         name : str
             name to use when creating ESM catalog json file and csv catalog.
@@ -532,20 +536,20 @@
                 self.derivedcat.keys()
             )
         return unique
 
     @pydantic.validate_arguments
     def to_dataset_dict(
         self,
-        xarray_open_kwargs: dict[str, typing.Any] = None,
-        xarray_combine_by_coords_kwargs: dict[str, typing.Any] = None,
-        preprocess: typing.Callable = None,
-        storage_options: dict[pydantic.StrictStr, typing.Any] = None,
-        progressbar: pydantic.StrictBool = None,
-        aggregate: pydantic.StrictBool = None,
+        xarray_open_kwargs: typing.Optional[dict[str, typing.Any]] = None,
+        xarray_combine_by_coords_kwargs: typing.Optional[dict[str, typing.Any]] = None,
+        preprocess: typing.Optional[typing.Callable] = None,
+        storage_options: typing.Optional[dict[pydantic.StrictStr, typing.Any]] = None,
+        progressbar: typing.Optional[pydantic.StrictBool] = None,
+        aggregate: typing.Optional[pydantic.StrictBool] = None,
         skip_on_error: pydantic.StrictBool = False,
         **kwargs,
     ) -> dict[str, xr.Dataset]:
         """
         Load catalog entries into a dictionary of xarray datasets.
 
         Column values, dataset keys and requested variables are added as global
@@ -682,20 +686,20 @@
                         raise exc
         self.datasets = self._create_derived_variables(datasets, skip_on_error)
         return self.datasets
 
     @pydantic.validate_arguments
     def to_datatree(
         self,
-        xarray_open_kwargs: dict[str, typing.Any] = None,
-        xarray_combine_by_coords_kwargs: dict[str, typing.Any] = None,
-        preprocess: typing.Callable = None,
-        storage_options: dict[pydantic.StrictStr, typing.Any] = None,
-        progressbar: pydantic.StrictBool = None,
-        aggregate: pydantic.StrictBool = None,
+        xarray_open_kwargs: typing.Optional[dict[str, typing.Any]] = None,
+        xarray_combine_by_coords_kwargs: typing.Optional[dict[str, typing.Any]] = None,
+        preprocess: typing.Optional[typing.Callable] = None,
+        storage_options: typing.Optional[dict[pydantic.StrictStr, typing.Any]] = None,
+        progressbar: typing.Optional[pydantic.StrictBool] = None,
+        aggregate: typing.Optional[pydantic.StrictBool] = None,
         skip_on_error: pydantic.StrictBool = False,
         **kwargs,
     ):
         """
         Load catalog entries into a tree of xarray datasets.
 
         Parameters
```

### Comparing `intake-esm-2023.6.14/intake_esm/derived.py` & `intake-esm-2023.7.7/intake_esm/derived.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class DerivedVariable(pydantic.BaseModel):
     func: typing.Callable
     variable: pydantic.StrictStr
     query: dict[pydantic.StrictStr, typing.Union[typing.Any, list[typing.Any]]]
     prefer_derived: bool
 
-    @pydantic.validator('query')
+    @pydantic.field_validator('query')
     def validate_query(cls, values):
         _query = values.copy()
         for key, value in _query.items():
             if isinstance(value, (str, int, float, bool)):
                 _query[key] = [value]
         return _query
 
@@ -42,15 +42,15 @@
             ) from exc
 
 
 @pydantic.dataclasses.dataclass
 class DerivedVariableRegistry:
     """Registry of derived variables"""
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         self._registry = {}
 
     @classmethod
     def load(cls, name: str, package: str = None) -> 'DerivedVariableRegistry':
         """Load a DerivedVariableRegistry from a Python module/file
 
         Parameters
```

### Comparing `intake-esm-2023.6.14/intake_esm/source.py` & `intake-esm-2023.7.7/intake_esm/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,20 +132,20 @@
         records: list[dict[str, typing.Any]],
         path_column_name: pydantic.StrictStr,
         data_format: typing.Optional[DataFormat],
         format_column_name: typing.Optional[pydantic.StrictStr],
         *,
         variable_column_name: typing.Optional[pydantic.StrictStr] = None,
         aggregations: typing.Optional[list[Aggregation]] = None,
-        requested_variables: list[str] = None,
-        preprocess: typing.Callable = None,
-        storage_options: dict[str, typing.Any] = None,
-        xarray_open_kwargs: dict[str, typing.Any] = None,
-        xarray_combine_by_coords_kwargs: dict[str, typing.Any] = None,
-        intake_kwargs: dict[str, typing.Any] = None,
+        requested_variables: typing.Optional[list[str]] = None,
+        preprocess: typing.Optional[typing.Callable] = None,
+        storage_options: typing.Optional[dict[str, typing.Any]] = None,
+        xarray_open_kwargs: typing.Optional[dict[str, typing.Any]] = None,
+        xarray_combine_by_coords_kwargs: typing.Optional[dict[str, typing.Any]] = None,
+        intake_kwargs: typing.Optional[dict[str, typing.Any]] = None,
     ):
         """An intake compatible Data Source for ESM data.
 
         Parameters
         ----------
         key: str
             The key of the data source.
@@ -248,24 +248,19 @@
                 datasets = sorted(
                     datasets,
                     key=lambda ds: tuple(
                         f"{OPTIONS['attrs_prefix']}/{agg.attribute_name}"
                         for agg in self.aggregations
                     ),
                 )
-                with dask.config.set(
-                    {'scheduler': 'single-threaded', 'array.slicing.split_large_chunks': True}
-                ):  # Use single-threaded scheduler
-                    datasets = [
-                        ds.set_coords(set(ds.variables) - set(ds.attrs[OPTIONS['vars_key']]))
-                        for ds in datasets
-                    ]
-                    self._ds = xr.combine_by_coords(
-                        datasets, **self.xarray_combine_by_coords_kwargs
-                    )
+                datasets = [
+                    ds.set_coords(set(ds.variables) - set(ds.attrs[OPTIONS['vars_key']]))
+                    for ds in datasets
+                ]
+                self._ds = xr.combine_by_coords(datasets, **self.xarray_combine_by_coords_kwargs)
 
             self._ds.attrs[OPTIONS['dataset_key']] = self.key
 
         except Exception as exc:
             raise ESMDataSourceError(
                 f"""Failed to load dataset with key='{self.key}'
                  You can use `cat['{self.key}'].df` to inspect the assets/files for this key.
```

### Comparing `intake-esm-2023.6.14/intake_esm/tutorial.py` & `intake-esm-2023.7.7/intake_esm/tutorial.py`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/intake_esm/utils.py` & `intake-esm-2023.7.7/intake_esm/utils.py`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/intake_esm.egg-info/PKG-INFO` & `intake-esm-2023.7.7/intake_esm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-esm
-Version: 2023.6.14
+Version: 2023.7.7
 Summary: An intake plugin for parsing an Earth System Model (ESM) catalog and loading netCDF files and/or Zarr stores into Xarray datasets.
 Home-page: https://intake-esm.readthedocs.io
 Maintainer: NCAR XDev Team
 Maintainer-email: xdev@ucar.edu
 License: Apache 2.0
 Project-URL: Documentation, https://intake-esm.readthedocs.io
 Project-URL: Source, https://github.com/intake/intake-esm
```

### Comparing `intake-esm-2023.6.14/intake_esm.egg-info/SOURCES.txt` & `intake-esm-2023.7.7/intake_esm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/pyproject.toml` & `intake-esm-2023.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/setup.py` & `intake-esm-2023.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/tutorial-catalogs/AWS-CESM2-LENS.json` & `intake-esm-2023.7.7/tutorial-catalogs/AWS-CESM2-LENS.json`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/tutorial-catalogs/AWS-CMIP6.json` & `intake-esm-2023.7.7/tutorial-catalogs/AWS-CMIP6.json`

 * *Files identical despite different names*

### Comparing `intake-esm-2023.6.14/tutorial-catalogs/GOOGLE-CMIP6.json` & `intake-esm-2023.7.7/tutorial-catalogs/GOOGLE-CMIP6.json`

 * *Files identical despite different names*

