# Comparing `tmp/hfttai-0.1.0.tar.gz` & `tmp/hfttai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfttai-0.1.0.tar", max compression
+gzip compressed data, was "hfttai-0.1.2.tar", max compression
```

## Comparing `hfttai-0.1.0.tar` & `hfttai-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,51 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 hfttai-0.1.0/LICENSE
--rw-r--r--   0        0        0    26002 2023-07-07 10:58:51.060953 hfttai-0.1.0/pandasai/__init__.py
--rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 hfttai-0.1.0/pandasai/constants.py
--rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 hfttai-0.1.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 hfttai-0.1.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 hfttai-0.1.0/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 hfttai-0.1.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 hfttai-0.1.0/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 hfttai-0.1.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 hfttai-0.1.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3587 2023-07-07 01:01:47.985267 hfttai-0.1.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 hfttai-0.1.0/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 hfttai-0.1.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 hfttai-0.1.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11573 2023-07-07 10:58:51.061950 hfttai-0.1.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 hfttai-0.1.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 hfttai-0.1.0/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 hfttai-0.1.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 hfttai-0.1.0/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 hfttai-0.1.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3289 2023-07-07 10:58:51.062948 hfttai-0.1.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 hfttai-0.1.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 hfttai-0.1.0/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 hfttai-0.1.0/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 hfttai-0.1.0/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 hfttai-0.1.0/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 hfttai-0.1.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 hfttai-0.1.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1318 2023-07-07 10:58:51.062948 hfttai-0.1.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1120 2023-07-07 10:58:51.063944 hfttai-0.1.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1113 2023-07-07 10:58:51.063944 hfttai-0.1.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 hfttai-0.1.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1108 2023-07-07 10:58:51.064942 hfttai-0.1.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1968 2023-07-07 11:00:42.601535 hfttai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7891 2023-07-07 10:58:51.059956 hfttai-0.1.0/README.md
--rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 hfttai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-07 08:51:50.000000 hfttai-0.1.2/LICENSE
+-rw-r--r--   0        0        0    25266 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-26 02:00:53.639839 hfttai-0.1.2/pandasai/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7444 2023-05-26 02:00:53.642831 hfttai-0.1.2/pandasai/helpers/__pycache__/anonymizer.cpython-311.pyc
+-rw-r--r--   0        0        0     1019 2023-05-26 02:00:56.795406 hfttai-0.1.2/pandasai/helpers/__pycache__/from_excel.cpython-311.pyc
+-rw-r--r--   0        0        0     2337 2023-05-26 02:00:53.645824 hfttai-0.1.2/pandasai/helpers/__pycache__/notebook.cpython-311.pyc
+-rw-r--r--   0        0        0     3814 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3471 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-26 02:00:55.181718 hfttai-0.1.2/pandasai/llm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5613 2023-05-26 02:00:56.832306 hfttai-0.1.2/pandasai/llm/__pycache__/azure_openai.cpython-311.pyc
+-rw-r--r--   0        0        0    13653 2023-05-26 07:42:15.392075 hfttai-0.1.2/pandasai/llm/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1450 2023-05-26 02:00:56.817346 hfttai-0.1.2/pandasai/llm/__pycache__/fake.cpython-311.pyc
+-rw-r--r--   0        0        0     2506 2023-05-26 02:00:56.878184 hfttai-0.1.2/pandasai/llm/__pycache__/google_palm.cpython-311.pyc
+-rw-r--r--   0        0        0     3499 2023-05-26 02:00:56.890152 hfttai-0.1.2/pandasai/llm/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0     1615 2023-05-26 02:00:56.899128 hfttai-0.1.2/pandasai/llm/__pycache__/starcoder.cpython-311.pyc
+-rw-r--r--   0        0        0     4335 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11156 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3176 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     1062 2023-05-26 02:00:56.781443 hfttai-0.1.2/pandasai/prompts/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1876 2023-05-26 02:00:56.779448 hfttai-0.1.2/pandasai/prompts/__pycache__/correct_error_prompt.cpython-311.pyc
+-rw-r--r--   0        0        0     1809 2023-05-28 12:33:38.926133 hfttai-0.1.2/pandasai/prompts/__pycache__/generate_python_code.cpython-311.pyc
+-rw-r--r--   0        0        0      824 2023-05-26 02:00:56.786429 hfttai-0.1.2/pandasai/prompts/__pycache__/generate_response.cpython-311.pyc
+-rw-r--r--   0        0        0      647 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1270 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1076 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1081 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1072 2023-07-07 08:51:50.000000 hfttai-0.1.2/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1898 2023-07-07 11:28:40.525215 hfttai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7705 2023-07-07 08:51:50.000000 hfttai-0.1.2/README.md
+-rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 hfttai-0.1.2/PKG-INFO
```

### Comparing `hfttai-0.1.0/LICENSE` & `hfttai-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Copyright (c) Gabriele Venturi
-
-Permission is hereby granted, free of charge, to any person
-obtaining a copy of this software and associated documentation
-files (the "Software"), to deal in the Software without
-restriction, including without limitation the rights to use,
-copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
+Copyright (c) Gabriele Venturi
+
+Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation
+files (the "Software"), to deal in the Software without
+restriction, including without limitation the rights to use,
+copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hfttai-0.1.0/pandasai/__init__.py` & `hfttai-0.1.2/pandasai/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,736 +1,736 @@
-# -*- coding: utf-8 -*-
-"""
-PandasAI is a wrapper around a LLM to make dataframes conversational
-
-This module includes the implementation of basis  PandasAI class with methods to run
-the LLMs models on Pandas dataframes. Following LLMs are implemented so far.
-
-Example:
-
-    This module is the Entry point of the `pandasai` package. Following is an example
-    of how to use this Class.
-
-    ```python
-    import pandas as pd
-    from pandasai import PandasAI
-
-    # Sample DataFrame
-    df = pd.DataFrame({
-        "country": ["United States", "United Kingdom", "France", "Germany", "Italy",
-        "Spain", "Canada", "Australia", "Japan", "China"],
-        "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832,
-        1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440,
-        14631844184064],
-        "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
-    })
-
-    # Instantiate a LLM
-    from pandasai.llm.openai import OpenAI
-    llm = OpenAI(api_token="YOUR_API_TOKEN")
-
-    pandas_ai = PandasAI(llm)
-    pandas_ai(df, prompt='Which are the 5 happiest countries?')
-
-    ```
-"""
-
-import ast
-import io
-import logging
-import re
-import sys
-import uuid
-import time
-from contextlib import redirect_stdout
-from typing import List, Optional, Union, Dict, Type
-import importlib.metadata
-
-__version__ = importlib.metadata.version(__package__ or __name__)
-import astor
-import pandas as pd
-from .constants import (
-    WHITELISTED_BUILTINS,
-    WHITELISTED_LIBRARIES,
-)
-from .exceptions import BadImportError, LLMNotFoundError
-from .helpers._optional import import_dependency
-from .helpers.anonymizer import anonymize_dataframe_head
-from .helpers.cache import Cache
-from .helpers.notebook import Notebook
-from .helpers.save_chart import add_save_chart
-from .helpers.shortcuts import Shortcuts
-from .llm.base import LLM
-from .llm.langchain import LangchainLLM
-from .middlewares.base import Middleware
-from .middlewares.charts import ChartsMiddleware
-from .prompts.base import Prompt
-from .prompts.correct_error_prompt import CorrectErrorPrompt
-from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
-from .prompts.generate_python_code import GeneratePythonCodePrompt
-from .prompts.generate_response import GenerateResponsePrompt
-from .prompts.multiple_dataframes import MultipleDataframesPrompt
-
-
-def get_version():
-    """
-    Get the version from the package metadata
-    """
-    from importlib.metadata import version
-
-    return version("pandasai")
-
-
-__version__ = get_version()
-
-
-class PandasAI(Shortcuts):
-    """
-    PandasAI is a wrapper around a LLM to make dataframes conversational.
-
-
-    This is an entry point of `pandasai` object. This class consists of methods
-    to interface the LLMs with Pandas     dataframes. A pandas dataframe metadata i.e.
-    df.head() and prompt is passed on to chosen LLMs API end point to generate a Python
-    code to answer the questions asked. The resultant python code is run on actual data
-    and answer is converted into a conversational form.
-
-    Note:
-        Do not include the `self` parameter in the ``Args`` section.
-    Args:
-        _llm (obj): LLMs option to be used for API access
-        _verbose (bool, optional): To show the intermediate outputs e.g. python code
-        generated and execution step on the prompt. Default to False
-        _is_conversational_answer (bool, optional): Whether to return answer in
-        conversational form. Default to False
-        _enforce_privacy (bool, optional): Do not display the data on prompt in case of
-        Sensitive data. Default to False
-        _max_retries (int, optional): max no. of tries to generate code on failure.
-        Default to 3
-        _in_notebook (bool, optional): Whether to run code in notebook. Default to False
-        _original_instructions (dict, optional): The dict of instruction to run. Default
-        to None
-        _cache (Cache, optional): Cache object to store the results. Default to None
-        _enable_cache (bool, optional): Whether to enable cache. Default to True
-        _logger (logging.Logger, optional): Logger object to log the messages. Default
-        to None
-        _logs (List[dict], optional): List of logs to be stored. Default to []
-        _prompt_id (str, optional): Unique ID to differentiate calls. Default to None
-        _middlewares (List[Middleware], optional): List of middlewares to run. Default
-        to [ChartsMiddleware()]
-        _additional_dependencies (List[dict], optional): List of additional dependencies
-        to be added. Default to []
-        _custom_whitelisted_dependencies (List[str], optional): List of custom
-        whitelisted dependencies. Default to []
-        last_code_generated (str, optional): Pass last Code if generated. Default to
-        None
-        last_code_executed (str, optional): Pass the last execution / run. Default to
-        None
-        code_output (str, optional): The code output if any. Default to None
-        last_error (str, optional): Error of running code last time. Default to None
-        prompt_id (str, optional): Unique ID to differentiate calls. Default to None
-
-
-    Returns (str): Response to a Question related to Data
-
-    """
-
-    _llm: LLM
-    _verbose: bool = False
-    _is_conversational_answer: bool = False
-    _enforce_privacy: bool = False
-    _max_retries: int = 3
-    _in_notebook: bool = False
-    _original_instructions: dict = {
-        "question": None,
-        "df_head": None,
-        "num_rows": None,
-        "num_columns": None,
-    }
-    _cache: Cache = None
-    _enable_cache: bool = True
-    _prompt_id: Optional[str] = None
-    _middlewares: List[Middleware] = [ChartsMiddleware()]
-    _additional_dependencies: List[dict] = []
-    _custom_whitelisted_dependencies: List[str] = []
-    _start_time: float = 0
-    _enable_logging: bool = True
-    _logger: logging.Logger = None
-    _logs: List[str] = []
-    last_code_generated: Optional[str] = None
-    last_code_executed: Optional[str] = None
-    code_output: Optional[str] = None
-    last_error: Optional[str] = None
-
-    def __init__(
-        self,
-        llm=None,
-        conversational=False,
-        verbose=False,
-        enforce_privacy=False,
-        save_charts=False,
-        save_charts_path=None,
-        enable_cache=True,
-        middlewares=None,
-        custom_whitelisted_dependencies=None,
-        enable_logging=True,
-        non_default_prompts: Optional[Dict[str, Type[Prompt]]] = None,
-    ):
-        """
-
-        __init__ method of the Class PandasAI
-
-        Args:
-            llm (object): LLMs option to be used for API access. Default is None
-            conversational (bool): Whether to return answer in conversational form.
-            Default to False
-            verbose (bool): To show the intermediate outputs e.g. python code
-            generated and execution step on the prompt.  Default to False
-            enforce_privacy (bool): Execute the codes with Privacy Mode ON.
-            Default to False
-            save_charts (bool): Save the charts generated in the notebook.
-            Default to False
-            enable_cache (bool): Enable the cache to store the results.
-            Default to True
-            middlewares (list): List of middlewares to be used. Default to None
-            custom_whitelisted_dependencies (list): List of custom dependencies to
-            be used. Default to None
-            enable_logging (bool): Enable the logging. Default to True
-            non_default_prompts (dict): Mapping from keys to replacement prompt classes.
-            Used to override specific types of prompts. Defaults to None.
-        """
-
-        # configure the logging
-        # noinspection PyArgumentList
-        # https://stackoverflow.com/questions/61226587/pycharm-does-not-recognize-logging-basicconfig-handlers-argument
-        if enable_logging:
-            handlers = [logging.FileHandler("pandasai.log")]
-        else:
-            handlers = []
-
-        if verbose:
-            handlers.append(logging.StreamHandler(sys.stdout))
-        logging.basicConfig(
-            level=logging.INFO,
-            format="%(asctime)s [%(levelname)s] %(message)s",
-            datefmt="%Y-%m-%d %H:%M:%S",
-            handlers=handlers,
-        )
-        self._logger = logging.getLogger(__name__)
-
-        if llm is None:
-            raise LLMNotFoundError(
-                "An LLM should be provided to instantiate a PandasAI instance"
-            )
-        self._load_llm(llm)
-        self._is_conversational_answer = conversational
-        self._verbose = verbose
-        self._enforce_privacy = enforce_privacy
-        self._save_charts = save_charts
-        self._save_charts_path = save_charts_path
-        self._process_id = str(uuid.uuid4())
-        self._logs = []
-
-        self._non_default_prompts = (
-            {} if non_default_prompts is None else non_default_prompts
-        )
-
-        self.notebook = Notebook()
-        self._in_notebook = self.notebook.in_notebook()
-
-        self._enable_cache = enable_cache
-        if self._enable_cache:
-            self._cache = Cache()
-
-        if middlewares is not None:
-            self.add_middlewares(*middlewares)
-
-        if custom_whitelisted_dependencies is not None:
-            self._custom_whitelisted_dependencies = custom_whitelisted_dependencies
-
-    def _load_llm(self, llm):
-        """
-        Check if it is a PandasAI LLM or a Langchain LLM.
-        If it is a Langchain LLM, wrap it in a PandasAI LLM.
-
-        Args:
-            llm (object): LLMs option to be used for API access
-
-        Raises:
-            BadImportError: If the LLM is a Langchain LLM but the langchain package
-            is not installed
-        """
-
-        try:
-            llm.is_pandasai_llm()
-        except AttributeError:
-            llm = LangchainLLM(llm)
-
-        self._llm = llm
-
-    def conversational_answer(self, question: str, answer: str) -> str:
-        """
-        Returns the answer in conversational form about the resultant data.
-
-        Args:
-            question (str): A question in Conversational form
-            answer (str): A summary / resultant Data
-
-        Returns (str): Response
-
-        """
-
-        if self._enforce_privacy:
-            # we don't want to send potentially sensitive data to the LLM server
-            # if the user has set enforce_privacy to True
-            return answer
-
-        generate_response_instruction = self._non_default_prompts.get(
-            "generate_response", GenerateResponsePrompt
-        )(question=question, answer=answer)
-        return self._llm.call(generate_response_instruction, "")
-
-    def run(
-        self,
-        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
-        prompt: str,
-        is_conversational_answer: bool = None,
-        show_code: bool = False,
-        anonymize_df: bool = True,
-        use_error_correction_framework: bool = True,
-    ) -> Union[str, pd.DataFrame]:
-        """
-        Run the PandasAI to make Dataframes Conversational.
-
-        Args:
-            data_frame (Union[pd.DataFrame, List[pd.DataFrame]]): A pandas Dataframe
-            prompt (str): A prompt to query about the Dataframe
-            is_conversational_answer (bool): Whether to return answer in conversational
-            form. Default to False
-            show_code (bool): To show the intermediate python code generated on the
-            prompt. Default to False
-            anonymize_df (bool): Running the code with Sensitive Data. Default to True
-            use_error_correction_framework (bool): Turn on Error Correction mechanism.
-            Default to True
-
-        Returns (str): Answer to the Input Questions about the DataFrame
-
-        """
-
-        self._start_time = time.time()
-
-        self.log(f"Question: {prompt}")
-        self.log(f"Running PandasAI with {self._llm.type} LLM...")
-
-        self._prompt_id = str(uuid.uuid4())
-        self.log(f"Prompt ID: {self._prompt_id}")
-
-        try:
-            if self._enable_cache and self._cache and self._cache.get(prompt):
-                self.log("Using cached response")
-                code = self._cache.get(prompt)
-            else:
-                rows_to_display = 0 if self._enforce_privacy else 5
-
-                multiple: bool = isinstance(data_frame, list)
-
-                if multiple:
-                    heads = [
-                        anonymize_dataframe_head(dataframe)
-                        if anonymize_df
-                        else dataframe.head(rows_to_display)
-                        for dataframe in data_frame
-                    ]
-
-                    multiple_dataframes_instruction = self._non_default_prompts.get(
-                        "multiple_dataframes", MultipleDataframesPrompt
-                    )
-                    code = self._llm.generate_code(
-                        multiple_dataframes_instruction(dataframes=heads),
-                        prompt,
-                    )
-
-                    self._original_instructions = {
-                        "question": prompt,
-                        "df_head": heads,
-                    }
-
-                else:
-                    df_head = data_frame.head(rows_to_display)
-                    if anonymize_df:
-                        df_head = anonymize_dataframe_head(df_head)
-                    df_head = df_head.to_csv(index=False)
-
-                    generate_code_instruction = self._non_default_prompts.get(
-                        "generate_python_code", GeneratePythonCodePrompt
-                    )(
-                        prompt=prompt,
-                        df_head=df_head,
-                        num_rows=data_frame.shape[0],
-                        num_columns=data_frame.shape[1],
-                    )
-                    code = self._llm.generate_code(
-                        generate_code_instruction,
-                        prompt,
-                    )
-
-                    self._original_instructions = {
-                        "question": prompt,
-                        "df_head": df_head,
-                        "num_rows": data_frame.shape[0],
-                        "num_columns": data_frame.shape[1],
-                    }
-
-                self.last_code_generated = code
-                self.log(
-                    f"""
-                        Code generated:
-                        ```
-                        {code}
-                        ```
-                    """
-                )
-
-                if self._enable_cache and self._cache:
-                    self._cache.set(prompt, code)
-
-            if show_code and self._in_notebook:
-                self.notebook.create_new_cell(code)
-
-            for middleware in self._middlewares:
-                code = middleware(code)
-
-            answer = self.run_code(
-                code,
-                data_frame,
-                use_error_correction_framework=use_error_correction_framework,
-            )
-            self.code_output = answer
-            self.log(f"Answer: {answer}")
-
-            if is_conversational_answer is None:
-                is_conversational_answer = self._is_conversational_answer
-            if is_conversational_answer:
-                answer = self.conversational_answer(prompt, answer)
-                self.log(f"Conversational answer: {answer}")
-
-            self.log(f"Executed in: {time.time() - self._start_time}s")
-
-            return answer
-        except Exception as exception:
-            self.last_error = str(exception)
-            print(exception)
-            return (
-                "Unfortunately, I was not able to answer your question, "
-                "because of the following error:\n"
-                f"\n{exception}\n"
-            )
-
-    def add_middlewares(self, *middlewares: List[Middleware]):
-        """
-        Add middlewares to PandasAI instance.
-
-        Args:
-            *middlewares: A list of middlewares
-
-        """
-        self._middlewares.extend(middlewares)
-
-    def clear_cache(self):
-        """
-        Clears the cache of the PandasAI instance.
-        """
-        if self._cache:
-            self._cache.clear()
-
-    def __call__(
-        self,
-        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
-        prompt: str,
-        is_conversational_answer: bool = None,
-        show_code: bool = False,
-        anonymize_df: bool = True,
-        use_error_correction_framework: bool = True,
-    ) -> Union[str, pd.DataFrame]:
-        """
-        __call__ method of PandasAI class. It calls the `run` method.
-
-        Args:
-            data_frame:
-            prompt:
-            is_conversational_answer:
-            show_code:
-            anonymize_df:
-            use_error_correction_framework:
-
-        Returns (str): Answer to the Input Questions about the DataFrame.
-
-        """
-
-        return self.run(
-            data_frame,
-            prompt,
-            is_conversational_answer,
-            show_code,
-            anonymize_df,
-            use_error_correction_framework,
-        )
-
-    def _check_imports(self, node: Union[ast.Import, ast.ImportFrom]):
-        """
-        Add whitelisted imports to _additional_dependencies.
-
-        Args:
-            node (object): ast.Import or ast.ImportFrom
-
-        Raises:
-            BadImportError: If the import is not whitelisted
-
-        """
-        if isinstance(node, ast.Import):
-            module = node.names[0].name
-        else:
-            module = node.module
-
-        library = module.split(".")[0]
-
-        if library == "pandas":
-            return
-
-        if library in WHITELISTED_LIBRARIES + self._custom_whitelisted_dependencies:
-            for alias in node.names:
-                self._additional_dependencies.append(
-                    {
-                        "module": module,
-                        "name": alias.name,
-                        "alias": alias.asname or alias.name,
-                    }
-                )
-            return
-
-        if library not in WHITELISTED_BUILTINS:
-            raise BadImportError(library)
-
-    def _is_df_overwrite(self, node: ast.stmt) -> bool:
-        """
-        Remove df declarations from the code to prevent malicious code execution.
-
-        Args:
-            node (object): ast.stmt
-
-        Returns (bool):
-
-        """
-
-        return (
-            isinstance(node, ast.Assign)
-            and isinstance(node.targets[0], ast.Name)
-            and re.match(r"df\d{0,2}$", node.targets[0].id)
-        )
-
-    def _clean_code(self, code: str) -> str:
-        """
-        A method to clean the code to prevent malicious code execution
-
-        Args:
-            code(str): A python code
-
-        Returns (str): Returns a Clean Code String
-
-        """
-
-        tree = ast.parse(code)
-
-        new_body = []
-
-        # clear recent optional dependencies
-        self._additional_dependencies = []
-
-        for node in tree.body:
-            if isinstance(node, (ast.Import, ast.ImportFrom)):
-                self._check_imports(node)
-                continue
-            if self._is_df_overwrite(node):
-                continue
-            new_body.append(node)
-
-        new_tree = ast.Module(body=new_body)
-        return astor.to_source(new_tree).strip()
-
-    def _get_environment(self) -> dict:
-        """
-        Returns the environment for the code to be executed.
-
-        Returns (dict): A dictionary of environment variables
-        """
-
-        return {
-            "pd": pd,
-            **{
-                lib["alias"]: getattr(import_dependency(lib["module"]), lib["name"])
-                if hasattr(import_dependency(lib["module"]), lib["name"])
-                else import_dependency(lib["module"])
-                for lib in self._additional_dependencies
-            },
-            "__builtins__": {
-                **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
-            },
-        }
-
-    def _retry_run_code(self, code: str, e: Exception, multiple: bool = False):
-        """
-        A method to retry the code execution with error correction framework.
-
-        Args:
-            code (str): A python code
-            e (Exception): An exception
-            multiple (bool): A boolean to indicate if the code is for multiple
-            dataframes
-
-        Returns (str): A python code
-        """
-
-        if multiple:
-            error_correcting_instruction = self._non_default_prompts.get(
-                "correct_multiple_dataframes_error",
-                CorrectMultipleDataframesErrorPrompt,
-            )(
-                code=code,
-                error_returned=e,
-                question=self._original_instructions["question"],
-                df_head=self._original_instructions["df_head"],
-            )
-
-        else:
-            error_correcting_instruction = self._non_default_prompts.get(
-                "correct_error", CorrectErrorPrompt
-            )(
-                code=code,
-                error_returned=e,
-                question=self._original_instructions["question"],
-                df_head=self._original_instructions["df_head"],
-                num_rows=self._original_instructions["num_rows"],
-                num_columns=self._original_instructions["num_columns"],
-            )
-
-        return self._llm.generate_code(error_correcting_instruction, "")
-
-    def run_code(
-        self,
-        code: str,
-        data_frame: pd.DataFrame,
-        use_error_correction_framework: bool = True,
-    ) -> str:
-        """
-        A method to execute the python code generated by LLMs to answer the question
-        about the input dataframe. Run the code in the current context and return the
-        result.
-
-        Args:
-            code (str): A python code to execute
-            data_frame (pd.DataFrame): A full Pandas DataFrame
-            use_error_correction_framework (bool): Turn on Error Correction mechanism.
-            Default to True
-
-        Returns (str): String representation of the result of the code execution.
-
-        """
-
-        multiple: bool = isinstance(data_frame, list)
-
-        # Add save chart code
-        if self._save_charts:
-            code = add_save_chart(
-                code, self._prompt_id, self._save_charts_path, not self._verbose
-            )
-
-        # Get the code to run removing unsafe imports and df overwrites
-        code_to_run = self._clean_code(code)
-        self.last_code_executed = code_to_run
-        self.log(
-            f"""
-Code running:
-```
-{code_to_run}
-```"""
-        )
-
-        environment: dict = self._get_environment()
-
-        if multiple:
-            environment.update(
-                {f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start=1)}
-            )
-        else:
-            environment["df"] = data_frame
-
-        # Redirect standard output to a StringIO buffer
-        with redirect_stdout(io.StringIO()) as output:
-            count = 0
-            while count < self._max_retries:
-                try:
-                    # Execute the code
-                    exec(code_to_run, environment)
-                    code = code_to_run
-                    break
-                except Exception as e:
-                    if not use_error_correction_framework:
-                        raise e
-
-                    count += 1
-
-                    code_to_run = self._retry_run_code(code, e, multiple)
-
-        captured_output = output.getvalue().strip()
-        if code.count("print(") > 1:
-            return captured_output
-
-        # Evaluate the last line and return its value or the captured output
-        # We do this because we want to return the right value and the right
-        # type of the value. For example, if the last line is `df.head()`, we
-        # want to return the head of the dataframe, not the captured output.
-        lines = code.strip().split("\n")
-        last_line = lines[-1].strip()
-
-        match = re.match(r"^print\((.*)\)$", last_line)
-        if match:
-            last_line = match.group(1)
-
-        try:
-            result = eval(last_line, environment)
-
-            # In some cases, the result is a tuple of values. For example, when
-            # the last line is `print("Hello", "World")`, the result is a tuple
-            # of two strings. In this case, we want to return a string
-            if isinstance(result, tuple):
-                result = " ".join([str(element) for element in result])
-
-            return result
-        except Exception:
-            return captured_output
-
-    def log(self, message: str):
-        """Log a message"""
-        self._logger.info(message)
-        self._logs.append(message)
-
-    @property
-    def logs(self) -> List[str]:
-        """Return the logs"""
-        return self._logs
-
-    def process_id(self) -> str:
-        """Return the id of this PandasAI object."""
-        return self._process_id
-
-    @property
-    def last_prompt_id(self) -> str:
-        """Return the id of the last prompt that was run."""
-        if self._prompt_id is None:
-            raise ValueError("Pandas AI has not been run yet.")
-        return self._prompt_id
-
-    @property
-    def last_prompt(self) -> str:
-        """Return the last prompt that was executed."""
-        if self._llm:
-            return self._llm.last_prompt
+# -*- coding: utf-8 -*-
+"""
+PandasAI is a wrapper around a LLM to make dataframes conversational
+
+This module includes the implementation of basis  PandasAI class with methods to run
+the LLMs models on Pandas dataframes. Following LLMs are implemented so far.
+
+Example:
+
+    This module is the Entry point of the `pandasai` package. Following is an example
+    of how to use this Class.
+
+    ```python
+    import pandas as pd
+    from pandasai import PandasAI
+
+    # Sample DataFrame
+    df = pd.DataFrame({
+        "country": ["United States", "United Kingdom", "France", "Germany", "Italy",
+        "Spain", "Canada", "Australia", "Japan", "China"],
+        "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832,
+        1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440,
+        14631844184064],
+        "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+    })
+
+    # Instantiate a LLM
+    from pandasai.llm.openai import OpenAI
+    llm = OpenAI(api_token="YOUR_API_TOKEN")
+
+    pandas_ai = PandasAI(llm)
+    pandas_ai(df, prompt='Which are the 5 happiest countries?')
+
+    ```
+"""
+
+import ast
+import io
+import logging
+import re
+import sys
+import uuid
+import time
+from contextlib import redirect_stdout
+from typing import List, Optional, Union, Dict, Type
+import importlib.metadata
+
+__version__ = importlib.metadata.version(__package__ or __name__)
+import astor
+import pandas as pd
+from .constants import (
+    WHITELISTED_BUILTINS,
+    WHITELISTED_LIBRARIES,
+)
+from .exceptions import BadImportError, LLMNotFoundError
+from .helpers._optional import import_dependency
+from .helpers.anonymizer import anonymize_dataframe_head
+from .helpers.cache import Cache
+from .helpers.notebook import Notebook
+from .helpers.save_chart import add_save_chart
+from .helpers.shortcuts import Shortcuts
+from .llm.base import LLM
+from .llm.langchain import LangchainLLM
+from .middlewares.base import Middleware
+from .middlewares.charts import ChartsMiddleware
+from .prompts.base import Prompt
+from .prompts.correct_error_prompt import CorrectErrorPrompt
+from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
+from .prompts.generate_python_code import GeneratePythonCodePrompt
+from .prompts.generate_response import GenerateResponsePrompt
+from .prompts.multiple_dataframes import MultipleDataframesPrompt
+
+
+def get_version():
+    """
+    Get the version from the package metadata
+    """
+    from importlib.metadata import version
+
+    return version("pandasai")
+
+
+__version__ = get_version()
+
+
+class PandasAI(Shortcuts):
+    """
+    PandasAI is a wrapper around a LLM to make dataframes conversational.
+
+
+    This is an entry point of `pandasai` object. This class consists of methods
+    to interface the LLMs with Pandas     dataframes. A pandas dataframe metadata i.e.
+    df.head() and prompt is passed on to chosen LLMs API end point to generate a Python
+    code to answer the questions asked. The resultant python code is run on actual data
+    and answer is converted into a conversational form.
+
+    Note:
+        Do not include the `self` parameter in the ``Args`` section.
+    Args:
+        _llm (obj): LLMs option to be used for API access
+        _verbose (bool, optional): To show the intermediate outputs e.g. python code
+        generated and execution step on the prompt. Default to False
+        _is_conversational_answer (bool, optional): Whether to return answer in
+        conversational form. Default to False
+        _enforce_privacy (bool, optional): Do not display the data on prompt in case of
+        Sensitive data. Default to False
+        _max_retries (int, optional): max no. of tries to generate code on failure.
+        Default to 3
+        _in_notebook (bool, optional): Whether to run code in notebook. Default to False
+        _original_instructions (dict, optional): The dict of instruction to run. Default
+        to None
+        _cache (Cache, optional): Cache object to store the results. Default to None
+        _enable_cache (bool, optional): Whether to enable cache. Default to True
+        _logger (logging.Logger, optional): Logger object to log the messages. Default
+        to None
+        _logs (List[dict], optional): List of logs to be stored. Default to []
+        _prompt_id (str, optional): Unique ID to differentiate calls. Default to None
+        _middlewares (List[Middleware], optional): List of middlewares to run. Default
+        to [ChartsMiddleware()]
+        _additional_dependencies (List[dict], optional): List of additional dependencies
+        to be added. Default to []
+        _custom_whitelisted_dependencies (List[str], optional): List of custom
+        whitelisted dependencies. Default to []
+        last_code_generated (str, optional): Pass last Code if generated. Default to
+        None
+        last_code_executed (str, optional): Pass the last execution / run. Default to
+        None
+        code_output (str, optional): The code output if any. Default to None
+        last_error (str, optional): Error of running code last time. Default to None
+        prompt_id (str, optional): Unique ID to differentiate calls. Default to None
+
+
+    Returns (str): Response to a Question related to Data
+
+    """
+
+    _llm: LLM
+    _verbose: bool = False
+    _is_conversational_answer: bool = False
+    _enforce_privacy: bool = False
+    _max_retries: int = 3
+    _in_notebook: bool = False
+    _original_instructions: dict = {
+        "question": None,
+        "df_head": None,
+        "num_rows": None,
+        "num_columns": None,
+    }
+    _cache: Cache = None
+    _enable_cache: bool = True
+    _prompt_id: Optional[str] = None
+    _middlewares: List[Middleware] = [ChartsMiddleware()]
+    _additional_dependencies: List[dict] = []
+    _custom_whitelisted_dependencies: List[str] = []
+    _start_time: float = 0
+    _enable_logging: bool = True
+    _logger: logging.Logger = None
+    _logs: List[str] = []
+    last_code_generated: Optional[str] = None
+    last_code_executed: Optional[str] = None
+    code_output: Optional[str] = None
+    last_error: Optional[str] = None
+
+    def __init__(
+        self,
+        llm=None,
+        conversational=False,
+        verbose=False,
+        enforce_privacy=False,
+        save_charts=False,
+        save_charts_path=None,
+        enable_cache=True,
+        middlewares=None,
+        custom_whitelisted_dependencies=None,
+        enable_logging=True,
+        non_default_prompts: Optional[Dict[str, Type[Prompt]]] = None,
+    ):
+        """
+
+        __init__ method of the Class PandasAI
+
+        Args:
+            llm (object): LLMs option to be used for API access. Default is None
+            conversational (bool): Whether to return answer in conversational form.
+            Default to False
+            verbose (bool): To show the intermediate outputs e.g. python code
+            generated and execution step on the prompt.  Default to False
+            enforce_privacy (bool): Execute the codes with Privacy Mode ON.
+            Default to False
+            save_charts (bool): Save the charts generated in the notebook.
+            Default to False
+            enable_cache (bool): Enable the cache to store the results.
+            Default to True
+            middlewares (list): List of middlewares to be used. Default to None
+            custom_whitelisted_dependencies (list): List of custom dependencies to
+            be used. Default to None
+            enable_logging (bool): Enable the logging. Default to True
+            non_default_prompts (dict): Mapping from keys to replacement prompt classes.
+            Used to override specific types of prompts. Defaults to None.
+        """
+
+        # configure the logging
+        # noinspection PyArgumentList
+        # https://stackoverflow.com/questions/61226587/pycharm-does-not-recognize-logging-basicconfig-handlers-argument
+        if enable_logging:
+            handlers = [logging.FileHandler("pandasai.log")]
+        else:
+            handlers = []
+
+        if verbose:
+            handlers.append(logging.StreamHandler(sys.stdout))
+        logging.basicConfig(
+            level=logging.INFO,
+            format="%(asctime)s [%(levelname)s] %(message)s",
+            datefmt="%Y-%m-%d %H:%M:%S",
+            handlers=handlers,
+        )
+        self._logger = logging.getLogger(__name__)
+
+        if llm is None:
+            raise LLMNotFoundError(
+                "An LLM should be provided to instantiate a PandasAI instance"
+            )
+        self._load_llm(llm)
+        self._is_conversational_answer = conversational
+        self._verbose = verbose
+        self._enforce_privacy = enforce_privacy
+        self._save_charts = save_charts
+        self._save_charts_path = save_charts_path
+        self._process_id = str(uuid.uuid4())
+        self._logs = []
+
+        self._non_default_prompts = (
+            {} if non_default_prompts is None else non_default_prompts
+        )
+
+        self.notebook = Notebook()
+        self._in_notebook = self.notebook.in_notebook()
+
+        self._enable_cache = enable_cache
+        if self._enable_cache:
+            self._cache = Cache()
+
+        if middlewares is not None:
+            self.add_middlewares(*middlewares)
+
+        if custom_whitelisted_dependencies is not None:
+            self._custom_whitelisted_dependencies = custom_whitelisted_dependencies
+
+    def _load_llm(self, llm):
+        """
+        Check if it is a PandasAI LLM or a Langchain LLM.
+        If it is a Langchain LLM, wrap it in a PandasAI LLM.
+
+        Args:
+            llm (object): LLMs option to be used for API access
+
+        Raises:
+            BadImportError: If the LLM is a Langchain LLM but the langchain package
+            is not installed
+        """
+
+        try:
+            llm.is_pandasai_llm()
+        except AttributeError:
+            llm = LangchainLLM(llm)
+
+        self._llm = llm
+
+    def conversational_answer(self, question: str, answer: str) -> str:
+        """
+        Returns the answer in conversational form about the resultant data.
+
+        Args:
+            question (str): A question in Conversational form
+            answer (str): A summary / resultant Data
+
+        Returns (str): Response
+
+        """
+
+        if self._enforce_privacy:
+            # we don't want to send potentially sensitive data to the LLM server
+            # if the user has set enforce_privacy to True
+            return answer
+
+        generate_response_instruction = self._non_default_prompts.get(
+            "generate_response", GenerateResponsePrompt
+        )(question=question, answer=answer)
+        return self._llm.call(generate_response_instruction, "")
+
+    def run(
+        self,
+        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
+        prompt: str,
+        is_conversational_answer: bool = None,
+        show_code: bool = False,
+        anonymize_df: bool = True,
+        use_error_correction_framework: bool = True,
+    ) -> Union[str, pd.DataFrame]:
+        """
+        Run the PandasAI to make Dataframes Conversational.
+
+        Args:
+            data_frame (Union[pd.DataFrame, List[pd.DataFrame]]): A pandas Dataframe
+            prompt (str): A prompt to query about the Dataframe
+            is_conversational_answer (bool): Whether to return answer in conversational
+            form. Default to False
+            show_code (bool): To show the intermediate python code generated on the
+            prompt. Default to False
+            anonymize_df (bool): Running the code with Sensitive Data. Default to True
+            use_error_correction_framework (bool): Turn on Error Correction mechanism.
+            Default to True
+
+        Returns (str): Answer to the Input Questions about the DataFrame
+
+        """
+
+        self._start_time = time.time()
+
+        self.log(f"Question: {prompt}")
+        self.log(f"Running PandasAI with {self._llm.type} LLM...")
+
+        self._prompt_id = str(uuid.uuid4())
+        self.log(f"Prompt ID: {self._prompt_id}")
+
+        try:
+            if self._enable_cache and self._cache and self._cache.get(prompt):
+                self.log("Using cached response")
+                code = self._cache.get(prompt)
+            else:
+                rows_to_display = 0 if self._enforce_privacy else 5
+
+                multiple: bool = isinstance(data_frame, list)
+
+                if multiple:
+                    heads = [
+                        anonymize_dataframe_head(dataframe)
+                        if anonymize_df
+                        else dataframe.head(rows_to_display)
+                        for dataframe in data_frame
+                    ]
+
+                    multiple_dataframes_instruction = self._non_default_prompts.get(
+                        "multiple_dataframes", MultipleDataframesPrompt
+                    )
+                    code = self._llm.generate_code(
+                        multiple_dataframes_instruction(dataframes=heads),
+                        prompt,
+                    )
+
+                    self._original_instructions = {
+                        "question": prompt,
+                        "df_head": heads,
+                    }
+
+                else:
+                    df_head = data_frame.head(rows_to_display)
+                    if anonymize_df:
+                        df_head = anonymize_dataframe_head(df_head)
+                    df_head = df_head.to_csv(index=False)
+
+                    generate_code_instruction = self._non_default_prompts.get(
+                        "generate_python_code", GeneratePythonCodePrompt
+                    )(
+                        prompt=prompt,
+                        df_head=df_head,
+                        num_rows=data_frame.shape[0],
+                        num_columns=data_frame.shape[1],
+                    )
+                    code = self._llm.generate_code(
+                        generate_code_instruction,
+                        prompt,
+                    )
+
+                    self._original_instructions = {
+                        "question": prompt,
+                        "df_head": df_head,
+                        "num_rows": data_frame.shape[0],
+                        "num_columns": data_frame.shape[1],
+                    }
+
+                self.last_code_generated = code
+                self.log(
+                    f"""
+                        Code generated:
+                        ```
+                        {code}
+                        ```
+                    """
+                )
+
+                if self._enable_cache and self._cache:
+                    self._cache.set(prompt, code)
+
+            if show_code and self._in_notebook:
+                self.notebook.create_new_cell(code)
+
+            for middleware in self._middlewares:
+                code = middleware(code)
+
+            answer = self.run_code(
+                code,
+                data_frame,
+                use_error_correction_framework=use_error_correction_framework,
+            )
+            self.code_output = answer
+            self.log(f"Answer: {answer}")
+
+            if is_conversational_answer is None:
+                is_conversational_answer = self._is_conversational_answer
+            if is_conversational_answer:
+                answer = self.conversational_answer(prompt, answer)
+                self.log(f"Conversational answer: {answer}")
+
+            self.log(f"Executed in: {time.time() - self._start_time}s")
+
+            return answer
+        except Exception as exception:
+            self.last_error = str(exception)
+            print(exception)
+            return (
+                "Unfortunately, I was not able to answer your question, "
+                "because of the following error:\n"
+                f"\n{exception}\n"
+            )
+
+    def add_middlewares(self, *middlewares: List[Middleware]):
+        """
+        Add middlewares to PandasAI instance.
+
+        Args:
+            *middlewares: A list of middlewares
+
+        """
+        self._middlewares.extend(middlewares)
+
+    def clear_cache(self):
+        """
+        Clears the cache of the PandasAI instance.
+        """
+        if self._cache:
+            self._cache.clear()
+
+    def __call__(
+        self,
+        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
+        prompt: str,
+        is_conversational_answer: bool = None,
+        show_code: bool = False,
+        anonymize_df: bool = True,
+        use_error_correction_framework: bool = True,
+    ) -> Union[str, pd.DataFrame]:
+        """
+        __call__ method of PandasAI class. It calls the `run` method.
+
+        Args:
+            data_frame:
+            prompt:
+            is_conversational_answer:
+            show_code:
+            anonymize_df:
+            use_error_correction_framework:
+
+        Returns (str): Answer to the Input Questions about the DataFrame.
+
+        """
+
+        return self.run(
+            data_frame,
+            prompt,
+            is_conversational_answer,
+            show_code,
+            anonymize_df,
+            use_error_correction_framework,
+        )
+
+    def _check_imports(self, node: Union[ast.Import, ast.ImportFrom]):
+        """
+        Add whitelisted imports to _additional_dependencies.
+
+        Args:
+            node (object): ast.Import or ast.ImportFrom
+
+        Raises:
+            BadImportError: If the import is not whitelisted
+
+        """
+        if isinstance(node, ast.Import):
+            module = node.names[0].name
+        else:
+            module = node.module
+
+        library = module.split(".")[0]
+
+        if library == "pandas":
+            return
+
+        if library in WHITELISTED_LIBRARIES + self._custom_whitelisted_dependencies:
+            for alias in node.names:
+                self._additional_dependencies.append(
+                    {
+                        "module": module,
+                        "name": alias.name,
+                        "alias": alias.asname or alias.name,
+                    }
+                )
+            return
+
+        if library not in WHITELISTED_BUILTINS:
+            raise BadImportError(library)
+
+    def _is_df_overwrite(self, node: ast.stmt) -> bool:
+        """
+        Remove df declarations from the code to prevent malicious code execution.
+
+        Args:
+            node (object): ast.stmt
+
+        Returns (bool):
+
+        """
+
+        return (
+            isinstance(node, ast.Assign)
+            and isinstance(node.targets[0], ast.Name)
+            and re.match(r"df\d{0,2}$", node.targets[0].id)
+        )
+
+    def _clean_code(self, code: str) -> str:
+        """
+        A method to clean the code to prevent malicious code execution
+
+        Args:
+            code(str): A python code
+
+        Returns (str): Returns a Clean Code String
+
+        """
+
+        tree = ast.parse(code)
+
+        new_body = []
+
+        # clear recent optional dependencies
+        self._additional_dependencies = []
+
+        for node in tree.body:
+            if isinstance(node, (ast.Import, ast.ImportFrom)):
+                self._check_imports(node)
+                continue
+            if self._is_df_overwrite(node):
+                continue
+            new_body.append(node)
+
+        new_tree = ast.Module(body=new_body)
+        return astor.to_source(new_tree).strip()
+
+    def _get_environment(self) -> dict:
+        """
+        Returns the environment for the code to be executed.
+
+        Returns (dict): A dictionary of environment variables
+        """
+
+        return {
+            "pd": pd,
+            **{
+                lib["alias"]: getattr(import_dependency(lib["module"]), lib["name"])
+                if hasattr(import_dependency(lib["module"]), lib["name"])
+                else import_dependency(lib["module"])
+                for lib in self._additional_dependencies
+            },
+            "__builtins__": {
+                **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
+            },
+        }
+
+    def _retry_run_code(self, code: str, e: Exception, multiple: bool = False):
+        """
+        A method to retry the code execution with error correction framework.
+
+        Args:
+            code (str): A python code
+            e (Exception): An exception
+            multiple (bool): A boolean to indicate if the code is for multiple
+            dataframes
+
+        Returns (str): A python code
+        """
+
+        if multiple:
+            error_correcting_instruction = self._non_default_prompts.get(
+                "correct_multiple_dataframes_error",
+                CorrectMultipleDataframesErrorPrompt,
+            )(
+                code=code,
+                error_returned=e,
+                question=self._original_instructions["question"],
+                df_head=self._original_instructions["df_head"],
+            )
+
+        else:
+            error_correcting_instruction = self._non_default_prompts.get(
+                "correct_error", CorrectErrorPrompt
+            )(
+                code=code,
+                error_returned=e,
+                question=self._original_instructions["question"],
+                df_head=self._original_instructions["df_head"],
+                num_rows=self._original_instructions["num_rows"],
+                num_columns=self._original_instructions["num_columns"],
+            )
+
+        return self._llm.generate_code(error_correcting_instruction, "")
+
+    def run_code(
+        self,
+        code: str,
+        data_frame: pd.DataFrame,
+        use_error_correction_framework: bool = True,
+    ) -> str:
+        """
+        A method to execute the python code generated by LLMs to answer the question
+        about the input dataframe. Run the code in the current context and return the
+        result.
+
+        Args:
+            code (str): A python code to execute
+            data_frame (pd.DataFrame): A full Pandas DataFrame
+            use_error_correction_framework (bool): Turn on Error Correction mechanism.
+            Default to True
+
+        Returns (str): String representation of the result of the code execution.
+
+        """
+
+        multiple: bool = isinstance(data_frame, list)
+
+        # Add save chart code
+        if self._save_charts:
+            code = add_save_chart(
+                code, self._prompt_id, self._save_charts_path, not self._verbose
+            )
+
+        # Get the code to run removing unsafe imports and df overwrites
+        code_to_run = self._clean_code(code)
+        self.last_code_executed = code_to_run
+        self.log(
+            f"""
+Code running:
+```
+{code_to_run}
+```"""
+        )
+
+        environment: dict = self._get_environment()
+
+        if multiple:
+            environment.update(
+                {f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start=1)}
+            )
+        else:
+            environment["df"] = data_frame
+
+        # Redirect standard output to a StringIO buffer
+        with redirect_stdout(io.StringIO()) as output:
+            count = 0
+            while count < self._max_retries:
+                try:
+                    # Execute the code
+                    exec(code_to_run, environment)
+                    code = code_to_run
+                    break
+                except Exception as e:
+                    if not use_error_correction_framework:
+                        raise e
+
+                    count += 1
+
+                    code_to_run = self._retry_run_code(code, e, multiple)
+
+        captured_output = output.getvalue().strip()
+        if code.count("print(") > 1:
+            return captured_output
+
+        # Evaluate the last line and return its value or the captured output
+        # We do this because we want to return the right value and the right
+        # type of the value. For example, if the last line is `df.head()`, we
+        # want to return the head of the dataframe, not the captured output.
+        lines = code.strip().split("\n")
+        last_line = lines[-1].strip()
+
+        match = re.match(r"^print\((.*)\)$", last_line)
+        if match:
+            last_line = match.group(1)
+
+        try:
+            result = eval(last_line, environment)
+
+            # In some cases, the result is a tuple of values. For example, when
+            # the last line is `print("Hello", "World")`, the result is a tuple
+            # of two strings. In this case, we want to return a string
+            if isinstance(result, tuple):
+                result = " ".join([str(element) for element in result])
+
+            return result
+        except Exception:
+            return captured_output
+
+    def log(self, message: str):
+        """Log a message"""
+        self._logger.info(message)
+        self._logs.append(message)
+
+    @property
+    def logs(self) -> List[str]:
+        """Return the logs"""
+        return self._logs
+
+    def process_id(self) -> str:
+        """Return the id of this PandasAI object."""
+        return self._process_id
+
+    @property
+    def last_prompt_id(self) -> str:
+        """Return the id of the last prompt that was run."""
+        if self._prompt_id is None:
+            raise ValueError("Pandas AI has not been run yet.")
+        return self._prompt_id
+
+    @property
+    def last_prompt(self) -> str:
+        """Return the last prompt that was executed."""
+        if self._llm:
+            return self._llm.last_prompt
```

### Comparing `hfttai-0.1.0/pandasai/exceptions.py` & `hfttai-0.1.2/pandasai/exceptions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""PandasAI's custom exceptions.
-
-This module contains the implementation of Custom Exceptions.
-
-"""
-
-
-class APIKeyNotFoundError(Exception):
-
-    """
-    Raised when the API key is not defined/declared.
-
-    Args:
-        Exception (Exception): APIKeyNotFoundError
-    """
-
-
-class LLMNotFoundError(Exception):
-    """
-    Raised when the LLM is not provided.
-
-    Args:
-        Exception (Exception): LLMNotFoundError
-    """
-
-
-class NoCodeFoundError(Exception):
-    """
-    Raised when no code is found in the response.
-
-    Args:
-        Exception (Exception): NoCodeFoundError
-    """
-
-
-class MethodNotImplementedError(Exception):
-    """
-    Raised when a method is not implemented.
-
-    Args:
-        Exception (Exception): MethodNotImplementedError
-    """
-
-
-class UnsupportedOpenAIModelError(Exception):
-    """
-    Raised when an unsupported OpenAI model is used.
-
-    Args:
-        Exception (Exception): UnsupportedOpenAIModelError
-    """
-
-
-class BadImportError(Exception):
-    """
-    Raised when a library not in the whitelist is imported.
-
-    Args:
-        Exception (Exception): BadImportError
-    """
-
-    def __init__(self, library_name):
-        """
-        __init__ method of BadImportError Class
-
-        Args:
-            library_name (str): Name of the library that is not in the whitelist.
-        """
-        self.library_name = library_name
-        super().__init__(
-            f"Generated code includes import of {library_name} which"
-            " is not in whitelist."
-        )
+"""PandasAI's custom exceptions.
+
+This module contains the implementation of Custom Exceptions.
+
+"""
+
+
+class APIKeyNotFoundError(Exception):
+
+    """
+    Raised when the API key is not defined/declared.
+
+    Args:
+        Exception (Exception): APIKeyNotFoundError
+    """
+
+
+class LLMNotFoundError(Exception):
+    """
+    Raised when the LLM is not provided.
+
+    Args:
+        Exception (Exception): LLMNotFoundError
+    """
+
+
+class NoCodeFoundError(Exception):
+    """
+    Raised when no code is found in the response.
+
+    Args:
+        Exception (Exception): NoCodeFoundError
+    """
+
+
+class MethodNotImplementedError(Exception):
+    """
+    Raised when a method is not implemented.
+
+    Args:
+        Exception (Exception): MethodNotImplementedError
+    """
+
+
+class UnsupportedOpenAIModelError(Exception):
+    """
+    Raised when an unsupported OpenAI model is used.
+
+    Args:
+        Exception (Exception): UnsupportedOpenAIModelError
+    """
+
+
+class BadImportError(Exception):
+    """
+    Raised when a library not in the whitelist is imported.
+
+    Args:
+        Exception (Exception): BadImportError
+    """
+
+    def __init__(self, library_name):
+        """
+        __init__ method of BadImportError Class
+
+        Args:
+            library_name (str): Name of the library that is not in the whitelist.
+        """
+        self.library_name = library_name
+        super().__init__(
+            f"Generated code includes import of {library_name} which"
+            " is not in whitelist."
+        )
```

### Comparing `hfttai-0.1.0/pandasai/helpers/_optional.py` & `hfttai-0.1.2/pandasai/helpers/_optional.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-"""Module to import optional dependencies.
-
-Source: Taken from pandas/compat/_optional.py
-"""
-from __future__ import annotations
-
-import importlib
-import sys
-import warnings
-from typing import TYPE_CHECKING
-
-from pandas.util.version import Version
-
-if TYPE_CHECKING:
-    import types
-
-# Minimum version required for each optional dependency
-
-VERSIONS = {
-    "sklearn": "1.2.2",
-    "statsmodels": "0.14.0",
-    "seaborn": "0.12.2",
-    "plotly": "5.14.1",
-    "ggplot": "0.11.5",
-    "scipy": "1.9.0",
-    "streamlit": "1.23.1",
-}
-
-# A mapping from import name to package name (on PyPI) for packages where
-# these two names are different.
-
-INSTALL_MAPPING = {}
-
-
-def get_version(module: types.ModuleType) -> str:
-    """Get the version of a module."""
-    version = getattr(module, "__version__", None)
-
-    if version is None:
-        raise ImportError(f"Can't determine version for {module.__name__}")
-
-    return version
-
-
-def import_dependency(
-    name: str,
-    extra: str = "",
-    errors: str = "raise",
-    min_version: str | None = None,
-):
-    """
-    Import an optional dependency.
-
-    By default, if a dependency is missing an ImportError with a nice
-    message will be raised. If a dependency is present, but too old,
-    we raise.
-
-    Parameters
-    ----------
-    name : str
-        The module name.
-    extra : str
-        Additional text to include in the ImportError message.
-    errors : str {'raise', 'warn', 'ignore'}
-        What to do when a dependency is not found or its version is too old.
-
-        * raise : Raise an ImportError
-        * warn : Only applicable when a module's version is to old.
-          Warns that the version is too old and returns None
-        * ignore: If the module is not installed, return None, otherwise,
-          return the module, even if the version is too old.
-          It's expected that users validate the version locally when
-          using ``errors="ignore"`` (see. ``io/html.py``)
-    min_version : str, default None
-        Specify a minimum version that is different from the global pandas
-        minimum version required.
-    Returns
-    -------
-    maybe_module : Optional[ModuleType]
-        The imported module, when found and the version is correct.
-        None is returned when the package is not found and `errors`
-        is False, or when the package's version is too old and `errors`
-        is ``'warn'``.
-    """
-
-    assert errors in {"warn", "raise", "ignore"}
-
-    package_name = INSTALL_MAPPING.get(name)
-    install_name = package_name if package_name is not None else name
-
-    msg = (
-        f"Missing optional dependency '{install_name}'. {extra} "
-        f"Use pip or conda to install {install_name}."
-    )
-    try:
-        module = importlib.import_module(name)
-    except ImportError as exc:
-        if errors == "raise":
-            raise ImportError(msg) from exc
-        return None
-
-    # Handle submodules: if we have submodule, grab parent module from sys.modules
-    parent = name.split(".")[0]
-    if parent != name:
-        install_name = parent
-        module_to_get = sys.modules[install_name]
-    else:
-        module_to_get = module
-    minimum_version = min_version if min_version is not None else VERSIONS.get(parent)
-    if minimum_version:
-        version = get_version(module_to_get)
-        if version and Version(version) < Version(minimum_version):
-            msg = (
-                f"Pandas requires version '{minimum_version}' or newer of '{parent}' "
-                f"(version '{version}' currently installed)."
-            )
-            if errors == "warn":
-                warnings.warn(
-                    msg,
-                    UserWarning,
-                )
-                return None
-            if errors == "raise":
-                raise ImportError(msg)
-
-    return module
+"""Module to import optional dependencies.
+
+Source: Taken from pandas/compat/_optional.py
+"""
+from __future__ import annotations
+
+import importlib
+import sys
+import warnings
+from typing import TYPE_CHECKING
+
+from pandas.util.version import Version
+
+if TYPE_CHECKING:
+    import types
+
+# Minimum version required for each optional dependency
+
+VERSIONS = {
+    "sklearn": "1.2.2",
+    "statsmodels": "0.14.0",
+    "seaborn": "0.12.2",
+    "plotly": "5.14.1",
+    "ggplot": "0.11.5",
+    "scipy": "1.9.0",
+    "streamlit": "1.23.1",
+}
+
+# A mapping from import name to package name (on PyPI) for packages where
+# these two names are different.
+
+INSTALL_MAPPING = {}
+
+
+def get_version(module: types.ModuleType) -> str:
+    """Get the version of a module."""
+    version = getattr(module, "__version__", None)
+
+    if version is None:
+        raise ImportError(f"Can't determine version for {module.__name__}")
+
+    return version
+
+
+def import_dependency(
+    name: str,
+    extra: str = "",
+    errors: str = "raise",
+    min_version: str | None = None,
+):
+    """
+    Import an optional dependency.
+
+    By default, if a dependency is missing an ImportError with a nice
+    message will be raised. If a dependency is present, but too old,
+    we raise.
+
+    Parameters
+    ----------
+    name : str
+        The module name.
+    extra : str
+        Additional text to include in the ImportError message.
+    errors : str {'raise', 'warn', 'ignore'}
+        What to do when a dependency is not found or its version is too old.
+
+        * raise : Raise an ImportError
+        * warn : Only applicable when a module's version is to old.
+          Warns that the version is too old and returns None
+        * ignore: If the module is not installed, return None, otherwise,
+          return the module, even if the version is too old.
+          It's expected that users validate the version locally when
+          using ``errors="ignore"`` (see. ``io/html.py``)
+    min_version : str, default None
+        Specify a minimum version that is different from the global pandas
+        minimum version required.
+    Returns
+    -------
+    maybe_module : Optional[ModuleType]
+        The imported module, when found and the version is correct.
+        None is returned when the package is not found and `errors`
+        is False, or when the package's version is too old and `errors`
+        is ``'warn'``.
+    """
+
+    assert errors in {"warn", "raise", "ignore"}
+
+    package_name = INSTALL_MAPPING.get(name)
+    install_name = package_name if package_name is not None else name
+
+    msg = (
+        f"Missing optional dependency '{install_name}'. {extra} "
+        f"Use pip or conda to install {install_name}."
+    )
+    try:
+        module = importlib.import_module(name)
+    except ImportError as exc:
+        if errors == "raise":
+            raise ImportError(msg) from exc
+        return None
+
+    # Handle submodules: if we have submodule, grab parent module from sys.modules
+    parent = name.split(".")[0]
+    if parent != name:
+        install_name = parent
+        module_to_get = sys.modules[install_name]
+    else:
+        module_to_get = module
+    minimum_version = min_version if min_version is not None else VERSIONS.get(parent)
+    if minimum_version:
+        version = get_version(module_to_get)
+        if version and Version(version) < Version(minimum_version):
+            msg = (
+                f"Pandas requires version '{minimum_version}' or newer of '{parent}' "
+                f"(version '{version}' currently installed)."
+            )
+            if errors == "warn":
+                warnings.warn(
+                    msg,
+                    UserWarning,
+                )
+                return None
+            if errors == "raise":
+                raise ImportError(msg)
+
+    return module
```

### Comparing `hfttai-0.1.0/pandasai/helpers/anonymizer.py` & `hfttai-0.1.2/pandasai/helpers/anonymizer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-"""
-This module contains helper functions for anonymizing data and generating random data
- before sending it to the LLM (An External API).
-
-Only df.head() is sent to LLM API, hence the df.head() is processed
- to remove any personal or sensitive information.
-
-"""
-
-import random
-import re
-import string
-
-import pandas as pd
-
-
-def is_valid_email(email: str) -> bool:
-    """Check if the given email is valid based on regex pattern.
-
-    Args:
-        email (str): email address to be checked.
-
-    Returns (bool): True if the email is valid, otherwise False.
-    """
-
-    email_regex = r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
-    return re.match(email_regex, email) is not None
-
-
-def is_valid_phone_number(phone_number: str) -> bool:
-    """Check if the given phone number is valid based on regex pattern.
-
-    Args:
-        phone_number (str): phone number to be checked.
-
-    Returns (bool): True if the phone number is valid, otherwise False.
-    """
-
-    pattern = r"\b(?:\+?\d{1,3}[- ]?)?\(?\d{3}\)?[- ]?\d{3}[- ]?\d{4}\b"
-    return re.search(pattern, phone_number) is not None
-
-
-def is_valid_credit_card(credit_card_number: str) -> bool:
-    """Check if the given credit card number is valid based on regex pattern.
-
-    Args:
-        credit_card_number (str): credit card number to be checked.
-
-    Returns (str): True if the credit card number is valid, otherwise False.
-    """
-
-    pattern = r"^\d{4}[- ]?\d{4}[- ]?\d{4}[- ]?\d{4}$"
-    return re.search(pattern, credit_card_number) is not None
-
-
-def generate_random_email() -> str:
-    """Generates a random email address using predefined domains.
-
-    Returns (str): generated random email address.
-    """
-
-    domains = [
-        "gmail.com",
-        "yahoo.com",
-        "hotmail.com",
-        "outlook.com",
-        "icloud.com",
-        "aol.com",
-        "protonmail.com",
-        "zoho.com",
-    ]
-    name_length = random.randint(6, 12)
-    domain = random.choice(domains)
-    letters = string.ascii_lowercase + string.digits + "-_"
-    username = "".join(random.choice(letters) for i in range(name_length))
-    email = username + "@" + domain
-    return email
-
-
-def generate_random_phone_number(original_field: str) -> str:
-    """Generate a random phone number with country code if originally present.
-
-    Args:
-        original_field (str): original phone number field.
-
-    Returns (str): generated random phone number.
-    """
-
-    if original_field.startswith("+"):
-        # Extract country code if present
-        country_code = original_field.split()[0]
-    else:
-        country_code = ""
-
-    number = "".join(random.choices("0123456789", k=10))
-
-    if country_code:
-        phone_number = f"{country_code} {number}"
-    else:
-        phone_number = number
-
-    return phone_number
-
-
-def generate_random_credit_card() -> str:
-    """Generate a random credit card number.
-
-    Returns (str): generated random credit card number.
-    """
-
-    groups = []
-    for _i in range(4):
-        group = "".join(random.choices("0123456789", k=4))
-        groups.append(group)
-    separator = random.choice(["-", " "])
-    return separator.join(groups)
-
-
-def copy_head(data_frame: pd.DataFrame) -> pd.DataFrame:
-    """Copy the head of a DataFrame.
-
-    Args:
-        data_frame (pd.DataFrame): The pd.DataFrame to copy the head from.
-
-    Returns (pd.DataFrame): copied head of the DataFrame.
-    """
-
-    return data_frame.head().copy()
-
-
-def anonymize_dataframe_head(
-    data_frame: pd.DataFrame, force_conversion: bool = True
-) -> pd.DataFrame:
-    """Anonymize the head of a given DataFrame by replacing sensitive data.
-
-    Args:
-
-        data_frame (pd.DataFrame):  The DataFrame to anonymize the head data.
-        force_conversion (bool): Convert it with instruction. Default is True.
-
-    Returns: Anonymized head of the DataFrame.
-    """
-
-    data_frame = copy_head(data_frame)
-    dtypes = data_frame.dtypes
-    for col in data_frame.columns:
-        col_idx = data_frame.columns.get_loc(col)
-        # check category type column and temporarily convert to object type
-        if force_conversion:
-            if pd.api.types.is_categorical_dtype(data_frame[col]):
-                if data_frame[col].isna().any():
-                    data_frame[col] = data_frame[col].astype(object)
-        for row_idx, val in enumerate(data_frame[col]):
-            cell_value = str(val)
-
-            if is_valid_email(cell_value):
-                data_frame.iloc[row_idx, col_idx] = generate_random_email()
-                continue
-            if is_valid_phone_number(cell_value):
-                data_frame.iloc[row_idx, col_idx] = generate_random_phone_number(
-                    cell_value
-                )
-                continue
-            if is_valid_credit_card(cell_value):
-                data_frame.iloc[row_idx, col_idx] = generate_random_credit_card()
-                continue
-
-            # anonymize data
-            random_row_index = random.choice(
-                [i for i in range(len(data_frame.index)) if i != row_idx]
-            )
-            random_value = data_frame.iloc[random_row_index, col_idx]
-            data_frame.iloc[row_idx, col_idx] = random_value
-            data_frame.iloc[random_row_index, col_idx] = (
-                pd.eval(cell_value) if cell_value in ["True", "False"] else cell_value
-            )
-    # restore the original data types
-    data_frame = data_frame.astype(dtypes)
-    return data_frame
+"""
+This module contains helper functions for anonymizing data and generating random data
+ before sending it to the LLM (An External API).
+
+Only df.head() is sent to LLM API, hence the df.head() is processed
+ to remove any personal or sensitive information.
+
+"""
+
+import random
+import re
+import string
+
+import pandas as pd
+
+
+def is_valid_email(email: str) -> bool:
+    """Check if the given email is valid based on regex pattern.
+
+    Args:
+        email (str): email address to be checked.
+
+    Returns (bool): True if the email is valid, otherwise False.
+    """
+
+    email_regex = r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
+    return re.match(email_regex, email) is not None
+
+
+def is_valid_phone_number(phone_number: str) -> bool:
+    """Check if the given phone number is valid based on regex pattern.
+
+    Args:
+        phone_number (str): phone number to be checked.
+
+    Returns (bool): True if the phone number is valid, otherwise False.
+    """
+
+    pattern = r"\b(?:\+?\d{1,3}[- ]?)?\(?\d{3}\)?[- ]?\d{3}[- ]?\d{4}\b"
+    return re.search(pattern, phone_number) is not None
+
+
+def is_valid_credit_card(credit_card_number: str) -> bool:
+    """Check if the given credit card number is valid based on regex pattern.
+
+    Args:
+        credit_card_number (str): credit card number to be checked.
+
+    Returns (str): True if the credit card number is valid, otherwise False.
+    """
+
+    pattern = r"^\d{4}[- ]?\d{4}[- ]?\d{4}[- ]?\d{4}$"
+    return re.search(pattern, credit_card_number) is not None
+
+
+def generate_random_email() -> str:
+    """Generates a random email address using predefined domains.
+
+    Returns (str): generated random email address.
+    """
+
+    domains = [
+        "gmail.com",
+        "yahoo.com",
+        "hotmail.com",
+        "outlook.com",
+        "icloud.com",
+        "aol.com",
+        "protonmail.com",
+        "zoho.com",
+    ]
+    name_length = random.randint(6, 12)
+    domain = random.choice(domains)
+    letters = string.ascii_lowercase + string.digits + "-_"
+    username = "".join(random.choice(letters) for i in range(name_length))
+    email = username + "@" + domain
+    return email
+
+
+def generate_random_phone_number(original_field: str) -> str:
+    """Generate a random phone number with country code if originally present.
+
+    Args:
+        original_field (str): original phone number field.
+
+    Returns (str): generated random phone number.
+    """
+
+    if original_field.startswith("+"):
+        # Extract country code if present
+        country_code = original_field.split()[0]
+    else:
+        country_code = ""
+
+    number = "".join(random.choices("0123456789", k=10))
+
+    if country_code:
+        phone_number = f"{country_code} {number}"
+    else:
+        phone_number = number
+
+    return phone_number
+
+
+def generate_random_credit_card() -> str:
+    """Generate a random credit card number.
+
+    Returns (str): generated random credit card number.
+    """
+
+    groups = []
+    for _i in range(4):
+        group = "".join(random.choices("0123456789", k=4))
+        groups.append(group)
+    separator = random.choice(["-", " "])
+    return separator.join(groups)
+
+
+def copy_head(data_frame: pd.DataFrame) -> pd.DataFrame:
+    """Copy the head of a DataFrame.
+
+    Args:
+        data_frame (pd.DataFrame): The pd.DataFrame to copy the head from.
+
+    Returns (pd.DataFrame): copied head of the DataFrame.
+    """
+
+    return data_frame.head().copy()
+
+
+def anonymize_dataframe_head(
+    data_frame: pd.DataFrame, force_conversion: bool = True
+) -> pd.DataFrame:
+    """Anonymize the head of a given DataFrame by replacing sensitive data.
+
+    Args:
+
+        data_frame (pd.DataFrame):  The DataFrame to anonymize the head data.
+        force_conversion (bool): Convert it with instruction. Default is True.
+
+    Returns: Anonymized head of the DataFrame.
+    """
+
+    data_frame = copy_head(data_frame)
+    dtypes = data_frame.dtypes
+    for col in data_frame.columns:
+        col_idx = data_frame.columns.get_loc(col)
+        # check category type column and temporarily convert to object type
+        if force_conversion:
+            if pd.api.types.is_categorical_dtype(data_frame[col]):
+                if data_frame[col].isna().any():
+                    data_frame[col] = data_frame[col].astype(object)
+        for row_idx, val in enumerate(data_frame[col]):
+            cell_value = str(val)
+
+            if is_valid_email(cell_value):
+                data_frame.iloc[row_idx, col_idx] = generate_random_email()
+                continue
+            if is_valid_phone_number(cell_value):
+                data_frame.iloc[row_idx, col_idx] = generate_random_phone_number(
+                    cell_value
+                )
+                continue
+            if is_valid_credit_card(cell_value):
+                data_frame.iloc[row_idx, col_idx] = generate_random_credit_card()
+                continue
+
+            # anonymize data
+            random_row_index = random.choice(
+                [i for i in range(len(data_frame.index)) if i != row_idx]
+            )
+            random_value = data_frame.iloc[random_row_index, col_idx]
+            data_frame.iloc[row_idx, col_idx] = random_value
+            data_frame.iloc[random_row_index, col_idx] = (
+                pd.eval(cell_value) if cell_value in ["True", "False"] else cell_value
+            )
+    # restore the original data types
+    data_frame = data_frame.astype(dtypes)
+    return data_frame
```

### Comparing `hfttai-0.1.0/pandasai/helpers/from_excel.py` & `hfttai-0.1.2/pandasai/helpers/from_excel.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""
-Helper Module to Handle Data
-This module collects the helper function on handling various Data Sources.
-
-"""
-from __future__ import annotations
-
-import pandas as pd
-
-
-def from_excel(file, sheet: str | int | None = 0) -> pd.DataFrame:
-    """
-    Return a pandas DataFrame from an Excel file.
-    Wrapper for pandas.read_excel().
-
-    Args:
-        file (str):  A file path to be read
-        sheet (str | int): Name of the sheet or Sheet No. Default is 0
-
-    Returns (pd.DataFrame): A Pandas Dataframe
-
-    """
-
-    return pd.read_excel(file, sheet_name=sheet)
+"""
+Helper Module to Handle Data
+This module collects the helper function on handling various Data Sources.
+
+"""
+from __future__ import annotations
+
+import pandas as pd
+
+
+def from_excel(file, sheet: str | int | None = 0) -> pd.DataFrame:
+    """
+    Return a pandas DataFrame from an Excel file.
+    Wrapper for pandas.read_excel().
+
+    Args:
+        file (str):  A file path to be read
+        sheet (str | int): Name of the sheet or Sheet No. Default is 0
+
+    Returns (pd.DataFrame): A Pandas Dataframe
+
+    """
+
+    return pd.read_excel(file, sheet_name=sheet)
```

### Comparing `hfttai-0.1.0/pandasai/helpers/notebook.py` & `hfttai-0.1.2/pandasai/helpers/notebook.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-""" Helper Module to Handle Jupyter Notebook
-This module contains helper functions to interact with Jupyter Notebook Functionalities.
-
-"""
-
-from IPython import get_ipython
-
-
-class Notebook:
-
-    """Baseclass to implement Notebook helper functions"""
-
-    def in_notebook(self) -> bool:
-        """
-        Checks whether the code is running inside a notebook environment.
-
-        Returns (bool): True if the code is running inside a Jupyter notebook,
-        False otherwise.
-        """
-        try:
-            if "IPKernelApp" not in get_ipython().config:
-                return False
-        except (ImportError, AttributeError):
-            return False
-        return True
-
-    def create_new_cell(self, contents: str) -> None:
-        """
-        Creates a new code cell in the Jupyter notebook and populates
-        it with the specified contents.
-        Args:
-            contents (str): The contents to be added to the new code cell.
-
-        ImportError:
-            If the IPython module is not installed.
-
-        AttributeError:
-            If the 'get_ipython()' call raises an AttributeError, which can happen
-            if the code is not running inside a Jupyter notebook.
-
-        Returns: None
-
-        """
-
-        payload = {"source": "set_next_input", "text": contents, "replace": False}
-        try:
-            get_ipython().payload_manager.write_payload(payload, single=False)
-        except (ImportError, AttributeError) as exception:
-            raise exception
+""" Helper Module to Handle Jupyter Notebook
+This module contains helper functions to interact with Jupyter Notebook Functionalities.
+
+"""
+
+from IPython import get_ipython
+
+
+class Notebook:
+
+    """Baseclass to implement Notebook helper functions"""
+
+    def in_notebook(self) -> bool:
+        """
+        Checks whether the code is running inside a notebook environment.
+
+        Returns (bool): True if the code is running inside a Jupyter notebook,
+        False otherwise.
+        """
+        try:
+            if "IPKernelApp" not in get_ipython().config:
+                return False
+        except (ImportError, AttributeError):
+            return False
+        return True
+
+    def create_new_cell(self, contents: str) -> None:
+        """
+        Creates a new code cell in the Jupyter notebook and populates
+        it with the specified contents.
+        Args:
+            contents (str): The contents to be added to the new code cell.
+
+        ImportError:
+            If the IPython module is not installed.
+
+        AttributeError:
+            If the 'get_ipython()' call raises an AttributeError, which can happen
+            if the code is not running inside a Jupyter notebook.
+
+        Returns: None
+
+        """
+
+        payload = {"source": "set_next_input", "text": contents, "replace": False}
+        try:
+            get_ipython().payload_manager.write_payload(payload, single=False)
+        except (ImportError, AttributeError) as exception:
+            raise exception
```

### Comparing `hfttai-0.1.0/pandasai/helpers/save_chart.py` & `hfttai-0.1.2/pandasai/helpers/save_chart.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""Helper functions to save charts to a file, if plt.show() is called."""
-import ast
-import logging
-import os
-from itertools import zip_longest
-from os.path import dirname
-from typing import Union
-
-import astor
-
-
-def compare_ast(
-    node1: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
-    node2: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
-    ignore_args=False,
-) -> bool:
-    """
-    Compare two AST nodes for equality.
-    Source: https://stackoverflow.com/a/66733795/11080806
-
-    Args:
-        node1 (ast.AST): First AST node to compare.
-        node2 (ast.AST): Second AST node to compare.
-        ignore_args (bool, optional): Whether to ignore the arguments of the nodes.
-            Defaults to False.
-
-    Returns:
-        bool: True if the nodes are equal, False otherwise.
-
-    """
-    if type(node1) is not type(node2):
-        return False
-
-    if isinstance(node1, ast.AST):
-        for k, node in vars(node1).items():
-            if k in {"lineno", "end_lineno", "col_offset", "end_col_offset", "ctx"}:
-                continue
-            if ignore_args and k == "args":
-                continue
-            if not compare_ast(node, getattr(node2, k), ignore_args):
-                return False
-        return True
-
-    if isinstance(node1, list) and isinstance(node2, list):
-        return all(
-            compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
-        )
-
-    return node1 == node2
-
-
-def add_save_chart(
-    code: str,
-    folder_name: str,
-    save_charts_path: str = None,
-    print_save_dir: bool = True,
-) -> str:
-    """
-    Add line to code that save charts to a file, if plt.show() is called.
-
-    Args:
-        code (str): Code to add line to.
-        folder_name (str): Name of folder to save charts to.
-        save_charts_path (str): User Defined Path to save Charts
-        print_save_dir (bool): Print the save directory to the console.
-            Defaults to True.
-
-    Returns:
-        str: Code with line added.
-
-    """
-
-    if save_charts_path is not None:
-        charts_root_dir = save_charts_path
-    else:
-        # define chart save directory
-        charts_root_dir = dirname(dirname(dirname(__file__)))
-
-    chart_save_dir = os.path.join(charts_root_dir, "exports", "charts", folder_name)
-
-    tree = ast.parse(code)
-
-    # count number of plt.show() calls
-    show_count = sum(
-        compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
-        for node in ast.walk(tree)
-    )
-
-    # if there are no plt.show() calls, return the original code
-    if show_count == 0:
-        return code
-
-    if not os.path.exists(chart_save_dir):
-        os.makedirs(chart_save_dir)
-
-    # iterate through the AST and add plt.savefig() calls before plt.show() calls
-    counter = ord("a")
-    new_body = []
-    for node in tree.body:
-        if compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True):
-            filename = "chart"
-            if show_count > 1:
-                filename += f"_{chr(counter)}"
-                counter += 1
-
-            chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
-            new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
-        new_body.append(node)
-
-    chart_save_msg = f"Charts saving to: {chart_save_dir}"
-    if print_save_dir:
-        print(chart_save_msg)
-    logging.info(chart_save_msg)
-
-    new_tree = ast.Module(body=new_body)
-    return astor.to_source(new_tree).strip()
+"""Helper functions to save charts to a file, if plt.show() is called."""
+import ast
+import logging
+import os
+from itertools import zip_longest
+from os.path import dirname
+from typing import Union
+
+import astor
+
+
+def compare_ast(
+    node1: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
+    node2: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
+    ignore_args=False,
+) -> bool:
+    """
+    Compare two AST nodes for equality.
+    Source: https://stackoverflow.com/a/66733795/11080806
+
+    Args:
+        node1 (ast.AST): First AST node to compare.
+        node2 (ast.AST): Second AST node to compare.
+        ignore_args (bool, optional): Whether to ignore the arguments of the nodes.
+            Defaults to False.
+
+    Returns:
+        bool: True if the nodes are equal, False otherwise.
+
+    """
+    if type(node1) is not type(node2):
+        return False
+
+    if isinstance(node1, ast.AST):
+        for k, node in vars(node1).items():
+            if k in {"lineno", "end_lineno", "col_offset", "end_col_offset", "ctx"}:
+                continue
+            if ignore_args and k == "args":
+                continue
+            if not compare_ast(node, getattr(node2, k), ignore_args):
+                return False
+        return True
+
+    if isinstance(node1, list) and isinstance(node2, list):
+        return all(
+            compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
+        )
+
+    return node1 == node2
+
+
+def add_save_chart(
+    code: str,
+    folder_name: str,
+    save_charts_path: str = None,
+    print_save_dir: bool = True,
+) -> str:
+    """
+    Add line to code that save charts to a file, if plt.show() is called.
+
+    Args:
+        code (str): Code to add line to.
+        folder_name (str): Name of folder to save charts to.
+        save_charts_path (str): User Defined Path to save Charts
+        print_save_dir (bool): Print the save directory to the console.
+            Defaults to True.
+
+    Returns:
+        str: Code with line added.
+
+    """
+
+    if save_charts_path is not None:
+        charts_root_dir = save_charts_path
+    else:
+        # define chart save directory
+        charts_root_dir = dirname(dirname(dirname(__file__)))
+
+    chart_save_dir = os.path.join(charts_root_dir, "exports", "charts", folder_name)
+
+    tree = ast.parse(code)
+
+    # count number of plt.show() calls
+    show_count = sum(
+        compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
+        for node in ast.walk(tree)
+    )
+
+    # if there are no plt.show() calls, return the original code
+    if show_count == 0:
+        return code
+
+    if not os.path.exists(chart_save_dir):
+        os.makedirs(chart_save_dir)
+
+    # iterate through the AST and add plt.savefig() calls before plt.show() calls
+    counter = ord("a")
+    new_body = []
+    for node in tree.body:
+        if compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True):
+            filename = "chart"
+            if show_count > 1:
+                filename += f"_{chr(counter)}"
+                counter += 1
+
+            chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
+            new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
+        new_body.append(node)
+
+    chart_save_msg = f"Charts saving to: {chart_save_dir}"
+    if print_save_dir:
+        print(chart_save_msg)
+    logging.info(chart_save_msg)
+
+    new_tree = ast.Module(body=new_body)
+    return astor.to_source(new_tree).strip()
```

### Comparing `hfttai-0.1.0/pandasai/helpers/shortcuts.py` & `hfttai-0.1.2/pandasai/helpers/shortcuts.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-from typing import Union
-import pandas as pd
-from abc import ABC, abstractmethod
-
-
-class Shortcuts(ABC):
-    @abstractmethod
-    def run(self, df: pd.DataFrame, prompt: str) -> Union[str, pd.DataFrame]:
-        """
-        Run method from PandasAI class.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            prompt (str): The prompt to be executed.
-
-        Returns:
-            Union[str, pd.DataFrame]: The response from the LLM.
-        """
-
-        pass
-
-    def clean_data(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Do data cleaning and return the dataframe.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-
-        Returns:
-            pd.DataFrame: The cleaned DataFrame.
-        """
-
-        return self.run(
-            df,
-            """
-1. Copy the dataframe to a new variable named df_cleaned.
-2. Do data cleaning.
-3. Return df_cleaned.
-""",
-        )
-
-    def impute_missing_values(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Do missing value imputation and return the dataframe.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-
-        Returns:
-            pd.DataFrame: The DataFrame with imputed missing values.
-        """
-
-        return self.run(
-            df,
-            """
-1. Copy the dataframe to a new variable named df_imputed.
-2. Do the imputation of missing values.
-3. Return df_imputed.
-""",
-        )
-
-    def generate_features(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Do feature generation and return the dataframe.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-
-        Returns:
-            pd.DataFrame: The DataFrame with generated features.
-        """
-
-        return self.run(
-            df,
-            """
-1. Copy the dataframe to a new variable named df_features.
-2. Do feature generation.
-3. Return df_features.
-""",
-        )
-
-    def plot_pie_chart(self, df: pd.DataFrame, labels: list, values: list) -> None:
-        """
-        Plot a pie chart.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            labels (list): The labels for the pie chart.
-            values (list): The values for the pie chart.
-
-        Returns:
-            None
-        """
-
-        self.run(
-            df,
-            f"""
-Plot a pie chart with the following labels and values:
-labels = {labels}
-values = {values}
-""",
-        )
-
-    def plot_bar_chart(self, df: pd.DataFrame, x: list, y: list) -> None:
-        """
-        Plot a bar chart.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            x (list): The x values for the bar chart.
-            y (list): The y values for the bar chart.
-
-        Returns:
-            None
-        """
-
-        self.run(
-            df,
-            f"""
-Plot a bar chart with the following x and y:
-x = {x}
-y = {y}
-""",
-        )
-
-    def plot_histogram(self, df: pd.DataFrame, column: str) -> None:
-        """
-        Plot a histogram.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            column (str): The column to plot the histogram for.
-
-        Returns:
-            None
-        """
-
-        self.run(df, f"Plot a histogram of the column {column}.")
-
-    def plot_line_chart(self, df: pd.DataFrame, x: list, y: list) -> None:
-        """
-        Plot a line chart.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            x (list): The x values for the line chart.
-            y (list): The y values for the line chart.
-
-        Returns:
-            None
-        """
-
-        self.run(
-            df,
-            f"""
-Plot a line chart with the following x and y:
-x = {x}
-y = {y}
-""",
-        )
-
-    def plot_scatter_chart(self, df: pd.DataFrame, x: list, y: list) -> None:
-        """
-        Plot a scatter chart.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            x (list): The x values for the scatter chart.
-            y (list): The y values for the scatter chart.
-
-        Returns:
-            None
-        """
-
-        self.run(
-            df,
-            f"""
-Plot a scatter chart with the following x and y:
-x = {x}
-y = {y}
-""",
-        )
-
-    def plot_correlation_heatmap(self, df: pd.DataFrame) -> None:
-        """
-        Plot a correlation heatmap.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-
-        Returns:
-            None
-        """
-
-        self.run(df, "Plot a correlation heatmap.")
-
-    def plot_confusion_matrix(
-        self, df: pd.DataFrame, y_true: list, y_pred: list
-    ) -> None:
-        """
-        Plot a confusion matrix.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            y_true (list): The true values.
-            y_pred (list): The predicted values.
-
-        Returns:
-            None
-        """
-
-        self.run(
-            df,
-            f"""
-Plot a confusion matrix with the following y_true and y_pred:
-y_true = {y_true}
-y_pred = {y_pred}
-""",
-        )
-
-    def plot_roc_curve(self, df: pd.DataFrame, y_true: list, y_pred: list) -> None:
-        """
-        Plot a ROC curve.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            y_true (list): The true values.
-            y_pred (list): The predicted values.
-
-        Returns:
-            None
-        """
-
-        self.run(
-            df,
-            f"""
-Plot a ROC curve with the following y_true and y_pred:
-y_true = {y_true}
-y_pred = {y_pred}
-""",
-        )
-
-    def boxplot(
-        self,
-        df: pd.DataFrame,
-        col: Union[str, list[str]] = None,
-        by: Union[str, list[str]] = None,
-        style: str = None,
-    ):
-        """
-        Draw a box plot to show distributions with respect to categories.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            col (str | list[str] | None): The column(s) of interest
-            for the box plot. Defaults to None.
-            by (str | list[str] | None): The grouping variable(s)
-            for the box plot. Defaults to None.
-            style (str | None): The textual description of the desired
-            style. Defaults to None.
-
-        Returns:
-            str: LLM response
-        """
-
-        if not isinstance(col, (str, list, type(None))):
-            raise TypeError(
-                "The 'col' argument must be a string, a list of strings, or None."
-            )
-        if not isinstance(by, (str, list, type(None))):
-            raise TypeError(
-                "The 'by' argument must be a string, a list of strings, or None."
-            )
-
-        prompt = "Plot a box-and-whisker plot"
-
-        if isinstance(col, str):
-            prompt += f" for the variable '{col}'"
-        elif isinstance(col, list):
-            var_list = [f"'{v}'" for v in col]
-            if len(var_list) > 1:
-                variables_str = ", ".join(var_list[:-1])
-                prompt += f" for the variables {variables_str} and {var_list[-1]}"
-            else:
-                prompt += f" for the variable {var_list[0]}"
-
-        if by is not None:
-            prompt += f" grouped by '{by}'"
-
-        if style is not None:
-            prompt += f"\nStyle: '''{style}'''"
-
-        self.run(df, prompt)
-
-    def rolling_mean(self, df: pd.DataFrame, column: str, window: int) -> pd.DataFrame:
-        """
-        Calculate the rolling mean.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            column (str): The column to calculate the rolling mean for.
-            window (int): The window size.
-
-        Returns:
-            pd.DataFrame: The DataFrame containing the rolling mean.
-        """
-
-        return self.run(
-            df,
-            f"Calculate the rolling mean of the column {column} with a window"
-            " of {window}.",
-        )
-
-    def rolling_median(
-        self, df: pd.DataFrame, column: str, window: int
-    ) -> pd.DataFrame:
-        """
-        Calculate the rolling median.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            column (str): The column to calculate the rolling median for.
-            window (int): The window size.
-
-        Returns:
-            pd.DataFrame: The DataFrame containing the rolling median.
-        """
-
-        return self.run(
-            df,
-            f"Calculate the rolling median of the column {column} with a window"
-            " of {window}.",
-        )
-
-    def rolling_std(self, df: pd.DataFrame, column: str, window: int) -> pd.DataFrame:
-        """
-        Calculate the rolling standard deviation.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            column (str): The column to calculate the rolling standard deviation for.
-            window (int): The window size.
-
-        Returns:
-            pd.DataFrame: The DataFrame containing the rolling standard deviation.
-        """
-
-        return self.run(
-            df,
-            f"Calculate the rolling standard deviation of the column {column} with a"
-            "window of {window}.",
-        )
-
-    def segment_customers(
-        self, df: pd.DataFrame, features: list, n_clusters: int
-    ) -> pd.DataFrame:
-        """
-        Segment customers.
-
-        Args:
-            df (pd.DataFrame): The DataFrame containing the data.
-            features (list): The features to use for the segmentation.
-            n_clusters (int): The number of clusters.
-
-        Returns:
-            pd.DataFrame: The DataFrame containing the segmentation.
-        """
-
-        return self.run(
-            df,
-            f"""
-Segment customers with the following features and number of clusters:
-features = {features}
-n_clusters = {n_clusters}
-""",
-        )
+from typing import Union
+import pandas as pd
+from abc import ABC, abstractmethod
+
+
+class Shortcuts(ABC):
+    @abstractmethod
+    def run(self, df: pd.DataFrame, prompt: str) -> Union[str, pd.DataFrame]:
+        """
+        Run method from PandasAI class.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            prompt (str): The prompt to be executed.
+
+        Returns:
+            Union[str, pd.DataFrame]: The response from the LLM.
+        """
+
+        pass
+
+    def clean_data(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Do data cleaning and return the dataframe.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+
+        Returns:
+            pd.DataFrame: The cleaned DataFrame.
+        """
+
+        return self.run(
+            df,
+            """
+1. Copy the dataframe to a new variable named df_cleaned.
+2. Do data cleaning.
+3. Return df_cleaned.
+""",
+        )
+
+    def impute_missing_values(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Do missing value imputation and return the dataframe.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+
+        Returns:
+            pd.DataFrame: The DataFrame with imputed missing values.
+        """
+
+        return self.run(
+            df,
+            """
+1. Copy the dataframe to a new variable named df_imputed.
+2. Do the imputation of missing values.
+3. Return df_imputed.
+""",
+        )
+
+    def generate_features(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Do feature generation and return the dataframe.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+
+        Returns:
+            pd.DataFrame: The DataFrame with generated features.
+        """
+
+        return self.run(
+            df,
+            """
+1. Copy the dataframe to a new variable named df_features.
+2. Do feature generation.
+3. Return df_features.
+""",
+        )
+
+    def plot_pie_chart(self, df: pd.DataFrame, labels: list, values: list) -> None:
+        """
+        Plot a pie chart.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            labels (list): The labels for the pie chart.
+            values (list): The values for the pie chart.
+
+        Returns:
+            None
+        """
+
+        self.run(
+            df,
+            f"""
+Plot a pie chart with the following labels and values:
+labels = {labels}
+values = {values}
+""",
+        )
+
+    def plot_bar_chart(self, df: pd.DataFrame, x: list, y: list) -> None:
+        """
+        Plot a bar chart.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            x (list): The x values for the bar chart.
+            y (list): The y values for the bar chart.
+
+        Returns:
+            None
+        """
+
+        self.run(
+            df,
+            f"""
+Plot a bar chart with the following x and y:
+x = {x}
+y = {y}
+""",
+        )
+
+    def plot_histogram(self, df: pd.DataFrame, column: str) -> None:
+        """
+        Plot a histogram.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            column (str): The column to plot the histogram for.
+
+        Returns:
+            None
+        """
+
+        self.run(df, f"Plot a histogram of the column {column}.")
+
+    def plot_line_chart(self, df: pd.DataFrame, x: list, y: list) -> None:
+        """
+        Plot a line chart.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            x (list): The x values for the line chart.
+            y (list): The y values for the line chart.
+
+        Returns:
+            None
+        """
+
+        self.run(
+            df,
+            f"""
+Plot a line chart with the following x and y:
+x = {x}
+y = {y}
+""",
+        )
+
+    def plot_scatter_chart(self, df: pd.DataFrame, x: list, y: list) -> None:
+        """
+        Plot a scatter chart.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            x (list): The x values for the scatter chart.
+            y (list): The y values for the scatter chart.
+
+        Returns:
+            None
+        """
+
+        self.run(
+            df,
+            f"""
+Plot a scatter chart with the following x and y:
+x = {x}
+y = {y}
+""",
+        )
+
+    def plot_correlation_heatmap(self, df: pd.DataFrame) -> None:
+        """
+        Plot a correlation heatmap.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+
+        Returns:
+            None
+        """
+
+        self.run(df, "Plot a correlation heatmap.")
+
+    def plot_confusion_matrix(
+        self, df: pd.DataFrame, y_true: list, y_pred: list
+    ) -> None:
+        """
+        Plot a confusion matrix.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            y_true (list): The true values.
+            y_pred (list): The predicted values.
+
+        Returns:
+            None
+        """
+
+        self.run(
+            df,
+            f"""
+Plot a confusion matrix with the following y_true and y_pred:
+y_true = {y_true}
+y_pred = {y_pred}
+""",
+        )
+
+    def plot_roc_curve(self, df: pd.DataFrame, y_true: list, y_pred: list) -> None:
+        """
+        Plot a ROC curve.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            y_true (list): The true values.
+            y_pred (list): The predicted values.
+
+        Returns:
+            None
+        """
+
+        self.run(
+            df,
+            f"""
+Plot a ROC curve with the following y_true and y_pred:
+y_true = {y_true}
+y_pred = {y_pred}
+""",
+        )
+
+    def boxplot(
+        self,
+        df: pd.DataFrame,
+        col: Union[str, list[str]] = None,
+        by: Union[str, list[str]] = None,
+        style: str = None,
+    ):
+        """
+        Draw a box plot to show distributions with respect to categories.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            col (str | list[str] | None): The column(s) of interest
+            for the box plot. Defaults to None.
+            by (str | list[str] | None): The grouping variable(s)
+            for the box plot. Defaults to None.
+            style (str | None): The textual description of the desired
+            style. Defaults to None.
+
+        Returns:
+            str: LLM response
+        """
+
+        if not isinstance(col, (str, list, type(None))):
+            raise TypeError(
+                "The 'col' argument must be a string, a list of strings, or None."
+            )
+        if not isinstance(by, (str, list, type(None))):
+            raise TypeError(
+                "The 'by' argument must be a string, a list of strings, or None."
+            )
+
+        prompt = "Plot a box-and-whisker plot"
+
+        if isinstance(col, str):
+            prompt += f" for the variable '{col}'"
+        elif isinstance(col, list):
+            var_list = [f"'{v}'" for v in col]
+            if len(var_list) > 1:
+                variables_str = ", ".join(var_list[:-1])
+                prompt += f" for the variables {variables_str} and {var_list[-1]}"
+            else:
+                prompt += f" for the variable {var_list[0]}"
+
+        if by is not None:
+            prompt += f" grouped by '{by}'"
+
+        if style is not None:
+            prompt += f"\nStyle: '''{style}'''"
+
+        self.run(df, prompt)
+
+    def rolling_mean(self, df: pd.DataFrame, column: str, window: int) -> pd.DataFrame:
+        """
+        Calculate the rolling mean.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            column (str): The column to calculate the rolling mean for.
+            window (int): The window size.
+
+        Returns:
+            pd.DataFrame: The DataFrame containing the rolling mean.
+        """
+
+        return self.run(
+            df,
+            f"Calculate the rolling mean of the column {column} with a window"
+            " of {window}.",
+        )
+
+    def rolling_median(
+        self, df: pd.DataFrame, column: str, window: int
+    ) -> pd.DataFrame:
+        """
+        Calculate the rolling median.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            column (str): The column to calculate the rolling median for.
+            window (int): The window size.
+
+        Returns:
+            pd.DataFrame: The DataFrame containing the rolling median.
+        """
+
+        return self.run(
+            df,
+            f"Calculate the rolling median of the column {column} with a window"
+            " of {window}.",
+        )
+
+    def rolling_std(self, df: pd.DataFrame, column: str, window: int) -> pd.DataFrame:
+        """
+        Calculate the rolling standard deviation.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            column (str): The column to calculate the rolling standard deviation for.
+            window (int): The window size.
+
+        Returns:
+            pd.DataFrame: The DataFrame containing the rolling standard deviation.
+        """
+
+        return self.run(
+            df,
+            f"Calculate the rolling standard deviation of the column {column} with a"
+            "window of {window}.",
+        )
+
+    def segment_customers(
+        self, df: pd.DataFrame, features: list, n_clusters: int
+    ) -> pd.DataFrame:
+        """
+        Segment customers.
+
+        Args:
+            df (pd.DataFrame): The DataFrame containing the data.
+            features (list): The features to use for the segmentation.
+            n_clusters (int): The number of clusters.
+
+        Returns:
+            pd.DataFrame: The DataFrame containing the segmentation.
+        """
+
+        return self.run(
+            df,
+            f"""
+Segment customers with the following features and number of clusters:
+features = {features}
+n_clusters = {n_clusters}
+""",
+        )
```

### Comparing `hfttai-0.1.0/pandasai/llm/azure_openai.py` & `hfttai-0.1.2/pandasai/llm/azure_openai.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-"""OpenAI LLM via Microsoft Azure Cloud
-
-This module is to run the OpenAI API when using Microsoft Cloud infrastructure.
-Azure has implemented the openai API access to its platform.
-For details https://learn.microsoft.com/en-us/azure/cognitive-services/openai/reference.
-
-Example:
-    Use below example to call AzureOpenAI class
-
-    >>> from pandasai.llm.azure_openai import AzureOpenAI
-
-"""
-
-import os
-from typing import Any, Dict, Optional
-
-import openai
-from dotenv import load_dotenv
-
-from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
-from .base import BaseOpenAI
-
-load_dotenv()
-
-
-class AzureOpenAI(BaseOpenAI):
-    """OpenAI LLM via Microsoft Azure
-    This class in using BaseOpenAI class to include Azure OpenAI Features.
-    """
-
-    api_base: str
-    api_type: str = "azure"
-    api_version: str
-    engine: str
-
-    def __init__(
-        self,
-        api_token: Optional[str] = None,
-        api_base: Optional[str] = None,
-        api_version: Optional[str] = None,
-        deployment_name: str = None,
-        is_chat_model: Optional[bool] = False,
-        **kwargs,
-    ):
-        """
-        __init__ method of AzureOpenAI Class
-
-        Args:
-            api_token (str): Azure OpenAI API token.
-            api_base (str): Base url of the Azure endpoint.
-                It should look like the following:
-                <https://YOUR_RESOURCE_NAME.openai.azure.com/>
-            api_version (str): Version of the Azure OpenAI API.
-                Be aware the API version may change.
-            deployment_name (str): Custom name of the deployed model
-            is_chat_model (bool): Whether ``deployment_name`` corresponds to a Chat
-                or a Completion model
-            **kwargs: Inference Parameters
-        """
-
-        self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
-        self.api_base = api_base or os.getenv("OPENAI_API_BASE") or None
-        self.api_version = api_version or os.getenv("OPENAI_API_VERSION")
-        if self.api_token is None:
-            raise APIKeyNotFoundError(
-                "Azure OpenAI key is required. Please add an environment variable "
-                "`OPENAI_API_KEY` or pass `api_token` as a named parameter"
-            )
-        if self.api_base is None:
-            raise APIKeyNotFoundError(
-                "Azure OpenAI base is required. Please add an environment variable "
-                "`OPENAI_API_BASE` or pass `api_base` as a named parameter"
-            )
-        if self.api_version is None:
-            raise APIKeyNotFoundError(
-                "Azure OpenAI version is required. Please add an environment variable "
-                "`OPENAI_API_VERSION` or pass `api_version` as a named parameter"
-            )
-        openai.api_key = self.api_token
-        openai.api_base = self.api_base
-        openai.api_version = self.api_version
-        openai.api_type = self.api_type
-
-        if deployment_name is None:
-            raise UnsupportedOpenAIModelError("Model deployment name is required.")
-
-        self.is_chat_model = is_chat_model
-        self.engine = deployment_name
-
-        self.openai_proxy = kwargs.get("openai_proxy") or os.getenv("OPENAI_PROXY")
-        if self.openai_proxy:
-            openai.proxy = {
-                "http": self.openai_proxy,
-                "https": self.openai_proxy
-            }
-
-        self._set_params(**kwargs)
-
-    @property
-    def _default_params(self) -> Dict[str, Any]:
-        """Get the default parameters for calling OpenAI API
-
-        Returns: A dict of Default Params
-
-        """
-        return {**super()._default_params, "engine": self.engine}
-
-    def call(self, instruction: str, value: str, suffix: str = "") -> str:
-        """
-        Call the Azure OpenAI LLM.
-
-        Args:
-            instruction (str): Instruction to pass
-            value (str): Value to pass
-            suffix(str): Suffix to pass
-
-        Returns:
-            str: Response
-        """
-        self.last_prompt = str(instruction) + str(value)
-
-        if self.is_chat_model:
-            response = self.chat_completion(str(instruction) + str(value) + suffix)
-        else:
-            response = self.completion(str(instruction) + str(value) + suffix)
-
-        return response
-
-    @property
-    def type(self) -> str:
-        return "azure-openai"
+"""OpenAI LLM via Microsoft Azure Cloud
+
+This module is to run the OpenAI API when using Microsoft Cloud infrastructure.
+Azure has implemented the openai API access to its platform.
+For details https://learn.microsoft.com/en-us/azure/cognitive-services/openai/reference.
+
+Example:
+    Use below example to call AzureOpenAI class
+
+    >>> from pandasai.llm.azure_openai import AzureOpenAI
+
+"""
+
+import os
+from typing import Any, Dict, Optional
+
+import openai
+from dotenv import load_dotenv
+
+from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
+from .base import BaseOpenAI
+
+load_dotenv()
+
+
+class AzureOpenAI(BaseOpenAI):
+    """OpenAI LLM via Microsoft Azure
+    This class in using BaseOpenAI class to include Azure OpenAI Features.
+    """
+
+    api_base: str
+    api_type: str = "azure"
+    api_version: str
+    engine: str
+
+    def __init__(
+        self,
+        api_token: Optional[str] = None,
+        api_base: Optional[str] = None,
+        api_version: Optional[str] = None,
+        deployment_name: str = None,
+        is_chat_model: Optional[bool] = False,
+        **kwargs,
+    ):
+        """
+        __init__ method of AzureOpenAI Class
+
+        Args:
+            api_token (str): Azure OpenAI API token.
+            api_base (str): Base url of the Azure endpoint.
+                It should look like the following:
+                <https://YOUR_RESOURCE_NAME.openai.azure.com/>
+            api_version (str): Version of the Azure OpenAI API.
+                Be aware the API version may change.
+            deployment_name (str): Custom name of the deployed model
+            is_chat_model (bool): Whether ``deployment_name`` corresponds to a Chat
+                or a Completion model
+            **kwargs: Inference Parameters
+        """
+
+        self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
+        self.api_base = api_base or os.getenv("OPENAI_API_BASE") or None
+        self.api_version = api_version or os.getenv("OPENAI_API_VERSION")
+        if self.api_token is None:
+            raise APIKeyNotFoundError(
+                "Azure OpenAI key is required. Please add an environment variable "
+                "`OPENAI_API_KEY` or pass `api_token` as a named parameter"
+            )
+        if self.api_base is None:
+            raise APIKeyNotFoundError(
+                "Azure OpenAI base is required. Please add an environment variable "
+                "`OPENAI_API_BASE` or pass `api_base` as a named parameter"
+            )
+        if self.api_version is None:
+            raise APIKeyNotFoundError(
+                "Azure OpenAI version is required. Please add an environment variable "
+                "`OPENAI_API_VERSION` or pass `api_version` as a named parameter"
+            )
+        openai.api_key = self.api_token
+        openai.api_base = self.api_base
+        openai.api_version = self.api_version
+        openai.api_type = self.api_type
+
+        if deployment_name is None:
+            raise UnsupportedOpenAIModelError("Model deployment name is required.")
+
+        self.is_chat_model = is_chat_model
+        self.engine = deployment_name
+
+        self.openai_proxy = kwargs.get("openai_proxy") or os.getenv("OPENAI_PROXY")
+        if self.openai_proxy:
+            openai.proxy = {
+                "http": self.openai_proxy,
+                "https": self.openai_proxy
+            }
+
+        self._set_params(**kwargs)
+
+    @property
+    def _default_params(self) -> Dict[str, Any]:
+        """Get the default parameters for calling OpenAI API
+
+        Returns: A dict of Default Params
+
+        """
+        return {**super()._default_params, "engine": self.engine}
+
+    def call(self, instruction: str, value: str, suffix: str = "") -> str:
+        """
+        Call the Azure OpenAI LLM.
+
+        Args:
+            instruction (str): Instruction to pass
+            value (str): Value to pass
+            suffix(str): Suffix to pass
+
+        Returns:
+            str: Response
+        """
+        self.last_prompt = str(instruction) + str(value)
+
+        if self.is_chat_model:
+            response = self.chat_completion(str(instruction) + str(value) + suffix)
+        else:
+            response = self.completion(str(instruction) + str(value) + suffix)
+
+        return response
+
+    @property
+    def type(self) -> str:
+        return "azure-openai"
```

### Comparing `hfttai-0.1.0/pandasai/llm/base.py` & `hfttai-0.1.2/pandasai/llm/base.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,417 +1,417 @@
-""" Base class to implement a new LLM
-
-This module is the base class to integrate the various LLMs API. This module also
-includes the Base LLM classes for OpenAI, HuggingFace and Google PaLM.
-
-Example:
-
-    ```
-    from .base import BaseOpenAI
-
-    class CustomLLM(BaseOpenAI):
-
-        Custom Class Starts here!!
-    ```
-"""
-
-import ast
-import re
-from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional
-
-import openai
-import requests
-
-from ..exceptions import (
-    APIKeyNotFoundError,
-    MethodNotImplementedError,
-    NoCodeFoundError,
-)
-from ..helpers._optional import import_dependency
-from ..prompts.base import Prompt
-
-
-class LLM:
-    """Base class to implement a new LLM."""
-
-    last_prompt: Optional[str] = None
-
-    def is_pandasai_llm(self) -> bool:
-        """
-        Return True if the LLM is from pandasAI.
-
-        Returns:
-            bool: True if the LLM is from pandasAI
-        """
-        return True
-
-    @property
-    def type(self) -> str:
-        """
-        Return type of LLM.
-
-        Raises:
-            APIKeyNotFoundError: Type has not been implemented
-
-        Returns:
-            str: Type of LLM a string
-        """
-        raise APIKeyNotFoundError("Type has not been implemented")
-
-    def _polish_code(self, code: str) -> str:
-        """
-        Polish the code by removing the leading "python" or "py",  \
-        removing the imports and removing trailing spaces and new lines.
-
-        Args:
-            code (str): Code
-
-        Returns:
-            str: Polished code
-        """
-        if re.match(r"^(python|py)", code):
-            code = re.sub(r"^(python|py)", "", code)
-        if re.match(r"^`.*`$", code):
-            code = re.sub(r"^`(.*)`$", r"\1", code)
-        code = code.strip()
-        return code
-
-    def _is_python_code(self, string):
-        """
-        Return True if it is valid python code.
-        Args:
-            string (str):
-
-        Returns (bool): True if Python Code otherwise False
-
-        """
-        try:
-            ast.parse(string)
-            return True
-        except SyntaxError:
-            return False
-
-    def _extract_code(self, response: str, separator: str = "```") -> str:
-        """
-        Extract the code from the response.
-
-        Args:
-            response (str): Response
-            separator (str, optional): Separator. Defaults to "```".
-
-        Raises:
-            NoCodeFoundError: No code found in the response
-
-        Returns:
-            str: Extracted code from the response
-        """
-        code = response
-        if len(code.split(separator)) > 1:
-            code = code.split(separator)[1]
-        code = self._polish_code(code)
-        if not self._is_python_code(code):
-            raise NoCodeFoundError("No code found in the response")
-
-        return code
-
-    @abstractmethod
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-        """
-        Execute the LLM with given prompt.
-
-        Args:
-            instruction (Prompt): Prompt
-            value (str): Value
-            suffix (str, optional): Suffix. Defaults to "".
-
-        Raises:
-            MethodNotImplementedError: Call method has not been implemented
-        """
-        raise MethodNotImplementedError("Call method has not been implemented")
-
-    def generate_code(self, instruction: Prompt, prompt: str) -> str:
-        """
-        Generate the code based on the instruction and the given prompt.
-
-        Returns:
-            str: Code
-        """
-        return self._extract_code(self.call(instruction, prompt, suffix="\n\nCode:\n"))
-
-
-class BaseOpenAI(LLM, ABC):
-    """Base class to implement a new OpenAI LLM
-    LLM base class, this class is extended to be used with OpenAI API.
-
-    """
-
-    api_token: str
-    temperature: float = 0
-    max_tokens: int = 512
-    top_p: float = 1
-    frequency_penalty: float = 0
-    presence_penalty: float = 0.6
-    stop: Optional[str] = None
-    # support explicit proxy for OpenAI
-    openai_proxy: Optional[str] = None
-
-    def _set_params(self, **kwargs):
-        """
-        Set Parameters
-        Args:
-            **kwargs: ["model", "engine", "deployment_id", "temperature","max_tokens",
-            "top_p", "frequency_penalty", "presence_penalty", "stop", ]
-
-        Returns: None
-
-        """
-
-        valid_params = [
-            "model",
-            "engine",
-            "deployment_id",
-            "temperature",
-            "max_tokens",
-            "top_p",
-            "frequency_penalty",
-            "presence_penalty",
-            "stop",
-        ]
-        for key, value in kwargs.items():
-            if key in valid_params:
-                setattr(self, key, value)
-
-    @property
-    def _default_params(self) -> Dict[str, Any]:
-        """
-        Get the default parameters for calling OpenAI API
-
-        Returns (Dict): A dict of OpenAi API parameters
-
-        """
-
-        return {
-            "temperature": self.temperature,
-            "max_tokens": self.max_tokens,
-            "top_p": self.top_p,
-            "frequency_penalty": self.frequency_penalty,
-            "presence_penalty": self.presence_penalty,
-        }
-
-    def completion(self, prompt: str) -> str:
-        """
-        Query the completion API
-
-        Args:
-            prompt (str): Prompt
-
-        Returns:
-            str: LLM response
-        """
-        params = {**self._default_params, "prompt": prompt}
-
-        if self.stop is not None:
-            params["stop"] = [self.stop]
-
-        response = openai.Completion.create(**params)
-
-        return response["choices"][0]["text"]
-
-    def chat_completion(self, value: str) -> str:
-        """
-        Query the chat completion API
-
-        Args:
-            value (str): Prompt
-
-        Returns:
-            str: LLM response
-        """
-        params = {
-            **self._default_params,
-            "messages": [
-                {
-                    "role": "system",
-                    "content": value,
-                }
-            ],
-        }
-
-        if self.stop is not None:
-            params["stop"] = [self.stop]
-
-        response = openai.ChatCompletion.create(**params)
-
-        return response["choices"][0]["message"]["content"]
-
-
-class HuggingFaceLLM(LLM):
-    """Base class to implement a new Hugging Face LLM.
-
-    LLM base class is extended to be used with HuggingFace LLM Modes APIs
-
-    """
-
-    last_prompt: Optional[str] = None
-    api_token: str
-    _api_url: str = "https://api-inference.huggingface.co/models/"
-    _max_retries: int = 3
-
-    @property
-    def type(self) -> str:
-        return "huggingface-llm"
-
-    def query(self, payload):
-        """
-        Query the HF API
-        Args:
-            payload: A JSON form payload
-
-        Returns: Generated Response
-
-        """
-
-        headers = {"Authorization": f"Bearer {self.api_token}"}
-
-        response = requests.post(
-            self._api_url, headers=headers, json=payload, timeout=60
-        )
-
-        return response.json()[0]["generated_text"]
-
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-        """
-        A call method of HuggingFaceLLM class.
-        Args:
-            instruction (object): A prompt object
-            value (str):
-            suffix (str):
-
-        Returns (str): A string response
-
-        """
-
-        prompt = str(instruction)
-        payload = prompt + value + suffix
-
-        # sometimes the API doesn't return a valid response, so we retry passing the
-        # output generated from the previous call as the input
-        for _i in range(self._max_retries):
-            response = self.query({"inputs": payload})
-            payload = response
-            if response.count("<endCode>") >= 2:
-                break
-
-        # replace instruction + value from the inputs to avoid showing it in the output
-        output = response.replace(prompt + value + suffix, "")
-        return output
-
-
-class BaseGoogle(LLM):
-    """Base class to implement a new Google LLM
-
-    LLM base class is extended to be used with Google Palm API.
-    """
-
-    genai: Any
-    temperature: Optional[float] = 0
-    top_p: Optional[float] = 0.8
-    top_k: Optional[float] = 0.3
-    max_output_tokens: Optional[int] = 1000
-
-    def _configure(self, api_key: str):
-        """
-        Configure Google Palm API Key
-        Args:
-            api_key (str): A string of API keys generated from Google Cloud
-
-        Returns:
-
-        """
-
-        if not api_key:
-            raise APIKeyNotFoundError("Google Palm API key is required")
-
-        err_msg = "Install google-generativeai >= 0.1 for Google Palm API"
-        genai = import_dependency("google.generativeai", extra=err_msg)
-
-        genai.configure(api_key=api_key)
-        self.genai = genai
-
-    def _configurevertexai(self, project_id: str, location: str):
-        """
-        Configure Google VertexAi
-        Args:
-            project_id: GCP Project
-            location: Location of Project
-
-        Returns: Vertexai Object
-
-        """
-
-        err_msg = "Install google-cloud-aiplatform for Google Vertexai"
-        vertexai = import_dependency("vertexai", extra=err_msg)
-        vertexai.init(project=project_id, location=location)
-        self.vertexai = vertexai
-
-    def _valid_params(self):
-        return ["temperature", "top_p", "top_k", "max_output_tokens"]
-
-    def _set_params(self, **kwargs):
-        """
-        Set Parameters
-        Args:
-            **kwargs: ["temperature", "top_p", "top_k", "max_output_tokens"]
-
-        Returns:
-
-        """
-
-        valid_params = self._valid_params()
-        for key, value in kwargs.items():
-            if key in valid_params:
-                setattr(self, key, value)
-
-    def _validate(self):
-        """Validates the parameters for Google"""
-
-        if self.temperature is not None and not 0 <= self.temperature <= 1:
-            raise ValueError("temperature must be in the range [0.0, 1.0]")
-
-        if self.top_p is not None and not 0 <= self.top_p <= 1:
-            raise ValueError("top_p must be in the range [0.0, 1.0]")
-
-        if self.top_k is not None and not 0 <= self.top_k <= 1:
-            raise ValueError("top_k must be in the range [0.0, 1.0]")
-
-        if self.max_output_tokens is not None and self.max_output_tokens <= 0:
-            raise ValueError("max_output_tokens must be greater than zero")
-
-    @abstractmethod
-    def _generate_text(self, prompt: str) -> str:
-        """
-        Generates text for prompt, specific to implementation.
-
-        Args:
-            prompt (str): Prompt
-
-        Returns:
-            str: LLM response
-        """
-        raise MethodNotImplementedError("method has not been implemented")
-
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-        """
-        Call the Google LLM.
-
-        Args:
-            instruction (object): Instruction to pass
-            value (str): Value to pass
-            suffix (str): Suffix to pass
-
-        Returns:
-            str: Response
-        """
-        self.last_prompt = str(instruction) + value
-        prompt = str(instruction) + value + suffix
-        return self._generate_text(prompt)
+""" Base class to implement a new LLM
+
+This module is the base class to integrate the various LLMs API. This module also
+includes the Base LLM classes for OpenAI, HuggingFace and Google PaLM.
+
+Example:
+
+    ```
+    from .base import BaseOpenAI
+
+    class CustomLLM(BaseOpenAI):
+
+        Custom Class Starts here!!
+    ```
+"""
+
+import ast
+import re
+from abc import ABC, abstractmethod
+from typing import Any, Dict, Optional
+
+import openai
+import requests
+
+from ..exceptions import (
+    APIKeyNotFoundError,
+    MethodNotImplementedError,
+    NoCodeFoundError,
+)
+from ..helpers._optional import import_dependency
+from ..prompts.base import Prompt
+
+
+class LLM:
+    """Base class to implement a new LLM."""
+
+    last_prompt: Optional[str] = None
+
+    def is_pandasai_llm(self) -> bool:
+        """
+        Return True if the LLM is from pandasAI.
+
+        Returns:
+            bool: True if the LLM is from pandasAI
+        """
+        return True
+
+    @property
+    def type(self) -> str:
+        """
+        Return type of LLM.
+
+        Raises:
+            APIKeyNotFoundError: Type has not been implemented
+
+        Returns:
+            str: Type of LLM a string
+        """
+        raise APIKeyNotFoundError("Type has not been implemented")
+
+    def _polish_code(self, code: str) -> str:
+        """
+        Polish the code by removing the leading "python" or "py",  \
+        removing the imports and removing trailing spaces and new lines.
+
+        Args:
+            code (str): Code
+
+        Returns:
+            str: Polished code
+        """
+        if re.match(r"^(python|py)", code):
+            code = re.sub(r"^(python|py)", "", code)
+        if re.match(r"^`.*`$", code):
+            code = re.sub(r"^`(.*)`$", r"\1", code)
+        code = code.strip()
+        return code
+
+    def _is_python_code(self, string):
+        """
+        Return True if it is valid python code.
+        Args:
+            string (str):
+
+        Returns (bool): True if Python Code otherwise False
+
+        """
+        try:
+            ast.parse(string)
+            return True
+        except SyntaxError:
+            return False
+
+    def _extract_code(self, response: str, separator: str = "```") -> str:
+        """
+        Extract the code from the response.
+
+        Args:
+            response (str): Response
+            separator (str, optional): Separator. Defaults to "```".
+
+        Raises:
+            NoCodeFoundError: No code found in the response
+
+        Returns:
+            str: Extracted code from the response
+        """
+        code = response
+        if len(code.split(separator)) > 1:
+            code = code.split(separator)[1]
+        code = self._polish_code(code)
+        if not self._is_python_code(code):
+            raise NoCodeFoundError("No code found in the response")
+
+        return code
+
+    @abstractmethod
+    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+        """
+        Execute the LLM with given prompt.
+
+        Args:
+            instruction (Prompt): Prompt
+            value (str): Value
+            suffix (str, optional): Suffix. Defaults to "".
+
+        Raises:
+            MethodNotImplementedError: Call method has not been implemented
+        """
+        raise MethodNotImplementedError("Call method has not been implemented")
+
+    def generate_code(self, instruction: Prompt, prompt: str) -> str:
+        """
+        Generate the code based on the instruction and the given prompt.
+
+        Returns:
+            str: Code
+        """
+        return self._extract_code(self.call(instruction, prompt, suffix="\n\nCode:\n"))
+
+
+class BaseOpenAI(LLM, ABC):
+    """Base class to implement a new OpenAI LLM
+    LLM base class, this class is extended to be used with OpenAI API.
+
+    """
+
+    api_token: str
+    temperature: float = 0
+    max_tokens: int = 512
+    top_p: float = 1
+    frequency_penalty: float = 0
+    presence_penalty: float = 0.6
+    stop: Optional[str] = None
+    # support explicit proxy for OpenAI
+    openai_proxy: Optional[str] = None
+
+    def _set_params(self, **kwargs):
+        """
+        Set Parameters
+        Args:
+            **kwargs: ["model", "engine", "deployment_id", "temperature","max_tokens",
+            "top_p", "frequency_penalty", "presence_penalty", "stop", ]
+
+        Returns: None
+
+        """
+
+        valid_params = [
+            "model",
+            "engine",
+            "deployment_id",
+            "temperature",
+            "max_tokens",
+            "top_p",
+            "frequency_penalty",
+            "presence_penalty",
+            "stop",
+        ]
+        for key, value in kwargs.items():
+            if key in valid_params:
+                setattr(self, key, value)
+
+    @property
+    def _default_params(self) -> Dict[str, Any]:
+        """
+        Get the default parameters for calling OpenAI API
+
+        Returns (Dict): A dict of OpenAi API parameters
+
+        """
+
+        return {
+            "temperature": self.temperature,
+            "max_tokens": self.max_tokens,
+            "top_p": self.top_p,
+            "frequency_penalty": self.frequency_penalty,
+            "presence_penalty": self.presence_penalty,
+        }
+
+    def completion(self, prompt: str) -> str:
+        """
+        Query the completion API
+
+        Args:
+            prompt (str): Prompt
+
+        Returns:
+            str: LLM response
+        """
+        params = {**self._default_params, "prompt": prompt}
+
+        if self.stop is not None:
+            params["stop"] = [self.stop]
+
+        response = openai.Completion.create(**params)
+
+        return response["choices"][0]["text"]
+
+    def chat_completion(self, value: str) -> str:
+        """
+        Query the chat completion API
+
+        Args:
+            value (str): Prompt
+
+        Returns:
+            str: LLM response
+        """
+        params = {
+            **self._default_params,
+            "messages": [
+                {
+                    "role": "system",
+                    "content": value,
+                }
+            ],
+        }
+
+        if self.stop is not None:
+            params["stop"] = [self.stop]
+
+        response = openai.ChatCompletion.create(**params)
+
+        return response["choices"][0]["message"]["content"]
+
+
+class HuggingFaceLLM(LLM):
+    """Base class to implement a new Hugging Face LLM.
+
+    LLM base class is extended to be used with HuggingFace LLM Modes APIs
+
+    """
+
+    last_prompt: Optional[str] = None
+    api_token: str
+    _api_url: str = "https://api-inference.huggingface.co/models/"
+    _max_retries: int = 3
+
+    @property
+    def type(self) -> str:
+        return "huggingface-llm"
+
+    def query(self, payload):
+        """
+        Query the HF API
+        Args:
+            payload: A JSON form payload
+
+        Returns: Generated Response
+
+        """
+
+        headers = {"Authorization": f"Bearer {self.api_token}"}
+
+        response = requests.post(
+            self._api_url, headers=headers, json=payload, timeout=60
+        )
+
+        return response.json()[0]["generated_text"]
+
+    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+        """
+        A call method of HuggingFaceLLM class.
+        Args:
+            instruction (object): A prompt object
+            value (str):
+            suffix (str):
+
+        Returns (str): A string response
+
+        """
+
+        prompt = str(instruction)
+        payload = prompt + value + suffix
+
+        # sometimes the API doesn't return a valid response, so we retry passing the
+        # output generated from the previous call as the input
+        for _i in range(self._max_retries):
+            response = self.query({"inputs": payload})
+            payload = response
+            if response.count("<endCode>") >= 2:
+                break
+
+        # replace instruction + value from the inputs to avoid showing it in the output
+        output = response.replace(prompt + value + suffix, "")
+        return output
+
+
+class BaseGoogle(LLM):
+    """Base class to implement a new Google LLM
+
+    LLM base class is extended to be used with Google Palm API.
+    """
+
+    genai: Any
+    temperature: Optional[float] = 0
+    top_p: Optional[float] = 0.8
+    top_k: Optional[float] = 0.3
+    max_output_tokens: Optional[int] = 1000
+
+    def _configure(self, api_key: str):
+        """
+        Configure Google Palm API Key
+        Args:
+            api_key (str): A string of API keys generated from Google Cloud
+
+        Returns:
+
+        """
+
+        if not api_key:
+            raise APIKeyNotFoundError("Google Palm API key is required")
+
+        err_msg = "Install google-generativeai >= 0.1 for Google Palm API"
+        genai = import_dependency("google.generativeai", extra=err_msg)
+
+        genai.configure(api_key=api_key)
+        self.genai = genai
+
+    def _configurevertexai(self, project_id: str, location: str):
+        """
+        Configure Google VertexAi
+        Args:
+            project_id: GCP Project
+            location: Location of Project
+
+        Returns: Vertexai Object
+
+        """
+
+        err_msg = "Install google-cloud-aiplatform for Google Vertexai"
+        vertexai = import_dependency("vertexai", extra=err_msg)
+        vertexai.init(project=project_id, location=location)
+        self.vertexai = vertexai
+
+    def _valid_params(self):
+        return ["temperature", "top_p", "top_k", "max_output_tokens"]
+
+    def _set_params(self, **kwargs):
+        """
+        Set Parameters
+        Args:
+            **kwargs: ["temperature", "top_p", "top_k", "max_output_tokens"]
+
+        Returns:
+
+        """
+
+        valid_params = self._valid_params()
+        for key, value in kwargs.items():
+            if key in valid_params:
+                setattr(self, key, value)
+
+    def _validate(self):
+        """Validates the parameters for Google"""
+
+        if self.temperature is not None and not 0 <= self.temperature <= 1:
+            raise ValueError("temperature must be in the range [0.0, 1.0]")
+
+        if self.top_p is not None and not 0 <= self.top_p <= 1:
+            raise ValueError("top_p must be in the range [0.0, 1.0]")
+
+        if self.top_k is not None and not 0 <= self.top_k <= 1:
+            raise ValueError("top_k must be in the range [0.0, 1.0]")
+
+        if self.max_output_tokens is not None and self.max_output_tokens <= 0:
+            raise ValueError("max_output_tokens must be greater than zero")
+
+    @abstractmethod
+    def _generate_text(self, prompt: str) -> str:
+        """
+        Generates text for prompt, specific to implementation.
+
+        Args:
+            prompt (str): Prompt
+
+        Returns:
+            str: LLM response
+        """
+        raise MethodNotImplementedError("method has not been implemented")
+
+    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+        """
+        Call the Google LLM.
+
+        Args:
+            instruction (object): Instruction to pass
+            value (str): Value to pass
+            suffix (str): Suffix to pass
+
+        Returns:
+            str: Response
+        """
+        self.last_prompt = str(instruction) + value
+        prompt = str(instruction) + value + suffix
+        return self._generate_text(prompt)
```

### Comparing `hfttai-0.1.0/pandasai/llm/falcon.py` & `hfttai-0.1.2/pandasai/llm/falcon.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-""" Falcon LLM
-This module is to run the Falcon API hosted and maintained by HuggingFace.co.
-To generate HF_TOKEN go to https://huggingface.co/settings/tokens after creating Account
-on the platform.
-
-Example:
-    Use below example to call Falcon Model
-
-    >>> from pandasai.llm.falcon import Falcon
-"""
-
-
-import os
-from typing import Optional
-
-from dotenv import load_dotenv
-
-from ..exceptions import APIKeyNotFoundError
-from .base import HuggingFaceLLM
-
-load_dotenv()
-
-
-class Falcon(HuggingFaceLLM):
-
-    """Falcon LLM API
-
-    A base HuggingFaceLLM class is extended to use Falcon model.
-
-    """
-
-    api_token: str
-    _api_url: str = (
-        "https://api-inference.huggingface.co/models/tiiuae/falcon-7b-instruct"
-    )
-    _max_retries: int = 5
-
-    def __init__(self, api_token: Optional[str] = None):
-        """
-        __init__ method of Falcon Class
-        Args:
-            api_token (str): API token from Huggingface platform
-        """
-
-        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
-        if self.api_token is None:
-            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
-
-    @property
-    def type(self) -> str:
-        return "falcon"
+""" Falcon LLM
+This module is to run the Falcon API hosted and maintained by HuggingFace.co.
+To generate HF_TOKEN go to https://huggingface.co/settings/tokens after creating Account
+on the platform.
+
+Example:
+    Use below example to call Falcon Model
+
+    >>> from pandasai.llm.falcon import Falcon
+"""
+
+
+import os
+from typing import Optional
+
+from dotenv import load_dotenv
+
+from ..exceptions import APIKeyNotFoundError
+from .base import HuggingFaceLLM
+
+load_dotenv()
+
+
+class Falcon(HuggingFaceLLM):
+
+    """Falcon LLM API
+
+    A base HuggingFaceLLM class is extended to use Falcon model.
+
+    """
+
+    api_token: str
+    _api_url: str = (
+        "https://api-inference.huggingface.co/models/tiiuae/falcon-7b-instruct"
+    )
+    _max_retries: int = 5
+
+    def __init__(self, api_token: Optional[str] = None):
+        """
+        __init__ method of Falcon Class
+        Args:
+            api_token (str): API token from Huggingface platform
+        """
+
+        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
+        if self.api_token is None:
+            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
+
+    @property
+    def type(self) -> str:
+        return "falcon"
```

### Comparing `hfttai-0.1.0/pandasai/llm/google_palm.py` & `hfttai-0.1.2/pandasai/llm/google_palm.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-"""Google Palm LLM
-
-This module is to run the Google PaLM API hosted and maintained by Google.
-To read more on Google PaLM follow
-https://developers.generativeai.google/products/palm.
-
-Example:
-    Use below example to call GooglePalm Model
-
-    >>> from pandasai.llm.google_palm import GooglePalm
-
-Example:
-    Use below example to call Google VertexAi
-
-    >>> from pandasai.llm.google_palm import GoogleVertexai
-
-"""
-from typing import Optional
-
-from .base import BaseGoogle
-
-
-class GooglePalm(BaseGoogle):
-    """Google Palm LLM
-    BaseGoogle class is extended for Google Palm model. The default and only model
-    support at the moment is models/text-bison-001.
-
-    """
-
-    model: str = "models/text-bison-001"
-
-    def __init__(self, api_key: str, **kwargs):
-        """
-        __init__ method of GooglePalm Class
-        Args:
-            api_key (str): API Key
-            **kwargs: Extended Parameters inferred from BaseGoogle Class
-        """
-        self._configure(api_key=api_key)
-        self._set_params(**kwargs)
-
-    def _valid_params(self):
-        """Returns if the Parameters are valid or Not"""
-        return super()._valid_params() + ["model"]
-
-    def _validate(self):
-        """
-        A method to Validate the Model
-
-        """
-
-        super()._validate()
-
-        if not self.model:
-            raise ValueError("model is required.")
-
-    def _generate_text(self, prompt: str) -> str:
-        """
-        Generates text for prompt
-
-        Args:
-            prompt (str): Prompt
-
-        Returns:
-            str: LLM response
-        """
-        self._validate()
-        completion = self.genai.generate_text(
-            model=self.model,
-            prompt=prompt,
-            temperature=self.temperature,
-            top_p=self.top_p,
-            top_k=self.top_k,
-            max_output_tokens=self.max_output_tokens,
-        )
-        return completion.result
-
-    @property
-    def type(self) -> str:
-        return "google-palm"
-
-
-class GoogleVertexai(BaseGoogle):
-    """Google Palm Vertexai LLM
-    BaseGoogle class is extended for Google Palm model using Vertexai.
-    The default model support at the moment is text-bison-001.
-    However, user can choose to use code-bison-001 too.
-
-    """
-
-    def __init__(
-        self, project_id: str, location: str, model: Optional[str] = None, **kwargs
-    ):
-        """
-        A init class to implement the Google Vertexai Models
-
-        Args:
-            project_id (str): GCP project
-            location (str): GCP project Location
-            model Optional (str): Model to use Default to text-bison@001
-            **kwargs: Arguments to control the Model Parameters
-        """
-
-        if model is None:
-            self.model = "text-bison@001"
-        else:
-            self.model = model
-
-        self._configurevertexai(project_id, location)
-        self.project_id = project_id
-        self.location = location
-        self._set_params(**kwargs)
-
-    def _valid_params(self):
-        """Returns if the Parameters are valid or Not"""
-        return super()._valid_params() + ["model"]
-
-    def _validate(self):
-        """
-        A method to Validate the Model
-
-        """
-
-        super()._validate()
-
-        if not self.model:
-            raise ValueError("model is required.")
-
-    def _generate_text(self, prompt: str) -> str:
-        """
-        Generates text for prompt
-
-        Args:
-            prompt (str): Prompt
-
-        Returns:
-            str: LLM response
-        """
-        self._validate()
-
-        from vertexai.preview.language_models import (
-            CodeGenerationModel,
-            TextGenerationModel,
-        )
-
-        if self.model == "code-bison@001":
-            code_generation = CodeGenerationModel.from_pretrained(self.model)
-
-            completion = code_generation.predict(
-                prefix=prompt,
-                temperature=self.temperature,
-                max_output_tokens=self.max_output_tokens,
-            )
-        else:
-            text_generation = TextGenerationModel.from_pretrained(self.model)
-
-            completion = text_generation.predict(
-                prompt=prompt,
-                temperature=self.temperature,
-                top_p=self.top_p,
-                top_k=self.top_k,
-                max_output_tokens=self.max_output_tokens,
-            )
-
-        return str(completion)
-
-    @property
-    def type(self) -> str:
-        return "google-vertexai"
+"""Google Palm LLM
+
+This module is to run the Google PaLM API hosted and maintained by Google.
+To read more on Google PaLM follow
+https://developers.generativeai.google/products/palm.
+
+Example:
+    Use below example to call GooglePalm Model
+
+    >>> from pandasai.llm.google_palm import GooglePalm
+
+Example:
+    Use below example to call Google VertexAi
+
+    >>> from pandasai.llm.google_palm import GoogleVertexai
+
+"""
+from typing import Optional
+
+from .base import BaseGoogle
+
+
+class GooglePalm(BaseGoogle):
+    """Google Palm LLM
+    BaseGoogle class is extended for Google Palm model. The default and only model
+    support at the moment is models/text-bison-001.
+
+    """
+
+    model: str = "models/text-bison-001"
+
+    def __init__(self, api_key: str, **kwargs):
+        """
+        __init__ method of GooglePalm Class
+        Args:
+            api_key (str): API Key
+            **kwargs: Extended Parameters inferred from BaseGoogle Class
+        """
+        self._configure(api_key=api_key)
+        self._set_params(**kwargs)
+
+    def _valid_params(self):
+        """Returns if the Parameters are valid or Not"""
+        return super()._valid_params() + ["model"]
+
+    def _validate(self):
+        """
+        A method to Validate the Model
+
+        """
+
+        super()._validate()
+
+        if not self.model:
+            raise ValueError("model is required.")
+
+    def _generate_text(self, prompt: str) -> str:
+        """
+        Generates text for prompt
+
+        Args:
+            prompt (str): Prompt
+
+        Returns:
+            str: LLM response
+        """
+        self._validate()
+        completion = self.genai.generate_text(
+            model=self.model,
+            prompt=prompt,
+            temperature=self.temperature,
+            top_p=self.top_p,
+            top_k=self.top_k,
+            max_output_tokens=self.max_output_tokens,
+        )
+        return completion.result
+
+    @property
+    def type(self) -> str:
+        return "google-palm"
+
+
+class GoogleVertexai(BaseGoogle):
+    """Google Palm Vertexai LLM
+    BaseGoogle class is extended for Google Palm model using Vertexai.
+    The default model support at the moment is text-bison-001.
+    However, user can choose to use code-bison-001 too.
+
+    """
+
+    def __init__(
+        self, project_id: str, location: str, model: Optional[str] = None, **kwargs
+    ):
+        """
+        A init class to implement the Google Vertexai Models
+
+        Args:
+            project_id (str): GCP project
+            location (str): GCP project Location
+            model Optional (str): Model to use Default to text-bison@001
+            **kwargs: Arguments to control the Model Parameters
+        """
+
+        if model is None:
+            self.model = "text-bison@001"
+        else:
+            self.model = model
+
+        self._configurevertexai(project_id, location)
+        self.project_id = project_id
+        self.location = location
+        self._set_params(**kwargs)
+
+    def _valid_params(self):
+        """Returns if the Parameters are valid or Not"""
+        return super()._valid_params() + ["model"]
+
+    def _validate(self):
+        """
+        A method to Validate the Model
+
+        """
+
+        super()._validate()
+
+        if not self.model:
+            raise ValueError("model is required.")
+
+    def _generate_text(self, prompt: str) -> str:
+        """
+        Generates text for prompt
+
+        Args:
+            prompt (str): Prompt
+
+        Returns:
+            str: LLM response
+        """
+        self._validate()
+
+        from vertexai.preview.language_models import (
+            CodeGenerationModel,
+            TextGenerationModel,
+        )
+
+        if self.model == "code-bison@001":
+            code_generation = CodeGenerationModel.from_pretrained(self.model)
+
+            completion = code_generation.predict(
+                prefix=prompt,
+                temperature=self.temperature,
+                max_output_tokens=self.max_output_tokens,
+            )
+        else:
+            text_generation = TextGenerationModel.from_pretrained(self.model)
+
+            completion = text_generation.predict(
+                prompt=prompt,
+                temperature=self.temperature,
+                top_p=self.top_p,
+                top_k=self.top_k,
+                max_output_tokens=self.max_output_tokens,
+            )
+
+        return str(completion)
+
+    @property
+    def type(self) -> str:
+        return "google-vertexai"
```

### Comparing `hfttai-0.1.0/pandasai/llm/langchain.py` & `hfttai-0.1.2/pandasai/llm/fake.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from pandasai.prompts.base import Prompt
-from .base import LLM
-
-
-class LangchainLLM(LLM):
-    """
-    Class to wrap Langchain LLMs and make PandasAI interoperable
-    with LangChain.
-    """
-
-    _langchain_llm = None
-
-    def __init__(self, langchain_llm):
-        self._langchain_llm = langchain_llm
-
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-        prompt = str(instruction) + value + suffix
-        return self._langchain_llm(prompt)
-
-    @property
-    def type(self) -> str:
-        return "langchain_" + self._langchain_llm._llm_type
+"""Fake LLM"""
+
+from typing import Optional
+
+from ..prompts.base import Prompt
+from .base import LLM
+
+
+class FakeLLM(LLM):
+    """Fake LLM"""
+
+    _output: str = 'print("Hello world")'
+
+    def __init__(self, output: Optional[str] = None):
+        if output is not None:
+            self._output = output
+
+    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+        self.last_prompt = str(instruction) + str(value) + suffix
+        return self._output
+
+    @property
+    def type(self) -> str:
+        return "fake"
```

### Comparing `hfttai-0.1.0/pandasai/llm/open_assistant.py` & `hfttai-0.1.2/pandasai/llm/open_assistant.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-""" Open Assistant LLM
-
-This module is to run the HuggingFace OpenAssistant API hosted and maintained by
-HuggingFace.co. To generate HF_TOKEN go to https://huggingface.co/settings/tokens after
-creating Account on the platform.
-
-Example:
-    Use below example to call OpenAssistant Model
-
-    >>> from pandasai.llm.open_assistant import OpenAssistant
-"""
-
-import os
-from typing import Optional
-
-from dotenv import load_dotenv
-
-from ..exceptions import APIKeyNotFoundError
-from .base import HuggingFaceLLM
-
-load_dotenv()
-
-
-class OpenAssistant(HuggingFaceLLM):
-    """Open Assistant LLM
-    A base HuggingFaceLLM class is extended to use OpenAssistant Model via its API.
-    Currently `oasst-sft-1-pythia-12b` is supported via this module.
-    """
-
-    api_token: str
-    _api_url: str = (
-        "https://api-inference.huggingface.co/models/"
-        "OpenAssistant/oasst-sft-1-pythia-12b"
-    )
-    _max_retries: int = 10
-
-    def __init__(self, api_token: Optional[str] = None):
-        """
-        __init__ method of OpenAssistant Class
-
-        Raises:
-            APIKeyNotFoundError: HuggingFace Hub API key is required
-
-        Args:
-            api_token (str): API token from Huggingface platform
-        """
-        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
-        if self.api_token is None:
-            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
-
-    @property
-    def type(self) -> str:
-        return "open-assistant"
+""" Open Assistant LLM
+
+This module is to run the HuggingFace OpenAssistant API hosted and maintained by
+HuggingFace.co. To generate HF_TOKEN go to https://huggingface.co/settings/tokens after
+creating Account on the platform.
+
+Example:
+    Use below example to call OpenAssistant Model
+
+    >>> from pandasai.llm.open_assistant import OpenAssistant
+"""
+
+import os
+from typing import Optional
+
+from dotenv import load_dotenv
+
+from ..exceptions import APIKeyNotFoundError
+from .base import HuggingFaceLLM
+
+load_dotenv()
+
+
+class OpenAssistant(HuggingFaceLLM):
+    """Open Assistant LLM
+    A base HuggingFaceLLM class is extended to use OpenAssistant Model via its API.
+    Currently `oasst-sft-1-pythia-12b` is supported via this module.
+    """
+
+    api_token: str
+    _api_url: str = (
+        "https://api-inference.huggingface.co/models/"
+        "OpenAssistant/oasst-sft-1-pythia-12b"
+    )
+    _max_retries: int = 10
+
+    def __init__(self, api_token: Optional[str] = None):
+        """
+        __init__ method of OpenAssistant Class
+
+        Raises:
+            APIKeyNotFoundError: HuggingFace Hub API key is required
+
+        Args:
+            api_token (str): API token from Huggingface platform
+        """
+        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
+        if self.api_token is None:
+            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
+
+    @property
+    def type(self) -> str:
+        return "open-assistant"
```

### Comparing `hfttai-0.1.0/pandasai/llm/starcoder.py` & `hfttai-0.1.2/pandasai/llm/starcoder.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-""" Starcoder LLM
-This module is to run the StartCoder API hosted and maintained by HuggingFace.co.
-To generate HF_TOKEN go to https://huggingface.co/settings/tokens after creating Account
-on the platform.
-
-Example:
-    Use below example to call Starcoder Model
-
-    >>> from pandasai.llm.starcoder import Starcoder
-"""
-
-
-import os
-from typing import Optional
-
-from dotenv import load_dotenv
-
-from ..exceptions import APIKeyNotFoundError
-from .base import HuggingFaceLLM
-
-load_dotenv()
-
-
-class Starcoder(HuggingFaceLLM):
-
-    """Starcoder LLM API
-
-    A base HuggingFaceLLM class is extended to use Starcoder model.
-
-    """
-
-    api_token: str
-    _api_url: str = "https://api-inference.huggingface.co/models/bigcode/starcoder"
-    _max_retries: int = 5
-
-    def __init__(self, api_token: Optional[str] = None):
-        """
-        __init__ method of Starcoder Class
-        Args:
-            api_token (str): API token from Huggingface platform
-        """
-
-        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
-        if self.api_token is None:
-            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
-
-    @property
-    def type(self) -> str:
-        return "starcoder"
+""" Starcoder LLM
+This module is to run the StartCoder API hosted and maintained by HuggingFace.co.
+To generate HF_TOKEN go to https://huggingface.co/settings/tokens after creating Account
+on the platform.
+
+Example:
+    Use below example to call Starcoder Model
+
+    >>> from pandasai.llm.starcoder import Starcoder
+"""
+
+
+import os
+from typing import Optional
+
+from dotenv import load_dotenv
+
+from ..exceptions import APIKeyNotFoundError
+from .base import HuggingFaceLLM
+
+load_dotenv()
+
+
+class Starcoder(HuggingFaceLLM):
+
+    """Starcoder LLM API
+
+    A base HuggingFaceLLM class is extended to use Starcoder model.
+
+    """
+
+    api_token: str
+    _api_url: str = "https://api-inference.huggingface.co/models/bigcode/starcoder"
+    _max_retries: int = 5
+
+    def __init__(self, api_token: Optional[str] = None):
+        """
+        __init__ method of Starcoder Class
+        Args:
+            api_token (str): API token from Huggingface platform
+        """
+
+        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
+        if self.api_token is None:
+            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
+
+    @property
+    def type(self) -> str:
+        return "starcoder"
```

### Comparing `hfttai-0.1.0/pandasai/middlewares/charts.py` & `hfttai-0.1.2/pandasai/middlewares/charts.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""
-Charts Middleware class
-
-Middleware to handle the charts in PandasAI.
-"""
-
-from pandasai.middlewares.base import Middleware
-import sys
-
-
-class ChartsMiddleware(Middleware):
-    """Charts Middleware class"""
-
-    def _is_running_in_console(self) -> bool:
-        """
-        Check if the code is running in console or not.
-
-        Returns:
-            bool: True if running in console else False
-        """
-
-        return sys.stdout.isatty()
-
-    def run(self, code: str) -> str:
-        """
-        Run the middleware to remove issues with displaying charts in PandasAI.
-
-        Returns:
-            str: Modified code
-        """
-
-        if "plt.show()" in code:
-            if "plt.close('all')" not in code:
-                code = code.replace("plt.show()", "plt.show()\nplt.close('all')")
-
-            if not self._is_running_in_console():
-                code = code.replace("plt.show()", "plt.show(block=False)")
-        return code
+"""
+Charts Middleware class
+
+Middleware to handle the charts in PandasAI.
+"""
+
+from pandasai.middlewares.base import Middleware
+import sys
+
+
+class ChartsMiddleware(Middleware):
+    """Charts Middleware class"""
+
+    def _is_running_in_console(self) -> bool:
+        """
+        Check if the code is running in console or not.
+
+        Returns:
+            bool: True if running in console else False
+        """
+
+        return sys.stdout.isatty()
+
+    def run(self, code: str) -> str:
+        """
+        Run the middleware to remove issues with displaying charts in PandasAI.
+
+        Returns:
+            str: Modified code
+        """
+
+        if "plt.show()" in code:
+            if "plt.close('all')" not in code:
+                code = code.replace("plt.show()", "plt.show()\nplt.close('all')")
+
+            if not self._is_running_in_console():
+                code = code.replace("plt.show()", "plt.show(block=False)")
+        return code
```

### Comparing `hfttai-0.1.0/pandasai/middlewares/streamlit.py` & `hfttai-0.1.2/pandasai/middlewares/streamlit.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-Streamlit Middleware class
-
-Middleware to run the code in streamlit and address the issues with streamlit
-integration with PandasAI.
-"""
-
-from pandasai.middlewares.base import Middleware
-
-
-class StreamlitMiddleware(Middleware):
-    """Streamlit Middleware class"""
-
-    def run(self, code: str) -> str:
-        """
-        Run the middleware to make the code compatible with streamlit.
-        For example, it replaces `plt.show()` with `st.pyplot()`.
-
-        Returns:
-            str: Modified code
-        """
-
-        code = code.replace("plt.show()", "st.pyplot(plt.gcf())")
-        code = "import streamlit as st\n" + code
-        return code
+"""
+Streamlit Middleware class
+
+Middleware to run the code in streamlit and address the issues with streamlit
+integration with PandasAI.
+"""
+
+from pandasai.middlewares.base import Middleware
+
+
+class StreamlitMiddleware(Middleware):
+    """Streamlit Middleware class"""
+
+    def run(self, code: str) -> str:
+        """
+        Run the middleware to make the code compatible with streamlit.
+        For example, it replaces `plt.show()` with `st.pyplot()`.
+
+        Returns:
+            str: Modified code
+        """
+
+        code = code.replace("plt.show()", "st.pyplot(plt.gcf())")
+        code = "import streamlit as st\n" + code
+        return code
```

### Comparing `hfttai-0.1.0/pandasai/prompts/correct_error_prompt.py` & `hfttai-0.1.2/pandasai/prompts/generate_python_code.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,32 @@
-""" Prompt to correct Python Code on Error
-```
-Today is {today_date}.
-You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the metadata of the dataframe:
-{df_head}.
-
-The user asked the following question:
-{question}
-
-You generated this python code:
-{code}
-
-It fails with the following error:
-{error_returned}
-
-Correct the python code and return a new python code (do not import anything) that fixes the above
-mentioned error. Do not generate the same code again.
-```
-"""  # noqa: E501
-from datetime import date
-
-from .base import Prompt
-
-
-class CorrectErrorPrompt(Prompt):
-    """Prompt to Correct Python code on Error"""
-
-    text: str = """
-Today is {today_date}.
-You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the metadata of the dataframe:
-{df_head}.
-
-The user asked the following question:
-{question}
-
-You generated this python code:
-{code}
-
-It fails with the following error:
-{error_returned}
-
-Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
-"""  # noqa: E501
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs, today_date=date.today())
+""" Prompt to generate Python code
+```
+Today is {today_date}.
+You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
+This is the metadata of the dataframe:
+{df_head}.
+
+When asked about the data, your response should include a python code that describes the
+dataframe `df`. Using the provided dataframe, df, return the python code to get the answer to the following question:
+```
+"""  # noqa: E501
+
+from datetime import date
+
+from .base import Prompt
+
+
+class GeneratePythonCodePrompt(Prompt):
+    """Prompt to generate Python code"""
+
+    text: str = """
+Today is {today_date}.
+You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
+This is the metadata of the dataframe:
+{df_head}.
+
+When asked about the data, your response should include a python code that describes the dataframe `df`.
+Using the provided dataframe, df, return the python code to get the answer to the following question:
+"""  # noqa: E501
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs, today_date=date.today())
```

### Comparing `hfttai-0.1.0/pandasai/prompts/correct_multiples_prompt.py` & `hfttai-0.1.2/pandasai/prompts/correct_multiples_prompt.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-""" Prompt to correct error """
-
-import pandas as pd
-
-from .base import Prompt
-
-
-class CorrectMultipleDataframesErrorPrompt(Prompt):
-    """Prompt to generate Python code"""
-
-    text: str = """
-You are provided with the following pandas dataframes:"""
-
-    def __init__(
-        self,
-        code: str,
-        error_returned: Exception,
-        question: str,
-        df_head: list[pd.DataFrame],
-    ):
-        for i, dataframe in enumerate(df_head, start=1):
-            row, col = dataframe.shape
-            self.text += f"""
-Dataframe df{i}, with {row} rows and {col} columns.
-This is the metadata of the dataframe df{i}:
-{dataframe}"""
-
-        instruction: str = f"""
-The user asked the following question:
-{question}
-
-You generated this python code:
-{code}
-
-It fails with the following error:
-{error_returned}
-
-Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
-"""  # noqa: E501
-
-        self.text += instruction
-
-    def __str__(self):
-        return self.text
+""" Prompt to correct error """
+
+import pandas as pd
+
+from .base import Prompt
+
+
+class CorrectMultipleDataframesErrorPrompt(Prompt):
+    """Prompt to generate Python code"""
+
+    text: str = """
+You are provided with the following pandas dataframes:"""
+
+    def __init__(
+        self,
+        code: str,
+        error_returned: Exception,
+        question: str,
+        df_head: list[pd.DataFrame],
+    ):
+        for i, dataframe in enumerate(df_head, start=1):
+            row, col = dataframe.shape
+            self.text += f"""
+Dataframe df{i}, with {row} rows and {col} columns.
+This is the metadata of the dataframe df{i}:
+{dataframe}"""
+
+        instruction: str = f"""
+The user asked the following question:
+{question}
+
+You generated this python code:
+{code}
+
+It fails with the following error:
+{error_returned}
+
+Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
+"""  # noqa: E501
+
+        self.text += instruction
+
+    def __str__(self):
+        return self.text
```

### Comparing `hfttai-0.1.0/pandasai/prompts/generate_python_code.py` & `hfttai-0.1.2/pandasai/prompts/correct_error_prompt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,48 @@
-""" Prompt to generate Python code
-```
-Today is {today_date}.
-You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the metadata of the dataframe:
-{df_head}.
-
-When asked about the data, your response should include a python code that describes the
-dataframe `df`. Using the provided dataframe, df, return the python code to get the answer to the following question:
-```
-"""  # noqa: E501
-
-from datetime import date
-
-from .base import Prompt
-
-
-class GeneratePythonCodePrompt(Prompt):
-    """Prompt to generate Python code"""
-
-    text: str = """
-Today is {today_date}.
-You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the metadata of the dataframe:
-{df_head}.
-
-When asked about the data, your response should include a python code that describes the dataframe `df`.
-Using the provided dataframe, df, return the python code to get the answer to the following question:
-"""  # noqa: E501
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs, today_date=date.today())
+""" Prompt to correct Python Code on Error
+```
+Today is {today_date}.
+You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
+This is the metadata of the dataframe:
+{df_head}.
+
+The user asked the following question:
+{question}
+
+You generated this python code:
+{code}
+
+It fails with the following error:
+{error_returned}
+
+Correct the python code and return a new python code (do not import anything) that fixes the above
+mentioned error. Do not generate the same code again.
+```
+"""  # noqa: E501
+from datetime import date
+
+from .base import Prompt
+
+
+class CorrectErrorPrompt(Prompt):
+    """Prompt to Correct Python code on Error"""
+
+    text: str = """
+Today is {today_date}.
+You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
+This is the metadata of the dataframe:
+{df_head}.
+
+The user asked the following question:
+{question}
+
+You generated this python code:
+{code}
+
+It fails with the following error:
+{error_returned}
+
+Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
+"""  # noqa: E501
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs, today_date=date.today())
```

### Comparing `hfttai-0.1.0/pandasai/prompts/multiple_dataframes.py` & `hfttai-0.1.2/pandasai/prompts/multiple_dataframes.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-""" Prompt to generate Python code for multiple dataframes """
-
-from datetime import date
-
-import pandas as pd
-
-from .base import Prompt
-
-
-class MultipleDataframesPrompt(Prompt):
-    """Prompt to generate Python code"""
-
-    text: str = """
-Today is {today_date}.
-You are provided with the following pandas dataframes:"""
-    instruction: str = """
-When asked about the data, your response should include a python code that describes the dataframes provided.
-Using the provided dataframes and no other dataframes, return the python code to get the answer to the following question:
-"""  # noqa: E501
-
-    def __init__(self, dataframes: list[pd.DataFrame]):
-        for i, dataframe in enumerate(dataframes, start=1):
-            row, col = dataframe.shape
-
-            self.text += f"""
-Dataframe df{i}, with {row} rows and {col} columns.
-This is the metadata of the dataframe df{i}:
-{dataframe}"""
-
-        self.text += self.instruction
-        self.text = self.text.format(
-            today_date=date.today(),
-        )
-
-    def __str__(self):
-        return self.text
+""" Prompt to generate Python code for multiple dataframes """
+
+from datetime import date
+
+import pandas as pd
+
+from .base import Prompt
+
+
+class MultipleDataframesPrompt(Prompt):
+    """Prompt to generate Python code"""
+
+    text: str = """
+Today is {today_date}.
+You are provided with the following pandas dataframes:"""
+    instruction: str = """
+When asked about the data, your response should include a python code that describes the dataframes provided.
+Using the provided dataframes and no other dataframes, return the python code to get the answer to the following question:
+"""  # noqa: E501
+
+    def __init__(self, dataframes: list[pd.DataFrame]):
+        for i, dataframe in enumerate(dataframes, start=1):
+            row, col = dataframe.shape
+
+            self.text += f"""
+Dataframe df{i}, with {row} rows and {col} columns.
+This is the metadata of the dataframe df{i}:
+{dataframe}"""
+
+        self.text += self.instruction
+        self.text = self.text.format(
+            today_date=date.today(),
+        )
+
+    def __str__(self):
+        return self.text
```

### Comparing `hfttai-0.1.0/pyproject.toml` & `hfttai-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-[tool.poetry]
-name = "hfttai"
-version = "0.1.0"
-description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
-authors = ["Gabriele Venturi"]
-license = "MIT"
-readme = "README.md"
-packages = [{include = "pandasai"}]
-
-[tool.poetry.dependencies]
-python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
-python-dotenv = "^1.0.0"
-pandas = "1.5.3"
-astor = "^0.8.1"
-openai = "^0.27.5"
-ipython = "^8.13.1"
-matplotlib = "^3.7.1"
-google-generativeai = { version = "^0.1.0rc2", optional = true }
-google-cloud-aiplatform = { version = "^1.26.1", optional = true }
-langchain = { version = "^0.0.199", optional = true}
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-pre-commit = "^3.2.2"
-ruff = "^0.0.220"
-pytest = "^7.3.1"
-pytest-mock = "^3.10.0"
-pytest-env = "^0.8.1"
-click = "^8.1.3"
-
-
-[tool.poetry.group.extras.dependencies]
-google-cloud-aiplatform = "^1.26.1"
-
-[tool.poetry.extras]
-google = ["google-generativeai"]
-tests = ["numpy", "seaborn"]
-langchain = ["langchain"]
-google-cloud = ["google-cloud-aiplatform"]
-
-[tool.poetry.group.whitelist.dependencies]
-statsmodels = {version = "^0.14.0", optional = true}
-scikit-learn = {version = "^1.2.2", optional = true}
-seaborn = {version = "^0.12.2", optional = true}
-plotly = {version = "^5.14.1", optional = true}
-ggplot = {version = "^0.11.5", optional = true}
-numpy = {version = "^1.17", optional = true}
-scipy = {version = "^1.9.0", optional = true}
-streamlit = { version = "^1.23.1", optional = true }
-
-[tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.0"
-mkdocstrings-python = "0.7.1"
-markdown-include = "^0.6.0"
-
-[tool.poetry.scripts]
-pai = "pai.__main__:main"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.ruff]
-exclude = ["tests_*"]
-
-[tool.pytest.ini_options]
-env = [
-    "HUGGINGFACE_API_KEY=",
-    "OPENAI_API_KEY="
-]
+[tool.poetry]
+name = "hfttai"
+version = "0.1.2"
+description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
+authors = ["Gabriele Venturi"]
+license = "MIT"
+readme = "README.md"
+packages = [{include = "pandasai"}]
+
+[tool.poetry.dependencies]
+python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
+python-dotenv = "^1.0.0"
+pandas = "1.5.3"
+astor = "^0.8.1"
+openai = "^0.27.5"
+ipython = "^8.13.1"
+matplotlib = "^3.7.1"
+google-generativeai = { version = "^0.1.0rc2", optional = true }
+google-cloud-aiplatform = { version = "^1.26.1", optional = true }
+langchain = { version = "^0.0.199", optional = true}
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pre-commit = "^3.2.2"
+ruff = "^0.0.220"
+pytest = "^7.3.1"
+pytest-mock = "^3.10.0"
+pytest-env = "^0.8.1"
+click = "^8.1.3"
+
+
+[tool.poetry.group.extras.dependencies]
+google-cloud-aiplatform = "^1.26.1"
+
+[tool.poetry.extras]
+google = ["google-generativeai"]
+tests = ["numpy", "seaborn"]
+langchain = ["langchain"]
+google-cloud = ["google-cloud-aiplatform"]
+
+[tool.poetry.group.whitelist.dependencies]
+statsmodels = {version = "^0.14.0", optional = true}
+scikit-learn = {version = "^1.2.2", optional = true}
+seaborn = {version = "^0.12.2", optional = true}
+plotly = {version = "^5.14.1", optional = true}
+ggplot = {version = "^0.11.5", optional = true}
+numpy = {version = "^1.17", optional = true}
+scipy = {version = "^1.9.0", optional = true}
+streamlit = { version = "^1.23.1", optional = true }
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "1.4.0"
+mkdocstrings-python = "0.7.1"
+markdown-include = "^0.6.0"
+
+[tool.poetry.scripts]
+pai = "pai.__main__:main"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+exclude = ["tests_*"]
+
+[tool.pytest.ini_options]
+env = [
+    "HUGGINGFACE_API_KEY=",
+    "OPENAI_API_KEY="
+]
```

### Comparing `hfttai-0.1.0/README.md` & `hfttai-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-# PandasAI 🐼
-
-[![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
-[![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
-[![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
-[![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
-[![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
-[![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
-
-PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
-
-<!-- Add images/pandas-ai.png -->
-
-![PandasAI](images/pandas-ai.png?raw=true)
-
-## 🔧 Quick install
-
-```bash
-pip install pandasai
-```
-
-## 🔍 Demo
-
-Try out PandasAI in your browser:
-
-[![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
-
-## 📖 Documentation
-
-The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
-
-## 💻 Usage
-
-> Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
-
-PandasAI is designed to be used in conjunction with pandas. It makes pandas conversational, allowing you to ask questions to your data in natural language.
-
-### Queries
-
-For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
-
-```python
-import pandas as pd
-from pandasai import PandasAI
-
-# Sample DataFrame
-df = pd.DataFrame({
-    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
-    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
-    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
-})
-
-# Instantiate a LLM
-from pandasai.llm.openai import OpenAI
-llm = OpenAI(api_token="YOUR_API_TOKEN")
-
-pandas_ai = PandasAI(llm)
-pandas_ai(df, prompt='Which are the 5 happiest countries?')
-```
-
-The above code will return the following:
-
-```
-6            Canada
-7         Australia
-1    United Kingdom
-3           Germany
-0     United States
-Name: country, dtype: object
-```
-
-Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
-
-```python
-pandas_ai(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
-```
-
-The above code will return the following:
-
-```
-19012600725504
-```
-
-### Charts
-
-You can also ask PandasAI to draw a graph:
-
-```python
-pandas_ai(
-    df,
-    "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
-)
-```
-
-![Chart](images/histogram-chart.png?raw=true)
-
-You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
-
-### Multiple DataFrames
-
-Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
-
-```python
-import pandas as pd
-from pandasai import PandasAI
-
-employees_data = {
-    'EmployeeID': [1, 2, 3, 4, 5],
-    'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
-    'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
-}
-
-salaries_data = {
-    'EmployeeID': [1, 2, 3, 4, 5],
-    'Salary': [5000, 6000, 4500, 7000, 5500]
-}
-
-employees_df = pd.DataFrame(employees_data)
-salaries_df = pd.DataFrame(salaries_data)
-
-
-llm = OpenAI()
-pandas_ai = PandasAI(llm)
-pandas_ai([employees_df, salaries_df], "Who gets paid the most?")
-```
-
-The above code will return the following:
-
-```
-Oh, Olivia gets paid the most.
-```
-
-You can find more examples in the [examples](examples) directory.
-
-### ⚡️ Shortcuts
-
-PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
-
-```python
-# Clean data
-pandas_ai.clean_data(df)
-
-# Impute missing values
-pandas_ai.impute_missing_values(df)
-
-# Generate features
-pandas_ai.generate_features(df)
-
-# Plot histogram
-pandas_ai.plot_histogram(df, column="gdp")
-```
-
-Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
-
-## 🔒 Privacy & Security
-
-In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
-
-Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
-
-## ⚙️ Command-Line Tool
-
-Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
-
-Read more about how to use the CLI [here](https://pandas-ai.readthedocs.io/en/latest/pai_cli/).
-
-## 🤝 Contributing
-
-Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
-For more information, please see the [contributing guidelines](CONTRIBUTING.md).
-
-After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
-
-```bash
-pre-commit install
-```
-
-## 📜 License
-
-PandasAI is licensed under the MIT License. See the LICENSE file for more details.
-
-## Acknowledgements
-
-- This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
-- This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
+# PandasAI 🐼
+
+[![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
+[![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
+[![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
+[![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
+[![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
+
+PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
+
+<!-- Add images/pandas-ai.png -->
+
+![PandasAI](images/pandas-ai.png?raw=true)
+
+## 🔧 Quick install
+
+```bash
+pip install pandasai
+```
+
+## 🔍 Demo
+
+Try out PandasAI in your browser:
+
+[![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
+
+## 📖 Documentation
+
+The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
+
+## 💻 Usage
+
+> Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
+
+PandasAI is designed to be used in conjunction with pandas. It makes pandas conversational, allowing you to ask questions to your data in natural language.
+
+### Queries
+
+For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
+
+```python
+import pandas as pd
+from pandasai import PandasAI
+
+# Sample DataFrame
+df = pd.DataFrame({
+    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
+    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+})
+
+# Instantiate a LLM
+from pandasai.llm.openai import OpenAI
+llm = OpenAI(api_token="YOUR_API_TOKEN")
+
+pandas_ai = PandasAI(llm)
+pandas_ai(df, prompt='Which are the 5 happiest countries?')
+```
+
+The above code will return the following:
+
+```
+6            Canada
+7         Australia
+1    United Kingdom
+3           Germany
+0     United States
+Name: country, dtype: object
+```
+
+Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
+
+```python
+pandas_ai(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
+```
+
+The above code will return the following:
+
+```
+19012600725504
+```
+
+### Charts
+
+You can also ask PandasAI to draw a graph:
+
+```python
+pandas_ai(
+    df,
+    "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
+)
+```
+
+![Chart](images/histogram-chart.png?raw=true)
+
+You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
+
+### Multiple DataFrames
+
+Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
+
+```python
+import pandas as pd
+from pandasai import PandasAI
+
+employees_data = {
+    'EmployeeID': [1, 2, 3, 4, 5],
+    'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
+    'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
+}
+
+salaries_data = {
+    'EmployeeID': [1, 2, 3, 4, 5],
+    'Salary': [5000, 6000, 4500, 7000, 5500]
+}
+
+employees_df = pd.DataFrame(employees_data)
+salaries_df = pd.DataFrame(salaries_data)
+
+
+llm = OpenAI()
+pandas_ai = PandasAI(llm)
+pandas_ai([employees_df, salaries_df], "Who gets paid the most?")
+```
+
+The above code will return the following:
+
+```
+Oh, Olivia gets paid the most.
+```
+
+You can find more examples in the [examples](examples) directory.
+
+### ⚡️ Shortcuts
+
+PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
+
+```python
+# Clean data
+pandas_ai.clean_data(df)
+
+# Impute missing values
+pandas_ai.impute_missing_values(df)
+
+# Generate features
+pandas_ai.generate_features(df)
+
+# Plot histogram
+pandas_ai.plot_histogram(df, column="gdp")
+```
+
+Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
+
+## 🔒 Privacy & Security
+
+In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
+
+Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
+
+## ⚙️ Command-Line Tool
+
+Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
+
+Read more about how to use the CLI [here](https://pandas-ai.readthedocs.io/en/latest/pai_cli/).
+
+## 🤝 Contributing
+
+Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
+For more information, please see the [contributing guidelines](CONTRIBUTING.md).
+
+After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
+
+```bash
+pre-commit install
+```
+
+## 📜 License
+
+PandasAI is licensed under the MIT License. See the LICENSE file for more details.
+
+## Acknowledgements
+
+- This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
+- This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
```

### Comparing `hfttai-0.1.0/PKG-INFO` & `hfttai-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfttai
-Version: 0.1.0
+Version: 0.1.2
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

