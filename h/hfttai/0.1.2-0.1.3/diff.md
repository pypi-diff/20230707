# Comparing `tmp/hfttai-0.1.2.tar.gz` & `tmp/hfttai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfttai-0.1.2.tar", max compression
+gzip compressed data, was "hfttai-0.1.3.tar", max compression
```

## Comparing `hfttai-0.1.2.tar` & `hfttai-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,62 @@
--rw-r--r--   0        0        0     1055 2023-07-07 08:51:50.000000 hfttai-0.1.2/LICENSE
--rw-r--r--   0        0        0    25266 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/__init__.py
--rw-r--r--   0        0        0     1235 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0      159 2023-05-26 02:00:53.639839 hfttai-0.1.2/pandasai/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7444 2023-05-26 02:00:53.642831 hfttai-0.1.2/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc
--rw-r--r--   0        0        0     1019 2023-05-26 02:00:56.795406 hfttai-0.1.2/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc
--rw-r--r--   0        0        0     2337 2023-05-26 02:00:53.645824 hfttai-0.1.2/pandasai/helpers/__pycache__/notebook.cpython-311.pyc
--rw-r--r--   0        0        0     3814 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3471 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0      155 2023-05-26 02:00:55.181718 hfttai-0.1.2/pandasai/llm/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5613 2023-05-26 02:00:56.832306 hfttai-0.1.2/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc
--rw-r--r--   0        0        0    13653 2023-05-26 07:42:15.392075 hfttai-0.1.2/pandasai/llm/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1450 2023-05-26 02:00:56.817346 hfttai-0.1.2/pandasai/llm/__pycache__/fake.cpython-311.pyc
--rw-r--r--   0        0        0     2506 2023-05-26 02:00:56.878184 hfttai-0.1.2/pandasai/llm/__pycache__/google_palm.cpython-311.pyc
--rw-r--r--   0        0        0     3499 2023-05-26 02:00:56.890152 hfttai-0.1.2/pandasai/llm/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0     1615 2023-05-26 02:00:56.899128 hfttai-0.1.2/pandasai/llm/__pycache__/starcoder.cpython-311.pyc
--rw-r--r--   0        0        0     4335 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11156 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3176 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0     1062 2023-05-26 02:00:56.781443 hfttai-0.1.2/pandasai/prompts/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1876 2023-05-26 02:00:56.779448 hfttai-0.1.2/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc
--rw-r--r--   0        0        0     1809 2023-05-28 12:33:38.926133 hfttai-0.1.2/pandasai/prompts/__pycache__/generate_python_code.cpython-311.pyc
--rw-r--r--   0        0        0      824 2023-05-26 02:00:56.786429 hfttai-0.1.2/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc
--rw-r--r--   0        0        0      647 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1270 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1076 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1081 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1072 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1898 2023-07-07 11:28:40.525215 hfttai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7705 2023-07-07 08:51:50.000000 hfttai-0.1.2/README.md
--rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 hfttai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-07 08:51:50.000000 hfttai-0.1.3/LICENSE
+-rw-r--r--   0        0        0    25266 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-07 11:43:18.700269 hfttai-0.1.3/pandasai/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4372 2023-07-07 11:43:18.702263 hfttai-0.1.3/pandasai/helpers/__pycache__/_optional.cpython-311.pyc
+-rw-r--r--   0        0        0     7796 2023-07-07 11:43:18.705256 hfttai-0.1.3/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc
+-rw-r--r--   0        0        0     3375 2023-07-07 11:43:18.708266 hfttai-0.1.3/pandasai/helpers/__pycache__/cache.cpython-311.pyc
+-rw-r--r--   0        0        0     1019 2023-05-26 02:00:56.795406 hfttai-0.1.3/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc
+-rw-r--r--   0        0        0     2334 2023-07-07 11:43:18.713235 hfttai-0.1.3/pandasai/helpers/__pycache__/notebook.cpython-311.pyc
+-rw-r--r--   0        0        0     5526 2023-07-07 11:43:20.132058 hfttai-0.1.3/pandasai/helpers/__pycache__/save_chart.cpython-311.pyc
+-rw-r--r--   0        0        0    13373 2023-07-07 11:43:20.135050 hfttai-0.1.3/pandasai/helpers/__pycache__/shortcuts.cpython-311.pyc
+-rw-r--r--   0        0        0     3814 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3471 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-07 11:43:20.138042 hfttai-0.1.3/pandasai/llm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5613 2023-05-26 02:00:56.832306 hfttai-0.1.3/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc
+-rw-r--r--   0        0        0    16066 2023-07-07 11:43:20.142031 hfttai-0.1.3/pandasai/llm/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1450 2023-05-26 02:00:56.817346 hfttai-0.1.3/pandasai/llm/__pycache__/fake.cpython-311.pyc
+-rw-r--r--   0        0        0     2506 2023-05-26 02:00:56.878184 hfttai-0.1.3/pandasai/llm/__pycache__/google_palm.cpython-311.pyc
+-rw-r--r--   0        0        0     1481 2023-07-07 11:43:20.757703 hfttai-0.1.3/pandasai/llm/__pycache__/langchain.cpython-311.pyc
+-rw-r--r--   0        0        0     4711 2023-07-07 11:47:40.378877 hfttai-0.1.3/pandasai/llm/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0     1615 2023-05-26 02:00:56.899128 hfttai-0.1.3/pandasai/llm/__pycache__/starcoder.cpython-311.pyc
+-rw-r--r--   0        0        0     4335 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11156 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3176 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-07 11:43:20.760693 hfttai-0.1.3/pandasai/middlewares/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1529 2023-07-07 11:43:20.762689 hfttai-0.1.3/pandasai/middlewares/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1710 2023-07-07 11:43:20.764521 hfttai-0.1.3/pandasai/middlewares/__pycache__/charts.cpython-311.pyc
+-rw-r--r--   0        0        0      663 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-07 11:43:20.751742 hfttai-0.1.3/pandasai/prompts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1274 2023-07-07 11:43:20.754709 hfttai-0.1.3/pandasai/prompts/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     2060 2023-07-07 11:43:20.768114 hfttai-0.1.3/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc
+-rw-r--r--   0        0        0     2107 2023-07-07 11:43:20.770111 hfttai-0.1.3/pandasai/prompts/__pycache__/correct_multiples_prompt.cpython-311.pyc
+-rw-r--r--   0        0        0     1876 2023-07-07 11:43:20.773104 hfttai-0.1.3/pandasai/prompts/__pycache__/generate_python_code.cpython-311.pyc
+-rw-r--r--   0        0        0      938 2023-07-07 11:43:20.775099 hfttai-0.1.3/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc
+-rw-r--r--   0        0        0     2184 2023-07-07 11:43:20.778091 hfttai-0.1.3/pandasai/prompts/__pycache__/multiple_dataframes.cpython-311.pyc
+-rw-r--r--   0        0        0      647 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1270 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1076 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1081 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1072 2023-07-07 08:51:50.000000 hfttai-0.1.3/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1898 2023-07-07 11:51:58.691807 hfttai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7705 2023-07-07 08:51:50.000000 hfttai-0.1.3/README.md
+-rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 hfttai-0.1.3/PKG-INFO
```

### Comparing `hfttai-0.1.2/LICENSE` & `hfttai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/__init__.py` & `hfttai-0.1.3/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/constants.py` & `hfttai-0.1.3/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/exceptions.py` & `hfttai-0.1.3/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc` & `hfttai-0.1.3/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xaaaa6e64 (Thu May 25 00:24:10 2023 UTC)
-files sz: 5085
+moddate:  0x26d2a764 (Fri Jul  7 08:51:50 2023 UTC)
+files sz: 5434
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c015a01640164026c025a02640164026c035a
@@ -13,231 +13,231 @@
       066602640a84045a0b640b6506640465066604640c84045a0c6404650666
       02640d84045a0d640e65056a0e0000000000000000640465056a0e000000
       00000000006604640f84045a0f09006413640e65056a0e00000000000000
       0064116507640465056a0e00000000000000006606641284055a10640253
       00
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nThis module contains helper functions for anonymizing data and generating random data\nbefore sending it to the LLM.\n')
+     1           2 LOAD_CONST               0 ('\nThis module contains helper functions for anonymizing data and generating random data\n before sending it to the LLM (An External API).\n\nOnly df.head() is sent to LLM API, hence the df.head() is processed\n to remove any personal or sensitive information.\n\n')
                  4 STORE_NAME               0 (__doc__)
    
-     6           6 LOAD_CONST               1 (0)
+    10           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (random)
                 12 STORE_NAME               1 (random)
    
-     7          14 LOAD_CONST               1 (0)
+    11          14 LOAD_CONST               1 (0)
                 16 LOAD_CONST               2 (None)
                 18 IMPORT_NAME              2 (re)
                 20 STORE_NAME               2 (re)
    
-     8          22 LOAD_CONST               1 (0)
+    12          22 LOAD_CONST               1 (0)
                 24 LOAD_CONST               2 (None)
                 26 IMPORT_NAME              3 (string)
                 28 STORE_NAME               3 (string)
    
-    10          30 LOAD_CONST               1 (0)
+    14          30 LOAD_CONST               1 (0)
                 32 LOAD_CONST               2 (None)
                 34 IMPORT_NAME              4 (pandas)
                 36 STORE_NAME               5 (pd)
    
-    13          38 LOAD_CONST               3 ('email')
+    17          38 LOAD_CONST               3 ('email')
                 40 LOAD_NAME                6 (str)
                 42 LOAD_CONST               4 ('return')
                 44 LOAD_NAME                7 (bool)
                 46 BUILD_TUPLE              4
-                48 LOAD_CONST               5 (<code object is_valid_email, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 13>)
+                48 LOAD_CONST               5 (<code object is_valid_email, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 17>)
                 50 MAKE_FUNCTION            4 (annotations)
                 52 STORE_NAME               8 (is_valid_email)
    
-    24          54 LOAD_CONST               6 ('phone_number')
+    30          54 LOAD_CONST               6 ('phone_number')
                 56 LOAD_NAME                6 (str)
                 58 LOAD_CONST               4 ('return')
                 60 LOAD_NAME                7 (bool)
                 62 BUILD_TUPLE              4
-                64 LOAD_CONST               7 (<code object is_valid_phone_number, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 24>)
+                64 LOAD_CONST               7 (<code object is_valid_phone_number, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 30>)
                 66 MAKE_FUNCTION            4 (annotations)
                 68 STORE_NAME               9 (is_valid_phone_number)
    
-    35          70 LOAD_CONST               8 ('credit_card_number')
+    43          70 LOAD_CONST               8 ('credit_card_number')
                 72 LOAD_NAME                6 (str)
                 74 LOAD_CONST               4 ('return')
                 76 LOAD_NAME                7 (bool)
                 78 BUILD_TUPLE              4
-                80 LOAD_CONST               9 (<code object is_valid_credit_card, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 35>)
+                80 LOAD_CONST               9 (<code object is_valid_credit_card, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 43>)
                 82 MAKE_FUNCTION            4 (annotations)
                 84 STORE_NAME              10 (is_valid_credit_card)
    
-    46          86 LOAD_CONST               4 ('return')
+    56          86 LOAD_CONST               4 ('return')
                 88 LOAD_NAME                6 (str)
                 90 BUILD_TUPLE              2
-                92 LOAD_CONST              10 (<code object generate_random_email, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 46>)
+                92 LOAD_CONST              10 (<code object generate_random_email, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 56>)
                 94 MAKE_FUNCTION            4 (annotations)
                 96 STORE_NAME              11 (generate_random_email)
    
-    70          98 LOAD_CONST              11 ('original_field')
+    80          98 LOAD_CONST              11 ('original_field')
                100 LOAD_NAME                6 (str)
                102 LOAD_CONST               4 ('return')
                104 LOAD_NAME                6 (str)
                106 BUILD_TUPLE              4
-               108 LOAD_CONST              12 (<code object generate_random_phone_number, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 70>)
+               108 LOAD_CONST              12 (<code object generate_random_phone_number, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 80>)
                110 MAKE_FUNCTION            4 (annotations)
                112 STORE_NAME              12 (generate_random_phone_number)
    
-    93         114 LOAD_CONST               4 ('return')
+   105         114 LOAD_CONST               4 ('return')
                116 LOAD_NAME                6 (str)
                118 BUILD_TUPLE              2
-               120 LOAD_CONST              13 (<code object generate_random_credit_card, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 93>)
+               120 LOAD_CONST              13 (<code object generate_random_credit_card, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 105>)
                122 MAKE_FUNCTION            4 (annotations)
                124 STORE_NAME              13 (generate_random_credit_card)
    
-   107         126 LOAD_CONST              14 ('data_frame')
+   119         126 LOAD_CONST              14 ('data_frame')
                128 LOAD_NAME                5 (pd)
                130 LOAD_ATTR               14 (DataFrame)
                140 LOAD_CONST               4 ('return')
                142 LOAD_NAME                5 (pd)
                144 LOAD_ATTR               14 (DataFrame)
                154 BUILD_TUPLE              4
-               156 LOAD_CONST              15 (<code object copy_head, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 107>)
+               156 LOAD_CONST              15 (<code object copy_head, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 119>)
                158 MAKE_FUNCTION            4 (annotations)
                160 STORE_NAME              15 (copy_head)
    
-   118         162 NOP
+   132         162 NOP
    
-   117         164 LOAD_CONST              19 ((True,))
+   131         164 LOAD_CONST              19 ((True,))
                166 LOAD_CONST              14 ('data_frame')
    
-   118         168 LOAD_NAME                5 (pd)
+   132         168 LOAD_NAME                5 (pd)
                170 LOAD_ATTR               14 (DataFrame)
    
-   117         180 LOAD_CONST              17 ('force_conversion')
+   131         180 LOAD_CONST              17 ('force_conversion')
    
-   118         182 LOAD_NAME                7 (bool)
+   132         182 LOAD_NAME                7 (bool)
    
-   117         184 LOAD_CONST               4 ('return')
+   131         184 LOAD_CONST               4 ('return')
    
-   119         186 LOAD_NAME                5 (pd)
+   133         186 LOAD_NAME                5 (pd)
                188 LOAD_ATTR               14 (DataFrame)
    
-   117         198 BUILD_TUPLE              6
-               200 LOAD_CONST              18 (<code object anonymize_dataframe_head, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 117>)
+   131         198 BUILD_TUPLE              6
+               200 LOAD_CONST              18 (<code object anonymize_dataframe_head, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 131>)
                202 MAKE_FUNCTION            5 (defaults, annotations)
                204 STORE_NAME              16 (anonymize_dataframe_head)
                206 LOAD_CONST               2 (None)
                208 RETURN_VALUE
    consts
-      '\nThis module contains helper functions for anonymizing data and generating random data\nbefore sending it to the LLM.\n'
+      '\nThis module contains helper functions for anonymizing data and generating random data\n before sending it to the LLM (An External API).\n\nOnly df.head() is sent to LLM API, hence the df.head() is processed\n to remove any personal or sensitive information.\n\n'
       0
       None
       'email'
       'return'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             017c00a6020000ab020000000000000000640275015300
-          13           0 RESUME                   0
+          17           0 RESUME                   0
          
-          20           2 LOAD_CONST               1 ('^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$')
+          26           2 LOAD_CONST               1 ('^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$')
                        4 STORE_FAST               1 (email_regex)
          
-          21           6 LOAD_GLOBAL              1 (NULL + re)
+          27           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (match)
                       28 LOAD_FAST                1 (email_regex)
                       30 LOAD_FAST                0 (email)
                       32 PRECALL                  2
                       36 CALL                     2
                       46 LOAD_CONST               2 (None)
                       48 IS_OP                    1
                       50 RETURN_VALUE
          consts
-            '\n    Check if the given email is valid based on regex pattern.\n\n    :param email: str, email address to be checked\n    :return: bool, True if the email is valid, otherwise False\n    '
+            'Check if the given email is valid based on regex pattern.\n\n    Args:\n        email (str): email address to be checked.\n\n    Returns (bool): True if the email is valid, otherwise False.\n    '
             '^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$'
             None
          names      ('re', 'match')
          varnames   ('email', 'email_regex')
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'is_valid_email'
-         firstlineno 13
-         lnotab 0x02070401
+         firstlineno 17
+         lnotab 0x02090401
       'phone_number'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             017c00a6020000ab020000000000000000640275015300
-          24           0 RESUME                   0
+          30           0 RESUME                   0
          
-          31           2 LOAD_CONST               1 ('\\b(?:\\+?\\d{1,3}[- ]?)?\\(?\\d{3}\\)?[- ]?\\d{3}[- ]?\\d{4}\\b')
+          39           2 LOAD_CONST               1 ('\\b(?:\\+?\\d{1,3}[- ]?)?\\(?\\d{3}\\)?[- ]?\\d{3}[- ]?\\d{4}\\b')
                        4 STORE_FAST               1 (pattern)
          
-          32           6 LOAD_GLOBAL              1 (NULL + re)
+          40           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (search)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_FAST                0 (phone_number)
                       32 PRECALL                  2
                       36 CALL                     2
                       46 LOAD_CONST               2 (None)
                       48 IS_OP                    1
                       50 RETURN_VALUE
          consts
-            '\n    Check if the given phone number is valid based on regex pattern.\n\n    :param phone_number: str, phone number to be checked\n    :return: bool, True if the phone number is valid, otherwise False\n    '
+            'Check if the given phone number is valid based on regex pattern.\n\n    Args:\n        phone_number (str): phone number to be checked.\n\n    Returns (bool): True if the phone number is valid, otherwise False.\n    '
             '\\b(?:\\+?\\d{1,3}[- ]?)?\\(?\\d{3}\\)?[- ]?\\d{3}[- ]?\\d{4}\\b'
             None
          names      ('re', 'search')
          varnames   ('phone_number', 'pattern')
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'is_valid_phone_number'
-         firstlineno 24
-         lnotab 0x02070401
+         firstlineno 30
+         lnotab 0x02090401
       'credit_card_number'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             017c00a6020000ab020000000000000000640275015300
-          35           0 RESUME                   0
+          43           0 RESUME                   0
          
-          42           2 LOAD_CONST               1 ('^\\d{4}[- ]?\\d{4}[- ]?\\d{4}[- ]?\\d{4}$')
+          52           2 LOAD_CONST               1 ('^\\d{4}[- ]?\\d{4}[- ]?\\d{4}[- ]?\\d{4}$')
                        4 STORE_FAST               1 (pattern)
          
-          43           6 LOAD_GLOBAL              1 (NULL + re)
+          53           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (search)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_FAST                0 (credit_card_number)
                       32 PRECALL                  2
                       36 CALL                     2
                       46 LOAD_CONST               2 (None)
                       48 IS_OP                    1
                       50 RETURN_VALUE
          consts
-            '\n    Check if the given credit card number is valid based on regex pattern.\n\n    :param credit_card_number: str, credit card number to be checked\n    :return: bool, True if the credit card number is valid, otherwise False\n    '
+            'Check if the given credit card number is valid based on regex pattern.\n\n    Args:\n        credit_card_number (str): credit card number to be checked.\n\n    Returns (str): True if the credit card number is valid, otherwise False.\n    '
             '^\\d{4}[- ]?\\d{4}[- ]?\\d{4}[- ]?\\d{4}$'
             None
          names      ('re', 'search')
          varnames   ('credit_card_number', 'pattern')
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'is_valid_credit_card'
-         firstlineno 35
-         lnotab 0x02070401
+         firstlineno 43
+         lnotab 0x02090401
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x8705970067006401a2017d007401000000000000000000006a01000000
@@ -247,73 +247,73 @@
             0000000000000000006a0500000000000000007a00000064047a0000008a
             056405a00600000000000000000000000000000000000000008805660164
             068408740f000000000000000000007c01a6010000ab0100000000000000
             004400a6000000ab000000000000000000a6010000ab0100000000000000
             007d037c0364077a0000007c027a0000007d047c045300
                        0 MAKE_CELL                5 (letters)
          
-          46           2 RESUME                   0
+          56           2 RESUME                   0
          
-          52           4 BUILD_LIST               0
+          62           4 BUILD_LIST               0
                        6 LOAD_CONST               1 (('gmail.com', 'yahoo.com', 'hotmail.com', 'outlook.com', 'icloud.com', 'aol.com', 'protonmail.com', 'zoho.com'))
                        8 LIST_EXTEND              1
                       10 STORE_FAST               0 (domains)
          
-          62          12 LOAD_GLOBAL              1 (NULL + random)
+          72          12 LOAD_GLOBAL              1 (NULL + random)
                       24 LOAD_ATTR                1 (randint)
                       34 LOAD_CONST               2 (6)
                       36 LOAD_CONST               3 (12)
                       38 PRECALL                  2
                       42 CALL                     2
                       52 STORE_FAST               1 (name_length)
          
-          63          54 LOAD_GLOBAL              1 (NULL + random)
+          73          54 LOAD_GLOBAL              1 (NULL + random)
                       66 LOAD_ATTR                2 (choice)
                       76 LOAD_FAST                0 (domains)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (domain)
          
-          64          94 LOAD_GLOBAL              6 (string)
+          74          94 LOAD_GLOBAL              6 (string)
                      106 LOAD_ATTR                4 (ascii_lowercase)
                      116 LOAD_GLOBAL              6 (string)
                      128 LOAD_ATTR                5 (digits)
                      138 BINARY_OP                0 (+)
                      142 LOAD_CONST               4 ('-_')
                      144 BINARY_OP                0 (+)
                      148 STORE_DEREF              5 (letters)
          
-          65         150 LOAD_CONST               5 ('')
+          75         150 LOAD_CONST               5 ('')
                      152 LOAD_METHOD              6 (join)
                      174 LOAD_CLOSURE             5 (letters)
                      176 BUILD_TUPLE              1
-                     178 LOAD_CONST               6 (<code object <genexpr>, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 65>)
+                     178 LOAD_CONST               6 (<code object <genexpr>, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 75>)
                      180 MAKE_FUNCTION            8 (closure)
                      182 LOAD_GLOBAL             15 (NULL + range)
                      194 LOAD_FAST                1 (name_length)
                      196 PRECALL                  1
                      200 CALL                     1
                      210 GET_ITER
                      212 PRECALL                  0
                      216 CALL                     0
                      226 PRECALL                  1
                      230 CALL                     1
                      240 STORE_FAST               3 (username)
          
-          66         242 LOAD_FAST                3 (username)
+          76         242 LOAD_FAST                3 (username)
                      244 LOAD_CONST               7 ('@')
                      246 BINARY_OP                0 (+)
                      250 LOAD_FAST                2 (domain)
                      252 BINARY_OP                0 (+)
                      256 STORE_FAST               4 (email)
          
-          67         258 LOAD_FAST                4 (email)
+          77         258 LOAD_FAST                4 (email)
                      260 RETURN_VALUE
          consts
-            '\n    Generate a random email address using predefined domains.\n\n    :return: str, generated random email address\n    '
+            'Generates a random email address using predefined domains.\n\n    Returns (str): generated random email address.\n    '
             ('gmail.com', 'yahoo.com', 'hotmail.com', 'outlook.com', 'icloud.com', 'aol.com', 'protonmail.com', 'zoho.com')
             6
             12
             '-_'
             ''
             code
                argcount  : 1
@@ -322,15 +322,15 @@
                flags     : 51
                code
                   0x95014b00010097007c005d187d017401000000000000000000006a0100
                   000000000000008902a6010000ab0100000000000000005600970101008c
                   1964005300
                              0 COPY_FREE_VARS           1
                
-                65           2 RETURN_GENERATOR
+                75           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                24 (to 60)
                             12 STORE_FAST               1 (i)
                             14 LOAD_GLOBAL              1 (NULL + random)
                             26 LOAD_ATTR                1 (choice)
@@ -347,24 +347,24 @@
                   None
                names      ('random', 'choice')
                varnames   ('.0', 'i')
                freevars   ('letters',)
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
                name       '<genexpr>'
-               firstlineno 65
+               firstlineno 75
                lnotab 0x
             '@'
          names      ('random', 'randint', 'choice', 'string', 'ascii_lowercase', 'digits', 'join', 'range')
          varnames   ('domains', 'name_length', 'domain', 'username', 'email')
          freevars   ()
          cellvars   ('letters',)
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'generate_random_email'
-         firstlineno 46
+         firstlineno 56
          lnotab 0x0406080a2a01280138015c011001
       'original_field'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -373,82 +373,82 @@
             010000ab010000000000000000721b7c00a0010000000000000000000000
             000000000000000000a6000000ab00000000000000000064021900000000
             00000000007d016e0264037d016403a00200000000000000000000000000
             000000000000007407000000000000000000006a04000000000000000064
             046405ac06a6020000ab020000000000000000a6010000ab010000000000
             0000007d027c0172087c019b0064077c029b009d037d036e027c027d037c
             035300
-          70           0 RESUME                   0
+          80           0 RESUME                   0
          
-          77           2 LOAD_FAST                0 (original_field)
+          89           2 LOAD_FAST                0 (original_field)
                        4 LOAD_METHOD              0 (startswith)
                       26 LOAD_CONST               1 ('+')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 POP_JUMP_FORWARD_IF_FALSE    27 (to 98)
          
-          79          44 LOAD_FAST                0 (original_field)
+          91          44 LOAD_FAST                0 (original_field)
                       46 LOAD_METHOD              1 (split)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 LOAD_CONST               2 (0)
                       84 BINARY_SUBSCR
                       94 STORE_FAST               1 (country_code)
                       96 JUMP_FORWARD             2 (to 102)
          
-          81     >>   98 LOAD_CONST               3 ('')
+          93     >>   98 LOAD_CONST               3 ('')
                      100 STORE_FAST               1 (country_code)
          
-          83     >>  102 LOAD_CONST               3 ('')
+          95     >>  102 LOAD_CONST               3 ('')
                      104 LOAD_METHOD              2 (join)
                      126 LOAD_GLOBAL              7 (NULL + random)
                      138 LOAD_ATTR                4 (choices)
                      148 LOAD_CONST               4 ('0123456789')
                      150 LOAD_CONST               5 (10)
                      152 KW_NAMES                 6
                      154 PRECALL                  2
                      158 CALL                     2
                      168 PRECALL                  1
                      172 CALL                     1
                      182 STORE_FAST               2 (number)
          
-          85         184 LOAD_FAST                1 (country_code)
+          97         184 LOAD_FAST                1 (country_code)
                      186 POP_JUMP_FORWARD_IF_FALSE     8 (to 204)
          
-          86         188 LOAD_FAST                1 (country_code)
+          98         188 LOAD_FAST                1 (country_code)
                      190 FORMAT_VALUE             0
                      192 LOAD_CONST               7 (' ')
                      194 LOAD_FAST                2 (number)
                      196 FORMAT_VALUE             0
                      198 BUILD_STRING             3
                      200 STORE_FAST               3 (phone_number)
                      202 JUMP_FORWARD             2 (to 208)
          
-          88     >>  204 LOAD_FAST                2 (number)
+         100     >>  204 LOAD_FAST                2 (number)
                      206 STORE_FAST               3 (phone_number)
          
