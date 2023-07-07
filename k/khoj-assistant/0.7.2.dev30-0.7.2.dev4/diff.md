# Comparing `tmp/khoj_assistant-0.7.2.dev30.tar.gz` & `tmp/khoj_assistant-0.7.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Jul  7 19:49:58 2023, max compression
+gzip compressed data, last modified: Tue Jul  4 05:28:18 2023, max compression
```

## Comparing `khoj_assistant-0.7.2.dev30.tar` & `khoj_assistant-0.7.2.dev4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/__init__.py
--rw-r--r--   0        0        0    11056 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/configure.py
--rw-r--r--   0        0        0     5247 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3910 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    17566 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    13551 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    18840 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3661 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6331 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4065 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8709 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5392 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    20365 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4646 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2385 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2500 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6889 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4136 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/LICENSE
--rw-r--r--   0        0        0    24572 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/README.md
--rw-r--r--   0        0        0     2792 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/pyproject.toml
--rw-r--r--   0        0        0    26937 2023-07-07 19:49:58.000000 khoj_assistant-0.7.2.dev30/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10727 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/configure.py
+-rw-r--r--   0        0        0     5282 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3910 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    15023 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    13551 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6739 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    19388 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3583 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4065 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5392 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    18345 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4646 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2385 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2500 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4136 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/LICENSE
+-rw-r--r--   0        0        0    23342 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/README.md
+-rw-r--r--   0        0        0     2792 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/pyproject.toml
+-rw-r--r--   0        0        0    25706 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/PKG-INFO
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/configure.py` & `khoj_assistant-0.7.2.dev4/src/khoj/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,22 +63,20 @@
 
     app.mount("/static", StaticFiles(directory=constants.web_directory), name="static")
     app.include_router(api, prefix="/api")
     app.include_router(api_beta, prefix="/api/beta")
     app.include_router(web_client)
 
 
-if not state.demo:
-
-    @schedule.repeat(schedule.every(61).minutes)
-    def update_search_index():
-        state.search_index_lock.acquire()
-        state.model = configure_search(state.model, state.config, regenerate=False)
-        state.search_index_lock.release()
-        logger.info("📬 Search index updated via Scheduler")
+@schedule.repeat(schedule.every(61).minutes)
+def update_search_index():
+    state.search_index_lock.acquire()
+    state.model = configure_search(state.model, state.config, regenerate=False)
+    state.search_index_lock.release()
+    logger.info("📬 Search index updated via Scheduler")
 
 
 def configure_search_types(config: FullConfig):
     # Extract core search types
     core_search_types = {e.name: e.value for e in SearchType}
     # Extract configured plugin search types
     plugin_search_types = {}
@@ -251,19 +249,12 @@
     if not state.config or not state.config.app.should_log_telemetry or not state.telemetry:
         message = "📡 No telemetry to upload" if not state.telemetry else "📡 Telemetry logging disabled"
         logger.debug(message)
         return
 
     try:
         logger.debug(f"📡 Upload usage telemetry to {constants.telemetry_server}:\n{state.telemetry}")
-        for log in state.telemetry:
-            for field in log:
-                # Check if the value for the field is JSON serializable
-                try:
-                    json.dumps(log[field])
-                except TypeError:
-                    log[field] = str(log[field])
         requests.post(constants.telemetry_server, json=state.telemetry)
     except Exception as e:
         logger.error(f"📡 Error uploading telemetry: {e}")
     else:
         state.telemetry = []
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/main.py` & `khoj_assistant-0.7.2.dev4/src/khoj/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,17 @@
     fh = logging.FileHandler(state.config_file.parent / "khoj.log", encoding="utf-8")
     fh.setLevel(logging.DEBUG)
     logger.addHandler(fh)
 
     logger.info("🌘 Starting Khoj")
 
     if not args.gui:
