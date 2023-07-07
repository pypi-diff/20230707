# Comparing `tmp/Brian2-2.5.3.tar.gz` & `tmp/Brian2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Brian2-2.5.3.tar", last modified: Thu Jun 29 09:28:43 2023, max compression
+gzip compressed data, was "Brian2-2.5.4.tar", last modified: Fri Jul  7 13:26:37 2023, max compression
```

## Comparing `Brian2-2.5.3.tar` & `Brian2-2.5.4.tar`

### file list

```diff
@@ -1,533 +1,533 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.701420 Brian2-2.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.637419 Brian2-2.5.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-29 09:28:15.000000 Brian2-2.5.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-29 09:28:15.000000 Brian2-2.5.3/.devcontainer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 09:28:15.000000 Brian2-2.5.3/.devcontainer/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-29 09:28:15.000000 Brian2-2.5.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-29 09:28:15.000000 Brian2-2.5.3/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 09:28:15.000000 Brian2-2.5.3/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.629419 Brian2-2.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.637419 Brian2-2.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-29 09:28:15.000000 Brian2-2.5.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-29 09:28:15.000000 Brian2-2.5.3/.github/workflows/test_latest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-29 09:28:15.000000 Brian2-2.5.3/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-29 09:28:15.000000 Brian2-2.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 09:28:15.000000 Brian2-2.5.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-29 09:28:15.000000 Brian2-2.5.3/AUTHORS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.637419 Brian2-2.5.3/Brian2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-29 09:28:43.000000 Brian2-2.5.3/Brian2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-06-29 09:28:43.000000 Brian2-2.5.3/Brian2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:28:43.000000 Brian2-2.5.3/Brian2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:28:43.000000 Brian2-2.5.3/Brian2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 09:28:43.000000 Brian2-2.5.3/Brian2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 09:28:43.000000 Brian2-2.5.3/Brian2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-29 09:28:15.000000 Brian2-2.5.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-29 09:28:15.000000 Brian2-2.5.3/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-29 09:28:15.000000 Brian2-2.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-06-29 09:28:15.000000 Brian2-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-29 09:28:15.000000 Brian2-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-29 09:28:43.701420 Brian2-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-29 09:28:15.000000 Brian2-2.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.637419 Brian2-2.5.3/brian2/
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 09:28:43.000000 Brian2-2.5.3/brian2/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.637419 Brian2-2.5.3/brian2/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/_prefs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/codeobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/cpp_prefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.637419 Brian2-2.5.3/brian2/codegen/generators/
--rw-r--r--   0 runner    (1001) docker     (123)    45261 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/generators/GSL_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/generators/cpp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/generators/cython_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/generators/numpy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/get_cpu_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    27207 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/optimisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/permutation_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.641420 Brian2-2.5.3/brian2/codegen/runtime/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.641420 Brian2-2.5.3/brian2/codegen/runtime/GSLcython_rt/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/GSLcython_rt/GSLcython_rt.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/GSLcython_rt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.641420 Brian2-2.5.3/brian2/codegen/runtime/GSLcython_rt/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/GSLcython_rt/templates/stateupdate.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.641420 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/cython_rt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/extension_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.641420 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/common_group.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_get_indices.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_variable_get.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_variable_get_conditional.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_variable_set.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_variable_set_conditional.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/ratemonitor.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/reset.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/spatialstateupdate.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/spikegenerator.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/spikemonitor.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/statemonitor.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/stateupdate.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/summed_variable.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/synapses.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/synapses_create_array.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/synapses_create_generator.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/synapses_push_spikes.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/threshold.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.641420 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/numpy_rt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.645419 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/common_group.py_
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/group_get_indices.py_
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/group_variable_get.py_
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/group_variable_get_conditional.py_
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/group_variable_set.py_
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/group_variable_set_conditional.py_
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/ratemonitor.py_
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/reset.py_
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/spatialstateupdate.py_
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/spikegenerator.py_
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/spikemonitor.py_
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/statemonitor.py_
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/stateupdate.py_
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/summed_variable.py_
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/synapses.py_
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/synapses_create_array.py_
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/synapses_create_generator.py_
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/synapses_push_spikes.py_
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/threshold.py_
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/statements.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/codegen/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.649419 Brian2-2.5.3/brian2/core/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/clocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/core_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    34429 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    54492 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/spikesource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)    77722 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/core/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.649419 Brian2-2.5.3/brian2/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.649419 Brian2-2.5.3/brian2/devices/cpp_standalone/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/GSLcodeobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.649419 Brian2-2.5.3/brian2/devices/cpp_standalone/brianlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/brianlib/clocks.h
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/brianlib/common_math.h
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/brianlib/dynamic_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/codeobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    76047 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.653420 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/common_group.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/common_synapses.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/group_variable_set.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/group_variable_set_conditional.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/network.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/objects.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/ratemonitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/reset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/run.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/spatialstateupdate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/spikegenerator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/spikemonitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/statemonitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/stateupdate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/summed_variable.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_classes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_create_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_create_generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_push_spikes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/threshold.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates/win_makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.653420 Brian2-2.5.3/brian2/devices/cpp_standalone/templates_GSL/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/cpp_standalone/templates_GSL/stateupdate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/devices/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.653420 Brian2-2.5.3/brian2/equations/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/equations/codestrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    49697 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/equations/equations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/equations/refractory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/equations/unitcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.653420 Brian2-2.5.3/brian2/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49452 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    40545 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/groups/neurongroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/groups/subgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/hears.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.653420 Brian2-2.5.3/brian2/importexport/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/importexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/importexport/dictlike.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/importexport/importexport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/input/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/input/binomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/input/poissongroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/input/poissoninput.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/input/spikegeneratorgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/input/timedarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/memory/dynamicarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/monitors/ratemonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21346 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/monitors/spikemonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/monitors/statemonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/numpy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/only.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/bast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/parsing/sympytools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/random/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/random/randomkit/
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/random/randomkit/randomkit.c
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/random/randomkit/randomkit.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/spatialneuron/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/spatialneuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84474 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/spatialneuron/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/spatialneuron/mp_ma_40984_gc2.CNG.swc
--rw-r--r--   0 runner    (1001) docker     (123)    28264 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/spatialneuron/spatialneuron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.657420 Brian2-2.5.3/brian2/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/sphinxext/briandoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/sphinxext/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/sphinxext/docscrape_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/sphinxext/examplefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/sphinxext/generate_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/sphinxext/generate_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.661419 Brian2-2.5.3/brian2/stateupdaters/
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/stateupdaters/GSL.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/stateupdaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/stateupdaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/stateupdaters/exact.py
--rw-r--r--   0 runner    (1001) docker     (123)    32865 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/stateupdaters/explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/stateupdaters/exponential_euler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.661419 Brian2-2.5.3/brian2/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/synapses/cspikequeue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)  1052869 2023-06-29 09:28:42.000000 Brian2-2.5.3/brian2/synapses/cythonspikequeue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/synapses/cythonspikequeue.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/synapses/parse_synaptic_generator_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/synapses/spikequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/synapses/stdint_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    90340 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/synapses/synapses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.669420 Brian2-2.5.3/brian2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19714 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.669420 Brian2-2.5.3/brian2/tests/features/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/features/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/features/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/features/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/features/neurongroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/features/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/features/synapses.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/func_def_cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/func_def_cpp.h
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/func_def_cython.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/func_def_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.669420 Brian2-2.5.3/brian2/tests/rallpack_data/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/rallpack_data/README
--rw-r--r--   0 runner    (1001) docker     (123)    91545 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/rallpack_data/ref_axon.0.neuron
--rw-r--r--   0 runner    (1001) docker     (123)    91387 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/rallpack_data/ref_axon.x.neuron
--rw-r--r--   0 runner    (1001) docker     (123)   115023 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/rallpack_data/ref_branch.0
--rw-r--r--   0 runner    (1001) docker     (123)   115023 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/rallpack_data/ref_branch.x
--rw-r--r--   0 runner    (1001) docker     (123)   110212 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/rallpack_data/ref_cable.0
--rw-r--r--   0 runner    (1001) docker     (123)   110885 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/rallpack_data/ref_cable.x
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_GSL.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_clocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22945 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_codestrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_complex_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_cpp_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_equations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32728 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    25861 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    61373 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    66962 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_neurongroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_numpy_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_poissongroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_poissoninput.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_refractory.py
--rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_spatialneuron.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_spikegenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_spikequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33239 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_stateupdaters.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_subgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_synapses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.669420 Brian2-2.5.3/brian2/tests/test_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.669420 Brian2-2.5.3/brian2/tests/test_templates/fake_package_1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.669420 Brian2-2.5.3/brian2/tests/test_templates/fake_package_1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_1/templates/A.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_1/templates/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_1/templates/C.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_1/templates/D.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.673420 Brian2-2.5.3/brian2/tests/test_templates/fake_package_2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.673420 Brian2-2.5.3/brian2/tests/test_templates/fake_package_2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_2/templates/A.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/fake_package_2/templates/D.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_templates/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_thresholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_timedarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    52444 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.673420 Brian2-2.5.3/brian2/units/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   260560 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/units/allunits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/units/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    93505 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/units/fundamentalunits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/units/stdunits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/units/unitsafefunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.673420 Brian2-2.5.3/brian2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/filetools.py
--rw-r--r--   0 runner    (1001) docker     (123)    30699 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/stringtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-29 09:28:15.000000 Brian2-2.5.3/brian2/utils/topsort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.673420 Brian2-2.5.3/docs_sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.673420 Brian2-2.5.3/docs_sphinx/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/_static/brian-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.677420 Brian2-2.5.3/docs_sphinx/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/custom_events.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/custom_events.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/custom_events.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/how_brian_works.rst
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/namespaces.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/preferences.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/random.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/scheduling.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/advanced/state_update.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.677420 Brian2-2.5.3/docs_sphinx/developer/
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/GSL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/codegen.rst
--rw-r--r--   0 runner    (1001) docker     (123)   184235 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/codegen_code_paths.png
--rw-r--r--   0 runner    (1001) docker     (123)    72864 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/codegen_code_paths.pptx
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/equations_namespaces.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/functions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.681420 Brian2-2.5.3/docs_sphinx/developer/guidelines/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/defensive_programming.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/representation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/style.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/guidelines/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/oldcodegen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/openmp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/preferences.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/standalone.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/developer/variables_indices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.681420 Brian2-2.5.3/docs_sphinx/introduction/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.681420 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/brian1hears_bridge.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/inputs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/monitors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/multicompartmental.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/networks_and_clocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21957 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/neurongroup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/preferences.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/synapses.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)    94329 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/introduction/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.685420 Brian2-2.5.3/docs_sphinx/user/
--rw-r--r--   0 runner    (1001) docker     (123)    16663 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/computation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/converting_from_integrated_form.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/equations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.685420 Brian2-2.5.3/docs_sphinx/user/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/cylinder.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/cylinder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/function_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    61652 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/morphology_deterministic_coords.png
--rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_compartment_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_compartment_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_compartment_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/section.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/section.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/soma.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/images/soma.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/import.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/input.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/multicompartmental.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/numerical_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/plotting_functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/recording.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/refractoriness.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28910 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/synapses.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-29 09:28:15.000000 Brian2-2.5.3/docs_sphinx/user/units.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.689420 Brian2-2.5.3/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/COBAHH.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/CUBA.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/IF_curve_Hodgkin_Huxley.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/IF_curve_LIF.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/adaptive_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.689420 Brian2-2.5.3/examples/advanced/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11236 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/COBAHH_approximated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1285 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/Ornstein_Uhlenbeck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/compare_GSL_to_conventional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/custom_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/exprel_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/float_32_64_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/modelfitting_sbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/opencv_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/advanced/stochastic_odes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.689420 Brian2-2.5.3/examples/compartmental/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/bipolar_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/bipolar_with_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/bipolar_with_inputs2.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/hh_with_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/hodgkin_huxley_1952.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/infinite_cable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/lfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/morphotest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/rall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/compartmental/spike_initiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/coupled_oscillators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.697420 Brian2-2.5.3/examples/frompapers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2004.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.697420 Brian2-2.5.3/examples/frompapers/Brette_2012/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2012/Fig1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2012/Fig3AB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2012/Fig3CF.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2012/Fig4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2012/Fig5A.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2012/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_2012/params.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_Gerstner_2005.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brette_Guigon_2003.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brunel_2000.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brunel_Hakim_1999.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Brunel_Wang_2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Clopath_et_al_2010_homeostasis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Clopath_et_al_2010_no_homeostasis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Destexhe_et_al_1998.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1436 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Diesmann_et_al_1999.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4637 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Graupner_Brunel_2012.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Hindmarsh_Rose_1984.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Izhikevich_2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Izhikevich_2007.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Jansen_Rit_1995_single_column.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6508 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Kremer_et_al_2011_barrel_cortex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11959 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Maass_Natschlaeger_Markram_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Morris_Lecar_1981.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4421 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Naud_et_al_2008_adex_firing_patterns.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Nicola_Clopath_2017.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2879 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Platkiewicz_Brette_2011.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Rossant_et_al_2011bis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4454 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Rothman_Manis_2003.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.697420 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_1_COBA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_2_gchi_astrocyte.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_3_io_synapse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_4_rsmean.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_4_synrel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_5_astro_ring.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_6_COBA_with_astro.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/figures.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/plot_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2216 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Sturzl_et_al_2000.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7097 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Tetzlaff_2015.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Touboul_Brette_2008.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5508 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Tsodyks_Pawelzik_Markram_1998.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7895 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Tsodyks_Uziel_Markram_2000.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Vogels_et_al_2011.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/frompapers/Wang_Buszaki_1996.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.697420 Brian2-2.5.3/examples/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/multiprocessing/01_using_cython.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/multiprocessing/02_using_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/multiprocessing/03_standalone_joblib.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/non_reliability.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/phase_locking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/reliability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.697420 Brian2-2.5.3/examples/standalone/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/standalone/STDP_standalone.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/standalone/cuba_openmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/standalone/simple_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/standalone/simple_case_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/standalone/standalone_multiplerun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:28:43.701420 Brian2-2.5.3/examples/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/STDP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/continuous_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/efficient_gaussian_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/gapjunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2074 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/jeffress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/licklider.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/nonlinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/spatial_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4610 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/spike_based_homeostasis.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/state_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-29 09:28:15.000000 Brian2-2.5.3/examples/synapses/synapses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-29 09:28:15.000000 Brian2-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-29 09:28:15.000000 Brian2-2.5.3/rtd-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 09:28:43.701420 Brian2-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-29 09:28:15.000000 Brian2-2.5.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-29 09:28:15.000000 Brian2-2.5.3/versions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.108244 Brian2-2.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.052244 Brian2-2.5.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 13:26:10.000000 Brian2-2.5.4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-07 13:26:10.000000 Brian2-2.5.4/.devcontainer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 13:26:10.000000 Brian2-2.5.4/.devcontainer/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-07 13:26:10.000000 Brian2-2.5.4/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 13:26:10.000000 Brian2-2.5.4/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 13:26:10.000000 Brian2-2.5.4/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.048244 Brian2-2.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-07 13:26:10.000000 Brian2-2.5.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-07 13:26:10.000000 Brian2-2.5.4/.github/workflows/test_latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-07 13:26:10.000000 Brian2-2.5.4/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-07 13:26:10.000000 Brian2-2.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 13:26:10.000000 Brian2-2.5.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-07 13:26:10.000000 Brian2-2.5.4/AUTHORS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/Brian2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-07 13:26:36.000000 Brian2-2.5.4/Brian2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-07-07 13:26:37.000000 Brian2-2.5.4/Brian2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:26:36.000000 Brian2-2.5.4/Brian2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:26:36.000000 Brian2-2.5.4/Brian2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-07 13:26:36.000000 Brian2-2.5.4/Brian2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 13:26:36.000000 Brian2-2.5.4/Brian2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-07 13:26:10.000000 Brian2-2.5.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-07 13:26:10.000000 Brian2-2.5.4/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-07 13:26:10.000000 Brian2-2.5.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-07-07 13:26:10.000000 Brian2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-07 13:26:10.000000 Brian2-2.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-07 13:26:37.108244 Brian2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-07 13:26:10.000000 Brian2-2.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/brian2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 13:26:36.000000 Brian2-2.5.4/brian2/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/brian2/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/_prefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/codeobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/cpp_prefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/brian2/codegen/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)    45261 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/generators/GSL_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/generators/cpp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/generators/cython_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/generators/numpy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/get_cpu_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27207 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/permutation_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/brian2/codegen/runtime/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/brian2/codegen/runtime/GSLcython_rt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/GSLcython_rt/GSLcython_rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/GSLcython_rt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.056244 Brian2-2.5.4/brian2/codegen/runtime/GSLcython_rt/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/GSLcython_rt/templates/stateupdate.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.060244 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/cython_rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/extension_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.060244 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/common_group.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_get_indices.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_variable_get.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_variable_get_conditional.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_variable_set.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_variable_set_conditional.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/ratemonitor.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/reset.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/spatialstateupdate.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/spikegenerator.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/spikemonitor.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/statemonitor.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/stateupdate.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/summed_variable.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/synapses.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/synapses_create_array.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/synapses_create_generator.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/synapses_push_spikes.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/threshold.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.060244 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/numpy_rt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.064244 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/common_group.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/group_get_indices.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/group_variable_get.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/group_variable_get_conditional.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/group_variable_set.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/group_variable_set_conditional.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/ratemonitor.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/reset.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/spatialstateupdate.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/spikegenerator.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/spikemonitor.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/statemonitor.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/stateupdate.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/summed_variable.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/synapses.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/synapses_create_array.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/synapses_create_generator.py_
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/synapses_push_spikes.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/threshold.py_
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/codegen/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.064244 Brian2-2.5.4/brian2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/clocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/core_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34429 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54492 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/spikesource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77722 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/core/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.064244 Brian2-2.5.4/brian2/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.064244 Brian2-2.5.4/brian2/devices/cpp_standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/GSLcodeobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.064244 Brian2-2.5.4/brian2/devices/cpp_standalone/brianlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/brianlib/clocks.h
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/brianlib/common_math.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/brianlib/dynamic_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/codeobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76047 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.068244 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/common_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/common_synapses.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/group_variable_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/group_variable_set_conditional.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/network.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/objects.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/ratemonitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/reset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/run.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/spatialstateupdate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/spikegenerator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/spikemonitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/statemonitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/stateupdate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/summed_variable.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_classes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_create_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_create_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_push_spikes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/threshold.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates/win_makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.068244 Brian2-2.5.4/brian2/devices/cpp_standalone/templates_GSL/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/cpp_standalone/templates_GSL/stateupdate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/devices/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.068244 Brian2-2.5.4/brian2/equations/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/equations/codestrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49697 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/equations/equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/equations/refractory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/equations/unitcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.068244 Brian2-2.5.4/brian2/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49452 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40545 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/groups/neurongroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/groups/subgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/hears.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.068244 Brian2-2.5.4/brian2/importexport/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/importexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/importexport/dictlike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/importexport/importexport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.068244 Brian2-2.5.4/brian2/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/input/binomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/input/poissongroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/input/poissoninput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/input/spikegeneratorgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/input/timedarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/memory/dynamicarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/monitors/ratemonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21346 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/monitors/spikemonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/monitors/statemonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/numpy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/only.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/bast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/parsing/sympytools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/random/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/random/randomkit/
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/random/randomkit/randomkit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/random/randomkit/randomkit.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/spatialneuron/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/spatialneuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84474 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/spatialneuron/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/spatialneuron/mp_ma_40984_gc2.CNG.swc
+-rw-r--r--   0 runner    (1001) docker     (123)    28264 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/spatialneuron/spatialneuron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/sphinxext/briandoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/sphinxext/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/sphinxext/docscrape_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/sphinxext/examplefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/sphinxext/generate_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/sphinxext/generate_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.072244 Brian2-2.5.4/brian2/stateupdaters/
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/stateupdaters/GSL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/stateupdaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/stateupdaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/stateupdaters/exact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32865 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/stateupdaters/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/stateupdaters/exponential_euler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.076244 Brian2-2.5.4/brian2/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/synapses/cspikequeue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)  1054046 2023-07-07 13:26:35.000000 Brian2-2.5.4/brian2/synapses/cythonspikequeue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/synapses/cythonspikequeue.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/synapses/parse_synaptic_generator_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/synapses/spikequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/synapses/stdint_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    90340 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/synapses/synapses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.080244 Brian2-2.5.4/brian2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19714 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.084244 Brian2-2.5.4/brian2/tests/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/features/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/features/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/features/neurongroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/features/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/features/synapses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/func_def_cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/func_def_cpp.h
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/func_def_cython.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/func_def_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.084244 Brian2-2.5.4/brian2/tests/rallpack_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/rallpack_data/README
+-rw-r--r--   0 runner    (1001) docker     (123)    91545 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/rallpack_data/ref_axon.0.neuron
+-rw-r--r--   0 runner    (1001) docker     (123)    91387 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/rallpack_data/ref_axon.x.neuron
+-rw-r--r--   0 runner    (1001) docker     (123)   115023 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/rallpack_data/ref_branch.0
+-rw-r--r--   0 runner    (1001) docker     (123)   115023 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/rallpack_data/ref_branch.x
+-rw-r--r--   0 runner    (1001) docker     (123)   110212 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/rallpack_data/ref_cable.0
+-rw-r--r--   0 runner    (1001) docker     (123)   110885 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/rallpack_data/ref_cable.x
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_GSL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_clocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22945 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_codestrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_complex_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_cpp_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32728 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25861 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61373 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66962 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_neurongroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_numpy_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_poissongroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_poissoninput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_refractory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_spatialneuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_spikegenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_spikequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33239 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_stateupdaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_subgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_synapses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.084244 Brian2-2.5.4/brian2/tests/test_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.084244 Brian2-2.5.4/brian2/tests/test_templates/fake_package_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.084244 Brian2-2.5.4/brian2/tests/test_templates/fake_package_1/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_1/templates/A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_1/templates/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_1/templates/C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_1/templates/D.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.084244 Brian2-2.5.4/brian2/tests/test_templates/fake_package_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.084244 Brian2-2.5.4/brian2/tests/test_templates/fake_package_2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_2/templates/A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/fake_package_2/templates/D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_templates/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_thresholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_timedarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52444 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.088244 Brian2-2.5.4/brian2/units/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   260560 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/units/allunits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/units/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93505 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/units/fundamentalunits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/units/stdunits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/units/unitsafefunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.088244 Brian2-2.5.4/brian2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/filetools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30699 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/stringtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-07 13:26:10.000000 Brian2-2.5.4/brian2/utils/topsort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.088244 Brian2-2.5.4/docs_sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.088244 Brian2-2.5.4/docs_sphinx/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/_static/brian-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.088244 Brian2-2.5.4/docs_sphinx/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/custom_events.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/custom_events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/custom_events.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/how_brian_works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/namespaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/preferences.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/random.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/scheduling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/advanced/state_update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.092244 Brian2-2.5.4/docs_sphinx/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/GSL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/codegen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   184235 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/codegen_code_paths.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72864 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/codegen_code_paths.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/equations_namespaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/functions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.092244 Brian2-2.5.4/docs_sphinx/developer/guidelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/defensive_programming.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/representation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/style.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/guidelines/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/oldcodegen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/openmp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/preferences.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/standalone.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/developer/variables_indices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.092244 Brian2-2.5.4/docs_sphinx/introduction/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.096244 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/brian1hears_bridge.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/inputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/monitors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/multicompartmental.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/networks_and_clocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21957 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/neurongroup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/preferences.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/synapses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    95276 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/introduction/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.096244 Brian2-2.5.4/docs_sphinx/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    16663 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/computation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/converting_from_integrated_form.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/equations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.100244 Brian2-2.5.4/docs_sphinx/user/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/cylinder.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/cylinder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/function_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61652 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/morphology_deterministic_coords.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_compartment_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_compartment_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_compartment_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/section.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/section.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/soma.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/images/soma.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/import.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/input.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/multicompartmental.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/numerical_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/plotting_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/recording.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/refractoriness.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28910 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/synapses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-07 13:26:10.000000 Brian2-2.5.4/docs_sphinx/user/units.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.100244 Brian2-2.5.4/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/COBAHH.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/CUBA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/IF_curve_Hodgkin_Huxley.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/IF_curve_LIF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/adaptive_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.100244 Brian2-2.5.4/examples/advanced/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11236 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/COBAHH_approximated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1285 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/Ornstein_Uhlenbeck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/compare_GSL_to_conventional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/custom_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/exprel_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/float_32_64_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/modelfitting_sbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/opencv_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/advanced/stochastic_odes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.100244 Brian2-2.5.4/examples/compartmental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/bipolar_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/bipolar_with_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/bipolar_with_inputs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/hh_with_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/hodgkin_huxley_1952.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/infinite_cable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/lfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/morphotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/rall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/compartmental/spike_initiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/coupled_oscillators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.104244 Brian2-2.5.4/examples/frompapers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2004.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.104244 Brian2-2.5.4/examples/frompapers/Brette_2012/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2012/Fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2012/Fig3AB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2012/Fig3CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2012/Fig4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2012/Fig5A.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2012/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_2012/params.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_Gerstner_2005.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brette_Guigon_2003.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brunel_2000.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brunel_Hakim_1999.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Brunel_Wang_2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Clopath_et_al_2010_homeostasis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Clopath_et_al_2010_no_homeostasis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Destexhe_et_al_1998.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1436 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Diesmann_et_al_1999.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4637 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Graupner_Brunel_2012.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Hindmarsh_Rose_1984.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Izhikevich_2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Izhikevich_2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Jansen_Rit_1995_single_column.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6508 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Kremer_et_al_2011_barrel_cortex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11959 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Maass_Natschlaeger_Markram_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Morris_Lecar_1981.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4421 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Naud_et_al_2008_adex_firing_patterns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Nicola_Clopath_2017.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2879 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Platkiewicz_Brette_2011.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Rossant_et_al_2011bis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4454 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Rothman_Manis_2003.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.108244 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_1_COBA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_2_gchi_astrocyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_3_io_synapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_4_rsmean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_4_synrel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_5_astro_ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_6_COBA_with_astro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/figures.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/plot_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2216 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Sturzl_et_al_2000.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7097 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Tetzlaff_2015.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Touboul_Brette_2008.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5508 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Tsodyks_Pawelzik_Markram_1998.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7895 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Tsodyks_Uziel_Markram_2000.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Vogels_et_al_2011.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/frompapers/Wang_Buszaki_1996.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.108244 Brian2-2.5.4/examples/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/multiprocessing/01_using_cython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/multiprocessing/02_using_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/multiprocessing/03_standalone_joblib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/non_reliability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/phase_locking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/reliability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.108244 Brian2-2.5.4/examples/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/standalone/STDP_standalone.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/standalone/cuba_openmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/standalone/simple_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/standalone/simple_case_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/standalone/standalone_multiplerun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:26:37.108244 Brian2-2.5.4/examples/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/STDP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/continuous_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/efficient_gaussian_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/gapjunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2074 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/jeffress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/licklider.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/spatial_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4610 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/spike_based_homeostasis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/state_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-07 13:26:10.000000 Brian2-2.5.4/examples/synapses/synapses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-07 13:26:10.000000 Brian2-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-07 13:26:10.000000 Brian2-2.5.4/rtd-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-07 13:26:37.112244 Brian2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-07 13:26:10.000000 Brian2-2.5.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-07 13:26:10.000000 Brian2-2.5.4/versions.md
```

### Comparing `Brian2-2.5.3/.devcontainer/Dockerfile` & `Brian2-2.5.4/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/.devcontainer/README.md` & `Brian2-2.5.4/.devcontainer/README.md`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/.devcontainer/devcontainer.json` & `Brian2-2.5.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/.git-blame-ignore-revs` & `Brian2-2.5.4/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/.github/workflows/publish_to_pypi.yml` & `Brian2-2.5.4/.github/workflows/publish_to_pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         with:
           output-dir: dist
         env:
           CIBW_PROJECT_REQUIRES_PYTHON: ">=${{ needs.get_python_versions.outputs.min-python }}"
           CIBW_ARCHS_WINDOWS: auto64
           CIBW_ARCHS_MACOS: x86_64 universal2
           CIBW_TEST_SKIP: '*_arm64 *_universal2:arm64'
-          CIBW_SKIP: 'pp* *-musllinux_*'
+          CIBW_SKIP: 'pp*'
           CIBW_TEST_COMMAND: python {project}/dev/continuous-integration/run_simple_test.py
           CIBW_TEST_REQUIRES: pytest
       - name: store distribution 📦
         uses: actions/upload-artifact@v3
         with:
           name: packages
           path: dist
@@ -79,15 +79,15 @@
         uses: pypa/cibuildwheel@v2.12.1
         with:
           output-dir: dist
         env:
           CIBW_PROJECT_REQUIRES_PYTHON: ">=${{ needs.get_python_versions.outputs.min-python }}"
           CIBW_ARCHS_LINUX: ${{ matrix.arch }}
           CIBW_MANYLINUX_X86_64_IMAGE: manylinux2014
-          CIBW_SKIP: 'pp* *-musllinux_*'
+          CIBW_SKIP: 'pp* *-musllinux_aarch64'
           CIBW_TEST_COMMAND: python {project}/dev/continuous-integration/run_simple_test.py
           CIBW_TEST_REQUIRES: pytest
       - name: store distribution 📦
         uses: actions/upload-artifact@v3
         with:
           name: packages
           path: dist
```