-          90     >>  208 LOAD_FAST                3 (phone_number)
+         102     >>  208 LOAD_FAST                3 (phone_number)
                      210 RETURN_VALUE
          consts
-            '\n    Generate a random phone number with country code if originally present.\n\n    :param original_field: str, original phone number field\n    :return: str, generated random phone number\n    '
+            'Generate a random phone number with country code if originally present.\n\n    Args:\n        original_field (str): original phone number field.\n\n    Returns (str): generated random phone number.\n    '
             '+'
             0
             ''
             '0123456789'
             10
             ('k',)
             ' '
          names      ('startswith', 'split', 'join', 'random', 'choices')
          varnames   ('original_field', 'country_code', 'number', 'phone_number')
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'generate_random_phone_number'
-         firstlineno 70
-         lnotab 0x02072a02360204025202040110020402
+         firstlineno 80
+         lnotab 0x02092a02360204025202040110020402
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
             0x970067007d007401000000000000000000006401a6010000ab01000000
@@ -456,362 +456,377 @@
             00000000007405000000000000000000006a030000000000000000640364
             01ac04a6020000ab020000000000000000a6010000ab0100000000000000
             007d027c00a00400000000000000000000000000000000000000007c02a6
             010000ab01000000000000000001008c417405000000000000000000006a
             050000000000000000640564066702a6010000ab0100000000000000007d
             037c03a00100000000000000000000000000000000000000007c00a60100
             00ab0100000000000000005300
-          93           0 RESUME                   0
+         105           0 RESUME                   0
          
-          99           2 BUILD_LIST               0
+         111           2 BUILD_LIST               0
                        4 STORE_FAST               0 (groups)
          
-         100           6 LOAD_GLOBAL              1 (NULL + range)
+         112           6 LOAD_GLOBAL              1 (NULL + range)
                       18 LOAD_CONST               1 (4)
                       20 PRECALL                  1
                       24 CALL                     1
                       34 GET_ITER
                  >>   36 FOR_ITER                64 (to 166)
                       38 STORE_FAST               1 (_i)
          
-         101          40 LOAD_CONST               2 ('')
+         113          40 LOAD_CONST               2 ('')
                       42 LOAD_METHOD              1 (join)
                       64 LOAD_GLOBAL              5 (NULL + random)
                       76 LOAD_ATTR                3 (choices)
                       86 LOAD_CONST               3 ('0123456789')
                       88 LOAD_CONST               1 (4)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (group)
          
-         102         122 LOAD_FAST                0 (groups)
+         114         122 LOAD_FAST                0 (groups)
                      124 LOAD_METHOD              4 (append)
                      146 LOAD_FAST                2 (group)
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
                      164 JUMP_BACKWARD           65 (to 36)
          
-         103     >>  166 LOAD_GLOBAL              5 (NULL + random)
+         115     >>  166 LOAD_GLOBAL              5 (NULL + random)
                      178 LOAD_ATTR                5 (choice)
                      188 LOAD_CONST               5 ('-')
                      190 LOAD_CONST               6 (' ')
                      192 BUILD_LIST               2
                      194 PRECALL                  1
                      198 CALL                     1
                      208 STORE_FAST               3 (separator)
          
-         104         210 LOAD_FAST                3 (separator)
+         116         210 LOAD_FAST                3 (separator)
                      212 LOAD_METHOD              1 (join)
                      234 LOAD_FAST                0 (groups)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 RETURN_VALUE
          consts
-            '\n    Generate a random credit card number.\n\n    :return: str, generated random credit card number\n    '
+            'Generate a random credit card number.\n\n    Returns (str): generated random credit card number.\n    '
             4
             ''
             '0123456789'
             ('k',)
             '-'
             ' '
          names      ('range', 'join', 'random', 'choices', 'append', 'choice')
          varnames   ('groups', '_i', 'group', 'separator')
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'generate_random_credit_card'
-         firstlineno 93
+         firstlineno 105
          lnotab 0x02060401220152012c012c01
       'data_frame'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000a60000
             00ab000000000000000000a0010000000000000000000000000000000000
             000000a6000000ab0000000000000000005300
-         107           0 RESUME                   0
+         119           0 RESUME                   0
          
-         114           2 LOAD_FAST                0 (data_frame)
+         128           2 LOAD_FAST                0 (data_frame)
                        4 LOAD_METHOD              0 (head)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 LOAD_METHOD              1 (copy)
                       62 PRECALL                  0
                       66 CALL                     0
                       76 RETURN_VALUE
          consts
-            '\n    Copy the head of a DataFrame.\n\n    :param data_frame: pd.DataFrame, the DataFrame to copy the head from\n    :return: pd.DataFrame, copied head of the DataFrame\n    '
+            'Copy the head of a DataFrame.\n\n    Args:\n        data_frame (pd.DataFrame): The pd.DataFrame to copy the head from.\n\n    Returns (pd.DataFrame): copied head of the DataFrame.\n    '
          names      ('head', 'copy')
          varnames   ('data_frame',)
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'copy_head'
-         firstlineno 107
-         lnotab 0x0207
+         firstlineno 119
+         lnotab 0x0209
       True
       'force_conversion'
       code
          argcount  : 2
          nlocals   : 9
          stacksize : 10
          flags     : 3
          code
             0x870997007401000000000000000000007c00a6010000ab010000000000
             0000007d007c006a0100000000000000007d027c006a0200000000000000
-            00440090015da17d037c006a020000000000000000a00300000000000000
+            00440090015dbb7d037c006a020000000000000000a00300000000000000
             000000000000000000000000007c03a6010000ab0100000000000000007d
             047c0172797408000000000000000000006a0500000000000000006a0600
             00000000000000a00700000000000000000000000000000000000000007c
             007c0319000000000000000000a6010000ab010000000000000000724f7c
             007c0319000000000000000000a008000000000000000000000000000000
             0000000000a6000000ab000000000000000000a009000000000000000000
             0000000000000000000000a6000000ab00000000000000000072237c007c
             0319000000000000000000a00a0000000000000000000000000000000000
             000000741600000000000000000000a6010000ab0100000000000000007c
             007c033c0000007419000000000000000000007c007c0319000000000000
-            000000a6010000ab01000000000000000044005df35c0200008a097d0574
-            1b000000000000000000007c05a6010000ab0100000000000000007d0674
-            1d000000000000000000007c06a6010000ab010000000000000000721974
-            1f00000000000000000000a6000000ab0000000000000000007c006a1000
-            0000000000000089097c0466023c0000008c3c7423000000000000000000
-            007c06a6010000ab010000000000000000721a7425000000000000000000
-            007c06a6010000ab0100000000000000007c006a10000000000000000089
-            097c0466023c0000008c657427000000000000000000007c06a6010000ab
-            0100000000000000007219742900000000000000000000a6000000ab0000
-            000000000000007c006a10000000000000000089097c0466023c0000008c
-            8d742b000000000000000000006a16000000000000000088096601640184
-            08742f000000000000000000007431000000000000000000007c006a1900
-            00000000000000a6010000ab010000000000000000a6010000ab01000000
-            00000000004400a6000000ab000000000000000000a6010000ab01000000
-            00000000007d077c006a1000000000000000007c077c0466021900000000
-            00000000007d087c087c006a10000000000000000089097c0466023c0000
-            007c067c006a1000000000000000007c077c0466023c0000008cf490018c
-            a37c00a00a00000000000000000000000000000000000000007c02a60100
-            00ab0100000000000000007d007c005300
+            000000a6010000ab010000000000000000440090015d0c5c0200008a097d
+            05741b000000000000000000007c05a6010000ab0100000000000000007d
+            06741d000000000000000000007c06a6010000ab01000000000000000072
+            19741f00000000000000000000a6000000ab0000000000000000007c006a
+            10000000000000000089097c0466023c0000008c3d742300000000000000
+            0000007c06a6010000ab010000000000000000721a742500000000000000
+            0000007c06a6010000ab0100000000000000007c006a1000000000000000
+            0089097c0466023c0000008c667427000000000000000000007c06a60100
+            00ab0100000000000000007219742900000000000000000000a6000000ab
+            0000000000000000007c006a10000000000000000089097c0466023c0000
+            008c8e742b000000000000000000006a1600000000000000008809660164
+            018408742f000000000000000000007431000000000000000000007c006a
+            190000000000000000a6010000ab010000000000000000a6010000ab0100
+            000000000000004400a6000000ab000000000000000000a6010000ab0100
+            000000000000007d077c006a1000000000000000007c077c046602190000
+            000000000000007d087c087c006a10000000000000000089097c0466023c
+            0000007c066402760072147409000000000000000000006a1a0000000000
+            0000007c06a6010000ab0100000000000000006e017c067c006a10000000
+            00000000007c077c0466023c00000090018c0e90018cbd7c00a00a000000
+            00000000000000000000000000000000007c02a6010000ab010000000000
+            0000007d007c005300
                        0 MAKE_CELL                9 (row_idx)
          
-         117           2 RESUME                   0
+         131           2 RESUME                   0
          
-         126           4 LOAD_GLOBAL              1 (NULL + copy_head)
+         144           4 LOAD_GLOBAL              1 (NULL + copy_head)
                       16 LOAD_FAST                0 (data_frame)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               0 (data_frame)
          
-         127          34 LOAD_FAST                0 (data_frame)
+         145          34 LOAD_FAST                0 (data_frame)
                       36 LOAD_ATTR                1 (dtypes)
                       46 STORE_FAST               2 (dtypes)
          
-         128          48 LOAD_FAST                0 (data_frame)
+         146          48 LOAD_FAST                0 (data_frame)
                       50 LOAD_ATTR                2 (columns)
                       60 GET_ITER
                  >>   62 EXTENDED_ARG             1
-                      64 FOR_ITER               417 (to 900)
+                      64 FOR_ITER               443 (to 952)
                       66 STORE_FAST               3 (col)
          
-         129          68 LOAD_FAST                0 (data_frame)
+         147          68 LOAD_FAST                0 (data_frame)
                       70 LOAD_ATTR                2 (columns)
                       80 LOAD_METHOD              3 (get_loc)
                      102 LOAD_FAST                3 (col)
                      104 PRECALL                  1
                      108 CALL                     1
                      118 STORE_FAST               4 (col_idx)
          
-         131         120 LOAD_FAST                1 (force_conversion)
+         149         120 LOAD_FAST                1 (force_conversion)
                      122 POP_JUMP_FORWARD_IF_FALSE   121 (to 366)
          
-         132         124 LOAD_GLOBAL              8 (pd)
+         150         124 LOAD_GLOBAL              8 (pd)
                      136 LOAD_ATTR                5 (api)
                      146 LOAD_ATTR                6 (types)
                      156 LOAD_METHOD              7 (is_categorical_dtype)
                      178 LOAD_FAST                0 (data_frame)
                      180 LOAD_FAST                3 (col)
                      182 BINARY_SUBSCR
                      192 PRECALL                  1
                      196 CALL                     1
                      206 POP_JUMP_FORWARD_IF_FALSE    79 (to 366)
          
-         133         208 LOAD_FAST                0 (data_frame)
+         151         208 LOAD_FAST                0 (data_frame)
                      210 LOAD_FAST                3 (col)
                      212 BINARY_SUBSCR
                      222 LOAD_METHOD              8 (isna)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 LOAD_METHOD              9 (any)
                      280 PRECALL                  0
                      284 CALL                     0
                      294 POP_JUMP_FORWARD_IF_FALSE    35 (to 366)
          
-         134         296 LOAD_FAST                0 (data_frame)
+         152         296 LOAD_FAST                0 (data_frame)
                      298 LOAD_FAST                3 (col)
                      300 BINARY_SUBSCR
                      310 LOAD_METHOD             10 (astype)
                      332 LOAD_GLOBAL             22 (object)
                      344 PRECALL                  1
                      348 CALL                     1
                      358 LOAD_FAST                0 (data_frame)
                      360 LOAD_FAST                3 (col)
                      362 STORE_SUBSCR
          
-         135     >>  366 LOAD_GLOBAL             25 (NULL + enumerate)
+         153     >>  366 LOAD_GLOBAL             25 (NULL + enumerate)
                      378 LOAD_FAST                0 (data_frame)
                      380 LOAD_FAST                3 (col)
                      382 BINARY_SUBSCR
                      392 PRECALL                  1
                      396 CALL                     1
                      406 GET_ITER
-                 >>  408 FOR_ITER               243 (to 896)
-                     410 UNPACK_SEQUENCE          2
-                     414 STORE_DEREF              9 (row_idx)
-                     416 STORE_FAST               5 (val)
-         
-         136         418 LOAD_GLOBAL             27 (NULL + str)
-                     430 LOAD_FAST                5 (val)
-                     432 PRECALL                  1
-                     436 CALL                     1
-                     446 STORE_FAST               6 (cell_value)
-         
-         138         448 LOAD_GLOBAL             29 (NULL + is_valid_email)
-                     460 LOAD_FAST                6 (cell_value)
-                     462 PRECALL                  1
-                     466 CALL                     1
-                     476 POP_JUMP_FORWARD_IF_FALSE    25 (to 528)
-         
-         139         478 LOAD_GLOBAL             31 (NULL + generate_random_email)
-                     490 PRECALL                  0
-                     494 CALL                     0
-                     504 LOAD_FAST                0 (data_frame)
-                     506 LOAD_ATTR               16 (iloc)
-                     516 LOAD_DEREF               9 (row_idx)
-                     518 LOAD_FAST                4 (col_idx)
-                     520 BUILD_TUPLE              2
-                     522 STORE_SUBSCR
-         
-         140         526 JUMP_BACKWARD           60 (to 408)
-         
-         141     >>  528 LOAD_GLOBAL             35 (NULL + is_valid_phone_number)
-                     540 LOAD_FAST                6 (cell_value)
-                     542 PRECALL                  1
-                     546 CALL                     1
-                     556 POP_JUMP_FORWARD_IF_FALSE    26 (to 610)
-         
-         142         558 LOAD_GLOBAL             37 (NULL + generate_random_phone_number)
-         
-         143         570 LOAD_FAST                6 (cell_value)
-         
-         142         572 PRECALL                  1
-                     576 CALL                     1
-                     586 LOAD_FAST                0 (data_frame)
-                     588 LOAD_ATTR               16 (iloc)
-                     598 LOAD_DEREF               9 (row_idx)
-                     600 LOAD_FAST                4 (col_idx)
-                     602 BUILD_TUPLE              2
-                     604 STORE_SUBSCR
-         
-         145         608 JUMP_BACKWARD          101 (to 408)
-         
-         146     >>  610 LOAD_GLOBAL             39 (NULL + is_valid_credit_card)
-                     622 LOAD_FAST                6 (cell_value)
-                     624 PRECALL                  1
-                     628 CALL                     1
-                     638 POP_JUMP_FORWARD_IF_FALSE    25 (to 690)
-         
-         147         640 LOAD_GLOBAL             41 (NULL + generate_random_credit_card)
-                     652 PRECALL                  0
-                     656 CALL                     0
-                     666 LOAD_FAST                0 (data_frame)
-                     668 LOAD_ATTR               16 (iloc)
-                     678 LOAD_DEREF               9 (row_idx)
-                     680 LOAD_FAST                4 (col_idx)
-                     682 BUILD_TUPLE              2
-                     684 STORE_SUBSCR
-         
-         148         688 JUMP_BACKWARD          141 (to 408)
-         
-         151     >>  690 LOAD_GLOBAL             43 (NULL + random)
-                     702 LOAD_ATTR               22 (choice)
-         
-         152         712 LOAD_CLOSURE             9 (row_idx)
-                     714 BUILD_TUPLE              1
-                     716 LOAD_CONST               1 (<code object <listcomp>, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 152>)
-                     718 MAKE_FUNCTION            8 (closure)
-                     720 LOAD_GLOBAL             47 (NULL + range)
-                     732 LOAD_GLOBAL             49 (NULL + len)
-                     744 LOAD_FAST                0 (data_frame)
-                     746 LOAD_ATTR               25 (index)
-                     756 PRECALL                  1
-                     760 CALL                     1
-                     770 PRECALL                  1
-                     774 CALL                     1
-                     784 GET_ITER
-                     786 PRECALL                  0
-                     790 CALL                     0
-         
-         151         800 PRECALL                  1
-                     804 CALL                     1
-                     814 STORE_FAST               7 (random_row_index)
-         
-         154         816 LOAD_FAST                0 (data_frame)
-                     818 LOAD_ATTR               16 (iloc)
-                     828 LOAD_FAST                7 (random_row_index)
-                     830 LOAD_FAST                4 (col_idx)
-                     832 BUILD_TUPLE              2
-                     834 BINARY_SUBSCR
-                     844 STORE_FAST               8 (random_value)
-         
-         155         846 LOAD_FAST                8 (random_value)
-                     848 LOAD_FAST                0 (data_frame)
-                     850 LOAD_ATTR               16 (iloc)
-                     860 LOAD_DEREF               9 (row_idx)
-                     862 LOAD_FAST                4 (col_idx)
-                     864 BUILD_TUPLE              2
-                     866 STORE_SUBSCR
-         
-         156         870 LOAD_FAST                6 (cell_value)
-                     872 LOAD_FAST                0 (data_frame)
-                     874 LOAD_ATTR               16 (iloc)
-                     884 LOAD_FAST                7 (random_row_index)
-                     886 LOAD_FAST                4 (col_idx)
-                     888 BUILD_TUPLE              2
-                     890 STORE_SUBSCR
-                     894 JUMP_BACKWARD          244 (to 408)
-         
-         135     >>  896 EXTENDED_ARG             1
-                     898 JUMP_BACKWARD          419 (to 62)
-         
-         158     >>  900 LOAD_FAST                0 (data_frame)
-                     902 LOAD_METHOD             10 (astype)
-                     924 LOAD_FAST                2 (dtypes)
-                     926 PRECALL                  1
-                     930 CALL                     1
-                     940 STORE_FAST               0 (data_frame)
+                 >>  408 EXTENDED_ARG             1
+                     410 FOR_ITER               268 (to 948)
+                     412 UNPACK_SEQUENCE          2
+                     416 STORE_DEREF              9 (row_idx)
+                     418 STORE_FAST               5 (val)
+         
+         154         420 LOAD_GLOBAL             27 (NULL + str)
+                     432 LOAD_FAST                5 (val)
+                     434 PRECALL                  1
+                     438 CALL                     1
+                     448 STORE_FAST               6 (cell_value)
+         
+         156         450 LOAD_GLOBAL             29 (NULL + is_valid_email)
+                     462 LOAD_FAST                6 (cell_value)
+                     464 PRECALL                  1
+                     468 CALL                     1
+                     478 POP_JUMP_FORWARD_IF_FALSE    25 (to 530)
+         
+         157         480 LOAD_GLOBAL             31 (NULL + generate_random_email)
+                     492 PRECALL                  0
+                     496 CALL                     0
+                     506 LOAD_FAST                0 (data_frame)
+                     508 LOAD_ATTR               16 (iloc)
+                     518 LOAD_DEREF               9 (row_idx)
+                     520 LOAD_FAST                4 (col_idx)
+                     522 BUILD_TUPLE              2
+                     524 STORE_SUBSCR
+         
+         158         528 JUMP_BACKWARD           61 (to 408)
+         
+         159     >>  530 LOAD_GLOBAL             35 (NULL + is_valid_phone_number)
+                     542 LOAD_FAST                6 (cell_value)
+                     544 PRECALL                  1
+                     548 CALL                     1
+                     558 POP_JUMP_FORWARD_IF_FALSE    26 (to 612)
+         
+         160         560 LOAD_GLOBAL             37 (NULL + generate_random_phone_number)
+         
+         161         572 LOAD_FAST                6 (cell_value)
+         
+         160         574 PRECALL                  1
+                     578 CALL                     1
+                     588 LOAD_FAST                0 (data_frame)
+                     590 LOAD_ATTR               16 (iloc)
+                     600 LOAD_DEREF               9 (row_idx)
+                     602 LOAD_FAST                4 (col_idx)
+                     604 BUILD_TUPLE              2
+                     606 STORE_SUBSCR
+         
+         163         610 JUMP_BACKWARD          102 (to 408)
+         
+         164     >>  612 LOAD_GLOBAL             39 (NULL + is_valid_credit_card)
+                     624 LOAD_FAST                6 (cell_value)
+                     626 PRECALL                  1
+                     630 CALL                     1
+                     640 POP_JUMP_FORWARD_IF_FALSE    25 (to 692)
+         
+         165         642 LOAD_GLOBAL             41 (NULL + generate_random_credit_card)
+                     654 PRECALL                  0
+                     658 CALL                     0
+                     668 LOAD_FAST                0 (data_frame)
+                     670 LOAD_ATTR               16 (iloc)
+                     680 LOAD_DEREF               9 (row_idx)
+                     682 LOAD_FAST                4 (col_idx)
+                     684 BUILD_TUPLE              2
+                     686 STORE_SUBSCR
+         
+         166         690 JUMP_BACKWARD          142 (to 408)
+         
+         169     >>  692 LOAD_GLOBAL             43 (NULL + random)
+                     704 LOAD_ATTR               22 (choice)
+         
+         170         714 LOAD_CLOSURE             9 (row_idx)
+                     716 BUILD_TUPLE              1
+                     718 LOAD_CONST               1 (<code object <listcomp>, file "D:\Pro\pandas-ai-main\pandasai\helpers\anonymizer.py", line 170>)
+                     720 MAKE_FUNCTION            8 (closure)
+                     722 LOAD_GLOBAL             47 (NULL + range)
+                     734 LOAD_GLOBAL             49 (NULL + len)
+                     746 LOAD_FAST                0 (data_frame)
+                     748 LOAD_ATTR               25 (index)
+                     758 PRECALL                  1
+                     762 CALL                     1
+                     772 PRECALL                  1
+                     776 CALL                     1
+                     786 GET_ITER
+                     788 PRECALL                  0
+                     792 CALL                     0
+         
+         169         802 PRECALL                  1
+                     806 CALL                     1
+                     816 STORE_FAST               7 (random_row_index)
+         
+         172         818 LOAD_FAST                0 (data_frame)
+                     820 LOAD_ATTR               16 (iloc)
+                     830 LOAD_FAST                7 (random_row_index)
+                     832 LOAD_FAST                4 (col_idx)
+                     834 BUILD_TUPLE              2
+                     836 BINARY_SUBSCR
+                     846 STORE_FAST               8 (random_value)
+         
+         173         848 LOAD_FAST                8 (random_value)
+                     850 LOAD_FAST                0 (data_frame)
+                     852 LOAD_ATTR               16 (iloc)
+                     862 LOAD_DEREF               9 (row_idx)
+                     864 LOAD_FAST                4 (col_idx)
+                     866 BUILD_TUPLE              2
+                     868 STORE_SUBSCR
+         
+         175         872 LOAD_FAST                6 (cell_value)
+                     874 LOAD_CONST               2 (('True', 'False'))
+                     876 CONTAINS_OP              0
+                     878 POP_JUMP_FORWARD_IF_FALSE    20 (to 920)
+                     880 LOAD_GLOBAL              9 (NULL + pd)
+                     892 LOAD_ATTR               26 (eval)
+                     902 LOAD_FAST                6 (cell_value)
+                     904 PRECALL                  1
+                     908 CALL                     1
+                     918 JUMP_FORWARD             1 (to 922)
+                 >>  920 LOAD_FAST                6 (cell_value)
+         
+         174     >>  922 LOAD_FAST                0 (data_frame)
+                     924 LOAD_ATTR               16 (iloc)
+                     934 LOAD_FAST                7 (random_row_index)
+                     936 LOAD_FAST                4 (col_idx)
+                     938 BUILD_TUPLE              2
+                     940 STORE_SUBSCR
+                     944 EXTENDED_ARG             1
+                     946 JUMP_BACKWARD          270 (to 408)
+         
+         153     >>  948 EXTENDED_ARG             1
+                     950 JUMP_BACKWARD          445 (to 62)
+         
+         178     >>  952 LOAD_FAST                0 (data_frame)
+                     954 LOAD_METHOD             10 (astype)
+                     976 LOAD_FAST                2 (dtypes)
+                     978 PRECALL                  1
+                     982 CALL                     1
+                     992 STORE_FAST               0 (data_frame)
          
-         159         942 LOAD_FAST                0 (data_frame)
-                     944 RETURN_VALUE
+         179         994 LOAD_FAST                0 (data_frame)
+                     996 RETURN_VALUE
          consts
-            '\n    Anonymize the head of a given DataFrame by replacing sensitive data.\n\n    :param data_frame: pd.DataFrame, the DataFrame to anonymize the head\n    :return: pd.DataFrame, anonymized head of the DataFrame\n    '
+            'Anonymize the head of a given DataFrame by replacing sensitive data.\n\n    Args:\n\n        data_frame (pd.DataFrame):  The DataFrame to anonymize the head data.\n        force_conversion (bool): Convert it with instruction. Default is True.\n\n    Returns: Anonymized head of the DataFrame.\n    '
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x9501970067007c005d0a7d017c0189026b0300000000af087c0191028c
                   0b5300
                              0 COPY_FREE_VARS           1
                
-               152           2 RESUME                   0
+               170           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                10 (to 30)
                             10 STORE_FAST               1 (i)
                             12 LOAD_FAST                1 (i)
                             14 LOAD_DEREF               2 (row_idx)
                             16 COMPARE_OP               3 (!=)
@@ -823,31 +838,32 @@
                consts
                names      ()
                varnames   ('.0', 'i')
                freevars   ('row_idx',)
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
                name       '<listcomp>'
-               firstlineno 152
+               firstlineno 170
                lnotab 0x
-         names      ('copy_head', 'dtypes', 'columns', 'get_loc', 'pd', 'api', 'types', 'is_categorical_dtype', 'isna', 'any', 'astype', 'object', 'enumerate', 'str', 'is_valid_email', 'generate_random_email', 'iloc', 'is_valid_phone_number', 'generate_random_phone_number', 'is_valid_credit_card', 'generate_random_credit_card', 'random', 'choice', 'range', 'len', 'index')
+            ('True', 'False')
+         names      ('copy_head', 'dtypes', 'columns', 'get_loc', 'pd', 'api', 'types', 'is_categorical_dtype', 'isna', 'any', 'astype', 'object', 'enumerate', 'str', 'is_valid_email', 'generate_random_email', 'iloc', 'is_valid_phone_number', 'generate_random_phone_number', 'is_valid_credit_card', 'generate_random_credit_card', 'random', 'choice', 'range', 'len', 'index', 'eval')
          varnames   ('data_frame', 'force_conversion', 'dtypes', 'col', 'col_idx', 'val', 'cell_value', 'random_row_index', 'random_value')
          freevars   ()
          cellvars   ('row_idx',)
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
          name       'anonymize_dataframe_head'
-         firstlineno 117
+         firstlineno 131
          lnotab
