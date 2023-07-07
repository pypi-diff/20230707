# Comparing `tmp/pyphetools-0.4.5.tar.gz` & `tmp/pyphetools-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.4.5.tar", last modified: Sun Jul  2 16:47:00 2023, max compression
+gzip compressed data, was "pyphetools-0.4.7.tar", last modified: Fri Jul  7 15:05:29 2023, max compression
```

## Comparing `pyphetools-0.4.5.tar` & `pyphetools-0.4.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:47:00.007690 pyphetools-0.4.5/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.5/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.5/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-02 16:47:00.007690 pyphetools-0.4.5/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.5/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.5/docs/conf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/pyphetools/
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.5/pyphetools/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/pyphetools/analyze/
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.5/pyphetools/analyze/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/analyze/downsampler.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/pyphetools/creation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      882 2023-06-29 12:30:59.000000 pyphetools-0.4.5/pyphetools/creation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.5/pyphetools/creation/age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7929 2023-06-29 13:53:18.000000 pyphetools-0.4.5/pyphetools/creation/case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.5/pyphetools/creation/cohort_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.5/pyphetools/creation/column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/creation/constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.5/pyphetools/creation/constants.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.5/pyphetools/creation/custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5506 2023-06-29 11:35:00.000000 pyphetools-0.4.5/pyphetools/creation/hgvs_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.5/pyphetools/creation/hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.5/pyphetools/creation/hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.4.5/pyphetools/creation/hpo_exact_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.5/pyphetools/creation/hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7515 2023-06-29 13:36:57.000000 pyphetools-0.4.5/pyphetools/creation/individual.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6402 2023-06-29 15:58:37.000000 pyphetools-0.4.5/pyphetools/creation/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6257 2023-07-02 16:29:47.000000 pyphetools-0.4.5/pyphetools/creation/option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.5/pyphetools/creation/sex_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.4.5/pyphetools/creation/simple_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6969 2023-06-29 11:43:08.000000 pyphetools-0.4.5/pyphetools/creation/structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.5/pyphetools/creation/thresholded_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      268 2023-06-29 11:43:15.000000 pyphetools-0.4.5/pyphetools/creation/variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5641 2023-06-29 13:35:41.000000 pyphetools-0.4.5/pyphetools/creation/variant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.5/pyphetools/creation/variant_validator.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/pyphetools/output/
--rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.5/pyphetools/output/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/output/detailed_suppl_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/output/focus_count_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.5/pyphetools/output/hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.5/pyphetools/output/phenopacket_ingestor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.5/pyphetools/output/phenopacket_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.5/pyphetools/output/simple_patient.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.4.5/pyphetools/output/simple_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.5/pyphetools/output/term_count.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/pyphetools/validation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      111 2023-06-29 14:50:29.000000 pyphetools-0.4.5/pyphetools/validation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3792 2023-06-29 17:31:14.000000 pyphetools-0.4.5/pyphetools/validation/content_validator.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      187 2023-06-29 14:49:26.000000 pyphetools-0.4.5/pyphetools/validation/phenopacket_validator.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1115 2023-06-29 17:46:07.000000 pyphetools-0.4.5/pyphetools/validation/validation_result.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/pyphetools.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2326 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-07-02 16:30:04.000000 pyphetools-0.4.5/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-02 16:47:00.007690 pyphetools-0.4.5/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.5/test/test_age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3370 2023-06-29 13:58:19.000000 pyphetools-0.4.5/test/test_case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.5/test/test_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.5/test/test_constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.5/test/test_custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.5/test/test_hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.5/test/test_hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.5/test/test_hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.5/test/test_hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.4.5/test/test_option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.4.5/test/test_structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.5/test/test_threshold_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.5/test/test_variant.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/venv/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:47:00.007690 pyphetools-0.4.5/venv/bin/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2html.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2html4.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2html5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2latex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2man.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2odt.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2s5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2xetex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2xml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rstpep2html.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.456592 pyphetools-0.4.7/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.7/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.7/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-07 15:05:29.456592 pyphetools-0.4.7/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.7/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.7/docs/conf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/pyphetools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.7/pyphetools/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/pyphetools/analyze/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.7/pyphetools/analyze/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/analyze/downsampler.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/pyphetools/creation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      911 2023-07-07 14:16:51.000000 pyphetools-0.4.7/pyphetools/creation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.7/pyphetools/creation/age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7929 2023-06-29 13:53:18.000000 pyphetools-0.4.7/pyphetools/creation/case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.7/pyphetools/creation/cohort_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.7/pyphetools/creation/column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/creation/constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.7/pyphetools/creation/constants.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.7/pyphetools/creation/custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5506 2023-06-29 11:35:00.000000 pyphetools-0.4.7/pyphetools/creation/hgvs_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.7/pyphetools/creation/hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.7/pyphetools/creation/hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7408 2023-07-07 14:18:33.000000 pyphetools-0.4.7/pyphetools/creation/hpo_exact_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.7/pyphetools/creation/hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7515 2023-06-29 13:36:57.000000 pyphetools-0.4.7/pyphetools/creation/individual.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6402 2023-06-29 15:58:37.000000 pyphetools-0.4.7/pyphetools/creation/metadata.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6643 2023-07-07 15:03:31.000000 pyphetools-0.4.7/pyphetools/creation/option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.7/pyphetools/creation/sex_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6191 2023-07-07 14:27:35.000000 pyphetools-0.4.7/pyphetools/creation/simple_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6969 2023-06-29 11:43:08.000000 pyphetools-0.4.7/pyphetools/creation/structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.7/pyphetools/creation/thresholded_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      268 2023-06-29 11:43:15.000000 pyphetools-0.4.7/pyphetools/creation/variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5641 2023-06-29 13:35:41.000000 pyphetools-0.4.7/pyphetools/creation/variant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.7/pyphetools/creation/variant_validator.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/pyphetools/output/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.7/pyphetools/output/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/output/detailed_suppl_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/output/focus_count_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.7/pyphetools/output/hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.7/pyphetools/output/phenopacket_ingestor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.7/pyphetools/output/phenopacket_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.7/pyphetools/output/simple_patient.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3306 2023-07-04 23:45:19.000000 pyphetools-0.4.7/pyphetools/output/simple_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.7/pyphetools/output/term_count.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/pyphetools/validation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      111 2023-06-29 14:50:29.000000 pyphetools-0.4.7/pyphetools/validation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3792 2023-06-29 17:31:14.000000 pyphetools-0.4.7/pyphetools/validation/content_validator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      187 2023-06-29 14:49:26.000000 pyphetools-0.4.7/pyphetools/validation/phenopacket_validator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1115 2023-06-29 17:46:07.000000 pyphetools-0.4.7/pyphetools/validation/validation_result.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/pyphetools.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2326 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-07-07 15:04:43.000000 pyphetools-0.4.7/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-07 15:05:29.456592 pyphetools-0.4.7/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.7/test/test_age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3370 2023-06-29 13:58:19.000000 pyphetools-0.4.7/test/test_case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.7/test/test_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.7/test/test_constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.7/test/test_custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.7/test/test_hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.7/test/test_hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.7/test/test_hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.7/test/test_hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5398 2023-07-07 15:04:27.000000 pyphetools-0.4.7/test/test_option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.4.7/test/test_structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.7/test/test_threshold_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.7/test/test_variant.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/venv/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.456592 pyphetools-0.4.7/venv/bin/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2html.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2html4.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2html5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2latex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2man.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2odt.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2s5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2xml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.4.5/LICENSE` & `pyphetools-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/PKG-INFO` & `pyphetools-0.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.5
+Version: 0.4.7
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.5/README.md` & `pyphetools-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/docs/conf.py` & `pyphetools-0.4.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/analyze/downsampler.py` & `pyphetools-0.4.7/pyphetools/analyze/downsampler.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/__init__.py` & `pyphetools-0.4.7/pyphetools/creation/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 from .hpo_cr import HpoConceptRecognizer
 from .hpo_parser import HpoParser
 from .hp_term import HpTerm
 from .individual import Individual
 from .metadata import MetaData
 from .option_column_mapper import OptionColumnMapper
 from .sex_column_mapper import SexColumnMapper
