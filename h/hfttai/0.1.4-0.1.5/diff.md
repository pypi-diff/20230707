# Comparing `tmp/hfttai-0.1.4.tar.gz` & `tmp/hfttai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfttai-0.1.4.tar", max compression
+gzip compressed data, was "hfttai-0.1.5.tar", max compression
```

## Comparing `hfttai-0.1.4.tar` & `hfttai-0.1.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1055 2023-07-07 08:51:50.000000 hfttai-0.1.4/LICENSE
--rw-r--r--   0        0        0    25251 2023-07-07 13:34:59.248524 hfttai-0.1.4/pandasai/__init__.py
--rw-r--r--   0        0        0     1235 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0      159 2023-07-07 11:43:18.700269 hfttai-0.1.4/pandasai/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4372 2023-07-07 11:43:18.702263 hfttai-0.1.4/pandasai/helpers/__pycache__/_optional.cpython-311.pyc
--rw-r--r--   0        0        0     7796 2023-07-07 11:43:18.705256 hfttai-0.1.4/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc
--rw-r--r--   0        0        0     3375 2023-07-07 11:43:18.708266 hfttai-0.1.4/pandasai/helpers/__pycache__/cache.cpython-311.pyc
--rw-r--r--   0        0        0     1019 2023-05-26 02:00:56.795406 hfttai-0.1.4/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc
--rw-r--r--   0        0        0     2334 2023-07-07 11:43:18.713235 hfttai-0.1.4/pandasai/helpers/__pycache__/notebook.cpython-311.pyc
--rw-r--r--   0        0        0     5526 2023-07-07 11:43:20.132058 hfttai-0.1.4/pandasai/helpers/__pycache__/save_chart.cpython-311.pyc
--rw-r--r--   0        0        0    13373 2023-07-07 11:43:20.135050 hfttai-0.1.4/pandasai/helpers/__pycache__/shortcuts.cpython-311.pyc
--rw-r--r--   0        0        0     3814 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3471 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/__init__.py
--rw-r--r--   0        0        0      155 2023-07-07 11:43:20.138042 hfttai-0.1.4/pandasai/llm/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5613 2023-05-26 02:00:56.832306 hfttai-0.1.4/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc
--rw-r--r--   0        0        0    16066 2023-07-07 11:43:20.142031 hfttai-0.1.4/pandasai/llm/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1450 2023-05-26 02:00:56.817346 hfttai-0.1.4/pandasai/llm/__pycache__/fake.cpython-311.pyc
--rw-r--r--   0        0        0     2506 2023-05-26 02:00:56.878184 hfttai-0.1.4/pandasai/llm/__pycache__/google_palm.cpython-311.pyc
--rw-r--r--   0        0        0     1481 2023-07-07 11:43:20.757703 hfttai-0.1.4/pandasai/llm/__pycache__/langchain.cpython-311.pyc
--rw-r--r--   0        0        0     4711 2023-07-07 11:47:40.378877 hfttai-0.1.4/pandasai/llm/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0     1615 2023-05-26 02:00:56.899128 hfttai-0.1.4/pandasai/llm/__pycache__/starcoder.cpython-311.pyc
--rw-r--r--   0        0        0     4335 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11156 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3176 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      163 2023-07-07 11:43:20.760693 hfttai-0.1.4/pandasai/middlewares/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1529 2023-07-07 11:43:20.762689 hfttai-0.1.4/pandasai/middlewares/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1710 2023-07-07 11:43:20.764521 hfttai-0.1.4/pandasai/middlewares/__pycache__/charts.cpython-311.pyc
--rw-r--r--   0        0        0      663 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      159 2023-07-07 11:43:20.751742 hfttai-0.1.4/pandasai/prompts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1274 2023-07-07 11:43:20.754709 hfttai-0.1.4/pandasai/prompts/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     2060 2023-07-07 11:43:20.768114 hfttai-0.1.4/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc
--rw-r--r--   0        0        0     2107 2023-07-07 11:43:20.770111 hfttai-0.1.4/pandasai/prompts/__pycache__/correct_multiples_prompt.cpython-311.pyc
--rw-r--r--   0        0        0     1876 2023-07-07 11:43:20.773104 hfttai-0.1.4/pandasai/prompts/__pycache__/generate_python_code.cpython-311.pyc
--rw-r--r--   0        0        0      938 2023-07-07 11:43:20.775099 hfttai-0.1.4/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc
--rw-r--r--   0        0        0     2184 2023-07-07 11:43:20.778091 hfttai-0.1.4/pandasai/prompts/__pycache__/multiple_dataframes.cpython-311.pyc
--rw-r--r--   0        0        0      647 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1270 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1076 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1081 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1072 2023-07-07 08:51:50.000000 hfttai-0.1.4/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1898 2023-07-07 13:35:08.306901 hfttai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7705 2023-07-07 08:51:50.000000 hfttai-0.1.4/README.md
--rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 hfttai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-07 08:51:50.000000 hfttai-0.1.5/LICENSE
+-rw-r--r--   0        0        0    25249 2023-07-07 13:41:28.761523 hfttai-0.1.5/pandasai/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-07 11:43:18.700269 hfttai-0.1.5/pandasai/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4372 2023-07-07 11:43:18.702263 hfttai-0.1.5/pandasai/helpers/__pycache__/_optional.cpython-311.pyc
+-rw-r--r--   0        0        0     7796 2023-07-07 11:43:18.705256 hfttai-0.1.5/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc
+-rw-r--r--   0        0        0     3375 2023-07-07 11:43:18.708266 hfttai-0.1.5/pandasai/helpers/__pycache__/cache.cpython-311.pyc
+-rw-r--r--   0        0        0     1019 2023-05-26 02:00:56.795406 hfttai-0.1.5/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc
+-rw-r--r--   0        0        0     2334 2023-07-07 11:43:18.713235 hfttai-0.1.5/pandasai/helpers/__pycache__/notebook.cpython-311.pyc
+-rw-r--r--   0        0        0     5526 2023-07-07 11:43:20.132058 hfttai-0.1.5/pandasai/helpers/__pycache__/save_chart.cpython-311.pyc
+-rw-r--r--   0        0        0    13373 2023-07-07 11:43:20.135050 hfttai-0.1.5/pandasai/helpers/__pycache__/shortcuts.cpython-311.pyc
+-rw-r--r--   0        0        0     3814 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3471 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-07 11:43:20.138042 hfttai-0.1.5/pandasai/llm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5613 2023-05-26 02:00:56.832306 hfttai-0.1.5/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc
+-rw-r--r--   0        0        0    16066 2023-07-07 11:43:20.142031 hfttai-0.1.5/pandasai/llm/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1450 2023-05-26 02:00:56.817346 hfttai-0.1.5/pandasai/llm/__pycache__/fake.cpython-311.pyc
+-rw-r--r--   0        0        0     2506 2023-05-26 02:00:56.878184 hfttai-0.1.5/pandasai/llm/__pycache__/google_palm.cpython-311.pyc
+-rw-r--r--   0        0        0     1481 2023-07-07 11:43:20.757703 hfttai-0.1.5/pandasai/llm/__pycache__/langchain.cpython-311.pyc
+-rw-r--r--   0        0        0     4711 2023-07-07 11:47:40.378877 hfttai-0.1.5/pandasai/llm/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0     1615 2023-05-26 02:00:56.899128 hfttai-0.1.5/pandasai/llm/__pycache__/starcoder.cpython-311.pyc
+-rw-r--r--   0        0        0     4335 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11156 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3176 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-07 11:43:20.760693 hfttai-0.1.5/pandasai/middlewares/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1529 2023-07-07 11:43:20.762689 hfttai-0.1.5/pandasai/middlewares/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1710 2023-07-07 11:43:20.764521 hfttai-0.1.5/pandasai/middlewares/__pycache__/charts.cpython-311.pyc
+-rw-r--r--   0        0        0      663 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-07 11:43:20.751742 hfttai-0.1.5/pandasai/prompts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1274 2023-07-07 11:43:20.754709 hfttai-0.1.5/pandasai/prompts/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     2060 2023-07-07 11:43:20.768114 hfttai-0.1.5/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc
+-rw-r--r--   0        0        0     2107 2023-07-07 11:43:20.770111 hfttai-0.1.5/pandasai/prompts/__pycache__/correct_multiples_prompt.cpython-311.pyc
+-rw-r--r--   0        0        0     1876 2023-07-07 11:43:20.773104 hfttai-0.1.5/pandasai/prompts/__pycache__/generate_python_code.cpython-311.pyc
+-rw-r--r--   0        0        0      938 2023-07-07 11:43:20.775099 hfttai-0.1.5/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc
+-rw-r--r--   0        0        0     2184 2023-07-07 11:43:20.778091 hfttai-0.1.5/pandasai/prompts/__pycache__/multiple_dataframes.cpython-311.pyc
+-rw-r--r--   0        0        0      647 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1270 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1076 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1081 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1072 2023-07-07 08:51:50.000000 hfttai-0.1.5/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1898 2023-07-07 13:41:37.594050 hfttai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7705 2023-07-07 08:51:50.000000 hfttai-0.1.5/README.md
+-rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 hfttai-0.1.5/PKG-INFO
```

### Comparing `hfttai-0.1.4/LICENSE` & `hfttai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/__init__.py` & `hfttai-0.1.5/pandasai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 def get_version():
     """
     Get the version from the package metadata
     """
     from importlib.metadata import version
 