-            0x04091e010e0114013402040154015801460134011e021e01300102011e
-            010c0102ff240302011e0130010203160158ff10031e0118011aeb04172a
-            01
+            0x040d1e010e0114013402040154015801460136011e021e01300102011e
+            010c0102ff240302011e0130010203160158ff10031e01180232ff1aeb04
+            192a01
       (True,)
    names      ('__doc__', 'random', 're', 'string', 'pandas', 'pd', 'str', 'bool', 'is_valid_email', 'is_valid_phone_number', 'is_valid_credit_card', 'generate_random_email', 'generate_random_phone_number', 'generate_random_credit_card', 'DataFrame', 'copy_head', 'anonymize_dataframe_head')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\anonymizer.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104050801080108020803100b100b100b0c1810170c0e240b02
+      0x00ff020104090801080108020803100d100d100d0c1810190c0e240d02
       ff04010cff020102ff02020cfe
```

### Comparing `hfttai-0.1.2/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc` & `hfttai-0.1.3/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/__pycache__/notebook.cpython-311.pyc` & `hfttai-0.1.3/pandasai/helpers/__pycache__/notebook.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,74 +1,74 @@
 magic:    0xa70d0d0a
-moddate:  0xaaaa6e64 (Thu May 25 00:24:10 2023 UTC)
-files sz: 1505
+moddate:  0x26d2a764 (Fri Jul  7 08:51:50 2023 UTC)
+files sz: 1493
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970064005a00640164026c016d025a02010002004700640384006404a6
       020000ab0200000000000000005a0364055300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (' Notebook helper functions ')
+     1           2 LOAD_CONST               0 (' Helper Module to Handle Jupyter Notebook\nThis module contains helper functions to interact with Jupyter Notebook Functionalities.\n\n')
                  4 STORE_NAME               0 (__doc__)
    
-     3           6 LOAD_CONST               1 (0)
+     6           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('get_ipython',))
                 10 IMPORT_NAME              1 (IPython)
                 12 IMPORT_FROM              2 (get_ipython)
                 14 STORE_NAME               2 (get_ipython)
                 16 POP_TOP
    
-     6          18 PUSH_NULL
+     9          18 PUSH_NULL
                 20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               3 (<code object Notebook, file "D:\Pro\pandas-ai-main\pandasai\helpers\notebook.py", line 6>)
+                22 LOAD_CONST               3 (<code object Notebook, file "D:\Pro\pandas-ai-main\pandasai\helpers\notebook.py", line 9>)
                 24 MAKE_FUNCTION            0
                 26 LOAD_CONST               4 ('Notebook')
                 28 PRECALL                  2
                 32 CALL                     2
                 42 STORE_NAME               3 (Notebook)
                 44 LOAD_CONST               5 (None)
                 46 RETURN_VALUE
    consts
-      ' Notebook helper functions '
+      ' Helper Module to Handle Jupyter Notebook\nThis module contains helper functions to interact with Jupyter Notebook Functionalities.\n\n'
       0
       ('get_ipython',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264015a03640265046602640384045a05640465
             06640264056604640684045a0764055300
-           6           0 RESUME                   0
+           9           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Notebook')
                        8 STORE_NAME               2 (__qualname__)
          
-           8          10 LOAD_CONST               1 ('Baseclass to implement Notebook helper functions')
+          11          10 LOAD_CONST               1 ('Baseclass to implement Notebook helper functions')
                       12 STORE_NAME               3 (__doc__)
          
-          10          14 LOAD_CONST               2 ('return')
+          13          14 LOAD_CONST               2 ('return')
                       16 LOAD_NAME                4 (bool)
                       18 BUILD_TUPLE              2
-                      20 LOAD_CONST               3 (<code object in_notebook, file "D:\Pro\pandas-ai-main\pandasai\helpers\notebook.py", line 10>)
+                      20 LOAD_CONST               3 (<code object in_notebook, file "D:\Pro\pandas-ai-main\pandasai\helpers\notebook.py", line 13>)
                       22 MAKE_FUNCTION            4 (annotations)
                       24 STORE_NAME               5 (in_notebook)
          
-          26          26 LOAD_CONST               4 ('contents')
+          27          26 LOAD_CONST               4 ('contents')
                       28 LOAD_NAME                6 (str)
                       30 LOAD_CONST               2 ('return')
                       32 LOAD_CONST               5 (None)
                       34 BUILD_TUPLE              4
-                      36 LOAD_CONST               6 (<code object create_new_cell, file "D:\Pro\pandas-ai-main\pandasai\helpers\notebook.py", line 26>)
+                      36 LOAD_CONST               6 (<code object create_new_cell, file "D:\Pro\pandas-ai-main\pandasai\helpers\notebook.py", line 27>)
                       38 MAKE_FUNCTION            4 (annotations)
                       40 STORE_NAME               7 (create_new_cell)
                       42 LOAD_CONST               5 (None)
                       44 RETURN_VALUE
          consts
             'Notebook'
             'Baseclass to implement Notebook helper functions'
@@ -76,167 +76,159 @@
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970009006401740100000000000000000000a6000000ab000000000000
-                  0000006a01000000000000000076017202640253006e1d23007404000000
-                  000000000000002400720401005900640253007406000000000000000000
-                  00240072040100590064025300770078035900770164035300
-                10           0 RESUME                   0
+                  0000006a01000000000000000076017202640253006e1823007404000000
+                  000000000000007406000000000000000000006602240072040100590064
+                  025300770078035900770164035300
+                13           0 RESUME                   0
                
-                17           2 NOP
+                20           2 NOP
                
-                18           4 LOAD_CONST               1 ('IPKernelApp')
+                21           4 LOAD_CONST               1 ('IPKernelApp')
                              6 LOAD_GLOBAL              1 (NULL + get_ipython)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (config)
                             42 CONTAINS_OP              1
                             44 POP_JUMP_FORWARD_IF_FALSE     2 (to 50)
                
-                19          46 LOAD_CONST               2 (False)
+                22          46 LOAD_CONST               2 (False)
                             48 RETURN_VALUE
                
-                18     >>   50 JUMP_FORWARD            29 (to 110)
+                21     >>   50 JUMP_FORWARD            24 (to 100)
                        >>   52 PUSH_EXC_INFO
                
-                20          54 LOAD_GLOBAL              4 (ImportError)
-                            66 CHECK_EXC_MATCH
-                            68 POP_JUMP_FORWARD_IF_FALSE     4 (to 78)
-                            70 POP_TOP
-               
-                21          72 POP_EXCEPT
-                            74 LOAD_CONST               2 (False)
-                            76 RETURN_VALUE
-               
-                22     >>   78 LOAD_GLOBAL              6 (AttributeError)
-                            90 CHECK_EXC_MATCH
-                            92 POP_JUMP_FORWARD_IF_FALSE     4 (to 102)
-                            94 POP_TOP
-               
-                23          96 POP_EXCEPT
-                            98 LOAD_CONST               2 (False)
-                           100 RETURN_VALUE
-               
-                22     >>  102 RERAISE                  0
-                       >>  104 COPY                     3
-                           106 POP_EXCEPT
-                           108 RERAISE                  1
+                23          54 LOAD_GLOBAL              4 (ImportError)
+                            66 LOAD_GLOBAL              6 (AttributeError)
+                            78 BUILD_TUPLE              2
+                            80 CHECK_EXC_MATCH
+                            82 POP_JUMP_FORWARD_IF_FALSE     4 (to 92)
+                            84 POP_TOP
+               
+                24          86 POP_EXCEPT
+                            88 LOAD_CONST               2 (False)
+                            90 RETURN_VALUE
+               
+                23     >>   92 RERAISE                  0
+                       >>   94 COPY                     3
+                            96 POP_EXCEPT
+                            98 RERAISE                  1
                
-                24     >>  110 LOAD_CONST               3 (True)
-                           112 RETURN_VALUE
+                25     >>  100 LOAD_CONST               3 (True)
+                           102 RETURN_VALUE
                ExceptionTable:
                  4 to 44 -> 52 [0]
-                 52 to 70 -> 104 [1] lasti
-                 78 to 94 -> 104 [1] lasti
-                 102 to 102 -> 104 [1] lasti
+                 52 to 84 -> 94 [1] lasti
+                 92 to 92 -> 94 [1] lasti
                consts
-                  '\n        Checks whether the code is running inside a notebook environment.\n\n        Returns:\n            bool: True if the code is running inside a Jupyter notebook, False otherwise.\n        '
+                  '\n        Checks whether the code is running inside a notebook environment.\n\n        Returns (bool): True if the code is running inside a Jupyter notebook,\n        False otherwise.\n        '
                   'IPKernelApp'
                   False
                   True
                names      ('get_ipython', 'config', 'ImportError', 'AttributeError')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\notebook.py'
                name       'in_notebook'
-               firstlineno 10
-               lnotab 0x020702012a0104ff040212010601120106ff0802
+               firstlineno 13
+               lnotab 0x020702012a0104ff0402200106ff0802
             'contents'
             None
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x970064017c01640264039c037d020900740100000000000000000000a6
                   000000ab0000000000000000006a010000000000000000a0020000000000
                   0000000000000000000000000000007c026402ac04a6020000ab02000000
                   000000000001006405530023007406000000000000000000007408000000
                   000000000000006602240072077d037c03820164057d037e037701770078
                   0359007701
-                26           0 RESUME                   0
+                27           0 RESUME                   0
                
-                48           2 LOAD_CONST               1 ('set_next_input')
+                45           2 LOAD_CONST               1 ('set_next_input')
                              4 LOAD_FAST                1 (contents)
                              6 LOAD_CONST               2 (False)
                              8 LOAD_CONST               3 (('source', 'text', 'replace'))
                             10 BUILD_CONST_KEY_MAP      3
                             12 STORE_FAST               2 (payload)
                
-                49          14 NOP
+                46          14 NOP
                
-                50          16 LOAD_GLOBAL              1 (NULL + get_ipython)
+                47          16 LOAD_GLOBAL              1 (NULL + get_ipython)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 LOAD_ATTR                1 (payload_manager)
                             52 LOAD_METHOD              2 (write_payload)
                             74 LOAD_FAST                2 (payload)
                             76 LOAD_CONST               2 (False)
                             78 KW_NAMES                 4
                             80 PRECALL                  2
                             84 CALL                     2
                             94 POP_TOP
                             96 LOAD_CONST               5 (None)
                             98 RETURN_VALUE
                        >>  100 PUSH_EXC_INFO
                
-                51         102 LOAD_GLOBAL              6 (ImportError)
+                48         102 LOAD_GLOBAL              6 (ImportError)
                            114 LOAD_GLOBAL              8 (AttributeError)
                            126 BUILD_TUPLE              2
                            128 CHECK_EXC_MATCH
                            130 POP_JUMP_FORWARD_IF_FALSE     7 (to 146)
                            132 STORE_FAST               3 (exception)
                
-                52         134 LOAD_FAST                3 (exception)
+                49         134 LOAD_FAST                3 (exception)
                            136 RAISE_VARARGS            1
                        >>  138 LOAD_CONST               5 (None)
                            140 STORE_FAST               3 (exception)
                            142 DELETE_FAST              3 (exception)
                            144 RERAISE                  1
                
-                51     >>  146 RERAISE                  0
+                48     >>  146 RERAISE                  0
                        >>  148 COPY                     3
                            150 POP_EXCEPT
                            152 RERAISE                  1
                ExceptionTable:
                  16 to 94 -> 100 [0]
                  100 to 132 -> 148 [1] lasti
                  134 to 136 -> 138 [1] lasti
                  138 to 146 -> 148 [1] lasti
                consts
-                  "\n        Creates a new code cell in the Jupyter notebook and populates it with the specified\n        contents.\n\n        Parameters:\n        -----------\n        contents : str\n            The contents to be added to the new code cell.\n\n        Raises:\n        -------\n        ImportError:\n            If the IPython module is not installed.\n\n        AttributeError:\n            If the 'get_ipython()' call raises an AttributeError, which can happen if the code is\n            not running inside a Jupyter notebook.\n\n        Returns:\n            None\n        "
+                  "\n        Creates a new code cell in the Jupyter notebook and populates\n        it with the specified contents.\n        Args:\n            contents (str): The contents to be added to the new code cell.\n\n        ImportError:\n            If the IPython module is not installed.\n\n        AttributeError:\n            If the 'get_ipython()' call raises an AttributeError, which can happen\n            if the code is not running inside a Jupyter notebook.\n\n        Returns: None\n\n        "
                   'set_next_input'
                   False
                   ('source', 'text', 'replace')
                   ('single',)
                   None
                names      ('get_ipython', 'payload_manager', 'write_payload', 'ImportError', 'AttributeError')
                varnames   ('self', 'contents', 'payload', 'exception')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\notebook.py'
                name       'create_new_cell'
-               firstlineno 26
-               lnotab 0x02160c010201560120010cff
+               firstlineno 27
+               lnotab 0x02120c010201560120010cff
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'bool', 'in_notebook', 'str', 'create_new_cell')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\notebook.py'
          name       'Notebook'
-         firstlineno 6
-         lnotab 0x0a0204020c10
+         firstlineno 9
+         lnotab 0x0a0204020c0e
       'Notebook'
       None
    names      ('__doc__', 'IPython', 'get_ipython', 'Notebook')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Pro\\pandas-ai-main\\pandasai\\helpers\\notebook.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104020c03
+   lnotab 0x00ff020104050c03
```

### Comparing `hfttai-0.1.2/pandasai/helpers/_optional.py` & `hfttai-0.1.3/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/anonymizer.py` & `hfttai-0.1.3/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/cache.py` & `hfttai-0.1.3/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/from_excel.py` & `hfttai-0.1.3/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/notebook.py` & `hfttai-0.1.3/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/save_chart.py` & `hfttai-0.1.3/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/helpers/shortcuts.py` & `hfttai-0.1.3/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc` & `hfttai-0.1.3/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/__pycache__/base.cpython-311.pyc` & `hfttai-0.1.3/pandasai/llm/__pycache__/base.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,280 +1,306 @@
 magic:    0xa70d0d0a
-moddate:  0xc7617064 (Fri May 26 07:37:43 2023 UTC)
-files sz: 8803
+moddate:  0x26d2a764 (Fri Jul  7 08:51:50 2023 UTC)
+files sz: 11156
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c015a01640164026c025a02640164036c036d
       045a046d055a050100640164046c066d075a076d085a086d095a09010064
-      0164026c0a5a0a640164026c0b5a0b640164056c0c6d0d5a0d0100640664
-      076c0e6d0f5a0f6d105a100100640664086c116d125a126d135a136d145a
-      1401000200470064098400640aa6020000ab0200000000000000005a1502
-      004700640b8400640c65156504a6040000ab0400000000000000005a1602
-      004700640d8400640e6515a6030000ab0300000000000000005a17020047
-      00640f840064106515a6030000ab0300000000000000005a1864025300
+      0164026c0a5a0a640164026c0b5a0b640564066c0c6d0d5a0d6d0e5a0e6d
+      0f5a0f0100640564076c106d115a110100640564086c126d135a13010002
+      00470064098400640aa6020000ab0200000000000000005a140200470064
+      0b8400640c65146504a6040000ab0400000000000000005a150200470064
+      0d8400640e6514a6030000ab0300000000000000005a1602004700640f84
+      0064106514a6030000ab0300000000000000005a1764025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (' Base class to implement a new LLM. ')
+     1           2 LOAD_CONST               0 (' Base class to implement a new LLM\n\nThis module is the base class to integrate the various LLMs API. This module also\nincludes the Base LLM classes for OpenAI, HuggingFace and Google PaLM.\n\nExample:\n\n    ```\n    from .base import BaseOpenAI\n\n    class CustomLLM(BaseOpenAI):\n\n        Custom Class Starts here!!\n    ```\n')
                  4 STORE_NAME               0 (__doc__)
    
-     3           6 LOAD_CONST               1 (0)
+    17           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (ast)
                 12 STORE_NAME               1 (ast)
    
-     4          14 LOAD_CONST               1 (0)
+    18          14 LOAD_CONST               1 (0)
                 16 LOAD_CONST               2 (None)
                 18 IMPORT_NAME              2 (re)
                 20 STORE_NAME               2 (re)
    
-     5          22 LOAD_CONST               1 (0)
+    19          22 LOAD_CONST               1 (0)
                 24 LOAD_CONST               3 (('ABC', 'abstractmethod'))
                 26 IMPORT_NAME              3 (abc)
                 28 IMPORT_FROM              4 (ABC)
                 30 STORE_NAME               4 (ABC)
                 32 IMPORT_FROM              5 (abstractmethod)
                 34 STORE_NAME               5 (abstractmethod)
                 36 POP_TOP
    
-     6          38 LOAD_CONST               1 (0)
+    20          38 LOAD_CONST               1 (0)
                 40 LOAD_CONST               4 (('Any', 'Dict', 'Optional'))
                 42 IMPORT_NAME              6 (typing)
                 44 IMPORT_FROM              7 (Any)
                 46 STORE_NAME               7 (Any)
                 48 IMPORT_FROM              8 (Dict)
                 50 STORE_NAME               8 (Dict)
                 52 IMPORT_FROM              9 (Optional)
                 54 STORE_NAME               9 (Optional)
                 56 POP_TOP
    
-     8          58 LOAD_CONST               1 (0)
+    22          58 LOAD_CONST               1 (0)
                 60 LOAD_CONST               2 (None)
                 62 IMPORT_NAME             10 (openai)
                 64 STORE_NAME              10 (openai)
    
-     9          66 LOAD_CONST               1 (0)
+    23          66 LOAD_CONST               1 (0)
                 68 LOAD_CONST               2 (None)
                 70 IMPORT_NAME             11 (requests)
                 72 STORE_NAME              11 (requests)
    
-    10          74 LOAD_CONST               1 (0)
-                76 LOAD_CONST               5 (('generativeai',))
-                78 IMPORT_NAME             12 (google)
-                80 IMPORT_FROM             13 (generativeai)
-                82 STORE_NAME              13 (generativeai)
-                84 POP_TOP
+    25          74 LOAD_CONST               5 (2)
+                76 LOAD_CONST               6 (('APIKeyNotFoundError', 'MethodNotImplementedError', 'NoCodeFoundError'))
+                78 IMPORT_NAME             12 (exceptions)
+                80 IMPORT_FROM             13 (APIKeyNotFoundError)
+                82 STORE_NAME              13 (APIKeyNotFoundError)
+                84 IMPORT_FROM             14 (MethodNotImplementedError)
+                86 STORE_NAME              14 (MethodNotImplementedError)
+                88 IMPORT_FROM             15 (NoCodeFoundError)
+                90 STORE_NAME              15 (NoCodeFoundError)
+                92 POP_TOP
    
-    12          86 LOAD_CONST               6 (2)
-                88 LOAD_CONST               7 (('END_CODE_TAG', 'START_CODE_TAG'))
-                90 IMPORT_NAME             14 (constants)
-                92 IMPORT_FROM             15 (END_CODE_TAG)
-                94 STORE_NAME              15 (END_CODE_TAG)
-                96 IMPORT_FROM             16 (START_CODE_TAG)
-                98 STORE_NAME              16 (START_CODE_TAG)
-               100 POP_TOP
+    30          94 LOAD_CONST               5 (2)
+                96 LOAD_CONST               7 (('import_dependency',))
+                98 IMPORT_NAME             16 (helpers._optional)
+               100 IMPORT_FROM             17 (import_dependency)
+               102 STORE_NAME              17 (import_dependency)
+               104 POP_TOP
    
-    13         102 LOAD_CONST               6 (2)
-               104 LOAD_CONST               8 (('APIKeyNotFoundError', 'MethodNotImplementedError', 'NoCodeFoundError'))
-               106 IMPORT_NAME             17 (exceptions)
-               108 IMPORT_FROM             18 (APIKeyNotFoundError)
-               110 STORE_NAME              18 (APIKeyNotFoundError)
-               112 IMPORT_FROM             19 (MethodNotImplementedError)
-               114 STORE_NAME              19 (MethodNotImplementedError)
-               116 IMPORT_FROM             20 (NoCodeFoundError)
-               118 STORE_NAME              20 (NoCodeFoundError)
-               120 POP_TOP
+    31         106 LOAD_CONST               5 (2)
+               108 LOAD_CONST               8 (('Prompt',))
+               110 IMPORT_NAME             18 (prompts.base)
+               112 IMPORT_FROM             19 (Prompt)
+               114 STORE_NAME              19 (Prompt)
+               116 POP_TOP
    
-    20         122 PUSH_NULL
-               124 LOAD_BUILD_CLASS
-               126 LOAD_CONST               9 (<code object LLM, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 20>)
-               128 MAKE_FUNCTION            0
-               130 LOAD_CONST              10 ('LLM')
-               132 PRECALL                  2
-               136 CALL                     2
-               146 STORE_NAME              21 (LLM)
+    34         118 PUSH_NULL
+               120 LOAD_BUILD_CLASS
+               122 LOAD_CONST               9 (<code object LLM, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 34>)
+               124 MAKE_FUNCTION            0
+               126 LOAD_CONST              10 ('LLM')
+               128 PRECALL                  2
+               132 CALL                     2
+               142 STORE_NAME              20 (LLM)
    
-   118         148 PUSH_NULL
-               150 LOAD_BUILD_CLASS
-               152 LOAD_CONST              11 (<code object BaseOpenAI, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 118>)
-               154 MAKE_FUNCTION            0
-               156 LOAD_CONST              12 ('BaseOpenAI')
-               158 LOAD_NAME               21 (LLM)
-               160 LOAD_NAME                4 (ABC)
-               162 PRECALL                  4
-               166 CALL                     4
-               176 STORE_NAME              22 (BaseOpenAI)
+   142         144 PUSH_NULL
+               146 LOAD_BUILD_CLASS
+               148 LOAD_CONST              11 (<code object BaseOpenAI, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 142>)
+               150 MAKE_FUNCTION            0
+               152 LOAD_CONST              12 ('BaseOpenAI')
+               154 LOAD_NAME               20 (LLM)
+               156 LOAD_NAME                4 (ABC)
+               158 PRECALL                  4
+               162 CALL                     4
+               172 STORE_NAME              21 (BaseOpenAI)
    
-   204         178 PUSH_NULL
-               180 LOAD_BUILD_CLASS
-               182 LOAD_CONST              13 (<code object HuggingFaceLLM, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 204>)
-               184 MAKE_FUNCTION            0
-               186 LOAD_CONST              14 ('HuggingFaceLLM')
-               188 LOAD_NAME               21 (LLM)
-               190 PRECALL                  3
-               194 CALL                     3
-               204 STORE_NAME              23 (HuggingFaceLLM)
+   248         174 PUSH_NULL
+               176 LOAD_BUILD_CLASS
+               178 LOAD_CONST              13 (<code object HuggingFaceLLM, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 248>)
+               180 MAKE_FUNCTION            0
+               182 LOAD_CONST              14 ('HuggingFaceLLM')
+               184 LOAD_NAME               20 (LLM)
+               186 PRECALL                  3
+               190 CALL                     3
+               200 STORE_NAME              22 (HuggingFaceLLM)
    
-   245         206 PUSH_NULL
-               208 LOAD_BUILD_CLASS
-               210 LOAD_CONST              15 (<code object BaseGoogle, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 245>)
-               212 MAKE_FUNCTION            0
-               214 LOAD_CONST              16 ('BaseGoogle')
-               216 LOAD_NAME               21 (LLM)
-               218 PRECALL                  3
-               222 CALL                     3
-               232 STORE_NAME              24 (BaseGoogle)
-               234 LOAD_CONST               2 (None)
-               236 RETURN_VALUE
+   310         202 PUSH_NULL
+               204 LOAD_BUILD_CLASS
+               206 LOAD_CONST              15 (<code object BaseGoogle, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 310>)
+               208 MAKE_FUNCTION            0
+               210 LOAD_CONST              16 ('BaseGoogle')
+               212 LOAD_NAME               20 (LLM)
+               214 PRECALL                  3
+               218 CALL                     3
+               228 STORE_NAME              23 (BaseGoogle)
+               230 LOAD_CONST               2 (None)
+               232 RETURN_VALUE
    consts
-      ' Base class to implement a new LLM. '
+      ' Base class to implement a new LLM\n\nThis module is the base class to integrate the various LLMs API. This module also\nincludes the Base LLM classes for OpenAI, HuggingFace and Google PaLM.\n\nExample:\n\n    ```\n    from .base import BaseOpenAI\n\n    class CustomLLM(BaseOpenAI):\n\n        Custom Class Starts here!!\n    ```\n'
       0
       None
       ('ABC', 'abstractmethod')
       ('Any', 'Dict', 'Optional')
-      ('generativeai',)
       2
-      ('END_CODE_TAG', 'START_CODE_TAG')
       ('APIKeyNotFoundError', 'MethodNotImplementedError', 'NoCodeFoundError')
