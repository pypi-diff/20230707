# Comparing `tmp/autora-core-3.2.0a1.tar.gz` & `tmp/autora-core-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-core-3.2.0a1.tar", last modified: Wed Jun 28 18:48:54 2023, max compression
+gzip compressed data, was "autora-core-3.3.0.tar", last modified: Fri Jul  7 20:56:55 2023, max compression
```

## Comparing `autora-core-3.2.0a1.tar` & `autora-core-3.3.0.tar`

### file list

```diff
@@ -1,66 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.731861 autora-core-3.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.723862 autora-core-3.2.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.723862 autora-core-3.2.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/CONTRIBUTE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-28 18:48:54.731861 autora-core-3.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.719861 autora-core-3.2.0a1/docs/experimentalists/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.719861 autora-core-3.2.0a1/docs/experimentalists/pooler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/docs/experimentalists/pooler/grid/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/experimentalists/pooler/grid/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/experimentalists/pooler/grid/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/docs/experimentalists/pooler/random/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/experimentalists/pooler/random/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/experimentalists/pooler/random/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.719861 autora-core-3.2.0a1/docs/experimentalists/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/docs/experimentalists/sampler/random/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/experimentalists/sampler/random/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/experimentalists/sampler/random/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/docs/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/docs/pipeline/Experimentalist Pipeline Examples.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 18:48:54.735862 autora-core-3.2.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.719861 autora-core-3.2.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.719861 autora-core-3.2.0a1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/src/autora/experimentalist/
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/experimentalist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.727862 autora-core-3.2.0a1/src/autora/experimentalist/pooler/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/experimentalist/pooler/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/experimentalist/pooler/random_pooler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.731861 autora-core-3.2.0a1/src/autora/experimentalist/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/experimentalist/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/experimentalist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.731861 autora-core-3.2.0a1/src/autora/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/utils/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.731861 autora-core-3.2.0a1/src/autora/variable/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/variable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/src/autora/variable/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.731861 autora-core-3.2.0a1/src/autora_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-28 18:48:54.000000 autora-core-3.2.0a1/src/autora_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-28 18:48:54.000000 autora-core-3.2.0a1/src/autora_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 18:48:54.000000 autora-core-3.2.0a1/src/autora_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-28 18:48:54.000000 autora-core-3.2.0a1/src/autora_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 18:48:54.000000 autora-core-3.2.0a1/src/autora_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:48:54.731861 autora-core-3.2.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/tests/test_experimentalist_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-28 18:48:38.000000 autora-core-3.2.0a1/tests/test_experimentalist_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.872944 autora-core-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-07 20:56:43.000000 autora-core-3.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.860944 autora-core-3.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-07 20:56:43.000000 autora-core-3.3.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-07 20:56:43.000000 autora-core-3.3.0/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 20:56:43.000000 autora-core-3.3.0/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-07 20:56:43.000000 autora-core-3.3.0/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-07 20:56:43.000000 autora-core-3.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-07 20:56:43.000000 autora-core-3.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:43.000000 autora-core-3.3.0/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 20:56:43.000000 autora-core-3.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 20:56:43.000000 autora-core-3.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-07 20:56:43.000000 autora-core-3.3.0/CONTRIBUTE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 20:56:43.000000 autora-core-3.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-07 20:56:55.872944 autora-core-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-07 20:56:43.000000 autora-core-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/docs/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)   376928 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/cycle/Linear and Cyclical Workflows using Functions and States.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.860944 autora-core-3.3.0/docs/experimentalists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.856944 autora-core-3.3.0/docs/experimentalists/pooler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/docs/experimentalists/pooler/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/experimentalists/pooler/grid/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/experimentalists/pooler/grid/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/docs/experimentalists/pooler/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/experimentalists/pooler/random/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/experimentalists/pooler/random/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.860944 autora-core-3.3.0/docs/experimentalists/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/docs/experimentalists/sampler/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/experimentalists/sampler/random/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/experimentalists/sampler/random/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/docs/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-07 20:56:43.000000 autora-core-3.3.0/docs/pipeline/Experimentalist Pipeline Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 20:56:43.000000 autora-core-3.3.0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-07 20:56:43.000000 autora-core-3.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-07 20:56:43.000000 autora-core-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:56:55.872944 autora-core-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.860944 autora-core-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.860944 autora-core-3.3.0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.864944 autora-core-3.3.0/src/autora/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/experimentalist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.868944 autora-core-3.3.0/src/autora/experimentalist/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/experimentalist/pooler/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/experimentalist/pooler/random_pooler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.868944 autora-core-3.3.0/src/autora/experimentalist/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/experimentalist/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/experimentalist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.868944 autora-core-3.3.0/src/autora/state/
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/state/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29514 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/state/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/state/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/state/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.868944 autora-core-3.3.0/src/autora/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/utils/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.868944 autora-core-3.3.0/src/autora/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-07 20:56:43.000000 autora-core-3.3.0/src/autora/variable/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.868944 autora-core-3.3.0/src/autora_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-07 20:56:55.000000 autora-core-3.3.0/src/autora_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-07 20:56:55.000000 autora-core-3.3.0/src/autora_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:56:55.000000 autora-core-3.3.0/src/autora_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-07 20:56:55.000000 autora-core-3.3.0/src/autora_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 20:56:55.000000 autora-core-3.3.0/src/autora_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:56:55.872944 autora-core-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 20:56:43.000000 autora-core-3.3.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-07-07 20:56:43.000000 autora-core-3.3.0/tests/test_experimentalist_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-07 20:56:43.000000 autora-core-3.3.0/tests/test_experimentalist_random.py
```

### Comparing `autora-core-3.2.0a1/.github/pull_request_template.md` & `autora-core-3.3.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/.github/workflows/publish-package-pypi.yml` & `autora-core-3.3.0/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/.github/workflows/test-pytest.yml` & `autora-core-3.3.0/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/.gitignore` & `autora-core-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/.pre-commit-config.yaml` & `autora-core-3.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/CONTRIBUTE.md` & `autora-core-3.3.0/CONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/LICENSE.md` & `autora-core-3.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/PKG-INFO` & `autora-core-3.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.2.0a1
+Version: 3.3.0
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-core
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-core-3.2.0a1/README.md` & `autora-core-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/docs/experimentalists/pooler/grid/index.md` & `autora-core-3.3.0/docs/experimentalists/pooler/grid/index.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/docs/experimentalists/pooler/random/index.md` & `autora-core-3.3.0/docs/experimentalists/pooler/random/index.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/docs/pipeline/Experimentalist Pipeline Examples.ipynb` & `autora-core-3.3.0/docs/pipeline/Experimentalist Pipeline Examples.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/mkdocs/base.yml` & `autora-core-3.3.0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/pyproject.toml` & `autora-core-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/src/autora/experimentalist/pipeline.py` & `autora-core-3.3.0/src/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/src/autora/experimentalist/pooler/grid.py` & `autora-core-3.3.0/src/autora/experimentalist/pooler/grid.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/src/autora/experimentalist/pooler/random_pooler.py` & `autora-core-3.3.0/src/autora/experimentalist/pooler/random_pooler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 import random
+from typing import Iterable, List, Tuple
 
 import numpy as np
 
 from autora.utils.deprecation import deprecated_alias