-        # Setup task scheduler
-        poll_task_scheduler()
+        if not state.demo:
+            # Setup task scheduler
+            poll_task_scheduler()
 
         # Start Server
         configure_server(args, required=False)
         configure_routes(app)
         start_server(app, host=args.host, port=args.port, socket=args.socket)
     else:
         # Setup GUI
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/chat.html`

 * *Files 6% similar despite different names*

```diff
@@ -60,77 +60,33 @@
             // Add message by user to chat body
             renderMessage(query, "you");
             document.getElementById("chat-input").value = "";
 
             // Generate backend API URL to execute query
             let url = `/api/chat?q=${encodeURIComponent(query)}&client=web`;
 
-            let chat_body = document.getElementById("chat-body");
-            let new_response = document.createElement("div");
-            new_response.classList.add("chat-message", "khoj");
-            new_response.attributes["data-meta"] = "🏮 Khoj at " + formatDate(new Date());
-            chat_body.appendChild(new_response);
-
-            let new_response_text = document.createElement("div");
-            new_response_text.classList.add("chat-message-text", "khoj");
-            new_response.appendChild(new_response_text);
-
-            // Temporary status message to indicate that Khoj is thinking
-            new_response_text.innerHTML = "🤔";
-            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
-
-            // Call specified Khoj API which returns a streamed response of type text/plain
+            // Call specified Khoj API
             fetch(url)
