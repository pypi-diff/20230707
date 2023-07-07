# Comparing `tmp/datumaro-1.3.2.tar.gz` & `tmp/datumaro-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.3.2.tar", last modified: Fri Jun 16 08:40:52 2023, max compression
+gzip compressed data, was "datumaro-1.4.0rc1.tar", last modified: Fri Jul  7 13:23:30 2023, max compression
```

## Comparing `datumaro-1.3.2.tar` & `datumaro-1.4.0rc1.tar`

### file list

```diff
@@ -1,330 +1,361 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.431728 datumaro-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)   375078 2023-06-16 08:40:38.000000 datumaro-1.3.2/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 08:40:38.000000 datumaro-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 08:40:38.000000 datumaro-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-16 08:40:38.000000 datumaro-1.3.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-16 08:40:52.431728 datumaro-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-16 08:40:38.000000 datumaro-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.399728 datumaro-1.3.2/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/abstracts/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    48306 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.403728 datumaro-1.3.2/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89679 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.407728 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.411728 datumaro-1.3.2/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28664 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20633 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.415728 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17893 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.419728 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38725 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/synthia/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.423728 datumaro-1.3.2/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.427728 datumaro-1.3.2/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.431728 datumaro-1.3.2/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 08:40:38.000000 datumaro-1.3.2/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:40:52.395728 datumaro-1.3.2/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 08:40:52.000000 datumaro-1.3.2/datumaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-16 08:40:39.000000 datumaro-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-16 08:40:39.000000 datumaro-1.3.2/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 08:40:39.000000 datumaro-1.3.2/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:40:52.431728 datumaro-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-16 08:40:39.000000 datumaro-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.620827 datumaro-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)   375078 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-07 13:23:30.620827 datumaro-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-07 13:23:18.000000 datumaro-1.4.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:23:30.620827 datumaro-1.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.544827 datumaro-1.4.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.560827 datumaro-1.4.0rc1/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.560827 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.564827 datumaro-1.4.0rc1/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.572827 datumaro-1.4.0rc1/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.572827 datumaro-1.4.0rc1/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.572827 datumaro-1.4.0rc1/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29044 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.576827 datumaro-1.4.0rc1/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.580827 datumaro-1.4.0rc1/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.580827 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.580827 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.588827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.592827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28677 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.592827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.592827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.596827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.600827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.604827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31336 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.608827 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46895 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.612827 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.616827 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.616827 datumaro-1.4.0rc1/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 13:23:19.000000 datumaro-1.4.0rc1/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:23:30.556827 datumaro-1.4.0rc1/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 13:23:30.000000 datumaro-1.4.0rc1/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.3.2/3rd-party.txt` & `datumaro-1.4.0rc1/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/LICENSE` & `datumaro-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/PKG-INFO` & `datumaro-1.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.3.2
+Version: 1.4.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tf
 Provides-Extra: tfds
 Provides-Extra: tf-gpu
 Provides-Extra: default
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `datumaro-1.3.2/README.md` & `datumaro-1.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,33 +28,33 @@
     PointsCategories,
     Polygon,
     PolyLine,
     RgbColor,
     RleMask,
 )
 from .components.cli_plugin import CliPlugin
-from .components.dataset import Dataset, DatasetPatch, DatasetSubset, ItemStatus, eager_mode
+from .components.dataset import Dataset, eager_mode
 from .components.dataset_base import (
     DEFAULT_SUBSET_NAME,
     CategoriesInfo,
     DatasetBase,
     DatasetItem,
     IDataset,
     SubsetBase,
 )
 from .components.environment import Environment, PluginRegistry
 from .components.exporter import Exporter, ExportErrorPolicy, FailingExportErrorPolicy
 from .components.hl_ops import HLOps
 from .components.importer import FailingImportErrorPolicy, Importer, ImportErrorPolicy
-from .components.launcher import Launcher, ModelTransform
+from .components.launcher import Launcher
 from .components.media import ByteImage, Image, MediaElement, Video, VideoFrame
 from .components.media_manager import MediaManager
 from .components.progress_reporting import (
     NullProgressReporter,
     ProgressReporter,
     SimpleProgressReporter,
     TQDMProgressReporter,
 )
-from .components.transformer import ItemTransform, Transform
+from .components.transformer import ItemTransform, ModelTransform, Transform
 from .components.validator import Validator
 from .components.visualizer import Visualizer
 from .version import __version__
```

### Comparing `datumaro-1.3.2/datumaro/capi/pybind.cpp` & `datumaro-1.4.0rc1/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/__main__.py` & `datumaro-1.4.0rc1/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # pylint: disable=redefined-builtin
 
 from . import (
+    compare,
     convert,
     detect_format,
-    diff,
     download,
     explain,
     explore,
     filter,
     generate,
     info,
     merge,
     patch,
+    prune,
     stats,
     transform,
     validate,
 )
 from .require_project import get_project_commands
 
 __all__ = [
@@ -28,20 +29,21 @@
 ]
 
 
 def get_non_project_commands():
     return [
         ("convert", convert, "Convert dataset between formats"),
         ("detect", detect_format, "Detect the format of a dataset"),
-        ("diff", diff, "Compare datasets"),
+        ("compare", compare, "Compare datasets"),
         ("dinfo", info, "Print dataset info"),
         ("download", download, "Download a publicly available dataset"),
         ("explain", explain, "Run Explainable AI algorithm for model"),
+        ("explore", explore, "Explore similar datasetitems of query"),
         ("filter", filter, "Filter dataset items"),
         ("generate", generate, "Generate synthetic dataset"),
         ("merge", merge, "Merge datasets"),
         ("patch", patch, "Update dataset from another one"),
-        ("explore", explore, "Explore similar datasetitems of query"),
+        ("prune", prune, "Prune dataset"),
         ("stats", stats, "Compute dataset statistics"),
         ("transform", transform, "Modify dataset items"),
         ("validate", validate, "Validate dataset"),
     ]
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/convert.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
 from datumaro.components.dataset import Dataset
-from datumaro.components.project import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.util.os_util import make_file_name
 
 from ..util import MultilineFormatter
 from ..util.errors import CliException
 from ..util.project import FilterModes, generate_next_file_name
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    builtin_readers = sorted(set(Environment().importers) | set(Environment().extractors))
-    builtin_writers = sorted(Environment().exporters)
+    builtin_readers = sorted(
+        set(DEFAULT_ENVIRONMENT.importers) | set(DEFAULT_ENVIRONMENT.extractors)
+    )
+    builtin_writers = sorted(DEFAULT_ENVIRONMENT.exporters)
 
     parser = parser_ctor(
         help="Convert an existing dataset to another format",
         description="""
         Converts a dataset from one format to another.
         You can add your own formats and do many more by creating a
         Datumaro project.|n
@@ -77,14 +79,18 @@
         "--filter-mode",
         default=FilterModes.i.name,
         type=FilterModes.parse,
         help="Filter mode, one of %s (default: %s)"
         % (", ".join(FilterModes.list_options()), "%(default)s"),
     )
     parser.add_argument(
+        "--encryption-key",
+        help="Secret key. It is required only if the input dataset is encrypted.",
+    )
+    parser.add_argument(
         "extra_args",
         nargs=argparse.REMAINDER,
         help="Additional arguments for output format (pass '-- -h' for help). "
         "Must be specified after the main command arguments",
     )
     parser.set_defaults(command=convert_command)
 
@@ -94,15 +100,15 @@
 def get_sensitive_args():
     return {
         convert_command: ["source", "dst_dir", "extra_args"],
     }
 
 
 def convert_command(args):
-    env = Environment()
+    env = DEFAULT_ENVIRONMENT
 
     try:
         exporter = env.exporters[args.output_format]
     except KeyError:
         raise CliException("Exporter for format '%s' is not found" % args.output_format)
     extra_args = exporter.parse_cmdline(args.extra_args)
 
@@ -142,15 +148,18 @@
             )
     else:
         dst_dir = generate_next_file_name(
             "%s-%s" % (osp.basename(source), make_file_name(args.output_format))
         )
     dst_dir = osp.abspath(dst_dir)
 
-    dataset = Dataset.import_from(source, fmt)
+    import_kwargs = {}
+    if args.encryption_key:
+        import_kwargs["encryption_key"] = args.encryption_key
+    dataset = Dataset.import_from(source, fmt, **import_kwargs)
 
     log.info("Exporting the dataset")
     if args.filter:
         dataset = dataset.filter(args.filter, **filter_args)
     dataset.export(format=args.output_format, save_dir=dst_dir, **extra_args)
 
     log.info("Dataset exported to '%s' as '%s'" % (dst_dir, args.output_format))
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/detect_format.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/detect_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 
 from datumaro.cli.util import MultilineFormatter
 from datumaro.cli.util.project import load_project
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.format_detection import RejectionReason
 from datumaro.util import dump_json_file
 from datumaro.util.scope import scope_add, scoped
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
@@ -73,15 +73,15 @@
     except ProjectNotFoundError:
         if args.project_dir:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     report = {"rejected_formats": {}}
 
     def rejection_callback(
         format_name: str,
         reason: RejectionReason,
         human_message: str,
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/diff.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/compare.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright (C) 2019-2022 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 from enum import Enum, auto
 
+from datumaro.components.comparator import DistanceComparator, EqualityComparator, TableComparator
 from datumaro.components.errors import ProjectNotFoundError
-from datumaro.components.operations import DistanceComparator, ExactComparator
-from datumaro.util import dump_json_file
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scope_add, scoped
 
 from ..util import MultilineFormatter
-from ..util.diff import DiffVisualizer
+from ..util.compare import DistanceCompareVisualizer
 from ..util.errors import CliException
 from ..util.project import generate_next_file_name, load_project, parse_full_revpath
 
 
 class ComparisonMethod(Enum):
+    table = auto()
     equality = auto()
     distance = auto()
 
 
 eq_default_if = ["id", "group"]  # avoid https://bugs.python.org/issue16399
 
 
@@ -49,45 +49,46 @@
         |s|s- <rev> [ :<target> ]|n
         |s|s- <target>|n
         |n
         Both forms use the -p/--project as a context for plugins. It can be
         useful for dataset paths in targets. When not specified, the current
         project's working tree is used.|n
         |n
-        Annotations can be matched 2 ways:|n
+        Annotations can be matched 3 ways:|n
+        - by comparision table|n
         - by equality checking|n
         - by distance computation|n
         |n
         Examples:|n
         - Compare two projects by distance, match boxes if IoU > 0.7,|n
         |s|s|s|ssave results to Tensorboard:|n
         |s|s%(prog)s other/project -o diff/ -f tensorboard --iou-thresh 0.7|n
         |n
         - Compare two projects for equality, exclude annotation groups |n
         |s|s|s|sand the 'is_crowd' attribute from comparison:|n
-        |s|s%(prog)s other/project/ -if group -ia is_crowd|n
+        |s|s%(prog)s other/project/ -if group -ia is_crowd -m equality|n
         |n
         - Compare two datasets, specify formats:|n
         |s|s%(prog)s path/to/dataset1:voc path/to/dataset2:coco|n
         |n
         - Compare the current working tree and a dataset:|n
         |s|s%(prog)s path/to/dataset2:coco|n
         |n
         - Compare a source from a previous revision and a dataset:|n
         |s|s%(prog)s HEAD~2:source-2 path/to/dataset2:yolo
         """,
         formatter_class=MultilineFormatter,
     )
 
-    formats = ", ".join(f.name for f in DiffVisualizer.OutputFormat)
+    formats = ", ".join(f.name for f in DistanceCompareVisualizer.OutputFormat)
     comp_methods = ", ".join(m.name for m in ComparisonMethod)
 
     def _parse_output_format(s):
         try:
-            return DiffVisualizer.OutputFormat[s.lower()]
+            return DistanceCompareVisualizer.OutputFormat[s.lower()]
         except KeyError:
             raise argparse.ArgumentError(
                 "format",
                 message="Unknown output " "format '%s', the only available are: %s" % (s, formats),
             )
 
     def _parse_comparison_method(s):
@@ -111,40 +112,40 @@
         default=None,
         help="Directory to save comparison results " "(default: generate automatically)",
     )
     parser.add_argument(
         "-m",
         "--method",
         type=_parse_comparison_method,
-        default=ComparisonMethod.equality.name,
+        default=ComparisonMethod.table.name,
         help="Comparison method, one of {} (default: %(default)s)".format(comp_methods),
     )
     parser.add_argument(
         "--overwrite", action="store_true", help="Overwrite existing files in the save directory"
     )
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
         help="Directory of the current project (default: current dir)",
     )
-    parser.set_defaults(command=diff_command)
+    parser.set_defaults(command=compare_command)
 
     distance_parser = parser.add_argument_group("Distance comparison options")
     distance_parser.add_argument(
         "--iou-thresh",
         default=0.5,
         type=float,
         help="IoU match threshold for shapes (default: %(default)s)",
     )
     parser.add_argument(
         "-f",
         "--format",
         type=_parse_output_format,
-        default=DiffVisualizer.DEFAULT_FORMAT.name,
+        default=DistanceCompareVisualizer.DEFAULT_FORMAT.name,
         help="Output format, one of {} (default: %(default)s)".format(formats),
     )
 
     equality_parser = parser.add_argument_group("Equality comparison options")
     equality_parser.add_argument(
         "-iia", "--ignore-item-attr", action="append", help="Ignore item attribute (repeatable)"
     )
@@ -165,33 +166,33 @@
     equality_parser.add_argument("--all", action="store_true", help="Include matches in the output")
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        diff_command: [
+        compare_command: [
             "first_target",
             "second_target",
             "dst_dir",
             "project_dir",
         ],
     }
 
 
 @scoped
-def diff_command(args):
+def compare_command(args):
     dst_dir = args.dst_dir
     if dst_dir:
         if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
             raise CliException(
                 "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
             )
     else:
-        dst_dir = generate_next_file_name("diff")
+        dst_dir = generate_next_file_name("compare")
     dst_dir = osp.abspath(dst_dir)
 
     if not osp.exists(dst_dir):
         on_error_do(rmtree, dst_dir, ignore_errors=True)
         os.makedirs(dst_dir)
 
     project = None
@@ -214,51 +215,44 @@
 
             second_dataset, target_project = parse_full_revpath(args.second_target, project)
             if target_project:
                 scope_add(target_project)
     except Exception as e:
         raise CliException(str(e))
 
-    if args.method is ComparisonMethod.equality:
+    if args.method is ComparisonMethod.table:
+        comparator = TableComparator()
+        (
+            high_level_table,
+            mid_level_table,
+            low_level_table,
+            comparison_dict,
+        ) = comparator.compare_datasets(first_dataset, second_dataset)
+        if args.dst_dir:
+            comparator.save_compare_report(
+                high_level_table, mid_level_table, low_level_table, comparison_dict, args.dst_dir
+            )
+
+    elif args.method is ComparisonMethod.equality:
         if args.ignore_field:
             args.ignore_field = eq_default_if
