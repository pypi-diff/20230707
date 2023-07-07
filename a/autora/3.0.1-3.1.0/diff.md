# Comparing `tmp/autora-3.0.1.tar.gz` & `tmp/autora-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-3.0.1.tar", last modified: Fri Jun  2 17:26:48 2023, max compression
+gzip compressed data, was "autora-3.1.0.tar", last modified: Fri Jul  7 15:49:03 2023, max compression
```

## Comparing `autora-3.0.1.tar` & `autora-3.1.0.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 17:26:37.000000 autora-3.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 17:26:37.000000 autora-3.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 17:26:37.000000 autora-3.0.1/.github/workflows/publish-documentation-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 17:26:37.000000 autora-3.0.1/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 17:26:37.000000 autora-3.0.1/.github/workflows/test-pre-commit-hooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 17:26:37.000000 autora-3.0.1/.github/workflows/test-pypi-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-02 17:26:37.000000 autora-3.0.1/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-02 17:26:37.000000 autora-3.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/autora.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 17:26:37.000000 autora-3.0.1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-02 17:26:37.000000 autora-3.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:37.000000 autora-3.0.1/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 17:26:37.000000 autora-3.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-02 17:26:37.000000 autora-3.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 17:26:37.000000 autora-3.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-02 17:26:37.000000 autora-3.0.1/MAINTAINING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-02 17:26:48.695572 autora-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-02 17:26:37.000000 autora-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/docs/contribute/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 17:26:37.000000 autora-3.0.1/docs/contribute/core.md
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-02 17:26:37.000000 autora-3.0.1/docs/contribute/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-02 17:26:37.000000 autora-3.0.1/docs/contribute/module.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-02 17:26:37.000000 autora-3.0.1/docs/contribute/pre-commit-hooks.md
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-02 17:26:37.000000 autora-3.0.1/docs/contribute/setup.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/docs/experiment-runner/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 17:26:37.000000 autora-3.0.1/docs/experiment-runner/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/docs/experimentalist/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-02 17:26:37.000000 autora-3.0.1/docs/experimentalist/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 17:26:37.000000 autora-3.0.1/docs/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.691573 autora-3.0.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   189630 2023-06-02 17:26:37.000000 autora-3.0.1/docs/img/experimentalist.png
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-06-02 17:26:37.000000 autora-3.0.1/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-06-02 17:26:37.000000 autora-3.0.1/docs/img/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-02 17:26:37.000000 autora-3.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 17:26:37.000000 autora-3.0.1/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/docs/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-02 17:26:37.000000 autora-3.0.1/docs/theorist/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 17:26:37.000000 autora-3.0.1/docs/tutorials/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.687572 autora-3.0.1/mkdocs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-02 17:26:37.000000 autora-3.0.1/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-02 17:26:37.000000 autora-3.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-02 17:26:37.000000 autora-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:26:48.695572 autora-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 17:26:37.000000 autora-3.0.1/src/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/src/autora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-02 17:26:48.000000 autora-3.0.1/src/autora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-02 17:26:48.000000 autora-3.0.1/src/autora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:26:48.000000 autora-3.0.1/src/autora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-02 17:26:48.000000 autora-3.0.1/src/autora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:26:48.000000 autora-3.0.1/src/autora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:26:48.695572 autora-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 17:26:37.000000 autora-3.0.1/tests/test_core_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.697049 autora-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 15:48:52.000000 autora-3.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.689048 autora-3.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-07 15:48:52.000000 autora-3.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.689048 autora-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-07 15:48:52.000000 autora-3.1.0/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-07 15:48:52.000000 autora-3.1.0/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 15:48:52.000000 autora-3.1.0/.github/workflows/test-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 15:48:52.000000 autora-3.1.0/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 15:48:52.000000 autora-3.1.0/.github/workflows/test-pypi-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-07 15:48:52.000000 autora-3.1.0/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-07 15:48:52.000000 autora-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-07 15:48:52.000000 autora-3.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.689048 autora-3.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:48:52.000000 autora-3.1.0/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 15:48:52.000000 autora-3.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 15:48:52.000000 autora-3.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 15:48:52.000000 autora-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-07 15:48:52.000000 autora-3.1.0/MAINTAINING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-07 15:49:03.697049 autora-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-07 15:48:52.000000 autora-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.689048 autora-3.1.0/autora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-07 15:49:03.000000 autora-3.1.0/autora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-07 15:49:03.000000 autora-3.1.0/autora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:49:03.000000 autora-3.1.0/autora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-07 15:49:03.000000 autora-3.1.0/autora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:49:03.000000 autora-3.1.0/autora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.689048 autora-3.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/contribute/
+-rw-r--r--   0 runner    (1001) docker     (123)   918314 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/Notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/core.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/contribute/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/modules/experiment-runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/modules/experimentalist.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/modules/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/modules/theorist.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/pre-commit-hooks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-07 15:48:52.000000 autora-3.1.0/docs/contribute/setup.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/experiment-runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 15:48:52.000000 autora-3.1.0/docs/experiment-runner/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-07 15:48:52.000000 autora-3.1.0/docs/experimentalist/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   153857 2023-07-07 15:48:52.000000 autora-3.1.0/docs/img/experiment_runner.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160409 2023-07-07 15:48:52.000000 autora-3.1.0/docs/img/experimentalist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-07-07 15:48:52.000000 autora-3.1.0/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   188766 2023-07-07 15:48:52.000000 autora-3.1.0/docs/img/modules_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   340646 2023-07-07 15:48:52.000000 autora-3.1.0/docs/img/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68999 2023-07-07 15:48:52.000000 autora-3.1.0/docs/img/package_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150962 2023-07-07 15:48:52.000000 autora-3.1.0/docs/img/theorist.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-07 15:48:52.000000 autora-3.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-07 15:48:52.000000 autora-3.1.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 15:48:52.000000 autora-3.1.0/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/online-experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-07 15:48:52.000000 autora-3.1.0/docs/online-experiments/firebase.md
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 15:48:52.000000 autora-3.1.0/docs/online-experiments/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.693048 autora-3.1.0/docs/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-07 15:48:52.000000 autora-3.1.0/docs/theorist/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.697049 autora-3.1.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   431620 2023-07-07 15:48:52.000000 autora-3.1.0/docs/tutorials/Experimentalist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   398855 2023-07-07 15:48:52.000000 autora-3.1.0/docs/tutorials/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   236210 2023-07-07 15:48:52.000000 autora-3.1.0/docs/tutorials/Theorist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-07 15:48:52.000000 autora-3.1.0/docs/tutorials/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.697049 autora-3.1.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-07 15:48:52.000000 autora-3.1.0/mkdocs/generate_code_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 15:48:52.000000 autora-3.1.0/mkdocs/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.697049 autora-3.1.0/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 15:48:52.000000 autora-3.1.0/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-07-07 15:48:52.000000 autora-3.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-07 15:48:52.000000 autora-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:49:03.697049 autora-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:49:03.697049 autora-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 15:48:52.000000 autora-3.1.0/tests/test_core_imports.py
```

### Comparing `autora-3.0.1/.github/pull_request_template.md` & `autora-3.1.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.1/.github/workflows/publish-documentation-gh-pages.yml` & `autora-3.1.0/.github/workflows/publish-documentation-gh-pages.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 name: Publish Documentation to GitHub Pages
 
 on:
+  push:
+    branches:
+      - 'main' # when someone pushes to the 'main' branch
+  schedule:
+    - cron: '59 3 * * *' # this triggers deployment every night at 3:59 UTC / 23:59 EST
   workflow_dispatch:  # this allows us to run it manually
   release:
     types: [released]  # only deploy when we make a new `latest` release
 
 permissions:
   contents: write
```

### Comparing `autora-3.0.1/.github/workflows/publish-package-pypi.yml` & `autora-3.1.0/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.1/.github/workflows/test-pre-commit-hooks.yml` & `autora-3.1.0/.github/workflows/test-pre-commit-hooks.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.1/.github/workflows/test-pytest.yml` & `autora-3.1.0/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.1/.gitignore` & `autora-3.1.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -67,7 +67,10 @@
 dmypy.json
 
 # Material for MkDocs
 site/
 
 # Jupyter Notebook load data
 .ipynb_checkpoints
+
+# IDE-specific directories
+.idea
```

### Comparing `autora-3.0.1/.pre-commit-config.yaml` & `autora-3.1.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -21,9 +21,16 @@
         - "--per-file-ignores=__init__.py:F401"
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v0.991"
     hooks:
       - id: mypy
         additional_dependencies: [types-requests]
         language_version: python3.8
+  - repo: https://github.com/srstevenson/nb-clean
+    rev: 2.4.0
+    hooks:
+      - id: nb-clean
+        args:
+          - --preserve-cell-outputs
+
 default_language_version:
   python: python3