+      ('import_dependency',)
+      ('Prompt',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 10
          flags     : 0
          code
             0x970065005a0164005a02550064015a0364025a04650565061900000000
-            0000000000650764033c000000650864046506660264058404a6000000ab
-            0000000000000000005a0964066506640465066604640784045a0a640884
-            005a0b6414640a6506640b6506640465066606640c84055a0c650d641564
-            0e6506640f65066410650664046506660864118405a6000000ab00000000
-            00000000005a0e640e650664126506640465066606641384045a0f640253
-            00
-          20           0 RESUME                   0
+            0000000000650764033c000000640465086602640584045a09650a640465
+            06660264068404a6000000ab0000000000000000005a0b64076506640465
+            066604640884045a0c640984005a0d6415640b6506640c65066404650666
+            06640d84055a0e650f6416640f6510641065066411650664046506660864
+            128405a6000000ab0000000000000000005a11640f651064136506640465
+            066606641484045a1264025300
+          34           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LLM')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          21          12 LOAD_CONST               1 ('Base class to implement a new LLM.')
+          35          12 LOAD_CONST               1 ('Base class to implement a new LLM.')
                       14 STORE_NAME               3 (__doc__)
          
-          23          16 LOAD_CONST               2 (None)
+          37          16 LOAD_CONST               2 (None)
                       18 STORE_NAME               4 (last_prompt)
                       20 LOAD_NAME                5 (Optional)
                       22 LOAD_NAME                6 (str)
                       24 BINARY_SUBSCR
                       34 LOAD_NAME                7 (__annotations__)
                       36 LOAD_CONST               3 ('last_prompt')
                       38 STORE_SUBSCR
          
-          25          42 LOAD_NAME                8 (property)
+          39          42 LOAD_CONST               4 ('return')
+                      44 LOAD_NAME                8 (bool)
+                      46 BUILD_TUPLE              2
+                      48 LOAD_CONST               5 (<code object is_pandasai_llm, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 39>)
+                      50 MAKE_FUNCTION            4 (annotations)
+                      52 STORE_NAME               9 (is_pandasai_llm)
+         
+          48          54 LOAD_NAME               10 (property)
+         
+          49          56 LOAD_CONST               4 ('return')
+                      58 LOAD_NAME                6 (str)
+                      60 BUILD_TUPLE              2
+                      62 LOAD_CONST               6 (<code object type, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 48>)
+                      64 MAKE_FUNCTION            4 (annotations)
          
-          26          44 LOAD_CONST               4 ('return')
-                      46 LOAD_NAME                6 (str)
-                      48 BUILD_TUPLE              2
-                      50 LOAD_CONST               5 (<code object type, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 25>)
-                      52 MAKE_FUNCTION            4 (annotations)
-         
-          25          54 PRECALL                  0
-                      58 CALL                     0
-         
-          26          68 STORE_NAME               9 (type)
-         
-          38          70 LOAD_CONST               6 ('code')
-                      72 LOAD_NAME                6 (str)
-                      74 LOAD_CONST               4 ('return')
-                      76 LOAD_NAME                6 (str)
-                      78 BUILD_TUPLE              4
-                      80 LOAD_CONST               7 (<code object _polish_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 38>)
-                      82 MAKE_FUNCTION            4 (annotations)
-                      84 STORE_NAME              10 (_polish_code)
-         
-          56          86 LOAD_CONST               8 (<code object _is_python_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 56>)
-                      88 MAKE_FUNCTION            0
-                      90 STORE_NAME              11 (_is_python_code)
-         
-          63          92 LOAD_CONST              20 (('```',))
-                      94 LOAD_CONST              10 ('response')
-                      96 LOAD_NAME                6 (str)
-                      98 LOAD_CONST              11 ('separator')
-                     100 LOAD_NAME                6 (str)
-                     102 LOAD_CONST               4 ('return')
-                     104 LOAD_NAME                6 (str)
-                     106 BUILD_TUPLE              6
-                     108 LOAD_CONST              12 (<code object _extract_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 63>)
-                     110 MAKE_FUNCTION            5 (defaults, annotations)
-                     112 STORE_NAME              12 (_extract_code)
-         
-          93         114 LOAD_NAME               13 (abstractmethod)
-         
-          94         116 LOAD_CONST              21 (('',))
-                     118 LOAD_CONST              14 ('instruction')
-                     120 LOAD_NAME                6 (str)
-                     122 LOAD_CONST              15 ('value')
-                     124 LOAD_NAME                6 (str)
-                     126 LOAD_CONST              16 ('suffix')
-                     128 LOAD_NAME                6 (str)
-                     130 LOAD_CONST               4 ('return')
-                     132 LOAD_NAME                6 (str)
-                     134 BUILD_TUPLE              8
-                     136 LOAD_CONST              17 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 93>)
-                     138 MAKE_FUNCTION            5 (defaults, annotations)
-         
-          93         140 PRECALL                  0
-                     144 CALL                     0
-         
-          94         154 STORE_NAME              14 (call)
-         
-         108         156 LOAD_CONST              14 ('instruction')
-                     158 LOAD_NAME                6 (str)
-                     160 LOAD_CONST              18 ('prompt')
-                     162 LOAD_NAME                6 (str)
-                     164 LOAD_CONST               4 ('return')
-                     166 LOAD_NAME                6 (str)
-                     168 BUILD_TUPLE              6
-                     170 LOAD_CONST              19 (<code object generate_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 108>)
-                     172 MAKE_FUNCTION            4 (annotations)
-                     174 STORE_NAME              15 (generate_code)
-                     176 LOAD_CONST               2 (None)
-                     178 RETURN_VALUE
+          48          66 PRECALL                  0
+                      70 CALL                     0
+         
+          49          80 STORE_NAME              11 (type)
+         
+          61          82 LOAD_CONST               7 ('code')
+                      84 LOAD_NAME                6 (str)
+                      86 LOAD_CONST               4 ('return')
+                      88 LOAD_NAME                6 (str)
+                      90 BUILD_TUPLE              4
+                      92 LOAD_CONST               8 (<code object _polish_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 61>)
+                      94 MAKE_FUNCTION            4 (annotations)
+                      96 STORE_NAME              12 (_polish_code)
+         
+          79          98 LOAD_CONST               9 (<code object _is_python_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 79>)
+                     100 MAKE_FUNCTION            0
+                     102 STORE_NAME              13 (_is_python_code)
+         
+          94         104 LOAD_CONST              21 (('```',))
+                     106 LOAD_CONST              11 ('response')
+                     108 LOAD_NAME                6 (str)
+                     110 LOAD_CONST              12 ('separator')
+                     112 LOAD_NAME                6 (str)
+                     114 LOAD_CONST               4 ('return')
+                     116 LOAD_NAME                6 (str)
+                     118 BUILD_TUPLE              6
+                     120 LOAD_CONST              13 (<code object _extract_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 94>)
+                     122 MAKE_FUNCTION            5 (defaults, annotations)
+                     124 STORE_NAME              14 (_extract_code)
+         
+         117         126 LOAD_NAME               15 (abstractmethod)
+         
+         118         128 LOAD_CONST              22 (('',))
+                     130 LOAD_CONST              15 ('instruction')
+                     132 LOAD_NAME               16 (Prompt)
+                     134 LOAD_CONST              16 ('value')
+                     136 LOAD_NAME                6 (str)
+                     138 LOAD_CONST              17 ('suffix')
+                     140 LOAD_NAME                6 (str)
+                     142 LOAD_CONST               4 ('return')
+                     144 LOAD_NAME                6 (str)
+                     146 BUILD_TUPLE              8
+                     148 LOAD_CONST              18 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 117>)
+                     150 MAKE_FUNCTION            5 (defaults, annotations)
+         
+         117         152 PRECALL                  0
+                     156 CALL                     0
+         
+         118         166 STORE_NAME              17 (call)
+         
+         132         168 LOAD_CONST              15 ('instruction')
+                     170 LOAD_NAME               16 (Prompt)
+                     172 LOAD_CONST              19 ('prompt')
+                     174 LOAD_NAME                6 (str)
+                     176 LOAD_CONST               4 ('return')
+                     178 LOAD_NAME                6 (str)
+                     180 BUILD_TUPLE              6
+                     182 LOAD_CONST              20 (<code object generate_code, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 132>)
+                     184 MAKE_FUNCTION            4 (annotations)
+                     186 STORE_NAME              18 (generate_code)
+                     188 LOAD_CONST               2 (None)
+                     190 RETURN_VALUE
          consts
             'LLM'
             'Base class to implement a new LLM.'
             None
             'last_prompt'
             'return'
             code
                argcount  : 1
                nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x970064015300
+                39           0 RESUME                   0
+               
+                46           2 LOAD_CONST               1 (True)
+                             4 RETURN_VALUE
+               consts
+                  '\n        Return True if the LLM is from pandasAI.\n\n        Returns:\n            bool: True if the LLM is from pandasAI\n        '
+                  True
+               names      ()
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
+               name       'is_pandasai_llm'
+               firstlineno 39
+               lnotab 0x0207
+            code
+               argcount  : 1
+               nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   008201
-                25           0 RESUME                   0
+                48           0 RESUME                   0
                
-                36           2 LOAD_GLOBAL              1 (NULL + APIKeyNotFoundError)
+                59           2 LOAD_GLOBAL              1 (NULL + APIKeyNotFoundError)
                             14 LOAD_CONST               1 ('Type has not been implemented')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RAISE_VARARGS            1
                consts
                   '\n        Return type of LLM.\n\n        Raises:\n            APIKeyNotFoundError: Type has not been implemented\n\n        Returns:\n            str: Type of LLM a string\n        '
                   'Type has not been implemented'
                names      ('APIKeyNotFoundError',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'type'
-               firstlineno 25
+               firstlineno 48
                lnotab 0x020b
             'code'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
@@ -283,300 +309,247 @@
                   020000ab02000000000000000072167401000000000000000000006a0200
                   00000000000000640164027c01a6030000ab0300000000000000007d0174
                   01000000000000000000006a01000000000000000064037c01a6020000ab
                   02000000000000000072167401000000000000000000006a020000000000
                   000000640464057c01a6030000ab0300000000000000007d017c01a00300
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007d017c015300
-                38           0 RESUME                   0
+                61           0 RESUME                   0
                
-                49           2 LOAD_GLOBAL              1 (NULL + re)
+                72           2 LOAD_GLOBAL              1 (NULL + re)
                             14 LOAD_ATTR                1 (match)
                             24 LOAD_CONST               1 ('^(python|py)')
                             26 LOAD_FAST                1 (code)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE    22 (to 88)
                
-                50          44 LOAD_GLOBAL              1 (NULL + re)
+                73          44 LOAD_GLOBAL              1 (NULL + re)
                             56 LOAD_ATTR                2 (sub)
                             66 LOAD_CONST               1 ('^(python|py)')
                             68 LOAD_CONST               2 ('')
                             70 LOAD_FAST                1 (code)
                             72 PRECALL                  3
                             76 CALL                     3
                             86 STORE_FAST               1 (code)
                
-                51     >>   88 LOAD_GLOBAL              1 (NULL + re)
+                74     >>   88 LOAD_GLOBAL              1 (NULL + re)
                            100 LOAD_ATTR                1 (match)
                            110 LOAD_CONST               3 ('^`.*`$')
                            112 LOAD_FAST                1 (code)
                            114 PRECALL                  2
                            118 CALL                     2
                            128 POP_JUMP_FORWARD_IF_FALSE    22 (to 174)
                
-                52         130 LOAD_GLOBAL              1 (NULL + re)
+                75         130 LOAD_GLOBAL              1 (NULL + re)
                            142 LOAD_ATTR                2 (sub)
                            152 LOAD_CONST               4 ('^`(.*)`$')
                            154 LOAD_CONST               5 ('\\1')
                            156 LOAD_FAST                1 (code)
                            158 PRECALL                  3
                            162 CALL                     3
                            172 STORE_FAST               1 (code)
                
-                53     >>  174 LOAD_FAST                1 (code)
+                76     >>  174 LOAD_FAST                1 (code)
                            176 LOAD_METHOD              3 (strip)
                            198 PRECALL                  0
                            202 CALL                     0
                            212 STORE_FAST               1 (code)
                
-                54         214 LOAD_FAST                1 (code)
+                77         214 LOAD_FAST                1 (code)
                            216 RETURN_VALUE
                consts
                   '\n        Polish the code by removing the leading "python" or "py",          removing the imports and removing trailing spaces and new lines.\n\n        Args:\n            code (str): Code\n\n        Returns:\n            str: Polished code\n        '
                   '^(python|py)'
                   ''
                   '^`.*`$'
                   '^`(.*)`$'
                   '\\1'
                names      ('re', 'match', 'sub', 'strip')
                varnames   ('self', 'code')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_polish_code'
-               firstlineno 38
+               firstlineno 61
                lnotab 0x020b2a012c012a012c012801
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x970009007401000000000000000000006a0100000000000000007c01a6
                   010000ab0100000000000000000100640153002300740400000000000000
                   0000002400720401005900640253007700780359007701
-                56           0 RESUME                   0
+                79           0 RESUME                   0
                
-                57           2 NOP
+                88           2 NOP
                
-                58           4 LOAD_GLOBAL              1 (NULL + ast)
+                89           4 LOAD_GLOBAL              1 (NULL + ast)
                             16 LOAD_ATTR                1 (parse)
                             26 LOAD_FAST                1 (string)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-                59          44 LOAD_CONST               1 (True)
+                90          44 LOAD_CONST               1 (True)
                             46 RETURN_VALUE
                        >>   48 PUSH_EXC_INFO
                
-                60          50 LOAD_GLOBAL              4 (SyntaxError)
+                91          50 LOAD_GLOBAL              4 (SyntaxError)
                             62 CHECK_EXC_MATCH
                             64 POP_JUMP_FORWARD_IF_FALSE     4 (to 74)
                             66 POP_TOP
                
-                61          68 POP_EXCEPT
+                92          68 POP_EXCEPT
                             70 LOAD_CONST               2 (False)
                             72 RETURN_VALUE
                
-                60     >>   74 RERAISE                  0
+                91     >>   74 RERAISE                  0
                        >>   76 COPY                     3
                             78 POP_EXCEPT
                             80 RERAISE                  1
                ExceptionTable:
                  4 to 42 -> 48 [0]
                  48 to 66 -> 76 [1] lasti
                  74 to 74 -> 76 [1] lasti
                consts
-                  None
+                  '\n        Return True if it is valid python code.\n        Args:\n            string (str):\n\n        Returns (bool): True if Python Code otherwise False\n\n        '
                   True
                   False
                names      ('ast', 'parse', 'SyntaxError')
                varnames   ('self', 'string')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_is_python_code'
-               firstlineno 56
-               lnotab 0x0201020128010601120106ff
+               firstlineno 79
+               lnotab 0x0209020128010601120106ff
             '```'
             'response'
             'separator'
             code
                argcount  : 3
-               nlocals   : 5
-               stacksize : 10
+               nlocals   : 4
+               stacksize : 5
                flags     : 3
                code
-                  0x97007c017d037401000000000000000000006a01000000000000000074
-                  04000000000000000000009b0064017406000000000000000000009b0064
-                  027407000000000000000000006a04000000000000000064036404a60200
-                  00ab0200000000000000009b0064059d067c037400000000000000000000
-                  006a050000000000000000a6030000ab0300000000000000007d047c0472
-                  277c04a00600000000000000000000000000000000000000006406a60100
-                  00ab010000000000000000a0070000000000000000000000000000000000
-                  000000a6000000ab0000000000000000007d037411000000000000000000
-                  007c03a00900000000000000000000000000000000000000007c02a60100
-                  00ab010000000000000000a6010000ab01000000000000000064066b0400
-                  000000721b7c03a00900000000000000000000000000000000000000007c
-                  02a6010000ab0100000000000000006406190000000000000000007d037c
-                  00a00a00000000000000000000000000000000000000007c03a6010000ab
-                  0100000000000000007d037c00a00b000000000000000000000000000000
-                  00000000007c03a6010000ab010000000000000000730f74190000000000
-                  00000000006407a6010000ab01000000000000000082017c035300
-                63           0 RESUME                   0
+                  0x97007c017d037401000000000000000000007c03a00100000000000000
+                  000000000000000000000000007c02a6010000ab010000000000000000a6
+                  010000ab01000000000000000064016b0400000000721b7c03a001000000
+                  00000000000000000000000000000000007c02a6010000ab010000000000
+                  0000006401190000000000000000007d037c00a002000000000000000000
+                  00000000000000000000007c03a6010000ab0100000000000000007d037c
+                  00a00300000000000000000000000000000000000000007c03a6010000ab
+                  010000000000000000730f7409000000000000000000006402a6010000ab
+                  01000000000000000082017c035300
+                94           0 RESUME                   0
                
-                77           2 LOAD_FAST                1 (response)
+               108           2 LOAD_FAST                1 (response)
                              4 STORE_FAST               3 (code)
                
-                78           6 LOAD_GLOBAL              1 (NULL + re)
-                            18 LOAD_ATTR                1 (search)
+               109           6 LOAD_GLOBAL              1 (NULL + len)
+                            18 LOAD_FAST                3 (code)
+                            20 LOAD_METHOD              1 (split)
+                            42 LOAD_FAST                2 (separator)
+                            44 PRECALL                  1
+                            48 CALL                     1
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 LOAD_CONST               1 (1)
+                            74 COMPARE_OP               4 (>)
+                            80 POP_JUMP_FORWARD_IF_FALSE    27 (to 136)
+               
+               110          82 LOAD_FAST                3 (code)
+                            84 LOAD_METHOD              1 (split)
+                           106 LOAD_FAST                2 (separator)
+                           108 PRECALL                  1
+                           112 CALL                     1
+                           122 LOAD_CONST               1 (1)
+                           124 BINARY_SUBSCR
+                           134 STORE_FAST               3 (code)
                
-                79          28 LOAD_GLOBAL              4 (START_CODE_TAG)
-                            40 FORMAT_VALUE             0
-                            42 LOAD_CONST               1 ('(.*)(')
-                            44 LOAD_GLOBAL              6 (END_CODE_TAG)
-                            56 FORMAT_VALUE             0
-                            58 LOAD_CONST               2 ('|')
-                            60 LOAD_GLOBAL              7 (NULL + END_CODE_TAG)
-                            72 LOAD_ATTR                4 (replace)
-                            82 LOAD_CONST               3 ('<')
-                            84 LOAD_CONST               4 ('</')
-                            86 PRECALL                  2
-                            90 CALL                     2
-                           100 FORMAT_VALUE             0
-                           102 LOAD_CONST               5 (')')
-                           104 BUILD_STRING             6
-               
-                80         106 LOAD_FAST                3 (code)
-               
-                81         108 LOAD_GLOBAL              0 (re)
-                           120 LOAD_ATTR                5 (DOTALL)
-               
-                78         130 PRECALL                  3
-                           134 CALL                     3
-                           144 STORE_FAST               4 (match)
-               
-                83         146 LOAD_FAST                4 (match)
-                           148 POP_JUMP_FORWARD_IF_FALSE    39 (to 228)
-               
-                84         150 LOAD_FAST                4 (match)
-                           152 LOAD_METHOD              6 (group)
-                           174 LOAD_CONST               6 (1)
-                           176 PRECALL                  1
-                           180 CALL                     1
-                           190 LOAD_METHOD              7 (strip)
-                           212 PRECALL                  0
-                           216 CALL                     0
-                           226 STORE_FAST               3 (code)
-               
-                85     >>  228 LOAD_GLOBAL             17 (NULL + len)
-                           240 LOAD_FAST                3 (code)
-                           242 LOAD_METHOD              9 (split)
-                           264 LOAD_FAST                2 (separator)
-                           266 PRECALL                  1
-                           270 CALL                     1
-                           280 PRECALL                  1
-                           284 CALL                     1
-                           294 LOAD_CONST               6 (1)
-                           296 COMPARE_OP               4 (>)
-                           302 POP_JUMP_FORWARD_IF_FALSE    27 (to 358)
-               
-                86         304 LOAD_FAST                3 (code)
-                           306 LOAD_METHOD              9 (split)
-                           328 LOAD_FAST                2 (separator)
-                           330 PRECALL                  1
-                           334 CALL                     1
-                           344 LOAD_CONST               6 (1)
-                           346 BINARY_SUBSCR
-                           356 STORE_FAST               3 (code)
-               
-                87     >>  358 LOAD_FAST                0 (self)
-                           360 LOAD_METHOD             10 (_polish_code)
-                           382 LOAD_FAST                3 (code)
-                           384 PRECALL                  1
-                           388 CALL                     1
-                           398 STORE_FAST               3 (code)
-               
-                88         400 LOAD_FAST                0 (self)
-                           402 LOAD_METHOD             11 (_is_python_code)
-                           424 LOAD_FAST                3 (code)
-                           426 PRECALL                  1
-                           430 CALL                     1
-                           440 POP_JUMP_FORWARD_IF_TRUE    15 (to 472)
-               
-                89         442 LOAD_GLOBAL             25 (NULL + NoCodeFoundError)
-                           454 LOAD_CONST               7 ('No code found in the response')
-                           456 PRECALL                  1
-                           460 CALL                     1
-                           470 RAISE_VARARGS            1
+               111     >>  136 LOAD_FAST                0 (self)
+                           138 LOAD_METHOD              2 (_polish_code)
+                           160 LOAD_FAST                3 (code)
+                           162 PRECALL                  1
+                           166 CALL                     1
+                           176 STORE_FAST               3 (code)
+               
+               112         178 LOAD_FAST                0 (self)
+                           180 LOAD_METHOD              3 (_is_python_code)
+                           202 LOAD_FAST                3 (code)
+                           204 PRECALL                  1
+                           208 CALL                     1
+                           218 POP_JUMP_FORWARD_IF_TRUE    15 (to 250)
+               
+               113         220 LOAD_GLOBAL              9 (NULL + NoCodeFoundError)
+                           232 LOAD_CONST               2 ('No code found in the response')
+                           234 PRECALL                  1
+                           238 CALL                     1
+                           248 RAISE_VARARGS            1
                
-                91     >>  472 LOAD_FAST                3 (code)
-                           474 RETURN_VALUE
+               115     >>  250 LOAD_FAST                3 (code)
+                           252 RETURN_VALUE
                consts
                   '\n        Extract the code from the response.\n\n        Args:\n            response (str): Response\n            separator (str, optional): Separator. Defaults to "```".\n\n        Raises:\n            NoCodeFoundError: No code found in the response\n\n        Returns:\n            str: Extracted code from the response\n        '
-                  '(.*)('
-                  '|'
-                  '<'
-                  '</'
-                  ')'
                   1
                   'No code found in the response'
-               names      ('re', 'search', 'START_CODE_TAG', 'END_CODE_TAG', 'replace', 'DOTALL', 'group', 'strip', 'len', 'split', '_polish_code', '_is_python_code', 'NoCodeFoundError')
-               varnames   ('self', 'response', 'separator', 'code', 'match')
+               names      ('len', 'split', '_polish_code', '_is_python_code', 'NoCodeFoundError')
+               varnames   ('self', 'response', 'separator', 'code')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_extract_code'
-               firstlineno 63
-               lnotab 0x020e040116014e01020116fd100504014e014c0136012a012a011e02
+               firstlineno 94
+               lnotab 0x020e04014c0136012a012a011e02
             ''
             'instruction'
             'value'
             'suffix'
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   008201
-                93           0 RESUME                   0
+               117           0 RESUME                   0
                
-               106           2 LOAD_GLOBAL              1 (NULL + MethodNotImplementedError)
+               130           2 LOAD_GLOBAL              1 (NULL + MethodNotImplementedError)
                             14 LOAD_CONST               1 ('Call method has not been implemented')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RAISE_VARARGS            1
                consts
-                  '\n        Execute the LLM with given prompt.\n\n        Args:\n            instruction (str): Prompt\n            value (str): Value\n            suffix (str, optional): Suffix. Defaults to "".\n\n        Raises:\n            MethodNotImplementedError: Call method has not been implemented\n        '
+                  '\n        Execute the LLM with given prompt.\n\n        Args:\n            instruction (Prompt): Prompt\n            value (str): Value\n            suffix (str, optional): Suffix. Defaults to "".\n\n        Raises:\n            MethodNotImplementedError: Call method has not been implemented\n        '
                   'Call method has not been implemented'
                names      ('MethodNotImplementedError',)
                varnames   ('self', 'instruction', 'value', 'suffix')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'call'
-               firstlineno 93
+               firstlineno 117
                lnotab 0x020d
             'prompt'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c00a0
                   0100000000000000000000000000000000000000007c017c026401ac02a6
                   030000ab030000000000000000a6010000ab0100000000000000005300
-               108           0 RESUME                   0
+               132           0 RESUME                   0
                
-               115           2 LOAD_FAST                0 (self)
+               139           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_extract_code)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_METHOD              1 (call)
                             50 LOAD_FAST                1 (instruction)
                             52 LOAD_FAST                2 (prompt)
                             54 LOAD_CONST               1 ('\n\nCode:\n')
                             56 KW_NAMES                 2
@@ -591,295 +564,309 @@
                   ('suffix',)
                names      ('_extract_code', 'call')
                varnames   ('self', 'instruction', 'prompt')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'generate_code'
-               firstlineno 108
+               firstlineno 132
                lnotab 0x0207
             ('```',)
             ('',)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'last_prompt', 'Optional', 'str', '__annotations__', 'property', 'type', '_polish_code', '_is_python_code', '_extract_code', 'abstractmethod', 'call', 'generate_code')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'last_prompt', 'Optional', 'str', '__annotations__', 'bool', 'is_pandasai_llm', 'property', 'type', '_polish_code', '_is_python_code', '_extract_code', 'abstractmethod', 'Prompt', 'call', 'generate_code')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
          name       'LLM'
-         firstlineno 20
-         lnotab 0x0c0104021a0202010aff0e01020c10120607161e020118ff0e01020e
+         firstlineno 34
+         lnotab
+            0x0c0104021a020c0902010aff0e01020c1012060f1617020118ff0e0102
+            0e
       'LLM'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02550064015a036504650564023c00000064035a
             066507650564043c00000064055a086509650564063c00000064075a0a65
             07650564083c00000064035a0b6507650564093c000000640a5a0c650765
             05640b3c000000640c5a0d650e6504190000000000000000006505640d3c