-        comparator = ExactComparator(
+
+        comparator = EqualityComparator(
             match_images=args.match_images,
             ignored_fields=args.ignore_field,
             ignored_attrs=args.ignore_attr,
             ignored_item_attrs=args.ignore_item_attr,
+            all=args.all,
         )
-        matches, mismatches, a_extra, b_extra, errors = comparator.compare_datasets(
-            first_dataset, second_dataset
-        )
+        output = comparator.compare_datasets(first_dataset, second_dataset)
+        if args.dst_dir:
+            comparator.save_compare_report(output, args.dst_dir)
 
-        output = {
-            "mismatches": mismatches,
-            "a_extra_items": sorted(a_extra),
-            "b_extra_items": sorted(b_extra),
-            "errors": errors,
-        }
-        if args.all:
-            output["matches"] = matches
-
-        output_file = osp.join(
-            dst_dir, generate_next_file_name("diff", ext=".json", basedir=dst_dir)
-        )
-        log.info("Saving diff to '%s'" % output_file)
-        dump_json_file(output_file, output, indent=True)
-
-        print("Found:")
-        print("The first project has %s unmatched items" % len(a_extra))
-        print("The second project has %s unmatched items" % len(b_extra))
-        print("%s item conflicts" % len(errors))
-        print("%s matching annotations" % len(matches))
-        print("%s mismatching annotations" % len(mismatches))
     elif args.method is ComparisonMethod.distance:
         comparator = DistanceComparator(iou_threshold=args.iou_thresh)
-
-        with DiffVisualizer(
+        with DistanceCompareVisualizer(
             save_dir=dst_dir, comparator=comparator, output_format=args.format
         ) as visualizer:
-            log.info("Saving diff to '%s'" % dst_dir)
+            log.info("Saving compare to '%s'" % dst_dir)
             visualizer.save(first_dataset, second_dataset)
 
     return 0
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/download.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import contextlib
 import logging as log
 import os
 import os.path as osp
 import sys
 from typing import Dict
 
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.extractor_tfds import (
     AVAILABLE_TFDS_DATASETS,
     TFDS_EXTRACTOR_AVAILABLE,
     TfdsDatasetRemoteMetadata,
 )
-from datumaro.components.project import Environment
 from datumaro.util import dump_json
 from datumaro.util.os_util import make_file_name
 
 from ..util import MultilineFormatter
 from ..util.errors import CliException
 from ..util.project import generate_next_file_name
 
@@ -44,15 +44,15 @@
     subparsers = parser.add_subparsers(title="Commands")
 
     build_get_subparser(subparsers)
     build_describe_subparser(subparsers)
 
 
 def build_get_subparser(subparsers: argparse._SubParsersAction):
-    builtin_writers = sorted(Environment().exporters)
+    builtin_writers = sorted(DEFAULT_ENVIRONMENT.exporters)
     if TFDS_EXTRACTOR_AVAILABLE:
         available_datasets = ", ".join(f"tfds:{name}" for name in AVAILABLE_TFDS_DATASETS)
     else:
         available_datasets = "N/A (TensorFlow and/or TensorFlow Datasets " "are not installed)"
 
     parser = subparsers.add_parser(
         name="get",
@@ -133,15 +133,15 @@
     return {
         download_command: ["dst_dir", "extra_args"],
         describe_downloads_command: ["report-file"],
     }
 
 
 def download_command(args):
-    env = Environment()
+    env = DEFAULT_ENVIRONMENT
 
     if args.dataset_id.startswith("tfds:"):
         if TFDS_EXTRACTOR_AVAILABLE:
             tfds_ds_name = args.dataset_id[5:]
             tfds_ds = AVAILABLE_TFDS_DATASETS.get(tfds_ds_name)
             if tfds_ds:
                 default_output_format = tfds_ds.metadata.default_output_format
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/explain.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/explore.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/explore.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 import shutil
 
+from datumaro.components.algorithms.hash_key_inference.explorer import Explorer
 from datumaro.components.errors import ProjectNotFoundError
-from datumaro.components.explorer import Explorer
 from datumaro.util import str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.project import load_project, parse_full_revpath
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/filter.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/generate.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging as log
 import os
 import os.path as osp
 from shutil import rmtree
 
 from datumaro.cli.util.errors import CliException
 from datumaro.plugins.synthetic_data import FractalImageGenerator
+from datumaro.util.definitions import DATUMARO_CACHE_DIR
 
 from ..util import MultilineFormatter
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Generate synthetic dataset",
@@ -52,16 +53,18 @@
         "--type",
         default="image",
         choices=["image"],
         help="Specify type of data to generate (default: %(default)s)",
     )
     parser.add_argument(
         "--model-dir",
+        type=str,
+        default=DATUMARO_CACHE_DIR,
         help="Path to load the colorization model from. "
-        "If no model is found, the model will be downloaded (default: current dir)",
+        "If no model is found, the model will be downloaded (default: %(default)s)",
     )
     parser.add_argument(
         "--overwrite", action="store_true", help="Overwrite existing files in the save directory"
     )
 
     parser.set_defaults(command=generate_command)
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/info.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/merge.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
 from datumaro.components.dataset import DEFAULT_FORMAT
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.hl_ops import HLOps
 from datumaro.components.merge.intersect_merge import IntersectMerge
 from datumaro.components.project import ProjectBuildTargets
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter, join_cli_args
@@ -228,15 +228,15 @@
     except ProjectNotFoundError:
         if not show_plugin_help and len(args.targets) == 1 and args.project_dir:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     try:
         exporter = env.exporters[args.format]
     except KeyError:
         raise CliException("Exporter for format '%s' is not found" % args.format)
 
     export_args = exporter.parse_cmdline(args.extra_args)
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/patch.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.errors import CliException
 from ..util.project import load_project, parse_full_revpath
 
@@ -127,15 +127,15 @@
     except ProjectNotFoundError:
         if args.project_dir:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     target_dataset, _project = parse_full_revpath(args.target, project)
     if _project is not None:
         scope_add(_project)
 
     try:
         exporter = env.exporters[target_dataset.format]
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 #
 # SPDX-License-Identifier: MIT
 
 
 import argparse
 import logging as log
 
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.util.scope import on_error_do, scope_add, scoped
 
 from ....util import MultilineFormatter, join_cli_args, show_video_import_warning
 from ....util.errors import CliException
 from ....util.project import load_project
 
 __all__ = [
     "build_parser",
     "get_sensitive_args",
 ]
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    env = Environment()
+    env = DEFAULT_ENVIRONMENT
     builtins = sorted(set(env.extractors) | set(env.importers))
 
     parser = parser_ctor(
         help="Add data source to project",
         description="""
         Adds a data source to a project. A data source is a dataset
         in a supported format (check 'formats' section below).|n
@@ -121,15 +121,15 @@
     except ProjectNotFoundError:
         if not show_plugin_help:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     fmt = args.format
     if fmt in env.importers:
         arg_parser = env.importers[fmt]
     elif fmt in env.extractors:
         arg_parser = env.extractors[fmt]
     else:
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.project import ProjectBuildTargets
 from datumaro.util.os_util import make_file_name
 from datumaro.util.scope import scope_add, scoped
 
 from ....util import MultilineFormatter
 from ....util.errors import CliException
@@ -20,15 +20,15 @@
 __all__ = [
     "build_parser",
     "get_sensitive_args",
 ]
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    builtins = sorted(Environment().exporters)
+    builtins = sorted(DEFAULT_ENVIRONMENT.exporters)
 
     parser = parser_ctor(
         help="Export project",
         description="""
         Exports a project in some format.|n
         |n
         Each dataset format has its own export
@@ -139,15 +139,15 @@
     except ProjectNotFoundError:
         if not show_plugin_help:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     try:
         exporter = env.exporters[args.format]
     except KeyError:
         raise CliException("Exporter for format '%s' is not found" % args.format)
 
     extra_args = exporter.parse_cmdline(args.extra_args)
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.util.scope import on_error_do, scope_add, scoped
 
 from ....util import MultilineFormatter, join_cli_args, show_video_import_warning
 from ....util.errors import CliException
 from ....util.project import generate_next_name, load_project
 
 __all__ = [
     "build_parser",
     "get_sensitive_args",
 ]
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    env = Environment()
+    env = DEFAULT_ENVIRONMENT
     builtins = sorted(set(env.extractors) | set(env.importers))
 
     parser = parser_ctor(
         help="Import dataset to project",
         description="""
         Imports a data source to a project. A data source is a dataset
         in a supported format (check 'formats' section below).|n
@@ -127,15 +127,15 @@
     except ProjectNotFoundError:
         if not show_plugin_help:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     fmt = args.format
     if fmt in env.importers:
         arg_parser = env.importers[fmt]
     elif fmt in env.extractors:
         arg_parser = env.extractors[fmt]
     else:
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/commands/stats.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (C) 2019-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 
-from datumaro.components.errors import ProjectNotFoundError
+from datumaro.cli.util.errors import CliException, WrongRevpathError
+from datumaro.components.errors import ConflictingCategoriesError, ProjectNotFoundError
 from datumaro.components.operations import compute_ann_statistics, compute_image_statistics
 from datumaro.util import dump_json_file, str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.project import generate_next_file_name, load_project, parse_full_revpath
 
@@ -83,15 +84,29 @@
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
     except ProjectNotFoundError:
         if args.project_dir:
             raise
 
-    dataset, target_project = parse_full_revpath(args.target, project)
+    try:
+        dataset, target_project = parse_full_revpath(args.target, project)
+    except WrongRevpathError as e:
+        for p in e.problems:
+            if isinstance(p, ConflictingCategoriesError):
+                src_names = [src for src in project.working_tree.sources]
+                raise CliException(
+                    "There are more than two sources with heterogeneous categories in the project. "
+                    "This prevents computing the statistics of the merged one. "
+                    f"Please specify one of the sources in the project ({src_names}), "
+                    f"such as `datum stats {src_names[0]}`"
+                ) from e
+
+        raise e
+
     if target_project:
         scope_add(target_project)
 
     if args.subset:
         dataset = dataset.get_subset(args.subset)
 
     stats = {}
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/transform.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.project import ProjectBuildTargets
 from datumaro.util import str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.errors import CliException
 from ..util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    builtins = sorted(Environment().transforms)
+    builtins = sorted(DEFAULT_ENVIRONMENT.transforms)
 
     parser = parser_ctor(
         help="Transform project",
         description="""
         Applies a batch operation to a dataset and produces a new dataset.|n
         |n
         By default, datasets are updated in-place. The '-o/--output-dir'
@@ -162,15 +162,15 @@
     except ProjectNotFoundError:
         if not show_plugin_help and args.project_dir:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     try:
         transform = env.transforms[args.transform]
     except KeyError:
         raise CliException("Transform '%s' is not found" % args.transform)
 
     extra_args = transform.parse_cmdline(args.extra_args)
```

### Comparing `datumaro-1.3.2/datumaro/cli/commands/validate.py` & `datumaro-1.4.0rc1/src/datumaro/cli/commands/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2020-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 
-from datumaro.components.environment import Environment
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.validator import TaskType
 from datumaro.util import dump_json_file
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.errors import CliException
@@ -109,15 +109,15 @@
     except ProjectNotFoundError:
         if not show_plugin_help and args.project_dir:
             raise
 
     if project is not None:
         env = project.env
     else:
-        env = Environment()
+        env = DEFAULT_ENVIRONMENT
 
     try:
         validator_type = env.validators[args.task]
     except KeyError:
         raise CliException("Validator type '%s' is not found" % args.task)
 
     extra_args = validator_type.parse_cmdline(args.extra_args)
```

### Comparing `datumaro-1.3.2/datumaro/cli/contexts/model.py` & `datumaro-1.4.0rc1/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/contexts/source.py` & `datumaro-1.4.0rc1/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/contexts/util.py` & `datumaro-1.4.0rc1/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/util/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/cli/util/diff.py` & `datumaro-1.4.0rc1/src/datumaro/cli/util/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset import IDataset
 from datumaro.util import parse_str_enum_value
 from datumaro.util.image import save_image
 
 
-class DiffVisualizer:
+class DistanceCompareVisualizer:
     class OutputFormat(Enum):
         simple = auto()
         tensorboard = auto()
 
     DEFAULT_FORMAT = OutputFormat.simple
     _UNMATCHED_LABEL = -1
 
@@ -45,15 +45,15 @@
 
         self._save_dir = save_dir
 
     def __enter__(self):
         os.makedirs(self._save_dir, exist_ok=True)
 
         if self._output_format is self.OutputFormat.tensorboard:
-            logdir = osp.join(self._save_dir, "logs", "diff")
+            logdir = osp.join(self._save_dir, "logs", "compare")
             self._file_writer = tb.SummaryWriter(logdir)
         elif self._output_format is self.OutputFormat.simple:
             self._label_diff_writer = None
 
         self._a_classes = {}
         self._b_classes = {}
```

### Comparing `datumaro-1.3.2/datumaro/cli/util/project.py` & `datumaro-1.4.0rc1/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.4.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/algorithms/rise.py` & `datumaro-1.4.0rc1/src/datumaro/components/algorithms/rise.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 
         rng = lambda shape=None: np.random.rand(*shape)
         samples = np.prod(image_size)
         if self.max_samples is not None:
             samples = min(self.max_samples, samples)
         batch_size = self.batch_size
 
-        result = next(iter(model.launch(_expand(image, 0))))
+        pred = next(iter(model.infer(_expand(image, 0))))
+        result = model.postprocess(pred, None)
         result_labels, result_bboxes = self.split_outputs(result)
         if 0 < self.det_conf_thresh:
             result_bboxes = [
                 b for b in result_bboxes if self.det_conf_thresh <= b.attributes["score"]
             ]
         if 0 < self.nms_thresh:
             result_bboxes = nms(result_bboxes, self.nms_thresh)
@@ -161,15 +162,16 @@
                     int(offsets[1]) : int(image_size[1] + offsets[1]),
                 ]
                 batch_masks[i] = mask
 
             batch_inputs = full_batch_inputs[:current_batch_size]
             np.multiply(_expand(batch_masks), _expand(image, 0), out=batch_inputs)
 
-            results = model.launch(batch_inputs)
+            preds = model.infer(batch_inputs)
+            results = [model.postprocess(pred, None) for pred in preds]
             for mask, result in zip(batch_masks, results):
                 result_labels, result_bboxes = self.split_outputs(result)
 
                 confs.fill(0)
                 if len(predicted_labels) != 0:
                     for r in result_labels:
                         idx = predicted_labels.get(r.label, None)
```

### Comparing `datumaro-1.3.2/datumaro/components/annotation.py` & `datumaro-1.4.0rc1/src/datumaro/components/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     bbox = 6
     caption = 7
     cuboid_3d = 8
     super_resolution_annotation = 9
     depth_annotation = 10
     ellipse = 11
     hash_key = 12
+    feature_vector = 13
 
 
 COORDINATE_ROUNDING_DIGITS = 2
 CHECK_POLYGON_EQ_EPSILONE = 1e-7
 NO_GROUP = 0
 
 
@@ -107,15 +108,15 @@
     @attrs(slots=True, order=False)
     class LabelGroup:
         name: str = field(converter=str, validator=not_empty)
         labels: List[str] = field(default=[], validator=default_if_none(list))
         group_type: str = field(default="exclusive", validator=default_if_none(str))
 
     items: List[str] = field(factory=list, validator=default_if_none(list))
-    label_groups: List[str] = field(factory=list, validator=default_if_none(list))
+    label_groups: List[LabelGroup] = field(factory=list, validator=default_if_none(list))
     _indices: Dict[str, int] = field(factory=dict, init=False, eq=False)
 
     @classmethod
     def from_iterable(
         cls,
         iterable: Iterable[
             Union[
@@ -211,15 +212,40 @@
     _type = AnnotationType.label
     label: int = field(converter=int)
 
 
 @attrs(slots=True, eq=False, order=False)
 class HashKey(Annotation):
     _type = AnnotationType.hash_key
-    hash_key: np.ndarray = field(factory=lambda: np.zeros((1, 64), dtype=np.uint8))
+    hash_key: np.ndarray = field(validator=attr.validators.instance_of(np.ndarray))
+
+    @hash_key.validator
+    def _validate(self, attribute, value: np.ndarray):
+        """Check whether value is a 1D Numpy array having 64 np.uint8 values"""
+        if value.ndim != 1 or value.shape[0] != 64 or value.dtype != np.uint8:
+            raise ValueError(value)
+
+    def __eq__(self, other):
+        if not super().__eq__(other):
+            return False
+        if not isinstance(other, __class__):
+            return False
+        return np.array_equal(self.hash_key, other.hash_key)
+
+
+@attrs(eq=False, order=False)
+class FeatureVector(Annotation):
+    _type = AnnotationType.feature_vector
+    vector: np.ndarray = field(validator=attr.validators.instance_of(np.ndarray))
+
+    @vector.validator
+    def _validate(self, attribute, value: np.ndarray):
+        """Check whether value is a 1D Numpy array"""
+        if value.ndim != 1:
+            raise ValueError(value)
 
     def __eq__(self, other):
         if not super().__eq__(other):
             return False
         if not isinstance(other, __class__):
             return False
         return np.array_equal(self.hash_key, other.hash_key)
```

### Comparing `datumaro-1.3.2/datumaro/components/annotations/merger.py` & `datumaro-1.4.0rc1/src/datumaro/components/annotations/merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from datumaro.util.annotation_util import mean_bbox, segment_iou
 
 from .matcher import (
     AnnotationMatcher,
     BboxMatcher,
     CaptionsMatcher,
     Cuboid3dMatcher,
+    FeatureVectorMatcher,
     HashKeyMatcher,
     ImageAnnotationMatcher,
     LabelMatcher,
     LineMatcher,
     MaskMatcher,
     PointsMatcher,
     PolygonMatcher,
@@ -32,14 +33,15 @@
     "PointsMerger",
     "LineMerger",
     "CaptionsMerger",
     "Cuboid3dMerger",
     "ImageAnnotationMerger",
     "EllipseMerger",
     "HashKeyMerger",
+    "FeatureVectorMerger",
 ]
 
 
 @attrs(kw_only=True)
 class AnnotationMerger(AnnotationMatcher):
     def merge_clusters(self, clusters):
         raise NotImplementedError()
@@ -186,7 +188,12 @@
 class EllipseMerger(_ShapeMerger, ShapeMatcher):
     pass
 
 
 @attrs
 class HashKeyMerger(AnnotationMerger, HashKeyMatcher):
     pass
+
+
+@attrs
+class FeatureVectorMerger(AnnotationMerger, FeatureVectorMatcher):
+    pass
```

### Comparing `datumaro-1.3.2/datumaro/components/cli_plugin.py` & `datumaro-1.4.0rc1/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/config.py` & `datumaro-1.4.0rc1/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/config_model.py` & `datumaro-1.4.0rc1/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/crypter.py` & `datumaro-1.4.0rc1/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/dataset_base.py` & `datumaro-1.4.0rc1/src/datumaro/components/dataset_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,22 @@
 
         All the items are supposed to have the same media type.
         Supposed to be constant and known immediately after the
         object construction (i.e. doesn't require dataset iteration).
         """
         raise NotImplementedError()
 
+    @property
+    def is_stream(self) -> bool:
+        """Boolean indicating whether the dataset is a stream
+
+        If the dataset is a stream, the dataset item is generated on demand from its iterator.
+        """
+        return False
+
 
 class _DatasetBase(IDataset):
     def __init__(self, *, length: Optional[int] = None, subsets: Optional[Sequence[str]] = None):
         self._length = length
         self._subsets = subsets
 
     def _init_cache(self):
```

### Comparing `datumaro-1.3.2/datumaro/components/dataset_item_storage.py` & `datumaro-1.4.0rc1/src/datumaro/components/dataset_item_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from copy import copy
+from enum import Enum, auto
 from typing import Any, Iterator, Optional, Tuple, Type, Union
 
 from datumaro.components.annotation import AnnotationType
 from datumaro.components.dataset_base import CategoriesInfo, DatasetInfo, DatasetItem, IDataset
 from datumaro.components.media import MediaElement
 from datumaro.util.definitions import DEFAULT_SUBSET_NAME
 
+__all__ = ["ItemStatus", "DatasetItemStorage", "DatasetItemStorageDatasetView"]
+
+
+class ItemStatus(Enum):
+    added = auto()
+    modified = auto()
+    removed = auto()
+
 
 class DatasetItemStorage:
     def __init__(self):
         self.data = {}  # { subset_name: { id: DatasetItem } }
         self._traversal_order = {}  # maintain the order of elements
 
     def __iter__(self) -> Iterator[DatasetItem]:
```

### Comparing `datumaro-1.3.2/datumaro/components/environment.py` & `datumaro-1.4.0rc1/src/datumaro/components/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,109 +7,133 @@
 import logging as log
 import os.path as osp
 from functools import partial
 from inspect import isclass
 from typing import (
     Callable,
     Dict,
+    Generator,
     Generic,
     Iterable,
     Iterator,
     List,
     Optional,
     Sequence,
     Set,
+    Tuple,
     Type,
     TypeVar,
 )
 
 from datumaro.components.cli_plugin import CliPlugin, plugin_types
 from datumaro.components.format_detection import (
     DetectedFormat,
     FormatDetectionConfidence,
     RejectionReason,
     detect_dataset_format,
 )
+from datumaro.components.lazy_plugin import PLUGIN_TYPES, LazyPlugin
 from datumaro.util.os_util import import_foreign_module, split_path
 
 T = TypeVar("T")
 
 
 class Registry(Generic[T]):
     def __init__(self):
-        self.items: Dict[str, T] = {}
+        self._items: Dict[str, T] = {}
 
     def register(self, name: str, value: T) -> T:
-        self.items[name] = value
+        self._items[name] = value
         return value
 
     def unregister(self, name: str) -> Optional[T]:
-        return self.items.pop(name, None)
+        return self._items.pop(name, None)
 
     def get(self, key: str):
         """Returns a class or a factory function"""
-        return self.items[key]
+        return self._items[key]
 
     def __getitem__(self, key: str) -> T:
         return self.get(key)
 
     def __contains__(self, key) -> bool:
-        return key in self.items
+        return key in self._items
 
     def __iter__(self) -> Iterator[str]:
-        return iter(self.items)
+        return iter(self._items)
+
+    def items(self) -> Generator[Tuple[str, T], None, None]:
+        for key in self:
+            yield key, self.get(key)
 
 
 class PluginRegistry(Registry[Type[CliPlugin]]):
     def __init__(
         self, filter: Callable[[Type[CliPlugin]], bool] = None
     ):  # pylint: disable=redefined-builtin
         super().__init__()
         self._filter = filter
 
+    def get(self, key: str) -> PLUGIN_TYPES:
+        """Returns a class or a factory function"""
+        item = self._items[key]
+        if issubclass(item, LazyPlugin):
+            return item.get_plugin_cls()
+        return item
+
     def batch_register(self, values: Iterable[CliPlugin]):
         for v in values:
             if self._filter and not self._filter(v):
                 continue
 
             self.register(v.NAME, v)
 
 
 class Environment:
     _builtin_plugins = None
 
     @classmethod
-    def _make_filter(cls, accept, skip=None):
+    def _make_filter(cls, accept, decline=None, skip=None):
         accept = (accept,) if isclass(accept) else tuple(accept)
         skip = {skip} if isclass(skip) else set(skip or [])
         skip = tuple(skip | set(accept))
-        return partial(cls._check_type, accept=accept, skip=skip)
+        return partial(cls._check_type, accept=accept, decline=decline, skip=skip)
 
     @staticmethod
-    def _check_type(t, *, accept, skip):
-        return issubclass(t, accept) and t not in skip
+    def _check_type(t, *, accept, decline, skip):
+        if not issubclass(t, accept) or t in skip or (decline and issubclass(t, decline)):
+            return False
 
-    def __init__(self):
+        return True
+
+    def __init__(self, use_lazy_import: bool = True):
         from datumaro.components.dataset_base import DatasetBase, SubsetBase
         from datumaro.components.exporter import Exporter
         from datumaro.components.generator import DatasetGenerator
         from datumaro.components.importer import Importer
         from datumaro.components.launcher import Launcher
         from datumaro.components.transformer import ItemTransform, Transform
         from datumaro.components.validator import Validator
 
         _filter = self._make_filter
-        self._extractors = PluginRegistry(_filter(DatasetBase, skip=SubsetBase))
+        self._extractors = PluginRegistry(
+            _filter(
+                DatasetBase,
+                decline=Transform,
+                skip=(SubsetBase, Transform, ItemTransform),
+            )
+        )
         self._importers = PluginRegistry(_filter(Importer))
         self._launchers = PluginRegistry(_filter(Launcher))
         self._exporters = PluginRegistry(_filter(Exporter))
         self._generators = PluginRegistry(_filter(DatasetGenerator))
         self._transforms = PluginRegistry(_filter(Transform, skip=ItemTransform))
         self._validators = PluginRegistry(_filter(Validator))
         self._builtins_initialized = False
+        self._use_lazy_import = use_lazy_import
 
     def _get_plugin_registry(self, name):
         if not self._builtins_initialized:
             self._builtins_initialized = True
             self._register_builtin_plugins()
         return getattr(self, name)
 
@@ -206,14 +230,24 @@
             )
             all_exports.extend(exports)
 
         return all_exports
 
     @classmethod
     def _load_builtin_plugins(cls):
+        """Load builtin plugins which will be imported lazily using plugin spec files"""
+        if cls._builtin_plugins is None:
+            from datumaro.plugins.specs import get_lazy_plugins
+
+            cls._builtin_plugins = get_lazy_plugins()
+        return cls._builtin_plugins
+
+    @classmethod
+    def _load_builtin_plugins_from_importlib(cls):
+        """Load builtin plugins from importlib, not lazy import from plugin spec files"""
         if cls._builtin_plugins is None:
             import datumaro.plugins
 
             plugins_dir = osp.dirname(datumaro.plugins.__file__)
             module_names = [
                 datumaro.plugins.__name__ + "." + name for name in cls._find_plugins(plugins_dir)
             ]
@@ -225,15 +259,19 @@
         plugins = self._load_plugins(
             module_names, importer=partial(import_foreign_module, path=plugins_dir)
         )
 
         self.register_plugins(plugins)
 
     def _register_builtin_plugins(self):
-        self.register_plugins(self._load_builtin_plugins())
+        self.register_plugins(
+            self._load_builtin_plugins()
+            if self._use_lazy_import
+            else self._load_builtin_plugins_from_importlib()
+        )
 
     def register_plugins(self, plugins):
         self.extractors.batch_register(plugins)
         self.importers.batch_register(plugins)
         self.launchers.batch_register(plugins)
         self.exporters.batch_register(plugins)
         self.generators.batch_register(plugins)
@@ -270,15 +308,15 @@
         ignore_dirs = {"__MSOSX", "__MACOSX"}
         all_matched_formats: Set[DetectedFormat] = set()
 
         for _ in range(depth + 1):
             detected_formats = detect_dataset_format(
                 (
                     (format_name, importer.detect)
-                    for format_name, importer in self.importers.items.items()
+                    for format_name, importer in self.importers.items()
                 ),
                 path,
                 rejection_callback=rejection_callback,
             )
 
             if detected_formats:
                 all_matched_formats |= set(detected_formats)
@@ -318,9 +356,13 @@
             _register(env.exporters)
             _register(env.generators)
             _register(env.transforms)
             _register(env.validators)
 
         return merged
 
+    @classmethod
+    def release_builtin_plugins(cls):
+        cls._builtin_plugins = None
+
 
 DEFAULT_ENVIRONMENT = Environment()
```

### Comparing `datumaro-1.3.2/datumaro/components/errors.py` & `datumaro-1.4.0rc1/src/datumaro/components/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,18 @@
         return """
             The project you're trying to load was
             created by the old Datumaro version. Try to migrate the
             project with 'datum project migrate' and then reload.
             """
 
 
+class NotAvailableError(DatumaroError):
+    pass
+
+
 @define(auto_exc=False)
 class ProjectNotFoundError(DatumaroError):
     path = field()
 
     def __str__(self):
         return f"Can't find project at '{self.path}'"
```

### Comparing `datumaro-1.3.2/datumaro/components/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/extractor_tfds.py` & `datumaro-1.4.0rc1/src/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/filter.py` & `datumaro-1.4.0rc1/src/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/format_detection.py` & `datumaro-1.4.0rc1/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/generator.py` & `datumaro-1.4.0rc1/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/importer.py` & `datumaro-1.4.0rc1/src/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/media.py` & `datumaro-1.4.0rc1/src/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/media_manager.py` & `datumaro-1.4.0rc1/src/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/merge/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/merge/base.py` & `datumaro-1.4.0rc1/src/datumaro/components/merge/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 #
 # SPDX-License-Identifier: MIT
 import logging as log
 import os
 from collections import OrderedDict
 from typing import Dict, Optional, Sequence, Type
 
-from datumaro.components.abstracts.merger import IMerger
+from datumaro.components.abstracts.merger import IMergerContext
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import IDataset
 from datumaro.components.dataset_item_storage import DatasetItemStorageDatasetView
 from datumaro.components.errors import (
     ConflictingCategoriesError,
     DatasetMergeError,
     DatasetQualityError,
     MediaTypeError,
 )
 from datumaro.components.media import MediaElement
 from datumaro.util import dump_json_file
 
 
-class Merger(IMerger, CliPlugin):
+class Merger(IMergerContext, CliPlugin):
     """Merge multiple datasets into one dataset"""
 
     def __init__(self, **options):
         super().__init__(**options)
         self.__dict__["_sources"] = None
         self.errors = []
 
@@ -100,7 +100,10 @@
                 ("All errors", all_errors),
             ]
         )
 
         os.makedirs(os.path.dirname(path), exist_ok=True)
 
         dump_json_file(path, errors, indent=True)
+
+    def get_any_label_name(self, ann, label_id):
+        raise NotImplementedError
```

### Comparing `datumaro-1.3.2/datumaro/components/merge/exact_merge.py` & `datumaro-1.4.0rc1/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/merge/intersect_merge.py` & `datumaro-1.4.0rc1/src/datumaro/components/merge/intersect_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 from datumaro.components.annotations.merger import (
     AnnotationMerger,
     BboxMerger,
     CaptionsMerger,
     Cuboid3dMerger,
     EllipseMerger,
+    FeatureVectorMerger,
     HashKeyMerger,
     ImageAnnotationMerger,
     LabelMerger,
     LineMerger,
     MaskMerger,
     PointsMerger,
     PolygonMerger,
@@ -437,14 +438,16 @@
                 return _make(ImageAnnotationMerger, **kwargs)
             elif t is AnnotationType.depth_annotation:
                 return _make(ImageAnnotationMerger, **kwargs)
             elif t is AnnotationType.ellipse:
                 return _make(EllipseMerger, **kwargs)
             elif t is AnnotationType.hash_key:
                 return _make(HashKeyMerger, **kwargs)
+            elif t is AnnotationType.feature_vector:
+                return _make(FeatureVectorMerger, **kwargs)
             else:
                 raise NotImplementedError("Type %s is not supported" % t)
 
         instance_map = {}
         for s in sources:
             s_instances = find_instances(s)
             for inst in s_instances:
@@ -608,15 +611,15 @@
             return None
         item_id = self._ann_map[id(ann)][1]
         dataset_id = self._item_map[item_id][1]
         return (
             self._dataset_map[dataset_id][0].categories()[AnnotationType.label].items[label_id].name
         )
 
-    def _get_any_label_name(self, ann, label_id):
+    def get_any_label_name(self, ann, label_id):
         if label_id is None:
             return None
         try:
             return self._get_src_label_name(ann, label_id)
         except KeyError:
             return self._get_label_name(label_id)
```

### Comparing `datumaro-1.3.2/datumaro/components/merge/union_merge.py` & `datumaro-1.4.0rc1/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/operations.py` & `datumaro-1.4.0rc1/src/datumaro/components/comparator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,348 +1,37 @@
-# Copyright (C) 2020-2023 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import hashlib
 import logging as log
-import warnings
-from copy import deepcopy
-from typing import Callable, Dict, Optional, Set, Tuple
+import os
+import os.path as osp
+from textwrap import wrap
+from typing import Dict, List, Set, Tuple
 from unittest import TestCase
 
-import cv2
-import numpy as np
 from attr import attrib, attrs
+from tabulate import tabulate
 
+from datumaro.cli.util.project import generate_next_file_name
 from datumaro.components.annotation import AnnotationType, LabelCategories
-from datumaro.components.annotations.matcher import LineMatcher, PointsMatcher, match_segments
-from datumaro.components.dataset_base import CategoriesInfo, DatasetItem, IDataset
-from datumaro.components.errors import DatumaroError
-from datumaro.components.media import Image
-from datumaro.util import filter_dict, find
+from datumaro.components.annotations.matcher import LineMatcher, PointsMatcher, match_segments_pair
+from datumaro.components.dataset import Dataset
+from datumaro.components.operations import (
+    compute_ann_statistics,
+    compute_image_statistics,
+    match_items_by_id,
+    match_items_by_image_hash,
+)
+from datumaro.components.shift_analyzer import ShiftAnalyzer
+from datumaro.util import dump_json_file, filter_dict, find
 from datumaro.util.annotation_util import find_instances, max_bbox
 from datumaro.util.attrs_util import default_if_none
 
 
-def mean_std(dataset: IDataset):
-    counter = _MeanStdCounter()
-
-    for item in dataset:
-        counter.accumulate(item)
-
-    return counter.get_result()
-
-
-class _MeanStdCounter:
-    """
-    Computes unbiased mean and std. dev. for dataset images, channel-wise.
-    """
-
-    def __init__(self):
-        self._stats = {}  # (id, subset) -> (pixel count, mean vec, std vec)
-
-    def accumulate(self, item: DatasetItem):
-        size = item.media.size
-        if size is None:
-            log.warning(
-                "Item %s: can't detect image size, "
-                "the image will be skipped from pixel statistics",
-                item.id,
-            )
-            return
-        count = np.prod(item.media.size)
-
-        image = item.media.data
-        if len(image.shape) == 2:
-            image = image[:, :, np.newaxis]
-        else:
-            image = image[:, :, :3]
-        # opencv is much faster than numpy here
-        mean, std = cv2.meanStdDev(image.astype(np.double) / 255)
-
-        self._stats[(item.id, item.subset)] = (count, mean, std)
-
-    def get_result(self) -> Tuple[Tuple[float, float, float], Tuple[float, float, float]]:
-        n = len(self._stats)
-
-        if n == 0:
-            return [0, 0, 0], [0, 0, 0]
-
-        counts = np.empty(n, dtype=np.uint32)
-        stats = np.empty((n, 2, 3), dtype=np.double)
-
-        for i, v in enumerate(self._stats.values()):
-            counts[i] = v[0]
-            stats[i][0] = v[1].reshape(-1)
-            stats[i][1] = v[2].reshape(-1)
-
-        mean = lambda i, s: s[i][0]
-        var = lambda i, s: s[i][1]
-
-        # make variance unbiased
-        np.multiply(np.square(stats[:, 1]), (counts / (counts - 1))[:, np.newaxis], out=stats[:, 1])
-
-        # Use an online algorithm to:
-        # - handle different image sizes
-        # - avoid cancellation problem
-        _, mean, var = self._compute_stats(stats, counts, mean, var)
-        return mean * 255, np.sqrt(var) * 255
-
-    # Implements online parallel computation of sample variance
-    # https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Parallel_algorithm
-    @staticmethod
-    def _pairwise_stats(count_a, mean_a, var_a, count_b, mean_b, var_b):
-        """
-        Computes vector mean and variance.
-
-        Needed do avoid catastrophic cancellation in floating point computations
-
-        Returns:
-            A tuple (total count, mean, variance)
-        """
-
-        # allow long arithmetics
-        count_a = int(count_a)
-        count_b = int(count_b)
-
-        delta = mean_b - mean_a
-        m_a = var_a * (count_a - 1)
-        m_b = var_b * (count_b - 1)
-        M2 = m_a + m_b + delta**2 * (count_a * count_b / (count_a + count_b))
-
-        return (count_a + count_b, mean_a * 0.5 + mean_b * 0.5, M2 / (count_a + count_b - 1))
-
-    @staticmethod
-    def _compute_stats(stats, counts, mean_accessor, variance_accessor):
-        """
-        Recursively computes total count, mean and variance,
-        does O(log(N)) calls.
-
-        Args:
-            stats: (float array of shape N, 2 * d, d = dimensions of values)
-            count: (integer array of shape N)
-            mean_accessor: (function(idx, stats)) to retrieve element mean
-            variance_accessor: (function(idx, stats)) to retrieve element variance
-
-        Returns:
-            A tuple (total count, mean, variance)
-        """
-
-        m = mean_accessor
-        v = variance_accessor
-        n = len(stats)
-        if n == 1:
-            return counts[0], m(0, stats), v(0, stats)
-        if n == 2:
-            return __class__._pairwise_stats(
-                counts[0], m(0, stats), v(0, stats), counts[1], m(1, stats), v(1, stats)
-            )
-        h = n // 2
-        return __class__._pairwise_stats(
-            *__class__._compute_stats(stats[:h], counts[:h], m, v),
-            *__class__._compute_stats(stats[h:], counts[h:], m, v),
-        )
-
-    def __len__(self) -> int:
-        return len(self._stats)
-
-
-IMAGE_STATS_SCHEMA = {
-    "dataset": {
-        "images count": 0,
-        "unique images count": 0,
-        "repeated images count": 0,
-        "repeated images": [],  # [[id1, id2], [id3, id4, id5], ...]
-    },
-    "subsets": {},
-}
-
-
-def compute_image_statistics(dataset: IDataset):
-    if dataset.media_type() != Image:
-        raise DatumaroError(
-            f"Your dataset's media_type is {dataset.media_type()}, "
-            "but only Image media_type is allowed."
-        )
-
-    stats = deepcopy(IMAGE_STATS_SCHEMA)
-
-    stats_counter = _MeanStdCounter()
-    unique_counter = _ItemMatcher()
-
-    for item in dataset:
-        if not isinstance(item.media, Image):
-            warnings.warn(
-                f"item (id: {item.id}, subset: {item.subset})"
-                f" has media_type, {item.media} but only Image media_type is allowed."
-            )
-            continue
-
-        stats_counter.accumulate(item)
-        unique_counter.process_item(item)
-
-    def _extractor_stats(subset_name):
-        sub_counter = _MeanStdCounter()
-        sub_counter._stats = {
-            k: v
-            for k, v in stats_counter._stats.items()
-            if subset_name and k[1] == subset_name or not subset_name
-        }
-
-        available = len(sub_counter._stats) != 0
-
-        stats = {
-            "images count": len(sub_counter),
-        }
-
-        if available:
-            mean, std = sub_counter.get_result()
-
-            stats.update(
-                {
-                    "image mean": [float(v) for v in mean[::-1]],
-                    "image std": [float(v) for v in std[::-1]],
-                }
-            )
-        else:
-            stats.update(
-                {
-                    "image mean": "n/a",
-                    "image std": "n/a",
-                }
-            )
-        return stats
-
-    for subset_name in dataset.subsets():
-        stats["subsets"][subset_name] = _extractor_stats(subset_name)
-
-    unique_items = unique_counter.get_result()
-    repeated_items = [sorted(g) for g in unique_items.values() if 1 < len(g)]
-
-    stats["dataset"].update(
-        {
-            "images count": len(stats_counter),
-            "unique images count": len(unique_items),
-            "repeated images count": len(repeated_items),
-            "repeated images": repeated_items,  # [[id1, id2], [id3, id4, id5], ...]
-        }
-    )
-
-    return stats
-
-
-def compute_ann_statistics(dataset: IDataset):
-    labels = dataset.categories().get(AnnotationType.label, LabelCategories())
-
-    def get_label(ann):
-        return labels.items[ann.label].name if ann.label is not None else None
-
-    stats = {
-        "images count": 0,
-        "annotations count": 0,
-        "unannotated images count": 0,
-        "unannotated images": [],
-        "annotations by type": {
-            t.name: {
-                "count": 0,
-            }
-            for t in AnnotationType
-        },
-        "annotations": {},
-    }
-    by_type = stats["annotations by type"]
-
-    attr_template = {
-        "count": 0,
-        "values count": 0,
-        "values present": set(),
-        "distribution": {},  # value -> (count, total%)
-    }
-    label_stat = {
-        "count": 0,
-        "distribution": {l.name: [0, 0] for l in labels.items},  # label -> (count, total%)
-        "attributes": {},
-    }
-    stats["annotations"]["labels"] = label_stat
-    segm_stat = {
-        "avg. area": 0,
-        "area distribution": [],  # a histogram with 10 bins
-        # (min, min+10%), ..., (min+90%, max) -> (count, total%)
-        "pixel distribution": {l.name: [0, 0] for l in labels.items},  # label -> (count, total%)
-    }
-    stats["annotations"]["segments"] = segm_stat
-    segm_areas = []
-    pixel_dist = segm_stat["pixel distribution"]
-    total_pixels = 0
-
-    for item in dataset:
-        if len(item.annotations) == 0:
-            stats["unannotated images"].append(item.id)
-            continue
-
-        for ann in item.annotations:
-            by_type[ann.type.name]["count"] += 1
-
-            if not hasattr(ann, "label") or ann.label is None:
-                continue
-
-            if ann.type in {AnnotationType.mask, AnnotationType.polygon, AnnotationType.bbox}:
-                area = ann.get_area()
-                segm_areas.append(area)
-                pixel_dist[get_label(ann)][0] += int(area)
-
-            label_stat["count"] += 1
-            label_stat["distribution"][get_label(ann)][0] += 1
-
-            for name, value in ann.attributes.items():
-                if name.lower() in {"occluded", "visibility", "score", "id", "track_id"}:
-                    continue
-                attrs_stat = label_stat["attributes"].setdefault(name, deepcopy(attr_template))
-                attrs_stat["count"] += 1
-                attrs_stat["values present"].add(str(value))
-                attrs_stat["distribution"].setdefault(str(value), [0, 0])[0] += 1
-
-    stats["images count"] = len(dataset)
-
-    stats["annotations count"] = sum(t["count"] for t in stats["annotations by type"].values())
-    stats["unannotated images count"] = len(stats["unannotated images"])
-
-    for label_info in label_stat["distribution"].values():
-        label_info[1] = label_info[0] / (label_stat["count"] or 1)
-
-    for label_attr in label_stat["attributes"].values():
-        label_attr["values count"] = len(label_attr["values present"])
-        label_attr["values present"] = sorted(label_attr["values present"])
-        for attr_info in label_attr["distribution"].values():
-            attr_info[1] = attr_info[0] / (label_attr["count"] or 1)
-
-    # numpy.sum might be faster, but could overflow with large datasets.
-    # Python's int can transparently mutate to be of indefinite precision (long)
-    total_pixels = sum(int(a) for a in segm_areas)
-
-    segm_stat["avg. area"] = total_pixels / (len(segm_areas) or 1.0)
-
-    for label_info in segm_stat["pixel distribution"].values():
-        label_info[1] = label_info[0] / (total_pixels or 1)
-
-    if len(segm_areas) != 0:
-        hist, bins = np.histogram(segm_areas)
-        segm_stat["area distribution"] = [
-            {
-                "min": float(bin_min),
-                "max": float(bin_max),
-                "count": int(c),
-                "percent": int(c) / len(segm_areas),
-            }
-            for c, (bin_min, bin_max) in zip(hist, zip(bins[:-1], bins[1:]))
-        ]
-
-    return stats
-
-
 @attrs
 class DistanceComparator:
     iou_threshold = attrib(converter=float, default=0.5)
 
     def match_annotations(self, item_a, item_b):
         return {t: self._match_ann_type(t, item_a, item_b) for t in AnnotationType}
 
@@ -376,15 +65,15 @@
         a_unmatched = a_labels - b_labels
         b_unmatched = b_labels - a_labels
         return matches, a_unmatched, b_unmatched
 
     def _match_segments(self, t, item_a, item_b):
         a_boxes = self._get_ann_type(t, item_a)
         b_boxes = self._get_ann_type(t, item_b)
-        return match_segments(a_boxes, b_boxes, dist_thresh=self.iou_threshold)
+        return match_segments_pair(a_boxes, b_boxes, dist_thresh=self.iou_threshold)
 
     def match_polygons(self, item_a, item_b):
         return self._match_segments(AnnotationType.polygon, item_a, item_b)
 
     def match_masks(self, item_a, item_b):
         return self._match_segments(AnnotationType.mask, item_a, item_b)
 
@@ -400,116 +89,36 @@
             s_instances = find_instances(s)
             for inst in s_instances:
                 inst_bbox = max_bbox(inst)
                 for ann in inst:
                     instance_map[id(ann)] = [inst, inst_bbox]
         matcher = PointsMatcher(instance_map=instance_map)
 
-        return match_segments(
+        return match_segments_pair(
             a_points, b_points, dist_thresh=self.iou_threshold, distance=matcher.distance
         )
 
     def match_lines(self, item_a, item_b):
         a_lines = self._get_ann_type(AnnotationType.polyline, item_a)
         b_lines = self._get_ann_type(AnnotationType.polyline, item_b)
 
         matcher = LineMatcher()
 
-        return match_segments(
+        return match_segments_pair(
             a_lines, b_lines, dist_thresh=self.iou_threshold, distance=matcher.distance
         )
 
 
-def match_items_by_id(a: IDataset, b: IDataset):
-    a_items = set((item.id, item.subset) for item in a)
-    b_items = set((item.id, item.subset) for item in b)
-
-    matches = a_items & b_items
-    matches = [([m], [m]) for m in matches]
-    a_unmatched = a_items - b_items
-    b_unmatched = b_items - a_items
-    return matches, a_unmatched, b_unmatched
-
-
-def match_items_by_image_hash(a: IDataset, b: IDataset):
-    a_hash = find_unique_images(a)
-    b_hash = find_unique_images(b)
-
-    a_items = set(a_hash)
-    b_items = set(b_hash)
-
-    matches = a_items & b_items
-    a_unmatched = a_items - b_items
-    b_unmatched = b_items - a_items
-
-    matches = [(a_hash[h], b_hash[h]) for h in matches]
-    a_unmatched = set(i for h in a_unmatched for i in a_hash[h])
-    b_unmatched = set(i for h in b_unmatched for i in b_hash[h])
-
-    return matches, a_unmatched, b_unmatched
-
-
-class _ItemMatcher:
-    @staticmethod
-    def _default_item_hash(item: DatasetItem):
-        if not item.media or not item.media.has_data:
-            if item.media and hasattr(item.media, "path"):
-                return hash(item.media.path)
-
-            log.warning(
-                "Item (%s, %s) has no image " "info, counted as unique", item.id, item.subset
-            )
-            return None
-
-        # Disable B303:md5, because the hash is not used in a security context
-        return hashlib.md5(item.media.data.tobytes()).hexdigest()  # nosec
-
-    def __init__(self, item_hash: Optional[Callable] = None):
-        self._hash = item_hash or self._default_item_hash
-
-        # hash -> [(id, subset), ...]
-        self._unique: Dict[str, Set[Tuple[str, str]]] = {}
-
-    def process_item(self, item: DatasetItem):
-        h = self._hash(item)
-        if h is None:
-            h = str(id(item))  # anything unique
-
-        self._unique.setdefault(h, set()).add((item.id, item.subset))
-
-    def get_result(self):
-        return self._unique
-
-
-def find_unique_images(dataset: IDataset, item_hash: Optional[Callable] = None):
-    matcher = _ItemMatcher(item_hash=item_hash)
-    for item in dataset:
-        matcher.process_item(item)
-    return matcher.get_result()
-
-
-def match_classes(a: CategoriesInfo, b: CategoriesInfo):
-    a_label_cat = a.get(AnnotationType.label, LabelCategories())
-    b_label_cat = b.get(AnnotationType.label, LabelCategories())
-
-    a_labels = set(c.name for c in a_label_cat)
-    b_labels = set(c.name for c in b_label_cat)
-
-    matches = a_labels & b_labels
-    a_unmatched = a_labels - b_labels
-    b_unmatched = b_labels - a_labels
-    return matches, a_unmatched, b_unmatched
-
-
 @attrs
-class ExactComparator:
+class EqualityComparator:
     match_images: bool = attrib(kw_only=True, default=False)
     ignored_fields = attrib(kw_only=True, factory=set, validator=default_if_none(set))
     ignored_attrs = attrib(kw_only=True, factory=set, validator=default_if_none(set))
     ignored_item_attrs = attrib(kw_only=True, factory=set, validator=default_if_none(set))
+    all = attrib(kw_only=True, default=False)
 
     _test: TestCase = attrib(init=False)
     errors: list = attrib(init=False)
 
     def __attrs_post_init__(self):
         self._test = TestCase()
         self._test.maxDiff = None
@@ -610,27 +219,46 @@
             matched.append({"a_item": a_id, "b_item": b_id, "a": str(ann_a), "b": str(ann_b)})
 
         for ann_b in b_annotations:
             unmatched.append({"item": b_id, "source": "b", "ann": str(ann_b)})
 
         return matched, unmatched, errors
 
+    @staticmethod
+    def _print_output(output: dict):
+        print("Found:")
+        print("The first project has %s unmatched items" % len(output.get("a_extra_items", [])))
+        print("The second project has %s unmatched items" % len(output.get("b_extra_items", [])))
+        print("%s item conflicts" % len(output.get("errors", [])))
+        print("%s matching annotations" % len(output.get("matches", [])))
+        print("%s mismatching annotations" % len(output.get("mismatches", [])))
+
     def compare_datasets(self, a, b):
         self.errors = []
         errors = self.errors
 
         self._compare_categories(a.categories(), b.categories())
 
         matched = []
         unmatched = []
 
         matches, a_unmatched, b_unmatched = self._match_items(a, b)
 
         if a.categories().get(AnnotationType.label) != b.categories().get(AnnotationType.label):
-            return matched, unmatched, a_unmatched, b_unmatched, errors
+            output = {
+                "mismatches": unmatched,
+                "a_extra_items": sorted(a_unmatched),
+                "b_extra_items": sorted(b_unmatched),
+                "errors": errors,
+            }
+            if self.all:
+                output["matches"] = matched
+
+            self._print_output(output)
+            return output
 
         _dist = lambda s: len(s[1]) + len(s[2])
         for a_ids, b_ids in matches:
             # build distance matrix
             match_status = {}  # (a_id, b_id): [matched, unmatched, errors]
             a_matches = {a_id: None for a_id in a_ids}
             b_matches = {b_id: None for b_id in b_ids}
@@ -682,8 +310,362 @@
                 matched.extend(m[0])
                 unmatched.extend(m[1])
                 errors.extend(m[2])
 
             a_unmatched |= set(a_id for a_id, m in a_matches.items() if not m)
             b_unmatched |= set(b_id for b_id, m in b_matches.items() if not m)
 
-        return matched, unmatched, a_unmatched, b_unmatched, errors
+        output = {
+            "mismatches": unmatched,
+            "a_extra_items": sorted(a_unmatched),
+            "b_extra_items": sorted(b_unmatched),
+            "errors": errors,
+        }
+        if self.all:
+            output["matches"] = matched
+        self._print_output(output)
+        return output
+
+    @staticmethod
+    def save_compare_report(
+        output: Dict,
+        report_dir: str,
+    ) -> None:
+        """Saves the comparison report to JSON and text files.
+
+        Args:
+            output: A dictionary containing the comparison data.
+            report_dir: A string representing the directory to save the report files.
+        """
+        os.makedirs(report_dir, exist_ok=True)
+        output_file = osp.join(
+            report_dir,
+            generate_next_file_name("equality_compare", ext=".json", basedir=report_dir),
+        )
+
+        log.info(f"Saving compare json to {output_file}")
+        dump_json_file(output_file, output, indent=True)
+
+
+@attrs
+class TableComparator:
+    """
+    Class for comparing datasets and generating comparison report table.
+    """
+
+    @staticmethod
+    def _extract_labels(dataset: Dataset) -> Set[str]:
+        """Extracts labels from the dataset.
+
+        Args:
+            dataset: An instance of a Dataset class.
+
+        Returns:
+            A set of labels present in the dataset.
+        """
+        label_cat = dataset.categories().get(AnnotationType.label, LabelCategories())
+        return set(c.name for c in label_cat)
+
+    @staticmethod
+    def _compute_statistics(dataset: Dataset) -> Tuple[Dict, Dict]:
+        """Computes image and annotation statistics of the dataset.
+
+        Args:
+            dataset: An instance of a Dataset class.
+
+        Returns:
+            A tuple containing image statistics and annotation statistics.
+        """
+        image_stats = compute_image_statistics(dataset)
+        ann_stats = compute_ann_statistics(dataset)
+        return image_stats, ann_stats
+
+    def _analyze_dataset(self, dataset: Dataset) -> Tuple[str, Set[str], Dict, Dict]:
+        """Analyzes the dataset to get labels, format, and statistics.
+
+        Args:
+            dataset: An instance of a Dataset class.
+
+        Returns:
+            A tuple containing Dataset format, set of label names, image statistics,
+            and annotation statistics.
+        """
+        dataset_format = dataset.format
+        dataset_labels = self._extract_labels(dataset)
+        image_stats, ann_stats = self._compute_statistics(dataset)
+        return dataset_format, dataset_labels, image_stats, ann_stats
+
+    @staticmethod
+    def _create_table(headers: List[str], rows: List[List[str]]) -> str:
+        """Creates a table with the given headers and rows using the tabulate module.
+
+        Args:
+            headers: A list containing table headers.
+            rows: A list containing table rows.
+
+        Returns:
+            A string representation of the table.
+        """
+
+        def wrapfunc(item):
+            """Wrap a item consisted of text, returning a list of wrapped lines."""
+            max_len = 35
+            return "\n".join(wrap(item, max_len))
+
+        wrapped_rows = []
+        for row in rows:
+            new_row = [wrapfunc(item) for item in row]
+            wrapped_rows.append(new_row)
+
+        return tabulate(wrapped_rows, headers, tablefmt="grid")
+
+    @staticmethod
+    def _create_dict(rows: List[List[str]]) -> Dict[str, List[str]]:
+        """Creates a dictionary from the rows of the table.
+
+        Args:
+            rows: A list containing table rows.
+
+        Returns:
+            A dictionary where the key is the first element of a row and the value is
+            the rest of the row.
+        """
+        data_dict = {row[0]: row[1:] for row in rows[1:]}
+        return data_dict
+
+    def _create_high_level_comparison_table(
+        self, first_info: Tuple, second_info: Tuple
+    ) -> Tuple[str, Dict]:
+        """Generates a high-level comparison table.
+
+        Args:
+            first_info: A tuple containing information about the first dataset.
+            second_info: A tuple containing information about the second dataset.
+
+        Returns:
+            A tuple containing the table as a string and a dictionary representing the data
+            of the table.
+        """
+        first_format, first_labels, first_image_stats, first_ann_stats = first_info
+        second_format, second_labels, second_image_stats, second_ann_stats = second_info
+
+        headers = ["Field", "First", "Second"]
+
+        rows = [
+            ["Format", first_format, second_format],
+            ["Number of classes", str(len(first_labels)), str(len(second_labels))],
+            [
+                "Common classes",
+                ", ".join(sorted(list(first_labels.intersection(second_labels)))),
+                ", ".join(sorted(list(second_labels.intersection(first_labels)))),
+            ],
+            ["Classes", ", ".join(sorted(first_labels)), ", ".join(sorted(second_labels))],
+            [
+                "Images count",
+                str(first_image_stats["dataset"]["images count"]),
+                str(second_image_stats["dataset"]["images count"]),
+            ],
+            [
+                "Unique images count",
+                str(first_image_stats["dataset"]["unique images count"]),
+                str(second_image_stats["dataset"]["unique images count"]),
+            ],
+            [
+                "Repeated images count",
+                str(first_image_stats["dataset"]["repeated images count"]),
+                str(second_image_stats["dataset"]["repeated images count"]),
+            ],
+            [
+                "Annotations count",
+                str(first_ann_stats["annotations count"]),
+                str(second_ann_stats["annotations count"]),
+            ],
+            [
+                "Unannotated images count",
+                str(first_ann_stats["unannotated images count"]),
+                str(second_ann_stats["unannotated images count"]),
+            ],
+        ]
+
+        table = self._create_table(headers, rows)
+        data_dict = self._create_dict(rows)
+
+        return table, data_dict
+
+    def _create_mid_level_comparison_table(
+        self, first_info: Tuple, second_info: Tuple
+    ) -> Tuple[str, Dict]:
+        """Generates a mid-level comparison table.
+
+        Args:
+            first_info: A tuple containing information about the first dataset.
+            second_info: A tuple containing information about the second dataset.
+
+        Returns:
+            A tuple containing the table as a string and a dictionary representing the data
+            of the table.
+        """
+        _, _, first_image_stats, first_ann_stats = first_info
+        _, _, second_image_stats, second_ann_stats = second_info
+
+        headers = ["Field", "First", "Second"]
+
+        rows = []
+
+        first_subsets = sorted(list(first_image_stats["subsets"].keys()))
+        second_subsets = sorted(list(second_image_stats["subsets"].keys()))
+
+        subset_names = first_subsets.copy()
+        subset_names.extend(item for item in second_subsets if item not in first_subsets)
+
+        for subset_name in subset_names:
+            first_subset_data = first_image_stats["subsets"].get(subset_name, {})
+            second_subset_data = second_image_stats["subsets"].get(subset_name, {})
+            mean_str_first = (
+                ", ".join(f"{val:6.2f}" for val in first_subset_data.get("image mean", []))
+                if "image mean" in first_subset_data
+                else ""
+            )
+            std_str_first = (
+                ", ".join(f"{val:6.2f}" for val in first_subset_data.get("image std", []))
+                if "image std" in first_subset_data
+                else ""
+            )
+            mean_str_second = (
+                ", ".join(f"{val:6.2f}" for val in second_subset_data.get("image mean", []))
+                if "image mean" in second_subset_data
+                else ""
+            )
+            std_str_second = (
+                ", ".join(f"{val:6.2f}" for val in second_subset_data.get("image std", []))
+                if "image std" in second_subset_data
+                else ""
+            )
+            rows.append([f"{subset_name} - Image Mean", mean_str_first, mean_str_second])
+            rows.append([f"{subset_name} - Image Std", std_str_first, std_str_second])
+
+        first_labels = sorted(list(first_ann_stats["annotations"]["labels"]["distribution"].keys()))
+        second_labels = sorted(
+            list(second_ann_stats["annotations"]["labels"]["distribution"].keys())
+        )
+
+        label_names = first_labels.copy()
+        label_names.extend(item for item in second_labels if item not in first_labels)
+
+        for label_name in label_names:
+            count_dist_first = first_ann_stats["annotations"]["labels"]["distribution"].get(
+                label_name, [0, 0.0]
+            )
+            count_dist_second = second_ann_stats["annotations"]["labels"]["distribution"].get(
+                label_name, [0, 0.0]
+            )
+            count_first, dist_first = count_dist_first if count_dist_first[0] != 0 else ["", ""]
+            count_second, dist_second = count_dist_second if count_dist_second[0] != 0 else ["", ""]
+            rows.append(
+                [
+                    f"Label - {label_name}",
+                    f"imgs: {count_first}, percent: {dist_first:.4f}" if count_first != "" else "",
+                    f"imgs: {count_second}, percent: {dist_second:.4f}"
+                    if count_second != ""
+                    else "",
+                ]
+            )
+
+        table = self._create_table(headers, rows)
+        data_dict = self._create_dict(rows)
+
+        return table, data_dict
+
+    def _create_low_level_comparison_table(
+        self, first_dataset: Dataset, second_dataset: Dataset
+    ) -> Tuple[str, Dict]:
+        """Generates a low-level comparison table.
+
+        Args:
+            first_dataset: The first dataset to compare.
+            second_dataset: The second dataset to compare.
+
+        Returns:
+            A tuple containing the table as a string and a dictionary representing the data
+            of the table.
+        """
+        shift_analyzer = ShiftAnalyzer()
+        cov_shift = shift_analyzer.compute_covariate_shift([first_dataset, second_dataset])
+        label_shift = shift_analyzer.compute_label_shift([first_dataset, second_dataset])
+
+        headers = ["Field", "Value"]
+
+        rows = [
+            ["Covariate shift", str(cov_shift)],
+            ["Label shift", str(label_shift)],
+        ]
+
+        table = self._create_table(headers, rows)
+        data_dict = self._create_dict(rows)
+
+        return table, data_dict
+
+    def compare_datasets(self, first: Dataset, second: Dataset) -> Tuple[str, str, str, Dict]:
+        """Compares two datasets and generates comparison reports.
+
+        Args:
+            first: The first dataset to compare.
+            second: The second dataset to compare.
+
+        Returns:
+            A tuple containing high-level table, mid-level table, low-level table, and a
+            dictionary representation of the comparison.
+        """
+        first_info = self._analyze_dataset(first)
+        second_info = self._analyze_dataset(second)
+
+        high_level_table, high_level_dict = self._create_high_level_comparison_table(
+            first_info, second_info
+        )
+        mid_level_table, mid_level_dict = self._create_mid_level_comparison_table(
+            first_info, second_info
+        )
+        low_level_table, low_level_dict = self._create_low_level_comparison_table(first, second)
+
+        comparison_dict = dict(
+            high_level=high_level_dict, mid_level=mid_level_dict, low_level=low_level_dict
+        )
+
+        print(f"High-level comparison:\n{high_level_table}\n")
+        print(f"Mid-level comparison:\n{mid_level_table}\n")
+        print(f"Low-level comparison:\n{low_level_table}\n")
+
+        return high_level_table, mid_level_table, low_level_table, comparison_dict
+
+    @staticmethod
+    def save_compare_report(
+        high_level_table: str,
+        mid_level_table: str,
+        low_level_table: str,
+        comparison_dict: Dict,
+        report_dir: str,
+    ) -> None:
+        """Saves the comparison report to JSON and text files.
+
+        Args:
+            high_level_table: High-level comparison table as a string.
+            mid_level_table: Mid-level comparison table as a string.
+            low_level_table: Low-level comparison table as a string.
+            comparison_dict: A dictionary containing the comparison data.
+            report_dir: A string representing the directory to save the report files.
+        """
+        os.makedirs(report_dir, exist_ok=True)
+        json_output_file = osp.join(
+            report_dir, generate_next_file_name("table_compare", ext=".json", basedir=report_dir)
+        )
+        txt_output_file = osp.join(
+            report_dir, generate_next_file_name("table_compare", ext=".txt", basedir=report_dir)
+        )
+
+        log.info(f"Saving compare json to {json_output_file}")
+        log.info(f"Saving compare table to {txt_output_file}")
+
+        dump_json_file(json_output_file, comparison_dict, indent=True)
+        with open(txt_output_file, "w") as f:
+            f.write(f"High-level Comparison:\n{high_level_table}\n\n")
+            f.write(f"Mid-level Comparison:\n{mid_level_table}\n\n")
+            f.write(f"Low-level Comparison:\n{low_level_table}\n\n")
```

### Comparing `datumaro-1.3.2/datumaro/components/progress_reporting.py` & `datumaro-1.4.0rc1/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/project.py` & `datumaro-1.4.0rc1/src/datumaro/components/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1272,16 +1272,16 @@
 
 
 class DvcWrapper:
     @staticmethod
     def module():
         try:
             import dvc
+            import dvc.cli
             import dvc.env
-            import dvc.main
             import dvc.repo
 
             return dvc
         except ModuleNotFoundError as e:
             raise ModuleNotFoundError(
                 "Can't import the 'dvc' package. "
                 "Make sure DVC is installed, or install it with "
@@ -1334,24 +1334,18 @@
         if targets:
             if isinstance(targets, str):
                 args.append(targets)
             else:
                 args.extend(targets)
         self._exec(args)
 
-    def add(self, paths, dvc_path=None, no_commit=False, allow_external=False):
+    def add(self, paths, no_commit=False):
         args = ["add"]
-        if dvc_path:
-            args.append("--file")
-            args.append(dvc_path)
-            os.makedirs(osp.dirname(dvc_path), exist_ok=True)
         if no_commit:
             args.append("--no-commit")
-        if allow_external:
-            args.append("--external")
         if paths:
             if isinstance(paths, str):
                 args.append(paths)
             else:
                 args.extend(paths)
         self._exec(args)
 
@@ -1371,15 +1365,15 @@
                     return answer_on_input
 
                 es.enter_context(unittest.mock.patch("dvc.prompt.input", new=_input))
 
             log.debug("Calling DVC main with args: %s", args)
 
             logs = es.enter_context(catch_logs("dvc"))
-            retcode = self.module().main.main(args)
+            retcode = self.module().cli.main(args)
 
         logs = logs.getvalue()
         if retcode != 0:
             raise self.DvcError(logs)
         if not hide_output:
             print(logs)
         return logs
@@ -1396,15 +1390,15 @@
                     return False
 
         return True
 
     def obj_path(self, obj_hash, root=None):
         assert self.is_hash(obj_hash), obj_hash
         if not root:
-            root = osp.join(self._project_dir, ".dvc", "cache")
+            root = osp.join(self._project_dir, ".dvc", "cache", "files", "md5")
         return osp.join(root, obj_hash[:2], obj_hash[2:])
 
     def ignore(
         self,
         paths: Union[str, List[str]],
         mode: Union[None, str, IgnoreMode] = None,
         dvcignore: Optional[str] = None,
@@ -2059,17 +2053,15 @@
         else:
             raise UnexpectedUrlError(url)
         on_error_do(rmtree, data_dir, ignore_errors=True)
 
         log.debug("Done")
 
         if not no_hash:
-            obj_hash = self.compute_source_hash(
-                data_dir, dvcfile=dvcfile, no_cache=no_cache, allow_external=True
-            )
+            obj_hash = self.compute_source_hash(data_dir, dvcfile=dvcfile, no_cache=no_cache)
             if not no_cache:
                 log.debug("Data is added to DVC cache")
             log.debug("Data hash: '%s'", obj_hash)
         else:
             obj_hash = ""
 
         return obj_hash, dvcfile, data_dir
@@ -2083,21 +2075,25 @@
 
     @scoped
     def compute_source_hash(
         self,
         data_dir: str,
         dvcfile: Optional[str] = None,
         no_cache: bool = True,
-        allow_external: bool = True,
     ) -> ObjectId:
         if not dvcfile:
             tmp_dir = scope_add(self._make_tmp_dir())
             dvcfile = osp.join(tmp_dir, "source.dvc")
 
-        self._dvc.add(data_dir, dvc_path=dvcfile, no_commit=no_cache, allow_external=allow_external)
+        self._dvc.add(data_dir, no_commit=no_cache)
+
+        gen_dvcfile = osp.join(self._root_dir, data_dir + ".dvc")
+        if os.path.isfile(gen_dvcfile):
+            shutil.move(gen_dvcfile, dvcfile)
+
         obj_hash = self._get_source_hash(dvcfile)
         return obj_hash
 
     def refresh_source_hash(self, source: str, no_cache: bool = True) -> ObjectId:
         """
         Computes and updates the source hash in the working directory.
```

### Comparing `datumaro-1.3.2/datumaro/components/shift_analyzer.py` & `datumaro-1.4.0rc1/src/datumaro/components/shift_analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # ruff: noqa: E501
 
+import itertools
 from collections import defaultdict
 from typing import Dict, List, Optional
 
 import numpy as np
 import pyemd
 from scipy import linalg
 from scipy.stats import anderson_ksamp
 
+from datumaro.components.annotation import FeatureVector
 from datumaro.components.dataset import IDataset
-from datumaro.plugins.shift_analyzer import ShiftAnalyzerLauncher
+from datumaro.components.launcher import LauncherWithModelInterpreter
+from datumaro.plugins.openvino_plugin.shift_launcher import ShiftLauncher
 from datumaro.util import take_by
 
 
 class RunningStats1D:
     def __init__(self):
         self.running_mean = None
         self.running_sq_mean = None
         self.num: int = 0
 
-    def add(self, arr: np.ndarray) -> None:
+    def add(self, feats: List[FeatureVector]) -> None:
+        arr = np.stack([feat.vector for feat in feats], axis=0)
         assert arr.ndim == 2
 
         batch_size, _ = arr.shape
         mean = arr.mean(0)
         arr = np.expand_dims(arr, axis=-1)  # B x D x 1
         sq_mean = np.mean(np.matmul(arr, np.transpose(arr, axes=(0, 2, 1))), axis=0)  # D x D
 
@@ -54,55 +58,46 @@
     @property
     def cov(self) -> np.ndarray:
         mean = np.expand_dims(self.running_mean, axis=-1)  # D x 1
         return self.running_sq_mean - np.matmul(mean, mean.transpose())
 
 
 class FeatureAccumulator:
-    def __init__(self, model):
+    def __init__(self, model: LauncherWithModelInterpreter):
         self.model = model
         self._batch_size = 1
 
     def get_activation_stats(self, dataset: IDataset) -> RunningStats1D:
         running_stats = RunningStats1D()
 
         for batch in take_by(dataset, self._batch_size):
-            inputs = []
-            for item in batch:
-                inputs.append(np.atleast_3d(item.media.data))
-            inputs = np.array(inputs)
-            features = self.model.launch(inputs)
-            running_stats.add(features)
+            features = self.model.launch(batch)
+            running_stats.add(list(itertools.chain(*features)))
 
         return running_stats
 
 
 class FeatureAccumulatorByLabel(FeatureAccumulator):
     def __init__(self, model):
         super().__init__(model)
 
     def get_activation_stats(self, dataset: IDataset) -> Dict[int, RunningStats1D]:
-        running_stats: Dict[int, RunningStats1D] = {}
+        running_stats = defaultdict(RunningStats1D)
 
         for batch in take_by(dataset, self._batch_size):
             inputs, targets = [], []
             for item in batch:
                 for ann in item.annotations:
                     inputs.append(np.atleast_3d(item.media.data))
                     targets.append(ann.label)
 
-            inputs = np.array(inputs)
-            features = self.model.launch(inputs)
-
-            unique_indices = np.unique(targets)
-            for idx in unique_indices:
-                if idx not in running_stats:
-                    running_stats[idx] = RunningStats1D()
+            features = self.model.launch(batch)
 
-                running_stats[idx].add(features[targets == idx])
+            for feat, target in zip(features, targets):
+                running_stats[target].add(feat)
 
         return running_stats
 
 
 class ShiftAnalyzer:
     def __init__(self) -> None:
         """
@@ -111,17 +106,17 @@
         Parameters
         ----------
         dataset:
             Datumaro dataset to search similar dataitem.
         topk:
             Number of images.
         """
-        self._model = ShiftAnalyzerLauncher(
+        self._model = ShiftLauncher(
             model_name="googlenet-v4-tf",
-            output_layers="InceptionV4/Logits/PreLogitsFlatten/flatten_1/Reshape",
+            output_layers="InceptionV4/Logits/PreLogitsFlatten/flatten_1/Reshape:0",
         )
 
     def compute_covariate_shift(self, sources: List[IDataset], method: Optional[str] = "fid"):
         assert (
             len(sources) == 2
         ), "Shift analyzer should get two datasets to compute shifts between them."
```

### Comparing `datumaro-1.3.2/datumaro/components/validator.py` & `datumaro-1.4.0rc1/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/components/visualizer.py` & `datumaro-1.4.0rc1/src/datumaro/components/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,16 @@
     def get_random_items(self, n_samples: int) -> List[DatasetItem]:
         """Get random samples from the dataset"""
         if n_samples >= len(self.dataset):
             raise ValueError(
                 f"n_samples={n_samples} should be less than the dataset size ({len(self.dataset)})."
             )
 
-        return random.choices(self._items, k=n_samples)
+        # Disable B311: random - used for general random sampling not for security/crypto
+        return random.choices(self._items, k=n_samples)  # nosec B311
 
     @overload
     def vis_gallery(
         self,
         ids: List[str],
         ann_ids: List[int],
         subsets: Union[str, List[str]],
```

### Comparing `datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 import os.path as osp
 
 import yaml
 
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.launcher import Launcher
+from datumaro.components.lazy_plugin import extra_deps
 
 from .details.ac import GenericAcLauncher as _GenericAcLauncher
 
 
+@extra_deps("openvino.tools", "tensorflow")
 class AcLauncher(Launcher, CliPlugin):
     """
     Generic model launcher with Accuracy Checker backend.
     """
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
```

### Comparing `datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/brats.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/camvid.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
     Mask,
     MaskCategories,
 )
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import AnnotationExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import find, str_to_bool
 from datumaro.util.annotation_util import make_label_id_mapping
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cifar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
-import pickle  # nosec import_pickle
+import pickle  # nosec B403
 from collections import OrderedDict
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import cast
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
     Mask,
     MaskCategories,
 )
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import AnnotationExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import find
 from datumaro.util.annotation_util import make_label_id_mapping
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
             keep_original_ids=keep_original_category_ids,
         )
 
         if self._task == CocoTask.panoptic:
             self._mask_dir = osp.splitext(path)[0]
         self._items = self._load_items(json_data)
 
+        del json_data
+
     def __iter__(self):
         yield from self._items.values()
 
     def _load_categories(self, json_data, *, keep_original_ids):
         self._categories = {}
 
         if has_meta_file(self._rootpath):
@@ -221,18 +223,24 @@
                 joints=self._parse_field(cat, "skeleton", list),
             )
 
         self._categories[AnnotationType.points] = categories
 
     def _load_items(self, json_data):
         pbars = self._ctx.progress_reporter.split(2)
+
+        def _gen_ann(info_lists):
+            while info_lists:
+                yield info_lists.pop()
+
         items = {}
         img_infos = {}
+        img_lists = self._parse_field(json_data, "images", list)
         for img_info in pbars[0].iter(
-            self._parse_field(json_data, "images", list),
+            _gen_ann(img_lists),
             desc=f"Parsing image info in '{osp.basename(self._path)}'",
         ):
             img_id = None
             try:
                 img_id = self._parse_field(img_info, "id", int)
                 img_infos[img_id] = img_info
 
@@ -254,16 +262,17 @@
                     annotations=[],
                     attributes={"id": img_id},
                 )
             except Exception as e:
                 self._ctx.error_policy.report_item_error(e, item_id=(img_id, self._subset))
 
         if self._task is not CocoTask.panoptic:
+            ann_lists = self._parse_field(json_data, "annotations", list)
             for ann in pbars[1].iter(
-                self._parse_field(json_data, "annotations", list),
+                _gen_ann(ann_lists),
                 desc=f"Parsing annotations in '{osp.basename(self._path)}'",
             ):
                 img_id = None
                 try:
                     img_id = self._parse_field(ann, "image_id", int)
                     if img_id not in img_infos:
                         log.warn(f"Unknown image id '{img_id}'")
@@ -273,16 +282,17 @@
                         ann, img_infos[img_id], parsed_annotations=items[img_id].annotations
                     )
                 except Exception as e:
                     self._ctx.error_policy.report_annotation_error(
                         e, item_id=(img_id, self._subset)
                     )
         else:
+            ann_lists = self._parse_field(json_data, "annotations", list)
             for ann in pbars[1].iter(
-                self._parse_field(json_data, "annotations", list),
+                _gen_ann(ann_lists),
                 desc=f"Parsing annotations in '{osp.basename(self._path)}'",
             ):
                 img_id = None
                 try:
                     img_id = self._parse_field(ann, "image_id", int)
                     if img_id not in img_infos:
                         log.warn(f"Unknown image id '{img_id}'")
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from datumaro.components.annotation import (
     COORDINATE_ROUNDING_DIGITS,
     AnnotationType,
     Ellipse,
     Points,
     Polygon,
 )
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
 from datumaro.util import cast, dump_json_file, find, str_to_bool
 from datumaro.util.image import save_image
 
 from .format import CocoPath, CocoTask
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,33 +182,7 @@
     _TASK = CocoTask.panoptic
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
 class CocoStuffImporter(CocoImporter):
     _TASK = CocoTask.stuff
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
-
-
-class CocoRoboflowImporter(CocoImporter):
-    # Currently, All Roboflow exported COCO format can be handled by our Coco instances task implements.
-    _TASK = CocoTask.instances
-    _IMPORTER_TYPE = CocoImporterType.roboflow
-
-    @classmethod
-    def detect(
-        cls,
-        context: FormatDetectionContext,
-    ) -> FormatDetectionConfidence:
-        context.require_file("*/_annotations.coco.json")
-        return FormatDetectionConfidence.MEDIUM
-
-    @classmethod
-    def find_sources(cls, path):
-        subset_paths = glob(osp.join(path, "*", "_annotations.coco.json"), recursive=True)
-
-        subsets = {}
-        for subset_path in subset_paths:
-            subset_name = osp.basename(osp.dirname(subset_path))
-            osp.basename(subset_path)
-            subsets.setdefault(subset_name, {})[cls._TASK] = subset_path
-
-        return subsets
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from collections import OrderedDict
 from copy import deepcopy
 from typing import Optional
 
+import numpy as np
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Label,
     LabelCategories,
+    Mask,
     Points,
     Polygon,
     PolyLine,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
+from datumaro.util import mask_tools
 
 from .format import CvatPath
 
 
 def _find_meta_root(path: str):
     context = ElementTree.iterparse(path, events=("start", "end"))
     context = iter(context)
@@ -42,16 +45,14 @@
     if meta_root is None:
         raise DatasetImportError("CVAT XML file should have <meta> tag.")
 
     return meta_root, context
 
 
 class CvatBase(SubsetBase):
-    _SUPPORTED_SHAPES = ("box", "polygon", "polyline", "points")
-
     def __init__(
         self,
         path: str,
         *,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
     ):
@@ -99,15 +100,15 @@
                     image = {
                         "name": el.attrib.get("name"),
                         "frame": el.attrib["id"],
                         "width": el.attrib.get("width"),
                         "height": el.attrib.get("height"),
                     }
                     subset = el.attrib.get("subset")
-                elif el.tag in self._SUPPORTED_SHAPES and (track or image):
+                elif el.tag in CvatPath.SUPPORTED_IMPORT_SHAPES and (track or image):
                     attributes = {}
                     shape = {
                         "type": None,
                         "attributes": attributes,
                     }
                     if track:
                         shape.update(track)
@@ -130,15 +131,15 @@
                         attr_value = attr_value == "true"
                     elif attr_type is not None and attr_type != "text":
                         try:
                             attr_value = float(attr_value)
                         except ValueError:
                             pass
                     attributes[el.attrib["name"]] = attr_value
-                elif el.tag in self._SUPPORTED_SHAPES:
+                elif el.tag in CvatPath.SUPPORTED_IMPORT_SHAPES:
                     if track is not None:
                         shape["frame"] = el.attrib["frame"]
                         shape["outside"] = el.attrib.get("outside") == "1"
                         shape["keyframe"] = el.attrib.get("keyframe") == "1"
                     if image is not None:
                         shape["label"] = el.attrib.get("label")
                         shape["group"] = int(el.attrib.get("group_id", 0))
@@ -155,22 +156,30 @@
                                     el.attrib["xtl"],
                                     el.attrib["ytl"],
                                     el.attrib["xbr"],
                                     el.attrib["ybr"],
                                 ],
                             )
                         )