+from autora.variable import IV
 
 
-def random_pool(*args, n: int = 1, duplicates: bool = True):
+def random_pool(
+    ivs: List[IV], num_samples: int = 1, duplicates: bool = True
+) -> Iterable:
     """
     Creates combinations from lists of discrete values using random selection.
     Args:
-        *args: m lists of discrete values. One value will be sampled from each list.
+        ivs: List of independent variables
         n: Number of samples to sample
         duplicates: Boolean if duplicate value are allowed.
 
     """
-    l_samples = []
+    l_samples: List[Tuple] = []
     # Create list of pools of values sample from
-    pools = [tuple(pool) for pool in args]
+    l_iv_values = []
+    for iv in ivs:
+        assert iv.allowed_values is not None, (
+            f"gridsearch_pool only supports independent variables with discrete allowed values, "
+            f"but allowed_values is None on {iv=} "
+        )
+        l_iv_values.append(iv.allowed_values)
 
     # Check to ensure infinite search won't occur if duplicates not allowed
     if not duplicates:
-        l_pool_len = [len(set(s)) for s in pools]
+        l_pool_len = [len(set(s)) for s in l_iv_values]
         n_combinations = np.product(l_pool_len)
         try:
-            assert n <= n_combinations
+            assert num_samples <= n_combinations
         except AssertionError:
             raise AssertionError(
-                f"Number to sample n({n}) is larger than the number "
+                f"Number to sample n({num_samples}) is larger than the number "
                 f"of unique combinations({n_combinations})."
             )
 
     # Random sample from the pools until n is met