### Comparing `Brian2-2.5.3/.github/workflows/test_latest.yml` & `Brian2-2.5.4/.github/workflows/test_latest.yml`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/.github/workflows/testsuite.yml` & `Brian2-2.5.4/.github/workflows/testsuite.yml`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/.pre-commit-config.yaml` & `Brian2-2.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/AUTHORS` & `Brian2-2.5.4/AUTHORS`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/Brian2.egg-info/PKG-INFO` & `Brian2-2.5.4/Brian2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: Brian2
-Version: 2.5.3
+Version: 2.5.4
 Summary: A clock-driven simulator for spiking neural networks
-Author: Dan Goodman, Romain Brette
-Author-email: Marcel Stimberg <marcel.stimberg@inserm.fr>
+Author: Marcel Stimberg, Dan Goodman, Romain Brette
 Project-URL: Homepage, https://briansimulator.org
 Project-URL: Documentation, https://brian2.readthedocs.io/
 Project-URL: Source, https://github.com/brian-team/brian2
 Project-URL: Tracker, https://github.com/brian-team/brian2/issues
 Keywords: computational neuroscience,simulation,neural networks,spiking neurons,biological neural networks,research
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -63,20 +62,22 @@
    :target: https://spack.readthedocs.io/en/latest/package_list.html#py-brian2
 
 .. image:: https://img.shields.io/aur/version/python-brian2
    :alt: AUR version   
    :target: https://aur.archlinux.org/packages/python-brian2
 
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5910837.svg
-   :target: https://doi.org/10.5281/zenodo.5910837
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8099373.svg
+   :target: https://doi.org/10.5281/zenodo.8099373
 