+                    elif el.tag == "mask":
+                        shape["rle"] = el.attrib["rle"]
+                        shape["left"] = el.attrib["left"]
+                        shape["top"] = el.attrib["top"]
+                        shape["width"] = el.attrib["width"]
+                        shape["height"] = el.attrib["height"]
                     else:
                         shape["points"] = []
                         for pair in el.attrib["points"].split(";"):
                             shape["points"].extend(map(float, pair.split(",")))
 
                     if subset is None or subset == self._subset:
                         frame_desc = items.get(shape["frame"], {"annotations": []})
-                        frame_desc["annotations"].append(self._parse_shape_ann(shape, categories))
+                        frame_desc["annotations"].append(
+                            self._parse_shape_ann(shape, categories, image)
+                        )
                         items[shape["frame"]] = frame_desc
                     shape = None
 
                 elif el.tag == "tag":
                     if subset is None or subset == self._subset:
                         frame_desc = items.get(tag["frame"], {"annotations": []})
                         frame_desc["annotations"].append(self._parse_tag_ann(tag, categories))
@@ -236,15 +245,15 @@
             for attr in attrs:
                 attribute_types[attr["name"]] = attr["input_type"]
 
         categories[AnnotationType.label] = label_cat
         return categories, frame_size, attribute_types
 
     @classmethod
