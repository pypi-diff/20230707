# Comparing `tmp/scitacean-23.5.0.tar.gz` & `tmp/scitacean-23.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitacean-23.5.0.tar", last modified: Mon May 15 15:28:23 2023, max compression
+gzip compressed data, was "scitacean-23.7.7.tar", last modified: Fri Jul  7 07:20:37 2023, max compression
```

## Comparing `scitacean-23.5.0.tar` & `scitacean-23.7.7.tar`

### file list

```diff
@@ -1,177 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.109059 scitacean-23.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.089058 scitacean-23.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-15 15:28:08.000000 scitacean-23.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 15:28:08.000000 scitacean-23.5.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 15:28:08.000000 scitacean-23.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-15 15:28:08.000000 scitacean-23.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-15 15:28:08.000000 scitacean-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 15:28:08.000000 scitacean-23.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-15 15:28:23.109059 scitacean-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-15 15:28:08.000000 scitacean-23.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-15 15:28:08.000000 scitacean-23.5.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/anaconda-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_templates/scitacean-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_templates/scitacean-dataclass-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/coding-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/dependency-management.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/downloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/testing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/uploading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-15 15:28:08.000000 scitacean-23.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-15 15:28:23.109059 scitacean-23.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.085058 scitacean-23.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/src/scitacean/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45630 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_dataset_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/src/scitacean/_html_repr/
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_html_repr/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/images/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_html_repr/styles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/styles/dataset.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_html_repr/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/dataset_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/files_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/metadata_repr.html.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_internal/orcid.py
--rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/datablock.py
--rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17714 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/transfer/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/transfer/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/util/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/util/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/src/scitacean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/client_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.089058 scitacean-23.5.0/tests/common/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/common/data/ssh_server_seed/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/data/ssh_server_seed/table.csv
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/data/ssh_server_seed/text.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/docker-compose-ssh-server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/ssh_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/data/datasets.json
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/data/orig_datablocks.json
--rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/dataset_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/download_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/filesystem_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/html_repr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/html_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/html_repr/html_repr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/testing/strategies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/transfer/ssh_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/upload_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/util/formatter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.089058 scitacean-23.5.0/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tools/model-generation/
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.109059 scitacean-23.5.0/tools/model-generation/spec/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/data-file.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/datablock.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/dataset-lifecycle.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/dataset.yml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/mongo-queryable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/orig-datablock.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/ownable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/technique.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.109059 scitacean-23.5.0/tools/model-generation/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/dataset.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/field_spec.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/model.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 15:28:08.000000 scitacean-23.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-07 07:20:26.000000 scitacean-23.7.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-07 07:20:26.000000 scitacean-23.7.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 07:20:26.000000 scitacean-23.7.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-07 07:20:26.000000 scitacean-23.7.7/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-07 07:20:26.000000 scitacean-23.7.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-07 07:20:26.000000 scitacean-23.7.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-07 07:20:26.000000 scitacean-23.7.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-07 07:20:26.000000 scitacean-23.7.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 07:20:26.000000 scitacean-23.7.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 07:20:26.000000 scitacean-23.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 07:20:26.000000 scitacean-23.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-07 07:20:37.889715 scitacean-23.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-07 07:20:26.000000 scitacean-23.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-07 07:20:26.000000 scitacean-23.7.7/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/_static/anaconda-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/_templates/scitacean-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/_templates/scitacean-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/developer/coding-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/developer/dependency-management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/developer/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/developer/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.873715 scitacean-23.7.7/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.877715 scitacean-23.7.7/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/user-guide/downloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/user-guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/user-guide/testing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-07 07:20:26.000000 scitacean-23.7.7/docs/user-guide/uploading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-07 07:20:26.000000 scitacean-23.7.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.877715 scitacean-23.7.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.877715 scitacean-23.7.7/requirements-pydantic2/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements-pydantic2/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 07:20:26.000000 scitacean-23.7.7/requirements-pydantic2/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-07 07:20:37.889715 scitacean-23.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.869715 scitacean-23.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44842 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_dataset_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean/_html_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean/_html_repr/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/images/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean/_html_repr/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/styles/dataset.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean/_html_repr/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/templates/dataset_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/templates/files_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_html_repr/templates/metadata_repr.html.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_internal/dataclass_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_internal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_internal/file_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_internal/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/_internal/pydantic_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26833 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/datablock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22531 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/_pytest_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.885715 scitacean-23.7.7/src/scitacean/testing/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/backend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/backend/_pytest_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/backend/docker-compose-backend-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/backend/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/backend/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.885715 scitacean-23.7.7/src/scitacean/testing/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/ssh/_pytest_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/ssh/_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/ssh/docker-compose-ssh-server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/ssh/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.885715 scitacean-23.7.7/src/scitacean/testing/ssh/ssh_server_seed/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/ssh/ssh_server_seed/table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/ssh/ssh_server_seed/text.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/testing/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.885715 scitacean-23.7.7/src/scitacean/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17714 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/transfer/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/transfer/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.885715 scitacean-23.7.7/src/scitacean/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/util/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-07 07:20:26.000000 scitacean-23.7.7/src/scitacean/util/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.881715 scitacean-23.7.7/src/scitacean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-07 07:20:37.000000 scitacean-23.7.7/src/scitacean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-07 07:20:37.000000 scitacean-23.7.7/src/scitacean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:20:37.000000 scitacean-23.7.7/src/scitacean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-07 07:20:37.000000 scitacean-23.7.7/src/scitacean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 07:20:37.000000 scitacean-23.7.7/src/scitacean.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.885715 scitacean-23.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.885715 scitacean-23.7.7/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16471 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/dataset_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/download_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/filesystem_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/tests/html_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/html_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/html_repr/html_repr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/testing/strategies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/tests/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/transfer/ssh_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/upload_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-07 07:20:26.000000 scitacean-23.7.7/tests/util/formatter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.869715 scitacean-23.7.7/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/tools/model-generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/generate_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/tools/model-generation/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/spec/dataset-fields.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/spec/field-name-overrides.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/spec/field-type-overrides.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/spec/field-validations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/spec/masked-fields.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/spec/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:37.889715 scitacean-23.7.7/tools/model-generation/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/templates/dataset_fields.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-07 07:20:26.000000 scitacean-23.7.7/tools/model-generation/templates/model.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-07 07:20:26.000000 scitacean-23.7.7/tox.ini
```

### Comparing `scitacean-23.5.0/.github/workflows/ci.yml` & `scitacean-23.7.7/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,21 @@
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e static
       - uses: stefanzweifel/git-auto-commit-action@v4
         with:
           commit_message: Apply automatic formatting
 
   tests:
-    name: Tests py${{ matrix.python }} ${{ matrix.os }}
+    name: Tests ${{ matrix.os }} ${{ matrix.tox }}
     needs: formatting
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
+          - {python: '3.11', os: ubuntu-22.04, tox: pydantic2-full}
           - {python: '3.11', os: ubuntu-22.04, tox: py311-full}
           - {python: '3.10', os: ubuntu-22.04, tox: py310-full}
           - {python: '3.9', os: ubuntu-22.04, tox: py39-full}
           - {python: '3.8', os: ubuntu-22.04, tox: py38-full}
           - {python: '3.8', os: macos-12, tox: py38}
           - {python: '3.8', os: windows-2022, tox: py38}
     steps:
```

### Comparing `scitacean-23.5.0/.github/workflows/codeql-analysis.yml` & `scitacean-23.7.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/.github/workflows/dependency-review.yml` & `scitacean-23.7.7/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/.github/workflows/docs.yml` & `scitacean-23.7.7/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     name: Build documentation
     runs-on: ubuntu-22.04
     steps:
       - run: sudo apt install --yes pandoc
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: 3.11
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e docs
       - run: touch html/.nojekyll
       - uses: actions/upload-artifact@v3
         with:
           name: documentation
           path: html/
-      - uses: JamesIves/github-pages-deploy-action@v4.4.1
+      - uses: JamesIves/github-pages-deploy-action@v4.4.2
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           single-commit: true
           ssh-key: ${{ secrets.GH_PAGES_DEPLOY_KEY }}
```

### Comparing `scitacean-23.5.0/.github/workflows/release.yml` & `scitacean-23.7.7/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     name: Deploy packages
     needs: [build_wheels]
     runs-on: ubuntu-22.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v2
-      - uses: pypa/gh-action-pypi-publish@v1.8.6
+      - uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   docs:
     needs: upload_packages
     uses: ./.github/workflows/docs.yml
```

### Comparing `scitacean-23.5.0/.pre-commit-config.yaml` & `scitacean-23.7.7/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
   hooks:
     - id: ruff
       args: ["--fix"]
 - repo: https://github.com/codespell-project/codespell
   rev: v2.2.2
   hooks:
     - id: codespell