-    while len(l_samples) < n:
-        l_samples.append(tuple(map(random.choice, pools)))
+    while len(l_samples) < num_samples:
+        l_samples.append(tuple(map(random.choice, l_iv_values)))
         if not duplicates:
             l_samples = [*set(l_samples)]
 
     return iter(l_samples)
 
 
 random_pooler = deprecated_alias(random_pool, "random_pooler")
```

### Comparing `autora-core-3.2.0a1/src/autora/experimentalist/sampler/random_sampler.py` & `autora-core-3.3.0/src/autora/experimentalist/sampler/random_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import random
 from typing import Iterable, Sequence, Union
 
 from autora.utils.deprecation import deprecated_alias
 
 
-def random_sample(conditions: Union[Iterable, Sequence], n: int = 1):
+def random_sample(conditions: Union[Iterable, Sequence], num_samples: int = 1):
     """
     Uniform random sampling without replacement from a pool of conditions.
     Args:
         conditions: Pool of conditions
         n: number of samples to collect
 
     Returns: Sampled pool
 
     """
 
     if isinstance(conditions, Iterable):
         conditions = list(conditions)
     random.shuffle(conditions)
-    samples = conditions[0:n]
+    samples = conditions[0:num_samples]
 
     return samples
 
 
 random_sampler = deprecated_alias(random_sample, "random_sampler")
```

### Comparing `autora-core-3.2.0a1/src/autora/experimentalist/utils.py` & `autora-core-3.3.0/src/autora/experimentalist/utils.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/src/autora/utils/deprecation.py` & `autora-core-3.3.0/src/autora/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/src/autora/variable/__init__.py` & `autora-core-3.3.0/src/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/src/autora/variable/time.py` & `autora-core-3.3.0/src/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/src/autora_core.egg-info/PKG-INFO` & `autora-core-3.3.0/src/autora_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.2.0a1
+Version: 3.3.0
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-core
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-core-3.2.0a1/src/autora_core.egg-info/SOURCES.txt` & `autora-core-3.3.0/src/autora_core.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,33 +4,41 @@
 CONTRIBUTE.md
 LICENSE.md
 README.md
 mkdocs.yml
 pyproject.toml
 .github/pull_request_template.md
 .github/workflows/publish-package-pypi.yml
+.github/workflows/test-pre-commit-hooks.yml
 .github/workflows/test-pytest.yml
 .vscode/.gitignore
 .vscode/extensions.json
 .vscode/launch.json
 docs/index.md
