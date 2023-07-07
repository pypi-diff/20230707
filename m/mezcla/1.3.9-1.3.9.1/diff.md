# Comparing `tmp/mezcla-1.3.9.tar.gz` & `tmp/mezcla-1.3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.9.tar", last modified: Wed Jul  5 20:42:19 2023, max compression
+gzip compressed data, was "mezcla-1.3.9.1.tar", last modified: Fri Jul  7 05:50:45 2023, max compression
```

## Comparing `mezcla-1.3.9.tar` & `mezcla-1.3.9.1.tar`

### file list

```diff
@@ -1,165 +1,166 @@
--rw-r--r--   0        0        0      542 2023-04-30 22:44:00.000000 mezcla-1.3.9/.coveragerc
--rw-r--r--   0        0        0     1253 2023-07-04 06:24:29.977415 mezcla-1.3.9/.github/workflows/act.yml
--rw-r--r--   0        0        0     1042 2023-06-01 22:36:35.000000 mezcla-1.3.9/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1937 2023-06-10 03:29:46.000000 mezcla-1.3.9/.gitignore
--rw-r--r--   0        0        0     4950 2023-07-01 21:24:22.402445 mezcla-1.3.9/Dockerfile
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9/LICENSE.txt
--rw-r--r--   0        0        0      777 2022-06-03 04:33:57.000000 mezcla-1.3.9/README.txt
--rw-r--r--   0        0        0      380 2023-06-01 22:36:35.000000 mezcla-1.3.9/TODO.txt
--rw-r--r--   0        0        0      130 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/TODO.md
--rwxr-xr-x   0        0        0     2259 2023-07-04 06:10:43.446939 mezcla-1.3.9/mezcla/__init__.py
--rwxr-xr-x   0        0        0    10872 2023-07-01 01:05:14.785985 mezcla-1.3.9/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    13025 2023-06-18 00:32:33.000000 mezcla-1.3.9/mezcla/audio.py
--rwxr-xr-x   0        0        0     4707 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/bash_ast.py
--rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.000000 mezcla-1.3.9/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25718 2023-07-01 01:12:47.735987 mezcla-1.3.9/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     7625 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     9241 2023-06-29 05:58:21.372447 mezcla-1.3.9/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14284 2023-07-01 01:05:14.785985 mezcla-1.3.9/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0     3145 2023-07-02 23:54:56.761692 mezcla-1.3.9/mezcla/convert_emoticons.py
--rwxr-xr-x   0        0        0    22279 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/cut.py
--rwxr-xr-x   0        0        0     4307 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    48772 2023-07-05 20:15:46.458028 mezcla-1.3.9/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12874 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3644 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/download_user_gist.py
--rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.000000 mezcla-1.3.9/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.000000 mezcla-1.3.9/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8811 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0    30001 2023-07-05 20:16:25.630128 mezcla-1.3.9/mezcla/examples/hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     3338 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     3922 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.9/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.9/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.000000 mezcla-1.3.9/mezcla/examples/plot_forest_importances.py
--rwxr-xr-x   0        0        0    13004 2023-07-01 01:56:03.422567 mezcla-1.3.9/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     2068 2023-07-02 23:30:29.556473 mezcla-1.3.9/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0     5070 2023-06-29 06:26:07.199936 mezcla-1.3.9/mezcla/examples/tests/test_hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     3617 2023-07-01 01:05:14.793985 mezcla-1.3.9/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     4031 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     7708 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.9/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32976 2023-07-01 21:43:17.040662 mezcla-1.3.9/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    33811 2023-07-03 00:58:21.152566 mezcla-1.3.9/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    35278 2023-07-05 20:22:18.399100 mezcla-1.3.9/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17916 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    46774 2023-07-02 23:33:30.418758 mezcla-1.3.9/mezcla/main.py
--rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11717 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0    11648 2023-07-01 01:58:45.279182 mezcla-1.3.9/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0     9993 2023-07-02 23:34:27.331430 mezcla-1.3.9/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    13776 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0      737 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31508 2023-07-01 01:12:47.743987 mezcla-1.3.9/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      828 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     7053 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     7604 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.9/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.000000 mezcla-1.3.9/mezcla/run_bert_classifier.py
--rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    19931 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3011 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.9/mezcla/sys_version_info_hack.py
--rwxr-xr-x   0        0        0    51914 2023-07-05 20:23:04.687235 mezcla-1.3.9/mezcla/system.py
--rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     5625 2023-07-02 23:50:24.908274 mezcla-1.3.9/mezcla/template.py
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      462 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/TODO.md
--rw-r--r--   0        0        0     1082 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/adhoc-tests.batspp
--rw-r--r--   0        0        0      204 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/misc-tests.batspp
--rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.000000 mezcla-1.3.9/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0      810 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/resources/cars-csv-len-3.txt
--rw-r--r--   0        0        0      113 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      602 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/resources/cars-tsv-len-3.txt
--rw-r--r--   0        0        0      659 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      655 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0       65 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/word-POS.freq
--rw-r--r--   0        0        0      254 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     4836 2023-07-02 23:52:07.820771 mezcla-1.3.9/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     2489 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/test___init__.py
--rwxr-xr-x   0        0        0     4736 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0      834 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     1974 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_compute_tfidf.py
--rw-r--r--   0        0        0     3523 2023-07-02 23:26:56.041382 mezcla-1.3.9/mezcla/tests/test_convert_emoticons.py
--rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    16047 2023-07-01 02:00:52.582153 mezcla-1.3.9/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     1030 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0     3449 2023-07-01 21:45:57.905414 mezcla-1.3.9/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    15711 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13008 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0      892 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     2114 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0     8972 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     6565 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     2886 2023-07-01 02:02:49.768496 mezcla-1.3.9/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0      916 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0      991 2023-07-01 01:12:47.747987 mezcla-1.3.9/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8297 2023-07-01 01:12:47.747987 mezcla-1.3.9/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0     1183 2023-07-01 02:02:49.768496 mezcla-1.3.9/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0      854 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2873 2023-07-01 02:02:49.768496 mezcla-1.3.9/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0      916 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     2083 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    33490 2023-07-04 06:33:21.263049 mezcla-1.3.9/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     1769 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     3714 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0     7264 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7362 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    21785 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0      725 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0      686 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_transpose_data.py
--rwxr-xr-x   0        0        0     2859 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_xml_utils.py
--rwxr-xr-x   0        0        0      676 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_corpus.py
--rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_dockeyword.py
--rwxr-xr-x   0        0        0      688 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_document.py
--rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    33820 2023-07-01 01:05:14.801984 mezcla-1.3.9/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    23204 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    16223 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.000000 mezcla-1.3.9/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0    18423 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     2282 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7983 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/document.py
-lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.000000 mezcla-1.3.9/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
--rwxr-xr-x   0        0        0    16168 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/preprocess.py
--rwxr-xr-x   0        0        0    59922 2023-07-01 01:05:14.805985 mezcla-1.3.9/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.9/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.9/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/transpose_data.py
--rwxr-xr-x   0        0        0    13455 2023-07-02 23:53:11.409104 mezcla-1.3.9/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.9/mezcla/xml_utils.py
--rw-r--r--   0        0        0      958 2022-06-03 04:33:57.000000 mezcla-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     2469 2023-07-01 05:11:48.148105 mezcla-1.3.9/requirements.txt
--rwxr-xr-x   0        0        0     1162 2023-07-04 06:10:43.450939 mezcla-1.3.9/setup.py
--rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.000000 mezcla-1.3.9/temp/simple_batspp.py
--rw-r--r--   0        0        0      697 2023-07-01 19:46:38.387644 mezcla-1.3.9/tools/local-workflows.sh
--rwxr-xr-x   0        0        0      862 2023-06-01 22:36:35.000000 mezcla-1.3.9/tools/run_tests.bash
--rw-r--r--   0        0        0      612 2023-06-01 22:36:35.000000 mezcla-1.3.9/tox.ini
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/.coveragerc
+-rw-r--r--   0        0        0     1253 2023-07-04 06:24:29.977415 mezcla-1.3.9.1/.github/workflows/act.yml
+-rw-r--r--   0        0        0     1138 2023-07-06 21:26:09.495920 mezcla-1.3.9.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1996 2023-07-05 22:24:53.748059 mezcla-1.3.9.1/.gitignore
+-rw-r--r--   0        0        0     4950 2023-07-06 18:59:36.543927 mezcla-1.3.9.1/Dockerfile
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/LICENSE.txt
+-rw-r--r--   0        0        0      777 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/README.txt
+-rw-r--r--   0        0        0      380 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/TODO.txt
+-rw-r--r--   0        0        0      130 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/TODO.md
+-rwxr-xr-x   0        0        0     2261 2023-07-06 23:03:45.553197 mezcla-1.3.9.1/mezcla/__init__.py
+-rwxr-xr-x   0        0        0     1196 2023-07-06 23:04:24.377280 mezcla-1.3.9.1/mezcla/__main__.py
+-rwxr-xr-x   0        0        0    10872 2023-07-01 01:05:14.785985 mezcla-1.3.9.1/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    13025 2023-06-18 00:32:33.000000 mezcla-1.3.9.1/mezcla/audio.py
+-rwxr-xr-x   0        0        0     4707 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/bash_ast.py
+-rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.000000 mezcla-1.3.9.1/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25718 2023-07-01 01:12:47.735987 mezcla-1.3.9.1/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     7625 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     9241 2023-06-29 05:58:21.372447 mezcla-1.3.9.1/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14284 2023-07-01 01:05:14.785985 mezcla-1.3.9.1/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0     3145 2023-07-02 23:54:56.761692 mezcla-1.3.9.1/mezcla/convert_emoticons.py
+-rwxr-xr-x   0        0        0    22279 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4307 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    49448 2023-07-06 18:32:47.183393 mezcla-1.3.9.1/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12874 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3644 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/download_user_gist.py
+-rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.000000 mezcla-1.3.9.1/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.000000 mezcla-1.3.9.1/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8811 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0    30001 2023-07-05 20:16:25.630128 mezcla-1.3.9.1/mezcla/examples/hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3338 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     3922 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.9.1/mezcla/examples/iris.csv
+-rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.9.1/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.000000 mezcla-1.3.9.1/mezcla/examples/plot_forest_importances.py
+-rwxr-xr-x   0        0        0    13004 2023-07-01 01:56:03.422567 mezcla-1.3.9.1/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     2068 2023-07-02 23:30:29.556473 mezcla-1.3.9.1/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0     5070 2023-06-29 06:26:07.199936 mezcla-1.3.9.1/mezcla/examples/tests/test_hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3617 2023-07-01 01:05:14.793985 mezcla-1.3.9.1/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     4031 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     7708 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.9.1/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32976 2023-07-01 21:43:17.040662 mezcla-1.3.9.1/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    33907 2023-07-06 18:39:58.553067 mezcla-1.3.9.1/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0    35278 2023-07-05 20:22:18.399100 mezcla-1.3.9.1/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17916 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    46774 2023-07-02 23:33:30.418758 mezcla-1.3.9.1/mezcla/main.py
+-rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11717 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0    11648 2023-07-01 01:58:45.279182 mezcla-1.3.9.1/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0     9993 2023-07-02 23:34:27.331430 mezcla-1.3.9.1/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    13776 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0      737 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31508 2023-07-01 01:12:47.743987 mezcla-1.3.9.1/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      828 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     7053 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     7604 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.9.1/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.000000 mezcla-1.3.9.1/mezcla/run_bert_classifier.py
+-rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    19931 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3011 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.9.1/mezcla/sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    51914 2023-07-05 20:23:04.687235 mezcla-1.3.9.1/mezcla/system.py
+-rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     5625 2023-07-02 23:50:24.908274 mezcla-1.3.9.1/mezcla/template.py
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      462 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/TODO.md
+-rw-r--r--   0        0        0     1082 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/adhoc-tests.batspp
+-rw-r--r--   0        0        0      204 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/misc-tests.batspp
+-rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/mezcla/tests/misc_doctests.py
+-rw-r--r--   0        0        0      810 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars-csv-len-3.txt
+-rw-r--r--   0        0        0      113 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      602 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars-tsv-len-3.txt
+-rw-r--r--   0        0        0      659 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      655 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0       65 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/word-POS.freq
+-rw-r--r--   0        0        0      254 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     4836 2023-07-02 23:52:07.820771 mezcla-1.3.9.1/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     2489 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/test___init__.py
+-rwxr-xr-x   0        0        0     4736 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0      834 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     1974 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_compute_tfidf.py
+-rw-r--r--   0        0        0     3523 2023-07-02 23:26:56.041382 mezcla-1.3.9.1/mezcla/tests/test_convert_emoticons.py
+-rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    16047 2023-07-01 02:00:52.582153 mezcla-1.3.9.1/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     1030 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0     3449 2023-07-01 21:45:57.905414 mezcla-1.3.9.1/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    15711 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0    13008 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0      892 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     2114 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0     8972 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     6565 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     2886 2023-07-01 02:02:49.768496 mezcla-1.3.9.1/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0      916 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0      991 2023-07-01 01:12:47.747987 mezcla-1.3.9.1/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8297 2023-07-01 01:12:47.747987 mezcla-1.3.9.1/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0     1183 2023-07-01 02:02:49.768496 mezcla-1.3.9.1/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0      854 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2873 2023-07-01 02:02:49.768496 mezcla-1.3.9.1/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0      916 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     2083 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    33490 2023-07-04 06:33:21.263049 mezcla-1.3.9.1/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     1769 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     3714 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0     7264 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7362 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    21785 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0      725 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0      686 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_transpose_data.py
+-rwxr-xr-x   0        0        0     2859 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_xml_utils.py
+-rwxr-xr-x   0        0        0      676 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_corpus.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_dockeyword.py
+-rwxr-xr-x   0        0        0      688 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_document.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    33820 2023-07-01 01:05:14.801984 mezcla-1.3.9.1/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    23204 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    16223 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.000000 mezcla-1.3.9.1/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0    18423 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     2282 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7983 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/document.py
+lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
+-rwxr-xr-x   0        0        0    16168 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/preprocess.py
+-rwxr-xr-x   0        0        0    59922 2023-07-01 01:05:14.805985 mezcla-1.3.9.1/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.9.1/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.9.1/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/transpose_data.py
+-rwxr-xr-x   0        0        0    13455 2023-07-02 23:53:11.409104 mezcla-1.3.9.1/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.9.1/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      753 2023-07-07 05:49:33.581744 mezcla-1.3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2469 2023-07-01 05:11:48.148105 mezcla-1.3.9.1/requirements.txt
+-rwxr-xr-x   0        0        0     1243 2023-07-06 23:03:45.553197 mezcla-1.3.9.1/setup.py
+-rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.000000 mezcla-1.3.9.1/temp/simple_batspp.py
+-rw-r--r--   0        0        0      697 2023-07-01 19:46:38.387644 mezcla-1.3.9.1/tools/local-workflows.sh
+-rwxr-xr-x   0        0        0      862 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/tools/run_tests.bash
+-rw-r--r--   0        0        0      612 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/tox.ini
+-rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 mezcla-1.3.9.1/PKG-INFO
```

### Comparing `mezcla-1.3.9/.coveragerc` & `mezcla-1.3.9.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/.github/workflows/act.yml` & `mezcla-1.3.9.1/.github/workflows/act.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/.github/workflows/tests.yml` & `mezcla-1.3.9.1/.github/workflows/tests.yml`

 * *Files 19% similar despite different names*

```diff
@@ -18,13 +18,16 @@
 on: [push, pull_request]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
