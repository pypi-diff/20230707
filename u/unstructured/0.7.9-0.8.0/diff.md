# Comparing `tmp/unstructured-0.7.9.tar.gz` & `tmp/unstructured-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.9.tar", last modified: Mon Jun 26 21:56:55 2023, max compression
+gzip compressed data, was "unstructured-0.8.0.tar", last modified: Fri Jul  7 15:46:52 2023, max compression
```

## Comparing `unstructured-0.7.9.tar` & `unstructured-0.8.0.tar`

### file list

```diff
@@ -1,134 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.377841 unstructured-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-26 21:56:47.000000 unstructured-0.7.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-26 21:56:47.000000 unstructured-0.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-06-26 21:56:55.377841 unstructured-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-06-26 21:56:47.000000 unstructured-0.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.361840 unstructured-0.7.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:56:47.000000 unstructured-0.7.9/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-26 21:56:55.377841 unstructured-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-26 21:56:47.000000 unstructured-0.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.361840 unstructured-0.7.9/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-26 21:56:47.000000 unstructured-0.7.9/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.369840 unstructured-0.7.9/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.369840 unstructured-0.7.9/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26315 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.369840 unstructured-0.7.9/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.373841 unstructured-0.7.9/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.377841 unstructured-0.7.9/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.377841 unstructured-0.7.9/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-26 21:56:47.000000 unstructured-0.7.9/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:55.365840 unstructured-0.7.9/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:56:55.000000 unstructured-0.7.9/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.844953 unstructured-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-07 15:46:44.000000 unstructured-0.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 15:46:44.000000 unstructured-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19205 2023-07-07 15:46:52.844953 unstructured-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-07 15:46:44.000000 unstructured-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.828952 unstructured-0.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 15:46:44.000000 unstructured-0.8.0/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-07 15:46:52.844953 unstructured-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-07 15:46:44.000000 unstructured-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.828952 unstructured-0.8.0/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.828952 unstructured-0.8.0/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-07 15:46:44.000000 unstructured-0.8.0/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.832953 unstructured-0.8.0/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.832953 unstructured-0.8.0/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28317 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.836953 unstructured-0.8.0/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.840953 unstructured-0.8.0/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.844953 unstructured-0.8.0/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.844953 unstructured-0.8.0/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-07 15:46:44.000000 unstructured-0.8.0/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:46:52.832953 unstructured-0.8.0/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19205 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 15:46:52.000000 unstructured-0.8.0/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.9/LICENSE.md` & `unstructured-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/PKG-INFO` & `unstructured-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.9
+Version: 0.8.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -38,16 +38,16 @@
         </div>
         
         <h3 align="center">
           <p>API Announcement!</p>
         </h3>
         
         <p>While access to the hosted Unstructured API will remain free, API Keys will soon be required to make requests. To prevent any disruption, get yours <a href="https://www.unstructured.io/api-key/">here</a> now and start using it today!</p>
-          
-        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. 
+        
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls.
         We'd love to hear your feedback, let us know how it goes in our
           community slack. And stay tuned for improvements to both quality and performance!</p>
         
         <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
@@ -102,35 +102,35 @@
         the partitioning function listed in the table directly.
         See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
         about the library.
         
         | Document Type | Partition Function | Strategies | Table Support | Options |
         | --- | --- | --- | --- | --- |
         | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
-        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
-        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
+        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max Partition; Process Attachments |
+        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding; Max Partition; Process Attachments |
         | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
         | Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
-        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
+        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR Languages, Strategy |
+        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding; Max Partition; Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
         | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
-        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
+        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags |
         
         
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
@@ -311,7 +311,9 @@
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
 Provides-Extra: gcs
+Provides-Extra: elasticsearch
+Provides-Extra: dropbox
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.9 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -60,38 +60,40 @@
 `unstructured` library currently supports. `partition` will recognize each of
 these document types and route the document to the appropriate partitioning
 function. If you already know your document type, you can use the partitioning
 function listed in the table directly. See our [documentation page](https://
 unstructured-io.github.io/unstructured/) for more details about the library. |
 Document Type | Partition Function | Strategies | Table Support | Options | | -
 -- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
-| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
-(`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
+| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max
+Partition; Process Attachments | | E-mails (`.msg`) | `partition_msg` | N/A |
+No | Encoding; Max Partition; Process Attachments | | EPubs (`.epub`) |
 `partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
 (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
 | `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
 (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
 Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
-Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
-Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
-Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
-Include Page Breaks | | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None
-| | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | | Word
-Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | Word Documents
-(`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
-(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
-Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
-:dizzy: Instructions for using the docker image The following instructions are
+| Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR
+Languages, Strategy | | Plain Text (`.txt`) | `partition_text` | N/A | No |
+Encoding; Max Partition; Paragraph Grouper | | Power Points (`.ppt`) |
+`partition_ppt` | N/A | Yes | Include Page Breaks | | Power Points (`.pptx`) |
+`partition_pptx` | N/A | Yes | Include Page Breaks | | ReStructured Text
+(`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks | | Rich Text
+Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks | | TSV
+Files (`.tsv`) | `partition_tsv` | N/A | Yes | None | | Word Documents (`.doc`)
+| `partition_doc` | N/A | Yes | None | | Word Documents (`.docx`) |
+`partition_docx` | N/A | Yes | None | | Word Documents (`.doc`) |
+`partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents (`.docx`)
+| `partition_docx` | N/A | Yes | Include Page Breaks | | XML Documents (`.xml`)
+| `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags | ## :
+dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
 with `--platform` (e.g. `--platform linux/amd64`) if needed. We build Docker
 images for all pushes to `main`. We tag each image with the corresponding short
@@ -205,8 +207,8 @@
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
 Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
 discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
 Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
-Provides-Extra: gcs
+Provides-Extra: gcs Provides-Extra: elasticsearch Provides-Extra: dropbox
```

### Comparing `unstructured-0.7.9/README.md` & `unstructured-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 </div>
 
 <h3 align="center">
   <p>API Announcement!</p>
 </h3>
 
 <p>While access to the hosted Unstructured API will remain free, API Keys will soon be required to make requests. To prevent any disruption, get yours <a href="https://www.unstructured.io/api-key/">here</a> now and start using it today!</p>
-  
-<p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. 
+
+<p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls.
 We'd love to hear your feedback, let us know how it goes in our
   community slack. And stay tuned for improvements to both quality and performance!</p>
 
 <h3 align="center">
   <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
 </h3>
 
@@ -94,35 +94,35 @@
 the partitioning function listed in the table directly.
 See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
 about the library.
 
 | Document Type | Partition Function | Strategies | Table Support | Options |
 | --- | --- | --- | --- | --- |
 | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
-| E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
-| E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
+| E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max Partition; Process Attachments |
+| E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding; Max Partition; Process Attachments |
 | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
 | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
 | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
 | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
 | Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
 | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
-| PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-| Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
+| PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR Languages, Strategy |
+| Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding; Max Partition; Paragraph Grouper |
 | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
 | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
 | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
 | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
 | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
 | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
 | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
 | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
 | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
-| XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
+| XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags |
 
 
 
 ## :dizzy: Instructions for using the docker image
 
 The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
 See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
```

#### html2text {}

```diff
@@ -56,38 +56,40 @@
 `unstructured` library currently supports. `partition` will recognize each of
 these document types and route the document to the appropriate partitioning
 function. If you already know your document type, you can use the partitioning
 function listed in the table directly. See our [documentation page](https://
 unstructured-io.github.io/unstructured/) for more details about the library. |
 Document Type | Partition Function | Strategies | Table Support | Options | | -
 -- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
-| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
-(`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
+| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max
+Partition; Process Attachments | | E-mails (`.msg`) | `partition_msg` | N/A |
+No | Encoding; Max Partition; Process Attachments | | EPubs (`.epub`) |
 `partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
 (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
 | `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
 (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
 Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
-Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
-Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
-Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
-Include Page Breaks | | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None
-| | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | | Word
-Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | Word Documents
-(`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
-(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
-Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
-:dizzy: Instructions for using the docker image The following instructions are
+| Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR
+Languages, Strategy | | Plain Text (`.txt`) | `partition_text` | N/A | No |
+Encoding; Max Partition; Paragraph Grouper | | Power Points (`.ppt`) |
+`partition_ppt` | N/A | Yes | Include Page Breaks | | Power Points (`.pptx`) |
+`partition_pptx` | N/A | Yes | Include Page Breaks | | ReStructured Text
+(`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks | | Rich Text
+Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks | | TSV
+Files (`.tsv`) | `partition_tsv` | N/A | Yes | None | | Word Documents (`.doc`)
+| `partition_doc` | N/A | Yes | None | | Word Documents (`.docx`) |
+`partition_docx` | N/A | Yes | None | | Word Documents (`.doc`) |
+`partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents (`.docx`)
+| `partition_docx` | N/A | Yes | Include Page Breaks | | XML Documents (`.xml`)
+| `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags | ## :
+dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
 with `--platform` (e.g. `--platform linux/amd64`) if needed. We build Docker
 images for all pushes to `main`. We tag each image with the corresponding short
```

### Comparing `unstructured-0.7.9/setup.py` & `unstructured-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,11 +78,13 @@
         "github": load_requirements("requirements/ingest-github.in"),
         "gitlab": load_requirements("requirements/ingest-gitlab.in"),
         "reddit": load_requirements("requirements/ingest-reddit.in"),
         "slack": load_requirements("requirements/ingest-slack.in"),
         "wikipedia": load_requirements("requirements/ingest-wikipedia.in"),
         "google-drive": load_requirements("requirements/ingest-google-drive.in"),
         "gcs": load_requirements("requirements/ingest-gcs.in"),
+        "elasticsearch": load_requirements("requirements/ingest-elasticsearch.in"),
+        "dropbox": load_requirements("requirements/ingest-dropbox.in"),
     },
     package_dir={"unstructured": "unstructured"},
     package_data={"unstructured": ["nlp/*.txt"]},
 )
```

### Comparing `unstructured-0.7.9/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.8.0/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.8.0/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/test_unstructured/test_utils.py` & `unstructured-0.8.0/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/cleaners/core.py` & `unstructured-0.8.0/unstructured/cleaners/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import quopri
 import re
 import sys
 import unicodedata
 
+from unstructured.file_utils.encoding import (
+    format_encoding_str,
+)
 from unstructured.nlp.patterns import (
     DOUBLE_PARAGRAPH_PATTERN_RE,
     PARAGRAPH_PATTERN,
     PARAGRAPH_PATTERN_RE,
     UNICODE_BULLETS_RE,
 )
 
@@ -190,15 +193,16 @@
 def replace_mime_encodings(text: str, encoding: str = "utf-8") -> str:
     """Replaces MIME encodings with their equivalent characters in the specified encoding.
 
     Example
     -------
     5 w=E2=80-99s -> 5 w’s
     """
-    return quopri.decodestring(text.encode(encoding)).decode(encoding)
+    formatted_encoding = format_encoding_str(encoding)
+    return quopri.decodestring(text.encode(formatted_encoding)).decode(formatted_encoding)
 
 
 def clean_prefix(text: str, pattern: str, ignore_case: bool = False, strip: bool = True) -> str:
     """Removes prefixes from a string according to the specified pattern. Strips leading
     whitespace if the strip parameter is set to True.
 
     Input
@@ -260,8 +264,9 @@
     return cleaned_text.strip()
 
 
 def bytes_string_to_string(text: str, encoding: str = "utf-8"):
     """Converts a string representation of a byte string to a regular string using the
     specified encoding."""
     text_bytes = bytes([ord(char) for char in text])
-    return text_bytes.decode(encoding)
+    formatted_encoding = format_encoding_str(encoding)
+    return text_bytes.decode(formatted_encoding)
```

### Comparing `unstructured-0.7.9/unstructured/cleaners/extract.py` & `unstructured-0.8.0/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/cleaners/translate.py` & `unstructured-0.8.0/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/documents/base.py` & `unstructured-0.8.0/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/documents/coordinates.py` & `unstructured-0.8.0/unstructured/documents/coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Tuple, Union
+from typing import Any, Dict, Tuple, Union
 
 
 class Orientation(Enum):
     SCREEN = (1, -1)  # Origin in top left, y increases in the down direction
     CARTESIAN = (1, 1)  # Origin in bottom left, y increases in upward direction
 
 
@@ -87,7 +87,14 @@
 
 
 class PointSpace(CoordinateSystem):
     """Coordinate system representing a point space, such as a pdf. The origin is at the top
     right."""
 
     orientation = Orientation.CARTESIAN
+
+
+TYPE_TO_COORDINATE_SYSTEM_MAP: Dict[str, Any] = {
+    "PixelSpace": PixelSpace,
+    "PointSpace": PointSpace,
+    "CoordinateSystem": CoordinateSystem,
+}
```

### Comparing `unstructured-0.7.9/unstructured/documents/elements.py` & `unstructured-0.8.0/unstructured/partition/pdf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,424 +1,380 @@
-from __future__ import annotations
-
-import datetime
-import hashlib
-import inspect
 import os
-import pathlib
 import re
-from abc import ABC
-from dataclasses import dataclass
-from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Tuple, TypedDict, Union, cast
-
-from unstructured.documents.coordinates import CoordinateSystem
-
-
-class NoID(ABC):
-    """Class to indicate that an element do not have an ID."""
-
-    pass
-
-
-@dataclass
-class DataSourceMetadata:
-    """Metadata fields that pertain to the data source of the document."""
-
-    url: Optional[str] = None
-    version: Optional[str] = None
-    record_locator: Optional[Dict[str, Any]] = None  # Values must be JSON-serializable
-    date_created: Optional[str] = None
-    date_modified: Optional[str] = None
-    date_processed: Optional[str] = None
-
-    def to_dict(self):
-        return {key: value for key, value in self.__dict__.items() if value is not None}
-
-
-class RegexMetadata(TypedDict):
-    """Metadata that is extracted from a document element via regex."""
-
-    text: str
-    start: int
-    end: int
-
-
-@dataclass
-class ElementMetadata:
-    data_source: Optional[DataSourceMetadata] = None
-    filename: Optional[str] = None
-    file_directory: Optional[str] = None
-    date: Optional[str] = None
-    filetype: Optional[str] = None
-
-    # Page numbers currenlty supported for PDF, HTML and PPT documents
-    page_number: Optional[int] = None
-
-    # Page name. The sheet name in XLXS documents.
-    page_name: Optional[str] = None
-
-    # Webpage specific metadata fields
-    url: Optional[str] = None
-
-    # E-mail specific metadata fields
-    sent_from: Optional[List[str]] = None
-    sent_to: Optional[List[str]] = None
-    subject: Optional[str] = None
-
-    # MSFT Word specific metadata fields
-    header_footer_type: Optional[str] = None
-
-    # Text format metadata fields
-    text_as_html: Optional[str] = None
-
-    # Metadata extracted via regex
-    regex_metadata: Optional[Dict[str, List[RegexMetadata]]] = None
-
-    def __post_init__(self):
-        if isinstance(self.filename, pathlib.Path):
-            self.filename = str(self.filename)
-
-        if self.filename is not None:
-            file_directory, filename = os.path.split(self.filename)
-            self.file_directory = file_directory or None
-            self.filename = filename
-
-    def to_dict(self):
-        _dict = {key: value for key, value in self.__dict__.items() if value is not None}
-        if "regex_metadata" in _dict and not _dict["regex_metadata"]:
-            _dict.pop("regex_metadata")
-        if self.data_source:
-            _dict["data_source"] = cast(DataSourceMetadata, self.data_source).to_dict()
-        return _dict
-
-    @classmethod
-    def from_dict(cls, input_dict):
-        return cls(**input_dict)
-
-    def merge(self, other: ElementMetadata):
-        for k in self.__dict__:
-            if getattr(self, k) is None:
-                setattr(self, k, getattr(other, k))
-        return self
-
-    def get_date(self) -> Optional[datetime.datetime]:
-        """Converts the date field to a datetime object."""
-        dt = None
-        if self.date is not None:
-            dt = datetime.datetime.fromisoformat(self.date)
-        return dt
-
-
-def process_metadata():
-    """Decorator for processing metadata for document elements."""
-
-    def decorator(func: Callable):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            elements = func(*args, **kwargs)
-            sig = inspect.signature(func)
-            params = dict(**dict(zip(sig.parameters, args)), **kwargs)
-            for param in sig.parameters.values():
-                if param.name not in params and param.default is not param.empty:
-                    params[param.name] = param.default
-
-            regex_metadata: Dict["str", "str"] = params.get("regex_metadata", {})
-            elements = _add_regex_metadata(elements, regex_metadata)
-
-            return elements
-
-        return wrapper
-
-    return decorator
-
-
-def _add_regex_metadata(
-    elements: List[Element],
-    regex_metadata: Dict[str, str] = {},
+import warnings
+from tempfile import SpooledTemporaryFile
+from typing import BinaryIO, List, Optional, Union, cast
+
+import pdf2image
+import PIL
+from pdfminer.high_level import extract_pages
+from pdfminer.layout import LTContainer, LTImage, LTItem, LTTextBox
+from pdfminer.utils import open_filename
+
+from unstructured.cleaners.core import clean_extra_whitespace
+from unstructured.documents.coordinates import PixelSpace
+from unstructured.documents.elements import (
+    CoordinatesMetadata,
+    Element,
+    ElementMetadata,
+    Image,
+    PageBreak,
+    Text,
+    process_metadata,
+)
+from unstructured.file_utils.filetype import (
+    FileType,
+    add_metadata_with_filetype,
+    document_to_element_list,
+)
+from unstructured.nlp.patterns import PARAGRAPH_PATTERN
+from unstructured.partition.common import (
+    exactly_one,
+    spooled_to_bytes_io_if_needed,
+)
+from unstructured.partition.strategies import determine_pdf_or_image_strategy
+from unstructured.partition.text import element_from_text, partition_text
+from unstructured.utils import requires_dependencies
+
+RE_MULTISPACE_INCLUDING_NEWLINES = re.compile(pattern=r"\s+", flags=re.DOTALL)
+
+
+@process_metadata()
+@add_metadata_with_filetype(FileType.PDF)
+def partition_pdf(
+    filename: str = "",
+    file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
+    include_page_breaks: bool = False,
+    strategy: str = "auto",
+    infer_table_structure: bool = False,
+    ocr_languages: str = "eng",
+    max_partition: Optional[int] = 1500,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
+    **kwargs,
 ) -> List[Element]:
-    """Adds metadata based on a user provided regular expression.
-    The additional metadata will be added to the regex_metadata
-    attrbuted in the element metadata."""
-    for element in elements:
-        if isinstance(element, Text):
-            _regex_metadata: Dict["str", List[RegexMetadata]] = {}
-            for field_name, pattern in regex_metadata.items():
-                results: List[RegexMetadata] = []
-                for result in re.finditer(pattern, element.text):
-                    start, end = result.span()
-                    results.append(
-                        {
-                            "text": element.text[start:end],
-                            "start": start,
-                            "end": end,
-                        },
-                    )
-                if len(results) > 0:
-                    _regex_metadata[field_name] = results
+    """Parses a pdf document into a list of interpreted elements.
+    Parameters
+    ----------
+    filename
+        A string defining the target filename path.
+    file
+        A file-like object as bytes --> open(filename, "rb").
+    strategy
+        The strategy to use for partitioning the PDF. Valid strategies are "hi_res",
+        "ocr_only", and "fast". When using the "hi_res" strategy, the function uses
+        a layout detection model to identify document elements. When using the
+        "ocr_only" strategy, partition_pdf simply extracts the text from the
+        document using OCR and processes it. If the "fast" strategy is used, the text
+        is extracted directly from the PDF. The default strategy `auto` will determine
+        when a page can be extracted using `fast` mode, otherwise it will fall back to `hi_res`.
+    infer_table_structure
+        Only applicable if `strategy=hi_res`.
+        If True, any Table elements that are extracted will also have a metadata field
+        named "text_as_html" where the table's text content is rendered into an html string.
+        I.e., rows and cells are preserved.
+        Whether True or False, the "text" field is always present in any Table element
+        and is the text content of the table (no structure).
+    ocr_languages
+        The languages to use for the Tesseract agent. To use a language, you'll first need
+        to isntall the appropriate Tesseract language pack.
+    max_partition
+        The maximum number of characters to include in a partition. If None is passed,
+        no maximum is applied. Only applies to the "ocr_only" strategy.
+    """
+    exactly_one(filename=filename, file=file)
+    return partition_pdf_or_image(
+        filename=filename,
+        file=file,
+        include_page_breaks=include_page_breaks,
+        strategy=strategy,
+        infer_table_structure=infer_table_structure,
+        ocr_languages=ocr_languages,
+        max_partition=max_partition,
+        **kwargs,
+    )
+
+
+def partition_pdf_or_image(
+    filename: str = "",
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
+    is_image: bool = False,
+    include_page_breaks: bool = False,
+    strategy: str = "auto",
+    infer_table_structure: bool = False,
+    ocr_languages: str = "eng",
+    max_partition: Optional[int] = 1500,
+    **kwargs,
+) -> List[Element]:
+    """Parses a pdf or image document into a list of interpreted elements."""
+    # TODO(alan): Extract information about the filetype to be processed from the template
+    # route. Decoding the routing should probably be handled by a single function designed for
+    # that task so as routing design changes, those changes are implemented in a single
+    # function.
+
+    strategy = determine_pdf_or_image_strategy(
+        strategy,
+        filename=filename,
+        file=file,
+        is_image=is_image,
+        infer_table_structure=infer_table_structure,
+    )
+
+    if strategy == "hi_res":
+        # NOTE(robinson): Catches a UserWarning that occurs when detectron is called
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            layout_elements = _partition_pdf_or_image_local(
+                filename=filename,
+                file=spooled_to_bytes_io_if_needed(file),
+                is_image=is_image,
+                infer_table_structure=infer_table_structure,
+                include_page_breaks=include_page_breaks,
+                ocr_languages=ocr_languages,
+                **kwargs,
+            )
 
-            element.metadata.regex_metadata = _regex_metadata
+    elif strategy == "fast":
+        return _partition_pdf_with_pdfminer(
+            filename=filename,
+            file=spooled_to_bytes_io_if_needed(file),
+            include_page_breaks=include_page_breaks,
+        )
 
-    return elements
+    elif strategy == "ocr_only":
+        # NOTE(robinson): Catches file conversion warnings when running with PDFs
+        with warnings.catch_warnings():
+            return _partition_pdf_or_image_with_ocr(
+                filename=filename,
+                file=file,
+                include_page_breaks=include_page_breaks,
+                ocr_languages=ocr_languages,
+                is_image=is_image,
+                max_partition=max_partition,
+            )
 
+    return layout_elements
 
-class Element(ABC):
-    """An element is a section of a page in the document."""
 
-    def __init__(
-        self,
-        element_id: Union[str, NoID] = NoID(),
-        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
-        coordinate_system: Optional[CoordinateSystem] = None,
-        metadata: ElementMetadata = ElementMetadata(),
-    ):
-        self.id: Union[str, NoID] = element_id
-        self.coordinates: Optional[Tuple[Tuple[float, float], ...]] = coordinates
-        self._coordinate_system = coordinate_system
-        self.metadata = metadata
-
-    def to_dict(self) -> dict:
-        return {
-            "type": None,
-            "coordinates": self.coordinates,
-            "coordinate_system": None
-            if self._coordinate_system is None
-            else str(self._coordinate_system.__class__.__name__),
-            "layout_width": None
-            if self._coordinate_system is None
-            else self._coordinate_system.width,
-            "layout_height": None
-            if self._coordinate_system is None
-            else self._coordinate_system.height,
-            "element_id": self.id,
-            "metadata": self.metadata.to_dict(),
-        }
-
-    def convert_coordinates_to_new_system(
-        self,
-        new_system: CoordinateSystem,
-        in_place=True,
-    ) -> Optional[Tuple[Tuple[Union[int, float], Union[int, float]], ...]]:
-        """Converts the element location coordinates to a new coordinate system. If inplace is true,
-        changes the coordinates in place and updates the coordinate system."""
-        if self._coordinate_system is None or self.coordinates is None:
-            return None
-        new_coordinates = tuple(
-            self._coordinate_system.convert_coordinates_to_new_system(
-                new_system=new_system,
-                x=x,
-                y=y,
-            )
-            for x, y in self.coordinates
-        )
-        if in_place:
-            self.coordinates = new_coordinates
-            self._coordinate_system = new_system
-        return new_coordinates
-
-    @property
-    def coordinate_system(self) -> Optional[Dict[str, Optional[Union[str, int, float]]]]:
-        if self._coordinate_system is None:
-            return None
-        return {
-            "name": self._coordinate_system.__class__.__name__,
-            "description": self._coordinate_system.__doc__,
-            "layout_width": self._coordinate_system.width,
-            "layout_height": self._coordinate_system.height,
-        }
-
-
-class CheckBox(Element):
-    """A checkbox with an attribute indicating whether its checked or not. Primarily used
-    in documents that are forms"""
-
-    def __init__(
-        self,
-        element_id: Union[str, NoID] = NoID(),
-        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
-        coordinate_system: Optional[CoordinateSystem] = None,
-        checked: bool = False,
-        metadata: ElementMetadata = ElementMetadata(),
-    ):
-        super().__init__(
-            element_id=element_id,
-            coordinates=coordinates,
-            coordinate_system=coordinate_system,
-            metadata=metadata,
+@requires_dependencies("unstructured_inference")
+def _partition_pdf_or_image_local(
+    filename: str = "",
+    file: Optional[Union[bytes, BinaryIO]] = None,
+    is_image: bool = False,
+    infer_table_structure: bool = False,
+    include_page_breaks: bool = False,
+    ocr_languages: str = "eng",
+    model_name: Optional[str] = None,
+    **kwargs,
+) -> List[Element]:
+    """Partition using package installed locally."""
+    try:
+        from unstructured_inference.inference.layout import (
+            process_data_with_model,
+            process_file_with_model,
         )
-        self.checked: bool = checked
-
-    def __eq__(self, other):
-        return (self.checked == other.checked) and (self.coordinates) == (other.coordinates)
-
-    def to_dict(self) -> dict:
-        out = super().to_dict()
-        out["type"] = "CheckBox"
-        out["checked"] = self.checked
-        out["element_id"] = self.id
-        return out
-
-
-class Text(Element):
-    """Base element for capturing free text from within document."""
-
-    category = "UncategorizedText"
-
-    def __init__(
-        self,
-        text: str,
-        element_id: Union[str, NoID] = NoID(),
-        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
-        coordinate_system: Optional[CoordinateSystem] = None,
-        metadata: ElementMetadata = ElementMetadata(),
-    ):
-        self.text: str = text
-
-        if isinstance(element_id, NoID):
-            # NOTE(robinson) - Cut the SHA256 hex in half to get the first 128 bits
-            element_id = hashlib.sha256(text.encode()).hexdigest()[:32]
-
-        super().__init__(
-            element_id=element_id,
-            metadata=metadata,
-            coordinates=coordinates,
-            coordinate_system=coordinate_system,
+    except ModuleNotFoundError as e:
+        raise Exception(
+            "unstructured_inference module not found... try running pip install "
+            "unstructured[local-inference] if you installed the unstructured library as a package. "
+            "If you cloned the unstructured repository, try running make install-local-inference "
+            "from the root directory of the repository.",
+        ) from e
+    except ImportError as e:
+        raise Exception(
+            "There was a problem importing unstructured_inference module - it may not be installed "
+            "correctly... try running pip install unstructured[local-inference] if you installed "
+            "the unstructured library as a package. If you cloned the unstructured repository, try "
+            "running make install-local-inference from the root directory of the repository.",
+        ) from e
+
+    model_name = model_name if model_name else os.environ.get("UNSTRUCTURED_HI_RES_MODEL_NAME")
+    if file is None:
+        layout = process_file_with_model(
+            filename,
+            is_image=is_image,
+            ocr_languages=ocr_languages,
+            extract_tables=infer_table_structure,
+            model_name=model_name,
         )
-
-    def __str__(self):
-        return self.text
-
-    def __eq__(self, other):
-        return all(
-            [
-                (self.text == other.text),
-                (self.coordinates == other.coordinates),
-                (self._coordinate_system == other._coordinate_system),
-                (self.category == other.category),
-            ],
+    else:
+        layout = process_data_with_model(
+            file,
+            is_image=is_image,
+            ocr_languages=ocr_languages,
+            extract_tables=infer_table_structure,
+            model_name=model_name,
         )
+    elements = document_to_element_list(layout, include_page_breaks=include_page_breaks, sort=False)
+    out_elements = []
 
-    def to_dict(self) -> dict:
-        out = super().to_dict()
-        out["element_id"] = self.id
-        out["type"] = self.category
-        out["text"] = self.text
-        return out
-
-    def apply(self, *cleaners: Callable):
-        """Applies a cleaning brick to the text element. The function that's passed in
-        should take a string as input and produce a string as output."""
-        cleaned_text = self.text
-        for cleaner in cleaners:
-            cleaned_text = cleaner(cleaned_text)
-
-        if not isinstance(cleaned_text, str):
-            raise ValueError("Cleaner produced a non-string output.")
-
-        self.text = cleaned_text
-
-
-class FigureCaption(Text):
-    """An element for capturing text associated with figure captions."""
-
-    category = "FigureCaption"
-
-    pass
-
-
-class NarrativeText(Text):
-    """NarrativeText is an element consisting of multiple, well-formulated sentences. This
-    excludes elements such titles, headers, footers, and captions."""
-
-    category = "NarrativeText"
-
-    pass
-
-
-class ListItem(Text):
-    """ListItem is a NarrativeText element that is part of a list."""
-
-    category = "ListItem"
-
-    pass
-
-
-class Title(Text):
-    """A text element for capturing titles."""
-
-    category = "Title"
-
-    pass
-
-
-class Address(Text):
-    """A text element for capturing addresses."""
-
-    category = "Address"
-
-    pass
-
-
-class Image(Text):
-    """A text element for capturing image metadata."""
-
-    category = "Image"
-
-    pass
-
-
-class PageBreak(Text):
-    """An element for capturing page breaks."""
-
-    category = "PageBreak"
-
-    def __init__(
-        self,
-        text: Optional[str] = None,
-        element_id: Union[str, NoID] = NoID(),
-        coordinates: Optional[List[float]] = None,
-        coordinate_system: Optional[CoordinateSystem] = None,
-        metadata: ElementMetadata = ElementMetadata(),
-    ):
-        super().__init__(text="<PAGE BREAK>")
-
-
-class Table(Text):
-    """An element for capturing tables."""
+    for el in elements:
+        if (isinstance(el, PageBreak) and not include_page_breaks) or (
+            # NOTE(crag): small chunks of text from Image elements tend to be garbage
+            isinstance(el, Image)
+            and (el.text is None or len(el.text) < 24 or el.text.find(" ") == -1)
+        ):
+            continue
+        # NOTE(crag): this is probably always a Text object, but check for the sake of typing
+        if isinstance(el, Text):
+            el.text = re.sub(RE_MULTISPACE_INCLUDING_NEWLINES, " ", el.text or "").strip()
+            if el.text or isinstance(el, PageBreak):
+                out_elements.append(cast(Element, el))
+
+    return out_elements
+
+
+@requires_dependencies("pdfminer", "local-inference")
+def _partition_pdf_with_pdfminer(
+    filename: str = "",
+    file: Optional[BinaryIO] = None,
+    include_page_breaks: bool = False,
+) -> List[Element]:
+    """Partitions a PDF using PDFMiner instead of using a layoutmodel. Used for faster
+    processing or detectron2 is not available.
 
-    category = "Table"
+    Implementation is based on the `extract_text` implemenation in pdfminer.six, but
+    modified to support tracking page numbers and working with file-like objects.
 
-    pass
+    ref: https://github.com/pdfminer/pdfminer.six/blob/master/pdfminer/high_level.py
+    """
+    exactly_one(filename=filename, file=file)
+    if filename:
+        with open_filename(filename, "rb") as fp:
+            fp = cast(BinaryIO, fp)
+            elements = _process_pdfminer_pages(
+                fp=fp,
+                filename=filename,
+                include_page_breaks=include_page_breaks,
+            )
 
+    elif file:
+        fp = cast(BinaryIO, file)
+        elements = _process_pdfminer_pages(
+            fp=fp,
+            filename=filename,
+            include_page_breaks=include_page_breaks,
+        )
 
-class Header(Text):
-    """An element for capturing document headers."""
+    return elements
 
-    category = "Header"
 
-    pass
+def _extract_text(item: LTItem) -> str:
+    """Recursively extracts text from PDFMiner objects to account
+    for scenarios where the text is in a sub-container."""
+    if hasattr(item, "get_text"):
+        return item.get_text()
+
+    elif isinstance(item, LTContainer):
+        text = ""
+        for child in item:
+            text += _extract_text(child) or ""
+        return text
+
+    elif isinstance(item, (LTTextBox, LTImage)):
+        # TODO(robinson) - Support pulling text out of images
+        # https://github.com/pdfminer/pdfminer.six/blob/master/pdfminer/image.py#L90
+        return "\n"
+    return "\n"
+
+
+def _process_pdfminer_pages(
+    fp: BinaryIO,
+    filename: str = "",
+    include_page_breaks: bool = False,
+):
+    """Uses PDF miner to split a document into pages and process them."""
+    elements: List[Element] = []
+
+    for i, page in enumerate(extract_pages(fp)):  # type: ignore
+        width, height = page.width, page.height
+
+        text_segments = []
+        page_elements = []
+        for obj in page:
+            x1, y2, x2, y1 = obj.bbox
+            y1 = height - y1
+            y2 = height - y2
+
+            if hasattr(obj, "get_text"):
+                _text_snippets = [obj.get_text()]
+            else:
+                _text = _extract_text(obj)
+                _text_snippets = re.split(PARAGRAPH_PATTERN, _text)
+
+            for _text in _text_snippets:
+                _text = clean_extra_whitespace(_text)
+                if _text.strip():
+                    text_segments.append(_text)
+                    element = element_from_text(_text)
+                    coordinate_system = PixelSpace(
+                        width=width,
+                        height=height,
+                    )
+                    points = ((x1, y1), (x1, y2), (x2, y2), (x2, y1))
+                    coordinates_metadata = CoordinatesMetadata(
+                        points=points,
+                        system=coordinate_system,
+                    )
+                    element.metadata = ElementMetadata(
+                        filename=filename,
+                        page_number=i + 1,
+                        coordinates=coordinates_metadata,
+                    )
+                    page_elements.append(element)
 
+        sorted_page_elements = sorted(
+            page_elements,
+            key=lambda el: (
+                el.metadata.coordinates.points[0][1] if el.metadata.coordinates else float("inf"),
+                el.metadata.coordinates.points[0][0] if el.metadata.coordinates else float("inf"),
+                el.id,
+            ),
+        )
+        elements += sorted_page_elements
 
-class Footer(Text):
-    """An element for capturing document footers."""
+        if include_page_breaks:
+            elements.append(PageBreak(text=""))
 
-    category = "Footer"
+    return elements
 
-    pass
 
+@requires_dependencies("pytesseract")
+def _partition_pdf_or_image_with_ocr(
+    filename: str = "",
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
+    include_page_breaks: bool = False,
+    ocr_languages: str = "eng",
+    is_image: bool = False,
+    max_partition: Optional[int] = 1500,
+):
+    """Partitions and image or PDF using Tesseract OCR. For PDFs, each page is converted
+    to an image prior to processing."""
+    import pytesseract
+
+    if is_image:
+        if file is not None:
+            image = PIL.Image.open(file)
+            text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
+        else:
+            text = pytesseract.image_to_string(filename, config=f"-l '{ocr_languages}'")
+        elements = partition_text(text=text, max_partition=max_partition)
+    else:
+        elements = []
+        if file is not None:
+            document = pdf2image.convert_from_bytes(file.read())  # type: ignore
+            file.seek(0)  # type: ignore
+        else:
+            document = pdf2image.convert_from_path(filename)
+
+        for i, image in enumerate(document):
+            metadata = ElementMetadata(filename=filename, page_number=i + 1)
+            text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
+
+            _elements = partition_text(text=text, max_partition=max_partition)
+            for element in _elements:
+                element.metadata = metadata
+                elements.append(element)
 
-TYPE_TO_TEXT_ELEMENT_MAP: Dict[str, Any] = {
-    "UncategorizedText": Text,
-    "FigureCaption": FigureCaption,
-    "Figure": FigureCaption,
-    "Text": NarrativeText,
-    "NarrativeText": NarrativeText,
-    "ListItem": ListItem,
-    "BulletedText": ListItem,
-    "Title": Title,
-    "Address": Address,
-    "Image": Image,
-    "PageBreak": PageBreak,
-    "Table": Table,
-    "Header": Header,
-    "Footer": Footer,
-}
+            if include_page_breaks:
+                elements.append(PageBreak(text=""))
+    return elements
```

### Comparing `unstructured-0.7.9/unstructured/documents/email_elements.py` & `unstructured-0.8.0/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/documents/html.py` & `unstructured-0.8.0/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/documents/xml.py` & `unstructured-0.8.0/unstructured/documents/xml.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import List, Optional, Union
 
 from lxml import etree
 
 from unstructured.documents.base import Document, Page
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.logger import logger
+from unstructured.partition.text import (
+    element_from_text,
+    split_by_paragraph,
+)
 
 VALID_PARSERS = Union[etree.HTMLParser, etree.XMLParser, None]
 
 
 class XMLDocument(Document):
     """Class for handling .xml documents. This class uses rules based parsing to identify
     sections of interest within the document."""
@@ -63,21 +67,33 @@
         if content and not content.startswith("\n") and is_html_parser:
             content = "\n" + content
         if self.document_tree is None:
             try:
                 document_tree = etree.fromstring(content, self.parser)
                 if document_tree is None:
                     raise ValueError("document_tree is None")
+
             # NOTE(robinson) - The following ValueError occurs with unicode strings. In that
             # case, we call back to encoding the string and passing in bytes.
             #     ValueError: Unicode strings with encoding declaration are not supported.
             #     Please use  bytes input or XML fragments without declaration.
             except ValueError:
                 document_tree = etree.fromstring(content.encode(), self.parser)
 
+            if "<pre>" and "</pre>" in content:
+                tree = etree.HTML(content)
+                for element in tree.xpath("//pre"):
+                    if not element.text:
+                        continue
+                    text_content = split_by_paragraph(element.text)
+                    for text in text_content:
+                        element = etree.Element("span")
+                        element.text = str(element_from_text(text=text))
+                        document_tree.append(element)
+
             if self.stylesheet:
                 if isinstance(self.parser, etree.HTMLParser):
                     logger.warning(
                         "You are using the HTML parser with an XSLT stylesheet. "
                         "Stylesheets are more commonly parsed with the "
                         "XMLParser. If your HTML does not display properly, try "
                         "`import lxml.etree as etree` and setting "
```

### Comparing `unstructured-0.7.9/unstructured/file_utils/encoding.py` & `unstructured-0.8.0/unstructured/file_utils/encoding.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import IO, Optional, Tuple, Union
 
 import chardet
 
 from unstructured.partition.common import convert_to_bytes
 
-ENCODE_REC_THRESHOLD = 0.5
+ENCODE_REC_THRESHOLD = 0.8
 
 # popular encodings from https://en.wikipedia.org/wiki/Popularity_of_text_encodings
 COMMON_ENCODINGS = [
     "utf_8",
     "iso_8859_1",
+    "iso_8859_6",
+    "iso_8859_8",
     "ascii",
     "big5",
     "utf_16",
     "utf_16_be",
     "utf_16_le",
     "utf_32",
     "utf_32_be",
@@ -33,20 +35,36 @@
     """Format input encoding string (e.g., `utf-8`, `iso-8859-1`, etc).
     Parameters
     ----------
     encoding
         The encoding string to be formatted (e.g., `UTF-8`, `utf_8`, `ISO-8859-1`, `iso_8859_1`,
         etc).
     """
-    return encoding.lower().replace("_", "-")
+    formatted_encoding = encoding.lower().replace("_", "-")
+
+    # Special case for Arabic and Hebrew charsets with directional annotations
+    annotated_encodings = ["iso-8859-6-i", "iso-8859-6-e", "iso-8859-8-i", "iso-8859-8-e"]
+    if formatted_encoding in annotated_encodings:
+        formatted_encoding = formatted_encoding[:-2]  # remove the annotation
+
+    return formatted_encoding
+
+
+def validate_encoding(encoding: str) -> bool:
+    """Checks if an encoding string is valid. Helps to avoid errors in cases where
+    invalid encodings are extracted from malformed documents."""
+    for common_encoding in COMMON_ENCODINGS:
+        if format_encoding_str(common_encoding) == format_encoding_str(encoding):
+            return True
+    return False
 
 
 def detect_file_encoding(
     filename: str = "",
-    file: Optional[Union[bytes, IO]] = None,
+    file: Optional[Union[bytes, IO[bytes]]] = None,
 ) -> Tuple[str, str]:
     if filename:
         with open(filename, "rb") as f:
             byte_data = f.read()
     elif file:
         byte_data = convert_to_bytes(file)
     else:
@@ -78,43 +96,45 @@
                 len(byte_data),
                 "Invalid encoding",
             )
 
     else:
         file_text = byte_data.decode(encoding)
 
-    return encoding, file_text
+    formatted_encoding = format_encoding_str(encoding)
+
+    return formatted_encoding, file_text
 
 
 def read_txt_file(
     filename: str = "",
-    file: Optional[Union[bytes, IO]] = None,
+    file: Optional[Union[bytes, IO[bytes]]] = None,
     encoding: Optional[str] = None,
 ) -> Tuple[str, str]:
     """Extracts document metadata from a plain text document."""
     if filename:
         if encoding:
-            with open(filename, encoding=encoding) as f:
+            formatted_encoding = format_encoding_str(encoding)
+            with open(filename, encoding=formatted_encoding) as f:
                 try:
                     file_text = f.read()
                 except (UnicodeDecodeError, UnicodeError) as error:
                     raise error
         else:
-            encoding, file_text = detect_file_encoding(filename)
+            formatted_encoding, file_text = detect_file_encoding(filename)
     elif file:
         if encoding:
+            formatted_encoding = format_encoding_str(encoding)
             try:
                 file_content = file if isinstance(file, bytes) else file.read()
                 if isinstance(file_content, bytes):
-                    file_text = file_content.decode(encoding)
+                    file_text = file_content.decode(formatted_encoding)
                 else:
                     file_text = file_content
             except (UnicodeDecodeError, UnicodeError) as error:
                 raise error
         else:
-            encoding, file_text = detect_file_encoding(file=file)
+            formatted_encoding, file_text = detect_file_encoding(file=file)
     else:
         raise FileNotFoundError("No filename was specified")
 
-    formatted_encoding = format_encoding_str(encoding)
-
     return formatted_encoding, file_text
```

### Comparing `unstructured-0.7.9/unstructured/file_utils/exploration.py` & `unstructured-0.8.0/unstructured/file_utils/exploration.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             raise ValueError(
                 f"There are {len(filenames)} filenames and {len(file_contents)} "
                 "file_contents. Both inputs must be the same length.",
             )
         data["filename"] = []
 
     for i, file_content in enumerate(file_contents):
-        _, content_string = file_content.split(",")
+        content_string = file_content.split(",")[-1]
         content_bytes = base64.b64decode(content_string)
         f = io.BytesIO(content_bytes)
         filetype = detect_filetype(file=f)
         f.seek(0, os.SEEK_END)
         filesize = f.tell()
 
         data["filesize"].append(filesize)
```

### Comparing `unstructured-0.7.9/unstructured/file_utils/file_conversion.py` & `unstructured-0.8.0/unstructured/file_utils/file_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     return text
 
 
 def convert_file_to_html_text(
     source_format: str,
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
 ) -> str:
     """Converts a document to HTML raw text. Enables the doucment to be
     processed using the partition_html function."""
     exactly_one(filename=filename, file=file)
 
     if file is not None:
         tmp = tempfile.NamedTemporaryFile(delete=False)
```

### Comparing `unstructured-0.7.9/unstructured/file_utils/filetype.py` & `unstructured-0.8.0/unstructured/file_utils/filetype.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import zipfile
 from enum import Enum
 from functools import wraps
 from typing import IO, TYPE_CHECKING, Callable, List, Optional
 
 from unstructured.documents.coordinates import PixelSpace
 from unstructured.documents.elements import Element, PageBreak
-from unstructured.file_utils.encoding import detect_file_encoding
+from unstructured.file_utils.encoding import detect_file_encoding, format_encoding_str
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import (
     _add_element_metadata,
     _remove_element_metadata,
     exactly_one,
     normalize_layout_element,
 )
@@ -203,15 +203,15 @@
         file_path = os.path.realpath(file_path)
     return file_path
 
 
 def detect_filetype(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     file_filename: Optional[str] = None,
     encoding: Optional[str] = "utf-8",
 ) -> Optional[FileType]:
     """Use libmagic to determine a file's type. Helps determine which partition brick
     to use for a given file. A return value of None indicates a non-supported file type.
     """
     mime_type = None
@@ -254,15 +254,15 @@
             mime_type = magic.from_buffer(file.read(4096), mime=True)
         else:
             import filetype as ft
 
             mime_type = ft.guess_mime(file.read(4096))
         if mime_type is None:
             logger.warning(
-                "libmagic is unavailable but assists in filetype detection on file-like objects."
+                "libmagic is unavailable but assists in filetype detection on file-like objects. "
                 "Please consider installing libmagic for better results.",
             )
             return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
     else:
         raise ValueError("No filename, file, nor file_filename were specified.")
 
@@ -276,29 +276,33 @@
     elif mime_type.endswith("xml"):
         if extension == ".html" or extension == ".htm":
             return FileType.HTML
         else:
             return FileType.XML
 
     elif mime_type in TXT_MIME_TYPES or mime_type.startswith("text"):
+        if not encoding:
+            encoding = "utf-8"
+        formatted_encoding = format_encoding_str(encoding)
+
+        if extension in [".eml", ".md", ".rtf", ".html", ".rst", ".org", ".csv", ".tsv", ".json"]:
+            return EXT_TO_FILETYPE.get(extension)
+
         # NOTE(crag): for older versions of the OS libmagic package, such as is currently
         # installed on the Unstructured docker image, .json files resolve to "text/plain"
         # rather than "application/json". this corrects for that case.
-        if _is_text_file_a_json(file=file, filename=filename, encoding=encoding):
+        if _is_text_file_a_json(file=file, filename=filename, encoding=formatted_encoding):
             return FileType.JSON
 
-        if _is_text_file_a_csv(file=file, filename=filename, encoding=encoding):
+        if _is_text_file_a_csv(file=file, filename=filename, encoding=formatted_encoding):
             return FileType.CSV
 
         if file and _check_eml_from_buffer(file=file) is True:
             return FileType.EML
 
-        if extension in [".eml", ".md", ".rtf", ".html", ".rst", ".org", ".tsv", ".json"]:
-            return EXT_TO_FILETYPE.get(extension)
-
         # Safety catch
         if mime_type in STR_TO_FILETYPE:
             return STR_TO_FILETYPE[mime_type]
 
         return FileType.TXT
 
     elif mime_type == "application/octet-stream":
@@ -362,15 +366,15 @@
         "Could not detect the filetype from application/octet-stream MIME type.",
     )
     return FileType.UNK
 
 
 def _read_file_start_for_type_check(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     encoding: Optional[str] = "utf-8",
 ) -> str:
     """Reads the start of the file and returns the text content."""
     exactly_one(filename=filename, file=file)
     if file is not None:
         file.seek(0)
         file_content = file.read(4096)
@@ -380,45 +384,52 @@
             file_text = file_content.decode(errors="ignore")
         file.seek(0)
     if filename is not None:
         try:
             with open(filename, encoding=encoding) as f:
                 file_text = f.read(4096)
         except UnicodeDecodeError:
-            encoding, _ = detect_file_encoding(filename=filename)
-            with open(filename, encoding=encoding) as f:
+            formatted_encoding, _ = detect_file_encoding(filename=filename)
+            with open(filename, encoding=formatted_encoding) as f:
                 file_text = f.read(4096)
     return file_text
 
 
 def _is_text_file_a_json(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     encoding: Optional[str] = "utf-8",
 ):
     """Detects if a file that has a text/plain MIME type is a JSON file."""
     file_text = _read_file_start_for_type_check(file=file, filename=filename, encoding=encoding)
     return re.match(LIST_OF_DICTS_PATTERN, file_text) is not None
 
 
+def _count_commas(text: str):
+    """Counts the number of commas in a line, excluding commas in quotes."""
+    pattern = r"(?=(?:[^\"]*\"[^\"]*\")*[^\"]*$),"
+    matches = re.findall(pattern, text)
+    return len(matches)
+
+
 def _is_text_file_a_csv(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     encoding: Optional[str] = "utf-8",
 ):
     """Detects if a file that has a text/plain MIME type is a CSV file."""
     file_text = _read_file_start_for_type_check(file=file, filename=filename, encoding=encoding)
     lines = file_text.strip().splitlines()
     if len(lines) < 2:
         return False
     lines = lines[: len(lines)] if len(lines) < 10 else lines[:10]
-    header = lines[0].split(",")
+    header_count = _count_commas(lines[0])
     if any("," not in line for line in lines):
         return False
-    return all(len(line.split(",")) == len(header) for line in lines[:-1])
+    return all(_count_commas(line) == header_count for line in lines[:1])
 
 
 def _check_eml_from_buffer(file: IO) -> bool:
     """Checks if a text/plain file is actually a .eml file. Uses a regex pattern to see if the
     start of the file matches the typical pattern for a .eml file."""
     file.seek(0)
     file_content = file.read(4096)
@@ -428,41 +439,65 @@
         file_head = file_content
     return EMAIL_HEAD_RE.match(file_head) is not None
 
 
 def document_to_element_list(
     document: "DocumentLayout",
     include_page_breaks: bool = False,
+    sort: bool = False,
 ) -> List[Element]:
     """Converts a DocumentLayout object to a list of unstructured elements."""
     elements: List[Element] = []
     num_pages = len(document.pages)
     for i, page in enumerate(document.pages):
+        page_elements: List[Element] = []
         for layout_element in page.elements:
-            element = normalize_layout_element(layout_element)
+            if hasattr(page, "image"):
+                image_format = page.image.format
+                coordinate_system = PixelSpace(width=page.image.width, height=page.image.height)
+            else:
+                image_format = None
+                coordinate_system = None
+            element = normalize_layout_element(layout_element, coordinate_system=coordinate_system)
             if isinstance(element, List):
                 for el in element:
                     el.metadata.page_number = i + 1
-                elements.extend(element)
+                page_elements.extend(element)
                 continue
             else:
                 element.metadata.text_as_html = (
                     layout_element.text_as_html if hasattr(layout_element, "text_as_html") else None
                 )
-                elements.append(element)
-            if hasattr(page, "image"):
-                image_format = page.image.format
-                coordinate_system = PixelSpace(width=page.image.width, height=page.image.height)
-            else:
-                image_format = None
-                coordinate_system = None
-            element._coordinate_system = coordinate_system
-            _add_element_metadata(element, page_number=i + 1, filetype=image_format)
+                page_elements.append(element)
+            coordinates = (
+                element.metadata.coordinates.points if element.metadata.coordinates else None
+            )
+            _add_element_metadata(
+                element,
+                page_number=i + 1,
+                filetype=image_format,
+                coordinates=coordinates,
+                coordinate_system=coordinate_system,
+            )
+        if sort:
+            page_elements = sorted(
+                page_elements,
+                key=lambda el: (
+                    el.metadata.coordinates.points[0][1]
+                    if el.metadata.coordinates
+                    else float("inf"),
+                    el.metadata.coordinates.points[0][0]
+                    if el.metadata.coordinates
+                    else float("inf"),
+                    el.id,
+                ),
+            )
         if include_page_breaks and i < num_pages - 1:
-            elements.append(PageBreak())
+            page_elements.append(PageBreak(text=""))
+        elements.extend(page_elements)
 
     return elements
 
 
 PROGRAMMING_LANGUAGES = [
     "javascript",
     "python",
@@ -497,23 +532,30 @@
             sig = inspect.signature(func)
             params = dict(**dict(zip(sig.parameters, args)), **kwargs)
             for param in sig.parameters.values():
                 if param.name not in params and param.default is not param.empty:
                     params[param.name] = param.default
             include_metadata = params.get("include_metadata", True)
             if include_metadata:
+                if params.get("metadata_filename"):
+                    params["filename"] = params.get("metadata_filename")
+
                 metadata_kwargs = {
                     kwarg: params.get(kwarg) for kwarg in ("filename", "url", "text_as_html")
                 }
+
                 for element in elements:
-                    _add_element_metadata(
-                        element,
-                        filetype=FILETYPE_TO_MIMETYPE[filetype],
-                        **metadata_kwargs,  # type: ignore
-                    )
+                    # NOTE(robinson) - Attached files have already run through this logic
+                    # in their own partitioning function
+                    if element.metadata.attached_to_filename is None:
+                        _add_element_metadata(
+                            element,
+                            filetype=FILETYPE_TO_MIMETYPE[filetype],
+                            **metadata_kwargs,  # type: ignore
+                        )
 
                 return elements
             else:
                 return _remove_element_metadata(
                     elements,
                 )
```

### Comparing `unstructured-0.7.9/unstructured/file_utils/metadata.py` & `unstructured-0.8.0/unstructured/file_utils/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def to_dict(self):
         return self.__dict__
 
 
 def get_docx_metadata(
     filename: str = "",
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
 ) -> Metadata:
     """Extracts document metadata from a Microsoft .docx document."""
     if filename:
         doc = docx.Document(filename)
     elif file:
         doc = docx.Document(file)
     else:
@@ -70,15 +70,15 @@
     )
 
     return metadata
 
 
 def get_xlsx_metadata(
     filename: str = "",
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
 ) -> Metadata:
     """Extracts document metadata from a Microsoft .xlsx document."""
     if filename:
         workbook = openpyxl.load_workbook(filename)
     elif file:
         workbook = openpyxl.load_workbook(file)
     else:
@@ -104,15 +104,15 @@
     )
 
     return metadata
 
 
 def get_jpg_metadata(
     filename: str = "",
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
 ) -> Metadata:
     """Extracts metadata from a JPG image, including EXIF metadata."""
     if filename:
         image = Image.open(filename)
     elif file:
         image = Image.open(io.BytesIO(file.read()))
     else:
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/azure.py` & `unstructured-0.8.0/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/biomed.py` & `unstructured-0.8.0/unstructured/ingest/connector/biomed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 import urllib.request
 from dataclasses import dataclass
 from ftplib import FTP, error_perm
 from pathlib import Path
 from typing import List, Union
 
@@ -11,14 +10,16 @@
 from requests.adapters import HTTPAdapter
 from urllib3.util import Retry
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    ConnectorCleanupMixin,
+    IngestDocCleanupMixin,
     StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 from unstructured.utils import (
     validate_date_args,
 )
 
@@ -102,83 +103,62 @@
                 else:
                     raise ValueError(
                         "Something went wrong when validating the path: {path}.",
                     )
 
 
 @dataclass
-class BiomedIngestDoc(BaseIngestDoc):
+class BiomedIngestDoc(IngestDocCleanupMixin, BaseIngestDoc):
     config: SimpleBiomedConfig
     file_meta: BiomedFileMeta
 
     @property
     def filename(self):
         return Path(self.file_meta.download_filepath).resolve()  # type: ignore
 
+    @property
     def _output_filename(self):
         return Path(f"{self.file_meta.output_filepath}.json").resolve()
 
     def cleanup_file(self):
         if (
             not self.standard_config.preserve_downloads
             and self.filename.is_file()
             and not self.standard_config.download_only
         ):
             logger.debug(f"Cleaning up {self}")
             Path.unlink(self.filename)
 
-    def has_output(self):
-        """Determine if structured output for this doc already exists."""
-        output_filename = self._output_filename()
-        return output_filename.is_file() and output_filename.stat()
-
+    @BaseIngestDoc.skip_if_file_exists
     def get_file(self):
         download_path = self.file_meta.download_filepath  # type: ignore
-
         dir_ = Path(os.path.dirname(download_path))  # type: ignore
         if not dir_.is_dir():
             logger.debug(f"Creating directory: {dir_}")
 
             if dir_:
                 dir_.mkdir(parents=True, exist_ok=True)
-
         urllib.request.urlretrieve(
             self.file_meta.ftp_path,  # type: ignore
             self.file_meta.download_filepath,
         )
-
         logger.debug(f"File downloaded: {self.file_meta.download_filepath}")
 
-    def write_result(self):
-        """Write the structured json result for this doc. result must be json serializable."""
-        if self.standard_config.download_only:
-            return
-        output_filename = self._output_filename()
-        output_filename.parent.mkdir(parents=True, exist_ok=True)
-        with open(output_filename, "w") as output_f:
-            output_f.write(
-                json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2),
-            )
-        logger.info(f"Wrote {output_filename}")
-
 
-class BiomedConnector(BaseConnector):
+class BiomedConnector(ConnectorCleanupMixin, BaseConnector):
     """Objects of this class support fetching documents from Biomedical literature FTP directory"""
 
     config: SimpleBiomedConfig
 
     def __init__(
         self,
         standard_config: StandardConnectorConfig,
         config: SimpleBiomedConfig,
     ):
         super().__init__(standard_config, config)
-        self.cleanup_files = (
-            not self.standard_config.preserve_downloads and not self.standard_config.download_only
-        )
 
     def _list_objects_api(self):
         def urls_to_metadata(urls):
             files = []
             for url in urls:
                 parts = url.split(PDF_DIR)
                 if len(parts) > 1:
@@ -296,33 +276,13 @@
                 Path(self.config.path),
                 Path(self.standard_config.download_dir),
                 Path(self.standard_config.output_dir),
             )
 
         return files
 
-    def cleanup(self, cur_dir=None):
-        if not self.cleanup_files:
-            return
-
-        if cur_dir is None:
-            cur_dir = self.standard_config.download_dir
-
-        if cur_dir is None or not Path(cur_dir).is_dir():
-            return
-
-        sub_dirs = os.listdir(cur_dir)
-        os.chdir(cur_dir)
-        for sub_dir in sub_dirs:
-            # don't traverse symlinks, not that there every should be any
-            if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
-                self.cleanup(sub_dir)
-        os.chdir("..")
-        if len(os.listdir(cur_dir)) == 0:
-            os.rmdir(cur_dir)
-
     def initialize(self):
         pass
 
     def get_ingest_docs(self):
         files = self._list_objects_api() if self.config.is_api else self._list_objects()
         return [BiomedIngestDoc(self.standard_config, self.config, file) for file in files]
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/discord.py` & `unstructured-0.8.0/unstructured/ingest/connector/slack.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,172 @@
-import datetime as dt
-import json
 import os
 from dataclasses import dataclass
+from datetime import datetime
 from pathlib import Path
 from typing import List
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    ConnectorCleanupMixin,
+    IngestDocCleanupMixin,
     StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 from unstructured.utils import (
     requires_dependencies,
+    validate_date_args,
 )
 
+DATE_FORMATS = ("%Y-%m-%d", "%Y-%m-%dT%H:%M:%S", "%Y-%m-%dT%H:%M:%S%z")
+
 
 @dataclass
-class SimpleDiscordConfig(BaseConnectorConfig):
-    """Connector config where channels is a comma separated list of
-    Discord channels to pull messages from.
-    """
+class SimpleSlackConfig(BaseConnectorConfig):
+    """Connector config to process all messages by channel id's."""
 
-    # Discord Specific Options
     channels: List[str]
     token: str
-    days: int
+    oldest: str
+    latest: str
     verbose: bool = False
 
-    def __post_init__(self):
-        if self.days:
-            try:
-                self.days = int(self.days)
-            except ValueError:
-                raise ValueError("--discord-period must be an integer")
+    def validate_inputs(self):
+        oldest_valid = True
+        latest_valid = True
 
-        pass
+        if self.oldest:
+            oldest_valid = validate_date_args(self.oldest)
+
+        if self.latest:
+            latest_valid = validate_date_args(self.latest)
+
+        return oldest_valid, latest_valid
+
+    def __post_init__(self):
+        oldest_valid, latest_valid = self.validate_inputs()
+        if not oldest_valid and not latest_valid:
+            raise ValueError(
+                "Start and/or End dates are not valid. ",
+            )
 
     @staticmethod
     def parse_channels(channel_str: str) -> List[str]:
         """Parses a comma separated list of channels into a list."""
         return [x.strip() for x in channel_str.split(",")]
 
 
 @dataclass
-class DiscordIngestDoc(BaseIngestDoc):
+class SlackIngestDoc(IngestDocCleanupMixin, BaseIngestDoc):
     """Class encapsulating fetching a doc and writing processed results (but not
     doing the processing!).
+
     Also includes a cleanup method. When things go wrong and the cleanup
     method is not called, the file is left behind on the filesystem to assist debugging.
     """
 
-    config: SimpleDiscordConfig
+    config: SimpleSlackConfig
     channel: str
-    days: int
     token: str
+    oldest: str
+    latest: str
 
     # NOTE(crag): probably doesn't matter,  but intentionally not defining tmp_download_file
     # __post_init__ for multiprocessing simplicity (no Path objects in initially
     # instantiated object)
     def _tmp_download_file(self):
         channel_file = self.channel + ".txt"
         return Path(self.standard_config.download_dir) / channel_file
 
+    @property
     def _output_filename(self):
         output_file = self.channel + ".json"
         return Path(self.standard_config.output_dir) / output_file
 
-    def has_output(self):
-        """Determine if structured output for this doc already exists."""
-        return self._output_filename().is_file() and os.path.getsize(self._output_filename())
-
     def _create_full_tmp_dir_path(self):
         self._tmp_download_file().parent.mkdir(parents=True, exist_ok=True)
 
-    @requires_dependencies(dependencies=["discord"], extras="discord")
+    @BaseIngestDoc.skip_if_file_exists
+    @requires_dependencies(dependencies=["slack_sdk"], extras="slack")
     def get_file(self):
-        """Actually fetches the data from discord and stores it locally."""
+        from slack_sdk import WebClient
+        from slack_sdk.errors import SlackApiError
 
-        import discord
-        from discord.ext import commands
+        """Fetches the data from a slack channel and stores it locally."""
 
         self._create_full_tmp_dir_path()
-        if (
-            not self.standard_config.re_download
-            and self._tmp_download_file().is_file()
-            and os.path.getsize(self._tmp_download_file())
-        ):
-            if self.config.verbose:
-                logger.debug(f"File exists: {self._tmp_download_file()}, skipping download")
-            return
 
         if self.config.verbose:
-            logger.debug(f"fetching {self} - PID: {os.getpid()}")
+            logger.debug(f"fetching channel {self.channel} - PID: {os.getpid()}")
 
-        messages: List[discord.Message] = []
+        messages = []
+        self.client = WebClient(token=self.token)
 
-        intents = discord.Intents.default()
-        intents.message_content = True
-        bot = commands.Bot(command_prefix=">", intents=intents)
+        try:
+            oldest = "0"
+            latest = "0"
+            if self.oldest:
+                oldest = self.convert_datetime(self.oldest)
+
+            if self.latest:
+                latest = self.convert_datetime(self.latest)
+
+            result = self.client.conversations_history(
+                channel=self.channel,
+                oldest=oldest,
+                latest=latest,
+            )
+            messages.extend(result["messages"])
+            while result["has_more"]:
+                result = self.client.conversations_history(
+                    channel=self.channel,
+                    oldest=oldest,
+                    latest=latest,
+                    cursor=result["response_metadata"]["next_cursor"],
+                )
+                messages.extend(result["messages"])
+        except SlackApiError as e:
+            logger.error(f"Error: {e}")
+
+        with open(self._tmp_download_file(), "w") as channel_file:
+            for message in messages:
+                channel_file.write(message["text"] + "\n")
 
-        @bot.event
-        async def on_ready():
+    def convert_datetime(self, date_time):
+        for format in DATE_FORMATS:
             try:
-                after_date = None
-                if self.days:
-                    after_date = dt.datetime.utcnow() - dt.timedelta(days=self.days)
-
-                channel = bot.get_channel(int(self.channel))
-                async for msg in channel.history(after=after_date):  # type: ignore
-                    messages.append(msg)
-
-                await bot.close()
-            except Exception as e:
-                logger.error(f"Error fetching messages: {e}")
-                await bot.close()
-
-        bot.run(self.token)
-
-        with open(self._tmp_download_file(), "w") as f:
-            for m in messages:
-                f.write(m.content + "\n")
-
-    def write_result(self):
-        """Write the structured json result for this doc. result must be json serializable."""
-        output_filename = self._output_filename()
-        output_filename.parent.mkdir(parents=True, exist_ok=True)
-        with open(output_filename, "w") as output_f:
-            output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
-        logger.info(f"Wrote {output_filename}")
+                return datetime.strptime(date_time, format).timestamp()
+            except ValueError:
+                pass
 
     @property
     def filename(self):
-        """The filename of the file created from a discord channel"""
+        """The filename of the file created from a slack channel"""
         return self._tmp_download_file()
 
-    def cleanup_file(self):
-        """Removes the local copy the file after successful processing."""
-        if not self.standard_config.preserve_downloads:
-            if self.config.verbose:
-                logger.info(f"cleaning up channel {self.channel}")
-            os.unlink(self._tmp_download_file())
-
 
-class DiscordConnector(BaseConnector):
+@requires_dependencies(dependencies=["slack_sdk"], extras="slack")
+class SlackConnector(ConnectorCleanupMixin, BaseConnector):
     """Objects of this class support fetching document(s) from"""
 
-    config: SimpleDiscordConfig
+    config: SimpleSlackConfig
 
-    def __init__(
-        self,
-        standard_config: StandardConnectorConfig,
-        config: SimpleDiscordConfig,
-    ):
+    def __init__(self, standard_config: StandardConnectorConfig, config: SimpleSlackConfig):
         super().__init__(standard_config, config)
-        self.cleanup_files = not standard_config.preserve_downloads
-
-    def cleanup(self, cur_dir=None):
-        """cleanup linginering empty sub-dirs from s3 paths, but leave remaining files
-        (and their paths) in tact as that indicates they were not processed"""
-        if not self.cleanup_files:
-            return
-
-        if cur_dir is None:
-            cur_dir = self.standard_config.download_dir
-        sub_dirs = os.listdir(cur_dir)
-        os.chdir(cur_dir)
-        for sub_dir in sub_dirs:
-            # don't traverse symlinks, not that there every should be any
-            if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
-                self.cleanup(sub_dir)
-        os.chdir("..")
-        if len(os.listdir(cur_dir)) == 0:
-            os.rmdir(cur_dir)
 
     def initialize(self):
         """Verify that can get metadata for an object, validates connections info."""
-        os.mkdir(self.standard_config.download_dir)
+        pass
 
     def get_ingest_docs(self):
         return [
-            DiscordIngestDoc(
+            SlackIngestDoc(
                 self.standard_config,
                 self.config,
                 channel,
-                self.config.days,
                 self.config.token,
+                self.config.oldest,
+                self.config.latest,
             )
             for channel in self.config.channels
         ]
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/fsspec.py` & `unstructured-0.8.0/unstructured/ingest/connector/fsspec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-import json
 import os
 import re
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Type
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    ConnectorCleanupMixin,
+    IngestDocCleanupMixin,
     StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 
 SUPPORTED_REMOTE_FSSPEC_PROTOCOLS = [
     "s3",
     "s3a",
     "abfs",
     "az",
     "gs",
     "gcs",
+    "dropbox",
 ]
 
 
 @dataclass
 class SimpleFsspecConfig(BaseConnectorConfig):
     # fsspec specific options
     path: str
@@ -38,14 +40,21 @@
         self.protocol, self.path_without_protocol = self.path.split("://")
         if self.protocol not in SUPPORTED_REMOTE_FSSPEC_PROTOCOLS:
             raise ValueError(
                 f"Protocol {self.protocol} not supported yet, only "
                 f"{SUPPORTED_REMOTE_FSSPEC_PROTOCOLS} are supported.",
             )
 
+        # dropbox root is an empty string
+        match = re.match(rf"{self.protocol}://([\s])/", self.path)
+        if match and self.protocol == "dropbox":
+            self.dir_path = " "
+            self.file_path = ""
+            return
+
         # just a path with no trailing prefix
         match = re.match(rf"{self.protocol}://([^/\s]+?)(/*)$", self.path)
         if match:
             self.dir_path = match.group(1)
             self.file_path = ""
             return
 
@@ -56,15 +65,15 @@
                 f"Invalid path {self.path}. Expected <protocol>://<dir-path>/<file-or-dir-path>.",
             )
         self.dir_path = match.group(1)
         self.file_path = match.group(2) or ""
 
 
 @dataclass
-class FsspecIngestDoc(BaseIngestDoc):
+class FsspecIngestDoc(IngestDocCleanupMixin, BaseIngestDoc):
     """Class encapsulating fetching a doc and writing processed results (but not
     doing the processing!).
 
     Also includes a cleanup method. When things go wrong and the cleanup
     method is not called, the file is left behind on the filesystem to assist debugging.
     """
 
@@ -73,78 +82,44 @@
 
     def _tmp_download_file(self):
         return Path(self.standard_config.download_dir) / self.remote_file_path.replace(
             f"{self.config.dir_path}/",
             "",
         )
 
+    @property
     def _output_filename(self):
         return (
             Path(self.standard_config.output_dir)
             / f"{self.remote_file_path.replace(f'{self.config.dir_path}/', '')}.json"
         )
 
-    def has_output(self):
-        """Determine if structured output for this doc already exists."""
-        return self._output_filename().is_file() and os.path.getsize(
-            self._output_filename(),
-        )
-
     def _create_full_tmp_dir_path(self):
         """Includes "directories" in the object path"""
         self._tmp_download_file().parent.mkdir(parents=True, exist_ok=True)
 
+    @BaseIngestDoc.skip_if_file_exists
     def get_file(self):
         """Fetches the file from the current filesystem and stores it locally."""
         from fsspec import AbstractFileSystem, get_filesystem_class
 
         self._create_full_tmp_dir_path()
-        if (
-            not self.standard_config.re_download
-            and self._tmp_download_file().is_file()
-            and os.path.getsize(self._tmp_download_file())
-        ):
-            logger.debug(f"File exists: {self._tmp_download_file()}, skipping download")
-            return
-
         fs: AbstractFileSystem = get_filesystem_class(self.config.protocol)(
             **self.config.access_kwargs,
         )
-
         logger.debug(f"Fetching {self} - PID: {os.getpid()}")
         fs.get(rpath=self.remote_file_path, lpath=self._tmp_download_file().as_posix())
 
-    def write_result(self):
-        """Write the structured json result for this doc. result must be json serializable."""
-        if self.standard_config.download_only:
-            return
-        output_filename = self._output_filename()
-        output_filename.parent.mkdir(parents=True, exist_ok=True)
-        with open(output_filename, "w") as output_f:
-            output_f.write(
-                json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2),
-            )
-        logger.info(f"Wrote {output_filename}")
-
     @property
     def filename(self):
         """The filename of the file after downloading from cloud"""
         return self._tmp_download_file()
 
-    def cleanup_file(self):
-        """Removes the local copy of the file after successful processing."""
-        if not self.standard_config.preserve_downloads and not self.standard_config.download_only:
-            logger.debug(f"Cleaning up {self}")
-            try:
-                os.unlink(self._tmp_download_file())
-            except OSError as e:  # Don't think we need to raise an exception
-                logger.debug(f"Failed to remove {self._tmp_download_file()} due to {e}")
-
 
-class FsspecConnector(BaseConnector):
+class FsspecConnector(ConnectorCleanupMixin, BaseConnector):
     """Objects of this class support fetching document(s) from"""
 
     config: SimpleFsspecConfig
     ingest_doc_cls: Type[FsspecIngestDoc] = FsspecIngestDoc
 
     def __init__(
         self,
@@ -153,35 +128,14 @@
     ):
         from fsspec import AbstractFileSystem, get_filesystem_class
 
         super().__init__(standard_config, config)
         self.fs: AbstractFileSystem = get_filesystem_class(self.config.protocol)(
             **self.config.access_kwargs,
         )
-        self.cleanup_files = (
-            not standard_config.preserve_downloads and not standard_config.download_only
-        )
-
-    def cleanup(self, cur_dir=None):
-        """cleanup linginering empty sub-dirs from cloud paths, but leave remaining files
-        (and their paths) in tact as that indicates they were not processed"""
-        if not self.cleanup_files:
-            return
-
-        if cur_dir is None:
-            cur_dir = self.standard_config.download_dir
-        sub_dirs = os.listdir(cur_dir)
-        os.chdir(cur_dir)
-        for sub_dir in sub_dirs:
-            # don't traverse symlinks, not that there every should be any
-            if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
-                self.cleanup(sub_dir)
-        os.chdir("..")
-        if len(os.listdir(cur_dir)) == 0:
-            os.rmdir(cur_dir)
 
     def initialize(self):
         """Verify that can get metadata for an object, validates connections info."""
         ls_output = self.fs.ls(self.config.path_without_protocol)
         if len(ls_output) < 1:
             raise ValueError(
                 f"No objects found in {self.config.path}.",
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/gcs.py` & `unstructured-0.8.0/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/git.py` & `unstructured-0.8.0/unstructured/ingest/connector/dropbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,126 @@
-import fnmatch
-import json
-import os
-from dataclasses import dataclass, field
+"""
+Dropbox Connector
+The Dropbox Connector presents a couple abnormal situations.
+1) They don't have an unexpiring token
+2) They require a forward slash `/` in front of the remote_file_path. This presents
+some real problems creating paths. When appending a path that begins with a
+forward slash to any path, whether using the / shorthand or joinpath, causes the
+starting path to disappear. So the `/` needs to be stripped off.
+3) To list and get files from the root directory Dropbox you need a ""," ", or " /"
+"""
+import re
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Optional
+from typing import Type
 
-from unstructured.ingest.interfaces import (
-    BaseConnector,
-    BaseConnectorConfig,
-    BaseIngestDoc,
+from unstructured.ingest.connector.fsspec import (
+    FsspecConnector,
+    FsspecIngestDoc,
+    SimpleFsspecConfig,
 )
-from unstructured.ingest.logger import logger
+from unstructured.ingest.interfaces import StandardConnectorConfig
+from unstructured.utils import requires_dependencies
 
 
-@dataclass
-class SimpleGitConfig(BaseConnectorConfig):
-    url: str
-    access_token: Optional[str]
-    branch: Optional[str]
-    file_glob: Optional[str]
-    repo_path: str = field(init=False, repr=False)
+class MissingFolderError(Exception):
+    """There is no folder by that name. For root try `dropbox:// /`"""
 
 
 @dataclass
-class GitIngestDoc(BaseIngestDoc):
-    config: SimpleGitConfig = field(repr=False)
-    path: str
-
-    @property
-    def filename(self):
-        return (Path(self.standard_config.download_dir) / self.path).resolve()
+class SimpleDropboxConfig(SimpleFsspecConfig):
+    pass
 
-    def _output_filename(self):
-        return Path(self.standard_config.output_dir) / f"{self.path}.json"
-
-    def _create_full_tmp_dir_path(self):
-        """includes directories in in the gitlab repository"""
-        self.filename.parent.mkdir(parents=True, exist_ok=True)
-
-    def cleanup_file(self):
-        """Removes the local copy of the file (or anything else) after successful processing."""
-        if not self.standard_config.preserve_downloads and not self.standard_config.download_only:
-            logger.debug(f"Cleaning up {self}")
-            os.unlink(self.filename)
 
+class DropboxIngestDoc(FsspecIngestDoc):
+    @requires_dependencies(["dropboxdrivefs", "fsspec"])
     def get_file(self):
-        """Fetches the "remote" doc and stores it locally on the filesystem."""
-        self._create_full_tmp_dir_path()
-        if (
-            not self.standard_config.re_download
-            and self.filename.is_file()
-            and self.filename.stat()
-        ):
-            logger.debug(f"File exists: {self.filename}, skipping download")
-            return
-
-        logger.debug(f"Fetching {self} - PID: {os.getpid()}")
-        self._fetch_and_write()
-
-    def _fetch_and_write(self) -> None:
-        raise NotImplementedError()
-
-    def has_output(self):
-        """Determine if structured output for this doc already exists."""
-        output_filename = self._output_filename()
-        return output_filename.is_file() and output_filename.stat()
-
-    def write_result(self):
-        """Write the structured json result for this doc. result must be json serializable."""
-        if self.standard_config.download_only:
-            return
-        output_filename = self._output_filename()
-        output_filename.parent.mkdir(parents=True, exist_ok=True)
-        with open(output_filename, "w", encoding="utf8") as output_f:
-            json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
-        logger.info(f"Wrote {output_filename}")
-
+        super().get_file()
 
-@dataclass
-class GitConnector(BaseConnector):
-    config: SimpleGitConfig
+    @property
+    def _output_filename(self):
+        # Dropbox requires a forward slash at the front of the folder path. This
+        # creates some complications in path joining so a custom path is created here.
+        # Dropbox uses an empty string `""`, or a space `" "`` or a `" /"` to list root
+        if self.config.dir_path == " ":
+            return Path(self.standard_config.output_dir) / re.sub(
+                "^/",
+                "",
+                f"{self.remote_file_path}.json",
+            )
+        else:
+            return (
+                Path(self.standard_config.output_dir)
+                / f"{self.remote_file_path.replace(f'/{self.config.dir_path}/', '')}.json"
+            )
 
-    def __post_init__(self) -> None:
-        self.cleanup_files = (
-            not self.standard_config.preserve_downloads and not self.standard_config.download_only
-        )
+    def _tmp_download_file(self):
+        # Dropbox requires a forward slash at the front of the folder path. This
+        # creates some complications in path joining so a custom path is created here.
+        # Dropbox uses an empty string `""`, or a space `" "`` or a `" /"` to list root
+        if self.config.dir_path == " ":
+            return Path(self.standard_config.download_dir) / re.sub(
+                "^/",
+                "",
+                self.remote_file_path,
+            )
+        else:
+            return Path(
+                self.standard_config.download_dir,
+            ) / self.remote_file_path.replace(
+                f"/{self.config.dir_path}/",
+                "",
+            )
 
-    def cleanup(self, cur_dir=None):
-        if not self.cleanup_files:
-            return
 
-        if cur_dir is None:
-            cur_dir = self.standard_config.download_dir
-        sub_dirs = os.listdir(cur_dir)
-        os.chdir(cur_dir)
-        for sub_dir in sub_dirs:
-            # don't traverse symlinks, not that there every should be any
-            if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
-                self.cleanup(sub_dir)
-        os.chdir("..")
-        if len(os.listdir(cur_dir)) == 0:
-            os.rmdir(cur_dir)
+@requires_dependencies(["dropboxdrivefs", "fsspec"])
+class DropboxConnector(FsspecConnector):
+    ingest_doc_cls: Type[DropboxIngestDoc] = DropboxIngestDoc
+
+    def __init__(
+        self,
+        config: SimpleDropboxConfig,
+        standard_config: StandardConnectorConfig,
+    ) -> None:
+        super().__init__(standard_config, config)
 
     def initialize(self):
-        pass
+        # Dropbox requires a forward slash at the front of the folder path. This
+        # creates some complications in path joining so a custom path is created here.
+        ls_output = self.fs.ls(f"/{self.config.path_without_protocol}")
+        if ls_output and len(ls_output) >= 1:
+            return
+        elif ls_output:
+            raise ValueError(
+                f"No objects found in {self.config.path}.",
+            )
+        else:
+            raise MissingFolderError(
+                "There is no folder by that name. For root try `dropbox:// /`",
+            )
 
-    def is_file_type_supported(self, path: str) -> bool:
-        # Workaround to ensure that auto.partition isn't fed with .yaml, .py, etc. files
-        # TODO: What to do with no filenames? e.g. LICENSE, Makefile, etc.
-        supported = path.endswith(
-            (
-                ".md",
-                ".txt",
-                ".pdf",
-                ".doc",
-                ".docx",
-                ".eml",
-                ".html",
-                ".png",
-                ".jpg",
-                ".ppt",
-                ".pptx",
-                ".xml",
-            ),
-        )
-        if not supported:
-            logger.debug(
-                f"The file {path!r} is discarded as it does not contain a supported filetype.",
-            )
-        return supported
-
-    def does_path_match_glob(self, path: str) -> bool:
-        if not self.config.file_glob:
-            return True
-        patterns = self.config.file_glob.split(",")
-        for pattern in patterns:
-            if fnmatch.filter([path], pattern):
-                return True
-        logger.debug(f"The file {path!r} is discarded as it does not match any given glob.")
-        return False
+    def _list_files(self):
+        # Dropbox requires a forward slash at the front of the folder path. This
+        # creates some complications in path joining so a custom path is created here.
+        if not self.config.recursive:
+            # fs.ls does not walk directories
+            # directories that are listed in cloud storage can cause problems because they are seen
+            # as 0byte files
+            return [
+                x.get("name")
+                for x in self.fs.ls(
+                    f"/{self.config.path_without_protocol}",
+                    detail=True,
+                )
+                if x.get("size")
+            ]
+        else:
+            # fs.find will recursively walk directories
+            # "size" is a common key for all the cloud protocols with fs
+            return [
+                k
+                for k, v in self.fs.find(
+                    f"/{self.config.path_without_protocol}",
+                    detail=True,
+                ).items()
+                if v.get("size")
+            ]
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/github.py` & `unstructured-0.8.0/unstructured/ingest/connector/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             f.write(contents)
 
 
 @requires_dependencies(["github"], extras="github")
 @dataclass
 class GitHubConnector(GitConnector):
     def __post_init__(self) -> None:
-        super().__post_init__()
         from github import Github
 
         self.github = Github(self.config.access_token)
 
     def get_ingest_docs(self):
         repo = self.github.get_repo(self.config.repo_path)
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/gitlab.py` & `unstructured-0.8.0/unstructured/ingest/connector/gitlab.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             f.write(contents)
 
 
 @requires_dependencies(["gitlab"], extras="gitlab")
 @dataclass
 class GitLabConnector(GitConnector):
     def __post_init__(self) -> None:
-        super().__post_init__()
         from gitlab import Gitlab
 
         self.gitlab = Gitlab(self.config.url, private_token=self.config.access_token)
 
     def get_ingest_docs(self):
         # Load the Git tree with all files, and then create Ingest docs
         # for all blobs, i.e. all files, ignoring directories
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/google_drive.py` & `unstructured-0.8.0/unstructured/ingest/connector/google_drive.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from unstructured.file_utils.filetype import EXT_TO_FILETYPE
 from unstructured.file_utils.google_filetype import GOOGLE_DRIVE_EXPORT_TYPES
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    ConnectorCleanupMixin,
+    IngestDocCleanupMixin,
     StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 from unstructured.utils import requires_dependencies
 
 FILE_FORMAT = "{id}-{name}{ext}"
 DIRECTORY_FORMAT = "{id}-{name}"
@@ -79,52 +81,32 @@
                 f"Extension not supported. "
                 f"Value MUST be one of {', '.join([k for k in EXT_TO_FILETYPE if k is not None])}.",
             )
         self.service = create_service_account_object(self.service_account_key, self.drive_id)
 
 
 @dataclass
-class GoogleDriveIngestDoc(BaseIngestDoc):
+class GoogleDriveIngestDoc(IngestDocCleanupMixin, BaseIngestDoc):
     config: SimpleGoogleDriveConfig
     file_meta: Dict
 
     @property
     def filename(self):
         return Path(self.file_meta.get("download_filepath")).resolve()  # type: ignore
 
+    @property
     def _output_filename(self):
         return Path(f"{self.file_meta.get('output_filepath')}.json").resolve()
 
-    def cleanup_file(self):
-        if (
-            not self.standard_config.preserve_downloads
-            and self.filename.is_file()
-            and not self.standard_config.download_only
-        ):
-            logger.debug(f"Cleaning up {self}")
-            Path.unlink(self.filename)
-
-    def has_output(self):
-        """Determine if structured output for this doc already exists."""
-        output_filename = self._output_filename()
-        return output_filename.is_file() and output_filename.stat()
-
+    @BaseIngestDoc.skip_if_file_exists
     @requires_dependencies(["googleapiclient"], extras="google-drive")
     def get_file(self):
         from googleapiclient.errors import HttpError
         from googleapiclient.http import MediaIoBaseDownload
 
-        if (
-            not self.standard_config.re_download
-            and self.filename.is_file()
-            and self.filename.stat()
-        ):
-            logger.debug(f"File exists: {self.filename}, skipping download")
-            return
-
         self.config.service = create_service_account_object(self.config.service_account_key)
 
         if self.file_meta.get("mimeType", "").startswith("application/vnd.google-apps"):
             export_mime = GOOGLE_DRIVE_EXPORT_TYPES.get(
                 self.file_meta.get("mimeType"),  # type: ignore
             )
             if not export_mime:
@@ -139,15 +121,14 @@
                 fileId=self.file_meta.get("id"),
                 mimeType=export_mime,
             )
         else:
             request = self.config.service.files().get_media(fileId=self.file_meta.get("id"))
         file = io.BytesIO()
         downloader = MediaIoBaseDownload(file, request)
-
         downloaded = False
         try:
             while downloaded is False:
                 status, downloaded = downloader.next_chunk()
         except HttpError:
             pass
 
@@ -169,31 +150,27 @@
         if not saved:
             logger.error(f"Error while downloading and saving file: {self.filename}.")
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
         if self.standard_config.download_only:
             return
-        output_filename = self._output_filename()
-        output_filename.parent.mkdir(parents=True, exist_ok=True)
-        with open(output_filename, "w") as output_f:
+        self._output_filename.parent.mkdir(parents=True, exist_ok=True)
+        with open(self._output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
-        logger.info(f"Wrote {output_filename}")
+        logger.info(f"Wrote {self._output_filename}")
 
 
-class GoogleDriveConnector(BaseConnector):
+class GoogleDriveConnector(ConnectorCleanupMixin, BaseConnector):
     """Objects of this class support fetching documents from Google Drive"""
 
     config: SimpleGoogleDriveConfig
 
     def __init__(self, standard_config: StandardConnectorConfig, config: SimpleGoogleDriveConfig):
         super().__init__(standard_config, config)
-        self.cleanup_files = (
-            not self.standard_config.preserve_downloads and not self.standard_config.download_only
-        )
 
     def _list_objects(self, drive_id, recursive=False):
         files = []
 
         def traverse(drive_id, download_dir, output_dir, recursive=False):
             page_token = None
             while True:
@@ -258,34 +235,14 @@
             drive_id,
             Path(self.standard_config.download_dir),
             Path(self.standard_config.output_dir),
             recursive,
         )
         return files
 
-    def cleanup(self, cur_dir=None):
-        if not self.cleanup_files:
-            return
-
-        if cur_dir is None:
-            cur_dir = self.standard_config.download_dir
-
-        if cur_dir is None or not Path(cur_dir).is_dir():
-            return
-
-        sub_dirs = os.listdir(cur_dir)
-        os.chdir(cur_dir)
-        for sub_dir in sub_dirs:
-            # don't traverse symlinks, not that there every should be any
-            if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
-                self.cleanup(sub_dir)
-        os.chdir("..")
-        if len(os.listdir(cur_dir)) == 0:
-            os.rmdir(cur_dir)
-
     def initialize(self):
         pass
 
     def get_ingest_docs(self):
         files = self._list_objects(self.config.drive_id, self.config.recursive)
         # Setting to None because service object can't be pickled for multiprocessing.
         self.config.service = None
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/local.py` & `unstructured-0.8.0/unstructured/ingest/connector/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import fnmatch
 import glob
-import json
 import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Type
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
@@ -47,33 +46,27 @@
         """Not applicable to local file system"""
         pass
 
     def get_file(self):
         """Not applicable to local file system"""
         pass
 
-    def _output_filename(self):
-        return (
-            Path(self.standard_config.output_dir)
-            / f"{self.path.replace(f'{self.config.input_path}/', '')}.json"
+    @property
+    def _output_filename(self) -> Path:
+        """Returns output filename for the doc
+        If input path argument is a file itself, it returns the filename of the doc.
+        If input path argument is a folder, it returns the relative path of the doc.
+        """
+        input_path = Path(self.config.input_path)
+        basename = (
+            f"{Path(self.path).name}.json"
+            if input_path.is_file()
+            else f"{Path(self.path).relative_to(input_path)}.json"
         )
-
-    def has_output(self):
-        """Determine if structured output for this doc already exists."""
-        return self._output_filename().is_file() and os.path.getsize(self._output_filename())
-
-    def write_result(self):
-        """Write the structured json result for this doc. result must be json serializable."""
-        if self.standard_config.download_only:
-            return
-        output_filename = self._output_filename()
-        output_filename.parent.mkdir(parents=True, exist_ok=True)
-        with open(output_filename, "w") as output_f:
-            output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
-        logger.info(f"Wrote {output_filename}")
+        return Path(self.standard_config.output_dir) / basename
 
 
 class LocalConnector(BaseConnector):
     """Objects of this class support fetching document(s) from local file system"""
 
     config: SimpleLocalConfig
     ingest_doc_cls: Type[LocalIngestDoc] = LocalIngestDoc
```

### Comparing `unstructured-0.7.9/unstructured/ingest/connector/s3.py` & `unstructured-0.8.0/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.8.0/unstructured/ingest/doc_processor/generalized.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-"""Process aribritrary files with the Unstructured library"""
+"""Process arbitrary files with the Unstructured library"""
 
+import os
 from typing import Any, Dict, List, Optional
 
 from unstructured_inference.models.base import get_model
 
 from unstructured.ingest.interfaces import BaseIngestDoc as IngestDoc
 from unstructured.ingest.logger import logger
 
 
 def initialize():
-    """Download default model (avoids subprocesses all doing the same)"""
+    """Download default model or model specified by UNSTRUCTURED_HI_RES_MODEL_NAME environment
+    variable (avoids subprocesses all doing the same)"""
 
-    get_model()
+    # If more than one model will be supported and left up to user selection
+    supported_model = os.environ.get("UNSTRUCTURED_HI_RES_SUPPORTED_MODEL", "")
+    if supported_model:
+        for model_name in supported_model.split(","):
+            get_model(model_name=model_name)
+
+    get_model(os.environ.get("UNSTRUCTURED_HI_RES_MODEL_NAME"))
 
 
 def process_document(doc: "IngestDoc", **partition_kwargs) -> Optional[List[Dict[str, Any]]]:
     """Process any IngestDoc-like class of document with chosen Unstructured's partition logic.
 
     Parameters
     ----------
```

### Comparing `unstructured-0.7.9/unstructured/ingest/interfaces.py` & `unstructured-0.8.0/unstructured/ingest/interfaces.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Defines Abstract Base Classes (ABC's) core to batch processing documents
 through Unstructured."""
 
+import functools
+import json
+import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime
+from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import requests
 
 from unstructured.documents.elements import DataSourceMetadata
 from unstructured.ingest.logger import logger
 from unstructured.partition.auto import partition
@@ -114,14 +118,19 @@
 
     @property
     @abstractmethod
     def filename(self):
         """The local filename of the document after fetching from remote source."""
 
     @property
+    @abstractmethod
+    def _output_filename(self):
+        """Filename of the structured output for this doc."""
+
+    @property
     def record_locator(self) -> Optional[Dict[str, Any]]:  # Values must be JSON-serializable
         """A dictionary with any data necessary to uniquely identify the document on
         the source system."""
         return None
 
     @property
     def source_url(self) -> Optional[str]:
@@ -136,30 +145,51 @@
         return None
 
     @abstractmethod
     def cleanup_file(self):
         """Removes the local copy the file (or anything else) after successful processing."""
         pass
 
+    @staticmethod
+    def skip_if_file_exists(func):
+        """Decorator that checks if a file exists, is not empty, and should not re-download,
+        if so log a message indicating as much and skip the decorated function."""
+
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if (
+                not self.standard_config.re_download
+                and self.filename.is_file()
+                and self.filename.stat().st_size
+            ):
+                logger.debug(f"File exists: {self.filename}, skipping {func.__name__}")
+                return None
+            return func(self, *args, **kwargs)
+
+        return wrapper
+
     # NOTE(crag): Future BaseIngestDoc classes could define get_file_object() methods
     # in addition to or instead of get_file()
     @abstractmethod
     def get_file(self):
         """Fetches the "remote" doc and stores it locally on the filesystem."""
         pass
 
-    @abstractmethod
     def has_output(self) -> bool:
         """Determine if structured output for this doc already exists."""
-        pass
+        return self._output_filename.is_file() and self._output_filename.stat().st_size
 
-    @abstractmethod
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        pass
+        if self.standard_config.download_only:
+            return
+        self._output_filename.parent.mkdir(parents=True, exist_ok=True)
+        with open(self._output_filename, "w", encoding="utf8") as output_f:
+            json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
+        logger.info(f"Wrote {self._output_filename}")
 
     def partition_file(self, **partition_kwargs) -> List[Dict[str, Any]]:
         if not self.standard_config.partition_by_api:
             logger.debug("Using local partition")
             elements = partition(
                 filename=str(self.filename),
                 data_source_metadata=DataSourceMetadata(
@@ -242,7 +272,48 @@
                 for k, v in elem["metadata"].items():  # type: ignore[attr-defined]
                     elem[k] = v
                 elem.pop("metadata")  # type: ignore[attr-defined]
 
             self.isd_elems_no_filename.append(elem)
 
         return self.isd_elems_no_filename
+
+
+class ConnectorCleanupMixin:
+    standard_config: StandardConnectorConfig
+
+    def cleanup(self, cur_dir=None):
+        """Recursively clean up downloaded files and directories."""
+        if self.standard_config.preserve_downloads or self.standard_config.download_only:
+            return
+        if cur_dir is None:
+            cur_dir = self.standard_config.download_dir
+        if cur_dir is None or not Path(cur_dir).is_dir():
+            return
+        sub_dirs = os.listdir(cur_dir)
+        os.chdir(cur_dir)
+        for sub_dir in sub_dirs:
+            # don't traverse symlinks, not that there every should be any
+            if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
+                self.cleanup(sub_dir)
+        os.chdir("..")
+        if len(os.listdir(cur_dir)) == 0:
+            os.rmdir(cur_dir)
+
+
+class IngestDocCleanupMixin:
+    standard_config: StandardConnectorConfig
+
+    @property
+    @abstractmethod
+    def filename(self):
+        """The local filename of the document after fetching from remote source."""
+
+    def cleanup_file(self):
+        """Removes the local copy of the file after successful processing."""
+        if (
+            not self.standard_config.preserve_downloads
+            and self.filename.is_file()
+            and not self.standard_config.download_only
+        ):
+            logger.debug(f"Cleaning up {self}")
+            os.unlink(self.filename)
```

### Comparing `unstructured-0.7.9/unstructured/ingest/main.py` & `unstructured-0.8.0/unstructured/ingest/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,15 @@
             docs = self._filter_docs_with_outputs(docs)
             if not docs:
                 return
 
         # Debugging tip: use the below line and comment out the mp.Pool loop
         # block to remain in single process
         # self.doc_processor_fn(docs[0])
+
         with mp.Pool(
             processes=self.num_processes,
             initializer=ingest_log_streaming_init,
             initargs=(logging.DEBUG if self.verbose else logging.INFO,),
         ) as pool:
             pool.map(self.doc_processor_fn, docs)
 
@@ -176,29 +177,34 @@
     " e.g. '*.html,*.txt'",
 )
 @click.option(
     "--remote-url",
     default=None,
     help="Remote fsspec URL formatted as `protocol://dir/path`, it can contain both "
     "a directory or a single file. Supported protocols are: `gcs`, `gs`, `s3`, `s3a`, `abfs` "
-    "and `az`.",
+    "`az` and `dropbox`.",
 )
 @click.option(
     "--gcs-token",
     default=None,
     help="Token used to access Google Cloud. GCSFS will attempt to use your default gcloud creds"
     "or get creds from the google metadata service or fall back to anonymous access.",
 )
 @click.option(
     "--s3-anonymous",
     is_flag=True,
     default=False,
     help="Connect to s3 without local AWS credentials.",
 )
 @click.option(
+    "--dropbox-token",
+    default=None,
+    help="Dropbox access token.",
+)
+@click.option(
     "--azure-account-name",
     default=None,
     help="Azure Blob Storage or DataLake account name.",
 )
 @click.option(
     "--azure-account-key",
     default=None,
@@ -382,14 +388,32 @@
 )
 @click.option(
     "--discord-period",
     default=None,
     help="Number of days to go back in the history of discord channels, must be an number",
 )
 @click.option(
+    "--elasticsearch-url",
+    default=None,
+    help='URL to the Elasticsearch cluster, e.g. "http://localhost:9200"',
+)
+@click.option(
+    "--elasticsearch-index-name",
+    default=None,
+    help="Name for the Elasticsearch index to pull data from",
+)
+@click.option(
+    "--jq-query",
+    default=None,
+    help="JQ query to get and concatenate a subset of the fields from a JSON document. "
+    "For a group of JSON documents, it assumes that all of the documents have the same schema. "
+    "Currently only supported for the Elasticsearch connector. "
+    "Example: --jq-query '{meta, body}'",
+)
+@click.option(
     "--download-dir",
     help="Where files are downloaded to, defaults to `$HOME/.cache/unstructured/ingest/<SHA256>`.",
 )
 @click.option(
     "--preserve-downloads",
     is_flag=True,
     default=False,
@@ -417,21 +441,22 @@
 @click.option(
     "--recursive",
     is_flag=True,
     default=False,
     help="Recursively download files in their respective folders"
     "otherwise stop at the files in provided folder level."
     " Supported protocols are: `gcs`, `gs`, `s3`, `s3a`, `abfs` "
-    "`az`, `google drive` and `local`.",
+    "`az`, `google drive`, `dropbox` and `local`.",
 )
 @click.option("-v", "--verbose", is_flag=True, default=False)
 def main(
     ctx,
     remote_url,
     s3_anonymous,
+    dropbox_token,
     gcs_token,
     azure_account_name,
     azure_account_key,
     azure_connection_string,
     drive_id,
     drive_service_account_key,
     drive_extension,
@@ -459,14 +484,17 @@
     slack_channels,
     slack_token,
     start_date,
     end_date,
     discord_channels,
     discord_token,
     discord_period,
+    elasticsearch_url,
+    elasticsearch_index_name,
+    jq_query,
     download_dir,
     preserve_downloads,
     structured_output_dir,
     reprocess,
     num_processes,
     recursive,
     verbose,
@@ -554,14 +582,18 @@
             if not biomed_path:
                 base_path = (
                     f"{biomed_api_id or ''}-{biomed_api_from or ''}-" f"{biomed_api_until or ''}"
                 )
             hashed_dir_name = hashlib.sha256(
                 base_path.encode("utf-8"),
             )
+        elif elasticsearch_url:
+            hashed_dir_name = hashlib.sha256(
+                f"{elasticsearch_url}_{elasticsearch_index_name}".encode("utf-8"),
+            )
         else:
             raise ValueError(
                 "This connector does not support saving downloads to ~/.cache/  ,"
                 " --download-dir must be provided",
             )
         download_dir = cache_path / hashed_dir_name.hexdigest()[:10]
         if preserve_downloads:
@@ -603,14 +635,28 @@
                 standard_config=standard_config,
                 config=SimpleGcsConfig(
                     path=remote_url,
                     recursive=recursive,
                     access_kwargs={"token": gcs_token},
                 ),
             )
+        elif protocol in ("dropbox"):
+            from unstructured.ingest.connector.dropbox import (
+                DropboxConnector,
+                SimpleDropboxConfig,
+            )
+
+            doc_connector = DropboxConnector(  # type: ignore
+                standard_config=standard_config,
+                config=SimpleDropboxConfig(
+                    path=remote_url,
+                    recursive=recursive,
+                    access_kwargs={"token": dropbox_token},
+                ),
+            )
         elif protocol in ("abfs", "az"):
             from unstructured.ingest.connector.azure import (
                 AzureBlobStorageConnector,
                 SimpleAzureBlobStorageConfig,
             )
 
             if azure_account_name:
@@ -630,15 +676,15 @@
                     access_kwargs=access_kwargs,
                 ),
             )
         else:
             warnings.warn(
                 f"`fsspec` protocol {protocol} is not directly supported by `unstructured`,"
                 " so use it at your own risk. Supported protocols are `gcs`, `gs`, `s3`, `s3a`,"
-                "`abfs` and `az`.",
+                "`dropbox`, `abfs` and `az`.",
                 UserWarning,
             )
 
             from unstructured.ingest.connector.fsspec import (
                 FsspecConnector,
                 SimpleFsspecConfig,
             )
@@ -779,14 +825,28 @@
             standard_config=standard_config,
             config=SimpleLocalConfig(
                 input_path=local_input_path,
                 recursive=recursive,
                 file_glob=local_file_glob,
             ),
         )
+    elif elasticsearch_url:
+        from unstructured.ingest.connector.elasticsearch import (
+            ElasticsearchConnector,
+            SimpleElasticsearchConfig,
+        )
+
+        doc_connector = ElasticsearchConnector(  # type: ignore
+            standard_config=standard_config,
+            config=SimpleElasticsearchConfig(
+                url=elasticsearch_url,
+                index_name=elasticsearch_index_name,
+                jq_query=jq_query,
+            ),
+        )
     # Check for other connector-specific options here and define the doc_connector object
     # e.g. "elif azure_container:  ..."
 
     else:
         logger.error("No connector-specific option was specified!")
         sys.exit(1)
```

### Comparing `unstructured-0.7.9/unstructured/nlp/english-words.txt` & `unstructured-0.8.0/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/nlp/english_words.py` & `unstructured-0.8.0/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/nlp/patterns.py` & `unstructured-0.8.0/unstructured/nlp/patterns.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,28 +53,31 @@
     "\u29BF",
     "\u002D",
     "",
     "\*",  # noqa: W605 NOTE(robinson) - skipping qa because we need the escape for the regex
     "\x95",
     "·",
 ]
-UNICODE_BULLETS_RE = re.compile(f"(?:{'|'.join(UNICODE_BULLETS)})")
+BULLETS_PATTERN = "|".join(UNICODE_BULLETS)
+UNICODE_BULLETS_RE = re.compile(f"(?:{BULLETS_PATTERN})(?!{BULLETS_PATTERN})")
 
 ENUMERATED_BULLETS_RE = re.compile(r"(?:(?:\d{1,3}|[a-z][A-Z])\.?){1,3}")
 
 EMAIL_HEAD_PATTERN = (
     r"(MIME-Version: 1.0(.*)?\n)?Date:.*\nMessage-ID:.*\nSubject:.*\nFrom:.*\nTo:.*"
 )
 EMAIL_HEAD_RE = re.compile(EMAIL_HEAD_PATTERN)
 
 # Helps split text by paragraphs. There must be one newline, with potential whitespace
 # (incluing \r and \n chars) on either side
 PARAGRAPH_PATTERN = r"\s*\n\s*"  # noqa: W605 NOTE(harrell)
 
-PARAGRAPH_PATTERN_RE = re.compile(f"((?:{'|'.join(UNICODE_BULLETS)})|{PARAGRAPH_PATTERN})")
+PARAGRAPH_PATTERN_RE = re.compile(
+    f"((?:{BULLETS_PATTERN})|{PARAGRAPH_PATTERN})(?!{BULLETS_PATTERN}|$)",
+)
 DOUBLE_PARAGRAPH_PATTERN_RE = re.compile("(" + PARAGRAPH_PATTERN + "){2}")
 
 # IP Address examples: ba23::58b5:2236:45g2:88h2 or 10.0.2.01
 IP_ADDRESS_PATTERN = (
     "[0-9]{1,2}\.[0-9]{1,2}\.[0-9]{1,2}\.[0-9]{1,2}",  # noqa: W605 NOTE(harrell)
     # - skipping qa because we need the escape for the regex
     "[a-z0-9]{4}::[a-z0-9]{4}:[a-z0-9]{4}:[a-z0-9]{4}:[a-z0-9]{4}%?[0-9]*",
```

### Comparing `unstructured-0.7.9/unstructured/nlp/tokenize.py` & `unstructured-0.8.0/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/partition/__init__.py` & `unstructured-0.8.0/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/partition/api.py` & `unstructured-0.8.0/unstructured/partition/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from unstructured.partition.common import exactly_one
 from unstructured.staging.base import dict_to_elements, elements_from_json
 
 
 def partition_via_api(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     file_filename: Optional[str] = None,
     api_url: str = "https://api.unstructured.io/general/v0/general",
     api_key: str = "",
     **request_kwargs,
 ) -> List[Element]:
     """Partitions a document using the Unstructured REST API. This is equivalent to
     running the document through partition.
@@ -106,15 +106,15 @@
 
     See https://api.unstructured.io/general/docs for the hosted API documentation or
     https://github.com/Unstructured-IO/unstructured-api for instructions on how to run
     the API locally as a container.
 
     Parameters
     ----------
-    filename
+    filenames
         A list of strings defining the target filename paths.
     content_types
         A list of strings defining the file contents in MIME types.
     files
         A list of file-like object using "rb" mode --> open(filename, "rb").
     file_filename
         When file is not None, the filename (string) to store in element metadata. E.g. "foo.txt"
```

### Comparing `unstructured-0.7.9/unstructured/partition/auto.py` & `unstructured-0.8.0/unstructured/partition/auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from unstructured.partition.xlsx import partition_xlsx
 from unstructured.partition.xml import partition_xml
 
 
 def partition(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     file_filename: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     headers: Dict[str, str] = {},
```

### Comparing `unstructured-0.7.9/unstructured/partition/common.py` & `unstructured-0.8.0/unstructured/partition/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,95 +4,128 @@
 from io import BufferedReader, BytesIO, TextIOWrapper
 from tempfile import SpooledTemporaryFile
 from typing import IO, TYPE_CHECKING, Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
 from docx import table as docxtable
 from tabulate import tabulate
 
+from unstructured.documents.coordinates import CoordinateSystem
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
+    CoordinatesMetadata,
     Element,
     ElementMetadata,
     ListItem,
     PageBreak,
     Text,
 )
 from unstructured.logger import logger
 from unstructured.nlp.patterns import ENUMERATED_BULLETS_RE, UNICODE_BULLETS_RE
 
 if TYPE_CHECKING:
-    from unstructured_inference.inference.layoutelement import LayoutElement
+    from unstructured_inference.inference.layoutelement import (
+        LayoutElement,
+        LocationlessLayoutElement,
+    )
 
 
 def normalize_layout_element(
-    layout_element: Union["LayoutElement", Element, Dict[str, Any]],
+    layout_element: Union["LayoutElement", "LocationlessLayoutElement", Element, Dict[str, Any]],
+    coordinate_system: Optional[CoordinateSystem] = None,
 ) -> Union[Element, List[Element]]:
     """Converts an unstructured_inference LayoutElement object to an unstructured Element."""
 
     if isinstance(layout_element, Element):
         return layout_element
 
     # NOTE(alan): Won't the lines above ensure this never runs (PageBreak is a subclass of Element)?
     if isinstance(layout_element, PageBreak):
-        return PageBreak()
+        return PageBreak(text="")
 
     if not isinstance(layout_element, dict):
         layout_dict = layout_element.to_dict()
     else:
         layout_dict = layout_element
 
     text = layout_dict.get("text")
+    # Both `coordinates` and `coordinate_system` must be present
+    # in order to add coordinates metadata to the element.
     coordinates = layout_dict.get("coordinates")
     element_type = layout_dict.get("type")
-
     if element_type == "List":
-        return layout_list_to_list_items(text, coordinates)
+        return layout_list_to_list_items(
+            text,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     elif element_type in TYPE_TO_TEXT_ELEMENT_MAP:
         _element_class = TYPE_TO_TEXT_ELEMENT_MAP[element_type]
-        return _element_class(text=text, coordinates=coordinates)
+        return _element_class(
+            text=text,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     elif element_type == "Checked":
-        return CheckBox(checked=True, coordinates=coordinates)
+        return CheckBox(checked=True, coordinates=coordinates, coordinate_system=coordinate_system)
     elif element_type == "Unchecked":
-        return CheckBox(checked=False, coordinates=coordinates)
+        return CheckBox(checked=False, coordinates=coordinates, coordinate_system=coordinate_system)
     else:
-        return Text(text=text, coordinates=coordinates)
+        return Text(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
 
 
 def layout_list_to_list_items(
     text: str,
     coordinates: Tuple[Tuple[float, float], ...],
+    coordinate_system: Optional[CoordinateSystem],
 ) -> List[Element]:
     """Converts a list LayoutElement to a list of ListItem elements."""
     split_items = ENUMERATED_BULLETS_RE.split(text)
     # NOTE(robinson) - this means there wasn't a match for the enumerated bullets
     if len(split_items) == 1:
         split_items = UNICODE_BULLETS_RE.split(text)
 
     list_items: List[Element] = []
     for text_segment in split_items:
         if len(text_segment.strip()) > 0:
+            # Both `coordinates` and `coordinate_system` must be present
+            # in order to add coordinates metadata to the element.
             list_items.append(
-                ListItem(text=text_segment.strip(), coordinates=coordinates),
+                ListItem(
+                    text=text_segment.strip(),
+                    coordinates=coordinates,
+                    coordinate_system=coordinate_system,
+                ),
             )
 
     return list_items
 
 
 def _add_element_metadata(
     element: Element,
     filename: Optional[str] = None,
     filetype: Optional[str] = None,
     page_number: Optional[int] = None,
     url: Optional[str] = None,
     text_as_html: Optional[str] = None,
+    coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
+    coordinate_system: Optional[CoordinateSystem] = None,
 ) -> Element:
     """Adds document metadata to the document element. Document metadata includes information
     like the filename, source url, and page number."""
+    coordinates_metadata = (
+        CoordinatesMetadata(
+            points=coordinates,
+            system=coordinate_system,
+        )
+        if coordinates is not None and coordinate_system is not None
+        else None
+    )
     metadata = ElementMetadata(
+        coordinates=coordinates_metadata,
         filename=filename,
         filetype=filetype,
         page_number=page_number,
         url=url,
         text_as_html=text_as_html,
     )
     element.metadata = metadata.merge(element.metadata)
@@ -181,15 +214,15 @@
         return BytesIO(contents)
     else:
         # Return the original file object if it's not a SpooledTemporaryFile
         return file_obj
 
 
 def convert_to_bytes(
-    file: Optional[Union[bytes, SpooledTemporaryFile, IO]] = None,
+    file: Optional[Union[bytes, SpooledTemporaryFile, IO[bytes]]] = None,
 ) -> bytes:
     if isinstance(file, bytes):
         f_bytes = file
     elif isinstance(file, SpooledTemporaryFile):
         file.seek(0)
         f_bytes = file.read()
     elif isinstance(file, BytesIO):
```

### Comparing `unstructured-0.7.9/unstructured/partition/csv.py` & `unstructured-0.8.0/unstructured/partition/csv.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,47 +14,43 @@
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.CSV)
 def partition_csv(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Excel Documents in .csv format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    metadata_filename
-        The filename to use for the metadata.
     include_metadata
         Determines whether or not metadata is included in the output.
     """
     exactly_one(filename=filename, file=file)
 
     if filename:
         table = pd.read_csv(filename)
     else:
         f = spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file))
         table = pd.read_csv(f)
 
-    metadata_filename = filename or metadata_filename
-
     html_text = table.to_html(index=False, header=False, na_rep="")
     text = lxml.html.document_fromstring(html_text).text_content()
 
     if include_metadata:
         metadata = ElementMetadata(
             text_as_html=html_text,
-            filename=metadata_filename,
+            filename=metadata_filename or filename,
         )
     else:
         metadata = ElementMetadata()
 
     return [Table(text=text, metadata=metadata)]
```

### Comparing `unstructured-0.7.9/unstructured/partition/doc.py` & `unstructured-0.8.0/unstructured/partition/tsv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import os
-import tempfile
-from typing import IO, List, Optional
+from tempfile import SpooledTemporaryFile
+from typing import IO, BinaryIO, List, Optional, Union, cast
 
-from unstructured.documents.elements import Element, process_metadata
+import lxml.html
+import pandas as pd
+
+from unstructured.documents.elements import (
+    Element,
+    ElementMetadata,
+    Table,
+    process_metadata,
+)
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import convert_office_doc, exactly_one
-from unstructured.partition.docx import partition_docx
+from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.DOC)
-def partition_doc(
+@add_metadata_with_filetype(FileType.TSV)
+def partition_tsv(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
-    include_page_breaks: bool = True,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
+    metadata_filename: Optional[str] = None,
+    include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
-    """Partitions Microsoft Word Documents in .doc format into its document elements.
+    """Partitions TSV files into document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
+    include_metadata
+        Determines whether or not metadata is included in the output.
     """
-    # Verify that only one of the arguments was provided
-    if filename is None:
-        filename = ""
     exactly_one(filename=filename, file=file)
 
-    if len(filename) > 0:
-        _, filename_no_path = os.path.split(os.path.abspath(filename))
-        base_filename, _ = os.path.splitext(filename_no_path)
-        if not os.path.exists(filename):
-            raise ValueError(f"The file {filename} does not exist.")
-    elif file is not None:
-        tmp = tempfile.NamedTemporaryFile(delete=False)
-        tmp.write(file.read())
-        tmp.close()
-        filename = tmp.name
-        _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
-
-    base_filename, _ = os.path.splitext(filename_no_path)
-
-    with tempfile.TemporaryDirectory() as tmpdir:
-        convert_office_doc(filename, tmpdir, target_format="docx")
-        docx_filename = os.path.join(tmpdir, f"{base_filename}.docx")
-        elements = partition_docx(
-            filename=docx_filename,
-            metadata_filename=filename,
-            include_page_breaks=include_page_breaks,
+    if filename:
+        table = pd.read_csv(filename, sep="\t")
+    else:
+        f = spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file))
+        table = pd.read_csv(f, sep="\t")
+
+    html_text = table.to_html(index=False, header=False, na_rep="")
+    text = lxml.html.document_fromstring(html_text).text_content()
+
+    if include_metadata:
+        metadata = ElementMetadata(
+            text_as_html=html_text,
+            filename=metadata_filename or filename,
         )
+    else:
+        metadata = ElementMetadata()
 
-    return elements
+    return [Table(text=text, metadata=metadata)]
```

### Comparing `unstructured-0.7.9/unstructured/partition/docx.py` & `unstructured-0.8.0/unstructured/partition/docx.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,24 +103,25 @@
 Paragraph.runs = property(lambda self: _get_paragraph_runs(self))
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.DOCX)
 def partition_docx(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_page_breaks: bool = True,
+    include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .docx format into its document elements.
 
     Parameters
     ----------
-     filename
+    filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     metadata_filename
         The filename to use for the metadata. Relevant because partition_doc converts the
         document to .docx before partition. We want the original source filename in the
         metadata.
@@ -134,15 +135,14 @@
     elif file is not None:
         document = docx.Document(
             spooled_to_bytes_io_if_needed(
                 cast(Union[BinaryIO, SpooledTemporaryFile], file),
             ),
         )
 
-    metadata_filename = metadata_filename or filename
     elements: List[Element] = []
     table_index = 0
 
     headers_and_footers = _get_headers_and_footers(document, metadata_filename)
     if len(headers_and_footers) > 0:
         elements.extend(headers_and_footers[0][0])
 
@@ -182,15 +182,15 @@
             if len(headers_and_footers) > section:
                 headers = headers_and_footers[section][0]
                 elements.extend(headers)
 
         if page_number is not None and _element_contains_pagebreak(element_item):
             page_number += 1
             if include_page_breaks:
-                elements.append(PageBreak())
+                elements.append(PageBreak(text=""))
 
     return elements
 
 
 def _paragraph_to_element(paragraph: docx.text.paragraph.Paragraph) -> Optional[Text]:
     """Converts a docx Paragraph object into the appropriate unstructured document element.
     If the paragraph style is "Normal" or unknown, we try to predict the element type from the
@@ -284,27 +284,32 @@
 
     return headers_and_footers
 
 
 def convert_and_partition_docx(
     source_format: str,
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Converts a document to DOCX and then partitions it using partition_html. Works with
     any file format support by pandoc.
 
     Parameters
     ----------
     source_format
         The format of the source document, .e.g. odt
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
+    include_metadata
+        Determines whether or not metadata is included in the metadata attribute on the
+        elements in the output.
     """
     if filename is None:
         filename = ""
     exactly_one(filename=filename, file=file)
 
     if len(filename) > 0:
         _, filename_no_path = os.path.split(os.path.abspath(filename))
@@ -324,10 +329,14 @@
         docx_filename = os.path.join(tmpdir, f"{base_filename}.docx")
         pypandoc.convert_file(
             filename,
             "docx",
             format=source_format,
             outputfile=docx_filename,
         )
-        elements = partition_docx(filename=docx_filename, metadata_filename=filename)
+        elements = partition_docx(
+            filename=docx_filename,
+            metadata_filename=metadata_filename,
+            include_metadata=include_metadata,
+        )
 
     return elements
```

### Comparing `unstructured-0.7.9/unstructured/partition/email.py` & `unstructured-0.8.0/unstructured/partition/email.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import datetime
 import email
+import os
 import re
 import sys
 from email.message import Message
 from functools import partial
-from tempfile import SpooledTemporaryFile
-from typing import IO, Dict, List, Optional, Tuple, Union
+from tempfile import SpooledTemporaryFile, TemporaryDirectory
+from typing import IO, Callable, Dict, List, Optional, Tuple, Union
 
 from unstructured.file_utils.encoding import (
     COMMON_ENCODINGS,
     format_encoding_str,
     read_txt_file,
+    validate_encoding,
 )
 from unstructured.partition.common import (
     convert_to_bytes,
     exactly_one,
 )
 
 if sys.version_info < (3, 8):
@@ -189,62 +191,77 @@
     element.text = element.text.replace("[image: " + image_info[:-1] + "]", "")
 
     return Image(text=image_info[:-1]), element
 
 
 def parse_email(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
 ) -> Tuple[Optional[str], Message]:
     if filename is not None:
         with open(filename, "rb") as f:
             msg = email.message_from_binary_file(f)
     elif file is not None:
         f_bytes = convert_to_bytes(file)
         msg = email.message_from_bytes(f_bytes)
     else:
         raise ValueError("Either 'filename' or 'file' must be provided.")
 
     encoding = None
     charsets = msg.get_charsets() or []
     for charset in charsets:
-        if charset and charset.strip():
+        if charset and charset.strip() and validate_encoding(charset):
             encoding = charset
             break
 
     formatted_encoding = format_encoding_str(encoding) if encoding else None
 
     return formatted_encoding, msg
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.EML)
 def partition_email(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     text: Optional[str] = None,
     content_source: str = "text/html",
     encoding: Optional[str] = None,
     include_headers: bool = False,
+    max_partition: Optional[int] = 1500,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
+    process_attachments: bool = False,
+    attachment_partitioner: Optional[Callable] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .eml documents into its constituent elements.
     Parameters
     ----------
-     filename
+    filename
         A string defining the target filename path.
     file
         A file-like object using "r" mode --> open(filename, "r").
     text
         The string representation of the .eml document.
     content_source
         default: "text/html"
         other: "text/plain"
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
+    max_partition
+        The maximum number of characters to include in a partition. If None is passed,
+        no maximum is applied. Only applies if processing the text/plain content.
+    metadata_filename
+        The filename to use for the metadata.
+    process_attachments
+        If True, partition_email will process email attachments in addition to
+        processing the content of the email itself.
+    attachment_partitioner
+        The partitioning function to use to process attachments.
     """
     if content_source not in VALID_CONTENT_SOURCES:
         raise ValueError(
             f"{content_source} is not a valid value for content_source. "
             f"Valid content sources are: {VALID_CONTENT_SOURCES}",
         )
 
@@ -268,15 +285,14 @@
             detected_encoding = extracted_encoding
         else:
             detected_encoding, file_text = read_txt_file(file=file, encoding=encoding)
             msg = email.message_from_string(file_text)
     elif text is not None:
         _text: str = str(text)
         msg = email.message_from_string(_text)
-
     if not encoding:
         encoding = detected_encoding
 
     content_map: Dict[str, str] = {}
     for part in msg.walk():
         # NOTE(robinson) - content dispostiion is None for the content of the email itself.
         # Other dispositions include "attachment" for attachments
@@ -295,15 +311,19 @@
         # you don't clean it up
         # <ul> =
         #    <li>Item 1</li>=
         #    <li>Item 2<li>=
         # </ul>
         list_content = content.split("=\n")
         content = "".join(list_content)
-        elements = partition_html(text=content, include_metadata=False)
+        elements = partition_html(
+            text=content,
+            include_metadata=False,
+            metadata_filename=metadata_filename,
+        )
         for element in elements:
             if isinstance(element, Text):
                 _replace_mime_encodings = partial(replace_mime_encodings, encoding=encoding)
                 try:
                     element.apply(_replace_mime_encodings)
                 except (UnicodeDecodeError, UnicodeError):
                     # If decoding fails, try decoding through common encodings
@@ -319,25 +339,48 @@
                             element.apply(_replace_mime_encodings)
                             break
                         except (UnicodeDecodeError, UnicodeError):
                             continue
 
     elif content_source == "text/plain":
         list_content = split_by_paragraph(content)
-        elements = partition_text(text=content, encoding=encoding)
+        elements = partition_text(
+            text=content,
+            encoding=encoding,
+            max_partition=max_partition,
+            metadata_filename=metadata_filename or filename,
+        )
 
     for idx, element in enumerate(elements):
         indices = has_embedded_image(element)
         if (isinstance(element, (NarrativeText, Title))) and indices:
             image_info, clean_element = find_embedded_image(element, indices)
             elements[idx] = clean_element
             elements.insert(idx + 1, image_info)
 
     header: List[Element] = []
     if include_headers:
         header = partition_email_header(msg)
     all_elements = header + elements
 
-    metadata = build_email_metadata(msg, filename=filename)
+    metadata = build_email_metadata(msg, filename=metadata_filename or filename)
     for element in all_elements:
         element.metadata = metadata
+
+    if process_attachments:
+        with TemporaryDirectory() as tmpdir:
+            extract_attachment_info(msg, tmpdir)
+            attached_files = os.listdir(tmpdir)
+            for attached_file in attached_files:
+                attached_filename = os.path.join(tmpdir, attached_file)
+                if attachment_partitioner is None:
+                    raise ValueError(
+                        "Specify the attachment_partitioner kwarg to process attachments.",
+                    )
+                attached_elements = attachment_partitioner(filename=attached_filename)
+                for element in attached_elements:
+                    element.metadata.filename = attached_file
+                    element.metadata.file_directory = None
+                    element.metadata.attached_to_filename = metadata_filename or filename
+                    all_elements.append(element)
+
     return all_elements
```

### Comparing `unstructured-0.7.9/unstructured/partition/epub.py` & `unstructured-0.8.0/unstructured/partition/epub.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from unstructured.partition.html import convert_and_partition_html
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.EPUB)
 def partition_epub(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an EPUB document. The document is first converted to HTML and then
     partitoned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
+        If True, the output will include page breaks if the filetype supports it.
     """
     return convert_and_partition_html(
         source_format="epub",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
+        metadata_filename=metadata_filename,
     )
```

### Comparing `unstructured-0.7.9/unstructured/partition/html.py` & `unstructured-0.8.0/unstructured/partition/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 )
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.HTML)
 def partition_html(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     encoding: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     parser: VALID_PARSERS = None,
     html_assemble_articles: bool = False,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an HTML document into its constituent elements.
 
     Parameters
     ----------
     filename
@@ -58,15 +59,14 @@
         If the URL parameter is set, determines whether or not partition uses SSL verification
         in the HTTP request.
     parser
         The parser to use for parsing the HTML document. If None, default parser will be used.
     """
     if text is not None and text.strip() == "" and not file and not filename and not url:
         return []
-
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text, url=url)
 
     if filename is not None:
         document = HTMLDocument.from_file(
             filename,
             parser=parser,
@@ -103,33 +103,36 @@
 
     return document_to_element_list(document, include_page_breaks=include_page_breaks)
 
 
 def convert_and_partition_html(
     source_format: str,
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
+    metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Converts a document to HTML and then partitions it using partition_html. Works with
     any file format support by pandoc.
 
     Parameters
     ----------
     source_format
         The format of the source document, i.e. rst
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
+        If True, the output will include page breaks if the filetype supports it.
+    metadata_filename
+        The filename to use in element metadata.
     """
     html_text = convert_file_to_html_text(source_format=source_format, filename=filename, file=file)
     # NOTE(robinson) - pypandoc returns a text string with unicode encoding
     # ref: https://github.com/JessicaTegner/pypandoc#usage
     return partition_html(
         text=html_text,
         include_page_breaks=include_page_breaks,
         encoding="unicode",
+        metadata_filename=metadata_filename,
     )
```

### Comparing `unstructured-0.7.9/unstructured/partition/json.py` & `unstructured-0.8.0/unstructured/partition/json.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,19 +9,31 @@
 from unstructured.staging.base import dict_to_elements
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.JSON)
 def partition_json(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     text: Optional[str] = None,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions an .json document into its constituent elements."""
+    """Partitions an .json document into its constituent elements.
+
+    Parameters
+    ----------
+    filename
+        A string defining the target filename path.
+    file
+        A file-like object as bytes --> open(filename, "rb").
+    text
+        The string representation of the .json document.
+    """
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     exactly_one(filename=filename, file=file, text=text)
 
     if filename is not None:
         with open(filename, encoding="utf8") as f:
```

### Comparing `unstructured-0.7.9/unstructured/partition/md.py` & `unstructured-0.8.0/unstructured/partition/md.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,22 +16,42 @@
     return contents
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.MD)
 def partition_md(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     parser: VALID_PARSERS = None,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
+    """Partitions a markdown file into its constituent elements
+
+    Parameters
+    ----------
+    filename
+        A string defining the target filename path.
+    file
+        A file-like object using "rb" mode --> open(filename, "rb").
+    text
+        The string representation of the markdown document.
+    url
+        The URL of a webpage to parse. Only for URLs that return a markdown document.
+    include_page_breaks
+        If True, the output will include page breaks if the filetype supports it.
+    include_metadata
+        Determines whether or not metadata is included in the output.
+    parser
+        The parser to use for parsing the markdown document. If None, default parser will be used.
+    """
     # Verify that only one of the arguments was provided
     if text is None:
         text = ""
     exactly_one(filename=filename, file=file, text=text, url=url)
 
     if filename is not None:
         with open(filename, encoding="utf8") as f:
@@ -54,8 +74,9 @@
     html = markdown.markdown(text)
 
     return partition_html(
         text=html,
         include_page_breaks=include_page_breaks,
         include_metadata=include_metadata,
         parser=parser,
+        metadata_filename=metadata_filename,
     )
```

### Comparing `unstructured-0.7.9/unstructured/partition/msg.py` & `unstructured-0.8.0/unstructured/partition/msg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import os
 import tempfile
-from typing import IO, Dict, List, Optional
+from typing import IO, Callable, Dict, List, Optional
 
 import msg_parser
 
 from unstructured.documents.elements import Element, ElementMetadata, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one
 from unstructured.partition.email import convert_to_iso_8601
@@ -11,25 +12,40 @@
 from unstructured.partition.text import partition_text
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.MSG)
 def partition_msg(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
+    max_partition: Optional[int] = 1500,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
+    process_attachments: bool = False,
+    attachment_partitioner: Optional[Callable] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions a MSFT Outlook .msg file
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
+    max_partition
+        The maximum number of characters to include in a partition. If None is passed,
+        no maximum is applied. Only applies if processing text/plain content.
+    metadata_filename
+        The filename to use for the metadata.
+    process_attachments
+        If True, partition_email will process email attachments in addition to
+        processing the content of the email itself.
+    attachment_partitioner
+        The partitioning function to use to process attachments.
     """
     exactly_one(filename=filename, file=file)
 
     if filename is not None:
         msg_obj = msg_parser.MsOxMessage(filename)
     elif file is not None:
         tmp = tempfile.NamedTemporaryFile(delete=False)
@@ -37,25 +53,42 @@
         tmp.close()
         msg_obj = msg_parser.MsOxMessage(tmp.name)
 
     text = msg_obj.body
     if "<html>" in text or "</div>" in text:
         elements = partition_html(text=text)
     else:
-        elements = partition_text(text=text)
+        elements = partition_text(text=text, max_partition=max_partition)
 
-    metadata = build_msg_metadata(msg_obj, filename)
+    metadata = build_msg_metadata(msg_obj, metadata_filename or filename)
     for element in elements:
         element.metadata = metadata
 
+    if process_attachments:
+        with tempfile.TemporaryDirectory() as tmpdir:
+            extract_msg_attachment_info(msg_obj=msg_obj, output_dir=tmpdir)
+            attached_files = os.listdir(tmpdir)
+            for attached_file in attached_files:
+                attached_filename = os.path.join(tmpdir, attached_file)
+                if attachment_partitioner is None:
+                    raise ValueError(
+                        "Specify the attachment_partitioner kwarg to process attachments.",
+                    )
+                attached_elements = attachment_partitioner(filename=attached_filename)
+                for element in attached_elements:
+                    element.metadata.filename = attached_file
+                    element.metadata.file_directory = None
+                    element.metadata.attached_to_filename = metadata_filename or filename
+                    elements.append(element)
+
     return elements
 
 
 def build_msg_metadata(msg_obj: msg_parser.MsOxMessage, filename: Optional[str]) -> ElementMetadata:
-    """Creates an ElementMetadata object from the header information in the emai."""
+    """Creates an ElementMetadata object from the header information in the email."""
     email_date = getattr(msg_obj, "sent_date", None)
     if email_date is not None:
         email_date = convert_to_iso_8601(email_date)
 
     sent_from = getattr(msg_obj, "sender", None)
     if sent_from is not None:
         sent_from = [str(sender) for sender in sent_from]
@@ -70,39 +103,42 @@
         subject=getattr(msg_obj, "subject", None),
         date=email_date,
         filename=filename,
     )
 
 
 def extract_msg_attachment_info(
-    filename: str,
-    file: Optional[IO] = None,
+    filename: Optional[str] = None,
+    file: Optional[IO[bytes]] = None,
     output_dir: Optional[str] = None,
+    msg_obj: Optional[msg_parser.MsOxMessage] = None,
 ) -> List[Dict[str, str]]:
-    exactly_one(filename=filename, file=file)
+    exactly_one(filename=filename, file=file, msg_obj=msg_obj)
 
     if filename is not None:
         msg_obj = msg_parser.MsOxMessage(filename)
     elif file is not None:
         tmp = tempfile.NamedTemporaryFile(delete=False)
         tmp.write(file.read())
         tmp.close()
         msg_obj = msg_parser.MsOxMessage(tmp.name)
+    elif msg_obj is not None:
+        msg_obj = msg_obj
 
     list_attachments = []
 
     for attachment in msg_obj.attachments:
         attachment_info = {}
 
         attachment_info["filename"] = attachment.AttachLongFilename
         attachment_info["extension"] = attachment.AttachExtension
         attachment_info["file_size"] = attachment.AttachmentSize
         attachment_info["payload"] = attachment.data
 
         list_attachments.append(attachment_info)
 
         if output_dir is not None:
-            filename = output_dir + "/" + attachment_info["filename"]
-            with open(filename, "wb") as f:
+            output_filename = output_dir + "/" + attachment_info["filename"]
+            with open(output_filename, "wb") as f:
                 f.write(attachment.data)
 
     return list_attachments
```

### Comparing `unstructured-0.7.9/unstructured/partition/odt.py` & `unstructured-0.8.0/unstructured/partition/odt.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 from unstructured.partition.docx import convert_and_partition_docx
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.ODT)
 def partition_odt(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Open Office Documents in .odt format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     """
-    return convert_and_partition_docx(source_format="odt", filename=filename, file=file)
+    return convert_and_partition_docx(
+        source_format="odt",
+        filename=filename,
+        file=file,
+        metadata_filename=metadata_filename,
+    )
```

### Comparing `unstructured-0.7.9/unstructured/partition/org.py` & `unstructured-0.8.0/unstructured/partition/org.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
 @add_metadata_with_filetype(FileType.ORG)
 def partition_org(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Partitions an org document. The document is first converted to HTML and then
     partitioned using partition_html.
 
     Parameters
     ----------
     filename
@@ -24,8 +26,9 @@
         If True, the output will include page breaks if the filetype supports it
     """
     return convert_and_partition_html(
         source_format="org",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
+        metadata_filename=metadata_filename,
     )
```

### Comparing `unstructured-0.7.9/unstructured/partition/ppt.py` & `unstructured-0.8.0/unstructured/partition/xlsx.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,65 @@
-import os
-import tempfile
-from typing import IO, List, Optional
+from tempfile import SpooledTemporaryFile
+from typing import IO, BinaryIO, List, Optional, Union, cast
 
-from unstructured.documents.elements import Element, process_metadata
+import lxml.html
+import pandas as pd
+
+from unstructured.documents.elements import (
+    Element,
+    ElementMetadata,
+    Table,
+    process_metadata,
+)
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import convert_office_doc, exactly_one
-from unstructured.partition.pptx import partition_pptx
+from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.PPT)
-def partition_ppt(
+@add_metadata_with_filetype(FileType.XLSX)
+def partition_xlsx(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
-    include_page_breaks: bool = False,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
+    metadata_filename: Optional[str] = None,
+    include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
-    """Partitions Microsoft PowerPoint Documents in .ppt format into their document elements.
+    """Partitions Microsoft Excel Documents in .xlsx format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    include_page_breaks
-        If True, includes a PageBreak element between slides
+    include_metadata
+        Determines whether or not metadata is included in the output.
     """
-    # Verify that only one of the arguments was provided
-    if filename is None:
-        filename = ""
     exactly_one(filename=filename, file=file)
 
-    if len(filename) > 0:
-        _, filename_no_path = os.path.split(os.path.abspath(filename))
-        base_filename, _ = os.path.splitext(filename_no_path)
-        if not os.path.exists(filename):
-            raise ValueError(f"The file {filename} does not exist.")
-    elif file is not None:
-        tmp = tempfile.NamedTemporaryFile(delete=False)
-        tmp.write(file.read())
-        tmp.close()
-        filename = tmp.name
-        _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
-
-    base_filename, _ = os.path.splitext(filename_no_path)
-
-    with tempfile.TemporaryDirectory() as tmpdir:
-        convert_office_doc(filename, tmpdir, target_format="pptx")
-        pptx_filename = os.path.join(tmpdir, f"{base_filename}.pptx")
-        elements = partition_pptx(filename=pptx_filename, metadata_filename=filename)
+    if filename:
+        sheets = pd.read_excel(filename, sheet_name=None)
+    else:
+        f = spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file))
+        sheets = pd.read_excel(f, sheet_name=None)
+
+    elements: List[Element] = []
+    page_number = 0
+    for sheet_name, table in sheets.items():
+        page_number += 1
+        html_text = table.to_html(index=False, header=False, na_rep="")
+        text = lxml.html.document_fromstring(html_text).text_content()
+
+        if include_metadata:
+            metadata = ElementMetadata(
+                text_as_html=html_text,
+                page_name=sheet_name,
+                page_number=page_number,
+                filename=metadata_filename or filename,
+            )
+        else:
+            metadata = ElementMetadata()
+
+        table = Table(text=text, metadata=metadata)
+        elements.append(table)
 
     return elements
```

### Comparing `unstructured-0.7.9/unstructured/partition/pptx.py` & `unstructured-0.8.0/unstructured/partition/pptx.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 OPENXML_SCHEMA_NAME = "{http://schemas.openxmlformats.org/drawingml/2006/main}"
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.PPTX)
 def partition_pptx(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     include_page_breaks: bool = True,
     metadata_filename: Optional[str] = None,
+    include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .pptx format into its document elements.
 
     Parameters
     ----------
      filename
@@ -60,29 +61,28 @@
         presentation = pptx.Presentation(filename)
     elif file is not None:
         presentation = pptx.Presentation(
             spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file)),
         )
 
     elements: List[Element] = []
-    metadata_filename = metadata_filename or filename
-    metadata = ElementMetadata(filename=metadata_filename)
+    metadata = ElementMetadata(filename=metadata_filename or filename)
     num_slides = len(presentation.slides)
     for i, slide in enumerate(presentation.slides):
-        metadata = ElementMetadata(**metadata.to_dict())
+        metadata = ElementMetadata.from_dict(metadata.to_dict())
         metadata.page_number = i + 1
 
         for shape in _order_shapes(slide.shapes):
             if shape.has_table:
                 table: pptx.table.Table = shape.table
                 html_table = convert_ms_office_table_to_text(table, as_html=True)
                 text_table = convert_ms_office_table_to_text(table, as_html=False)
                 if (text_table := text_table.strip()) != "":
                     metadata = ElementMetadata(
-                        filename=metadata_filename,
+                        filename=metadata_filename or filename,
                         text_as_html=html_table,
                         page_number=metadata.page_number,
                     )
                     elements.append(Table(text=text_table, metadata=metadata))
                 continue
             if not shape.has_text_frame:
                 continue
@@ -100,15 +100,15 @@
                     elements.append(NarrativeText(text=text, metadata=metadata))
                 elif is_possible_title(text):
                     elements.append(Title(text=text, metadata=metadata))
                 else:
                     elements.append(Text(text=text, metadata=metadata))
 
         if include_page_breaks and i < num_slides - 1:
-            elements.append(PageBreak())
+            elements.append(PageBreak(text=""))
 
     return elements
 
 
 def _order_shapes(shapes):
     """Orders the shapes from top to bottom and left to right."""
     return sorted(shapes, key=lambda x: (x.top or 0, x.left or 0))
```

### Comparing `unstructured-0.7.9/unstructured/partition/rst.py` & `unstructured-0.8.0/unstructured/partition/rst.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from unstructured.partition.html import convert_and_partition_html
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.RST)
 def partition_rst(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an RST document. The document is first converted to HTML and then
     partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
+        If True, the output will include page breaks if the filetype supports it.
     """
     return convert_and_partition_html(
         source_format="rst",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
+        metadata_filename=metadata_filename,
     )
```

### Comparing `unstructured-0.7.9/unstructured/partition/rtf.py` & `unstructured-0.8.0/unstructured/partition/rtf.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from unstructured.partition.html import convert_and_partition_html
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.RTF)
 def partition_rtf(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
+    include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an RTF document. The document is first converted to HTML and then
     partitioned using partiton_html.
 
     Parameters
     ----------
@@ -26,8 +28,9 @@
         If True, the output will include page breaks if the filetype supports it
     """
     return convert_and_partition_html(
         source_format="rtf",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
+        metadata_filename=metadata_filename,
     )
```

### Comparing `unstructured-0.7.9/unstructured/partition/strategies.py` & `unstructured-0.8.0/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/partition/text.py` & `unstructured-0.8.0/unstructured/partition/doc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,62 @@
-import re
-from typing import IO, Callable, List, Optional
+import os
+import tempfile
+from typing import IO, List, Optional
 
-from unstructured.cleaners.core import clean_bullets, group_broken_paragraphs
-from unstructured.documents.elements import (
-    Address,
-    Element,
-    ElementMetadata,
-    ListItem,
-    NarrativeText,
-    Text,
-    Title,
-    process_metadata,
-)
-from unstructured.file_utils.encoding import read_txt_file
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.nlp.patterns import PARAGRAPH_PATTERN
-from unstructured.partition.common import exactly_one
-from unstructured.partition.text_type import (
-    is_bulleted_text,
-    is_possible_narrative_text,
-    is_possible_title,
-    is_us_city_state_zip,
-)
-
-
-def split_by_paragraph(content: str) -> List[str]:
-    return re.split(PARAGRAPH_PATTERN, content)
+from unstructured.partition.common import convert_office_doc, exactly_one
+from unstructured.partition.docx import partition_docx
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.TXT)
-def partition_text(
+@add_metadata_with_filetype(FileType.DOC)
+def partition_doc(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
-    text: Optional[str] = None,
-    encoding: Optional[str] = None,
-    paragraph_grouper: Optional[Callable[[str], str]] = None,
-    metadata_filename: Optional[str] = None,
+    file: Optional[IO[bytes]] = None,
+    include_page_breaks: bool = True,
     include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions an .txt documents into its constituent elements.
+    """Partitions Microsoft Word Documents in .doc format into its document elements.
+
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
-        A file-like object using "r" mode --> open(filename, "r").
-    text
-        The string representation of the .txt document.
-    encoding
-        The encoding method used to decode the text input. If None, utf-8 will be used.
-    paragrapher_grouper
-        A str -> str function for fixing paragraphs that are interrupted by line breaks
-        for formatting purposes.
-    include_metadata
-        Determines whether or not metadata is included in the output.
+        A file-like object using "rb" mode --> open(filename, "rb").
     """
-    if text is not None and text.strip() == "" and not file and not filename:
-        return []
-
     # Verify that only one of the arguments was provided
-    exactly_one(filename=filename, file=file, text=text)
-
-    if filename is not None:
-        encoding, file_text = read_txt_file(filename=filename, encoding=encoding)
-
+    if filename is None:
+        filename = ""
+    exactly_one(filename=filename, file=file)
+
+    if len(filename) > 0:
+        _, filename_no_path = os.path.split(os.path.abspath(filename))
+        base_filename, _ = os.path.splitext(filename_no_path)
+        if not os.path.exists(filename):
+            raise ValueError(f"The file {filename} does not exist.")
     elif file is not None:
-        encoding, file_text = read_txt_file(file=file, encoding=encoding)
-
-    elif text is not None:
-        file_text = str(text)
-
-    if paragraph_grouper is not None:
-        file_text = paragraph_grouper(file_text)
-    else:
-        file_text = group_broken_paragraphs(file_text)
-
-    file_content = split_by_paragraph(file_text)
-
-    metadata_filename = metadata_filename or filename
-
-    elements: List[Element] = []
-    metadata = (
-        ElementMetadata(filename=metadata_filename) if include_metadata else ElementMetadata()
-    )
-    for ctext in file_content:
-        ctext = ctext.strip()
-
-        if ctext:
-            element = element_from_text(ctext)
-            element.metadata = metadata
-            elements.append(element)
+        tmp = tempfile.NamedTemporaryFile(delete=False)
+        tmp.write(file.read())
+        tmp.close()
+        filename = tmp.name
+        _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
+        base_filename, _ = os.path.splitext(filename_no_path)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        convert_office_doc(filename, tmpdir, target_format="docx")
+        docx_filename = os.path.join(tmpdir, f"{base_filename}.docx")
+        elements = partition_docx(
+            filename=docx_filename,
+            metadata_filename=metadata_filename,
+            include_page_breaks=include_page_breaks,
+            include_metadata=include_metadata,
+        )
+        # remove tmp.name from filename if parsing file
+        if file:
+            for element in elements:
+                element.metadata.filename = metadata_filename
 
     return elements
-
-
-def element_from_text(text: str) -> Element:
-    if is_bulleted_text(text):
-        return ListItem(text=clean_bullets(text))
-    elif is_us_city_state_zip(text):
-        return Address(text=text)
-    elif is_possible_narrative_text(text):
-        return NarrativeText(text=text)
-    elif is_possible_title(text):
-        return Title(text=text)
-    else:
-        return Text(text=text)
```

### Comparing `unstructured-0.7.9/unstructured/partition/text_type.py` & `unstructured-0.8.0/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/partition/tsv.py` & `unstructured-0.8.0/unstructured/partition/ppt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-from tempfile import SpooledTemporaryFile
-from typing import IO, BinaryIO, List, Optional, Union, cast
+import os
+import tempfile
+from typing import IO, List, Optional
 
-import lxml.html
-import pandas as pd
-
-from unstructured.documents.elements import (
-    Element,
-    ElementMetadata,
-    Table,
-    process_metadata,
-)
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
+from unstructured.partition.common import convert_office_doc, exactly_one
+from unstructured.partition.pptx import partition_pptx
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.TSV)
-def partition_tsv(
+@add_metadata_with_filetype(FileType.PPT)
+def partition_ppt(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
-    metadata_filename: Optional[str] = None,
+    file: Optional[IO[bytes]] = None,
+    include_page_breaks: bool = False,
     include_metadata: bool = True,
+    metadata_filename: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions TSV files into document elements.
+    """Partitions Microsoft PowerPoint Documents in .ppt format into their document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    metadata_filename
-        The filename to use for the metadata.
-    include_metadata
-        Determines whether or not metadata is included in the output.
+    include_page_breaks
+        If True, includes a PageBreak element between slides
     """
+    # Verify that only one of the arguments was provided
+    if filename is None:
+        filename = ""
     exactly_one(filename=filename, file=file)
 
-    if filename:
-        table = pd.read_csv(filename, sep="\t")
-    else:
-        f = spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file))
-        table = pd.read_csv(f, sep="\t")
-
-    metadata_filename = filename or metadata_filename
-
-    html_text = table.to_html(index=False, header=False, na_rep="")
-    text = lxml.html.document_fromstring(html_text).text_content()
-
-    if include_metadata:
-        metadata = ElementMetadata(
-            text_as_html=html_text,
-            filename=metadata_filename,
-        )
-    else:
-        metadata = ElementMetadata()
+    if len(filename) > 0:
+        _, filename_no_path = os.path.split(os.path.abspath(filename))
+        base_filename, _ = os.path.splitext(filename_no_path)
+        if not os.path.exists(filename):
+            raise ValueError(f"The file {filename} does not exist.")
+    elif file is not None:
+        tmp = tempfile.NamedTemporaryFile(delete=False)
+        tmp.write(file.read())
+        tmp.close()
+        filename = tmp.name
+        _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
+
+    base_filename, _ = os.path.splitext(filename_no_path)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        convert_office_doc(filename, tmpdir, target_format="pptx")
+        pptx_filename = os.path.join(tmpdir, f"{base_filename}.pptx")
+        elements = partition_pptx(filename=pptx_filename, metadata_filename=metadata_filename)
+
+    # remove tmp.name from filename if parsing file
+    if file:
+        for element in elements:
+            element.metadata.filename = metadata_filename
 
-    return [Table(text=text, metadata=metadata)]
+    return elements
```

### Comparing `unstructured-0.7.9/unstructured/partition/xml.py` & `unstructured-0.8.0/unstructured/partition/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def is_string(elem):
     return isinstance(elem, str) or (hasattr(elem, "text") and isinstance(elem.text, str))
 
 
 def get_leaf_elements(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     xml_path: str = ".",
 ):
     if filename:
         _, raw_text = read_txt_file(filename=filename)
     elif file:
         f = spooled_to_bytes_io_if_needed(
             cast(Union[BinaryIO, SpooledTemporaryFile], file),
@@ -43,20 +43,21 @@
     return "\n".join(leaf_elements)  # type: ignore
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.XML)
 def partition_xml(
     filename: Optional[str] = None,
-    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     xml_keep_tags: bool = False,
     xml_path: str = ".",
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
     encoding: Optional[str] = None,
+    max_partition: Optional[int] = 1500,
     **kwargs,
 ) -> List[Element]:
     """Partitions an XML document into its document elements.
 
     Parameters
     ----------
     filename
@@ -64,24 +65,24 @@
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     xml_keep_tags
         If True, will retain the XML tags in the output. Otherwise it will simply extract
         the text from within the tags.
     xml_path
         The xml_path to use for extracting the text. Only used if xml_keep_tags=False
-    metadata_filename
-        The filename to use for the metadata.
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     include_metadata
         Determines whether or not metadata is included in the metadata attribute on the
         elements in the output.
+    max_partition
+        The maximum number of characters to include in a partition. If None is passed,
+        no maximum is applied.
     """
     exactly_one(filename=filename, file=file)
-    metadata_filename = metadata_filename or filename
 
     if xml_keep_tags:
         if filename:
             _, raw_text = read_txt_file(filename=filename, encoding=encoding)
         elif file:
             f = spooled_to_bytes_io_if_needed(
                 cast(Union[BinaryIO, SpooledTemporaryFile], file),
@@ -91,10 +92,11 @@
             raise ValueError("Either 'filename' or 'file' must be provided.")
     else:
         raw_text = get_leaf_elements(filename=filename, file=file, xml_path=xml_path)
     elements = partition_text(
         text=raw_text,
         metadata_filename=metadata_filename,
         include_metadata=include_metadata,
+        max_partition=max_partition,
     )
 
     return elements
```

### Comparing `unstructured-0.7.9/unstructured/staging/argilla.py` & `unstructured-0.8.0/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/staging/base.py` & `unstructured-0.8.0/unstructured/staging/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import csv
 import io
 import json
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 import pandas as pd
 
-from unstructured.documents import coordinates as coordinates_module
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     Element,
     ElementMetadata,
     NoID,
 )
 from unstructured.partition.common import exactly_one
 
 TABLE_FIELDNAMES: List[str] = [
     "type",
     "text",
     "element_id",
-    "coordinates",
-    "coordinate_system",
-    "layout_width",
-    "layout_height",
+    "coordinates_points",
+    "coordinates_system",
+    "coordinates_layout_width",
+    "coordinates_layout_height",
     "filename",
     "page_number",
     "url",
     "sent_from",
     "sent_to",
     "subject",
     "sender",
@@ -68,51 +67,34 @@
 
 def isd_to_elements(isd: List[Dict[str, Any]]) -> List[Element]:
     """Converts an Initial Structured Data (ISD) dictionary to a list of elements."""
     elements: List[Element] = []
 
     for item in isd:
         element_id: str = item.get("element_id", NoID())
-        coord_value: Optional[List[List[float]]] = item.get("coordinates")
-        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None
-        if coord_value is not None:
-            coordinates = tuple((x, y) for x, y in coord_value)
-        coordinate_system_name: Optional[str] = item.get("coordinate_system")
-        if coordinate_system_name is not None:
-            width = item["layout_width"]
-            height = item["layout_height"]
-            coordinate_system_class = getattr(coordinates_module, coordinate_system_name)
-            coordinate_system = coordinate_system_class(width, height)
-        else:
-            coordinate_system = None
-
         metadata = ElementMetadata()
         _metadata_dict = item.get("metadata")
         if _metadata_dict is not None:
             metadata = ElementMetadata.from_dict(_metadata_dict)
 
-        if item["type"] in TYPE_TO_TEXT_ELEMENT_MAP:
+        if item.get("type") in TYPE_TO_TEXT_ELEMENT_MAP:
             _text_class = TYPE_TO_TEXT_ELEMENT_MAP[item["type"]]
             elements.append(
                 _text_class(
                     text=item["text"],
                     element_id=element_id,
                     metadata=metadata,
-                    coordinates=coordinates,
-                    coordinate_system=coordinate_system,
                 ),
             )
-        elif item["type"] == "CheckBox":
+        elif item.get("type") == "CheckBox":
             elements.append(
                 CheckBox(
                     checked=item["checked"],
                     element_id=element_id,
                     metadata=metadata,
-                    coordinates=coordinates,
-                    coordinate_system=coordinate_system,
                 ),
             )
 
     return elements
 
 
 def dict_to_elements(element_dict: List[Dict[str, Any]]) -> List[Element]:
@@ -133,24 +115,35 @@
             element_dict = json.load(f)
         return dict_to_elements(element_dict)
     else:
         element_dict = json.loads(text)
         return dict_to_elements(element_dict)
 
 
+def flatten_dict(dictionary, parent_key="", separator="_"):
+    flattened_dict = {}
+    for key, value in dictionary.items():
+        new_key = f"{parent_key}{separator}{key}" if parent_key else key
+        if isinstance(value, dict):
+            flattened_dict.update(flatten_dict(value, new_key, separator))
+        else:
+            flattened_dict[new_key] = value
+    return flattened_dict
+
+
 def convert_to_isd_csv(elements: List[Element]) -> str:
     """
     Returns the representation of document elements as an Initial Structured Document (ISD)
     in CSV Format.
     """
     rows: List[Dict[str, Any]] = convert_to_isd(elements)
     # NOTE(robinson) - flatten metadata and add it to the table
     for row in rows:
         metadata = row.pop("metadata")
-        for key, value in metadata.items():
+        for key, value in flatten_dict(metadata).items():
             if key in TABLE_FIELDNAMES:
                 row[key] = value
 
         if row.get("sent_from"):
             row["sender"] = row.get("sent_from")
             if type(row["sender"]) == list:
                 row["sender"] = row["sender"][0]
```

### Comparing `unstructured-0.7.9/unstructured/staging/baseplate.py` & `unstructured-0.8.0/unstructured/staging/baseplate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List, TypedDict
 
 from unstructured.documents.elements import Text
+from unstructured.staging.base import flatten_dict
 
 
 class BaseplateRow(TypedDict):
     """Typed dictionary for an individual Baseplate row. Baseplate docs show what the JSON
     representation should look like:
         https://docs.baseplate.ai/api-reference/documents/overview
     """
@@ -28,18 +29,22 @@
     into Baseplate via the API.
 
     References
     ----------
     https://docs.baseplate.ai/api-reference/documents/overview
     https://docs.baseplate.ai/api-reference/documents/upsert-data-rows
     """
+
     rows: List[BaseplateRow] = []
     for element in elements:
         element_dict = element.to_dict()
         metadata = element_dict.pop("metadata")
         row: BaseplateRow = {
-            "data": element_dict,
-            "metadata": metadata,
+            # Baseplate maps each key in the row's data object to a column in the dataset and
+            # each key in the row's metadata object to a metadata column in the dataset.
+            # We infer that Baseplate cannot map a nested object to a column in its dataset.
+            "data": flatten_dict(element_dict),
+            "metadata": flatten_dict(metadata),
         }
         rows.append(row)
 
     return {"rows": rows}
```

### Comparing `unstructured-0.7.9/unstructured/staging/datasaur.py` & `unstructured-0.8.0/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/staging/huggingface.py` & `unstructured-0.8.0/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/staging/label_box.py` & `unstructured-0.8.0/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/staging/label_studio.py` & `unstructured-0.8.0/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/staging/prodigy.py` & `unstructured-0.8.0/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured/staging/weaviate.py` & `unstructured-0.8.0/unstructured/staging/weaviate.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,32 @@
 
 
 class Properties(TypedDict):
     name: str
     dataType: List[str]
 
 
+exclude_metadata_keys = ("data_source", "coordinates")
+
+
 def stage_for_weaviate(elements: List[Text]) -> List[Dict[str, Any]]:
     """Converts a list of elements into a list of dictionaries that can be uploaded to
     Weaviate. The outputs will conform to the schema created with
     create_unstructured_weaviate_class.
 
     References
     ----------
     https://weaviate.io/developers/weaviate/tutorials/import#batch-import-process
     """
     data: List[Dict[str, Any]] = []
     for element in elements:
         properties = element.metadata.to_dict()
+        for k in exclude_metadata_keys:
+            if k in properties:
+                del properties[k]
         properties["text"] = element.text
         properties["category"] = element.category
         data.append(properties)
 
     return data
 
 
@@ -49,16 +55,14 @@
         },
         {
             "name": "category",
             "dataType": ["text"],
         },
     ]
 
-    exclude_metadata_keys = ["data_source"]
-
     for name, annotation in ElementMetadata.__annotations__.items():
         if name not in exclude_metadata_keys:
             data_type = _annotation_to_weaviate_data_type(annotation)
             properties.append(
                 {
                     "name": name,
                     "dataType": data_type,
```

### Comparing `unstructured-0.7.9/unstructured/utils.py` & `unstructured-0.8.0/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.9/unstructured.egg-info/PKG-INFO` & `unstructured-0.8.0/unstructured.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.9
+Version: 0.8.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -38,16 +38,16 @@
         </div>
         
         <h3 align="center">
           <p>API Announcement!</p>
         </h3>
         
         <p>While access to the hosted Unstructured API will remain free, API Keys will soon be required to make requests. To prevent any disruption, get yours <a href="https://www.unstructured.io/api-key/">here</a> now and start using it today!</p>
-          
-        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. 
+        
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls.
         We'd love to hear your feedback, let us know how it goes in our
           community slack. And stay tuned for improvements to both quality and performance!</p>
         
         <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
@@ -102,35 +102,35 @@
         the partitioning function listed in the table directly.
         See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
         about the library.
         
         | Document Type | Partition Function | Strategies | Table Support | Options |
         | --- | --- | --- | --- | --- |
         | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
-        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
-        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
+        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max Partition; Process Attachments |
+        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding; Max Partition; Process Attachments |
         | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
         | Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
-        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
+        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR Languages, Strategy |
+        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding; Max Partition; Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
         | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
-        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
+        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags |
         
         
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
@@ -311,7 +311,9 @@
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
 Provides-Extra: gcs
+Provides-Extra: elasticsearch
+Provides-Extra: dropbox
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.9 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -60,38 +60,40 @@
 `unstructured` library currently supports. `partition` will recognize each of
 these document types and route the document to the appropriate partitioning
 function. If you already know your document type, you can use the partitioning
 function listed in the table directly. See our [documentation page](https://
 unstructured-io.github.io/unstructured/) for more details about the library. |
 Document Type | Partition Function | Strategies | Table Support | Options | | -
 -- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
-| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
-(`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
+| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max
+Partition; Process Attachments | | E-mails (`.msg`) | `partition_msg` | N/A |
+No | Encoding; Max Partition; Process Attachments | | EPubs (`.epub`) |
 `partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
 (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
 | `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
 (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
 Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
-Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
-Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
-Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
-Include Page Breaks | | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None
-| | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | | Word
-Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | Word Documents
-(`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
-(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
-Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
-:dizzy: Instructions for using the docker image The following instructions are
+| Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR
+Languages, Strategy | | Plain Text (`.txt`) | `partition_text` | N/A | No |
+Encoding; Max Partition; Paragraph Grouper | | Power Points (`.ppt`) |
+`partition_ppt` | N/A | Yes | Include Page Breaks | | Power Points (`.pptx`) |
+`partition_pptx` | N/A | Yes | Include Page Breaks | | ReStructured Text
+(`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks | | Rich Text
+Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks | | TSV
+Files (`.tsv`) | `partition_tsv` | N/A | Yes | None | | Word Documents (`.doc`)
+| `partition_doc` | N/A | Yes | None | | Word Documents (`.docx`) |
+`partition_docx` | N/A | Yes | None | | Word Documents (`.doc`) |
+`partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents (`.docx`)
+| `partition_docx` | N/A | Yes | Include Page Breaks | | XML Documents (`.xml`)
+| `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags | ## :
+dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
 with `--platform` (e.g. `--platform linux/amd64`) if needed. We build Docker
 images for all pushes to `main`. We tag each image with the corresponding short
@@ -205,8 +207,8 @@
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
 Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
 discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
 Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
-Provides-Extra: gcs
+Provides-Extra: gcs Provides-Extra: elasticsearch Provides-Extra: dropbox
```

### Comparing `unstructured-0.7.9/unstructured.egg-info/SOURCES.txt` & `unstructured-0.8.0/unstructured.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.cfg
 setup.py
 requirements/base.in
 requirements/huggingface.in
 requirements/ingest-azure.in
 requirements/ingest-discord.in
+requirements/ingest-dropbox.in
 requirements/ingest-gcs.in
 requirements/ingest-github.in
 requirements/ingest-gitlab.in
 requirements/ingest-google-drive.in
 requirements/ingest-reddit.in
 requirements/ingest-s3.in
 requirements/ingest-slack.in
@@ -54,14 +55,16 @@
 unstructured/ingest/interfaces.py
 unstructured/ingest/logger.py
 unstructured/ingest/main.py
 unstructured/ingest/connector/__init__.py
 unstructured/ingest/connector/azure.py
 unstructured/ingest/connector/biomed.py
 unstructured/ingest/connector/discord.py
+unstructured/ingest/connector/dropbox.py
+unstructured/ingest/connector/elasticsearch.py
 unstructured/ingest/connector/fsspec.py
 unstructured/ingest/connector/gcs.py
 unstructured/ingest/connector/git.py
 unstructured/ingest/connector/github.py
 unstructured/ingest/connector/gitlab.py
 unstructured/ingest/connector/google_drive.py
 unstructured/ingest/connector/local.py
```