-from .simple_column_mapper import SimpleColumnMapper
+from .simple_column_mapper import SimpleColumnMapper, SimpleColumnMapperGenerator
 from .structural_variant import StructuralVariant
 from .thresholded_column_mapper import ThresholdedColumnMapper
 from .variant_validator import VariantValidator
 from .variant_column_mapper import VariantColumnMapper
 from .variant import Variant
```

### Comparing `pyphetools-0.4.5/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/case_encoder.py` & `pyphetools-0.4.7/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.4.7/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/hgvs_variant.py` & `pyphetools-0.4.7/pyphetools/creation/hgvs_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/hp_term.py` & `pyphetools-0.4.7/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/hpo_cr.py` & `pyphetools-0.4.7/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.4.7/pyphetools/creation/hpo_exact_cr.py`

 * *Files 8% similar despite different names*

```diff
@@ -146,14 +146,19 @@
         if label_lc not in self._label_to_id:
             raise ValueError(f"Could not find HPO id for {label}")
         hpo_id = self._label_to_id.get(label_lc)
         return HpTerm(hpo_id=hpo_id, label=label)
 
     def contains_term(self, hpo_id) -> bool:
         return hpo_id in self._id_to_primary_label
+    
+    def contains_term_label(self, hpo_label) -> bool:
+        """return True iff the argument is the primary label of an HPO term
+        """
+        return hpo_label.lower() in self._label_to_id
 
     def initialize_simple_column_maps(self, column_name_to_hpo_label_map, observed, excluded, non_measured=None):
         if observed is None or excluded is None:
             raise ValueError("Symbols for observed (e.g., +, Y, yes) and excluded (e.g., -, N, no) required")
         if not isinstance(column_name_to_hpo_label_map, dict):
             raise ValueError("column_name_to_hpo_label_map must be a dict with column to HPO label mappings")
         simple_mapper_d = defaultdict(ColumnMapper)