-.. image:: https://archive.softwareheritage.org/badge/swh:1:rel:5f3d6b8e531d64530ac93ce5134194cf66a495b9/
-    :target: https://archive.softwareheritage.org/swh:1:rel:5f3d6b8e531d64530ac93ce5134194cf66a495b9;origin=https://github.com/brian-team/brian2;visit=swh:1:snp:06606ee7c757a47bc7dc168d0bfa8b0a5aecb620
+.. image:: https://archive.softwareheritage.org/badge/origin/https://github.com/brian-team/brian2/
+    :target: https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/brian-team/brian2
 
+.. image:: https://archive.softwareheritage.org/badge/swh:1:rel:e4d609023553bfbd62bf57960dd6f9d342a1d0e8/
+    :target: https://archive.softwareheritage.org/swh:1:rel:e4d609023553bfbd62bf57960dd6f9d342a1d0e8;origin=https://github.com/brian-team/brian2;visit=swh:1:snp:becb452d988ab8ea1386d27f3ad4c2221ec0ae7b
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg
         :target: CODE_OF_CONDUCT.md
         :alt: Contributor Covenant
 
 .. image:: https://img.shields.io/discourse/topics?server=https%3A%2F%2Fbrian.discourse.group
         :target: https://brian.discourse.group
```

### Comparing `Brian2-2.5.3/Brian2.egg-info/SOURCES.txt` & `Brian2-2.5.4/Brian2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/CITATION.cff` & `Brian2-2.5.4/CITATION.cff`

 * *Files 12% similar despite different names*

```diff
@@ -9,26 +9,26 @@
   - family-names: Goodman
     given-names: Dan F. M.
     orcid: "https://orcid.org/0000-0003-1007-6474"
   - family-names: Brette
     given-names: Romain
     orcid: "https://orcid.org/0000-0003-0110-1623"
   - name: "Brian contributors"
