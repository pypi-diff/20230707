# Comparing `tmp/autora-workflow-0.3.6.tar.gz` & `tmp/autora-workflow-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.3.6.tar", last modified: Thu Jun  1 21:14:23 2023, max compression
+gzip compressed data, was "autora-workflow-0.4.0b1.tar", last modified: Fri Jul  7 21:49:31 2023, max compression
```

## Comparing `autora-workflow-0.3.6.tar` & `autora-workflow-0.4.0b1.tar`

### file list

```diff
@@ -1,109 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.920358 autora-workflow-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.904358 autora-workflow-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-01 21:14:23.920358 autora-workflow-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/docs/cli/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)   246597 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/cli/basic-usage/Readme.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/cli/basic-usage/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/docs/cli/with-cylc/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/cli/with-cylc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/docs/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/interactive/Accessing State Dependent Properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/interactive/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/interactive/Passing Static Parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45729 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/interactive/Saving And Loading With Dill.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/interactive/Using Alternative Planners And Executors.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.912358 autora-workflow-0.3.6/examples/cylc-conda/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-conda/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-conda/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-conda/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/examples/cylc-conda/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/examples/cylc-conda/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-conda/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-conda/lib/python/dump_initial_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/examples/cylc-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-pip/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-pip/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-pip/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/examples/cylc-pip/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/examples/cylc-pip/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-pip/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-pip/lib/python/dump_initial_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-pip/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/examples/cylc-slurm-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-slurm-pip/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-slurm-pip/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-slurm-pip/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-slurm-pip/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/examples/cylc-slurm-pip/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/examples/cylc-slurm-pip/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-slurm-pip/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-slurm-pip/lib/python/dump_initial_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/examples/cylc-slurm-pip/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:14:23.920358 autora-workflow-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.908357 autora-workflow-0.3.6/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.916358 autora-workflow-0.3.6/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.920358 autora-workflow-0.3.6/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.920358 autora-workflow-0.3.6/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-01 21:14:23.000000 autora-workflow-0.3.6/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-01 21:14:23.000000 autora-workflow-0.3.6/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:14:23.000000 autora-workflow-0.3.6/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-01 21:14:23.000000 autora-workflow-0.3.6/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 21:14:23.000000 autora-workflow-0.3.6/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:14:23.920358 autora-workflow-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-01 21:14:13.000000 autora-workflow-0.3.6/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.696504 autora-workflow-0.4.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.696504 autora-workflow-0.4.0b1/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/docs/cli/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)   238637 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/cli/basic-usage/Readme.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/cli/basic-usage/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/docs/cli/with-cylc/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/cli/with-cylc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/docs/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/interactive/Accessing State Dependent Properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/interactive/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/interactive/Passing Static Parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/interactive/Saving And Loading With Dill.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30261 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/interactive/Using Alternative Planners And Executors.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.696504 autora-workflow-0.4.0b1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/examples/cylc-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-conda/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-conda/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.696504 autora-workflow-0.4.0b1/examples/cylc-conda/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/examples/cylc-conda/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-conda/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-conda/lib/python/dump_initial_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/examples/cylc-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-pip/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-pip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-pip/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.696504 autora-workflow-0.4.0b1/examples/cylc-pip/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/examples/cylc-pip/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-pip/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-pip/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-pip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/examples/cylc-slurm-pip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.704504 autora-workflow-0.4.0b1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.700504 autora-workflow-0.4.0b1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/state/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-07 21:49:31.000000 autora-workflow-0.4.0b1/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-07 21:49:31.000000 autora-workflow-0.4.0b1/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:49:31.000000 autora-workflow-0.4.0b1/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 21:49:31.000000 autora-workflow-0.4.0b1/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 21:49:31.000000 autora-workflow-0.4.0b1/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:49:31.708504 autora-workflow-0.4.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-07-07 21:49:16.000000 autora-workflow-0.4.0b1/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.3.6/.github/workflows/python-publish.yml` & `autora-workflow-0.4.0b1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/.github/workflows/test-pytest.yml` & `autora-workflow-0.4.0b1/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/.gitignore` & `autora-workflow-0.4.0b1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -65,7 +65,13 @@
 
 # Material for MkDocs
 site/
 docs/reference/
 
 # Jupyter Notebook load data
 .ipynb_checkpoints
+
+# Dill pickle files
+*.dill
+# IDE-specific directories
+.idea
+
```

### Comparing `autora-workflow-0.3.6/.pre-commit-config.yaml` & `autora-workflow-0.4.0b1/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -23,9 +23,10 @@
         exclude: ^examples/
   - repo: https://github.com/srstevenson/nb-clean
     rev: 2.4.0
     hooks:
       - id: nb-clean
         args:
           - --preserve-cell-outputs
+          - --remove-empty-cells
 default_language_version:
   python: python3
