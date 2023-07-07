# Comparing `tmp/wpp-bavapi-0.4.1.tar.gz` & `tmp/wpp-bavapi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpp-bavapi-0.4.1.tar", last modified: Tue Jul  4 09:55:19 2023, max compression
+gzip compressed data, was "wpp-bavapi-0.5.0.tar", last modified: Fri Jul  7 17:43:11 2023, max compression
```

## Comparing `wpp-bavapi-0.4.1.tar` & `wpp-bavapi-0.5.0.tar`

### file list

```diff
@@ -1,68 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.778684 wpp-bavapi-0.4.1/
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.528960 wpp-bavapi-0.4.1/.github/
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.537962 wpp-bavapi-0.4.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      627 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      624 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-rw-   0        0        0     1094 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.544423 wpp-bavapi-0.4.1/.github/workflows/
--rw-rw-rw-   0        0        0     2108 2023-06-29 13:14:09.000000 wpp-bavapi-0.4.1/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0     3277 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/.gitignore
--rw-rw-rw-   0        0        0    13312 2023-06-29 13:15:42.000000 wpp-bavapi-0.4.1/BAVAPI Jupyter Demo.ipynb
--rw-rw-rw-   0        0        0    11541 2023-07-04 09:19:30.000000 wpp-bavapi-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     4606 2023-07-04 09:55:19.776688 wpp-bavapi-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3509 2023-07-04 09:27:00.000000 wpp-bavapi-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.592969 wpp-bavapi-0.4.1/bavapi/
--rw-rw-rw-   0        0        0     1233 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/__init__.py
--rw-rw-rw-   0        0        0    21759 2023-06-29 17:25:51.000000 wpp-bavapi-0.4.1/bavapi/client.py
--rw-rw-rw-   0        0        0      295 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/exceptions.py
--rw-rw-rw-   0        0        0    11618 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/filters.py
--rw-rw-rw-   0        0        0     6952 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/http.py
--rw-rw-rw-   0        0        0     1026 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/jupyter.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.609815 wpp-bavapi-0.4.1/bavapi/parsing/
--rw-rw-rw-   0        0        0      100 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/parsing/__init__.py
--rw-rw-rw-   0        0        0     2181 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/parsing/params.py
--rw-rw-rw-   0        0        0     4906 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/parsing/responses.py
--rw-rw-rw-   0        0        0        0 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/py.typed
--rw-rw-rw-   0        0        0     4614 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/query.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.624816 wpp-bavapi-0.4.1/bavapi/reference/
--rw-rw-rw-   0        0        0        0 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/reference/__init__.py
--rw-rw-rw-   0        0        0      419 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/reference/_int_enum.py
--rw-rw-rw-   0        0        0     8802 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/reference/generate_reference.py
--rw-rw-rw-   0        0        0    15050 2023-06-29 17:25:22.000000 wpp-bavapi-0.4.1/bavapi/sync.py
--rw-rw-rw-   0        0        0     1623 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/bavapi/typing.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.636816 wpp-bavapi-0.4.1/bavapi_refs/
--rw-rw-rw-   0        0        0     3115 2023-06-19 20:12:53.000000 wpp-bavapi-0.4.1/bavapi_refs/audiences.py
--rw-rw-rw-   0        0        0     1341 2023-06-19 20:12:53.000000 wpp-bavapi-0.4.1/bavapi_refs/countries.py
--rw-rw-rw-   0        0        0     5732 2023-06-22 12:18:08.000000 wpp-bavapi-0.4.1/noxfile.py
--rw-rw-rw-   0        0        0     2277 2023-07-04 09:54:37.000000 wpp-bavapi-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      933 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 09:55:19.779694 wpp-bavapi-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.685261 wpp-bavapi-0.4.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/__init__.py
--rw-rw-rw-   0        0        0      520 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/conftest.py
--rw-rw-rw-   0        0        0      446 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.703412 wpp-bavapi-0.4.1/tests/integration/
--rw-rw-rw-   0        0        0        0 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/integration/__init__.py
--rw-rw-rw-   0        0        0     2346 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/integration/test_async.py
--rw-rw-rw-   0        0        0     2191 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/integration/test_sync.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.718035 wpp-bavapi-0.4.1/tests/parsing/
--rw-rw-rw-   0        0        0        0 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/parsing/__init__.py
--rw-rw-rw-   0        0        0      992 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/parsing/test_params.py
--rw-rw-rw-   0        0        0     2687 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/parsing/test_responses.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.734104 wpp-bavapi-0.4.1/tests/reference/
--rw-rw-rw-   0        0        0        0 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/reference/__init__.py
--rw-rw-rw-   0        0        0     4688 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/reference/test_generate_reference.py
--rw-rw-rw-   0        0        0      435 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/reference/test_int_enum.py
--rw-rw-rw-   0        0        0     3898 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/test_client.py
--rw-rw-rw-   0        0        0     2841 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/test_filters.py
--rw-rw-rw-   0        0        0     8118 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/test_http.py
--rw-rw-rw-   0        0        0     1227 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/test_jupyter.py
--rw-rw-rw-   0        0        0     1491 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/test_queries.py
--rw-rw-rw-   0        0        0     1842 2023-06-21 17:02:54.000000 wpp-bavapi-0.4.1/tests/test_sync.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:55:19.770616 wpp-bavapi-0.4.1/wpp_bavapi.egg-info/
--rw-rw-rw-   0        0        0     4606 2023-07-04 09:55:18.000000 wpp-bavapi-0.4.1/wpp_bavapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1302 2023-07-04 09:55:19.000000 wpp-bavapi-0.4.1/wpp_bavapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:55:18.000000 wpp-bavapi-0.4.1/wpp_bavapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-04 09:55:18.000000 wpp-bavapi-0.4.1/wpp_bavapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      248 2023-07-04 09:55:18.000000 wpp-bavapi-0.4.1/wpp_bavapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 09:55:18.000000 wpp-bavapi-0.4.1/wpp_bavapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.397636 wpp-bavapi-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/BAVAPI Jupyter Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/bavapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/bavapi/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/parsing/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/parsing/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/bavapi/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/reference/_int_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/reference/generate_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/assets/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/assets/wpp-bav-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/audiences.md
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/brands.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/brandscape-data.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/studies.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/gen_ref_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/getting-started/authentication.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/getting-started/reference-classes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/reference/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/usage/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/usage/basic.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/integration/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/integration/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/parsing/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/parsing/test_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/reference/test_generate_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/reference/test_int_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/type_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/type_stubs/nest_asyncio.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/top_level.txt
```

### Comparing `wpp-bavapi-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
----
-name: Bug report
-about: Create a report to help us improve
-title: "[BUG]"
-labels: ''
-assignees: ''
-
----
-
-**Describe the bug**
-A clear and concise description of what the bug is.
-
-**To Reproduce**
-Steps to reproduce the behavior:
-
-**Expected behavior**
-A clear and concise description of what you expected to happen.
-
-**Screenshots**
-If applicable, add screenshots to help explain your problem.
-
-**Desktop (please complete the following information):**
- - OS: [e.g. Windows]
- - IDE [e.g. Jupyter, VSCode]
- - Version [e.g. 22]
-
-**Additional context**
-Add any other context about the problem here.
+---
+name: Bug report
+about: Create a report to help us improve
+title: "[BUG]"
+labels: ''
+assignees: ''
+
+---
+
+**Describe the bug**
+A clear and concise description of what the bug is.
+
+**To Reproduce**
+Steps to reproduce the behavior:
+
+**Expected behavior**
+A clear and concise description of what you expected to happen.
+
+**Screenshots**
+If applicable, add screenshots to help explain your problem.
+
+**Desktop (please complete the following information):**
+ - OS: [e.g. Windows]
+ - IDE [e.g. Jupyter, VSCode]
+ - Version [e.g. 22]
+
+**Additional context**
+Add any other context about the problem here.
```

### Comparing `wpp-bavapi-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
----
-name: Feature request
-about: Suggest an idea for this project
-title: "[FEATURE]"
-labels: ''
-assignees: ''
-
----
-
-**Is your feature request related to a problem? Please describe.**
-A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
-
-**Describe the solution you'd like**
-A clear and concise description of what you want to happen.
-
-**Describe alternatives you've considered**
-A clear and concise description of any alternative solutions or features you've considered.
-
-**Additional context**
-Add any other context or screenshots about the feature request here.
+---
+name: Feature request
+about: Suggest an idea for this project
+title: "[FEATURE]"
+labels: ''
+assignees: ''
+
+---
+
+**Is your feature request related to a problem? Please describe.**
+A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
+
+**Describe the solution you'd like**
+A clear and concise description of what you want to happen.
+
+**Describe alternatives you've considered**
+A clear and concise description of any alternative solutions or features you've considered.
+
+**Additional context**
+Add any other context or screenshots about the feature request here.
```

### Comparing `wpp-bavapi-0.4.1/.gitignore` & `wpp-bavapi-0.5.0/.gitignore`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-# dev files
-.vscode/
-bavapi_refs/
-
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+# dev files
+.vscode/
+bavapi_refs/
+
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
```