-    return version("pandasai")
+    return version("hfttai")
 
 
 __version__ = get_version()
 
 
 class PandasAI(Shortcuts):
     """
```

### Comparing `hfttai-0.1.4/pandasai/constants.py` & `hfttai-0.1.5/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/exceptions.py` & `hfttai-0.1.5/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/__pycache__/_optional.cpython-311.pyc` & `hfttai-0.1.5/pandasai/helpers/__pycache__/_optional.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc` & `hfttai-0.1.5/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/__pycache__/cache.cpython-311.pyc` & `hfttai-0.1.5/pandasai/helpers/__pycache__/cache.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc` & `hfttai-0.1.5/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/__pycache__/notebook.cpython-311.pyc` & `hfttai-0.1.5/pandasai/helpers/__pycache__/notebook.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/__pycache__/save_chart.cpython-311.pyc` & `hfttai-0.1.5/pandasai/helpers/__pycache__/save_chart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/__pycache__/shortcuts.cpython-311.pyc` & `hfttai-0.1.5/pandasai/helpers/__pycache__/shortcuts.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/_optional.py` & `hfttai-0.1.5/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/anonymizer.py` & `hfttai-0.1.5/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/cache.py` & `hfttai-0.1.5/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/from_excel.py` & `hfttai-0.1.5/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/notebook.py` & `hfttai-0.1.5/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/save_chart.py` & `hfttai-0.1.5/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/helpers/shortcuts.py` & `hfttai-0.1.5/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc` & `hfttai-0.1.5/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/__pycache__/base.cpython-311.pyc` & `hfttai-0.1.5/pandasai/llm/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/__pycache__/fake.cpython-311.pyc` & `hfttai-0.1.5/pandasai/llm/__pycache__/fake.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/__pycache__/google_palm.cpython-311.pyc` & `hfttai-0.1.5/pandasai/llm/__pycache__/google_palm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/__pycache__/langchain.cpython-311.pyc` & `hfttai-0.1.5/pandasai/llm/__pycache__/langchain.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/__pycache__/openai.cpython-311.pyc` & `hfttai-0.1.5/pandasai/llm/__pycache__/openai.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/__pycache__/starcoder.cpython-311.pyc` & `hfttai-0.1.5/pandasai/llm/__pycache__/starcoder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/azure_openai.py` & `hfttai-0.1.5/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/base.py` & `hfttai-0.1.5/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/fake.py` & `hfttai-0.1.5/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/falcon.py` & `hfttai-0.1.5/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/google_palm.py` & `hfttai-0.1.5/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/langchain.py` & `hfttai-0.1.5/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/open_assistant.py` & `hfttai-0.1.5/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/openai.py` & `hfttai-0.1.5/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/llm/starcoder.py` & `hfttai-0.1.5/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/middlewares/__pycache__/base.cpython-311.pyc` & `hfttai-0.1.5/pandasai/middlewares/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/middlewares/__pycache__/charts.cpython-311.pyc` & `hfttai-0.1.5/pandasai/middlewares/__pycache__/charts.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/middlewares/base.py` & `hfttai-0.1.5/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/middlewares/charts.py` & `hfttai-0.1.5/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/middlewares/streamlit.py` & `hfttai-0.1.5/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/__pycache__/base.cpython-311.pyc` & `hfttai-0.1.5/pandasai/prompts/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc` & `hfttai-0.1.5/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/__pycache__/correct_multiples_prompt.cpython-311.pyc` & `hfttai-0.1.5/pandasai/prompts/__pycache__/correct_multiples_prompt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/__pycache__/generate_python_code.cpython-311.pyc` & `hfttai-0.1.5/pandasai/prompts/__pycache__/generate_python_code.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc` & `hfttai-0.1.5/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/__pycache__/multiple_dataframes.cpython-311.pyc` & `hfttai-0.1.5/pandasai/prompts/__pycache__/multiple_dataframes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/base.py` & `hfttai-0.1.5/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/correct_error_prompt.py` & `hfttai-0.1.5/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/correct_multiples_prompt.py` & `hfttai-0.1.5/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/generate_python_code.py` & `hfttai-0.1.5/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pandasai/prompts/multiple_dataframes.py` & `hfttai-0.1.5/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/pyproject.toml` & `hfttai-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hfttai"
-version = "0.1.4"
+version = "0.1.5"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `hfttai-0.1.4/README.md` & `hfttai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hfttai-0.1.4/PKG-INFO` & `hfttai-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfttai
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