-    def _parse_shape_ann(cls, ann, categories):
+    def _parse_shape_ann(cls, ann, categories, image):
         ann_id = ann.get("id", 0)
         ann_type = ann["type"]
 
         attributes = ann.get("attributes") or {}
         if "occluded" in categories[AnnotationType.label].attributes:
             attributes["occluded"] = ann.get("occluded", False)
         if "outside" in ann:
@@ -303,14 +312,43 @@
                 label=label_id,
                 z_order=z_order,
                 id=ann_id,
                 attributes=attributes,
                 group=group,
             )
 
+        elif ann_type == "mask":
+            rle = ann.get("rle")
+            mask_w, mask_h = int(ann.get("width")), int(ann.get("height"))
+            mask_l, mask_t = int(ann.get("left")), int(ann.get("top"))
+            img_w, img_h = int(image.get("width")), int(image.get("height"))
+
+            rle_uncompressed = {
+                "counts": np.array([int(str_num) for str_num in rle.split(",")], dtype=np.uint32),
+                "size": np.array([mask_w, mask_h]),
+            }
+
+            def _gen_mask():
+                # From the manual test for the dataset exported from the CVAT 2.5,
+                # the RLE encoding in the dataset has (W, H) binary 2D np.ndarray, not (H, W)
+                # Therefore, we need to tranpose it to make its shape as (H, W).
+                mask = mask_tools.rle_to_mask(rle_uncompressed).transpose()
+                canvas = np.zeros(shape=[img_h, img_w], dtype=np.uint8)
+                canvas[mask_t : mask_t + mask_h, mask_l : mask_l + mask_w] = mask
+                return canvas
+
+            return Mask(
+                image=_gen_mask,
+                label=label_id,
+                z_order=z_order,
+                id=ann_id,
+                attributes=attributes,
+                group=group,
+            )
+
         else:
             raise NotImplementedError("Unknown annotation type '%s'" % ann_type)
 
     @classmethod
     def _parse_tag_ann(cls, ann, categories):
         label = ann.get("label")
         label_id = categories[AnnotationType.label].find(label)[0]
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from collections import OrderedDict, defaultdict
 from itertools import chain
 
 # Disable B406: import_xml_sax - the library is used for writing
 from xml.sax.saxutils import XMLGenerator  # nosec
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
-from datumaro.util import cast, pairs
+from datumaro.util import cast, mask_tools, pairs
 
 from .format import CvatPath
 
 
 class XmlAnnotationWriter:
     VERSION = "1.1"
 