+docs/cycle/Linear and Cyclical Workflows using Functions and States.ipynb
 docs/experimentalists/pooler/grid/index.md
 docs/experimentalists/pooler/grid/quickstart.md
 docs/experimentalists/pooler/random/index.md
 docs/experimentalists/pooler/random/quickstart.md
 docs/experimentalists/sampler/random/index.md
 docs/experimentalists/sampler/random/quickstart.md
 docs/javascripts/mathjax.js
 docs/pipeline/Experimentalist Pipeline Examples.ipynb
 mkdocs/base.yml
 src/autora/experimentalist/pipeline.py
 src/autora/experimentalist/utils.py
 src/autora/experimentalist/pooler/grid.py
 src/autora/experimentalist/pooler/random_pooler.py
 src/autora/experimentalist/sampler/random_sampler.py
+src/autora/state/delta.py
+src/autora/state/history.py
+src/autora/state/param.py
+src/autora/state/protocol.py
+src/autora/state/snapshot.py
+src/autora/state/wrapper.py
 src/autora/utils/deprecation.py
 src/autora/utils/dictionary.py
 src/autora/variable/__init__.py
 src/autora/variable/time.py
 src/autora_core.egg-info/PKG-INFO
 src/autora_core.egg-info/SOURCES.txt
 src/autora_core.egg-info/dependency_links.txt
```

### Comparing `autora-core-3.2.0a1/tests/README.md` & `autora-core-3.3.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/tests/test_experimentalist_pipeline.py` & `autora-core-3.3.0/tests/test_experimentalist_pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.2.0a1/tests/test_experimentalist_random.py` & `autora-core-3.3.0/tests/test_experimentalist_random.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 from functools import partial
 
 import numpy as np
 import pytest
 
 from autora.experimentalist.pipeline import make_pipeline
 from autora.experimentalist.pooler.grid import grid_pool
+from autora.experimentalist.pooler.random_pooler import random_pool
 from autora.experimentalist.sampler.random_sampler import random_sample
 from autora.variable import DV, IV, ValueType, VariableCollection
 
 
 def weber_filter(values):
     return filter(lambda s: s[0] <= s[1], values)
 
 
-def test_random_experimentalist(metadata):
+def test_random_pooler_experimentalist(metadata):
+    """
+    Tests the implementation of a random pooler.
+    """
+    num_samples = 10
+
+    conditions = random_pool(metadata.independent_variables, num_samples=num_samples)
+
+    conditions = np.array(list(conditions))
+
+    assert conditions.shape[0] == num_samples
+    assert conditions.shape[1] == len(metadata.independent_variables)
+    for condition in conditions:
+        for idx, value in enumerate(condition):
+            assert value in metadata.independent_variables[idx].allowed_values
+
+
+def test_random_sampler_experimentalist(metadata):
     """
     Tests the implementation of the experimentalist pipeline with an exhaustive pool of discrete
     values, Weber filter, random selector. Tests two different implementations of the pool function
     as a callable and passing in as interator/generator.
 
     """
 
     n_trials = 25  # Number of trails for sampler to select
 
     # ---Implementation 1 - Pool using Callable via partial function----
     # Set up pipeline functions with partial
     pooler_callable = partial(grid_pool, ivs=metadata.independent_variables)
-    sampler = partial(random_sample, n=n_trials)
+    sampler = partial(random_sample, num_samples=n_trials)
     pipeline_random_samp = make_pipeline(
         [pooler_callable, weber_filter, sampler],
     )
 
     results = pipeline_random_samp.run()
 
     # ***Checks***
@@ -60,15 +78,15 @@
     )
 
 
 def test_random_experimentalist_generator(metadata):
     n_trials = 25  # Number of trails for sampler to select
 
     pooler_generator = grid_pool(metadata.independent_variables)
-    sampler = partial(random_sample, n=n_trials)
+    sampler = partial(random_sample, num_samples=n_trials)
     pipeline_random_samp_poolgen = make_pipeline(
         [pooler_generator, weber_filter, sampler]
     )
 
     results_poolgen = list(pipeline_random_samp_poolgen.run())
 
     # Is sampling the number of trials we expect
```