-version: 2.5.0.3
-date-released: "2022-01-27"
+version: 2.5.3
+date-released: "2023-06-29"
 identifiers:
   - description: This is the collection of archived snapshots of all versions of Brian 2
     type: doi
     value: "10.5281/zenodo.654861"
-  - description: This is the archived snapshot of version 2.5.0.3 of Brian 2
+  - description: This is the archived snapshot of version 2.5.3 of Brian 2
     type: doi
-    value: "10.5281/zenodo.5910837"
-  - description: Software heritage identifier for version 2.5.0.3
+    value: "10.5281/zenodo.8099373"
+  - description: Software heritage identifier for version 2.5.3
     type: swh
-    value: "swh:1:rel:5f3d6b8e531d64530ac93ce5134194cf66a495b9"
+    value: "swh:1:rel:e4d609023553bfbd62bf57960dd6f9d342a1d0e8"
 license: CECILL-2.1
 repository-code: "https://github.com/brian-team/brian2"
 preferred-citation:
     authors:
       - family-names: Stimberg
         given-names: Marcel
         orcid: "https://orcid.org/0000-0002-2648-4790"
```

### Comparing `Brian2-2.5.3/CODE_OF_CONDUCT.md` & `Brian2-2.5.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/LICENSE` & `Brian2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/MANIFEST.in` & `Brian2-2.5.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/PKG-INFO` & `Brian2-2.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: Brian2
-Version: 2.5.3
+Version: 2.5.4
 Summary: A clock-driven simulator for spiking neural networks
-Author: Dan Goodman, Romain Brette
-Author-email: Marcel Stimberg <marcel.stimberg@inserm.fr>
+Author: Marcel Stimberg, Dan Goodman, Romain Brette
 Project-URL: Homepage, https://briansimulator.org
 Project-URL: Documentation, https://brian2.readthedocs.io/
 Project-URL: Source, https://github.com/brian-team/brian2
 Project-URL: Tracker, https://github.com/brian-team/brian2/issues
 Keywords: computational neuroscience,simulation,neural networks,spiking neurons,biological neural networks,research
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -63,20 +62,22 @@
    :target: https://spack.readthedocs.io/en/latest/package_list.html#py-brian2
 
 .. image:: https://img.shields.io/aur/version/python-brian2
    :alt: AUR version   
    :target: https://aur.archlinux.org/packages/python-brian2
 
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5910837.svg
-   :target: https://doi.org/10.5281/zenodo.5910837
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8099373.svg
+   :target: https://doi.org/10.5281/zenodo.8099373
 
-.. image:: https://archive.softwareheritage.org/badge/swh:1:rel:5f3d6b8e531d64530ac93ce5134194cf66a495b9/
-    :target: https://archive.softwareheritage.org/swh:1:rel:5f3d6b8e531d64530ac93ce5134194cf66a495b9;origin=https://github.com/brian-team/brian2;visit=swh:1:snp:06606ee7c757a47bc7dc168d0bfa8b0a5aecb620
+.. image:: https://archive.softwareheritage.org/badge/origin/https://github.com/brian-team/brian2/
+    :target: https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/brian-team/brian2
 
+.. image:: https://archive.softwareheritage.org/badge/swh:1:rel:e4d609023553bfbd62bf57960dd6f9d342a1d0e8/
+    :target: https://archive.softwareheritage.org/swh:1:rel:e4d609023553bfbd62bf57960dd6f9d342a1d0e8;origin=https://github.com/brian-team/brian2;visit=swh:1:snp:becb452d988ab8ea1386d27f3ad4c2221ec0ae7b
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg
         :target: CODE_OF_CONDUCT.md
         :alt: Contributor Covenant
 
 .. image:: https://img.shields.io/discourse/topics?server=https%3A%2F%2Fbrian.discourse.group
         :target: https://brian.discourse.group
```

### Comparing `Brian2-2.5.3/README.rst` & `Brian2-2.5.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,22 @@
    :target: https://spack.readthedocs.io/en/latest/package_list.html#py-brian2
 
 .. image:: https://img.shields.io/aur/version/python-brian2
    :alt: AUR version   
    :target: https://aur.archlinux.org/packages/python-brian2
 
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5910837.svg
-   :target: https://doi.org/10.5281/zenodo.5910837
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8099373.svg
+   :target: https://doi.org/10.5281/zenodo.8099373
 