+      additional_dependencies:
+        - tomli
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
     - id: python-use-type-annotations
     - id: rst-backticks
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
```

### Comparing `scitacean-23.5.0/CONTRIBUTING.md` & `scitacean-23.7.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/LICENSE` & `scitacean-23.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/PKG-INFO` & `scitacean-23.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 23.5.0
+Version: 23.7.7
 Summary: High-level interface for SciCat
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -47,14 +47,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ssh
+Provides-Extra: test
 License-File: LICENSE
 
 [![PyPI badge](https://img.shields.io/pypi/v/scitacean.svg?style=flat-square&color=green)](https://pypi.python.org/pypi/scitacean)
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/scitacean?style=flat-square&color=green)](https://anaconda.org/conda-forge/scitacean)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7520487.svg)](https://doi.org/10.5281/zenodo.7520487)
 [![License: BSD 3-Clause](https://img.shields.io/github/license/SciCatProject/scitacean?style=flat-square&color=yellowgreen)](LICENSE)
```

### Comparing `scitacean-23.5.0/README.md` & `scitacean-23.7.7/README.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/SECURITY.md` & `scitacean-23.7.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/_static/anaconda-logo.svg` & `scitacean-23.7.7/docs/_static/anaconda-logo.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/_static/css/custom.css` & `scitacean-23.7.7/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/_static/favicon.ico` & `scitacean-23.7.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/_static/logo-dark.svg` & `scitacean-23.7.7/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/_static/logo.svg` & `scitacean-23.7.7/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/_templates/scitacean-class-template.rst` & `scitacean-23.7.7/docs/_templates/scitacean-class-template.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/conf.py` & `scitacean-23.7.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/developer/coding-conventions.rst` & `scitacean-23.7.7/docs/developer/coding-conventions.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/developer/dependency-management.rst` & `scitacean-23.7.7/docs/developer/dependency-management.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/developer/getting-started.rst` & `scitacean-23.7.7/docs/developer/getting-started.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/developer/testing.rst` & `scitacean-23.7.7/docs/developer/testing.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/index.rst` & `scitacean-23.7.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/docs/reference/index.rst` & `scitacean-23.7.7/docs/reference/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -34,101 +34,48 @@
 ~~~~~~~~~~~~~~~~~
 
 .. autosummary::
    :toctree: ../generated/classes
    :template: scitacean-class-template.rst
    :recursive:
 
-   datablock.OrigDatablockProxy
-   dataset.DatablockModels
+   datablock.OrigDatablock
+   dataset.DatablockUploadModels
    PID
    RemotePath
    model.DatasetType
 
-Dataclasses
-~~~~~~~~~~~
-
-.. currentmodule:: scitacean._dataset_fields
-
-.. autosummary::
-   :toctree: ../generated/classes
-   :template: scitacean-dataclass-template.rst
-   :recursive:
-
-   DatasetFields
-
 Exceptions
 ~~~~~~~~~~
 
-.. currentmodule:: scitacean
-
 .. autosummary::
    :toctree: ../generated/classes
    :template: scitacean-class-template.rst
    :recursive:
 
    FileUploadError
    IntegrityError
    ScicatCommError
    ScicatLoginError
 
-Models
-~~~~~~
-
-.. currentmodule:: scitacean
-
-Pydantic models for communication with a SciCat server.
-
-.. autosummary::
-   :toctree: ../generated/classes
-
-   model.Datablock
-   model.DataFile
-   model.DatasetLifecycle
-   model.DerivedDataset
-   model.MongoQueryable
-   model.OrigDatablock
-   model.Ownable
-   model.RawDataset
-   model.Technique
-
-Typing
-~~~~~~
-
-.. currentmodule:: scitacean
-
-.. autosummary::
-   :toctree: ../generated/classes
-   :template: scitacean-class-template.rst
-   :recursive:
-
-   typing.Downloader
-   typing.DownloadConnection
-   typing.FileTransfer
-   typing.UploadConnection
-   typing.Uploader
-
-Testing
-~~~~~~~
-
-.. currentmodule:: scitacean
+Submodules
+~~~~~~~~~~
 
 .. autosummary::
-   :toctree: ../generated/classes
-   :template: scitacean-class-template.rst
+   :toctree: ../generated/modules
+   :template: scitacean-module-template.rst
    :recursive:
 
-   testing.client.FakeClient
-   testing.transfer.FakeFileTransfer
+   model
+   testing
+   typing
 
 Miscellaneous
 ~~~~~~~~~~~~~
 
-.. currentmodule:: scitacean
-
 .. autosummary::
    :toctree: ../generated/functions
    :recursive:
 
    filesystem.checksum_of_file
    filesystem.escape_path
    filesystem.file_size
```

### Comparing `scitacean-23.5.0/docs/release-notes.rst` & `scitacean-23.7.7/docs/release-notes.rst`

 * *Files 15% similar despite different names*

```diff
@@ -28,24 +28,46 @@
 
    Deprecations
    ~~~~~~~~~~~~
 
    Stability, Maintainability, and Testing
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+v23.07.07
+---------
+
+Features
+~~~~~~~~
+
+* Proper support for the new SciCat backend version 4.
+* ``scitacean.testing`` now contains tools for managing locally deployed SciCat servers and SSH servers.
+* Pydantic version 2 is not supported in addition to version 1.
+  Prior versions of Scitacean are incompatible with Pydantic version 2 and users need to ensure to install a compatible version.
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+* Models have been split into 'download' and 'upload' models for communication with SciCat as well as 'user' models that are exposed in the high level interface.
+  For users, this mostly affects tests with ``FakeClient``.
+
 v23.05.0 (2023-05-15)
 ---------------------
 
 Features
 ~~~~~~~~
 
 * Early support for the new SciCat backend version 4.
   It is possible to upload and download datasets as before.
   But the new fields added in v4 are not supported yet.
 
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+* It is no longer possible to set the dataset PID during upload.
+
 Bugfixes
 ~~~~~~~~
 
 * Fixed a bug in ``Client.download_files`` where if a file already existed on local, its local path was not set. This was introduced in v23.04.0.
 
 v23.04.0 (2023-04-05)
 ---------------------
```

### Comparing `scitacean-23.5.0/docs/user-guide/downloading.ipynb` & `scitacean-23.7.7/docs/user-guide/downloading.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954825680272109%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(26, 'Do **not** hard code secrets like tokens or passwords "*

 * *            "in notebooks or scripts!\\n'), (27, 'There is a high risk of exposing them when code "*

 * *            "is under version control or uploaded to SciCat.\\n')], delete: [27, 26]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.3'}}"}*

```diff
@@ -27,16 +27,16 @@
                 "Here, we authenticate using a token.\n",
                 "You can find your token in the web interface by logging in and opening the settings.\n",
                 "Alternatively, we could use username and password via [Client.from_credentials](../generated/classes/scitacean.Client.rst#scitacean.Client.from_credentials).\n",
                 "\n",
                 "<div class=\"alert alert-warning\">\n",
                 "    <b>WARNING:</b>\n",
                 "\n",
-                "Do *not* hard code secrets like tokens in notebooks or scripts!\n",
-                "As there is a high risk of exposing them when code is under version control or uploaded to SciCat.\n",
+                "Do **not** hard code secrets like tokens or passwords in notebooks or scripts!\n",
+                "There is a high risk of exposing them when code is under version control or uploaded to SciCat.\n",
                 "\n",
                 "Scitacean currently requires secrets to be passed as function arguments.\n",
                 "So you will have to find your own solution for now.\n",
                 "\n",
                 "</div>\n",
                 "\n",
                 "While the client itself is responsible for talking to SciCat, a `file_transfer` object is required to download data files.\n",
@@ -307,13 +307,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scitacean-23.5.0/docs/user-guide/testing.ipynb` & `scitacean-23.7.7/docs/user-guide/testing.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951972192678011%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'This is why Scitacean provides "*

 * *            '[FakeClient](../generated/modules/scitacean.testing.client.FakeClient.rst) and '*

 * *            "[FakeFileTransfer](../generated/modules/scitacean.testing.transfer.FakeFileTransfer.rst).\\n')], "*

 * *            "delete: [3]}}, 1: {'source': {insert: [(6, '    "*

 * *            'principal_investigator="Ridcully",\\n\'), (9, \'    '*

 * *            'source_folder="/upload/abcd",\\n\'), (10, \'    '*

 * *            'creation_location="Unsee […]*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "markdown",
             "id": "955a4d05-166f-4456-8dac-f81d0e40805a",
             "metadata": {},
             "source": [
                 "# Testing code with Scitacean\n",
                 "\n",
                 "Testing programs that use Scitacean can be tricky as those tests might try to access a SciCat server or fileserver.\n",
-                "This is why Scitacean provides [FakeClient](../generated/classes/scitacean.testing.client.FakeClient.rst) and [FakeFileTransfer](../generated/classes/scitacean.testing.transfer.FakeFileTransfer.rst).\n",
+                "This is why Scitacean provides [FakeClient](../generated/modules/scitacean.testing.client.FakeClient.rst) and [FakeFileTransfer](../generated/modules/scitacean.testing.transfer.FakeFileTransfer.rst).\n",
                 "Those two classes follow the same separation of concerns as the real classes.\n",
                 "That is `FakeClient` handles metadata and `FakeFileTransfer` handles files.\n",
                 "They can be mixed and matched freely with the real client and file transfers.\n",
                 "But it is generally recommended to combine them.\n",
                 "\n",
                 "First, create a test dataset and file."
             ]
@@ -26,18 +26,19 @@
             "source": [
                 "from scitacean import Dataset\n",
                 "\n",
                 "dataset = Dataset(\n",
                 "    type=\"raw\",\n",
                 "    owner_group=\"faculty\",\n",
                 "    owner=\"ridcully\",\n",
-                "    principal_investigator=\"ridcully\",\n",
+                "    principal_investigator=\"Ridcully\",\n",
                 "    contact_email=\"ridcully@uu.am\",\n",
                 "    data_format=\"spellbook-9000\",\n",
-                "    source_folder=\"/upload\",\n",
+                "    source_folder=\"/upload/abcd\",\n",
+                "    creation_location=\"UnseenUniversity\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e7ff9e70-9d75-4e15-b0ad-ccddc02741fd",
@@ -65,15 +66,15 @@
         {
             "cell_type": "markdown",
             "id": "94eace31-d349-40e6-8942-1ceea4830f0f",
             "metadata": {},
             "source": [
                 "## FakeClient\n",
                 "\n",
-                "[scitacean.testing.client.FakeClient](../generated/classes/scitacean.testing.client.FakeClient.rst) has the same interface as the regular [Client](../generated/classes/scitacean.Client.rst) but never connects to any SciCat server.\n",
+                "[scitacean.testing.client.FakeClient](../generated/modules/scitacean.testing.client.FakeClient.rst) has the same interface as the regular [Client](../generated/classes/scitacean.Client.rst) but never connects to any SciCat server.\n",
                 "Instead, it maintains an internal record of datasets and datablocks.\n",
                 "It is easiest to explain with an example.\n",
                 "First, create a `FakeClient`.\n",
                 "The url is completely arbitrary and only needs to be passed for parity with the real client."
             ]
         },
         {
@@ -84,15 +85,15 @@
             "outputs": [],
             "source": [
                 "from scitacean.testing.client import FakeClient\n",
                 "from scitacean.testing.transfer import FakeFileTransfer\n",
                 "\n",
                 "client = FakeClient.without_login(\n",
                 "    url=\"https://fake.scicat\",\n",
-                "    file_transfer=FakeFileTransfer(source_folder=\"/upload/{uid}\"))"
+                "    file_transfer=FakeFileTransfer())"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e566a6bd-e7e1-4c0b-bb80-c92bcc1b30ba",
             "metadata": {},
             "source": [
@@ -145,15 +146,15 @@
         },
         {
             "cell_type": "markdown",
             "id": "25c2ddd3-0105-4370-b57e-65ac94e67b28",
             "metadata": {},
             "source": [
                 "The client has recorded the upload from earlier.\n",
-                "However, it stored the dataset as a [model](../reference/index.rst#models), not as a regular `Dataset` object.\n",
+                "However, it stored the dataset as a [model](../generated/modules/scitacean.model.rst), not as a regular `Dataset` object.\n",
                 "In addition, since the dataset has a file, an original datablock was uploaded as well: (Datablocks store metadata and paths of files in SciCat.)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b9538f81-18d6-4441-9c09-b8dc4c8c1c71",
@@ -201,15 +202,15 @@
             "cell_type": "markdown",
             "id": "2919ab29-8d74-416d-b611-d1f1b5ba8fdb",
             "metadata": {},
             "source": [
                 "This is now an actual `Dataset` object like you would get from a real client.\n",
                 "\n",
                 "If we want to test downloads independently of uploads, we can populate `client.datasets` and `cliend.orig_datablocks` manually.\n",
-                "But keep in mind that those store *models*. See the [model reference](../reference/index.rst#models) for an overview.\n",
+                "But keep in mind that those store *models*. See the [model reference](../generated/modules/scitacean.model.rst) for an overview.\n",
                 "And also note that `orig_datablocks` stores a list of models for each dataset as there can be multiple datablocks per dataset.\n",
                 "\n",
                 "### Fidelity\n",
                 "\n",
                 "Although `FakeClient` is sufficient for many tests, it does not behave exactly the same way as a real client.\n",
                 "For example, it does not perform any validation of datasets or handle credentials.\n",
                 "In addition, it does not modify uploaded datasets like a real server would.\n",
@@ -223,15 +224,16 @@
             "cell_type": "markdown",
             "id": "da104640-ce5f-4e04-81fd-878167b8bd08",
             "metadata": {},
             "source": [
                 "## FakeFileTransfer\n",
                 "\n",
                 "`FakeClient` used above only fakes a SciCat server, i.e. handling of metadata.\n",
-                "If we also want to test file uploads and downloads, we can use [scitacean.testing.transfer.FakeFileTransfer](../generated/classes/scitacean.testing.transfer.FakeFileTransfer.rst).\n",
+                "If we also want to test file uploads and downloads, we can use [scitacean.testing.transfer.FakeFileTransfer](../generated/modules/scitacean.testing.transfer.FakeFileTransfer.rst).\n",
+                "\n",
                 "Starting from a clean slate, create a fake client with a fake file transfer as above:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7457b8a6-b067-443d-adda-88cc97af22f5",
@@ -241,15 +243,15 @@
             "outputs": [],
             "source": [
                 "from scitacean.testing.client import FakeClient\n",
                 "from scitacean.testing.transfer import FakeFileTransfer\n",
                 "\n",
                 "client = FakeClient.without_login(\n",
                 "    url=\"https://fake.scicat\",\n",
-                "    file_transfer=FakeFileTransfer(source_folder=\"/upload/{uid}\"))"
+                "    file_transfer=FakeFileTransfer())"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "15d15535-78c1-440f-b50e-626ea5457cd0",
             "metadata": {},
             "source": [
@@ -277,15 +279,17 @@
                 "We can inspect all files on the fake fileserver using:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e015c1f5-1f6b-4289-b6a5-435bcdf02512",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "client.file_transfer.files"
             ]
         },
         {
             "cell_type": "markdown",
@@ -297,37 +301,43 @@
                 "We can also download the file."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cc713b35-29d5-4a36-a51b-c3f437e8e4f7",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "downloaded = client.get_dataset(finalized.pid)\n",
                 "with_downloaded_file = client.download_files(downloaded, target=\"test-data/download\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ce5bd08a-9399-4c3b-9a92-ea5ae733e29a",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "file = list(with_downloaded_file.files)[0]\n",
                 "file"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d3135347-569b-49c2-8726-e65cdc07ac0b",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "with file.local_path.open() as f:\n",
                 "    print(f.read())"
             ]
         },
         {
@@ -367,13 +377,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scitacean-23.5.0/docs/user-guide/uploading.ipynb` & `scitacean-23.7.7/docs/user-guide/uploading.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935307395905222%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(14, \'    creation_location="lancre/whichhut",\\n\')]}}, '*

 * *            "6: {'source': {insert: [(1, 'See "*

 * *            "[scitacean.Dataset](../generated/classes/scitacean.Dataset.rst).\\n')], delete: "*

 * *            "[1]}}, 7: {'metadata': {replace: OrderedDict([('tags', [])])}}, 9: {'metadata': "*

 * *            "{replace: OrderedDict([('tags', [])])}}, 10: {'metadata': {replace: "*

 * *            "OrderedDict([('tags', [])])}}, 11: {'metadata': {replace: OrderedDict([('tags' […]*

```diff
@@ -89,40 +89,43 @@
                 "    owner_group=\"wyrdsisters\",\n",
                 "    access_groups=[\"witches\"],\n",
                 "\n",
                 "    owner=\"Nanny Ogg\",\n",
                 "    principal_investigator=\"Esme Weatherwax\",\n",
                 "    contact_email=\"nogg@wyrd.lancre\",\n",
                 "\n",
+                "    creation_location=\"lancre/whichhut\",\n",
                 "    data_format=\"space-separated\",\n",
                 "    source_folder=\"/somewhere/on/remote\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "53bfee0c-82b3-4e2f-ad4b-929ea7df6519",
             "metadata": {},
             "source": [
                 "There are many more fields that can be filled in as needed.\n",
-                "See [scitacean.Dataset](../generated/classes/scitacean.Dataset.rst) and [scitacean.DatasetFields](../generated/classes/scitacean._dataset_fields.DatasetFields.rst).\n",
+                "See [scitacean.Dataset](../generated/classes/scitacean.Dataset.rst).\n",
                 "\n",
                 "Some fields require an explanation:\n",
                 "\n",
                 "- `dataset_type` is either `raw` or `derived`. The main difference is that derived datasets point to one or more input datasets.\n",
                 "- `owner_group` and `access_groups` correspond to users/usergroups on the file server and determine who can access the files.\n",
                 "\n",
                 "Now we can attach our file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "01e303db-0e94-450a-acce-3ab48d034bb3",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "dset.add_local_files(\"data/witchcraft.dat\", base_path=\"data\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -136,45 +139,53 @@
                 "Now, let's inspect the dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "27ea91e9-5d9d-4856-b452-b20d3b3009da",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "dset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1c1c11a1-c29d-4c92-9efc-d120d5bf2582",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "len(list(dset.files))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d0763ba4-5fa4-4db8-b7ac-ed225efd3993",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "dset.size  # in bytes"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "249c1e79-40be-4e2c-bfa2-8b662604ede0",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "file = list(dset.files)[0]\n",
                 "print(f\"{file.remote_access_path(dset.source_folder) = }\")\n",
                 "print(f\"{file.local_path = }\")\n",
                 "print(f\"{file.size = } bytes\")"
             ]
@@ -196,15 +207,17 @@
                 "Once the dataset is ready, we can upload it using"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "46ac5ffe-c544-49b4-baf2-a71b3008f5af",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "finalized = client.upload_new_dataset_now(dset)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -226,15 +239,17 @@
                 "For example, it has been assigned a new ID:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e98e4339-970b-4b0b-9d3c-2dd03b9794c2",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "finalized.pid"
             ]
         },
         {
             "cell_type": "markdown",
@@ -244,15 +259,17 @@
                 "And the remote access path of our file has been set:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6c6d3650-410c-4ab6-9f56-fcd5290c8004",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "list(finalized.files)[0].remote_access_path(finalized.source_folder)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -271,15 +288,17 @@
                 "In any case, we can find out where files were uploaded by inspecting the finalized dataset that was returned by `client.upload_new_dataset_now`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "71beba39-b330-4251-bc2a-5584eb246fb2",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "finalized.source_folder"
             ]
         },
         {
             "cell_type": "markdown",
@@ -318,13 +337,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scitacean-23.5.0/pyproject.toml` & `scitacean-23.7.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -26,25 +26,26 @@
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "email-validator",
     "pydantic >= 1.9",
     "python-dateutil",
-    "requests",
+    "requests >= 2.31",
 ]
 dynamic = ["version"]
 
 [project.urls]
     "Documentation" = "https://scicatproject.github.io/scitacean"
     "Bug Tracker" = "https://github.com/SciCatProject/scitacean/issues"
     "Source" = "https://github.com/SciCatProject/scitacean"
 
 [project.optional-dependencies]
 ssh = ["fabric"]
+test = ["filelock", "hypothesis", "pyyaml"]
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 testpaths = "tests"
 addopts = """
@@ -60,14 +61,15 @@
     "ignore:Cannot check if local file:UserWarning",
     # From fabric / invoke
     "ignore:_SixMetaPathImporter:ImportWarning",
     "ignore:the imp module is deprecated in favour of importlib:DeprecationWarning",
 ]
 
 [tool.mypy]
+plugins = "pydantic.mypy"
 mypy_path = "src"
 exclude = ["venv"]
 ignore_missing_imports = true
 enable_error_code = [
     "ignore-without-code",
     "redundant-expr",
     "truthy-bool",
@@ -91,7 +93,10 @@
 "tests/*" = ["S101"]  # asserts are fine in tests
 
 [tool.ruff.isort]
 known-first-party = ["scitacean"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
+
+[tool.codespell]
+ignore-words-list = "specfield"
```

### Comparing `scitacean-23.5.0/requirements/base.txt` & `scitacean-23.7.7/requirements/base.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-# SHA1:7d04d6082ad9fa4c20034b17bf0e831ba768596f
+# SHA1:a579aa51495a128838b22e1692012f3918753a8c
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 bcrypt==4.0.1
     # via paramiko
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
-cryptography==39.0.1
+cryptography==41.0.1
     # via paramiko
+decorator==5.1.1
+    # via fabric
 dnspython==2.3.0
     # via email-validator
-email-validator==1.3.1
+email-validator==2.0.0.post2
     # via -r requirements/base.in
-fabric==3.0.0
+fabric==3.1.0
     # via -r requirements/base.in
 idna==3.4
     # via
     #   email-validator
     #   requests
-invoke==2.0.0
+invoke==2.1.3
     # via fabric
-paramiko==3.0.0
+paramiko==3.2.0
     # via fabric
 pycparser==2.21
     # via cffi
-pydantic==1.10.5
+pydantic==1.10.11
     # via -r requirements/base.in
 pynacl==1.5.0
     # via paramiko
 python-dateutil==2.8.2
     # via -r requirements/base.in
-requests==2.28.2
+requests==2.31.0
     # via -r requirements/base.in
 six==1.16.0
     # via python-dateutil
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via pydantic
-urllib3==1.26.14
+urllib3==2.0.3
     # via requests
```

### Comparing `scitacean-23.5.0/requirements/ci.txt` & `scitacean-23.7.7/requirements/ci.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # SHA1:7bdf31978c0210720b3420242d2f1d74927c098c
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.0.0
+platformdirs==3.8.0
     # via
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via tox
-pyproject-api==1.5.0
+pyproject-api==1.5.2
     # via tox
-tomli==2.0.1
-    # via
-    #   pyproject-api
-    #   tox
-tox==4.4.6
+tox==4.6.3
     # via -r requirements/ci.in
-virtualenv==20.20.0
+virtualenv==20.23.1
     # via tox
```

### Comparing `scitacean-23.5.0/requirements/dev.txt` & `scitacean-23.7.7/requirements/dev.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,125 +1,138 @@
-# SHA1:9fd2c3a421596ff11bdd6a1d27ca7e15d74c7bee
+# SHA1:31304de61247705152d0b8ea537e673329d56cc6
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
 -r ci.txt
 -r docs.txt
 -r static.txt
 -r test.txt
 -r wheels.txt
-anyio==3.6.2
+anyio==3.7.1
     # via jupyter-server
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.2.3
     # via isoduration
+black==23.3.0
+    # via -r requirements/dev.in
 click==8.1.3
     # via
+    #   black
     #   pip-compile-multi
     #   pip-tools
 fqdn==1.5.1
     # via jsonschema
 ipython-genutils==0.2.0
     # via
     #   nbclassic
     #   notebook
 isoduration==20.11.0
     # via jsonschema
-json5==0.9.11
+json5==0.9.14
     # via jupyterlab-server
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.17.3
+jsonschema[format-nongpl]==4.18.0
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.3.0
+jupyter-server==2.7.0
     # via
     #   jupyterlab
     #   jupyterlab-server
     #   nbclassic
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
 jupyterlab==3.5.3
     # via -r requirements/dev.in
-jupyterlab-server==2.19.0
+jupyterlab-server==2.23.0
     # via jupyterlab
-nbclassic==0.5.2
+mypy-extensions==1.0.0
+    # via black
+nbclassic==1.0.0
     # via
     #   jupyterlab
     #   notebook
-notebook==6.5.2
+notebook==6.5.4
     # via jupyterlab
-notebook-shim==0.2.2
+notebook-shim==0.2.3
     # via nbclassic
-pip-compile-multi==2.6.2
+overrides==7.3.1
+    # via jupyter-server
+pathspec==0.11.1
+    # via black
+pip-compile-multi==2.6.3
     # via -r requirements/dev.in
-pip-tools==6.12.3
+pip-tools==6.14.0
     # via pip-compile-multi
-prometheus-client==0.16.0
+prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 python-json-logger==2.0.7
     # via jupyter-events
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-send2trash==1.8.0
+send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 sniffio==1.3.0
     # via anyio
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
     #   nbclassic
     #   notebook
+tomli==2.0.1
+    # via jupyterlab
 toposort==1.10
     # via pip-compile-multi
-types-docutils==0.19.1.6
+types-docutils==0.20.0.1
     # via -r requirements/dev.in
-types-paramiko==3.0.0.4
+types-paramiko==3.2.0.0
     # via -r requirements/dev.in
-types-python-dateutil==2.8.19.9
+types-python-dateutil==2.8.19.13
     # via -r requirements/dev.in
-types-pyyaml==6.0.12.8
+types-pyyaml==6.0.12.10
     # via -r requirements/dev.in
-types-requests==2.28.11.15
+types-requests==2.31.0.1
     # via -r requirements/dev.in
-types-urllib3==1.26.25.8
+types-urllib3==1.26.25.13
     # via types-requests
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-webcolors==1.12
+webcolors==1.13
     # via jsonschema
-websocket-client==1.5.1
+websocket-client==1.6.1
     # via jupyter-server
-wheel==0.38.4
-    # via pip-tools
+wheel==0.40.0
+    # via
+    #   pip-tools
+    #   sphinx-copybutton
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `scitacean-23.5.0/requirements/docs.txt` & `scitacean-23.7.7/requirements/docs.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,178 +2,186 @@
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-accessible-pygments==0.0.3
+accessible-pygments==0.0.4
     # via pydata-sphinx-theme
 alabaster==0.7.13
     # via sphinx
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
-    # via jsonschema
-autodoc-pydantic==1.8.0
+attrs==23.1.0
+    # via
+    #   jsonschema
+    #   referencing
+autodoc-pydantic==1.9.0
     # via -r requirements/docs.in
 babel==2.12.1
     # via
     #   pydata-sphinx-theme
     #   sphinx
 backcall==0.2.0
     # via ipython
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.0.0
     # via nbconvert
-comm==0.1.2
+comm==0.1.3
     # via ipykernel
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
-decorator==5.1.1
-    # via ipython
 defusedxml==0.7.1
     # via nbconvert
 docutils==0.19
     # via
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx
 executing==1.2.0
     # via stack-data
-fastjsonschema==2.16.3
+fastjsonschema==2.17.1
     # via nbformat
 imagesize==1.4.1
     # via sphinx
-ipykernel==6.21.2
+ipykernel==6.24.0
     # via -r requirements/docs.in
-ipython==8.11.0
+ipython==8.14.0
     # via
     #   -r requirements/docs.in
     #   ipykernel
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.17.3
+jsonschema==4.18.0
     # via nbformat
-jupyter-client==8.0.3
+jsonschema-specifications==2023.6.1
+    # via jsonschema
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.2.0
+jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyterlab-pygments==0.2.2
     # via nbconvert
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.4
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
-myst-parser==0.19.0
+myst-parser==2.0.0
     # via -r requirements/docs.in
-nbclient==0.7.2
+nbclient==0.8.0
     # via nbconvert
-nbconvert==7.2.9
+nbconvert==7.6.0
     # via nbsphinx
-nbformat==5.7.3
+nbformat==5.9.0
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.8.12
+nbsphinx==0.9.2
     # via -r requirements/docs.in
 nest-asyncio==1.5.6
     # via ipykernel
-packaging==23.0
+packaging==23.1
     # via
     #   ipykernel
     #   nbconvert
     #   pydata-sphinx-theme
     #   sphinx
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-platformdirs==3.0.0
+platformdirs==3.8.0
     # via jupyter-core
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pydata-sphinx-theme==0.13.0
+pydata-sphinx-theme==0.13.3
     # via -r requirements/docs.in
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   accessible-pygments
     #   ipython
     #   nbconvert
     #   pydata-sphinx-theme
     #   sphinx
-pyrsistent==0.19.3
-    # via jsonschema
 pyyaml==6.0
     # via myst-parser
-pyzmq==25.0.0
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
+referencing==0.29.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+rpds-py==0.8.7
+    # via
+    #   jsonschema
+    #   referencing
 snowballstemmer==2.2.0
     # via sphinx
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==6.2.1
     # via
     #   -r requirements/docs.in
     #   autodoc-pydantic
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
     #   sphinx-copybutton
     #   sphinx-design
-sphinx-autodoc-typehints==1.22
+sphinx-autodoc-typehints==1.23.0
     # via -r requirements/docs.in
-sphinx-copybutton==0.5.1
+sphinx-copybutton==0.5.2
     # via -r requirements/docs.in
-sphinx-design==0.3.0
+sphinx-design==0.4.1
     # via -r requirements/docs.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -183,15 +191,15 @@
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 stack-data==0.6.2
     # via ipython
 tinycss2==1.2.1
     # via nbconvert
-tornado==6.2
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
```

### Comparing `scitacean-23.5.0/requirements/static.txt` & `scitacean-23.7.7/requirements/static.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 #
 #    pip-compile-multi
 #
 cfgv==3.3.1
     # via pre-commit
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.12.2
     # via virtualenv
-identify==2.5.18
+identify==2.5.24
     # via pre-commit
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-platformdirs==3.0.0
+platformdirs==3.8.0
     # via virtualenv
-pre-commit==3.1.1
+pre-commit==3.3.3
     # via -r requirements/static.in
 pyyaml==6.0
     # via pre-commit
-virtualenv==20.20.0
+virtualenv==20.23.1
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `scitacean-23.5.0/requirements/test.txt` & `scitacean-23.7.7/requirements/test.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-# SHA1:2214c6d55b321d222605254309163f46e0b6841e
+# SHA1:cefe43dc5cb9d9d7430647ec8f8955a6f1576e53
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-attrs==22.2.0
-    # via
-    #   hypothesis
-    #   pytest
-exceptiongroup==1.1.0
-    # via
-    #   hypothesis
-    #   pytest
+attrs==23.1.0
+    # via hypothesis
 execnet==1.9.0
     # via pytest-xdist
-hypothesis==6.68.2
+filelock==3.12.2
+    # via -r requirements/test.in
+hypothesis==6.80.0
     # via -r requirements/test.in
 iniconfig==2.0.0
     # via pytest
-packaging==23.0
+packaging==23.1
     # via pytest
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-pyfakefs==5.1.0
+pyfakefs==5.2.2
     # via -r requirements/test.in
-pytest==7.2.1
+pytest==7.4.0
     # via
     #   -r requirements/test.in
     #   pytest-randomly
     #   pytest-xdist
 pytest-randomly==3.12.0
     # via -r requirements/test.in
-pytest-xdist==3.2.0
+pytest-xdist==3.3.1
     # via -r requirements/test.in
 pyyaml==6.0
     # via -r requirements/test.in
 sortedcontainers==2.4.0
     # via hypothesis
-tomli==2.0.1
-    # via pytest
```

### Comparing `scitacean-23.5.0/src/scitacean/__init__.py` & `scitacean-23.7.7/src/scitacean/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 try:
     __version__ = importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:
     __version__ = "0.0.0"
 
 from .client import Client
-from .datablock import OrigDatablockProxy
+from .datablock import OrigDatablock
 from .dataset import Dataset
 from .error import FileUploadError, IntegrityError, ScicatCommError, ScicatLoginError
 from .file import File
 from .filesystem import RemotePath
 from .model import DatasetType
 from .pid import PID
 
 __all__ = (
     "Client",
     "Dataset",
     "DatasetType",
     "File",
     "FileUploadError",
     "IntegrityError",
-    "OrigDatablockProxy",
+    "OrigDatablock",
     "PID",
     "RemotePath",
     "ScicatCommError",
     "ScicatLoginError",
 )
```

### Comparing `scitacean-23.5.0/src/scitacean/_dataset_fields.py` & `scitacean-23.7.7/src/scitacean/_dataset_fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1185 +1,1074 @@
 ##########################################
 # This file was automatically generated. #
 # Do not modify it directly!             #
 ##########################################
+
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 # flake8: noqa
 
-"""Base dataclass for Dataset."""
+"""Base class for Dataset."""
 
 from __future__ import annotations
 
-import dataclasses
 from datetime import datetime, timezone
-from typing import Any, Callable, Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import dateutil.parser
 
-from .datablock import OrigDatablockProxy
+from ._internal.dataclass_wrapper import dataclass_optional_args
+from .datablock import OrigDatablock
 from .filesystem import RemotePath
 from .model import (
-    DatasetLifecycle,
     DatasetType,
-    DerivedDataset,
-    OrigDatablock,
-    RawDataset,
+    DownloadDataset,
+    Lifecycle,
+    History,
+    Relationship,
     Technique,
 )
 from .pid import PID
 
 
-def _apply_default(
-    value: Any, default: Any, default_factory: Optional[Callable[[], Any]]
-) -> Any:
-    if value is not None:
-        return value
-    if default_factory is not None:
-        return default_factory()
-    return default
+def _parse_datetime(x: Optional[Union[datetime, str]]) -> Optional[datetime]:
+    if isinstance(x, datetime) or x is None:
+        return x
+    if x == "now":
+        return datetime.now(tz=timezone.utc)
+    return dateutil.parser.parse(x)
 
 
-def _parse_datetime(x: Optional[Union[datetime, str]]) -> datetime:
-    if isinstance(x, datetime):
-        return x
-    if isinstance(x, str):
-        if x != "now":
-            return dateutil.parser.parse(x)
-    return datetime.now(tz=timezone.utc)
+def _parse_pid(pid: Optional[Union[str, PID]]) -> Optional[PID]:
+    if pid is None:
+        return pid
+    return PID.parse(pid)
+
+
+def _parse_remote_path(path: Optional[Union[str, RemotePath]]) -> Optional[RemotePath]:
+    if path is None:
+        return path
+    return RemotePath(path)
+
+
+def _validate_checksum_algorithm(algorithm: Optional[str]) -> Optional[str]:
+    if algorithm is None:
+        return algorithm
+    import hashlib
+
+    if algorithm not in hashlib.algorithms_available:
+        raise ValueError(f"Checksum algorithm not recognized: {algorithm}")
+    return algorithm
 
 
-class DatasetFields:
-    @dataclasses.dataclass(frozen=True)
+class DatasetBase:
+    @dataclass_optional_args(frozen=True, kw_only=True, slots=True)
     class Field:
         name: str
         description: str
         read_only: bool
-        required_by_derived: bool
-        required_by_raw: bool
+        required: bool
+        scicat_name: str
         type: type
         used_by_derived: bool
         used_by_raw: bool
 
-        def required(self, dataset_type: DatasetType) -> bool:
-            return (
-                self.required_by_raw
-                if dataset_type == DatasetType.RAW
-                else self.required_by_derived
-            )
-
         def used_by(self, dataset_type: DatasetType) -> bool:
             return (
                 self.used_by_raw
                 if dataset_type == DatasetType.RAW
                 else self.used_by_derived
             )
 
     _FIELD_SPEC = [
         Field(
             name="access_groups",
-            description="Groups which have read access to the data. The special group 'public' makes data available to all users.",
+            description="Optional additional groups which have read access to the data. Users which are members in one of the groups listed here are allowed to access this data. The special group 'public' makes data available to all users.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="accessGroups",
             type=List[str],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
+            name="api_version",
+            description="Version of the API used in creation of the dataset.",
+            read_only=True,
+            required=False,
+            scicat_name="version",
+            type=str,
+            used_by_derived=True,
+            used_by_raw=True,
+        ),
+        Field(
             name="classification",
-            description="ACIA information about AUthenticity,COnfidentiality,INtegrity and AVailability requirements of dataset. E.g. AV(ailabilty)=medium could trigger the creation of two tape copies. Format 'AV=medium,CO=low'",
+            description="ACIA information about AUthenticity,COnfidentiality,INtegrity and AVailability requirements of dataset. E.g. AV(ailabilty)=medium could trigger the creation of a two tape copies. Format 'AV=medium,CO=low'",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="classification",
+            type=str,
+            used_by_derived=True,
+            used_by_raw=True,
+        ),
+        Field(
+            name="comment",
+            description="Comment the user has about a given dataset.",
+            read_only=False,
+            required=False,
+            scicat_name="comment",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="contact_email",
-            description="Email of contact person for this dataset. May contain a list of emails, which should then be separated by semicolons.",
+            description="Email of the contact person for this dataset. The string may contain a list of emails, which should then be separated by semicolons.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="contactEmail",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="created_at",
-            description="Time when the object was created in the database.",
+            description="Date and time when this record was created. This property is added and maintained by mongoose.",
             read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="createdAt",
             type=datetime,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="created_by",
-            description="Account name who created the object in the database.",
+            description="Indicate the user who created this record. This property is added and maintained by the system.",
             read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="createdBy",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="creation_location",
-            description="Unique location identifier where data was taken, usually in the form /Site-name/facility-name/instrumentOrBeamline-name",
+            description="Unique location identifier where data was taken, usually in the form /Site-name/facility-name/instrumentOrBeamline-name. This field is required if the dataset is a Raw dataset.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=True,
+            scicat_name="creationLocation",
             type=str,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
             name="creation_time",
-            description="Time when dataset became fully available on disk, i.e. all containing files have been written.",
+            description="Time when dataset became fully available on disk, i.e. all containing files have been written. Format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="creationTime",
             type=datetime,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="data_format",
-            description="Defines format of subsequent scientific meta data, e.g Nexus Version x.y",
+            description="Defines the format of the data files in this dataset, e.g Nexus Version x.y.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="dataFormat",
             type=str,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
+            name="data_quality_metrics",
+            description="Data Quality Metrics given by the user to rate the dataset.",
+            read_only=False,
+            required=False,
+            scicat_name="dataQualityMetrics",
+            type=int,
+            used_by_derived=True,
+            used_by_raw=True,
+        ),
+        Field(
             name="description",
-            description="Free text explanation of the contents of the dataset.",
+            description="Free text explanation of contents of dataset.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="description",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="end_time",
-            description="Time of end of data taking for this dataset.",
+            description="End time of data acquisition for this dataset, format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="endTime",
             type=datetime,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
             name="history",
-            description="List of previous versions of the dataset. Populated automatically by SciCat.",
+            description="List of objects containing old and new values.",
             read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=List[dict],
+            required=False,
+            scicat_name="history",
+            type=None,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="input_datasets",
-            description="Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs.",
+            description="Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs. This field is required if the dataset is a Derived dataset.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="inputDatasets",
             type=List[PID],
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="instrument_group",
-            description="Groups which have read and write access to the data.",
+            description="Optional additional groups which have read and write access to the data. Users which are members in one of the groups listed here are allowed to access this data.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="instrumentGroup",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="instrument_id",
-            description="SciCat ID of the instrument used to measure the data.",
+            description="ID of the instrument where the data was created.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="instrumentId",
             type=str,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
             name="investigator",
-            description="Name(s) of the investigator(s). The string may contain a list of names, which should then be separated by semicolons.",
+            description="First name and last name of the person or people pursuing the data analysis. The string may contain a list of names, which should then be separated by semicolons.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="investigator",
             type=str,
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="is_published",
-            description="Indicate whether the dataset is publicly available.",
+            description="Flag is true when data are made publicly available.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="isPublished",
             type=bool,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="job_log_data",
             description="The output job logfile. Keep the size of this log data well below 15 MB.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="jobLogData",
             type=str,
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="job_parameters",
-            description="Input parameters to the job that produced the derived data.",
+            description="The creation process of the derived data will usually depend on input job parameters. The full structure of these input parameters are stored here.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=dict,
+            required=False,
+            scicat_name="jobParameters",
+            type=Dict[str, Any],
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="keywords",
             description="Array of tags associated with the meaning or contents of this dataset. Values should ideally come from defined vocabularies, taxonomies, ontologies or knowledge graphs.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="keywords",
             type=List[str],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="license",
-            description="Name of license under which data can be used.",
+            description="Name of the license under which the data can be used.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="license",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="lifecycle",
-            description="Parameters for storage and publishing of dataset.",
-            read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=DatasetLifecycle,
-            used_by_derived=True,
-            used_by_raw=True,
-        ),
-        Field(
-            name="meta",
-            description="Free form meta data.",
-            read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=Dict,
+            description="Describes the current status of the dataset during its lifetime with respect to the storage handling systems.",
+            read_only=True,
+            required=False,
+            scicat_name="datasetlifecycle",
+            type=Lifecycle,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="name",
-            description="A name for the dataset.",
+            description="A name for the dataset, given by the creator to carry some semantic meaning. Useful for display purposes e.g. instead of displaying the pid. Will be autofilled if missing using info from sourceFolder.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="datasetName",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
-            name="number_of_files",
-            description="Total number of files in directly accessible storage associated with the dataset. (Corresponds to OrigDatablocks.)",
-            read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=int,
-            used_by_derived=True,
-            used_by_raw=True,
-        ),
-        Field(
-            name="number_of_files_archived",
-            description="Total number of archived files associated with the dataset. (Corresponds to Datablocks.)",
-            read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=int,
-            used_by_derived=True,
-            used_by_raw=True,
-        ),
-        Field(
             name="orcid_of_owner",
-            description="ORCID of owner/custodian. The string may contain a list of ORCID, which should then be separated by semicolons. ORCIDs must include the prefix https://orcid.org/",
+            description="ORCID of the owner or custodian. The string may contain a list of ORCIDs, which should then be separated by semicolons.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="orcidOfOwner",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="owner",
-            description="Owner or custodian of the dataset, usually first name + lastname. The string may contain a list of persons, which should then be separated by semicolons.",
+            description="Owner or custodian of the dataset, usually first name + last name. The string may contain a list of persons, which should then be separated by semicolons.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="owner",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="owner_email",
-            description="Email of owner or of custodian of the dataset. The string may contain a list of emails, which should then be separated by semicolons.",
+            description="Email of the owner or custodian of the dataset. The string may contain a list of emails, which should then be separated by semicolons.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="ownerEmail",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="owner_group",
-            description="Defines the group which owns the data, and therefore has unrestricted access to this data. Usually a pgroup like p12151.",
+            description="Defines the group which owns the data, and therefore has unrestricted access to this data. Usually a pgroup like p12151",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="ownerGroup",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
-            name="packed_size",
-            description="Total size of all datablock package files created for this dataset.",
-            read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=int,
-            used_by_derived=True,
-            used_by_raw=True,
-        ),
-        Field(
             name="pid",
-            description="Persistent identifier for datasets.",
-            read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            description="Persistent Identifier for datasets derived from UUIDv4 and prepended automatically by site specific PID prefix like 20.500.12345/",
+            read_only=True,
+            required=False,
+            scicat_name="pid",
             type=PID,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="principal_investigator",
-            description="Name(s) of the principal investigator(s). The string may contain a list of names, which should then be separated by semicolons.",
+            description="First name and last name of principal investigator(s). If multiple PIs are present, use a semicolon separated list. This field is required if the dataset is a Raw dataset.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="principalInvestigator",
             type=str,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
             name="proposal_id",
-            description="Identifier for the proposal that the dataset was produced for.",
+            description="The ID of the proposal to which the dataset belongs.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="proposalId",
             type=str,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
+            name="relationships",
+            description="Stores the relationships with other datasets.",
+            read_only=False,
+            required=False,
+            scicat_name="relationships",
+            type=List[Relationship],
+            used_by_derived=True,
+            used_by_raw=True,
+        ),
+        Field(
             name="sample_id",
-            description="Identifier for the sample that the dataset contains a measurement of.",
+            description="ID of the sample used when collecting the data.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="sampleId",
             type=str,
             used_by_derived=False,
             used_by_raw=True,
         ),
         Field(
             name="shared_with",
             description="List of users that the dataset has been shared with.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="sharedWith",
             type=List[str],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
-            name="size",
-            description="Total size of all files contained in source folder on disk when unpacked.",
-            read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=int,
-            used_by_derived=True,
-            used_by_raw=True,
-        ),
-        Field(
             name="source_folder",
-            description="Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename.",
+            description="Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename. Trailing slashes are removed.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="sourceFolder",
             type=RemotePath,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="source_folder_host",
-            description="DNS host name of file server hosting source_folder, optionally including protocol e.g. [protocol://]fileserver1.example.com",
+            description="DNS host name of file server hosting sourceFolder, optionally including a protocol e.g. [protocol://]fileserver1.example.com",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="sourceFolderHost",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="techniques",
-            description="List of techniques used to produce the data.",
+            description="Stores the metadata information for techniques.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="techniques",
             type=List[Technique],
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="type",
-            description="Dataset type. 'Derived' or 'Raw'",
+            description="Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="type",
             type=DatasetType,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="updated_at",
-            description="Time when the object was last updated in the database.",
+            description="Date and time when this record was updated last. This property is added and maintained by mongoose.",
             read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="updatedAt",
             type=datetime,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="updated_by",
-            description="Account name who last updated the object in the database.",
+            description="Indicate the user who updated this record last. This property is added and maintained by the system.",
             read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="updatedBy",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
         Field(
             name="used_software",
-            description="A list of links to software repositories which uniquely identifies the software used and the version for producing the derived data.",
+            description="A list of links to software repositories which uniquely identifies the pieces of software, including versions, used for yielding the derived data. This field is required if the dataset is a Derived dataset.",
             read_only=False,
-            required_by_derived=True,
-            required_by_raw=True,
+            required=True,
+            scicat_name="usedSoftware",
             type=List[str],
             used_by_derived=True,
             used_by_raw=False,
         ),
         Field(
             name="validation_status",
             description="Defines a level of trust, e.g. a measure of how much data was verified or used by other persons.",
             read_only=False,
-            required_by_derived=False,
-            required_by_raw=False,
-            type=str,
-            used_by_derived=True,
-            used_by_raw=True,
-        ),
-        Field(
-            name="version",
-            description="Version of SciCat API used in creation of dataset.",
-            read_only=True,
-            required_by_derived=False,
-            required_by_raw=False,
+            required=False,
+            scicat_name="validationStatus",
             type=str,
             used_by_derived=True,
             used_by_raw=True,
         ),
     ]
 
+    __slots__ = (
+        "_access_groups",
+        "_api_version",
+        "_classification",
+        "_comment",
+        "_contact_email",
+        "_created_at",
+        "_created_by",
+        "_creation_location",
+        "_creation_time",
+        "_data_format",
+        "_data_quality_metrics",
+        "_description",
+        "_end_time",
+        "_history",
+        "_input_datasets",
+        "_instrument_group",
+        "_instrument_id",
+        "_investigator",
+        "_is_published",
+        "_job_log_data",
+        "_job_parameters",
+        "_keywords",
+        "_license",
+        "_lifecycle",
+        "_name",
+        "_orcid_of_owner",
+        "_owner",
+        "_owner_email",
+        "_owner_group",
+        "_pid",
+        "_principal_investigator",
+        "_proposal_id",
+        "_relationships",
+        "_sample_id",
+        "_shared_with",
+        "_source_folder",
+        "_source_folder_host",
+        "_techniques",
+        "_type",
+        "_updated_at",
+        "_updated_by",
+        "_used_software",
+        "_validation_status",
+        "_meta",
+        "_default_checksum_algorithm",
+        "_orig_datablocks",
+    )
+
     def __init__(
         self,
-        *,
-        type: Union[DatasetType, Literal["derived", "raw"]],
-        creation_time: Optional[Union[datetime, str]] = None,
-        pid: Optional[Union[str, PID]] = None,
+        type: Union[DatasetType, Literal["raw", "derived"]],
         access_groups: Optional[List[str]] = None,
         classification: Optional[str] = None,
+        comment: Optional[str] = None,
         contact_email: Optional[str] = None,
         creation_location: Optional[str] = None,
+        creation_time: Optional[Union[str, datetime]] = "now",
         data_format: Optional[str] = None,
+        data_quality_metrics: Optional[int] = None,
         description: Optional[str] = None,
         end_time: Optional[datetime] = None,
         input_datasets: Optional[List[PID]] = None,
         instrument_group: Optional[str] = None,
         instrument_id: Optional[str] = None,
         investigator: Optional[str] = None,
         is_published: Optional[bool] = None,
         job_log_data: Optional[str] = None,
-        job_parameters: Optional[dict] = None,
+        job_parameters: Optional[Dict[str, Any]] = None,
         keywords: Optional[List[str]] = None,
         license: Optional[str] = None,
-        lifecycle: Optional[DatasetLifecycle] = None,
-        meta: Optional[Dict] = None,
         name: Optional[str] = None,
         orcid_of_owner: Optional[str] = None,
         owner: Optional[str] = None,
         owner_email: Optional[str] = None,
         owner_group: Optional[str] = None,
         principal_investigator: Optional[str] = None,
         proposal_id: Optional[str] = None,
+        relationships: Optional[List[Relationship]] = None,
         sample_id: Optional[str] = None,
         shared_with: Optional[List[str]] = None,
-        source_folder: Optional[RemotePath] = None,
+        source_folder: Optional[Union[RemotePath, str]] = None,
         source_folder_host: Optional[str] = None,
         techniques: Optional[List[Technique]] = None,
         used_software: Optional[List[str]] = None,
         validation_status: Optional[str] = None,
+        meta: Optional[Dict[str, Any]] = None,
         checksum_algorithm: Optional[str] = "blake2b",
-        _read_only: Optional[Dict[str, Any]] = None,
-        _orig_datablocks: Optional[List[OrigDatablockProxy]] = None,
-    ):
-        """Construct a dataset with given values.
-
-        All arguments correspond to dataset fields, except `checksum_algorithm` which
-        is used as the default algorithm when files are added.
-
-        Arguments starting with an underscore are used internally to initialize
-        datasets from SciCat models, and you should generally avoid setting them
-        yourself!
-        """
-        _read_only = _read_only or {}
-        self._fields = {
-            "creation_time": _parse_datetime(creation_time),
-            "history": _apply_default(_read_only.get("history"), None, None),
-            "pid": PID.parse(pid) if isinstance(pid, str) else pid,
-            "type": DatasetType(type),
-            "access_groups": _apply_default(access_groups, None, None),
-            "classification": _apply_default(classification, None, None),
-            "contact_email": _apply_default(contact_email, None, None),
-            "created_at": _apply_default(_read_only.get("created_at"), None, None),
-            "created_by": _apply_default(_read_only.get("created_by"), None, None),
-            "creation_location": _apply_default(creation_location, None, None),
-            "data_format": _apply_default(data_format, None, None),
-            "description": _apply_default(description, None, None),
-            "end_time": _apply_default(end_time, None, None),
-            "input_datasets": _apply_default(input_datasets, None, None),
-            "instrument_group": _apply_default(instrument_group, None, None),
-            "instrument_id": _apply_default(instrument_id, None, None),
-            "investigator": _apply_default(investigator, None, None),
-            "is_published": _apply_default(is_published, False, None),
-            "job_log_data": _apply_default(job_log_data, None, None),
-            "job_parameters": _apply_default(job_parameters, None, None),
-            "keywords": _apply_default(keywords, None, None),
-            "license": _apply_default(license, None, None),
-            "lifecycle": _apply_default(lifecycle, None, None),
-            "meta": _apply_default(meta, None, dict),
-            "name": _apply_default(name, None, None),
-            "orcid_of_owner": _apply_default(orcid_of_owner, None, None),
-            "owner": _apply_default(owner, None, None),
-            "owner_email": _apply_default(owner_email, None, None),
-            "owner_group": _apply_default(owner_group, None, None),
-            "principal_investigator": _apply_default(
-                principal_investigator, None, None
-            ),
-            "proposal_id": _apply_default(proposal_id, None, None),
-            "sample_id": _apply_default(sample_id, None, None),
-            "shared_with": _apply_default(shared_with, None, None),
-            "source_folder": _apply_default(source_folder, None, None),
-            "source_folder_host": _apply_default(source_folder_host, None, None),
-            "techniques": _apply_default(techniques, None, None),
-            "updated_at": _apply_default(_read_only.get("updated_at"), None, None),
-            "updated_by": _apply_default(_read_only.get("updated_by"), None, None),
-            "used_software": _apply_default(used_software, None, None),
-            "validation_status": _apply_default(validation_status, None, None),
-            "version": _apply_default(_read_only.get("version"), None, None),
-        }
-        self._orig_datablocks = (
-            [] if _orig_datablocks is None else list(_orig_datablocks)
-        )
-        self._default_checksum_algorithm = self._validate_checksum_algorithm(
+    ) -> None:
+        self._type = DatasetType(type)
+        self._access_groups = access_groups
+        self._classification = classification
+        self._comment = comment
+        self._contact_email = contact_email
+        self._creation_location = creation_location
+        self._creation_time = _parse_datetime(creation_time)
+        self._data_format = data_format
+        self._data_quality_metrics = data_quality_metrics
+        self._description = description
+        self._end_time = end_time
+        self._input_datasets = input_datasets
+        self._instrument_group = instrument_group
+        self._instrument_id = instrument_id
+        self._investigator = investigator
+        self._is_published = is_published
+        self._job_log_data = job_log_data
+        self._job_parameters = job_parameters
+        self._keywords = keywords
+        self._license = license
+        self._name = name
+        self._orcid_of_owner = orcid_of_owner
+        self._owner = owner
+        self._owner_email = owner_email
+        self._owner_group = owner_group
+        self._principal_investigator = principal_investigator
+        self._proposal_id = proposal_id
+        self._relationships = relationships
+        self._sample_id = sample_id
+        self._shared_with = shared_with
+        self._source_folder = _parse_remote_path(source_folder)
+        self._source_folder_host = source_folder_host
+        self._techniques = techniques
+        self._used_software = used_software
+        self._validation_status = validation_status
+        self._api_version = None
+        self._created_at = None
+        self._created_by = None
+        self._history = None
+        self._lifecycle = None
+        self._pid = None
+        self._updated_at = None
+        self._updated_by = None
+        self._meta = meta or {}
+        self._default_checksum_algorithm = _validate_checksum_algorithm(
             checksum_algorithm
         )
-
-    @staticmethod
-    def _validate_checksum_algorithm(algorithm: Optional[str]) -> Optional[str]:
-        if algorithm is None:
-            return algorithm
-        import hashlib
-
-        if algorithm not in hashlib.algorithms_available:
-            raise ValueError(f"Checksum algorithm not recognized: {algorithm}")
-        return algorithm
-
-    @property
-    def type(self) -> DatasetType:
-        """Dataset type, Derived or Raw."""
-        return self._fields["type"]  # type: ignore[no-any-return]
-
-    @type.setter
-    def type(self, val: DatasetType) -> None:
-        """Dataset type, Derived or Raw."""
-        self._fields["type"] = val
-
-    @property
-    def pid(self) -> Optional[PID]:
-        """Persistent identifier for datasets."""
-        return self._fields["pid"]  # type: ignore[no-any-return]
-
-    @pid.setter
-    def pid(self, pid: Optional[Union[PID, str]]) -> None:
-        """Persistent identifier for datasets."""
-        self._fields["pid"] = None if pid is None else PID.parse(pid)
-
-    @property
-    def creation_time(self) -> datetime:
-        """Time when the dataset became fully available on disk,
-        i.e. all containing files have been written."""
-        return self._fields["creation_time"]  # type: ignore[no-any-return]
-
-    @creation_time.setter
-    def creation_time(self, value: Union[datetime, str]) -> None:
-        """Time when the dataset became fully available on disk,
-        i.e. all containing files have been written."""
-        if value is None:
-            raise TypeError("Cannot set creation_time to None")
-        self._fields["creation_time"] = _parse_datetime(value)
+        self._orig_datablocks: List[OrigDatablock] = []
 
     @property
     def access_groups(self) -> Optional[List[str]]:
-        """Groups which have read access to the data. The special group 'public' makes data available to all users."""
-        return self._fields["access_groups"]  # type: ignore[no-any-return]
+        """Optional additional groups which have read access to the data. Users which are members in one of the groups listed here are allowed to access this data. The special group 'public' makes data available to all users."""
+        return self._access_groups
 
     @access_groups.setter
-    def access_groups(self, val: Optional[List[str]]) -> None:
-        self._fields["access_groups"] = val
+    def access_groups(self, access_groups: Optional[List[str]]) -> None:
+        """Optional additional groups which have read access to the data. Users which are members in one of the groups listed here are allowed to access this data. The special group 'public' makes data available to all users."""
+        self._access_groups = access_groups
+
+    @property
+    def api_version(self) -> Optional[str]:
+        """Version of the API used in creation of the dataset."""
+        return self._api_version
 
     @property
     def classification(self) -> Optional[str]:
-        """ACIA information about AUthenticity,COnfidentiality,INtegrity and AVailability requirements of dataset. E.g. AV(ailabilty)=medium could trigger the creation of two tape copies. Format 'AV=medium,CO=low'"""
-        return self._fields["classification"]  # type: ignore[no-any-return]
+        """ACIA information about AUthenticity,COnfidentiality,INtegrity and AVailability requirements of dataset. E.g. AV(ailabilty)=medium could trigger the creation of a two tape copies. Format 'AV=medium,CO=low'"""
+        return self._classification
 
     @classification.setter
-    def classification(self, val: Optional[str]) -> None:
-        self._fields["classification"] = val
+    def classification(self, classification: Optional[str]) -> None:
+        """ACIA information about AUthenticity,COnfidentiality,INtegrity and AVailability requirements of dataset. E.g. AV(ailabilty)=medium could trigger the creation of a two tape copies. Format 'AV=medium,CO=low'"""
+        self._classification = classification
+
+    @property
+    def comment(self) -> Optional[str]:
+        """Comment the user has about a given dataset."""
+        return self._comment
+
+    @comment.setter
+    def comment(self, comment: Optional[str]) -> None:
+        """Comment the user has about a given dataset."""
+        self._comment = comment
 
     @property
     def contact_email(self) -> Optional[str]:
-        """Email of contact person for this dataset. May contain a list of emails, which should then be separated by semicolons."""
-        return self._fields["contact_email"]  # type: ignore[no-any-return]
+        """Email of the contact person for this dataset. The string may contain a list of emails, which should then be separated by semicolons."""
+        return self._contact_email
 
     @contact_email.setter
-    def contact_email(self, val: Optional[str]) -> None:
-        self._fields["contact_email"] = val
+    def contact_email(self, contact_email: Optional[str]) -> None:
+        """Email of the contact person for this dataset. The string may contain a list of emails, which should then be separated by semicolons."""
+        self._contact_email = contact_email
 
     @property
     def created_at(self) -> Optional[datetime]:
-        """Time when the object was created in the database."""
-        return self._fields["created_at"]  # type: ignore[no-any-return]
+        """Date and time when this record was created. This property is added and maintained by mongoose."""
+        return self._created_at
 
     @property
     def created_by(self) -> Optional[str]:
-        """Account name who created the object in the database."""
-        return self._fields["created_by"]  # type: ignore[no-any-return]
+        """Indicate the user who created this record. This property is added and maintained by the system."""
+        return self._created_by
 
     @property
     def creation_location(self) -> Optional[str]:
-        """Unique location identifier where data was taken, usually in the form /Site-name/facility-name/instrumentOrBeamline-name"""
-        return self._fields["creation_location"]  # type: ignore[no-any-return]
+        """Unique location identifier where data was taken, usually in the form /Site-name/facility-name/instrumentOrBeamline-name. This field is required if the dataset is a Raw dataset."""
+        return self._creation_location
 
     @creation_location.setter
-    def creation_location(self, val: Optional[str]) -> None:
-        self._fields["creation_location"] = val
+    def creation_location(self, creation_location: Optional[str]) -> None:
+        """Unique location identifier where data was taken, usually in the form /Site-name/facility-name/instrumentOrBeamline-name. This field is required if the dataset is a Raw dataset."""
+        self._creation_location = creation_location
+
+    @property
+    def creation_time(self) -> Optional[datetime]:
+        """Time when dataset became fully available on disk, i.e. all containing files have been written. Format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
+        return self._creation_time
+
+    @creation_time.setter
+    def creation_time(self, creation_time: Optional[Union[str, datetime]]) -> None:
+        """Time when dataset became fully available on disk, i.e. all containing files have been written. Format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
+        self._creation_time = _parse_datetime(creation_time)
 
     @property
     def data_format(self) -> Optional[str]:
-        """Defines format of subsequent scientific meta data, e.g Nexus Version x.y"""
-        return self._fields["data_format"]  # type: ignore[no-any-return]
+        """Defines the format of the data files in this dataset, e.g Nexus Version x.y."""
+        return self._data_format
 
     @data_format.setter
-    def data_format(self, val: Optional[str]) -> None:
-        self._fields["data_format"] = val
+    def data_format(self, data_format: Optional[str]) -> None:
+        """Defines the format of the data files in this dataset, e.g Nexus Version x.y."""
+        self._data_format = data_format
+
+    @property
+    def data_quality_metrics(self) -> Optional[int]:
+        """Data Quality Metrics given by the user to rate the dataset."""
+        return self._data_quality_metrics
+
+    @data_quality_metrics.setter
+    def data_quality_metrics(self, data_quality_metrics: Optional[int]) -> None:
+        """Data Quality Metrics given by the user to rate the dataset."""
+        self._data_quality_metrics = data_quality_metrics
 
     @property
     def description(self) -> Optional[str]:
-        """Free text explanation of the contents of the dataset."""
-        return self._fields["description"]  # type: ignore[no-any-return]
+        """Free text explanation of contents of dataset."""
+        return self._description
 
     @description.setter
-    def description(self, val: Optional[str]) -> None:
-        self._fields["description"] = val
+    def description(self, description: Optional[str]) -> None:
+        """Free text explanation of contents of dataset."""
+        self._description = description
 
     @property
     def end_time(self) -> Optional[datetime]:
-        """Time of end of data taking for this dataset."""
-        return self._fields["end_time"]  # type: ignore[no-any-return]
+        """End time of data acquisition for this dataset, format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
+        return self._end_time
 
     @end_time.setter
-    def end_time(self, val: Optional[datetime]) -> None:
-        self._fields["end_time"] = val
+    def end_time(self, end_time: Optional[datetime]) -> None:
+        """End time of data acquisition for this dataset, format according to chapter 5.6 internet date/time format in RFC 3339. Local times without timezone/offset info are automatically transformed to UTC using the timezone of the API server."""
+        self._end_time = end_time
+
+    @property
+    def history(self) -> Optional[None]:
+        """List of objects containing old and new values."""
+        return self._history
 
     @property
     def input_datasets(self) -> Optional[List[PID]]:
-        """Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs."""
-        return self._fields["input_datasets"]  # type: ignore[no-any-return]
+        """Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs. This field is required if the dataset is a Derived dataset."""
+        return self._input_datasets
 
     @input_datasets.setter
-    def input_datasets(self, val: Optional[List[PID]]) -> None:
-        self._fields["input_datasets"] = val
+    def input_datasets(self, input_datasets: Optional[List[PID]]) -> None:
+        """Array of input dataset identifiers used in producing the derived dataset. Ideally these are the global identifier to existing datasets inside this or federated data catalogs. This field is required if the dataset is a Derived dataset."""
+        self._input_datasets = input_datasets
 
     @property
     def instrument_group(self) -> Optional[str]:
-        """Groups which have read and write access to the data."""
-        return self._fields["instrument_group"]  # type: ignore[no-any-return]
+        """Optional additional groups which have read and write access to the data. Users which are members in one of the groups listed here are allowed to access this data."""
+        return self._instrument_group
 
     @instrument_group.setter
-    def instrument_group(self, val: Optional[str]) -> None:
-        self._fields["instrument_group"] = val
+    def instrument_group(self, instrument_group: Optional[str]) -> None:
+        """Optional additional groups which have read and write access to the data. Users which are members in one of the groups listed here are allowed to access this data."""
+        self._instrument_group = instrument_group
 
     @property
     def instrument_id(self) -> Optional[str]:
-        """SciCat ID of the instrument used to measure the data."""
-        return self._fields["instrument_id"]  # type: ignore[no-any-return]
+        """ID of the instrument where the data was created."""
+        return self._instrument_id
 
     @instrument_id.setter
-    def instrument_id(self, val: Optional[str]) -> None:
-        self._fields["instrument_id"] = val
+    def instrument_id(self, instrument_id: Optional[str]) -> None:
+        """ID of the instrument where the data was created."""
+        self._instrument_id = instrument_id
 
     @property
     def investigator(self) -> Optional[str]:
-        """Name(s) of the investigator(s). The string may contain a list of names, which should then be separated by semicolons."""
-        return self._fields["investigator"]  # type: ignore[no-any-return]
+        """First name and last name of the person or people pursuing the data analysis. The string may contain a list of names, which should then be separated by semicolons."""
+        return self._investigator
 
     @investigator.setter
-    def investigator(self, val: Optional[str]) -> None:
-        self._fields["investigator"] = val
+    def investigator(self, investigator: Optional[str]) -> None:
+        """First name and last name of the person or people pursuing the data analysis. The string may contain a list of names, which should then be separated by semicolons."""
+        self._investigator = investigator
 
     @property
     def is_published(self) -> Optional[bool]:
-        """Indicate whether the dataset is publicly available."""
-        return self._fields["is_published"]  # type: ignore[no-any-return]
+        """Flag is true when data are made publicly available."""
+        return self._is_published
 
     @is_published.setter
-    def is_published(self, val: Optional[bool]) -> None:
-        self._fields["is_published"] = val
+    def is_published(self, is_published: Optional[bool]) -> None:
+        """Flag is true when data are made publicly available."""
+        self._is_published = is_published
 
     @property
     def job_log_data(self) -> Optional[str]:
         """The output job logfile. Keep the size of this log data well below 15 MB."""
-        return self._fields["job_log_data"]  # type: ignore[no-any-return]
+        return self._job_log_data
 
     @job_log_data.setter
-    def job_log_data(self, val: Optional[str]) -> None:
-        self._fields["job_log_data"] = val
+    def job_log_data(self, job_log_data: Optional[str]) -> None:
+        """The output job logfile. Keep the size of this log data well below 15 MB."""
+        self._job_log_data = job_log_data
 
     @property
-    def job_parameters(self) -> Optional[dict]:
-        """Input parameters to the job that produced the derived data."""
-        return self._fields["job_parameters"]  # type: ignore[no-any-return]
+    def job_parameters(self) -> Optional[Dict[str, Any]]:
+        """The creation process of the derived data will usually depend on input job parameters. The full structure of these input parameters are stored here."""
+        return self._job_parameters
 
     @job_parameters.setter
-    def job_parameters(self, val: Optional[dict]) -> None:
-        self._fields["job_parameters"] = val
+    def job_parameters(self, job_parameters: Optional[Dict[str, Any]]) -> None:
+        """The creation process of the derived data will usually depend on input job parameters. The full structure of these input parameters are stored here."""
+        self._job_parameters = job_parameters
 
     @property
     def keywords(self) -> Optional[List[str]]:
         """Array of tags associated with the meaning or contents of this dataset. Values should ideally come from defined vocabularies, taxonomies, ontologies or knowledge graphs."""
-        return self._fields["keywords"]  # type: ignore[no-any-return]
+        return self._keywords
 
     @keywords.setter
-    def keywords(self, val: Optional[List[str]]) -> None:
-        self._fields["keywords"] = val
+    def keywords(self, keywords: Optional[List[str]]) -> None:
+        """Array of tags associated with the meaning or contents of this dataset. Values should ideally come from defined vocabularies, taxonomies, ontologies or knowledge graphs."""
+        self._keywords = keywords
 
     @property
     def license(self) -> Optional[str]:
-        """Name of license under which data can be used."""
-        return self._fields["license"]  # type: ignore[no-any-return]
+        """Name of the license under which the data can be used."""
+        return self._license
 
     @license.setter
-    def license(self, val: Optional[str]) -> None:
-        self._fields["license"] = val
+    def license(self, license: Optional[str]) -> None:
+        """Name of the license under which the data can be used."""
+        self._license = license
 
     @property
-    def lifecycle(self) -> Optional[DatasetLifecycle]:
-        """Parameters for storage and publishing of dataset."""
-        return self._fields["lifecycle"]  # type: ignore[no-any-return]
-
-    @lifecycle.setter
-    def lifecycle(self, val: Optional[DatasetLifecycle]) -> None:
-        self._fields["lifecycle"] = val
-
-    @property
-    def meta(self) -> Optional[Dict]:
-        """Free form meta data."""
-        return self._fields["meta"]  # type: ignore[no-any-return]
-
-    @meta.setter
-    def meta(self, val: Optional[Dict]) -> None:
-        self._fields["meta"] = val
+    def lifecycle(self) -> Optional[Lifecycle]:
+        """Describes the current status of the dataset during its lifetime with respect to the storage handling systems."""
+        return self._lifecycle
 
     @property
     def name(self) -> Optional[str]:
-        """A name for the dataset."""
-        return self._fields["name"]  # type: ignore[no-any-return]
+        """A name for the dataset, given by the creator to carry some semantic meaning. Useful for display purposes e.g. instead of displaying the pid. Will be autofilled if missing using info from sourceFolder."""
+        return self._name
 
     @name.setter
-    def name(self, val: Optional[str]) -> None:
-        self._fields["name"] = val
+    def name(self, name: Optional[str]) -> None:
+        """A name for the dataset, given by the creator to carry some semantic meaning. Useful for display purposes e.g. instead of displaying the pid. Will be autofilled if missing using info from sourceFolder."""
+        self._name = name
 
     @property
     def orcid_of_owner(self) -> Optional[str]:
-        """ORCID of owner/custodian. The string may contain a list of ORCID, which should then be separated by semicolons. ORCIDs must include the prefix https://orcid.org/"""
-        return self._fields["orcid_of_owner"]  # type: ignore[no-any-return]
+        """ORCID of the owner or custodian. The string may contain a list of ORCIDs, which should then be separated by semicolons."""
+        return self._orcid_of_owner
 
     @orcid_of_owner.setter
-    def orcid_of_owner(self, val: Optional[str]) -> None:
-        self._fields["orcid_of_owner"] = val
+    def orcid_of_owner(self, orcid_of_owner: Optional[str]) -> None:
+        """ORCID of the owner or custodian. The string may contain a list of ORCIDs, which should then be separated by semicolons."""
+        self._orcid_of_owner = orcid_of_owner
 
     @property
     def owner(self) -> Optional[str]:
-        """Owner or custodian of the dataset, usually first name + lastname. The string may contain a list of persons, which should then be separated by semicolons."""
-        return self._fields["owner"]  # type: ignore[no-any-return]
+        """Owner or custodian of the dataset, usually first name + last name. The string may contain a list of persons, which should then be separated by semicolons."""
+        return self._owner
 
     @owner.setter
-    def owner(self, val: Optional[str]) -> None:
-        self._fields["owner"] = val
+    def owner(self, owner: Optional[str]) -> None:
+        """Owner or custodian of the dataset, usually first name + last name. The string may contain a list of persons, which should then be separated by semicolons."""
+        self._owner = owner
 
     @property
     def owner_email(self) -> Optional[str]:
-        """Email of owner or of custodian of the dataset. The string may contain a list of emails, which should then be separated by semicolons."""
-        return self._fields["owner_email"]  # type: ignore[no-any-return]
+        """Email of the owner or custodian of the dataset. The string may contain a list of emails, which should then be separated by semicolons."""
+        return self._owner_email
 
     @owner_email.setter
-    def owner_email(self, val: Optional[str]) -> None:
-        self._fields["owner_email"] = val
+    def owner_email(self, owner_email: Optional[str]) -> None:
+        """Email of the owner or custodian of the dataset. The string may contain a list of emails, which should then be separated by semicolons."""
+        self._owner_email = owner_email
 
     @property
     def owner_group(self) -> Optional[str]:
-        """Defines the group which owns the data, and therefore has unrestricted access to this data. Usually a pgroup like p12151."""
-        return self._fields["owner_group"]  # type: ignore[no-any-return]
+        """Defines the group which owns the data, and therefore has unrestricted access to this data. Usually a pgroup like p12151"""
+        return self._owner_group
 
     @owner_group.setter
-    def owner_group(self, val: Optional[str]) -> None:
-        self._fields["owner_group"] = val
+    def owner_group(self, owner_group: Optional[str]) -> None:
+        """Defines the group which owns the data, and therefore has unrestricted access to this data. Usually a pgroup like p12151"""
+        self._owner_group = owner_group
+
+    @property
+    def pid(self) -> Optional[PID]:
+        """Persistent Identifier for datasets derived from UUIDv4 and prepended automatically by site specific PID prefix like 20.500.12345/"""
+        return self._pid
 
     @property
     def principal_investigator(self) -> Optional[str]:
-        """Name(s) of the principal investigator(s). The string may contain a list of names, which should then be separated by semicolons."""
-        return self._fields["principal_investigator"]  # type: ignore[no-any-return]
+        """First name and last name of principal investigator(s). If multiple PIs are present, use a semicolon separated list. This field is required if the dataset is a Raw dataset."""
+        return self._principal_investigator
 
     @principal_investigator.setter
-    def principal_investigator(self, val: Optional[str]) -> None:
-        self._fields["principal_investigator"] = val
+    def principal_investigator(self, principal_investigator: Optional[str]) -> None:
+        """First name and last name of principal investigator(s). If multiple PIs are present, use a semicolon separated list. This field is required if the dataset is a Raw dataset."""
+        self._principal_investigator = principal_investigator
 
     @property
     def proposal_id(self) -> Optional[str]:
-        """Identifier for the proposal that the dataset was produced for."""
-        return self._fields["proposal_id"]  # type: ignore[no-any-return]
+        """The ID of the proposal to which the dataset belongs."""
+        return self._proposal_id
 
     @proposal_id.setter
-    def proposal_id(self, val: Optional[str]) -> None:
-        self._fields["proposal_id"] = val
+    def proposal_id(self, proposal_id: Optional[str]) -> None:
+        """The ID of the proposal to which the dataset belongs."""
+        self._proposal_id = proposal_id
+
+    @property
+    def relationships(self) -> Optional[List[Relationship]]:
+        """Stores the relationships with other datasets."""
+        return self._relationships
+
+    @relationships.setter
+    def relationships(self, relationships: Optional[List[Relationship]]) -> None:
+        """Stores the relationships with other datasets."""
+        self._relationships = relationships
 
     @property
     def sample_id(self) -> Optional[str]:
-        """Identifier for the sample that the dataset contains a measurement of."""
-        return self._fields["sample_id"]  # type: ignore[no-any-return]
+        """ID of the sample used when collecting the data."""
+        return self._sample_id
 
     @sample_id.setter
-    def sample_id(self, val: Optional[str]) -> None:
-        self._fields["sample_id"] = val
+    def sample_id(self, sample_id: Optional[str]) -> None:
+        """ID of the sample used when collecting the data."""
+        self._sample_id = sample_id
 
     @property
     def shared_with(self) -> Optional[List[str]]:
         """List of users that the dataset has been shared with."""
-        return self._fields["shared_with"]  # type: ignore[no-any-return]
+        return self._shared_with
 
     @shared_with.setter
-    def shared_with(self, val: Optional[List[str]]) -> None:
-        self._fields["shared_with"] = val
+    def shared_with(self, shared_with: Optional[List[str]]) -> None:
+        """List of users that the dataset has been shared with."""
+        self._shared_with = shared_with
 
     @property
     def source_folder(self) -> Optional[RemotePath]:
-        """Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename."""
-        return self._fields["source_folder"]  # type: ignore[no-any-return]
+        """Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename. Trailing slashes are removed."""
+        return self._source_folder
 
     @source_folder.setter
-    def source_folder(self, val: Optional[RemotePath]) -> None:
-        self._fields["source_folder"] = val
+    def source_folder(self, source_folder: Optional[Union[RemotePath, str]]) -> None:
+        """Absolute file path on file server containing the files of this dataset, e.g. /some/path/to/sourcefolder. In case of a single file dataset, e.g. HDF5 data, it contains the path up to, but excluding the filename. Trailing slashes are removed."""
+        self._source_folder = _parse_remote_path(source_folder)
 
     @property
     def source_folder_host(self) -> Optional[str]:
-        """DNS host name of file server hosting source_folder, optionally including protocol e.g. [protocol://]fileserver1.example.com"""
-        return self._fields["source_folder_host"]  # type: ignore[no-any-return]
+        """DNS host name of file server hosting sourceFolder, optionally including a protocol e.g. [protocol://]fileserver1.example.com"""
+        return self._source_folder_host
 
     @source_folder_host.setter
-    def source_folder_host(self, val: Optional[str]) -> None:
-        self._fields["source_folder_host"] = val
+    def source_folder_host(self, source_folder_host: Optional[str]) -> None:
+        """DNS host name of file server hosting sourceFolder, optionally including a protocol e.g. [protocol://]fileserver1.example.com"""
+        self._source_folder_host = source_folder_host
 
     @property
     def techniques(self) -> Optional[List[Technique]]:
-        """List of techniques used to produce the data."""
-        return self._fields["techniques"]  # type: ignore[no-any-return]
+        """Stores the metadata information for techniques."""
+        return self._techniques
 
     @techniques.setter
-    def techniques(self, val: Optional[List[Technique]]) -> None:
-        self._fields["techniques"] = val
+    def techniques(self, techniques: Optional[List[Technique]]) -> None:
+        """Stores the metadata information for techniques."""
+        self._techniques = techniques
+
+    @property
+    def type(self) -> Optional[DatasetType]:
+        """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
+        return self._type
+
+    @type.setter
+    def type(self, type: Optional[DatasetType]) -> None:
+        """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
+        self._type = type
 
     @property
     def updated_at(self) -> Optional[datetime]:
-        """Time when the object was last updated in the database."""
-        return self._fields["updated_at"]  # type: ignore[no-any-return]
+        """Date and time when this record was updated last. This property is added and maintained by mongoose."""
+        return self._updated_at
 
     @property
     def updated_by(self) -> Optional[str]:
-        """Account name who last updated the object in the database."""
-        return self._fields["updated_by"]  # type: ignore[no-any-return]
+        """Indicate the user who updated this record last. This property is added and maintained by the system."""
+        return self._updated_by
 
     @property
     def used_software(self) -> Optional[List[str]]:
-        """A list of links to software repositories which uniquely identifies the software used and the version for producing the derived data."""
-        return self._fields["used_software"]  # type: ignore[no-any-return]
+        """A list of links to software repositories which uniquely identifies the pieces of software, including versions, used for yielding the derived data. This field is required if the dataset is a Derived dataset."""
+        return self._used_software
 
     @used_software.setter
-    def used_software(self, val: Optional[List[str]]) -> None:
-        self._fields["used_software"] = val
+    def used_software(self, used_software: Optional[List[str]]) -> None:
+        """A list of links to software repositories which uniquely identifies the pieces of software, including versions, used for yielding the derived data. This field is required if the dataset is a Derived dataset."""
+        self._used_software = used_software
 
     @property
     def validation_status(self) -> Optional[str]:
         """Defines a level of trust, e.g. a measure of how much data was verified or used by other persons."""
-        return self._fields["validation_status"]  # type: ignore[no-any-return]
+        return self._validation_status
 
     @validation_status.setter
-    def validation_status(self, val: Optional[str]) -> None:
-        self._fields["validation_status"] = val
+    def validation_status(self, validation_status: Optional[str]) -> None:
+        """Defines a level of trust, e.g. a measure of how much data was verified or used by other persons."""
+        self._validation_status = validation_status
 
     @property
-    def version(self) -> Optional[str]:
-        """Version of SciCat API used in creation of dataset."""
-        return self._fields["version"]  # type: ignore[no-any-return]
-
-    def _make_derived_model(self) -> DerivedDataset:
-        extra_fields = {
-            name: None
-            for name in (
-                "creation_location",
-                "data_format",
-                "end_time",
-                "instrument_id",
-                "principal_investigator",
-                "proposal_id",
-                "sample_id",
-            )
-            if getattr(self, name, None) is not None
-        }
-        return DerivedDataset(
-            accessGroups=self.access_groups,
-            classification=self.classification,
-            contactEmail=self.contact_email,
-            createdAt=self.created_at,
-            createdBy=self.created_by,
-            creationTime=self.creation_time,
-            description=self.description,
-            history=self.history,
-            inputDatasets=self.input_datasets,
-            instrumentGroup=self.instrument_group,
-            investigator=self.investigator,
-            isPublished=self.is_published,
-            jobLogData=self.job_log_data,
-            jobParameters=self.job_parameters,
-            keywords=self.keywords,
-            license=self.license,
-            datasetlifecycle=self.lifecycle,
-            scientificMetadata=self.meta,
-            datasetName=self.name,
-            numberOfFiles=self.number_of_files,
-            numberOfFilesArchived=self.number_of_files_archived,
-            orcidOfOwner=self.orcid_of_owner,
-            owner=self.owner,
-            ownerEmail=self.owner_email,
-            ownerGroup=self.owner_group,
-            packedSize=self.packed_size,
-            pid=self.pid,
-            sharedWith=self.shared_with,
-            size=self.size,
-            sourceFolder=self.source_folder,
-            sourceFolderHost=self.source_folder_host,
-            techniques=self.techniques,
-            type=self.type,
-            updatedAt=self.updated_at,
-            updatedBy=self.updated_by,
-            usedSoftware=self.used_software,
-            validationStatus=self.validation_status,
-            version=self.version,
-            **extra_fields,
-        )
+    def meta(self) -> Dict[str, Any]:
+        """Dict of scientific metadata."""
+        return self._meta
 
-    def _make_raw_model(self) -> RawDataset:
-        extra_fields = {
-            name: None
-            for name in (
-                "input_datasets",
-                "investigator",
-                "job_log_data",
-                "job_parameters",
-                "used_software",
-            )
-            if getattr(self, name, None) is not None
-        }
-        return RawDataset(
-            accessGroups=self.access_groups,
-            classification=self.classification,
-            contactEmail=self.contact_email,
-            createdAt=self.created_at,
-            createdBy=self.created_by,
-            creationLocation=self.creation_location,
-            creationTime=self.creation_time,
-            dataFormat=self.data_format,
-            description=self.description,
-            endTime=self.end_time,
-            history=self.history,
-            instrumentGroup=self.instrument_group,
-            instrumentId=self.instrument_id,
-            isPublished=self.is_published,
-            keywords=self.keywords,
-            license=self.license,
-            datasetlifecycle=self.lifecycle,
-            scientificMetadata=self.meta,
-            datasetName=self.name,
-            numberOfFiles=self.number_of_files,
-            numberOfFilesArchived=self.number_of_files_archived,
-            orcidOfOwner=self.orcid_of_owner,
-            owner=self.owner,
-            ownerEmail=self.owner_email,
-            ownerGroup=self.owner_group,
-            packedSize=self.packed_size,
-            pid=self.pid,
-            principalInvestigator=self.principal_investigator,
-            proposalId=self.proposal_id,
-            sampleId=self.sample_id,
-            sharedWith=self.shared_with,
-            size=self.size,
-            sourceFolder=self.source_folder,
-            sourceFolderHost=self.source_folder_host,
-            techniques=self.techniques,
-            type=self.type,
-            updatedAt=self.updated_at,
-            updatedBy=self.updated_by,
-            validationStatus=self.validation_status,
-            version=self.version,
-            **extra_fields,
-        )
-
-
-def fields_from_model(model: Union[DerivedDataset, RawDataset]) -> dict:
-    return (
-        _fields_from_derived_model(model)
-        if isinstance(model, DerivedDataset)
-        else _fields_from_raw_model(model)
-    )
+    @meta.setter
+    def meta(self, meta: Dict[str, Any]) -> None:
+        """Dict of scientific metadata."""
+        self._meta = meta
 
+    @staticmethod
+    def _prepare_fields_from_download(
+        download_model: DownloadDataset,
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        init_args = {}
+        read_only = {}
+        for field in DatasetBase._FIELD_SPEC:
+            if field.read_only:
+                read_only["_" + field.name] = getattr(download_model, field.scicat_name)
+            else:
+                init_args[field.name] = getattr(download_model, field.scicat_name)
 
-def _fields_from_derived_model(model) -> dict:
-    return dict(
-        _read_only=dict(
-            created_at=model.createdAt,
-            created_by=model.createdBy,
-            updated_at=model.updatedAt,
-            updated_by=model.updatedBy,
-            version=model.version,
-        ),
-        access_groups=model.accessGroups,
-        classification=model.classification,
-        contact_email=model.contactEmail,
-        description=model.description,
-        input_datasets=model.inputDatasets,
-        instrument_group=model.instrumentGroup,
-        investigator=model.investigator,
-        is_published=model.isPublished,
-        job_log_data=model.jobLogData,
-        job_parameters=model.jobParameters,
-        keywords=model.keywords,
-        license=model.license,
-        lifecycle=model.datasetlifecycle,
-        meta=model.scientificMetadata,
-        name=model.datasetName,
-        orcid_of_owner=model.orcidOfOwner,
-        owner=model.owner,
-        owner_email=model.ownerEmail,
-        owner_group=model.ownerGroup,
-        shared_with=model.sharedWith,
-        source_folder=model.sourceFolder,
-        source_folder_host=model.sourceFolderHost,
-        techniques=model.techniques,
-        used_software=model.usedSoftware,
-        validation_status=model.validationStatus,
-    )
+        init_args["meta"] = download_model.scientificMetadata
+        DatasetBase._convert_readonly_fields_in_place(read_only)
 
+        return init_args, read_only
 
-def _fields_from_raw_model(model) -> dict:
-    return dict(
-        _read_only=dict(
-            created_at=model.createdAt,
-            created_by=model.createdBy,
-            updated_at=model.updatedAt,
-            updated_by=model.updatedBy,
-            version=model.version,
-        ),
-        access_groups=model.accessGroups,
-        classification=model.classification,
-        contact_email=model.contactEmail,
-        creation_location=model.creationLocation,
-        data_format=model.dataFormat,
-        description=model.description,
-        end_time=model.endTime,
-        instrument_group=model.instrumentGroup,
-        instrument_id=model.instrumentId,
-        is_published=model.isPublished,
-        keywords=model.keywords,
-        license=model.license,
-        lifecycle=model.datasetlifecycle,
-        meta=model.scientificMetadata,
-        name=model.datasetName,
-        orcid_of_owner=model.orcidOfOwner,
-        owner=model.owner,
-        owner_email=model.ownerEmail,
-        owner_group=model.ownerGroup,
-        principal_investigator=model.principalInvestigator,
-        proposal_id=model.proposalId,
-        sample_id=model.sampleId,
-        shared_with=model.sharedWith,
-        source_folder=model.sourceFolder,
-        source_folder_host=model.sourceFolderHost,
-        techniques=model.techniques,
-        validation_status=model.validationStatus,
-    )
+    @staticmethod
+    def _convert_readonly_fields_in_place(read_only: Dict[str, Any]) -> Dict[str, Any]:
+        if "_pid" in read_only:
+            read_only["_pid"] = _parse_pid(read_only["_pid"])
+        return read_only
```

### Comparing `scitacean-23.5.0/src/scitacean/_html_repr/__init__.py` & `scitacean-23.7.7/src/scitacean/_html_repr/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import pydantic
 
 from ..dataset import Dataset
 from ..filesystem import RemotePath
-from ..model import DatasetLifecycle, DatasetType, Technique
+from ..model import DatasetType, History, Lifecycle, Relationship, Technique
 from ..pid import PID
 from . import resources
 
 
 def dataset_html_repr(dset: Dataset) -> str:
     template = resources.dataset_repr_template()
     style_sheet = resources.dataset_style()
@@ -157,15 +157,15 @@
     fields = [
         Field(
             name=field.name,
             value=getattr(dset, field.name, None),
             type=field.type,
             description=field.description,
             read_only=field.read_only,
-            required=field.required(dset.type),
+            required=field.required,
             error=_check_error(field, validation),
             main=field.name in _MAIN_FIELDS,
         )
         for field in dset.fields()
         if field.name not in _EXCLUDED_FIELDS
         and (field.used_by(dset.type) or getattr(dset, field.name, None) is not None)
     ]
@@ -194,23 +194,25 @@
         return {single_elem(error["loc"]): error["msg"] for error in e.errors()}
 
 
 _TYPE_NAME = {
     str: "str",
     int: "int",
     bool: "bool",
+    dict: "dict",
     datetime: "datetime",
+    History: "History",
+    Lifecycle: "Lifecycle",
     PID: "PID",
-    DatasetLifecycle: "DatasetLifecycle",
     RemotePath: "RemotePath",
     List[str]: "list[str]",
     List[PID]: "list[PID]",
+    List[Relationship]: "list[Relationship]",
     List[Technique]: "list[Technique]",
     List[dict]: "list[dict]",  # type: ignore[type-arg]
-    dict: "dict",
 }
 
 
 def _format_type(typ: Any) -> str:
     try:
         return _TYPE_NAME[typ]
     except KeyError:
```

### Comparing `scitacean-23.5.0/src/scitacean/_html_repr/images/lock.svg` & `scitacean-23.7.7/src/scitacean/_html_repr/images/lock.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/_html_repr/resources.py` & `scitacean-23.7.7/src/scitacean/_html_repr/resources.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/_html_repr/styles/dataset.css` & `scitacean-23.7.7/src/scitacean/_html_repr/styles/dataset.css`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/_html_repr/templates/dataset_repr.html.template` & `scitacean-23.7.7/src/scitacean/_html_repr/templates/dataset_repr.html.template`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/_internal/orcid.py` & `scitacean-23.7.7/src/scitacean/_internal/orcid.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/client.py` & `scitacean-23.7.7/src/scitacean/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,26 +161,25 @@
             A warning will be logged if validation fails.
 
         Returns
         -------
         :
             A new dataset.
         """
-        if isinstance(pid, str):
-            pid = PID.parse(pid)
+        pid = PID.parse(pid)
         try:
             orig_datablocks = self.scicat.get_orig_datablocks(
                 pid, strict_validation=strict_validation
             )
         except ScicatCommError:
             # TODO more precise error handling. We only want to set to None if
             #   communication succeeded and the dataset exists but there simply
             #   are no datablocks.
             orig_datablocks = None
-        return Dataset.from_models(
+        return Dataset.from_download_models(
             dataset_model=self.scicat.get_dataset_model(
                 pid, strict_validation=strict_validation
             ),
             orig_datablock_models=orig_datablocks,
         )
 
     def upload_new_dataset_now(self, dataset: Dataset) -> Dataset:
@@ -207,48 +206,46 @@
         scitacean.ScicatCommError
             If the upload to SciCat fails.
         RuntimeError
             If the file upload fails or if a critical error is encountered
             and some files or a partial dataset are left on the servers.
             Note the error message if that happens.
         """
-        if dataset.pid is not None:
-            raise ValueError(
-                "Cannot upload the dataset because it has a PID. "
-                "Set the PID to None, the server will assign one for you."
-            )
         dataset = dataset.replace(
             source_folder=self._expect_file_transfer().source_folder_for(dataset)
         )
         dataset.validate()
+        # TODO skip if there are no files
         with self._connect_for_file_upload(dataset) as con:
             # TODO check if any remote file is out of date.
             #  if so, raise an error. We never overwrite remote files!
             uploaded_files = con.upload_files(*dataset.files)
             dataset = dataset.replace_files(*uploaded_files)
             try:
-                finalized_model = self.scicat.create_dataset_model(dataset.make_model())
+                finalized_model = self.scicat.create_dataset_model(
+                    dataset.make_upload_model()
+                )
             except ScicatCommError:
                 con.revert_upload(*uploaded_files)
                 raise
 
-        with_new_pid = dataset.replace(pid=finalized_model.pid)
-        datablock_models = with_new_pid.make_datablock_models()
+        with_new_pid = dataset.replace(_read_only={"pid": finalized_model.pid})
+        datablock_models = with_new_pid.make_datablock_upload_models()
         finalized_orig_datablocks = self._upload_orig_datablocks(
             datablock_models.orig_datablocks
         )
 
-        return Dataset.from_models(
+        return Dataset.from_download_models(
             dataset_model=finalized_model,
             orig_datablock_models=finalized_orig_datablocks,
         )
 
     def _upload_orig_datablocks(
-        self, orig_datablocks: Optional[List[model.OrigDatablock]]
-    ) -> Optional[List[model.OrigDatablock]]:
+        self, orig_datablocks: Optional[List[model.UploadOrigDatablock]]
+    ) -> Optional[List[model.DownloadOrigDatablock]]:
         if orig_datablocks is None:
             return None
 
         try:
             return [
                 self.scicat.create_orig_datablock(orig_datablock)
                 for orig_datablock in orig_datablocks
@@ -459,15 +456,15 @@
     def without_login(
         cls, url: str, timeout: Optional[datetime.timedelta] = None
     ) -> ScicatClient:
         return ScicatClient(url=url, token=None, timeout=timeout)
 
     def get_dataset_model(
         self, pid: PID, strict_validation: bool = False
-    ) -> Union[model.DerivedDataset, model.RawDataset]:
+    ) -> model.DownloadDataset:
         """Fetch a dataset from SciCat.
 
         Parameters
         ----------
         pid:
             Unique ID of the dataset. Must include the facility ID.
         strict_validation:
@@ -475,37 +472,35 @@
             If ``False``, a dataset is still returned if validation fails.
             Note that some dataset fields may have a bad value or type.
             A warning will be logged if validation fails.
 
         Returns
         -------
         :
-            A model of the dataset. The type is deduced from the received data.
+            A model of the dataset.
 
         Raises
         ------
         scitacean.ScicatCommError
             If the dataset does not exist or communication fails for some other reason.
         """
         dset_json = self._call_endpoint(
             cmd="get",
             url=f"datasets/{quote_plus(str(pid))}",
             operation="get_dataset_model",
         )
         return model.construct(
-            model.DerivedDataset
-            if dset_json["type"] == "derived"
-            else model.RawDataset,
+            model.DownloadDataset,
             _strict_validation=strict_validation,
             **dset_json,
-        )  # type: ignore[return-value]
+        )
 
     def get_orig_datablocks(
         self, pid: PID, strict_validation: bool = False
-    ) -> List[model.OrigDatablock]:
+    ) -> List[model.DownloadOrigDatablock]:
         """Fetch all orig datablocks from SciCat for a given dataset.
 
         Parameters
         ----------
         pid:
             Unique ID of the *dataset*. Must include the facility ID.
         strict_validation:
@@ -523,25 +518,25 @@
         ------
         scitacean.ScicatCommError
             If the datablock does not exist or communication
             fails for some other reason.
         """
         dblock_json = self._call_endpoint(
             cmd="get",
-            url=f"Datasets/{quote_plus(str(pid))}/origdatablocks",
+            url=f"datasets/{quote_plus(str(pid))}/origdatablocks",
             operation="get_orig_datablocks",
         )
         return [
             _make_orig_datablock(dblock, strict_validation=strict_validation)
             for dblock in dblock_json
         ]
 
     def create_dataset_model(
-        self, dset: Union[model.DerivedDataset, model.RawDataset]
-    ) -> Union[model.DerivedDataset, model.RawDataset]:
+        self, dset: Union[model.UploadDerivedDataset, model.UploadRawDataset]
+    ) -> model.DownloadDataset:
         """Create a new dataset in SciCat.
 
         The dataset PID must be either
 
         - ``None``, in which case SciCat assigns an ID,
         - an unused id, in which case SciCat uses it for the new dataset.
 
@@ -554,32 +549,33 @@
         ----------
         dset:
             Model of the dataset to create.
 
         Returns
         -------
         :
-            The PID of the new dataset in the catalogue.
+            The uploaded dataset as returned by SciCat.
+            This is the input plus some modifications.
 
         Raises
         ------
         scitacean.ScicatCommError
             If SciCat refuses the dataset or communication
             fails for some other reason.
         """
         uploaded = self._call_endpoint(
             cmd="post", url="datasets", data=dset, operation="create_dataset_model"
         )