-            000000640e84005a0f6510640f6511650465126602190000000000000000
-            00660264108404a6000000ab0000000000000000005a1364116504640f65
-            046604641284045a1464136504640f65046604641484045a15640c5300
-         118           0 RESUME                   0
+            000000640c5a0f650e6504190000000000000000006505640e3c00000064
+            0f84005a1065116410651265046513660219000000000000000000660264
+            118404a6000000ab0000000000000000005a146412650464106504660464
+            1384045a1564146504641065046604641584045a16640c5300
+         142           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseOpenAI')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         119          12 LOAD_CONST               1 ('Base class to implement a new OpenAI LLM')
+         143          12 LOAD_CONST               1 ('Base class to implement a new OpenAI LLM\n    LLM base class, this class is extended to be used with OpenAI API.\n\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         121          16 LOAD_NAME                4 (str)
+         148          16 LOAD_NAME                4 (str)
                       18 LOAD_NAME                5 (__annotations__)
                       20 LOAD_CONST               2 ('api_token')
                       22 STORE_SUBSCR
          
-         122          26 LOAD_CONST               3 (0)
+         149          26 LOAD_CONST               3 (0)
                       28 STORE_NAME               6 (temperature)
                       30 LOAD_NAME                7 (float)
                       32 LOAD_NAME                5 (__annotations__)
                       34 LOAD_CONST               4 ('temperature')
                       36 STORE_SUBSCR
          
-         123          40 LOAD_CONST               5 (512)
+         150          40 LOAD_CONST               5 (512)
                       42 STORE_NAME               8 (max_tokens)
                       44 LOAD_NAME                9 (int)
                       46 LOAD_NAME                5 (__annotations__)
                       48 LOAD_CONST               6 ('max_tokens')
                       50 STORE_SUBSCR
          
-         124          54 LOAD_CONST               7 (1)
+         151          54 LOAD_CONST               7 (1)
                       56 STORE_NAME              10 (top_p)
                       58 LOAD_NAME                7 (float)
                       60 LOAD_NAME                5 (__annotations__)
                       62 LOAD_CONST               8 ('top_p')
                       64 STORE_SUBSCR
          
-         125          68 LOAD_CONST               3 (0)
+         152          68 LOAD_CONST               3 (0)
                       70 STORE_NAME              11 (frequency_penalty)
                       72 LOAD_NAME                7 (float)
                       74 LOAD_NAME                5 (__annotations__)
                       76 LOAD_CONST               9 ('frequency_penalty')
                       78 STORE_SUBSCR
          
-         126          82 LOAD_CONST              10 (0.6)
+         153          82 LOAD_CONST              10 (0.6)
                       84 STORE_NAME              12 (presence_penalty)
                       86 LOAD_NAME                7 (float)
                       88 LOAD_NAME                5 (__annotations__)
                       90 LOAD_CONST              11 ('presence_penalty')
                       92 STORE_SUBSCR
          
-         127          96 LOAD_CONST              12 (None)
+         154          96 LOAD_CONST              12 (None)
                       98 STORE_NAME              13 (stop)
                      100 LOAD_NAME               14 (Optional)
                      102 LOAD_NAME                4 (str)
                      104 BINARY_SUBSCR
                      114 LOAD_NAME                5 (__annotations__)
                      116 LOAD_CONST              13 ('stop')
                      118 STORE_SUBSCR
          
-         129         122 LOAD_CONST              14 (<code object _set_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 129>)
-                     124 MAKE_FUNCTION            0
-                     126 STORE_NAME              15 (_set_params)
-         
-         145         128 LOAD_NAME               16 (property)
-         
-         146         130 LOAD_CONST              15 ('return')
-                     132 LOAD_NAME               17 (Dict)
-                     134 LOAD_NAME                4 (str)
-                     136 LOAD_NAME               18 (Any)
-                     138 BUILD_TUPLE              2
-                     140 BINARY_SUBSCR
-                     150 BUILD_TUPLE              2
-                     152 LOAD_CONST              16 (<code object _default_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 145>)
-                     154 MAKE_FUNCTION            4 (annotations)
+         156         122 LOAD_CONST              12 (None)
+                     124 STORE_NAME              15 (openai_proxy)
+                     126 LOAD_NAME               14 (Optional)
+                     128 LOAD_NAME                4 (str)
+                     130 BINARY_SUBSCR
+                     140 LOAD_NAME                5 (__annotations__)
+                     142 LOAD_CONST              14 ('openai_proxy')
+                     144 STORE_SUBSCR
          
-         145         156 PRECALL                  0
-                     160 CALL                     0
+         158         148 LOAD_CONST              15 (<code object _set_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 158>)
+                     150 MAKE_FUNCTION            0
+                     152 STORE_NAME              16 (_set_params)
          
-         146         170 STORE_NAME              19 (_default_params)
+         184         154 LOAD_NAME               17 (property)
          
-         156         172 LOAD_CONST              17 ('prompt')
-                     174 LOAD_NAME                4 (str)
-                     176 LOAD_CONST              15 ('return')
-                     178 LOAD_NAME                4 (str)
-                     180 BUILD_TUPLE              4
-                     182 LOAD_CONST              18 (<code object completion, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 156>)
-                     184 MAKE_FUNCTION            4 (annotations)
-                     186 STORE_NAME              20 (completion)
-         
-         175         188 LOAD_CONST              19 ('value')
-                     190 LOAD_NAME                4 (str)
-                     192 LOAD_CONST              15 ('return')
-                     194 LOAD_NAME                4 (str)
-                     196 BUILD_TUPLE              4
-                     198 LOAD_CONST              20 (<code object chat_completion, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 175>)
-                     200 MAKE_FUNCTION            4 (annotations)
-                     202 STORE_NAME              21 (chat_completion)
-                     204 LOAD_CONST              12 (None)
-                     206 RETURN_VALUE
+         185         156 LOAD_CONST              16 ('return')
+                     158 LOAD_NAME               18 (Dict)
+                     160 LOAD_NAME                4 (str)
+                     162 LOAD_NAME               19 (Any)
+                     164 BUILD_TUPLE              2
+                     166 BINARY_SUBSCR
+                     176 BUILD_TUPLE              2
+                     178 LOAD_CONST              17 (<code object _default_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 184>)
+                     180 MAKE_FUNCTION            4 (annotations)
+         
+         184         182 PRECALL                  0
+                     186 CALL                     0
+         
+         185         196 STORE_NAME              20 (_default_params)
+         
+         201         198 LOAD_CONST              18 ('prompt')
+                     200 LOAD_NAME                4 (str)
+                     202 LOAD_CONST              16 ('return')
+                     204 LOAD_NAME                4 (str)
+                     206 BUILD_TUPLE              4
+                     208 LOAD_CONST              19 (<code object completion, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 201>)
+                     210 MAKE_FUNCTION            4 (annotations)
+                     212 STORE_NAME              21 (completion)
+         
+         220         214 LOAD_CONST              20 ('value')
+                     216 LOAD_NAME                4 (str)
+                     218 LOAD_CONST              16 ('return')
+                     220 LOAD_NAME                4 (str)
+                     222 BUILD_TUPLE              4
+                     224 LOAD_CONST              21 (<code object chat_completion, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 220>)
+                     226 MAKE_FUNCTION            4 (annotations)
+                     228 STORE_NAME              22 (chat_completion)
+                     230 LOAD_CONST              12 (None)
+                     232 RETURN_VALUE
          consts
             'BaseOpenAI'
-            'Base class to implement a new OpenAI LLM'
+            'Base class to implement a new OpenAI LLM\n    LLM base class, this class is extended to be used with OpenAI API.\n\n    '
             'api_token'
             0
             'temperature'
             512
             'max_tokens'
             1
             'top_p'
             'frequency_penalty'
             0.6
             'presence_penalty'
             None
             'stop'
+            'openai_proxy'
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 6
                flags     : 11
                code
                   0x970067006401a2017d027c01a000000000000000000000000000000000
                   0000000000a6000000ab00000000000000000044005d1a5c0200007d037d
                   047c037c02760072117403000000000000000000007c007c037c04a60300
-                  00ab03000000000000000001008c1b64005300
-               129           0 RESUME                   0
+                  00ab03000000000000000001008c1b64025300
+               158           0 RESUME                   0
                
-               130           2 BUILD_LIST               0
+               169           2 BUILD_LIST               0
                              4 LOAD_CONST               1 (('model', 'engine', 'deployment_id', 'temperature', 'max_tokens', 'top_p', 'frequency_penalty', 'presence_penalty', 'stop'))
                              6 LIST_EXTEND              1
                              8 STORE_FAST               2 (valid_params)
                
-               141          10 LOAD_FAST                1 (kwargs)
+               180          10 LOAD_FAST                1 (kwargs)
                             12 LOAD_METHOD              0 (items)
                             34 PRECALL                  0
                             38 CALL                     0
                             48 GET_ITER
                        >>   50 FOR_ITER                26 (to 104)
                             52 UNPACK_SEQUENCE          2
                             56 STORE_FAST               3 (key)
                             58 STORE_FAST               4 (value)
                
-               142          60 LOAD_FAST                3 (key)
+               181          60 LOAD_FAST                3 (key)
                             62 LOAD_FAST                2 (valid_params)
                             64 CONTAINS_OP              0
                             66 POP_JUMP_FORWARD_IF_FALSE    17 (to 102)
                
-               143          68 LOAD_GLOBAL              3 (NULL + setattr)
+               182          68 LOAD_GLOBAL              3 (NULL + setattr)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_FAST                3 (key)
                             84 LOAD_FAST                4 (value)
                             86 PRECALL                  3
                             90 CALL                     3
                            100 POP_TOP
                        >>  102 JUMP_BACKWARD           27 (to 50)
                
-               141     >>  104 LOAD_CONST               0 (None)
+               180     >>  104 LOAD_CONST               2 (None)
                            106 RETURN_VALUE
                consts
-                  None
+                  '\n        Set Parameters\n        Args:\n            **kwargs: ["model", "engine", "deployment_id", "temperature","max_tokens",\n            "top_p", "frequency_penalty", "presence_penalty", "stop", ]\n\n        Returns: None\n\n        '
                   ('model', 'engine', 'deployment_id', 'temperature', 'max_tokens', 'top_p', 'frequency_penalty', 'presence_penalty', 'stop')
+                  None
                names      ('items', 'setattr')
                varnames   ('self', 'kwargs', 'valid_params', 'key', 'value')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_set_params'
-               firstlineno 129
-               lnotab 0x0201080b3201080124fe
+               firstlineno 158
+               lnotab 0x020b080b3201080124fe
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a0100000000000000007c006a
                   0200000000000000007c006a0300000000000000007c006a040000000000
                   00000064019c055300
-               145           0 RESUME                   0
+               184           0 RESUME                   0
                
-               149           2 LOAD_FAST                0 (self)
+               194           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (temperature)
                
-               150          14 LOAD_FAST                0 (self)
+               195          14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (max_tokens)
                
-               151          26 LOAD_FAST                0 (self)
+               196          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (top_p)
                
-               152          38 LOAD_FAST                0 (self)
+               197          38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                3 (frequency_penalty)
                
-               153          50 LOAD_FAST                0 (self)
+               198          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (presence_penalty)
                
-               148          62 LOAD_CONST               1 (('temperature', 'max_tokens', 'top_p', 'frequency_penalty', 'presence_penalty'))
+               193          62 LOAD_CONST               1 (('temperature', 'max_tokens', 'top_p', 'frequency_penalty', 'presence_penalty'))
                             64 BUILD_CONST_KEY_MAP      5
                             66 RETURN_VALUE
                consts
-                  'Get the default parameters for calling OpenAI API'
+                  '\n        Get the default parameters for calling OpenAI API\n\n        Returns (Dict): A dict of OpenAi API parameters\n\n        '
                   ('temperature', 'max_tokens', 'top_p', 'frequency_penalty', 'presence_penalty')
                names      ('temperature', 'max_tokens', 'top_p', 'frequency_penalty', 'presence_penalty')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_default_params'
-               firstlineno 145
-               lnotab 0x02040c010c010c010c010cfb
+               firstlineno 184
+               lnotab 0x020a0c010c010c010c010cfb
             'prompt'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x970069007c006a000000000000000000a50164017c016901a5017d027c
                   006a010000000000000000810b7c006a01000000000000000067017c0264
                   033c0000007405000000000000000000006a0300000000000000006a0400
                   00000000000000640769007c02a4018e017d037c03640419000000000000
                   0000006405190000000000000000006406190000000000000000005300
-               156           0 RESUME                   0
+               201           0 RESUME                   0
                
-               166           2 BUILD_MAP                0
+               211           2 BUILD_MAP                0
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (_default_params)
                             16 DICT_UPDATE              1
                             18 LOAD_CONST               1 ('prompt')
                             20 LOAD_FAST                1 (prompt)
                             22 BUILD_MAP                1
                             24 DICT_UPDATE              1
                             26 STORE_FAST               2 (params)
                
-               168          28 LOAD_FAST                0 (self)
+               213          28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                1 (stop)
                             40 POP_JUMP_FORWARD_IF_NONE    11 (to 64)
                
-               169          42 LOAD_FAST                0 (self)
+               214          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                1 (stop)
                             54 BUILD_LIST               1
                             56 LOAD_FAST                2 (params)
                             58 LOAD_CONST               3 ('stop')
                             60 STORE_SUBSCR
                
-               171     >>   64 LOAD_GLOBAL              5 (NULL + openai)
+               216     >>   64 LOAD_GLOBAL              5 (NULL + openai)
                             76 LOAD_ATTR                3 (Completion)
                             86 LOAD_ATTR                4 (create)
                             96 LOAD_CONST               7 (())
                             98 BUILD_MAP                0
                            100 LOAD_FAST                2 (params)
                            102 DICT_MERGE               1
                            104 CALL_FUNCTION_EX         1
                            106 STORE_FAST               3 (response)
                
-               173         108 LOAD_FAST                3 (response)
+               218         108 LOAD_FAST                3 (response)
                            110 LOAD_CONST               4 ('choices')
                            112 BINARY_SUBSCR
                            122 LOAD_CONST               5 (0)
                            124 BINARY_SUBSCR
                            134 LOAD_CONST               6 ('text')
                            136 BINARY_SUBSCR
                            146 RETURN_VALUE
@@ -894,75 +881,75 @@
                   ()
                names      ('_default_params', 'stop', 'openai', 'Completion', 'create')
                varnames   ('self', 'prompt', 'params', 'response')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'completion'
-               firstlineno 156
+               firstlineno 201
                lnotab 0x020a1a020e0116022c02
             'value'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x970069007c006a000000000000000000a501640164027c0164039c0267
                   016901a5017d027c006a010000000000000000810b7c006a010000000000
                   00000067017c0264053c0000007405000000000000000000006a03000000
                   00000000006a040000000000000000640a69007c02a4018e017d037c0364
                   061900000000000000000064071900000000000000000064081900000000
                   00000000006409190000000000000000005300
-               175           0 RESUME                   0
+               220           0 RESUME                   0
                
-               185           2 BUILD_MAP                0
+               230           2 BUILD_MAP                0
                
-               186           4 LOAD_FAST                0 (self)
+               231           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (_default_params)
                
-               185          16 DICT_UPDATE              1
+               230          16 DICT_UPDATE              1
                
-               187          18 LOAD_CONST               1 ('messages')
+               232          18 LOAD_CONST               1 ('messages')
                
-               189          20 LOAD_CONST               2 ('system')
+               234          20 LOAD_CONST               2 ('system')
                
-               190          22 LOAD_FAST                1 (value)
+               235          22 LOAD_FAST                1 (value)
                
-               188          24 LOAD_CONST               3 (('role', 'content'))
+               233          24 LOAD_CONST               3 (('role', 'content'))
                             26 BUILD_CONST_KEY_MAP      2
                
-               187          28 BUILD_LIST               1
+               232          28 BUILD_LIST               1
                
-               185          30 BUILD_MAP                1
+               230          30 BUILD_MAP                1
                             32 DICT_UPDATE              1
                             34 STORE_FAST               2 (params)
                
-               195          36 LOAD_FAST                0 (self)
+               240          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                1 (stop)
                             48 POP_JUMP_FORWARD_IF_NONE    11 (to 72)
                
-               196          50 LOAD_FAST                0 (self)
+               241          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                1 (stop)
                             62 BUILD_LIST               1
                             64 LOAD_FAST                2 (params)
                             66 LOAD_CONST               5 ('stop')
                             68 STORE_SUBSCR
                
-               199     >>   72 LOAD_GLOBAL              5 (NULL + openai)
+               243     >>   72 LOAD_GLOBAL              5 (NULL + openai)
                             84 LOAD_ATTR                3 (ChatCompletion)
                             94 LOAD_ATTR                4 (create)
                            104 LOAD_CONST              10 (())
                            106 BUILD_MAP                0
                            108 LOAD_FAST                2 (params)
                            110 DICT_MERGE               1
                            112 CALL_FUNCTION_EX         1
                            114 STORE_FAST               3 (response)
                
-               201         116 LOAD_FAST                3 (response)
+               245         116 LOAD_FAST                3 (response)
                            118 LOAD_CONST               6 ('choices')
                            120 BINARY_SUBSCR
                            130 LOAD_CONST               7 (0)
                            132 BINARY_SUBSCR
                            142 LOAD_CONST               8 ('message')
                            144 BINARY_SUBSCR
                            154 LOAD_CONST               9 ('content')
@@ -982,550 +969,639 @@
                   ()
                names      ('_default_params', 'stop', 'openai', 'ChatCompletion', 'create')
                varnames   ('self', 'value', 'params', 'response')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'chat_completion'
-               firstlineno 175
-               lnotab 0x020a02010cff02020202020102fe04ff02fe060a0e0116032c02
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__annotations__', 'temperature', 'float', 'max_tokens', 'int', 'top_p', 'frequency_penalty', 'presence_penalty', 'stop', 'Optional', '_set_params', 'property', 'Dict', 'Any', '_default_params', 'completion', 'chat_completion')
+               firstlineno 220
+               lnotab 0x020a02010cff02020202020102fe04ff02fe060a0e0116022c02
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__annotations__', 'temperature', 'float', 'max_tokens', 'int', 'top_p', 'frequency_penalty', 'presence_penalty', 'stop', 'Optional', 'openai_proxy', '_set_params', 'property', 'Dict', 'Any', '_default_params', 'completion', 'chat_completion')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
          name       'BaseOpenAI'
-         firstlineno 118
+         firstlineno 142
          lnotab
-            0x0c0104020a010e010e010e010e010e011a02061002011aff0e01020a10
-            13
+            0x0c0104050a010e010e010e010e010e011a021a02061a02011aff0e0102
+            101013
       'BaseOpenAI'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02550064015a0364025a04650565061900000000
             0000000000650764033c0000006506650764043c00000064055a08650665
             0764063c00000064075a09650a650764083c000000650b64096506660264
             0a8404a6000000ab0000000000000000005a0c640b84005a0d6411640d65
-            06640e6506640f6506640965066608641084055a0e64025300
-         204           0 RESUME                   0
+            0e640e6506640f6506640965066608641084055a0f64025300
+         248           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('HuggingFaceLLM')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         205          12 LOAD_CONST               1 ('Base class to implement a new Hugging Face LLM.')
+         249          12 LOAD_CONST               1 ('Base class to implement a new Hugging Face LLM.\n\n    LLM base class is extended to be used with HuggingFace LLM Modes APIs\n\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         207          16 LOAD_CONST               2 (None)
+         255          16 LOAD_CONST               2 (None)
                       18 STORE_NAME               4 (last_prompt)
                       20 LOAD_NAME                5 (Optional)
                       22 LOAD_NAME                6 (str)
                       24 BINARY_SUBSCR
                       34 LOAD_NAME                7 (__annotations__)
                       36 LOAD_CONST               3 ('last_prompt')
                       38 STORE_SUBSCR
          
-         208          42 LOAD_NAME                6 (str)
+         256          42 LOAD_NAME                6 (str)
                       44 LOAD_NAME                7 (__annotations__)
                       46 LOAD_CONST               4 ('api_token')
                       48 STORE_SUBSCR
          
-         209          52 LOAD_CONST               5 ('https://api-inference.huggingface.co/models/')
+         257          52 LOAD_CONST               5 ('https://api-inference.huggingface.co/models/')
                       54 STORE_NAME               8 (_api_url)
                       56 LOAD_NAME                6 (str)
                       58 LOAD_NAME                7 (__annotations__)
                       60 LOAD_CONST               6 ('_api_url')
                       62 STORE_SUBSCR
          
-         210          66 LOAD_CONST               7 (3)
+         258          66 LOAD_CONST               7 (3)
                       68 STORE_NAME               9 (_max_retries)
                       70 LOAD_NAME               10 (int)
                       72 LOAD_NAME                7 (__annotations__)
                       74 LOAD_CONST               8 ('_max_retries')
                       76 STORE_SUBSCR
          
-         212          80 LOAD_NAME               11 (property)
+         260          80 LOAD_NAME               11 (property)
          
-         213          82 LOAD_CONST               9 ('return')
+         261          82 LOAD_CONST               9 ('return')
                       84 LOAD_NAME                6 (str)
                       86 BUILD_TUPLE              2
-                      88 LOAD_CONST              10 (<code object type, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 212>)
+                      88 LOAD_CONST              10 (<code object type, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 260>)
                       90 MAKE_FUNCTION            4 (annotations)
          
-         212          92 PRECALL                  0
+         260          92 PRECALL                  0
                       96 CALL                     0
          
-         213         106 STORE_NAME              12 (type)
+         261         106 STORE_NAME              12 (type)
          
-         216         108 LOAD_CONST              11 (<code object query, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 216>)
+         264         108 LOAD_CONST              11 (<code object query, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 264>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              13 (query)
          
-         227         114 LOAD_CONST              17 (('',))
+         282         114 LOAD_CONST              17 (('',))
                      116 LOAD_CONST              13 ('instruction')
-                     118 LOAD_NAME                6 (str)
+                     118 LOAD_NAME               14 (Prompt)
                      120 LOAD_CONST              14 ('value')
                      122 LOAD_NAME                6 (str)
                      124 LOAD_CONST              15 ('suffix')
                      126 LOAD_NAME                6 (str)
                      128 LOAD_CONST               9 ('return')
                      130 LOAD_NAME                6 (str)
                      132 BUILD_TUPLE              8
-                     134 LOAD_CONST              16 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 227>)
+                     134 LOAD_CONST              16 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 282>)
                      136 MAKE_FUNCTION            5 (defaults, annotations)
-                     138 STORE_NAME              14 (call)
+                     138 STORE_NAME              15 (call)
                      140 LOAD_CONST               2 (None)
                      142 RETURN_VALUE
          consts
             'HuggingFaceLLM'
-            'Base class to implement a new Hugging Face LLM.'
+            'Base class to implement a new Hugging Face LLM.\n\n    LLM base class is extended to be used with HuggingFace LLM Modes APIs\n\n    '
             None
             'last_prompt'
             'api_token'
             'https://api-inference.huggingface.co/models/'
             '_api_url'
             3
             '_max_retries'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064015300
-               212           0 RESUME                   0
+               260           0 RESUME                   0
                
-               214           2 LOAD_CONST               1 ('huggingface-llm')
+               262           2 LOAD_CONST               1 ('huggingface-llm')
                              4 RETURN_VALUE
                consts
                   None
                   'huggingface-llm'
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'type'
-               firstlineno 212
+               firstlineno 260
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
                   0x9700640164027c006a0000000000000000009b009d0269017d02740300
                   0000000000000000006a0200000000000000007c006a0300000000000000
                   007c027c016403ac04a6040000ab0400000000000000007d037c03a00400
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000006405190000000000000000006406190000000000000000005300
-               216           0 RESUME                   0
+               264           0 RESUME                   0
                
-               219           2 LOAD_CONST               1 ('Authorization')
+               274           2 LOAD_CONST               1 ('Authorization')
                              4 LOAD_CONST               2 ('Bearer ')
                              6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (api_token)
                             18 FORMAT_VALUE             0
                             20 BUILD_STRING             2
                             22 BUILD_MAP                1
                             24 STORE_FAST               2 (headers)
                
-               221          26 LOAD_GLOBAL              3 (NULL + requests)
+               276          26 LOAD_GLOBAL              3 (NULL + requests)
                             38 LOAD_ATTR                2 (post)
                
-               222          48 LOAD_FAST                0 (self)
+               277          48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                3 (_api_url)
                             60 LOAD_FAST                2 (headers)
                             62 LOAD_FAST                1 (payload)
                             64 LOAD_CONST               3 (60)
                
-               221          66 KW_NAMES                 4
+               276          66 KW_NAMES                 4
                             68 PRECALL                  4
                             72 CALL                     4
                             82 STORE_FAST               3 (response)
                
-               225          84 LOAD_FAST                3 (response)
+               280          84 LOAD_FAST                3 (response)
                             86 LOAD_METHOD              4 (json)
                            108 PRECALL                  0
                            112 CALL                     0
                            122 LOAD_CONST               5 (0)
                            124 BINARY_SUBSCR
                            134 LOAD_CONST               6 ('generated_text')
                            136 BINARY_SUBSCR
                            146 RETURN_VALUE
                consts
-                  'Query the API'
+                  '\n        Query the HF API\n        Args:\n            payload: A JSON form payload\n\n        Returns: Generated Response\n\n        '
                   'Authorization'
                   'Bearer '
                   60
                   ('headers', 'json', 'timeout')
                   0
                   'generated_text'
                names      ('api_token', 'requests', 'post', '_api_url', 'json')
                varnames   ('self', 'payload', 'headers', 'response')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'query'
-               firstlineno 216
-               lnotab 0x02031802160112ff1204
+               firstlineno 264
+               lnotab 0x020a1802160112ff1204
             ''
             'instruction'
             'value'
             'suffix'
             code
                argcount  : 4
-               nlocals   : 8
+               nlocals   : 9
                stacksize : 5
                flags     : 3
                code
-                  0x97007c017c027a0000007c037a0000007d047401000000000000000000
-                  007c006a010000000000000000a6010000ab01000000000000000044005d
-                  367d057c00a002000000000000000000000000000000000000000064017c
-                  046901a6010000ab0100000000000000007d067c067d047c06a003000000
+                  0x97007401000000000000000000007c01a6010000ab0100000000000000
+                  007d047c047c027a0000007c037a0000007d057403000000000000000000
+                  007c006a020000000000000000a6010000ab01000000000000000044005d
+                  367d067c00a003000000000000000000000000000000000000000064017c
+                  056901a6010000ab0100000000000000007d077c077d057c07a004000000
                   00000000000000000000000000000000006402a6010000ab010000000000
-                  00000064036b0500000000720201006e018c377c06a00400000000000000
-                  000000000000000000000000007c017c027a0000007c037a0000006404a6
-                  020000ab0200000000000000007d077c075300
-               227           0 RESUME                   0
-               
-               230           2 LOAD_FAST                1 (instruction)
-                             4 LOAD_FAST                2 (value)
-                             6 BINARY_OP                0 (+)
-                            10 LOAD_FAST                3 (suffix)
-                            12 BINARY_OP                0 (+)
-                            16 STORE_FAST               4 (payload)
-               
-               234          18 LOAD_GLOBAL              1 (NULL + range)
-                            30 LOAD_FAST                0 (self)
-                            32 LOAD_ATTR                1 (_max_retries)
-                            42 PRECALL                  1
-                            46 CALL                     1
-                            56 GET_ITER
-                       >>   58 FOR_ITER                54 (to 168)
-                            60 STORE_FAST               5 (_i)
-               
-               235          62 LOAD_FAST                0 (self)
-                            64 LOAD_METHOD              2 (query)
-                            86 LOAD_CONST               1 ('inputs')
-                            88 LOAD_FAST                4 (payload)
-                            90 BUILD_MAP                1
-                            92 PRECALL                  1
-                            96 CALL                     1
-                           106 STORE_FAST               6 (response)
-               
-               236         108 LOAD_FAST                6 (response)
-                           110 STORE_FAST               4 (payload)
-               
-               237         112 LOAD_FAST                6 (response)
-                           114 LOAD_METHOD              3 (count)
-                           136 LOAD_CONST               2 ('<endCode>')
-                           138 PRECALL                  1
-                           142 CALL                     1
-                           152 LOAD_CONST               3 (2)
-                           154 COMPARE_OP               5 (>=)
-                           160 POP_JUMP_FORWARD_IF_FALSE     2 (to 166)
-               
-               238         162 POP_TOP
-                           164 JUMP_FORWARD             1 (to 168)
-               
-               237     >>  166 JUMP_BACKWARD           55 (to 58)
-               
-               241     >>  168 LOAD_FAST                6 (response)
-                           170 LOAD_METHOD              4 (replace)
-                           192 LOAD_FAST                1 (instruction)
-                           194 LOAD_FAST                2 (value)
-                           196 BINARY_OP                0 (+)
-                           200 LOAD_FAST                3 (suffix)
-                           202 BINARY_OP                0 (+)
-                           206 LOAD_CONST               4 ('')
-                           208 PRECALL                  2
-                           212 CALL                     2
-                           222 STORE_FAST               7 (output)
+                  00000064036b0500000000720201006e018c377c07a00500000000000000
+                  000000000000000000000000007c047c027a0000007c037a0000006404a6
+                  020000ab0200000000000000007d087c085300
+               282           0 RESUME                   0
+               
+               294           2 LOAD_GLOBAL              1 (NULL + str)
+                            14 LOAD_FAST                1 (instruction)
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 STORE_FAST               4 (prompt)
                
-               242         224 LOAD_FAST                7 (output)
-                           226 RETURN_VALUE
+               295          32 LOAD_FAST                4 (prompt)
+                            34 LOAD_FAST                2 (value)
+                            36 BINARY_OP                0 (+)
+                            40 LOAD_FAST                3 (suffix)
+                            42 BINARY_OP                0 (+)
+                            46 STORE_FAST               5 (payload)
+               
+               299          48 LOAD_GLOBAL              3 (NULL + range)
+                            60 LOAD_FAST                0 (self)
+                            62 LOAD_ATTR                2 (_max_retries)
+                            72 PRECALL                  1
+                            76 CALL                     1
+                            86 GET_ITER
+                       >>   88 FOR_ITER                54 (to 198)
+                            90 STORE_FAST               6 (_i)
+               
+               300          92 LOAD_FAST                0 (self)
+                            94 LOAD_METHOD              3 (query)
+                           116 LOAD_CONST               1 ('inputs')
+                           118 LOAD_FAST                5 (payload)
+                           120 BUILD_MAP                1
+                           122 PRECALL                  1
+                           126 CALL                     1
+                           136 STORE_FAST               7 (response)
+               
+               301         138 LOAD_FAST                7 (response)
+                           140 STORE_FAST               5 (payload)
+               
+               302         142 LOAD_FAST                7 (response)
+                           144 LOAD_METHOD              4 (count)
+                           166 LOAD_CONST               2 ('<endCode>')
+                           168 PRECALL                  1
+                           172 CALL                     1
+                           182 LOAD_CONST               3 (2)
+                           184 COMPARE_OP               5 (>=)
+                           190 POP_JUMP_FORWARD_IF_FALSE     2 (to 196)
+               
+               303         192 POP_TOP
+                           194 JUMP_FORWARD             1 (to 198)
+               
+               302     >>  196 JUMP_BACKWARD           55 (to 88)
+               
+               306     >>  198 LOAD_FAST                7 (response)
+                           200 LOAD_METHOD              5 (replace)
+                           222 LOAD_FAST                4 (prompt)
+                           224 LOAD_FAST                2 (value)
+                           226 BINARY_OP                0 (+)
+                           230 LOAD_FAST                3 (suffix)
+                           232 BINARY_OP                0 (+)
+                           236 LOAD_CONST               4 ('')
+                           238 PRECALL                  2
+                           242 CALL                     2
+                           252 STORE_FAST               8 (output)
+               
+               307         254 LOAD_FAST                8 (output)
+                           256 RETURN_VALUE
                consts
-                  'Call the LLM'
+                  '\n        A call method of HuggingFaceLLM class.\n        Args:\n            instruction (object): A prompt object\n            value (str):\n            suffix (str):\n\n        Returns (str): A string response\n\n        '
                   'inputs'
                   '<endCode>'
                   2
                   ''
-               names      ('range', '_max_retries', 'query', 'count', 'replace')
-               varnames   ('self', 'instruction', 'value', 'suffix', 'payload', '_i', 'response', 'output')
+               names      ('str', 'range', '_max_retries', 'query', 'count', 'replace')
+               varnames   ('self', 'instruction', 'value', 'suffix', 'prompt', 'payload', '_i', 'response', 'output')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'call'
-               firstlineno 227
-               lnotab 0x020310042c012e010401320104ff02043801
+               firstlineno 282
+               lnotab 0x020c1e0110042c012e010401320104ff02043801
             ('',)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'last_prompt', 'Optional', 'str', '__annotations__', '_api_url', '_max_retries', 'int', 'property', 'type', 'query', 'call')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'last_prompt', 'Optional', 'str', '__annotations__', '_api_url', '_max_retries', 'int', 'property', 'type', 'query', 'Prompt', 'call')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
          name       'HuggingFaceLLM'