+
     - name: Build docker image
       run: |
         docker build -t mezcla-dev -f- . <Dockerfile
+
     - name: Run tests
       run: |
+        ## TODO???: put repo under /mnt/local-mezcla and installed version under /home/mezcla
         docker run --rm --mount type=bind,source="$(pwd)",target=/home/mezcla mezcla-dev
```

### Comparing `mezcla-1.3.9/.gitignore` & `mezcla-1.3.9.1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 #
 
 # Log files and listings
 # TODO: figure out how to apply to subdirs
 **/*.log
 **/*.list
 
-# Any files with leading _, except specified cases
+# Any files with leading _, except specified cases (e.g., __xyz__.py)
+# TODO2?: _xyz.py
 **/_*
-!**/*__init__.py
+## OLD: !**/*__init__.py
+!**/*__*__.py
 # Likewise for trailing _'s (e.g., master-dir-link_)
 **/*_
 
 # Special cases
 # TODO: see why excluded by the rules
 # Workflow files (e.g., .github/workflows/tests.yml).
 !.github/**
```

### Comparing `mezcla-1.3.9/Dockerfile` & `mezcla-1.3.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/LICENSE.txt` & `mezcla-1.3.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/README.txt` & `mezcla-1.3.9.1/README.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/__init__.py` & `mezcla-1.3.9.1/mezcla/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-__VERSION__ = '1.3.9'
+__VERSION__ = '1.3.9.1'
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
 PYTHON3_PLUS = (sys.version_info[0] >= 3)
```

### Comparing `mezcla-1.3.9/mezcla/analyze_tfidf.py` & `mezcla-1.3.9.1/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/audio.py` & `mezcla-1.3.9.1/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/bash_ast.py` & `mezcla-1.3.9.1/mezcla/bash_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/bert_multi_classification.py` & `mezcla-1.3.9.1/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/bert_text_classification.py` & `mezcla-1.3.9.1/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/bing_search.py` & `mezcla-1.3.9.1/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/check_html_javascript.py` & `mezcla-1.3.9.1/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/compute_tfidf.py` & `mezcla-1.3.9.1/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/convert_emoticons.py` & `mezcla-1.3.9.1/mezcla/convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/cut.py` & `mezcla-1.3.9.1/mezcla/cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/data_utils.py` & `mezcla-1.3.9.1/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/debug.py` & `mezcla-1.3.9.1/mezcla/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,14 +623,15 @@
                     ## OLD: statement = str(context).replace(")\\n']", "")
                     statement = str(context).replace("\\n']", "")
                 # Format expression and message
                 # note: removes comments, along with the assertion call prefix and suffix
                 statement = re.sub("#.*$", "", statement)
                 statement = re.sub(r"^(\S*)assertion\(", "", statement)
                 expression = re.sub(r"\);?\s*$", "", statement)
+                expression = re.sub(r",\s*$", "", statement)
                 expression_text = expression
                 qualification_spec = (": " + message) if message else ""
                 # Output information
                 # TODO: omit subsequent warnings
                 trace_fmtd(ALWAYS, "Assertion failed: {expr} (at {file}:{line}){qual}",
                            expr=expression, file=filename, line=line_number, qual=qualification_spec)
             except:
@@ -643,30 +644,45 @@
         """Returns VALUE if at trace LEVEL or higher otherwise None
         Note: inspired by Lisp's convenient IF form without an explicit else: (if test value-if-true)"""
         # EX: (101 if ((get_level() == 1) and val(1, 101)) else None) => 101
         # EX: ((not __debug__) and val(trace_level, 101))) => None
         # TODO: rename as cond_value???
         return (value if (trace_level >= level) else None)
 
+
     def code(level, no_arg_function):
         """Execute NO_ARG_FUNCTION if at trace LEVEL or higher
         Notes:
+        - Use call() for more flexible invocation (e.g., can avoid lambda function)
         - Given the quirks of Python syntax, a two-step process is required:
            debug.code(4, { line1; line2; ...; lineN })
                =>
            def my_stupid_block_workaround(): 
                if __debug__:
                    line1; line2; ...; lineN
            debug.code(4, my_stupid_block_workaround)
         - Lambda functions can be used for simple expression-based functions"""
-        trace_object(VERBOSE, f"code({level}, {no_arg_function})")
+        trace(VERBOSE, f"code({level}, {no_arg_function})")
+        result = None
         if (trace_level >= level):
-            trace_object(QUITE_DETAILED, f"Executing {no_arg_function}")
-            no_arg_function()
-        return
+            trace(QUITE_DETAILED, f"Executing {no_arg_function}")
+            result = no_arg_function()
+        return result
+
+    
+    def call(level, function, *args, **kwargs):
+        """Invoke FUNCTION with ARGS and KWARGS if at trace LEVEL or higher
+        Note: Use code() for simpler invocation (e.g., via lambda function)
+        """
+        trace(VERBOSE, f"call({level}, {function}, a={args}, kw={kwargs})")
+        result = None
+        if (trace_level >= level):
+            trace(QUITE_DETAILED, f"Executing {function}")
+            result = function(*args, **kwargs)
+        return result
 
 else:
 
     trace_level = 0
     
     def non_debug_stub(*_args, **_kwargs):
         """Non-debug stub (i.e., no-op function)"""
@@ -702,14 +718,16 @@
     
     raise_exception = non_debug_stub
     
     assertion = non_debug_stub
 
     code = non_debug_stub
 
+    call = non_debug_stub
+
     ## TODO?:
     ## val = non_debug_stub
     ##
     def val(_expression):
         """Non-debug stub for value()--a no-op function"""
         # Note: implemented separately from non_debug_stub to ensure no return value
         return
```

### Comparing `mezcla-1.3.9/mezcla/docs/audio_uml.svg` & `mezcla-1.3.9.1/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.3.9.1/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.3.9.1/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/consume_all_memory.py` & `mezcla-1.3.9.1/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/download_user_gist.py` & `mezcla-1.3.9.1/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/dump_checkpoints.py` & `mezcla-1.3.9.1/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/encoded-iris.csv` & `mezcla-1.3.9.1/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/feature_importance.py` & `mezcla-1.3.9.1/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.3.9.1/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/hf_stable_diffusion.py` & `mezcla-1.3.9.1/mezcla/examples/hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.3.9.1/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/hugging_face_translation.py` & `mezcla-1.3.9.1/mezcla/examples/hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.3.9.1/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/iris.csv` & `mezcla-1.3.9.1/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.3.9.1/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/plot_forest_importances.py` & `mezcla-1.3.9.1/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.3.9.1/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/template.py` & `mezcla-1.3.9.1/mezcla/examples/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.3.9.1/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/tests/test_hf_stable_diffusion.py` & `mezcla-1.3.9.1/mezcla/examples/tests/test_hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/examples/tracemalloc_display.py` & `mezcla-1.3.9.1/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/extract_document_text.py` & `mezcla-1.3.9.1/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/file_utils.py` & `mezcla-1.3.9.1/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/filter_random.py` & `mezcla-1.3.9.1/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/format_profile.py` & `mezcla-1.3.9.1/mezcla/format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/gensim_test.py` & `mezcla-1.3.9.1/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/glue_helpers.py` & `mezcla-1.3.9.1/mezcla/glue_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,29 +312,30 @@
     Note: Invoked in unittest_wrapper.py"""
     tpo.debug_print("disable_subcommand_tracing()", 7)
     # Note this works by having run() temporarily setting DEBUG_LEVEL to 0."""
     global default_subtrace_level
     default_subtrace_level = 0
 
 
-def run(command, trace_level=4, subtrace_level=None, just_issue=False, **namespace):
+def run(command, trace_level=4, subtrace_level=None, just_issue=False, output=False, **namespace):
     """Invokes COMMAND via system shell, using TRACE_LEVEL for debugging output, returning result. The command can use format-style templates, resolved from caller's namespace. The optional SUBTRACE_LEVEL sets tracing for invoked commands (default is same as TRACE_LEVEL); this works around problem with stderr not being separated, which can be a problem when tracing unit tests.
    Notes:
    - The result includes stderr, so direct if not desired (see issue):
          run("ls /tmp/fubar 2> /dev/null")
    - This is only intended for running simple commands. It would be better to create a subprocess for any complex interactions.
    - This function doesn't work fully under Win32. Tabs are not preserved, so redirect stdout to a file if needed.
    - If TEMP_FILE or TEMP_BASE defined, these are modified to be unique to avoid conflicts across processeses.
+    - If OUTPUT, the result will be printed.
    """
     # TODO: add automatic log file support as in run_script from unittest_wrapper.py
     # TODO: make sure no template markers left in command text (e.g., "tar cvfz {tar_file}")
     # EX: "root" in run("ls /")
     # Note: Script tracing controlled DEBUG_LEVEL environment variable.
     debug.assertion(isinstance(trace_level, int))
-    debug_print("run(%s, [trace_level=%s], [subtrace_level=%s])" % (command, trace_level, subtrace_level), (trace_level + 2))
+    debug.trace(trace_level + 2, f"run({command}, tl={trace_level}, sub_tr={subtrace_level}, iss={just_issue}, out={output}")
     global default_subtrace_level
     # Keep track of current debug level setting
     debug_level_env = None
     if subtrace_level is None:
         subtrace_level = default_subtrace_level
     if subtrace_level != trace_level:
         debug_level_env = os.getenv("DEBUG_LEVEL")
@@ -359,14 +360,16 @@
     # it is not supported under Windows. To avoid unexpected porting issues, clients
     # should replace 'run("... >| f")' usages with 'delete_file(f); run(...)'.
     # note: TestWrapper.setUp handles the deletion automatically
     debug.assertion(">|" not in command_line)
     result = None
     ## TODO: if (just_issue or not wait): ... else: ...
     result = getoutput(command_line) if wait else str(os.system(command_line))
+    if output:
+        print(result)
     # Restore debug level setting in environment
     if debug_level_env:
         setenv("DEBUG_LEVEL", debug_level_env)
     if save_temp_base:
         setenv("TEMP_BASE", save_temp_base)
     if save_temp_file:
         setenv("TEMP_FILE", save_temp_file)
```

### Comparing `mezcla-1.3.9/mezcla/html_utils.py` & `mezcla-1.3.9.1/mezcla/html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/kenlm_example.py` & `mezcla-1.3.9.1/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/keras_param_search.py` & `mezcla-1.3.9.1/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/main.py` & `mezcla-1.3.9.1/mezcla/main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/merge_files.py` & `mezcla-1.3.9.1/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/merge_notes.py` & `mezcla-1.3.9.1/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/misc_utils.py` & `mezcla-1.3.9.1/mezcla/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/my_regex.py` & `mezcla-1.3.9.1/mezcla/my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/ngram_tfidf.py` & `mezcla-1.3.9.1/mezcla/ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/os_utils.py` & `mezcla-1.3.9.1/mezcla/os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/pandas_sklearn.py` & `mezcla-1.3.9.1/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/plot_utils.py` & `mezcla-1.3.9.1/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/randomize_lines.py` & `mezcla-1.3.9.1/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/rgb_color_name.py` & `mezcla-1.3.9.1/mezcla/rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/run_albert_classifier.py` & `mezcla-1.3.9.1/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/run_bert_classifier.py` & `mezcla-1.3.9.1/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/show_bert_representation.py` & `mezcla-1.3.9.1/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/simple_main_example.py` & `mezcla-1.3.9.1/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/spacy_nlp.py` & `mezcla-1.3.9.1/mezcla/spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/spell.py` & `mezcla-1.3.9.1/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/sys_version_info_hack.py` & `mezcla-1.3.9.1/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/system.py` & `mezcla-1.3.9.1/mezcla/system.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/temp/simple_batspp.py` & `mezcla-1.3.9.1/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/template.py` & `mezcla-1.3.9.1/mezcla/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/LICENSE.txt` & `mezcla-1.3.9.1/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.3.9.1/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/misc_doctests.py` & `mezcla-1.3.9.1/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/cars-csv-len-3.txt` & `mezcla-1.3.9.1/mezcla/tests/resources/cars-csv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/cars-tsv-len-3.txt` & `mezcla-1.3.9.1/mezcla/tests/resources/cars-tsv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/cars.csv` & `mezcla-1.3.9.1/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/cars.tsv` & `mezcla-1.3.9.1/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/example_text.txt` & `mezcla-1.3.9.1/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.3.9.1/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/iris_output.txt` & `mezcla-1.3.9.1/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.3.9.1/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/template.py` & `mezcla-1.3.9.1/mezcla/tests/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test___init__.py` & `mezcla-1.3.9.1/mezcla/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_audio.py` & `mezcla-1.3.9.1/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.3.9.1/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_bing_search.py` & `mezcla-1.3.9.1/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.3.9.1/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_convert_emoticons.py` & `mezcla-1.3.9.1/mezcla/tests/test_convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_cut.py` & `mezcla-1.3.9.1/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_data_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_debug.py` & `mezcla-1.3.9.1/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_extract_document_text.py` & `mezcla-1.3.9.1/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_file_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_filter_random.py` & `mezcla-1.3.9.1/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_gensim_test.py` & `mezcla-1.3.9.1/mezcla/tests/test_gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_glue_helpers.py` & `mezcla-1.3.9.1/mezcla/tests/test_glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_html_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_kenlm_example.py` & `mezcla-1.3.9.1/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_keras_param_search.py` & `mezcla-1.3.9.1/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_main.py` & `mezcla-1.3.9.1/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_merge_files.py` & `mezcla-1.3.9.1/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_merge_notes.py` & `mezcla-1.3.9.1/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_misc_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_my_regex.py` & `mezcla-1.3.9.1/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.3.9.1/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_os_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.3.9.1/mezcla/tests/test_pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_plot_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_randomize_lines.py` & `mezcla-1.3.9.1/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.3.9.1/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.3.9.1/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.3.9.1/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.3.9.1/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_simple_main_example.py` & `mezcla-1.3.9.1/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.3.9.1/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.3.9.1/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_system.py` & `mezcla-1.3.9.1/mezcla/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_template.py` & `mezcla-1.3.9.1/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_text_categorizer.py` & `mezcla-1.3.9.1/mezcla/tests/test_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_text_processing.py` & `mezcla-1.3.9.1/mezcla/tests/test_text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_text_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_tpo_common.py` & `mezcla-1.3.9.1/mezcla/tests/test_tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_train_language_model.py` & `mezcla-1.3.9.1/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.3.9.1/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_transpose_data.py` & `mezcla-1.3.9.1/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/test_xml_utils.py` & `mezcla-1.3.9.1/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.3.9.1/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.3.9.1/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/tfidf/test_document.py` & `mezcla-1.3.9.1/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.3.9.1/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/text_categorizer.py` & `mezcla-1.3.9.1/mezcla/text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/text_processing.py` & `mezcla-1.3.9.1/mezcla/text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/text_utils.py` & `mezcla-1.3.9.1/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tfidf/corpus.py` & `mezcla-1.3.9.1/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tfidf/dockeyword.py` & `mezcla-1.3.9.1/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tfidf/document.py` & `mezcla-1.3.9.1/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tfidf/preprocess.py` & `mezcla-1.3.9.1/mezcla/tfidf/preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/tpo_common.py` & `mezcla-1.3.9.1/mezcla/tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/train_language_model.py` & `mezcla-1.3.9.1/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/train_text_categorizer.py` & `mezcla-1.3.9.1/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/transpose_data.py` & `mezcla-1.3.9.1/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/unittest_wrapper.py` & `mezcla-1.3.9.1/mezcla/unittest_wrapper.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/mezcla/xml_utils.py` & `mezcla-1.3.9.1/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/pyproject.toml` & `mezcla-1.3.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 ## TODO: eliminate redundancy
 
 [tool.poetry]
-## name = "mezcla"
-## version = "1.1.1"
+name = "mezcla"
+version = "1.3.9.1"
 description = "Miscellaneous Python scripts developed over the course of several independent consulting projects. [Mezcla is Spanish for mixture.]"
 authors = ["Tom O'Hara <tomasohara@gmail.com>"]
 license = "LGPLv3"
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.9"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 realpython = "mezcla.__main__:main"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.flit.metadata]
-## name = "mezcla"
+## note: information taken from setup.py
 module = "mezcla"
-## version = "1.1.1"
-## description = "Miscellaneous Python scripts developed over the course of several independent consulting projects. [Mezcla is Spanish for mixture.]"
-## authors = ["Tom O'Hara <tomasohara@gmail.com>"]
 license = "LGPLv3"
 author="Tomás O'Hara"
 author-email="tomasohara@gmail.com"
 home-page = "https://github.com/tomasohara/mezcla"
 description-file="README.txt"
```

### Comparing `mezcla-1.3.9/requirements.txt` & `mezcla-1.3.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/setup.py` & `mezcla-1.3.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 """Simple installer"""
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla'],
       module="mezcla",
-      version='1.3.9',
+      ## TODO2: import mezcla; version=mezcla.VERSION
+      version='1.3.9.1',
       description-file="README.txt",
       dist-name="Mezcla",
-      ## OLD: py_modules=PYTHON_MODULE_NAMES,
       author="Tom O'Hara",
-      # TODO: find out which email key is preferred
+      # TODO3: find out which email key is preferred
       email="tomasohara@gmail.com",
       author-email="tomasohara@gmail.com"
-      requires-python=">=3.6",
-      ## TODO:
+      requires-python=">=3.8",
+      ## TODO4?:
       ## install_requires=["six"],
       home-page="https://github.com/tomasohara/Mezcla",
       classifiers=[
           "License :: OSI Approved :: LGPLv3",
           "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.7",
+          "Programming Language :: Python :: 3.8",
       ]
       description="""
 Package with core modules from https://github.com/tomasohara/misc-utility
 note: mezcla is Spanish for mixture.
 """)
+# TODO1: Muchas gracias a Bruno y Tana; <thanks in Tibet> to Aviyan
 
 [tool.flit.scripts]
 realpython = "mezcla.__main__:main"
```

### Comparing `mezcla-1.3.9/temp/simple_batspp.py` & `mezcla-1.3.9.1/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/tools/local-workflows.sh` & `mezcla-1.3.9.1/tools/local-workflows.sh`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/tools/run_tests.bash` & `mezcla-1.3.9.1/tools/run_tests.bash`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/tox.ini` & `mezcla-1.3.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9/PKG-INFO` & `mezcla-1.3.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.3.9
+Version: 1.3.9.1
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
```