-        return (
-            model.DerivedDataset(**uploaded)
-            if uploaded["type"] == "derived"
-            else model.RawDataset(**uploaded)
+        return model.construct(
+            model.DownloadDataset, _strict_validation=False, **uploaded
         )
 
-    def create_orig_datablock(self, dblock: model.OrigDatablock) -> model.OrigDatablock:
+    def create_orig_datablock(
+        self, dblock: model.UploadOrigDatablock
+    ) -> model.DownloadOrigDatablock:
         """Create a new orig datablock in SciCat.
 
         The datablock PID must be either
 
         - ``None``, in which case SciCat assigns an ID.
         - An unused id, in which case SciCat uses it for the new datablock.
 
@@ -593,21 +589,22 @@
 
         Raises
         ------
         scitacean.ScicatCommError
             If SciCat refuses the datablock or communication
             fails for some other reason.
         """
-        return model.OrigDatablock(
-            **self._call_endpoint(
-                cmd="post",
-                url="origdatablocks",
-                data=dblock,
-                operation="create_orig_datablock",
-            )
+        uploaded = self._call_endpoint(
+            cmd="post",
+            url="origdatablocks",
+            data=dblock,
+            operation="create_orig_datablock",
+        )
+        return model.construct(
+            model.DownloadOrigDatablock, _strict_validation=False, **uploaded
         )
 
     def _send_to_scicat(
         self, *, cmd: str, url: str, data: Optional[model.BaseModel] = None
     ) -> requests.Response:
         if self._token is not None:
             token = self._token.get_str()
@@ -621,15 +618,17 @@
         if data is not None:
             headers["Content-Type"] = "application/json"
 
         try:
             return requests.request(
                 method=cmd,
                 url=url,
-                data=data.json(exclude_none=True) if data is not None else None,
+                data=data.model_dump_json(exclude_none=True)
+                if data is not None
+                else None,
                 params=params,
                 headers=headers,
                 timeout=self._timeout.seconds,
                 stream=False,
                 verify=True,
             )
         except Exception as exc:
@@ -651,23 +650,34 @@
         operation: str,
     ) -> Any:
         full_url = _url_concat(self._base_url, url)
         logger = get_logger()
         logger.info("Calling SciCat API at %s for operation '%s'", full_url, operation)
 
         response = self._send_to_scicat(cmd=cmd, url=full_url, data=data)
-        if not response.ok:
-            err = response.json().get("message", {})
-            logger.error("API call failed, endpoint: %s, response: %s", full_url, err)
-            raise ScicatCommError(f"Error in operation {operation}: {err}")
+        if not response.ok or not response.text:
+            logger.error(
+                "SciCat API call to %s failed: %s %s: %s",
+                full_url,
+                response.status_code,
+                response.reason,
+                response.text,
+            )
+            raise ScicatCommError(
+                f"Error in operation '{operation}': {response.status_code} "
+                f"{response.reason}: {response.text}"
+            )
         logger.info("API call successful for operation '%s'", operation)
-        res = response.json()
+        res = response.json()  # TODO can fail
+        # TODO should this raise? This happens e.g. when listing all
+        #  datasets but there are none
         if not res:
             raise ScicatCommError(
-                f"{cmd} to {url} succeeded but di not return anything."
+                f"Internal SciCat communication error: {cmd.upper()} request to "
+                f"{full_url} succeeded but did not return anything."
             )
         return res
 
 
 def _url_concat(a: str, b: str) -> str:
     # Combine two pieces or a URL without handling absolute
     # paths as in urljoin.
@@ -682,23 +692,23 @@
     if token:  # token can be ""
         error = error.replace(token, "<HIDDEN>")
     return error
 
 
 def _make_orig_datablock(
     fields: Dict[str, Any], strict_validation: bool
-) -> model.OrigDatablock:
+) -> model.DownloadOrigDatablock:
     files = [
         model.construct(
-            model.DataFile, _strict_validation=strict_validation, **file_fields
+            model.DownloadDataFile, _strict_validation=strict_validation, **file_fields
         )
         for file_fields in fields["dataFileList"]
     ]
     return model.construct(
-        model.OrigDatablock,
+        model.DownloadOrigDatablock,
         _strict_validation=strict_validation,
         **{**fields, "dataFileList": files},
     )
 
 
 def _log_in_via_users_login(
     url: str, username: StrStorage, password: StrStorage, timeout: datetime.timedelta
```

### Comparing `scitacean-23.5.0/src/scitacean/dataset.py` & `scitacean-23.7.7/src/scitacean/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,76 +2,78 @@
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Main dataset structure."""
 
 from __future__ import annotations
 
 import dataclasses
 import itertools
-from copy import deepcopy
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Any, Dict, Generator, Iterable, List, Literal, Optional, Tuple, Union
+from typing import (
+    Any,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
-from ._dataset_fields import DatasetFields, fields_from_model
-from .datablock import OrigDatablockProxy
+from ._dataset_fields import DatasetBase
+from .datablock import OrigDatablock
 from .file import File
 from .model import (
+    BaseUserModel,
     DatasetType,
-    DerivedDataset,
-    OrigDatablock,
-    RawDataset,
+    DownloadDataset,
+    DownloadOrigDatablock,
+    Relationship,
+    Technique,
+    UploadDerivedDataset,
+    UploadOrigDatablock,
+    UploadRawDataset,
 )
 from .pid import PID
 
 
-class Dataset(DatasetFields):
+class Dataset(DatasetBase):
     @classmethod
-    def from_models(
+    def from_download_models(
         cls,
-        *,
-        dataset_model: Union[DerivedDataset, RawDataset],
-        orig_datablock_models: Optional[List[OrigDatablock]],
+        dataset_model: DownloadDataset,
+        orig_datablock_models: List[DownloadOrigDatablock],
     ) -> Dataset:
-        """Create a new dataset from pydantic models.
-
-        This function is mainly meant to be used with
-        models that were downloaded from SciCat.
-        :meth:`Dataset.__init__` should be preferred for other use cases.
+        """Construct a new dataset from SciCat download models.
 
         Parameters
         ----------
         dataset_model:
-            Fields, including scientific metadata are filled from this model.
+            Model of the dataset.
         orig_datablock_models:
-            File links are populated from this model.
-            All files are initialized to be on remote but not local.
+            List of all associated original datablock models for the dataset.
 
         Returns
         -------
         :
-            A new dataset.
+            A new Dataset instance.
         """
-        args = fields_from_model(dataset_model)
-        read_only_args = args.pop("_read_only")
-        read_only_args["history"] = dataset_model.history
-        return cls(
-            type=dataset_model.type,
-            creation_time=dataset_model.creationTime,
-            pid=dataset_model.pid,
-            _orig_datablocks=[]
-            if not orig_datablock_models
-            else [
-                OrigDatablockProxy.from_model(
-                    dataset_model=dataset_model, orig_datablock_model=dblock
-                )
-                for dblock in orig_datablock_models
-            ],
-            _read_only=read_only_args,
-            **args,
-        )
+        init_args, read_only = DatasetBase._prepare_fields_from_download(dataset_model)
+        for mod, key in ((Technique, "techniques"), (Relationship, "relationships")):
+            init_args[key] = _list_field_from_download(mod, init_args[key])
+        dset = cls(**init_args)
+        for key, val in read_only.items():
+            setattr(dset, key, val)
+        if orig_datablock_models is not None:
+            dset._orig_datablocks.extend(
+                map(OrigDatablock.from_download_model, orig_datablock_models)
+            )
+        return dset
 
     @classmethod
     def fields(
         cls,
         dataset_type: Optional[Union[DatasetType, Literal["derived", "raw"]]] = None,
         read_only: Optional[bool] = None,
     ) -> Generator[Dataset.Field, None, None]:
@@ -90,40 +92,59 @@
             If unset, do not filter fields.
 
         Returns
         -------
         :
             Iterable over the fields of datasets.
         """
-        it = iter(DatasetFields._FIELD_SPEC)
+        it = iter(DatasetBase._FIELD_SPEC)
         if dataset_type is not None:
             attr = (
                 "used_by_derived"
                 if dataset_type == DatasetType.DERIVED
                 else "used_by_raw"
             )
             it = filter(lambda field: getattr(field, attr), it)
         if read_only is not None:
             it = filter(lambda field: field.read_only == read_only, it)
         yield from it
 
-    @property
-    def history(self) -> List[Dataset]:
-        # TODO convert elements to Dataset
-        return self._fields["history"]
+    def __str__(self) -> str:
+        args = ", ".join(
+            f"{field.name}={value}"
+            for field in self.fields()
+            if (value := getattr(self, field.name)) is not None
+        )
+        return f"Dataset({args})"
+
+    def _repr_html_(self) -> str:
+        # Import here to prevent cycle.
+        from ._html_repr import dataset_html_repr
+
+        return dataset_html_repr(self)
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Dataset):
+            return False
+        eq = all(
+            getattr(self, field.name) == getattr(other, field.name)
+            for field in Dataset.fields()
+        )
+        eq = eq and self._orig_datablocks == other._orig_datablocks
+        return eq
 
     @property
     def number_of_files(self) -> int:
         """Number of files in directly accessible storage in the dataset.
 
         This includes files on both the local and remote filesystems.
 
         Corresponds to OrigDatablocks.
         """
-        return sum(map(lambda dblock: len(tuple(dblock.files)), self._orig_datablocks))
+        return sum(len(tuple(dblock.files)) for dblock in self._orig_datablocks)
 
     @property
     def number_of_files_archived(self) -> int:
         """Total number of archived files in the dataset.
 
         Corresponds to Datablocks.
         """
@@ -157,15 +178,15 @@
         """Add files to the dataset."""
         self._get_or_add_orig_datablock(datablock).add_files(*files)
 
     def add_local_files(
         self,
         *paths: Union[str, Path],
         base_path: Union[str, Path] = "",
-        datablock: Union[int, str, PID] = -1,
+        datablock: Union[int, str] = -1,
     ) -> None:
         """Add files on the local file system to the dataset.
 
         Parameters
         ----------
         paths:
             Local paths to the files.
@@ -186,15 +207,15 @@
             datablock=datablock,
         )
 
     def replace(
         self,
         *,
         _read_only: Optional[Dict[str, Any]] = None,
-        _orig_datablocks: Optional[List[OrigDatablockProxy]] = None,
+        _orig_datablocks: Optional[List[OrigDatablock]] = None,
         **replacements: Any,
     ) -> Dataset:
         """Return a new dataset with replaced fields.
 
         Parameters starting with an underscore are for internal use.
         Using them may result in a broken dataset.
 
@@ -217,33 +238,34 @@
             except KeyError:
                 return getattr(self, name)
 
         read_only = {
             field.name: get_val(_read_only, field.name)
             for field in Dataset.fields(read_only=True)
         }
+        DatasetBase._convert_readonly_fields_in_place(read_only)
         kwargs = {
             **{
                 field.name: get_val(replacements, field.name)
                 for field in Dataset.fields(read_only=False)
             },
         }
         if replacements or _read_only:
             raise TypeError(
                 f"Invalid arguments: {', '.join((*replacements, *_read_only))}"
             )
-        return Dataset(
-            _orig_datablocks=deepcopy(
-                _orig_datablocks
-                if _orig_datablocks is not None
-                else self._orig_datablocks
-            ),
-            _read_only=read_only,
+        dset = Dataset(
             **kwargs,
         )
+        dset._orig_datablocks.extend(
+            _orig_datablocks if _orig_datablocks is not None else self._orig_datablocks
+        )
+        for key, val in read_only.items():
+            setattr(dset, "_" + key, val)
+        return dset
 
     def as_new(self) -> Dataset:
         """Return a new dataset with lifecycle-related fields erased.
 
         The returned dataset has the same fields as ``self``.
         But fields that indicate when the dataset was created or
         by who are set to ``None``.