-         firstlineno 204
-         lnotab 0x0c0104021a010a010e010e0202010aff0e010203060b
+         firstlineno 248
+         lnotab 0x0c0104061a010a010e010e0202010aff0e0102030612
       'HuggingFaceLLM'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02550064015a036504650564023c00000064035a
             066507650819000000000000000000650564043c00000064055a09650765
-            0819000000000000000000650564063c00000064055a0a65076508190000
-            00000000000000650564073c00000064055a0b6507650c19000000000000
-            000000650564083c0000006409650d6602640a84045a0e640b84005a0f64
-            0c84005a10640d84005a116512640e650d640f650d660464108404a60000
-            00ab0000000000000000005a1364166412650d6413650d6414650d640f65
-            0d6608641584055a1464055300
-         245           0 RESUME                   0
+            0819000000000000000000650564063c00000064075a0a65076508190000
+            00000000000000650564083c00000064095a0b6507650c19000000000000
+            0000006505640a3c000000640b650d6602640c84045a0e640d650d640e65
+            0d6604640f84045a0f641084005a10641184005a11641284005a12651364
+            13650d6414650d660464158404a6000000ab0000000000000000005a1464
+            1c641765156418650d6419650d6414650d6608641a84055a16641b5300
+         310           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseGoogle')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         246          12 LOAD_CONST               1 ('Base class to implement a new Google LLM')
+         311          12 LOAD_CONST               1 ('Base class to implement a new Google LLM\n\n    LLM base class is extended to be used with Google Palm API.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         248          16 LOAD_NAME                4 (Any)
+         316          16 LOAD_NAME                4 (Any)
                       18 LOAD_NAME                5 (__annotations__)
                       20 LOAD_CONST               2 ('genai')
                       22 STORE_SUBSCR
          
-         249          26 LOAD_CONST               3 (0)
+         317          26 LOAD_CONST               3 (0)
                       28 STORE_NAME               6 (temperature)
                       30 LOAD_NAME                7 (Optional)
                       32 LOAD_NAME                8 (float)
                       34 BINARY_SUBSCR
                       44 LOAD_NAME                5 (__annotations__)
                       46 LOAD_CONST               4 ('temperature')
                       48 STORE_SUBSCR
          
-         250          52 LOAD_CONST               5 (None)
+         318          52 LOAD_CONST               5 (0.8)
                       54 STORE_NAME               9 (top_p)
                       56 LOAD_NAME                7 (Optional)
                       58 LOAD_NAME                8 (float)
                       60 BINARY_SUBSCR
                       70 LOAD_NAME                5 (__annotations__)
                       72 LOAD_CONST               6 ('top_p')
                       74 STORE_SUBSCR
          
-         251          78 LOAD_CONST               5 (None)
+         319          78 LOAD_CONST               7 (0.3)
                       80 STORE_NAME              10 (top_k)
                       82 LOAD_NAME                7 (Optional)
                       84 LOAD_NAME                8 (float)
                       86 BINARY_SUBSCR
                       96 LOAD_NAME                5 (__annotations__)
-                      98 LOAD_CONST               7 ('top_k')
+                      98 LOAD_CONST               8 ('top_k')
                      100 STORE_SUBSCR
          
-         252         104 LOAD_CONST               5 (None)
+         320         104 LOAD_CONST               9 (1000)
                      106 STORE_NAME              11 (max_output_tokens)
                      108 LOAD_NAME                7 (Optional)
                      110 LOAD_NAME               12 (int)
                      112 BINARY_SUBSCR
                      122 LOAD_NAME                5 (__annotations__)
-                     124 LOAD_CONST               8 ('max_output_tokens')
+                     124 LOAD_CONST              10 ('max_output_tokens')
                      126 STORE_SUBSCR
          
-         254         130 LOAD_CONST               9 ('api_key')
+         322         130 LOAD_CONST              11 ('api_key')
                      132 LOAD_NAME               13 (str)
                      134 BUILD_TUPLE              2
-                     136 LOAD_CONST              10 (<code object _configure, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 254>)
+                     136 LOAD_CONST              12 (<code object _configure, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 322>)
                      138 MAKE_FUNCTION            4 (annotations)
                      140 STORE_NAME              14 (_configure)
          
-         261         142 LOAD_CONST              11 (<code object _valid_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 261>)
-                     144 MAKE_FUNCTION            0
-                     146 STORE_NAME              15 (_valid_params)
-         
-         264         148 LOAD_CONST              12 (<code object _set_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 264>)
-                     150 MAKE_FUNCTION            0
-                     152 STORE_NAME              16 (_set_params)
+         341         142 LOAD_CONST              13 ('project_id')
+                     144 LOAD_NAME               13 (str)
+                     146 LOAD_CONST              14 ('location')
+                     148 LOAD_NAME               13 (str)
+                     150 BUILD_TUPLE              4
+                     152 LOAD_CONST              15 (<code object _configurevertexai, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 341>)
+                     154 MAKE_FUNCTION            4 (annotations)
+                     156 STORE_NAME              15 (_configurevertexai)
          
-         270         154 LOAD_CONST              13 (<code object _validate, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 270>)
-                     156 MAKE_FUNCTION            0
-                     158 STORE_NAME              17 (_validate)
-         
-         285         160 LOAD_NAME               18 (abstractmethod)
-         
-         286         162 LOAD_CONST              14 ('prompt')
-                     164 LOAD_NAME               13 (str)
-                     166 LOAD_CONST              15 ('return')
-                     168 LOAD_NAME               13 (str)
-                     170 BUILD_TUPLE              4
-                     172 LOAD_CONST              16 (<code object _generate_text, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 285>)
-                     174 MAKE_FUNCTION            4 (annotations)
-         
-         285         176 PRECALL                  0
-                     180 CALL                     0
-         
-         286         190 STORE_NAME              19 (_generate_text)
-         
-         298         192 LOAD_CONST              22 (('',))
-                     194 LOAD_CONST              18 ('instruction')
-                     196 LOAD_NAME               13 (str)
-                     198 LOAD_CONST              19 ('value')
-                     200 LOAD_NAME               13 (str)
-                     202 LOAD_CONST              20 ('suffix')
-                     204 LOAD_NAME               13 (str)
-                     206 LOAD_CONST              15 ('return')
-                     208 LOAD_NAME               13 (str)
-                     210 BUILD_TUPLE              8
-                     212 LOAD_CONST              21 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 298>)
-                     214 MAKE_FUNCTION            5 (defaults, annotations)
-                     216 STORE_NAME              20 (call)
-                     218 LOAD_CONST               5 (None)
-                     220 RETURN_VALUE
+         357         158 LOAD_CONST              16 (<code object _valid_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 357>)
+                     160 MAKE_FUNCTION            0
+                     162 STORE_NAME              16 (_valid_params)
+         
+         360         164 LOAD_CONST              17 (<code object _set_params, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 360>)
+                     166 MAKE_FUNCTION            0
+                     168 STORE_NAME              17 (_set_params)
+         
+         375         170 LOAD_CONST              18 (<code object _validate, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 375>)
+                     172 MAKE_FUNCTION            0
+                     174 STORE_NAME              18 (_validate)
+         
+         390         176 LOAD_NAME               19 (abstractmethod)
+         
+         391         178 LOAD_CONST              19 ('prompt')
+                     180 LOAD_NAME               13 (str)
+                     182 LOAD_CONST              20 ('return')
+                     184 LOAD_NAME               13 (str)
+                     186 BUILD_TUPLE              4
+                     188 LOAD_CONST              21 (<code object _generate_text, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 390>)
+                     190 MAKE_FUNCTION            4 (annotations)
+         
+         390         192 PRECALL                  0
+                     196 CALL                     0
+         
+         391         206 STORE_NAME              20 (_generate_text)
+         
+         403         208 LOAD_CONST              28 (('',))
+                     210 LOAD_CONST              23 ('instruction')
+                     212 LOAD_NAME               21 (Prompt)
+                     214 LOAD_CONST              24 ('value')
+                     216 LOAD_NAME               13 (str)
+                     218 LOAD_CONST              25 ('suffix')
+                     220 LOAD_NAME               13 (str)
+                     222 LOAD_CONST              20 ('return')
+                     224 LOAD_NAME               13 (str)
+                     226 BUILD_TUPLE              8
+                     228 LOAD_CONST              26 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\base.py", line 403>)
+                     230 MAKE_FUNCTION            5 (defaults, annotations)
+                     232 STORE_NAME              22 (call)
+                     234 LOAD_CONST              27 (None)
+                     236 RETURN_VALUE
          consts
             'BaseGoogle'
-            'Base class to implement a new Google LLM'
+            'Base class to implement a new Google LLM\n\n    LLM base class is extended to be used with Google Palm API.\n    '
             'genai'
             0
             'temperature'
-            None
+            0.8
             'top_p'
+            0.3
             'top_k'
+            1000
             'max_output_tokens'
             'api_key'
             code
                argcount  : 2
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 4
+               stacksize : 4
                flags     : 3
                code
                   0x97007c01730f7401000000000000000000006401a6010000ab01000000
-                  000000000082017403000000000000000000006a0200000000000000007c
-                  01ac02a6010000ab01000000000000000001007402000000000000000000
-                  007c005f03000000000000000064005300
-               254           0 RESUME                   0
+                  0000000000820164027d0274030000000000000000000064037c02ac04a6
+                  020000ab0200000000000000007d037c03a0020000000000000000000000
+                  0000000000000000007c01ac05a6010000ab01000000000000000001007c
+                  037c005f03000000000000000064065300
+               322           0 RESUME                   0
                
-               255           2 LOAD_FAST                1 (api_key)
+               332           2 LOAD_FAST                1 (api_key)
                              4 POP_JUMP_FORWARD_IF_TRUE    15 (to 36)
                
-               256           6 LOAD_GLOBAL              1 (NULL + APIKeyNotFoundError)
+               333           6 LOAD_GLOBAL              1 (NULL + APIKeyNotFoundError)
                             18 LOAD_CONST               1 ('Google Palm API key is required')
                             20 PRECALL                  1
                             24 CALL                     1
                             34 RAISE_VARARGS            1
                
-               258     >>   36 LOAD_GLOBAL              3 (NULL + generativeai)
-                            48 LOAD_ATTR                2 (configure)
-                            58 LOAD_FAST                1 (api_key)
-                            60 KW_NAMES                 2
-                            62 PRECALL                  1
-                            66 CALL                     1
-                            76 POP_TOP
+               335     >>   36 LOAD_CONST               2 ('Install google-generativeai >= 0.1 for Google Palm API')
+                            38 STORE_FAST               2 (err_msg)
                
-               259          78 LOAD_GLOBAL              2 (generativeai)
-                            90 LOAD_FAST                0 (self)
-                            92 STORE_ATTR               3 (genai)
-                           102 LOAD_CONST               0 (None)
-                           104 RETURN_VALUE
+               336          40 LOAD_GLOBAL              3 (NULL + import_dependency)
+                            52 LOAD_CONST               3 ('google.generativeai')
+                            54 LOAD_FAST                2 (err_msg)
+                            56 KW_NAMES                 4
+                            58 PRECALL                  2
+                            62 CALL                     2
+                            72 STORE_FAST               3 (genai)
+               
+               338          74 LOAD_FAST                3 (genai)
+                            76 LOAD_METHOD              2 (configure)
+                            98 LOAD_FAST                1 (api_key)
+                           100 KW_NAMES                 5
+                           102 PRECALL                  1
+                           106 CALL                     1
+                           116 POP_TOP
+               
+               339         118 LOAD_FAST                3 (genai)
+                           120 LOAD_FAST                0 (self)
+                           122 STORE_ATTR               3 (genai)
+                           132 LOAD_CONST               6 (None)
+                           134 RETURN_VALUE
                consts
-                  None
+                  '\n        Configure Google Palm API Key\n        Args:\n            api_key (str): A string of API keys generated from Google Cloud\n\n        Returns:\n\n        '
                   'Google Palm API key is required'
+                  'Install google-generativeai >= 0.1 for Google Palm API'
+                  'google.generativeai'
+                  ('extra',)
                   ('api_key',)
-               names      ('APIKeyNotFoundError', 'generativeai', 'configure', 'genai')
-               varnames   ('self', 'api_key')
+                  None
+               names      ('APIKeyNotFoundError', 'import_dependency', 'configure', 'genai')
+               varnames   ('self', 'api_key', 'err_msg', 'genai')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_configure'
-               firstlineno 254
-               lnotab 0x020104011e022a01
+               firstlineno 322
+               lnotab 0x020a04011e02040122022c01
+            'project_id'
+            'location'
+            code
+               argcount  : 3
+               nlocals   : 5
+               stacksize : 4
+               flags     : 3
+               code
+                  0x970064017d0374010000000000000000000064027c03ac03a6020000ab
+                  0200000000000000007d047c04a001000000000000000000000000000000
+                  00000000007c017c02ac04a6020000ab02000000000000000001007c047c
+                  005f02000000000000000064055300
+               341           0 RESUME                   0
+               
+               352           2 LOAD_CONST               1 ('Install google-cloud-aiplatform for Google Vertexai')
+                             4 STORE_FAST               3 (err_msg)
+               
+               353           6 LOAD_GLOBAL              1 (NULL + import_dependency)
+                            18 LOAD_CONST               2 ('vertexai')
+                            20 LOAD_FAST                3 (err_msg)
+                            22 KW_NAMES                 3
+                            24 PRECALL                  2
+                            28 CALL                     2
+                            38 STORE_FAST               4 (vertexai)
+               
+               354          40 LOAD_FAST                4 (vertexai)
+                            42 LOAD_METHOD              1 (init)
+                            64 LOAD_FAST                1 (project_id)
+                            66 LOAD_FAST                2 (location)
+                            68 KW_NAMES                 4
+                            70 PRECALL                  2
+                            74 CALL                     2
+                            84 POP_TOP
+               
+               355          86 LOAD_FAST                4 (vertexai)
+                            88 LOAD_FAST                0 (self)
+                            90 STORE_ATTR               2 (vertexai)
+                           100 LOAD_CONST               5 (None)
+                           102 RETURN_VALUE
+               consts
+                  '\n        Configure Google VertexAi\n        Args:\n            project_id: GCP Project\n            location: Location of Project\n\n        Returns: Vertexai Object\n\n        '
+                  'Install google-cloud-aiplatform for Google Vertexai'
+                  'vertexai'
+                  ('extra',)
+                  ('project', 'location')
+                  None
+               names      ('import_dependency', 'init', 'vertexai')
+               varnames   ('self', 'project_id', 'location', 'err_msg', 'vertexai')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
+               name       '_configurevertexai'
+               firstlineno 341
+               lnotab 0x020b040122012e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code 0x970067006401a2015300
-               261           0 RESUME                   0
+               357           0 RESUME                   0
                
-               262           2 BUILD_LIST               0
+               358           2 BUILD_LIST               0
                              4 LOAD_CONST               1 (('temperature', 'top_p', 'top_k', 'max_output_tokens'))
                              6 LIST_EXTEND              1
                              8 RETURN_VALUE
                consts
                   None
                   ('temperature', 'top_p', 'top_k', 'max_output_tokens')
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_valid_params'
-               firstlineno 261
+               firstlineno 357
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 6
                flags     : 11
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d027c01a00100000000000000000000000000
                   00000000000000a6000000ab00000000000000000044005d1a5c0200007d
                   037d047c037c02760072117405000000000000000000007c007c037c04a6
-                  030000ab03000000000000000001008c1b64005300
-               264           0 RESUME                   0
+                  030000ab03000000000000000001008c1b64015300
+               360           0 RESUME                   0
                
-               265           2 LOAD_FAST                0 (self)
+               370           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_valid_params)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               2 (valid_params)
                
-               266          42 LOAD_FAST                1 (kwargs)
+               371          42 LOAD_FAST                1 (kwargs)
                             44 LOAD_METHOD              1 (items)
                             66 PRECALL                  0
                             70 CALL                     0
                             80 GET_ITER
                        >>   82 FOR_ITER                26 (to 136)
                             84 UNPACK_SEQUENCE          2
                             88 STORE_FAST               3 (key)
                             90 STORE_FAST               4 (value)
                
-               267          92 LOAD_FAST                3 (key)
+               372          92 LOAD_FAST                3 (key)
                             94 LOAD_FAST                2 (valid_params)
                             96 CONTAINS_OP              0
                             98 POP_JUMP_FORWARD_IF_FALSE    17 (to 134)
                
-               268         100 LOAD_GLOBAL              5 (NULL + setattr)
+               373         100 LOAD_GLOBAL              5 (NULL + setattr)
                            112 LOAD_FAST                0 (self)
                            114 LOAD_FAST                3 (key)
                            116 LOAD_FAST                4 (value)
                            118 PRECALL                  3
                            122 CALL                     3
                            132 POP_TOP
                        >>  134 JUMP_BACKWARD           27 (to 82)
                
-               266     >>  136 LOAD_CONST               0 (None)
+               371     >>  136 LOAD_CONST               1 (None)
                            138 RETURN_VALUE
                consts
+                  '\n        Set Parameters\n        Args:\n            **kwargs: ["temperature", "top_p", "top_k", "max_output_tokens"]\n\n        Returns:\n\n        '
                   None
                names      ('_valid_params', 'items', 'setattr')
                varnames   ('self', 'kwargs', 'valid_params', 'key', 'value')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_set_params'
-               firstlineno 264
-               lnotab 0x020128013201080124fe
+               firstlineno 360
+               lnotab 0x020a28013201080124fe
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000812364027c006a0000000000000000
@@ -1535,17 +1611,17 @@
                   0100000000720664036b010000000073116e010100740300000000000000
                   0000006405a6010000ab01000000000000000082017c006a030000000000
                   000000812364027c006a030000000000000000630278026b010000000072
                   0664036b010000000073116e0101007403000000000000000000006406a6
                   010000ab01000000000000000082017c006a040000000000000000811a7c
                   006a04000000000000000064026b01000000007211740300000000000000
                   0000006407a6010000ab01000000000000000082016401530064015300
-               270           0 RESUME                   0
+               375           0 RESUME                   0
                
-               273           2 LOAD_FAST                0 (self)
+               378           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (temperature)
                             14 POP_JUMP_FORWARD_IF_NONE    35 (to 86)
                             16 LOAD_CONST               2 (0)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                0 (temperature)
                             30 SWAP                     2
                             32 COPY                     2
@@ -1553,21 +1629,21 @@
                             40 POP_JUMP_FORWARD_IF_FALSE     6 (to 54)
                             42 LOAD_CONST               3 (1)
                             44 COMPARE_OP               1 (<=)
                             50 POP_JUMP_FORWARD_IF_TRUE    17 (to 86)
                             52 JUMP_FORWARD             1 (to 56)
                        >>   54 POP_TOP
                
-               274     >>   56 LOAD_GLOBAL              3 (NULL + ValueError)
+               379     >>   56 LOAD_GLOBAL              3 (NULL + ValueError)
                             68 LOAD_CONST               4 ('temperature must be in the range [0.0, 1.0]')
                             70 PRECALL                  1
                             74 CALL                     1
                             84 RAISE_VARARGS            1
                
-               276     >>   86 LOAD_FAST                0 (self)
+               381     >>   86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                2 (top_p)
                             98 POP_JUMP_FORWARD_IF_NONE    35 (to 170)
                            100 LOAD_CONST               2 (0)
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                2 (top_p)
                            114 SWAP                     2
                            116 COPY                     2
@@ -1575,21 +1651,21 @@
                            124 POP_JUMP_FORWARD_IF_FALSE     6 (to 138)
                            126 LOAD_CONST               3 (1)
                            128 COMPARE_OP               1 (<=)
                            134 POP_JUMP_FORWARD_IF_TRUE    17 (to 170)
                            136 JUMP_FORWARD             1 (to 140)
                        >>  138 POP_TOP
                
-               277     >>  140 LOAD_GLOBAL              3 (NULL + ValueError)
+               382     >>  140 LOAD_GLOBAL              3 (NULL + ValueError)
                            152 LOAD_CONST               5 ('top_p must be in the range [0.0, 1.0]')
                            154 PRECALL                  1
                            158 CALL                     1
                            168 RAISE_VARARGS            1
                
-               279     >>  170 LOAD_FAST                0 (self)
+               384     >>  170 LOAD_FAST                0 (self)
                            172 LOAD_ATTR                3 (top_k)
                            182 POP_JUMP_FORWARD_IF_NONE    35 (to 254)
                            184 LOAD_CONST               2 (0)
                            186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                3 (top_k)
                            198 SWAP                     2
                            200 COPY                     2
@@ -1597,36 +1673,36 @@
                            208 POP_JUMP_FORWARD_IF_FALSE     6 (to 222)
                            210 LOAD_CONST               3 (1)
                            212 COMPARE_OP               1 (<=)
                            218 POP_JUMP_FORWARD_IF_TRUE    17 (to 254)
                            220 JUMP_FORWARD             1 (to 224)
                        >>  222 POP_TOP
                
-               280     >>  224 LOAD_GLOBAL              3 (NULL + ValueError)
+               385     >>  224 LOAD_GLOBAL              3 (NULL + ValueError)
                            236 LOAD_CONST               6 ('top_k must be in the range [0.0, 1.0]')
                            238 PRECALL                  1
                            242 CALL                     1
                            252 RAISE_VARARGS            1
                
-               282     >>  254 LOAD_FAST                0 (self)
+               387     >>  254 LOAD_FAST                0 (self)
                            256 LOAD_ATTR                4 (max_output_tokens)
                            266 POP_JUMP_FORWARD_IF_NONE    26 (to 320)
                            268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                4 (max_output_tokens)
                            280 LOAD_CONST               2 (0)
                            282 COMPARE_OP               1 (<=)
                            288 POP_JUMP_FORWARD_IF_FALSE    17 (to 324)
                
-               283         290 LOAD_GLOBAL              3 (NULL + ValueError)
+               388         290 LOAD_GLOBAL              3 (NULL + ValueError)
                            302 LOAD_CONST               7 ('max_output_tokens must be greater than zero')
                            304 PRECALL                  1
                            308 CALL                     1
                            318 RAISE_VARARGS            1
                
-               282     >>  320 LOAD_CONST               1 (None)
+               387     >>  320 LOAD_CONST               1 (None)
                            322 RETURN_VALUE
                        >>  324 LOAD_CONST               1 (None)
                            326 RETURN_VALUE
                consts
                   'Validates the parameters for Google'
                   None
                   0
@@ -1637,119 +1713,112 @@
                   'max_output_tokens must be greater than zero'
                names      ('temperature', 'ValueError', 'top_p', 'top_k', 'max_output_tokens')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_validate'
-               firstlineno 270
+               firstlineno 375
                lnotab 0x020336011e0236011e0236011e0224011eff
             'prompt'
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   008201
-               285           0 RESUME                   0
+               390           0 RESUME                   0
                
-               296           2 LOAD_GLOBAL              1 (NULL + MethodNotImplementedError)
+               401           2 LOAD_GLOBAL              1 (NULL + MethodNotImplementedError)
                             14 LOAD_CONST               1 ('method has not been implemented')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RAISE_VARARGS            1
                consts
                   '\n        Generates text for prompt, specific to implementation.\n\n        Args:\n            prompt (str): Prompt\n\n        Returns:\n            str: LLM response\n        '
                   'method has not been implemented'
                names      ('MethodNotImplementedError',)
                varnames   ('self', 'prompt')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       '_generate_text'
-               firstlineno 285
+               firstlineno 390
                lnotab 0x020b
             ''
             'instruction'
             'value'
             'suffix'
             code
                argcount  : 4
                nlocals   : 5
-               stacksize : 4
+               stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c01a6010000ab0100000000000000
-                  007401000000000000000000007c02a6010000ab0100000000000000007a
-                  0000007c005f0100000000000000007401000000000000000000007c01a6
-                  010000ab0100000000000000007401000000000000000000007c02a60100
-                  00ab0100000000000000007a0000007c037a0000007d047c00a002000000
-                  00000000000000000000000000000000007c04a6010000ab010000000000
-                  0000005300
-               298           0 RESUME                   0
+                  007c027a0000007c005f0100000000000000007401000000000000000000
+                  007c01a6010000ab0100000000000000007c027a0000007c037a0000007d
+                  047c00a00200000000000000000000000000000000000000007c04a60100
+                  00ab0100000000000000005300
+               403           0 RESUME                   0
                
