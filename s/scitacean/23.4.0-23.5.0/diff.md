# Comparing `tmp/scitacean-23.4.0.tar.gz` & `tmp/scitacean-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitacean-23.4.0.tar", last modified: Wed Apr  5 13:56:35 2023, max compression
+gzip compressed data, was "scitacean-23.5.0.tar", last modified: Mon May 15 15:28:23 2023, max compression
```

## Comparing `scitacean-23.4.0.tar` & `scitacean-23.5.0.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.717364 scitacean-23.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.701364 scitacean-23.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-05 13:56:23.000000 scitacean-23.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.701364 scitacean-23.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-05 13:56:23.000000 scitacean-23.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-05 13:56:23.000000 scitacean-23.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-05 13:56:23.000000 scitacean-23.4.0/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-05 13:56:23.000000 scitacean-23.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-05 13:56:23.000000 scitacean-23.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-05 13:56:23.000000 scitacean-23.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-05 13:56:23.000000 scitacean-23.4.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-05 13:56:23.000000 scitacean-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-05 13:56:23.000000 scitacean-23.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-05 13:56:23.000000 scitacean-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-05 13:56:23.000000 scitacean-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-05 13:56:35.717364 scitacean-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-05 13:56:23.000000 scitacean-23.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-05 13:56:23.000000 scitacean-23.4.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.701364 scitacean-23.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.701364 scitacean-23.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/_static/anaconda-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.701364 scitacean-23.4.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.701364 scitacean-23.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/_templates/scitacean-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/_templates/scitacean-dataclass-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.705364 scitacean-23.4.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/developer/coding-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/developer/dependency-management.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/developer/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/developer/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.705364 scitacean-23.4.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.705364 scitacean-23.4.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/user-guide/downloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/user-guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/user-guide/testing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-05 13:56:23.000000 scitacean-23.4.0/docs/user-guide/uploading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-05 13:56:23.000000 scitacean-23.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.705364 scitacean-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-05 13:56:23.000000 scitacean-23.4.0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-05 13:56:35.717364 scitacean-23.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.697364 scitacean-23.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45630 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_dataset_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/_html_repr/
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/_html_repr/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/images/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/_html_repr/styles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/styles/dataset.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/_html_repr/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/templates/dataset_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/templates/files_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_html_repr/templates/metadata_repr.html.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/_internal/orcid.py
--rw-r--r--   0 runner    (1001) docker     (123)    26374 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/datablock.py
--rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/testing/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/testing/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/testing/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/testing/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/transfer/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/transfer/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/src/scitacean/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/util/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-05 13:56:23.000000 scitacean-23.4.0/src/scitacean/util/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.709364 scitacean-23.4.0/src/scitacean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-05 13:56:35.000000 scitacean-23.4.0/src/scitacean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-05 13:56:35.000000 scitacean-23.4.0/src/scitacean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 13:56:35.000000 scitacean-23.4.0/src/scitacean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-05 13:56:35.000000 scitacean-23.4.0/src/scitacean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-05 13:56:35.000000 scitacean-23.4.0/src/scitacean.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/client_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.697364 scitacean-23.4.0/tests/common/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/common/data/ssh_server_seed/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/data/ssh_server_seed/table.csv
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/data/ssh_server_seed/text.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/docker-compose-ssh-server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/common/ssh_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/data/datasets.json
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/data/orig_datablocks.json
--rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/dataset_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/download_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/filesystem_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/html_repr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/html_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/html_repr/html_repr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/testing/strategies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/transfer/ssh_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/upload_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-05 13:56:23.000000 scitacean-23.4.0/tests/util/formatter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.701364 scitacean-23.4.0/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.713364 scitacean-23.4.0/tools/model-generation/
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.717364 scitacean-23.4.0/tools/model-generation/spec/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/data-file.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/datablock.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/dataset-lifecycle.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/dataset.yml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/mongo-queryable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/orig-datablock.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/ownable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/spec/technique.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:56:35.717364 scitacean-23.4.0/tools/model-generation/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/templates/dataset.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/templates/field_spec.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/templates/model.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-05 13:56:23.000000 scitacean-23.4.0/tools/model-generation/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-05 13:56:23.000000 scitacean-23.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.109059 scitacean-23.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.089058 scitacean-23.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-15 15:28:08.000000 scitacean-23.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-15 15:28:08.000000 scitacean-23.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 15:28:08.000000 scitacean-23.5.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 15:28:08.000000 scitacean-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-15 15:28:08.000000 scitacean-23.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-15 15:28:08.000000 scitacean-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 15:28:08.000000 scitacean-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-15 15:28:23.109059 scitacean-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-15 15:28:08.000000 scitacean-23.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-15 15:28:08.000000 scitacean-23.5.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/anaconda-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_templates/scitacean-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/_templates/scitacean-dataclass-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/coding-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/dependency-management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/developer/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.093058 scitacean-23.5.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/downloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/testing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-05-15 15:28:08.000000 scitacean-23.5.0/docs/user-guide/uploading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-15 15:28:08.000000 scitacean-23.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-15 15:28:08.000000 scitacean-23.5.0/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-15 15:28:23.109059 scitacean-23.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.085058 scitacean-23.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/src/scitacean/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45630 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_dataset_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/src/scitacean/_html_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_html_repr/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/images/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_html_repr/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/styles/dataset.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_html_repr/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/dataset_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/files_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_html_repr/templates/metadata_repr.html.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/_internal/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/datablock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/testing/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17714 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/transfer/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/transfer/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.101059 scitacean-23.5.0/src/scitacean/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/util/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-15 15:28:08.000000 scitacean-23.5.0/src/scitacean/util/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.097059 scitacean-23.5.0/src/scitacean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 15:28:23.000000 scitacean-23.5.0/src/scitacean.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.089058 scitacean-23.5.0/tests/common/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/common/data/ssh_server_seed/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/data/ssh_server_seed/table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/data/ssh_server_seed/text.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/docker-compose-ssh-server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/common/ssh_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/data/datasets.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/data/orig_datablocks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/dataset_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/download_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/filesystem_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/html_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/html_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/html_repr/html_repr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/testing/strategies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/transfer/ssh_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/upload_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-15 15:28:08.000000 scitacean-23.5.0/tests/util/formatter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.089058 scitacean-23.5.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.105059 scitacean-23.5.0/tools/model-generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.109059 scitacean-23.5.0/tools/model-generation/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/data-file.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/datablock.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/dataset-lifecycle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/mongo-queryable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/orig-datablock.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/ownable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/spec/technique.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:23.109059 scitacean-23.5.0/tools/model-generation/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/dataset.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/field_spec.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/templates/model.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-15 15:28:08.000000 scitacean-23.5.0/tools/model-generation/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 15:28:08.000000 scitacean-23.5.0/tox.ini
```

### Comparing `scitacean-23.4.0/.github/workflows/ci.yml` & `scitacean-23.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/.github/workflows/codeql-analysis.yml` & `scitacean-23.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/.github/workflows/dependency-review.yml` & `scitacean-23.5.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/.github/workflows/docs.yml` & `scitacean-23.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/.github/workflows/release.yml` & `scitacean-23.5.0/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     name: Deploy packages
     needs: [build_wheels]
     runs-on: ubuntu-22.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v2