@@ -253,15 +275,14 @@
         -------
         :
             A new dataset without lifecycle-related fields.
         """
         return self.replace(
             _read_only={field.name: None for field in Dataset.fields(read_only=True)},
             creation_time=datetime.now(tz=timezone.utc),
-            lifecycle=None,
         )
 
     def derive(
         self,
         *,
         keep: Iterable[str] = (
             "contact_email",
@@ -333,119 +354,114 @@
         return self.replace(
             _orig_datablocks=[
                 dataclasses.replace(dblock, init_files=map(new_or_old, dblock.files))
                 for dblock in self._orig_datablocks
             ]
         )
 
-    def make_datablock_models(self) -> DatablockModels:
-        """Build models for all contained (orig) datablocks.
-
-        Returns
-        -------
-        :
-            Structure with datablock and orig datablock models.
-        """
-        if self.number_of_files == 0:
-            return DatablockModels(orig_datablocks=None)
-        return DatablockModels(
-            orig_datablocks=[
-                dblock.make_model(self) for dblock in self._orig_datablocks
-            ]
-        )
-
-    def make_model(self) -> Union[DerivedDataset, RawDataset]:
-        """Build a dataset model to send to SciCat.
-
-        This triggers validation of the dataset.
-        All fields must therefore be properly initialized for a dataset of type
-        ``self.type`` before calling ``make_model``.
-
-        Returns
-        -------
-        :
-            Created model.
-        """
-        if self.type == DatasetType.DERIVED:
-            return self._make_derived_model()
-        return self._make_raw_model()
-
-    def validate(self) -> None:
-        """Validate the fields of the dataset.
-
-        Raises :class:`pydantic.ValidationError` if validation fails.
-        Returns normally if it passes.
-        """
-        self.make_model()
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, Dataset):
-            return False
-        eq = all(
-            getattr(self, field.name) == getattr(other, field.name)
-            for field in Dataset.fields()
-        )
-        return eq
-
-    def add_orig_datablock(
-        self, *, checksum_algorithm: Optional[str]
-    ) -> OrigDatablockProxy:
+    def add_orig_datablock(self, *, checksum_algorithm: Optional[str]) -> OrigDatablock:
         """Append a new orig datablock to the list of orig datablocks.
 
         Parameters
         ----------
         checksum_algorithm:
             Use this algorithm to compute checksums of files
             associated with this datablock.
 
         Returns
         -------
         :
             The newly added datablock.
         """
-        dblock = OrigDatablockProxy(checksum_algorithm=checksum_algorithm)
+        dblock = OrigDatablock(
+            checksum_algorithm=checksum_algorithm, _dataset_id=self.pid
+        )
         self._orig_datablocks.append(dblock)
         return dblock
 
-    def _lookup_orig_datablock(self, pid: PID) -> OrigDatablockProxy:
+    def _lookup_orig_datablock(self, id_: str) -> OrigDatablock:
         try:
-            return next(db for db in self._orig_datablocks if db.pid == pid)
+            return next(db for db in self._orig_datablocks if db.datablock_id == id_)
         except StopIteration:
-            raise KeyError(f"No OrigDatablock with id {PID}") from None
+            raise KeyError(f"No OrigDatablock with id {id_}") from None
 
-    def _get_or_add_orig_datablock(
-        self, key: Union[int, str, PID]
-    ) -> OrigDatablockProxy:
-        if isinstance(key, (str, PID)):
-            return self._lookup_orig_datablock(PID.parse(key))
-        # The oth datablock is implicitly always there and created on demand.
+    def _get_or_add_orig_datablock(self, key: Union[int, str]) -> OrigDatablock:
+        if isinstance(key, str):
+            return self._lookup_orig_datablock(key)
+        # The 0th datablock is implicitly always there and created on demand.
         if key in (0, -1) and not self._orig_datablocks:
             return self.add_orig_datablock(
                 checksum_algorithm=self._default_checksum_algorithm
             )
         return self._orig_datablocks[key]
 
-    def __str__(self) -> str:
-        args = ", ".join(
-            f"{name}={value}"
-            for name, value in (
-                (field.name, getattr(self, field.name)) for field in self.fields()
-            )
-            if value is not None
+    def make_upload_model(self) -> Union[UploadDerivedDataset, UploadRawDataset]:
+        """Construct a SciCat upload model from self."""
+        model = (
+            UploadRawDataset if self.type == DatasetType.RAW else UploadDerivedDataset
+        )
+        # Datablocks are not included here because they are handled separately
+        # by make_datablock_upload_models and their own endpoints.
+        special = ("relationships", "techniques")
+        return model(
+            numberOfFiles=self.number_of_files,
+            numberOfFilesArchived=self.number_of_files_archived,
+            size=self.size,
+            packedSize=self.packed_size,
+            scientificMetadata=self._meta or None,
+            techniques=_list_field_for_upload(self.techniques),
+            relationships=_list_field_for_upload(self.relationships),
+            **{
+                field.scicat_name: value
+                for field in self.fields()
+                if field.name not in special
+                and (value := getattr(self, field.name)) is not None
+            },
         )
-        return f"Dataset({args})"
 
-    def _repr_html_(self) -> str:
-        # Import here to prevent cycle.
-        from ._html_repr import dataset_html_repr
+    def make_datablock_upload_models(self) -> DatablockUploadModels:
+        """Build models for all contained (orig) datablocks.
 