```

### Comparing `autora-workflow-0.3.6/LICENSE.md` & `autora-workflow-0.4.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/PKG-INFO` & `autora-workflow-0.4.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.6
+Version: 0.4.0b1
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
```

### Comparing `autora-workflow-0.3.6/README.md` & `autora-workflow-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/docs/cli/basic-usage/Readme.ipynb` & `autora-workflow-0.4.0b1/docs/cli/basic-usage/Readme.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942122103386809%*

 * *Differences: {"'cells'": "{1: {'source': ['%cat lib.py']}, 5: {'outputs': []}, 7: {'outputs': {0: {'text': "*

 * *            "{insert: [(2, 'INFO:autora.workflow.base:running next_function=<function "*

 * *            'from_experimentalist_pipeline.<locals>._executor_experimentalist at '*

 * *            "0x15f97e310>\\r\\n')], delete: [12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2]}}}}, 8: "*

 * *            "{'outputs': {0: {'text': {insert: [(2, 'INFO:autora.workflow.base:running "*

 * *            'next_function=<function '*

 * *            'from_experime […]*

```diff
@@ -71,15 +71,15 @@
                         "    experimentalist=experimentalist,\r\n",
                         "    theorist=theorist,\r\n",
                         ")\r\n"
                     ]
                 }
             ],
             "source": [
-                "!pygmentize lib.py  # display the lib.py file"
+                "%cat lib.py"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Then, before we start the experiment, we\n",
@@ -107,32 +107,15 @@
                 "default next step for the specified controller."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "new_conditions=array([[-5.22],\r\n",
-                        "       [ 1.52],\r\n",
-                        "       [ 1.42],\r\n",
-                        "       [ 3.36],\r\n",
-                        "       [-1.74],\r\n",
-                        "       [ 1.06],\r\n",
-                        "       [ 8.74],\r\n",
-                        "       [-5.86],\r\n",
-                        "       [-1.16],\r\n",
-                        "       [-6.46]]) is an ndarray, so variable confusion is a possibility\r\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "!python -m autora.workflow \"simple-controller.dill\" \"intermediate-1.dill\"\n",
                 "!python -m autora.workflow \"intermediate-1.dill\" \"intermediate-2.dill\"\n",
                 "!python -m autora.workflow \"intermediate-2.dill\" \"result.dill\""
             ]
         },
         {
@@ -151,25 +134,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "INFO:__main__:using INFO logging level\r\n",
                         "INFO:autora.workflow.base:getting step_name='experimentalist'\r\n",
-                        "INFO:autora.workflow.base:running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14cba63e0>\r\n",
-                        "WARNING:autora.workflow.executor:new_conditions=array([[-5.22],\r\n",
-                        "       [ 1.52],\r\n",
-                        "       [ 1.42],\r\n",
-                        "       [ 3.36],\r\n",
-                        "       [-1.74],\r\n",
-                        "       [ 1.06],\r\n",
-                        "       [ 8.74],\r\n",
-                        "       [-5.86],\r\n",
-                        "       [-1.16],\r\n",
-                        "       [-6.46]]) is an ndarray, so variable confusion is a possibility\r\n",
+                        "INFO:autora.workflow.base:running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x15f97e310>\r\n",
                         "INFO:__main__:last result: Result(data=array([[-5.22],\r\n",
                         "       [ 1.52],\r\n",
                         "       [ 1.42],\r\n",
                         "       [ 3.36],\r\n",
                         "       [-1.74],\r\n",
                         "       [ 1.06],\r\n",
                         "       [ 8.74],\r\n",
@@ -191,15 +164,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "INFO:__main__:using INFO logging level\r\n",
                         "INFO:autora.workflow.base:getting step_name='experiment_runner'\r\n",
-                        "INFO:autora.workflow.base:running next_function=<function from_experiment_runner_callable.<locals>._executor_experiment_runner at 0x14d2a63e0>\r\n",
+                        "INFO:autora.workflow.base:running next_function=<function from_experiment_runner_callable.<locals>._executor_experiment_runner at 0x137ac0310>\r\n",
                         "INFO:__main__:last result: Result(data=array([[ -5.22      ,  44.17634595],\r\n",
                         "       [  1.52      ,   2.85614526],\r\n",
                         "       [  1.42      ,  -1.18727197],\r\n",
                         "       [  3.36      ,  42.40577088],\r\n",
                         "       [ -1.74      ,  -5.1408566 ],\r\n",
                         "       [  1.06      ,   1.85630186],\r\n",
                         "       [  8.74      , 184.75918836],\r\n",
@@ -221,15 +194,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "INFO:__main__:using INFO logging level\r\n",
                         "INFO:autora.workflow.base:getting step_name='theorist'\r\n",
-                        "INFO:autora.workflow.base:running next_function=<function from_theorist_estimator.<locals>._executor_theorist at 0x1688a63e0>\r\n",
+                        "INFO:autora.workflow.base:running next_function=<function from_theorist_estimator.<locals>._executor_theorist at 0x147780310>\r\n",
                         "INFO:__main__:last result: Result(data=GridSearchCV(estimator=Pipeline(steps=[('polynomialfeatures',\r\n",
                         "                                        PolynomialFeatures()),\r\n",
                         "                                       ('linearregression',\r\n",
                         "                                        LinearRegression())]),\r\n",
                         "             param_grid={'polynomialfeatures__degree': [0, 1, 2, 3, 4]},\r\n",
                         "             scoring='r2'), kind=ResultKind.MODEL)\r\n",
                         "INFO:__main__:writing out results\r\n"
@@ -269,61 +242,41 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[Result(data=VariableCollection(independent_variables=[Variable(name='x',\n",
-                        "                                                                value_range=None,\n",
-                        "                                                                allowed_values=None,\n",
-                        "                                                                units='',\n",
-                        "                                                                type=<ValueType.REAL: 'real'>,\n",
-                        "                                                                variable_label='',\n",
-                        "                                                                rescale=1,\n",
-                        "                                                                is_covariate=False)],\n",
-                        "                                dependent_variables=[Variable(name='y',\n",
-                        "                                                              value_range=None,\n",
-                        "                                                              allowed_values=None,\n",
-                        "                                                              units='',\n",
-                        "                                                              type=<ValueType.REAL: 'real'>,\n",
-                        "                                                              variable_label='',\n",
-                        "                                                              rescale=1,\n",
-                        "                                                              is_covariate=False)],\n",
-                        "                                covariates=[]),\n",
-                        "        kind=ResultKind.VARIABLES),\n",
+                        "[Result(data=VariableCollection(independent_variables=[Variable(name='x', value_range=None, allowed_values=None, units='', type=<ValueType.REAL: 'real'>, variable_label='', rescale=1, is_covariate=False)], dependent_variables=[Variable(name='y', value_range=None, allowed_values=None, units='', type=<ValueType.REAL: 'real'>, variable_label='', rescale=1, is_covariate=False)], covariates=[]), kind=ResultKind.VARIABLES),\n",
                         " Result(data=array([[-5.22],\n",
                         "       [ 1.52],\n",
                         "       [ 1.42],\n",
                         "       [ 3.36],\n",
                         "       [-1.74],\n",
                         "       [ 1.06],\n",
                         "       [ 8.74],\n",
                         "       [-5.86],\n",
                         "       [-1.16],\n",
-                        "       [-6.46]]),\n",
-                        "        kind=ResultKind.CONDITION),\n",
+                        "       [-6.46]]), kind=ResultKind.CONDITION),\n",
                         " Result(data=array([[ -5.22      ,  44.17634595],\n",
                         "       [  1.52      ,   2.85614526],\n",
                         "       [  1.42      ,  -1.18727197],\n",
                         "       [  3.36      ,  42.40577088],\n",
                         "       [ -1.74      ,  -5.1408566 ],\n",
                         "       [  1.06      ,   1.85630186],\n",
                         "       [  8.74      , 184.75918836],\n",
                         "       [ -5.86      ,  72.86977407],\n",
                         "       [ -1.16      , -14.10728103],\n",
-                        "       [ -6.46      ,  70.81902322]]),\n",
-                        "        kind=ResultKind.OBSERVATION),\n",
+                        "       [ -6.46      ,  70.81902322]]), kind=ResultKind.OBSERVATION),\n",
                         " Result(data=GridSearchCV(estimator=Pipeline(steps=[('polynomialfeatures',\n",
                         "                                        PolynomialFeatures()),\n",
                         "                                       ('linearregression',\n",
                         "                                        LinearRegression())]),\n",
                         "             param_grid={'polynomialfeatures__degree': [0, 1, 2, 3, 4]},\n",
-                        "             scoring='r2'),\n",
-                        "        kind=ResultKind.MODEL)]\n"
+                        "             scoring='r2'), kind=ResultKind.MODEL)]\n"
                     ]
                 }
             ],
             "source": [
                 "from pprint import pprint\n",
                 "pprint(controller_result.state.history)"
             ]
@@ -340,31 +293,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "VariableCollection(independent_variables=[Variable(name='x',\n",
-                        "                                                   value_range=None,\n",
-                        "                                                   allowed_values=None,\n",
-                        "                                                   units='',\n",
-                        "                                                   type=<ValueType.REAL: 'real'>,\n",
-                        "                                                   variable_label='',\n",
-                        "                                                   rescale=1,\n",
-                        "                                                   is_covariate=False)],\n",
-                        "                   dependent_variables=[Variable(name='y',\n",
-                        "                                                 value_range=None,\n",
-                        "                                                 allowed_values=None,\n",
-                        "                                                 units='',\n",
-                        "                                                 type=<ValueType.REAL: 'real'>,\n",
-                        "                                                 variable_label='',\n",
-                        "                                                 rescale=1,\n",
-                        "                                                 is_covariate=False)],\n",
-                        "                   covariates=[])\n"
+                        "VariableCollection(independent_variables=[Variable(name='x', value_range=None, allowed_values=None, units='', type=<ValueType.REAL: 'real'>, variable_label='', rescale=1, is_covariate=False)], dependent_variables=[Variable(name='y', value_range=None, allowed_values=None, units='', type=<ValueType.REAL: 'real'>, variable_label='', rescale=1, is_covariate=False)], covariates=[])\n"
                     ]
                 }
             ],
             "source": [
                 "pprint(controller_result.state.history[0].data)"
             ]
         },
@@ -535,52 +472,15 @@
                 "If we run the experiment for another 3 cycles, we can get results closer to the ground truth. In this example, we overwrite the results file each time the CLI is called."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "new_conditions=array([[ 9.64],\r\n",
-                        "       [ 0.54],\r\n",
-                        "       [-2.74],\r\n",
-                        "       [-4.06],\r\n",
-                        "       [ 7.4 ],\r\n",
-                        "       [ 9.26],\r\n",
-                        "       [-4.38],\r\n",
-                        "       [ 7.2 ],\r\n",
-                        "       [ 9.2 ],\r\n",
-                        "       [-5.98]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[-9.32],\r\n",
-                        "       [ 1.94],\r\n",
-                        "       [-8.74],\r\n",
-                        "       [-3.52],\r\n",
-                        "       [-2.66],\r\n",
-                        "       [-1.78],\r\n",
-                        "       [-8.98],\r\n",
-                        "       [ 6.18],\r\n",
-                        "       [ 3.28],\r\n",
-                        "       [ 6.74]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[ 5.16],\r\n",
-                        "       [-3.5 ],\r\n",
-                        "       [-0.68],\r\n",
-                        "       [-6.62],\r\n",
-                        "       [-6.94],\r\n",
-                        "       [-0.98],\r\n",
-                        "       [ 1.88],\r\n",
-                        "       [-5.18],\r\n",
-                        "       [ 1.98],\r\n",
-                        "       [-6.42]]) is an ndarray, so variable confusion is a possibility\r\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "!cp \"theorist-output.dill\" \"result.dill\"\n",
                 "for i in range(9):  # each cycle has 3 steps, and we take 1 step per CLI call\n",
                 "    !python -m autora.workflow \"result.dill\" \"result.dill\""
             ]
         },
         {
@@ -614,120 +514,14 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "new_conditions=array([[ 5.56],\r\n",
-                        "       [ 0.94],\r\n",
-                        "       [-8.16],\r\n",
-                        "       [ 6.08],\r\n",
-                        "       [-2.76],\r\n",
-                        "       [-9.74],\r\n",
-                        "       [ 9.82],\r\n",
-                        "       [-8.62],\r\n",
-                        "       [-9.24],\r\n",
-                        "       [ 6.5 ]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[-1.72],\r\n",
-                        "       [ 9.36],\r\n",
-                        "       [-4.58],\r\n",
-                        "       [ 4.7 ],\r\n",
-                        "       [-0.96],\r\n",
-                        "       [-7.76],\r\n",
-                        "       [ 0.34],\r\n",
-                        "       [-9.66],\r\n",
-                        "       [-8.2 ],\r\n",
-                        "       [-3.24]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[ 8.06],\r\n",
-                        "       [-2.1 ],\r\n",
-                        "       [ 3.1 ],\r\n",
-                        "       [-6.62],\r\n",
-                        "       [ 4.3 ],\r\n",
-                        "       [-7.  ],\r\n",
-                        "       [-4.5 ],\r\n",
-                        "       [-6.26],\r\n",
-                        "       [-7.34],\r\n",
-                        "       [-2.16]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[-1.74],\r\n",
-                        "       [ 4.12],\r\n",
-                        "       [-4.14],\r\n",
-                        "       [-0.32],\r\n",
-                        "       [-2.22],\r\n",
-                        "       [-5.76],\r\n",
-                        "       [ 4.92],\r\n",
-                        "       [-9.22],\r\n",
-                        "       [-2.34],\r\n",
-                        "       [-2.46]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[-2.54],\r\n",
-                        "       [ 2.32],\r\n",
-                        "       [ 0.52],\r\n",
-                        "       [ 1.56],\r\n",
-                        "       [ 0.46],\r\n",
-                        "       [-4.  ],\r\n",
-                        "       [ 4.98],\r\n",
-                        "       [ 7.56],\r\n",
-                        "       [-7.62],\r\n",
-                        "       [-5.96]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[ 9.86],\r\n",
-                        "       [-9.26],\r\n",
-                        "       [ 8.7 ],\r\n",
-                        "       [-5.56],\r\n",
-                        "       [ 0.76],\r\n",
-                        "       [ 9.48],\r\n",
-                        "       [ 6.54],\r\n",
-                        "       [ 9.82],\r\n",
-                        "       [-6.96],\r\n",
-                        "       [-0.4 ]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[-9.52],\r\n",
-                        "       [-5.48],\r\n",
-                        "       [-8.8 ],\r\n",
-                        "       [ 4.2 ],\r\n",
-                        "       [-5.6 ],\r\n",
-                        "       [-5.14],\r\n",
-                        "       [ 4.44],\r\n",
-                        "       [ 8.46],\r\n",
-                        "       [-0.76],\r\n",
-                        "       [ 0.8 ]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[ 1.8 ],\r\n",
-                        "       [-4.48],\r\n",
-                        "       [ 4.42],\r\n",
-                        "       [-1.88],\r\n",
-                        "       [ 1.3 ],\r\n",
-                        "       [ 6.22],\r\n",
-                        "       [ 5.74],\r\n",
-                        "       [ 2.34],\r\n",
-                        "       [-3.32],\r\n",
-                        "       [-3.14]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[ 8.04],\r\n",
-                        "       [-6.38],\r\n",
-                        "       [ 7.84],\r\n",
-                        "       [ 4.16],\r\n",
-                        "       [ 3.68],\r\n",
-                        "       [ 8.12],\r\n",
-                        "       [ 3.44],\r\n",
-                        "       [-6.26],\r\n",
-                        "       [ 0.98],\r\n",
-                        "       [ 0.28]]) is an ndarray, so variable confusion is a possibility\r\n",
-                        "new_conditions=array([[ 5.16],\r\n",
-                        "       [-5.66],\r\n",
-                        "       [ 5.32],\r\n",
-                        "       [-8.1 ],\r\n",
-                        "       [-0.74],\r\n",
-                        "       [ 3.02],\r\n",
-                        "       [ 0.18],\r\n",
-                        "       [-0.54],\r\n",
-                        "       [ 8.6 ],\r\n",
-                        "       [-2.94]]) is an ndarray, so variable confusion is a possibility\r\n"
-                    ]
-                },
-                {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
@@ -740,21 +534,14 @@
                 "    !python -m autora.workflow \"result-30.dill\" \"result-30.dill\"\n",
                 "\n",
                 "with open(\"result-30.dill\", \"rb\") as file:\n",
                 "    controller_after_13_cycles = dill.load(file)\n",
                 "\n",
                 "plot_results(controller_after_13_cycles)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `autora-workflow-0.3.6/docs/cli/basic-usage/lib.py` & `autora-workflow-0.4.0b1/docs/cli/basic-usage/lib.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
-from autora.experimentalist.pipeline import (
-    make_pipeline as make_experimentalist_pipeline,
-)
-from autora.variable import Variable, VariableCollection
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import GridSearchCV
 from sklearn.pipeline import make_pipeline as make_theorist_pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
+from autora.experimentalist.pipeline import (
+    make_pipeline as make_experimentalist_pipeline,
+)
+from autora.variable import Variable, VariableCollection
 from autora.workflow import Controller
 
 rng = np.random.default_rng(180)
 
 experimentalist = make_experimentalist_pipeline(
     [np.linspace, rng.choice],
     params={
```

### Comparing `autora-workflow-0.3.6/docs/interactive/Accessing State Dependent Properties.ipynb` & `autora-workflow-0.4.0b1/docs/interactive/Accessing State Dependent Properties.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9669909204623879%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, \'# Accessing "State-Dependent Properties"\\n\'), (11, '*

 * *            '\'- `"%experiment_data.conditions[-1]%"`: the last observed independent '*

 * *            'variables\\n\'), (12, \'- `"%experiment_data.observations[-1]%"`: the last observed '*

 * *            'dependent variables\\n\'), (13, \'- `"%experiment_data.conditions%"`: all the '*

 * *            'observed independent variables,\\n\'), (15, \'- `"%experiment_data.observations%"`: '*

 * *            "all the observed dep […]*

```diff
@@ -1,29 +1,29 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Accessing \"State-dependent Properties\"\n",
+                "# Accessing \"State-Dependent Properties\"\n",
                 "\n",
                 "Some experimentalists, experiment runners and theorists require access to the values\n",
                 "created during the cycle execution, e.g. experimentalists which require access\n",
                 "to the current best model or the observed data. These data update each cycle, and\n",
                 "so cannot easily be set using simple `params`.\n",
                 "\n",
                 "For this case, it is possible to use \"state-dependent properties\" in the `params`\n",
                 "dictionary. These are the following strings, which will be replaced during execution by\n",
                 "their respective current values:\n",
                 "\n",
-                "- `\"%observations.ivs[-1]%\"`: the last observed independent variables\n",
-                "- `\"%observations.dvs[-1]%\"`: the last observed dependent variables\n",
-                "- `\"%observations.ivs%\"`: all the observed independent variables,\n",
+                "- `\"%experiment_data.conditions[-1]%\"`: the last observed independent variables\n",
+                "- `\"%experiment_data.observations[-1]%\"`: the last observed dependent variables\n",
+                "- `\"%experiment_data.conditions%\"`: all the observed independent variables,\n",
                 "concatenated into a single array\n",
-                "- `\"%observations.dvs%\"`: all the observed dependent variables,\n",
+                "- `\"%experiment_data.observations%\"`: all the observed dependent variables,\n",
                 "concatenated into a single array\n",
                 "- `\"%models[-1]%\"`: the last fitted theorist\n",
                 "- `\"%models%\"`: all the fitted theorists\n",
                 "\n",
                 "In the following example, we use the `\"observations.ivs\"` cycle property for an\n",
                 "experimentalist which excludes those conditions which have\n",
                 "already been seen."
@@ -31,14 +31,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Uncomment the following line when running on Google Colab\n",
+                "# !pip install autora"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
                 "from autora.variable import VariableCollection, Variable\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "import pandas as pd\n",
                 "from functools import partial\n",
                 "\n",
@@ -87,15 +97,15 @@
                 "cycle_with_state_dep_properties = Cycle(\n",
                 "    variables=variables,\n",
                 "    theorist=example_theorist,\n",
                 "    experimentalist=unobserved_data_experimentalist,\n",
                 "    experiment_runner=example_synthetic_experiment_runner,\n",
                 "    params={\n",
                 "        \"experimentalist\": {\n",
-                "            \"exclude_conditions\": {\"excluded_conditions\": \"%observations.ivs%\"},\n",
+                "            \"exclude_conditions\": {\"excluded_conditions\": \"%experiment_data.conditions%\"},\n",
                 "            \"custom_random_sampler\": {\"n\": 1}\n",
                 "        }\n",
                 "    }\n",
                 ")"
             ]
         },
         {
@@ -233,46 +243,30 @@
                 {
                     "ename": "ValueError",
                     "evalue": "a cannot be empty unless no samples are taken",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[0;31mValueError\u001b[0m                                Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[5], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m \u001b[43mcycle_with_state_dep_properties\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mrun\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m  \u001b[38;5;66;03m# doctest: +ELLIPSIS\u001b[39;00m\n",
+                        "Cell \u001b[0;32mIn[6], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m \u001b[43mcycle_with_state_dep_properties\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mrun\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n",
                         "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/cycle.py:82\u001b[0m, in \u001b[0;36mCycle.run\u001b[0;34m(self, num_cycles)\u001b[0m\n\u001b[1;32m     80\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mrun\u001b[39m(\u001b[38;5;28mself\u001b[39m, num_cycles: \u001b[38;5;28mint\u001b[39m \u001b[38;5;241m=\u001b[39m \u001b[38;5;241m1\u001b[39m):\n\u001b[1;32m     81\u001b[0m \u001b[38;5;250m    \u001b[39m\u001b[38;5;124;03m\"\"\"Execute the next step in the cycle.\"\"\"\u001b[39;00m\n\u001b[0;32m---> 82\u001b[0m     \u001b[38;5;28;43msuper\u001b[39;49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mrun\u001b[49m\u001b[43m(\u001b[49m\u001b[43mnum_steps\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mnum_cycles\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     83\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[38;5;28mself\u001b[39m\n",
                         "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/base.py:85\u001b[0m, in \u001b[0;36mBaseController.run\u001b[0;34m(self, num_steps)\u001b[0m\n\u001b[1;32m     83\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"Run the next num_steps planned steps in the workflow.\"\"\"\u001b[39;00m\n\u001b[1;32m     84\u001b[0m \u001b[38;5;28;01mfor\u001b[39;00m i \u001b[38;5;129;01min\u001b[39;00m \u001b[38;5;28mrange\u001b[39m(num_steps):\n\u001b[0;32m---> 85\u001b[0m     \u001b[38;5;28;43mself\u001b[39;49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mrun_once\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     86\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[38;5;28mself\u001b[39m\n",
                         "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/base.py:71\u001b[0m, in \u001b[0;36mBaseController.run_once\u001b[0;34m(self, step_name)\u001b[0m\n\u001b[1;32m     68\u001b[0m _logger\u001b[38;5;241m.\u001b[39mdebug(\u001b[38;5;124mf\u001b[39m\u001b[38;5;124m\"\u001b[39m\u001b[38;5;132;01m{\u001b[39;00mnext_params\u001b[38;5;132;01m=}\u001b[39;00m\u001b[38;5;124m\"\u001b[39m)\n\u001b[1;32m     70\u001b[0m \u001b[38;5;66;03m# Execute\u001b[39;00m\n\u001b[0;32m---> 71\u001b[0m result \u001b[38;5;241m=\u001b[39m \u001b[43mnext_function\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;28;43mself\u001b[39;49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mstate\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mparams\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mnext_params\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     72\u001b[0m _logger\u001b[38;5;241m.\u001b[39mdebug(\u001b[38;5;124mf\u001b[39m\u001b[38;5;124m\"\u001b[39m\u001b[38;5;132;01m{\u001b[39;00mresult\u001b[38;5;132;01m=}\u001b[39;00m\u001b[38;5;124m\"\u001b[39m)\n\u001b[1;32m     74\u001b[0m \u001b[38;5;66;03m# Update\u001b[39;00m\n",
                         "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/executor.py:174\u001b[0m, in \u001b[0;36mfull_cycle_wrapper.<locals>._executor_full_cycle\u001b[0;34m(state, params)\u001b[0m\n\u001b[1;32m    169\u001b[0m experimentalist_params \u001b[38;5;241m=\u001b[39m params\u001b[38;5;241m.\u001b[39mget(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mexperimentalist\u001b[39m\u001b[38;5;124m\"\u001b[39m, {})\n\u001b[1;32m    171\u001b[0m experimentalist_executor \u001b[38;5;241m=\u001b[39m from_experimentalist_pipeline(\n\u001b[1;32m    172\u001b[0m     experimentalist_pipeline\n\u001b[1;32m    173\u001b[0m )\n\u001b[0;32m--> 174\u001b[0m experimentalist_result \u001b[38;5;241m=\u001b[39m \u001b[43mexperimentalist_executor\u001b[49m\u001b[43m(\u001b[49m\u001b[43mstate\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mexperimentalist_params\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m    176\u001b[0m experiment_runner_params \u001b[38;5;241m=\u001b[39m params\u001b[38;5;241m.\u001b[39mget(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mexperiment_runner\u001b[39m\u001b[38;5;124m\"\u001b[39m, {})\n\u001b[1;32m    177\u001b[0m experiment_runner_executor \u001b[38;5;241m=\u001b[39m from_experiment_runner_callable(\n\u001b[1;32m    178\u001b[0m     experiment_runner_callable\n\u001b[1;32m    179\u001b[0m )\n",
                         "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/executor.py:64\u001b[0m, in \u001b[0;36mfrom_experimentalist_pipeline.<locals>._executor_experimentalist\u001b[0;34m(state, params)\u001b[0m\n\u001b[1;32m     62\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21m_executor_experimentalist\u001b[39m(state: SupportsControllerState, params: Dict):\n\u001b[1;32m     63\u001b[0m     params_ \u001b[38;5;241m=\u001b[39m resolve_state_params(params, state)\n\u001b[0;32m---> 64\u001b[0m     new_conditions \u001b[38;5;241m=\u001b[39m \u001b[43mpipeline\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mparams_\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     66\u001b[0m     \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(new_conditions, pd\u001b[38;5;241m.\u001b[39mDataFrame):\n\u001b[1;32m     67\u001b[0m         new_conditions_array \u001b[38;5;241m=\u001b[39m new_conditions\n",
-                        "File \u001b[0;32m~/Developer/autora-workflow/venv/lib/python3.10/site-packages/autora/experimentalist/pipeline.py:171\u001b[0m, in \u001b[0;36mPipeline.__call__\u001b[0;34m(self, ex, **params)\u001b[0m\n\u001b[1;32m    169\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(pipe, Pipe)\n\u001b[1;32m    170\u001b[0m     all_params_for_pipe \u001b[38;5;241m=\u001b[39m merged_params\u001b[38;5;241m.\u001b[39mget(name, \u001b[38;5;28mdict\u001b[39m())\n\u001b[0;32m--> 171\u001b[0m     results\u001b[38;5;241m.\u001b[39mappend(\u001b[43mpipe\u001b[49m\u001b[43m(\u001b[49m\u001b[43mresults\u001b[49m\u001b[43m[\u001b[49m\u001b[38;5;241;43m-\u001b[39;49m\u001b[38;5;241;43m1\u001b[39;49m\u001b[43m]\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mall_params_for_pipe\u001b[49m\u001b[43m)\u001b[49m)\n\u001b[1;32m    173\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m results[\u001b[38;5;241m-\u001b[39m\u001b[38;5;241m1\u001b[39m]\n",
-                        "Cell \u001b[0;32mIn[2], line 9\u001b[0m, in \u001b[0;36mcustom_random_sampler\u001b[0;34m(conditions, n)\u001b[0m\n\u001b[1;32m      8\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mcustom_random_sampler\u001b[39m(conditions, n):\n\u001b[0;32m----> 9\u001b[0m     sampled_conditions \u001b[38;5;241m=\u001b[39m \u001b[43mrandom_sampler_rng\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mchoice\u001b[49m\u001b[43m(\u001b[49m\u001b[43mconditions\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43msize\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mn\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mreplace\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[38;5;28;43;01mFalse\u001b[39;49;00m\u001b[43m)\u001b[49m\n\u001b[1;32m     10\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m sampled_conditions\n",
+                        "File \u001b[0;32m~/Developer/autora-workflow/.venv/lib/python3.8/site-packages/autora/experimentalist/pipeline.py:171\u001b[0m, in \u001b[0;36mPipeline.__call__\u001b[0;34m(self, ex, **params)\u001b[0m\n\u001b[1;32m    169\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(pipe, Pipe)\n\u001b[1;32m    170\u001b[0m     all_params_for_pipe \u001b[38;5;241m=\u001b[39m merged_params\u001b[38;5;241m.\u001b[39mget(name, \u001b[38;5;28mdict\u001b[39m())\n\u001b[0;32m--> 171\u001b[0m     results\u001b[38;5;241m.\u001b[39mappend(\u001b[43mpipe\u001b[49m\u001b[43m(\u001b[49m\u001b[43mresults\u001b[49m\u001b[43m[\u001b[49m\u001b[38;5;241;43m-\u001b[39;49m\u001b[38;5;241;43m1\u001b[39;49m\u001b[43m]\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mall_params_for_pipe\u001b[49m\u001b[43m)\u001b[49m)\n\u001b[1;32m    173\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m results[\u001b[38;5;241m-\u001b[39m\u001b[38;5;241m1\u001b[39m]\n",
+                        "Cell \u001b[0;32mIn[3], line 9\u001b[0m, in \u001b[0;36mcustom_random_sampler\u001b[0;34m(conditions, n)\u001b[0m\n\u001b[1;32m      8\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mcustom_random_sampler\u001b[39m(conditions, n):\n\u001b[0;32m----> 9\u001b[0m     sampled_conditions \u001b[38;5;241m=\u001b[39m \u001b[43mrandom_sampler_rng\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mchoice\u001b[49m\u001b[43m(\u001b[49m\u001b[43mconditions\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43msize\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mn\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mreplace\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[38;5;28;43;01mFalse\u001b[39;49;00m\u001b[43m)\u001b[49m\n\u001b[1;32m     10\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m sampled_conditions\n",
                         "File \u001b[0;32m_generator.pyx:729\u001b[0m, in \u001b[0;36mnumpy.random._generator.Generator.choice\u001b[0;34m()\u001b[0m\n",
                         "\u001b[0;31mValueError\u001b[0m: a cannot be empty unless no samples are taken"
                     ]
                 }
             ],
             "source": [
-                "cycle_with_state_dep_properties.run()  # doctest: +ELLIPSIS"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pd.concat(cycle_with_state_dep_properties.data.conditions, ignore_index=True)\n"
+                "cycle_with_state_dep_properties.run()\n"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `autora-workflow-0.3.6/docs/interactive/Basic Usage.ipynb` & `autora-workflow-0.4.0b1/docs/interactive/Basic Usage.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966216216216216%*

 * *Differences: {"'cells'": "{insert: [(1, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['# Uncomment the following "*

 * *            "line when running on Google Colab\\n', '# !pip install autora'])]))]}"}*

```diff
@@ -11,14 +11,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Uncomment the following line when running on Google Colab\n",
+                "# !pip install autora"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
                 "from autora.variable import VariableCollection, Variable\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "\n",
                 "from autora.workflow import Cycle\n",
                 "from itertools import takewhile"
```

### Comparing `autora-workflow-0.3.6/docs/interactive/Passing Static Parameters.ipynb` & `autora-workflow-0.4.0b1/docs/interactive/Passing Static Parameters.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861363636363636%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(1, 'def uniform_random_sample(n):\\n'), (5, "*

 * *            "'example_experimentalist_with_parameters = make_pipeline([uniform_random_sample])')], "*

 * *            "delete: [5, 1]}}, 5: {'source': "*

 * *            '[\'example_experimentalist_with_parameters(**{"uniform_random_sample": {"n": '*

 * *            '1}})\']}, 8: {\'source\': {insert: [(5, \'    params={"experimentalist": '*

 * *            '{"uniform_random_sample": {"n": 3}}}\\n\')], delete: [5]}}, 10: {\'source\': {insert:  […]*

```diff
@@ -11,14 +11,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Uncomment the following line when running on Google Colab\n",
+                "# !pip install autora"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
                 "from autora.variable import VariableCollection, Variable\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "\n",
                 "from autora.workflow import Cycle"
@@ -34,19 +44,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "uniform_random_rng = np.random.default_rng(180)\n",
-                "def uniform_random_sampler(n):\n",
+                "def uniform_random_sample(n):\n",
                 "    new_conditions = uniform_random_rng.uniform(low=0, high=11, size=n)\n",
                 "    conditions_df = pd.DataFrame({\"x\": new_conditions})\n",
                 "    return conditions_df\n",
-                "example_experimentalist_with_parameters = make_pipeline([uniform_random_sampler])"
+                "example_experimentalist_with_parameters = make_pipeline([uniform_random_sample])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
@@ -90,15 +100,15 @@
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "example_experimentalist_with_parameters(**{\"uniform_random_sampler\": {\"n\": 1}})"
+                "example_experimentalist_with_parameters(**{\"uniform_random_sample\": {\"n\": 1}})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -192,15 +202,15 @@
             ],
             "source": [
                 "cycle_with_parameters = Cycle(\n",
                 "    variables=metadata,\n",
                 "    theorist=example_theorist,\n",
                 "    experimentalist=example_experimentalist_with_parameters,\n",
                 "    experiment_runner=example_synthetic_experiment_runner,\n",
-                "    params={\"experimentalist\": {\"uniform_random_sampler\": {\"n\": 3}}}\n",
+                "    params={\"experimentalist\": {\"uniform_random_sample\": {\"n\": 3}}}\n",
                 ")\n",
                 "cycle_with_parameters.run()\n",
                 "cycle_with_parameters.data.conditions[-1]"
             ]
         },
         {
             "cell_type": "markdown",
@@ -259,15 +269,15 @@
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "cycle_with_parameters.params[\"experimentalist\"][\"uniform_random_sampler\"][\"n\"] = 2\n",
+                "cycle_with_parameters.params[\"experimentalist\"][\"uniform_random_sample\"][\"n\"] = 2\n",
                 "cycle_with_parameters.run()\n",
                 "cycle_with_parameters.data.conditions[-1]\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `autora-workflow-0.3.6/docs/interactive/Saving And Loading With Dill.ipynb` & `autora-workflow-0.4.0b1/docs/interactive/Saving And Loading With Dill.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Saving And loading Controllers Using Dill\\n')], "*

 * *            "delete: [0]}}, insert: [(1, OrderedDict([('cell_type', 'code'), ('execution_count', "*

 * *            "None), ('metadata', OrderedDict()), ('outputs', []), ('source', ['# Uncomment the "*

 * *            "following line when running on Google Colab\\n', '# !pip install autora'])]))], "*

 * *            'delete: [10]}'}*

```diff
@@ -1,28 +1,38 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Saving and loading controllers using dill\n",
+                "# Saving And loading Controllers Using Dill\n",
                 "\n",
                 "## Basic usage\n",
                 "\n",
                 "Workflow managers can be saved to and loaded using [dill](https://github.com/uqfoundation/dill).\n",
                 "\n",
                 "For instance, you could generate a basic Controller object in an interactive python session as follows:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Uncomment the following line when running on Google Colab\n",
+                "# !pip install autora"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "import autora.workflow\n",
                 "import dill\n",
                 "\n",
                 "controller = autora.workflow.Controller()\n",
                 "\n",
                 "with open(\"default-controller.dill\", \"wb\") as file:\n",
                 "    dill.dump(controller, file)"
@@ -207,21 +217,14 @@
                 "         label=\"ground truth\",\n",
                 "         lw=10, alpha=0.2, c=\"black\")\n",
                 "plt.plot(x, controller_loaded.state.models[-1].best_estimator_.predict(x),\n",
                 "         label=\"prediction\",\n",
                 "         lw=1, alpha=1, c=\"red\")\n",
                 "plt.legend()\n"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `autora-workflow-0.3.6/docs/interactive/Using Alternative Planners And Executors.ipynb` & `autora-workflow-0.4.0b1/docs/interactive/Using Alternative Planners And Executors.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960387323943662%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Custom Planners And Executors\\n'), (5, '## Easier "*

 * *            "Seeding With A Smarter Planner\\n')], delete: [5, 0]}}, 29: {'source': {insert: [(0, "*

 * *            "'## Arbitrary Executors And Planners\\n')], delete: [0]}}, 33: {'source': {insert: "*

 * *            "[(1, 'from autora.state.history import History')], delete: [1]}}, 46: {'source': "*

 * *            "{insert: [(1, 'from autora.experimentalist.sampler.random_sampler import "*

 * *            "random_sample\\n')] […]*

```diff
@@ -1,31 +1,41 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Custom Planners and Executors\n",
+                "# Custom Planners And Executors\n",
                 "\n",
                 "By switching out the `executor_collection` and/or the `planner`, we can specify a\n",
                 "different way of running the cycle.\n",
                 "\n",
-                "## Easier Seeding with a Smarter Planner\n",
+                "## Easier Seeding With A Smarter Planner\n",
                 "\n",
                 "In this example, we use the `Controller` which allows much more control over execution\n",
                 "order. It considers the last available result and picks the matching next step. This means\n",
                 "that seeding is relatively simple."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Uncomment the following line when running on Google Colab\n",
+                "# !pip install autora"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
                 "from autora.variable import VariableCollection, Variable\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "from autora.workflow import Controller\n",
                 "from itertools import takewhile"
             ]
@@ -398,15 +408,15 @@
                 "_ = list(takewhile(lambda c: len(c.state.models) < 1, controller_with_random_planner))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Arbitrary Executors and Planners\n",
+                "## Arbitrary Executors And Planners\n",
                 "\n",
                 "In some cases, we need to go beyond adding different orders of planning the three\n",
                 "`experimentalist`, `experiment_runner` and `theorist` and build more complex cycles with\n",
                 "different Executors for different states.\n",
                 "\n",
                 "For instance, there might be a situation where at the start, the main \"active\" experimentalist\n",
                 "can't be run as it needs one or more models as input.\n",
@@ -453,15 +463,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from autora.workflow.planner import last_result_kind_planner\n",
-                "from autora.workflow.state import History"
+                "from autora.state.history import History"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -623,15 +633,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from autora.experimentalist.pipeline import make_pipeline, Pipeline\n",
-                "from autora.experimentalist.sampler.random_sampler import random_sampler\n",
+                "from autora.experimentalist.sampler.random_sampler import random_sample\n",
                 "from functools import partial"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -654,15 +664,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "experimentalist_which_needs_no_data = make_pipeline([\n",
                 "    np.linspace(*variables.independent_variables[0].value_range, 1_000),\n",
-                "    partial(random_sampler, n=10)]\n",
+                "    partial(random_sample, n=10)]\n",
                 ")\n",
                 "np.array(experimentalist_which_needs_no_data())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -808,15 +818,15 @@
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from autora.workflow.base import BaseController\n",
-                "from autora.workflow.state import History\n",
+                "from autora.state.history import History\n",
                 "c = BaseController(\n",
                 "        state=History(variables=variables, params=params),\n",
                 "        planner=seeding_planner,\n",
                 "        executor_collection=executor_collection\n",
                 ")\n",
                 "c"
             ]
@@ -983,21 +993,14 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "next(c).state.history[-1]\n"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `autora-workflow-0.3.6/examples/cylc-conda/README.md` & `autora-workflow-0.4.0b1/examples/cylc-conda/README.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/examples/cylc-conda/flow.cylc` & `autora-workflow-0.4.0b1/examples/cylc-conda/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/examples/cylc-conda/lib/python/controller_setup.py` & `autora-workflow-0.4.0b1/examples/cylc-conda/lib/python/controller_setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
-from autora.experimentalist.pipeline import (
-    make_pipeline as make_experimentalist_pipeline,
-)
-from autora.variable import Variable, VariableCollection
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import GridSearchCV
 from sklearn.pipeline import make_pipeline as make_theorist_pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
+from autora.experimentalist.pipeline import (
+    make_pipeline as make_experimentalist_pipeline,
+)
+from autora.variable import Variable, VariableCollection
 from autora.workflow import Controller
 
 rng = np.random.default_rng(180)
 
 experimentalist = make_experimentalist_pipeline(
     [np.linspace, rng.choice],
     params={
```

### Comparing `autora-workflow-0.3.6/examples/cylc-pip/README.md` & `autora-workflow-0.4.0b1/examples/cylc-pip/README.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/examples/cylc-pip/flow.cylc` & `autora-workflow-0.4.0b1/examples/cylc-pip/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/examples/cylc-pip/lib/python/controller_setup.py` & `autora-workflow-0.4.0b1/examples/cylc-pip/lib/python/controller_setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
-from autora.experimentalist.pipeline import (
-    make_pipeline as make_experimentalist_pipeline,
-)
-from autora.variable import Variable, VariableCollection
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import GridSearchCV
 from sklearn.pipeline import make_pipeline as make_theorist_pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
+from autora.experimentalist.pipeline import (
+    make_pipeline as make_experimentalist_pipeline,
+)
+from autora.variable import Variable, VariableCollection
 from autora.workflow import Controller
 
 rng = np.random.default_rng(180)
 
 experimentalist = make_experimentalist_pipeline(
     [np.linspace, rng.choice],
     params={
```

### Comparing `autora-workflow-0.3.6/examples/cylc-slurm-pip/README.md` & `autora-workflow-0.4.0b1/examples/cylc-slurm-pip/README.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/examples/cylc-slurm-pip/flow.cylc` & `autora-workflow-0.4.0b1/examples/cylc-slurm-pip/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/examples/cylc-slurm-pip/lib/python/controller_setup.py` & `autora-workflow-0.4.0b1/examples/cylc-slurm-pip/lib/python/controller_setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
-from autora.experimentalist.pipeline import (
-    make_pipeline as make_experimentalist_pipeline,
-)
-from autora.variable import Variable, VariableCollection
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import GridSearchCV
 from sklearn.pipeline import make_pipeline as make_theorist_pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
+from autora.experimentalist.pipeline import (
+    make_pipeline as make_experimentalist_pipeline,
+)
+from autora.variable import Variable, VariableCollection
 from autora.workflow import Controller
 
 rng = np.random.default_rng(180)
 
 experimentalist = make_experimentalist_pipeline(
     [np.linspace, rng.choice],
     params={
```

### Comparing `autora-workflow-0.3.6/mkdocs/base.yml` & `autora-workflow-0.4.0b1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/mkdocs.yml` & `autora-workflow-0.4.0b1/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # yaml-language-server: $schema=https://squidfunk.github.io/mkdocs-material/schema.json
 INHERIT: mkdocs/base.yml  # use the shared AutoRA configuration by default
 
 site_name: AutoRA Workflow
 
 nav:
 - Introduction: 'index.md'
-- Interactive:
+- Object-Oriented Approach:
     - 'interactive/Basic Usage.ipynb'
     - 'interactive/Passing Static Parameters.ipynb'
     - "interactive/Accessing State Dependent Properties.ipynb"
     - "interactive/Using Alternative Planners And Executors.ipynb"
     - "interactive/Saving And Loading With Dill.ipynb"
 - Command line:
     - "Basic Usage": "cli/basic-usage/Readme.ipynb"
```

### Comparing `autora-workflow-0.3.6/pyproject.toml` & `autora-workflow-0.4.0b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 dynamic = ["version"]
 
 readme = "docs/index.md"
 license = { text = "MIT License" }
 
 dependencies = [
-    "autora-core",
+    "autora-core>=3.3.0",
     "scikit-learn",
     "matplotlib",
     "pandas",
     "typer[all]",
     "dill",
     "pyyaml",
 ]
@@ -46,7 +46,8 @@
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [tool.isort]
 profile = "black"
+known_first_party = ["autora"]
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/__init__.py` & `autora-workflow-0.4.0b1/src/autora/workflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     step, demonstrating arbitrary execution order. We do this by modifying the planner attribute
     of an existing controller
 
     This might be useful in cases when different experimentalists or theorists are needed at
     different times in the cycle, e.g. for initial seeding.
     >>> from autora.workflow.planner import random_operation_planner
     >>> def monitor(state):
-    ...     print(f"MONITOR: Generated new {state.history[-1].kind.value}")
+    ...     print(f"MONITOR: Generated new { state.history[-1].kind.value}")
     >>> controller_with_random_planner = Controller(
     ...     planner=random_operation_planner,
     ...     monitor=monitor,
     ...     variables=variables_0,
     ...     theorist=example_theorist,
     ...     experimentalist=example_experimentalist,
     ...     experiment_runner=example_synthetic_experiment_runner,
@@ -416,30 +416,30 @@
     >>> variables_2 = VariableCollection(
     ...    independent_variables=[Variable(name="x1", value_range=(-10, 10))],
     ...    dependent_variables=[Variable(name="y", value_range=(-100, 100))],
     ...    )
 
     We now define a planner which chooses a different experimentalist when supplied with no data
     versus some data.
-    >>> from autora.workflow.protocol import ResultKind
+    >>> from autora.state.protocol import ResultKind
     >>> from autora.workflow.planner import last_result_kind_planner
     >>> def seeding_planner(state):
     ...     # We're going to reuse the "last_available_result" planner, and modify its output.
     ...     next_function = last_result_kind_planner(state)
     ...     if next_function == "experimentalist":
     ...         if len(state.models) >= 2:
     ...             return "main_experimentalist"
     ...         else:
     ...             return "seed_experimentalist"
     ...     else:
     ...         return next_function
 
     Now we can see what would happen with a particular state. If there are no results,
     then we get the seed experimentalist:
-    >>> from autora.workflow.state import History
+    >>> from autora.state.history import History
     >>> seeding_planner(History())
     'seed_experimentalist'
 
     ... and we also get the seed experimentalist if the last result was a model and there are less
     than two models:
     >>> seeding_planner(History(models=['a single model']))
     'seed_experimentalist'
@@ -460,30 +460,30 @@
     >>> from autora.experimentalist.pipeline import make_pipeline, Pipeline
     >>> from autora.experimentalist.sampler.random_sampler import random_sampler
     >>> from functools import partial
 
     Wen can run the seed pipeline with no data:
     >>> experimentalist_which_needs_no_data = make_pipeline([
     ...     np.linspace(*variables_2.independent_variables[0].value_range, 1_000),
-    ...     partial(random_sampler, n=10)]
+    ...     partial(random_sampler, num_samples=10)]
     ... )
     >>> np.array(experimentalist_which_needs_no_data())
     array([ 6.71671672, -0.73073073, -5.05505506,  6.13613614,  0.03003003,
             4.59459459,  2.79279279,  5.43543544, -1.65165165,  8.0980981 ])
 
 
     ... whereas we need some model for this sampler:
-    >>> from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
+    >>> from autora.experimentalist.sampler.model_disagreement import model_disagreement_sample
     >>> experimentalist_which_needs_a_model = Pipeline([
     ...     ('pool', np.linspace(*variables_2.independent_variables[0].value_range, 1_000)),
-    ...     ('sampler', partial(model_disagreement_sampler, num_samples=5)),])
+    ...     ('sampler', partial(model_disagreement_sample, num_samples=5)),])
     >>> experimentalist_which_needs_a_model()
     Traceback (most recent call last):
     ...
-    TypeError: model_disagreement_sampler() missing 1 required positional argument: 'models'
+    TypeError: model_disagreement_sample() missing 1 required positional argument: 'models'
 
     We'll have to provide the models during the cycle run.
 
     We need a reasonable theorist for this situation. For this problem, a linear regressor will
     suffice.
     >>> t = LinearRegression()
 
@@ -509,15 +509,15 @@
     ... )
 
     We need some special parameters to handle the main experimentalist, so we specify those:
     >>> params = {"main_experimentalist": {"sampler": {"models": "%models%"}}}
 
     We now instantiate the controller:
     >>> from autora.workflow.base import BaseController
-    >>> from autora.workflow.state import History
+    >>> from autora.state.history import History
     >>> c = BaseController(
     ...         state=History(variables=variables_2, params=params),
     ...         planner=seeding_planner,
     ...         executor_collection=executor_collection
     ... )
     >>> c  # doctest: +ELLIPSIS
     <...BaseController object at 0x...>
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/__main__.py` & `autora-workflow-0.4.0b1/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.6/src/autora/workflow/base.py` & `autora-workflow-0.4.0b1/src/autora/workflow/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """  The cycle controller for AER. """
 from __future__ import annotations
 
 import logging
-from typing import Callable, Generic, Mapping, Optional
+from typing import Callable, Generic, Mapping, Optional, TypeVar
 
-from .protocol import State
+from autora.state.protocol import Executor, SupportsStateParams
 
 _logger = logging.getLogger(__name__)
 
 
+State = TypeVar("State", bound=SupportsStateParams)
+
+
 class BaseController(Generic[State]):
     """
     Runs an experimentalist, theorist and experiment runner in a loop.
 
     Once initialized, the `controller` can be started by calling `next(controller)` or using the
         `controller.run` method.
 
@@ -31,15 +34,15 @@
 
     """
 
     def __init__(
         self,
         state: State,
         planner: Callable[[State], str],
-        executor_collection: Mapping[str, Callable[[State], State]],
+        executor_collection: Mapping[str, Executor[State]],
         monitor: Optional[Callable[[State], None]] = None,
     ):
         """
         Args:
             state: a fully instantiated controller state object compatible with the planner,
                 executor_collection and monitor
             planner: a function which maps from the state to the next ExecutorName
@@ -68,15 +71,15 @@
         _logger.debug(f"{next_params=}")
 
         # Execute
         result = next_function(self.state, params=next_params)
         _logger.debug(f"{result=}")
 
         # Update
-        _logger.debug(f"updating state")
+        _logger.debug("updating state")
         self.state = result
 
         if self.monitor is not None:
             self.monitor(self.state)
         return self
 
     def run(self, num_steps: int = 1):
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/controller.py` & `autora-workflow-0.4.0b1/src/autora/workflow/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """  The cycle controller for AER. """
 from __future__ import annotations
 
 import logging
 from typing import Callable, Dict, Optional
 
+from sklearn.base import BaseEstimator
+
 from autora.experimentalist.pipeline import Pipeline
+from autora.state.history import History
 from autora.variable import VariableCollection
-from sklearn.base import BaseEstimator
 
 from .base import BaseController
 from .executor import (
     ChainedFunctionMapping,
     from_experiment_runner_callable,
     from_experimentalist_pipeline,
     from_theorist_estimator,
 )
 from .planner import last_result_kind_planner
-from .state import History
 
 _logger = logging.getLogger(__name__)
 
 
 class Controller(BaseController[History]):
     """
     Runs an experimentalist, experiment runner, and theorist in order.
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/cycle.py` & `autora-workflow-0.4.0b1/src/autora/workflow/cycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """  The cycle controller for AER. """
 from __future__ import annotations
 
 import logging
 from typing import Callable, Dict, Optional
 
+from sklearn.base import BaseEstimator
+
 from autora.experimentalist.pipeline import Pipeline
+from autora.state.snapshot import Snapshot
 from autora.variable import VariableCollection
-from sklearn.base import BaseEstimator
 
 from .base import BaseController
 from .executor import full_cycle_wrapper
 from .planner import full_cycle_planner
-from .state import Snapshot
 
 _logger = logging.getLogger(__name__)
 
 
 class Cycle(BaseController):
     """
     Runs an experimentalist, experiment runner, and theorist in a loop.
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/executor.py` & `autora-workflow-0.4.0b1/src/autora/workflow/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import copy
 import logging
 import pprint
 from typing import Callable, Dict, Iterable, List
 
 import numpy as np
 import pandas as pd
-from autora.experimentalist.pipeline import Pipeline
 from sklearn.base import BaseEstimator
 
-from .protocol import Executor, SupportsControllerState
-from .state import resolve_state_params
+from autora.experimentalist.pipeline import Pipeline
+from autora.state.param import resolve_state_params
+from autora.state.protocol import Executor, SupportsControllerState
 
 _logger = logging.getLogger(__name__)
 
 
 class ChainedFunctionMapping(collections.UserDict):
     """
     Mapping name -> chains of functions applied like decorators.
@@ -44,15 +44,15 @@
 
         The "c" chain is the same as `f2_(f1_(f0_))`
         >>> c["c"]()
         2
 
     """
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str):
         functions: List = list(reversed(self.data[key]))
         f = functions[0]
         for fi in functions[1:]:
             f = fi(f)
         return f
 
 
@@ -190,14 +190,14 @@
 
 
 def no_op(state, params):
     """
     An Executor which has no effect on the state.
 
     Examples:
-         >>> from autora.workflow.state import Snapshot
+         >>> from autora.state.snapshot import Snapshot
          >>> s = Snapshot()
          >>> s_returned = no_op(s, {})
          >>> assert s_returned is s
     """
     _logger.warning("You called a `no_op` Executor. Returning the state unchanged.")
     return state
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/planner.py` & `autora-workflow-0.4.0b1/src/autora/workflow/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Functions which look at state and output the next function name to execute.
 """
 import random
 
-from .protocol import ResultKind, SupportsControllerStateHistory
+from autora.state.protocol import ResultKind, SupportsControllerStateHistory
 
 
 def full_cycle_planner(_):
     """Always returns the `full_cycle` method.
 
     Examples:
         The full_cycle_planner always returns the full cycle Executor
@@ -22,15 +22,15 @@
     """
     Chooses the operation based on the last result, e.g. new model -> run experimentalist.
 
     Interpretation: The "traditional" autora.workflow – a systematic research assistant.
 
     Examples:
         We initialize a new list to run our planner on:
-        >>> from autora.workflow.state import History
+        >>> from autora.state.history import History
         >>> state_ = History()
 
         Based on the results available in the state, we can get the next kind of executor we need.
         When we have no results of any kind, we get an experimentalist:
         >>> last_result_kind_planner(state_)
         'experimentalist'
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/plotting.py` & `autora-workflow-0.4.0b1/src/autora/workflow/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib import rcParams
 from matplotlib.patches import Patch
 from matplotlib.ticker import MaxNLocator
 
-from .protocol import SupportsControllerState
+from autora.state.protocol import SupportsControllerState
 
 # Change default plot styles
-rcParams["axes.spines.top"] = False
-rcParams["axes.spines.right"] = False
-rcParams["legend.frameon"] = False
+controller_plotting_rc_context = {
+    "axes.spines.top": False,
+    "axes.spines.right": False,
+    "legend.frameon": False,
+}
 
 
 def _get_variable_index(
     state: SupportsControllerState,
 ) -> Tuple[List[Tuple[int, str, str]], List[Tuple[int, str, str]]]:
     """
     Extracts information about independent and dependent variables from the cycle object.
@@ -293,62 +295,69 @@
 
     # Subplot configurations
     n_cycles_to_plot = len(cycle_idx)
     if n_cycles_to_plot < wrap:
         shape = (1, n_cycles_to_plot)
     else:
         shape = (int(np.ceil(n_cycles_to_plot / wrap)), wrap)
-    fig, axs = plt.subplots(*shape, **d_kw["subplot_kw"])
-    # Place axis object in an array if plotting single panel
-    if shape == (1, 1):
-        axs = np.array([axs])
-
-    # Loop by panel
-    for i, ax in enumerate(axs.flat):
-        if i + 1 <= n_cycles_to_plot:
-            # Get index of cycle to plot
-            i_cycle = cycle_idx[i]
-
-            # ---Plot observed data---
-            # Independent variable values
-            x_vals = df_observed.loc[:, iv[0]]
-            # Dependent values masked by current cycle vs previous data
-            dv_previous = np.ma.masked_where(
-                df_observed["cycle"] >= i_cycle, df_observed[dv[0]]
-            )
-            dv_current = np.ma.masked_where(
-                df_observed["cycle"] != i_cycle, df_observed[dv[0]]
-            )
-            # Plotting scatter
-            ax.scatter(x_vals, dv_previous, **d_kw["scatter_previous_kw"])
-            ax.scatter(x_vals, dv_current, **d_kw["scatter_current_kw"])
-
-            # ---Plot Model---
-            conditions = condition_space[:, iv[0]]
-            ax.plot(conditions, l_predictions[i_cycle], **d_kw["plot_model_kw"])
-
-            # Label Panels
-            ax.text(
-                0.05, 1, f"Cycle {i_cycle}", ha="left", va="top", transform=ax.transAxes
-            )
 
-        else:
-            ax.axis("off")
+    with plt.rc_context(controller_plotting_rc_context):
+        fig, axs = plt.subplots(*shape, **d_kw["subplot_kw"])
+        # Place axis object in an array if plotting single panel
+        if shape == (1, 1):
+            axs = np.array([axs])
+
+        # Loop by panel
+        for i, ax in enumerate(axs.flat):
+            if i + 1 <= n_cycles_to_plot:
+                # Get index of cycle to plot
+                i_cycle = cycle_idx[i]
+
+                # ---Plot observed data---
+                # Independent variable values
+                x_vals = df_observed.loc[:, iv[0]]
+                # Dependent values masked by current cycle vs previous data
+                dv_previous = np.ma.masked_where(
+                    df_observed["cycle"] >= i_cycle, df_observed[dv[0]]
+                )
+                dv_current = np.ma.masked_where(
+                    df_observed["cycle"] != i_cycle, df_observed[dv[0]]
+                )
+                # Plotting scatter
+                ax.scatter(x_vals, dv_previous, **d_kw["scatter_previous_kw"])
+                ax.scatter(x_vals, dv_current, **d_kw["scatter_current_kw"])
+
+                # ---Plot Model---
+                conditions = condition_space[:, iv[0]]
+                ax.plot(conditions, l_predictions[i_cycle], **d_kw["plot_model_kw"])
+
+                # Label Panels
+                ax.text(
+                    0.05,
+                    1,
+                    f"Cycle {i_cycle}",
+                    ha="left",
+                    va="top",
+                    transform=ax.transAxes,
+                )
 
-    # Super Labels
-    fig.supxlabel(iv_label, y=0.07)
-    fig.supylabel(dv_label)
-
-    # Legend
-    fig.legend(
-        ["Previous Data", "New Data", "Model"],
-        ncols=3,
-        bbox_to_anchor=(0.5, 0),
-        loc="lower center",
-    )
+            else:
+                ax.axis("off")
+
+        # Super Labels
+        fig.supxlabel(iv_label, y=0.07)
+        fig.supylabel(dv_label)
+
+        # Legend
+        fig.legend(
+            ["Previous Data", "New Data", "Model"],
+            ncols=3,
+            bbox_to_anchor=(0.5, 0),
+            loc="lower center",
+        )
 
     return fig
 
 
 def plot_results_panel_3d(
     state: SupportsControllerState,
     iv_names: Optional[List[str]] = None,
@@ -440,68 +449,68 @@
     l_predictions = _model_predict(state, np.column_stack((x1.ravel(), x2.ravel())))
 
     # Subplot configurations
     if n_cycles < wrap:
         shape = (1, n_cycles)
     else:
         shape = (int(np.ceil(n_cycles / wrap)), wrap)
+    with plt.rc_context(controller_plotting_rc_context):
+        fig, axs = plt.subplots(*shape, **d_kw["subplot_kw"])
 
-    fig, axs = plt.subplots(*shape, **d_kw["subplot_kw"])
-
-    # Loop by panel
-    for i, ax in enumerate(axs.flat):
-        if i + 1 <= n_cycles:
-            # ---Plot observed data---
-            # Independent variable values
-            l_x = [df_observed.loc[:, s[0]] for s in iv]
-            # Dependent values masked by current cycle vs previous data
-            dv_previous = np.ma.masked_where(
-                df_observed["cycle"] >= i, df_observed[dv[0]]
-            )
-            dv_current = np.ma.masked_where(
-                df_observed["cycle"] != i, df_observed[dv[0]]
-            )
-            # Plotting scatter
-            ax.scatter(*l_x, dv_previous, **d_kw["scatter_previous_kw"])
-            ax.scatter(*l_x, dv_current, **d_kw["scatter_current_kw"])
-
-            # ---Plot Model---
-            ax.plot_surface(
-                x1, x2, l_predictions[i].reshape(x1.shape), **d_kw["surface_kw"]
-            )
-            # ---Labels---
-            # Title
-            ax.set_title(f"Cycle {i}")
-
-            # Axis
-            ax.set_xlabel(iv_labels[0])
-            ax.set_ylabel(iv_labels[1])
-            ax.set_zlabel(dv_label)
-
-            # Viewing angle
-            if view:
-                ax.view_init(*view)
+        # Loop by panel
+        for i, ax in enumerate(axs.flat):
+            if i + 1 <= n_cycles:
+                # ---Plot observed data---
+                # Independent variable values
+                l_x = [df_observed.loc[:, s[0]] for s in iv]
+                # Dependent values masked by current cycle vs previous data
+                dv_previous = np.ma.masked_where(
+                    df_observed["cycle"] >= i, df_observed[dv[0]]
+                )
+                dv_current = np.ma.masked_where(
+                    df_observed["cycle"] != i, df_observed[dv[0]]
+                )
+                # Plotting scatter
+                ax.scatter(*l_x, dv_previous, **d_kw["scatter_previous_kw"])
+                ax.scatter(*l_x, dv_current, **d_kw["scatter_current_kw"])
+
+                # ---Plot Model---
+                ax.plot_surface(
+                    x1, x2, l_predictions[i].reshape(x1.shape), **d_kw["surface_kw"]
+                )
+                # ---Labels---
+                # Title
+                ax.set_title(f"Cycle {i}")
+
+                # Axis
+                ax.set_xlabel(iv_labels[0])
+                ax.set_ylabel(iv_labels[1])
+                ax.set_zlabel(dv_label)
+
+                # Viewing angle
+                if view:
+                    ax.view_init(*view)
 
-        else:
-            ax.axis("off")
+            else:
+                ax.axis("off")
 
-    # Legend
-    handles, labels = axs.flatten()[0].get_legend_handles_labels()
-    legend_elements = [
-        handles[0],
-        handles[1],
-        Patch(facecolor=handles[2].get_facecolors()[0]),
-    ]
-    fig.legend(
-        handles=legend_elements,
-        labels=labels,
-        ncols=3,
-        bbox_to_anchor=(0.5, 0),
-        loc="lower center",
-    )
+        # Legend
+        handles, labels = axs.flatten()[0].get_legend_handles_labels()
+        legend_elements = [
+            handles[0],
+            handles[1],
+            Patch(facecolor=handles[2].get_facecolors()[0]),
+        ]
+        fig.legend(
+            handles=legend_elements,
+            labels=labels,
+            ncols=3,
+            bbox_to_anchor=(0.5, 0),
+            loc="lower center",
+        )
 
     return fig
 
 
 def cycle_default_score(
     state: SupportsControllerState, x_vals: np.ndarray, y_true: np.ndarray
 ):
@@ -586,28 +595,29 @@
 
     # Use estimator's default scoring method if specific scorer is not supplied
     if scorer is None:
         l_scores = cycle_default_score(state, X, y_true)
     else:
         l_scores = cycle_specified_score(scorer, state, X, y_true, **scorer_kw)
 
-    # Plotting
-    fig, ax = plt.subplots(figsize=figsize)
-    ax.plot(np.arange(len(state.models)), l_scores, **plot_kw)
-
-    # Adjusting axis limits
-    if ylim:
-        ax.set_ylim(*ylim)
-    if xlim:
-        ax.set_xlim(*xlim)
-
-    # Labeling
-    ax.set_xlabel(x_label)
-    if y_label is None:
-        if scorer is not None:
-            y_label = scorer.__name__
-        else:
-            y_label = "Score"
-    ax.set_ylabel(y_label)
-    ax.xaxis.set_major_locator(MaxNLocator(integer=True))
+    with plt.rc_context(controller_plotting_rc_context):
+        # Plotting
+        fig, ax = plt.subplots(figsize=figsize)
+        ax.plot(np.arange(len(state.models)), l_scores, **plot_kw)
+
+        # Adjusting axis limits
+        if ylim:
+            ax.set_ylim(*ylim)
+        if xlim:
+            ax.set_xlim(*xlim)
+
+        # Labeling
+        ax.set_xlabel(x_label)
+        if y_label is None:
+            if scorer is not None:
+                y_label = scorer.__name__
+            else:
+                y_label = "Score"
+        ax.set_ylabel(y_label)
+        ax.xaxis.set_major_locator(MaxNLocator(integer=True))
 
     return fig
```

### Comparing `autora-workflow-0.3.6/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.4.0b1/src/autora/workflow/serializer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import pickle
 import tempfile
 from abc import abstractmethod
 from pathlib import Path
-from typing import Generic, Mapping, NamedTuple, Type, Union
+from typing import Generic, Mapping, NamedTuple, Type, TypeVar, Union
 
 import numpy as np
 
-from ..protocol import ResultKind, State, SupportsLoadDump
+from autora.state.history import History
+from autora.state.protocol import ResultKind, SupportsLoadDump
+
 from ..serializer import yaml_ as YAMLSerializer
-from ..state import History
+
+State = TypeVar("State")
 
 
 class _DumpSpec(NamedTuple):
     extension: str
     serializer: SupportsLoadDump
     mode: str
 
@@ -67,15 +70,15 @@
 
         Returns:
 
         Examples:
             First, we need to initialize a FilesystemCycleDataCollection. This is usually handled
             by the cycle itself. We start with a data collection as it would be at the very start of
             an experiment, with just a VariableCollection.
-            >>> from autora.workflow.state.history import History
+            >>> from autora.state.history import History
             >>> c = History()
             >>> c  #doctest: +NORMALIZE_WHITESPACE
             History([])
 
             Now we can serialize the data collection using _dumper. We define a helper function for
             demonstration purposes.
             >>> import tempfile
@@ -142,15 +145,15 @@
 
         Examples:
             First, we need to initialize a FilesystemCycleDataCollection. This is usually handled
             by the cycle itself. We construct a full set of results:
             >>> from sklearn.linear_model import LinearRegression
             >>> from autora.variable import VariableCollection
             >>> import numpy as np
-            >>> from autora.workflow.state.history import History
+            >>> from autora.state.history import History
             >>> import tempfile
             >>> x = np.linspace(-2, 2, 10).reshape(-1, 1) * np.pi
             >>> y = 3. * x + 0.1 * np.sin(x - 0.1) - 2.
             >>> estimator = LinearRegression().fit(x, y)
             >>> c = History(variables=VariableCollection(), conditions=[x],
             ...     observations=[np.column_stack([x, y])], models=[estimator])
 
@@ -158,15 +161,15 @@
             >>> with tempfile.TemporaryDirectory() as d:
             ...     s = HistorySerializer(d)
             ...     s.dump(c)
             ...     e = s.load()
 
             We can now compare the dumped object "c" with the reloaded object "e". The data arrays
             should be equal, and the models should
-            >>> from autora.workflow.protocol import ResultKind
+            >>> from autora.state.protocol import ResultKind
             >>> for e_i, c_i in zip(e.history, c.history):
             ...     assert isinstance(e_i.data, type(c_i.data)) # Types match
             ...     if e_i.kind in (ResultKind.CONDITION, ResultKind.OBSERVATION):
             ...         np.testing.assert_array_equal(e_i.data, c_i.data) # two numpy arrays
             ...     if e_i.kind == ResultKind.MODEL:
             ...         np.testing.assert_array_equal(e_i.data.coef_, c_i.data.coef_) # 2 estimators
```

### Comparing `autora-workflow-0.3.6/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.4.0b1/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.6
+Version: 0.4.0b1
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
```

### Comparing `autora-workflow-0.3.6/tests/test_controller_plots.py` & `autora-workflow-0.4.0b1/tests/test_controller_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import random
 
 import numpy as np
 import pytest
-from autora.experimentalist.pipeline import Pipeline
-from autora.experimentalist.pooler.grid import grid_pool
-from autora.experimentalist.sampler.random_sampler import random_sampler
-from autora.variable import Variable, VariableCollection
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import r2_score
 
+from autora.experimentalist.pipeline import Pipeline
+from autora.experimentalist.pooler.grid import grid_pool
+from autora.experimentalist.sampler.random_sampler import random_sample
+from autora.variable import Variable, VariableCollection
 from autora.workflow import Cycle
 from autora.workflow.plotting import (
     _check_replace_default_kw,
     cycle_default_score,
     cycle_specified_score,
     plot_cycle_score,
     plot_results_panel_2d,
@@ -43,20 +43,20 @@
     # Theorist
     lm = LinearRegression()
 
     # Experimentalist
     example_experimentalist = Pipeline(
         [
             ("pool", grid_pool),
-            ("sampler", random_sampler),
+            ("sampler", random_sample),
             ("transform", lambda x: [s[0] for s in x]),
         ],
         params={
             "pool": {"ivs": study_variables.independent_variables},
-            "sampler": {"n": 5},
+            "sampler": {"num_samples": 5},
         },
     )
 
     # Experiment Runner
     def get_example_synthetic_experiment_runner():
         rng = np.random.default_rng(seed=180)
 
@@ -108,20 +108,20 @@
     # Theorist
     lm = LinearRegression()
 
     # Experimentalist
     example_experimentalist = Pipeline(
         [
             ("pool", grid_pool),
-            ("sampler", random_sampler),
+            ("sampler", random_sample),
             ("transform", lambda x: np.array(x)),
         ],
         params={
             "pool": {"ivs": study_variables.independent_variables},
-            "sampler": {"n": 10},
+            "sampler": {"num_samples": 10},
         },
     )
 
     # Experiment Runner
     def get_example_synthetic_experiment_runner():
         rng = np.random.default_rng(seed=180)
```