@@ -102,14 +102,19 @@
         self._level += 1
 
     def open_points(self, points):
         self._indent()
         self.xmlgen.startElement("points", points)
         self._level += 1
 
+    def open_mask(self, mask):
+        self._indent()
+        self.xmlgen.startElement("mask", mask)
+        self._level += 1
+
     def open_tag(self, tag):
         self._indent()
         self.xmlgen.startElement("tag", tag)
         self._level += 1
 
     def add_attribute(self, attribute):
         self._indent()
@@ -130,14 +135,17 @@
 
     def close_polyline(self):
         self._close_element("polyline")
 
     def close_points(self):
         self._close_element("points")
 
+    def close_mask(self):
+        self._close_element("mask")
+
     def close_tag(self):
         self._close_element("tag")
 
     def close_image(self):
         self._close_element("image")
 
     def close_track(self):
@@ -178,20 +186,15 @@
         label_name = self._get_label(track["label"]).name
         annotations = track["annotations"]
 
         track_info = {"id": str(track_id), "label": label_name}
 
         self._writer.open_track(track_info)
         for ann in annotations:
-            if ann.type in {
-                AnnotationType.points,
-                AnnotationType.polyline,
-                AnnotationType.polygon,
-                AnnotationType.bbox,
-            }:
+            if ann.type in CvatPath.SUPPORTED_EXPORT_SHAPES:
                 self._write_shape(ann, write_label_info=False, write_frame=True)
         self._writer.close_track()
 
     def _get_tracks(self):
         track_infos = defaultdict(lambda: defaultdict(list))
         for item in self._extractor:
             if "frame" not in item.attributes:
@@ -250,20 +253,15 @@
             if self._context._save_media:
                 self._context._save_image(item, osp.join(self._context._images_dir, filename))
         else:
             log.debug("Item '%s' has no image info", item.id)
         self._writer.open_image(image_info)
 
         for ann in item.annotations:
-            if ann.type in {
-                AnnotationType.points,
-                AnnotationType.polyline,
-                AnnotationType.polygon,
-                AnnotationType.bbox,
-            }:
+            if ann.type in CvatPath.SUPPORTED_EXPORT_SHAPES:
                 self._write_shape(ann, item)
             elif ann.type == AnnotationType.label:
                 self._write_tag(ann, item)
             else:
                 continue
 
         self._writer.close_image()
@@ -385,14 +383,30 @@
                         ("xtl", "{:.2f}".format(shape.points[0])),
                         ("ytl", "{:.2f}".format(shape.points[1])),
                         ("xbr", "{:.2f}".format(shape.points[2])),
                         ("ybr", "{:.2f}".format(shape.points[3])),
                     ]
                 )
             )