-        return dataset_html_repr(self)
+        Returns
+        -------
+        :
+            Structure with datablock and orig datablock models.
+        """
+        if self.number_of_files == 0:
+            return DatablockUploadModels(orig_datablocks=None)
+        return DatablockUploadModels(
+            orig_datablocks=[
+                dblock.make_upload_model(self) for dblock in self._orig_datablocks
+            ]
+        )
+
+    def validate(self) -> None:
+        """Validate the fields of the dataset.
+
+        Raises :class:`pydantic.ValidationError` if validation fails.
+        Returns normally if it passes.
+        """
+        self.make_upload_model()
 
 
 @dataclasses.dataclass
-class DatablockModels:
+class DatablockUploadModels:
     """Pydantic models for (orig) datablocks."""
 
     # TODO
-    # datablocks: Optional[List[Datablock]]
-    orig_datablocks: Optional[List[OrigDatablock]]
+    # datablocks: Optional[List[UploadDatablock]]
+    orig_datablocks: Optional[List[UploadOrigDatablock]]
     """Orig datablocks"""
+
+
+def _list_field_for_upload(value: Optional[List[Any]]) -> Optional[List[Any]]:
+    if value is None:
+        return None
+    return [item.make_upload_model() for item in value]
+
+
+def _list_field_from_download(
+    mod: Type[BaseUserModel], value: Optional[List[Any]]
+) -> Optional[List[Any]]:
+    if value is None:
+        return None
+    return [mod.from_download_model(item) for item in value]
```

### Comparing `scitacean-23.5.0/src/scitacean/file.py` & `scitacean-23.7.7/src/scitacean/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import NoReturn, Optional, Union, cast
 
 from .error import IntegrityError
 from .filesystem import RemotePath, checksum_of_file, file_modification_time, file_size
 from .logging import get_logger
-from .model import DataFile
+from .model import DownloadDataFile, UploadDataFile
 
 
 @dataclasses.dataclass(frozen=True)
 class File:
     """Store local and remote paths and metadata for a file.
 
     There are two central properties:
@@ -47,22 +47,14 @@
     """Path to the file on the remote filesystem."""
     remote_gid: Optional[str]
     """Unix group ID on remote."""
     remote_perm: Optional[str]
     """Unix file mode on remote."""
     remote_uid: Optional[str]
     """Unix user ID on remote."""
-    created_at: Optional[datetime] = None
-    """Creator of the file entry in SciCat."""
-    created_by: Optional[str] = None
-    """Creation time of the file entry in SciCat."""
-    updated_at: Optional[datetime] = None
-    """Last updator of the file entry in SciCat."""
-    updated_by: Optional[str] = None
-    """Last update time of the file entry in SciCat."""
     checksum_algorithm: Optional[str] = None
     """Algorithm to use for checksums."""
     _remote_size: Optional[int] = dataclasses.field(default=None, repr=False)
     _remote_creation_time: Optional[datetime] = dataclasses.field(
         default=None, repr=False
     )
     _remote_checksum: Optional[str] = dataclasses.field(default=None, repr=False)
@@ -123,16 +115,17 @@
             remote_uid=remote_uid,
             _checksum_cache=_Checksum(),
         )
 
     @classmethod
     def from_scicat(
         cls,
-        model: DataFile,
+        model: DownloadDataFile,
         *,
+        checksum_algorithm: Optional[str] = None,
         local_path: Optional[Union[str, Path]] = None,
     ) -> File:
         """Construct a new file object from SciCat models.
 
         Parameters
         ----------
         model:
@@ -142,23 +135,20 @@
 
         Returns
         -------
         :
             A new file object.
         """
         return File(
+            checksum_algorithm=checksum_algorithm,
             local_path=Path(local_path) if isinstance(local_path, str) else local_path,
             remote_path=RemotePath(model.path),
             remote_gid=model.gid,
             remote_perm=model.perm,
             remote_uid=model.uid,
-            created_at=model.createdAt,
-            created_by=model.createdBy,
-            updated_at=model.updatedAt,
-            updated_by=model.updatedBy,
             _remote_size=model.size,
             _remote_creation_time=model.time,
             _remote_checksum=model.chk,
         )
 
     @property
     def size(self) -> int:
@@ -248,15 +238,15 @@
     def _local_is_up_to_date_with_checksum_algorithm(self, algorithm: str) -> bool:
         local_checksum = self._checksum_cache.get(  # type: ignore[union-attr]
             path=self.local_path,  # type: ignore[arg-type]
             algorithm=algorithm,
         )
         return self._remote_checksum == local_checksum
 
-    def make_model(self, *, for_archive: bool = False) -> DataFile:
+    def make_model(self, *, for_archive: bool = False) -> UploadDataFile:
         """Build a pydantic model for this file.
 
         Parameters
         ----------
         for_archive:
             Select whether the file is stored in an archive or on regular disk,
             that is whether it belongs to a Datablock or an OrigDatablock.
@@ -264,15 +254,15 @@
         Returns
         -------
         :
             A new pydantic model.
         """
         chk = self.checksum()
         # TODO if for_archive: ensure not out of date
-        return DataFile(
+        return UploadDataFile(
             path=self.remote_path.posix,
             size=self.size,
             chk=chk,
             gid=self.remote_gid,
             perm=self.remote_perm,
             time=self.creation_time,
             uid=self.remote_uid,
```

### Comparing `scitacean-23.5.0/src/scitacean/filesystem.py` & `scitacean-23.7.7/src/scitacean/filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,35 @@
 import hashlib
 import os
 import re
 from datetime import datetime, timezone
 from pathlib import Path, PurePath
 from typing import Any, Callable, Generator, Optional, TypeVar, Union
 
+from ._internal.pydantic_compat import is_pydantic_v1
+
+if not is_pydantic_v1():
+    from pydantic import GetCoreSchemaHandler
+    from pydantic_core import core_schema
+
+    def _get_remote_path_core_schema(
+        cls, _source_type: Any, _handler: GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_after_validator_function(
+            cls,
+            core_schema.union_schema(
+                [core_schema.is_instance_schema(RemotePath), core_schema.str_schema()]
+            ),
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                lambda p: p.posix if isinstance(p, RemotePath) else str(p),
+                info_arg=False,
+                return_schema=core_schema.str_schema(),
+            ),
+        )
+
 
 class RemotePath:
     """A path on the remote filesystem.
 
     Remote paths do not need to correspond to a regular filesystem path like
     :class:`pathlib.PosixPath` or :class:`pathlib.WindowsPath`.
     Instead, they can be any sequence of segments that are joined by forward slashes,
@@ -136,24 +157,29 @@
             name = parts[0]
             suffix = "." + parts[1] if len(parts) > 1 else ""
             return (name[: max(1, max_length - len(suffix))] + suffix)[:max_length]
 
         return RemotePath("/".join(map(trunc, self._path.split("/"))))
 
     @classmethod
-    def __get_validators__(
-        cls,
-    ) -> Generator[Callable[[Union[str, RemotePath]], RemotePath], None, None]:
-        yield cls.validate
-
-    @classmethod
     def validate(cls, value: Union[str, RemotePath]) -> RemotePath:
         """Pydantic validator for RemotePath fields."""
         return RemotePath(value)
 
+    if is_pydantic_v1():
+
+        @classmethod
+        def __get_validators__(
+            cls,
+        ) -> Generator[Callable[[Union[str, RemotePath]], RemotePath], None, None]:
+            yield cls.validate
+
+    else:
+        __get_pydantic_core_schema__ = classmethod(_get_remote_path_core_schema)
+
 
 def _posix(path: Union[str, RemotePath]) -> str:
     return path.posix if isinstance(path, RemotePath) else path
 
 
 def _strip_trailing_slash(s: str) -> str:
     return s[:-1] if s.endswith("/") else s
```

### Comparing `scitacean-23.5.0/src/scitacean/logging.py` & `scitacean-23.7.7/src/scitacean/logging.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/pid.py` & `scitacean-23.7.7/src/scitacean/pid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 from __future__ import annotations
 
 import uuid
 from typing import Callable, Generator, Optional, Union
 
+import pydantic
+
+from ._internal.pydantic_compat import is_pydantic_v1
+
+if not is_pydantic_v1():
+    from typing import Any
+
+    from pydantic import GetCoreSchemaHandler
+    from pydantic_core import core_schema
+
+    def _get_pid_core_schema(
+        cls, _source_type: Any, _handler: GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_after_validator_function(
+            cls.parse,
+            core_schema.union_schema(
+                [core_schema.is_instance_schema(PID), core_schema.str_schema()]
+            ),
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                cls.__str__, info_arg=False, return_schema=core_schema.str_schema()
+            ),
+        )
+
 
 class PID:
     """Stores the ID of database item.
 
     The ID is split into a prefix and the main identifier.
     The prefix identifies an instance of SciCat and the main identifier a dataset.
 
@@ -102,31 +125,36 @@
 
     def __str__(self) -> str:
         if self.prefix is not None:
             return self.prefix + "/" + self.pid
         return self.pid
 
     def __repr__(self) -> str:
-        return f"PID(prefix={self.prefix}, pid={self.pid})"
+        return f"PID(prefix={self.prefix!r}, pid={self.pid!r})"
 
     def __hash__(self) -> int:
         return hash(str(self))
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, PID):
             return False
         return self.prefix == other.prefix and self.pid == other.pid
 
     @classmethod
-    def __get_validators__(
-        cls,
-    ) -> Generator[Callable[[Union[str, PID]], PID], None, None]:
-        yield cls.validate
-
-    @classmethod
     def validate(cls, value: Union[str, PID]) -> PID:
         """Pydantic validator for PID fields."""
         if isinstance(value, str):
             return PID.parse(value)
         if isinstance(value, PID):
             return value
-        raise TypeError("expected a PID or str")
+        raise pydantic.ValidationError("expected a PID or str")
+
+    if is_pydantic_v1():
+
+        @classmethod
+        def __get_validators__(
+            cls,
+        ) -> Generator[Callable[[Union[str, PID]], PID], None, None]:
+            yield cls.validate
+
+    else:
+        __get_pydantic_core_schema__ = classmethod(_get_pid_core_schema)
```

### Comparing `scitacean-23.5.0/src/scitacean/testing/client.py` & `scitacean-23.7.7/src/scitacean/testing/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Fake client for testing."""
 
 from __future__ import annotations
 
 import datetime
 import functools
-import uuid
 from copy import deepcopy
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from .. import model
 from ..client import Client, ScicatClient
 from ..error import ScicatCommError
 from ..pid import PID
 from ..typing import FileTransfer
 from ..util.credentials import StrStorage
@@ -35,50 +34,49 @@
     This class is a stand in for :class:`scitacean.Client` to emulate downloading and
     uploading of datasets without actually accessing a SciCat server.
 
     Since this client fakes communication with SciCat, it stores raw
     `pydantic <https://docs.pydantic.dev/>`_ models, namely
 
     - ``FakeClient.datasets``:
-            :class:`dict` of :class:`pydantic.model.DerivedDataset` and
-            :class:`pydantic.model.RawDataset`,
-            indexed by dataset ID.
+            :class:`dict` of :class:`scitacean.model.DownloadDataset`,
+            indexed by dataset PID.
     - ``FakeClient.orig_datablocks``:
-            :class:`dict` of lists of :class:`pydantic.model.OrigDatablock`,
+            :class:`dict` of lists of :class:`scitacean.model.OrigDatablock`,
             indexed by the *dataset* ID.
 
-    Individual functions can be disabled (that is made to raise an exception)
+    Individual functions can be disabled (that is, made to raise an exception)
     using the ``disabled`` argument of the initializer.
 
     Important
     ---------
     ``FakeClient`` does not behave exactly like a ``Client`` connected to a real
     server as that would require reimplementing a large part of the SciCat backend.
-    You should thus always test your code against a (potentially locally deployed)
+    You should thus always also test your code against a (potentially locally deployed)
     real server.
 
     In particular, do not rely on specific error messages or the detailed settings
     in the datasets returned by ``FakeClient.upload_new_dataset_now``!
 
     Examples
     --------
     Set up a fake client for download:
 
     .. code-block:: python
 
         client = FakeClient()
         pid = PID(prefix="sample.prefix", pid="1234-5678-abcd")
-        client.datasets[pid] = model.DerivedDataset(...)
+        client.datasets[pid] = model.DownloadDataset(pid=pid, ...)
         client.orig_datablocks[pid] = [model.OrigDatablock(
             datasetId=str(pid),
             ...
         )]
         client.get_dataset(pid)
 
-    Use to upload a dataset:
+    Upload a dataset:
 
     .. code-block:: python
 
         client = FakeClient(file_transfer=FakeFileTransfer())
         finalized = client.upload_new_dataset_now(dset)
 
         # contains new dataset and datablock:
@@ -110,22 +108,23 @@
 
         Parameters
         ----------
         file_transfer:
             Typically :class:`scitacean.testing.transfer.FakeFileTransfer`
             but may be a real file transfer.
         disable:
-            dict function names to exceptions. Functions listed here raise
-            the given exception when called and do nothing else.
+            ``dict`` of function names to exceptions.
+            Functions listed here raise the given exception
+            when called and do nothing else.
         """
         super().__init__(client=FakeScicatClient(self), file_transfer=file_transfer)
 
         self.disabled = {} if disable is None else dict(disable)
-        self.datasets: Dict[PID, Union[model.DerivedDataset, model.RawDataset]] = {}
-        self.orig_datablocks: Dict[PID, List[model.OrigDatablock]] = {}
+        self.datasets: Dict[PID, model.DownloadDataset] = {}
+        self.orig_datablocks: Dict[PID, List[model.DownloadOrigDatablock]] = {}
 
     @classmethod
     def from_token(
         cls,
         *,
         url: str,
         token: Union[str, StrStorage],
@@ -169,47 +168,129 @@
     def __init__(self, main_client: FakeClient) -> None:
         super().__init__(url="", token="", timeout=datetime.timedelta(seconds=60))
         self.main = main_client
 
     @_conditionally_disabled
     def get_dataset_model(
         self, pid: PID, strict_validation: bool = False
-    ) -> Union[model.DerivedDataset, model.RawDataset]:
+    ) -> model.DownloadDataset:
         _ = strict_validation  # unused by fake
         try:
             return self.main.datasets[pid]
         except KeyError:
             raise ScicatCommError(f"Unable to retrieve dataset {pid}") from None
 
     @_conditionally_disabled
     def get_orig_datablocks(
         self, pid: PID, strict_validation: bool = False
-    ) -> List[model.OrigDatablock]:
+    ) -> List[model.DownloadOrigDatablock]:  # TODO here and rest of classes
         _ = strict_validation  # unused by fake
         try:
             return self.main.orig_datablocks[pid]
         except KeyError:
             raise ScicatCommError(
                 f"Unable to retrieve orig datablock for dataset {pid}"
             ) from None
 
     @_conditionally_disabled
     def create_dataset_model(
-        self, dset: Union[model.DerivedDataset, model.RawDataset]
-    ) -> Union[model.DerivedDataset, model.RawDataset]:
-        pid = PID(
-            pid=str(dset.pid) if dset.pid is not None else str(uuid.uuid4()),
-            prefix="PID.SAMPLE.PREFIX",
-        )
-        if pid in self.main.datasets:
-            raise ScicatCommError(f"Dataset id already exists: {pid}")
-        self.main.datasets[pid] = deepcopy(dset)
-        self.main.datasets[pid].pid = pid
-        return self.main.datasets[pid]
+        self, dset: Union[model.UploadDerivedDataset, model.UploadRawDataset]
+    ) -> model.DownloadDataset:
+        ingested = _process_dataset(dset)
+        self.main.datasets[ingested.pid] = ingested
+        return ingested
 
     @_conditionally_disabled
-    def create_orig_datablock(self, dblock: model.OrigDatablock) -> model.OrigDatablock:
-        dataset_id = dblock.datasetId
+    def create_orig_datablock(
+        self, dblock: model.UploadOrigDatablock
+    ) -> model.DownloadOrigDatablock:
+        ingested = _process_orig_datablock(dblock)
+        dataset_id = ingested.datasetId
         if dataset_id not in self.main.datasets:
             raise ScicatCommError(f"No dataset with id {dataset_id}")