```

### Comparing `pyphetools-0.4.5/pyphetools/creation/hpo_parser.py` & `pyphetools-0.4.7/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/individual.py` & `pyphetools-0.4.7/pyphetools/creation/individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/metadata.py` & `pyphetools-0.4.7/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/simple_column_mapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,134 +1,145 @@
 from .hp_term import HpTerm
 from .column_mapper import ColumnMapper
-from .hpo_cr import HpoConceptRecognizer
 from typing import List
 import pandas as pd
-import re
 from collections import defaultdict
 
-class OptionColumnMapper(ColumnMapper):
-    
-    def __init__(self, concept_recognizer, option_d, negative_symbol=None, negative_label=None):
-        """Mapper to be used if the column has a set of defined items but text mining is not required.
 
-        Args:
-            option_d (dict): key: item (e.g., MVP) in original publication; value: corresponding HPO label, e.g. Mitral Valve Prolapse
+def get_separate_hpos_from_df(df, hpo_cr):
+    """Loop through all the cells in a dataframe or series and try to parse each cell as HPO term.
+    Useful when the separate HPO terms are in the cells themselves.
+
+      Args:
+         df (dataframe): dataframe with phenotypic data
+         hpo_cr (HpoConceptRecognizer): instance of HpoConceptRecognizer to match HPO term and get label/id
+
+      Returns:
+          additional_hpos: list of lists with the additional HPO terms per individual
+      """
+    additional_hpos = []
+
+    for i in range(len(df)):
+        temp_hpos = []
+        for y in range(df.shape[1]):
+            hpo_term = hpo_cr.parse_cell(df.iloc[i, y])
+            if len(hpo_term) > 0:
+                temp_hpos.extend(hpo_term)
+        additional_hpos.append(list(set(temp_hpos)))
+    return additional_hpos
+
+
+
 
-        Raises:
-            ValueError: if option_d is not a dictionary
+
+
+class SimpleColumnMapper(ColumnMapper):
+
+    def __init__(self, hpo_id, hpo_label, observed=None, excluded=None, non_measured=None):
+        """ColumnMapper for columns that contain information about a single phenotypic abnormality only
+
+        Args:
+            hpo_id (_type_): HPO  id, e.g., HP:0004321
+            hpo_label (_type_): Corresponding term label
+            observed (_type_): symbol used in table if the phenotypic feature was observed
+            excluded (_type_): symbol used if the feature was excluded
+            non_measured (_type_, optional): symbol used if the feature was not measured or is N/A. Defaults to None.
+            constant (bool, optional): If true, all patients have this feature. Defaults to False.
         """
         super().__init__()
-        # Either have self._option_d be an empty dictionary or it must be a valid dictionary
-        if option_d is None or not isinstance(option_d, dict):
-            raise ValueError(f"option_d argument must be dictionary but was {type(option_d)}")
-        self._option_d = option_d
-        if not isinstance(concept_recognizer, HpoConceptRecognizer):
-            raise ValueError("concept_recognizer arg must be HpoConceptRecognizer but was {type(concept_recognizer)}")
-        self._hpo_cr = concept_recognizer
-        if negative_symbol is None:
-            negative_symbol = defaultdict()
-        self._negative_symbol = negative_symbol
-        self._negative_label = negative_label
-        self._has_negative = negative_label is not None and negative_symbol is not None
-        
+        self._hpo_id = hpo_id
+        self._hpo_label = hpo_label
+        if observed is None or excluded is None:
+            raise ValueError(
+                    "Need to provide arguments for both observed and excluded")
+        self._observed = observed
+        self._excluded = excluded
+        self._not_measured = non_measured
+
     def map_cell(self, cell_contents) -> List[HpTerm]:
-        """Map cell contents using the option dictionary 
-        
-        Args:
-            cell_contents (str): contents of one table cell
-        """
-        results = []
+        if not isinstance(cell_contents, str):
+            raise ValueError(
+                f"Error: cell_contents argument ({cell_contents}) must be string but was {type(cell_contents)} -- coerced to string")
         contents = cell_contents.strip()
-        if self._has_negative and contents == self._negative_symbol:
-            term = self._hpo_cr.get_term_from_label(label=self._negative_label)
-            term.excluded()
-            results.append(term)
-            return results
-        delimiters = ',;|/'
-        regex_pattern = '|'.join(map(re.escape, delimiters))
-        chunks = re.split(regex_pattern, contents)
-        chunks = [chunk.strip() for chunk in chunks]
-
-        hpo_labels = []
-        for c in chunks:
-            for my_key, my_label in self._option_d.items():
-                if my_key in c:
-                    if isinstance(my_label, list):
-                        for itm in my_label:
-                            hpo_labels.append(itm)
-                    else:
-                        hpo_labels.append(my_label)
-        for label in hpo_labels:    
-            term = self._hpo_cr.get_term_from_label(label=label)
-            results.append(term)
-        return results
-        
+        if contents in self._observed:
+            return [HpTerm(hpo_id=self._hpo_id, label=self._hpo_label)]
+        elif contents in self._excluded:
+            return [HpTerm(hpo_id=self._hpo_id, label=self._hpo_label, observed=False)]
+        else:
+            return [HpTerm(hpo_id=self._hpo_id, label=self._hpo_label, measured=False)]
+
     def preview_column(self, column) -> pd.DataFrame:
         if not isinstance(column, pd.Series):
             raise ValueError("column argument must be pandas Series, but was {type(column)}")
         dlist = []
         for _, value in column.items():
-            column_val = []
-            results  = self.map_cell(str(value))
-            if results is None:
-                print(f"Got None results for {str(value)}")
-                dlist.append({"terms": "n/a"})  
-            elif len(results) > 0:
-                for hpterm in results:
-                    column_val.append(f"{hpterm.id} ({hpterm.label}/{hpterm.display_value})")
-                dlist.append({"terms": "; ".join(column_val)})  
-            else:
-                dlist.append({"terms": "n/a"})  
-        return pd.DataFrame(dlist)   
+            value = self.map_cell(str(value))
+            hpterm = value[0]
+            dlist.append({"term": hpterm.hpo_term_and_id, "status": hpterm.display_value})
+        return pd.DataFrame(dlist)
     
-    @staticmethod
-    def autoformat(df: pd.DataFrame, concept_recognizer, delimiter=",") -> str:
-        """Autoformat code from the colums so that we can easily copy-paste and change it.
-        This method intends to save time by preformatting code the create OptionMappers.
-        
+class SimpleColumnMapperGenerator:
+    def __init__(self, df, observed, excluded, hpo_cr) -> None:
+        """Try to map the columns in a dataframe by matching the name of the column to correct HPO term.
+        This class can be used to generate SimpleColumn mappers for exact matches found in the columns names.
         Args:
-            df: data frame with the data about the individuals
-            concept_recognizer: HpoConceptRecognizer for text mining
-            delimiter: the string used to delimit individual items in a cell (default: comma)
-        Return:
-            a string that should be displayed using a print() command in the notebook
-        """  
-        lines = []
-        if not isinstance(df, pd.DataFrame):
-            raise ValueError(f"argument \"df\" must be a pandas DataFrame but was {type(df)}")
-        if not isinstance(concept_recognizer, HpoConceptRecognizer):
-            raise ValueError("concept_recognizer arg must be HpoConceptRecognizer but was {type(concept_recognizer)}")
-        # df.shape[1] gives us the number of columns
-        for y in range(df.shape[1]):
-            temp_dict = {}
-            for i in range(len(df)):
-                if len(str(df.iloc[i, y])) > 1:
-                    for entry in str(df.iloc[i, y]).split(delimiter):
-                        hpo_term = concept_recognizer.parse_cell(entry.strip())
-                        if len(hpo_term) > 0:
-                            temp_dict[entry.strip()] = hpo_term[0].label                
-                        else:
-                            temp_dict[entry.strip()] = 'PLACEHOLDER'
-            col_name = str(df.columns[y]).lower().replace(", ","_").replace(' ', '_')
-            col_name = col_name.lower()
-            # skip columns that are unlikely to be interesting for the OptionColumnMapper
-            if "patient" in col_name:
-                continue
-            if "family" in col_name:
-                continue
-            if "gender" in col_name:
-                continue
-            if "mutation" in col_name or "varia" in col_name:
-                continue
-            if "age" == col_name or "sex" == col_name or "gender" == col_name:
-                continue
-            items_d_name = f"{col_name}_d"
-            items_d_string = str(temp_dict).replace(',', ',\n')
-            lines.append(f"{items_d_name} = {items_d_string}")
-            lines.append(f"{col_name}Mapper = OptionColumnMapper(concept_recognizer=hpo_cr, option_d={items_d_name})")
-            lines.append(f"{col_name}Mapper.preview_column(df['" + str(df.columns[y]) + "']))")
-            lines.append(f"column_mapper_d['{str(df.columns[y])}'] = {col_name}Mapper")
-            lines.append("")
-        return "\n".join(lines)
+            df (dataframe): dataframe with phenotypic data
+            observed (str): symbol used in table if the phenotypic feature was observed
+            excluded (str): symbol used if the feature was excluded
+            hpo_cr (HpoConceptRecognizer): instance of HpoConceptRecognizer to match HPO term and get label/id
+        """
+        self._df = df
+        self._observed = observed
+        self._excluded = excluded
+        self._hpo_cr = hpo_cr
+        self._mapped_columns = []
+        self._unmapped_columns = []
+        self._error_messages = []
         
-   
+    
+    def try_mapping_columns(self) -> List[ColumnMapper]:
+        """As a side effect, this class initializes three lists of mapped, unmapped, and error columns
+
+        Returns:
+            list(ColumnMapper): simple_mappers (dict): dict with successfully mapped columns
+        """
+        simple_mappers = defaultdict(ColumnMapper)
+        for col in self._df.columns:
+            colname = str(col)
+            if self._hpo_cr.contains_term_label(colname):
+                hpo_term_list = self._hpo_cr.parse_cell(colname)
+                hpo_term = hpo_term_list[0]
+                simple_mappers[col] = SimpleColumnMapper(hpo_id=hpo_term.id,
+                                                                    hpo_label=hpo_term.label,
+                                                                    observed=self._observed,
+                                                                    excluded=self._excluded)
+            else:
+                self._unmapped_columns.append(colname)
+        self._mapped_columns = list(simple_mappers.keys())
+        return simple_mappers
+
+
+    def get_unmapped_columns(self):
+        return self._unmapped_columns
+    
+    def get_mapped_columns(self):
+        return self._mapped_columns
+    
+    def to_html(self):
+        """create an HTML table with names of mapped and unmapped columns
+        """
+        table_items = []
+        table_items.append('<table style="border: 2px solid black;">\n')
+        table_items.append("""<tr>
+            <th>Result</th>
+            <th>Columns</th>
+        </tr>
+      """)
+        mapped_str = "; ".join(self._mapped_columns)
+        unmapped_str = "; ".join([f"<q>{colname}</q>" for colname in self._unmapped_columns])
+        def two_item_table_row(cell1, cell2):
+            return f"<tr><td>{cell1}</td><td>{cell2}</td></tr>"
+        table_items.append(two_item_table_row("Mapped", mapped_str))
+        table_items.append(two_item_table_row("Unmapped", unmapped_str))
+        table_items.append('</table>\n') # close table content
+        return "\n".join(table_items)
+
```

### Comparing `pyphetools-0.4.5/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/structural_variant.py` & `pyphetools-0.4.7/pyphetools/creation/structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.4.7/pyphetools/creation/variant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/creation/variant_validator.py` & `pyphetools-0.4.7/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/output/detailed_suppl_table.py` & `pyphetools-0.4.7/pyphetools/output/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/output/focus_count_table.py` & `pyphetools-0.4.7/pyphetools/output/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/output/hpo_category.py` & `pyphetools-0.4.7/pyphetools/output/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.4.7/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/output/phenopacket_table.py` & `pyphetools-0.4.7/pyphetools/output/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/output/simple_patient.py` & `pyphetools-0.4.7/pyphetools/output/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/output/simple_variant.py` & `pyphetools-0.4.7/pyphetools/output/simple_variant.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         vdescript = vinterpretation.variation_descriptor
         if vdescript.gene_context is not None:
             self._gene_id = vdescript.gene_context.value_id
             self._gene_symbol = vdescript.gene_context.symbol
         else:
             self._gene_id = NA_STRING
             self._gene_symbol = NA_STRING
+        self._hgvs = NA_STRING
         if vdescript.expressions is not None and len(vdescript.expressions) > 0:
-            self._hgvs = NA_STRING
             for exprsn in vdescript.expressions:
                 if exprsn.syntax == "hgvs.c":
                     self._hgvs = exprsn.value       
         if vdescript.vcf_record is not None:
             vcf = vdescript.vcf_record
             self._genome_ass = vcf.genome_assembly
             self._chrom = vcf.chrom
```

### Comparing `pyphetools-0.4.5/pyphetools/output/term_count.py` & `pyphetools-0.4.7/pyphetools/output/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/validation/content_validator.py` & `pyphetools-0.4.7/pyphetools/validation/content_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools/validation/validation_result.py` & `pyphetools-0.4.7/pyphetools/validation/validation_result.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.4.7/pyphetools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.5
+Version: 0.4.7
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.5/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.4.7/pyphetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/pyproject.toml` & `pyphetools-0.4.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.4.5"
+version = "0.4.7"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `pyphetools-0.4.5/test/test_age_column_mapper.py` & `pyphetools-0.4.7/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_case_encoder.py` & `pyphetools-0.4.7/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_column_mapper.py` & `pyphetools-0.4.7/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_constant_column_mapper.py` & `pyphetools-0.4.7/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_custom_column_mapper.py` & `pyphetools-0.4.7/test/test_custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_hp_term.py` & `pyphetools-0.4.7/test/test_hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_hpo_category.py` & `pyphetools-0.4.7/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_hpo_cr.py` & `pyphetools-0.4.7/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_hpo_parser.py` & `pyphetools-0.4.7/test/test_hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_option_column_mapper.py` & `pyphetools-0.4.7/test/test_option_column_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,17 @@
         self.assertEqual("Broad hallux", hpterm1.label)
         self.assertEqual("HP:0010055", hpterm1.id)
 
     def test_options_negative(self):
         thumb_d = {"BT": "Broad thumb",
                    "BH": "Broad hallux",
                    "+": ["Broad thumb", "Broad hallux"]}
+        excluded_d = {"-":"Broad thumb"}
         thumbMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=thumb_d,
-                                         negative_symbol="-", negative_label="Broad thumb")
+                                         excluded_d=excluded_d)
         res = thumbMapper.map_cell("-")
         self.assertIsNotNone(res)
         self.assertEqual(1, len(res))
         hpterm0 = res[0]
         self.assertEqual("Broad thumb", hpterm0.label)
         self.assertEqual("HP:0011304", hpterm0.id)
         self.assertFalse(hpterm0.observed)
```

### Comparing `pyphetools-0.4.5/test/test_structural_variant.py` & `pyphetools-0.4.7/test/test_structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_threshold_column_mapper.py` & `pyphetools-0.4.7/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/test/test_variant.py` & `pyphetools-0.4.7/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2html.py` & `pyphetools-0.4.7/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2html4.py` & `pyphetools-0.4.7/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2html5.py` & `pyphetools-0.4.7/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2latex.py` & `pyphetools-0.4.7/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2man.py` & `pyphetools-0.4.7/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2odt.py` & `pyphetools-0.4.7/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.4.7/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2pseudoxml.py` & `pyphetools-0.4.7/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2s5.py` & `pyphetools-0.4.7/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2xetex.py` & `pyphetools-0.4.7/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rst2xml.py` & `pyphetools-0.4.7/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.5/venv/bin/rstpep2html.py` & `pyphetools-0.4.7/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