-      - uses: pypa/gh-action-pypi-publish@v1.8.5
+      - uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   docs:
     needs: upload_packages
     uses: ./.github/workflows/docs.yml
```

### Comparing `scitacean-23.4.0/.pre-commit-config.yaml` & `scitacean-23.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/CONTRIBUTING.md` & `scitacean-23.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/LICENSE` & `scitacean-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/PKG-INFO` & `scitacean-23.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 23.4.0
+Version: 23.5.0
 Summary: High-level interface for SciCat
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `scitacean-23.4.0/README.md` & `scitacean-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/SECURITY.md` & `scitacean-23.5.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/_static/anaconda-logo.svg` & `scitacean-23.5.0/docs/_static/anaconda-logo.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/_static/css/custom.css` & `scitacean-23.5.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/_static/favicon.ico` & `scitacean-23.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/_static/logo-dark.svg` & `scitacean-23.5.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/_static/logo.svg` & `scitacean-23.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/_templates/scitacean-class-template.rst` & `scitacean-23.5.0/docs/_templates/scitacean-class-template.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/conf.py` & `scitacean-23.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/developer/coding-conventions.rst` & `scitacean-23.5.0/docs/developer/coding-conventions.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/developer/dependency-management.rst` & `scitacean-23.5.0/docs/developer/dependency-management.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/developer/getting-started.rst` & `scitacean-23.5.0/docs/developer/getting-started.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/developer/testing.rst` & `scitacean-23.5.0/docs/developer/testing.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/index.rst` & `scitacean-23.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/reference/index.rst` & `scitacean-23.5.0/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/release-notes.rst` & `scitacean-23.5.0/docs/release-notes.rst`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,29 @@
 
    Deprecations
    ~~~~~~~~~~~~
 
    Stability, Maintainability, and Testing
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+v23.05.0 (2023-05-15)
+---------------------
+
+Features
+~~~~~~~~
+
+* Early support for the new SciCat backend version 4.
+  It is possible to upload and download datasets as before.
+  But the new fields added in v4 are not supported yet.
+
+Bugfixes
+~~~~~~~~
+
+* Fixed a bug in ``Client.download_files`` where if a file already existed on local, its local path was not set. This was introduced in v23.04.0.
+
 v23.04.0 (2023-04-05)
 ---------------------
 
 Features
 ~~~~~~~~
 
 * Better HTML formatting of ESS-style scientific metadata.