-        self.main.orig_datablocks.setdefault(dataset_id, []).append(dblock)
-        return dblock
+        self.main.orig_datablocks.setdefault(dataset_id, []).append(ingested)
+        return ingested
+
+
+def _model_dict(mod: model.BaseModel) -> Dict[str, Any]:
+    return {
+        key: deepcopy(val)
+        for key in mod.get_model_fields().keys()
+        if (val := getattr(mod, key)) is not None
+    }
+
+
+def _process_relationship(
+    relationship: model.UploadRelationship,
+) -> model.DownloadRelationship:
+    return model.DownloadRelationship(**_model_dict(relationship))
+
+
+def _process_technique(technique: model.UploadTechnique) -> model.DownloadTechnique:
+    return model.DownloadTechnique(**_model_dict(technique))
+
+
+def _process_data_file(file: model.UploadDataFile) -> model.DownloadDataFile:
+    return model.DownloadDataFile(**_model_dict(file))
+
+
+def _process_dataset(
+    dset: Union[model.UploadDerivedDataset, model.UploadRawDataset]
+) -> model.DownloadDataset:
+    created_at = datetime.datetime.now(tz=datetime.timezone.utc)
+    # TODO use user login if possible
+    # Using strict_validation=False because the input model should already be validated.
+    # If there are validation errors, it was probably intended by the user.
+    fields = _model_dict(dset)
+    if "relationships" in fields:
+        fields["relationships"] = list(
+            map(_process_relationship, fields["relationships"])
+        )
+    if "techniques" in fields:
+        fields["techniques"] = list(map(_process_technique, fields["techniques"]))
+    return model.construct(
+        model.DownloadDataset,
+        _strict_validation=False,
+        pid=PID.generate(prefix="PID.prefix.a0b1"),
+        createdBy="fake",
+        createdAt=created_at,
+        updatedBy="fake",
+        updatedAt=created_at,
+        **fields,
+    )
+
+
+def _process_orig_datablock(
+    dblock: model.UploadOrigDatablock,
+) -> model.DownloadOrigDatablock:
+    created_at = datetime.datetime.now(tz=datetime.timezone.utc)
+    # TODO use user login if possible
+    # TODO more fields
+    # Using strict_validation=False because the input model should already be validated.
+    # If there are validation errors, it was probably intended by the user.
+    fields = _model_dict(dblock)
+    if "dataFileList" in fields:
+        fields["dataFileList"] = list(map(_process_data_file, fields["dataFileList"]))
+    processed = model.construct(
+        model.DownloadOrigDatablock,
+        _strict_validation=False,
+        createdBy="fake",
+        createdAt=created_at,
+        updatedBy="fake",
+        updatedAt=created_at,
+        **fields,
+    )
+    if dblock.datasetId is not None:
+        processed.datasetId = dblock.datasetId
+    return processed
+
+
+def process_uploaded_dataset(
+    dataset: Union[model.UploadDerivedDataset, model.UploadRawDataset],
+    orig_datablocks: Optional[List[model.UploadOrigDatablock]],
+) -> Tuple[model.DownloadDataset, Optional[List[model.DownloadOrigDatablock]]]:
+    dblocks = (
+        list(map(_process_orig_datablock, orig_datablocks))
+        if orig_datablocks is not None
+        else None
+    )
+    return _process_dataset(dataset), dblocks
```

### Comparing `scitacean-23.5.0/src/scitacean/testing/docs.py` & `scitacean-23.7.7/src/scitacean/testing/docs.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 
 Should probably not be used externally.
 """
 
 from dateutil.parser import parse as parse_date
 
 from ..filesystem import RemotePath
-from ..model import DataFile, DatasetType, OrigDatablock, RawDataset
+from ..model import (
+    DatasetType,
+    DownloadDataFile,
+    DownloadDataset,
+    DownloadOrigDatablock,
+)
 from ..pid import PID
 from .client import FakeClient
 from .transfer import FakeFileTransfer
 
 
 def _add_file(client: FakeClient, name: str, content: bytes) -> None:
     client.file_transfer.files[name] = content  # type: ignore[union-attr]
@@ -22,51 +27,52 @@
     content2 = (
         b"INFO Starting measurement\nWARN Detector saturated\nINFO Measurement finished"
     )
     _add_file(client, "/hex/ps/thaum/flux.dat", content1)
     _add_file(client, "/hex/ps/thaum/logs/measurement.log", content2)
 
     dataset_id = PID(prefix="20.500.12269", pid="72fe3ff6-105b-4c7f-b9d0-073b67c90ec3")
-    client.datasets[dataset_id] = RawDataset(
+    client.datasets[dataset_id] = DownloadDataset(
         pid=dataset_id,
         datasetName="Thaum flux",
         description="Measured the thaum flux",
         createdBy="Ponder Stibbons",
         updatedBy="anonymous",
         updatedAt=parse_date("2022-11-01T13:22:08.927Z"),
         createdAt=parse_date("2022-08-17T14:20:23.675Z"),
         owner="Ponder Stibbons",
         ownerGroup="uu",
         accessGroups=["faculty"],
         principalInvestigator="p.stibbons@uu.am",
         contactEmail="p.stibbons@uu.am",
         creationTime=parse_date("2022-06-29T14:01:05.000Z"),
+        creationLocation="UnseenUniversity",
         numberOfFiles=2,
         size=len(content1) + len(content2),
         sourceFolder=RemotePath("/hex/ps/thaum"),
         scientificMetadata={
             "data_type": "histogram",
             "temperature": {"value": "123", "unit": "K"},
         },
         type=DatasetType.RAW,
     )
     client.orig_datablocks[dataset_id] = [
-        OrigDatablock(
+        DownloadOrigDatablock(
             id=PID(prefix="20.500.12269", pid="02dc390c-811c-4d6a-93bf-9f85a4214ca0"),
             datasetId=dataset_id,
             size=len(content1) + len(content2),
             ownerGroup="uu",
             accessGroups=["faculty"],
             dataFileList=[
-                DataFile(
+                DownloadDataFile(
                     path="flux.dat",
                     size=len(content1),
                     time=parse_date("2022-08-17T13:54:12Z"),
                 ),
-                DataFile(
+                DownloadDataFile(
                     path="logs/measurement.log",
                     size=len(content2),
                     time=parse_date("2022-08-17T13:55:21Z"),
                 ),
             ],
         )
     ]
```

### Comparing `scitacean-23.5.0/src/scitacean/testing/transfer.py` & `scitacean-23.7.7/src/scitacean/testing/transfer.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/transfer/ssh.py` & `scitacean-23.7.7/src/scitacean/transfer/ssh.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/transfer/util.py` & `scitacean-23.7.7/src/scitacean/transfer/util.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/typing.py` & `scitacean-23.7.7/src/scitacean/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 
+"""Definitions for type checking."""
+
 from pathlib import Path
 from typing import ContextManager, List, Protocol
 
 from .dataset import Dataset
 from .file import File
 from .filesystem import RemotePath
```

### Comparing `scitacean-23.5.0/src/scitacean/util/credentials.py` & `scitacean-23.7.7/src/scitacean/util/credentials.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/src/scitacean/util/formatter.py` & `scitacean-23.7.7/src/scitacean/util/formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
         formatter = DatasetPathFormatter()
         formatter.format("a string {owner}", dset=dset)
         # is equivalent to
         "a string {}".format(escape_path("{dset.owner}".format(dset=dset)))
 
     Note that only formatted fields are escaped, not the result as a whole.
+
+    Fields that are used by the formatter must not be ``None``.
+    Otherwise, a :class:`ValueError` will be raised.
     """
 
     def parse(
         self, format_string: str
     ) -> Iterator[Tuple[str, Optional[str], Optional[str], Optional[str]]]:
         def add0(field_name: Optional[str]) -> Optional[str]:
             if field_name == "uid":
@@ -49,8 +52,10 @@
             return None
 
         return map(
             lambda t: (t[0], add0(t[1]), t[2], t[3]), super().parse(format_string)
         )
 
     def format_field(self, value: Any, format_spec: str) -> str:
+        if value is None:
+            raise ValueError("Cannot format path, dataset field is None")
         return escape_path(super().format_field(value, format_spec))