-.. image:: https://archive.softwareheritage.org/badge/swh:1:rel:5f3d6b8e531d64530ac93ce5134194cf66a495b9/
-    :target: https://archive.softwareheritage.org/swh:1:rel:5f3d6b8e531d64530ac93ce5134194cf66a495b9;origin=https://github.com/brian-team/brian2;visit=swh:1:snp:06606ee7c757a47bc7dc168d0bfa8b0a5aecb620
+.. image:: https://archive.softwareheritage.org/badge/origin/https://github.com/brian-team/brian2/
+    :target: https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/brian-team/brian2
 
+.. image:: https://archive.softwareheritage.org/badge/swh:1:rel:e4d609023553bfbd62bf57960dd6f9d342a1d0e8/
+    :target: https://archive.softwareheritage.org/swh:1:rel:e4d609023553bfbd62bf57960dd6f9d342a1d0e8;origin=https://github.com/brian-team/brian2;visit=swh:1:snp:becb452d988ab8ea1386d27f3ad4c2221ec0ae7b
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg
         :target: CODE_OF_CONDUCT.md
         :alt: Contributor Covenant
 
 .. image:: https://img.shields.io/discourse/topics?server=https%3A%2F%2Fbrian.discourse.group
         :target: https://brian.discourse.group
```

### Comparing `Brian2-2.5.3/brian2/__init__.py` & `Brian2-2.5.4/brian2/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/_prefs.py` & `Brian2-2.5.4/brian2/codegen/_prefs.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/codeobject.py` & `Brian2-2.5.4/brian2/codegen/codeobject.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/cpp_prefs.py` & `Brian2-2.5.4/brian2/codegen/cpp_prefs.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/generators/GSL_generator.py` & `Brian2-2.5.4/brian2/codegen/generators/GSL_generator.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/generators/__init__.py` & `Brian2-2.5.4/brian2/codegen/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/generators/base.py` & `Brian2-2.5.4/brian2/codegen/generators/base.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/generators/cpp_generator.py` & `Brian2-2.5.4/brian2/codegen/generators/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/generators/cython_generator.py` & `Brian2-2.5.4/brian2/codegen/generators/cython_generator.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/generators/numpy_generator.py` & `Brian2-2.5.4/brian2/codegen/generators/numpy_generator.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/optimisation.py` & `Brian2-2.5.4/brian2/codegen/optimisation.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/permutation_analysis.py` & `Brian2-2.5.4/brian2/codegen/permutation_analysis.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/GSLcython_rt/GSLcython_rt.py` & `Brian2-2.5.4/brian2/codegen/runtime/GSLcython_rt/GSLcython_rt.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/GSLcython_rt/templates/stateupdate.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/GSLcython_rt/templates/stateupdate.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/__init__.py` & `Brian2-2.5.4/brian2/codegen/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/cython_rt.py` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/cython_rt.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/extension_manager.py` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/extension_manager.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/common_group.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/common_group.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_get_indices.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_get_indices.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_variable_get.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_variable_get.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_variable_get_conditional.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_variable_get_conditional.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/group_variable_set_conditional.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/group_variable_set_conditional.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/ratemonitor.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/ratemonitor.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/reset.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/reset.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/spatialstateupdate.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/spatialstateupdate.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/spikegenerator.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/spikegenerator.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/spikemonitor.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/spikemonitor.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/statemonitor.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/statemonitor.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/summed_variable.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/summed_variable.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/synapses.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/synapses.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/synapses_create_array.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/synapses_create_array.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/synapses_create_generator.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/synapses_create_generator.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/cython_rt/templates/threshold.pyx` & `Brian2-2.5.4/brian2/codegen/runtime/cython_rt/templates/threshold.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/numpy_rt.py` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/numpy_rt.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/common_group.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/common_group.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/group_variable_get.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/group_variable_get.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/group_variable_set_conditional.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/group_variable_set_conditional.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/ratemonitor.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/ratemonitor.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/reset.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/reset.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/spatialstateupdate.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/spatialstateupdate.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/spikegenerator.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/spikegenerator.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/spikemonitor.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/spikemonitor.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/statemonitor.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/statemonitor.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/summed_variable.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/summed_variable.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/synapses.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/synapses.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/synapses_create_array.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/synapses_create_array.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/synapses_create_generator.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/synapses_create_generator.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/runtime/numpy_rt/templates/threshold.py_` & `Brian2-2.5.4/brian2/codegen/runtime/numpy_rt/templates/threshold.py_`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/statements.py` & `Brian2-2.5.4/brian2/codegen/statements.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/templates.py` & `Brian2-2.5.4/brian2/codegen/templates.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/codegen/translation.py` & `Brian2-2.5.4/brian2/codegen/translation.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/conftest.py` & `Brian2-2.5.4/brian2/conftest.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/base.py` & `Brian2-2.5.4/brian2/core/base.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/clocks.py` & `Brian2-2.5.4/brian2/core/clocks.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/core_preferences.py` & `Brian2-2.5.4/brian2/core/core_preferences.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/functions.py` & `Brian2-2.5.4/brian2/core/functions.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/magic.py` & `Brian2-2.5.4/brian2/core/magic.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/names.py` & `Brian2-2.5.4/brian2/core/names.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/namespace.py` & `Brian2-2.5.4/brian2/core/namespace.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/network.py` & `Brian2-2.5.4/brian2/core/network.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/operations.py` & `Brian2-2.5.4/brian2/core/operations.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/preferences.py` & `Brian2-2.5.4/brian2/core/preferences.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/spikesource.py` & `Brian2-2.5.4/brian2/core/spikesource.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/tracking.py` & `Brian2-2.5.4/brian2/core/tracking.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/core/variables.py` & `Brian2-2.5.4/brian2/core/variables.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/GSLcodeobject.py` & `Brian2-2.5.4/brian2/devices/cpp_standalone/GSLcodeobject.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/brianlib/clocks.h` & `Brian2-2.5.4/brian2/devices/cpp_standalone/brianlib/clocks.h`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/brianlib/dynamic_array.h` & `Brian2-2.5.4/brian2/devices/cpp_standalone/brianlib/dynamic_array.h`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/codeobject.py` & `Brian2-2.5.4/brian2/devices/cpp_standalone/codeobject.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/device.py` & `Brian2-2.5.4/brian2/devices/cpp_standalone/device.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/common_group.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/common_group.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/group_variable_set.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/group_variable_set.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/group_variable_set_conditional.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/group_variable_set_conditional.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/main.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/main.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/makefile` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/makefile`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/network.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/network.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/objects.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/objects.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/ratemonitor.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/ratemonitor.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/reset.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/reset.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/run.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/run.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/spatialstateupdate.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/spatialstateupdate.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/spikegenerator.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/spikegenerator.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/spikemonitor.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/spikemonitor.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/statemonitor.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/statemonitor.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/stateupdate.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/stateupdate.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/summed_variable.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/summed_variable.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_classes.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_classes.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_create_array.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_create_array.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_create_generator.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_create_generator.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/synapses_push_spikes.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/synapses_push_spikes.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates/threshold.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates/threshold.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/cpp_standalone/templates_GSL/stateupdate.cpp` & `Brian2-2.5.4/brian2/devices/cpp_standalone/templates_GSL/stateupdate.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/devices/device.py` & `Brian2-2.5.4/brian2/devices/device.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/equations/codestrings.py` & `Brian2-2.5.4/brian2/equations/codestrings.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/equations/equations.py` & `Brian2-2.5.4/brian2/equations/equations.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/equations/refractory.py` & `Brian2-2.5.4/brian2/equations/refractory.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/equations/unitcheck.py` & `Brian2-2.5.4/brian2/equations/unitcheck.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/groups/group.py` & `Brian2-2.5.4/brian2/groups/group.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/groups/neurongroup.py` & `Brian2-2.5.4/brian2/groups/neurongroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/groups/subgroup.py` & `Brian2-2.5.4/brian2/groups/subgroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/hears.py` & `Brian2-2.5.4/brian2/hears.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/importexport/dictlike.py` & `Brian2-2.5.4/brian2/importexport/dictlike.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/importexport/importexport.py` & `Brian2-2.5.4/brian2/importexport/importexport.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/input/binomial.py` & `Brian2-2.5.4/brian2/input/binomial.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/input/poissongroup.py` & `Brian2-2.5.4/brian2/input/poissongroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/input/poissoninput.py` & `Brian2-2.5.4/brian2/input/poissoninput.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/input/spikegeneratorgroup.py` & `Brian2-2.5.4/brian2/input/spikegeneratorgroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/input/timedarray.py` & `Brian2-2.5.4/brian2/input/timedarray.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/memory/dynamicarray.py` & `Brian2-2.5.4/brian2/memory/dynamicarray.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/monitors/ratemonitor.py` & `Brian2-2.5.4/brian2/monitors/ratemonitor.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/monitors/spikemonitor.py` & `Brian2-2.5.4/brian2/monitors/spikemonitor.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/monitors/statemonitor.py` & `Brian2-2.5.4/brian2/monitors/statemonitor.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/numpy_.py` & `Brian2-2.5.4/brian2/numpy_.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/only.py` & `Brian2-2.5.4/brian2/only.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/parsing/bast.py` & `Brian2-2.5.4/brian2/parsing/bast.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/parsing/dependencies.py` & `Brian2-2.5.4/brian2/parsing/dependencies.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/parsing/expressions.py` & `Brian2-2.5.4/brian2/parsing/expressions.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/parsing/functions.py` & `Brian2-2.5.4/brian2/parsing/functions.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/parsing/rendering.py` & `Brian2-2.5.4/brian2/parsing/rendering.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/parsing/statements.py` & `Brian2-2.5.4/brian2/parsing/statements.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/parsing/sympytools.py` & `Brian2-2.5.4/brian2/parsing/sympytools.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/random/randomkit/randomkit.c` & `Brian2-2.5.4/brian2/random/randomkit/randomkit.c`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/random/randomkit/randomkit.h` & `Brian2-2.5.4/brian2/random/randomkit/randomkit.h`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/spatialneuron/morphology.py` & `Brian2-2.5.4/brian2/spatialneuron/morphology.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/spatialneuron/mp_ma_40984_gc2.CNG.swc` & `Brian2-2.5.4/brian2/spatialneuron/mp_ma_40984_gc2.CNG.swc`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/spatialneuron/spatialneuron.py` & `Brian2-2.5.4/brian2/spatialneuron/spatialneuron.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/sphinxext/briandoc.py` & `Brian2-2.5.4/brian2/sphinxext/briandoc.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/sphinxext/docscrape.py` & `Brian2-2.5.4/brian2/sphinxext/docscrape.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/sphinxext/docscrape_sphinx.py` & `Brian2-2.5.4/brian2/sphinxext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/sphinxext/examplefinder.py` & `Brian2-2.5.4/brian2/sphinxext/examplefinder.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/sphinxext/generate_examples.py` & `Brian2-2.5.4/brian2/sphinxext/generate_examples.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/sphinxext/generate_reference.py` & `Brian2-2.5.4/brian2/sphinxext/generate_reference.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/stateupdaters/GSL.py` & `Brian2-2.5.4/brian2/stateupdaters/GSL.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/stateupdaters/__init__.py` & `Brian2-2.5.4/brian2/stateupdaters/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/stateupdaters/base.py` & `Brian2-2.5.4/brian2/stateupdaters/base.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/stateupdaters/exact.py` & `Brian2-2.5.4/brian2/stateupdaters/exact.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/stateupdaters/explicit.py` & `Brian2-2.5.4/brian2/stateupdaters/explicit.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/stateupdaters/exponential_euler.py` & `Brian2-2.5.4/brian2/stateupdaters/exponential_euler.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/synapses/cspikequeue.cpp` & `Brian2-2.5.4/brian2/synapses/cspikequeue.cpp`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/synapses/cythonspikequeue.cpp` & `Brian2-2.5.4/brian2/synapses/cythonspikequeue.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "brian2/synapses/cspikequeue.cpp",
             "brian2/synapses/stdint_compat.h"