```

### Comparing `scitacean-23.4.0/docs/user-guide/downloading.ipynb` & `scitacean-23.5.0/docs/user-guide/downloading.ipynb`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/docs/user-guide/testing.ipynb` & `scitacean-23.5.0/docs/user-guide/testing.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975626026272578%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(5, '    "*

 * *            'file_transfer=FakeFileTransfer(source_folder="/upload/{uid}"))\')], delete: [5]}}, '*

 * *            "18: {'source': {insert: [(5, '    "*

 * *            'file_transfer=FakeFileTransfer(source_folder="/upload/{uid}"))\')], delete: [5]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.10'}}"}*

```diff
@@ -84,15 +84,15 @@
             "outputs": [],
             "source": [
                 "from scitacean.testing.client import FakeClient\n",
                 "from scitacean.testing.transfer import FakeFileTransfer\n",
                 "\n",
                 "client = FakeClient.without_login(\n",
                 "    url=\"https://fake.scicat\",\n",
-                "    file_transfer=FakeFileTransfer(source_folder=\"/upload/{pid.pid}\"))"
+                "    file_transfer=FakeFileTransfer(source_folder=\"/upload/{uid}\"))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e566a6bd-e7e1-4c0b-bb80-c92bcc1b30ba",
             "metadata": {},
             "source": [
@@ -241,15 +241,15 @@
             "outputs": [],
             "source": [
                 "from scitacean.testing.client import FakeClient\n",
                 "from scitacean.testing.transfer import FakeFileTransfer\n",
                 "\n",
                 "client = FakeClient.without_login(\n",
                 "    url=\"https://fake.scicat\",\n",
-                "    file_transfer=FakeFileTransfer(source_folder=\"/upload/{pid.pid}\"))"
+                "    file_transfer=FakeFileTransfer(source_folder=\"/upload/{uid}\"))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "15d15535-78c1-440f-b50e-626ea5457cd0",
             "metadata": {},
             "source": [
@@ -367,13 +367,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scitacean-23.4.0/docs/user-guide/uploading.ipynb` & `scitacean-23.5.0/docs/user-guide/uploading.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.10.10'}}"}*

```diff
@@ -318,13 +318,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scitacean-23.4.0/pyproject.toml` & `scitacean-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/requirements/base.txt` & `scitacean-23.5.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/requirements/ci.txt` & `scitacean-23.5.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/requirements/dev.txt` & `scitacean-23.5.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/requirements/docs.txt` & `scitacean-23.5.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/requirements/static.txt` & `scitacean-23.5.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/requirements/test.txt` & `scitacean-23.5.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/__init__.py` & `scitacean-23.5.0/src/scitacean/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/_dataset_fields.py` & `scitacean-23.5.0/src/scitacean/_dataset_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
         Arguments starting with an underscore are used internally to initialize
         datasets from SciCat models, and you should generally avoid setting them
         yourself!
         """
         _read_only = _read_only or {}
         self._fields = {
             "creation_time": _parse_datetime(creation_time),
-            "history": _apply_default(_read_only.get("history"), None, list),
+            "history": _apply_default(_read_only.get("history"), None, None),
             "pid": PID.parse(pid) if isinstance(pid, str) else pid,
             "type": DatasetType(type),
             "access_groups": _apply_default(access_groups, None, None),
             "classification": _apply_default(classification, None, None),
             "contact_email": _apply_default(contact_email, None, None),
             "created_at": _apply_default(_read_only.get("created_at"), None, None),
             "created_by": _apply_default(_read_only.get("created_by"), None, None),
```

### Comparing `scitacean-23.4.0/src/scitacean/_html_repr/__init__.py` & `scitacean-23.5.0/src/scitacean/_html_repr/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/_html_repr/images/lock.svg` & `scitacean-23.5.0/src/scitacean/_html_repr/images/lock.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/_html_repr/resources.py` & `scitacean-23.5.0/src/scitacean/_html_repr/resources.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/_html_repr/styles/dataset.css` & `scitacean-23.5.0/src/scitacean/_html_repr/styles/dataset.css`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/_html_repr/templates/dataset_repr.html.template` & `scitacean-23.5.0/src/scitacean/_html_repr/templates/dataset_repr.html.template`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/_internal/orcid.py` & `scitacean-23.5.0/src/scitacean/_internal/orcid.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/client.py` & `scitacean-23.5.0/src/scitacean/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,16 +207,19 @@
         scitacean.ScicatCommError
             If the upload to SciCat fails.
         RuntimeError
             If the file upload fails or if a critical error is encountered
             and some files or a partial dataset are left on the servers.
             Note the error message if that happens.
         """
-        if dataset.pid is None:
-            dataset = dataset.replace(pid=PID.generate())
+        if dataset.pid is not None:
+            raise ValueError(
+                "Cannot upload the dataset because it has a PID. "
+                "Set the PID to None, the server will assign one for you."
+            )
         dataset = dataset.replace(
             source_folder=self._expect_file_transfer().source_folder_for(dataset)
         )
         dataset.validate()
         with self._connect_for_file_upload(dataset) as con:
             # TODO check if any remote file is out of date.
             #  if so, raise an error. We never overwrite remote files!
@@ -367,30 +370,33 @@
         # TODO undo if later fails but only if no files were written
         target.mkdir(parents=True, exist_ok=True)
         files = _select_files(select, dataset)
         downloaded_files = [
             f.downloaded(local_path=target / f.remote_path.to_local()) for f in files
         ]
         if not force:
-            downloaded_files = _remove_up_to_date_local_files(
+            to_download = _remove_up_to_date_local_files(
                 downloaded_files, checksum_algorithm=checksum_algorithm
             )
-        if not downloaded_files:
-            return dataset.replace()
+        else:
+            to_download = downloaded_files
+
+        if not to_download:
+            return dataset.replace_files(*downloaded_files)
 
         with self._connect_for_file_download() as con:
             con.download_files(
                 remote=[
                     p
-                    for f in downloaded_files
+                    for f in to_download
                     if (p := f.remote_access_path(dataset.source_folder)) is not None
                 ],
-                local=[f.local_path for f in downloaded_files],
+                local=[f.local_path for f in to_download],
             )
-        for f in downloaded_files:
+        for f in to_download:
             f.validate_after_download()
         return dataset.replace_files(*downloaded_files)
 
     @contextmanager
     def _connect_for_file_download(self) -> Iterator[DownloadConnection]:
         if self.file_transfer is None:
             raise ValueError(
@@ -478,15 +484,15 @@
         Raises
         ------
         scitacean.ScicatCommError
             If the dataset does not exist or communication fails for some other reason.
         """
         dset_json = self._call_endpoint(
             cmd="get",
-            url=f"Datasets/{quote_plus(str(pid))}",
+            url=f"datasets/{quote_plus(str(pid))}",
             operation="get_dataset_model",
         )
         return model.construct(
             model.DerivedDataset
             if dset_json["type"] == "derived"
             else model.RawDataset,
             _strict_validation=strict_validation,
@@ -532,21 +538,21 @@
     def create_dataset_model(
         self, dset: Union[model.DerivedDataset, model.RawDataset]
     ) -> Union[model.DerivedDataset, model.RawDataset]:
         """Create a new dataset in SciCat.
 
         The dataset PID must be either
 
-        - ``None``, in which case SciCat assigns an ID.
-        - An unused id, in which case SciCat uses it for the new dataset.
+        - ``None``, in which case SciCat assigns an ID,
+        - an unused id, in which case SciCat uses it for the new dataset.
 
         If the ID already exists, creation will fail without
         modification to the database.
         Unless the new dataset is identical to the existing one,
-        in which case nothing happens.
+        in which case, nothing happens.
 
         Parameters
         ----------
         dset:
             Model of the dataset to create.
 
         Returns
@@ -557,15 +563,15 @@
         Raises
         ------
         scitacean.ScicatCommError
             If SciCat refuses the dataset or communication
             fails for some other reason.
         """
         uploaded = self._call_endpoint(
-            cmd="post", url="Datasets", data=dset, operation="create_dataset_model"
+            cmd="post", url="datasets", data=dset, operation="create_dataset_model"
         )
         return (
             model.DerivedDataset(**uploaded)
             if uploaded["type"] == "derived"
             else model.RawDataset(**uploaded)
         )
 
@@ -590,15 +596,15 @@
         scitacean.ScicatCommError
             If SciCat refuses the datablock or communication
             fails for some other reason.
         """
         return model.OrigDatablock(
             **self._call_endpoint(
                 cmd="post",
-                url=f"Datasets/{quote_plus(str(dblock.datasetId))}/origdatablocks",
+                url="origdatablocks",
                 data=dblock,
                 operation="create_orig_datablock",
             )
         )
 
     def _send_to_scicat(
         self, *, cmd: str, url: str, data: Optional[model.BaseModel] = None
@@ -646,15 +652,15 @@
     ) -> Any:
         full_url = _url_concat(self._base_url, url)
         logger = get_logger()
         logger.info("Calling SciCat API at %s for operation '%s'", full_url, operation)
 
         response = self._send_to_scicat(cmd=cmd, url=full_url, data=data)
         if not response.ok:
-            err = response.json().get("error", {})
+            err = response.json().get("message", {})
             logger.error("API call failed, endpoint: %s, response: %s", full_url, err)
             raise ScicatCommError(f"Error in operation {operation}: {err}")
         logger.info("API call successful for operation '%s'", operation)
         res = response.json()
         if not res:
             raise ScicatCommError(
                 f"{cmd} to {url} succeeded but di not return anything."
@@ -669,15 +675,16 @@
     b = b[1:] if b.endswith("/") else b
     return a + b
 
 
 def _strip_token(error: Any, token: str) -> str:
     error = str(error)
     error = re.sub(r"token=[\w\-./]+", "token=<HIDDEN>", error)
-    error = error.replace(token, "<HIDDEN>")
+    if token:  # token can be ""
+        error = error.replace(token, "<HIDDEN>")
     return error
 
 
 def _make_orig_datablock(
     fields: Dict[str, Any], strict_validation: bool
 ) -> model.OrigDatablock:
     files = [
```

### Comparing `scitacean-23.4.0/src/scitacean/datablock.py` & `scitacean-23.5.0/src/scitacean/datablock.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/dataset.py` & `scitacean-23.5.0/src/scitacean/dataset.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/file.py` & `scitacean-23.5.0/src/scitacean/file.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/filesystem.py` & `scitacean-23.5.0/src/scitacean/filesystem.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/logging.py` & `scitacean-23.5.0/src/scitacean/logging.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/model.py` & `scitacean-23.5.0/src/scitacean/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     _DatasetTypeBases = (
         str,
         _Enum,
     )
 
 import os
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Type, TypeVar
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import pydantic
 
 from ._internal.orcid import is_valid_orcid
 from .filesystem import RemotePath
 from .logging import get_logger
 from .pid import PID
@@ -36,17 +36,36 @@
 class DatasetType(*_DatasetTypeBases):
     """Type of Dataset"""
 
     RAW = "raw"
     DERIVED = "derived"
 
 
+# These fields are auto generated by MongoDB/Mongoose,
+# but we don't want them in Scitacean.
+# Drop them in the constructor if they are not in the model explicitly.
+_IGNORED_KWARGS = ("id", "_id", "_v")
+
+
+def _drop_ignored_args(
+    model: Union[pydantic.BaseModel, Type[pydantic.BaseModel]], args: Dict[str, Any]
+) -> None:
+    for key in _IGNORED_KWARGS:
+        if key not in model.__fields__:
+            args.pop(key, None)
+
+
 class BaseModel(pydantic.BaseModel):
+    def __init__(self, **kwargs: Any) -> None:
+        _drop_ignored_args(self, kwargs)
+        super().__init__(**kwargs)
+
     class Config:
-        extra = pydantic.Extra.forbid
+        # TODO remove when all v4 fields are supported
+        # extra = pydantic.Extra.forbid
         json_encoders = {
             PID: lambda v: str(v),
             RemotePath: lambda v: v.posix,
         }
 
 
 class DatasetLifecycle(BaseModel):
@@ -272,14 +291,15 @@
         Field values to pass to the model initializer.
 
     Returns
     -------
     :
         An initialized model.
     """
+    _drop_ignored_args(model, fields)
     try:
         return model(**fields)
     except pydantic.ValidationError as e:
         if _strict_validation:
             raise
         get_logger().warning(
             "Validation of metadata failed: %s\n"
```

### Comparing `scitacean-23.4.0/src/scitacean/pid.py` & `scitacean-23.5.0/src/scitacean/pid.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/testing/client.py` & `scitacean-23.5.0/src/scitacean/testing/client.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/testing/docs.py` & `scitacean-23.5.0/src/scitacean/testing/docs.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/testing/strategies.py` & `scitacean-23.5.0/src/scitacean/testing/strategies.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/testing/transfer.py` & `scitacean-23.5.0/src/scitacean/testing/transfer.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/transfer/ssh.py` & `scitacean-23.5.0/src/scitacean/transfer/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,16 +265,17 @@
     (Note that ``{name}`` is replaced by ``dset.name``.)
 
     .. code-block:: python
 
         file_transfer = SSHFileTransfer(host="fileserver",
                                         source_folder="transfer/{name}")
 
-    A useful approach is to include the PID in the source folder, for example
-    ``/some/base/folder/{pid.pid}``, to avoid clashes between different datasets.
+    A useful approach is to include a unique ID in the source folder, for example
+    ``"/some/base/folder/{uid}"``, to avoid clashes between different datasets.
+    Scitacean will fill in the ``"{uid}"`` placeholder with a new UUID4.
     """
 
     def __init__(
         self,
         *,
         host: str,
         port: Optional[int] = None,
```

### Comparing `scitacean-23.4.0/src/scitacean/transfer/util.py` & `scitacean-23.5.0/src/scitacean/transfer/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Common utilities for file transfers."""
 
 from typing import Optional, Union
+from uuid import uuid4
 
 from ..dataset import Dataset
 from ..filesystem import RemotePath
 from ..util.formatter import DatasetPathFormatter
 
 
 def source_folder_for(
@@ -34,8 +35,10 @@
                 "Either the dataset's source_folder or the "
                 "file transfer's source_folder must be set."
             )
         return dataset.source_folder
 
     if isinstance(pattern, RemotePath):
         pattern = pattern.posix
-    return RemotePath(DatasetPathFormatter().format(pattern, dataset))
+    return RemotePath(
+        DatasetPathFormatter().format(pattern, dset=dataset, uid=str(uuid4()))
+    )
```

### Comparing `scitacean-23.4.0/src/scitacean/typing.py` & `scitacean-23.5.0/src/scitacean/typing.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/util/credentials.py` & `scitacean-23.5.0/src/scitacean/util/credentials.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/src/scitacean/util/formatter.py` & `scitacean-23.5.0/src/scitacean/util/formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
 """String-formatting tools."""
 
-
 from string import Formatter
 from typing import Any, Iterator, Optional, Tuple
 
 from ..filesystem import escape_path
 
 
 class DatasetPathFormatter(Formatter):
@@ -14,40 +13,44 @@
 
     This formatter automatically modifies format strings such that the
     following two are equivalent (up to escaping, see below).
 
     .. code-block:: python
 
         formatter = DatasetPathFormatter()
-        formatter.format("{owner}-{pid.pid}", dset)
+        formatter.format("{owner}-{pid.pid}-{uid}", dset=dset, uid=uid)
         # is equivalent to (up to escaping)
-        "{0.owner}-{0.pid.pid}".format(dset)
+        "{dset.owner}-{dset.pid.pid}-{uid}".format(dset=dset, uid=uid)
 
     This means that all format fields are transformed to access attributes
-    for the first argument of ``format``. ``format`` thus supports only a
-    single argument.
+    of the keyword argument ``dset``.
+    Except for ``"uid"`` which is preserved to allow for a dedicated ``uid`` keyword.
 
     In addition, all field values are escaped as filesystem paths
     using :func:`scitacean.filesystem.escape_path`:
 
     .. code-block:: python
 
         formatter = DatasetPathFormatter()
-        formatter.format("a string {owner}", dset)
+        formatter.format("a string {owner}", dset=dset)
         # is equivalent to
-        "a string {}".format(escape_path("{0.owner}".format(dset)))
+        "a string {}".format(escape_path("{dset.owner}".format(dset=dset)))
 
     Note that only formatted fields are escaped, not the result as a whole.
     """
 
     def parse(
         self, format_string: str
     ) -> Iterator[Tuple[str, Optional[str], Optional[str], Optional[str]]]:
         def add0(field_name: Optional[str]) -> Optional[str]:
-            return "0." + field_name if isinstance(field_name, str) else None
+            if field_name == "uid":
+                return field_name
+            if isinstance(field_name, str):
+                return "dset." + field_name
+            return None
 
         return map(
             lambda t: (t[0], add0(t[1]), t[2], t[3]), super().parse(format_string)
         )
 
     def format_field(self, value: Any, format_spec: str) -> str:
         return escape_path(super().format_field(value, format_spec))
```

### Comparing `scitacean-23.4.0/src/scitacean.egg-info/PKG-INFO` & `scitacean-23.5.0/src/scitacean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 23.4.0
+Version: 23.5.0
 Summary: High-level interface for SciCat
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `scitacean-23.4.0/src/scitacean.egg-info/SOURCES.txt` & `scitacean-23.5.0/src/scitacean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/client_test.py` & `scitacean-23.5.0/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/common/backend.py` & `scitacean-23.5.0/tests/common/backend.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/common/docker-compose-ssh-server.yaml` & `scitacean-23.5.0/tests/common/docker-compose-ssh-server.yaml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/common/docker.py` & `scitacean-23.5.0/tests/common/docker.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/common/files.py` & `scitacean-23.5.0/tests/common/files.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/common/ssh_server.py` & `scitacean-23.5.0/tests/common/ssh_server.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/conftest.py` & `scitacean-23.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/data/__init__.py` & `scitacean-23.5.0/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/data/datasets.json` & `scitacean-23.5.0/tests/data/datasets.json`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/data/orig_datablocks.json` & `scitacean-23.5.0/tests/data/orig_datablocks.json`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/dataset_fields_test.py` & `scitacean-23.5.0/tests/dataset_fields_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     assert abs(dset.creation_time - datetime.now(tz=timezone.utc)) < timedelta(
         seconds=30
     )
 
 
 def test_init_dataset_default_values():
     dset = Dataset(type="derived")
-    assert dset.history == []
+    assert dset.history is None
     assert dset.is_published is False
     assert dset.meta == {}
 
 
 @pytest.mark.parametrize("field", Dataset.fields(read_only=True), ids=lambda f: f.name)
 def test_cannot_set_read_only_fields(field):
     dset = Dataset(type="raw")
@@ -308,15 +308,15 @@
         contactEmail="p.stibbons@uu.am",
         creationTime=dateutil.parser.parse("2142-04-02T16:44:56"),
         owner="Ponder Stibbons;Mustrum Ridcully",
         ownerGroup="faculty",
         principalInvestigator="my principal investigator",
         sourceFolder=RemotePath("/hex/source62"),
         type=DatasetType.RAW,
-        history=[],
+        history=None,
         isPublished=False,
         scientificMetadata={},
         creationLocation="ANK/UU",
         sharedWith=["librarian", "hicks"],
         numberOfFiles=0,
         numberOfFilesArchived=0,
         packedSize=0,
@@ -342,15 +342,15 @@
         contactEmail="p.stibbons@uu.am;m.ridcully@uu.am",
         creationTime=dateutil.parser.parse("2142-04-02T16:44:56"),
         owner="Ponder Stibbons;Mustrum Ridcully",
         ownerGroup="faculty",
         investigator="p.stibbons@uu.am",
         sourceFolder=RemotePath("/hex/source62"),
         type=DatasetType.DERIVED,
-        history=[],
+        history=None,
         isPublished=False,
         scientificMetadata={"weight": {"value": 5.23, "unit": "kg"}},
         inputDatasets=[PID(pid="623-122")],
         usedSoftware=["scitacean", "magick"],
         numberOfFiles=0,
         numberOfFilesArchived=0,
         packedSize=0,
@@ -380,14 +380,15 @@
         source_folder=RemotePath("/hex/source62"),
     )
     setattr(dset, field.name, data.draw(st.from_type(field.type)))
     with pytest.raises(ValueError):
         dset.make_model()
 
 
+@pytest.mark.skip("Validation is less strict until full migration to v4")
 @pytest.mark.parametrize(
     "field",
     filter(
         lambda f: not f.used_by_derived,
         Dataset.fields(dataset_type="raw", read_only=False),
     ),
     ids=lambda f: f.name,
```

### Comparing `scitacean-23.4.0/tests/dataset_test.py` & `scitacean-23.5.0/tests/dataset_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
 @settings(max_examples=5)
 def test_as_new(initial):
     new = initial.as_new()
     assert new.created_at is None
     assert new.created_by is None
     assert new.updated_at is None
     assert new.updated_by is None
-    assert new.history == []
+    assert new.history is None
     assert new.lifecycle is None
     assert abs(new.creation_time - datetime.now(tz=timezone.utc)) < timedelta(seconds=1)
 
     assert new.number_of_files == initial.number_of_files
     assert new.size == initial.size
     assert new.name == initial.name
     assert new.input_datasets == initial.input_datasets
@@ -331,15 +331,15 @@
 @given(sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=5)
 def test_derive_default(initial):
     derived = initial.derive()
     assert derived.type == "derived"
     assert derived.input_datasets == [initial.pid]
     assert derived.lifecycle is None
-    assert derived.history == []
+    assert derived.history is None
 
     assert derived.investigator == initial.investigator
     assert derived.owner == initial.owner
     assert derived.orcid_of_owner == initial.orcid_of_owner
     assert derived.owner_email == initial.owner_email
     assert derived.contact_email == initial.contact_email
     assert derived.techniques == initial.techniques
@@ -353,15 +353,15 @@
 @given(sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=5)
 def test_derive_set_keep(initial):
     derived = initial.derive(keep=("name", "used_software"))
     assert derived.type == "derived"
     assert derived.input_datasets == [initial.pid]
     assert derived.lifecycle is None
-    assert derived.history == []
+    assert derived.history is None
 
     assert derived.name == initial.name
     assert derived.used_software == initial.used_software
 
     assert derived.number_of_files == 0
     assert derived.number_of_files_archived == 0
 
@@ -369,15 +369,15 @@
 @given(sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=5)
 def test_derive_keep_nothing(initial):
     derived = initial.derive(keep=())
     assert derived.type == "derived"
     assert derived.input_datasets == [initial.pid]
     assert derived.lifecycle is None
-    assert derived.history == []
+    assert derived.history is None
 
     assert derived.investigator is None
     assert derived.owner is None
     assert derived.name is None
     assert derived.used_software is None
     assert derived.number_of_files == 0
     assert derived.number_of_files_archived == 0
```

### Comparing `scitacean-23.4.0/tests/download_test.py` & `scitacean-23.5.0/tests/download_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -279,15 +279,16 @@
             raise RuntimeError("Download disabled")
 
     client = Client.without_login(
         url="/",
         file_transfer=RaisingDownloader(fs=fs),
     )
     # Does not raise
-    client.download_files(dataset, target="./download", select=True)
+    downloaded = client.download_files(dataset, target="./download", select=True)
+    assert all(file.local_path is not None for file in downloaded.files)
 
 
 def test_download_does_not_download_up_to_date_file_manual_checksum(
     fs, dataset_and_files
 ):
     # Ensure the file exists locally
     dataset, contents = dataset_and_files
@@ -305,17 +306,18 @@
             raise RuntimeError("Download disabled")
 
     client = Client.without_login(
         url="/",
         file_transfer=RaisingDownloader(fs=fs),
     )
     # Does not raise
-    client.download_files(
+    downloaded = client.download_files(
         dataset, target="./download", select=True, checksum_algorithm="md5"
     )
+    assert all(file.local_path is not None for file in downloaded.files)
 
 
 def test_force_file_download(fs, dataset_and_files):
     # Ensure the file exists locally
     dataset, contents = dataset_and_files
     client = Client.without_login(
         url="/", file_transfer=FakeFileTransfer(fs=fs, files=contents)
```

### Comparing `scitacean-23.4.0/tests/file_test.py` & `scitacean-23.5.0/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/filesystem_test.py` & `scitacean-23.5.0/tests/filesystem_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/html_repr/html_repr_test.py` & `scitacean-23.5.0/tests/html_repr/html_repr_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/model_test.py` & `scitacean-23.5.0/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/testing/strategies_test.py` & `scitacean-23.5.0/tests/testing/strategies_test.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tests/transfer/ssh_test.py` & `scitacean-23.5.0/tests/transfer/ssh_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2022 Scitacean contributors (https://github.com/SciCatProject/scitacean)
 import dataclasses
+import re
 import tempfile
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
+from uuid import uuid4
 
 import fabric
 import paramiko
 import pytest
 
 from scitacean import Dataset, File, FileUploadError, RemotePath
 from scitacean.transfer.ssh import SSHFileTransfer
@@ -69,30 +71,31 @@
 def test_upload_one_file_source_folder_in_transfer(
     ssh_access, ssh_connect_with_username_password, tmp_path, ssh_data_dir
 ):
     ds = Dataset(type="raw", pid="abcd-12")
     with open(tmp_path / "file1.txt", "w") as f:
         f.write("File no. 2")
 
+    source_uid = str(uuid4())
     ssh = SSHFileTransfer(
         host=ssh_access.host,
         port=ssh_access.port,
-        source_folder="/data/upload/{pid.pid}",
+        source_folder=f"/data/upload/{source_uid}",
     )
     with ssh.connect_for_upload(
         dataset=ds, connect=ssh_connect_with_username_password
     ) as con:
-        assert con.source_folder == RemotePath("/data/upload/abcd-12")
+        assert re.match(r"/data/upload/[a-d0-9\-]+", con.source_folder.posix)
         con.upload_files(
             File.from_local(
                 path=tmp_path / "file1.txt", remote_path=RemotePath("upload_1.txt")
             )
         )
 
-    with open(ssh_data_dir / "upload" / "abcd-12" / "upload_1.txt", "r") as f:
+    with open(ssh_data_dir / "upload" / source_uid / "upload_1.txt", "r") as f:
         assert f.read() == "File no. 2"
 
 
 def test_upload_two_files(
     ssh_access, ssh_connect_with_username_password, tmp_path, ssh_data_dir
 ):
     ds = Dataset(type="raw", source_folder=RemotePath("/data/upload2"))
```

### Comparing `scitacean-23.4.0/tests/upload_test.py` & `scitacean-23.5.0/tests/upload_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,23 +88,14 @@
         }
     )
     assert finalized == expected
     with pytest.raises(ScicatCommError):
         client.scicat.get_orig_datablocks(finalized.pid)
 
 
-def test_upload_uses_given_pid(client, derived_dataset_model):
-    derived_dataset_model.pid = "my-custom-id"
-    dataset = Dataset.from_models(
-        dataset_model=derived_dataset_model, orig_datablock_models=None
-    )
-    finalized = client.upload_new_dataset_now(dataset)
-    assert "my-custom-id" in str(finalized.pid)
-
-
 def test_upload_creates_dataset_and_datablock(client, dataset):
     finalized = client.upload_new_dataset_now(dataset)
     assert client.datasets[finalized.pid] == finalized.make_model()
     assert (
         client.orig_datablocks[finalized.pid]
         == finalized.make_datablock_models().orig_datablocks
     )
```

### Comparing `scitacean-23.4.0/tools/model-generation/dataset.py` & `scitacean-23.5.0/tools/model-generation/dataset.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/generate.py` & `scitacean-23.5.0/tools/model-generation/generate.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/model.py` & `scitacean-23.5.0/tools/model-generation/model.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/__init__.py` & `scitacean-23.5.0/tools/model-generation/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/data-file.yml` & `scitacean-23.5.0/tools/model-generation/spec/data-file.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/datablock.yml` & `scitacean-23.5.0/tools/model-generation/spec/datablock.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/dataset-lifecycle.yml` & `scitacean-23.5.0/tools/model-generation/spec/dataset-lifecycle.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/dataset.yml` & `scitacean-23.5.0/tools/model-generation/spec/dataset.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/mongo-queryable.yml` & `scitacean-23.5.0/tools/model-generation/spec/mongo-queryable.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/orig-datablock.yml` & `scitacean-23.5.0/tools/model-generation/spec/orig-datablock.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/spec/ownable.yml` & `scitacean-23.5.0/tools/model-generation/spec/ownable.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/templates/__init__.py` & `scitacean-23.5.0/tools/model-generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `scitacean-23.4.0/tools/model-generation/templates/dataset.py.template` & `scitacean-23.5.0/tools/model-generation/templates/dataset.py.template`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         Arguments starting with an underscore are used internally to initialize
         datasets from SciCat models, and you should generally avoid setting them
         yourself!
         """
         _read_only = _read_only or {}
         self._fields = {
             "creation_time": _parse_datetime(creation_time),
-            "history": _apply_default(_read_only.get("history"), None, list),
+            "history": _apply_default(_read_only.get("history"), None, None),
             "pid": PID.parse(pid) if isinstance(pid, str) else pid,
             "type": DatasetType(type),
 $field_dict_construction
         }
         self._orig_datablocks = (
             [] if _orig_datablocks is None else list(_orig_datablocks)
         )
```

### Comparing `scitacean-23.4.0/tox.ini` & `scitacean-23.5.0/tox.ini`

 * *Files identical despite different names*