-               310           2 LOAD_GLOBAL              1 (NULL + str)
+               415           2 LOAD_GLOBAL              1 (NULL + str)
                             14 LOAD_FAST                1 (instruction)
                             16 PRECALL                  1
                             20 CALL                     1
-                            30 LOAD_GLOBAL              1 (NULL + str)
-                            42 LOAD_FAST                2 (value)
-                            44 PRECALL                  1
-                            48 CALL                     1
-                            58 BINARY_OP                0 (+)
-                            62 LOAD_FAST                0 (self)
-                            64 STORE_ATTR               1 (last_prompt)
-               
-               311          74 LOAD_GLOBAL              1 (NULL + str)
-                            86 LOAD_FAST                1 (instruction)
-                            88 PRECALL                  1
-                            92 CALL                     1
-                           102 LOAD_GLOBAL              1 (NULL + str)
-                           114 LOAD_FAST                2 (value)
+                            30 LOAD_FAST                2 (value)
+                            32 BINARY_OP                0 (+)
+                            36 LOAD_FAST                0 (self)
+                            38 STORE_ATTR               1 (last_prompt)
+               
+               416          48 LOAD_GLOBAL              1 (NULL + str)
+                            60 LOAD_FAST                1 (instruction)
+                            62 PRECALL                  1
+                            66 CALL                     1
+                            76 LOAD_FAST                2 (value)
+                            78 BINARY_OP                0 (+)
+                            82 LOAD_FAST                3 (suffix)
+                            84 BINARY_OP                0 (+)
+                            88 STORE_FAST               4 (prompt)
+               
+               417          90 LOAD_FAST                0 (self)
+                            92 LOAD_METHOD              2 (_generate_text)
+                           114 LOAD_FAST                4 (prompt)
                            116 PRECALL                  1
                            120 CALL                     1
-                           130 BINARY_OP                0 (+)
-                           134 LOAD_FAST                3 (suffix)
-                           136 BINARY_OP                0 (+)
-                           140 STORE_FAST               4 (prompt)
-               
-               312         142 LOAD_FAST                0 (self)
-                           144 LOAD_METHOD              2 (_generate_text)
-                           166 LOAD_FAST                4 (prompt)
-                           168 PRECALL                  1
-                           172 CALL                     1
-                           182 RETURN_VALUE
+                           130 RETURN_VALUE
                consts
-                  '\n        Call the Google LLM.\n\n        Args:\n            instruction (str): Instruction to pass\n            value (str): Value to pass\n            suffix (str): Suffix to pass\n\n        Returns:\n            str: Response\n        '
+                  '\n        Call the Google LLM.\n\n        Args:\n            instruction (object): Instruction to pass\n            value (str): Value to pass\n            suffix (str): Suffix to pass\n\n        Returns:\n            str: Response\n        '
                names      ('str', 'last_prompt', '_generate_text')
                varnames   ('self', 'instruction', 'value', 'suffix', 'prompt')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
                name       'call'
-               firstlineno 298
-               lnotab 0x020c48014401
+               firstlineno 403
+               lnotab 0x020c2e012a01
+            None
             ('',)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Any', '__annotations__', 'temperature', 'Optional', 'float', 'top_p', 'top_k', 'max_output_tokens', 'int', 'str', '_configure', '_valid_params', '_set_params', '_validate', 'abstractmethod', '_generate_text', 'call')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Any', '__annotations__', 'temperature', 'Optional', 'float', 'top_p', 'top_k', 'max_output_tokens', 'int', 'str', '_configure', '_configurevertexai', '_valid_params', '_set_params', '_validate', 'abstractmethod', '_generate_text', 'Prompt', 'call')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
          name       'BaseGoogle'
-         firstlineno 245
+         firstlineno 310
          lnotab
-            0x0c0104020a011a011a011a011a020c0706030606060f02010eff0e0102
-            0c
+            0x0c0104050a011a011a011a011a020c1310100603060f060f02010eff0e
+            01020c
       'BaseGoogle'
-   names      ('__doc__', 'ast', 're', 'abc', 'ABC', 'abstractmethod', 'typing', 'Any', 'Dict', 'Optional', 'openai', 'requests', 'google', 'generativeai', 'constants', 'END_CODE_TAG', 'START_CODE_TAG', 'exceptions', 'APIKeyNotFoundError', 'MethodNotImplementedError', 'NoCodeFoundError', 'LLM', 'BaseOpenAI', 'HuggingFaceLLM', 'BaseGoogle')
+   names      ('__doc__', 'ast', 're', 'abc', 'ABC', 'abstractmethod', 'typing', 'Any', 'Dict', 'Optional', 'openai', 'requests', 'exceptions', 'APIKeyNotFoundError', 'MethodNotImplementedError', 'NoCodeFoundError', 'helpers._optional', 'import_dependency', 'prompts.base', 'Prompt', 'LLM', 'BaseOpenAI', 'HuggingFaceLLM', 'BaseGoogle')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\base.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104020801080110011402080108010c02100114071a621e561c
-      29
+      0x00ff0201041008010801100114020801080214050c010c031a6c1e6a1c
+      3e
```

### Comparing `hfttai-0.1.2/pandasai/llm/__pycache__/fake.cpython-311.pyc` & `hfttai-0.1.3/pandasai/llm/__pycache__/fake.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/__pycache__/google_palm.cpython-311.pyc` & `hfttai-0.1.3/pandasai/llm/__pycache__/google_palm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/__pycache__/openai.cpython-311.pyc` & `hfttai-0.1.3/pandasai/llm/__pycache__/openai.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,315 +1,361 @@
 magic:    0xa70d0d0a
-moddate:  0xaaaa6e64 (Thu May 25 00:24:10 2023 UTC)
-files sz: 2033
+moddate:  0x26d2a764 (Fri Jul  7 08:51:50 2023 UTC)
+files sz: 3176
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c015a01640164036c026d035a036d045a046d
       055a050100640164026c065a06640164046c076d085a080100640564066c
-      096d0a5a0a6d0b5a0b0100640764086c0c6d0d5a0d010002006508a60000
-      00ab00000000000000000001000200470064098400640a650da6030000ab
-      0300000000000000005a0e64025300
+      096d0a5a0a6d0b5a0b0100640564076c0c6d0d5a0d0100640864096c0e6d
+      0f5a0f010002006508a6000000ab00000000000000000001000200470064
+      0a8400640b650fa6030000ab0300000000000000005a1064025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('OpenAI LLM')
+     1           2 LOAD_CONST               0 ('OpenAI LLM API\n\nThis module is to run the OpenAI API using OpenAI API.\n\nExample:\n    Use below example to call OpenAI Model\n\n    >>> from pandasai.llm.openai import OpenAI\n')
                  4 STORE_NAME               0 (__doc__)
    
-     3           6 LOAD_CONST               1 (0)
+    11           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (os)
                 12 STORE_NAME               1 (os)
    
-     4          14 LOAD_CONST               1 (0)
+    12          14 LOAD_CONST               1 (0)
                 16 LOAD_CONST               3 (('Any', 'Dict', 'Optional'))
                 18 IMPORT_NAME              2 (typing)
                 20 IMPORT_FROM              3 (Any)
                 22 STORE_NAME               3 (Any)
                 24 IMPORT_FROM              4 (Dict)
                 26 STORE_NAME               4 (Dict)
                 28 IMPORT_FROM              5 (Optional)
                 30 STORE_NAME               5 (Optional)
                 32 POP_TOP
    
-     6          34 LOAD_CONST               1 (0)
+    14          34 LOAD_CONST               1 (0)
                 36 LOAD_CONST               2 (None)
                 38 IMPORT_NAME              6 (openai)
                 40 STORE_NAME               6 (openai)
    
-     7          42 LOAD_CONST               1 (0)
+    15          42 LOAD_CONST               1 (0)
                 44 LOAD_CONST               4 (('load_dotenv',))
                 46 IMPORT_NAME              7 (dotenv)
                 48 IMPORT_FROM              8 (load_dotenv)
                 50 STORE_NAME               8 (load_dotenv)
                 52 POP_TOP
    
-     9          54 LOAD_CONST               5 (2)
+    17          54 LOAD_CONST               5 (2)
                 56 LOAD_CONST               6 (('APIKeyNotFoundError', 'UnsupportedOpenAIModelError'))
                 58 IMPORT_NAME              9 (exceptions)
                 60 IMPORT_FROM             10 (APIKeyNotFoundError)
                 62 STORE_NAME              10 (APIKeyNotFoundError)
                 64 IMPORT_FROM             11 (UnsupportedOpenAIModelError)
                 66 STORE_NAME              11 (UnsupportedOpenAIModelError)
                 68 POP_TOP
    
-    10          70 LOAD_CONST               7 (1)
-                72 LOAD_CONST               8 (('BaseOpenAI',))
-                74 IMPORT_NAME             12 (base)
-                76 IMPORT_FROM             13 (BaseOpenAI)
-                78 STORE_NAME              13 (BaseOpenAI)
+    18          70 LOAD_CONST               5 (2)
+                72 LOAD_CONST               7 (('Prompt',))
+                74 IMPORT_NAME             12 (prompts.base)
+                76 IMPORT_FROM             13 (Prompt)
+                78 STORE_NAME              13 (Prompt)
                 80 POP_TOP
    
-    12          82 PUSH_NULL
-                84 LOAD_NAME                8 (load_dotenv)
-                86 PRECALL                  0
-                90 CALL                     0
-               100 POP_TOP
+    19          82 LOAD_CONST               8 (1)
+                84 LOAD_CONST               9 (('BaseOpenAI',))
+                86 IMPORT_NAME             14 (base)
+                88 IMPORT_FROM             15 (BaseOpenAI)
+                90 STORE_NAME              15 (BaseOpenAI)
+                92 POP_TOP
    
-    15         102 PUSH_NULL
-               104 LOAD_BUILD_CLASS
-               106 LOAD_CONST               9 (<code object OpenAI, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 15>)
-               108 MAKE_FUNCTION            0
-               110 LOAD_CONST              10 ('OpenAI')
-               112 LOAD_NAME               13 (BaseOpenAI)
-               114 PRECALL                  3
-               118 CALL                     3
-               128 STORE_NAME              14 (OpenAI)
-               130 LOAD_CONST               2 (None)
-               132 RETURN_VALUE
+    21          94 PUSH_NULL
+                96 LOAD_NAME                8 (load_dotenv)
+                98 PRECALL                  0
+               102 CALL                     0
+               112 POP_TOP
+   
+    24         114 PUSH_NULL
+               116 LOAD_BUILD_CLASS
+               118 LOAD_CONST              10 (<code object OpenAI, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 24>)
+               120 MAKE_FUNCTION            0
+               122 LOAD_CONST              11 ('OpenAI')
+               124 LOAD_NAME               15 (BaseOpenAI)
+               126 PRECALL                  3
+               130 CALL                     3
+               140 STORE_NAME              16 (OpenAI)
+               142 LOAD_CONST               2 (None)
+               144 RETURN_VALUE
    consts
-      'OpenAI LLM'
+      'OpenAI LLM API\n\nThis module is to run the OpenAI API using OpenAI API.\n\nExample:\n    Use below example to call OpenAI Model\n\n    >>> from pandasai.llm.openai import OpenAI\n'
       0
       None
       ('Any', 'Dict', 'Optional')
       ('load_dotenv',)
       2
       ('APIKeyNotFoundError', 'UnsupportedOpenAIModelError')
+      ('Prompt',)
       1
       ('BaseOpenAI',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x8700970065005a0164005a02550064015a0367006402a2015a04640367
             015a0564045a066507650864053c00000009006411640765096507190000
             000000000000006602640884055a0a650b6409650c6507650d6602190000
             00000000000000660288006601640a840ca6000000ab0000000000000000
-            005a0e6412640c6507640d6507640e6507640965076608640f84055a0f65
-            0b64096507660264108404a6000000ab0000000000000000005a10880078
-            015a115300
+            005a0e6412640c650f640d6507640e6507640965076608640f84055a1065
+            0b64096507660264108404a6000000ab0000000000000000005a11880078
+            015a125300
                        0 MAKE_CELL                0 (__class__)
          
-          15           2 RESUME                   0
+          24           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('OpenAI')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-          16          14 LOAD_CONST               1 ('OpenAI LLM')
+          25          14 LOAD_CONST               1 ('OpenAI LLM using BaseOpenAI Class.\n\n    An API call to OpenAI API is sent and response is recorded and returned.\n    The default chat model is **gpt-3.5-turbo** while **text-davinci-003** is only\n    supported completion model.\n    The list of supported Chat models includes ["gpt-4", "gpt-4-0314", "gpt-4-32k",\n     "gpt-4-32k-0314","gpt-3.5-turbo", "gpt-3.5-turbo-0301"].\n\n    ')
                       16 STORE_NAME               3 (__doc__)
          
-          18          18 BUILD_LIST               0
-                      20 LOAD_CONST               2 (('gpt-4', 'gpt-4-0314', 'gpt-4-32k', 'gpt-4-32k-0314', 'gpt-3.5-turbo', 'gpt-3.5-turbo-0301'))
+          35          18 BUILD_LIST               0
+                      20 LOAD_CONST               2 (('gpt-4', 'gpt-4-0613', 'gpt-4-32k', 'gpt-4-32k-0613', 'gpt-3.5-turbo', 'gpt-3.5-turbo-16k', 'gpt-3.5-turbo-0613', 'gpt-3.5-turbo-16k-0613'))
                       22 LIST_EXTEND              1
                       24 STORE_NAME               4 (_supported_chat_models)
          
-          26          26 LOAD_CONST               3 ('text-davinci-003')
+          45          26 LOAD_CONST               3 ('text-davinci-003')
                       28 BUILD_LIST               1
                       30 STORE_NAME               5 (_supported_completion_models)
          
-          28          32 LOAD_CONST               4 ('gpt-3.5-turbo')
+          47          32 LOAD_CONST               4 ('gpt-3.5-turbo')
                       34 STORE_NAME               6 (model)
                       36 LOAD_NAME                7 (str)
                       38 LOAD_NAME                8 (__annotations__)
                       40 LOAD_CONST               5 ('model')
                       42 STORE_SUBSCR
          
-          32          46 NOP
+          51          46 NOP
          
-          30          48 LOAD_CONST              17 ((None,))
+          49          48 LOAD_CONST              17 ((None,))
                       50 LOAD_CONST               7 ('api_token')
          
-          32          52 LOAD_NAME                9 (Optional)
+          51          52 LOAD_NAME                9 (Optional)
                       54 LOAD_NAME                7 (str)
                       56 BINARY_SUBSCR
          
-          30          66 BUILD_TUPLE              2
-                      68 LOAD_CONST               8 (<code object __init__, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 30>)
+          49          66 BUILD_TUPLE              2
+                      68 LOAD_CONST               8 (<code object __init__, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 49>)
                       70 MAKE_FUNCTION            5 (defaults, annotations)
                       72 STORE_NAME              10 (__init__)
          
-          42          74 LOAD_NAME               11 (property)
+          77          74 LOAD_NAME               11 (property)
          
-          43          76 LOAD_CONST               9 ('return')
+          78          76 LOAD_CONST               9 ('return')
                       78 LOAD_NAME               12 (Dict)
                       80 LOAD_NAME                7 (str)
                       82 LOAD_NAME               13 (Any)
                       84 BUILD_TUPLE              2
                       86 BINARY_SUBSCR
                       96 BUILD_TUPLE              2
                       98 LOAD_CLOSURE             0 (__class__)
                      100 BUILD_TUPLE              1
-                     102 LOAD_CONST              10 (<code object _default_params, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 42>)
+                     102 LOAD_CONST              10 (<code object _default_params, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 77>)
                      104 MAKE_FUNCTION           12 (annotations, closure)
          
-          42         106 PRECALL                  0
+          77         106 PRECALL                  0
                      110 CALL                     0
          
-          43         120 STORE_NAME              14 (_default_params)
+          78         120 STORE_NAME              14 (_default_params)
          
-          50         122 LOAD_CONST              18 (('',))
+          85         122 LOAD_CONST              18 (('',))
                      124 LOAD_CONST              12 ('instruction')
-                     126 LOAD_NAME                7 (str)
+                     126 LOAD_NAME               15 (Prompt)
                      128 LOAD_CONST              13 ('value')
                      130 LOAD_NAME                7 (str)
                      132 LOAD_CONST              14 ('suffix')
                      134 LOAD_NAME                7 (str)
                      136 LOAD_CONST               9 ('return')
                      138 LOAD_NAME                7 (str)
                      140 BUILD_TUPLE              8
-                     142 LOAD_CONST              15 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 50>)
+                     142 LOAD_CONST              15 (<code object call, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 85>)
                      144 MAKE_FUNCTION            5 (defaults, annotations)
-                     146 STORE_NAME              15 (call)
+                     146 STORE_NAME              16 (call)
          
-          76         148 LOAD_NAME               11 (property)
+         111         148 LOAD_NAME               11 (property)
          
-          77         150 LOAD_CONST               9 ('return')
+         112         150 LOAD_CONST               9 ('return')
                      152 LOAD_NAME                7 (str)
                      154 BUILD_TUPLE              2
-                     156 LOAD_CONST              16 (<code object type, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 76>)
+                     156 LOAD_CONST              16 (<code object type, file "D:\Pro\pandas-ai-main\pandasai\llm\openai.py", line 111>)
                      158 MAKE_FUNCTION            4 (annotations)
          
-          76         160 PRECALL                  0
+         111         160 PRECALL                  0
                      164 CALL                     0
          
-          77         174 STORE_NAME              16 (type)
+         112         174 STORE_NAME              17 (type)
                      176 LOAD_CLOSURE             0 (__class__)
                      178 COPY                     1
-                     180 STORE_NAME              17 (__classcell__)
+                     180 STORE_NAME              18 (__classcell__)
                      182 RETURN_VALUE
          consts
             'OpenAI'
-            'OpenAI LLM'
-            ('gpt-4', 'gpt-4-0314', 'gpt-4-32k', 'gpt-4-32k-0314', 'gpt-3.5-turbo', 'gpt-3.5-turbo-0301')
+            'OpenAI LLM using BaseOpenAI Class.\n\n    An API call to OpenAI API is sent and response is recorded and returned.\n    The default chat model is **gpt-3.5-turbo** while **text-davinci-003** is only\n    supported completion model.\n    The list of supported Chat models includes ["gpt-4", "gpt-4-0314", "gpt-4-32k",\n     "gpt-4-32k-0314","gpt-3.5-turbo", "gpt-3.5-turbo-0301"].\n\n    '
+            ('gpt-4', 'gpt-4-0613', 'gpt-4-32k', 'gpt-4-32k-0613', 'gpt-3.5-turbo', 'gpt-3.5-turbo-16k', 'gpt-3.5-turbo-0613', 'gpt-3.5-turbo-16k-0613')
             'text-davinci-003'
             'gpt-3.5-turbo'
             'model'
             None
             'api_token'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
                flags     : 11
                code
                   0x97007c0170157401000000000000000000006a01000000000000000064
-                  01a6010000ab010000000000000000700164007c005f0200000000000000
-                  007c006a020000000000000000800f7407000000000000000000006402a6
+                  01a6010000ab010000000000000000700164027c005f0200000000000000
+                  007c006a020000000000000000800f7407000000000000000000006403a6
                   010000ab01000000000000000082017c006a020000000000000000740800
-                  0000000000000000005f05000000000000000002007c006a060000000000
-                  000000640369007c02a4018e01010064005300
-                30           0 RESUME                   0
+                  0000000000000000005f0500000000000000007c02a00600000000000000
+                  000000000000000000000000006404a6010000ab01000000000000000070
+                  137401000000000000000000006a0100000000000000006405a6010000ab
+                  0100000000000000007c005f0700000000000000007c006a070000000000
+                  00000072197c006a0700000000000000007c006a07000000000000000064
+                  069c027408000000000000000000005f08000000000000000002007c006a
+                  090000000000000000640769007c02a4018e01010064025300
+                49           0 RESUME                   0
                
-                35           2 LOAD_FAST                1 (api_token)
+                63           2 LOAD_FAST                1 (api_token)
                              4 JUMP_IF_TRUE_OR_POP     21 (to 48)
                              6 LOAD_GLOBAL              1 (NULL + os)
                             18 LOAD_ATTR                1 (getenv)
                             28 LOAD_CONST               1 ('OPENAI_API_KEY')
                             30 PRECALL                  1
                             34 CALL                     1
                             44 JUMP_IF_TRUE_OR_POP      1 (to 48)
-                            46 LOAD_CONST               0 (None)
+                            46 LOAD_CONST               2 (None)
                        >>   48 LOAD_FAST                0 (self)
                             50 STORE_ATTR               2 (api_token)
                
-                36          60 LOAD_FAST                0 (self)
+                64          60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                2 (api_token)
                             72 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 104)
                
-                37          74 LOAD_GLOBAL              7 (NULL + APIKeyNotFoundError)
-                            86 LOAD_CONST               2 ('OpenAI API key is required')
+                65          74 LOAD_GLOBAL              7 (NULL + APIKeyNotFoundError)
+                            86 LOAD_CONST               3 ('OpenAI API key is required')
                             88 PRECALL                  1
                             92 CALL                     1
                            102 RAISE_VARARGS            1
                
-                38     >>  104 LOAD_FAST                0 (self)
+                66     >>  104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                2 (api_token)
                            116 LOAD_GLOBAL              8 (openai)
                            128 STORE_ATTR               5 (api_key)
                
-                40         138 PUSH_NULL
-                           140 LOAD_FAST                0 (self)
-                           142 LOAD_ATTR                6 (_set_params)
-                           152 LOAD_CONST               3 (())
-                           154 BUILD_MAP                0
-                           156 LOAD_FAST                2 (kwargs)
-                           158 DICT_MERGE               1
-                           160 CALL_FUNCTION_EX         1
-                           162 POP_TOP
-                           164 LOAD_CONST               0 (None)
-                           166 RETURN_VALUE
+                68         138 LOAD_FAST                2 (kwargs)
+                           140 LOAD_METHOD              6 (get)
+                           162 LOAD_CONST               4 ('openai_proxy')
+                           164 PRECALL                  1
+                           168 CALL                     1
+                           178 JUMP_IF_TRUE_OR_POP     19 (to 218)
+                           180 LOAD_GLOBAL              1 (NULL + os)
+                           192 LOAD_ATTR                1 (getenv)
+                           202 LOAD_CONST               5 ('OPENAI_PROXY')
+                           204 PRECALL                  1
+                           208 CALL                     1
+                       >>  218 LOAD_FAST                0 (self)
+                           220 STORE_ATTR               7 (openai_proxy)
+               
+                69         230 LOAD_FAST                0 (self)
+                           232 LOAD_ATTR                7 (openai_proxy)
+                           242 POP_JUMP_FORWARD_IF_FALSE    25 (to 294)
+               
+                71         244 LOAD_FAST                0 (self)
+                           246 LOAD_ATTR                7 (openai_proxy)
+               
+                72         256 LOAD_FAST                0 (self)
+                           258 LOAD_ATTR                7 (openai_proxy)
+               
+                70         268 LOAD_CONST               6 (('http', 'https'))
+                           270 BUILD_CONST_KEY_MAP      2
+                           272 LOAD_GLOBAL              8 (openai)
+                           284 STORE_ATTR               8 (proxy)
+               
+                75     >>  294 PUSH_NULL
+                           296 LOAD_FAST                0 (self)
+                           298 LOAD_ATTR                9 (_set_params)
+                           308 LOAD_CONST               7 (())
+                           310 BUILD_MAP                0
+                           312 LOAD_FAST                2 (kwargs)
+                           314 DICT_MERGE               1
+                           316 CALL_FUNCTION_EX         1
+                           318 POP_TOP
+                           320 LOAD_CONST               2 (None)
+                           322 RETURN_VALUE
                consts
-                  None
+                  '\n        __init__ method of OpenAI Class\n        Args:\n            api_token (str): API Token for OpenAI platform.\n            **kwargs: Extended Parameters inferred from BaseOpenAI class\n\n        Returns: Response generated from OpenAI API\n        '
                   'OPENAI_API_KEY'
+                  None
                   'OpenAI API key is required'
+                  'openai_proxy'
+                  'OPENAI_PROXY'
+                  ('http', 'https')
                   ()