@@ -26,16 +26,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,15 +102,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -400,17 +400,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -480,14 +477,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1151,195 +1153,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1371,42 +1373,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_6brian2_8synapses_16cythonspikequeue_SpikeQueue;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2094,14 +2096,31 @@
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
@@ -2136,30 +2155,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
@@ -4878,15 +4897,15 @@
   __Pyx_AddTraceback("brian2.synapses.cythonspikequeue.SpikeQueue.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4895,29 +4914,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4928,15 +4947,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4945,29 +4964,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4978,15 +4997,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4995,29 +5014,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5028,15 +5047,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5045,29 +5064,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5078,15 +5097,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5095,29 +5114,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5128,212 +5147,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5349,15 +5368,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5365,53 +5384,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -5419,30 +5438,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5457,15 +5476,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5481,15 +5500,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5497,53 +5516,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -5551,30 +5570,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5589,15 +5608,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5613,15 +5632,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5629,53 +5648,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -5683,30 +5702,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5721,176 +5740,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -13769,15 +13788,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -19493,15 +19512,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6brian2_8synapses_16cythonspikequeue_SpikeQueue(PyObject *o) {
   struct __pyx_obj_6brian2_8synapses_16cythonspikequeue_SpikeQueue *p = (struct __pyx_obj_6brian2_8synapses_16cythonspikequeue_SpikeQueue *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -19647,15 +19666,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -19832,15 +19851,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -19963,15 +19982,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -20216,15 +20235,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -20581,26 +20600,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-z1zis4al/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-z0j_t_bj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -20882,14 +20901,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -21018,39 +21042,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -24345,18 +24369,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -24402,22 +24426,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `Brian2-2.5.3/brian2/synapses/cythonspikequeue.pyx` & `Brian2-2.5.4/brian2/synapses/cythonspikequeue.pyx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/synapses/parse_synaptic_generator_syntax.py` & `Brian2-2.5.4/brian2/synapses/parse_synaptic_generator_syntax.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/synapses/spikequeue.py` & `Brian2-2.5.4/brian2/synapses/spikequeue.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/synapses/synapses.py` & `Brian2-2.5.4/brian2/synapses/synapses.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/__init__.py` & `Brian2-2.5.4/brian2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/features/base.py` & `Brian2-2.5.4/brian2/tests/features/base.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/features/input.py` & `Brian2-2.5.4/brian2/tests/features/input.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/features/monitors.py` & `Brian2-2.5.4/brian2/tests/features/monitors.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/features/neurongroup.py` & `Brian2-2.5.4/brian2/tests/features/neurongroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/features/speed.py` & `Brian2-2.5.4/brian2/tests/features/speed.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/features/synapses.py` & `Brian2-2.5.4/brian2/tests/features/synapses.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/pytest.ini` & `Brian2-2.5.4/brian2/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/rallpack_data/ref_axon.0.neuron` & `Brian2-2.5.4/brian2/tests/rallpack_data/ref_axon.0.neuron`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/rallpack_data/ref_axon.x.neuron` & `Brian2-2.5.4/brian2/tests/rallpack_data/ref_axon.x.neuron`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/rallpack_data/ref_branch.0` & `Brian2-2.5.4/brian2/tests/rallpack_data/ref_branch.0`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/rallpack_data/ref_branch.x` & `Brian2-2.5.4/brian2/tests/rallpack_data/ref_branch.x`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/rallpack_data/ref_cable.0` & `Brian2-2.5.4/brian2/tests/rallpack_data/ref_cable.0`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/rallpack_data/ref_cable.x` & `Brian2-2.5.4/brian2/tests/rallpack_data/ref_cable.x`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_GSL.py` & `Brian2-2.5.4/brian2/tests/test_GSL.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_base.py` & `Brian2-2.5.4/brian2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_clocks.py` & `Brian2-2.5.4/brian2/tests/test_clocks.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_codegen.py` & `Brian2-2.5.4/brian2/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_codestrings.py` & `Brian2-2.5.4/brian2/tests/test_codestrings.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_complex_examples.py` & `Brian2-2.5.4/brian2/tests/test_complex_examples.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_cpp_standalone.py` & `Brian2-2.5.4/brian2/tests/test_cpp_standalone.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_devices.py` & `Brian2-2.5.4/brian2/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_equations.py` & `Brian2-2.5.4/brian2/tests/test_equations.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_functions.py` & `Brian2-2.5.4/brian2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_logger.py` & `Brian2-2.5.4/brian2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_memory.py` & `Brian2-2.5.4/brian2/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_monitor.py` & `Brian2-2.5.4/brian2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_morphology.py` & `Brian2-2.5.4/brian2/tests/test_morphology.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_namespaces.py` & `Brian2-2.5.4/brian2/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_network.py` & `Brian2-2.5.4/brian2/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_neurongroup.py` & `Brian2-2.5.4/brian2/tests/test_neurongroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_numpy_codegen.py` & `Brian2-2.5.4/brian2/tests/test_numpy_codegen.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_parsing.py` & `Brian2-2.5.4/brian2/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_poissongroup.py` & `Brian2-2.5.4/brian2/tests/test_poissongroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_poissoninput.py` & `Brian2-2.5.4/brian2/tests/test_poissoninput.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_preferences.py` & `Brian2-2.5.4/brian2/tests/test_preferences.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_refractory.py` & `Brian2-2.5.4/brian2/tests/test_refractory.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_spatialneuron.py` & `Brian2-2.5.4/brian2/tests/test_spatialneuron.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_spikegenerator.py` & `Brian2-2.5.4/brian2/tests/test_spikegenerator.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_spikequeue.py` & `Brian2-2.5.4/brian2/tests/test_spikequeue.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_stateupdaters.py` & `Brian2-2.5.4/brian2/tests/test_stateupdaters.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_subgroup.py` & `Brian2-2.5.4/brian2/tests/test_subgroup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_synapses.py` & `Brian2-2.5.4/brian2/tests/test_synapses.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_templates/test_templates.py` & `Brian2-2.5.4/brian2/tests/test_templates/test_templates.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_thresholder.py` & `Brian2-2.5.4/brian2/tests/test_thresholder.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_timedarray.py` & `Brian2-2.5.4/brian2/tests/test_timedarray.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_units.py` & `Brian2-2.5.4/brian2/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_utils.py` & `Brian2-2.5.4/brian2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/test_variables.py` & `Brian2-2.5.4/brian2/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/tests/utils.py` & `Brian2-2.5.4/brian2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/units/__init__.py` & `Brian2-2.5.4/brian2/units/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/units/allunits.py` & `Brian2-2.5.4/brian2/units/allunits.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/units/constants.py` & `Brian2-2.5.4/brian2/units/constants.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/units/fundamentalunits.py` & `Brian2-2.5.4/brian2/units/fundamentalunits.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/units/stdunits.py` & `Brian2-2.5.4/brian2/units/stdunits.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/units/unitsafefunctions.py` & `Brian2-2.5.4/brian2/units/unitsafefunctions.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/utils/arrays.py` & `Brian2-2.5.4/brian2/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/utils/caching.py` & `Brian2-2.5.4/brian2/utils/caching.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/utils/filelock.py` & `Brian2-2.5.4/brian2/utils/filelock.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/utils/filetools.py` & `Brian2-2.5.4/brian2/utils/filetools.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/utils/logger.py` & `Brian2-2.5.4/brian2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/brian2/utils/stringtools.py` & `Brian2-2.5.4/brian2/utils/stringtools.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/_static/brian-logo.png` & `Brian2-2.5.4/docs_sphinx/_static/brian-logo.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/custom_events.pdf` & `Brian2-2.5.4/docs_sphinx/advanced/custom_events.pdf`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/custom_events.rst` & `Brian2-2.5.4/docs_sphinx/advanced/custom_events.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/custom_events.svg` & `Brian2-2.5.4/docs_sphinx/advanced/custom_events.svg`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/functions.rst` & `Brian2-2.5.4/docs_sphinx/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/how_brian_works.rst` & `Brian2-2.5.4/docs_sphinx/advanced/how_brian_works.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/interface.rst` & `Brian2-2.5.4/docs_sphinx/advanced/interface.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/logging.rst` & `Brian2-2.5.4/docs_sphinx/advanced/logging.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/namespaces.rst` & `Brian2-2.5.4/docs_sphinx/advanced/namespaces.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/preferences.rst` & `Brian2-2.5.4/docs_sphinx/advanced/preferences.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/random.rst` & `Brian2-2.5.4/docs_sphinx/advanced/random.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/scheduling.rst` & `Brian2-2.5.4/docs_sphinx/advanced/scheduling.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/advanced/state_update.rst` & `Brian2-2.5.4/docs_sphinx/advanced/state_update.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/conf.py` & `Brian2-2.5.4/docs_sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/conftest.py` & `Brian2-2.5.4/docs_sphinx/conftest.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/GSL.rst` & `Brian2-2.5.4/docs_sphinx/developer/GSL.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/codegen.rst` & `Brian2-2.5.4/docs_sphinx/developer/codegen.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/codegen_code_paths.png` & `Brian2-2.5.4/docs_sphinx/developer/codegen_code_paths.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/codegen_code_paths.pptx` & `Brian2-2.5.4/docs_sphinx/developer/codegen_code_paths.pptx`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/devices.rst` & `Brian2-2.5.4/docs_sphinx/developer/devices.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/equations_namespaces.rst` & `Brian2-2.5.4/docs_sphinx/developer/equations_namespaces.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/functions.rst` & `Brian2-2.5.4/docs_sphinx/developer/functions.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/defensive_programming.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/defensive_programming.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/documentation.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/documentation.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/index.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/index.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/logging.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/logging.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/representation.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/representation.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/style.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/style.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/testing.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/testing.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/guidelines/workflow.rst` & `Brian2-2.5.4/docs_sphinx/developer/guidelines/workflow.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/index.rst` & `Brian2-2.5.4/docs_sphinx/developer/index.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/oldcodegen.rst` & `Brian2-2.5.4/docs_sphinx/developer/oldcodegen.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/openmp.rst` & `Brian2-2.5.4/docs_sphinx/developer/openmp.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/preferences.rst` & `Brian2-2.5.4/docs_sphinx/developer/preferences.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/standalone.rst` & `Brian2-2.5.4/docs_sphinx/developer/standalone.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/units.rst` & `Brian2-2.5.4/docs_sphinx/developer/units.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/developer/variables_indices.rst` & `Brian2-2.5.4/docs_sphinx/developer/variables_indices.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/index.rst` & `Brian2-2.5.4/docs_sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/brian1hears_bridge.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/brian1hears_bridge.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/container.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/container.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/inputs.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/inputs.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/library.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/library.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/monitors.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/monitors.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/multicompartmental.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/multicompartmental.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/networks_and_clocks.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/networks_and_clocks.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/neurongroup.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/neurongroup.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/preferences.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/preferences.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/brian1_to_2/synapses.rst` & `Brian2-2.5.4/docs_sphinx/introduction/brian1_to_2/synapses.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/changes.rst` & `Brian2-2.5.4/docs_sphinx/introduction/changes.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/code_of_conduct.rst` & `Brian2-2.5.4/docs_sphinx/introduction/code_of_conduct.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/compatibility.rst` & `Brian2-2.5.4/docs_sphinx/introduction/compatibility.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/install.rst` & `Brian2-2.5.4/docs_sphinx/introduction/install.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/known_issues.rst` & `Brian2-2.5.4/docs_sphinx/introduction/known_issues.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/release_notes.rst` & `Brian2-2.5.4/docs_sphinx/introduction/release_notes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 Release notes
 =============
 
+Brian 2.5.4
+-----------
+Yet another minor release that fixes an issue with the documentation build. As a bonus, we now provide wheels built
+with the `musl <https://musl.libc.org/>`_ standard library, which allows installing Brian on distributions such as
+`Alpine Linux <https://alpinelinux.org/>`_.
+
+Selected bug fixes
+~~~~~~~~~~~~~~~~~~
+- Re-introduce the tutorials and example plots that were omitted from the documentation by accident. Thanks to Felix Kern for making us aware of the issue.
+
+Infrastructure improvements
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+- Provide ``musllinux`` (see `PEP 656 <https://peps.python.org/pep-0656/>`_) wheels for distributions such as Alpine Linux (:issue:`1478`).
+
+Contributions
+~~~~~~~~~~~~~
+
+Github code, documentation, and issue contributions (ordered by the number of
+contributions):
+
+* Marcel Stimberg (`@mstimberg <https://github.com/mstimberg>`_)
+* Felix Benjamin Kern (`@kernfel <https://github.com/kernfel>`_)
+
 Brian 2.5.3
 -----------
 This new minor release only fixes two infrastructure issues that came up with the previous release.
 
 Selected bug fixes
 ~~~~~~~~~~~~~~~~~~
 - Re-introduce the reference documentation that was no longer created on https://brian2.readthedocs.org with the latest release (:issue:`1474`). Thanks to Michalis Pagkalos for making us aware of the issue.
```

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/scripts.rst` & `Brian2-2.5.4/docs_sphinx/introduction/scripts.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/introduction/support.rst` & `Brian2-2.5.4/docs_sphinx/introduction/support.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/computation.rst` & `Brian2-2.5.4/docs_sphinx/user/computation.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/converting_from_integrated_form.rst` & `Brian2-2.5.4/docs_sphinx/user/converting_from_integrated_form.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/equations.rst` & `Brian2-2.5.4/docs_sphinx/user/equations.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/cylinder.pdf` & `Brian2-2.5.4/docs_sphinx/user/images/cylinder.pdf`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/cylinder.svg` & `Brian2-2.5.4/docs_sphinx/user/images/cylinder.svg`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/function_plot.png` & `Brian2-2.5.4/docs_sphinx/user/images/function_plot.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/morphology_deterministic_coords.png` & `Brian2-2.5.4/docs_sphinx/user/images/morphology_deterministic_coords.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_1.png` & `Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_1.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_2.png` & `Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_2.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_3.png` & `Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_3.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_compartment_1.png` & `Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_compartment_1.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_compartment_2.png` & `Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_compartment_2.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/morphology_random_section_compartment_3.png` & `Brian2-2.5.4/docs_sphinx/user/images/morphology_random_section_compartment_3.png`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/section.pdf` & `Brian2-2.5.4/docs_sphinx/user/images/section.pdf`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/section.svg` & `Brian2-2.5.4/docs_sphinx/user/images/section.svg`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/soma.pdf` & `Brian2-2.5.4/docs_sphinx/user/images/soma.pdf`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/images/soma.svg` & `Brian2-2.5.4/docs_sphinx/user/images/soma.svg`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/import.rst` & `Brian2-2.5.4/docs_sphinx/user/import.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/input.rst` & `Brian2-2.5.4/docs_sphinx/user/input.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/models.rst` & `Brian2-2.5.4/docs_sphinx/user/models.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/multicompartmental.rst` & `Brian2-2.5.4/docs_sphinx/user/multicompartmental.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/numerical_integration.rst` & `Brian2-2.5.4/docs_sphinx/user/numerical_integration.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/plotting_functions.rst` & `Brian2-2.5.4/docs_sphinx/user/plotting_functions.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/recording.rst` & `Brian2-2.5.4/docs_sphinx/user/recording.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/refractoriness.rst` & `Brian2-2.5.4/docs_sphinx/user/refractoriness.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/running.rst` & `Brian2-2.5.4/docs_sphinx/user/running.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/synapses.rst` & `Brian2-2.5.4/docs_sphinx/user/synapses.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/docs_sphinx/user/units.rst` & `Brian2-2.5.4/docs_sphinx/user/units.rst`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/COBAHH.py` & `Brian2-2.5.4/examples/COBAHH.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/CUBA.py` & `Brian2-2.5.4/examples/CUBA.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/IF_curve_Hodgkin_Huxley.py` & `Brian2-2.5.4/examples/IF_curve_Hodgkin_Huxley.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/IF_curve_LIF.py` & `Brian2-2.5.4/examples/IF_curve_LIF.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/adaptive_threshold.py` & `Brian2-2.5.4/examples/adaptive_threshold.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/COBAHH_approximated.py` & `Brian2-2.5.4/examples/advanced/COBAHH_approximated.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/Ornstein_Uhlenbeck.py` & `Brian2-2.5.4/examples/advanced/Ornstein_Uhlenbeck.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/compare_GSL_to_conventional.py` & `Brian2-2.5.4/examples/advanced/compare_GSL_to_conventional.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/custom_events.py` & `Brian2-2.5.4/examples/advanced/custom_events.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/exprel_function.py` & `Brian2-2.5.4/examples/advanced/exprel_function.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/float_32_64_benchmark.py` & `Brian2-2.5.4/examples/advanced/float_32_64_benchmark.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/modelfitting_sbi.py` & `Brian2-2.5.4/examples/advanced/modelfitting_sbi.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/opencv_movie.py` & `Brian2-2.5.4/examples/advanced/opencv_movie.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/advanced/stochastic_odes.py` & `Brian2-2.5.4/examples/advanced/stochastic_odes.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/bipolar_cell.py` & `Brian2-2.5.4/examples/compartmental/bipolar_cell.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/bipolar_with_inputs.py` & `Brian2-2.5.4/examples/compartmental/bipolar_with_inputs.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/bipolar_with_inputs2.py` & `Brian2-2.5.4/examples/compartmental/bipolar_with_inputs2.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/cylinder.py` & `Brian2-2.5.4/examples/compartmental/cylinder.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/hh_with_spikes.py` & `Brian2-2.5.4/examples/compartmental/hh_with_spikes.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/hodgkin_huxley_1952.py` & `Brian2-2.5.4/examples/compartmental/hodgkin_huxley_1952.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/infinite_cable.py` & `Brian2-2.5.4/examples/compartmental/infinite_cable.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/lfp.py` & `Brian2-2.5.4/examples/compartmental/lfp.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/morphotest.py` & `Brian2-2.5.4/examples/compartmental/morphotest.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/rall.py` & `Brian2-2.5.4/examples/compartmental/rall.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/compartmental/spike_initiation.py` & `Brian2-2.5.4/examples/compartmental/spike_initiation.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/coupled_oscillators.py` & `Brian2-2.5.4/examples/coupled_oscillators.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_2004.py` & `Brian2-2.5.4/examples/frompapers/Brette_2004.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_2012/Fig1.py` & `Brian2-2.5.4/examples/frompapers/Brette_2012/Fig1.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_2012/Fig3AB.py` & `Brian2-2.5.4/examples/frompapers/Brette_2012/Fig3AB.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_2012/Fig3CF.py` & `Brian2-2.5.4/examples/frompapers/Brette_2012/Fig3CF.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_2012/Fig4.py` & `Brian2-2.5.4/examples/frompapers/Brette_2012/Fig4.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_2012/Fig5A.py` & `Brian2-2.5.4/examples/frompapers/Brette_2012/Fig5A.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_Gerstner_2005.py` & `Brian2-2.5.4/examples/frompapers/Brette_Gerstner_2005.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brette_Guigon_2003.py` & `Brian2-2.5.4/examples/frompapers/Brette_Guigon_2003.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brunel_2000.py` & `Brian2-2.5.4/examples/frompapers/Brunel_2000.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brunel_Hakim_1999.py` & `Brian2-2.5.4/examples/frompapers/Brunel_Hakim_1999.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Brunel_Wang_2001.py` & `Brian2-2.5.4/examples/frompapers/Brunel_Wang_2001.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Clopath_et_al_2010_homeostasis.py` & `Brian2-2.5.4/examples/frompapers/Clopath_et_al_2010_homeostasis.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Clopath_et_al_2010_no_homeostasis.py` & `Brian2-2.5.4/examples/frompapers/Clopath_et_al_2010_no_homeostasis.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Destexhe_et_al_1998.py` & `Brian2-2.5.4/examples/frompapers/Destexhe_et_al_1998.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Diesmann_et_al_1999.py` & `Brian2-2.5.4/examples/frompapers/Diesmann_et_al_1999.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Graupner_Brunel_2012.py` & `Brian2-2.5.4/examples/frompapers/Graupner_Brunel_2012.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Hindmarsh_Rose_1984.py` & `Brian2-2.5.4/examples/frompapers/Hindmarsh_Rose_1984.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Izhikevich_2003.py` & `Brian2-2.5.4/examples/frompapers/Izhikevich_2003.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Izhikevich_2007.py` & `Brian2-2.5.4/examples/frompapers/Izhikevich_2007.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Jansen_Rit_1995_single_column.py` & `Brian2-2.5.4/examples/frompapers/Jansen_Rit_1995_single_column.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Kremer_et_al_2011_barrel_cortex.py` & `Brian2-2.5.4/examples/frompapers/Kremer_et_al_2011_barrel_cortex.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Maass_Natschlaeger_Markram_2002.py` & `Brian2-2.5.4/examples/frompapers/Maass_Natschlaeger_Markram_2002.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Morris_Lecar_1981.py` & `Brian2-2.5.4/examples/frompapers/Morris_Lecar_1981.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Naud_et_al_2008_adex_firing_patterns.py` & `Brian2-2.5.4/examples/frompapers/Naud_et_al_2008_adex_firing_patterns.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Nicola_Clopath_2017.py` & `Brian2-2.5.4/examples/frompapers/Nicola_Clopath_2017.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Platkiewicz_Brette_2011.py` & `Brian2-2.5.4/examples/frompapers/Platkiewicz_Brette_2011.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Rossant_et_al_2011bis.py` & `Brian2-2.5.4/examples/frompapers/Rossant_et_al_2011bis.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Rothman_Manis_2003.py` & `Brian2-2.5.4/examples/frompapers/Rothman_Manis_2003.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/README.md` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/README.md`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_1_COBA.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_1_COBA.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_2_gchi_astrocyte.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_2_gchi_astrocyte.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_3_io_synapse.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_3_io_synapse.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_4_rsmean.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_4_rsmean.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_4_synrel.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_4_synrel.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_5_astro_ring.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_5_astro_ring.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/example_6_COBA_with_astro.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/example_6_COBA_with_astro.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Stimberg_et_al_2018/plot_utils.py` & `Brian2-2.5.4/examples/frompapers/Stimberg_et_al_2018/plot_utils.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Sturzl_et_al_2000.py` & `Brian2-2.5.4/examples/frompapers/Sturzl_et_al_2000.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Tetzlaff_2015.py` & `Brian2-2.5.4/examples/frompapers/Tetzlaff_2015.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Touboul_Brette_2008.py` & `Brian2-2.5.4/examples/frompapers/Touboul_Brette_2008.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Tsodyks_Pawelzik_Markram_1998.py` & `Brian2-2.5.4/examples/frompapers/Tsodyks_Pawelzik_Markram_1998.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Tsodyks_Uziel_Markram_2000.py` & `Brian2-2.5.4/examples/frompapers/Tsodyks_Uziel_Markram_2000.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Vogels_et_al_2011.py` & `Brian2-2.5.4/examples/frompapers/Vogels_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/frompapers/Wang_Buszaki_1996.py` & `Brian2-2.5.4/examples/frompapers/Wang_Buszaki_1996.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/multiprocessing/01_using_cython.py` & `Brian2-2.5.4/examples/multiprocessing/01_using_cython.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/multiprocessing/02_using_standalone.py` & `Brian2-2.5.4/examples/multiprocessing/02_using_standalone.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/multiprocessing/03_standalone_joblib.py` & `Brian2-2.5.4/examples/multiprocessing/03_standalone_joblib.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/non_reliability.py` & `Brian2-2.5.4/examples/non_reliability.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/phase_locking.py` & `Brian2-2.5.4/examples/phase_locking.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/reliability.py` & `Brian2-2.5.4/examples/reliability.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/standalone/STDP_standalone.py` & `Brian2-2.5.4/examples/standalone/STDP_standalone.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/standalone/cuba_openmp.py` & `Brian2-2.5.4/examples/standalone/cuba_openmp.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/standalone/standalone_multiplerun.py` & `Brian2-2.5.4/examples/standalone/standalone_multiplerun.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/STDP.py` & `Brian2-2.5.4/examples/synapses/STDP.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/continuous_interaction.py` & `Brian2-2.5.4/examples/synapses/continuous_interaction.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/efficient_gaussian_connectivity.py` & `Brian2-2.5.4/examples/synapses/efficient_gaussian_connectivity.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/gapjunctions.py` & `Brian2-2.5.4/examples/synapses/gapjunctions.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/jeffress.py` & `Brian2-2.5.4/examples/synapses/jeffress.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/licklider.py` & `Brian2-2.5.4/examples/synapses/licklider.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/nonlinear.py` & `Brian2-2.5.4/examples/synapses/nonlinear.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/spatial_connections.py` & `Brian2-2.5.4/examples/synapses/spatial_connections.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/spike_based_homeostasis.py` & `Brian2-2.5.4/examples/synapses/spike_based_homeostasis.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/state_variables.py` & `Brian2-2.5.4/examples/synapses/state_variables.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/examples/synapses/synapses.py` & `Brian2-2.5.4/examples/synapses/synapses.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/pyproject.toml` & `Brian2-2.5.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "Brian2"
 authors = [
-    {name = 'Marcel Stimberg', email="marcel.stimberg@inserm.fr"},
+    {name = 'Marcel Stimberg'},
     {name = 'Dan Goodman'},
     {name ='Romain Brette'}
 ]
 requires-python = '>=3.9'
 dependencies = [
     'numpy>=1.21',
     'cython>=0.29',
```

### Comparing `Brian2-2.5.3/setup.py` & `Brian2-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `Brian2-2.5.3/versions.md` & `Brian2-2.5.4/versions.md`

 * *Files identical despite different names*