```

### Comparing `scitacean-23.5.0/src/scitacean.egg-info/PKG-INFO` & `scitacean-23.7.7/src/scitacean.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 23.5.0
+Version: 23.7.7
 Summary: High-level interface for SciCat
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -47,14 +47,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ssh
+Provides-Extra: test
 License-File: LICENSE
 
 [![PyPI badge](https://img.shields.io/pypi/v/scitacean.svg?style=flat-square&color=green)](https://pypi.python.org/pypi/scitacean)
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/scitacean?style=flat-square&color=green)](https://anaconda.org/conda-forge/scitacean)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7520487.svg)](https://doi.org/10.5281/zenodo.7520487)
 [![License: BSD 3-Clause](https://img.shields.io/github/license/SciCatProject/scitacean?style=flat-square&color=yellowgreen)](LICENSE)
```

### Comparing `scitacean-23.5.0/src/scitacean.egg-info/SOURCES.txt` & `scitacean-23.7.7/src/scitacean.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .gitignore
-.gitmodules
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 SECURITY.md
 pyproject.toml
@@ -21,15 +20,15 @@
 docs/release-notes.rst
 docs/_static/anaconda-logo.svg
 docs/_static/favicon.ico
 docs/_static/logo-dark.svg
 docs/_static/logo.svg
 docs/_static/css/custom.css
 docs/_templates/scitacean-class-template.rst
-docs/_templates/scitacean-dataclass-template.rst
+docs/_templates/scitacean-module-template.rst
 docs/developer/coding-conventions.rst
 docs/developer/dependency-management.rst
 docs/developer/getting-started.rst
 docs/developer/index.rst
 docs/developer/testing.rst
 docs/reference/index.rst
 docs/user-guide/downloading.ipynb
@@ -47,15 +46,18 @@
 requirements/docs.txt
 requirements/static.in
 requirements/static.txt
 requirements/test.in
 requirements/test.txt
 requirements/wheels.in
 requirements/wheels.txt
+requirements-pydantic2/base.in
+requirements-pydantic2/test.in
 src/scitacean/__init__.py
+src/scitacean/_base_model.py
 src/scitacean/_dataset_fields.py
 src/scitacean/client.py
 src/scitacean/datablock.py
 src/scitacean/dataset.py
 src/scitacean/error.py
 src/scitacean/file.py
 src/scitacean/filesystem.py
@@ -77,20 +79,39 @@
 src/scitacean/_html_repr/styles/dataset.css
 src/scitacean/_html_repr/templates/__init__.py
 src/scitacean/_html_repr/templates/dataset_field_repr.html.template
 src/scitacean/_html_repr/templates/dataset_repr.html.template
 src/scitacean/_html_repr/templates/files_repr.html.template
 src/scitacean/_html_repr/templates/metadata_repr.html.template
 src/scitacean/_internal/__init__.py
+src/scitacean/_internal/dataclass_wrapper.py
+src/scitacean/_internal/docker.py
+src/scitacean/_internal/file_counter.py
 src/scitacean/_internal/orcid.py
+src/scitacean/_internal/pydantic_compat.py
 src/scitacean/testing/__init__.py
+src/scitacean/testing/_pytest_helpers.py
 src/scitacean/testing/client.py
 src/scitacean/testing/docs.py
 src/scitacean/testing/strategies.py
 src/scitacean/testing/transfer.py
+src/scitacean/testing/backend/__init__.py
+src/scitacean/testing/backend/_backend.py
+src/scitacean/testing/backend/_pytest_helpers.py
+src/scitacean/testing/backend/config.py
+src/scitacean/testing/backend/docker-compose-backend-template.yaml
+src/scitacean/testing/backend/fixtures.py
+src/scitacean/testing/backend/seed.py
+src/scitacean/testing/ssh/__init__.py
+src/scitacean/testing/ssh/_pytest_helpers.py
+src/scitacean/testing/ssh/_ssh.py
+src/scitacean/testing/ssh/docker-compose-ssh-server.yaml
+src/scitacean/testing/ssh/fixtures.py
+src/scitacean/testing/ssh/ssh_server_seed/table.csv
+src/scitacean/testing/ssh/ssh_server_seed/text.txt
 src/scitacean/transfer/__init__.py
 src/scitacean/transfer/ssh.py
 src/scitacean/transfer/util.py
 src/scitacean/util/__init__.py
 src/scitacean/util/credentials.py
 src/scitacean/util/formatter.py
 tests/__init__.py
@@ -100,42 +121,28 @@
 tests/dataset_test.py
 tests/download_test.py
 tests/file_test.py
 tests/filesystem_test.py
 tests/model_test.py
 tests/upload_test.py
 tests/common/__init__.py
-tests/common/backend.py
-tests/common/docker-compose-ssh-server.yaml
-tests/common/docker.py
 tests/common/files.py
-tests/common/ssh_server.py
-tests/common/data/ssh_server_seed/table.csv
-tests/common/data/ssh_server_seed/text.txt
-tests/data/__init__.py
-tests/data/datasets.json
-tests/data/orig_datablocks.json
 tests/html_repr/__init__.py
 tests/html_repr/html_repr_test.py
 tests/testing/__init__.py
 tests/testing/strategies_test.py
 tests/transfer/__init__.py
 tests/transfer/ssh_test.py
 tests/util/__init__.py
 tests/util/formatter_test.py
-tools/model-generation/dataset.py
-tools/model-generation/generate.py
-tools/model-generation/model.py
-tools/model-generation/util.py
+tools/model-generation/README.md
+tools/model-generation/generate_models.py
 tools/model-generation/spec/__init__.py
-tools/model-generation/spec/data-file.yml
-tools/model-generation/spec/datablock.yml
-tools/model-generation/spec/dataset-lifecycle.yml
-tools/model-generation/spec/dataset.yml
-tools/model-generation/spec/mongo-queryable.yml
-tools/model-generation/spec/orig-datablock.yml
-tools/model-generation/spec/ownable.yml
-tools/model-generation/spec/technique.yml
+tools/model-generation/spec/dataset-fields.yml
+tools/model-generation/spec/field-name-overrides.yml
+tools/model-generation/spec/field-type-overrides.yml
+tools/model-generation/spec/field-validations.yml
+tools/model-generation/spec/masked-fields.yml
+tools/model-generation/spec/schema.py
 tools/model-generation/templates/__init__.py
-tools/model-generation/templates/dataset.py.template
-tools/model-generation/templates/field_spec.py.template
-tools/model-generation/templates/model.py.template
+tools/model-generation/templates/dataset_fields.py.jinja
+tools/model-generation/templates/model.py.jinja
```

### Comparing `scitacean-23.5.0/tests/client_test.py` & `scitacean-23.7.7/tests/client_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 import pickle
-from copy import deepcopy
 
 import pydantic
 import pytest
 from dateutil.parser import parse as parse_date
 
-from scitacean import PID, Client, ScicatCommError
-from scitacean.model import DataFile, DatasetType, DerivedDataset, OrigDatablock
+from scitacean import PID, Client, RemotePath, ScicatCommError
+from scitacean.client import ScicatClient
+from scitacean.model import (
+    DatasetType,
+    UploadDataFile,
+    UploadDerivedDataset,
+    UploadOrigDatablock,
+)
+from scitacean.testing.backend.seed import INITIAL_DATASETS, INITIAL_ORIG_DATABLOCKS
 from scitacean.testing.client import FakeClient
 from scitacean.util.credentials import SecretStr
 
-from . import data
-from .common.backend import skip_if_not_backend
 
-
-@pytest.fixture
-def derived_dataset():
-    return data.as_dataset_model(data.load_datasets()[0])
-
-
-@pytest.fixture
-def orig_datablock():
-    return data.as_orig_datablock_model(data.load_orig_datablocks()[0])
-
-
-def make_fake_client(dataset, datablock):
-    client = FakeClient(file_transfer=None)
-    client.datasets[dataset.pid] = dataset
-    client.orig_datablocks[dataset.pid] = [datablock]
-    return client
+@pytest.fixture()
+def scicat_client(client) -> ScicatClient:
+    return client.scicat
 
 
-@pytest.fixture(params=["real", "fake"])
-def client(
-    request,
-    derived_dataset,
-    orig_datablock,
-    scicat_access,
-    scicat_backend,
-):
-    if request.param == "fake":
-        return make_fake_client(derived_dataset, orig_datablock)
-    if request.param == "real":
-        skip_if_not_backend(request)
-        return Client.from_credentials(
-            url=scicat_access.url, **scicat_access.functional_credentials
-        )
+@pytest.fixture()
+def derived_dataset(scicat_access):
+    return UploadDerivedDataset(
+        contactEmail="black.foess@dom.koelle",
+        creationTime=parse_date("1995-11-11T11:11:11.000Z"),
+        owner="bfoess",
+        investigator="b.foess@dom.koelle",
+        sourceFolder="/dom/platt",
+        type=DatasetType.DERIVED,
+        inputDatasets=[],
+        usedSoftware=[],
+        ownerGroup=scicat_access.user.group,
+        accessGroups=["koelle"],
+        numberOfFilesArchived=0,
+    )
 
 
-@pytest.fixture
-def scicat_client(client):
-    return client.scicat
+@pytest.fixture()
+def orig_datablock(scicat_access):
+    # NOTE the placeholder!
+    return UploadOrigDatablock(
+        size=9235,
+        dataFileList=[
+            UploadDataFile(
+                path="data.nxs", size=9235, time=parse_date("2023-08-18T13:52:33.000Z")
+            )
+        ],
+        datasetId="PLACEHOLDER",
+        ownerGroup="uu",
+        accessGroups=["group1", "2nd_group"],
+    )
 
 
 def test_from_token_fake():
     # This should not call the API
     client = FakeClient.from_token(url="some.url/api/v3", token="a-token")  # noqa: S106
     assert isinstance(client, FakeClient)
 
@@ -73,188 +75,152 @@
         FakeClient,
     )
 
 
 def test_from_credentials_real(scicat_access, scicat_backend):
     if not scicat_backend:
         pytest.skip("No backend")
-    Client.from_credentials(
-        url=scicat_access.url, **scicat_access.functional_credentials
-    )
+    Client.from_credentials(url=scicat_access.url, **scicat_access.user.credentials)
 
 
-def test_get_dataset_model(scicat_client, derived_dataset):
-    dset = scicat_client.get_dataset_model(derived_dataset.pid)
-    assert dset == derived_dataset
+@pytest.mark.parametrize("key", ("raw", "derived"))
+def test_get_dataset_model(scicat_client, key):
+    dset = INITIAL_DATASETS[key]
+    downloaded = scicat_client.get_dataset_model(dset.pid)
+    assert downloaded == dset
 
 
 def test_get_dataset_model_bad_id(scicat_client):
     with pytest.raises(ScicatCommError):
-        scicat_client.get_dataset_model("bad-pid")
+        scicat_client.get_dataset_model(PID(pid="bad-pid"))
 
 
-def test_get_orig_datablock(scicat_client, orig_datablock):
-    dblock = scicat_client.get_orig_datablocks(orig_datablock.datasetId)
-    assert [orig_datablock] == dblock
+@pytest.mark.parametrize("key", ("raw", "derived"))
+def test_get_orig_datablock(scicat_client, key):
+    dblock = INITIAL_ORIG_DATABLOCKS[key][0]
+    downloaded = scicat_client.get_orig_datablocks(dblock.datasetId)
+    assert downloaded == [dblock]
 
 
 def test_get_orig_datablock_bad_id(scicat_client):
     with pytest.raises(ScicatCommError):
-        scicat_client.get_orig_datablocks("bollocks")
+        scicat_client.get_orig_datablocks(PID(pid="bollocks"))
 
 
-@pytest.mark.parametrize("pid", ("PID.SAMPLE.PREFIX/jeck", "kamelle", None))
-def test_create_dataset_model(pid, scicat_client):
-    dset = DerivedDataset(
-        pid=pid,
-        contactEmail="black.foess@dom.koelle",
-        creationTime=parse_date("1995-11-11T11:11:11.000Z"),
-        owner="bfoess",
-        investigator="b.foess@dom.koelle",
-        sourceFolder="/dom/platt",
-        type=DatasetType.DERIVED,
-        inputDatasets=[],
-        usedSoftware=[],
-        ownerGroup="bfoess",
-        accessGroups=["koelle"],
-    )
-    finalized = scicat_client.create_dataset_model(dset)
+def test_create_dataset_model(scicat_client, derived_dataset):
+    finalized = scicat_client.create_dataset_model(derived_dataset)
     downloaded = scicat_client.get_dataset_model(finalized.pid)
-    for key, expected in finalized.dict(exclude_none=True).items():
+    for key, expected in finalized:
         # The database populates a number of fields that are None in dset.
         # But we don't want to test those here as we don't want to test the database.
-        assert expected == downloaded.dict(exclude_none=True)[key], f"key = {key}"
+        if expected is not None:
+            assert expected == dict(downloaded)[key], f"key = {key}"
 
 
-def test_create_dataset_model_id_clash(scicat_client, derived_dataset):
-    dset = deepcopy(derived_dataset)
-    dset.pid = PID(prefix=None, pid=dset.pid.pid)
-    dset.owner = "a new owner to trigger a failure"
-    with pytest.raises(ScicatCommError):
-        scicat_client.create_dataset_model(dset)
-
-
-def test_create_first_orig_datablock(scicat_client, derived_dataset):
-    dset = deepcopy(derived_dataset)
-    dset.pid = PID(pid="new-dataset-id")
-    uploaded = scicat_client.create_dataset_model(dset)
-
-    dblock = OrigDatablock(
-        id=PID(prefix="PID.SAMPLE.PREFIX", pid="new-datablock-id"),
-        size=9235,
-        dataFileList=[
-            DataFile(
-                path="data.nxs", size=9235, time=parse_date("2023-08-18T13:52:33.000Z")
-            )
-        ],
-        datasetId=uploaded.pid,
-        ownerGroup="uu",
-        accessGroups=["group1", "2nd_group"],
-    )
-    scicat_client.create_orig_datablock(dblock)
+def test_create_first_orig_datablock(scicat_client, derived_dataset, orig_datablock):
+    uploaded = scicat_client.create_dataset_model(derived_dataset)
+    orig_datablock.datasetId = uploaded.pid
+    scicat_client.create_orig_datablock(orig_datablock)
     downloaded = scicat_client.get_orig_datablocks(uploaded.pid)
     assert len(downloaded) == 1
     downloaded = downloaded[0]
-    for key, expected in dblock.dict(exclude_none=True).items():
+    for key, expected in orig_datablock:
         # The database populates a number of fields that are None in dset.
         # But we don't want to test those here as we don't want to test the database.
-        if key != "dataFileList":
-            assert expected == downloaded.dict()[key], f"key = {key}"
-    for i in range(len(dblock.dataFileList)):
-        for key, expected in dblock.dataFileList[i].dict(exclude_none=True).items():
+        if expected is not None and key != "dataFileList":
+            assert expected == dict(downloaded)[key], f"key = {key}"
+    for i in range(len(orig_datablock.dataFileList)):
+        for key, expected in orig_datablock.dataFileList[i]:
             assert (
-                expected == downloaded.dataFileList[i].dict()[key]
+                expected == dict(downloaded.dataFileList[i])[key]
             ), f"i = {i}, key = {key}"
 
 
-def test_get_dataset(client, derived_dataset, orig_datablock):
-    dset = client.get_dataset(derived_dataset.pid)
-
-    assert dset.source_folder == derived_dataset.sourceFolder
-    assert dset.creation_time == derived_dataset.creationTime
-    assert dset.access_groups == derived_dataset.accessGroups
-    assert dset.meta["temperature"] == derived_dataset.scientificMetadata["temperature"]
-    assert dset.meta["data_type"] == derived_dataset.scientificMetadata["data_type"]
+def test_get_dataset(client):
+    dset = INITIAL_DATASETS["raw"]
+    dblock = INITIAL_ORIG_DATABLOCKS["raw"][0]
+    downloaded = client.get_dataset(dset.pid)
+
+    assert downloaded.source_folder == dset.sourceFolder
+    assert downloaded.creation_time == dset.creationTime
+    assert downloaded.access_groups == dset.accessGroups
+    assert downloaded.meta["temperature"] == dset.scientificMetadata["temperature"]
+    assert downloaded.meta["data_type"] == dset.scientificMetadata["data_type"]
 
-    for dset_file, expected_file in zip(dset.files, orig_datablock.dataFileList):
+    for dset_file, expected_file in zip(downloaded.files, dblock.dataFileList):
         assert dset_file.local_path is None
         assert dset_file.size == expected_file.size
         assert dset_file.creation_time == expected_file.time
 
 
-def test_fake_can_disable_functions():
-    client = FakeClient(
-        disable={
-            "get_dataset_model": RuntimeError("custom failure"),
-            "get_orig_datablocks": IndexError("custom index error"),
-        }
-    )
-    with pytest.raises(RuntimeError, match="custom failure"):
-        client.scicat.get_dataset_model(PID(pid="some-pid"))
-    with pytest.raises(IndexError, match="custom index error"):
-        client.scicat.get_orig_datablocks(PID(pid="some-pid"))
+def test_can_get_public_dataset_without_login(require_scicat_backend, scicat_access):
+    client = Client.without_login(url=scicat_access.url)
 
+    dset = INITIAL_DATASETS["public"]
+    dblock = INITIAL_ORIG_DATABLOCKS["public"][0]
+    downloaded = client.get_dataset(dset.pid)
+
+    assert downloaded.source_folder == dset.sourceFolder
+    assert downloaded.creation_time == dset.creationTime
+    assert downloaded.access_groups == dset.accessGroups
 
-def test_can_get_public_dataset_without_login(request, scicat_access, scicat_backend):
-    skip_if_not_backend(request)
-    client = Client.without_login(url=scicat_access.url)
-    dset = client.get_dataset("PID.SAMPLE.PREFIX/public-dataset")
-    assert dset.type == DatasetType.RAW
-    assert dset.owner == "librarian"
-    assert dset.creation_time == parse_date("2022-11-25T22:12:04.512Z")
-    assert dset.number_of_files == 0
+    for dset_file, expected_file in zip(downloaded.files, dblock.dataFileList):
+        assert dset_file.local_path is None
+        assert dset_file.size == expected_file.size
+        assert dset_file.creation_time == expected_file.time
 
 
 def test_cannot_upload_without_login(
-    request, derived_dataset, scicat_access, scicat_backend
+    require_scicat_backend, derived_dataset, scicat_access
 ):
-    skip_if_not_backend(request)
     client = Client.without_login(url=scicat_access.url)
-    derived_dataset.pid = None
-    with pytest.raises(ScicatCommError):
+    with pytest.raises(ScicatCommError):  # TODO test return code 403
         client.scicat.create_dataset_model(derived_dataset)
 
 
-def test_get_broken_dataset(request, scicat_access, scicat_backend):
-    skip_if_not_backend(request)
-    client = Client.without_login(url=scicat_access.url)
-    dset = client.get_dataset("PID.SAMPLE.PREFIX/partially-broken")
-    assert dset.type == DatasetType.RAW
-    # Intact field; was not converted to RemotePath
-    assert isinstance(dset.source_folder, str)
-    assert dset.source_folder == "/remote/source"
+def test_get_broken_dataset(client):
+    dset = INITIAL_DATASETS["partially-broken"]
+    downloaded = client.get_dataset(dset.pid)
+    assert downloaded.type == DatasetType.DERIVED
+    # Intact field; was properly converted to RemotePath
+    assert isinstance(downloaded.source_folder, RemotePath)
+    assert downloaded.source_folder == "/remote/source"
 
     # Broken fields loaded
-    assert isinstance(dset.end_time, str)
-    assert dset.end_time == "yesterday"
+    assert isinstance(downloaded.orcid_of_owner, str)
+    assert downloaded.orcid_of_owner == "00-11-22-33"
 
+    # Ignored broken fields
+    assert isinstance(downloaded.number_of_files, int)
+    assert downloaded.number_of_files == 0
+    assert isinstance(downloaded.size, int)
+    assert downloaded.size == 0
 
-def test_get_broken_dataset_strict_validation(request, scicat_access, scicat_backend):
-    skip_if_not_backend(request)
-    client = Client.without_login(url=scicat_access.url)
+
+def test_get_broken_dataset_strict_validation(real_client, require_scicat_backend):
+    dset = INITIAL_DATASETS["partially-broken"]
     with pytest.raises(pydantic.ValidationError):
-        client.get_dataset("PID.SAMPLE.PREFIX/partially-broken", strict_validation=True)
+        real_client.get_dataset(dset.pid, strict_validation=True)
 
 
 def test_cannot_pickle_client_credentials_manual_token_str():
     client = Client.from_token(url="/", token="the-token")  # noqa: S106
     with pytest.raises(TypeError):
         pickle.dumps(client)
 
 
 def test_cannot_pickle_client_credentials_manual_token_secret_str():
     client = Client.from_token(url="/", token=SecretStr("the-token"))
     with pytest.raises(TypeError):
         pickle.dumps(client)
 
 
-def test_cannot_pickle_client_credentials_login(request, scicat_access, scicat_backend):
-    skip_if_not_backend(request)
+def test_cannot_pickle_client_credentials_login(scicat_access, require_scicat_backend):
     client = Client.from_credentials(
-        url=scicat_access.url, **scicat_access.functional_credentials
+        url=scicat_access.url, **scicat_access.user.credentials
     )
     with pytest.raises(TypeError):
         pickle.dumps(client)
 
 
 def test_connection_error_does_not_contain_token():
     client = Client.from_token(
@@ -264,7 +230,20 @@
     try:
         client.get_dataset("does not exist")
         assert False, "There must be an exception"  # noqa: B011
     except Exception as exc:
         assert "the token/which_must-be.kept secret" not in str(exc)
         for arg in exc.args:
             assert "the token/which_must-be.kept secret" not in str(arg)
+
+
+def test_fake_can_disable_functions():
+    client = FakeClient(
+        disable={
+            "get_dataset_model": RuntimeError("custom failure"),
+            "get_orig_datablocks": IndexError("custom index error"),
+        }
+    )
+    with pytest.raises(RuntimeError, match="custom failure"):
+        client.scicat.get_dataset_model(PID(pid="some-pid"))
+    with pytest.raises(IndexError, match="custom index error"):
+        client.scicat.get_orig_datablocks(PID(pid="some-pid"))
```

### Comparing `scitacean-23.5.0/tests/common/backend.py` & `scitacean-23.7.7/src/scitacean/testing/backend/_backend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,110 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
-import json
-import shutil
-import tempfile
+import importlib.resources
+import os
 import time
-from dataclasses import dataclass
-from pathlib import Path
-from typing import Dict, Union
+from copy import deepcopy
+from typing import Any, Union
 from urllib.parse import urljoin
 
-import pytest
 import requests
+import yaml
 
-from ..data import load_datasets, load_orig_datablocks
-from .docker import docker_compose
+from ..._internal.docker import docker_compose_down, docker_compose_up
+from . import config
 
-_TEST_BASE = Path(__file__).resolve().parent.parent
-_SCICAT_DOCKER_CONFIG = _TEST_BASE / "scicatlive/docker-compose.yaml"
-_SCICAT_DATASET_SEED_FILE = Path("seed_db/seed/Dataset.json")
-_SCICAT_ORIG_DATABLOCK_SEED_FILE = Path("seed_db/seed/OrigDatablock.json")
+_PathLike = Union[str, os.PathLike]
 
-_COMMAND_LINE_OPTION = "--backend-tests"
 
-# List of required services for tests.
-# We only need the backend and API to run tests.
-_SERVICES = ("catamel", "mongodb", "mongodb_seed", "reverse-proxy")
+def _read_yaml(filename: str) -> Any:
+    if hasattr(importlib.resources, "files"):
+        # Use new API added in Python 3.9
+        return yaml.safe_load(
+            importlib.resources.files("scitacean.testing.backend")
+            .joinpath(filename)
+            .read_text()
+        )
+    # Old API, deprecated as of Python 3.11
+    return yaml.safe_load(
+        importlib.resources.read_text("scitacean.testing.backend", filename)
+    )
 
 
-@dataclass
-class SciCatAccess:
-    url: str
-    functional_credentials: Dict[str, str]
+def _docker_compose_template() -> dict:
+    return _read_yaml("docker-compose-backend-template.yaml")
 
 
-@pytest.fixture(scope="session")
-def scicat_access():
-    return SciCatAccess(
-        url="http://localhost/api/v3/",
-        functional_credentials={"username": "ingestor", "password": "aman"},
-    )
+def _apply_config(template: dict) -> dict:
+    res = deepcopy(template)
+    scicat = res["services"]["scicat"]
+    ports = scicat["ports"][0].split(":")
+    scicat["ports"] = [f"{ports[0]}:{config.SCICAT_PORT}"]
 
+    env = scicat["environment"]
+    env["PORT"] = config.SCICAT_PORT
+    env["PID_PREFIX"] = config.PID_PREFIX
+    env["SITE"] = config.SITE
 
-@pytest.fixture(scope="session")
-def scicat_backend(request, scicat_access):
-    """Spin up a SciCat backend and API.
+    return res
 
-    Does nothing unless the --backend-tests command line option is set.
-    """
-    if not request.config.getoption(_COMMAND_LINE_OPTION):
-        yield False
-        return
-
-    with tempfile.TemporaryDirectory() as temp_dir:
-        config_file = configure(temp_dir)
-        with docker_compose(config_file, *_SERVICES):
-            wait_until_backend_is_live(scicat_access, max_time=20, n_tries=20)
-            yield True
-
-
-def can_connect(scicat_access: SciCatAccess) -> bool:
-    response = requests.post(
-        urljoin(scicat_access.url, "Users/login"),
-        json=scicat_access.functional_credentials,
-        timeout=0.5,
-    )
-    return response.ok
 
+def configure(target_path: _PathLike) -> None:
+    """Build a docker-compose file for the testing backend."""
+    c = yaml.dump(_apply_config(_docker_compose_template()))
+    if "PLACEHOLDER" in c:
+        raise RuntimeError("Incorrect config")
 
-def wait_until_backend_is_live(
-    scicat_access: SciCatAccess, max_time: float, n_tries: int
-):
-    # The containers take a while to be fully live.
-    for _ in range(n_tries):
-        if can_connect(scicat_access):
-            return
-        time.sleep(max_time / n_tries)
-    if not can_connect(scicat_access):
-        raise RuntimeError("Cannot connect to backend")
+    with open(target_path, "w") as f:
+        f.write(c)
 
 
-def _merge_seed_file(
-    target_dir: Path, seed_file_name: Union[str, Path], custom_seed: Union[list, dict]
-):
-    with open(target_dir / seed_file_name, "r") as f:
-        dset_seed = json.load(f)
-    dset_seed.extend(custom_seed)
-    with open(target_dir / seed_file_name, "w") as f:
-        json.dump(dset_seed, f)
+def start_backend(docker_compose_file: _PathLike) -> None:
+    """Start the docker container with SciCat backend."""
+    docker_compose_up(docker_compose_file)
 
 
-def configure(target_dir: Path) -> Path:
-    target = Path(target_dir) / "scicatlive"
-    shutil.copytree(
-        _SCICAT_DOCKER_CONFIG.parent, target, ignore=shutil.ignore_patterns(".git")
-    )
-    _merge_seed_file(target, _SCICAT_DATASET_SEED_FILE, load_datasets())
-    _merge_seed_file(target, _SCICAT_ORIG_DATABLOCK_SEED_FILE, load_orig_datablocks())
+def stop_backend(docker_compose_file: _PathLike) -> None:
+    """Stop the docker container with SciCat backend and remove volumes."""
+    docker_compose_down(docker_compose_file)
 
-    return target / _SCICAT_DOCKER_CONFIG.name
 
-
-def skip_if_not_backend(request):
-    if not request.config.getoption(_COMMAND_LINE_OPTION):
-        # The backend only exists if this option is set.
-        pytest.skip(
-            "Tests against a real backend are disabled, "
-            f"use {_COMMAND_LINE_OPTION} to enable them"
+def can_connect() -> bool:
+    """Test the connection to the testing SciCat backend."""
+    scicat_access = config.local_access("user1")
+    try:
+        response = requests.post(
+            urljoin(scicat_access.url, "Users/login"),
+            json=scicat_access.user.credentials,
+            timeout=0.5,
         )
+    except requests.ConnectionError:
+        return False
+    return response.ok
+
+
+def wait_until_backend_is_live(max_time: float, n_tries: int) -> None:
+    """Sleep until a connection to the backend can be made.
+
+    The backend takes a few seconds to become usable after the
+    docker container was started.
+    This function attempts to connect periodically until the connection
+    succeeds or ``max_time`` is reached.
+
+    Parameters
+    ----------
+    max_time:
+        Maximum time in seconds to wait for the backend to become usable.
+    n_tries:
+        Number of connection attempts within ``max_time``.
+
+    Raises
+    ------
+    RuntimeError
+        If no connection can be made within the time limit.
+    """
+    for _ in range(n_tries):
+        if can_connect():
+            return
+        time.sleep(max_time / n_tries)
+    if not can_connect():
+        raise RuntimeError("Cannot connect to backend")
```

### Comparing `scitacean-23.5.0/tests/common/docker-compose-ssh-server.yaml` & `scitacean-23.7.7/src/scitacean/testing/ssh/docker-compose-ssh-server.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 version: "2.1"
 services:
   scitacean-test-ssh-server:
     image: linuxserver/openssh-server:latest
-    container_name: openssh-server
+    container_name: scitacean-test-ssh
     hostname: scitacean-test-ssh-server
     environment:
       - PUID=1000
       - PGID=1000
       - TZ=CET  # Not UTC on purpose to test timezone detection
 #      - PUBLIC_KEY=yourpublickey #optional
 #      - PUBLIC_KEY_FILE=/path/to/file #optional
 #      - PUBLIC_KEY_DIR=/path/to/directory/containing/_only_/pubkeys #optional
 #      - PUBLIC_KEY_URL=https://github.com/username.keys #optional
       - SUDO_ACCESS=false
       - PASSWORD_ACCESS=true
       - USER_NAME=the-scitacean
       - USER_PASSWORD=sup3r-str0ng
-    volumes:
+    volumes: # configured in Python
       - ${DATA_DIR}:/data
       - ${SEED_DIR}:/data/seed
     ports:
       - "2222:2222"
     restart: unless-stopped
```

### Comparing `scitacean-23.5.0/tests/common/files.py` & `scitacean-23.7.7/tests/common/files.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/tests/dataset_fields_test.py` & `scitacean-23.7.7/tests/dataset_fields_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,20 +5,30 @@
 # public interface and make sure that Dataset does not break any behavior.
 
 from datetime import datetime, timedelta, timezone
 
 import dateutil.parser
 import pydantic
 import pytest
-from hypothesis import given, settings
+from hypothesis import assume, given, settings
 from hypothesis import strategies as st
 
 from scitacean import PID, Dataset, DatasetType
 from scitacean.filesystem import RemotePath
-from scitacean.model import DataFile, DerivedDataset, OrigDatablock, RawDataset
+from scitacean.model import (
+    DownloadDataFile,
+    DownloadDataset,
+    DownloadOrigDatablock,
+    UploadDerivedDataset,
+    UploadRawDataset,
+)
+
+# Fields whose types are not supported by hypothesis.
+# E.g. because they contain `Any`.
+_UNGENERATABLE_FIELDS = ("job_parameters", "meta")
 
 
 def test_init_dataset_with_only_type():
     dset = Dataset(type="raw")
     assert dset.type == DatasetType.RAW
 
 
@@ -61,137 +71,147 @@
 
     dset = Dataset(type="derived", creation_time="now")
     assert abs(dset.creation_time - datetime.now(tz=timezone.utc)) < timedelta(
         seconds=30
     )
 
 
-def test_init_dataset_default_values():
-    dset = Dataset(type="derived")
-    assert dset.history is None
-    assert dset.is_published is False
-    assert dset.meta == {}
-
-
 @pytest.mark.parametrize("field", Dataset.fields(read_only=True), ids=lambda f: f.name)
 def test_cannot_set_read_only_fields(field):
     dset = Dataset(type="raw")
     with pytest.raises(AttributeError):
         setattr(dset, field.name, None)
 
 
 @pytest.mark.parametrize(
     "field",
-    filter(lambda f: f.name != "type", Dataset.fields(read_only=False)),
+    filter(
+        lambda f: f.name not in ("type", *_UNGENERATABLE_FIELDS),
+        Dataset.fields(read_only=False),
+    ),
     ids=lambda f: f.name,
 )
 @given(st.data())
 @settings(max_examples=10)
 def test_can_init_writable_fields(field, data):
     value = data.draw(st.from_type(field.type))
     dset = Dataset(type="raw", **{field.name: value})
     assert getattr(dset, field.name) == value
 
 
-@pytest.mark.parametrize("field", Dataset.fields(read_only=False), ids=lambda f: f.name)
+@pytest.mark.parametrize(
+    "field",
+    filter(
+        lambda f: f.name not in _UNGENERATABLE_FIELDS, Dataset.fields(read_only=False)
+    ),
+    ids=lambda f: f.name,
+)
 @given(st.data())
 @settings(max_examples=10)
 def test_can_set_writable_fields(field, data):
     value = data.draw(st.from_type(field.type))
     dset = Dataset(type="raw")
     setattr(dset, field.name, value)
     assert getattr(dset, field.name) == value
 
 
 @pytest.mark.parametrize(
     "field",
-    filter(lambda f: not f.read_only and f.name != "creation_time", Dataset.fields()),
+    filter(lambda f: not f.read_only, Dataset.fields()),
     ids=lambda f: f.name,
 )
 def test_can_set_writable_fields_to_none(field):
     dset = Dataset(type="raw")
     setattr(dset, field.name, None)
     assert getattr(dset, field.name) is None
 
 
-def test_cannot_set_creation_time_to_none():
-    dset = Dataset(type="raw")
-    with pytest.raises(TypeError):
-        dset.creation_time = None
-
-
 def test_init_from_models_sets_metadata():
-    dset = Dataset.from_models(
-        dataset_model=RawDataset(
+    dset = Dataset.from_download_models(
+        dataset_model=DownloadDataset(
             contactEmail="p.stibbons@uu.am",
             creationTime=dateutil.parser.parse("2022-01-10T11:14:52+02:00"),
+            numberOfFiles=0,
+            numberOfFilesArchived=0,
+            packedSize=0,
+            pid=PID.parse("prefix/0123-ab"),
             principalInvestigator="my principal investigator",
             owner="PonderStibbons",
+            size=0,
             sourceFolder=RemotePath("/hex/source91"),
             type=DatasetType.RAW,
             ownerGroup="faculty",
             createdBy="pstibbons",
             createdAt=dateutil.parser.parse("2022-01-10T12:41:22+02:00"),
         ),
         orig_datablock_models=[
-            OrigDatablock(
+            DownloadOrigDatablock(
                 dataFileList=[],
+                datasetId=PID.parse("prefix/0123-ab"),
                 size=0,
                 ownerGroup="faculty",
+                chkAlg="md5",
             )
         ],
     )
 
     assert dset.contact_email == "p.stibbons@uu.am"
     assert dset.creation_time == dateutil.parser.parse("2022-01-10T11:14:52+02:00")
     assert dset.principal_investigator == "my principal investigator"
     assert dset.owner == "PonderStibbons"
     assert dset.source_folder == "/hex/source91"
     assert dset.type == DatasetType.RAW
     assert dset.owner_group == "faculty"
     assert dset.created_by == "pstibbons"
     assert dset.created_at == dateutil.parser.parse("2022-01-10T12:41:22+02:00")
 
-    assert dset.is_published is False
+    assert dset.is_published is None
     assert dset.owner_email is None
 
     assert len(list(dset.files)) == 0
     assert dset.number_of_files == 0
     assert dset.number_of_files_archived == 0
     assert dset.packed_size == 0
     assert dset.size == 0
 
 
 def test_init_from_models_sets_files():
-    dset = Dataset.from_models(
-        dataset_model=RawDataset(
+    dset = Dataset.from_download_models(
+        dataset_model=DownloadDataset(
             contactEmail="p.stibbons@uu.am",
             creationTime=dateutil.parser.parse("2022-01-10T11:14:52-01:00"),
+            numberOfFiles=2,
+            numberOfFilesArchived=0,
             principalInvestigator="librarian@uu.am",
             owner="PonderStibbons",
+            size=6123 + 551,
+            packedSize=0,
+            pid=PID.parse("prefix/abcd-de"),
             sourceFolder=RemotePath("/hex/source91"),
             type=DatasetType.RAW,
             ownerGroup="faculty",
         ),
         orig_datablock_models=[
-            OrigDatablock(
+            DownloadOrigDatablock(
                 dataFileList=[
-                    DataFile(
+                    DownloadDataFile(
                         path="file1.dat",
                         size=6123,
                         time=dateutil.parser.parse("2022-01-09T18:32:01-01:00"),
                     ),
-                    DataFile(
+                    DownloadDataFile(
                         path="sub/file2.png",
                         size=551,
                         time=dateutil.parser.parse("2022-01-09T18:32:42-01:00"),
                     ),
                 ],
                 size=6123 + 551,
                 ownerGroup="faculty",
+                datasetId=PID.parse("prefix/abcd-de"),
+                chkAlg="md5",
             )
         ],
     )
 
     assert len(list(dset.files)) == 2
     assert dset.number_of_files == 2
     assert dset.number_of_files_archived == 0
@@ -208,46 +228,57 @@
     assert f1.remote_access_path(dset.source_folder) == "/hex/source91/sub/file2.png"
     assert f1.local_path is None
     assert f1.size == 551
     assert f1.make_model().path == "sub/file2.png"
 
 
 def test_init_from_models_sets_files_multi_datablocks():
-    dataset_model = RawDataset(
+    dataset_model = DownloadDataset(
         contactEmail="p.stibbons@uu.am",
         creationTime=dateutil.parser.parse("2022-01-10T11:14:52-01:00"),
+        numberOfFiles=2,
+        numberOfFilesArchived=0,
+        packedSize=0,
+        pid=PID.parse("prefix/abcd-de"),
         principalInvestigator="librarian@uu.am",
         owner="PonderStibbons",
+        size=6123 + 992,
         sourceFolder=RemotePath("/hex/source91"),
         type=DatasetType.RAW,
         ownerGroup="faculty",
     )
     orig_datablock_models = [
-        OrigDatablock(
+        DownloadOrigDatablock(
             dataFileList=[
-                DataFile(
+                DownloadDataFile(
                     path="file1.dat",
                     size=6123,
+                    time=dateutil.parser.parse("2022-01-10T11:14:52-01:00"),
                 )
             ],
+            datasetId=PID.parse("prefix/abcd-de"),
             size=6123,
             ownerGroup="faculty",
+            chkAlg="md5",
         ),
-        OrigDatablock(
+        DownloadOrigDatablock(
             dataFileList=[
-                DataFile(
+                DownloadDataFile(
                     path="sub/file2.png",
                     size=992,
+                    time=dateutil.parser.parse("2022-01-10T11:14:52-01:00"),
                 )
             ],
+            datasetId=PID.parse("prefix/abcd-de"),
             size=992,
             ownerGroup="faculty",
+            chkAlg="md5",
         ),
     ]
-    dset = Dataset.from_models(
+    dset = Dataset.from_download_models(
         dataset_model=dataset_model,
         orig_datablock_models=orig_datablock_models,
     )
 
     assert len(list(dset.files)) == 2
     assert dset.number_of_files == 2
     assert dset.number_of_files_archived == 0
@@ -300,33 +331,31 @@
         owner="Ponder Stibbons;Mustrum Ridcully",
         owner_group="faculty",
         principal_investigator="my principal investigator",
         source_folder=RemotePath("/hex/source62"),
         creation_location="ANK/UU",
         shared_with=["librarian", "hicks"],
     )
-    expected = RawDataset(
+    expected = UploadRawDataset(
         contactEmail="p.stibbons@uu.am",
         creationTime=dateutil.parser.parse("2142-04-02T16:44:56"),
         owner="Ponder Stibbons;Mustrum Ridcully",
         ownerGroup="faculty",
         principalInvestigator="my principal investigator",
         sourceFolder=RemotePath("/hex/source62"),
         type=DatasetType.RAW,
-        history=None,
-        isPublished=False,
-        scientificMetadata={},
+        scientificMetadata=None,
         creationLocation="ANK/UU",
         sharedWith=["librarian", "hicks"],
         numberOfFiles=0,
         numberOfFilesArchived=0,
         packedSize=0,
         size=0,
     )
-    assert dset.make_model() == expected
+    assert dset.make_upload_model() == expected
 
 
 def test_make_derived_model():
     dset = Dataset(
         type="derived",
         contact_email="p.stibbons@uu.am;m.ridcully@uu.am",
         creation_time="2142-04-02T16:44:56",
@@ -334,65 +363,65 @@
         owner_group="faculty",
         investigator="p.stibbons@uu.am",
         source_folder=RemotePath("/hex/source62"),
         meta={"weight": {"value": 5.23, "unit": "kg"}},
         input_datasets=[PID(pid="623-122")],
         used_software=["scitacean", "magick"],
     )
-    expected = DerivedDataset(
+    expected = UploadDerivedDataset(
         contactEmail="p.stibbons@uu.am;m.ridcully@uu.am",
         creationTime=dateutil.parser.parse("2142-04-02T16:44:56"),
         owner="Ponder Stibbons;Mustrum Ridcully",
         ownerGroup="faculty",
         investigator="p.stibbons@uu.am",
         sourceFolder=RemotePath("/hex/source62"),
         type=DatasetType.DERIVED,
-        history=None,
-        isPublished=False,
+        isPublished=None,
         scientificMetadata={"weight": {"value": 5.23, "unit": "kg"}},
         inputDatasets=[PID(pid="623-122")],
         usedSoftware=["scitacean", "magick"],
         numberOfFiles=0,
         numberOfFilesArchived=0,
         packedSize=0,
         size=0,
     )
-    assert dset.make_model() == expected
+    assert dset.make_upload_model() == expected
 
 
 @pytest.mark.parametrize(
     "field",
     filter(
-        lambda f: not f.used_by_raw,
+        lambda f: not f.used_by_raw and f.name not in _UNGENERATABLE_FIELDS,
         Dataset.fields(dataset_type="derived", read_only=False),
     ),
     ids=lambda f: f.name,
 )
 @given(st.data())
 @settings(max_examples=10)
 def test_make_raw_model_raises_if_derived_field_set(field, data):
     dset = Dataset(
         type="raw",
         contact_email="p.stibbons@uu.am",
         creation_time="2142-04-02T16:44:56",
         owner="Mustrum Ridcully",
         owner_group="faculty",
-        investigator="p.stibbons@uu.am",
+        principal_investigator="p.stibbons@uu.am",
         source_folder=RemotePath("/hex/source62"),
     )
-    setattr(dset, field.name, data.draw(st.from_type(field.type)))
+    val = data.draw(st.from_type(field.type))
+    assume(val is not None)
+    setattr(dset, field.name, val)
     with pytest.raises(ValueError):
-        dset.make_model()
+        dset.make_upload_model()
 
 
-@pytest.mark.skip("Validation is less strict until full migration to v4")
 @pytest.mark.parametrize(
     "field",
     filter(
-        lambda f: not f.used_by_derived,
+        lambda f: not f.used_by_derived and f.name not in _UNGENERATABLE_FIELDS,
         Dataset.fields(dataset_type="raw", read_only=False),
     ),
     ids=lambda f: f.name,
 )
 @given(st.data())
 @settings(max_examples=10)
 def test_make_derived_model_raises_if_raw_field_set(field, data):
@@ -403,17 +432,19 @@
         owner="Ponder Stibbons",
         owner_group="faculty",
         investigator="p.stibbons@uu.am",
         source_folder=RemotePath("/hex/source62"),
         input_datasets=[PID(pid="623-122")],
         used_software=["scitacean", "magick"],
     )
-    setattr(dset, field.name, data.draw(st.from_type(field.type)))
+    val = data.draw(st.from_type(field.type))
+    assume(val is not None)
+    setattr(dset, field.name, val)
     with pytest.raises(ValueError):
-        dset.make_model()
+        dset.make_upload_model()
 
 
 @pytest.mark.parametrize("field", ("contact_email", "owner_email"))
 def test_email_validation(field):
     dset = Dataset(
         type="raw",
         contact_email="p.stibbons@uu.am",
@@ -421,37 +452,38 @@
         owner="Mustrum Ridcully",
         owner_group="faculty",
         principal_investigator="p.stibbons@uu.am",
         source_folder=RemotePath("/hex/source62"),
     )
     setattr(dset, field, "not-an-email")
     with pytest.raises(pydantic.ValidationError):
-        dset.make_model()
+        dset.make_upload_model()
 
 
 @pytest.mark.parametrize(
     "good_orcid",
     (
         "https://orcid.org/0000-0002-3761-3201",
         "https://orcid.org/0000-0001-2345-6789",
         "https://orcid.org/0000-0003-2818-0368",
     ),
 )
 def test_orcid_validation_valid(good_orcid):
     dset = Dataset(
         type="raw",
         contact_email="jan-lukas.wynen@ess.eu",
+        creation_location="scitacean/tests",
         creation_time="2142-04-02T16:44:56",
         owner="Jan-Lukas Wynen",
         owner_group="ess",
         principal_investigator="jan-lukas.wynen@ess.eu",
         source_folder=RemotePath("/hex/source62"),
         orcid_of_owner=good_orcid,
     )
-    assert dset.make_model().orcidOfOwner == good_orcid
+    assert dset.make_upload_model().orcidOfOwner == good_orcid
 
 
 @pytest.mark.parametrize(
     "bad_orcid",
     (
         "0000-0002-3761-3201",
         "https://not-orcid.eu/0000-0002-3761-3201",
@@ -467,11 +499,11 @@
         owner="Jan-Lukas Wynen",
         owner_group="ess",
         principal_investigator="jan-lukas.wynen@ess.eu",
         source_folder=RemotePath("/hex/source62"),
         orcid_of_owner=bad_orcid,
     )
     with pytest.raises(pydantic.ValidationError):
-        dset.make_model()
+        dset.make_upload_model()
 
 
 # TODO technique
```

### Comparing `scitacean-23.5.0/tests/dataset_test.py` & `scitacean-23.7.7/tests/dataset_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pytest
 from hypothesis import assume, given, settings
 from hypothesis import strategies as st
 
 from scitacean import PID, Dataset, DatasetType, File, model
 from scitacean.testing import strategies as sst
+from scitacean.testing.client import process_uploaded_dataset
 
 from .common.files import make_file
 
 
 @pytest.mark.parametrize("typ", (DatasetType.RAW, DatasetType.DERIVED))
 def test_new_dataset_has_no_files(typ):
     dset = Dataset(type=typ)
@@ -125,63 +126,81 @@
     dset = Dataset(type=typ, checksum_algorithm=algorithm)
     dset.add_local_files("local/data.dat")
 
     [f] = dset.files
     assert f.checksum_algorithm == algorithm
 
 
-@given(sst.datasets())
+@given(sst.datasets(for_upload=True))
 @settings(max_examples=100)
 def test_dataset_models_roundtrip(initial):
-    dataset_model = initial.make_model()
-    dblock_models = initial.make_datablock_models()
-    rebuilt = Dataset.from_models(
-        dataset_model=dataset_model, orig_datablock_models=dblock_models.orig_datablocks
+    dataset_model = initial.make_upload_model()
+    dblock_models = initial.make_datablock_upload_models().orig_datablocks
+    dataset_model, dblock_models = process_uploaded_dataset(
+        dataset_model, dblock_models
+    )
+    dataset_model.createdAt = None
+    dataset_model.createdBy = None
+    dataset_model.updatedAt = None
+    dataset_model.updatedBy = None
+    dataset_model.pid = None
+    rebuilt = Dataset.from_download_models(
+        dataset_model=dataset_model, orig_datablock_models=dblock_models
     )
     assert initial == rebuilt
 
 
 @given(sst.datasets())
 @settings(max_examples=10)
 def test_make_scicat_models_datablock_without_files(dataset):
-    assert dataset.make_datablock_models().orig_datablocks is None
+    assert dataset.make_datablock_upload_models().orig_datablocks is None
 
 
-@given(sst.datasets())
+@given(sst.datasets(pid=st.builds(PID)))
 @settings(max_examples=10)
 def test_make_scicat_models_datablock_with_one_file(dataset):
-    file_model = model.DataFile(path="path", size=6163, chk="8450ac0", gid="group")
+    file_model = model.DownloadDataFile(
+        path="path", size=6163, chk="8450ac0", gid="group", time=datetime.now()
+    )
     dataset.add_files(File.from_scicat(local_path=None, model=file_model))
 
-    blocks = dataset.make_datablock_models().orig_datablocks
+    blocks = dataset.make_datablock_upload_models().orig_datablocks
     assert len(blocks) == 1
 
     block = blocks[0]
     assert block.size == 6163
     assert block.datasetId == dataset.pid
-    assert block.dataFileList == [file_model]
+    assert block.dataFileList == [model.UploadDataFile(**file_model.model_dump())]
 
 
 @given(sst.datasets())
 @settings(max_examples=10)
 def test_eq_self(dset):
     dset.add_files(
         File.from_scicat(
             local_path=None,
-            model=model.DataFile(path="path", size=94571),
+            model=model.DownloadDataFile(path="path", size=94571, time=datetime.now()),
         )
     )
     assert dset == dset
 
 
+# Fields whose types are not supported by hypothesis.
+# E.g. because they contain `Any`.
+_UNGENERATABLE_FIELDS = ("job_parameters", "meta")
+
+
 # Filtering out bools because hypothesis struggles to find enough examples
 # where the new value is not the same as the old value.
 @pytest.mark.parametrize(
     "field",
-    filter(lambda f: f.type != bool, Dataset.fields(read_only=False)),
+    filter(
+        lambda f: f.type != bool and f.name not in _UNGENERATABLE_FIELDS,
+        Dataset.fields(read_only=False),
+    ),
     ids=lambda f: f.name,
 )
 @given(sst.datasets(), st.data())
 @settings(max_examples=10)
 def test_neq_single_mismatched_field_writable(field, initial, data):
     new_val = data.draw(st.from_type(field.type))
     assume(new_val != getattr(initial, field.name))
@@ -192,58 +211,74 @@
 @given(sst.datasets())
 @settings(max_examples=10)
 def test_neq_single_mismatched_file(initial):
     modified = initial.replace()
     modified.add_files(
         File.from_scicat(
             local_path=None,
-            model=model.DataFile(path="path", size=51553312),
+            model=model.DownloadDataFile(
+                path="path", size=51553312, time=datetime.now()
+            ),
         )
     )
     initial.add_files(
         File.from_scicat(
             local_path=None,
-            model=model.DataFile(path="path", size=94571),
+            model=model.DownloadDataFile(path="path", size=94571, time=datetime.now()),
         )
     )
     assert modified != initial
 
 
 @given(sst.datasets())
 @settings(max_examples=10)
 def test_neq_extra_file(initial):
     modified = initial.replace()
     modified.add_files(
         File.from_scicat(
             local_path="/local",
-            model=model.DataFile(path="path", size=51553312),
+            model=model.DownloadDataFile(
+                path="path", size=51553312, time=datetime.now()
+            ),
         )
     )
     assert modified != initial
 
 
 @pytest.mark.parametrize(
     "field",
-    Dataset.fields(read_only=False),
+    (
+        field
+        for field in Dataset.fields(read_only=False)
+        if field.name not in _UNGENERATABLE_FIELDS
+    ),
     ids=lambda f: f.name,
 )
 @given(sst.datasets(), st.data())
 @settings(max_examples=5)
 def test_replace_replaces_single_writable_field(field, initial, data):
     val = data.draw(st.from_type(field.type))
     replaced = initial.replace(**{field.name: val})
     assert getattr(replaced, field.name) == val
 
 
 @pytest.mark.parametrize(
     "field",
-    filter(
-        lambda f: f.name
-        not in ("number_of_files", "number_of_files_archived", "size", "packed_size"),
-        Dataset.fields(read_only=True),
+    (
+        field
+        for field in Dataset.fields(read_only=True)
+        if field.name
+        not in (
+            "history",
+            "lifecycle",
+            "number_of_files",
+            "number_of_files_archived",
+            "size",
+            "packed_size",
+        )
     ),
     ids=lambda f: f.name,
 )
 @given(sst.datasets(), st.data())
 @settings(max_examples=5)
 def test_replace_replaces_single_read_only_field(field, initial, data):
     val = data.draw(st.from_type(field.type))
@@ -267,15 +302,15 @@
 @given(sst.datasets())
 @settings(max_examples=5)
 def test_replace_other_fields_are_copied(initial):
     replaced = initial.replace(
         investigator="inv@esti.gator",
         techniques=[model.Technique(pid="tech/abcd.01", name="magick")],
         type="raw",
-        _read_only={"version": 666},
+        _read_only={"api_version": 666},
     )
     assert replaced.owner == initial.owner
     assert replaced.size == initial.size
     assert replaced.updated_at == initial.updated_at
     assert replaced.history == initial.history
 
 
@@ -296,15 +331,15 @@
 
 
 @given(sst.datasets())
 @settings(max_examples=1)
 def test_replace_does_not_change_files_with_input_files(initial):
     file = File.from_scicat(
         local_path=None,
-        model=model.DataFile(path="path", size=6163),
+        model=model.DownloadDataFile(path="path", size=6163, time=datetime.now()),
     )
     initial.add_files(file)
     replaced = initial.replace(owner="a-new-owner")
     assert replaced.number_of_files == 1
     assert replaced.size == 6163
     assert list(replaced.files) == list(initial.files)
```

### Comparing `scitacean-23.5.0/tests/download_test.py` & `scitacean-23.7.7/tests/download_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import pytest
 from dateutil.parser import parse as parse_date
 
 from scitacean import PID, Client, Dataset, DatasetType, File, IntegrityError
 from scitacean.filesystem import RemotePath
 from scitacean.logging import logger_name
-from scitacean.model import DataFile, OrigDatablock, RawDataset
+from scitacean.model import DownloadDataFile, DownloadDataset, DownloadOrigDatablock
 from scitacean.testing.transfer import FakeFileTransfer
 
 
 def _checksum(data: bytes) -> str:
     checksum = hashlib.new("md5")
     checksum.update(data)
     return checksum.hexdigest()
@@ -26,40 +26,52 @@
 def data_files():
     contents = {
         "file1.dat": b"contents-of-file1",
         "log/what-happened.log": b"ERROR Flux is off the scale",
         "thaum.dat": b"0 4 2 59 330 2314552",
     }
     files = [
-        DataFile(path=name, size=len(content), chk=_checksum(content))
+        DownloadDataFile(
+            path=name,
+            size=len(content),
+            chk=_checksum(content),
+            time=parse_date("1995-08-06T14:14:14"),
+        )
         for name, content in contents.items()
     ]
     return files, contents
 
 
 @pytest.fixture
 def dataset_and_files(data_files):
-    model = RawDataset(
+    model = DownloadDataset(
         contactEmail="p.stibbons@uu.am",
         creationTime=parse_date("1995-08-06T14:14:14"),
+        numberOfFiles=len(data_files[0]),
+        numberOfFilesArchived=0,
         owner="pstibbons",
         ownerGroup="faculty",
+        packedSize=0,
         pid=PID(prefix="UU.000", pid="5125.ab.663.8c9f"),
         principalInvestigator="m.ridcully@uu.am",
+        size=sum(f.size for f in data_files[0]),
         sourceFolder=RemotePath("/src/stibbons/774"),
         type=DatasetType.RAW,
     )
-    block = OrigDatablock(
+    block = DownloadOrigDatablock(
+        chkAlg="md5",
         ownerGroup="faculty",
         size=sum(f.size for f in data_files[0]),
         datasetId=PID(prefix="UU.000", pid="5125.ab.663.8c9f"),
         id=PID(prefix="UU.000", pid="0941.66.abff.41de"),
         dataFileList=data_files[0],
     )
-    dset = Dataset.from_models(dataset_model=model, orig_datablock_models=[block])
+    dset = Dataset.from_download_models(
+        dataset_model=model, orig_datablock_models=[block]
+    )
     return dset, {
         dset.source_folder / name: content for name, content in data_files[1].items()
     }
 
 
 def load(name: Union[str, Path]):
     with open(name, "rb") as f:
@@ -188,15 +200,15 @@
 
 
 def test_download_files_ignores_checksum_if_alg_is_none(fs, dataset_and_files):
     dataset, contents = dataset_and_files
 
     content = b"random-stuff"
     bad_checksum = "incorrect-checksum"
-    model = DataFile(
+    model = DownloadDataFile(
         path="file.txt",
         size=len(content),
         time=parse_date("2022-06-22T15:42:53+00:00"),
         chk=bad_checksum,
     )
     dataset.add_orig_datablock(checksum_algorithm=None)
     dataset.add_files(File.from_scicat(model))
@@ -212,15 +224,15 @@
 
 
 def test_download_files_detects_bad_checksum(fs, dataset_and_files):
     dataset, contents = dataset_and_files
 
     content = b"random-stuff"
     bad_checksum = "incorrect-checksum"
-    model = DataFile(
+    model = DownloadDataFile(
         path="file.txt",
         size=len(content),
         time=parse_date("2022-06-22T15:42:53+00:00"),
         chk=bad_checksum,
     )
     dataset.add_orig_datablock(checksum_algorithm="md5")
     dataset.add_files(File.from_scicat(model))
@@ -236,15 +248,15 @@
 
 
 def test_download_files_detects_bad_size(fs, dataset_and_files, caplog):
     dataset, contents = dataset_and_files
 
     content = b"random-stuff"
     bad_checksum = hashlib.md5(content).hexdigest()
-    model = DataFile(
+    model = DownloadDataFile(
         path="file.txt",
         size=89412,  # Too large
         time=parse_date("2022-06-22T15:42:53+00:00"),
         chk=bad_checksum,
     )
     dataset.add_orig_datablock(checksum_algorithm="md5")
     dataset.add_files(File.from_scicat(model))
```

### Comparing `scitacean-23.5.0/tests/file_test.py` & `scitacean-23.7.7/tests/file_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pytest
 from dateutil.parser import parse as parse_date
 
 from scitacean import File, IntegrityError, RemotePath
 from scitacean.file import checksum_of_file
 from scitacean.logging import logger_name
-from scitacean.model import DataFile
+from scitacean.model import DownloadDataFile
 
 from .common.files import make_file
 
 
 @pytest.fixture
 def fake_file(fs):
     return make_file(fs, path=Path("local", "dir", "events.nxs"))
@@ -110,39 +110,39 @@
         Path("data", "subdir", "file.dat"), base_path=Path("data") / "subdir"
     )
     assert file.remote_path == RemotePath("file.dat")
     assert file.make_model().path == "file.dat"
 
 
 def test_file_from_scicat():
-    model = DataFile(
+    model = DownloadDataFile(
         path="dir/image.jpg", size=12345, time=parse_date("2022-06-22T15:42:53.123Z")
     )
     file = File.from_scicat(model)
 
     assert file.remote_access_path("/remote/folder") == "/remote/folder/dir/image.jpg"
     assert file.local_path is None
     assert file.checksum() is None
     assert file.size == 12345
     assert file.creation_time == parse_date("2022-06-22T15:42:53.123Z")
 
 
 def test_file_from_scicat_remote_path_uses_forward_slash():
     file = File.from_scicat(
-        DataFile(
+        DownloadDataFile(
             path="data/subdir/file.dat",
             size=0,
             time=parse_date("2022-06-22T15:42:53.123Z"),
         ),
         local_path=None,
     )
     assert file.remote_path == RemotePath("data/subdir/file.dat")
 
     file = File.from_scicat(
-        DataFile(
+        DownloadDataFile(
             path="data/subdir/file.dat",
             size=0,
             time=parse_date("2022-06-22T15:42:53.123Z"),
         ),
         local_path=Path("data") / "subdir",
     )
     assert file.remote_path == RemotePath("data/subdir/file.dat")
@@ -190,31 +190,29 @@
     )
     assert uploaded.remote_uid == "the-user"
     assert uploaded.remote_gid == "the-group"
     assert uploaded._remote_creation_time == parse_date("2100-09-07T11:34:51")
 
 
 def test_downloaded():
-    model = DataFile(
+    model = DownloadDataFile(
         path="dir/stream.s",
         size=55123,
         time=parse_date("2025-01-09T21:00:21.421Z"),
         perm="xrw",
-        createdBy="creator-id",
     )
     file = File.from_scicat(model)
     downloaded = file.downloaded(local_path="/local/stream.s")
 
     assert downloaded.is_on_local
     assert downloaded.is_on_remote
 
     assert downloaded.remote_path == RemotePath("dir/stream.s")
     assert downloaded.local_path == Path("/local/stream.s")
     assert downloaded.remote_perm == "xrw"
-    assert downloaded.created_by == "creator-id"
 
 
 def test_creation_time_is_always_local_time(fake_file):
     file = File.from_local(path=fake_file["path"])
     model = file.make_model()
     model.time = parse_date("2105-04-01T04:52:23")
     uploaded = file.uploaded()
@@ -277,15 +275,15 @@
 
     with open(fake_file["path"], "wb") as f:
         f.write(new_contents)
     assert file.checksum() == checksum
 
 
 def test_validate_after_download_detects_bad_checksum(fake_file):
-    model = DataFile(
+    model = DownloadDataFile(
         path=fake_file["path"].name,
         size=fake_file["size"],
         time=parse_date("2022-06-22T15:42:53.123Z"),
         chk="incorrect-checksum",
     )
     file = replace(
         File.from_scicat(model),
@@ -294,29 +292,29 @@
     downloaded = file.downloaded(local_path=fake_file["path"])
 
     with pytest.raises(IntegrityError):
         downloaded.validate_after_download()
 
 
 def test_validate_after_download_ignores_checksum_if_no_algorithm(fake_file):
-    model = DataFile(
+    model = DownloadDataFile(
         path=fake_file["path"].name,
         size=fake_file["size"],
         time=parse_date("2022-06-22T15:42:53.123Z"),
         chk="incorrect-checksum",
     )
     file = File.from_scicat(model)
     downloaded = file.downloaded(local_path=fake_file["path"])
 
     # does not raise
     downloaded.validate_after_download()
 
 
 def test_validate_after_download_detects_size_mismatch(fake_file, caplog):
-    model = DataFile(
+    model = DownloadDataFile(
         path=fake_file["path"].name,
         size=fake_file["size"] + 100,
         time=parse_date("2022-06-22T15:42:53.123Z"),
         chk="incorrect-checksum",
     )
     file = replace(
         File.from_scicat(model),
@@ -326,15 +324,22 @@
     with caplog.at_level("INFO", logger=logger_name()):
         downloaded.validate_after_download()
     assert "does not match size reported in dataset" in caplog.text
 
 
 @pytest.mark.parametrize("chk", ("sha256", None))
 def test_local_is_not_up_to_date_for_remote_file(chk):
-    file = File.from_scicat(DataFile(path="data.csv", size=65178, chk=chk))
+    file = File.from_scicat(
+        DownloadDataFile(
+            path="data.csv",
+            size=65178,
+            chk=chk,
+            time=parse_date("2022-06-22T15:42:53.123Z"),
+        )
+    )
     assert not file.local_is_up_to_date()
 
 
 def test_local_is_up_to_date_for_local_file():
     # Note that the file does not actually exist on disk but the test still works.
     file = File.from_local(path="image.jpg")
     assert file.local_is_up_to_date()
@@ -344,36 +349,41 @@
     contents = b"some file content"
     checksum = hashlib.new("blake2b")
     checksum.update(contents)
     checksum = checksum.hexdigest()
     fs.create_file("data.csv", contents=contents)
 
     file = File.from_scicat(
-        DataFile(path="data.csv", size=65178, chk=checksum)
+        DownloadDataFile(
+            path="data.csv",
+            size=65178,
+            chk=checksum,
+            time=parse_date("2022-06-22T15:42:53.123Z"),
+        )
     ).downloaded(local_path="data.csv")
     with pytest.warns(UserWarning):
         assert file.local_is_up_to_date()
 
 
 def test_local_is_up_to_date_matching_checksum(fake_file):
-    model = DataFile(
+    model = DownloadDataFile(
         path=fake_file["path"].name,
         size=fake_file["size"],
         time=parse_date("2022-06-22T15:42:53.123Z"),
         chk=fake_file["checksum"],
     )
     file = replace(
         File.from_scicat(model).downloaded(local_path=fake_file["path"]),
         checksum_algorithm="md5",
     )
     assert file.local_is_up_to_date()
 
 
 def test_local_is_not_up_to_date_differing_checksum(fake_file):
-    model = DataFile(
+    model = DownloadDataFile(
         path=fake_file["path"].name,
         size=fake_file["size"],
         time=parse_date("2022-06-22T15:42:53.123Z"),
         chk="a-different-checksum",
     )
     file = replace(
         File.from_scicat(model).downloaded(local_path=fake_file["path"]),
```

### Comparing `scitacean-23.5.0/tests/filesystem_test.py` & `scitacean-23.7.7/tests/filesystem_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/tests/html_repr/html_repr_test.py` & `scitacean-23.7.7/tests/html_repr/html_repr_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/tests/testing/strategies_test.py` & `scitacean-23.7.7/tests/testing/strategies_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from scitacean import PID, DatasetType
 from scitacean.testing import strategies as sst
 
 
-@given(sst.datasets())
+@given(sst.datasets(for_upload=True))
 def test_datasets_makes_valid_dataset(dset):
-    _ = dset.make_model()
+    _ = dset.make_upload_model()
 
 
 @settings(max_examples=10)
 @given(sst.datasets(dataset_type=DatasetType.RAW))
 def test_datasets_can_set_type_to_raw(dset):
     assert dset.type == "raw"
```

### Comparing `scitacean-23.5.0/tests/transfer/ssh_test.py` & `scitacean-23.7.7/tests/transfer/ssh_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2022 Scitacean contributors (https://github.com/SciCatProject/scitacean)
 import dataclasses
-import re
 import tempfile
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
-from uuid import uuid4
 
 import fabric
 import paramiko
 import pytest
 
 from scitacean import Dataset, File, FileUploadError, RemotePath
+from scitacean.testing.ssh import IgnorePolicy, skip_if_not_ssh
 from scitacean.transfer.ssh import SSHFileTransfer
 
-from ..common.ssh_server import IgnorePolicy, skip_if_not_ssh
-
 
 @pytest.fixture(scope="session", autouse=True)
 def server(request, ssh_fileserver):
     skip_if_not_ssh(request)
 
 
 def test_download_one_file(ssh_access, ssh_connect_with_username_password, tmp_path):
@@ -67,35 +64,34 @@
     with open(ssh_data_dir / "upload" / "upload_0.txt", "r") as f:
         assert f.read() == "File to test upload123"
 
 
 def test_upload_one_file_source_folder_in_transfer(
     ssh_access, ssh_connect_with_username_password, tmp_path, ssh_data_dir
 ):
-    ds = Dataset(type="raw", pid="abcd-12")
+    ds = Dataset(type="raw", owner="librarian")
     with open(tmp_path / "file1.txt", "w") as f:
         f.write("File no. 2")
 
-    source_uid = str(uuid4())
     ssh = SSHFileTransfer(
         host=ssh_access.host,
         port=ssh_access.port,
-        source_folder=f"/data/upload/{source_uid}",
+        source_folder="/data/upload/{owner}",
     )
     with ssh.connect_for_upload(
         dataset=ds, connect=ssh_connect_with_username_password
     ) as con:
-        assert re.match(r"/data/upload/[a-d0-9\-]+", con.source_folder.posix)
+        assert con.source_folder == RemotePath("/data/upload/librarian")
         con.upload_files(
             File.from_local(
                 path=tmp_path / "file1.txt", remote_path=RemotePath("upload_1.txt")
             )
         )
 
-    with open(ssh_data_dir / "upload" / source_uid / "upload_1.txt", "r") as f:
+    with open(ssh_data_dir / "upload" / "librarian" / "upload_1.txt", "r") as f:
         assert f.read() == "File no. 2"
 
 
 def test_upload_two_files(
     ssh_access, ssh_connect_with_username_password, tmp_path, ssh_data_dir
 ):
     ds = Dataset(type="raw", source_folder=RemotePath("/data/upload2"))
@@ -235,18 +231,18 @@
             raise ValueError(
                 "connect_with_username_password must only be"
                 f" used without extra arguments. Got {kwargs=}"
             )
         connection = fabric.Connection(
             host=host,
             port=port,
-            user=ssh_access.username,
+            user=ssh_access.user.username,
             config=ssh_connection_config,
             connect_kwargs={
-                "password": ssh_access.password,
+                "password": ssh_access.user.password,
                 "transport_factory": CorruptingTransfer,
                 **ssh_connection_config.connect_kwargs,
             },
         )
         connection.client.set_missing_host_key_policy(IgnorePolicy())
         return connection
 
@@ -297,18 +293,18 @@
             raise ValueError(
                 "connect_with_username_password must only be"
                 f" used without extra arguments. Got {kwargs=}"
             )
         connection = fabric.Connection(
             host=host,
             port=port,
-            user=ssh_access.username,
+            user=ssh_access.user.username,
             config=ssh_connection_config,
             connect_kwargs={
-                "password": ssh_access.password,
+                "password": ssh_access.user.password,
                 "transport_factory": RaisingTransfer,
                 **ssh_connection_config.connect_kwargs,
             },
         )
         connection.client.set_missing_host_key_policy(IgnorePolicy())
         return connection
```

### Comparing `scitacean-23.5.0/tests/upload_test.py` & `scitacean-23.7.7/tests/upload_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,161 +2,152 @@
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 from contextlib import contextmanager
 
 import pytest
 from dateutil.parser import parse as parse_date
 
-from scitacean import Dataset, DatasetType, ScicatCommError, model
+from scitacean import Dataset, DatasetType, ScicatCommError
 from scitacean.testing.client import FakeClient
 from scitacean.testing.transfer import FakeFileTransfer
 
 from .common.files import make_file
 
 # TODO source_folder changed / populated in file after upload
 
 
 @pytest.fixture
-def ownable():
-    return model.Ownable(ownerGroup="uu", accessGroups=["group1", "2nd_group"])
-
-
-@pytest.fixture
-def derived_dataset_model(ownable):
-    return model.DerivedDataset(
-        owner="PonderStibbons",
+def dataset():
+    return Dataset(
+        access_groups=["group1", "2nd_group"],
         investigator="ridcully@uu.am",
-        contactEmail="p.stibbons@uu.am",
-        sourceFolder="/hex/source123",
-        size=0,
-        numberOfFiles=0,
-        creationTime=parse_date("2011-08-24T12:34:56Z"),
-        datasetName="Data A38",
-        inputDatasets=[],
-        usedSoftware=["EasyScience"],
-        scientificMetadata={
+        contact_email="p.stibbons@uu.am",
+        source_folder="/hex/source123",
+        creation_time=parse_date("2011-08-24T12:34:56Z"),
+        input_datasets=[],
+        name="Data A38",
+        owner="PonderStibbons",
+        owner_group="uu",
+        used_software=["EasyScience"],
+        meta={
             "data_type": "event data",
             "temperature": {"value": "123", "unit": "K"},
             "weight": {"value": "42", "unit": "mg"},
         },
         type=DatasetType.DERIVED,
-        **ownable.dict(),
     )
 
 
 @pytest.fixture
-def client(fs):
-    return FakeClient.from_token(
-        url="",
-        token="",
-        file_transfer=FakeFileTransfer(fs=fs, files={}, reverted={}),
-    )
+def dataset_with_files(dataset, fs):
+    make_file(fs, path="file.nxs", contents=b"contents of file.nxs")
+    make_file(fs, path="the_log_file.log", contents=b"this is a log file")
+    dataset.add_local_files("file.nxs", "the_log_file.log")
+    return dataset
 
 
 @pytest.fixture
-def dataset(derived_dataset_model, fs):
-    make_file(fs, path="file.nxs", contents=b"contents of file.nxs")
-    make_file(fs, path="the_log_file.log", contents=b"this is a log file")
-    dset = Dataset.from_models(
-        dataset_model=derived_dataset_model, orig_datablock_models=None
+def client(fs, scicat_access):
+    return FakeClient.from_credentials(
+        url="",
+        **scicat_access.user.credentials,
+        file_transfer=FakeFileTransfer(fs=fs, files={}, reverted={}),
     )
-    dset.add_local_files("file.nxs", "the_log_file.log")
-    return dset
 
 
-def test_upload_returns_updated_dataset(client, dataset):
-    finalized = client.upload_new_dataset_now(dataset)
+def test_upload_returns_updated_dataset(client, dataset_with_files):
+    finalized = client.upload_new_dataset_now(dataset_with_files)
     expected = client.get_dataset(finalized.pid).replace(
         # The backend may update the dataset after upload
         _read_only={
             "updated_at": finalized.updated_at,
             "updated_by": finalized.updated_by,
         }
     )
     assert finalized == expected
 
 
-def test_upload_without_files_creates_dataset(client, derived_dataset_model):
-    dataset = Dataset.from_models(
-        dataset_model=derived_dataset_model, orig_datablock_models=None
-    )
+def test_upload_without_files_creates_dataset(client, dataset):
     finalized = client.upload_new_dataset_now(dataset)
     expected = client.get_dataset(finalized.pid).replace(
         # The backend may update the dataset after upload
         _read_only={
             "updated_at": finalized.updated_at,
             "updated_by": finalized.updated_by,
         }
     )
     assert finalized == expected
     with pytest.raises(ScicatCommError):
         client.scicat.get_orig_datablocks(finalized.pid)
 
 
-def test_upload_creates_dataset_and_datablock(client, dataset):
-    finalized = client.upload_new_dataset_now(dataset)
-    assert client.datasets[finalized.pid] == finalized.make_model()
-    assert (
-        client.orig_datablocks[finalized.pid]
-        == finalized.make_datablock_models().orig_datablocks
-    )
+def test_upload_creates_dataset_and_datablock(client, dataset_with_files):
+    finalized = client.upload_new_dataset_now(dataset_with_files)
+    assert client.datasets[finalized.pid].createdAt == finalized.created_at
+    assert client.datasets[finalized.pid].datasetName == finalized.name
+    assert client.datasets[finalized.pid].owner == finalized.owner
+    assert client.datasets[finalized.pid].size == finalized.size
+
+    assert client.orig_datablocks[finalized.pid][0].createdBy == finalized.created_by
+    assert client.orig_datablocks[finalized.pid][0].datasetId == finalized.pid
+    assert client.orig_datablocks[finalized.pid][0].size == finalized.size
 
 
-def test_upload_uploads_files_to_source_folder(client, dataset):
-    finalized = client.upload_new_dataset_now(dataset)
+def test_upload_uploads_files_to_source_folder(client, dataset_with_files):
+    finalized = client.upload_new_dataset_now(dataset_with_files)
     source_folder = client.file_transfer.source_folder_for(finalized)
 
     assert (
         client.file_transfer.files[source_folder / "file.nxs"]
         == b"contents of file.nxs"
     )
     assert (
         client.file_transfer.files[source_folder / "the_log_file.log"]
         == b"this is a log file"
     )
 
 
-def test_upload_does_not_create_dataset_if_file_upload_fails(dataset, fs):
+def test_upload_does_not_create_dataset_if_file_upload_fails(dataset_with_files, fs):
     class RaisingUpload(FakeFileTransfer):
         source_dir = "/"
 
         def upload_files(self, *files):
             raise RuntimeError("Fake upload failure")
 
         @contextmanager
         def connect_for_upload(self, pid):
             yield self
 
     client = FakeClient(file_transfer=RaisingUpload(fs=fs))
 
     with pytest.raises(RuntimeError, match="Fake upload failure"):
-        client.upload_new_dataset_now(dataset)
+        client.upload_new_dataset_now(dataset_with_files)
 
-    assert dataset.pid not in client.datasets
-    assert dataset.pid not in client.orig_datablocks
+    assert not client.datasets
+    assert not client.orig_datablocks
 
 
-def test_upload_cleans_up_files_if_dataset_ingestion_fails(dataset, fs):
+def test_upload_cleans_up_files_if_dataset_ingestion_fails(dataset_with_files, fs):
     client = FakeClient(
         disable={"create_dataset_model": ScicatCommError("Ingestion failed")},
         file_transfer=FakeFileTransfer(fs=fs),
     )
     with pytest.raises(ScicatCommError):
-        client.upload_new_dataset_now(dataset)
+        client.upload_new_dataset_now(dataset_with_files)
 
     assert not client.file_transfer.files
 
 
-def test_failed_datablock_upload_does_not_revert(dataset, fs):
+def test_failed_datablock_upload_does_not_revert(dataset_with_files, fs):
     client = FakeClient(
         disable={"create_orig_datablock": ScicatCommError("Ingestion failed")},
         file_transfer=FakeFileTransfer(fs=fs),
     )
     with pytest.raises(RuntimeError):
-        client.upload_new_dataset_now(dataset)
+        client.upload_new_dataset_now(dataset_with_files)
 
     uploaded_dset = next(iter(client.datasets.values()))
     assert uploaded_dset.owner == "PonderStibbons"
     assert uploaded_dset.datasetName == "Data A38"
     assert uploaded_dset.usedSoftware == ["EasyScience"]
 
     assert client.file_transfer.files
```

### Comparing `scitacean-23.5.0/tests/util/formatter_test.py` & `scitacean-23.7.7/tests/util/formatter_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 
-from scitacean import Dataset
+import pytest
+
+from scitacean import PID, Dataset
 from scitacean.util.formatter import DatasetPathFormatter
 
 
 def test_dataset_formatter_uses_dataset_fields():
     dset = Dataset(type="raw", owner="magrat")
     fmt = "{type} {owner}"
     formatted = DatasetPathFormatter().format(fmt, dset=dset)
     expected = fmt.format(type=dset.type, owner=dset.owner)
     assert formatted == expected
 
 
 def test_dataset_formatter_can_access_attrs_of_fields():
-    dset = Dataset(type="raw", pid="prefix/actual-id")
+    dset = Dataset(type="raw")
+    dset._pid = PID.parse("prefix/actual-id")
     formatted = DatasetPathFormatter().format("{pid.pid}", dset=dset)
     assert formatted == "actual-id"
 
 
 def test_dataset_formatter_supports_special_uid():
     dset = Dataset(type="raw", owner="magrat")
     fmt = "id: {uid}"
@@ -48,7 +51,13 @@
     assert formatted == expected
 
 
 def test_dataset_formatter_preserves_path_separators():
     dset = Dataset(type="raw", owner="Nanny Ogg")
     formatted = DatasetPathFormatter().format("{type}/{owner}.data", dset=dset)
     assert formatted == "raw/Nanny Ogg.data"
+
+
+def test_dataset_formatter_does_not_allow_none():
+    dset = Dataset(type="raw", owner=None)
+    with pytest.raises(ValueError):
+        DatasetPathFormatter().format("{owner}", dset=dset)
```

### Comparing `scitacean-23.5.0/tools/model-generation/templates/__init__.py` & `scitacean-23.7.7/tools/model-generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.5.0/tox.ini` & `scitacean-23.7.7/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,24 @@
 
 [testenv]
 deps = -r requirements/test.txt
 commands =
     full: python -m pytest --backend-tests --ssh-tests
     !full: python -m pytest
 
+[testenv:pydantic2]
+envlist = py{311}-full
+deps = -r requirements-pydantic2/test.txt
+commands =
+    full: python -m pytest --backend-tests --ssh-tests
+    !full: python -m pytest
+
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
-basepython = python3.8
+basepython = python3.11
 deps = -r requirements/docs.txt
 allowlist_externals = find
 commands = python -m sphinx -v -b html -d {toxworkdir}/docs_doctrees docs html
            python -m sphinx -v -b doctest -d {toxworkdir}/docs_doctrees docs html
            python -m sphinx -v -b linkcheck -d {toxworkdir}/docs_doctrees docs html
            find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
```