### Comparing `wpp-bavapi-0.4.1/BAVAPI Jupyter Demo.ipynb` & `wpp-bavapi-0.5.0/BAVAPI Jupyter Demo.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925423534798534%*

 * *Differences: {"'cells'": '{3: {\'source\': [\'TOKEN = "your_token"  # paste your Fount API token here, or '*

 * *            "follow the instructions below']}, 5: {'source': ['>__**💡 Tip:**__ Uncomment the cell "*

 * *            "below to install `python-dotenv`']}, 8: {'source': {insert: [(4, '```\\n')], delete: "*

 * *            "[4]}}, 24: {'source': {insert: [(26, '>__**⚠ WARNING:**__ DO NOT PUSH REFERENCE FILES "*

 * *            "TO GIT! Add `bavapi_refs/` to your `.gitignore` file.')], delete: [26]}}, 32: "*

 * *            '{\'source\ […]*

```diff
@@ -42,23 +42,40 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "TOKEN = \"your_token\"  # paste your Fount API token here"
+                "TOKEN = \"your_token\"  # paste your Fount API token here, or follow the instructions below"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The following cell uses `dotenv` ([learn more](https://github.com/theskumar/python-dotenv)) to load the token from a `.env` file, as recommended in the `bavapi` [documentation](https://fountapi-documentation.vercel.app/getting-started/authentication/)."
+                "The following cells uses `python-dotenv` ([learn more](https://github.com/theskumar/python-dotenv)) to load the token from a `.env` file, as recommended in the `bavapi` [documentation](https://fountapi-documentation.vercel.app/getting-started/authentication/)."
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                ">__**\ud83d\udca1 Tip:**__ Uncomment the cell below to install `python-dotenv`"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# %pip install python-dotenv"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -75,15 +92,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Using `bavapi` to get BAV data\n",
                 "\n",
                 "To get started, install `bavapi` by running the following command:\n",
                 "\n",
-                "```prompt\n",
+                "```\n",
                 "pip install wpp-bavapi\n",
                 "```\n",
                 "\n",
                 "For more information, see the [installation](https://fountapi-documentation.vercel.app/getting-started/installation/) instructions in the `bavapi` documentation."
             ]
         },
         {
@@ -267,15 +284,15 @@
                 "\n",
                 "Run the following to generate reference files in a new directory `bavapi_refs`:\n",
                 "\n",
                 "```prompt\n",
                 "bavapi-gen-refs --all\n",
                 "```\n",
                 "\n",
-                ">__**WARNING:**__ DO NOT PUSH REFERENCE FILES TO GIT! Add `bavapi_refs/` to your `.gitignore` file."
+                ">__**\u26a0 WARNING:**__ DO NOT PUSH REFERENCE FILES TO GIT! Add `bavapi_refs/` to your `.gitignore` file."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -347,15 +364,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Get Spanish data for 2022 for the `Adults with kids` base sorted by Differentiation in descending order (highest first)\n",
-                "es_bss = bavapi.brandscape_data(TOKEN, \"ES\", 2022, audiences=Audiences.ADULTS_WITH_KIDS, sort=\"-differentiation_rank\")\n",
+                "es_bss = bavapi.brandscape_data(TOKEN, \"ES\", 2022, audiences=[Audiences.ADULTS_WITH_KIDS, Audiences.ADULTS_WITH_KIDS_0_11], sort=\"-differentiation_rank\")\n",
                 "es_bss.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -404,15 +421,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Advanced Usage\n",
                 "\n",
                 ">_**NOTE:**_ This section is more geared towards using `bavapi` in other libraries or applications, or when having to make many separate queries. For general Jupyter notebook use, the examples above should work in most cases.\n",
                 "\n",
-                "`bavapi` provides a `Client` class that provides a direct async interface for developing asynchronous programs or when having to make many separate queries.\n",
+                "`bavapi` provides a `Client` class that provides a direct `async` interface for developing asynchronous programs or when having to make many separate queries.\n",
                 "\n",
                 "`bavapi.Client` is an asynchronous context manager, similar in use to `httpx.AsyncClient` (which powers `bavapi`) or `requests.Session`.\n",
                 "\n",
                 "It also brings performance benefits and more. See the [documentation](https://bavapi-documentation.vercel.app/usage/advanced/) for more details.\n",
                 "\n",
                 "The `Client` can be used directly in Jupyter notebooks, or within asynchronous functions (defined with `async def`).\n",
                 "\n",
```

### Comparing `wpp-bavapi-0.4.1/LICENSE` & `wpp-bavapi-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [2023] [WPPBAV]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [2023] [WPPBAV]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `wpp-bavapi-0.4.1/PKG-INFO` & `wpp-bavapi-0.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,123 @@
-Metadata-Version: 2.1
-Name: wpp-bavapi
-Version: 0.4.1
-Summary: Python consumer for the WPPBAV Fount API.
-Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
-License: Apache 2.0
-Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database :: Database Engines/Servers
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: lint
-License-File: LICENSE
-
-# BAV API Python SDK
-
-[![CI status](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
-[![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/nachomaiz/32196acdc05431cd2bc7a8c73a587a8d/raw/covbadge.json)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
-[![docs](https://img.shields.io/badge/docs-passing-brightgreen)](https://fountapi-documentation.vercel.app/)
-[![version](https://img.shields.io/badge/version-v0.4.1-blue)](https://github.com/wppbav/bavapi-sdk-python)
-[![py-versions](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/wppbav/bavapi-sdk-python)
-
-`bavapi` is a Python SDK for the WPP BAV API.
-
-With `bavapi` you can access the full BAV data catalog, the largest and most comprehensive database of brand data in the world.
-
-Queries are validated automatically thanks to `pydantic` and retrieved asynchronously via the `httpx` package.
-
-For more information about the API, go to the [WPPBAV Developer Hub](https://developer.wppbav.com).
-
-## Prerequisites
-
-`bavapi` requires Python 3.9 or higher to run.
-
-If you don't have Python installed, you can find it from the [official](https://www.python.org/downloads/) website or via [Anaconda](https://www.anaconda.com/).
-
-You will also need a BAV API token. For more information, go to the [Authentication](https://developer.wppbav.com/docs/2.x/authentication) section of the API documentation.
-
-### Dependencies
-
-- `httpx >= 0.20`
-- `nest-asyncio >= 1.5.6`
-- `pandas >= 0.16.2`
-- `pydantic >= 1.10, < 2.0`
-- `tqdm >= 4.62`
-- `typing-extensions >= 3.10` for Python 3.9
-
-## Installation
-
-`bavapi` can be installed using `pip`.
-
-```prompt
-pip install wpp-bavapi
-```
-
-### Installing from source
-
-To install from source, clone the GitHub repository into your local machine:
-
-```prompt
-git clone https://github.com/wppbav/bavapi-sdk-python.git
-```
-
-Go into the cloned directory and install `bavapi`:
-
-```prompt
-cd bavapi-sdk-python
-pip install .
-```
-
-## Usage
-
-Once you have acquired a token, you can start using this library directly in python or in a Jupyter Notebook:
-
-```py
->>> import bavapi
->>> result = bavapi.brands("TOKEN", name="Swatch")  # Replace `"TOKEN"` with your BAV API token
->>> result
-```
-
-|     | sector_id | sector_name           |  id | name   | ... |
-| --: | --------: | --------------------- | --: | ------ | --- |
-|   0 |        11 | Apparel & Accessories | 342 | Swatch | ... |
-| ... |       ... | ...                   | ... | ...    | ... |
-
-## Features
-
-- Support for all endpoints in the Fount API. Extended support for the `audiences`, `brands`, `brandscape-data` and `studies` endpoints.
-  - Other endpoints are available via the `raw_query` functions and methods.
-- Validates query parameters are of the correct types.
-  - Provides type hints for better IDE support.
-- Retrieve multiple pages of data simultaneously.
-  - Monitors and prevents exceeding API rate limit.
-
-## Documentation
-
-Read more about `bavapi` in the [documentation](https://fountapi-documentation.vercel.app/).
-
-## Issues
-
-Please file an issue on GitHub [here](https://github.com/wppbav/bavapi-sdk-python/issues).
-
-## Contributing
-
-Please see the [Contributing](https://fountapi-documentation.vercel.app/contributing/) section of the documentation for more information.
+Metadata-Version: 2.1
+Name: wpp-bavapi
+Version: 0.5.0
+Summary: Python consumer for the WPPBAV Fount API.
+Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
+License: Apache 2.0
+Project-URL: homepage, https://github.com/wppbav/bavapi-sdk-python
+Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: test
+Provides-Extra: lint
+License-File: LICENSE
+
+# BAV API Python SDK
+
+[![CI status](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
+[![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/nachomaiz/32196acdc05431cd2bc7a8c73a587a8d/raw/covbadge.json)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
+[![PyPI](https://img.shields.io/pypi/v/wpp-bavapi)](https://pypi.org/project/wpp-bavapi/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wpp-bavapi)
+](https://pypi.org/project/wpp-bavapi/)
+
+`bavapi` is a Python SDK for the WPP BAV API.
+
+It is published on [PyPI](https://pypi.org/project/wpp-bavapi/) as `wpp-bavapi`.
+
+With `bavapi` you can access the full BAV data catalog, the largest and most comprehensive database of brand data in the world.
+
+Queries are validated automatically thanks to `pydantic` and retrieved asynchronously via the `httpx` package.
+
+For more information about the API, go to the [WPPBAV Developer Hub](https://developer.wppbav.com).
+
+## Prerequisites
+
+`bavapi` requires Python 3.8 or higher to run.
+
+If you don't have Python installed, you can find it from the [official](https://www.python.org/downloads/) website or via [Anaconda](https://www.anaconda.com/).
+
+You will also need a BAV API token. For more information, go to the [Authentication](https://developer.wppbav.com/docs/2.x/authentication) section of the API documentation.
+
+### Dependencies
+
+- `httpx >= 0.20`
+- `nest-asyncio >= 1.5.6`
+- `pandas >= 0.16.2`
+- `pydantic >= 1.10, < 2.0`
+- `tqdm >= 4.62`
+- `typing-extensions >= 3.10` for Python < 3.10
+
+## Installation
+
+`bavapi` can be installed using `pip`:
+
+```prompt
+pip install wpp-bavapi
+```
+
+### Installing from source
+
+To install from source, clone the GitHub repository into your local machine:
+
+```prompt
+git clone https://github.com/wppbav/bavapi-sdk-python.git
+```
+
+Go into the cloned directory and install `bavapi`:
+
+```prompt
+cd bavapi-sdk-python
+pip install .
+```
+
+## Usage
+
+Once you have acquired a token, you can start using this library directly in python or in a Jupyter Notebook:
+
+```py
+>>> import bavapi
+>>> result = bavapi.brands("TOKEN", name="Swatch")  # Replace `"TOKEN"` with your BAV API token
+>>> result
+```
+
+|     | sector_id | sector_name           | id   | name   | ... |
+| --: | :-------- | :-------------------- | :--- | :----- | :-- |
+|   0 | 233       | Apparel & Accessories | 8635 | Swatch | ... |
+| ... | ...       | ...                   | ...  | ...    | ... |
+
+## Features
+
+- Support for all endpoints in the Fount API. Extended support for the `audiences`, `brands`, `brandscape-data` and `studies` endpoints.
+  - Other endpoints are available via the `raw_query` functions and methods.
+- Validates query parameters are of the correct types.
+  - Provides type hints for better IDE support.
+- Retrieve multiple pages of data simultaneously.
+  - Monitors and prevents exceeding API rate limit.
+- Both synchronous and asynchronous APIs for accessing BAV data.
+
+## Documentation
+
+Read more about `bavapi` in the [documentation](https://fountapi-documentation.vercel.app/).
+
+## Issues
+
+Please file an issue on GitHub [here](https://github.com/wppbav/bavapi-sdk-python/issues).
+
+## Contributing
+
+Please see the [Contributing](https://fountapi-documentation.vercel.app/contributing/) section of the documentation for more information.
```

### Comparing `wpp-bavapi-0.4.1/README.md` & `wpp-bavapi-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,94 @@
-# BAV API Python SDK
-
-[![CI status](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
-[![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/nachomaiz/32196acdc05431cd2bc7a8c73a587a8d/raw/covbadge.json)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
-[![docs](https://img.shields.io/badge/docs-passing-brightgreen)](https://fountapi-documentation.vercel.app/)
-[![version](https://img.shields.io/badge/version-v0.4.1-blue)](https://github.com/wppbav/bavapi-sdk-python)
-[![py-versions](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/wppbav/bavapi-sdk-python)
-
-`bavapi` is a Python SDK for the WPP BAV API.
-
-With `bavapi` you can access the full BAV data catalog, the largest and most comprehensive database of brand data in the world.
-
-Queries are validated automatically thanks to `pydantic` and retrieved asynchronously via the `httpx` package.
-
-For more information about the API, go to the [WPPBAV Developer Hub](https://developer.wppbav.com).
-
-## Prerequisites
-
-`bavapi` requires Python 3.9 or higher to run.
-
-If you don't have Python installed, you can find it from the [official](https://www.python.org/downloads/) website or via [Anaconda](https://www.anaconda.com/).
-
-You will also need a BAV API token. For more information, go to the [Authentication](https://developer.wppbav.com/docs/2.x/authentication) section of the API documentation.
-
-### Dependencies
-
-- `httpx >= 0.20`
-- `nest-asyncio >= 1.5.6`
-- `pandas >= 0.16.2`
-- `pydantic >= 1.10, < 2.0`
-- `tqdm >= 4.62`
-- `typing-extensions >= 3.10` for Python 3.9
-
-## Installation
-
-`bavapi` can be installed using `pip`.
-
-```prompt
-pip install wpp-bavapi
-```
-
-### Installing from source
-
-To install from source, clone the GitHub repository into your local machine:
-
-```prompt
-git clone https://github.com/wppbav/bavapi-sdk-python.git
-```
-
-Go into the cloned directory and install `bavapi`:
-
-```prompt
-cd bavapi-sdk-python
-pip install .
-```
-
-## Usage
-
-Once you have acquired a token, you can start using this library directly in python or in a Jupyter Notebook:
-
-```py
->>> import bavapi
->>> result = bavapi.brands("TOKEN", name="Swatch")  # Replace `"TOKEN"` with your BAV API token
->>> result
-```
-
-|     | sector_id | sector_name           |  id | name   | ... |
-| --: | --------: | --------------------- | --: | ------ | --- |
-|   0 |        11 | Apparel & Accessories | 342 | Swatch | ... |
-| ... |       ... | ...                   | ... | ...    | ... |
-
-## Features
-
-- Support for all endpoints in the Fount API. Extended support for the `audiences`, `brands`, `brandscape-data` and `studies` endpoints.
-  - Other endpoints are available via the `raw_query` functions and methods.
-- Validates query parameters are of the correct types.
-  - Provides type hints for better IDE support.
-- Retrieve multiple pages of data simultaneously.
-  - Monitors and prevents exceeding API rate limit.
-
-## Documentation
-
-Read more about `bavapi` in the [documentation](https://fountapi-documentation.vercel.app/).
-
-## Issues
-
-Please file an issue on GitHub [here](https://github.com/wppbav/bavapi-sdk-python/issues).
-
-## Contributing
-
-Please see the [Contributing](https://fountapi-documentation.vercel.app/contributing/) section of the documentation for more information.
+# BAV API Python SDK
+
+[![CI status](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
+[![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/nachomaiz/32196acdc05431cd2bc7a8c73a587a8d/raw/covbadge.json)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
+[![PyPI](https://img.shields.io/pypi/v/wpp-bavapi)](https://pypi.org/project/wpp-bavapi/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wpp-bavapi)
+](https://pypi.org/project/wpp-bavapi/)
+
+`bavapi` is a Python SDK for the WPP BAV API.
+
+It is published on [PyPI](https://pypi.org/project/wpp-bavapi/) as `wpp-bavapi`.
+
+With `bavapi` you can access the full BAV data catalog, the largest and most comprehensive database of brand data in the world.
+
+Queries are validated automatically thanks to `pydantic` and retrieved asynchronously via the `httpx` package.
+
+For more information about the API, go to the [WPPBAV Developer Hub](https://developer.wppbav.com).
+
+## Prerequisites
+
+`bavapi` requires Python 3.8 or higher to run.
+
+If you don't have Python installed, you can find it from the [official](https://www.python.org/downloads/) website or via [Anaconda](https://www.anaconda.com/).
+
+You will also need a BAV API token. For more information, go to the [Authentication](https://developer.wppbav.com/docs/2.x/authentication) section of the API documentation.
+
+### Dependencies
+
+- `httpx >= 0.20`
+- `nest-asyncio >= 1.5.6`
+- `pandas >= 0.16.2`
+- `pydantic >= 1.10, < 2.0`
+- `tqdm >= 4.62`
+- `typing-extensions >= 3.10` for Python < 3.10
+
+## Installation
+
+`bavapi` can be installed using `pip`:
+
+```prompt
+pip install wpp-bavapi
+```
+
+### Installing from source
+
+To install from source, clone the GitHub repository into your local machine:
+
+```prompt
+git clone https://github.com/wppbav/bavapi-sdk-python.git
+```
+
+Go into the cloned directory and install `bavapi`:
+
+```prompt
+cd bavapi-sdk-python
+pip install .
+```
+
+## Usage
+
+Once you have acquired a token, you can start using this library directly in python or in a Jupyter Notebook:
+
+```py
+>>> import bavapi
+>>> result = bavapi.brands("TOKEN", name="Swatch")  # Replace `"TOKEN"` with your BAV API token
+>>> result
+```
+
+|     | sector_id | sector_name           | id   | name   | ... |
+| --: | :-------- | :-------------------- | :--- | :----- | :-- |
+|   0 | 233       | Apparel & Accessories | 8635 | Swatch | ... |
+| ... | ...       | ...                   | ...  | ...    | ... |
+
+## Features
+
+- Support for all endpoints in the Fount API. Extended support for the `audiences`, `brands`, `brandscape-data` and `studies` endpoints.
+  - Other endpoints are available via the `raw_query` functions and methods.
+- Validates query parameters are of the correct types.
+  - Provides type hints for better IDE support.
+- Retrieve multiple pages of data simultaneously.
+  - Monitors and prevents exceeding API rate limit.
+- Both synchronous and asynchronous APIs for accessing BAV data.
+
+## Documentation
+
+Read more about `bavapi` in the [documentation](https://fountapi-documentation.vercel.app/).
+
+## Issues
+
+Please file an issue on GitHub [here](https://github.com/wppbav/bavapi-sdk-python/issues).
+
+## Contributing
+
+Please see the [Contributing](https://fountapi-documentation.vercel.app/contributing/) section of the documentation for more information.
```

### Comparing `wpp-bavapi-0.4.1/bavapi/client.py` & `wpp-bavapi-0.5.0/bavapi/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,603 +1,580 @@
-"""Fount API interface."""
-
-# pylint: disable=too-many-arguments
-
-from typing import TYPE_CHECKING, Final, Literal, Optional, TypeVar, Union, overload
-
-from bavapi import filters as _filters
-from bavapi import parsing as _parsing
-from bavapi.http import HTTPClient
-from bavapi.query import Query
-from bavapi.typing import BaseListOrValues, JSONDict, OptionalListOr
-
-if TYPE_CHECKING:
-    from pandas import DataFrame
-
-__all__ = ("Client",)
-
-BASE_URL: Final[str] = "https://fount.wppbav.com/api/v2/"
-
-F = TypeVar("F", bound=_filters.FountFilters)
-
-OptionalFiltersOrMapping = Optional[_filters.FiltersOrMapping[F]]
-
-
-class Client:
-    """Asynchronous API to interact with the WPPBAV Fount.
-
-    This class uses `asyncio` to perform asynchronous requests to the Fount API.
-
-    Asynchronous requests allow you to make multiple requests at the same time,
-    extremely helpful for working with a paginated API like the Fount. (returns
-    data in multiple pages or requests instead of one single download)
-
-    To use the Client class, you will need to precede calls with `await`:
-
-    ```python
-    fount = Client("TOKEN")  # creating instance does not use `await`
-    data = await fount.brands("Swatch")  # must use `await`
-    ```
-
-    For more information, see the `asyncio` documentation for Python.
-
-    Either `auth_token` or `client` are required to instantiate a Client.
-
-    Parameters
-    ----------
-    auth_token : str, optional
-        Fount API authorization token, by default `''`
-    per_page : int, optional
-        Default number of entries per page, by default 100
-    timeout : float, optional
-        Maximum timeout for requests in seconds, by default 30.0
-    verify : bool or str, optional
-        Verify SSL credentials, by default True
-
-        Also accepts a path string to an SSL certificate file.
-    client : HTTPClient, optional
-        Authenticated async client from `bavapi.http`, by default None
-
-    Raises
-    ------
-    ValueError
-        If neither `auth_token` nor `client` are provided
-
-    Examples
-    --------
-    There are two main ways to use Client:
-
-    1. Using it in a `with` statement (`async with` since Client is async-based).
-
-    This is the recommended usage. Ideally you want to use Client to get some data,
-    close the connection, and continue your analysis.
-
-    The benefits of this approach are:
-
-    - The client can reuse one single connection for multiple requests, which brings
-    significant performance gains.
-    - The client pattern ensures the HTTP connection is closed when the request(s)
-    are finished.
-
-    >>> async with Client("TOKEN") as fount:
-    ...     data = await fount.brands("Swatch")
-
-    When the `with` block ends, the Client instance will close the connection, and
-    you will have to create a new instance of Client to use it again:
-
-    >>> fount = Client("TOKEN")
-    >>> async with fount as fount:
-    ...     data = await fount.brands("Swatch")  # ok
-    ... ...
-    >>> data = await fount.brands("Swatch")  # error, with block is already closed
-    >>> # create new instance to make a new request
-    >>> async with Client("TOKEN") as fount:
-    ...     data = await fount.brands("Swatch")  # should work again
-
-    2. Calling its methods as you would with any other class.
-    This will work, but is not ideal as it misses some of the benefits of using the
-    `with` version.
-
-    >>> fount = Client("TOKEN")
-    >>> data = await fount.brands("Swatch")
-    >>> data2 = await fount.brands("Facebook")  # still works
-
-    Calling the last two lines in the same file or Jupyter notebook cell may reuse
-    the HTTP connection (connections will remain open for 5s), but otherwise
-    will open a new connection for each call. It is also possible that the
-    connection remains open, and this pattern won't ensure that it is closed.
-
-    To close all open connections, you can use the `aclose` method:
-
-    >>> await fount.aclose()  # will close all connections
-    """
-
-    @overload
-    def __init__(self, auth_token: str) -> None:
-        ...
-
-    @overload
-    def __init__(
-        self,
-        auth_token: str,
-        per_page: int = 100,
-        timeout: float = 30.0,
-        verify: Union[bool, str] = True,
-    ) -> None:
-        ...
-
-    @overload
-    def __init__(
-        self,
-        *,
-        client: HTTPClient = ...,
-        per_page: int = 100,
-    ) -> None:
-        ...
-
-    def __init__(
-        self,
-        auth_token: str = "",
-        per_page: int = 100,
-        timeout: float = 30.0,
-        verify: Union[bool, str] = True,
-        *,
-        client: Optional[HTTPClient] = None,
-    ) -> None:
-        if client is not None:
-            self._client = client
-        else:
-            if not auth_token:
-                raise ValueError("You must provide `auth_token` or `client`.")
-            self._client = HTTPClient(
-                base_url=BASE_URL,
-                per_page=per_page,
-                timeout=timeout,
-                verify=verify,
-                headers={
-                    "Authorization": f"Bearer {auth_token}",
-                    "Accept": "application/json",
-                },
-            )
-
-    @property
-    def per_page(self) -> int:
-        """Default number of items to retrieve per page."""
-        return self._client.per_page
-
-    @per_page.setter
-    def per_page(self, value: int) -> None:
-        self._client.per_page = value
-
-    async def __aenter__(self) -> "Client":
-        await self._client.__aenter__()
-        return self
-
-    async def __aexit__(self, *args, **kwargs):
-        await self._client.__aexit__(*args, **kwargs)
-
-    async def aclose(self) -> None:
-        """Close existing HTTP connections."""
-        return await self._client.aclose()
-
-    async def raw_query(self, endpoint: str, params: Query[F]) -> list[JSONDict]:
-        """Perform a raw GET query to the Fount API, returning the response JSON data
-        instead of a `pandas` DataFrame.
-
-        Parameters
-        ----------
-        endpoint : str
-            Endpoint name
-        params : Query
-            Query `pydantic` model with query parameters.
-
-        Returns
-        -------
-        list[dict[str, Any]]
-            List of JSON response data
-        """
-        return list(await self._client.query(endpoint, params))
-
-    async def audiences(
-        self,
-        name: Optional[str] = None,
-        audience_id: Optional[int] = None,
-        active: Literal[0, 1] = 0,
-        inactive: Literal[0, 1] = 0,
-        public: Literal[0, 1] = 0,
-        private: Literal[0, 1] = 0,
-        groups: OptionalListOr[int] = None,
-        *,
-        filters: OptionalFiltersOrMapping[_filters.AudiencesFilters] = None,
-        fields: OptionalListOr[str] = None,
-        include: OptionalListOr[str] = None,
-        stack_data: bool = False,
-        **kwargs: BaseListOrValues,
-    ) -> "DataFrame":
-        """Query the Fount `audiences` endpoint.
-
-        Parameters
-        ----------
-        name : str, optional
-            Search audiences by name, by default None
-        audience_id : int, optional
-            Fount audience ID, by default None
-
-            If an audience ID is provided, only that audience will be returned
-        active : Literal[0, 1]
-            Return active audiences only if set to `1`, by default 0
-        inactive : Literal[0, 1]
-            Return inactive audiences only if set to `1`, by default 0
-        public : Literal[0, 1]
-            Return active audiences only if set to `1`, by default 0
-        private : Literal[0, 1]
-            Return inactive audiences only if set to `1`, by default 0
-        groups : int or list[int], optional
-            Audience group ID or list of audience group IDs, by default None
-        filters : AudiencesFilters or dict of filters, optional
-            AudiencesFilters object or dictionary of filter parameters, by default None
-        fields : str or list[str], optional
-            Fields to retrieve in API response, by default None
-
-            Only specified fields are returned.
-            If `fields` is None, all fields are returned.
-        include : str or list[str], optional
-            Additional resources to include in API response, by default None
-        stack_data : bool, optional
-            Whether to expand nested lists into new dictionaries, by default False
-        **kwargs
-            Additional parameters to pass to the Query. See `Other Parameters`.
-            For any filters, use the `filters` parameter.
-
-        Other Parameters
-        ----------------
-        page : int, optional
-            Page number to fetch, by default None
-        per_page : int, optional
-            Number of results per page, by default None
-        max_pages : int, optional
-            Max number of results to return, by default None
-        sort : str, optional
-            Sort response by field, by default None
-
-            To sort in descending (highest first) order, use a `-` before the field name:
-
-            `sort="-differentiation_rank"`
-
-            Sorts by item ID by default.
-
-        Returns
-        -------
-        pandas.DataFrame
-            DataFrame with `brands` endpoint results.
-        """
-
-        filters = _filters.AudiencesFilters.ensure(
-            filters,
-            name=name,
-            active=active,
-            inactive=inactive,
-            public=public,
-            private=private,
-            groups=groups,
-        )
-
-        query: Query[_filters.AudiencesFilters] = Query(
-            id=audience_id,
-            filters=filters,
-            fields=fields,
-            include=include,
-            **kwargs,  # type: ignore[arg-type]
-        )
-
-        items = await self._client.query("audiences", query)
-
-        return _parsing.responses.parse_response(items, expand=stack_data)
-
-    async def brands(
-        self,
-        name: Optional[str] = None,
-        country_codes: OptionalListOr[str] = None,
-        year_numbers: OptionalListOr[int] = None,
-        brand_id: Optional[int] = None,
-        studies: OptionalListOr[int] = None,
-        *,
-        filters: OptionalFiltersOrMapping[_filters.BrandsFilters] = None,
-        fields: OptionalListOr[str] = None,
-        include: OptionalListOr[str] = None,
-        stack_data: bool = False,
-        **kwargs: BaseListOrValues,
-    ) -> "DataFrame":
-        """Query the Fount `brands` endpoint.
-
-        Parameters
-        ----------
-        name : str, optional
-            Search brands by name, by default None
-        country_codes: str or list[str], optional
-            ISO-3166-1 alpha-2 country codes, by default None
-        year_numbers : int or list[int], optional
-            Study years, by default None
-        brand_id : int, optional
-            Fount brand ID, by default None
-
-            If a brand ID is provided, only that brand will be returned
-        studies : int or list[int], optional
-            Fount study IDs, by default None
-        filters : BrandsFilters or dict of filters, optional
-            BrandsFilters object or dictionary of filter parameters, by default None
-        fields : str or list[str], optional
-            Fields to retrieve in API response, by default None
-
-            Only specified fields are returned.
-            If `fields` is None, all fields are returned.
-        include : str or list[str], optional
-            Additional resources to include in API response, by default None
-        stack_data : bool, optional
-            Whether to expand nested lists into new dictionaries, by default False
-        **kwargs
-            Additional parameters to pass to the Query. See `Other Parameters`.
-            For any filters, use the `filters` parameter.
-
-        Other Parameters
-        ----------------
-        page : int, optional
-            Page number to fetch, by default None
-        per_page : int, optional
-            Number of results per page, by default None
-        max_pages : int, optional
-            Max number of results to return, by default None
-        sort : str, optional
-            Sort response by field, by default None
-
-            To sort in descending (highest first) order, use a `-` before the field name:
-
-            `sort="-differentiation_rank"`
-
-            Sorts by item ID by default.
-
-        Returns
-        -------
-        pandas.DataFrame
-            DataFrame with `brands` endpoint results.
-        """
-
-        filters = _filters.BrandsFilters.ensure(
-            filters,
-            name=name,
-            country_codes=country_codes,
-            year_numbers=year_numbers,
-            studies=studies,
-        )
-
-        query: Query[_filters.BrandsFilters] = Query(
-            id=brand_id,
-            filters=filters,
-            fields=fields,
-            include=include,
-            **kwargs,  # type: ignore[arg-type]
-        )
-
-        items = await self._client.query("brands", query)
-
-        return _parsing.responses.parse_response(items, expand=stack_data)
-
-    async def brandscape_data(
-        self,
-        country_code: OptionalListOr[str] = None,
-        year_number: OptionalListOr[int] = None,
-        audiences: OptionalListOr[int] = None,
-        brand_name: Optional[str] = None,
-        studies: OptionalListOr[int] = None,
-        *,
-        filters: OptionalFiltersOrMapping[_filters.BrandscapeFilters] = None,
-        fields: OptionalListOr[str] = None,
-        include: OptionalListOr[str] = None,
-        metric_keys: OptionalListOr[str] = None,
-        stack_data: bool = False,
-        **kwargs: BaseListOrValues,
-    ) -> "DataFrame":
-        """Query the Fount `brandscape-data` endpoint.
-
-        This endpoint requires at least one of the following combinations of parameters:
-
-        - `studies`
-        - `brand_name`
-        - `brands`
-        - `year_number` and `brands`/`brand_name`
-        - `country_code` and `brands`/`brand_name`
-        - `year_number` and `country_code`
-
-        An audience filter is also highly recommended, as otherwise the API will return
-        data for all audiences (there are more than 30 standard audiences).
-
-        The `Audiences` class is provided to make it easier to filter audiences.
-
-        Note that this endpoint has a default set of `include` resources:
-        - `brand`
-        - `study`
-        - `category`
-        - `audience`
-
-        Any additional valid includes will be added to the default set.
-
-        If any of the default includes are used in `include`, then only that resource
-        will be retrieved. This is to allow requesting individual includes if they are
-        part of the default.
-
-        Parameters
-        ----------
-        country_code : str or list[str], optional
-            ISO-3166-1 alpha-2 country codes, by default None
-        year_number : int or list[int], optional
-            Study years, by default None
-        audiences : int or list[int], optional
-            Audiences to retrieve by audience ID, by default None
-
-            The `Audiences` class can help with this filter.
-        brand_name : str, optional
-            Search by brand name, by default None
-        studies : int or list[int], optional
-            Fount studies IDs, by default None
-        filters : BrandscapeFilters or dict of filters, optional
-            BrandscapeFilters object or dictionary of filter parameters, by default None
-        fields : str or list[str], optional
-            Fields to retrieve in API response, by default None
-
-            Only specified fields are returned.
-            If `fields` is None, all fields are returned.
-        include : str or list[str], optional
-            Additional resources to include in API response, by default None
-        stack_data : bool, optional
-            Whether to expand nested lists into new dictionaries, by default False
-        **kwargs
-            Additional parameters to pass to the Query. See `Other Parameters`.
-            For any filters, use the `filters` parameter.
-
-        Other Parameters
-        ----------------
-        page : int, optional
-            Page number to fetch, by default None
-        per_page : int, optional
-            Number of results per page, by default None
-        max_pages : int, optional
-            Max number of results to return, by default None
-        sort : str, optional
-            Sort response by field, by default None
-
-            To sort in descending (highest first) order, use a `-` before the field name:
-
-            `sort="-differentiation_rank"`
-
-            Sorts by item ID by default.
-
-        Returns
-        -------
-        pandas.DataFrame
-            DataFrame with `brandscape-data` endpoint results.
-
-        Raises
-        ------
-        ValidationError
-            If used with an invalid combination of parameters (see above)
-        """
-
-        filters = _filters.BrandscapeFilters.ensure(
-            filters,
-            country_code=country_code,
-            year_number=year_number,
-            audiences=audiences,
-            brand_name=brand_name,
-            studies=studies,
-            metric_keys=metric_keys,
-        )
-
-        query: Query[_filters.BrandscapeFilters] = Query(
-            filters=filters,
-            fields=fields,
-            include=_default_brandscape_include(include),
-            **kwargs,  # type: ignore[arg-type]
-        )
-
-        items = await self._client.query("brandscape-data", query)
-
-        # Prefix 'global' to avoid clashing with 'brand_name' on 'brand' includes
-        return _parsing.responses.parse_response(items, "global", expand=stack_data)
-
-    async def studies(
-        self,
-        country_codes: OptionalListOr[str] = None,
-        year_numbers: OptionalListOr[int] = None,
-        full_year: Literal[0, 1] = 0,
-        study_id: Optional[int] = None,
-        *,
-        filters: OptionalFiltersOrMapping[_filters.StudiesFilters] = None,
-        fields: OptionalListOr[str] = None,
-        include: OptionalListOr[str] = None,
-        stack_data: bool = False,
-        **kwargs: BaseListOrValues,
-    ) -> "DataFrame":
-        """Query the Fount `studies` endpoint.
-
-        Parameters
-        ----------
-        country_codes: str or list[str], optional
-            ISO-3166-1 alpha-2 country codes, by default None
-        year_numbers : int or list[int], optional
-            Study years, by default None
-        full_year : Literal[0, 1], optional
-            Include or exclude studies which are not "full year" studies,
-            such as US quarterly studies or special studies, by default 0
-
-            A value of 1 will filter non-full-year studies.
-        study_id : int, optional
-            Fount study ID, by default None
-            If a study ID is provided, only that study will be returned
-        filters : StudiesFilters or dict of filters, optional
-            StudiesFilters object or dictionary of filter parameters, by default None
-        fields : str or list[str], optional
-            Fields to retrieve in API response, by default None
-
-            Only specified fields are returned.
-            If `fields` is None, all fields are returned.
-        include : str or list[str], optional
-            Additional resources to include in API response, by default None
-        stack_data : bool, optional
-            Whether to expand nested lists into new dictionaries, by default False
-        **kwargs
-            Additional parameters to pass to the Query. See `Other Parameters`.
-            For any filters, use the `filters` parameter.
-
-        Other Parameters
-        ----------------
-        page : int, optional
-            Page number to fetch, by default None
-        per_page : int, optional
-            Number of results per page, by default None
-        max_pages : int, optional
-            Max number of results to return, by default None
-        sort : str, optional
-            Sort response by field, by default None
-
-            To sort in descending (highest first) order, use a `-` before the field name:
-
-            `sort="-differentiation_rank"`
-
-            Sorts by item ID by default.
-
-        Returns
-        -------
-        pandas.DataFrame
-            DataFrame with `studies` endpoint results.
-        """
-        filters = _filters.StudiesFilters.ensure(
-            filters,
-            country_codes=country_codes,
-            year_numbers=year_numbers,
-            full_year=full_year,
-        )
-
-        query: Query[_filters.StudiesFilters] = Query(
-            id=study_id,
-            filters=filters,
-            fields=fields,
-            include=include,
-            **kwargs,  # type: ignore[arg-type]
-        )
-
-        items = await self._client.query("studies", query)
-
-        return _parsing.responses.parse_response(items, expand=stack_data)
-
-
-def _default_brandscape_include(value: OptionalListOr[str]) -> OptionalListOr[str]:
-    default: Final[list[str]] = ["study", "brand", "category", "audience"]
-
-    if value is None:
-        return default
-    if isinstance(value, list):
-        return list(set(default).union(value))
-    if value == "no_default":
-        return None
-    if value in default:
-        return value
-    return list(set(default).union((value,)))
+"""Fount API interface."""
+
+# pylint: disable=too-many-arguments
+
+from typing import (
+    TYPE_CHECKING,
+    Final,
+    List,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+    overload,
+)
+
+from bavapi import filters as _filters
+from bavapi.http import HTTPClient
+from bavapi.parsing.responses import parse_response
+from bavapi.query import Query
+from bavapi.typing import BaseListOrValues, JSONDict, OptionalListOr
+
+if TYPE_CHECKING:
+    from pandas import DataFrame
+
+__all__ = ("Client",)
+
+BASE_URL: Final[str] = "https://fount.wppbav.com/api/v2/"
+
+F = TypeVar("F", bound=_filters.FountFilters)
+
+OptionalFiltersOrMapping = Optional[_filters.FiltersOrMapping[F]]
+
+
+class Client:
+    """Asynchronous API to interact with the WPPBAV Fount.
+
+    This class uses `asyncio` to perform asynchronous requests to the Fount API.
+
+    Asynchronous requests allow you to make multiple requests at the same time,
+    extremely helpful for working with a paginated API like the Fount. (returns
+    data in multiple pages or requests instead of one single download)
+
+    To use the Client class, you will need to precede calls with `await`:
+
+    ```python
+    fount = Client("TOKEN")  # creating instance does not use `await`
+    data = await fount.brands("Swatch")  # must use `await`
+    ```
+
+    For more information, see the `asyncio` documentation for Python.
+
+    Either `auth_token` or `client` are required to instantiate a Client.
+
+    Parameters
+    ----------
+    auth_token : str, optional
+        Fount API authorization token, by default `''`
+    per_page : int, optional
+        Default number of entries per page, by default 100
+    timeout : float, optional
+        Maximum timeout for requests in seconds, by default 30.0
+    verify : bool or str, optional
+        Verify SSL credentials, by default True
+
+        Also accepts a path string to an SSL certificate file.
+    client : HTTPClient, optional
+        Authenticated async client from `bavapi.http`, by default None
+
+    Raises
+    ------
+    ValueError
+        If neither `auth_token` nor `client` are provided
+
+    Examples
+    --------
+    Use `async with` to get data and close the connection.
+
+    This way you get the benefits from `httpx` speed improvements
+    and closes the connection when exiting the async with block.
+
+    >>> async with Client("TOKEN") as fount:
+    ...     data = await fount.brands("Swatch")
+
+    When not using `async with`, close the connection manually by awaiting `aclose`.
+
+    >>> client = Client("TOKEN")
+    >>> data = await fount.brands("Swatch")
+    >>> await client.aclose()
+    """
+
+    @overload
+    def __init__(self, auth_token: str) -> None:
+        ...
+
+    @overload
+    def __init__(
+        self,
+        auth_token: str,
+        per_page: int = 100,
+        timeout: float = 30.0,
+        verify: Union[bool, str] = True,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *,
+        client: HTTPClient = ...,
+        per_page: int = 100,
+    ) -> None:
+        ...
+
+    def __init__(
+        self,
+        auth_token: str = "",
+        per_page: int = 100,
+        timeout: float = 30.0,
+        verify: Union[bool, str] = True,
+        *,
+        client: Optional[HTTPClient] = None,
+    ) -> None:
+        if client is not None:
+            self._client = client
+        else:
+            if not auth_token:
+                raise ValueError("You must provide `auth_token` or `client`.")
+            self._client = HTTPClient(
+                base_url=BASE_URL,
+                per_page=per_page,
+                timeout=timeout,
+                verify=verify,
+                headers={
+                    "Authorization": f"Bearer {auth_token}",
+                    "Accept": "application/json",
+                },
+            )
+
+    @property
+    def per_page(self) -> int:
+        """Default number of items to retrieve per page."""
+        return self._client.per_page
+
+    @per_page.setter
+    def per_page(self, value: int) -> None:
+        self._client.per_page = value
+
+    async def __aenter__(self) -> "Client":
+        await self._client.__aenter__()
+        return self
+
+    async def __aexit__(self, *args, **kwargs):
+        await self._client.__aexit__(*args, **kwargs)
+
+    async def aclose(self) -> None:
+        """Close existing HTTP connections."""
+        return await self._client.aclose()
+
+    async def raw_query(self, endpoint: str, params: Query[F]) -> List[JSONDict]:
+        """Perform a raw GET query to the Fount API, returning the response JSON data
+        instead of a `pandas` DataFrame.
+
+        Parameters
+        ----------
+        endpoint : str
+            Endpoint name
+        params : Query
+            Query `pydantic` model with query parameters.
+
+        Returns
+        -------
+        list[dict[str, Any]]
+            List of JSON response data
+        """
+        return list(await self._client.query(endpoint, params))
+
+    async def audiences(
+        self,
+        name: Optional[str] = None,
+        audience_id: Optional[int] = None,
+        active: Literal[0, 1] = 0,
+        inactive: Literal[0, 1] = 0,
+        public: Literal[0, 1] = 0,
+        private: Literal[0, 1] = 0,
+        groups: OptionalListOr[int] = None,
+        *,
+        filters: OptionalFiltersOrMapping[_filters.AudiencesFilters] = None,
+        fields: OptionalListOr[str] = None,
+        include: OptionalListOr[str] = None,
+        stack_data: bool = False,
+        **kwargs: BaseListOrValues,
+    ) -> "DataFrame":
+        """Query the Fount `audiences` endpoint.
+
+        Parameters
+        ----------
+        name : str, optional
+            Search audiences by name, by default None
+        audience_id : int, optional
+            Fount audience ID, by default None
+
+            If an audience ID is provided, only that audience will be returned
+        active : Literal[0, 1]
+            Return active audiences only if set to `1`, by default 0
+        inactive : Literal[0, 1]
+            Return inactive audiences only if set to `1`, by default 0
+        public : Literal[0, 1]
+            Return active audiences only if set to `1`, by default 0
+        private : Literal[0, 1]
+            Return inactive audiences only if set to `1`, by default 0
+        groups : int or list[int], optional
+            Audience group ID or list of audience group IDs, by default None
+        filters : AudiencesFilters or dict of filters, optional
+            AudiencesFilters object or dictionary of filter parameters, by default None
+        fields : str or list[str], optional
+            Fields to retrieve in API response, by default None
+
+            Only specified fields are returned.
+            If `fields` is None, all fields are returned.
+        include : str or list[str], optional
+            Additional resources to include in API response, by default None
+        stack_data : bool, optional
+            Whether to expand nested lists into new dictionaries, by default False
+        **kwargs
+            Additional parameters to pass to the Query. See `Other Parameters`.
+            For any filters, use the `filters` parameter.
+
+        Other Parameters
+        ----------------
+        page : int, optional
+            Page number to fetch, by default None
+        per_page : int, optional
+            Number of results per page, by default None
+        max_pages : int, optional
+            Max number of results to return, by default None
+        sort : str, optional
+            Sort response by field, by default None
+
+            To sort in descending (highest first) order, use a `-` before the field name:
+
+            `sort="-differentiation_rank"`
+
+            Sorts by item ID by default.
+
+        Returns
+        -------
+        pandas.DataFrame
+            DataFrame with `brands` endpoint results.
+        """
+
+        filters = _filters.AudiencesFilters.ensure(
+            filters,
+            name=name,
+            active=active,
+            inactive=inactive,
+            public=public,
+            private=private,
+            groups=groups,
+        )
+
+        query: Query[_filters.AudiencesFilters] = Query(
+            id=audience_id,
+            filters=filters,
+            fields=fields,
+            include=include,
+            **kwargs,  # type: ignore[arg-type]
+        )
+
+        items = await self._client.query("audiences", query)
+
+        return parse_response(items, expand=stack_data)
+
+    async def brands(
+        self,
+        name: Optional[str] = None,
+        country_codes: OptionalListOr[str] = None,
+        year_numbers: OptionalListOr[int] = None,
+        brand_id: Optional[int] = None,
+        studies: OptionalListOr[int] = None,
+        *,
+        filters: OptionalFiltersOrMapping[_filters.BrandsFilters] = None,
+        fields: OptionalListOr[str] = None,
+        include: OptionalListOr[str] = None,
+        stack_data: bool = False,
+        **kwargs: BaseListOrValues,
+    ) -> "DataFrame":
+        """Query the Fount `brands` endpoint.
+
+        Parameters
+        ----------
+        name : str, optional
+            Search brands by name, by default None
+        country_codes: str or list[str], optional
+            ISO-3166-1 alpha-2 country codes, by default None
+        year_numbers : int or list[int], optional
+            Study years, by default None
+        brand_id : int, optional
+            Fount brand ID, by default None
+
+            If a brand ID is provided, only that brand will be returned
+        studies : int or list[int], optional
+            Fount study IDs, by default None
+        filters : BrandsFilters or dict of filters, optional
+            BrandsFilters object or dictionary of filter parameters, by default None
+        fields : str or list[str], optional
+            Fields to retrieve in API response, by default None
+
+            Only specified fields are returned.
+            If `fields` is None, all fields are returned.
+        include : str or list[str], optional
+            Additional resources to include in API response, by default None
+        stack_data : bool, optional
+            Whether to expand nested lists into new dictionaries, by default False
+        **kwargs
+            Additional parameters to pass to the Query. See `Other Parameters`.
+            For any filters, use the `filters` parameter.
+
+        Other Parameters
+        ----------------
+        page : int, optional
+            Page number to fetch, by default None
+        per_page : int, optional
+            Number of results per page, by default None
+        max_pages : int, optional
+            Max number of results to return, by default None
+        sort : str, optional
+            Sort response by field, by default None
+
+            To sort in descending (highest first) order, use a `-` before the field name:
+
+            `sort="-differentiation_rank"`
+
+            Sorts by item ID by default.
+
+        Returns
+        -------
+        pandas.DataFrame
+            DataFrame with `brands` endpoint results.
+        """
+
+        filters = _filters.BrandsFilters.ensure(
+            filters,
+            name=name,
+            country_codes=country_codes,
+            year_numbers=year_numbers,
+            studies=studies,
+        )
+
+        query: Query[_filters.BrandsFilters] = Query(
+            id=brand_id,
+            filters=filters,
+            fields=fields,
+            include=include,
+            **kwargs,  # type: ignore[arg-type]
+        )
+
+        items = await self._client.query("brands", query)
+
+        return parse_response(items, expand=stack_data)
+
+    async def brandscape_data(
+        self,
+        country_code: OptionalListOr[str] = None,
+        year_number: OptionalListOr[int] = None,
+        audiences: OptionalListOr[int] = None,
+        brand_name: Optional[str] = None,
+        studies: OptionalListOr[int] = None,
+        *,
+        filters: OptionalFiltersOrMapping[_filters.BrandscapeFilters] = None,
+        fields: OptionalListOr[str] = None,
+        include: OptionalListOr[str] = None,
+        metric_keys: OptionalListOr[str] = None,
+        stack_data: bool = False,
+        **kwargs: BaseListOrValues,
+    ) -> "DataFrame":
+        """Query the Fount `brandscape-data` endpoint.
+
+        This endpoint requires at least one of the following combinations of parameters:
+
+        - `studies`
+        - `brand_name`
+        - `brands`
+        - `year_number` and `brands`/`brand_name`
+        - `country_code` and `brands`/`brand_name`
+        - `year_number` and `country_code`
+
+        An audience filter is also highly recommended, as otherwise the API will return
+        data for all audiences (there are more than 30 standard audiences).
+
+        The `Audiences` class is provided to make it easier to filter audiences.
+
+        Note that this endpoint has a default set of `include` resources:
+        - `brand`
+        - `study`
+        - `category`
+        - `audience`
+
+        Any additional valid includes will be added to the default set.
+
+        If any of the default includes are used in `include`, then only that resource
+        will be retrieved. This is to allow requesting individual includes if they are
+        part of the default.
+
+        Parameters
+        ----------
+        country_code : str or list[str], optional
+            ISO-3166-1 alpha-2 country codes, by default None
+        year_number : int or list[int], optional
+            Study years, by default None
+        audiences : int or list[int], optional
+            Audiences to retrieve by audience ID, by default None
+
+            The `Audiences` class can help with this filter.
+        brand_name : str, optional
+            Search by brand name, by default None
+        studies : int or list[int], optional
+            Fount studies IDs, by default None
+        filters : BrandscapeFilters or dict of filters, optional
+            BrandscapeFilters object or dictionary of filter parameters, by default None
+        fields : str or list[str], optional
+            Fields to retrieve in API response, by default None
+
+            Only specified fields are returned.
+            If `fields` is None, all fields are returned.
+        include : str or list[str], optional
+            Additional resources to include in API response, by default None
+        stack_data : bool, optional
+            Whether to expand nested lists into new dictionaries, by default False
+        **kwargs
+            Additional parameters to pass to the Query. See `Other Parameters`.
+            For any filters, use the `filters` parameter.
+
+        Other Parameters
+        ----------------
+        page : int, optional
+            Page number to fetch, by default None
+        per_page : int, optional
+            Number of results per page, by default None
+        max_pages : int, optional
+            Max number of results to return, by default None
+        sort : str, optional
+            Sort response by field, by default None
+
+            To sort in descending (highest first) order, use a `-` before the field name:
+
+            `sort="-differentiation_rank"`
+
+            Sorts by item ID by default.
+
+        Returns
+        -------
+        pandas.DataFrame
+            DataFrame with `brandscape-data` endpoint results.
+
+        Raises
+        ------
+        ValidationError
+            If used with an invalid combination of parameters (see above)
+        """
+
+        filters = _filters.BrandscapeFilters.ensure(
+            filters,
+            country_code=country_code,
+            year_number=year_number,
+            audiences=audiences,
+            brand_name=brand_name,
+            studies=studies,
+            metric_keys=metric_keys,
+        )
+
+        query: Query[_filters.BrandscapeFilters] = Query(
+            filters=filters,
+            fields=fields,
+            include=_default_brandscape_include(include),
+            **kwargs,  # type: ignore[arg-type]
+        )
+
+        items = await self._client.query("brandscape-data", query)
+
+        # Prefix 'global' to avoid clashing with 'brand_name' on 'brand' includes
+        return parse_response(items, "global", expand=stack_data)
+
+    async def studies(
+        self,
+        country_codes: OptionalListOr[str] = None,
+        year_numbers: OptionalListOr[int] = None,
+        full_year: Literal[0, 1] = 0,
+        study_id: Optional[int] = None,
+        *,
+        filters: OptionalFiltersOrMapping[_filters.StudiesFilters] = None,
+        fields: OptionalListOr[str] = None,
+        include: OptionalListOr[str] = None,
+        stack_data: bool = False,
+        **kwargs: BaseListOrValues,
+    ) -> "DataFrame":
+        """Query the Fount `studies` endpoint.
+
+        Parameters
+        ----------
+        country_codes: str or list[str], optional
+            ISO-3166-1 alpha-2 country codes, by default None
+        year_numbers : int or list[int], optional
+            Study years, by default None
+        full_year : Literal[0, 1], optional
+            Include or exclude studies which are not "full year" studies,
+            such as US quarterly studies or special studies, by default 0
+
+            A value of 1 will filter non-full-year studies.
+        study_id : int, optional
+            Fount study ID, by default None
+            If a study ID is provided, only that study will be returned
+        filters : StudiesFilters or dict of filters, optional
+            StudiesFilters object or dictionary of filter parameters, by default None
+        fields : str or list[str], optional
+            Fields to retrieve in API response, by default None
+
+            Only specified fields are returned.
+            If `fields` is None, all fields are returned.
+        include : str or list[str], optional
+            Additional resources to include in API response, by default None
+        stack_data : bool, optional
+            Whether to expand nested lists into new dictionaries, by default False
+        **kwargs
+            Additional parameters to pass to the Query. See `Other Parameters`.
+            For any filters, use the `filters` parameter.
+
+        Other Parameters
+        ----------------
+        page : int, optional
+            Page number to fetch, by default None
+        per_page : int, optional
+            Number of results per page, by default None
+        max_pages : int, optional
+            Max number of results to return, by default None
+        sort : str, optional
+            Sort response by field, by default None
+
+            To sort in descending (highest first) order, use a `-` before the field name:
+
+            `sort="-differentiation_rank"`
+
+            Sorts by item ID by default.
+
+        Returns
+        -------
+        pandas.DataFrame
+            DataFrame with `studies` endpoint results.
+        """
+        filters = _filters.StudiesFilters.ensure(
+            filters,
+            country_codes=country_codes,
+            year_numbers=year_numbers,
+            full_year=full_year,
+        )
+
+        query: Query[_filters.StudiesFilters] = Query(
+            id=study_id,
+            filters=filters,
+            fields=fields,
+            include=include,
+            **kwargs,  # type: ignore[arg-type]
+        )
+
+        items = await self._client.query("studies", query)
+
+        return parse_response(items, expand=stack_data)
+
+
+def _default_brandscape_include(value: OptionalListOr[str]) -> OptionalListOr[str]:
+    default: Final[List[str]] = ["study", "brand", "category", "audience"]
+
+    if value is None:
+        return default
+    if isinstance(value, list):
+        return list(set(default).union(value))
+    if value == "no_default":
+        return None
+    if value in default:
+        return value
+    return list(set(default).union((value,)))
```

### Comparing `wpp-bavapi-0.4.1/bavapi/filters.py` & `wpp-bavapi-0.5.0/bavapi/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,319 +1,320 @@
-"""Filter objects for Fount API queries based on `pydantic`."""
-
-# pylint: disable=no-name-in-module, too-few-public-methods
-
-from typing import Literal, Mapping, Optional, TypeVar, Union
-
-from pydantic import BaseModel, root_validator, validator
-
-from bavapi.parsing.params import parse_date
-from bavapi.typing import (
-    DTValues,
-    InputParamsMapping,
-    InputSequenceOrValues,
-    OptionalListOr,
-)
-
-__all__ = (
-    "FountFilters",
-    "AudiencesFilters",
-    "BrandsFilters",
-    "BrandscapeFilters",
-    "StudiesFilters",
-)
-
-F = TypeVar("F", bound="FountFilters")
-
-FiltersOrMapping = Union[F, InputParamsMapping]
-
-
-class FountFilters(BaseModel):
-    """Base class for Fount API Filters.
-    
-    Can be used with `raw_query` endpoints.
-
-    Attributes
-    ----------
-    updated_since : str, date or datetime, optional
-        Request items that have been updated since the specified date, by default None
-    **kwargs : str, int or float, or list of str, int or floats, optional
-        Any additional filters to apply to the request, including for columns within
-        the response data.
-    """
-
-    updated_since: DTValues = None
-
-    class Config:
-        extra = "allow"
-
-    @validator("updated_since", pre=True)
-    @classmethod
-    def _parse_date(cls, value: DTValues) -> Optional[str]:
-        if value is None:
-            return value
-        return parse_date(value)
-
-    @classmethod
-    def ensure(
-        cls: type[F],
-        filters: Optional[FiltersOrMapping["FountFilters"]],
-        **addl_filters: InputSequenceOrValues,
-    ) -> Optional[F]:
-        """Ensure FountFilters class from dictionary or other FountFilters class.
-
-        If `filters` is None, return None.
-
-        Parameters
-        ----------
-        filters : FountFilters or dict of filter values, optional
-            Dictionary of filters or FountFilters class.
-        **addl_filters : SequenceOrValues, optional
-            Additional filters to add to the new FountFilters instance.
-
-        Returns
-        -------
-        FountFilters, optional
-            FountFilters class or None.
-        """
-        addl_filters = {k: v for k, v in addl_filters.items() if v}
-
-        if filters is None:
-            if not addl_filters:
-                return None
-            return cls(**addl_filters)  # type: ignore[arg-type]
-
-        if isinstance(filters, Mapping):
-            return cls(**(addl_filters | filters))  # type: ignore[arg-type]
-
-        return cls(
-            **addl_filters  # type: ignore[arg-type]
-            | filters.dict(exclude_defaults=True)
-        )
-
-
-class AudiencesFilters(FountFilters):
-    """Filters for the `brands` endpoint.
-
-    See <https://developer.wppbav.com/docs/2.x/core-resources/audiences>
-    for more info.
-
-    Attributes
-    ----------
-    active : Literal[0, 1], optional
-        Return active audiences only if set to `1`, by default 0
-    inactive : Literal[0, 1], optional
-        Return inactive audiences only if set to `1`, by default 0
-    public : Literal[0, 1], optional
-        Return active audiences only if set to `1`, by default 0
-    private : Literal[0, 1], optional
-        Return inactive audiences only if set to `1`, by default 0
-    groups : int or list[int], optional
-        Audience group ID or list of audience group IDs, by default None
-
-    Other Parameters
-    ----------------
-    updated_since : str, date or datetime, optional
-        Request items that have been updated since the specified date, by default None
-    """
-
-    active: Literal[0, 1] = 0
-    inactive: Literal[0, 1] = 0
-    public: Literal[0, 1] = 0
-    private: Literal[0, 1] = 0
-    groups: OptionalListOr[int] = None
-
-
-class BrandsFilters(FountFilters):
-    """Filters for the `brands` endpoint.
-
-    Filters other than `country_codes` and `year_numbers` filter by
-    the Fount IDs of the specific resources.
-
-    See <https://developer.wppbav.com/docs/2.x/core-resources/brands>
-    for more info.
-
-    Attributes
-    ----------
-    country_codes : str or list[str], optional
-        Two-letter ISO-3166 country code or list of country codes, by default None
-    year_numbers : int or list[int], optional
-        Study years in numerical format (not IDs), by default None
-    categories : int or list[int], optional
-        Fount category ID or list of category IDs, by default None
-    countries : int or list[int], optional
-        Fount country ID or list of country IDs, by default None
-    regions : int or list[int], optional
-        Fount region ID or list of region IDs, by default None
-    sectors : int or list[int], optional
-        Fount sector ID or list of sector IDs, by default None
-    studies : int or list[int], optional
-        Fount study ID or list of study IDs, by default None
-    years : int or list[int], optional
-        Fount year ID or list of year IDs, by default None
-
-    Other Parameters
-    ----------------
-    updated_since : str, date or datetime, optional
-        Request items that have been updated since the specified date, by default None
-    """
-
-    country_codes: OptionalListOr[str] = None
-    year_numbers: OptionalListOr[int] = None
-    categories: OptionalListOr[int] = None
-    countries: OptionalListOr[int] = None
-    regions: OptionalListOr[int] = None
-    sectors: OptionalListOr[int] = None
-    studies: OptionalListOr[int] = None
-    years: OptionalListOr[int] = None
-
-
-class BrandscapeFilters(FountFilters):
-    """Filters for the `studies` endpoint.
-
-    `audiences`, `countries`, `studies`, `years`, `brands` and `categories` filter by
-    the Fount IDs of the specific resources.
-
-    See <https://developer.wppbav.com/docs/2.x/core-resources/brandscape-data>
-    for more info.
-
-    The `brandscape-data` endpoint requires the use of, at minimum, these filters:
-
-    - `studies`
-    - `brand_name` or `brands`
-    - `country_code` or `countries` and `brands` or `brand_name`
-    - `year_number` or `years` and `country_code` or `countries`
-
-    An audience filter is also highly recommended, as otherwise the API will return
-    data for all audiences (there are more than 30 standard audiences).
-
-    The `Audiences` class is provided to make it easier to filter audiences.
-
-    Attributes
-    ----------
-    country_code : str or list[str], optional
-        Two-letter ISO-3166 country code or list of country codes, by default None
-    year_number : int or list[int], optional
-        Study years in numerical format (not IDs), by default None
-    audiences : int or list[int], optional
-        Fount ID of the desired audience, by default None
-
-        The `Audiences` class can help with using audience IDs.
-    brand_name : str, optional
-        Perform a search on the brand name, by default None
-    metric_keys : str or list[str], optional
-        Metric keys to return as columns, by default None
-    brands : int or list[int], optional
-        Fount brand ID or list of brand IDs, by default None
-    categories : int or list[int], optional
-        Fount category ID or list of category IDs, by default None
-    countries : int or list[int], optional
-        Fount country ID or list of country IDs, by default None
-
-        The `Countries` class can help with using country IDs.
-    studies : int or list[int], optional
-        Fount study ID or list of study IDs, by default None
-    years : int or list[int], optional
-        Fount year ID or list of year IDs, by default None
-
-
-    Other Parameters
-    ----------------
-    updated_since : str, date or datetime, optional
-        Request items that have been updated since the specified date, by default None
-    """
-
-    country_code: OptionalListOr[str] = None
-    year_number: OptionalListOr[int] = None
-    audiences: OptionalListOr[int] = None
-    brand_name: Optional[str] = None
-    metric_keys: OptionalListOr[str] = None
-    studies: OptionalListOr[int] = None
-    countries: OptionalListOr[int] = None
-    years: OptionalListOr[int] = None
-    brands: OptionalListOr[int] = None
-    categories: OptionalListOr[int] = None
-
-    @root_validator(pre=True)
-    @classmethod
-    def _check_params(cls, values: dict[str, object]) -> dict[str, object]:
-        if not (
-            "brands" in values
-            or "brand_name" in values
-            or "studies" in values
-            or (
-                ("country_code" in values or "countries" in values)
-                and ("year_number" in values or "years" in values)
-            )
-        ):
-            raise ValueError(
-                "You need to apply either the `brands`, or `studies`, or `brand_name` "
-                "filters, or the `country_code`/`countries` "
-                "and `year_number`/`years` filters together."
-            )
-
-        return values
-
-
-class StudiesFilters(FountFilters):
-    """Filters for the `studies` endpoint.
-
-    `years`, `countries` and `regions` filter by the Fount IDs of the specific resources.
-
-    See <https://developer.wppbav.com/docs/2.x/core-resources/studies>
-    for more info.
-
-    Attributes
-    ----------
-    country_codes: str or list[str], optional
-        Two-letter ISO-3166 country code or list of country codes, by default None
-    year_numbers: int or list[int], optional
-        Study years in numerical format (not IDs), by default None
-    full_year: Literal[0, 1], optional
-        Return full year studies when set to `1` (excludes US quarterly), by default 0
-    released: Literal[0, 1], optional
-        Return released studies when set to `1`, by default 0
-    unreleased: Literal[0, 1], optional
-        Return unreleased studies when set to `1`, by default 0
-    open_survey: Literal[0, 1], optional
-        Return studies with open brand requests when set to `1`, by default 0
-    active: Literal[0, 1], optional
-        Return active audiences when set to `1`, by default 0
-    inactive: Literal[0, 1], optional
-        Return inactive audiences when set to `1`, by default 0
-    bav_study: Literal[0, 1], optional
-        Return full BAV studies when set to `1`, by default 0
-    data_updated_since: DTValues, optional
-        Return studies updated since datetime value, by default None
-    countries: int or list[int], optional
-        Fount country ID or list of country IDs, by default None
-    regions: int or list[int], optional
-        Fount region ID or list of region IDs, by default None
-    years: int or list[int], optional
-        Fount year ID or list of year IDs, by default None
-
-    Other Parameters
-    ----------------
-    updated_since : str, date or datetime, optional
-        Request items that have been updated since the specified date, by default None
-    """
-
-    country_codes: OptionalListOr[str] = None
-    year_numbers: OptionalListOr[int] = None
-    full_year: Literal[0, 1] = 0
-    released: Literal[0, 1] = 0
-    unreleased: Literal[0, 1] = 0
-    open_survey: Literal[0, 1] = 0
-    active: Literal[0, 1] = 0
-    inactive: Literal[0, 1] = 0
-    bav_study: Literal[0, 1] = 0
-    data_updated_since: DTValues = None
-    years: OptionalListOr[int] = None
-    countries: OptionalListOr[int] = None
-    regions: OptionalListOr[int] = None
-
-    @validator("data_updated_since", pre=True)
-    @classmethod
-    def _parse_date(cls, value: DTValues) -> Optional[str]:
-        if value is None:
-            return value
-        return parse_date(value)
+"""Filter objects for Fount API queries based on `pydantic`."""
+
+# pylint: disable=no-name-in-module, too-few-public-methods
+
+from typing import Dict, Literal, Mapping, Optional, Type, TypeVar, Union
+
+from pydantic import BaseModel, root_validator, validator
+
+from bavapi.parsing.params import parse_date
+from bavapi.typing import (
+    DTValues,
+    InputParamsMapping,
+    InputSequenceOrValues,
+    OptionalListOr,
+)
+
+__all__ = (
+    "FountFilters",
+    "AudiencesFilters",
+    "BrandsFilters",
+    "BrandscapeFilters",
+    "StudiesFilters",
+)
+
+F = TypeVar("F", bound="FountFilters")
+
+FiltersOrMapping = Union[F, InputParamsMapping]
+
+
+class FountFilters(BaseModel):
+    """Base class for Fount API Filters.
+
+    Can be used with `raw_query` endpoints.
+
+    Attributes
+    ----------
+    updated_since : str, date or datetime, optional
+        Request items that have been updated since the specified date, by default None
+    **kwargs : str, int or float, or list of str, int or floats, optional
+        Any additional filters to apply to the request, including for columns within
+        the response data.
+    """
+
+    updated_since: DTValues = None
+
+    class Config:  #pylint: disable=missing-class-docstring
+        extra = "allow"
+
+    @validator("updated_since", pre=True)
+    @classmethod
+    def _parse_date(cls, value: DTValues) -> Optional[str]:
+        if value is None:
+            return value
+        return parse_date(value)
+
+    @classmethod
+    def ensure(
+        cls: Type[F],
+        filters: Optional[FiltersOrMapping["FountFilters"]],
+        **addl_filters: InputSequenceOrValues,
+    ) -> Optional[F]:
+        """Ensure FountFilters class from dictionary or other FountFilters class.
+
+        If `filters` is None, returns None.
+
+        Parameters
+        ----------
+        filters : FountFilters or dict of filter values, optional
+            Dictionary of filters or FountFilters class.
+        **addl_filters : SequenceOrValues, optional
+            Additional filters to add to the new FountFilters instance.
+
+        Returns
+        -------
+        FountFilters, optional
+            FountFilters class or None.
+        """
+        addl_filters = {k: v for k, v in addl_filters.items() if v}
+
+        if filters is None:
+            if not addl_filters:
+                return None
+            return cls(**addl_filters)  # type: ignore[arg-type]
+
+        new_filters = addl_filters.copy()
+
+        if isinstance(filters, Mapping):
+            new_filters.update(filters)
+        else:
+            new_filters.update(filters.dict(exclude_defaults=True))
+
+        return cls(**new_filters)  # type: ignore[arg-type]
+
+
+class AudiencesFilters(FountFilters):
+    """Filters for the `brands` endpoint.
+
+    See <https://developer.wppbav.com/docs/2.x/core-resources/audiences>
+    for more info.
+
+    Attributes
+    ----------
+    active : Literal[0, 1], optional
+        Return active audiences only if set to `1`, by default 0
+    inactive : Literal[0, 1], optional
+        Return inactive audiences only if set to `1`, by default 0
+    public : Literal[0, 1], optional
+        Return active audiences only if set to `1`, by default 0
+    private : Literal[0, 1], optional
+        Return inactive audiences only if set to `1`, by default 0
+    groups : int or list[int], optional
+        Audience group ID or list of audience group IDs, by default None
+
+    Other Parameters
+    ----------------
+    updated_since : str, date or datetime, optional
+        Request items that have been updated since the specified date, by default None
+    """
+
+    active: Literal[0, 1] = 0
+    inactive: Literal[0, 1] = 0
+    public: Literal[0, 1] = 0
+    private: Literal[0, 1] = 0
+    groups: OptionalListOr[int] = None
+
+
+class BrandsFilters(FountFilters):
+    """Filters for the `brands` endpoint.
+
+    Filters other than `country_codes` and `year_numbers` filter by
+    the Fount IDs of the specific resources.
+
+    See <https://developer.wppbav.com/docs/2.x/core-resources/brands>
+    for more info.
+
+    Attributes
+    ----------
+    country_codes : str or list[str], optional
+        Two-letter ISO-3166 country code or list of country codes, by default None
+    year_numbers : int or list[int], optional
+        Study years in numerical format (not IDs), by default None
+    categories : int or list[int], optional
+        Fount category ID or list of category IDs, by default None
+    countries : int or list[int], optional
+        Fount country ID or list of country IDs, by default None
+    regions : int or list[int], optional
+        Fount region ID or list of region IDs, by default None
+    sectors : int or list[int], optional
+        Fount sector ID or list of sector IDs, by default None
+    studies : int or list[int], optional
+        Fount study ID or list of study IDs, by default None
+    years : int or list[int], optional
+        Fount year ID or list of year IDs, by default None
+
+    Other Parameters
+    ----------------
+    updated_since : str, date or datetime, optional
+        Request items that have been updated since the specified date, by default None
+    """
+
+    country_codes: OptionalListOr[str] = None
+    year_numbers: OptionalListOr[int] = None
+    categories: OptionalListOr[int] = None
+    countries: OptionalListOr[int] = None
+    regions: OptionalListOr[int] = None
+    sectors: OptionalListOr[int] = None
+    studies: OptionalListOr[int] = None
+    years: OptionalListOr[int] = None
+
+
+class BrandscapeFilters(FountFilters):
+    """Filters for the `studies` endpoint.
+
+    `audiences`, `countries`, `studies`, `years`, `brands` and `categories` filter by
+    the Fount IDs of the specific resources.
+
+    See <https://developer.wppbav.com/docs/2.x/core-resources/brandscape-data>
+    for more info.
+
+    The `brandscape-data` endpoint requires the use of, at minimum, these filters:
+
+    - `studies`
+    - `brand_name` or `brands`
+    - `country_code` or `countries` and `brands` or `brand_name`
+    - `year_number` or `years` and `country_code` or `countries`
+
+    An audience filter is also highly recommended, as otherwise the API will return
+    data for all audiences (there are more than 30 standard audiences).
+
+    The `Audiences` class is provided to make it easier to filter audiences.
+
+    Attributes
+    ----------
+    country_code : str or list[str], optional
+        Two-letter ISO-3166 country code or list of country codes, by default None
+    year_number : int or list[int], optional
+        Study years in numerical format (not IDs), by default None
+    audiences : int or list[int], optional
+        Fount ID of the desired audience, by default None
+
+        The `Audiences` class can help with using audience IDs.
+    brand_name : str, optional
+        Perform a search on the brand name, by default None
+    metric_keys : str or list[str], optional
+        Metric keys to return as columns, by default None
+    brands : int or list[int], optional
+        Fount brand ID or list of brand IDs, by default None
+    categories : int or list[int], optional
+        Fount category ID or list of category IDs, by default None
+    countries : int or list[int], optional
+        Fount country ID or list of country IDs, by default None
+
+        The `Countries` class can help with using country IDs.
+    studies : int or list[int], optional
+        Fount study ID or list of study IDs, by default None
+    years : int or list[int], optional
+        Fount year ID or list of year IDs, by default None
+
+
+    Other Parameters
+    ----------------
+    updated_since : str, date or datetime, optional
+        Request items that have been updated since the specified date, by default None
+    """
+
+    country_code: OptionalListOr[str] = None
+    year_number: OptionalListOr[int] = None
+    audiences: OptionalListOr[int] = None
+    brand_name: Optional[str] = None
+    metric_keys: OptionalListOr[str] = None
+    studies: OptionalListOr[int] = None
+    countries: OptionalListOr[int] = None
+    years: OptionalListOr[int] = None
+    brands: OptionalListOr[int] = None
+    categories: OptionalListOr[int] = None
+
+    @root_validator(pre=True)
+    @classmethod
+    def _check_params(cls, values: Dict[str, object]) -> Dict[str, object]:
+        if not (
+            "brands" in values
+            or "brand_name" in values
+            or "studies" in values
+            or (
+                ("country_code" in values or "countries" in values)
+                and ("year_number" in values or "years" in values)
+            )
+        ):
+            raise ValueError(
+                "You need to apply either the `brands`, or `studies`, or `brand_name` "
+                "filters, or the `country_code`/`countries` "
+                "and `year_number`/`years` filters together."
+            )
+
+        return values
+
+
+class StudiesFilters(FountFilters):
+    """Filters for the `studies` endpoint.
+
+    `years`, `countries` and `regions` filter by the Fount IDs of the specific resources.
+
+    See <https://developer.wppbav.com/docs/2.x/core-resources/studies>
+    for more info.
+
+    Attributes
+    ----------
+    country_codes: str or list[str], optional
+        Two-letter ISO-3166 country code or list of country codes, by default None
+    year_numbers: int or list[int], optional
+        Study years in numerical format (not IDs), by default None
+    full_year: Literal[0, 1], optional
+        Return full year studies when set to `1` (excludes US quarterly), by default 0
+    released: Literal[0, 1], optional
+        Return released studies when set to `1`, by default 0
+    unreleased: Literal[0, 1], optional
+        Return unreleased studies when set to `1`, by default 0
+    open_survey: Literal[0, 1], optional
+        Return studies with open brand requests when set to `1`, by default 0
+    active: Literal[0, 1], optional
+        Return active audiences when set to `1`, by default 0
+    inactive: Literal[0, 1], optional
+        Return inactive audiences when set to `1`, by default 0
+    bav_study: Literal[0, 1], optional
+        Return full BAV studies when set to `1`, by default 0
+    data_updated_since: DTValues, optional
+        Return studies updated since datetime value, by default None
+    countries: int or list[int], optional
+        Fount country ID or list of country IDs, by default None
+    regions: int or list[int], optional
+        Fount region ID or list of region IDs, by default None
+    years: int or list[int], optional
+        Fount year ID or list of year IDs, by default None
+
+    Other Parameters
+    ----------------
+    updated_since : str, date or datetime, optional
+        Request items that have been updated since the specified date, by default None
+    """
+
+    country_codes: OptionalListOr[str] = None
+    year_numbers: OptionalListOr[int] = None
+    full_year: Literal[0, 1] = 0
+    released: Literal[0, 1] = 0
+    unreleased: Literal[0, 1] = 0
+    open_survey: Literal[0, 1] = 0
+    active: Literal[0, 1] = 0
+    inactive: Literal[0, 1] = 0
+    bav_study: Literal[0, 1] = 0
+    data_updated_since: DTValues = None
+    years: OptionalListOr[int] = None
+    countries: OptionalListOr[int] = None
+    regions: OptionalListOr[int] = None
+
+    @validator("data_updated_since", pre=True)
+    @classmethod
+    def _parse_date(cls, value: DTValues) -> Optional[str]:
+        if value is None:
+            return value
+        return parse_date(value)
```

### Comparing `wpp-bavapi-0.4.1/bavapi/http.py` & `wpp-bavapi-0.5.0/bavapi/http.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,244 @@
-"""Class for interacting with paginated APIs over HTTP."""
-
-# pylint: disable=too-many-arguments, too-few-public-methods
-
-import asyncio
-import math
-from json import JSONDecodeError
-from typing import Iterator, Optional, Protocol, TypeVar, Union, cast, overload
-
-import httpx
-from tqdm.asyncio import tqdm
-
-from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
-from bavapi.typing import BaseParamsMapping, JSONData, JSONDict
-
-__all__ = ("HTTPClient",)
-
-
-class Query(Protocol):
-    """Protocol for Query objects."""
-
-    item_id: Optional[int]
-    max_pages: Optional[int]
-    per_page: Optional[int]
-    page: Optional[int]
-
-    def to_params(self, endpoint: str) -> BaseParamsMapping:
-        """HTTP-compatible params dictionary"""
-        raise NotImplementedError
-
-    def paginated(self, per_page: int, n_pages: int) -> Iterator["Query"]:
-        """Yields Query objects with page parameters for paginated queries"""
-        raise NotImplementedError
-
-
-class HTTPClient:
-    """HTTP client for interacting with paginated API.
-
-    Parameters
-    ----------
-    base_url : str
-        The base URL of the API.
-    per_page : int, optional
-        Default number of entries per page, by default 100
-    timeout : float, optional
-        Maximum timeout for requests in seconds, by default 5.0
-    verify : bool or str, optional
-        Verify SSL credentials, by default True
-
-        Also accepts a path string to an SSL certificate file.
-    headers : dict[str, str], optional
-        Collection of headers to send with each request, by default None
-    client : httpx.AsyncClient, optional
-        Authenticated `httpx.AsyncClient`, by default None
-    """
-
-    C = TypeVar("C", bound="HTTPClient")
-
-    @overload
-    def __init__(
-        self,
-        base_url: str,
-        per_page: int = 100,
-        timeout: float = 5.0,
-        verify: Union[bool, str] = True,
-        *,
-        headers: Optional[dict[str, str]] = None,
-    ) -> None:
-        ...
-
-    @overload
-    def __init__(self, *, client: httpx.AsyncClient = ..., per_page: int = 100) -> None:
-        ...
-
-    def __init__(
-        self,
-        base_url: str = "",
-        per_page: int = 100,
-        timeout: float = 5.0,
-        verify: Union[bool, str] = True,
-        *,
-        headers: Optional[dict[str, str]] = None,
-        client: Optional[httpx.AsyncClient] = None,
-    ) -> None:
-        self.per_page = per_page
-
-        if client is not None:
-            self.client = client
-        else:
-            self.client = httpx.AsyncClient(
-                headers=headers,
-                timeout=timeout,
-                verify=verify,
-                base_url=base_url,
-            )
-
-    async def __aenter__(self: C) -> C:
-        await self.client.__aenter__()
-        return self
-
-    async def __aexit__(self, *args, **kwargs) -> None:
-        await self.client.__aexit__(*args, **kwargs)
-
-    async def aclose(self) -> None:
-        """Asynchronously close all client connections."""
-        return await self.client.aclose()
-
-    async def get(self, endpoint: str, params: Query) -> httpx.Response:
-        """Perform GET request on the given endpoint.
-
-        Parameters
-        ----------
-        endpoint : str
-            Path to endpoint.
-        params : Query
-            Request parameters.
-
-        Returns
-        -------
-        httpx.Response
-            Requested response object.
-
-        Raises
-        ------
-        APIError
-            If request fails.
-        """
-        if params.item_id is not None:
-            resp = await self.client.get(f"{endpoint}/{params.item_id}")
-        else:
-            resp = await self.client.get(
-                endpoint,
-                params=params.to_params(endpoint),
-            )
-
-        if resp.status_code != 200:
-            try:
-                message = resp.json()["message"]
-            except (KeyError, JSONDecodeError):
-                message = "An error occurred with the Fount."
-
-            raise APIError(f"Error {resp.status_code}:\n{message}\nurl={resp.url}")
-
-        return resp
-
-    async def get_pages(
-        self, endpoint: str, params: Query, n_pages: int
-    ) -> list[httpx.Response]:
-        """Perform GET requests for a given number of pages on an endpoint.
-
-        Parameters
-        ----------
-        endpoint : str
-            Path to endpoint.
-        params : Query
-            Request parameters.
-        n_pages : int
-            Number of pages to request.
-
-        Returns
-        -------
-        list[httpx.Response]
-            List of response objects.
-        """
-        tasks = [
-            asyncio.create_task(self.get(endpoint, p))
-            for p in params.paginated(self.per_page, n_pages)
-        ]
-        try:
-            return cast(
-                list[httpx.Response],
-                await tqdm.gather(*tasks, desc=f"{endpoint} query"),
-            )
-        except Exception as exc:
-            for task in tasks:
-                task.cancel()
-
-            raise exc
-
-    async def query(self, endpoint: str, params: Query) -> Iterator[JSONDict]:
-        """Perform a paginated GET request on the given endpoint.
-
-        Parameters
-        ----------
-        endpoint : str
-            Path to endpoint.
-        params : Query
-            Request parameters.
-
-        Returns
-        -------
-        Iterator[JSONDict]
-            An iterator of JSONDict objects.
-
-        Raises
-        ------
-        APIError
-            If any request fails.
-        DataNotFoundError
-            If response data is empty.
-        RateLimitExceededError
-            If response would exceed the rate limit.
-        """
-        resp = await self.get(endpoint, params=params)
-
-        payload: dict[str, JSONData] = resp.json()
-        data: JSONData = payload["data"]
-
-        if not data:
-            raise DataNotFoundError("Your query returned no results.")
-
-        if isinstance(data, dict):
-            return iter((data,))
-
-        meta = cast(JSONDict, payload["meta"])
-        total = cast(int, meta["total"])
-
-        if params.page or len(data) == total:
-            return iter(data)
-
-        n_pages = params.max_pages or math.ceil(
-            (total) / (params.per_page or self.per_page)
-        )
-
-        if n_pages > int(resp.headers["x-ratelimit-remaining"]):
-            raise RateLimitExceededError(
-                f"Number of pages ({n_pages}) for this request "
-                f"exceeds the rate limit ({resp.headers['x-ratelimit-remaining']}, "
-                f"total={resp.headers['x-ratelimit-limit']})."
-            )
-
-        pages = await self.get_pages(endpoint, params, n_pages)
-
-        return (i for page in pages for i in page.json()["data"])
+"""Class for interacting with paginated APIs over HTTP."""
+
+# pylint: disable=too-many-arguments, too-few-public-methods
+
+import asyncio
+import math
+from json import JSONDecodeError
+from typing import (
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Protocol,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
+
+import httpx
+from tqdm.asyncio import tqdm
+
+from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
+from bavapi.typing import BaseParamsMapping, JSONData, JSONDict
+
+__all__ = ("HTTPClient",)
+
+
+class Query(Protocol):
+    """Protocol for Query objects."""
+
+    item_id: Optional[int]
+    max_pages: Optional[int]
+    per_page: Optional[int]
+    page: Optional[int]
+
+    def to_params(self, endpoint: str) -> BaseParamsMapping:
+        """HTTP-compatible params dictionary"""
+        raise NotImplementedError
+
+    def paginated(self, per_page: int, n_pages: int) -> Iterator["Query"]:
+        """Yields Query objects with page parameters for paginated queries"""
+        raise NotImplementedError
+
+
+class HTTPClient:
+    """HTTP client for interacting with paginated API.
+
+    Parameters
+    ----------
+    base_url : str
+        The base URL of the API.
+    per_page : int, optional
+        Default number of entries per page, by default 100
+    timeout : float, optional
+        Maximum timeout for requests in seconds, by default 5.0
+    verify : bool or str, optional
+        Verify SSL credentials, by default True
+
+        Also accepts a path string to an SSL certificate file.
+    headers : dict[str, str], optional
+        Collection of headers to send with each request, by default None
+    client : httpx.AsyncClient, optional
+        Authenticated `httpx.AsyncClient`, by default None
+    """
+
+    C = TypeVar("C", bound="HTTPClient")
+
+    @overload
+    def __init__(
+        self,
+        base_url: str,
+        per_page: int = 100,
+        timeout: float = 5.0,
+        verify: Union[bool, str] = True,
+        *,
+        headers: Optional[Dict[str, str]] = None,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(self, *, client: httpx.AsyncClient = ..., per_page: int = 100) -> None:
+        ...
+
+    def __init__(
+        self,
+        base_url: str = "",
+        per_page: int = 100,
+        timeout: float = 5.0,
+        verify: Union[bool, str] = True,
+        *,
+        headers: Optional[Dict[str, str]] = None,
+        client: Optional[httpx.AsyncClient] = None,
+    ) -> None:
+        self.per_page = per_page
+
+        if client is not None:
+            self.client = client
+        else:
+            self.client = httpx.AsyncClient(
+                headers=headers,
+                timeout=timeout,
+                verify=verify,
+                base_url=base_url,
+            )
+
+    async def __aenter__(self: C) -> C:
+        await self.client.__aenter__()
+        return self
+
+    async def __aexit__(self, *args, **kwargs) -> None:
+        await self.client.__aexit__(*args, **kwargs)
+
+    async def aclose(self) -> None:
+        """Asynchronously close all client connections."""
+        return await self.client.aclose()
+
+    async def get(self, endpoint: str, params: Query) -> httpx.Response:
+        """Perform GET request on the given endpoint.
+
+        Parameters
+        ----------
+        endpoint : str
+            Path to endpoint.
+        params : Query
+            Request parameters.
+
+        Returns
+        -------
+        httpx.Response
+            Requested response object.
+
+        Raises
+        ------
+        APIError
+            If request fails.
+        """
+        if params.item_id is not None:
+            resp = await self.client.get(f"{endpoint}/{params.item_id}")
+        else:
+            resp = await self.client.get(
+                endpoint,
+                params=params.to_params(endpoint),
+            )
+
+        if resp.status_code != 200:
+            try:
+                message = resp.json()["message"]
+            except (KeyError, JSONDecodeError):
+                message = "An error occurred with the Fount."
+
+            raise APIError(f"Error {resp.status_code}:\n{message}\nurl={resp.url}")
+
+        return resp
+
+    async def get_pages(
+        self, endpoint: str, params: Query, n_pages: int
+    ) -> List[httpx.Response]:
+        """Perform GET requests for a given number of pages on an endpoint.
+
+        Parameters
+        ----------
+        endpoint : str
+            Path to endpoint.
+        params : Query
+            Request parameters.
+        n_pages : int
+            Number of pages to request.
+
+        Returns
+        -------
+        list[httpx.Response]
+            List of response objects.
+        """
+        tasks = [
+            asyncio.create_task(self.get(endpoint, p))
+            for p in params.paginated(self.per_page, n_pages)
+        ]
+        try:
+            return cast(
+                List[httpx.Response],
+                await tqdm.gather(*tasks, desc=f"{endpoint} query"),
+            )
+        except Exception as exc:
+            for task in tasks:
+                task.cancel()
+
+            raise exc
+
+    async def query(self, endpoint: str, params: Query) -> Iterator[JSONDict]:
+        """Perform a paginated GET request on the given endpoint.
+
+        Parameters
+        ----------
+        endpoint : str
+            Path to endpoint.
+        params : Query
+            Request parameters.
+
+        Returns
+        -------
+        Iterator[JSONDict]
+            An iterator of JSONDict objects.
+
+        Raises
+        ------
+        APIError
+            If any request fails.
+        DataNotFoundError
+            If response data is empty.
+        RateLimitExceededError
+            If response would exceed the rate limit.
+        """
+        resp = await self.get(endpoint, params=params)
+
+        payload: Dict[str, JSONData] = resp.json()
+        data: JSONData = payload["data"]
+
+        if not data:
+            raise DataNotFoundError("Your query returned no results.")
+
+        if isinstance(data, dict):
+            return iter((data,))
+
+        meta = cast(JSONDict, payload["meta"])
+        total = cast(int, meta["total"])
+
+        if params.page or len(data) == total:
+            return iter(data)
+
+        n_pages = params.max_pages or math.ceil(
+            (total) / (params.per_page or self.per_page)
+        )
+
+        if n_pages > int(resp.headers["x-ratelimit-remaining"]):
+            raise RateLimitExceededError(
+                f"Number of pages ({n_pages}) for this request "
+                f"exceeds the rate limit ({resp.headers['x-ratelimit-remaining']}, "
+                f"total={resp.headers['x-ratelimit-limit']})."
+            )
+
+        pages = await self.get_pages(endpoint, params, n_pages)
+
+        return (i for page in pages for i in page.json()["data"])
```

### Comparing `wpp-bavapi-0.4.1/bavapi/parsing/params.py` & `wpp-bavapi-0.5.0/bavapi/parsing/params.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-"""Functions to parse parameter values."""
-
-import datetime as dt
-from typing import Mapping, Sequence, TypeVar, Union, cast
-
-from bavapi.typing import BaseMutableParamsMapping, BaseMutableParamsMappingValues
-
-T = TypeVar("T")
-
-
-def parse_date(value: Union[str, dt.datetime, dt.date]) -> str:
-    """Parse date string or datetime value into a date string.
-
-    Parameters
-    ----------
-    value : str, dt.datetime, dt.date
-        Input to parse into a date string.
-
-    Returns
-    -------
-    str
-        The parsed date as a string.
-    """
-    fmt_out = "%Y-%m-%d %H:%M:%S"
-    if isinstance(value, dt.datetime):
-        return value.strftime(fmt_out)
-    if isinstance(value, dt.date):
-        return dt.datetime.combine(value, dt.datetime.min.time()).strftime(fmt_out)
-    try:
-        return dt.datetime.strptime(value, fmt_out).strftime(value)
-    except ValueError:
-        return dt.datetime.fromisoformat(value).strftime(fmt_out)
-
-
-def to_fount_params(data: Mapping[str, T], param: str) -> dict[str, T]:
-    """Constructs dictionary keys for special Fount API formatting.
-
-    The resulting dictionary keys will be formatted to include `param` as the
-    main parameter name:
-
-    >>> to_fount_params({"a":1}, "test")
-    {"test[a]":1}
-
-    Parameters
-    ----------
-    data : dict[str, Any]
-        Dictionary to format.
-    param : str
-        Parameter name.
-
-    Returns
-    -------
-    dict[str, Any]
-        Fount API parameter dictionary.
-    """
-    return {f"{param}[{k}]": v for k, v in data.items()}
-
-
-def list_to_str(mapping: BaseMutableParamsMapping) -> BaseMutableParamsMappingValues:
-    """Convert any lists in a dictionary to a string with comma-separated elements.
-
-    Parameters
-    ----------
-    mapping : ParamsMapping
-        Dictionary with lists
-
-    Returns
-    -------
-    ParamsMappingValues
-        Dictionary without strings
-    """
-    for key, value in mapping.items():
-        if not isinstance(value, str) and isinstance(value, Sequence):
-            mapping[key] = ",".join(str(i) for i in value)
-
-    return cast(BaseMutableParamsMappingValues, mapping)
+"""Functions to parse parameter values."""
+
+import datetime as dt
+from typing import Dict, Mapping, Sequence, TypeVar, Union, cast
+
+from bavapi.typing import BaseMutableParamsMapping, BaseMutableParamsMappingValues
+
+T = TypeVar("T")
+
+
+def parse_date(value: Union[str, dt.datetime, dt.date]) -> str:
+    """Parse date string or datetime value into a date string.
+
+    Parameters
+    ----------
+    value : str, dt.datetime, dt.date
+        Input to parse into a date string.
+
+    Returns
+    -------
+    str
+        The parsed date as a string.
+    """
+    fmt_out = "%Y-%m-%d %H:%M:%S"
+    if isinstance(value, dt.datetime):
+        return value.strftime(fmt_out)
+    if isinstance(value, dt.date):
+        return dt.datetime.combine(value, dt.datetime.min.time()).strftime(fmt_out)
+    try:
+        return dt.datetime.strptime(value, fmt_out).strftime(value)
+    except ValueError:
+        return dt.datetime.fromisoformat(value).strftime(fmt_out)
+
+
+def to_fount_params(data: Mapping[str, T], param: str) -> Dict[str, T]:
+    """Constructs dictionary keys for special Fount API formatting.
+
+    The resulting dictionary keys will be formatted to include `param` as the
+    main parameter name:
+
+    >>> to_fount_params({"a":1}, "test")
+    {"test[a]":1}
+
+    Parameters
+    ----------
+    data : dict[str, Any]
+        Dictionary to format.
+    param : str
+        Parameter name.
+
+    Returns
+    -------
+    dict[str, Any]
+        Fount API parameter dictionary.
+    """
+    return {f"{param}[{k}]": v for k, v in data.items()}
+
+
+def list_to_str(mapping: BaseMutableParamsMapping) -> BaseMutableParamsMappingValues:
+    """Convert any lists in a dictionary to a string with comma-separated elements.
+
+    Parameters
+    ----------
+    mapping : ParamsMapping
+        Dictionary with lists
+
+    Returns
+    -------
+    ParamsMappingValues
+        Dictionary without strings
+    """
+    for key, value in mapping.items():
+        if not isinstance(value, str) and isinstance(value, Sequence):
+            mapping[key] = ",".join(str(i) for i in value)
+
+    return cast(BaseMutableParamsMappingValues, mapping)
```

### Comparing `wpp-bavapi-0.4.1/bavapi/parsing/responses.py` & `wpp-bavapi-0.5.0/bavapi/parsing/responses.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,160 @@
-"""Functions for parsing Fount API responses"""
-
-from typing import Iterable, Iterator, Mapping, Optional, TypeVar, Union, cast
-
-import pandas as pd
-
-T = TypeVar("T")
-
-
-def flatten_mapping(
-    mapping: Mapping[str, Union[T, Mapping[str, T]]],
-    parent: str = "",
-    sep: str = "_",
-    prefix: str = "",
-) -> dict[str, T]:
-    """Recursively flattens all nested dictionaries into top level key-value pairs.
-
-    Include prefixes or suffixes if nested keys clash with top-level keys.
-
-    Parameters
-    ----------
-    mapping : dict[str, Any] or mapping
-        Dictionary with potential nested dictionaries
-    parent : str
-        Parent key for generating children keys, by default ""
-    sep : str
-        Separator to use between keys and parent keys, by default ""
-    prefix: str
-        Prefix for nested keys that clash with keys in the top-level mapping, by default ""
-
-        An empty prefix will ignore key conflicts.
-
-    Returns
-    -------
-    dict[str, Any]
-        Flattened dictionary.
-    """
-    new: dict[str, T] = {}
-
-    for key, value in mapping.items():
-        if parent:
-            key = f"{parent}{sep}{key}"
-
-        if isinstance(value, Mapping):
-            if prefix and any(
-                k.startswith(key)
-                for k, v in mapping.items()
-                if not isinstance(v, Mapping)
-            ):
-                key = f"{prefix}{sep}{key}"
-
-            new |= flatten_mapping(value, key, sep, prefix)
-        else:
-            new[key] = value
-
-    return new
-
-
-def flatten(
-    mapping: Mapping[str, Union[T, Mapping[str, T]]],
-    parent: str = "",
-    sep: str = "_",
-    prefix: str = "",
-    expand: bool = False,
-) -> Iterator[dict[str, T]]:
-    """Recursively flatten all nested mappings and lists in the given mapping.
-
-    Returns an iterator because it expands any nested lists into new dictionaries,
-    then yields each repeated dictionary with its corresponding value from the list.
-
-    This is equivalent to a `JOIN` operation in a relational database, where lists
-    represent multiple entries on the right table of the `JOIN`.
-
-    Note: If many nested lists are present, this function will generate as many entries
-    as the PRODUCT of the nested lists. If the mapping has one nested list with 5
-    elements, and another nested list with 5 elements,
-    the function will yield 25 (5x5) dictionaries in total.
-
-    Parameters
-    ----------
-    mapping : dict[str, Any] or mapping
-        Dictionary with potential nested dictionaries and lists of dictionaries
-    parent : str
-        Parent key for generating children keys, by default ""
-    sep : str
-        Separator to use between keys and parent keys, by default ""
-    prefix: str
-        Prefix for keys that clash with keys in the top-level mapping, by default ""
-
-        An empty prefix will ignore key conflicts.
-    expand : bool, optional
-        Whether to expand nested lists into new dictionaries, by default False
-
-    Yields
-    ------
-    Iterator[dict[str, Any]]
-        Yield flattened dictionaries.
-
-        If expand is True and any nested lists are present, yield each resulting
-        flattened dictionary.
-    """
-    new: dict[str, T] = flatten_mapping(mapping, parent, sep, prefix)
-    expand_keys: list[str] = (
-        [k for k, v in new.items() if isinstance(v, list)] if expand else []
-    )
-
-    if not expand_keys:
-        yield new
-    else:
-        for key in expand_keys:
-            values = cast(list[Mapping[str, T]], new[key])
-            print(key)
-            for val in values:
-                yield from (
-                    {k: v for k, v in new.items() if k != key} | i
-                    for i in flatten(val, key, sep, prefix, expand)
-                )
-
-
-def parse_response(
-    page: Iterable[Mapping[str, object]],
-    prefix: str = "",
-    index: Optional[str] = None,
-    expand: bool = False,
-) -> pd.DataFrame:
-    """Parse Fount API JSON into a pandas DataFrame.
-
-    Parameters
-    ----------
-    page : iterable of dicts with keys of type str
-        Page from API response.
-    prefix : str, optional
-        Prefix to prepend to columns with clashing names, by default `""`
-    index : str, optional
-        Column name to use as index, by default None.
-    expand : bool, optional
-        Whether to expand lists of dictionaries into new entries (rows)
-        in the resulting DataFrame, by default False.
-
-    Returns
-    -------
-    pd.DataFrame
-        DataFrame of the response data.
-    """
-    return (
-        pd.DataFrame.from_records(
-            (i for item in page for i in flatten(item, prefix=prefix, expand=expand)),
-            index=index,
-        )
-        .dropna(axis=1, how="all")
-        .transform(pd.to_numeric, errors="ignore")
-    )
+"""Functions for parsing Fount API responses"""
+
+from typing import (
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    TypeVar,
+    Union,
+    cast,
+)
+
+import pandas as pd
+
+T = TypeVar("T")
+
+
+def flatten_mapping(
+    mapping: Mapping[str, Union[T, Mapping[str, T]]],
+    parent: str = "",
+    sep: str = "_",
+    prefix: str = "",
+) -> Dict[str, T]:
+    """Recursively flattens all nested dictionaries into top level key-value pairs.
+
+    Include prefixes or suffixes if nested keys clash with top-level keys.
+
+    Parameters
+    ----------
+    mapping : dict[str, Any] or mapping
+        Dictionary with potential nested dictionaries
+    parent : str
+        Parent key for generating children keys, by default ""
+    sep : str
+        Separator to use between keys and parent keys, by default ""
+    prefix: str
+        Prefix for nested keys that clash with keys in the top-level mapping, by default ""
+
+        An empty prefix will ignore key conflicts.
+
+    Returns
+    -------
+    dict[str, Any]
+        Flattened dictionary.
+    """
+    new: Dict[str, T] = {}
+
+    for key, value in mapping.items():
+        if parent:
+            key = f"{parent}{sep}{key}"
+
+        if isinstance(value, Mapping):
+            if prefix and any(
+                k.startswith(key)
+                for k, v in mapping.items()
+                if not isinstance(v, Mapping)
+            ):
+                key = f"{prefix}{sep}{key}"
+
+            new = {**new, **flatten_mapping(value, key, sep, prefix)}
+        else:
+            new[key] = value
+
+    return new
+
+
+def flatten(
+    mapping: Mapping[str, Union[T, Mapping[str, T]]],
+    parent: str = "",
+    sep: str = "_",
+    prefix: str = "",
+    expand: bool = False,
+) -> Iterator[Dict[str, T]]:
+    """Recursively flatten all nested mappings and lists in the given mapping.
+
+    Returns an iterator because it expands any nested lists into new dictionaries,
+    then yields each repeated dictionary with its corresponding value from the list.
+
+    This is equivalent to a `JOIN` operation in a relational database, where lists
+    represent multiple entries on the right table of the `JOIN`.
+
+    Note: If many nested lists are present, this function will generate as many entries
+    as the PRODUCT of the nested lists. If the mapping has one nested list with 5
+    elements, and another nested list with 5 elements,
+    the function will yield 25 (5x5) dictionaries in total.
+
+    Parameters
+    ----------
+    mapping : dict[str, Any] or mapping
+        Dictionary with potential nested dictionaries and lists of dictionaries
+    parent : str
+        Parent key for generating children keys, by default ""
+    sep : str
+        Separator to use between keys and parent keys, by default ""
+    prefix: str
+        Prefix for keys that clash with keys in the top-level mapping, by default ""
+
+        An empty prefix will ignore key conflicts.
+    expand : bool, optional
+        Whether to expand nested lists into new dictionaries, by default False
+
+    Yields
+    ------
+    Iterator[dict[str, Any]]
+        Yield flattened dictionaries.
+
+        If expand is True and any nested lists are present, yield each resulting
+        flattened dictionary.
+    """
+    new: Dict[str, T] = flatten_mapping(mapping, parent, sep, prefix)
+    expand_keys: List[str] = (
+        [k for k, v in new.items() if isinstance(v, list)] if expand else []
+    )
+
+    if not expand_keys:
+        yield new
+    else:
+        for key in expand_keys:
+            values = cast(List[Mapping[str, T]], new[key])
+            print(key)
+            for val in values:
+                for i in flatten(val, key, sep, prefix, expand):
+                    yield {**{k: v for k, v in new.items() if k != key}, **i}
+
+
+def parse_response(
+    page: Iterable[Mapping[str, object]],
+    prefix: str = "",
+    index: Optional[str] = None,
+    expand: bool = False,
+) -> pd.DataFrame:
+    """Parse Fount API JSON into a pandas DataFrame.
+
+    Parameters
+    ----------
+    page : iterable of dicts with keys of type str
+        Page from API response.
+    prefix : str, optional
+        Prefix to prepend to columns with clashing names, by default `""`
+    index : str, optional
+        Column name to use as index, by default None.
+    expand : bool, optional
+        Whether to expand lists of dictionaries into new entries (rows)
+        in the resulting DataFrame, by default False.
+
+    Returns
+    -------
+    pd.DataFrame
+        DataFrame of the response data.
+    """
+    return (
+        pd.DataFrame.from_records(
+            (i for item in page for i in flatten(item, prefix=prefix, expand=expand)),
+            index=index,
+        )
+        .dropna(axis=1, how="all")
+        .transform(pd.to_numeric, errors="ignore")
+    )
```

### Comparing `wpp-bavapi-0.4.1/bavapi/query.py` & `wpp-bavapi-0.5.0/bavapi/query.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""Query objects for Fount API queries based on `pydantic`."""
-
-# pylint: disable=no-name-in-module, too-few-public-methods
-
-from typing import Final, Generic, Iterator, Optional, TypeVar, cast
-
-from pydantic import BaseModel, Field
-
-from bavapi import filters as _filters
-from bavapi.parsing.params import list_to_str, to_fount_params
-from bavapi.typing import (
-    BaseMutableParamsMapping,
-    BaseParamsDict,
-    BaseParamsDictValues,
-    OptionalListOr,
-)
-
-__all__ = ("Query",)
-
-F = TypeVar("F", bound=_filters.FountFilters)
-
-
-class Query(BaseModel, Generic[F]):
-    """Base WPPBAV Fount query.
-
-    Attributes
-    ----------
-    id: int, optional
-        Get specific resource by ID, by default None
-    filters : FountFilters instance or dict of filter values, optional
-        Filters to apply to the query, by default None
-    fields: str or list[str], optional
-        Specific fields to retrieve from the query, by default None
-    include: str or list[str], optional
-        Additional resources to retrieve from the query, by default None
-    sort: str, optional
-        Sort response by field, by default None
-
-        To sort in descending (highest first) order, use a `-` before the field name:
-
-        `sort="-differentiation_rank"`
-
-        Sorts by item ID by default.
-    page: int, optional
-        Get specific page from paginated response, by default None
-
-        When None, the default value in the Fount is 1
-    per_page: int, optional
-        Number of items per page, by default None
-
-        When None, the default value in the Fount is 25
-
-        When performing paged queries, Client uses 100 as the default `per_page`.
-    max_pages: int, optional
-        Maximum number of pages to retrieve, by default None
-
-        When None, all pages will be retrieved with a `per_page` value of 100 by default.
-    """
-
-    item_id: Optional[int] = Field(default=None, alias="id")
-    filters: Optional[_filters.FiltersOrMapping[F]] = None
-    fields: OptionalListOr[str] = None
-    include: OptionalListOr[str] = None
-    sort: Optional[str] = None
-    page: Optional[int] = None
-    per_page: Optional[int] = None
-    max_pages: Optional[int] = None
-
-    def to_params(self, endpoint: str) -> BaseParamsDictValues:
-        """Return Fount-compatible dictionary of the query.
-
-        Returns
-        -------
-        dict[str, Any]
-            Fount-compatible dictionary of the query.
-        """
-        exclude: Final[set[str]] = {"filters", "fields", "max_pages"}
-
-        filters: BaseParamsDict = {}
-        fields: BaseMutableParamsMapping = {}
-
-        if isinstance(self.filters, _filters.FountFilters):
-            filters = self.filters.dict(by_alias=True, exclude_defaults=True)
-        filters = to_fount_params(filters, "filter")
-        fields = to_fount_params(
-            {endpoint: self.fields} if self.fields else fields, "fields"
-        )
-
-        params = (
-            self.dict(exclude=exclude, by_alias=True, exclude_defaults=True)
-            | filters
-            | fields
-        )
-
-        return cast(BaseParamsDictValues, list_to_str(params))
-
-    def with_page(self, page: int, per_page: int) -> "Query[F]":
-        """Create new instance of `Query` with page parameters if either is set to default.
-
-        Returns new instance of Query.
-
-        Parameters
-        ----------
-        page : int
-            Current page number
-        per_page : int
-            Number of results per page
-
-        Returns
-        -------
-        Query
-            New `Query` instance with page parameters.
-        """
-        if self.page and self.per_page:
-            return self
-
-        return self.__class__.construct(
-            self.__fields_set__.union({"page", "per_page"}),
-            page=self.page or page,
-            per_page=self.per_page or per_page,
-            filters=self.filters,  # avoid turning filters into dictionary
-            **self.dict(
-                by_alias=True,
-                exclude={"page", "per_page", "filters"},
-                exclude_defaults=True,
-            ),
-        )
-
-    def paginated(self, per_page: int, n_pages: int) -> Iterator["Query[F]"]:
-        """Yield `Query` instances with page parameters for each page in `n_pages`.
-
-        For performing multiple paginated requests.
-
-        Yields
-        ------
-        Query
-            Query instances with page parameters set.
-        """
-        yield from (self.with_page(p, per_page) for p in range(1, n_pages + 1))
+"""Query objects for Fount API queries based on `pydantic`."""
+
+# pylint: disable=no-name-in-module, too-few-public-methods
+
+from typing import Final, Generic, Iterator, Optional, Set, TypeVar, cast
+
+from pydantic import BaseModel, Field
+
+from bavapi import filters as _filters
+from bavapi.parsing.params import list_to_str, to_fount_params
+from bavapi.typing import (
+    BaseMutableParamsMapping,
+    BaseParamsDict,
+    BaseParamsDictValues,
+    OptionalListOr,
+)
+
+__all__ = ("Query",)
+
+F = TypeVar("F", bound=_filters.FountFilters)
+
+
+class Query(BaseModel, Generic[F]):
+    """Base WPPBAV Fount query.
+
+    Attributes
+    ----------
+    id: int, optional
+        Get specific resource by ID, by default None
+    filters : FountFilters instance or dict of filter values, optional
+        Filters to apply to the query, by default None
+    fields: str or list[str], optional
+        Specific fields to retrieve from the query, by default None
+    include: str or list[str], optional
+        Additional resources to retrieve from the query, by default None
+    sort: str, optional
+        Sort response by field, by default None
+
+        To sort in descending (highest first) order, use a `-` before the field name:
+
+        `sort="-differentiation_rank"`
+
+        Sorts by item ID by default.
+    page: int, optional
+        Get specific page from paginated response, by default None
+
+        When None, the default value in the Fount is 1
+    per_page: int, optional
+        Number of items per page, by default None
+
+        When None, the default value in the Fount is 25
+
+        When performing paged queries, Client uses 100 as the default `per_page`.
+    max_pages: int, optional
+        Maximum number of pages to retrieve, by default None
+
+        When None, all pages will be retrieved with a `per_page` value of 100 by default.
+    """
+
+    item_id: Optional[int] = Field(default=None, alias="id")
+    filters: Optional[_filters.FiltersOrMapping[F]] = None
+    fields: OptionalListOr[str] = None
+    include: OptionalListOr[str] = None
+    sort: Optional[str] = None
+    page: Optional[int] = None
+    per_page: Optional[int] = None
+    max_pages: Optional[int] = None
+
+    def to_params(self, endpoint: str) -> BaseParamsDictValues:
+        """Return Fount-compatible dictionary of the query.
+
+        Returns
+        -------
+        dict[str, Any]
+            Fount-compatible dictionary of the query.
+        """
+        exclude: Final[Set[str]] = {"filters", "fields", "max_pages"}
+
+        filters: BaseParamsDict = {}
+        fields: BaseMutableParamsMapping = {}
+
+        if isinstance(self.filters, _filters.FountFilters):
+            filters = self.filters.dict(by_alias=True, exclude_defaults=True)
+        filters = to_fount_params(filters, "filter")
+        fields = to_fount_params(
+            {endpoint: self.fields} if self.fields else fields, "fields"
+        )
+
+        params = {
+            **self.dict(exclude=exclude, by_alias=True, exclude_defaults=True),
+            **filters,
+            **fields,
+        }
+
+        return cast(BaseParamsDictValues, list_to_str(params))
+
+    def with_page(self, page: int, per_page: int) -> "Query[F]":
+        """Create new instance of `Query` with page parameters if either is set to default.
+
+        Returns new instance of Query.
+
+        Parameters
+        ----------
+        page : int
+            Current page number
+        per_page : int
+            Number of results per page
+
+        Returns
+        -------
+        Query
+            New `Query` instance with page parameters.
+        """
+        if self.page and self.per_page:
+            return self
+
+        return self.__class__.construct(
+            self.__fields_set__.union({"page", "per_page"}),
+            page=self.page or page,
+            per_page=self.per_page or per_page,
+            filters=self.filters,  # avoid turning filters into dictionary
+            **self.dict(
+                by_alias=True,
+                exclude={"page", "per_page", "filters"},
+                exclude_defaults=True,
+            ),
+        )
+
+    def paginated(self, per_page: int, n_pages: int) -> Iterator["Query[F]"]:
+        """Yield `Query` instances with page parameters for each page in `n_pages`.
+
+        For performing multiple paginated requests.
+
+        Yields
+        ------
+        Query
+            Query instances with page parameters set.
+        """
+        yield from (self.with_page(p, per_page) for p in range(1, n_pages + 1))
```

### Comparing `wpp-bavapi-0.4.1/bavapi/reference/generate_reference.py` & `wpp-bavapi-0.5.0/bavapi/reference/generate_reference.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,287 +1,285 @@
-"""Script to update reference classes with latest active definitions from the Fount."""
-
-# pylint: disable=too-few-public-methods
-
-import argparse
-import asyncio
-import datetime
-import functools
-import os
-from pathlib import Path
-from typing import Callable, NamedTuple, Optional
-
-import pandas as pd
-from dotenv import load_dotenv
-
-from bavapi import Client, Query
-from bavapi.parsing.responses import parse_response
-from bavapi.typing import JSONDict
-
-ReferenceParser = Callable[[pd.Series], dict[str, str]]
-
-
-class Args:
-    """Basic namespace for arguments with typing."""
-
-    __slots__ = ("all", "name", "folder")
-
-    def __init__(self, namespace: argparse.Namespace) -> None:
-        self.all: bool = namespace.all
-        self.name: str = namespace.name
-
-
-class RefConfig(NamedTuple):
-    """Config information for updating Fount references
-
-    Parameters
-    ----------
-    endpoint : str
-        Fount API resource endpoint to use for updating references.
-    filepath : str
-        Path to write the updated references to.
-    parser : Callable[[pd.Series], dict[str, str]]
-        Function to parse the reference in pandas form to a dict of strings.
-    resource_col : str
-        Column to get the names for each item in the reference.
-    """
-
-    endpoint: str
-    filename: str
-    parser: ReferenceParser
-    resource_col: str = "name"
-
-
-async def get_references(
-    fount: Client, configs: list[RefConfig]
-) -> list[list[JSONDict]]:
-    """Download items for the reference from the Fount.
-
-    Parameters
-    ----------
-    fount : Client
-        Client instance to perform requests with.
-    config : RefConfig
-        Reference config object, with information about the filepath, endpoint
-        resource parser function and the resource column.
-    loop : asyncio.AbstractEventLoop
-        Loop to execute the requests.
-
-    Returns
-    -------
-    dict[str, str]
-        Dictionary of reference information for generating reference files.
-    """
-    async with fount:
-        tasks = [
-            asyncio.create_task(fount.raw_query(config.endpoint, Query()))
-            for config in configs
-        ]
-        return await asyncio.gather(*tasks)
-
-
-def parse_reference(
-    fetched: pd.Series, symbols: dict[str, str], norm: dict[str, str]
-) -> dict[str, str]:
-    """Parse reference information from the Fount.
-
-    Parameters
-    ----------
-    fetched : pd.Series
-        Pandas Series with reference information
-    symbols : dict[str, str]
-        Symbols to replace
-    norm : dict[str, str]
-        Elements in reference to normalize
-
-    Returns
-    -------
-    dict[str, str]
-        Dictionary of reference information for generating reference files.
-    """
-    fetched = fetched.str.upper().replace(symbols, regex=True).replace(norm, regex=True)
-
-    return {str(v): str(k) for k, v in fetched.to_dict().items()}
-
-
-parse_audiences = functools.partial(
-    parse_reference,
-    symbols={r"\+": "_PLUS", r"\W+": "_"},
-    norm={
-        "MIDDLE_INCOME": "MEDIUM_INCOME",
-        "29_AND_UNDER": "UNDER_30",
-    },
-)
-
-parse_countries = functools.partial(
-    parse_reference,
-    symbols={r"\W+": "_"},
-    norm={"TÜRKIYE": "TURKIYE"},
-)
-
-
-def process_items(data: list[JSONDict], config: RefConfig) -> dict[str, str]:
-    """Process raw Fount response into a dictionary of name to filter code pairs.
-
-    Parameters
-    ----------
-    data : list[JSONDict]
-        List of JSON dictionaries representing each of the Fount reference items.
-    config : RefConfig
-        Reference configuration to use for processing items.
-
-    Returns
-    -------
-    dict[str, str]
-        Pairs of reference item names and their corresponding code.
-    """
-    res_df = parse_response(data, index="id")
-
-    if "is_active" in res_df.columns:
-        res_df = res_df[res_df["is_active"].astype(bool)]
-
-    items = res_df[config.resource_col].drop_duplicates().pipe(config.parser).items()
-    return dict(sorted(items))
-
-
-def generate_source(
-    ref_name: str,
-    ref_items: dict[str, str],
-    updated: datetime.datetime,
-    import_items: tuple[str, str] = ("bavapi.reference._int_enum", "IntEnum"),
-) -> str:
-    """Generate updated module source from reference items.
-
-    Parameters
-    ----------
-    ref_name : str
-        Name of the reference to generate. This name will also be the name of the
-        reference class ("countries" -> "Countries").
-    ref_items : dict[str, str]
-        Dictionary of reference information to generate from.
-    updated : datetime.datetime
-        Reference update timestamp.
-    import_items : tuple[str, str], optional
-        Elements for import statement, by default ("bavapi.reference.base", "IntEnum")
-
-    Returns
-    -------
-    str
-        Updated source as a string.
-    """
-    updated_comment = (
-        f"# This file was generated from active {ref_name.lower()} in the Fount.\n"
-        f"# {ref_name.capitalize()} retrieved on {updated.strftime('%Y-%m-%d %H:%M:%S')}"
-    )
-
-    class_docstring = f'"""{ref_name.capitalize()} IDs for Fount API queries."""'
-
-    source_items = [
-        f'"""{ref_name.capitalize()} class for holding {ref_name} IDs."""',
-        updated_comment,
-        f"from {import_items[0]} import {import_items[1]}\n",
-        f"class {ref_name.capitalize()}({import_items[1]}):\n" f"    {class_docstring}",
-        "\n".join(f"    {k} = {v}" for k, v in ref_items.items()),
-    ]
-
-    return "\n\n".join(source_items) + "\n"
-
-
-def write_to_file(source: str, filepath: Path) -> None:
-    """Write updated module source to file.
-
-    Parameters
-    ----------
-    source : str
-        Updated module source as a string.
-    filepath : pathlib.Path
-        Path to write the source to.
-    """
-    if not filepath.parent.exists():
-        filepath.parent.mkdir(parents=True, exist_ok=True)
-
-    with open(filepath, "w", encoding="utf-8") as file:
-        file.write(source)
-
-
-def parse_args(argv: Optional[list[str]] = None) -> Args:
-    """Parse arguments given to the script.
-
-    Returns
-    -------
-    argparse.Namespace
-        Object containing arguments and values for the script
-    """
-    parser = argparse.ArgumentParser(
-        description="Generate reference files for commonly used BAV filters.\n\n"
-        "The script will generate a set of reference files that contain "
-        "helpful classes for filtering BAV data in readable form.\n\n"
-        "The currently available reference classes are Audiences and Countries.\n"
-        "These classess will be stored in a `bavapi_refs` folder in your "
-        "current working directory. "
-        "You can import them using `from bavapi_refs.audiences import Audiences`.\n"
-        "Existing reference files will be overwritten.",
-        epilog="DON'T PUSH REFERENCES TO GIT! Add `bavapi_refs/` to `.gitignore`.",
-    )
-    parser.add_argument(
-        "-a", "--all", action="store_true", help="Generate all reference files."
-    )
-    parser.add_argument(
-        "-n",
-        "--name",
-        default="",
-        choices={"audiences", "countries"},
-        help="Name of reference to generate.",
-    )
-    return Args(parser.parse_args(argv))
-
-
-def main(argv: Optional[list[str]] = None) -> int:
-    """Main function to generate reference classes.
-
-    Returns
-    -------
-    int
-        CLI exit code
-    """
-    load_dotenv()
-
-    args = parse_args(argv)
-    fount = Client(os.getenv("FOUNT_API_KEY", "no_key"))
-
-    base_path = Path.cwd() / "bavapi_refs"
-    print(base_path)
-
-    ref_configs: dict[str, RefConfig] = {
-        "audiences": RefConfig("audiences", "audiences", parse_audiences),
-        "countries": RefConfig(
-            "studies",
-            "countries",
-            parse_countries,
-            "country_name",
-        ),
-    }
-
-    if args.all:
-        names, configs = list(ref_configs.keys()), list(ref_configs.values())
-    elif not args.name:
-        print("bavapi-refs: Run `bavapi-refs -h` for usage instructions.")
-        return 1
-    else:
-        names, configs = [args.name], [ref_configs[args.name]]
-
-    results = asyncio.run(get_references(fount, configs))
-
-    for name, data, config in zip(names, results, configs):
-        items = process_items(data, config)
-        source = generate_source(name, items, datetime.datetime.utcnow())
-        path = base_path / f"{name}.py"
-
-        print(f"Writing {name} file with {len(items)} items to {path}")
-        write_to_file(source, path)
-
-    print("Success!")
-    return 0
-
-
-if __name__ == "__main__":
-    raise SystemExit(main())  # pragma: no cover
+"""Script to update reference classes with latest active definitions from the Fount."""
+
+# pylint: disable=too-few-public-methods
+
+import argparse
+import asyncio
+import datetime
+import functools
+import os
+from pathlib import Path
+from typing import Callable, Dict, List, NamedTuple, Optional, Tuple
+
+import pandas as pd
+from dotenv import load_dotenv
+
+from bavapi import Client, Query
+from bavapi.parsing.responses import parse_response
+from bavapi.typing import JSONDict
+
+ReferenceParser = Callable[[pd.Series], Dict[str, str]]
+
+
+class Args:
+    """Basic namespace for arguments with typing."""
+
+    __slots__ = ("all", "name", "folder")
+
+    def __init__(self, namespace: argparse.Namespace) -> None:
+        self.all: bool = namespace.all
+        self.name: str = namespace.name
+
+
+class RefConfig(NamedTuple):
+    """Config information for updating Fount references
+
+    Attributes
+    ----------
+    endpoint : str
+        Fount API resource endpoint to use for updating references.
+    filepath : str
+        Path to write the updated references to.
+    parser : Callable[[pd.Series], dict[str, str]]
+        Function to parse the reference in pandas form to a dict of strings.
+    resource_col : str, optional
+        Column to get the names for each item in the reference, by default "name"
+    """
+
+    endpoint: str
+    filename: str
+    parser: ReferenceParser
+    resource_col: str = "name"
+
+
+async def get_references(
+    fount: Client, configs: List[RefConfig]
+) -> List[List[JSONDict]]:
+    """Download items for the reference from the Fount.
+
+    Parameters
+    ----------
+    fount : Client
+        Client instance to perform requests with.
+    configs : list[RefConfig]
+        Reference config object, with information about the filepath, endpoint
+        resource parser function and the resource column.
+
+    Returns
+    -------
+    dict[str, str]
+        Dictionary of reference information for generating reference files.
+    """
+    async with fount:
+        tasks = [
+            asyncio.create_task(fount.raw_query(config.endpoint, Query()))
+            for config in configs
+        ]
+        return await asyncio.gather(*tasks)
+
+
+def parse_reference(
+    fetched: pd.Series, symbols: Dict[str, str], norm: Dict[str, str]
+) -> Dict[str, str]:
+    """Parse reference information from the Fount.
+
+    Parameters
+    ----------
+    fetched : pd.Series
+        Pandas Series with reference information
+    symbols : dict[str, str]
+        Symbols to replace
+    norm : dict[str, str]
+        Elements in reference to normalize
+
+    Returns
+    -------
+    dict[str, str]
+        Dictionary of reference information for generating reference files.
+    """
+    fetched = fetched.str.upper().replace(symbols, regex=True).replace(norm, regex=True)
+
+    return {str(v): str(k) for k, v in fetched.to_dict().items()}
+
+
+parse_audiences = functools.partial(
+    parse_reference,
+    symbols={r"\+": "_PLUS", r"\W+": "_"},
+    norm={
+        "MIDDLE_INCOME": "MEDIUM_INCOME",
+        "29_AND_UNDER": "UNDER_30",
+    },
+)
+
+parse_countries = functools.partial(
+    parse_reference,
+    symbols={r"\W+": "_"},
+    norm={"TÜRKIYE": "TURKIYE"},
+)
+
+
+def process_items(data: List[JSONDict], config: RefConfig) -> Dict[str, str]:
+    """Process raw Fount response into a dictionary of name to filter code pairs.
+
+    Parameters
+    ----------
+    data : list[JSONDict]
+        List of JSON dictionaries representing each of the Fount reference items.
+    config : RefConfig
+        Reference configuration to use for processing items.
+
+    Returns
+    -------
+    dict[str, str]
+        Pairs of reference item names and their corresponding code.
+    """
+    res_df = parse_response(data, index="id")
+
+    if "is_active" in res_df.columns:
+        res_df = res_df[res_df["is_active"].astype(bool)]
+
+    items = res_df[config.resource_col].drop_duplicates().pipe(config.parser).items()
+    return dict(sorted(items))
+
+
+def generate_source(
+    ref_name: str,
+    ref_items: Dict[str, str],
+    updated: datetime.datetime,
+    import_items: Tuple[str, str] = ("bavapi.reference._int_enum", "IntEnum"),
+) -> str:
+    """Generate updated module source from reference items.
+
+    Parameters
+    ----------
+    ref_name : str
+        Name of the reference to generate. This name will also be the name of the
+        reference class ("countries" -> "Countries").
+    ref_items : dict[str, str]
+        Dictionary of reference information to generate from.
+    updated : datetime.datetime
+        Reference update timestamp.
+    import_items : tuple[str, str], optional
+        Elements for import statement, by default ("bavapi.reference.base", "IntEnum")
+
+    Returns
+    -------
+    str
+        Updated source as a string.
+    """
+    updated_comment = (
+        f"# This file was generated from active {ref_name.lower()} in the Fount.\n"
+        f"# {ref_name.capitalize()} retrieved on {updated.strftime('%Y-%m-%d %H:%M:%S')}"
+    )
+
+    class_docstring = f'"""{ref_name.capitalize()} IDs for Fount API queries."""'
+
+    source_items = [
+        f'"""{ref_name.capitalize()} class for holding {ref_name} IDs."""',
+        updated_comment,
+        f"from {import_items[0]} import {import_items[1]}\n",
+        f"class {ref_name.capitalize()}({import_items[1]}):\n" f"    {class_docstring}",
+        "\n".join(f"    {k} = {v}" for k, v in ref_items.items()),
+    ]
+
+    return "\n\n".join(source_items) + "\n"
+
+
+def write_to_file(source: str, filepath: Path) -> None:
+    """Write updated module source to file.
+
+    Parameters
+    ----------
+    source : str
+        Updated module source as a string.
+    filepath : pathlib.Path
+        Path to write the source to.
+    """
+    if not filepath.parent.exists():
+        filepath.parent.mkdir(parents=True, exist_ok=True)
+
+    with open(filepath, "w", encoding="utf-8") as file:
+        file.write(source)
+
+
+def parse_args(argv: Optional[List[str]] = None) -> Args:
+    """Parse arguments given to the script.
+
+    Returns
+    -------
+    argparse.Namespace
+        Object containing arguments and values for the script
+    """
+    parser = argparse.ArgumentParser(
+        description="Generate reference files for commonly used BAV filters.\n\n"
+        "The script will generate a set of reference files that contain "
+        "helpful classes for filtering BAV data in readable form.\n\n"
+        "The currently available reference classes are Audiences and Countries.\n"
+        "These classess will be stored in a `bavapi_refs` folder in your "
+        "current working directory. "
+        "You can import them using `from bavapi_refs.audiences import Audiences`.\n"
+        "Existing reference files will be overwritten.",
+        epilog="DON'T PUSH REFERENCES TO GIT! Add `bavapi_refs/` to `.gitignore`.",
+    )
+    parser.add_argument(
+        "-a", "--all", action="store_true", help="Generate all reference files."
+    )
+    parser.add_argument(
+        "-n",
+        "--name",
+        default="",
+        choices={"audiences", "countries"},
+        help="Name of reference to generate.",
+    )
+    return Args(parser.parse_args(argv))
+
+
+def main(argv: Optional[List[str]] = None) -> int:
+    """Main function to generate reference classes.
+
+    Returns
+    -------
+    int
+        CLI exit code
+    """
+    load_dotenv()
+
+    args = parse_args(argv)
+    fount = Client(os.getenv("FOUNT_API_KEY", "no_key"))
+
+    base_path = Path.cwd() / "bavapi_refs"
+    print(base_path)
+
+    ref_configs: Dict[str, RefConfig] = {
+        "audiences": RefConfig("audiences", "audiences", parse_audiences),
+        "countries": RefConfig(
+            "studies",
+            "countries",
+            parse_countries,
+            "country_name",
+        ),
+    }
+
+    if args.all:
+        names, configs = list(ref_configs.keys()), list(ref_configs.values())
+    elif not args.name:
+        print("bavapi-refs: Run `bavapi-refs -h` for usage instructions.")
+        return 1
+    else:
+        names, configs = [args.name], [ref_configs[args.name]]
+
+    results = asyncio.run(get_references(fount, configs))
+
+    for name, data, config in zip(names, results, configs):
+        items = process_items(data, config)
+        source = generate_source(name, items, datetime.datetime.utcnow())
+        path = base_path / f"{name}.py"
+
+        print(f"Writing {name} file with {len(items)} items to {path}")
+        write_to_file(source, path)
+
+    print("Success!")
+    return 0
+
+
+if __name__ == "__main__":
+    raise SystemExit(main())  # pragma: no cover
```

### Comparing `wpp-bavapi-0.4.1/bavapi/sync.py` & `wpp-bavapi-0.5.0/bavapi/sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,457 +1,466 @@
-"""Convenience functions to perform queries to the Fount synchronously.
-
-Can be used directly without using `asyncio`.
-
-Meant for experimentation, Jupyter notebooks, one-off scripts, etc.
-
-Use `bavapi.Client` for more advanced usage and performance benefits.
-"""
-
-# pylint: disable=redefined-outer-name, too-many-arguments
-
-import asyncio
-import functools
-import sys
-from typing import TYPE_CHECKING, Any, Callable, Coroutine, Literal, Optional, TypeVar
-
-from bavapi import filters as _filters
-from bavapi.client import Client, OptionalFiltersOrMapping
-from bavapi.jupyter import patch_loop, running_in_jupyter
-from bavapi.query import Query
-from bavapi.typing import BaseListOrValues, JSONDict, OptionalListOr
-
-if sys.version_info < (3, 10):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec
-
-if TYPE_CHECKING:
-    from pandas import DataFrame
-
-__all__ = ("raw_query", "audiences", "brands", "brandscape_data", "studies")
-
-T = TypeVar("T")
-P = ParamSpec("P")
-F = TypeVar("F", bound=_filters.FountFilters)
-
-
-def _coro(func: Callable[P, Coroutine[Any, Any, T]]) -> Callable[P, T]:
-    @functools.wraps(func)
-    def wrapper(*args: P.args, **kwargs: P.kwargs):
-        try:
-            loop = asyncio.get_event_loop_policy().get_event_loop()
-        except RuntimeError:
-            loop = asyncio.new_event_loop()
-
-        coro = func(*args, **kwargs)
-
-        if running_in_jupyter():
-            patch_loop(loop)
-
-        return loop.run_until_complete(coro)
-
-    return wrapper
-
-
-@_coro
-async def raw_query(token: str, endpoint: str, params: Query[F]) -> list[JSONDict]:
-    """Perform a raw GET query to the Fount API, returning the response JSON data
-    instead of a `pandas` DataFrame.
-
-    Parameters
-    ----------
-    token : str
-        Fount API token
-    endpoint : str
-        Endpoint name
-    params : Query
-        Query `pydantic` model with query parameters.
-
-    Returns
-    -------
-    list[dict[str, Any]]
-        List of JSON response data
-    """
-
-    async with Client(token) as fount:
-        return await fount.raw_query(endpoint, params)
-
-
-@_coro
-async def audiences(
-    token: str,
-    name: Optional[str] = None,
-    audience_id: Optional[int] = None,
-    active: Literal[0, 1] = 0,
-    inactive: Literal[0, 1] = 0,
-    public: Literal[0, 1] = 0,
-    private: Literal[0, 1] = 0,
-    groups: OptionalListOr[int] = None,
-    *,
-    filters: OptionalFiltersOrMapping[_filters.AudiencesFilters] = None,
-    fields: OptionalListOr[str] = None,
-    include: OptionalListOr[str] = None,
-    stack_data: bool = False,
-    **kwargs: BaseListOrValues,
-) -> "DataFrame":
-    """Query the Fount `audiences` endpoint.
-
-    Parameters
-    ----------
-    token : str
-        Fount API token
-    name : str, optional
-        Search audiences by name, by default None
-    audience_id : int, optional
-        Fount audience ID, by default None
-
-        If an audience ID is provided, only that audience will be returned
-    active : Literal[0, 1]
-        Return active audiences only if set to `1`, by default 0
-    inactive : Literal[0, 1]
-        Return inactive audiences only if set to `1`, by default 0
-    public : Literal[0, 1]
-        Return active audiences only if set to `1`, by default 0
-    private : Literal[0, 1]
-        Return inactive audiences only if set to `1`, by default 0
-    groups : int or list[int], optional
-        Audience group ID or list of audience group IDs, by default None
-    filters : AudiencesFilters or dict of filters, optional
-        AudiencesFilters object or dictionary of filter parameters, by default None
-    fields : str or list[str], optional
-        Fields to retrieve in API response, by default None
-
-        Only specified fields are returned.
-        If `fields` is None, all fields are returned.
-    include : str or list[str], optional
-        Additional resources to include in API response, by default None
-    stack_data : bool, optional
-        Whether to expand nested lists into new dictionaries, by default False
-    **kwargs
-        Additional parameters to pass to the Query. See `Other Parameters`.
-        For any filters, use the `filters` parameter.
-
-    Other Parameters
-    ----------------
-    page : int, optional
-        Page number to fetch, by default None
-    per_page : int, optional
-        Number of results per page, by default None
-    max_pages : int, optional
-        Max number of results to return, by default None
-    sort : str, optional
-        Sort response by field, by default None
-
-        To sort in descending (highest first) order, use a `-` before the field name:
-
-        `sort="-differentiation_rank"`
-
-        Sorts by item ID by default.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame with `brands` endpoint results
-    """
-
-    async with Client(token) as fount:
-        return await fount.audiences(
-            name,
-            audience_id,
-            active,
-            inactive,
-            public,
-            private,
-            groups,
-            filters=filters,
-            fields=fields,
-            include=include,
-            stack_data=stack_data,
-            **kwargs,
-        )
-
-
-@_coro
-async def brands(
-    token: str,
-    name: Optional[str] = None,
-    country_codes: OptionalListOr[str] = None,
-    year_numbers: OptionalListOr[int] = None,
-    brand_id: Optional[int] = None,
-    studies: OptionalListOr[int] = None,
-    *,
-    filters: OptionalFiltersOrMapping[_filters.BrandsFilters] = None,
-    fields: OptionalListOr[str] = None,
-    include: OptionalListOr[str] = None,
-    stack_data: bool = False,
-    **kwargs: BaseListOrValues,
-) -> "DataFrame":
-    """Query the Fount `brands` endpoint
-
-    Parameters
-    ----------
-    token : str
-        Fount API token
-    name : str, optional
-        Search brands by name, by default None
-    country_codes: str or list[str], optional
-        ISO-3166-1 alpha-2 country codes, by default None
-    year_numbers : int or list[int], optional
-        Study years, by default None
-    brand_id : int, optional
-        Fount brand ID, by default None
-
-        If a brand ID is provided, only that brand will be returned
-    studies : int or list[int], optional
-        Fount study IDs, by default None
-    filters : BrandsFilters or dict of filters, optional
-        BrandsFilters object or dictionary of filter parameters, by default None
-    fields : str or list[str], optional
-        Fields to retrieve in API response, by default None
-
-        Only specified fields are returned.
-        If `fields` is None, all fields are returned.
-    include : str or list[str], optional
-        Additional resources to include in API response, by default None
-    stack_data : bool, optional
-        Whether to expand nested lists into new dictionaries, by default False
-    **kwargs
-        Additional parameters to pass to the Query. See `Other Parameters`.
-        For any filters, use the `filters` parameter.
-
-    Other Parameters
-    ----------------
-    page : int, optional
-        Page number to fetch, by default None
-    per_page : int, optional
-        Number of results per page, by default None
-    max_pages : int, optional
-        Max number of results to return, by default None
-    sort : str, optional
-        Sort response by field, by default None
-
-        To sort in descending (highest first) order, use a `-` before the field name:
-
-        `sort="-differentiation_rank"`
-
-        Sorts by item ID by default.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame with `brands` endpoint results
-    """
-
-    async with Client(token) as fount:
-        return await fount.brands(
-            name,
-            country_codes,
-            year_numbers,
-            brand_id,
-            studies,
-            filters=filters,
-            fields=fields,
-            include=include,
-            stack_data=stack_data,
-            **kwargs,
-        )
-
-
-@_coro
-async def brandscape_data(
-    token: str,
-    country_code: OptionalListOr[str] = None,
-    year_number: OptionalListOr[int] = None,
-    audiences: OptionalListOr[int] = None,
-    brand_name: Optional[str] = None,
-    studies: OptionalListOr[int] = None,
-    *,
-    filters: OptionalFiltersOrMapping[_filters.BrandscapeFilters] = None,
-    fields: OptionalListOr[str] = None,
-    include: OptionalListOr[str] = None,
-    metric_keys: OptionalListOr[str] = None,
-    stack_data: bool = False,
-    **kwargs: BaseListOrValues,
-) -> "DataFrame":
-    """Query the Fount `brandscape-data` endpoint.
-
-    This endpoint requires at least one of the following combinations of parameters:
-
-    - `studies`
-    - `brand_name` or `brands`
-    - `country_code` or `countries` and `brands` or `brand_name`
-    - `year_number` or `years` and `country_code` or `countries`
-
-    An audience filter is also highly recommended, as otherwise the API will return
-    data for all audiences (there are more than 30 standard audiences).
-
-    The `Audiences` class is provided to make it easier to filter audiences.
-
-    Note that this endpoint has a default set of `include` resources:
-    - `brand`
-    - `study`
-    - `category`
-
-    Any additional valid includes will be added to the default set.
-
-    If any of the default includes are used in `include`, then only that resource
-    will be retrieved. This is to allow requesting individual includes if they are
-    part of the default.
-
-    Parameters
-    ----------
-    token : str
-        Fount API token
-    country_code : str or list[str], optional
-        ISO-3166-1 alpha-2 country codes, by default None
-    year_number : int or list[int], optional
-        Study years, by default None
-    audiences : int or list[int], optional
-        Audiences to retrieve by audience ID, by default None
-
-        The `Audiences` class can help with this filter.
-    brand_name : str, optional
-        Search by brand name, by default None
-    studies : int or list[int], optional
-        Fount studies IDs, by default None
-    filters : BrandscapeFilters or dict of filters, optional
-        BrandscapeFilters object or dictionary of filter parameters, by default None
-    fields : str or list[str], optional
-        Fields to retrieve in API response, by default None
-
-        Only specified fields are returned.
-        If `fields` is None, all fields are returned.
-    include : str or list[str], optional
-        Additional resources to include in API response, by default None
-    stack_data : bool, optional
-        Whether to expand nested lists into new dictionaries, by default False
-    **kwargs
-        Additional parameters to pass to the Query. See `Other Parameters`.
-        For any filters, use the `filters` parameter.
-
-    Other Parameters
-    ----------------
-    page : int, optional
-        Page number to fetch, by default None
-    per_page : int, optional
-        Number of results per page, by default None
-    max_pages : int, optional
-        Max number of results to return, by default None
-    sort : str, optional
-        Sort response by field, by default None
-
-        To sort in descending (highest first) order, use a `-` before the field name:
-
-        `sort="-differentiation_rank"`
-
-        Sorts by item ID by default.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame with `brandscape-data` endpoint results
-
-    Raises
-    ------
-    ValidationError
-        If used with an invalid combination of parameters (see above)
-    """
-
-    async with Client(token) as fount:
-        return await fount.brandscape_data(
-            country_code,
-            year_number,
-            audiences,
-            brand_name,
-            studies,
-            filters=filters,
-            fields=fields,
-            metric_keys=metric_keys,
-            include=include,
-            stack_data=stack_data,
-            **kwargs,
-        )
-
-
-@_coro
-async def studies(
-    token: str,
-    country_codes: OptionalListOr[str] = None,
-    year_numbers: OptionalListOr[int] = None,
-    full_year: Literal[0, 1] = 0,
-    study_id: Optional[int] = None,
-    *,
-    filters: OptionalFiltersOrMapping[_filters.StudiesFilters] = None,
-    fields: OptionalListOr[str] = None,
-    include: OptionalListOr[str] = None,
-    stack_data: bool = False,
-    **kwargs: BaseListOrValues,
-) -> "DataFrame":
-    """Query the Fount `studies` endpoint.
-
-    Parameters
-    ----------
-    token : str
-        Fount API token
-    country_codes: str or list[str], optional
-        ISO-3166-1 alpha-2 country codes, by default None
-    year_numbers : int or list[int], optional
-        Study years, by default None
-    full_year : Literal[0, 1], optional
-        Include or exclude studies which are not "full year" studies,
-        such as US quarterly studies or special studies, by default 0
-
-        A value of 1 will filter non-full-year studies.
-    study_id : int, optional
-        Fount study ID, by default None
-        If a study ID is provided, only that study will be returned
-    filters : StudiesFilters or dict of filters, optional
-        StudiesFilters object or dictionary of filter parameters, by default None
-    fields : str or list[str], optional
-        Fields to retrieve in API response, by default None
-
-        Only specified fields are returned.
-        If `fields` is None, all fields are returned.
-    include : str or list[str], optional
-        Additional resources to include in API response, by default None
-    stack_data : bool, optional
-        Whether to expand nested lists into new dictionaries, by default False
-    **kwargs
-        Additional parameters to pass to the Query. See `Other Parameters`.
-        For any filters, use the `filters` parameter.
-
-    Other Parameters
-    ----------------
-    page : int, optional
-        Page number to fetch, by default None
-    per_page : int, optional
-        Number of results per page, by default None
-    max_pages : int, optional
-        Max number of results to return, by default None
-    sort : str, optional
-        Sort response by field, by default None
-
-        To sort in descending (highest first) order, use a `-` before the field name:
-
-        `sort="-differentiation_rank"`
-
-        Sorts by item ID by default.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame with `studies` endpoint results
-    """
-
-    async with Client(token) as fount:
-        return await fount.studies(
-            country_codes,
-            year_numbers,
-            full_year,
-            study_id,
-            filters=filters,
-            fields=fields,
-            include=include,
-            stack_data=stack_data,
-            **kwargs,
-        )
+"""Convenience functions to perform queries to the Fount synchronously.
+
+Can be used directly without using `asyncio`.
+
+Meant for experimentation, Jupyter notebooks, one-off scripts, etc.
+
+Use `bavapi.Client` for more advanced usage and performance benefits.
+"""
+
+# pylint: disable=redefined-outer-name, too-many-arguments
+
+import asyncio
+import functools
+import sys
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Coroutine,
+    List,
+    Literal,
+    Optional,
+    TypeVar,
+)
+
+from bavapi import filters as _filters
+from bavapi.client import Client, OptionalFiltersOrMapping
+from bavapi.jupyter import patch_loop, running_in_jupyter
+from bavapi.query import Query
+from bavapi.typing import BaseListOrValues, JSONDict, OptionalListOr
+
+if sys.version_info < (3, 10):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec
+
+if TYPE_CHECKING:
+    from pandas import DataFrame
+
+__all__ = ("raw_query", "audiences", "brands", "brandscape_data", "studies")
+
+T = TypeVar("T")
+P = ParamSpec("P")
+F = TypeVar("F", bound=_filters.FountFilters)
+
+
+def _coro(func: Callable[P, Coroutine[Any, Any, T]]) -> Callable[P, T]:
+    @functools.wraps(func)
+    def wrapper(*args: P.args, **kwargs: P.kwargs):
+        try:
+            loop = asyncio.get_event_loop_policy().get_event_loop()
+        except RuntimeError:
+            loop = asyncio.new_event_loop()
+
+        coro = func(*args, **kwargs)
+
+        if running_in_jupyter():
+            patch_loop(loop)
+
+        return loop.run_until_complete(coro)
+
+    return wrapper
+
+
+@_coro
+async def raw_query(token: str, endpoint: str, params: Query[F]) -> List[JSONDict]:
+    """Perform a raw GET query to the Fount API, returning the response JSON data
+    instead of a `pandas` DataFrame.
+
+    Parameters
+    ----------
+    token : str
+        Fount API token
+    endpoint : str
+        Endpoint name
+    params : Query
+        Query `pydantic` model with query parameters.
+
+    Returns
+    -------
+    list[dict[str, Any]]
+        List of JSON response data
+    """
+
+    async with Client(token) as fount:
+        return await fount.raw_query(endpoint, params)
+
+
+@_coro
+async def audiences(
+    token: str,
+    name: Optional[str] = None,
+    audience_id: Optional[int] = None,
+    active: Literal[0, 1] = 0,
+    inactive: Literal[0, 1] = 0,
+    public: Literal[0, 1] = 0,
+    private: Literal[0, 1] = 0,
+    groups: OptionalListOr[int] = None,
+    *,
+    filters: OptionalFiltersOrMapping[_filters.AudiencesFilters] = None,
+    fields: OptionalListOr[str] = None,
+    include: OptionalListOr[str] = None,
+    stack_data: bool = False,
+    **kwargs: BaseListOrValues,
+) -> "DataFrame":
+    """Query the Fount `audiences` endpoint.
+
+    Parameters
+    ----------
+    token : str
+        Fount API token
+    name : str, optional
+        Search audiences by name, by default None
+    audience_id : int, optional
+        Fount audience ID, by default None
+
+        If an audience ID is provided, only that audience will be returned
+    active : Literal[0, 1]
+        Return active audiences only if set to `1`, by default 0
+    inactive : Literal[0, 1]
+        Return inactive audiences only if set to `1`, by default 0
+    public : Literal[0, 1]
+        Return active audiences only if set to `1`, by default 0
+    private : Literal[0, 1]
+        Return inactive audiences only if set to `1`, by default 0
+    groups : int or list[int], optional
+        Audience group ID or list of audience group IDs, by default None
+    filters : AudiencesFilters or dict of filters, optional
+        AudiencesFilters object or dictionary of filter parameters, by default None
+    fields : str or list[str], optional
+        Fields to retrieve in API response, by default None
+
+        Only specified fields are returned.
+        If `fields` is None, all fields are returned.
+    include : str or list[str], optional
+        Additional resources to include in API response, by default None
+    stack_data : bool, optional
+        Whether to expand nested lists into new dictionaries, by default False
+    **kwargs
+        Additional parameters to pass to the Query. See `Other Parameters`.
+        For any filters, use the `filters` parameter.
+
+    Other Parameters
+    ----------------
+    page : int, optional
+        Page number to fetch, by default None
+    per_page : int, optional
+        Number of results per page, by default None
+    max_pages : int, optional
+        Max number of results to return, by default None
+    sort : str, optional
+        Sort response by field, by default None
+
+        To sort in descending (highest first) order, use a `-` before the field name:
+
+        `sort="-differentiation_rank"`
+
+        Sorts by item ID by default.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with `brands` endpoint results
+    """
+
+    async with Client(token) as fount:
+        return await fount.audiences(
+            name,
+            audience_id,
+            active,
+            inactive,
+            public,
+            private,
+            groups,
+            filters=filters,
+            fields=fields,
+            include=include,
+            stack_data=stack_data,
+            **kwargs,
+        )
+
+
+@_coro
+async def brands(
+    token: str,
+    name: Optional[str] = None,
+    country_codes: OptionalListOr[str] = None,
+    year_numbers: OptionalListOr[int] = None,
+    brand_id: Optional[int] = None,
+    studies: OptionalListOr[int] = None,
+    *,
+    filters: OptionalFiltersOrMapping[_filters.BrandsFilters] = None,
+    fields: OptionalListOr[str] = None,
+    include: OptionalListOr[str] = None,
+    stack_data: bool = False,
+    **kwargs: BaseListOrValues,
+) -> "DataFrame":
+    """Query the Fount `brands` endpoint
+
+    Parameters
+    ----------
+    token : str
+        Fount API token
+    name : str, optional
+        Search brands by name, by default None
+    country_codes: str or list[str], optional
+        ISO-3166-1 alpha-2 country codes, by default None
+    year_numbers : int or list[int], optional
+        Study years, by default None
+    brand_id : int, optional
+        Fount brand ID, by default None
+
+        If a brand ID is provided, only that brand will be returned
+    studies : int or list[int], optional
+        Fount study IDs, by default None
+    filters : BrandsFilters or dict of filters, optional
+        BrandsFilters object or dictionary of filter parameters, by default None
+    fields : str or list[str], optional
+        Fields to retrieve in API response, by default None
+
+        Only specified fields are returned.
+        If `fields` is None, all fields are returned.
+    include : str or list[str], optional
+        Additional resources to include in API response, by default None
+    stack_data : bool, optional
+        Whether to expand nested lists into new dictionaries, by default False
+    **kwargs
+        Additional parameters to pass to the Query. See `Other Parameters`.
+        For any filters, use the `filters` parameter.
+
+    Other Parameters
+    ----------------
+    page : int, optional
+        Page number to fetch, by default None
+    per_page : int, optional
+        Number of results per page, by default None
+    max_pages : int, optional
+        Max number of results to return, by default None
+    sort : str, optional
+        Sort response by field, by default None
+
+        To sort in descending (highest first) order, use a `-` before the field name:
+
+        `sort="-differentiation_rank"`
+
+        Sorts by item ID by default.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with `brands` endpoint results
+    """
+
+    async with Client(token) as fount:
+        return await fount.brands(
+            name,
+            country_codes,
+            year_numbers,
+            brand_id,
+            studies,
+            filters=filters,
+            fields=fields,
+            include=include,
+            stack_data=stack_data,
+            **kwargs,
+        )
+
+
+@_coro
+async def brandscape_data(
+    token: str,
+    country_code: OptionalListOr[str] = None,
+    year_number: OptionalListOr[int] = None,
+    audiences: OptionalListOr[int] = None,
+    brand_name: Optional[str] = None,
+    studies: OptionalListOr[int] = None,
+    *,
+    filters: OptionalFiltersOrMapping[_filters.BrandscapeFilters] = None,
+    fields: OptionalListOr[str] = None,
+    include: OptionalListOr[str] = None,
+    metric_keys: OptionalListOr[str] = None,
+    stack_data: bool = False,
+    **kwargs: BaseListOrValues,
+) -> "DataFrame":
+    """Query the Fount `brandscape-data` endpoint.
+
+    This endpoint requires at least one of the following combinations of parameters:
+
+    - `studies`
+    - `brand_name` or `brands`
+    - `country_code` or `countries` and `brands` or `brand_name`
+    - `year_number` or `years` and `country_code` or `countries`
+
+    An audience filter is also highly recommended, as otherwise the API will return
+    data for all audiences (there are more than 30 standard audiences).
+
+    The `Audiences` class is provided to make it easier to filter audiences.
+
+    Note that this endpoint has a default set of `include` resources:
+    - `brand`
+    - `study`
+    - `category`
+
+    Any additional valid includes will be added to the default set.
+
+    If any of the default includes are used in `include`, then only that resource
+    will be retrieved. This is to allow requesting individual includes if they are
+    part of the default.
+
+    Parameters
+    ----------
+    token : str
+        Fount API token
+    country_code : str or list[str], optional
+        ISO-3166-1 alpha-2 country codes, by default None
+    year_number : int or list[int], optional
+        Study years, by default None
+    audiences : int or list[int], optional
+        Audiences to retrieve by audience ID, by default None
+
+        The `Audiences` class can help with this filter.
+    brand_name : str, optional
+        Search by brand name, by default None
+    studies : int or list[int], optional
+        Fount studies IDs, by default None
+    filters : BrandscapeFilters or dict of filters, optional
+        BrandscapeFilters object or dictionary of filter parameters, by default None
+    fields : str or list[str], optional
+        Fields to retrieve in API response, by default None
+
+        Only specified fields are returned.
+        If `fields` is None, all fields are returned.
+    include : str or list[str], optional
+        Additional resources to include in API response, by default None
+    stack_data : bool, optional
+        Whether to expand nested lists into new dictionaries, by default False
+    **kwargs
+        Additional parameters to pass to the Query. See `Other Parameters`.
+        For any filters, use the `filters` parameter.
+
+    Other Parameters
+    ----------------
+    page : int, optional
+        Page number to fetch, by default None
+    per_page : int, optional
+        Number of results per page, by default None
+    max_pages : int, optional
+        Max number of results to return, by default None
+    sort : str, optional
+        Sort response by field, by default None
+
+        To sort in descending (highest first) order, use a `-` before the field name:
+
+        `sort="-differentiation_rank"`
+
+        Sorts by item ID by default.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with `brandscape-data` endpoint results
+
+    Raises
+    ------
+    ValidationError
+        If used with an invalid combination of parameters (see above)
+    """
+
+    async with Client(token) as fount:
+        return await fount.brandscape_data(
+            country_code,
+            year_number,
+            audiences,
+            brand_name,
+            studies,
+            filters=filters,
+            fields=fields,
+            metric_keys=metric_keys,
+            include=include,
+            stack_data=stack_data,
+            **kwargs,
+        )
+
+
+@_coro
+async def studies(
+    token: str,
+    country_codes: OptionalListOr[str] = None,
+    year_numbers: OptionalListOr[int] = None,
+    full_year: Literal[0, 1] = 0,
+    study_id: Optional[int] = None,
+    *,
+    filters: OptionalFiltersOrMapping[_filters.StudiesFilters] = None,
+    fields: OptionalListOr[str] = None,
+    include: OptionalListOr[str] = None,
+    stack_data: bool = False,
+    **kwargs: BaseListOrValues,
+) -> "DataFrame":
+    """Query the Fount `studies` endpoint.
+
+    Parameters
+    ----------
+    token : str
+        Fount API token
+    country_codes: str or list[str], optional
+        ISO-3166-1 alpha-2 country codes, by default None
+    year_numbers : int or list[int], optional
+        Study years, by default None
+    full_year : Literal[0, 1], optional
+        Include or exclude studies which are not "full year" studies,
+        such as US quarterly studies or special studies, by default 0
+
+        A value of 1 will filter non-full-year studies.
+    study_id : int, optional
+        Fount study ID, by default None
+        If a study ID is provided, only that study will be returned
+    filters : StudiesFilters or dict of filters, optional
+        StudiesFilters object or dictionary of filter parameters, by default None
+    fields : str or list[str], optional
+        Fields to retrieve in API response, by default None
+
+        Only specified fields are returned.
+        If `fields` is None, all fields are returned.
+    include : str or list[str], optional
+        Additional resources to include in API response, by default None
+    stack_data : bool, optional
+        Whether to expand nested lists into new dictionaries, by default False
+    **kwargs
+        Additional parameters to pass to the Query. See `Other Parameters`.
+        For any filters, use the `filters` parameter.
+
+    Other Parameters
+    ----------------
+    page : int, optional
+        Page number to fetch, by default None
+    per_page : int, optional
+        Number of results per page, by default None
+    max_pages : int, optional
+        Max number of results to return, by default None
+    sort : str, optional
+        Sort response by field, by default None
+
+        To sort in descending (highest first) order, use a `-` before the field name:
+
+        `sort="-differentiation_rank"`
+
+        Sorts by item ID by default.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with `studies` endpoint results
+    """
+
+    async with Client(token) as fount:
+        return await fount.studies(
+            country_codes,
+            year_numbers,
+            full_year,
+            study_id,
+            filters=filters,
+            fields=fields,
+            include=include,
+            stack_data=stack_data,
+            **kwargs,
+        )
```

### Comparing `wpp-bavapi-0.4.1/bavapi/typing.py` & `wpp-bavapi-0.5.0/bavapi/typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,63 @@
-"""Common parameter types"""
-
-import datetime
-from typing import Mapping, MutableMapping, Optional, Sequence, TypeVar, Union
-
-T = TypeVar("T")
-
-# VALUE PRIMITIVES
-
-BaseValues = Optional[Union[str, int, float]]
-DTValues = Optional[Union[str, datetime.datetime, datetime.date]]
-
-# MUTABLE ABSTRACT COLLECTIONS
-
-SequenceOrValues = Union[T, Sequence[T]]
-
-ParamsMapping = Mapping[str, T]
-MutableParamsMapping = MutableMapping[str, T]
-
-BaseSequenceOrValues = SequenceOrValues[BaseValues]
-InputSequenceOrValues = Union[BaseSequenceOrValues, DTValues]
-
-BaseParamsMapping = ParamsMapping[BaseSequenceOrValues]
-BaseParamsMappingValues = ParamsMapping[BaseValues]
-BaseMutableParamsMapping = MutableParamsMapping[BaseSequenceOrValues]
-BaseMutableParamsMappingValues = MutableParamsMapping[BaseValues]
-
-InputParamsMapping = ParamsMapping[InputSequenceOrValues]
-InputMutableParamsMapping = MutableParamsMapping[InputSequenceOrValues]
-
-# MUTABLE CONCRETE COLLECTIONS
-
-ListOrValues = Union[T, list[T]]
-
-ParamsDict = dict[str, T]
-
-BaseListOrValues = ListOrValues[BaseValues]
-InputListOrValues = Union[BaseListOrValues, DTValues]
-
-BaseParamsDict = ParamsDict[BaseListOrValues]
-BaseParamsDictValues = ParamsDict[BaseValues]
-
-InputParamsDict = ParamsDict[InputListOrValues]
-
-# USER-FACING
-
-OptionalSequenceOr = Optional[Union[T, Sequence[T]]]
-OptionalListOr = Optional[Union[T, list[T]]]
-
-JSONDict = dict[str, ListOrValues[Union[BaseValues, "JSONDict"]]]
-JSONData = Union[JSONDict, list[JSONDict]]
-
-FlatJSONDict = dict[str, BaseSequenceOrValues]
-FlatJSONDictValues = dict[str, BaseValues]
+"""Common parameter types"""
+
+import datetime
+from typing import (
+    Dict,
+    List,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
+
+T = TypeVar("T")
+
+# VALUE PRIMITIVES
+
+BaseValues = Optional[Union[str, int, float]]
+DTValues = Optional[Union[str, datetime.datetime, datetime.date]]
+
+# MUTABLE ABSTRACT COLLECTIONS
+
+SequenceOrValues = Union[T, Sequence[T]]
+
+ParamsMapping = Mapping[str, T]
+MutableParamsMapping = MutableMapping[str, T]
+
+BaseSequenceOrValues = SequenceOrValues[BaseValues]
+InputSequenceOrValues = Union[BaseSequenceOrValues, DTValues]
+
+BaseParamsMapping = ParamsMapping[BaseSequenceOrValues]
+BaseParamsMappingValues = ParamsMapping[BaseValues]
+BaseMutableParamsMapping = MutableParamsMapping[BaseSequenceOrValues]
+BaseMutableParamsMappingValues = MutableParamsMapping[BaseValues]
+
+InputParamsMapping = ParamsMapping[InputSequenceOrValues]
+InputMutableParamsMapping = MutableParamsMapping[InputSequenceOrValues]
+
+# MUTABLE CONCRETE COLLECTIONS
+
+ListOrValues = Union[T, List[T]]
+
+ParamsDict = Dict[str, T]
+
+BaseListOrValues = ListOrValues[BaseValues]
+InputListOrValues = Union[BaseListOrValues, DTValues]
+
+BaseParamsDict = ParamsDict[BaseListOrValues]
+BaseParamsDictValues = ParamsDict[BaseValues]
+
+InputParamsDict = ParamsDict[InputListOrValues]
+
+# USER-FACING
+
+OptionalSequenceOr = Optional[Union[T, Sequence[T]]]
+OptionalListOr = Optional[Union[T, List[T]]]
+
+JSONDict = Dict[str, ListOrValues[Union[BaseValues, "JSONDict"]]]
+JSONData = Union[JSONDict, List[JSONDict]]
+
+FlatJSONDict = Dict[str, BaseSequenceOrValues]
+FlatJSONDictValues = Dict[str, BaseValues]
```

### Comparing `wpp-bavapi-0.4.1/noxfile.py` & `wpp-bavapi-0.5.0/noxfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,197 +1,200 @@
-"""Package tooling session definitions for `nox`"""
-
-import json
-import os
-import pathlib
-
-import nox
-
-
-@nox.session(python=("3.9", "3.10", "3.11"))
-def tests(session: nox.Session) -> None:
-    """Run tests on CI/CD pipeline."""
-    session.install("-e", ".[test]")
-
-    session.run(
-        "coverage",
-        "run",
-        "-m",
-        "--parallel",
-        "pytest",
-        "-m",
-        "not e2e",
-        *session.posargs,
-    )
-
-
-@nox.session(python=("3.9", "3.10", "3.11"))
-def tests_nocov(session: nox.Session) -> None:
-    """Run tests on CI/CD pipeline with no coverage."""
-    session.install("-e", ".[test]")
-
-    session.run("pytest", "-m", "not e2e", *session.posargs)
-
-
-@nox.session(python="3.11")
-def tests_e2e(session: nox.Session) -> None:
-    """Run end to end tests on CI/CD pipeline."""
-    session.install("-e", ".[test]")
-
-    session.run(
-        "coverage",
-        "run",
-        "-m",
-        "--parallel",
-        "pytest",
-        "-m",
-        "e2e",
-        *session.posargs,
-    )
-
-
-@nox.session(python="3.11")
-def tests_e2e_nocov(session: nox.Session) -> None:
-    """Run end to end tests on CI/CD pipeline with no coverage."""
-    session.install("-e", ".[test]")
-
-    session.run("pytest", "-m", "e2e", *session.posargs)
-
-
-@nox.session(python=("3.9", "3.10", "3.11"), venv_backend="mamba", reuse_venv=True)
-def tests_mamba(session: nox.Session) -> None:
-    """Run tests locally with `mamba` as the backend."""
-    session.conda_install("--file", "requirements.txt")
-    session.install("-e", ".[test]")
-
-    session.run(
-        "coverage",
-        "run",
-        "-m",
-        "--parallel",
-        "pytest",
-        "-m",
-        "not e2e",
-        *session.posargs,
-        external=True,
-    )
-
-
-@nox.session(python=("3.9", "3.10", "3.11"), venv_backend="mamba", reuse_venv=True)
-def tests_mamba_nocov(session: nox.Session) -> None:
-    """Run tests locally with `mamba` as the backend with no coverage."""
-    session.conda_install("--file", "requirements.txt")
-    session.install("-e", ".[test]")
-
-    session.run("pytest", "-m", "not e2e", *session.posargs, external=True)
-
-
-@nox.session(python="3.11", venv_backend="mamba", reuse_venv=True)
-def tests_mamba_e2e(session: nox.Session) -> None:
-    """Run end to end tests locally with `mamba` as the backend."""
-    session.conda_install("--file", "requirements.txt")
-    session.install("-e", ".[test]")
-
-    session.run(
-        "coverage",
-        "run",
-        "-m",
-        "--parallel",
-        "pytest",
-        "-m",
-        "e2e",
-        *session.posargs,
-        external=True,
-    )
-
-
-@nox.session(python="3.11", venv_backend="mamba", reuse_venv=True)
-def tests_mamba_e2e_nocov(session: nox.Session) -> None:
-    """Run end to end tests locally with `mamba` as the backend with no coverage."""
-    session.conda_install("--file", "requirements.txt")
-    session.install("-e", ".[test]")
-
-    session.run("pytest", "-m", "e2e", *session.posargs, external=True)
-
-
-@nox.session(python="3.11")
-def coverage(session: nox.Session) -> None:
-    """Compile and process coverage reports."""
-    args = session.posargs or ["report"]
-
-    session.install("coverage[toml]")
-
-    if not session.posargs and any(pathlib.Path().glob(".coverage.*")):
-        session.run("coverage", "combine")
-
-    session.run("coverage", *args)
-
-    if os.getenv("CI"):
-        session.run("coverage", "json")
-
-        with open("coverage.json", encoding="utf-8") as file:
-            total: str = json.load(file)["totals"]["percent_covered_display"]
-
-        with open(os.environ["GITHUB_ENV"], "a", encoding="utf-8") as file:
-            file.write(f"total={total}")
-
-        print(f"{total=} added to GITHUB_ENV.")
-
-        with open(os.environ["GITHUB_STEP_SUMMARY"], "a", encoding="utf-8") as file:
-            file.write(f"### Total coverage: {total}%")
-
-
-@nox.session(python="3.11")
-def lint(session: nox.Session) -> None:
-    """Lint package."""
-    session.install("pylint", "mypy")
-    session.install("-e", ".")
-
-    session.run("pylint", "bavapi")
-    session.run("mypy", "bavapi")
-
-
-@nox.session(python=None)
-def requirements(session: nox.Session) -> None:
-    """Run pip-tools to prepare `requirements.txt` files."""
-
-    # nox should only run this function in python 3.11 so this should be safe
-    import tomllib  # pylint: disable=import-outside-toplevel
-
-    session.install("pip-tools")
-
-    if "all-extras" not in session.posargs:
-        session.run(
-            "pip-compile", "--resolver=backtracking", "pyproject.toml", *session.posargs
-        )
-    else:
-        session.posargs.remove("all-extras")
-        with open("pyproject.toml", "rb") as file:
-            deps: dict[str, list[str]] = tomllib.load(file)["project"].get(
-                "optional-dependencies", {}
-            )
-
-        for dep in deps:
-            session.run(
-                "pip-compile",
-                f"--extra={dep}",
-                f"--output-file={dep}-requirements.txt",
-                "--resolver=backtracking",
-                "pyproject.toml",
-                *session.posargs,
-            )
-
-
-@nox.session(python=None)
-def build(session: nox.Session) -> None:
-    """Build package wheel and source distribution into dist folder."""
-    session.install("build")
-
-    session.run("python -m build")
-
-
-@nox.session(python=None)
-def publish(session: nox.Session) -> None:
-    """Publish package wheel and source distribution to PyPI."""
-    session.install("twine")
-
-    session.run("twine", "upload", "--repository", "wpp-bavapi", "dist/*")
+"""Package tooling session definitions for `nox`"""
+
+import json
+import os
+import pathlib
+from typing import Dict, List
+
+import nox
+
+python_versions = ("3.8", "3.9", "3.10", "3.11")
+
+
+@nox.session(python=python_versions)
+def tests(session: nox.Session) -> None:
+    """Run tests on CI/CD pipeline."""
+    session.install("-e", ".[test]")
+
+    session.run(
+        "coverage",
+        "run",
+        "-m",
+        "--parallel",
+        "pytest",
+        "-m",
+        "not e2e",
+        *session.posargs,
+    )
+
+
+@nox.session(python=python_versions)
+def tests_nocov(session: nox.Session) -> None:
+    """Run tests on CI/CD pipeline with no coverage."""
+    session.install("-e", ".[test]")
+
+    session.run("pytest", "-m", "not e2e", *session.posargs)
+
+
+@nox.session(python="3.11")
+def tests_e2e(session: nox.Session) -> None:
+    """Run end to end tests on CI/CD pipeline."""
+    session.install("-e", ".[test]")
+
+    session.run(
+        "coverage",
+        "run",
+        "-m",
+        "--parallel",
+        "pytest",
+        "-m",
+        "e2e",
+        *session.posargs,
+    )
+
+
+@nox.session(python="3.11")
+def tests_e2e_nocov(session: nox.Session) -> None:
+    """Run end to end tests on CI/CD pipeline with no coverage."""
+    session.install("-e", ".[test]")
+
+    session.run("pytest", "-m", "e2e", *session.posargs)
+
+
+@nox.session(python=python_versions, venv_backend="mamba", reuse_venv=True)
+def tests_mamba(session: nox.Session) -> None:
+    """Run tests locally with `mamba` as the backend."""
+    session.conda_install("--file", "requirements.txt")
+    session.install("-e", ".[test]")
+
+    session.run(
+        "coverage",
+        "run",
+        "-m",
+        "--parallel",
+        "pytest",
+        "-m",
+        "not e2e",
+        *session.posargs,
+        external=True,
+    )
+
+
+@nox.session(python=python_versions, venv_backend="mamba", reuse_venv=True)
+def tests_mamba_nocov(session: nox.Session) -> None:
+    """Run tests locally with `mamba` as the backend with no coverage."""
+    session.conda_install("--file", "requirements.txt")
+    session.install("-e", ".[test]")
+
+    session.run("pytest", "-m", "not e2e", *session.posargs, external=True)
+
+
+@nox.session(python="3.11", venv_backend="mamba", reuse_venv=True)
+def tests_mamba_e2e(session: nox.Session) -> None:
+    """Run end to end tests locally with `mamba` as the backend."""
+    session.conda_install("--file", "requirements.txt")
+    session.install("-e", ".[test]")
+
+    session.run(
+        "coverage",
+        "run",
+        "-m",
+        "--parallel",
+        "pytest",
+        "-m",
+        "e2e",
+        *session.posargs,
+        external=True,
+    )
+
+
+@nox.session(python="3.11", venv_backend="mamba", reuse_venv=True)
+def tests_mamba_e2e_nocov(session: nox.Session) -> None:
+    """Run end to end tests locally with `mamba` as the backend with no coverage."""
+    session.conda_install("--file", "requirements.txt")
+    session.install("-e", ".[test]")
+
+    session.run("pytest", "-m", "e2e", *session.posargs, external=True)
+
+
+@nox.session(python="3.11")
+def coverage(session: nox.Session) -> None:
+    """Compile and process coverage reports."""
+    args = session.posargs or ["report"]
+
+    session.install("coverage[toml]")
+
+    if not session.posargs and any(pathlib.Path().glob(".coverage.*")):
+        session.run("coverage", "combine")
+
+    session.run("coverage", *args)
+
+    if os.getenv("CI"):
+        session.run("coverage", "json")
+
+        with open("coverage.json", encoding="utf-8") as file:
+            total: str = json.load(file)["totals"]["percent_covered_display"]
+
+        with open(os.environ["GITHUB_ENV"], "a", encoding="utf-8") as file:
+            file.write(f"total={total}")
+
+        print(f"{total=} added to GITHUB_ENV.")
+
+        with open(os.environ["GITHUB_STEP_SUMMARY"], "a", encoding="utf-8") as file:
+            file.write(f"### Total coverage: {total}%")
+
+
+@nox.session(python="3.11")
+def lint(session: nox.Session) -> None:
+    """Lint package."""
+    session.install("pylint", "mypy")
+    session.install("-e", ".")
+
+    session.run("pylint", "bavapi")
+    session.run("mypy", "bavapi")
+
+
+@nox.session(python=None)
+def requirements(session: nox.Session) -> None:
+    """Run pip-tools to prepare `requirements.txt` files."""
+
+    # nox should only run this function in python 3.11 so this should be safe
+    import tomllib  # pylint: disable=import-outside-toplevel
+
+    session.install("pip-tools")
+
+    if "all-extras" not in session.posargs:
+        session.run(
+            "pip-compile", "--resolver=backtracking", "pyproject.toml", *session.posargs
+        )
+    else:
+        session.posargs.remove("all-extras")
+        with open("pyproject.toml", "rb") as file:
+            deps: Dict[str, List[str]] = tomllib.load(file)["project"].get(
+                "optional-dependencies", {}
+            )
+
+        for dep in deps:
+            session.run(
+                "pip-compile",
+                f"--extra={dep}",
+                f"--output-file={dep}-requirements.txt",
+                "--resolver=backtracking",
+                "pyproject.toml",
+                *session.posargs,
+            )
+
+
+@nox.session(python=None)
+def build(session: nox.Session) -> None:
+    """Build package wheel and source distribution into dist folder."""
+    session.install("build")
+
+    session.run("python", "-m", "build")
+
+
+@nox.session(python=None)
+def publish(session: nox.Session) -> None:
+    """Publish package wheel and source distribution to PyPI."""
+    session.install("twine")
+
+    session.run("twine", "upload", "dist/*")
```

### Comparing `wpp-bavapi-0.4.1/tests/integration/test_async.py` & `wpp-bavapi-0.5.0/tests/integration/test_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# pylint: disable=missing-module-docstring, missing-function-docstring
-# pylint: disable=redefined-outer-name, protected-access
-
-import os
-import ssl
-from typing import Any, AsyncGenerator, Callable, Coroutine
-
-import pandas as pd
-import pytest
-from dotenv import load_dotenv
-
-from bavapi import filters
-from bavapi.client import Client
-from bavapi.query import Query
-
-
-@pytest.mark.anyio
-@pytest.fixture(scope="module")
-async def fount() -> AsyncGenerator[Client, None]:
-    load_dotenv()
-
-    async with Client(os.environ["FOUNT_API_KEY"]) as _fount:
-        yield _fount
-
-
-@pytest.mark.e2e
-@pytest.mark.anyio
-async def test_raw_query(fount: Client):
-    result: list[dict[str, Any]] = []
-    for _ in range(5):  # pragma: no cover
-        try:
-            result = await fount.raw_query(
-                "countries",
-                Query(filters={"is_active": 1}, include="region", max_pages=2),
-            )
-            break
-        except ssl.SSLError:
-            print("Failed due to SSL error...")
-            continue
-
-    assert result
-    assert len(result) == 200
-    assert "region" in result[0]
-
-
-@pytest.mark.e2e
-@pytest.mark.anyio
-async def test_with_filters_one_page(fount: Client):
-    result: pd.DataFrame = pd.DataFrame()
-    for _ in range(5):  # pragma: no cover
-        try:
-            result = await fount.studies(
-                filters=filters.StudiesFilters(active=1),
-                include="country",
-                page=1,
-                per_page=25,
-            )
-            break
-        except ssl.SSLError:
-            print("Failed due to SSL error...")
-            continue
-
-    assert "country_id" in result
-    assert result["is_active"].unique()[0] == 1
-    assert result.shape[0] == 25
-
-
-@pytest.mark.e2e
-@pytest.mark.anyio
-@pytest.mark.parametrize(
-    ("endpoint", "filters"),
-    (
-        ("audiences", {}),
-        ("brands", {}),
-        ("brandscape_data", {"studies": 546}),
-        ("studies", {}),
-    ),
-)
-async def test_endpoints(fount: Client, endpoint: str, filters: dict[str, Any]):
-    func: Callable[..., Coroutine[Any, Any, pd.DataFrame]] = getattr(fount, endpoint)
-
-    result = await func(filters=filters, max_pages=2, per_page=25)
-
-    assert result.shape[0] == 50
-    assert "id" in result
+# pylint: disable=missing-module-docstring, missing-function-docstring
+# pylint: disable=redefined-outer-name, protected-access
+
+import os
+import ssl
+from typing import Any, AsyncGenerator, Callable, Coroutine, Dict, List
+
+import pandas as pd
+import pytest
+from dotenv import load_dotenv
+
+from bavapi import filters
+from bavapi.client import Client
+from bavapi.query import Query
+
+
+@pytest.mark.anyio
+@pytest.fixture(scope="module")
+async def fount() -> AsyncGenerator[Client, None]:
+    load_dotenv()
+
+    async with Client(os.environ["FOUNT_API_KEY"]) as _fount:
+        yield _fount
+
+
+@pytest.mark.e2e
+@pytest.mark.anyio
+async def test_raw_query(fount: Client):
+    result: List[Dict[str, Any]] = []
+    for _ in range(5):  # pragma: no cover
+        try:
+            result = await fount.raw_query(
+                "countries",
+                Query(filters={"is_active": 1}, include="region", max_pages=2),
+            )
+            break
+        except ssl.SSLError:
+            print("Failed due to SSL error...")
+            continue
+
+    assert result
+    assert len(result) == 200
+    assert "region" in result[0]
+
+
+@pytest.mark.e2e
+@pytest.mark.anyio
+async def test_with_filters_one_page(fount: Client):
+    result: pd.DataFrame = pd.DataFrame()
+    for _ in range(5):  # pragma: no cover
+        try:
+            result = await fount.studies(
+                filters=filters.StudiesFilters(active=1),
+                include="country",
+                page=1,
+                per_page=25,
+            )
+            break
+        except ssl.SSLError:
+            print("Failed due to SSL error...")
+            continue
+
+    assert "country_id" in result
+    assert result["is_active"].unique()[0] == 1
+    assert result.shape[0] == 25
+
+
+@pytest.mark.e2e
+@pytest.mark.anyio
+@pytest.mark.parametrize(
+    ("endpoint", "filters"),
+    (
+        ("audiences", {}),
+        ("brands", {}),
+        ("brandscape_data", {"studies": 546}),
+        ("studies", {}),
+    ),
+)
+async def test_endpoints(fount: Client, endpoint: str, filters: Dict[str, Any]):
+    func: Callable[..., Coroutine[Any, Any, pd.DataFrame]] = getattr(fount, endpoint)
+
+    result = await func(filters=filters, max_pages=2, per_page=25)
+
+    assert result.shape[0] == 50
+    assert "id" in result
```

### Comparing `wpp-bavapi-0.4.1/tests/integration/test_sync.py` & `wpp-bavapi-0.5.0/tests/integration/test_sync.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,83 @@
-# pylint: disable=missing-module-docstring, missing-function-docstring
-# pylint: disable=redefined-outer-name, protected-access
-
-import os
-import ssl
-from typing import Any, Callable, Generator
-
-import pandas as pd
-import pytest
-from dotenv import load_dotenv
-
-import bavapi
-from bavapi import filters
-from bavapi.query import Query
-
-
-@pytest.fixture(scope="module", autouse=True)
-def load_env() -> Generator[None, None, None]:
-    load_dotenv()
-    yield
-
-
-@pytest.mark.e2e
-def test_raw_query():
-    result: list[dict[str, Any]] = []
-    for _ in range(5):  # pragma: no cover
-        try:
-            result = bavapi.raw_query(
-                os.environ["FOUNT_API_KEY"],
-                "countries",
-                Query(filters={"is_active": 1}, include="region", max_pages=2),
-            )
-            break
-        except ssl.SSLError:
-            print("Failed due to SSL error...")
-            continue
-
-    assert result
-    assert len(result) == 200
-    assert "region" in result[0]
-
-
-@pytest.mark.e2e
-def test_with_filters_one_page():
-    result: pd.DataFrame = pd.DataFrame()
-    for _ in range(5):  # pragma: no cover
-        try:
-            result = bavapi.studies(
-                os.environ["FOUNT_API_KEY"],
-                filters=filters.StudiesFilters(active=1),
-                include="country",
-                page=1,
-                per_page=25,
-            )
-            break
-        except ssl.SSLError:
-            print("Failed due to SSL error...")
-            continue
-
-    assert "country_id" in result
-    assert result["is_active"].unique()[0] == 1
-    assert result.shape[0] == 25
-
-
-@pytest.mark.e2e
-@pytest.mark.parametrize(
-    ("endpoint", "filters"),
-    (
-        ("audiences", {}),
-        ("brands", {}),
-        ("brandscape_data", {"studies": 546}),
-        ("studies", {}),
-    ),
-)
-def test_endpoints(endpoint: str, filters: dict[str, Any]):
-    func: Callable[..., pd.DataFrame] = getattr(bavapi, endpoint)
-
-    result = func(os.environ["FOUNT_API_KEY"], filters=filters, max_pages=2, per_page=25)
-
-    assert result.shape[0] == 50
-    assert "id" in result
+# pylint: disable=missing-module-docstring, missing-function-docstring
+# pylint: disable=redefined-outer-name, protected-access
+
+import os
+import ssl
+from typing import Any, Callable, Dict, Generator, List
+
+import pandas as pd
+import pytest
+from dotenv import load_dotenv
+
+import bavapi
+from bavapi import filters
+from bavapi.query import Query
+
+
+@pytest.fixture(scope="module", autouse=True)
+def load_env() -> Generator[None, None, None]:
+    load_dotenv()
+    yield
+
+
+@pytest.mark.e2e
+def test_raw_query():
+    result: List[Dict[str, Any]] = []
+    for _ in range(5):  # pragma: no cover
+        try:
+            result = bavapi.raw_query(
+                os.environ["FOUNT_API_KEY"],
+                "countries",
+                Query(filters={"is_active": 1}, include="region", max_pages=2),
+            )
+            break
+        except ssl.SSLError:
+            print("Failed due to SSL error...")
+            continue
+
+    assert result
+    assert len(result) == 200
+    assert "region" in result[0]
+
+
+@pytest.mark.e2e
+def test_with_filters_one_page():
+    result: pd.DataFrame = pd.DataFrame()
+    for _ in range(5):  # pragma: no cover
+        try:
+            result = bavapi.studies(
+                os.environ["FOUNT_API_KEY"],
+                filters=filters.StudiesFilters(active=1),
+                include="country",
+                page=1,
+                per_page=25,
+            )
+            break
+        except ssl.SSLError:
+            print("Failed due to SSL error...")
+            continue
+
+    assert "country_id" in result
+    assert result["is_active"].unique()[0] == 1  # type: ignore
+    assert result.shape[0] == 25
+
+
+@pytest.mark.e2e
+@pytest.mark.parametrize(
+    ("endpoint", "filters"),
+    (
+        ("audiences", {}),
+        ("brands", {}),
+        ("brandscape_data", {"studies": 546}),
+        ("studies", {}),
+    ),
+)
+def test_endpoints(endpoint: str, filters: Dict[str, Any]):
+    func: Callable[..., pd.DataFrame] = getattr(bavapi, endpoint)
+
+    result = func(
+        os.environ["FOUNT_API_KEY"], filters=filters, max_pages=2, per_page=25
+    )
+
+    assert result.shape[0] == 50
+    assert "id" in result
```

### Comparing `wpp-bavapi-0.4.1/tests/parsing/test_params.py` & `wpp-bavapi-0.5.0/tests/parsing/test_params.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring
-
-import datetime
-
-import pytest
-
-from bavapi.parsing import params
-
-
-def test_to_fount_params():
-    assert params.to_fount_params({"test": 1}, "param") == {"param[test]": 1}
-
-
-@pytest.mark.parametrize(
-    ("value", "expected"),
-    (
-        ("2020-07-01 12:00:00", "2020-07-01 12:00:00"),
-        (datetime.datetime(2020, 7, 1, 12, 0, 0), "2020-07-01 12:00:00"),
-        (datetime.date(2020, 7, 1), "2020-07-01 00:00:00"),
-        ("2020-07-01", "2020-07-01 00:00:00"),
-    ),
-)
-def test_parse_date(value, expected):
-    assert params.parse_date(value) == expected
-
-
-@pytest.mark.parametrize(
-    "value",
-    ("bad_string", "2022-012-02 00:00:00"),
-)
-def test_parse_date_fails(value):
-    with pytest.raises(ValueError):
-        params.parse_date(value)
-
-
-def test_list_to_str():
-    parsed = params.list_to_str({"a": [1, 2], "b": 4})
-
-    assert parsed == {"a": "1,2", "b": 4}
+# pylint: disable=missing-function-docstring, missing-module-docstring
+
+import datetime
+
+import pytest
+
+from bavapi.parsing import params
+
+
+def test_to_fount_params():
+    assert params.to_fount_params({"test": 1}, "param") == {"param[test]": 1}
+
+
+@pytest.mark.parametrize(
+    ("value", "expected"),
+    (
+        ("2020-07-01 12:00:00", "2020-07-01 12:00:00"),
+        (datetime.datetime(2020, 7, 1, 12, 0, 0), "2020-07-01 12:00:00"),
+        (datetime.date(2020, 7, 1), "2020-07-01 00:00:00"),
+        ("2020-07-01", "2020-07-01 00:00:00"),
+    ),
+)
+def test_parse_date(value, expected):
+    assert params.parse_date(value) == expected
+
+
+@pytest.mark.parametrize(
+    "value",
+    ("bad_string", "2022-012-02 00:00:00"),
+)
+def test_parse_date_fails(value):
+    with pytest.raises(ValueError):
+        params.parse_date(value)
+
+
+def test_list_to_str():
+    parsed = params.list_to_str({"a": [1, 2], "b": 4})
+
+    assert parsed == {"a": "1,2", "b": 4}
```

### Comparing `wpp-bavapi-0.4.1/tests/reference/test_generate_reference.py` & `wpp-bavapi-0.5.0/tests/reference/test_generate_reference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# pylint: disable=redefined-outer-name, missing-function-docstring, missing-module-docstring
-
-import datetime
-from pathlib import Path
-from typing import Callable, Optional, TypeVar
-from unittest import mock
-
-import pandas as pd
-import pytest
-
-from bavapi.client import Client
-from bavapi.query import Query
-from bavapi.reference import generate_reference as uref
-
-TEST_DT = datetime.datetime(2023, 1, 1, 12, 0, 0)
-
-
-T = TypeVar("T")
-
-
-def wraps(return_value: Optional[T] = None) -> Callable[..., Optional[T]]:
-    def _wraps(*_, **__):
-        return return_value
-
-    return _wraps
-
-
-@pytest.fixture(scope="session")
-def anyio_backend() -> str:
-    return "asyncio"
-
-
-@pytest.fixture
-def fount(monkeypatch: pytest.MonkeyPatch) -> Client:
-    _fount = Client("TOKEN")
-
-    async def mock_func(*_, **__):
-        return [{"id": 1, "name": "A"}, {"id": 2, "name": "B"}]
-
-    monkeypatch.setattr(_fount, "raw_query", mock_func)
-
-    return _fount
-
-
-def test_parse_reference():
-    mock_data = pd.Series(("ITEM ONE", "ITEM 2"))
-
-    parsed = uref.parse_reference(mock_data, {" ": "_"}, {"2": "TWO"})
-
-    assert parsed == {"ITEM_ONE": "0", "ITEM_TWO": "1"}
-
-
-@pytest.mark.anyio
-async def test_get_references(fount: Client):
-    def func(x: pd.Series) -> dict[str, str]:
-        return {str(k): str(v) for k, v in x.to_dict().items()}  # pragma: no cover
-
-    items = await uref.get_references(fount, [uref.RefConfig("test", "", func)])
-
-    assert items == [[{"id": 1, "name": "A"}, {"id": 2, "name": "B"}]]
-
-
-def test_process_items():
-    data = [
-        {"id": 1, "name": "A", "is_active": 1},
-        {"id": 2, "name": "B", "is_active": 0},
-    ]
-    config = uref.RefConfig(
-        "test", "", lambda x: {str(k): str(v) for k, v in x.items()}
-    )
-
-    processed = uref.process_items(data, config)
-
-    assert processed == {"1": "A"}
-
-
-def test_generate_source():
-    updated_source = (
-        '"""Tests class for holding tests IDs."""\n\n'
-        "# This file was generated from active tests in the Fount.\n"
-        f"# Tests retrieved on {TEST_DT.strftime('%Y-%m-%d %H:%M:%S')}\n\n"
-        "from bavapi.reference._int_enum import IntEnum\n\n\n"
-        'class Tests(IntEnum):\n    """Tests IDs for Fount API queries."""\n\n'
-        "    A = 1\n"
-    )
-
-    assert (
-        uref.generate_source("tests", {"A": "1"}, TEST_DT).splitlines()
-        == updated_source.splitlines()
-    )
-
-
-@mock.patch("bavapi.reference.generate_reference.Path.exists", return_value=True)
-def test_write_to_file(mock_exists: mock.MagicMock):
-    with mock.patch("builtins.open", new_callable=mock.mock_open) as mock_open:
-        uref.write_to_file("", Path("folder/blah.py"))
-
-    mock_open.assert_called_once_with(Path("folder/blah.py"), "w", encoding="utf-8")
-    mock_exists.assert_called_once()
-
-
-@mock.patch("bavapi.reference.generate_reference.Path.mkdir")
-def test_write_to_file_not_exists(mock_mkdir: mock.MagicMock):
-    with mock.patch("builtins.open", new_callable=mock.mock_open) as mock_open:
-        uref.write_to_file("", Path("folder/blah.py"))
-
-    mock_open.assert_called_once_with(Path("folder/blah.py"), "w", encoding="utf-8")
-    mock_mkdir.assert_called_once_with(parents=True, exist_ok=True)
-
-
-def test_parse_args_name():
-    argv = ["-n", "audiences"]
-
-    args = uref.parse_args(argv)
-
-    assert not args.all
-    assert args.name == "audiences"
-
-
-def test_parse_args_all():
-    argv = ["-a"]
-
-    args = uref.parse_args(argv)
-
-    assert args.all
-    assert args.name == ""
-
-
-def test_main_no_args():
-    assert uref.main([]) == 1
-
-
-@mock.patch(
-    "bavapi.reference.generate_reference.Client.raw_query",
-    wraps=wraps([{"id": 1, "name": "A"}, {"id": 2, "name": "B"}]),
-)
-@mock.patch("bavapi.reference.generate_reference.write_to_file")
-def test_main(mock_write_to_file: mock.Mock, mock_raw_query: mock.AsyncMock):
-    args = ["-n", "audiences"]
-
-    uref.main(args)
-
-    mock_write_to_file.assert_called_once()
-    mock_raw_query.assert_awaited_once_with("audiences", Query())
-
-
-@mock.patch(
-    "bavapi.reference.generate_reference.Client.raw_query",
-    wraps=wraps(
-        [
-            {"id": 1, "name": "A", "country_name": "A"},
-            {"id": 2, "name": "B", "country_name": "B"},
-        ]
-    ),
-)
-@mock.patch("bavapi.reference.generate_reference.write_to_file")
-def test_main_all(mock_write_to_file: mock.Mock, mock_raw_query: mock.AsyncMock):
-    args = ["-a"]
-
-    uref.main(args)
-
-    assert len(mock_write_to_file.call_args_list) == 2
-    assert len(mock_raw_query.call_args_list) == 2
+# pylint: disable=redefined-outer-name, missing-function-docstring, missing-module-docstring
+
+import datetime
+from pathlib import Path
+from typing import Callable, Dict, Optional, TypeVar
+from unittest import mock
+
+import pandas as pd
+import pytest
+
+from bavapi.client import Client
+from bavapi.query import Query
+from bavapi.reference import generate_reference as uref
+
+TEST_DT = datetime.datetime(2023, 1, 1, 12, 0, 0)
+
+
+T = TypeVar("T")
+
+
+def wraps(return_value: Optional[T] = None) -> Callable[..., Optional[T]]:
+    def _wraps(*_, **__):
+        return return_value
+
+    return _wraps
+
+
+@pytest.fixture(scope="session")
+def anyio_backend() -> str:
+    return "asyncio"
+
+
+@pytest.fixture
+def fount(monkeypatch: pytest.MonkeyPatch) -> Client:
+    _fount = Client("TOKEN")
+
+    async def mock_func(*_, **__):
+        return [{"id": 1, "name": "A"}, {"id": 2, "name": "B"}]
+
+    monkeypatch.setattr(_fount, "raw_query", mock_func)
+
+    return _fount
+
+
+def test_parse_reference():
+    mock_data = pd.Series(("ITEM ONE", "ITEM 2"))
+
+    parsed = uref.parse_reference(mock_data, {" ": "_"}, {"2": "TWO"})
+
+    assert parsed == {"ITEM_ONE": "0", "ITEM_TWO": "1"}
+
+
+@pytest.mark.anyio
+async def test_get_references(fount: Client):
+    def func(x: pd.Series) -> Dict[str, str]:
+        return {str(k): str(v) for k, v in x.to_dict().items()}  # pragma: no cover
+
+    items = await uref.get_references(fount, [uref.RefConfig("test", "", func)])
+
+    assert items == [[{"id": 1, "name": "A"}, {"id": 2, "name": "B"}]]
+
+
+def test_process_items():
+    data = [
+        {"id": 1, "name": "A", "is_active": 1},
+        {"id": 2, "name": "B", "is_active": 0},
+    ]
+    config = uref.RefConfig(
+        "test", "", lambda x: {str(k): str(v) for k, v in x.items()}
+    )
+
+    processed = uref.process_items(data, config)
+
+    assert processed == {"1": "A"}
+
+
+def test_generate_source():
+    updated_source = (
+        '"""Tests class for holding tests IDs."""\n\n'
+        "# This file was generated from active tests in the Fount.\n"
+        f"# Tests retrieved on {TEST_DT.strftime('%Y-%m-%d %H:%M:%S')}\n\n"
+        "from bavapi.reference._int_enum import IntEnum\n\n\n"
+        'class Tests(IntEnum):\n    """Tests IDs for Fount API queries."""\n\n'
+        "    A = 1\n"
+    )
+
+    assert (
+        uref.generate_source("tests", {"A": "1"}, TEST_DT).splitlines()
+        == updated_source.splitlines()
+    )
+
+
+@mock.patch("bavapi.reference.generate_reference.Path.exists", return_value=True)
+def test_write_to_file(mock_exists: mock.MagicMock):
+    with mock.patch("builtins.open", new_callable=mock.mock_open) as mock_open:
+        uref.write_to_file("", Path("folder/blah.py"))
+
+    mock_open.assert_called_once_with(Path("folder/blah.py"), "w", encoding="utf-8")
+    mock_exists.assert_called_once()
+
+
+@mock.patch("bavapi.reference.generate_reference.Path.mkdir")
+def test_write_to_file_not_exists(mock_mkdir: mock.MagicMock):
+    with mock.patch("builtins.open", new_callable=mock.mock_open) as mock_open:
+        uref.write_to_file("", Path("folder/blah.py"))
+
+    mock_open.assert_called_once_with(Path("folder/blah.py"), "w", encoding="utf-8")
+    mock_mkdir.assert_called_once_with(parents=True, exist_ok=True)
+
+
+def test_parse_args_name():
+    argv = ["-n", "audiences"]
+
+    args = uref.parse_args(argv)
+
+    assert not args.all
+    assert args.name == "audiences"
+
+
+def test_parse_args_all():
+    argv = ["-a"]
+
+    args = uref.parse_args(argv)
+
+    assert args.all
+    assert args.name == ""
+
+
+def test_main_no_args():
+    assert uref.main([]) == 1
+
+
+@mock.patch(
+    "bavapi.reference.generate_reference.Client.raw_query",
+    wraps=wraps([{"id": 1, "name": "A"}, {"id": 2, "name": "B"}]),
+)
+@mock.patch("bavapi.reference.generate_reference.write_to_file")
+def test_main(mock_write_to_file: mock.Mock, mock_raw_query: mock.AsyncMock):
+    args = ["-n", "audiences"]
+
+    uref.main(args)
+
+    mock_write_to_file.assert_called_once()
+    mock_raw_query.assert_awaited_once_with("audiences", Query())
+
+
+@mock.patch(
+    "bavapi.reference.generate_reference.Client.raw_query",
+    wraps=wraps(
+        [
+            {"id": 1, "name": "A", "country_name": "A"},
+            {"id": 2, "name": "B", "country_name": "B"},
+        ]
+    ),
+)
+@mock.patch("bavapi.reference.generate_reference.write_to_file")
+def test_main_all(mock_write_to_file: mock.Mock, mock_raw_query: mock.AsyncMock):
+    args = ["-a"]
+
+    uref.main(args)
+
+    assert len(mock_write_to_file.call_args_list) == 2
+    assert len(mock_raw_query.call_args_list) == 2
```

### Comparing `wpp-bavapi-0.4.1/tests/test_client.py` & `wpp-bavapi-0.5.0/tests/test_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,137 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring
-# pylint: disable=protected-access, redefined-outer-name
-
-from typing import Optional, TypeVar, Union
-from unittest import mock
-
-import pytest
-
-from bavapi.client import Client, _default_brandscape_include
-from bavapi.http import HTTPClient
-from bavapi.query import Query
-
-from .helpers import wraps
-
-T = TypeVar("T")
-
-# CLASS INIT TESTS
-
-
-def test_init():
-    fount = Client("test_token")
-    assert isinstance(fount._client, HTTPClient)
-
-
-def test_init_with_client(client: HTTPClient):
-    fount = Client(client=client)
-    assert fount._client is client
-
-
-def test_init_no_token():
-    with pytest.raises(ValueError) as excinfo:
-        Client()
-
-    assert excinfo.value.args[0] == "You must provide `auth_token` or `client`."
-
-
-# PUBLIC TESTS
-
-
-def test_per_page():
-    _fount = Client("token")
-    assert _fount.per_page == 100
-    _fount.per_page = 1000
-    assert _fount._client.per_page == 1000
-
-
-@pytest.mark.anyio
-async def test_context_manager():
-    _fount = Client(client=HTTPClient())
-    async with _fount as fount_ctx:
-        assert isinstance(fount_ctx, Client)
-
-    assert _fount._client.client.is_closed
-
-
-@pytest.mark.anyio
-async def test_aclose(fount: Client):
-    with mock.patch("bavapi.client.HTTPClient.aclose", wraps=wraps()) as mock_aclose:
-        await fount.aclose()
-
-    mock_aclose.assert_called_once()
-
-@pytest.mark.anyio
-async def test_raw_query(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"t": 1}])
-    ) as mock_base_query:
-        assert await fount.raw_query("request", Query()) == [{"t": 1}]
-
-    mock_base_query.assert_awaited_once_with("request", Query())
-
-
-@pytest.mark.anyio
-async def test_audiences(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1}])
-    ) as mock_base_query:
-        assert (await fount.audiences(audience_id=1)).shape == (1, 1)
-
-    mock_base_query.assert_awaited_once_with("audiences", Query(id=1))
-
-
-@pytest.mark.anyio
-async def test_brands(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1}])
-    ) as mock_base_query:
-        assert (await fount.brands(brand_id=1)).shape == (1, 1)
-
-    mock_base_query.assert_awaited_once_with("brands", Query(id=1))
-
-
-@pytest.mark.anyio
-async def test_brandscape_data(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1, "2": 2}])
-    ) as mock_base_query:
-        res = await fount.brandscape_data(fields="")
-        assert res.shape == (1, 2)
-
-    mock_base_query.assert_awaited_once_with(
-        "brandscape-data",
-        Query(fields="", include=["study", "brand", "category", "audience"]),
-    )
-
-
-@pytest.mark.anyio
-async def test_studies(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1, "2": 2}])
-    ) as mock_base_query:
-        assert (await fount.studies(study_id=1)).shape == (1, 2)
-
-    mock_base_query.assert_awaited_once_with("studies", Query(id=1))
-
-
-@pytest.mark.parametrize(
-    ("value", "expected"),
-    (
-        ("test", {"brand", "study", "category", "audience", "test"}),
-        (None, {"brand", "study", "category", "audience"}),
-        (["test"], {"brand", "study", "category", "audience", "test"}),
-    ),
-)
-def test_brandscape_query_default_include(
-    value: Optional[Union[str, list[str]]], expected: set[str]
-):
-    assert set(_default_brandscape_include(value)) == expected  # type: ignore
-
-
-def test_brandscape_query_default_include_partial():
-    assert _default_brandscape_include("brand") == "brand"
-
-
-def test_brandscape_query_no_default_include():
-    assert _default_brandscape_include("no_default") is None
+# pylint: disable=missing-function-docstring, missing-module-docstring
+# pylint: disable=protected-access, redefined-outer-name
+
+from typing import List, Optional, Set, TypeVar, Union
+from unittest import mock
+
+import pytest
+
+from bavapi.client import Client, _default_brandscape_include
+from bavapi.http import HTTPClient
+from bavapi.query import Query
+
+from .helpers import wraps
+
+T = TypeVar("T")
+
+# CLASS INIT TESTS
+
+
+def test_init():
+    fount = Client("test_token")
+    assert isinstance(fount._client, HTTPClient)
+
+
+def test_init_with_client(client: HTTPClient):
+    fount = Client(client=client)
+    assert fount._client is client
+
+
+def test_init_no_token():
+    with pytest.raises(ValueError) as excinfo:
+        Client()
+
+    assert excinfo.value.args[0] == "You must provide `auth_token` or `client`."
+
+
+# PUBLIC TESTS
+
+
+def test_per_page():
+    _fount = Client("token")
+    assert _fount.per_page == 100
+    _fount.per_page = 1000
+    assert _fount._client.per_page == 1000
+
+
+@pytest.mark.anyio
+async def test_context_manager():
+    _fount = Client(client=HTTPClient())
+    async with _fount as fount_ctx:
+        assert isinstance(fount_ctx, Client)
+
+    assert _fount._client.client.is_closed
+
+
+@pytest.mark.anyio
+async def test_aclose(fount: Client):
+    with mock.patch("bavapi.client.HTTPClient.aclose", wraps=wraps()) as mock_aclose:
+        await fount.aclose()
+
+    mock_aclose.assert_called_once()
+
+
+@pytest.mark.anyio
+async def test_raw_query(fount: Client):
+    with mock.patch.object(
+        fount._client, "query", wraps=wraps([{"t": 1}])
+    ) as mock_base_query:
+        assert await fount.raw_query("request", Query()) == [{"t": 1}]
+
+    mock_base_query.assert_awaited_once_with("request", Query())
+
+
+@pytest.mark.anyio
+async def test_audiences(fount: Client):
+    with mock.patch.object(
+        fount._client, "query", wraps=wraps([{"1": 1}])
+    ) as mock_base_query:
+        assert (await fount.audiences(audience_id=1)).shape == (1, 1)
+
+    mock_base_query.assert_awaited_once_with("audiences", Query(id=1))
+
+
+@pytest.mark.anyio
+async def test_brands(fount: Client):
+    with mock.patch.object(
+        fount._client, "query", wraps=wraps([{"1": 1}])
+    ) as mock_base_query:
+        assert (await fount.brands(brand_id=1)).shape == (1, 1)
+
+    mock_base_query.assert_awaited_once_with("brands", Query(id=1))
+
+
+@pytest.mark.anyio
+async def test_brandscape_data(fount: Client):
+    with mock.patch.object(
+        fount._client, "query", wraps=wraps([{"1": 1, "2": 2}])
+    ) as mock_base_query:
+        res = await fount.brandscape_data(fields="")
+        assert res.shape == (1, 2)
+
+    mock_base_query.assert_awaited_once_with(
+        "brandscape-data",
+        Query(fields="", include=["study", "brand", "category", "audience"]),
+    )
+
+
+@pytest.mark.anyio
+async def test_studies(fount: Client):
+    with mock.patch.object(
+        fount._client, "query", wraps=wraps([{"1": 1, "2": 2}])
+    ) as mock_base_query:
+        assert (await fount.studies(study_id=1)).shape == (1, 2)
+
+    mock_base_query.assert_awaited_once_with("studies", Query(id=1))
+
+
+@pytest.mark.parametrize(
+    ("value", "expected"),
+    (
+        ("test", {"brand", "study", "category", "audience", "test"}),
+        (None, {"brand", "study", "category", "audience"}),
+        (["test"], {"brand", "study", "category", "audience", "test"}),
+    ),
+)
+def test_brandscape_query_default_include(
+    value: Optional[Union[str, List[str]]], expected: Set[str]
+):
+    assert set(_default_brandscape_include(value)) == expected  # type: ignore
+
+
+def test_brandscape_query_default_include_partial():
+    assert _default_brandscape_include("brand") == "brand"
+
+
+def test_brandscape_query_no_default_include():
+    assert _default_brandscape_include("no_default") is None
```

### Comparing `wpp-bavapi-0.4.1/tests/test_http.py` & `wpp-bavapi-0.5.0/tests/test_http.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring
-# pylint: disable=protected-access, redefined-outer-name
-
-from dataclasses import asdict, dataclass
-from typing import Any, Optional, TypeVar, Union
-from unittest import mock
-
-import httpx
-import pytest
-
-from bavapi.http import (
-    APIError,
-    DataNotFoundError,
-    HTTPClient,
-    RateLimitExceededError,
-)
-from bavapi.query import Query
-
-from .helpers import wraps
-
-T = TypeVar("T")
-
-# HELPERS
-
-
-@dataclass
-class QueryResult:
-    """Model for WPPBAV Fount query results"""
-
-    data: Union[dict[str, Any], list[dict[str, Any]]]
-    links: dict[str, str]
-    meta: dict[str, Any]
-
-    def dict(self) -> dict[str, Any]:
-        return asdict(self)
-
-
-def response(
-    status_code: int = 200,
-    message: str = "ok",
-    *,
-    json: Optional[Any] = None,
-    request_url: str = "http://test_url/request",
-    headers: Optional[httpx.Headers] = None,
-) -> httpx.Response:
-    return httpx.Response(
-        status_code=status_code,
-        json=json if json is not None else {"message": message},
-        request=httpx.Request("GET", url=request_url),
-        headers=headers
-        or httpx.Headers({"x-ratelimit-remaining": "500", "x-ratelimit-limit": "500"}),
-    )
-
-
-def sample_data(
-    data: Optional[Union[dict[str, Any], list[dict[str, Any]]]] = None,
-    per_page: int = 25,
-    on_page: int = 25,
-    total: int = 2000,
-) -> dict[str, Any]:
-    return QueryResult(
-        data=data if data is not None else {},
-        links={},
-        meta={
-            "per_page": per_page,
-            "to": on_page,
-            "total": total,
-        },
-    ).dict()
-
-
-def empty_response() -> httpx.Response:
-    return response(json=sample_data([{}]))
-
-
-def rate_limited_response() -> httpx.Response:
-    return response(
-        200,
-        json=sample_data([{}]),
-        headers=httpx.Headers(
-            {"x-ratelimit-remaining": "1", "x-ratelimit-limit": "500"}
-        ),
-    )
-
-
-# TESTS
-
-
-def test_client_init_with_client():
-    httpx_client = httpx.AsyncClient()
-
-    client = HTTPClient(client=httpx_client)
-
-    assert client.client is httpx_client
-
-
-@pytest.mark.anyio
-async def test_context_manager():
-    client = HTTPClient()
-    async with client as client:
-        assert isinstance(client, HTTPClient)
-
-    assert client.client.is_closed
-
-@pytest.mark.anyio
-async def test_aclose(client: HTTPClient):
-    with mock.patch("bavapi.http.httpx.AsyncClient.aclose", wraps=wraps()) as mock_aclose:
-        await client.aclose()
-
-    mock_aclose.assert_called_once()
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.httpx.AsyncClient.get", wraps=wraps(response()))
-async def test_get(mock_get: mock.AsyncMock, client: HTTPClient):
-    resp = await client.get("request", Query())
-
-    assert resp.status_code == 200
-    assert resp.json() == {"message": "ok"}
-
-    mock_get.assert_awaited_once_with("request", params={})
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.httpx.AsyncClient.get", wraps=wraps(response()))
-async def test_get_with_id(mock_get: mock.AsyncMock, client: HTTPClient):
-    assert await client.get("request", Query(id=1))
-
-    mock_get.assert_awaited_once_with("request/1")
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.httpx.AsyncClient.get", wraps=wraps(response(400, "bad.")))
-async def test_get_blah(mock_get: mock.AsyncMock, client: HTTPClient):
-    with pytest.raises(APIError) as excinfo:
-        await client.get("request", Query())
-
-    mock_get.assert_awaited_once_with("request", params={})
-
-    assert excinfo.value.args == ("Error 400:\nbad.\nurl=http://test_url/request",)
-
-
-@pytest.mark.anyio
-@mock.patch(
-    "bavapi.http.httpx.AsyncClient.get",
-    wraps=wraps(response(400, json={"data": "bad"})),
-)
-async def test_get_bad_error(mock_get: mock.AsyncMock, client: HTTPClient):
-    with pytest.raises(APIError) as excinfo:
-        await client.get("request", Query())
-
-    mock_get.assert_awaited_once_with("request", params={})
-
-    assert excinfo.value.args == (
-        "Error 400:\nAn error occurred with the Fount.\nurl=http://test_url/request",
-    )
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(["page"]))
-async def test_get_pages(mock_get: mock.AsyncMock, client: HTTPClient):
-    res = await client.get_pages("request", Query(), 1)
-
-    assert res == [["page"]]
-    mock_get.assert_awaited_once_with("request", Query(page=1, per_page=100))
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(raises=ValueError))
-async def test_get_pages_fails(mock_get: mock.AsyncMock, client: HTTPClient):
-    with pytest.raises(ValueError):  # raised from mocked `get` method
-        await client.get_pages("request", Query(), 1)
-
-    mock_get.assert_awaited_once()
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps([empty_response()]))
-@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(empty_response()))
-async def test_query(
-    mock_get: mock.AsyncMock,
-    mock_get_pages: mock.AsyncMock,
-    client: HTTPClient,
-):
-    assert len(tuple(await client.query("request", Query()))) == 1
-
-    mock_get.assert_awaited_once_with("request", params=Query())
-    mock_get_pages.assert_awaited_once_with("request", Query(), 20)
-
-
-@pytest.mark.anyio
-@mock.patch(
-    "bavapi.http.HTTPClient.get_pages",
-    wraps=wraps([response(json=sample_data([{"a": 1}]))]),
-)
-@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(empty_response()))
-async def test_query_per_page(
-    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
-):
-    assert len(tuple(await client.query("request", Query(per_page=25)))) == 1
-
-    mock_get.assert_awaited_once()
-    mock_get_pages.assert_awaited_once_with("request", Query(per_page=25), 80)
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
-@mock.patch(
-    "bavapi.http.HTTPClient.get",
-    wraps=wraps(response(json=sample_data([{"t": 1}], total=1, on_page=1))),
-)
-async def test_query_one_page(
-    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
-):
-    # should be a list of dictionaries
-    assert list(await client.query("request", Query())) == [{"t": 1}]
-
-    mock_get.assert_awaited_once()
-    mock_get_pages.assert_not_awaited()
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
-@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(response(json=sample_data({}))))
-async def test_query_no_results(
-    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
-):
-    with pytest.raises(DataNotFoundError) as excinfo:
-        await client.query("request", Query())
-
-    mock_get.assert_awaited_once()
-    mock_get_pages.assert_not_awaited()
-    assert excinfo.value.args[0] == "Your query returned no results."
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
-@mock.patch(
-    "bavapi.http.HTTPClient.get",
-    wraps=wraps(response(json=sample_data({"t": 1}))),
-)
-async def test_query_by_id(
-    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
-):
-    assert list(await client.query("request", Query(id=1))) == [{"t": 1}]
-
-    mock_get.assert_awaited_once()
-    mock_get_pages.assert_not_awaited()
-
-
-@pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
-@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(rate_limited_response()))
-async def test_query_rate_limit(
-    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
-):
-    with pytest.raises(RateLimitExceededError) as excinfo:
-        await client.query("request", Query())
-
-    mock_get.assert_awaited_once()
-    mock_get_pages.assert_not_awaited()
-    assert excinfo.value.args[0] == (
-        "Number of pages (20) for this request "
-        "exceeds the rate limit (1, "
-        "total=500)."
-    )
+# pylint: disable=missing-function-docstring, missing-module-docstring
+# pylint: disable=protected-access, redefined-outer-name
+
+from dataclasses import asdict, dataclass
+from typing import Any, Dict, List, Optional, TypeVar, Union
+from unittest import mock
+
+import httpx
+import pytest
+
+from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
+from bavapi.http import HTTPClient
+from bavapi.query import Query
+
+from .helpers import wraps
+
+T = TypeVar("T")
+
+# HELPERS
+
+
+@dataclass
+class QueryResult:
+    """Model for WPPBAV Fount query results"""
+
+    data: Union[Dict[str, Any], List[Dict[str, Any]]]
+    links: Dict[str, str]
+    meta: Dict[str, Any]
+
+    def dict(self) -> Dict[str, Any]:
+        return asdict(self)
+
+
+def response(
+    status_code: int = 200,
+    message: str = "ok",
+    *,
+    json: Optional[Any] = None,
+    request_url: str = "http://test_url/request",
+    headers: Optional[httpx.Headers] = None,
+) -> httpx.Response:
+    return httpx.Response(
+        status_code=status_code,
+        json=json if json is not None else {"message": message},
+        request=httpx.Request("GET", url=request_url),
+        headers=headers
+        or httpx.Headers({"x-ratelimit-remaining": "500", "x-ratelimit-limit": "500"}),
+    )
+
+
+def sample_data(
+    data: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
+    per_page: int = 25,
+    on_page: int = 25,
+    total: int = 2000,
+) -> Dict[str, Any]:
+    return QueryResult(
+        data=data if data is not None else {},
+        links={},
+        meta={
+            "per_page": per_page,
+            "to": on_page,
+            "total": total,
+        },
+    ).dict()
+
+
+def empty_response() -> httpx.Response:
+    return response(json=sample_data([{}]))
+
+
+def rate_limited_response() -> httpx.Response:
+    return response(
+        200,
+        json=sample_data([{}]),
+        headers=httpx.Headers(
+            {"x-ratelimit-remaining": "1", "x-ratelimit-limit": "500"}
+        ),
+    )
+
+
+# TESTS
+
+
+def test_client_init_with_client():
+    httpx_client = httpx.AsyncClient()
+
+    client = HTTPClient(client=httpx_client)
+
+    assert client.client is httpx_client
+
+
+@pytest.mark.anyio
+async def test_context_manager():
+    client = HTTPClient()
+    async with client as client:
+        assert isinstance(client, HTTPClient)
+
+    assert client.client.is_closed
+
+
+@pytest.mark.anyio
+async def test_aclose(client: HTTPClient):
+    with mock.patch(
+        "bavapi.http.httpx.AsyncClient.aclose", wraps=wraps()
+    ) as mock_aclose:
+        await client.aclose()
+
+    mock_aclose.assert_called_once()
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.httpx.AsyncClient.get", wraps=wraps(response()))
+async def test_get(mock_get: mock.AsyncMock, client: HTTPClient):
+    resp = await client.get("request", Query())
+
+    assert resp.status_code == 200
+    assert resp.json() == {"message": "ok"}
+
+    mock_get.assert_awaited_once_with("request", params={})
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.httpx.AsyncClient.get", wraps=wraps(response()))
+async def test_get_with_id(mock_get: mock.AsyncMock, client: HTTPClient):
+    assert await client.get("request", Query(id=1))
+
+    mock_get.assert_awaited_once_with("request/1")
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.httpx.AsyncClient.get", wraps=wraps(response(400, "bad.")))
+async def test_get_blah(mock_get: mock.AsyncMock, client: HTTPClient):
+    with pytest.raises(APIError) as excinfo:
+        await client.get("request", Query())
+
+    mock_get.assert_awaited_once_with("request", params={})
+
+    assert excinfo.value.args == ("Error 400:\nbad.\nurl=http://test_url/request",)
+
+
+@pytest.mark.anyio
+@mock.patch(
+    "bavapi.http.httpx.AsyncClient.get",
+    wraps=wraps(response(400, json={"data": "bad"})),
+)
+async def test_get_bad_error(mock_get: mock.AsyncMock, client: HTTPClient):
+    with pytest.raises(APIError) as excinfo:
+        await client.get("request", Query())
+
+    mock_get.assert_awaited_once_with("request", params={})
+
+    assert excinfo.value.args == (
+        "Error 400:\nAn error occurred with the Fount.\nurl=http://test_url/request",
+    )
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(["page"]))
+async def test_get_pages(mock_get: mock.AsyncMock, client: HTTPClient):
+    res = await client.get_pages("request", Query(), 1)
+
+    assert res == [["page"]]
+    mock_get.assert_awaited_once_with("request", Query(page=1, per_page=100))
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(raises=ValueError))
+async def test_get_pages_fails(mock_get: mock.AsyncMock, client: HTTPClient):
+    with pytest.raises(ValueError):  # raised from mocked `get` method
+        await client.get_pages("request", Query(), 1)
+
+    mock_get.assert_awaited_once()
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps([empty_response()]))
+@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(empty_response()))
+async def test_query(
+    mock_get: mock.AsyncMock,
+    mock_get_pages: mock.AsyncMock,
+    client: HTTPClient,
+):
+    assert len(tuple(await client.query("request", Query()))) == 1
+
+    mock_get.assert_awaited_once_with("request", params=Query())
+    mock_get_pages.assert_awaited_once_with("request", Query(), 20)
+
+
+@pytest.mark.anyio
+@mock.patch(
+    "bavapi.http.HTTPClient.get_pages",
+    wraps=wraps([response(json=sample_data([{"a": 1}]))]),
+)
+@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(empty_response()))
+async def test_query_per_page(
+    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
+):
+    assert len(tuple(await client.query("request", Query(per_page=25)))) == 1
+
+    mock_get.assert_awaited_once()
+    mock_get_pages.assert_awaited_once_with("request", Query(per_page=25), 80)
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
+@mock.patch(
+    "bavapi.http.HTTPClient.get",
+    wraps=wraps(response(json=sample_data([{"t": 1}], total=1, on_page=1))),
+)
+async def test_query_one_page(
+    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
+):
+    # should be a list of dictionaries
+    assert list(await client.query("request", Query())) == [{"t": 1}]
+
+    mock_get.assert_awaited_once()
+    mock_get_pages.assert_not_awaited()
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
+@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(response(json=sample_data({}))))
+async def test_query_no_results(
+    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
+):
+    with pytest.raises(DataNotFoundError) as excinfo:
+        await client.query("request", Query())
+
+    mock_get.assert_awaited_once()
+    mock_get_pages.assert_not_awaited()
+    assert excinfo.value.args[0] == "Your query returned no results."
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
+@mock.patch(
+    "bavapi.http.HTTPClient.get",
+    wraps=wraps(response(json=sample_data({"t": 1}))),
+)
+async def test_query_by_id(
+    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
+):
+    assert list(await client.query("request", Query(id=1))) == [{"t": 1}]
+
+    mock_get.assert_awaited_once()
+    mock_get_pages.assert_not_awaited()
+
+
+@pytest.mark.anyio
+@mock.patch("bavapi.http.HTTPClient.get_pages", wraps=wraps())
+@mock.patch("bavapi.http.HTTPClient.get", wraps=wraps(rate_limited_response()))
+async def test_query_rate_limit(
+    mock_get: mock.AsyncMock, mock_get_pages: mock.AsyncMock, client: HTTPClient
+):
+    with pytest.raises(RateLimitExceededError) as excinfo:
+        await client.query("request", Query())
+
+    mock_get.assert_awaited_once()
+    mock_get_pages.assert_not_awaited()
+    assert excinfo.value.args[0] == (
+        "Number of pages (20) for this request "
+        "exceeds the rate limit (1, "
+        "total=500)."
+    )
```

### Comparing `wpp-bavapi-0.4.1/tests/test_jupyter.py` & `wpp-bavapi-0.5.0/tests/test_jupyter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# pylint: disable=missing-module-docstring, missing-function-docstring
-# pylint: disable=redefined-outer-name, too-few-public-methods
-
-import asyncio
-import sys
-from types import ModuleType
-from typing import Callable, Optional
-from unittest import mock
-
-import pytest
-
-from bavapi import jupyter
-
-
-class IPython(ModuleType):
-    """Mock IPython module attributes and functions"""
-
-    def __init__(self, kernel: Optional[bool] = None) -> None:
-        self.kernel = kernel
-        self.get_ipython = self._get_ipython
-        super().__init__(self.__class__.__name__)
-
-    def _get_ipython(self) -> "IPython":
-        return self
-
-
-@pytest.fixture(scope="module")
-def set_ipython():
-    def _set_ipython(kernel: Optional[bool] = None) -> None:
-        sys.modules["IPython"] = IPython(kernel)
-
-    yield _set_ipython
-
-    del sys.modules["IPython"]
-
-
-def test_running_in_jupyter(set_ipython: Callable):
-    set_ipython(True)
-
-    assert jupyter.running_in_jupyter()
-
-
-@mock.patch("bavapi.jupyter.nest_asyncio.apply")
-def test_enabled_nested(mock_apply: mock.Mock):
-    loop = asyncio.new_event_loop()
-
-    jupyter.patch_loop(loop)
-
-    mock_apply.assert_called_once_with(loop)
+# pylint: disable=missing-module-docstring, missing-function-docstring
+# pylint: disable=redefined-outer-name, too-few-public-methods
+
+import asyncio
+import sys
+from types import ModuleType
+from typing import Callable, Optional
+from unittest import mock
+
+import pytest
+
+from bavapi import jupyter
+
+
+class IPython(ModuleType):
+    """Mock IPython module attributes and functions"""
+
+    def __init__(self, kernel: Optional[bool] = None) -> None:
+        self.kernel = kernel
+        self.get_ipython = self._get_ipython
+        super().__init__(self.__class__.__name__)
+
+    def _get_ipython(self) -> "IPython":
+        return self
+
+
+@pytest.fixture(scope="module")
+def set_ipython():
+    def _set_ipython(kernel: Optional[bool] = None) -> None:
+        sys.modules["IPython"] = IPython(kernel)
+
+    yield _set_ipython
+
+    del sys.modules["IPython"]
+
+
+def test_running_in_jupyter(set_ipython: Callable):
+    set_ipython(True)
+
+    assert jupyter.running_in_jupyter()
+
+
+@mock.patch("bavapi.jupyter.nest_asyncio.apply")
+def test_enabled_nested(mock_apply: mock.Mock):
+    loop = asyncio.new_event_loop()
+
+    jupyter.patch_loop(loop)
+
+    mock_apply.assert_called_once_with(loop)
```

### Comparing `wpp-bavapi-0.4.1/tests/test_queries.py` & `wpp-bavapi-0.5.0/tests/test_queries.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring
-
-from unittest import mock
-
-import pytest
-
-from bavapi import filters
-from bavapi.query import Query
-
-
-def test_with_page():
-    assert Query(filters={"audience": 1}).with_page(2, 25) == Query(
-        page=2, per_page=25, filters={"audience": 1}
-    )
-
-
-def test_with_page_no_construction():
-    query = Query(page=2, per_page=25)
-    assert query.with_page(1, 10) is query
-
-
-def test_paginated():
-    paginated = tuple(Query(filters={"audience": 1}).paginated(100, 10))
-
-    assert len(paginated) == 10
-    assert [p.page for p in paginated] == list(range(1, 11))
-
-
-@pytest.mark.parametrize(
-    "query",
-    (
-        Query(filters={"name": 1}),
-        Query(filters=filters.FountFilters(**{"name": 1})),
-    ),
-)
-def test_to_params_filters(query: Query):
-    with mock.patch(
-        "bavapi.query.to_fount_params", return_value={}
-    ) as mock_to_fount_params:
-        query.to_params("test")
-
-    assert mock_to_fount_params.call_args_list == [
-        mock.call({"name": 1}, "filter"),
-        mock.call({}, "fields"),
-    ]
-
-
-def test_to_params_fields():
-    with mock.patch(
-        "bavapi.query.to_fount_params", return_value={}
-    ) as mock_to_fount_params:
-        Query(fields=["name"]).to_params("test")
-
-    assert mock_to_fount_params.call_args_list == [
-        mock.call({}, "filter"),
-        mock.call({"test": ["name"]}, "fields"),
-    ]
+# pylint: disable=missing-function-docstring, missing-module-docstring
+
+from unittest import mock
+
+import pytest
+
+from bavapi import filters
+from bavapi.query import Query
+
+
+def test_with_page():
+    assert Query(filters={"audience": 1}).with_page(2, 25) == Query(
+        page=2, per_page=25, filters={"audience": 1}
+    )
+
+
+def test_with_page_no_construction():
+    query = Query(page=2, per_page=25)
+    assert query.with_page(1, 10) is query
+
+
+def test_paginated():
+    paginated = tuple(Query(filters={"audience": 1}).paginated(100, 10))
+
+    assert len(paginated) == 10
+    assert [p.page for p in paginated] == list(range(1, 11))
+
+
+@pytest.mark.parametrize(
+    "query",
+    (
+        Query(filters={"name": 1}),
+        Query(filters=filters.FountFilters(**{"name": 1})),  # type: ignore[arg-type]
+    ),
+)
+def test_to_params_filters(query: Query):
+    with mock.patch(
+        "bavapi.query.to_fount_params", return_value={}
+    ) as mock_to_fount_params:
+        query.to_params("test")
+
+    assert mock_to_fount_params.call_args_list == [
+        mock.call({"name": 1}, "filter"),
+        mock.call({}, "fields"),
+    ]
+
+
+def test_to_params_fields():
+    with mock.patch(
+        "bavapi.query.to_fount_params", return_value={}
+    ) as mock_to_fount_params:
+        Query(fields=["name"]).to_params("test")
+
+    assert mock_to_fount_params.call_args_list == [
+        mock.call({}, "filter"),
+        mock.call({"test": ["name"]}, "fields"),
+    ]
```

### Comparing `wpp-bavapi-0.4.1/tests/test_sync.py` & `wpp-bavapi-0.5.0/tests/test_sync.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# pylint: disable=missing-module-docstring, missing-function-docstring
-# pylint: disable=protected-access
-
-import asyncio
-from typing import Any, TypeVar
-from unittest import mock
-
-import pytest
-
-from bavapi import sync
-from bavapi.query import Query
-
-from .helpers import wraps
-
-T = TypeVar("T")
-
-
-@mock.patch(
-    "bavapi.sync.asyncio.new_event_loop", return_value=asyncio.new_event_loop()
-)
-def test_coro_new_loop(mock_new_loop: mock.AsyncMock):
-    @sync._coro
-    async def mock_func():
-        pass
-
-    with mock.patch(
-        "bavapi.sync.asyncio.get_event_loop_policy", wraps=wraps(raises=RuntimeError)
-    ) as mock_get_loop:
-        mock_func()
-
-    mock_get_loop.assert_called_once()
-    mock_new_loop.assert_called_once()
-
-
-@mock.patch("bavapi.sync.patch_loop")
-@mock.patch("bavapi.sync.running_in_jupyter", return_value=True)
-def test_coro_jupyter(mock_running_in_jupyter: mock.Mock, mock_enabled_nested: mock.Mock):
-    @sync._coro
-    async def mock_func():
-        pass
-
-    mock_func()
-
-    mock_enabled_nested.assert_called_once()
-    mock_running_in_jupyter.assert_called_once()
-
-
-def test_raw_query():
-    with mock.patch("bavapi.sync.Client.raw_query", wraps=wraps()) as mock_raw_query:
-        sync.raw_query("TOKEN", "companies", Query())
-
-    mock_raw_query.assert_called_with("companies", Query())
-
-
-@pytest.mark.parametrize(
-    ("endpoint", "filters"),
-    (
-        ("audiences", {}),
-        ("brands", {}),
-        ("brandscape_data", {"studies": 1}),
-        ("studies", {}),
-    ),
-)
-def test_function(endpoint: str, filters: dict[str, Any]):
-    func = getattr(sync, endpoint)
-    with mock.patch(f"bavapi.sync.Client.{endpoint}", wraps=wraps()) as mock_endpoint:
-        func("TOKEN", filters=filters)
-
-    mock_endpoint.assert_called()
+# pylint: disable=missing-module-docstring, missing-function-docstring
+# pylint: disable=protected-access
+
+import asyncio
+from typing import Any, Dict, TypeVar
+from unittest import mock
+
+import pytest
+
+from bavapi import sync
+from bavapi.query import Query
+
+from .helpers import wraps
+
+T = TypeVar("T")
+
+
+@mock.patch("bavapi.sync.asyncio.new_event_loop", return_value=asyncio.new_event_loop())
+def test_coro_new_loop(mock_new_loop: mock.AsyncMock):
+    @sync._coro
+    async def mock_func():
+        pass
+
+    with mock.patch(
+        "bavapi.sync.asyncio.get_event_loop_policy", wraps=wraps(raises=RuntimeError)
+    ) as mock_get_loop:
+        mock_func()
+
+    mock_get_loop.assert_called_once()
+    mock_new_loop.assert_called_once()
+
+
+@mock.patch("bavapi.sync.patch_loop")
+@mock.patch("bavapi.sync.running_in_jupyter", return_value=True)
+def test_coro_jupyter(
+    mock_running_in_jupyter: mock.Mock, mock_enabled_nested: mock.Mock
+):
+    @sync._coro
+    async def mock_func():
+        pass
+
+    mock_func()
+
+    mock_enabled_nested.assert_called_once()
+    mock_running_in_jupyter.assert_called_once()
+
+
+def test_raw_query():
+    with mock.patch("bavapi.sync.Client.raw_query", wraps=wraps()) as mock_raw_query:
+        sync.raw_query("TOKEN", "companies", Query())
+
+    mock_raw_query.assert_called_with("companies", Query())
+
+
+@pytest.mark.parametrize(
+    ("endpoint", "filters"),
+    (
+        ("audiences", {}),
+        ("brands", {}),
+        ("brandscape_data", {"studies": 1}),
+        ("studies", {}),
+    ),
+)
+def test_function(endpoint: str, filters: Dict[str, Any]):
+    func = getattr(sync, endpoint)
+    with mock.patch(f"bavapi.sync.Client.{endpoint}", wraps=wraps()) as mock_endpoint:
+        func("TOKEN", filters=filters)
+
+    mock_endpoint.assert_called()
```

### Comparing `wpp-bavapi-0.4.1/wpp_bavapi.egg-info/PKG-INFO` & `wpp-bavapi-0.5.0/wpp_bavapi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,123 @@
-Metadata-Version: 2.1
-Name: wpp-bavapi
-Version: 0.4.1
-Summary: Python consumer for the WPPBAV Fount API.
-Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
-License: Apache 2.0
-Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database :: Database Engines/Servers
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: lint
-License-File: LICENSE
-
-# BAV API Python SDK
-
-[![CI status](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
-[![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/nachomaiz/32196acdc05431cd2bc7a8c73a587a8d/raw/covbadge.json)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
-[![docs](https://img.shields.io/badge/docs-passing-brightgreen)](https://fountapi-documentation.vercel.app/)
-[![version](https://img.shields.io/badge/version-v0.4.1-blue)](https://github.com/wppbav/bavapi-sdk-python)
-[![py-versions](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/wppbav/bavapi-sdk-python)
-
-`bavapi` is a Python SDK for the WPP BAV API.
-
-With `bavapi` you can access the full BAV data catalog, the largest and most comprehensive database of brand data in the world.
-
-Queries are validated automatically thanks to `pydantic` and retrieved asynchronously via the `httpx` package.
-
-For more information about the API, go to the [WPPBAV Developer Hub](https://developer.wppbav.com).
-
-## Prerequisites
-
-`bavapi` requires Python 3.9 or higher to run.
-
-If you don't have Python installed, you can find it from the [official](https://www.python.org/downloads/) website or via [Anaconda](https://www.anaconda.com/).
-
-You will also need a BAV API token. For more information, go to the [Authentication](https://developer.wppbav.com/docs/2.x/authentication) section of the API documentation.
-
-### Dependencies
-
-- `httpx >= 0.20`
-- `nest-asyncio >= 1.5.6`
-- `pandas >= 0.16.2`
-- `pydantic >= 1.10, < 2.0`
-- `tqdm >= 4.62`
-- `typing-extensions >= 3.10` for Python 3.9
-
-## Installation
-
-`bavapi` can be installed using `pip`.
-
-```prompt
-pip install wpp-bavapi
-```
-
-### Installing from source
-
-To install from source, clone the GitHub repository into your local machine:
-
-```prompt
-git clone https://github.com/wppbav/bavapi-sdk-python.git
-```
-
-Go into the cloned directory and install `bavapi`:
-
-```prompt
-cd bavapi-sdk-python
-pip install .
-```
-
-## Usage
-
-Once you have acquired a token, you can start using this library directly in python or in a Jupyter Notebook:
-
-```py
->>> import bavapi
->>> result = bavapi.brands("TOKEN", name="Swatch")  # Replace `"TOKEN"` with your BAV API token
->>> result
-```
-
-|     | sector_id | sector_name           |  id | name   | ... |
-| --: | --------: | --------------------- | --: | ------ | --- |
-|   0 |        11 | Apparel & Accessories | 342 | Swatch | ... |
-| ... |       ... | ...                   | ... | ...    | ... |
-
-## Features
-
-- Support for all endpoints in the Fount API. Extended support for the `audiences`, `brands`, `brandscape-data` and `studies` endpoints.
-  - Other endpoints are available via the `raw_query` functions and methods.
-- Validates query parameters are of the correct types.
-  - Provides type hints for better IDE support.
-- Retrieve multiple pages of data simultaneously.
-  - Monitors and prevents exceeding API rate limit.
-
-## Documentation
-
-Read more about `bavapi` in the [documentation](https://fountapi-documentation.vercel.app/).
-
-## Issues
-
-Please file an issue on GitHub [here](https://github.com/wppbav/bavapi-sdk-python/issues).
-
-## Contributing
-
-Please see the [Contributing](https://fountapi-documentation.vercel.app/contributing/) section of the documentation for more information.
+Metadata-Version: 2.1
+Name: wpp-bavapi
+Version: 0.5.0
+Summary: Python consumer for the WPPBAV Fount API.
+Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
+License: Apache 2.0
+Project-URL: homepage, https://github.com/wppbav/bavapi-sdk-python
+Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: test
+Provides-Extra: lint
+License-File: LICENSE
+
+# BAV API Python SDK
+
+[![CI status](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
+[![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/nachomaiz/32196acdc05431cd2bc7a8c73a587a8d/raw/covbadge.json)](https://github.com/wppbav/bavapi-sdk-python/actions/workflows/ci.yml)
+[![PyPI](https://img.shields.io/pypi/v/wpp-bavapi)](https://pypi.org/project/wpp-bavapi/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wpp-bavapi)
+](https://pypi.org/project/wpp-bavapi/)
+
+`bavapi` is a Python SDK for the WPP BAV API.
+
+It is published on [PyPI](https://pypi.org/project/wpp-bavapi/) as `wpp-bavapi`.
+
+With `bavapi` you can access the full BAV data catalog, the largest and most comprehensive database of brand data in the world.
+
+Queries are validated automatically thanks to `pydantic` and retrieved asynchronously via the `httpx` package.
+
+For more information about the API, go to the [WPPBAV Developer Hub](https://developer.wppbav.com).
+
+## Prerequisites
+
+`bavapi` requires Python 3.8 or higher to run.
+
+If you don't have Python installed, you can find it from the [official](https://www.python.org/downloads/) website or via [Anaconda](https://www.anaconda.com/).
+
+You will also need a BAV API token. For more information, go to the [Authentication](https://developer.wppbav.com/docs/2.x/authentication) section of the API documentation.
+
+### Dependencies
+
+- `httpx >= 0.20`
+- `nest-asyncio >= 1.5.6`
+- `pandas >= 0.16.2`
+- `pydantic >= 1.10, < 2.0`
+- `tqdm >= 4.62`
+- `typing-extensions >= 3.10` for Python < 3.10
+
+## Installation
+
+`bavapi` can be installed using `pip`:
+
+```prompt
+pip install wpp-bavapi
+```
+
+### Installing from source
+
+To install from source, clone the GitHub repository into your local machine:
+
+```prompt
+git clone https://github.com/wppbav/bavapi-sdk-python.git
+```
+
+Go into the cloned directory and install `bavapi`:
+
+```prompt
+cd bavapi-sdk-python
+pip install .
+```
+
+## Usage
+
+Once you have acquired a token, you can start using this library directly in python or in a Jupyter Notebook:
+
+```py
+>>> import bavapi
+>>> result = bavapi.brands("TOKEN", name="Swatch")  # Replace `"TOKEN"` with your BAV API token
+>>> result
+```
+
+|     | sector_id | sector_name           | id   | name   | ... |
+| --: | :-------- | :-------------------- | :--- | :----- | :-- |
+|   0 | 233       | Apparel & Accessories | 8635 | Swatch | ... |
+| ... | ...       | ...                   | ...  | ...    | ... |
+
+## Features
+
+- Support for all endpoints in the Fount API. Extended support for the `audiences`, `brands`, `brandscape-data` and `studies` endpoints.
+  - Other endpoints are available via the `raw_query` functions and methods.
+- Validates query parameters are of the correct types.
+  - Provides type hints for better IDE support.
+- Retrieve multiple pages of data simultaneously.
+  - Monitors and prevents exceeding API rate limit.
+- Both synchronous and asynchronous APIs for accessing BAV data.
+
+## Documentation
+
+Read more about `bavapi` in the [documentation](https://fountapi-documentation.vercel.app/).
+
+## Issues
+
+Please file an issue on GitHub [here](https://github.com/wppbav/bavapi-sdk-python/issues).
+
+## Contributing
+
+Please see the [Contributing](https://fountapi-documentation.vercel.app/contributing/) section of the documentation for more information.
```