+        elif shape.type == AnnotationType.mask:
+            # From the manual test for the dataset exported from the CVAT 2.5,
+            # the RLE encoding in the dataset has (W, H) binary 2D np.ndarray, not (H, W)
+            # Therefore, we need to tranpose it to make its shape as (H, W).
+            mask = shape.image.transpose()
+            rle_uncompressed = mask_tools.mask_to_rle(mask)
+            width, height = mask.shape
+            shape_data.update(
+                OrderedDict(
+                    rle=", ".join([str(c) for c in rle_uncompressed["counts"]]),
+                    left=str(0),
+                    top=str(0),
+                    width=str(width),
+                    height=str(height),
+                )
+            )
         else:
             shape_data.update(
                 OrderedDict(
                     [
                         (
                             "points",
                             ";".join(
@@ -414,14 +428,16 @@
             self._writer.open_box(shape_data)
         elif shape.type == AnnotationType.polygon:
             self._writer.open_polygon(shape_data)
         elif shape.type == AnnotationType.polyline:
             self._writer.open_polyline(shape_data)
         elif shape.type == AnnotationType.points:
             self._writer.open_points(shape_data)
+        elif shape.type == AnnotationType.mask:
+            self._writer.open_mask(shape_data)
         else:
             raise NotImplementedError("unknown shape type")
 
         if write_label_info:
             for attr_name, attr_value in shape.attributes.items():
                 if attr_name in self._context._builtin_attrs:
                     continue
@@ -452,14 +468,16 @@
             self._writer.close_box()
         elif shape.type == AnnotationType.polygon:
             self._writer.close_polygon()
         elif shape.type == AnnotationType.polyline:
             self._writer.close_polyline()
         elif shape.type == AnnotationType.points:
             self._writer.close_points()
+        elif shape.type == AnnotationType.mask:
+            self._writer.close_mask()
         else:
             raise NotImplementedError("unknown shape type")
 
     def _write_tag(self, label, item):
         if label.label is None:
             log.warning("Item %s: skipping a %s with no label", item.id, label.type.name)
             return
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,17 @@
             categories[AnnotationType.points] = point_categories
 
         return categories
 
     def _load_items(self, parsed):
         items = []
 
-        for item_desc in parsed["items"]:
+        item_descs = parsed["items"]
+        while item_descs:
+            item_desc = item_descs.pop()
             item_id = item_desc["id"]
 
             media = None
             image_info = item_desc.get("image")
             if image_info:
                 image_filename = image_info.get("path") or item_id + DatumaroPath.IMAGE_EXT
                 image_path = osp.join(self._images_dir, self._subset, image_filename)
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     PointsCategories,
     Polygon,
     PolyLine,
     RleMask,
     _Shape,
 )
 from datumaro.components.crypter import NULL_CRYPTER
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetItem
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.exporter import ExportContextComponent, Exporter
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util import cast, dump_json_file
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import os.path as osp
 from copy import deepcopy
 
 # Disable B406: import_xml_sax - the library is used for writing
 from xml.sax.saxutils import XMLGenerator  # nosec
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import DatasetExportError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import PointCloud
 from datumaro.util import cast
 from datumaro.util.image import find_images
 
 from .format import KittiRawPath, OcclusionStates, PoseStates, TruncationStates
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/labelme.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import cast, escape, unescape
 from datumaro.util.image import save_image
 from datumaro.util.mask_tools import find_mask_bbox, load_mask
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
-from datumaro.util.os_util import split_path
 
 
 class LabelMePath:
+    IMAGES_DIR = "Images"
+    ANNOTATIONS_DIR = "Annotations"
     MASKS_DIR = "Masks"
     IMAGE_EXT = ".jpg"
 
     ATTR_IMPORT_ESCAPES = [
         ("\\=", r"%%{eq}%%"),
         ('\\"', r"%%{doublequote}%%"),
         ("\\,", r"%%{comma}%%"),
@@ -49,55 +50,48 @@
     def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         assert osp.isdir(path), path
         super().__init__(ctx=ctx)
 
         self._items, self._categories, self._subsets = self._parse(path)
         self._length = len(self._items)
 
-    def _parse(self, dataset_root):
+    def _parse(self, path):
         items = []
         subsets = set()
 
-        if has_meta_file(dataset_root):
+        if has_meta_file(path):
             categories = {
                 AnnotationType.label: LabelCategories(
                     attributes={"occluded", "username"}
-                ).from_iterable(parse_meta_file(dataset_root).keys())
+                ).from_iterable(parse_meta_file(path).keys())
             }
         else:
             categories = {
                 AnnotationType.label: LabelCategories(attributes={"occluded", "username"})
             }
 
-        for xml_path in sorted(glob(osp.join(dataset_root, "**", "*.xml"), recursive=True)):
-            item_path = osp.relpath(xml_path, dataset_root)
-            path_parts = split_path(item_path)
-            subset = ""
-            if 1 < len(path_parts):
-                subset = path_parts[0]
-                item_path = osp.join(*path_parts[1:])  # pylint: disable=no-value-for-parameter
-
+        for xml_path in sorted(glob(osp.join(path, "**", "*.xml"), recursive=True)):
             root = ElementTree.parse(xml_path)
 
-            item_id = (
-                osp.join(root.find("folder").text or "", root.find("filename").text) or item_path
-            )
-            image_path = osp.join(osp.dirname(xml_path), osp.basename(item_id))
-            item_id = osp.splitext(item_id)[0]
+            subset = root.find("folder").text or ""
+            item_id = osp.splitext(root.find("filename").text)[0]
+            image_path = osp.join(path, "Images", subset, root.find("filename").text)
 
             image_size = None
             imagesize_elem = root.find("imagesize")
             if imagesize_elem is not None:
-                width_elem = imagesize_elem.find("ncols")
-                height_elem = imagesize_elem.find("nrows")
-                image_size = (int(height_elem.text), int(width_elem.text))
+                width_elem = imagesize_elem.find("ncols").text
+                height_elem = imagesize_elem.find("nrows").text
+                image_size = (
+                    (int(height_elem), int(width_elem)) if height_elem and width_elem else None
+                )
 
             image = Image.from_file(path=image_path, size=image_size)
 
-            annotations = self._parse_annotations(root, osp.join(dataset_root, subset), categories)
+            annotations = self._parse_annotations(root, path, subset, categories)
 
             items.append(
                 DatasetItem(id=item_id, subset=subset, media=image, annotations=annotations)
             )
             subsets.add(items[-1].subset)
         return items, categories, subsets
 
@@ -108,15 +102,15 @@
     @staticmethod
     def _unescape(s):
         s = unescape(s, LabelMePath.ATTR_IMPORT_ESCAPES)
         s = unescape(s, LabelMePath.ATTR_EXPORT_ESCAPES)
         return s
 
     @classmethod
-    def _parse_annotations(cls, xml_root, subset_root, categories):
+    def _parse_annotations(cls, xml_root, path, subset, categories):
         def _parse_attributes(attr_str):
             parsed = []
             if not attr_str:
                 return parsed
 
             for attr in [a.strip() for a in cls._escape(attr_str).split(",")]:
                 if not attr:
@@ -226,15 +220,15 @@
             elif segm_elem is not None:
                 user_elem = segm_elem.find("username")
                 if user_elem is not None and user_elem.text:
                     user = user_elem.text
                 attributes.append(("username", user))
 
                 mask_path = osp.join(
-                    subset_root, LabelMePath.MASKS_DIR, segm_elem.find("mask").text
+                    path, LabelMePath.MASKS_DIR, subset, segm_elem.find("mask").text
                 )
                 if not osp.isfile(mask_path):
                     raise FileNotFoundError(errno.ENOENT, "Can't find mask", mask_path)
                 mask = load_mask(mask_path)
                 mask = np.any(mask, axis=2)
                 ann_items.append(Mask(image=mask, label=label, id=obj_id, attributes=attributes))
 
@@ -368,19 +362,16 @@
 
         os.makedirs(self._save_dir, exist_ok=True)
 
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
 
         for subset_name, subset in self._extractor.subsets().items():
-            subset_dir = osp.join(self._save_dir, subset_name)
-            os.makedirs(subset_dir, exist_ok=True)
-
             for item in subset:
-                self._save_item(item, subset_dir)
+                self._save_item(item, subset_name)
 
     def _get_label(self, label_id):
         if label_id is None:
             return ""
         return self._extractor.categories()[AnnotationType.label][label_id].name
 
     @staticmethod
@@ -392,21 +383,23 @@
         from lxml import etree as ET  # nosec
 
         log.debug("Converting item '%s'", item.id)
 
         image_filename = self._make_image_filename(item)
         if self._save_media:
             if item.media and item.media.has_data:
-                self._save_image(item, osp.join(subset_dir, image_filename))
+                image_dir = osp.join(self._save_dir, LabelMePath.IMAGES_DIR, subset_dir)
+                os.makedirs(image_dir, exist_ok=True)
+                self._save_image(item, osp.join(image_dir, image_filename))
             else:
                 log.debug("Item '%s' has no image", item.id)
 
         root_elem = ET.Element("annotation")
-        ET.SubElement(root_elem, "filename").text = osp.basename(image_filename)
-        ET.SubElement(root_elem, "folder").text = osp.dirname(image_filename)
+        ET.SubElement(root_elem, "filename").text = image_filename
+        ET.SubElement(root_elem, "folder").text = subset_dir
 
         source_elem = ET.SubElement(root_elem, "source")
         ET.SubElement(source_elem, "sourceImage").text = ""
         ET.SubElement(source_elem, "sourceAnnotation").text = "Datumaro"
 
         if item.media:
             image_elem = ET.SubElement(root_elem, "imagesize")
@@ -457,15 +450,15 @@
                     ET.SubElement(point_elem, "x").text = "%.2f" % x
                     ET.SubElement(point_elem, "y").text = "%.2f" % y
 
                 ET.SubElement(poly_elem, "username").text = str(ann.attributes.get("username", ""))
             elif ann.type == AnnotationType.mask:
                 mask_filename = "%s_mask_%s.png" % (item.id, obj_id)
                 save_image(
-                    osp.join(subset_dir, LabelMePath.MASKS_DIR, mask_filename),
+                    osp.join(self._save_dir, LabelMePath.MASKS_DIR, subset_dir, mask_filename),
                     self._paint_mask(ann.image),
                     create_dir=True,
                 )
 
                 segm_elem = ET.SubElement(obj_elem, "segm")
                 ET.SubElement(segm_elem, "mask").text = mask_filename
 
@@ -505,18 +498,19 @@
             ET.SubElement(leader_parts_elem, "hasparts").text = ",".join(leader_parts)
             ET.SubElement(leader_parts_elem, "ispartof").text = ""
 
             for obj_id, parts_elem in group[1:]:
                 ET.SubElement(parts_elem, "hasparts").text = ""
                 ET.SubElement(parts_elem, "ispartof").text = str(leader_id)
 
-        os.makedirs(osp.join(subset_dir, osp.dirname(image_filename)), exist_ok=True)
-        xml_path = osp.join(subset_dir, osp.splitext(image_filename)[0] + ".xml")
+        ann_path = osp.join(self._save_dir, LabelMePath.ANNOTATIONS_DIR, subset_dir)
+        os.makedirs(osp.join(ann_path, osp.dirname(image_filename)), exist_ok=True)
+        xml_path = osp.join(ann_path, osp.splitext(image_filename)[0] + ".xml")
         if osp.exists(xml_path):
-            xml_path = osp.join(subset_dir, image_filename + ".xml")
+            xml_path = osp.join(ann_path, image_filename + ".xml")
         with open(xml_path, "w", encoding="utf-8") as f:
             xml_data = ET.tostring(root_elem, encoding="unicode", pretty_print=True)
             f.write(xml_data)
 
     @staticmethod
     def _paint_mask(mask):
         # TODO: check if mask colors are random
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mars.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mot.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mots.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/open_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from typing import Optional, Union
 
 import cv2
 import numpy as np
 from attr import attrs
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Mask
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import (
     DatasetError,
     MediaTypeError,
     RepeatedItemError,
     UndefinedLabel,
 )
 from datumaro.components.exporter import Exporter
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import os
 import os.path as osp
 import shutil
 import uuid
 from datetime import datetime
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, IDataset
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import DatasetExportError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import PointCloud
 from datumaro.util import cast, dump_json_file
 
 from .format import PointCloudPath
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import os
 import os.path as osp
 import re
 from collections import OrderedDict
 from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.importer import ImportContext, Importer
+from datumaro.components.lazy_plugin import extra_deps
 from datumaro.components.media import Image
 from datumaro.util.image import decode_image, lazy_image
 from datumaro.util.tf_util import import_tf as _import_tf
 
-from .format import DetectionApiPath
+from .format import DetectionApiPath, TfrecordImporterType
 
 tf = _import_tf()
 
 
 def clamp(value, _min, _max):
     return max(min(_max, value), _min)
 
 
+@extra_deps("tensorflow")
 class TfDetectionApiBase(SubsetBase):
     def __init__(
         self,
         path: str,
         *,
+        tfrecord_importer_type: TfrecordImporterType = TfrecordImporterType.default,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
     ):
         assert osp.isfile(path), path
         images_dir = ""
         root_dir = osp.dirname(osp.abspath(path))
         if osp.basename(root_dir) == DetectionApiPath.ANNOTATIONS_DIR:
@@ -42,27 +46,48 @@
             if not osp.isdir(images_dir):
                 images_dir = ""
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
         super().__init__(subset=subset, ctx=ctx)
 
+        self._features = {
+            "image/filename": tf.io.FixedLenFeature([], tf.string),
+            "image/source_id": tf.io.FixedLenFeature([], tf.string),
+            "image/height": tf.io.FixedLenFeature([], tf.int64),
+            "image/width": tf.io.FixedLenFeature([], tf.int64),
+            "image/encoded": tf.io.FixedLenFeature([], tf.string),
+            "image/format": tf.io.FixedLenFeature([], tf.string),
+            # use varlen to avoid errors when this field is missing
+            "image/key/sha256": tf.io.VarLenFeature(tf.string),
+            # Object boxes and classes.
+            "image/object/bbox/xmin": tf.io.VarLenFeature(tf.float32),
+            "image/object/bbox/xmax": tf.io.VarLenFeature(tf.float32),
+            "image/object/bbox/ymin": tf.io.VarLenFeature(tf.float32),
+            "image/object/bbox/ymax": tf.io.VarLenFeature(tf.float32),
+            "image/object/class/label": tf.io.VarLenFeature(tf.int64),
+            "image/object/class/text": tf.io.VarLenFeature(tf.string),
+            "image/object/mask": tf.io.VarLenFeature(tf.string),
+        }
+        if tfrecord_importer_type == TfrecordImporterType.roboflow:
+            del self._features["image/source_id"]
+
         items, labels = self._parse_tfrecord_file(path, self._subset, images_dir)
         self._items = items
         self._categories = self._load_categories(labels)
 
     @staticmethod
     def _load_categories(labels):
         label_categories = LabelCategories().from_iterable(
             e[0] for e in sorted(labels.items(), key=lambda item: item[1])
         )
         return {AnnotationType.label: label_categories}
 
-    @classmethod
-    def _parse_labelmap(cls, text):
+    @staticmethod
+    def _parse_labelmap(text):
         id_pattern = r"(?:id\s*:\s*(?P<id>\d+))"
         name_pattern = r"(?:name\s*:\s*[\'\"](?P<name>.*?)[\'\"])"
         entry_pattern = r"(\{(?:[\s\n]*(?:%(id)s|%(name)s)[\s\n]*){2}\})+" % {
             "id": id_pattern,
             "name": name_pattern,
         }
         matches = re.finditer(entry_pattern, text)
@@ -72,53 +97,40 @@
             label_id = match.group("id")
             label_name = match.group("name")
             if label_id is not None and label_name is not None:
                 labelmap[label_name] = int(label_id)
 
         return labelmap
 
-    @classmethod
-    def _parse_tfrecord_file(cls, filepath, subset, images_dir):
+    def _parse_tfrecord_file(self, filepath, subset, images_dir):
         dataset = tf.data.TFRecordDataset(filepath)
-        features = {
-            "image/filename": tf.io.FixedLenFeature([], tf.string),
-            "image/source_id": tf.io.FixedLenFeature([], tf.string),
-            "image/height": tf.io.FixedLenFeature([], tf.int64),
-            "image/width": tf.io.FixedLenFeature([], tf.int64),
-            "image/encoded": tf.io.FixedLenFeature([], tf.string),
-            "image/format": tf.io.FixedLenFeature([], tf.string),
-            # use varlen to avoid errors when this field is missing
-            "image/key/sha256": tf.io.VarLenFeature(tf.string),
-            # Object boxes and classes.
-            "image/object/bbox/xmin": tf.io.VarLenFeature(tf.float32),
-            "image/object/bbox/xmax": tf.io.VarLenFeature(tf.float32),
-            "image/object/bbox/ymin": tf.io.VarLenFeature(tf.float32),
-            "image/object/bbox/ymax": tf.io.VarLenFeature(tf.float32),
-            "image/object/class/label": tf.io.VarLenFeature(tf.int64),
-            "image/object/class/text": tf.io.VarLenFeature(tf.string),
-            "image/object/mask": tf.io.VarLenFeature(tf.string),
-        }
+
+        files = os.listdir(osp.dirname(filepath))
+        for filename in files:
+            if DetectionApiPath.LABELMAP_FILE in filename:
+                labelmap_path = osp.join(osp.dirname(filepath), filename)
+                break
 
         dataset_labels = OrderedDict()
-        labelmap_path = osp.join(osp.dirname(filepath), DetectionApiPath.LABELMAP_FILE)
         if osp.exists(labelmap_path):
             with open(labelmap_path, "r", encoding="utf-8") as f:
                 labelmap_text = f.read()
             dataset_labels.update(
-                {label: id - 1 for label, id in cls._parse_labelmap(labelmap_text).items()}
+                {label: id - 1 for label, id in self._parse_labelmap(labelmap_text).items()}
             )
 
         dataset_items = []
 
         for record in dataset:
-            parsed_record = tf.io.parse_single_example(record, features)
-            frame_id = parsed_record["image/source_id"].numpy().decode("utf-8")
-            frame_filename = parsed_record["image/filename"].numpy().decode("utf-8")
-            frame_height = tf.cast(parsed_record["image/height"], tf.int64).numpy().item()
-            frame_width = tf.cast(parsed_record["image/width"], tf.int64).numpy().item()
+            parsed_record = tf.io.parse_single_example(record, self._features)
+            frame_id = parsed_record.get("image/source_id", None)
+            frame_id = frame_id.numpy().decode("utf-8") if frame_id else frame_id
+            frame_filename = parsed_record.get("image/filename", None).numpy().decode("utf-8")
+            frame_height = tf.cast(parsed_record.get("image/height", 0), tf.int64).numpy().item()
+            frame_width = tf.cast(parsed_record.get("image/width", 0), tf.int64).numpy().item()
             frame_image = parsed_record["image/encoded"].numpy()
             xmins = tf.sparse.to_dense(parsed_record["image/object/bbox/xmin"]).numpy()
             ymins = tf.sparse.to_dense(parsed_record["image/object/bbox/ymin"]).numpy()
             xmaxs = tf.sparse.to_dense(parsed_record["image/object/bbox/xmax"]).numpy()
             ymaxs = tf.sparse.to_dense(parsed_record["image/object/bbox/ymax"]).numpy()
             label_ids = tf.sparse.to_dense(parsed_record["image/object/class/label"]).numpy()
             labels = tf.sparse.to_dense(
@@ -181,11 +193,12 @@
                     attributes={"source_id": frame_id},
                 )
             )
 
         return dataset_items, dataset_labels
 
 
+@extra_deps("tensorflow")
 class TfDetectionApiImporter(Importer):
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".tfrecord", "tf_detection_api")
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import os.path as osp
 import string
 from collections import OrderedDict
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.errors import DatasetExportError
 from datumaro.components.exporter import Exporter
+from datumaro.components.lazy_plugin import extra_deps
 from datumaro.components.media import ByteImage, Image, ImageFromBytes
 from datumaro.util.annotation_util import find_group_leader, find_instances, max_bbox
 from datumaro.util.image import encode_image
 from datumaro.util.mask_tools import merge_masks
 from datumaro.util.tf_util import import_tf as _import_tf
 
 from .format import DetectionApiPath
@@ -48,14 +49,15 @@
     return tf.train.Feature(bytes_list=tf.train.BytesList(value=value))
 
 
 def float_list_feature(value):
     return tf.train.Feature(float_list=tf.train.FloatList(value=value))
 
 
+@extra_deps("tensorflow")
 class TfDetectionApiExporter(Exporter):
     DEFAULT_IMAGE_EXT = DetectionApiPath.DEFAULT_IMAGE_EXT
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument(
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/video.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.mask_tools import invert_colormap, lazy_mask
 from datumaro.util.meta_file_util import has_meta_file
 
 from .format import (
+    VocImporterType,
     VocInstColormap,
     VocPath,
     VocTask,
     make_voc_categories,
     parse_label_map,
     parse_meta_file,
 )
@@ -48,29 +49,39 @@
 class VocBase(SubsetBase):
     def __init__(
         self,
         path: str,
         task: Optional[VocTask] = VocTask.voc,
         *,
         subset: Optional[str] = None,
+        voc_importer_type: VocImporterType = VocImporterType.default,
         ctx: Optional[ImportContext] = None,
     ):
-        if not osp.isfile(path):
-            raise DatasetImportError(f"Can't find txt subset list file at '{path}'")
-        self._path = path
-        self._dataset_dir = osp.dirname(osp.dirname(osp.dirname(path)))
-
-        self._task = task
-
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
 
         super().__init__(subset=subset, ctx=ctx)
 
-        self._categories = self._load_categories(self._dataset_dir)
+        if voc_importer_type == VocImporterType.default:
+            dataset_dir = osp.dirname(osp.dirname(osp.dirname(path)))
+            self._image_dir = osp.join(dataset_dir, VocPath.IMAGES_DIR)
+            self._anno_dir = osp.join(dataset_dir, VocPath.ANNOTATIONS_DIR)
+            self._mask_dir = osp.join(dataset_dir, VocPath.SEGMENTATION_DIR)
+            self._inst_dir = osp.join(dataset_dir, VocPath.INSTANCES_DIR)
+        elif voc_importer_type == VocImporterType.roboflow:
+            dataset_dir = path
+            self._image_dir = dataset_dir
+            self._anno_dir = dataset_dir
+        else:
+            raise DatasetImportError(f"Not supported type: {voc_importer_type}")
+
+        self._path = path
+        self._task = task
+
+        self._categories = self._load_categories(dataset_dir)
 
         if self._task in [VocTask.voc, VocTask.voc_segmentation, VocTask.voc_instance_segmentation]:
             label_color = lambda label_idx: self._categories[AnnotationType.mask].colormap.get(
                 label_idx, None
             )
             log.debug(
                 "Loaded labels: %s",
@@ -98,14 +109,17 @@
             label_map_path = osp.join(dataset_path, VocPath.LABELMAP_FILE)
             if osp.isfile(label_map_path):
                 label_map = parse_label_map(label_map_path)
 
         return make_voc_categories(label_map, self._task)
 
     def _load_subset_list(self, subset_path):
+        if not osp.isfile(subset_path):
+            raise DatasetImportError(f"Can't find txt subset list file at '{subset_path}'")
+
         subset_list = []
         with open(subset_path, encoding="utf-8") as f:
             for i, line in enumerate(f):
                 line = line.strip()
                 if not line or line[0] == "#":
                     continue
 
@@ -123,40 +137,37 @@
                         line = line.split()[0]
                 else:
                     line = line.strip()
                 subset_list.append(line)
             return subset_list
 
     def __iter__(self):
-        image_dir = osp.join(self._dataset_dir, VocPath.IMAGES_DIR)
-        if osp.isdir(image_dir):
+        if osp.isdir(self._image_dir):
             images = {
-                osp.splitext(osp.relpath(p, image_dir))[0].replace("\\", "/"): p
-                for p in find_images(image_dir, recursive=True)
+                osp.splitext(osp.relpath(p, self._image_dir))[0].replace("\\", "/"): p
+                for p in find_images(self._image_dir, recursive=True)
             }
         else:
             images = {}
 
         annotations = (
             self._parse_labels() if self._task in [VocTask.voc, VocTask.voc_classification] else {}
         )
 
-        anno_dir = osp.join(self._dataset_dir, VocPath.ANNOTATIONS_DIR)
-
         for item_id in self._ctx.progress_reporter.iter(
             self._items, desc=f"Parsing boxes in '{self._subset}'"
         ):
             log.debug("Reading item '%s'" % item_id)
             size = None
 
             try:
                 anns = annotations.get(item_id, [])
                 image = None
 
-                ann_file = osp.join(anno_dir, item_id + ".xml")
+                ann_file = osp.join(self._anno_dir, item_id + ".xml")
                 if osp.isfile(ann_file) and self._task not in [
                     VocTask.voc_classification,
                     VocTask.voc_segmentation,
                 ]:
                     root_elem = ElementTree.parse(ann_file).getroot()
                     if root_elem.tag != "annotation":
                         raise MissingFieldError("annotation")
@@ -164,15 +175,15 @@
                     height = self._parse_field(root_elem, "size/height", int, required=False)
                     width = self._parse_field(root_elem, "size/width", int, required=False)
                     if height and width:
                         size = (height, width)
 
                     filename_elem = root_elem.find("filename")
                     if filename_elem is not None:
-                        image = osp.join(image_dir, filename_elem.text)
+                        image = osp.join(self._image_dir, filename_elem.text)
 
                     anns += self._parse_annotations(root_elem, item_id=(item_id, self._subset))
 
                 if self._task in [
                     VocTask.voc,
                     VocTask.voc_segmentation,
                     VocTask.voc_instance_segmentation,
@@ -317,23 +328,21 @@
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
 
     def _parse_masks(self, item_id):
         item_annotations = []
 
         class_mask = None
-        segm_path = osp.join(
-            self._dataset_dir, VocPath.SEGMENTATION_DIR, item_id + VocPath.SEGM_EXT
-        )
+        segm_path = osp.join(self._mask_dir, item_id + VocPath.SEGM_EXT)
         if osp.isfile(segm_path):
             inverse_cls_colormap = self._categories[AnnotationType.mask].inverse_colormap
             class_mask = lazy_mask(segm_path, inverse_cls_colormap)
 
         instances_mask = None
-        inst_path = osp.join(self._dataset_dir, VocPath.INSTANCES_DIR, item_id + VocPath.SEGM_EXT)
+        inst_path = osp.join(self._inst_dir, item_id + VocPath.SEGM_EXT)
         if osp.isfile(inst_path):
             instances_mask = lazy_mask(inst_path, _inverse_inst_colormap)
 
         label_cat = self._categories[AnnotationType.label]
 
         if instances_mask is not None:
             compiled_mask = CompiledMask(class_mask, instances_mask)
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     AnnotationType,
     Bbox,
     CompiledMask,
     Label,
     LabelCategories,
     Mask,
 )
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import DatasetExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
 from datumaro.util import find, str_to_bool
 from datumaro.util.annotation_util import make_label_id_mapping
 from datumaro.util.image import save_image
 from datumaro.util.mask_tools import paint_mask, remap_mask
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 
 VocColormap: Colormap = {
     id: color for id, color in generate_colormap(256).items() if id in {l.value for l in VocLabel}
 }
 VocInstColormap = generate_colormap(256)
 
 
+class VocImporterType(Enum):
+    default = auto()
+    roboflow = auto()
+
+
 class VocPath:
     IMAGES_DIR = "JPEGImages"
     ANNOTATIONS_DIR = "Annotations"
     SEGMENTATION_DIR = "SegmentationClass"
     INSTANCES_DIR = "SegmentationObject"
     SUBSETS_DIR = "ImageSets"
     IMAGE_EXT = ".jpg"
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,21 +196,21 @@
             except Exception as e:
                 self._ctx.error_policy.report_item_error(e, item_id=(item_id, subset_name))
                 subset.items.pop(item_id)
                 item = None
 
         return item
 
-    @staticmethod
-    def _parse_field(value: str, cls: Type[T], field_name: str) -> T:
+    @classmethod
+    def _parse_field(cls, value: str, desired_type: Type[T], field_name: str) -> T:
         try:
-            return cls(value)
+            return desired_type(value)
         except Exception as e:
             raise InvalidAnnotationError(
-                f"Can't parse {field_name} from '{value}'. Expected {cls}"
+                f"Can't parse {field_name} from '{value}'. Expected {desired_type}"
             ) from e
 
     @classmethod
     def _parse_annotations(
         cls,
         anno_path: str,
         image: ImageFromFile,
@@ -230,15 +230,15 @@
             # Use image info as late as possible to avoid unnecessary image loading
             if image.size is None:
                 raise DatasetImportError(
                     f"Can't find image info for '{cls.localize_path(image.path)}'"
                 )
             image_height, image_width = image.size
 
-        for line in lines:
+        for idx, line in enumerate(lines):
             parts = line.split()
             if len(parts) != 5:
                 raise InvalidAnnotationError(
                     f"Unexpected field count {len(parts)} in the bbox description. "
                     "Expected 5 fields (label, xc, yc, w, h)."
                 )
             label_id, xc, yc, w, h = parts
@@ -254,14 +254,16 @@
             annotations.append(
                 Bbox(
                     x * image_width,
                     y * image_height,
                     w * image_width,
                     h * image_height,
                     label=label_id,
+                    id=idx,
+                    group=idx,
                 )
             )
 
         return annotations
 
     @staticmethod
     def _load_categories(names_path):
@@ -305,51 +307,67 @@
         ctx: Optional[ImportContext] = None,
     ) -> None:
         super().__init__(subset=subset, ctx=ctx)
 
         if not osp.isdir(config_path):
             raise DatasetImportError(f"{config_path} should be a directory.")
 
-        rootpath = config_path
-        self._path = rootpath
+        rootpath = self._get_rootpath(config_path)
 
         self._image_info = YoloStrictBase.parse_image_info(rootpath, image_info)
 
         # Init label categories
         label_categories = self._load_categories(osp.join(rootpath, self.META_FILE))
         self._categories = {AnnotationType.label: label_categories}
 
-        # Parse dataset items
-        def _get_fname(fpath: str) -> str:
-            return osp.splitext(osp.basename(fpath))[0]
-
-        img_files = {
-            _get_fname(img_file): img_file
-            for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
-            if extract_subset_name_from_parent(img_file, rootpath) == self._subset
-        }
+        img_files = self._load_img_files(rootpath)
 
         for url in urls:
             try:
-                fname = _get_fname(url)
+                fname = self._get_fname(url)
                 img = Image.from_file(path=img_files[fname])
-                anns = YoloStrictBase._parse_annotations(
+                anns = self._parse_annotations(
                     url,
                     img,
                     label_categories=label_categories,
                 )
                 self._items.append(
                     DatasetItem(id=fname, subset=self._subset, media=img, annotations=anns)
                 )
             except Exception as e:
                 self._ctx.error_policy.report_item_error(e, item_id=(fname, self._subset))
 
+    def _get_rootpath(self, config_path: str) -> str:
+        return config_path
+
     def _load_categories(self, names_path: str) -> LabelCategories:
         return YoloStrictBase._load_categories(names_path)
 
+    def _get_fname(self, fpath: str) -> str:
+        return osp.splitext(osp.basename(fpath))[0]
+
+    def _load_img_files(self, rootpath: str) -> Dict:
+        return {
+            self._get_fname(img_file): img_file
+            for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
+            if extract_subset_name_from_parent(img_file, rootpath) == self._subset
+        }
+
+    def _parse_annotations(
+        self, anno_path: str, image: ImageFromFile, label_categories: LabelCategories
+    ) -> List[Annotation]:
+        return YoloStrictBase._parse_annotations(
+            anno_path=anno_path, image=image, label_categories=label_categories
+        )
+
+    def _parse_field(self, value: str, desired_type: Type[T], field_name: str) -> T:
+        return YoloStrictBase._parse_field(
+            value=value, desired_type=desired_type, field_name=field_name
+        )
+
 
 class YoloUltralyticsBase(YoloLooseBase):
     META_FILE = YoloUltralyticsPath.META_FILE
 
     def __init__(
         self,
         config_path: str,
@@ -363,11 +381,18 @@
         if has_meta_file(osp.dirname(names_path)):
             return LabelCategories.from_iterable(parse_meta_file(osp.dirname(names_path)).keys())
 
         label_categories = LabelCategories()
 
         with open(names_path, "r") as fp:
             loaded = yaml.safe_load(fp.read())
-            for label_name in loaded["names"].values():
-                label_categories.add(label_name)
+            if isinstance(loaded["names"], list):
+                label_names = loaded["names"]
+            elif isinstance(loaded["names"], dict):
+                label_names = list(loaded["names"].values())
+            else:
+                raise DatasetImportError(f"Can't read dataset category file '{names_path}'")
+
+        for label_name in label_names:
+            label_categories.add(label_name)
 
         return label_categories
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import os
 import os.path as osp
 from collections import OrderedDict, defaultdict
 
 import yaml
 
 from datumaro.components.annotation import AnnotationType, Bbox
-from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetItem, IDataset
+from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import DatasetExportError, DatumaroError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
 from datumaro.util import str_to_bool
 
 from .format import YoloPath
```

### Comparing `datumaro-1.3.2/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/explorer.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/explorer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+from typing import List, Sequence
+
 import numpy as np
 from tokenizers import Tokenizer
 
+from datumaro.components.annotation import Annotation, HashKey
+from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.media import Image
 from datumaro.plugins.openvino_plugin.launcher import OpenvinoLauncher
 
 
 class ExplorerLauncher(OpenvinoLauncher):
     def __init__(
@@ -23,15 +27,14 @@
     ):
         super().__init__(
             description, weights, interpreter, model_dir, model_name, output_layers, device
         )
 
         self._device = device or "cpu"
         self._output_blobs = next(iter(self._net.outputs))
-        self._input_blobs = next(iter(self._net.input_info))
         self._tokenizer = None
 
     def _tokenize(self, texts: str, context_length: int = 77, truncate: bool = True):
         if not self._tokenizer:
             checkpoint = "openai/clip-vit-base-patch32"
             self._tokenizer = Tokenizer.from_pretrained(checkpoint)
         tokens = self._tokenizer.encode(texts).ids
@@ -50,36 +53,26 @@
     def _compute_hash(self, features):
         features = np.sign(features)
         hash_key = np.clip(features, 0, None)
         hash_key = hash_key.astype(np.uint8)
         hash_key = np.packbits(hash_key, axis=-1)
         return hash_key
 
-    def infer(self, inputs):
-        if isinstance(inputs, str):
-            if len(inputs.split()) > 1:
-                prompt_text = inputs
-            else:
-                prompt_text = f"a photo of a {inputs}"
-            inputs = self._tokenize(prompt_text)
-            inputs = {self._input_blob: inputs}
-        elif isinstance(inputs, np.ndarray):
-            # when processing a query key, we expand HWC to NHWC
-            if len(inputs.shape) == 3:
-                inputs = np.expand_dims(inputs, axis=0)
-            inputs = self.process_inputs(inputs)
-        else:
-            raise ValueError(f"inputs={inputs} is not allowed type.")
-
-        results = self._net.infer(inputs)
-        hash_key = self._compute_hash(results[self._output_blobs])
-        return hash_key
-
-    def launch(self, inputs):
-        hash_key = self.infer(inputs)
-        results = self.process_outputs(inputs, hash_key)
-        return results
+    def infer_text(self, text: str, use_prompt: bool = True) -> HashKey:
+        prompt_text = f"a photo of a {text}" if use_prompt else text
+        inputs = self._tokenize(prompt_text)
+        preds = self.infer(inputs)
+        anns = self.postprocess(preds[0], None)
+        return anns[0]
+
+    def infer_item(self, item: DatasetItem) -> HashKey:
+        anns = self.launch([item])[0]
+        return anns[0]
+
+    def launch(self, batch: Sequence[DatasetItem]) -> List[List[Annotation]]:
+        outputs = super().launch(batch)
+        return outputs
 
     def type_check(self, item):
         if not isinstance(item.media, Image):
             raise MediaTypeError(f"Media type should be Image, Current type={type(item.media)}")
         return True
```

### Comparing `datumaro-1.3.2/datumaro/plugins/ndr.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # Copyright (C) 2019-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # pylint: disable=exec-used
 
+
 import logging as log
-import os
 import os.path as osp
 import shutil
 import urllib
+from dataclasses import dataclass, fields
+from typing import Dict, List, Optional
 
-import cv2
 import numpy as np
-from openvino.inference_engine import IECore
+from openvino.runtime import Core
 from tqdm import tqdm
 
+from datumaro.components.abstracts.model_interpreter import ModelPred
 from datumaro.components.cli_plugin import CliPlugin
-from datumaro.components.launcher import Launcher
+from datumaro.components.launcher import LauncherWithModelInterpreter
+from datumaro.errors import DatumaroError
+from datumaro.util.definitions import DATUMARO_CACHE_DIR
 from datumaro.util.samples import get_samples_path
 
 
 class _OpenvinoImporter(CliPlugin):
     @staticmethod
     def _parse_output_layers(s):
         return [s.strip() for s in s.split(",")]
@@ -56,117 +60,83 @@
         shutil.copy(model["weights"], osp.join(model_dir, osp.basename(model["weights"])))
         model["weights"] = osp.basename(model["weights"])
 
         shutil.copy(model["interpreter"], osp.join(model_dir, osp.basename(model["interpreter"])))
         model["interpreter"] = osp.basename(model["interpreter"])
 
 
-class InterpreterScript:
-    def __init__(self, path):
-        with open(path, "r", encoding="utf-8") as f:
-            script = f.read()
-
-        context = {}
-        exec(script, context, context)
-
-        normalize = context.get("normalize")
-        if not callable(normalize):
-            raise Exception("Can't find 'normalize' function in the interpreter script")
-        self.__dict__["normalize"] = normalize
-
-        process_outputs = context.get("process_outputs")
-        if not callable(process_outputs):
-            raise Exception("Can't find 'process_outputs' function in the interpreter script")
-        self.__dict__["process_outputs"] = process_outputs
-
-        get_categories = context.get("get_categories")
-        assert get_categories is None or callable(get_categories)
-        if get_categories:
-            self.__dict__["get_categories"] = get_categories
-
-    @staticmethod
-    def get_categories():
-        return None
-
-    @staticmethod
-    def process_outputs(inputs, outputs):
-        raise NotImplementedError("Function should be implemented in the interpreter script")
-
-    @staticmethod
-    def normalize(inputs):
-        raise NotImplementedError("Function should be implemented in the interpreter script")
-
-
-class OpenvinoLauncher(Launcher):
-    cli_plugin = _OpenvinoImporter
+@dataclass
+class OpenvinoModelInfo:
+    interpreter: Optional[str]
+    description: Optional[str]
+    weights: Optional[str]
+    model_dir: Optional[str]
+
+    def validate(self):
+        """Validate integrity of the member variables"""
+
+        def _validate(key: str):
+            path = getattr(self, key)
+            if not osp.isfile(path):
+                path = osp.join(self.model_dir, path)
+            if not osp.isfile(path):
+                raise DatumaroError(f'Failed to open model {key} file "{path}"')
+            setattr(self, key, path)
+
+        for field in fields(self):
+            if field.name != "model_dir":
+                _validate(field.name)
+
+
+@dataclass
+class BuiltinOpenvinoModelInfo(OpenvinoModelInfo):
+    downloadable_models = {
+        "clip_text_ViT-B_32",
+        "clip_visual_ViT-B_32",
+        "googlenet-v4-tf",
+    }
 
-    def __init__(
-        self,
-        description=None,
-        weights=None,
-        interpreter=None,
-        model_dir=None,
-        model_name=None,
-        output_layers=None,
-        device=None,
-    ):
-        if model_name:
-            model_dir = os.path.join(os.path.expanduser("~"), ".cache", "datumaro")
-            if not osp.exists(model_dir):
-                os.makedirs(model_dir)
-
-            # Please visit open-model-zoo repository for OpenVINO public models if you are interested in
-            # https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md
-            url_folder = "https://storage.openvinotoolkit.org/repositories/datumaro/models/"
-
-            description = osp.join(model_dir, model_name + ".xml")
-            if not osp.exists(description):
-                cached_description_url = osp.join(url_folder, model_name + ".xml")
-                log.info('Downloading: "{}" to {}\n'.format(cached_description_url, description))
-                self._download_file(cached_description_url, description)
-
-            weights = osp.join(model_dir, model_name + ".bin")
-            if not osp.exists(weights):
-                cached_weights_url = osp.join(url_folder, model_name + ".bin")
-                log.info('Downloading: "{}" to {}\n'.format(cached_weights_url, weights))
-                self._download_file(cached_weights_url, weights)
-
-            if not interpreter:
-                openvino_plugin_samples_dir = get_samples_path()
-                interpreter = osp.join(openvino_plugin_samples_dir, model_name + "_interp.py")
-
-        if not model_dir:
-            model_dir = ""
-
-        if not osp.isfile(description):
-            description = osp.join(model_dir, description)
-        if not osp.isfile(description):
-            raise Exception('Failed to open model description file "%s"' % (description))
-
-        if not osp.isfile(weights):
-            weights = osp.join(model_dir, weights)
-        if not osp.isfile(weights):
-            raise Exception('Failed to open model weights file "%s"' % (weights))
-
-        if not osp.isfile(interpreter):
-            interpreter = osp.join(model_dir, interpreter)
-        if not osp.isfile(interpreter):
-            raise Exception('Failed to open model interpreter script file "%s"' % (interpreter))
-
-        self._interpreter = InterpreterScript(interpreter)
+    @classmethod
+    def create_from_model_name(cls, model_name: str) -> "BuiltinOpenvinoModelInfo":
+        openvino_plugin_samples_dir = get_samples_path()
+        interpreter = osp.join(openvino_plugin_samples_dir, model_name + "_interp.py")
+        interpreter = interpreter if osp.exists(interpreter) else interpreter
+
+        model_dir = DATUMARO_CACHE_DIR
+
+        # Please visit open-model-zoo repository for OpenVINO public models if you are interested in
+        # https://github.com/openvinotoolkit/open_model_zoo/blob/master/models/public/index.md
+        url_folder = "https://storage.openvinotoolkit.org/repositories/datumaro/models/"
+
+        description = osp.join(model_dir, model_name + ".xml")
+        if not osp.exists(description):
+            description = (
+                cls._download_file(osp.join(url_folder, model_name + ".xml"), description)
+                if model_name in cls.downloadable_models
+                else None
+            )
 
-        self._device = device or "CPU"
-        self._output_blobs = output_layers
+        weights = osp.join(model_dir, model_name + ".bin")
+        if not osp.exists(weights):
+            weights = (
+                cls._download_file(osp.join(url_folder, model_name + ".bin"), weights)
+                if model_name in cls.downloadable_models
+                else None
+            )
 
-        self._ie = IECore()
-        self._network = self._ie.read_network(description, weights)
-        self._check_model_support(self._network, self._device)
-        self._load_executable_net()
+        return cls(
+            interpreter=interpreter,
+            description=description,
+            weights=weights,
+            model_dir=model_dir,
+        )
 
-    def _download_file(self, url: str, file_root: str):
+    @staticmethod
+    def _download_file(url: str, file_root: str) -> str:
+        log.info('Downloading: "{}" to {}\n'.format(url, file_root))
         req = urllib.request.Request(url)
         with urllib.request.urlopen(req) as source, open(file_root, "wb") as output:  # nosec B310
             with tqdm(
                 total=int(source.info().get("Content-Length")),
                 ncols=80,
                 unit="iB",
                 unit_scale=True,
@@ -175,93 +145,126 @@
                 while True:
                     buffer = source.read(8192)
                     if not buffer:
                         break
 
                     output.write(buffer)
                     loop.update(len(buffer))
-        return 0
+        return file_root
+
+    def override(self, other: OpenvinoModelInfo) -> None:
+        """Override builtin model variables to other"""
+
+        def _apply(key: str) -> None:
+            other_item = getattr(other, key)
+            self_item = getattr(self, key)
+            if other_item is None and self_item:
+                log.info(f"Override description with the builtin model {key}: {self.description}.")
+                setattr(other, key, self_item)
+
+        for field in fields(self):
+            _apply(field.name)
+
+
+class OpenvinoLauncher(LauncherWithModelInterpreter):
+    cli_plugin = _OpenvinoImporter
+
+    def __init__(
+        self,
+        description: Optional[str] = None,
+        weights: Optional[str] = None,
+        interpreter: Optional[str] = None,
+        model_dir: Optional[str] = None,
+        model_name: Optional[str] = None,
+        output_layers: List[str] = [],
+        device: Optional[str] = None,
+        compile_model_config: Optional[Dict] = None,
+    ):
+        model_info = OpenvinoModelInfo(
+            interpreter=interpreter,
+            description=description,
+            weights=weights,
+            model_dir=model_dir,
+        )
+        if model_name:
+            builtin_model_info = BuiltinOpenvinoModelInfo.create_from_model_name(model_name)
+            builtin_model_info.override(model_info)
+
+        model_info.validate()
+
+        super().__init__(model_interpreter_path=model_info.interpreter)
+
+        self.model_info = model_info
+
+        self._device = device or "CPU"
+        self._compile_model_config = compile_model_config
+
+        self._core = Core()
+        self._network = self._core.read_model(model_info.description, model_info.weights)
+
+        if output_layers:
+            log.info(f"Add additional output layers {output_layers} to the model outputs.")
+            self._network.add_outputs(output_layers)
+
+        self._check_model_support(self._network, self._device)
+        self._load_executable_net()
 
     def _check_model_support(self, net, device):
         not_supported_layers = set(
-            name for name, dev in self._ie.query_network(net, device).items() if not dev
+            name for name, dev in self._core.query_model(net, device).items() if not dev
         )
         if len(not_supported_layers) != 0:
             log.error(
                 "The following layers are not supported "
                 "by the plugin for device '%s': %s." % (device, ", ".join(not_supported_layers))
             )
             raise NotImplementedError("Some layers are not supported on the device")
 
-    def _load_executable_net(self, batch_size=1):
+    def _load_executable_net(self, batch_size: int = 1):
         network = self._network
 
-        if self._output_blobs:
-            network.add_outputs(self._output_blobs)
-
-        iter_inputs = iter(network.input_info)
+        iter_inputs = iter(network.inputs)
         self._input_blob = next(iter_inputs)
 
-        # NOTE: handling for the inclusion of `image_info` in OpenVino2019
-        self._require_image_info = "image_info" in network.input_info
-        if self._input_blob == "image_info":
-            self._input_blob = next(iter_inputs)
-
-        self._input_layout = network.input_info[self._input_blob].input_data.shape
-        self._input_layout[0] = batch_size
-        network.reshape({self._input_blob: self._input_layout})
-        self._batch_size = batch_size
+        is_dynamic_layout = False
+        try:
+            self._input_layout = self._input_blob.shape
+        except ValueError:
+            # In case of that the input has dynamic shape
+            self._input_layout = self._input_blob.partial_shape
+            is_dynamic_layout = True
+
+        if is_dynamic_layout:
+            self._input_layout[0] = batch_size
+            network.reshape({self._input_blob: self._input_layout})
+        else:
+            model_batch_size = self._input_layout[0]
+            if batch_size != model_batch_size:
+                log.warning(
+                    "Input layout of the model is static, so that we cannot change "
+                    f"the model batch size ({model_batch_size}) to batch size ({batch_size})! "
+                    "Set the batch size to {model_batch_size}."
+                )
+                batch_size = model_batch_size
 
-        self._net = self._ie.load_network(network=network, num_requests=1, device_name=self._device)
+        self._batch_size = batch_size
 
-    def infer(self, inputs):
-        inputs = self.process_inputs(inputs)
-        results = self._net.infer(inputs)
-        if len(results) == 1:
-            return next(iter(results.values()))
-        else:
-            return results
+        self._net = self._core.compile_model(
+            model=network,
+            device_name=self._device,
+            config=self._compile_model_config,
+        )
+        self._request = self._net.create_infer_request()
 
-    def launch(self, inputs):
+    def infer(self, inputs: np.ndarray) -> List[ModelPred]:
         batch_size = len(inputs)
         if self._batch_size < batch_size:
             self._load_executable_net(batch_size)
 
-        outputs = self.infer(inputs)
-        results = self.process_outputs(inputs, outputs)
-        return results
-
-    def categories(self):
-        return self._interpreter.get_categories()
-
-    def process_outputs(self, inputs, outputs):
-        return self._interpreter.process_outputs(inputs, outputs)
-
-    def process_inputs(self, inputs):
-        assert len(inputs.shape) == 4, "Expected an input image in (N, H, W, C) format, got %s" % (
-            inputs.shape,
-        )
-
-        if inputs.shape[3] == 1:  # A batch of single-channel images
-            inputs = np.repeat(inputs, 3, axis=3)
-
-        assert inputs.shape[3] == 3, "Expected BGR input, got %s" % (inputs.shape,)
+        results = self._request.infer(inputs={self._input_blob.get_any_name(): inputs})
 
-        n, c, h, w = self._input_layout
-        if inputs.shape[1:3] != (h, w):
-            resized_inputs = np.empty((n, h, w, c), dtype=inputs.dtype)
-            for inp, resized_input in zip(inputs, resized_inputs):
-                cv2.resize(inp, (w, h), resized_input)
-            inputs = resized_inputs
-        inputs = inputs.transpose((0, 3, 1, 2))  # NHWC to NCHW
-
-        inputs = self._interpreter.normalize(inputs)
-
-        inputs = {self._input_blob: inputs}
-        if self._require_image_info:
-            info = np.zeros([1, 3])
-            info[0, 0] = h
-            info[0, 1] = w
-            info[0, 2] = 1.0  # scale
-            inputs["image_info"] = info
+        outputs_group_by_item = [
+            {key.any_name: output for key, output in zip(results.keys(), outputs)}
+            for outputs in zip(*results.values())
+        ]
 
-        return inputs
+        return outputs_group_by_item
```

### Comparing `datumaro-1.3.2/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+from datumaro.components.abstracts import IModelInterpreter
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.util.annotation_util import softmax
 
 
-def normalize(inputs):
-    return inputs
+class MobilenetV2PytorchModelInterpreter(IModelInterpreter):
+    def normalize(self, inputs):
+        return inputs
 
+    def process_outputs(self, inputs, outputs):
+        # inputs = model input; array or images; shape = (B, H, W, C)
+        # outputs = model output; shape = (1, 1, N, 7); N is the number of detected bounding boxes.
+        # det = [image_id, label(class id), conf, x_min, y_min, x_max, y_max]
+        # results = conversion result; [[ Annotation, ... ], ... ]
 
-def process_outputs(inputs, outputs):
-    # inputs = model input; array or images; shape = (B, H, W, C)
-    # outputs = model output; shape = (1, 1, N, 7); N is the number of detected bounding boxes.
-    # det = [image_id, label(class id), conf, x_min, y_min, x_max, y_max]
-    # results = conversion result; [[ Annotation, ... ], ... ]
+        results = []
+        for input_, output in zip(inputs, outputs):  # pylint: disable=unused-variable
+            image_results = []
+            output = softmax(output).tolist()
+            label = output.index(max(output))
+            image_results.append(Label(label=label, attributes={"scores": output}))
 
-    results = []
-    for input_, output in zip(inputs, outputs):  # pylint: disable=unused-variable
-        image_results = []
-        output = softmax(output).tolist()
-        label = output.index(max(output))
-        image_results.append(Label(label=label, attributes={"scores": output}))
+            results.append(image_results)
 
-        results.append(image_results)
+        return results
 
-    return results
+    def get_categories(self):
+        # output categories - label map etc.
 
+        label_categories = LabelCategories()
 
-def get_categories():
-    # output categories - label map etc.
+        with open("samples/imagenet.class", "r", encoding="utf-8") as file:
+            for line in file.readlines():
+                label = line.strip()
+                label_categories.add(label)
 
-    label_categories = LabelCategories()
+        return {AnnotationType.label: label_categories}
 
-    with open("samples/imagenet.class", "r", encoding="utf-8") as file:
-        for line in file.readlines():
-            label = line.strip()
-            label_categories.add(label)
-
-    return {AnnotationType.label: label_categories}
+    def resize(self, inputs):
+        return inputs
```

### Comparing `datumaro-1.3.2/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/splitter.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import List, Optional, Tuple
 
 import cv2 as cv
 import numpy as np
 import requests
 
 from datumaro.components.generator import DatasetGenerator
+from datumaro.util.definitions import DATUMARO_CACHE_DIR
 from datumaro.util.image import save_image
 from datumaro.util.scope import on_error_do, on_exit_do, scope_add, scoped
 
 from .utils import IFSFunction, augment, colorize, suppress_computation_warnings
 
 
 class FractalImageGenerator(DatasetGenerator):
@@ -30,21 +31,25 @@
 
     _MODEL_PROTO_FILENAME = "colorization_deploy_v2.prototxt"
     _MODEL_WEIGHTS_FILENAME = "colorization_release_v2.caffemodel"
     _HULL_PTS_FILE_NAME = "pts_in_hull.npy"
     _COLORS_FILE = "background_colors.txt"
 
     def __init__(
-        self, output_dir: str, count: int, shape: Tuple[int, int], model_path: Optional[str] = None
+        self,
+        output_dir: str,
+        count: int,
+        shape: Tuple[int, int],
+        model_path: str = DATUMARO_CACHE_DIR,
     ) -> None:
         assert 0 < count, "Image count cannot be lesser than 1"
         self._count = count
 
         self._output_dir = output_dir
-        self._model_dir = model_path if model_path else os.getcwd()
+        self._model_dir = model_path
 
         self._cpu_count = min(os.cpu_count(), self._count)
 
         assert len(shape) == 2
         self._height, self._width = shape
 
         self._weights = self._create_weights(IFSFunction.NUM_PARAMS)
```

### Comparing `datumaro-1.3.2/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/tiling/tile.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/tiling/util.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/transforms.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/plugins/validators.py` & `datumaro-1.4.0rc1/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/__init__.py` & `datumaro-1.4.0rc1/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/annotation_util.py` & `datumaro-1.4.0rc1/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/attrs_util.py` & `datumaro-1.4.0rc1/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/file_utils.py` & `datumaro-1.4.0rc1/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/image.py` & `datumaro-1.4.0rc1/src/datumaro/util/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 
         import datumaro.components.media as media_module
 
         return getattr(media_module, name)
     raise AttributeError(f"module {__name__} has no attribute {name}")
 
 
-def load_image(path: str, dtype: DTypeLike = np.float32, crypter: Crypter = NULL_CRYPTER):
+def load_image(path: str, dtype: DTypeLike = np.uint8, crypter: Crypter = NULL_CRYPTER):
     """
-    Reads an image in the HWC Grayscale/BGR(A) float [0; 255] format.
+    Reads an image in the HWC Grayscale/BGR(A) [0; 255] format (default dtype is uint8).
     """
 
     if _IMAGE_BACKEND == _IMAGE_BACKENDS.cv2:
         # cv2.imread does not support paths that are not representable
         # in the locale encoding on Windows, so we read the image bytes
         # ourselves.
 
@@ -79,14 +79,15 @@
 
         if not crypter.is_null_crypter:
             raise DatumaroError("PIL backend should have crypter=NullCrypter.")
 
         image = Image.open(path)
         image = np.asarray(image, dtype=dtype)
         if len(image.shape) == 3 and image.shape[2] in {3, 4}:
+            image = np.array(image)  # Release read-only
             image[:, :, :3] = image[:, :, 2::-1]  # RGB to BGR
     else:
         raise NotImplementedError()
 
     assert len(image.shape) in {2, 3}
     if len(image.shape) == 3:
         assert image.shape[2] in {3, 4}
@@ -221,27 +222,28 @@
         with BytesIO() as buffer:
             image.save(buffer, format=ext, **params)
             return buffer.getvalue()
     else:
         raise NotImplementedError()
 
 
-def decode_image(image_bytes: bytes, dtype: DTypeLike = np.float32) -> np.ndarray:
+def decode_image(image_bytes: bytes, dtype: DTypeLike = np.uint8) -> np.ndarray:
     if _IMAGE_BACKEND == _IMAGE_BACKENDS.cv2:
         import cv2
 
         image = np.frombuffer(image_bytes, dtype=np.uint8)
         image = cv2.imdecode(image, cv2.IMREAD_UNCHANGED)
         image = image.astype(dtype)
     elif _IMAGE_BACKEND == _IMAGE_BACKENDS.PIL:
         from PIL import Image
 
         image = Image.open(BytesIO(image_bytes))
         image = np.asarray(image, dtype=dtype)
         if len(image.shape) == 3 and image.shape[2] in {3, 4}:
+            image = np.array(image)  # Release read-only
             image[:, :, :3] = image[:, :, 2::-1]  # RGB to BGR
     else:
         raise NotImplementedError()
 
     assert len(image.shape) in {2, 3}
     if len(image.shape) == 3:
         assert image.shape[2] in {3, 4}
```

### Comparing `datumaro-1.3.2/datumaro/util/image_cache.py` & `datumaro-1.4.0rc1/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/log_utils.py` & `datumaro-1.4.0rc1/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/mask_tools.py` & `datumaro-1.4.0rc1/src/datumaro/util/mask_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (C) 2019-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from functools import partial
 from itertools import chain
-from typing import Tuple
+from typing import Dict, Tuple
 
 import numpy as np
+from pycocotools import mask as pycocotools_mask
 
 from datumaro._capi import encode
 from datumaro.util.image import lazy_image, load_image
 
 
 def generate_colormap(length=256, *, include_background=True):
     """
@@ -219,23 +220,22 @@
         tolerance: maximum distance from original points of
             a polygon to the approximated ones
         area_threshold: minimal area of generated polygons
 
     Returns:
         A list of polygons like [[x1,y1, x2,y2 ...], [...]]
     """
-    from pycocotools import mask as mask_utils
 
     contours = extract_contours(mask)
 
     polygons = []
     for contour in contours:
         # Check if the polygon is big enough
-        rle = mask_utils.frPyObjects([contour], mask.shape[0], mask.shape[1])
-        area = sum(mask_utils.area(rle))
+        rle = pycocotools_mask.frPyObjects([contour], mask.shape[0], mask.shape[1])
+        area = sum(pycocotools_mask.area(rle))
         if area_threshold <= area:
             polygons.append(contour)
     return polygons
 
 
 def mask_to_bboxes(mask):
     """
@@ -292,34 +292,32 @@
             [
                 [[x1,y1, x2,y2 ...], ...], # input segment #0 parts
                 mask1, # input segment #1 mask (if source segment is mask)
                 [], # when source segment is too small
                 ...
             ]
     """
-    from pycocotools import mask as mask_utils
-
     segments = [[s] for s in segments]
-    input_rles = [mask_utils.frPyObjects(s, height, width) for s in segments]
+    input_rles = [pycocotools_mask.frPyObjects(s, height, width) for s in segments]
 
     for i, rle_bottom in enumerate(input_rles):
-        area_bottom = sum(mask_utils.area(rle_bottom))
+        area_bottom = sum(pycocotools_mask.area(rle_bottom))
         if area_bottom < area_threshold:
             segments[i] = [] if not return_masks else None
             continue
 
         rles_top = []
         for j in range(i + 1, len(input_rles)):
             rle_top = input_rles[j]
-            iou = sum(mask_utils.iou(rle_bottom, rle_top, [0]))[0]
+            iou = sum(pycocotools_mask.iou(rle_bottom, rle_top, [0]))[0]
 
             if iou <= iou_threshold:
                 continue
 
-            area_top = sum(mask_utils.area(rle_top))
+            area_top = sum(pycocotools_mask.area(rle_top))
             area_ratio = area_top / area_bottom
 
             # If a segment is fully inside another one, skip this segment
             if abs(area_ratio - iou) < ratio_tolerance:
                 continue
 
             # Check if the bottom segment is fully covered by the top one.
@@ -330,40 +328,49 @@
 
             rles_top += rle_top
 
         if not rles_top and not isinstance(segments[i][0], dict) and not return_masks:
             continue
 
         rle_bottom = rle_bottom[0]
-        bottom_mask = mask_utils.decode(rle_bottom).astype(np.uint8)
+        bottom_mask = pycocotools_mask.decode(rle_bottom).astype(np.uint8)
 
         if rles_top:
-            rle_top = mask_utils.merge(rles_top)
-            top_mask = mask_utils.decode(rle_top).astype(np.uint8)
+            rle_top = pycocotools_mask.merge(rles_top)
+            top_mask = pycocotools_mask.decode(rle_top).astype(np.uint8)
 
             bottom_mask -= top_mask
             bottom_mask[bottom_mask != 1] = 0
 
         if not return_masks and not isinstance(segments[i][0], dict):
             segments[i] = mask_to_polygons(bottom_mask, area_threshold=area_threshold)
         else:
             segments[i] = bottom_mask
 
     return segments
 
 
 def rles_to_mask(rles, width, height):
-    from pycocotools import mask as mask_utils
-
-    rles = mask_utils.frPyObjects(rles, height, width)
-    rles = mask_utils.merge(rles)
-    mask = mask_utils.decode(rles)
+    rles = pycocotools_mask.frPyObjects(rles, height, width)
+    rles = pycocotools_mask.merge(rles)
+    mask = pycocotools_mask.decode(rles)
     return mask
 
 
+def rle_to_mask(rle_uncompressed: Dict[str, np.ndarray]) -> np.ndarray:
+    """Decode the uncompressed RLE string to the binary mask (2D np.ndarray)
+
+    The uncompressed RLE string can be obtained by
+    the datumaro.util.mask_tools.mask_to_rle() function
+    """
+    resulting_mask = pycocotools_mask.frPyObjects(rle_uncompressed, *rle_uncompressed["size"])
+    resulting_mask = pycocotools_mask.decode(resulting_mask)
+    return resulting_mask
+
+
 def find_mask_bbox(mask) -> Tuple[int, int, int, int]:
     cols = np.any(mask, axis=0)
     rows = np.any(mask, axis=1)
     x0, x1 = np.where(cols)[0][[0, -1]]
     y0, y1 = np.where(rows)[0][[0, -1]]
     return (x0, y0, x1 - x0, y1 - y0)
```

### Comparing `datumaro-1.3.2/datumaro/util/meta_file_util.py` & `datumaro-1.4.0rc1/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/os_util.py` & `datumaro-1.4.0rc1/src/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/pickle_util.py` & `datumaro-1.4.0rc1/src/datumaro/util/pickle_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import pickle  # nosec import_pickle
+import pickle  # nosec B403
 
 import numpy.core.multiarray
 
 
 class RestrictedUnpickler(pickle.Unpickler):
     def find_class(self, module, name):
         if module == "numpy.core.multiarray" and name in PickleLoader.safe_numpy:
```

### Comparing `datumaro-1.3.2/datumaro/util/scope.py` & `datumaro-1.4.0rc1/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/telemetry_stub.py` & `datumaro-1.4.0rc1/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro/util/telemetry_utils.py` & `datumaro-1.4.0rc1/src/datumaro/util/telemetry_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         return "checkout_result"
     elif command is commands.require_project.versioning.commit.commit_command:
         return "commit_result"
     elif command is commands.convert.convert_command:
         return "convert_result"
     elif command is commands.require_project.modification.create.create_command:
         return "create_result"
-    elif command is commands.diff.diff_command:
+    elif command is commands.compare.compare_command:
         return "diff_result"
     elif command is commands.explain.explain_command:
         return "explain_result"
     elif command is commands.generate.generate_command:
         return "generate_result"
     elif command is commands.info.info_command:
         return "info_result"
```

### Comparing `datumaro-1.3.2/datumaro/util/tf_util.py` & `datumaro-1.4.0rc1/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.3.2/datumaro.egg-info/PKG-INFO` & `datumaro-1.4.0rc1/src/datumaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.3.2
+Version: 1.4.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tf
 Provides-Extra: tfds
 Provides-Extra: tf-gpu
 Provides-Extra: default
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `datumaro-1.3.2/datumaro.egg-info/requires.txt` & `datumaro-1.4.0rc1/src/datumaro.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -13,37 +13,42 @@
 typing_extensions>=3.7.4.3
 tqdm
 PyYAML>=5.3.1
 tensorboardX!=2.3,>=1.8
 scipy
 requests
 pandas>=1.1.5
-openvino==2022.3.0
+openvino==2023.0.0
 tokenizers
 cryptography>=38.03
 pyemd
 pyarrow
-protobuf
+protobuf<4
+tabulate
+ovmsclient
+tritonclient[all]
+scikit-learn
 opencv-python
 
 [:platform_system != "Windows" or python_version >= "3.9"]
 pycocotools>=2.0.4
 
 [:platform_system == "Windows" and python_version < "3.9"]
 pycocotools-windows
 
 [default]
-dvc<3.0.0,>=2.7.0
+dvc>=3.0.0
 GitPython!=3.1.25,>=3.1.18
 openvino-telemetry>=2022.1.0
+openvino-dev==2023.0.0
 
 [default:python_version < "3.8"]
 fsspec<=2022.11.0
 
 [tf]
 tensorflow
 
 [tf-gpu]
 tensorflow-gpu
 
 [tfds]
-tensorflow-datasets<4.9.0
+tensorflow-datasets
```

### Comparing `datumaro-1.3.2/pyproject.toml` & `datumaro-1.4.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 line_length = 100
 
 [tool.coverage.run]
 branch = true
 # relative_files = true # does not work?
 
 source = [
-    "datumaro/",
+    "src/",
 ]
 
 omit = [
-    "datumaro/__main__.py",
-    "datumaro/version.py",
+    "src/datumaro/__main__.py",
+    "src/datumaro/version.py",
     "tests/*",
 ]
 
+[tool.cibuildwheel]
+build = "cp38-*_x86_64 cp39-*_x86_64 cp310-*_x86_64 cp311-*_x86_64 cp38-*_amd64 cp39-*_amd64 cp310-*_amd64 cp311-*_amd64"
+
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_lines = [
     # Have to re-enable the standard pragma
     'pragma: no cover',
 
     # Don't complain about missing debug-only code:
@@ -43,15 +46,15 @@
 # don't fail on the code that can be found
 ignore_errors = true
 
 skip_empty = true
 
 [tool.black]
 line-length = 100
-target-version = ['py37']
+target-version = ['py38']
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
 
 # Need to review all ignore items below
 ignore = [
@@ -88,35 +91,35 @@
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
 
 extend-exclude = [
-    "datumaro/plugins/openvino_plugin/samples"
+    "src/datumaro/plugins/openvino_plugin/samples"
 ]
 
 # Same as Black.
 line-length = 120
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 # minimum target version
-target-version = "py37"
+target-version = "py38"
 
 # ignore-init-module-imports = true
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = [
     "F401"      # unused-import
 ]
-"datumaro/plugins/data_formats/ava/ava_label_pb2.py" = [
+"src/datumaro/plugins/data_formats/ava/ava_label_pb2.py" = [
     "E501"      # line-too-long
 ]
 
 [tool.nbqa.addopts]
 ruff = ["--ignore=E402"]
```

### Comparing `datumaro-1.3.2/requirements-core.txt` & `datumaro-1.4.0rc1/requirements-core.txt`

 * *Files 12% similar despite different names*

```diff
@@ -29,21 +29,31 @@
 # Image generator
 requests
 
 # Sampler
 pandas>=1.1.5
 
 # OpenVINO
-openvino==2022.3.0
+openvino==2023.0.0
 tokenizers
 
 # Encryption
 cryptography>= 38.03
 
 # Shift analyzer
 pyemd
 
 # apache arrow
 pyarrow
 
 # ava data format
-protobuf
+protobuf<4
+
+# Comparator
+tabulate
+
+# Model inference launcher from the dedicated inference server
+ovmsclient
+tritonclient[all]
+
+# prune
+scikit-learn
```

### Comparing `datumaro-1.3.2/setup.py` & `datumaro-1.4.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 import os.path as osp
 import re
 from distutils.util import strtobool
 
 import setuptools
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
-# Snyk scan integration
-here = None
-
 
 def find_version(project_dir=None):
     if not project_dir:
         project_dir = osp.dirname(osp.abspath(__file__))
 
     file_path = osp.join(project_dir, "datumaro", "version.py")
 
@@ -56,48 +53,50 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 ext_modules = [
     Pybind11Extension(
         "datumaro._capi",
-        ["datumaro/capi/pybind.cpp"],
-        define_macros=[("VERSION_INFO", find_version(here))],
+        ["src/datumaro/capi/pybind.cpp"],
+        define_macros=[("VERSION_INFO", find_version("./src"))],
         extra_compile_args=["-O3"],
     ),
 ]
 
 setuptools.setup(
     name="datumaro",
-    version=find_version(here),
+    version=find_version("./src"),
     author="Intel",
     author_email="emily.chun@intel.com",
     description="Dataset Management Framework (Datumaro)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/openvinotoolkit/datumaro",
-    packages=setuptools.find_packages(include=["datumaro*"]),
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src", include=["datumaro*"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=CORE_REQUIREMENTS,
     extras_require={
         "tf": ["tensorflow"],
-        "tfds": [
-            "tensorflow-datasets<4.9.0"
-        ],  # 4.9.0 fails on Windows and MacOS, https://github.com/openvinotoolkit/datumaro/actions/runs/4618774184
+        "tfds": ["tensorflow-datasets"],
         "tf-gpu": ["tensorflow-gpu"],
         "default": DEFAULT_REQUIREMENTS,
     },
     ext_modules=ext_modules,
     entry_points={
         "console_scripts": [
             "datum=datumaro.cli.__main__:main",
         ],
     },
     cmdclass={"build_ext": build_ext},
-    package_data={"datumaro.plugins.synthetic_data": ["background_colors.txt"]},
+    package_data={
+        "datumaro.plugins.synthetic_data": ["background_colors.txt"],
+        "datumaro.plugins.openvino_plugin.samples": ["coco.class", "imagenet.class"],
+    },
     include_package_data=True,
 )
```