-                .then(response => {
-                    const reader = response.body.getReader();
-                    const decoder = new TextDecoder();
-
-                    function readStream() {
-                        reader.read().then(({ done, value }) => {
-                            if (done) {
-                                return;
-                            }
-
-                            // Decode message chunk from stream
-                            const chunk = decoder.decode(value, { stream: true });
-                            if (chunk.startsWith("### compiled references:")) {
-                                // Display references used to generate response
-                                const rawReferences = chunk.split("### compiled references:")[1];
-                                const rawReferencesAsJson = JSON.parse(rawReferences);
-                                let polishedReferences = rawReferencesAsJson
-                                    .map((reference, index) => generateReference(reference, index))
-                                    .join("<sup>,</sup>");
-                                new_response_text.innerHTML += polishedReferences;
-                            } else {
-                                // Display response from Khoj
-                                if (new_response_text.innerHTML === "🤔") {
-                                    // Clear temporary status message
-                                    new_response_text.innerHTML = "";
-                                }
-                                new_response_text.innerHTML += chunk;
-                                readStream();
-                            }
-
-                            // Scroll to bottom of chat window as chat response is streamed
-                            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
-                        });
-                    }
-                    readStream();
+                .then(response => response.json())
+                .then(data => {
+                    // Render message by Khoj to chat body
+                    console.log(data.response);
+                    renderMessageWithReference(data.response, "khoj", data.context);
                 });
         }
 
         function incrementalChat(event) {
             // Send chat message on 'Enter'
             if (event.key === 'Enter') {
                 chat();
             }
         }
 
         window.onload = function () {
-            fetch('/api/chat/init?client=web')
+            fetch('/api/chat?client=web')
                 .then(response => response.json())
                 .then(data => {
                     if (data.detail) {
                         // If the server returns a 500 error with detail, render it as a message.
                         renderMessage("Hi 👋🏾, to get started <br/>1. Get your <a class='inline-chat-link' href='https://platform.openai.com/account/api-keys'>OpenAI API key</a><br/>2. Save it in the Khoj <a class='inline-chat-link' href='/config/processor/conversation'>chat settings</a> <br/>3. Click Configure on the Khoj <a class='inline-chat-link' href='/config'>settings page</a>", "khoj");
 
                         // Disable chat input field and update placeholder text
@@ -424,15 +380,15 @@
             color: black;
             text-decoration: none;
         }
     </style>
     <script>
         var khojBannerSubmit = document.getElementById("khoj-banner-submit");
 
-        khojBannerSubmit?.addEventListener("click", function(event) {
+        khojBannerSubmit.addEventListener("click", function(event) {
             event.preventDefault();
             var email = document.getElementById("khoj-banner-email").value;
             fetch("https://lantern.khoj.dev/beta/users/", {
                     method: "POST",
                     body: JSON.stringify({
                         email: email
                     }),
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_input.html`

 * *Files 5% similar despite different names*

```diff
@@ -6,39 +6,39 @@
             <img class="card-icon" src="/static/assets/icons/{{ content_type }}.svg" alt="{{ content_type|capitalize }}">
             <span class="card-title-text">{{ content_type|capitalize }}</span>
         </h2>
         <form id="config-form">
             <table>
                 <tr>
                     <td>
-                        <label for="input-files" title="Add a {{content_type}} file for Khoj to index">Files</label>
+                        <label for="input-files">Input Files</label>
                     </td>
                     <td id="input-files-cell">
                         {% if current_config['input_files'] is none %}
-                            <input type="text" id="input-files" name="input-files" placeholder="~\Documents\notes.{{content_type}}">
+                            <input type="text" id="input-files" name="input-files">
                         {% else %}
                             {% for input_file in current_config['input_files'] %}
-                                <input type="text" id="input-files" name="input-files" value="{{ input_file }}" placeholder="~\Documents\notes.{{content_type}}">
+                                <input type="text" id="input-files" name="input-files" value="{{ input_file }}">
                             {% endfor %}
                         {% endif %}
                     </td>
                     <td>
                         <button type="button" id="input-files-button">Add</button>
                     </td>
                 </tr>
                 <tr>
                     <td>
-                        <label for="input-filter" title="Add a folder with {{content_type}} files for Khoj to index">Folders</label>
+                        <label for="input-filter">Input Filter</label>
                     </td>
                     <td id="input-filter-cell">
                         {% if current_config['input_filter'] is none %}
-                            <input type="text" id="input-filter" name="input-filter" placeholder="~/Documents/{{content_type}}">
+                            <input type="text" id="input-filter" name="input-filter">
                         {% else %}
                             {% for input_filter in current_config['input_filter'] %}
-                                <input type="text" id="input-filter" name="input-filter" placeholder="~/Documents/{{content_type}}" value="{{ input_filter.split('/*')[0] }}">
+                                <input type="text" id="input-filter" name="input-filter" value="{{ input_filter }}">
                             {% endfor %}
                         {% endif %}
                     </td>
                     <td>
                         <button type="button" id="input-filter-button">Add</button>
                     </td>
                 </tr>
@@ -102,27 +102,19 @@
             validNodes.push(nodes[i]);
         }
         return validNodes;
     }
 
     submit.addEventListener("click", function(event) {
         event.preventDefault();
-        let suffix = ""
-        if ('{{content_type}}' == "markdown")
-            suffix = "**/*.md"
-        else if ('{{content_type}}' == "org")
-            suffix = "**/*.org"
-        else if ('{{content_type}}' === "pdf")
-            suffix = "**/*.pdf"
-
         var inputFileNodes = document.getElementsByName("input-files");
         var input_files = getValidInputNodes(inputFileNodes).map(node => node.value);
 
         var inputFilterNodes = document.getElementsByName("input-filter");
-        var input_filter = getValidInputNodes(inputFilterNodes).map(node => `${node.value}/${suffix}`);
+        var input_filter = getValidInputNodes(inputFilterNodes).map(node => node.value);
 
         if (input_files.length === 0 && input_filter.length === 0) {
             alert("You must specify at least one input file or input filter.");
             return;
         }
 
         if (input_files.length == 0) {
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 {% extends "base_config.html" %} {% block content %}
 ***** [{{ content_type|capitalize }}] {{ content_type|capitalize }} *****
-        {% if current_config['input_files'] is none %} [input-files
-Files   ] {% else %} {% for input_file in current_config['input_files'] %}  Add
-        [{{ input_file }}    ] {% endfor %} {% endif %}
-        {% if current_config['input_filter'] is none %} [input-filter
-Folders ] {% else %} {% for input_filter in current_config['input_filter']  Add
-        %} [{{ input_filter.split('/*')[0] }}] {% endfor %} {% endif %}
+             {% if current_config['input_files'] is none %} [input-files
+Input Files  ] {% else %} {% for input_file in current_config              Add
+             ['input_files'] %} [{{ input_file }}    ] {% endfor %} {%
+             endif %}
+             {% if current_config['input_filter'] is none %} [input-filter
+Input Filter ] {% else %} {% for input_filter in current_config            Add
+             ['input_filter'] %} [{{ input_filter }}  ] {% endfor %} {%
+             endif %}
 Compressed JSONL (Output) [{{ current_config['compressed_jsonl'] }}]
 Embeddings File (Output)  [{{ current_config['embeddings_file'] }}]
 Index Heading Entries     [{{ current_config['index_heading_entries'] }}]
 Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,25 @@
                 .then(response => response.json())
                 .then(data => {
                     console.log(data);
                     document.getElementById("results").innerHTML = render_results(data, query, type);
                 });
         }
 
+        function updateIndex() {
+            type = document.getElementById("type").value;
+            fetch(`/api/update?t=${type}&client=web`)
+                .then(response => response.json())
+                .then(data => {
+                    console.log(data);
+                    document.getElementById("results").innerHTML =
+                        render_results(data);
+                });
+        }
+
         function incrementalSearch(event) {
             type = document.getElementById("type").value;
             // Search with reranking on 'Enter'
             if (event.key === 'Enter') {
                 search(rerank=true);
             }
             // Limit incremental search to text types
@@ -253,14 +264,17 @@
         <!--Add Text Box To Enter Query, Trigger Incremental Search OnChange -->
         <input type="text" id="query" class="option" onkeyup=incrementalSearch(event) autofocus="autofocus" placeholder="What is the meaning of life?">
 
         <div id="options">
             <!--Add Dropdown to Select Query Type -->
             <select id="type" class="option" onchange="setTypeFieldInUrl(this)"></select>
 
+            <!--Add Button To Regenerate -->
+            <button id="update" class="option" onclick="updateIndex()">Update</button>
+
             <!--Add Results Count Input To Set Results Count -->
             <input type="number" id="results-count" min="1" max="100" value="6" placeholder="results count" onchange="setCountFieldInUrl(this)">
         </div>
 
         <!-- Section to Render Results -->
         <div id="results"></div>
     </body>
@@ -300,15 +314,15 @@
         body > * {
             padding: 10px;
             margin: 10px;
         }
         #options {
             padding: 0;
             display: grid;
-            grid-template-columns: 1fr minmax(70px, 0.5fr);
+            grid-template-columns: 1fr 1fr minmax(70px, 0.5fr);
         }
         #options > * {
             padding: 15px;
             border-radius: 5px;
             border: 1px solid #475569;
             background: #f9fafc
         }
```

#### html2text {}

```diff
@@ -3,8 +3,8 @@
 
 {% if demo %}
 Enroll_in_Khoj_cloud_to_get_your_own_Github_assistant
  [                    ] Submit
 [Khoj] {% else %} [Khoj] {% endif %}  Chat Search {% if not demo %} Settings {%
 endif %}
  [                    ]
-  [Unknown INPUT type]
+  Update  [Unknown INPUT type]
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/processor_conversation_input.html`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             <img class="card-icon" src="/static/assets/icons/chat.svg" alt="Chat">
             <span class="card-title-text">Chat</span>
         </h2>
         <form id="config-form">
             <table>
                 <tr>
                     <td>
-                        <label for="openai-api-key" title="Get your OpenAI key from https://platform.openai.com/account/api-keys">OpenAI API key</label>
+                        <label for="openai-api-key">OpenAI API key</label>
                     </td>
                     <td>
                         <input type="text" id="openai-api-key" name="openai-api-key" value="{{ current_config['openai_api_key'] }}">
                     </td>
                 </tr>
             </table>
             <table >
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Standard Packages
 import json
 import logging
 from datetime import datetime
-from typing import Optional
 
 # Internal Packages
 from khoj.utils.constants import empty_escape_sequences
 from khoj.processor.conversation import prompts
 from khoj.processor.conversation.utils import (
     chat_completion_with_backoff,
     completion_with_backoff,
@@ -44,16 +43,14 @@
     Summarize user input using OpenAI's GPT
     """
     # Setup Prompt based on Summary Type
     if summary_type == "chat":
         prompt = prompts.summarize_chat.format(text=text)
     elif summary_type == "notes":
         prompt = prompts.summarize_notes.format(text=text, user_query=user_query)
-    else:
-        raise ValueError(f"Invalid summary type: {summary_type}")
 
     # Get Response from GPT
     logger.debug(f"Prompt for GPT: {prompt}")
     response = completion_with_backoff(
         prompt=prompt,
         model_name=model,
         temperature=temperature,
@@ -63,17 +60,15 @@
         api_key=api_key,
     )
 
     # Extract, Clean Message from GPT's Response
     return str(response).replace("\n\n", "")
 
 
-def extract_questions(
-    text, model: Optional[str] = "text-davinci-003", conversation_log={}, api_key=None, temperature=0, max_tokens=100
-):
+def extract_questions(text, model="text-davinci-003", conversation_log={}, api_key=None, temperature=0, max_tokens=100):
     """
     Infer search queries to retrieve relevant notes to answer user query
     """
     # Extract Past User Message and Inferred Questions from Conversation Log
     chat_history = "".join(
         [
             f'Q: {chat["intent"]["query"]}\n\n{chat["intent"].get("inferred-queries") or list([chat["intent"]["query"]])}\n\n{chat["message"]}\n\n'
@@ -145,23 +140,15 @@
         api_key=api_key,
     )
 
     # Extract, Clean Message from GPT's Response
     return json.loads(response.strip(empty_escape_sequences))
 
 
-def converse(
-    references,
-    user_query,
-    conversation_log={},
-    model: Optional[str] = "gpt-3.5-turbo",
-    api_key=None,
-    temperature=0.2,
-    completion_func=None,
-):
+def converse(references, user_query, conversation_log={}, model="gpt-3.5-turbo", api_key=None, temperature=0.2):
     """
     Converse with user using OpenAI's ChatGPT
     """
     # Initialize Variables
     current_date = datetime.now().strftime("%Y-%m-%d")
     compiled_references = "\n\n".join({f"# {item}" for item in references})
 
@@ -176,19 +163,19 @@
     # Setup Prompt with Primer or Conversation History
     messages = generate_chatml_messages_with_context(
         conversation_primer,
         prompts.personality.format(),
         conversation_log,
         model,
     )
-    truncated_messages = "\n".join({f"{message.content[:40]}..." for message in messages})
-    logger.debug(f"Conversation Context for GPT: {truncated_messages}")
 
     # Get Response from GPT
-    return chat_completion_with_backoff(
+    logger.debug(f"Conversation Context for GPT: {messages}")
+    response = chat_completion_with_backoff(
         messages=messages,
-        compiled_references=references,
         model_name=model,
         temperature=temperature,
         openai_api_key=api_key,
-        completion_func=completion_func,
     )
+
+    # Extract, Clean Message from GPT's Response
+    return response.strip(empty_escape_sequences)
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.2.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/routers/api.py` & `khoj_assistant-0.7.2.dev4/src/khoj/routers/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import concurrent.futures
 import math
 import time
 import yaml
 import logging
 from datetime import datetime
 from typing import List, Optional, Union
-from functools import partial
 
 # External Packages
 from fastapi import APIRouter, HTTPException, Header, Request
 from sentence_transformers import util
 
 # Internal Packages
 from khoj.configure import configure_processor, configure_search
@@ -31,21 +30,19 @@
     TextContentConfig,
     ConversationProcessorConfig,
     GithubContentConfig,
 )
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
 from khoj.utils.yaml import save_config_to_file_updated_state
-from fastapi.responses import StreamingResponse
 
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
 
-# If it's a demo instance, prevent updating any of the configuration.
 if not state.demo:
 
     @api.get("/config/data", response_model=FullConfig)
     def get_config_data():
         return state.config
 
     @api.post("/config/data")
@@ -321,15 +318,15 @@
             # Sort results across all content types and take top results
             results = sorted(results, key=lambda x: float(x.score), reverse=True)[:results_count]
 
     # Cache results
     state.query_cache[query_cache_key] = results
 
     user_state = {
-        "client_host": request.client.host if request.client else "unknown",
+        "client_host": request.client.host,
         "user_agent": user_agent or "unknown",
         "referer": referer or "unknown",
         "host": host or "unknown",
     }
 
     # Only log telemetry if query is new and not a continuation of previous query
     if state.previous_query is None or state.previous_query not in user_query:
@@ -377,109 +374,54 @@
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
     else:
         logger.info("📬 Processor reconfigured via API")
 
     user_state = {
-        "client_host": request.client.host if request.client else None,
+        "client_host": request.client.host,
         "user_agent": user_agent or "unknown",
         "referer": referer or "unknown",
         "host": host or "unknown",
     }
 
     state.telemetry += [
         log_telemetry(
             telemetry_type="api", api="update", client=client, app_config=state.config.app, properties=user_state
         )
     ]
 
     return {"status": "ok", "message": "khoj reloaded"}
 
 
-@api.get("/chat/init")
-def chat_init(
-    request: Request,
-    client: Optional[str] = None,
-    user_agent: Optional[str] = Header(None),
-    referer: Optional[str] = Header(None),
-    host: Optional[str] = Header(None),
-):
-    if (
-        state.processor_config is None
-        or state.processor_config.conversation is None
-        or state.processor_config.conversation.openai_api_key is None
-    ):
-        raise HTTPException(
-            status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
-        )
-
-    # Load Conversation History
-    meta_log = state.processor_config.conversation.meta_log
-
-    user_state = {
-        "client_host": request.client.host if request.client else None,
-        "user_agent": user_agent or "unknown",
-        "referer": referer or "unknown",
-        "host": host or "unknown",
-    }
-
-    state.telemetry += [
-        log_telemetry(
-            telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
-        )
-    ]
-
-    return {"status": "ok", "response": meta_log.get("chat", [])}
-
-
-@api.get("/chat", response_class=StreamingResponse)
+@api.get("/chat")
 async def chat(
     request: Request,
     q: Optional[str] = None,
-    n: Optional[int] = 5,
     client: Optional[str] = None,
     user_agent: Optional[str] = Header(None),
     referer: Optional[str] = Header(None),
     host: Optional[str] = Header(None),
-) -> StreamingResponse:
-    def _save_to_conversation_log(
-        q: str,
-        gpt_response: str,
-        user_message_time: str,
-        compiled_references: List[str],
-        inferred_queries: List[str],
-        chat_session: str,
-        meta_log,
-    ):
-        state.processor_config.conversation.chat_session = message_to_prompt(q, chat_session, gpt_message=gpt_response)
-        state.processor_config.conversation.meta_log["chat"] = message_to_log(
-            q,
-            gpt_response,
-            user_message_metadata={"created": user_message_time},
-            khoj_message_metadata={"context": compiled_references, "intent": {"inferred-queries": inferred_queries}},
-            conversation_log=meta_log.get("chat", []),
-        )
-
+):
     if (
         state.processor_config is None
         or state.processor_config.conversation is None
         or state.processor_config.conversation.openai_api_key is None
     ):
         raise HTTPException(
             status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
         )
 
     # Load Conversation History
     chat_session = state.processor_config.conversation.chat_session
     meta_log = state.processor_config.conversation.meta_log
 
-    # If user query is empty, return nothing
+    # If user query is empty, return chat history
     if not q:
-        return StreamingResponse(None)
+        return {"status": "ok", "response": meta_log.get("chat", [])}
 
     # Initialize Variables
     api_key = state.processor_config.conversation.openai_api_key
     model = state.processor_config.conversation.model
     chat_model = state.processor_config.conversation.chat_model
     user_message_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     conversation_type = "general" if q.startswith("@general") else "notes"
@@ -492,48 +434,47 @@
             inferred_queries = extract_questions(q, model=model, api_key=api_key, conversation_log=meta_log)
 
         # Collate search results as context for GPT
         with timer("Searching knowledge base took", logger):
             result_list = []
             for query in inferred_queries:
                 result_list.extend(
-                    await search(query, request=request, n=n, r=False, score_threshold=-5.0, dedupe=False)
+                    await search(query, request=request, n=5, r=True, score_threshold=-5.0, dedupe=False)
                 )
             compiled_references = [item.additional["compiled"] for item in result_list]
 
     # Switch to general conversation type if no relevant notes found for the given query
     conversation_type = "notes" if compiled_references else "general"
     logger.debug(f"Conversation Type: {conversation_type}")
 
+    try:
+        with timer("Generating chat response took", logger):
+            gpt_response = converse(compiled_references, q, meta_log, model=chat_model, api_key=api_key)
+        status = "ok"
+    except Exception as e:
+        gpt_response = str(e)
+        status = "error"
+
+    # Update Conversation History
+    state.processor_config.conversation.chat_session = message_to_prompt(q, chat_session, gpt_message=gpt_response)
+    state.processor_config.conversation.meta_log["chat"] = message_to_log(
+        q,
+        gpt_response,
+        user_message_metadata={"created": user_message_time},
+        khoj_message_metadata={"context": compiled_references, "intent": {"inferred-queries": inferred_queries}},
+        conversation_log=meta_log.get("chat", []),
+    )
+
     user_state = {
-        "client_host": request.client.host if request.client else None,
+        "client_host": request.client.host,
         "user_agent": user_agent or "unknown",
         "referer": referer or "unknown",
         "host": host or "unknown",
     }
 
     state.telemetry += [
         log_telemetry(
             telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
         )
     ]
 
-    try:
-        with timer("Generating chat response took", logger):
-            partial_completion = partial(
-                _save_to_conversation_log,
-                q,
-                user_message_time=user_message_time,
-                compiled_references=compiled_references,
-                inferred_queries=inferred_queries,
-                chat_session=chat_session,
-                meta_log=meta_log,
-            )
-
-            gpt_response = converse(
-                compiled_references, q, meta_log, model=chat_model, api_key=api_key, completion_func=partial_completion
-            )
-
-    except Exception as e:
-        gpt_response = str(e)
-
-    return StreamingResponse(gpt_response, media_type="text/event-stream", status_code=200)
+    return {"status": status, "response": gpt_response, "context": compiled_references}
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.2.dev4/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.2.dev4/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.2.dev4/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.2.dev4/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/cli.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/config.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/constants.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,19 +171,15 @@
         with open(app_env_filename, "w") as f:
             f.write("server_id=" + server_id + "\n")
 
     return server_id
 
 
 def log_telemetry(
-    telemetry_type: str,
-    api: str = None,
-    client: Optional[str] = None,
-    app_config: Optional[AppConfig] = None,
-    properties: dict = None,
+    telemetry_type: str, api: str = None, client: str = None, app_config: AppConfig = None, properties: dict = None
 ):
     """Log basic app usage telemetry like client, os, api called"""
     # Do not log usage telemetry, if telemetry is disabled via app config
     if not app_config or not app_config.should_log_telemetry:
         return []
 
     # Populate telemetry data to log
```

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/models.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/state.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.2.dev4/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/.gitignore` & `khoj_assistant-0.7.2.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/LICENSE` & `khoj_assistant-0.7.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/README.md` & `khoj_assistant-0.7.2.dev4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
   - [Khoj Obsidian](#upgrade-khoj-on-obsidian)
 - [Uninstall](#uninstall)
 - [Troubleshoot](#Troubleshoot)
 - [Advanced Usage](#advanced-usage)
   - [Access Khoj on Mobile](#access-khoj-on-mobile)
   - [Use OpenAI Models for Search](#use-openai-models-for-search)
   - [Search across Different Languages](#search-across-different-languages)
-  - [Boostrap Khoj Search for Offline Usage Later](#bootstrap-khoj-search-for-offline-usage-later)
 - [Miscellaneous](#Miscellaneous)
   - [Setup OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   - [GPT API](#gpt-api)
 - [Performance](#Performance)
   - [Query Performance](#Query-performance)
   - [Indexing Performance](#Indexing-performance)
   - [Miscellaneous](#Miscellaneous-1)
@@ -305,27 +304,14 @@
 + encoder: "paraphrase-multilingual-MiniLM-L12-v2"
      cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
      model_directory: "~/.khoj/search/asymmetric/"
   ```
 
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
-### Bootstrap Khoj Search for Offline Usage later
-
-  You can bootstrap Khoj pre-emptively to run on machines that do not have internet access. An example use-case would be to run Khoj on an air-gapped machine.
-  Note: *Only search can currently run in fully offline mode, not chat.*
-
-  - With Internet
-    1. Manually download the [asymmetric text](https://huggingface.co/sentence-transformers/multi-qa-MiniLM-L6-cos-v1), [symmetric text](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2)and [image search](https://huggingface.co/sentence-transformers/clip-ViT-B-32) models from HuggingFace
-    2. Pip install khoj (and dependencies) in an associated virtualenv. E.g `python -m venv .venv && source .venv/bin/activate && pip install khoj-assistant`
-  - Without Internet
-    1. Copy each of the search models into their respective folders, `asymmetric`, `symmetric` and `image` under the `~/.khoj/search/` directory on the air-gapped machine
-    2. Copy the khoj virtual environment directory onto the air-gapped machine, activate the environment and start and khoj as normal. E.g `source .venv/bin/activate && khoj`
-
-
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
  - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
```

### Comparing `khoj_assistant-0.7.2.dev30/pyproject.toml` & `khoj_assistant-0.7.2.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev30/PKG-INFO` & `khoj_assistant-0.7.2.dev4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.2.dev30
+Version: 0.7.2.dev4
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -91,15 +91,14 @@
   - [Khoj Obsidian](#upgrade-khoj-on-obsidian)
 - [Uninstall](#uninstall)
 - [Troubleshoot](#Troubleshoot)
 - [Advanced Usage](#advanced-usage)
   - [Access Khoj on Mobile](#access-khoj-on-mobile)
   - [Use OpenAI Models for Search](#use-openai-models-for-search)
   - [Search across Different Languages](#search-across-different-languages)
-  - [Boostrap Khoj Search for Offline Usage Later](#bootstrap-khoj-search-for-offline-usage-later)
 - [Miscellaneous](#Miscellaneous)
   - [Setup OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   - [GPT API](#gpt-api)
 - [Performance](#Performance)
   - [Query Performance](#Query-performance)
   - [Indexing Performance](#Indexing-performance)
   - [Miscellaneous](#Miscellaneous-1)
@@ -363,27 +362,14 @@
 + encoder: "paraphrase-multilingual-MiniLM-L12-v2"
      cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
      model_directory: "~/.khoj/search/asymmetric/"
   ```
 
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
-### Bootstrap Khoj Search for Offline Usage later
-
-  You can bootstrap Khoj pre-emptively to run on machines that do not have internet access. An example use-case would be to run Khoj on an air-gapped machine.
-  Note: *Only search can currently run in fully offline mode, not chat.*
-
-  - With Internet
-    1. Manually download the [asymmetric text](https://huggingface.co/sentence-transformers/multi-qa-MiniLM-L6-cos-v1), [symmetric text](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2)and [image search](https://huggingface.co/sentence-transformers/clip-ViT-B-32) models from HuggingFace
-    2. Pip install khoj (and dependencies) in an associated virtualenv. E.g `python -m venv .venv && source .venv/bin/activate && pip install khoj-assistant`
-  - Without Internet
-    1. Copy each of the search models into their respective folders, `asymmetric`, `symmetric` and `image` under the `~/.khoj/search/` directory on the air-gapped machine
-    2. Copy the khoj virtual environment directory onto the air-gapped machine, activate the environment and start and khoj as normal. E.g `source .venv/bin/activate && khoj`
-
-
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
  - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
```