-               names      ('os', 'getenv', 'api_token', 'APIKeyNotFoundError', 'openai', 'api_key', '_set_params')
+               names      ('os', 'getenv', 'api_token', 'APIKeyNotFoundError', 'openai', 'api_key', 'get', 'openai_proxy', 'proxy', '_set_params')
                varnames   ('self', 'api_token', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\openai.py'
                name       '__init__'
-               firstlineno 30
-               lnotab 0x02053a010e011e012202
+               firstlineno 49
+               lnotab 0x020e3a010e011e0122025c010e020c010cfe1a05
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x950197006900740100000000000000000000a6000000ab000000000000
                   0000006a010000000000000000a50164017c006a02000000000000000069
                   01a5015300
                              0 COPY_FREE_VARS           1
                
-                42           2 RESUME                   0
+                77           2 RESUME                   0
                
-                45           4 BUILD_MAP                0
+                80           4 BUILD_MAP                0
                
-                46           6 LOAD_GLOBAL              1 (NULL + super)
+                81           6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (_default_params)
                
-                45          42 DICT_UPDATE              1
+                80          42 DICT_UPDATE              1
                
-                47          44 LOAD_CONST               1 ('model')
+                82          44 LOAD_CONST               1 ('model')
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                2 (model)
                
-                45          58 BUILD_MAP                1
+                80          58 BUILD_MAP                1
                             60 DICT_UPDATE              1
                             62 RETURN_VALUE
                consts
                   'Get the default parameters for calling OpenAI API'
                   'model'
                names      ('super', '_default_params', 'model')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\openai.py'
                name       '_default_params'
-               firstlineno 42
+               firstlineno 77
                lnotab 0x0403020124ff02020efe
             ''
             'instruction'
             'value'
             'suffix'
             code
                argcount  : 4
@@ -326,36 +372,36 @@
                   0000007a0000007c037a000000a6010000ab0100000000000000007d046e
                   537c006a0200000000000000007c006a050000000000000000760072367c
                   00a006000000000000000000000000000000000000000074010000000000
                   00000000007c01a6010000ab010000000000000000740100000000000000
                   0000007c02a6010000ab0100000000000000007a0000007c037a000000a6
                   010000ab0100000000000000007d046e0f740f0000000000000000000064
                   01a6010000ab01000000000000000082017c045300
-                50           0 RESUME                   0
+                85           0 RESUME                   0
                
-                65           2 LOAD_GLOBAL              1 (NULL + str)
+               100           2 LOAD_GLOBAL              1 (NULL + str)
                             14 LOAD_FAST                1 (instruction)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_GLOBAL              1 (NULL + str)
                             42 LOAD_FAST                2 (value)
                             44 PRECALL                  1
                             48 CALL                     1
                             58 BINARY_OP                0 (+)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               1 (last_prompt)
                
-                67          74 LOAD_FAST                0 (self)
+               102          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                2 (model)
                             86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                3 (_supported_completion_models)
                             98 CONTAINS_OP              0
                            100 POP_JUMP_FORWARD_IF_FALSE    54 (to 210)
                
-                68         102 LOAD_FAST                0 (self)
+               103         102 LOAD_FAST                0 (self)
                            104 LOAD_METHOD              4 (completion)
                            126 LOAD_GLOBAL              1 (NULL + str)
                            138 LOAD_FAST                1 (instruction)
                            140 PRECALL                  1
                            144 CALL                     1
                            154 LOAD_GLOBAL              1 (NULL + str)
                            166 LOAD_FAST                2 (value)
@@ -365,22 +411,22 @@
                            186 LOAD_FAST                3 (suffix)
                            188 BINARY_OP                0 (+)
                            192 PRECALL                  1
                            196 CALL                     1
                            206 STORE_FAST               4 (response)
                            208 JUMP_FORWARD            83 (to 376)
                
-                69     >>  210 LOAD_FAST                0 (self)
+               104     >>  210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                2 (model)
                            222 LOAD_FAST                0 (self)
                            224 LOAD_ATTR                5 (_supported_chat_models)
                            234 CONTAINS_OP              0
                            236 POP_JUMP_FORWARD_IF_FALSE    54 (to 346)
                
-                70         238 LOAD_FAST                0 (self)
+               105         238 LOAD_FAST                0 (self)
                            240 LOAD_METHOD              6 (chat_completion)
                            262 LOAD_GLOBAL              1 (NULL + str)
                            274 LOAD_FAST                1 (instruction)
                            276 PRECALL                  1
                            280 CALL                     1
                            290 LOAD_GLOBAL              1 (NULL + str)
                            302 LOAD_FAST                2 (value)
@@ -390,68 +436,68 @@
                            322 LOAD_FAST                3 (suffix)
                            324 BINARY_OP                0 (+)
                            328 PRECALL                  1
                            332 CALL                     1
                            342 STORE_FAST               4 (response)
                            344 JUMP_FORWARD            15 (to 376)
                
-                72     >>  346 LOAD_GLOBAL             15 (NULL + UnsupportedOpenAIModelError)
+               107     >>  346 LOAD_GLOBAL             15 (NULL + UnsupportedOpenAIModelError)
                            358 LOAD_CONST               1 ('Unsupported model')
                            360 PRECALL                  1
                            364 CALL                     1
                            374 RAISE_VARARGS            1
                
-                74     >>  376 LOAD_FAST                4 (response)
+               109     >>  376 LOAD_FAST                4 (response)
                            378 RETURN_VALUE
                consts
-                  '\n        Call the OpenAI LLM.\n\n        Args:\n            instruction (str): Instruction to pass\n            value (str): Value to pass\n            suffix (str): Suffix to pass\n\n        Raises:\n            UnsupportedOpenAIModelError: Unsupported model\n\n        Returns:\n            str: Response\n        '
+                  '\n        Call the OpenAI LLM.\n\n        Args:\n            instruction (Prompt): Instruction to pass\n            value (str): Value to pass\n            suffix (str): Suffix to pass\n\n        Raises:\n            UnsupportedOpenAIModelError: Unsupported model\n\n        Returns:\n            str: Response\n        '
                   'Unsupported model'
                names      ('str', 'last_prompt', 'model', '_supported_completion_models', 'completion', '_supported_chat_models', 'chat_completion', 'UnsupportedOpenAIModelError')
                varnames   ('self', 'instruction', 'value', 'suffix', 'response')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\openai.py'
                name       'call'
-               firstlineno 50
+               firstlineno 85
                lnotab 0x020f48021c016c011c016c021e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064015300
-                76           0 RESUME                   0
+               111           0 RESUME                   0
                
-                78           2 LOAD_CONST               1 ('openai')
+               113           2 LOAD_CONST               1 ('openai')
                              4 RETURN_VALUE
                consts
                   None
                   'openai'
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\openai.py'
                name       'type'
-               firstlineno 76
+               firstlineno 111
                lnotab 0x0202
             (None,)
             ('',)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', '_supported_chat_models', '_supported_completion_models', 'model', 'str', '__annotations__', 'Optional', '__init__', 'property', 'Dict', 'Any', '_default_params', 'call', 'type', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', '_supported_chat_models', '_supported_completion_models', 'model', 'str', '__annotations__', 'Optional', '__init__', 'property', 'Dict', 'Any', '_default_params', 'Prompt', 'call', 'type', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\openai.py'
          name       'OpenAI'
-         firstlineno 15
+         firstlineno 24
          lnotab
-            0x0e010402080806020e0402fe04020efe080c02011eff0e0102071a1a02
+            0x0e01040a080a06020e0402fe04020efe081c02011eff0e0102071a1a02
             010aff0e01
       'OpenAI'
-   names      ('__doc__', 'os', 'typing', 'Any', 'Dict', 'Optional', 'openai', 'dotenv', 'load_dotenv', 'exceptions', 'APIKeyNotFoundError', 'UnsupportedOpenAIModelError', 'base', 'BaseOpenAI', 'OpenAI')
+   names      ('__doc__', 'os', 'typing', 'Any', 'Dict', 'Optional', 'openai', 'dotenv', 'load_dotenv', 'exceptions', 'APIKeyNotFoundError', 'UnsupportedOpenAIModelError', 'prompts.base', 'Prompt', 'base', 'BaseOpenAI', 'OpenAI')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Pro\\pandas-ai-main\\pandasai\\llm\\openai.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104020801140208010c0210010c021403
+   lnotab 0x00ff0201040a0801140208010c0210010c010c021403
```

### Comparing `hfttai-0.1.2/pandasai/llm/__pycache__/starcoder.cpython-311.pyc` & `hfttai-0.1.3/pandasai/llm/__pycache__/starcoder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/azure_openai.py` & `hfttai-0.1.3/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/base.py` & `hfttai-0.1.3/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/fake.py` & `hfttai-0.1.3/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/falcon.py` & `hfttai-0.1.3/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/google_palm.py` & `hfttai-0.1.3/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/langchain.py` & `hfttai-0.1.3/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/open_assistant.py` & `hfttai-0.1.3/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/openai.py` & `hfttai-0.1.3/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/llm/starcoder.py` & `hfttai-0.1.3/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/middlewares/base.py` & `hfttai-0.1.3/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/middlewares/charts.py` & `hfttai-0.1.3/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/middlewares/streamlit.py` & `hfttai-0.1.3/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/prompts/__pycache__/base.cpython-311.pyc` & `hfttai-0.1.3/pandasai/prompts/__pycache__/base.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,128 +1,129 @@
 magic:    0xa70d0d0a
-moddate:  0xaaaa6e64 (Thu May 25 00:24:10 2023 UTC)
-files sz: 430
+moddate:  0x26d2a764 (Fri Jul  7 08:51:50 2023 UTC)
+files sz: 647
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970064005a00640164026c016d025a02010002004700640384006404a6
       020000ab0200000000000000005a0364055300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (' Base class to implement a new Prompt ')
+     1           2 LOAD_CONST               0 (' Base class to implement a new Prompt\nIn order to better handle the instructions, this prompt module is written.\n')
                  4 STORE_NAME               0 (__doc__)
    
-     3           6 LOAD_CONST               1 (0)
+     5           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('MethodNotImplementedError',))
                 10 IMPORT_NAME              1 (pandasai.exceptions)
                 12 IMPORT_FROM              2 (MethodNotImplementedError)
                 14 STORE_NAME               2 (MethodNotImplementedError)
                 16 POP_TOP
    
-     6          18 PUSH_NULL
+     8          18 PUSH_NULL
                 20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               3 (<code object Prompt, file "D:\Pro\pandas-ai-main\pandasai\prompts\base.py", line 6>)
+                22 LOAD_CONST               3 (<code object Prompt, file "D:\Pro\pandas-ai-main\pandasai\prompts\base.py", line 8>)
                 24 MAKE_FUNCTION            0
                 26 LOAD_CONST               4 ('Prompt')
                 28 PRECALL                  2
                 32 CALL                     2
                 42 STORE_NAME               3 (Prompt)
                 44 LOAD_CONST               5 (None)
                 46 RETURN_VALUE
    consts
-      ' Base class to implement a new Prompt '
+      ' Base class to implement a new Prompt\nIn order to better handle the instructions, this prompt module is written.\n'
       0
       ('MethodNotImplementedError',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0469005a05640384005a0664
             0484005a0764025300
-           6           0 RESUME                   0
+           8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Prompt')
                        8 STORE_NAME               2 (__qualname__)
          
-           7          10 LOAD_CONST               1 ('Base class to implement a new Prompt')
+           9          10 LOAD_CONST               1 ('Base class to implement a new Prompt')
                       12 STORE_NAME               3 (__doc__)
          
-           9          14 LOAD_CONST               2 (None)
+          11          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (text)
          
-          10          18 BUILD_MAP                0
+          12          18 BUILD_MAP                0
                       20 STORE_NAME               5 (_args)
          
-          12          22 LOAD_CONST               3 (<code object __init__, file "D:\Pro\pandas-ai-main\pandasai\prompts\base.py", line 12>)
+          14          22 LOAD_CONST               3 (<code object __init__, file "D:\Pro\pandas-ai-main\pandasai\prompts\base.py", line 14>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (__init__)
          
-          16          28 LOAD_CONST               4 (<code object __str__, file "D:\Pro\pandas-ai-main\pandasai\prompts\base.py", line 16>)
+          23          28 LOAD_CONST               4 (<code object __str__, file "D:\Pro\pandas-ai-main\pandasai\prompts\base.py", line 23>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               7 (__str__)
                       34 LOAD_CONST               2 (None)
                       36 RETURN_VALUE
          consts
             'Prompt'
             'Base class to implement a new Prompt'
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 2
                flags     : 11
-               code 0x97007c0172097c017c005f0000000000000000006400530064005300
-                12           0 RESUME                   0
+               code 0x97007c0172097c017c005f0000000000000000006401530064015300
+                14           0 RESUME                   0
                
-                13           2 LOAD_FAST                1 (kwargs)
+                20           2 LOAD_FAST                1 (kwargs)
                              4 POP_JUMP_FORWARD_IF_FALSE     9 (to 24)
                
-                14           6 LOAD_FAST                1 (kwargs)
+                21           6 LOAD_FAST                1 (kwargs)
                              8 LOAD_FAST                0 (self)
                             10 STORE_ATTR               0 (_args)
-                            20 LOAD_CONST               0 (None)
+                            20 LOAD_CONST               1 (None)
                             22 RETURN_VALUE
                
-                13     >>   24 LOAD_CONST               0 (None)
+                20     >>   24 LOAD_CONST               1 (None)
                             26 RETURN_VALUE
                consts
+                  '\n        __init__ method of Base class of Prompt Module\n        Args:\n            **kwargs: Inferred Keyword Arguments\n        '
                   None
                names      ('_args',)
                varnames   ('self', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\base.py'
                name       '__init__'
-               firstlineno 12
-               lnotab 0x0201040112ff
+               firstlineno 14
+               lnotab 0x0206040112ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000800774020000000000000000000082
                   0102007c006a0000000000000000006a020000000000000000640169007c
                   006a030000000000000000a4018e015300
-                16           0 RESUME                   0
+                23           0 RESUME                   0
                
-                17           2 LOAD_FAST                0 (self)
+                24           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text)
                             14 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 30)
                
-                18          16 LOAD_GLOBAL              2 (MethodNotImplementedError)
+                25          16 LOAD_GLOBAL              2 (MethodNotImplementedError)
                             28 RAISE_VARARGS            1
                
-                20     >>   30 PUSH_NULL
+                27     >>   30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                0 (text)
                             44 LOAD_ATTR                2 (format)
                             54 LOAD_CONST               1 (())
                             56 BUILD_MAP                0
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                3 (_args)
@@ -134,27 +135,27 @@
                   ()
                names      ('text', 'MethodNotImplementedError', 'format', '_args')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\base.py'
                name       '__str__'
-               firstlineno 16
+               firstlineno 23
                lnotab 0x02010e010e02
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'text', '_args', '__init__', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\base.py'
          name       'Prompt'
-         firstlineno 6
-         lnotab 0x0a010402040104020604
+         firstlineno 8
+         lnotab 0x0a010402040104020609
       'Prompt'
       None
    names      ('__doc__', 'pandasai.exceptions', 'MethodNotImplementedError', 'Prompt')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\base.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104020c03
+   lnotab 0x00ff020104040c03
```

### Comparing `hfttai-0.1.2/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc` & `hfttai-0.1.3/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,172 +1,153 @@
 magic:    0xa70d0d0a
-moddate:  0xaaaa6e64 (Thu May 25 00:24:10 2023 UTC)
-files sz: 1069
+moddate:  0x26d2a764 (Fri Jul  7 08:51:50 2023 UTC)
+files sz: 1270
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x970064005a00640164026c016d025a020100640164036c036d045a046d
-      055a050100640464056c066d075a070100020047006406840064076507a6
-      030000ab0300000000000000005a0864085300
+      0x970064005a00640164026c016d025a020100640364046c036d045a0401
+      00020047006405840064066504a6030000ab0300000000000000005a0564
+      075300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (' Prompt to correct error ')
+     1           2 LOAD_CONST               0 (' Prompt to correct Python Code on Error\n```\nToday is {today_date}.\nYou are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.\nThis is the metadata of the dataframe:\n{df_head}.\n\nThe user asked the following question:\n{question}\n\nYou generated this python code:\n{code}\n\nIt fails with the following error:\n{error_returned}\n\nCorrect the python code and return a new python code (do not import anything) that fixes the above\nmentioned error. Do not generate the same code again.\n```\n')
                  4 STORE_NAME               0 (__doc__)
    
-     3           6 LOAD_CONST               1 (0)
+    21           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('date',))
                 10 IMPORT_NAME              1 (datetime)
                 12 IMPORT_FROM              2 (date)
                 14 STORE_NAME               2 (date)
                 16 POP_TOP
    
-     5          18 LOAD_CONST               1 (0)
-                20 LOAD_CONST               3 (('END_CODE_TAG', 'START_CODE_TAG'))
-                22 IMPORT_NAME              3 (pandasai.constants)
-                24 IMPORT_FROM              4 (END_CODE_TAG)
-                26 STORE_NAME               4 (END_CODE_TAG)
-                28 IMPORT_FROM              5 (START_CODE_TAG)
-                30 STORE_NAME               5 (START_CODE_TAG)
-                32 POP_TOP
+    23          18 LOAD_CONST               3 (1)
+                20 LOAD_CONST               4 (('Prompt',))
+                22 IMPORT_NAME              3 (base)
+                24 IMPORT_FROM              4 (Prompt)
+                26 STORE_NAME               4 (Prompt)
+                28 POP_TOP
    
-     7          34 LOAD_CONST               4 (1)
-                36 LOAD_CONST               5 (('Prompt',))
-                38 IMPORT_NAME              6 (base)
-                40 IMPORT_FROM              7 (Prompt)
-                42 STORE_NAME               7 (Prompt)
-                44 POP_TOP
-   
-    10          46 PUSH_NULL
-                48 LOAD_BUILD_CLASS
-                50 LOAD_CONST               6 (<code object CorrectErrorPrompt, file "D:\Pro\pandas-ai-main\pandasai\prompts\correct_error_prompt.py", line 10>)
-                52 MAKE_FUNCTION            0
-                54 LOAD_CONST               7 ('CorrectErrorPrompt')
-                56 LOAD_NAME                7 (Prompt)
-                58 PRECALL                  3
-                62 CALL                     3
-                72 STORE_NAME               8 (CorrectErrorPrompt)
-                74 LOAD_CONST               8 (None)
-                76 RETURN_VALUE
+    26          30 PUSH_NULL
+                32 LOAD_BUILD_CLASS
+                34 LOAD_CONST               5 (<code object CorrectErrorPrompt, file "D:\Pro\pandas-ai-main\pandasai\prompts\correct_error_prompt.py", line 26>)
+                36 MAKE_FUNCTION            0
+                38 LOAD_CONST               6 ('CorrectErrorPrompt')
+                40 LOAD_NAME                4 (Prompt)
+                42 PRECALL                  3
+                46 CALL                     3
+                56 STORE_NAME               5 (CorrectErrorPrompt)
+                58 LOAD_CONST               7 (None)
+                60 RETURN_VALUE
    consts
-      ' Prompt to correct error '
+      ' Prompt to correct Python Code on Error\n```\nToday is {today_date}.\nYou are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.\nThis is the metadata of the dataframe:\n{df_head}.\n\nThe user asked the following question:\n{question}\n\nYou generated this python code:\n{code}\n\nIt fails with the following error:\n{error_returned}\n\nCorrect the python code and return a new python code (do not import anything) that fixes the above\nmentioned error. Do not generate the same code again.\n```\n'
       0
       ('date',)
-      ('END_CODE_TAG', 'START_CODE_TAG')
       1
       ('Prompt',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a02550064015a0364025a046505650664033c
             00000088006601640484085a07880078015a085300
                        0 MAKE_CELL                0 (__class__)
          
-          10           2 RESUME                   0
+          26           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('CorrectErrorPrompt')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-          11          14 LOAD_CONST               1 ('Prompt to generate Python code')
+          27          14 LOAD_CONST               1 ('Prompt to Correct Python code on Error')
                       16 STORE_NAME               3 (__doc__)
          
-          13          18 LOAD_CONST               2 ('\nToday is {today_date}.\nYou are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.\nThis is the result of `print(df.head({rows_to_display}))`:\n{df_head}.\n\nThe user asked the following question:\n{question}\n\nYou generated this python code:\n{code}\n\nIt fails with the following error:\n{error_returned}\n\nCorrect the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.\nMake sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.\n')
+          29          18 LOAD_CONST               2 ('\nToday is {today_date}.\nYou are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.\nThis is the metadata of the dataframe:\n{df_head}.\n\nThe user asked the following question:\n{question}\n\nYou generated this python code:\n{code}\n\nIt fails with the following error:\n{error_returned}\n\nCorrect the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.\n')
                       20 STORE_NAME               4 (text)
                       22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                6 (__annotations__)
                       26 LOAD_CONST               3 ('text')
                       28 STORE_SUBSCR
          
-          32          32 LOAD_CLOSURE             0 (__class__)
+          47          32 LOAD_CLOSURE             0 (__class__)
                       34 BUILD_TUPLE              1
-                      36 LOAD_CONST               4 (<code object __init__, file "D:\Pro\pandas-ai-main\pandasai\prompts\correct_error_prompt.py", line 32>)
+                      36 LOAD_CONST               4 (<code object __init__, file "D:\Pro\pandas-ai-main\pandasai\prompts\correct_error_prompt.py", line 47>)
                       38 MAKE_FUNCTION            8 (closure)
                       40 STORE_NAME               7 (__init__)
                       42 LOAD_CLOSURE             0 (__class__)
                       44 COPY                     1
                       46 STORE_NAME               8 (__classcell__)
                       48 RETURN_VALUE
          consts
             'CorrectErrorPrompt'
-            'Prompt to generate Python code'
-            '\nToday is {today_date}.\nYou are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.\nThis is the result of `print(df.head({rows_to_display}))`:\n{df_head}.\n\nThe user asked the following question:\n{question}\n\nYou generated this python code:\n{code}\n\nIt fails with the following error:\n{error_returned}\n\nCorrect the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.\nMake sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.\n'
+            'Prompt to Correct Python code on Error'
+            '\nToday is {today_date}.\nYou are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.\nThis is the metadata of the dataframe:\n{df_head}.\n\nThe user asked the following question:\n{question}\n\nYou generated this python code:\n{code}\n\nIt fails with the following error:\n{error_returned}\n\nCorrect the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.\n'
             'text'
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 8
+               stacksize : 7
                flags     : 11
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
-                  0000006a010000000000000000640269007c01a401740400000000000000
-                  0000007406000000000000000000007409000000000000000000006a0500
-                  00000000000000a6000000ab00000000000000000064019c03a4018e0101
-                  0064005300
+                  0000006a010000000000000000640269007c01a401640174050000000000
+                  00000000006a030000000000000000a6000000ab00000000000000000069
+                  01a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-                32           2 RESUME                   0
+                47           2 RESUME                   0
                
-                33           4 PUSH_NULL
+                48           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_CONST               2 (())
                             44 BUILD_MAP                0
-               
-                34          46 LOAD_FAST                1 (kwargs)
-               
-                33          48 DICT_MERGE               1
-               
-                35          50 LOAD_GLOBAL              4 (START_CODE_TAG)
-               
-                36          62 LOAD_GLOBAL              6 (END_CODE_TAG)
-               
-                37          74 LOAD_GLOBAL              9 (NULL + date)
-                            86 LOAD_ATTR                5 (today)
-                            96 PRECALL                  0
-                           100 CALL                     0
-               
-                33         110 LOAD_CONST               1 (('START_CODE_TAG', 'END_CODE_TAG', 'today_date'))
-                           112 BUILD_CONST_KEY_MAP      3
-                           114 DICT_MERGE               1
-                           116 CALL_FUNCTION_EX         1
-                           118 POP_TOP
-                           120 LOAD_CONST               0 (None)
-                           122 RETURN_VALUE
+                            46 LOAD_FAST                1 (kwargs)
+                            48 DICT_MERGE               1
+                            50 LOAD_CONST               1 ('today_date')
+                            52 LOAD_GLOBAL              5 (NULL + date)
+                            64 LOAD_ATTR                3 (today)
+                            74 PRECALL                  0
+                            78 CALL                     0
+                            88 BUILD_MAP                1
+                            90 DICT_MERGE               1
+                            92 CALL_FUNCTION_EX         1
+                            94 POP_TOP
+                            96 LOAD_CONST               0 (None)
+                            98 RETURN_VALUE
                consts
                   None
-                  ('START_CODE_TAG', 'END_CODE_TAG', 'today_date')
+                  'today_date'
                   ()
-               names      ('super', '__init__', 'START_CODE_TAG', 'END_CODE_TAG', 'date', 'today')
+               names      ('super', '__init__', 'date', 'today')
                varnames   ('self', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\correct_error_prompt.py'
                name       '__init__'
-               firstlineno 32
-               lnotab 0x04012a0102ff02020c010c0124fc
+               firstlineno 47
+               lnotab 0x0401
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'text', 'str', '__annotations__', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\correct_error_prompt.py'
          name       'CorrectErrorPrompt'
-         firstlineno 10
-         lnotab 0x0e0104020e13
+         firstlineno 26
+         lnotab 0x0e0104020e12
       'CorrectErrorPrompt'
       None
-   names      ('__doc__', 'datetime', 'date', 'pandasai.constants', 'END_CODE_TAG', 'START_CODE_TAG', 'base', 'Prompt', 'CorrectErrorPrompt')
+   names      ('__doc__', 'datetime', 'date', 'base', 'Prompt', 'CorrectErrorPrompt')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\correct_error_prompt.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104020c0210020c03
+   lnotab 0x00ff020104140c020c03
```

### Comparing `hfttai-0.1.2/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc` & `hfttai-0.1.3/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,64 +1,64 @@
 magic:    0xa70d0d0a
-moddate:  0xaaaa6e64 (Thu May 25 00:24:10 2023 UTC)
-files sz: 352
+moddate:  0x26d2a764 (Fri Jul  7 08:51:50 2023 UTC)
+files sz: 460
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a0201000200470064038400640465
       02a6030000ab0300000000000000005a0364055300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (' Prompt to generate the response to the question in a conversational way ')
+     1           2 LOAD_CONST               0 (' Prompt to generate the response to the question in a conversational way\n```\nQuestion: {question}\nAnswer: {answer}\n\nRewrite the answer to the question in a conversational way.\n```\n\n')
                  4 STORE_NAME               0 (__doc__)
    
-     3           6 LOAD_CONST               1 (1)
+    11           6 LOAD_CONST               1 (1)
                  8 LOAD_CONST               2 (('Prompt',))
                 10 IMPORT_NAME              1 (base)
                 12 IMPORT_FROM              2 (Prompt)
                 14 STORE_NAME               2 (Prompt)
                 16 POP_TOP
    
-     6          18 PUSH_NULL
+    14          18 PUSH_NULL
                 20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               3 (<code object GenerateResponsePrompt, file "D:\Pro\pandas-ai-main\pandasai\prompts\generate_response.py", line 6>)
+                22 LOAD_CONST               3 (<code object GenerateResponsePrompt, file "D:\Pro\pandas-ai-main\pandasai\prompts\generate_response.py", line 14>)
                 24 MAKE_FUNCTION            0
                 26 LOAD_CONST               4 ('GenerateResponsePrompt')
                 28 LOAD_NAME                2 (Prompt)
                 30 PRECALL                  3
                 34 CALL                     3
                 44 STORE_NAME               3 (GenerateResponsePrompt)
                 46 LOAD_CONST               5 (None)
                 48 RETURN_VALUE
    consts
-      ' Prompt to generate the response to the question in a conversational way '
+      ' Prompt to generate the response to the question in a conversational way\n```\nQuestion: {question}\nAnswer: {answer}\n\nRewrite the answer to the question in a conversational way.\n```\n\n'
       1
       ('Prompt',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a02550064015a0364025a046505650664033c0000
             0064045300
-           6           0 RESUME                   0
+          14           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GenerateResponsePrompt')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-           7          12 LOAD_CONST               1 ('Prompt to generate the response to the question in a conversational way')
+          15          12 LOAD_CONST               1 ('Prompt to generate the response to the question in a conversational way')
                       14 STORE_NAME               3 (__doc__)
          
-           9          16 LOAD_CONST               2 ('\nQuestion: {question}\nAnswer: {answer}\n\nRewrite the answer to the question in a conversational way.\n')
+          17          16 LOAD_CONST               2 ('\nQuestion: {question}\nAnswer: {answer}\n\nRewrite the answer to the question in a conversational way.\n')
                       18 STORE_NAME               4 (text)
                       20 LOAD_NAME                5 (str)
                       22 LOAD_NAME                6 (__annotations__)
                       24 LOAD_CONST               3 ('text')
                       26 STORE_SUBSCR
                       30 LOAD_CONST               4 (None)
                       32 RETURN_VALUE
@@ -70,19 +70,19 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'text', 'str', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\generate_response.py'
          name       'GenerateResponsePrompt'
-         firstlineno 6
+         firstlineno 14
          lnotab 0x0c010402
       'GenerateResponsePrompt'
       None
    names      ('__doc__', 'base', 'Prompt', 'GenerateResponsePrompt')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Pro\\pandas-ai-main\\pandasai\\prompts\\generate_response.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104020c03
+   lnotab 0x00ff0201040a0c03
```

### Comparing `hfttai-0.1.2/pandasai/prompts/base.py` & `hfttai-0.1.3/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/prompts/correct_error_prompt.py` & `hfttai-0.1.3/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/prompts/correct_multiples_prompt.py` & `hfttai-0.1.3/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/prompts/generate_python_code.py` & `hfttai-0.1.3/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pandasai/prompts/multiple_dataframes.py` & `hfttai-0.1.3/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/pyproject.toml` & `hfttai-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hfttai"
-version = "0.1.2"
+version = "0.1.3"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `hfttai-0.1.2/README.md` & `hfttai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.2/PKG-INFO` & `hfttai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfttai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