```

### Comparing `autora-3.0.1/LICENSE.md` & `autora-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.1/MAINTAINING.md` & `autora-3.1.0/MAINTAINING.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.1/PKG-INFO` & `autora-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.1
+Version: 3.1.0
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 Maintainer-email: Ben Andrew <benwallaceandrew@gmail.com>, George Dang <george_dang@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
@@ -37,14 +37,15 @@
 Provides-Extra: all-experimentalists
 Provides-Extra: experimentalist-sampler-inequality
 Provides-Extra: experimentalist-sampler-novelty
 Provides-Extra: experimentalist-sampler-nearest-value
 Provides-Extra: experimentalist-sampler-model-disagreement
 Provides-Extra: experimentalist-sampler-uncertainty
 Provides-Extra: experimentalist-falsification
+Provides-Extra: experimentalist-sampler-mixture
 Provides-Extra: all-experiment-runners
 Provides-Extra: experiment-runner-firebase-prolific
 Provides-Extra: all-experiment-runner-experimentation-managers
 Provides-Extra: experiment-runner-experimentation-manager-firebase
 Provides-Extra: all-experiment-runner-recruitment-managers
 Provides-Extra: experiment-runner-recruitment-manager-prolific
 Provides-Extra: docs
@@ -54,28 +55,29 @@
 # Automated Research Assistant
 
 ![PyPI](https://img.shields.io/pypi/v/autora)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/autoresearch/autora/test-pytest.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/autora)
 
 <b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
-automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
+automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science. 
+
+AutoRA was initially intended for accelerating research in the behavioral and brain sciences. However, AutoRA is designed as a general framework that enables automation of the research processes in other empirical sciences, such as material science or physics.
 
 ![Autonomous Empirical Research Paradigm](https://github.com/AutoResearch/autora/raw/main/docs/img/overview.png)
 
 ## Getting Started
 
 Check out the documentation at 
 [https://autoresearch.github.io/autora](https://autoresearch.github.io/autora).
 
 ## About
 
 This project is in active development by 
 the [Autonomous Empirical Research Group](http://empiricalresearch.ai), 
-led by [Sebastian Musslick](https://smusslick.com), 
 in collaboration with the [Center for Computation and Visualization at Brown University](https://ccv.brown.edu).
 
 The development of this package is supported by Schmidt Science Fellows, in partnership with the Rhodes Trust, as well as the Carney BRAINSTORM program at Brown University.
 
 ## Read More
 
 - [Package Documentation](https://autoresearch.github.io/autora/)
```

### Comparing `autora-3.0.1/README.md` & `autora-3.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Automated Research Assistant
 
 ![PyPI](https://img.shields.io/pypi/v/autora)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/autoresearch/autora/test-pytest.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/autora)
 
 <b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
-automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
+automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science. 
+
+AutoRA was initially intended for accelerating research in the behavioral and brain sciences. However, AutoRA is designed as a general framework that enables automation of the research processes in other empirical sciences, such as material science or physics.
 
 ![Autonomous Empirical Research Paradigm](https://github.com/AutoResearch/autora/raw/main/docs/img/overview.png)
 
 ## Getting Started
 
 Check out the documentation at 
 [https://autoresearch.github.io/autora](https://autoresearch.github.io/autora).
 
 ## About
 
 This project is in active development by 
 the [Autonomous Empirical Research Group](http://empiricalresearch.ai), 
-led by [Sebastian Musslick](https://smusslick.com), 
 in collaboration with the [Center for Computation and Visualization at Brown University](https://ccv.brown.edu).
 
 The development of this package is supported by Schmidt Science Fellows, in partnership with the Rhodes Trust, as well as the Carney BRAINSTORM program at Brown University.
 
 ## Read More
 
 - [Package Documentation](https://autoresearch.github.io/autora/)
```

### Comparing `autora-3.0.1/docs/contribute/core.md` & `autora-3.1.0/docs/contribute/core.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,44 @@
-# Contribute to the Core
+# Contributions To Core Packages
 
-Core contributions are changes to AutoRA which aren't experimentalists, (synthetic) experiment runners and theorists. 
+Core contributions are changes to AutoRA which aren't experimentalists, (synthetic) experiment runners, or theorists. 
 The primary purpose of the core is to provide utilities for:
 
 - describing experiments (in the [`autora-core` package](https://github.com/autoresearch/autora-core))
 - handle workflows for automated experiments
   (currently in the [`autora-workflow` package](https://github.com/autoresearch/autora-workflow))
+- run synthetic experiments (currently in the [`autora-synthetic` package](https://github.com/autoresearch/autora-synthetic). Synthetic experiment runners may be submitted as pull requests to the 
+    [`autora-synthetic`](https://github.com/AutoResearch/autora-synthetic/blob/main/CONTRIBUTING.md) package, providing they 
+    require no additional dependencies. However, if your contribution requires additional dependencies, you can submit it as a full package following 
+    the [module contribution guide](modules/index.md).
+
+## How to Contribute
+
+In order to make a contribution to autora core, you may start by cloning the repository:
+```bash
+git clone https://github.com/AutoResearch/autora-core.git
+```
+
+You should then follow the [Development Setup Guide](https://autoresearch.github.io/autora/contribute/setup/), to set up your environment. 
 
 Suggested changes to the core should be submitted as follows, depending on their content:
 
 - For fixes or new features closely associated with existing core functionality: pull request to the existing 
   core package
 - For new features which don't fit into the current module structure, or which are experimental and could lead to 
   instability for users: as new namespace packages.
 
 !!! success
     Reach out to the core team about new core contributions to discuss how best to incorporate them by posting your 
     idea on the [discussions page](https://github.com/orgs/AutoResearch/discussions/categories/ideas).
 
+## Development Requirements
+
 Core packages should as a minimum:
 
 - Follow standard python coding guidelines including PEP8
 - Run under all minor versions of python (e.g. 3.8, 3.9) allowed in 
   [`autora-core`](https://github.com/autoresearch/autora-core)
 - Be compatible with all current AutoRA packages
 - Have comprehensive test suites
 - Use the linters and checkers defined in the `autora-core` 
-  [.pre-commit-config.yaml](https://github.com/AutoResearch/autora-core/blob/main/.pre-commit-config.yaml)
+  [.pre-commit-config.yaml](https://github.com/AutoResearch/autora-core/blob/main/.pre-commit-config.yaml) (see [pre-commit hooks](pre-commit-hooks.md))
```

### Comparing `autora-3.0.1/docs/contribute/pre-commit-hooks.md` & `autora-3.1.0/docs/contribute/pre-commit-hooks.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Pre-Commit Hooks
 
 We use [`pre-commit`](https://pre-commit.com) to manage pre-commit hooks. 
 
 Pre-commit hooks are programs which run before each git commit, and can read and potentially modify the files which are to be committed. 
 
 We use pre-commit hooks to:
-- enforce coding guidelines, including the `python` style-guide [PEP8](https://peps.python.org/pep-0008/) (`black` and `flake8`), 
+- enforce coding guidelines, including the `python` style-guide [PEP8](https://peps.python.org/pep-0008/) (`black` and `flake8`),
 - to check the order of `import` statements (`isort`),
 - to check the types of `python` objects (`mypy`).
 
 The hooks and their settings are specified in the `.pre-commit-config.yaml` in each repository.
 
 ## Handling Pre-Commit Hook Errors
```

### Comparing `autora-3.0.1/docs/contribute/setup.md` & `autora-3.1.0/docs/contribute/setup.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,32 +24,31 @@
     It is helpful to be familiar with the command line for your operating system. The topics required are covered in:
 
     - **macOS**: Joe Kissell. [*Take Control of the Mac Command Line with Terminal, 3rd Edition*](https://bruknow.library.brown.edu/permalink/01BU_INST/528fgv/cdi_safari_books_v2_9781947282513). Take Control Books, 2022. Chapters *Read Me First* through *Bring the Command Line Into The Real World*.
     - **Linux**: William E. Shotts. [*The Linux Command Line: a Complete Introduction. 2nd edition.*](https://bruknow.library.brown.edu/permalink/01BU_INST/9mvq88/alma991043239704906966). No Starch Press, 2019. Parts *I: Learning the Shell* and *II: Configuration and the Environment*.
 
 ## Development Setup
 
-### Clone the Repository
+### Clone The Repository
 
 The easiest way to clone the repo is to go to [the repository page on GitHub](https://github.com/AutoResearch/autora)
 and click the "<> Code" button and follow the prompts. 
 
 !!! hint
     We recommend using:
     
     - the [GitHub Desktop Application](https://desktop.github.com) on macOS or Windows, or 
     - the [GitHub command line utility](https://cli.github.com) on Linux.
 
-### Install `python`
+### Install `Python`
 
 !!! success
     All contributions to the AutoRA core packages should work under **python 3.8**, so we recommend using that version 
     for development.
     
-
 You can install python:
 
 - Using the instructions at [python.org](https://www.python.org), or
 - Using a package manager, e.g.
   [homebrew](https://docs.brew.sh/Homebrew-and-Python), 
   [pyenv](https://github.com/pyenv/pyenv),
   [asdf](https://github.com/asdf-community/asdf-python), 
@@ -63,15 +62,15 @@
 
 ...and see some output like this:
 ```
 Python 3.11.3 (main, Apr  7 2023, 20:13:31) [Clang 14.0.0 (clang-1400.0.29.202)] on darwin
 Type "help", "copyright", "credits" or "license" for more information.
 ```
 
-#### Create a virtual environment
+#### Create A Virtual Environment
 
 !!! success
     We recommend setting up your development environment using a manager like `venv`, which creates isolated python 
     environments. Other environment managers, like 
     [virtualenv](https://virtualenv.pypa.io/en/latest/),
     [pipenv](https://pipenv.pypa.io/en/latest/),
     [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/), 
@@ -83,20 +82,26 @@
 
 In the `<project directory>`, run the following command to create a new virtual environment in the `.venv` directory
 
 ```shell
 python3 -m "venv" ".venv" 
 ```
 
+!!! hint
+    If you have multiple Python versions installed on your system, it may be necessary to specify the Python version when creating a virtual environment. For example, run the following command to specify Python 3.8 for the virtual environment. 
+    ```shell
+    python3.8 -m "venv" ".venv" 
+    ```
+
 Activate it by running
 ```shell
 source ".venv/bin/activate"
 ```
 
-#### Install dependencies
+#### Install Dependencies
 
 Upgrade pip:
 ```shell
 pip install --upgrade pip
 ```
 
 Install the current project development dependencies:
@@ -106,15 +111,15 @@
 
 Your IDE may have special support for python environments. For IDE-specific setup, see:
 
 - [PyCharm Documentation](https://www.jetbrains.com/help/pycharm/configuring-python-interpreter.html)
 - [VSCode Documentation](https://code.visualstudio.com/docs/python/environments)
 
 
-### Activating and using the environment
+### Activating And Using The Environment
 
 To run interactive commands, you can activate the virtualenv environment. From the `<project directory>` 
 directory, run:
 
 ```shell
 source ".venv/bin/activate"
 ```
@@ -165,15 +170,15 @@
     as follows:
     ```
     (venv) % deactivate
     % 
     ```
 
 
-### Running code non-interactively
+### Running Code Non-Interactively
 
 You can run python programs without activating the environment, by using `/path/to/python run {command}`. For example,
 to run unittests tests, execute:
 
 ```shell
 .venv/bin/python -m pytest
 ```
@@ -185,15 +190,15 @@
 .
 --------------------------------
 Ran 1 test in 0.000s
 
 OK
 ```
 
-### Pre-commit hooks
+### Pre-Commit Hooks
 
 If you wish to commit to the repository, you should install and activate `pre-commit` as follows. 
 ```shell
 pip install pre-commit
 pre-commit install
 ```
```

### Comparing `autora-3.0.1/docs/experimentalist/index.md` & `autora-3.1.0/docs/experimentalist/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # Experimentalist Overview
 
 The primary goal of an experimentalist is to identify experiments that yield 
 scientific merit. AutoRA implements techniques for automating the identification 
 of novel experiments.
 
-An experiment consists of a series of **experiment conditions** $\vec{x} \in X$. 
-The experimental variables manipulated in each experiment condition 
+An experiment consists of a series of **experimental conditions** $\vec{x} \in X$. 
+The experimental variables manipulated in each experimental condition 
 are defined as **factors**, and the values of each variable to be sampled 
 in the experiment are defined as **levels** of the corresponding **factors**. 
 As an example, consider a visual discrimination tasks in which participants are presented
 with two lines of different lengths, and are asked to indicate which line is longer.
 There are two factors in this experiment: the length of the first line and 
 the length of the second line. Instances of the two line lengths 
 (e.g., 2.0 cm for the first line and 2.1 cm for the sceond line) 
-can be considered levels of the two factors, respectively. Thus, *an experiment condition is a vector of values that
+can be considered levels of the two factors, respectively. Thus, *an experimental condition is a vector of values that
 corresponds to a specific combination of experiment levels $x_i$, 
 each of which is an instance of an experiment factor.*
 
 Experimentalists in AutoRA serve to identify novel 
-experiment conditions $\vec{x} \in X$, where $x_i$ corresponds 
+experimental conditions $\vec{x} \in X$, where $x_i$ corresponds 
 to the level of an experimental factor $i$.
 
 ![Overview](../img/experimentalist.png)
 
 Experimentalists may use information about candidate models $M$ obtained from a theorist, 
-experiment conditions that have already been probed $\vec{x}' \in X'$, or 
+experimental conditions that have already been probed $\vec{x}' \in X'$, or 
 respective dependent measures $\vec{y}' \in Y'$. The following table includes the experimentalists currently implemented
  in AutoRA.
 
 | Experimentalist  | Function                                                                                                                      | Arguments   |
 |------------------|-------------------------------------------------------------------------------------------------------------------------------|-------------|
 | Random           | $\vec{x_i} \sim U[a_i,b_i]$                                                                                                   |             |
 | Novelty          | $\underset{\vec{x}}{\arg\max}~\min(d(\vec{x}, \vec{x}'))$                                                                     | $X'$        |
```

### Comparing `autora-3.0.1/docs/img/logo.png` & `autora-3.1.0/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.1/docs/index.md` & `autora-3.1.0/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,53 +12,41 @@
 experiments that can refine and validate the models generated by the theorist. Together, these agents
 implement an automated scientific discovery process. To enable closed-loop empirical research, AutoRA 
 interfaces with platforms for automated data collection, such as Prolific or Amazon Mechanical Turk, 
 which enable the efficient acquisition of behavioral data from human participants. Finally, AutoRA 
 is designed to support the automated documentation and dissemination of steps in the empirical research process.
 
 AutoRA was initially intended for accelerating research in the behavioral and brain sciences. 
-However, AutoRA is designed as a general framework that enables automation of the research processes in
-other empirical sciences, such as material science or physics.
+However, AutoRA is designed as a general framework that enables automation of research processes in
+other empirical sciences, such as materials science or physics.
 
 ## Features
 
 AutoRA consists of different modules that can be used independently or in combination, such as:
 
-- <b>Automated theorists</b> that support the discovery of formal scientific models from data
-- <b>Automated experimentalists</b> that support the design of follow-up experiments
-- <b>Interfaces for automated data collection</b>, e.g., for behavioral experiments via Prolific or Amazon Mechanical Turk
-- <b>Workflow logic</b> for defining interactions between different components of the research process
+- [**Theorists**](theorist/index.md) that support the discovery of formal scientific models from data
+- [**Experimentalists**](experimentalist/index.md) that support the design of follow-up experiments
+- [**Experiment runners**](experiment-runner/index.md) that support data collection from experimentation platforms (e.g., Prolific or Amazon Mechanical Turk)
+- [**Workflow logic**](user-guide/workflow) for defining interactions between different components of the research process
 - <b>Interfaces for automated documentation</b> of the research process
 
-## Usages
+## Uses
 
 AutoRA can be used for a variety of research purposes in empirical sciences, such as psychology, 
-neuroscience, economics, physics, or material science. Usages include:
+neuroscience, economics, physics, or materials science. Usages, as illustrated in the following tutorials, include:
 
-- <b>Equation discovery</b> from empirical data
-- <b>Experimental design</b> for follow-up experiments
-- <b>Research documentation and dissemination</b>
-- <b>Closed-loop empirical research</b>
-- <b>Computational analyses of the scientific process</b> (metascience, computational philosophy of science)
+- [**Equation discovery**](tutorials/Theorist.ipynb) from empirical data
+- [**Experimental design**](tutorials/Experimentalist.ipynb) for follow-up experiments
+- **Research documentation and dissemination**
+- **Closed-loop empirical research**
+- **Computational analyses of the scientific process** (metascience, computational philosophy of science)
 
 ## Motivation
 
-Various empirical sciences are beset by a replication crisis, 
-which can be attributed to inadequately precise hypotheses, lack of transparency
-in research procedures, and insufficient rigor in testing findings. These limitations
-are the result of three primary bottlenecks—a lack of formal modeling, the
-demanding requirements of open science, and a shortage of resources to reproduce 
-individual studies. Empirical scientists face difficulties in formalizing their 
-theories, find it arduous to document their research activities, and often lack 
-time and funds to conduct follow-up experiments to test and revise their
-hypotheses. These limitations impede scientific progress and hinder
-the development of new knowledge. We seek to overcome these limitations by providing
-a tool for the generation, estimation, and empirical testing of scientific models. 
-It is our hope that AutoRA will help accelerate scientific discovery by overcoming
-these limitations and promoting greater transparency and rigor in empirical research.
+The pace of empirical research is constrained by the rate at which scientists can alternate between the development of formal theories and the execution of experiments. However, attempts to increase this rate often compromise scientific rigor, leading to deficiencies such as the absence of formal modeling, non-replicable findings, and insufficient documentation. In order to surmount these limitations, we aim to develop AutoRA––an open-source framework that automates the generation, estimation, and empirical testing of scientific models. By automating steps of the empirical research process, we hope AutoRA can accelerate scientific discovery while promoting greater transparency and rigor in empirical research.
 
 ## Pointers
 
 - [AutoRA Pip Package](https://pypi.org/project/autora/)
 - [GitHub Repository](https://github.com/AutoResearch/autora)
 - [Autonomous Empirical Research Group](http://www.empiricalresearch.ai)
```

### Comparing `autora-3.0.1/mkdocs/overrides/main.html` & `autora-3.1.0/mkdocs/overrides/main.html`

 * *Files 16% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 {% if page.nb_url %}
     <a href="{{ page.canonical_url }}{{ page.file.src_uri | basename | quote }}" title="Download Notebook"
        class="md-content__button md-icon">
         {% include ".icons/material/download.svg" %}
     </a>
     <a href="{{ config.extra.colab_base_url }}{{ page.url }}{{ page.file.src_uri | basename | quote }}"
        title="Open Notebook in Google Colab" class="md-content__button md-icon">
-        {% include ".icons/material/play-circle-outline.svg" %}
+        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     </a>
 {% endif %}
 {{ super() }}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
 {% extends "base.html" %} {% block content %} {% if page.nb_url %} {%_include
-".icons/material/download.svg"_%} {%_include_".icons/material/play-circle-
-outline.svg"_%} {% endif %} {{ super() }} {% endblock content %}
+".icons/material/download.svg"_%} [Open_In_Colab] {% endif %} {{ super() }} {%
+endblock content %}
```

### Comparing `autora-3.0.1/pyproject.toml` & `autora-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 all-experimentalists = [
   "autora[experimentalist-sampler-inequality]",
   "autora[experimentalist-sampler-novelty]",
   "autora[experimentalist-sampler-nearest-value]",
   "autora[experimentalist-sampler-model-disagreement]",
   "autora[experimentalist-sampler-uncertainty]",
   "autora[experimentalist-falsification]",
+  "autora[experimentalist-sampler-mixture]",
 ]
 experimentalist-sampler-inequality =[
   "autora-experimentalist-sampler-inequality"
 ]
 experimentalist-sampler-novelty =[
   "autora-experimentalist-sampler-novelty"
 ]
@@ -68,14 +69,17 @@
 ]
 experimentalist-sampler-uncertainty =[
   "autora-experimentalist-sampler-uncertainty"
 ]
 experimentalist-falsification =[
   "autora-experimentalist-falsification"
 ]
+experimentalist-sampler-mixture =[
+  "mixture-experimentalist==1.0.0a4"
+]
 
 all-experiment-runners = [
   "autora[experiment-runner-firebase-prolific]"
 ]
 experiment-runner-firebase-prolific = [
   "autora-experiment-runner-firebase-prolific"
 ]
@@ -90,15 +94,14 @@
 ]
 experiment-runner-recruitment-manager-prolific = [
   "autora-experiment-runner-recruitment-manager-prolific"
 ]
 
 docs = [
   "autora-core[docs]",
-  "mkdocs-simple-hooks",
 ]
 
 test = [
   "pytest"
 ]
 
 [project.urls]
@@ -107,7 +110,10 @@
 documentation = "https://autoresearch.github.io/autora/"
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
+
+[tool.setuptools]
+packages = []
```

### Comparing `autora-3.0.1/src/autora.egg-info/PKG-INFO` & `autora-3.1.0/autora.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.1
+Version: 3.1.0
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 Maintainer-email: Ben Andrew <benwallaceandrew@gmail.com>, George Dang <george_dang@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
@@ -37,14 +37,15 @@
 Provides-Extra: all-experimentalists
 Provides-Extra: experimentalist-sampler-inequality
 Provides-Extra: experimentalist-sampler-novelty
 Provides-Extra: experimentalist-sampler-nearest-value
 Provides-Extra: experimentalist-sampler-model-disagreement
 Provides-Extra: experimentalist-sampler-uncertainty
 Provides-Extra: experimentalist-falsification
+Provides-Extra: experimentalist-sampler-mixture
 Provides-Extra: all-experiment-runners
 Provides-Extra: experiment-runner-firebase-prolific
 Provides-Extra: all-experiment-runner-experimentation-managers
 Provides-Extra: experiment-runner-experimentation-manager-firebase
 Provides-Extra: all-experiment-runner-recruitment-managers
 Provides-Extra: experiment-runner-recruitment-manager-prolific
 Provides-Extra: docs
@@ -54,28 +55,29 @@
 # Automated Research Assistant
 
 ![PyPI](https://img.shields.io/pypi/v/autora)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/autoresearch/autora/test-pytest.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/autora)
 
 <b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
-automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
+automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science. 
+
+AutoRA was initially intended for accelerating research in the behavioral and brain sciences. However, AutoRA is designed as a general framework that enables automation of the research processes in other empirical sciences, such as material science or physics.
 
 ![Autonomous Empirical Research Paradigm](https://github.com/AutoResearch/autora/raw/main/docs/img/overview.png)
 
 ## Getting Started
 
 Check out the documentation at 
 [https://autoresearch.github.io/autora](https://autoresearch.github.io/autora).
 
 ## About
 
 This project is in active development by 
 the [Autonomous Empirical Research Group](http://empiricalresearch.ai), 
-led by [Sebastian Musslick](https://smusslick.com), 
 in collaboration with the [Center for Computation and Visualization at Brown University](https://ccv.brown.edu).
 
 The development of this package is supported by Schmidt Science Fellows, in partnership with the Rhodes Trust, as well as the Carney BRAINSTORM program at Brown University.
 
 ## Read More
 
 - [Package Documentation](https://autoresearch.github.io/autora/)
```

### Comparing `autora-3.0.1/src/autora.egg-info/requires.txt` & `autora-3.1.0/autora.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 [all-experimentalists]
 autora[experimentalist-sampler-inequality]
 autora[experimentalist-sampler-novelty]
 autora[experimentalist-sampler-nearest-value]
 autora[experimentalist-sampler-model-disagreement]
 autora[experimentalist-sampler-uncertainty]
 autora[experimentalist-falsification]
+autora[experimentalist-sampler-mixture]
 
 [all-theorists]
 autora[theorist-darts]
 autora[theorist-bms]
 autora[theorist-bsr]
 
 [dev]
 autora-core[dev]
 
 [docs]
 autora-core[docs]
-mkdocs-simple-hooks
 
 [experiment-runner-experimentation-manager-firebase]
 autora-experiment-runner-experimentation-manager-firebase
 
 [experiment-runner-firebase-prolific]
 autora-experiment-runner-firebase-prolific
 
@@ -47,14 +47,17 @@
 
 [experimentalist-falsification]
 autora-experimentalist-falsification
 
 [experimentalist-sampler-inequality]
 autora-experimentalist-sampler-inequality
 
+[experimentalist-sampler-mixture]
+mixture-experimentalist==1.0.0a4
+
 [experimentalist-sampler-model-disagreement]
 autora-experimentalist-sampler-model-disagreement
 
 [experimentalist-sampler-nearest-value]
 autora-experimentalist-sampler-nearest-value
 
 [experimentalist-sampler-novelty]
```

