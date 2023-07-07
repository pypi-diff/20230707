# Comparing `tmp/idoctorai-0.6.9.tar.gz` & `tmp/idoctorai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.6.9.tar", max compression
+gzip compressed data, was "idoctorai-0.7.0.tar", max compression
```

## Comparing `idoctorai-0.6.9.tar` & `idoctorai-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.6.9/LICENSE
--rw-r--r--   0        0        0    20920 2023-07-05 15:03:07.850396 idoctorai-0.6.9/pandasai/__init__.py
--rw-r--r--   0        0        0     1858 2023-07-03 05:12:09.354788 idoctorai-0.6.9/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.6.9/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.6.9/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.6.9/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.6.9/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.6.9/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.6.9/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.6.9/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.6.9/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     3599 2023-07-05 14:48:11.904812 idoctorai-0.6.9/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.6.9/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.6.9/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11306 2023-07-05 13:28:00.529087 idoctorai-0.6.9/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.6.9/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.6.9/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     4154 2023-07-03 02:41:28.389857 idoctorai-0.6.9/pandasai/llm/model.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.6.9/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3275 2023-07-02 06:33:47.366335 idoctorai-0.6.9/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.6.9/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.6.9/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.6.9/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.6.9/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1386 2023-07-05 15:05:10.817161 idoctorai-0.6.9/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.6.9/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.6.9/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1710 2023-07-05 14:14:57.617365 idoctorai-0.6.9/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1593 2023-07-05 15:07:05.714213 idoctorai-0.6.9/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.6.9/README.md
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 idoctorai-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.7.0/LICENSE
+-rw-r--r--   0        0        0    28544 2023-07-07 03:58:45.008438 idoctorai-0.7.0/pandasai/__init__.py
+-rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 idoctorai-0.7.0/pandasai/constants.py
+-rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 idoctorai-0.7.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.7.0/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 idoctorai-0.7.0/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 idoctorai-0.7.0/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 idoctorai-0.7.0/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.7.0/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 idoctorai-0.7.0/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3587 2023-07-07 01:01:47.985267 idoctorai-0.7.0/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 idoctorai-0.7.0/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0     3761 2023-07-07 04:30:13.258251 idoctorai-0.7.0/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.7.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 idoctorai-0.7.0/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11783 2023-07-07 01:01:48.055081 idoctorai-0.7.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.7.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 idoctorai-0.7.0/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 idoctorai-0.7.0/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 idoctorai-0.7.0/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     4154 2023-07-07 00:58:33.292900 idoctorai-0.7.0/pandasai/llm/model.py
+-rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 idoctorai-0.7.0/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3599 2023-07-07 01:57:17.309051 idoctorai-0.7.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.7.0/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 idoctorai-0.7.0/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 idoctorai-0.7.0/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 idoctorai-0.7.0/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 idoctorai-0.7.0/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.7.0/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 idoctorai-0.7.0/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1349 2023-07-07 01:01:48.046105 idoctorai-0.7.0/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1125 2023-07-07 01:01:48.041118 idoctorai-0.7.0/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1295 2023-07-07 04:03:12.348983 idoctorai-0.7.0/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 idoctorai-0.7.0/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1339 2023-07-07 04:06:37.487951 idoctorai-0.7.0/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1922 2023-07-07 04:39:52.971790 idoctorai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-07-07 02:10:07.752756 idoctorai-0.7.0/README.md
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 idoctorai-0.7.0/PKG-INFO
```

### Comparing `idoctorai-0.6.9/LICENSE` & `idoctorai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.9/pandasai/__init__.py` & `idoctorai-0.7.0/pandasai/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,174 +1,284 @@
 # -*- coding: utf-8 -*-
 """
 PandasAI is a wrapper around a LLM to make dataframes conversational
 
-This module includes the implementation of basis  PandasAI class with methods to run the LLMs
-models on Pandas dataframes. Following LLMs are implemented so far.
+This module includes the implementation of basis  PandasAI class with methods to run
+the LLMs models on Pandas dataframes. Following LLMs are implemented so far.
 
 Example:
 
-    This module is the Entry point of the `pandasai` package. Following is an example of how to
-    use this Class.
+    This module is the Entry point of the `pandasai` package. Following is an example
+    of how to use this Class.
 
     ```python
     import pandas as pd
     from pandasai import PandasAI
 
     # Sample DataFrame
     df = pd.DataFrame({
-        "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain",
-        "Canada", "Australia", "Japan", "China"],
-        "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416,
-        1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+        "country": ["United States", "United Kingdom", "France", "Germany", "Italy",
+        "Spain", "Canada", "Australia", "Japan", "China"],
+        "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832,
+        1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440,
+        14631844184064],
         "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
     })
 
     # Instantiate a LLM
     from pandasai.llm.openai import OpenAI
     llm = OpenAI(api_token="YOUR_API_TOKEN")
 
     pandas_ai = PandasAI(llm)
     pandas_ai(df, prompt='Which are the 5 happiest countries?')
 
     ```
 """
+
 import ast
 import io
+import logging
 import re
 import sys
 import uuid
+import time
 from contextlib import redirect_stdout
-from typing import Optional, Union
+from typing import List, Optional, Union, Dict, Type
+import importlib.metadata
 
+__version__ = importlib.metadata.version(__package__ or __name__)
 import astor
-import matplotlib.pyplot as plt
 import pandas as pd
-
 from .constants import (
-    ENVIRONMENT_DEFAULTS,
     WHITELISTED_BUILTINS,
     WHITELISTED_LIBRARIES,
-    WHITELISTED_OPTIONAL_LIBRARIES,
 )
 from .exceptions import BadImportError, LLMNotFoundError
-from .helpers._optional import import_optional_dependency
+from .helpers._optional import import_dependency
 from .helpers.anonymizer import anonymize_dataframe_head
 from .helpers.cache import Cache
 from .helpers.notebook import Notebook
 from .helpers.save_chart import add_save_chart
+from .helpers.shortcuts import Shortcuts
 from .llm.base import LLM
+from .llm.langchain import LangchainLLM
+from .middlewares.base import Middleware
+from .middlewares.charts import ChartsMiddleware
+from .prompts.base import Prompt
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
 
 import toml
 import os
 
 
-# pylint: disable=too-many-instance-attributes disable=too-many-arguments
-class PandasAI:
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
     """
     PandasAI is a wrapper around a LLM to make dataframes conversational.
 
 
-    This is an entry point of `pandasai` object. This class consists of methods to interface the
-    LLMs with Pandas     dataframes. A pandas dataframe metadata i.e. df.head() and prompt is
-    passed on to chosen LLMs API end point to     generate a Python code to answer the questions
-    asked. The resultant python code is run on actual data and answer is converted into a
-    conversational form.
+    This is an entry point of `pandasai` object. This class consists of methods
+    to interface the LLMs with Pandas     dataframes. A pandas dataframe metadata i.e.
+    df.head() and prompt is passed on to chosen LLMs API end point to generate a Python
+    code to answer the questions asked. The resultant python code is run on actual data
+    and answer is converted into a conversational form.
 
     Note:
         Do not include the `self` parameter in the ``Args`` section.
     Args:
         _llm (obj): LLMs option to be used for API access
         _verbose (bool, optional): To show the intermediate outputs e.g. python code
         generated and execution step on the prompt. Default to False
-        _is_conversational_answer (bool, optional): Whether to return answer in conversational
-        form. Default to False
+        _is_conversational_answer (bool, optional): Whether to return answer in
+        conversational form. Default to False
         _enforce_privacy (bool, optional): Do not display the data on prompt in case of
         Sensitive data. Default to False
-        _max_retries (int, optional): max no. of tries to generate code on failure. Default to 3
-        _is_notebook (bool, optional): Whether to run code in notebook. Default to False
-        _original_instructions (dict, optional): The dict of instruction to run. Default to None
-        last_code_generated (str, optional): Pass last Code if generated. Default to None
-        last_run_code (str, optional): Pass the last execution / run. Default to None
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
         code_output (str, optional): The code output if any. Default to None
         last_error (str, optional): Error of running code last time. Default to None
         prompt_id (str, optional): Unique ID to differentiate calls. Default to None
 
 
     Returns (str): Response to a Question related to Data
 
     """
 
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = False
     _enforce_privacy: bool = False
     _max_retries: int = 3
-    _is_notebook: bool = False
+    _in_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "df_columns": None,
         "num_rows": None,
         "num_columns": None,
-        "rows_to_display": None,
     }
-    _cache: Cache = Cache()
+    _cache: Cache = None
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
+    _middlewares: List[Middleware] = [ChartsMiddleware()]
+    _additional_dependencies: List[dict] = []
+    _custom_whitelisted_dependencies: List[str] = []
+    _start_time: float = 0
+    _enable_logging: bool = True
+    _logger: logging.Logger = None
+    _logs: List[str] = []
     last_code_generated: Optional[str] = None
-    last_run_code: Optional[str] = None
+    last_code_executed: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
     _history: list = None
 
     def __init__(
         self,
         llm=None,
         conversational=False,
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
+        save_charts_path=None,
         enable_cache=True,
         max_retries=3,
+        middlewares=None,
+        custom_whitelisted_dependencies=None,
+        enable_logging=True,
+        non_default_prompts: Optional[Dict[str, Type[Prompt]]] = None,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
-            conversational (bool): Whether to return answer in conversational form. Default to False
-            verbose (bool): To show the intermediate outputs e.g. python code generated and
-             execution step on the prompt.  Default to False
-            enforce_privacy (bool): Execute the codes with Privacy Mode ON.  Default to False
-            save_charts (bool): Save the charts generated in the notebook. Default to False
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
         """
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
         if llm is None:
             raise LLMNotFoundError(
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
-        self._llm = llm
+        self._load_llm(llm)
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
-        self._enable_cache = enable_cache
+        self._save_charts_path = save_charts_path
         self._process_id = str(uuid.uuid4())
+        self._logs = []
+
+        self._non_default_prompts = (
+            {} if non_default_prompts is None else non_default_prompts
+        )
 
         self._max_retries = max_retries
 
         self.notebook = Notebook()
         self._in_notebook = self.notebook.in_notebook()
 
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
     def conversational_answer(self, question: str, answer: str) -> str:
         """
         Returns the answer in conversational form about the resultant data.
 
         Args:
             question (str): A question in Conversational form
             answer (str): A summary / resultant Data
@@ -178,171 +288,189 @@
         """
 
         if self._enforce_privacy:
             # we don't want to send potentially sensitive data to the LLM server
             # if the user has set enforce_privacy to True
             return answer
 
-        instruction = GenerateResponsePrompt(question=question, answer=answer)
-        return self._llm.call(instruction, "")
+        generate_response_instruction = self._non_default_prompts.get(
+            "generate_response", GenerateResponsePrompt
+        )(question=question, answer=answer)
+        return self._llm.call(generate_response_instruction, "")
 
     def run(
         self,
-        data_frame: pd.DataFrame,
+        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
         history: list = None,
     ) -> Union[str, pd.DataFrame]:
         """
         Run the PandasAI to make Dataframes Conversational.
 
         Args:
-            data_frame (pd.Dataframe): A pandas Dataframe
+            data_frame (Union[pd.DataFrame, List[pd.DataFrame]]): A pandas Dataframe
             prompt (str): A prompt to query about the Dataframe
-            is_conversational_answer (bool): Whether to return answer in conversational form.
-            Default to False
-            show_code (bool): To show the intermediate python code generated on the prompt.
-            Default to False
+            is_conversational_answer (bool): Whether to return answer in conversational
+            form. Default to False
+            show_code (bool): To show the intermediate python code generated on the
+            prompt. Default to False
             anonymize_df (bool): Running the code with Sensitive Data. Default to True
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
         Returns (str): Answer to the Input Questions about the DataFrame
 
         """
 
+        self._start_time = time.time()
+
+        self.log(f"Question: {prompt}")
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
         self._prompt_id = str(uuid.uuid4())
         self.log(f"Prompt ID: {self._prompt_id}")
 
         
         self._history = history or []
 
         try:
-            if self._enable_cache and self._cache.get(prompt):
+            if self._enable_cache and self._cache and self._cache.get(prompt):
                 self.log("Using cached response")
                 code = self._cache.get(prompt)
             else:
                 rows_to_display = 0 if self._enforce_privacy else 5
 
                 multiple: bool = isinstance(data_frame, list)
 
                 if multiple:
-                    heads = [
-                        anonymize_dataframe_head(dataframe)
-                        if anonymize_df
-                        else dataframe.head(rows_to_display)
-                        for dataframe in data_frame
-                    ]
+                    # heads = [
+                    #     anonymize_dataframe_head(dataframe)
+                    #     if anonymize_df
+                    #     else dataframe.head(rows_to_display)
+                    #     for dataframe in data_frame
+                    # ]
 
+                    heads = data_frame
 
+                    multiple_dataframes_instruction = self._non_default_prompts.get(
+                        "multiple_dataframes", MultipleDataframesPrompt
+                    )
                     code = self._llm.generate_code(
-                        MultipleDataframesPrompt(dataframes=heads),
+                        multiple_dataframes_instruction(dataframes=heads),
                         prompt,
                         history,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": heads,
-                        "rows_to_display": rows_to_display,
                     }
 
                 else:
                     df_head = data_frame.head(rows_to_display)
                     if anonymize_df:
                         df_head = anonymize_dataframe_head(df_head)
+                    df_head = df_head.to_csv(index=False)
 
+                    generate_code_instruction = self._non_default_prompts.get(
+                        "generate_python_code", GeneratePythonCodePrompt
+                    )(
+                        prompt=prompt,
+                        df_head=df_head,
+                        num_rows=data_frame.shape[0],
+                        num_columns=data_frame.shape[1],
+                    )
                     code = self._llm.generate_code(
-                        GeneratePythonCodePrompt(
-                            prompt=prompt,
-                            df_head=df_head.to_string(),
-                            df_columns=data_frame.columns.tolist(),
-                            num_rows=data_frame.shape[0],
-                            num_columns=data_frame.shape[1],
-                            rows_to_display=rows_to_display,
-                        ),
+                        generate_code_instruction,
                         prompt,
                         history,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
-                        "df_head": df_head.to_string(),
+                        "df_head": df_head,
                         "df_columns": data_frame.columns.tolist(),
                         "num_rows": data_frame.shape[0],
                         "num_columns": data_frame.shape[1],
-                        "rows_to_display": rows_to_display,
                     }
 
                 self.last_code_generated = code
                 self.log(
                     f"""
                         Code generated:
                         ```
                         {code}
                         ```
                     """
                 )
 
-                
+
+                if self._enable_cache and self._cache:
+                    self._cache.set(prompt, code)
+
 
             if show_code and self._in_notebook:
                 self.notebook.create_new_cell(code)
 
+
+            for middleware in self._middlewares:
+                code = middleware(code)
+
+
             answer = self.run_code(
                 code,
                 data_frame,
                 use_error_correction_framework=use_error_correction_framework,
             )
             self.code_output = answer
             self.log(f"Answer: {answer}")
 
             if is_conversational_answer is None:
                 is_conversational_answer = self._is_conversational_answer
             if is_conversational_answer:
                 answer = self.conversational_answer(prompt, answer)
                 self.log(f"Conversational answer: {answer}")
 
-            ## add code to cache    
-            self._cache.set(prompt, code)
+            self.log(f"Executed in: {time.time() - self._start_time}s")
+
             return answer
-        except Exception as exception:  # pylint: disable=broad-except
+        except Exception as exception:
             self.last_error = str(exception)
+            print(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
             )
 
-    def original_chat(self,prompt: str,history: list = None) -> str:
+    def add_middlewares(self, *middlewares: List[Middleware]):
         """
-        Returns the original chat between the user and the AI.
+        Add middlewares to PandasAI instance.
 
-        Returns (str): Original Chat
+        Args:
+            *middlewares: A list of middlewares
 
         """
-        
-        answer  = self._llm.langchain_input(prompt, history)
+        self._middlewares.extend(middlewares)
+
 
-        return answer
-    
     def clear_cache(self):
         """
         Clears the cache of the PandasAI instance.
         """
-        self._cache.clear()
+        if self._cache:
+            self._cache.clear()
 
     def __call__(
         self,
-        data_frame: pd.DataFrame,
+        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
     ) -> Union[str, pd.DataFrame]:
         """
@@ -365,225 +493,285 @@
             prompt,
             is_conversational_answer,
             show_code,
             anonymize_df,
             use_error_correction_framework,
         )
 
-    def _is_unsafe_import(self, node: ast.stmt) -> bool:
+    def _check_imports(self, node: Union[ast.Import, ast.ImportFrom]):
         """
-        Remove non-whitelisted imports from the code to prevent malicious code execution
+        Add whitelisted imports to _additional_dependencies.
 
         Args:
-            node (object): ast.stmt
+            node (object): ast.Import or ast.ImportFrom
 
-        Returns (bool): A flag if unsafe_imports found.
+        Raises:
+            BadImportError: If the import is not whitelisted
 
         """
+        if isinstance(node, ast.Import):
+            module = node.names[0].name
+        else:
+            module = node.module
 
-        if isinstance(node, (ast.Import, ast.ImportFrom)):
+        library = module.split(".")[0]
+
+        if library == "pandas":
+            return
+
+        if library in WHITELISTED_LIBRARIES + self._custom_whitelisted_dependencies:
             for alias in node.names:
-                if (
-                    alias.name in WHITELISTED_BUILTINS
-                    or alias.name in ENVIRONMENT_DEFAULTS
-                ):
-                    return True
-                if alias.name in WHITELISTED_OPTIONAL_LIBRARIES:
-                    import_optional_dependency(alias.name)
-                    continue
-                if alias.name.split(".")[0] not in WHITELISTED_LIBRARIES:
-                    raise BadImportError(alias.name)
+                self._additional_dependencies.append(
+                    {
+                        "module": module,
+                        "name": alias.name,
+                        "alias": alias.asname or alias.name,
+                    }
+                )
+            return
 
-        return False
+        if library not in WHITELISTED_BUILTINS:
+            raise BadImportError(library)
 
-    def _is_df_overwrite(self, node: ast.stmt, multiple: bool) -> bool:
+    def _is_df_overwrite(self, node: ast.stmt) -> bool:
         """
-        Remove df declarations from the code to prevent malicious code execution. A helper method.
+        Remove df declarations from the code to prevent malicious code execution.
 
         Args:
             node (object): ast.stmt
 
         Returns (bool):
 
-        """ 
+        """
 
-        if multiple:
-            return (
-                isinstance(node, ast.Assign)
-                and isinstance(node.targets[0], ast.Name)
-                and re.match(r"^df\d+$", node.targets[0].id)
-            )
-        else:
-            return (
+        return (
             isinstance(node, ast.Assign)
             and isinstance(node.targets[0], ast.Name)
-            and re.match(r"df$", node.targets[0].id)
+            and re.match(r"df\d{0,2}$", node.targets[0].id)
         )
 
-
-     
-        
-    def _clean_code(self, code: str, multiple: bool) -> str:
+    def _clean_code(self, code: str) -> str:
         """
         A method to clean the code to prevent malicious code execution
 
         Args:
             code(str): A python code
 
         Returns (str): Returns a Clean Code String
 
         """
 
         tree = ast.parse(code)
 
-        new_body = [
-            node
-            for node in tree.body
-            if not (self._is_unsafe_import(node) or self._is_df_overwrite(node, multiple))
-        ]
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
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree).strip()
 
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
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
         """
-        A method to execute the python code generated by LLMs to answer the question about the
-        input dataframe. Run the code in the current context and return the result.
+        A method to execute the python code generated by LLMs to answer the question
+        about the input dataframe. Run the code in the current context and return the
+        result.
 
         Args:
             code (str): A python code to execute
             data_frame (pd.DataFrame): A full Pandas DataFrame
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
         Returns (str): String representation of the result of the code execution.
 
         """
 
-        # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
-
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
-            code = add_save_chart(code, self._prompt_id)
+            code = add_save_chart(
+                code, self._prompt_id, self._save_charts_path, not self._verbose
+            )
+
+        # code = "import pandas as pd\nfrom sklearn.linear_model import LinearRegression\n\n# Load the data into a pandas DataFrame\ndf1 = pd.DataFrame({\n    'Bank Name': ['Silicon Valley Bank', 'Signature Bank', 'Almena State Bank', \n                  'First City Bank of Florida', 'First Republic Bank'],\n    'City': ['Fort Walton Beach', 'San Francisco', 'New York', 'Almena', 'Santa Clara'],\n    'State': ['CA', 'KS', 'CA', 'FL', 'NY'],\n    'Cert': [16748, 15426, 15426, 24735, 24735],\n    'Acquiring Institution': ['Flagstar Bank, N.A.', 'First Citizens Bank & Trust Company', \n                              'United Fidelity Bank, fsb', 'Equity Bank', 'JPMorgan Chase Bank, N.A.'],\n    'Closing Date': ['23-Oct-20', '10-Mar-23', '1-May-23', '12-Mar-23', '16-Oct-20'],\n    'Fund': [10538, 10538, 10539, 10537, 10539]\n})\n\n# Convert the Closing Date column to a datetime object\ndf1['Closing Date'] = pd.to_datetime(df1['Closing Date'])\n\n# Add a column for the year of the closing date\ndf1['Closing Year'] = df1['Closing Date'].apply(lambda x: x.year)\n\n# Group the data by year and count the number of bank closures\ngrouped = df1.groupby('Closing Year').count()['Bank Name']\n\n# Create a linear regression model\nX = grouped.index.values.reshape(-1, 1)\ny = grouped.values.reshape(-1, 1)\nmodel = LinearRegression()\nmodel.fit(X, y)\n\n# Predict the number of bank closures in 2024\ny_pred = model.predict([[2024]])\nprint(int(round(y_pred[0][0])))"
 
         # Get the code to run removing unsafe imports and df overwrites
-        code_to_run = self._clean_code(code, multiple)
-        self.last_run_code = code_to_run
+        code_to_run = self._clean_code(code)
+        self.last_code_executed = code_to_run
         self.log(
             f"""
 Code running:
 ```
 {code_to_run}
 ```"""
         )
 
-        environment: dict = {
-            **{
-                alias: sys.modules[library]
-                for library, alias in ENVIRONMENT_DEFAULTS.items()
-            },
-            "__builtins__": {
-                **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
-            },
-        }
+        environment: dict = self._get_environment()
 
         if multiple:
             environment.update(
                 {f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start=1)}
             )
-
         else:
             environment["df"] = data_frame
 
         # Redirect standard output to a StringIO buffer
         with redirect_stdout(io.StringIO()) as output:
             count = 0
             while count < self._max_retries:
                 try:
                     # Execute the code
                     exec(code_to_run, environment)
                     code = code_to_run
                     break
-                except Exception as e:  # pylint: disable=W0718 disable=C0103
-                    # raise e
+                except Exception as e:
+                    if not use_error_correction_framework:
+                        raise e
 
                     count += 1
 
-                    if multiple:
-                        error_correcting_instruction = (
-                            CorrectMultipleDataframesErrorPrompt(
-                                code=code,
-                                error_returned=e,
-                                question=self._original_instructions["question"],
-                                df_head=self._original_instructions["df_head"],
-                            )
-                        )
-                    else:
-                        error_correcting_instruction = CorrectErrorPrompt(
-                            code=code,
-                            error_returned=e,
-                            question=self._original_instructions["question"],
-                            df_head=self._original_instructions["df_head"],
-                            df_columns=self._original_instructions["df_columns"],
-                            num_rows=self._original_instructions["num_rows"],
-                            num_columns=self._original_instructions["num_columns"],
-                            rows_to_display=self._original_instructions[
-                                "rows_to_display"
-                            ],
-                        )
-                    # print(error_correcting_instruction.text)
-                    code_to_run = self._llm.generate_code(
-                        error_correcting_instruction, "", self._history
-                    )
+                    code_to_run = self._retry_run_code(code, e, multiple)
 
-        captured_output = output.getvalue()
+        captured_output = output.getvalue().strip()
+        if code.count("print(") > 1:
+            return captured_output
 
         # Evaluate the last line and return its value or the captured output
+        # We do this because we want to return the right value and the right
+        # type of the value. For example, if the last line is `df.head()`, we
+        # want to return the head of the dataframe, not the captured output.
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
 
         match = re.match(r"^print\((.*)\)$", last_line)
         if match:
             last_line = match.group(1)
-            try:
-                return eval(last_line, environment)
-            except Exception as e:  # pylint: disable=W0718
-                raise e
-        else:
+
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
             return captured_output
 
         
     def log(self, message: str):
         """Log a message"""
-        if self._verbose:
-            print(message)
+        self._logger.info(message)
+        self._logs.append(message)
+
+    @property
+    def logs(self) -> List[str]:
+        """Return the logs"""
+        return self._logs
 
     def process_id(self) -> str:
         """Return the id of this PandasAI object."""
         return self._process_id
 
+    @property
     def last_prompt_id(self) -> str:
         """Return the id of the last prompt that was run."""
         if self._prompt_id is None:
             raise ValueError("Pandas AI has not been run yet.")
         return self._prompt_id
-    
+
+    @property
+    def last_prompt(self) -> str:
+        """Return the last prompt that was executed."""
+        if self._llm:
+            return self._llm.last_prompt
+
     def output_version(self) -> str:
         # 优先从pyproject.toml.orig获取,如果不存在则从pyproject.toml获取
         orig_file = 'pyproject.toml.orig'
         if os.path.exists(orig_file):
             with open(orig_file) as f:
                 pyproject_toml = toml.load(f)
         else:
             parent_dir = os.path.dirname(os.path.dirname(__file__))
             file_path = os.path.join(parent_dir, 'pyproject.toml')
             with open(file_path) as f:
                 pyproject_toml = toml.load(f)
         version = pyproject_toml['tool']['poetry']['version']
-        return version
+        return version
+
```

### Comparing `idoctorai-0.6.9/pandasai/exceptions.py` & `idoctorai-0.7.0/pandasai/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,9 +64,10 @@
         __init__ method of BadImportError Class
 
         Args:
             library_name (str): Name of the library that is not in the whitelist.
         """
         self.library_name = library_name
         super().__init__(
-            f"Generated code includes import of {library_name} which is not in whitelist."
+            f"Generated code includes import of {library_name} which"
+            " is not in whitelist."
         )
```

### Comparing `idoctorai-0.6.9/pandasai/helpers/_optional.py` & `idoctorai-0.7.0/pandasai/helpers/_optional.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 VERSIONS = {
     "sklearn": "1.2.2",
     "statsmodels": "0.14.0",
     "seaborn": "0.12.2",
     "plotly": "5.14.1",
     "ggplot": "0.11.5",
+    "scipy": "1.9.0",
+    "streamlit": "1.23.1",
 }
 
 # A mapping from import name to package name (on PyPI) for packages where
 # these two names are different.
 
 INSTALL_MAPPING = {}
 
@@ -36,15 +38,15 @@
 
     if version is None:
         raise ImportError(f"Can't determine version for {module.__name__}")
 
     return version
 
 
-def import_optional_dependency(
+def import_dependency(
     name: str,
     extra: str = "",
     errors: str = "raise",
     min_version: str | None = None,
 ):
     """
     Import an optional dependency.
```

### Comparing `idoctorai-0.6.9/pandasai/helpers/anonymizer.py` & `idoctorai-0.7.0/pandasai/helpers/anonymizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 """
 This module contains helper functions for anonymizing data and generating random data
-before sending it to the LLM (An External API). Only df.head() is sent to LLM API,
- hence the df.head() is processed to remove any personal or sensitive information.
+ before sending it to the LLM (An External API).
+
+Only df.head() is sent to LLM API, hence the df.head() is processed
+ to remove any personal or sensitive information.
 
 """
 
 import random
 import re
 import string
+
 import pandas as pd
 
 
 def is_valid_email(email: str) -> bool:
-
     """Check if the given email is valid based on regex pattern.
 
     Args:
         email (str): email address to be checked.
 
     Returns (bool): True if the email is valid, otherwise False.
     """
 
     email_regex = r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
     return re.match(email_regex, email) is not None
 
 
 def is_valid_phone_number(phone_number: str) -> bool:
-
     """Check if the given phone number is valid based on regex pattern.
 
     Args:
         phone_number (str): phone number to be checked.
 
     Returns (bool): True if the phone number is valid, otherwise False.
     """
 
     pattern = r"\b(?:\+?\d{1,3}[- ]?)?\(?\d{3}\)?[- ]?\d{3}[- ]?\d{4}\b"
     return re.search(pattern, phone_number) is not None
 
 
 def is_valid_credit_card(credit_card_number: str) -> bool:
-
     """Check if the given credit card number is valid based on regex pattern.
 
     Args:
         credit_card_number (str): credit card number to be checked.
 
     Returns (str): True if the credit card number is valid, otherwise False.
     """
 
     pattern = r"^\d{4}[- ]?\d{4}[- ]?\d{4}[- ]?\d{4}$"
     return re.search(pattern, credit_card_number) is not None
 
 
 def generate_random_email() -> str:
-
     """Generates a random email address using predefined domains.
 
     Returns (str): generated random email address.
     """
 
     domains = [
         "gmail.com",
@@ -75,15 +74,14 @@
     letters = string.ascii_lowercase + string.digits + "-_"
     username = "".join(random.choice(letters) for i in range(name_length))
     email = username + "@" + domain
     return email
 
 
 def generate_random_phone_number(original_field: str) -> str:
-
     """Generate a random phone number with country code if originally present.
 
     Args:
         original_field (str): original phone number field.
 
     Returns (str): generated random phone number.
     """
@@ -101,45 +99,42 @@
     else:
         phone_number = number
 
     return phone_number
 
 
 def generate_random_credit_card() -> str:
-
     """Generate a random credit card number.
 
     Returns (str): generated random credit card number.
     """
 
     groups = []
     for _i in range(4):
         group = "".join(random.choices("0123456789", k=4))
         groups.append(group)
     separator = random.choice(["-", " "])
     return separator.join(groups)
 
 
 def copy_head(data_frame: pd.DataFrame) -> pd.DataFrame:
-
     """Copy the head of a DataFrame.
 
     Args:
         data_frame (pd.DataFrame): The pd.DataFrame to copy the head from.
 
     Returns (pd.DataFrame): copied head of the DataFrame.
     """
 
     return data_frame.head().copy()
 
 
 def anonymize_dataframe_head(
     data_frame: pd.DataFrame, force_conversion: bool = True
 ) -> pd.DataFrame:
-
     """Anonymize the head of a given DataFrame by replacing sensitive data.
 
     Args:
 
         data_frame (pd.DataFrame):  The DataFrame to anonymize the head data.
         force_conversion (bool): Convert it with instruction. Default is True.
 
@@ -172,11 +167,13 @@
 
             # anonymize data
             random_row_index = random.choice(
                 [i for i in range(len(data_frame.index)) if i != row_idx]
             )
             random_value = data_frame.iloc[random_row_index, col_idx]
             data_frame.iloc[row_idx, col_idx] = random_value
-            data_frame.iloc[random_row_index, col_idx] = cell_value
+            data_frame.iloc[random_row_index, col_idx] = (
+                pd.eval(cell_value) if cell_value in ["True", "False"] else cell_value
+            )
     # restore the original data types
     data_frame = data_frame.astype(dtypes)
     return data_frame
```

### Comparing `idoctorai-0.6.9/pandasai/helpers/cache.py` & `idoctorai-0.7.0/pandasai/helpers/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Cache module for caching queries."""
 import glob
 import os
 import shelve
-from os.path import dirname
+from pathlib import Path
 
 
 class Cache:
-    """Cache class for caching queries. It is used to cache queries to avoid save time and money.
+    """Cache class for caching queries. It is used to cache queries
+    to save time and money.
 
     Args:
         filename (str): filename to store the cache.
     """
 
     def __init__(self, filename="cache"):
         # define cache directory and create directory if it does not exist
-        project_root = dirname(dirname(dirname(__file__)))
-        cache_dir = os.path.join(project_root, "cache")
-        if not os.path.exists(cache_dir):
-            os.makedirs(cache_dir)
+        cache_dir = os.path.join(Path.cwd(), "cache")
+        os.makedirs(cache_dir, mode=0o777, exist_ok=True)
 
         self.filepath = os.path.join(cache_dir, filename)
         self.cache = shelve.open(self.filepath)
 
     def set(self, key: str, value: str) -> None:
         """Set a key value pair in the cache.
```

### Comparing `idoctorai-0.6.9/pandasai/helpers/from_excel.py` & `idoctorai-0.7.0/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.9/pandasai/helpers/notebook.py` & `idoctorai-0.7.0/pandasai/helpers/notebook.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,41 +7,40 @@
 
 
 class Notebook:
 
     """Baseclass to implement Notebook helper functions"""
 
     def in_notebook(self) -> bool:
-
         """
         Checks whether the code is running inside a notebook environment.
 
-        Returns (bool): True if the code is running inside a Jupyter notebook, False otherwise.
+        Returns (bool): True if the code is running inside a Jupyter notebook,
+        False otherwise.
         """
         try:
             if "IPKernelApp" not in get_ipython().config:
                 return False
         except (ImportError, AttributeError):
             return False
         return True
 
     def create_new_cell(self, contents: str) -> None:
-
         """
-        Creates a new code cell in the Jupyter notebook and populates it with the specified
-        contents.
+        Creates a new code cell in the Jupyter notebook and populates
+        it with the specified contents.
         Args:
             contents (str): The contents to be added to the new code cell.
 
         ImportError:
             If the IPython module is not installed.
 
         AttributeError:
-            If the 'get_ipython()' call raises an AttributeError, which can happen if the code is
-            not running inside a Jupyter notebook.
+            If the 'get_ipython()' call raises an AttributeError, which can happen
+            if the code is not running inside a Jupyter notebook.
 
         Returns: None
 
         """
 
         payload = {"source": "set_next_input", "text": contents, "replace": False}
         try:
```

### Comparing `idoctorai-0.6.9/pandasai/helpers/save_chart.py` & `idoctorai-0.7.0/pandasai/helpers/save_chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Helper functions to save charts to a file, if plt.show() is called."""
 import ast
+import logging
 import os
 from itertools import zip_longest
 from os.path import dirname
 from typing import Union
 
 import astor
 
@@ -44,30 +45,42 @@
         return all(
             compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
         )
 
     return node1 == node2
 
 
-def add_save_chart(code: str, folder_name: str) -> str:
+def add_save_chart(
+    code: str,
+    folder_name: str,
+    save_charts_path: str = None,
+    print_save_dir: bool = True,
+) -> str:
     """
     Add line to code that save charts to a file, if plt.show() is called.
 
     Args:
         code (str): Code to add line to.
         folder_name (str): Name of folder to save charts to.
+        save_charts_path (str): User Defined Path to save Charts
+        print_save_dir (bool): Print the save directory to the console.
+            Defaults to True.
 
     Returns:
         str: Code with line added.
 
     """
 
-    # define chart save directory
-    project_root = dirname(dirname(dirname(__file__)))
-    chart_save_dir = os.path.join(project_root, "exports", "charts", folder_name)
+    if save_charts_path is not None:
+        charts_root_dir = save_charts_path
+    else:
+        # define chart save directory
+        charts_root_dir = dirname(dirname(dirname(__file__)))
+
+    chart_save_dir = os.path.join(charts_root_dir, "exports", "charts", folder_name)
 
     tree = ast.parse(code)
 
     # count number of plt.show() calls
     show_count = sum(
         compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
         for node in ast.walk(tree)
@@ -90,11 +103,14 @@
                 filename += f"_{chr(counter)}"
                 counter += 1
 
             chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
             new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
         new_body.append(node)
 
-    new_body.append(ast.parse(f"print(r'Charts saved to: {chart_save_dir}')"))
+    chart_save_msg = f"Charts saving to: {chart_save_dir}"
+    if print_save_dir:
+        print(chart_save_msg)
+    logging.info(chart_save_msg)
 
     new_tree = ast.Module(body=new_body)
     return astor.to_source(new_tree).strip()
```

### Comparing `idoctorai-0.6.9/pandasai/langchain/__init__.py` & `idoctorai-0.7.0/pandasai/langchain/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,17 +33,23 @@
 
 {history}
 Human: {human_input}
 Assistant:"""
     
     template= """Assistant is a large language model trained by OpenAI.
 
-Assistant is constantly learning and improving, and its capabilities are constantly evolving.Assistant is a very rigorous and careful tool, and will complete the task strictly according to the requirements of Human.
+Assistant is constantly learning and improving, and its capabilities are constantly evolving.
 
-Assistant was smart enough to complete my request based on the dataframe example I provided.
+Assistant was smart enough to complete my request based on the incomplete dataframe I provided.Assistant can complete the prediction based on the incomplete data I provided.
+
+{history}
+Human: {human_input}
+Assistant:"""
+
+    template= """Assistant is a large language model trained by OpenAI.Assistant can complete the prediction based on the incomplete data I provided.
 
 {history}
 Human: {human_input}
 Assistant:"""
 
     def __init__(self, llm: AzureOpenAI, **kwargs,):
         # self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0)
```

### Comparing `idoctorai-0.6.9/pandasai/llm/azure_openai.py` & `idoctorai-0.7.0/pandasai/llm/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,128 @@
-"""OpenAI LLM via Microsoft Azure Cloud
+from dotenv import load_dotenv
+import os
+from typing import Any, Dict, Optional
+from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
 
-This module is to run the OpenAI API when using Microsoft Cloud infrastructure. Azure has
-implemented the openai API access to its platform.
-For details https://learn.microsoft.com/en-us/azure/cognitive-services/openai/reference.
+from langchain.chat_models import AzureChatOpenAI
 
-Example:
-    Use below example to call AzureOpenAI class
+from ..prompts.base import Prompt
+from langchain.llms import AzureOpenAI
+from .base import BaseOpenAI
+from ..langchain import LangChain
 
-    >>> from pandasai.llm.azure_openai import AzureOpenAI
 
-"""
 
-import os
-from typing import Any, Dict, Optional
+load_dotenv()
 
-import openai
-from dotenv import load_dotenv
-from openai import InvalidRequestError
-from openai.error import APIConnectionError
 
-from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
-from .base import BaseOpenAI
+class Model(BaseOpenAI):
 
-load_dotenv()
 
+    """AzureOpenAI LLM using BaseOpenAI Class.
+
+    model_name: str  # gpt-35-turbo-16k  gpt-35-turbo
+    api_version: str  # 2023-03-15-preview  2023-05-15
+    deployment_name: str  # gpt-35-16k GPT35
 
-class AzureOpenAI(BaseOpenAI):
-    """OpenAI LLM via Microsoft Azure
-    This class in using BaseOpenAI class to include Azure OpenAI Features.
     """
 
-    api_base: str
-    api_type: str = "azure"
-    api_version: str
-    engine: str
+    api_token: str
+    api_base:str
+    model_name: str  
+    api_version: str  
+    max_tokens: int = 4097
+    deployment_name: str  
+    llm: AzureOpenAI
+    
+    _supported_chat_models = [
+        "gpt-4",
+        "gpt-4-0314",
+        "gpt-4-32k",
+        "gpt-4-32k-0314",
+        "gpt-3.5-turbo",
+        "gpt-3.5-turbo-0301",
+    ]
+    _supported_completion_models = ["text-davinci-003"]
+
+    model: str = "gpt-3.5-turbo"
+    langchain: LangChain
 
-    def __init__(
-        self,
+    def __init__(self,
         api_token: Optional[str] = None,
         api_base: Optional[str] = None,
         api_version: Optional[str] = None,
         deployment_name: str = None,
+        model_name: str = None,
         **kwargs, ):
 
-        """
-        __init__ method of AzureOpenAI Class
-
-        Args:
-            api_token (str): Azure OpenAI API token.
-            api_base (str): Base url of the Azure endpoint.
-                It should look like the following: <https://YOUR_RESOURCE_NAME.openai.azure.com/>
-            api_version (str): Version of the Azure OpenAI API. Be aware the API version may change.
-            deployment_name: Custom name of the deployed model
-            **kwargs: Inference Parameters
-        """
-
         self.api_token = api_token or os.getenv("AZURE_OPENAI_KEY") or None
         self.api_base = api_base or os.getenv("AZURE_OPENAI_ENDPOINT") or None
-        self.api_version = api_version or "2023-03-15-preview"
+        self.api_version = api_version or os.getenv("AZURE_OPENAI_VERSION") or None
+        self.deployment_name = deployment_name or os.getenv("DEPLOYMENT_NAME") or None
+        self.model_name = model_name or os.getenv("MODEL_NAME") or None
+
         if self.api_token is None:
             raise APIKeyNotFoundError("Azure OpenAI key is required")
         if self.api_base is None:
             raise APIKeyNotFoundError("Azure OpenAI base endpoint is required")
-
-        openai.api_key = self.api_token
-        openai.api_base = self.api_base
-        openai.api_version = self.api_version
-        openai.api_type = self.api_type
-
-        if deployment_name is None:
+        if self.deployment_name is None:
             raise UnsupportedOpenAIModelError("Model deployment name is required.")
-        try:
-            model_name = openai.Deployment.retrieve(deployment_name).model
-            model_capabilities = openai.Model.retrieve(model_name).capabilities
-            if (
-                not model_capabilities.completion
-                and not model_capabilities.chat_completion
-            ):
-                raise UnsupportedOpenAIModelError(
-                    "Model deployment name does not correspond to a "
-                    "chat nor a completion model."
-                )
-            self.is_chat_model = model_capabilities.chat_completion
-            self.engine = deployment_name
-        except InvalidRequestError as ex:
-            raise UnsupportedOpenAIModelError(
-                "Model deployment name does not correspond to a valid model entity."
-            ) from ex
-        except APIConnectionError as ex:
-            raise UnsupportedOpenAIModelError(
-                f"Invalid Azure OpenAI Base Endpoint {api_base}"
-            ) from ex
-
+        if self.model_name is None:
+            raise UnsupportedOpenAIModelError("Model name is required.")
+        if self.api_version is None:
+            raise UnsupportedOpenAIModelError("Azure OpenAI version is required.")
+
+        self.llm = AzureChatOpenAI(
+            openai_api_base=self.api_base,
+            openai_api_version=self.api_version,
+            deployment_name=self.deployment_name,
+            openai_api_key=self.api_token,
+            openai_api_type="azure",
+            max_tokens = self.max_tokens,
+            model_name = self.model_name,
+          )
+        # print(self.llm)
+        self.langchain = LangChain(llm = self.llm)
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
+        """Get the default parameters for calling OpenAI API"""
+        return {
+            **super()._default_params,
+            "model": self.model,
+        }
 
-        """Get the default parameters for calling OpenAI API
-
-        Returns: A dict of Default Params
-
-        """
-        return {**super()._default_params, "engine": self.engine}
-
-    def call(self, instruction: str, value: str, suffix: str = "") -> str:
-
+    def call(self, instruction: Prompt, value: str, suffix: str = "", history: list = None) -> str:
         """
-        Call the Azure OpenAI LLM.
+        Call the OpenAI LLM.
 
         Args:
-            instruction (str): Instruction to pass
+            instruction (Prompt): Instruction to pass
             value (str): Value to pass
-            suffix(str): Suffix to pass
+            suffix (str): Suffix to pass
+
+        Raises:
+            UnsupportedOpenAIModelError: Unsupported model
 
         Returns:
             str: Response
         """
         self.last_prompt = str(instruction) + str(value)
 
-        if self.is_chat_model:
-            response = self.chat_completion(str(instruction) + str(value) + suffix)
-        else:
+        if self.model in self._supported_completion_models:
             response = self.completion(str(instruction) + str(value) + suffix)
+        elif self.model in self._supported_chat_models:
+            # response = self.chat_completion(str(instruction) + str(value) + suffix)
+            response = self.langchain_input(str(instruction) + str(value) + suffix, history)
+            # print(response)
+        else:
+            raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
     def type(self) -> str:
-        return "azure-openai"
+        return "openai"
+        
+
```

### Comparing `idoctorai-0.6.9/pandasai/llm/base.py` & `idoctorai-0.7.0/pandasai/llm/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Base class to implement a new LLM
 
-This module is the base class to integrate the various LLMs API. This module also includes the
-Base LLM classes for OpenAI, HuggingFace and Google PaLM.
+This module is the base class to integrate the various LLMs API. This module also
+includes the Base LLM classes for OpenAI, HuggingFace and Google PaLM.
 
 Example:
 
     ```
     from .base import BaseOpenAI
 
     class CustomLLM(BaseOpenAI):
@@ -18,29 +18,37 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
 
 import openai
 import requests
 
-from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
-from ..helpers._optional import import_optional_dependency
+from ..helpers._optional import import_dependency
 from ..prompts.base import Prompt
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
     last_prompt: Optional[str] = None
 
+    def is_pandasai_llm(self) -> bool:
+        """
+        Return True if the LLM is from pandasAI.
+
+        Returns:
+            bool: True if the LLM is from pandasAI
+        """
+        return True
+
     @property
     def type(self) -> str:
         """
         Return type of LLM.
 
         Raises:
             APIKeyNotFoundError: Type has not been implemented
@@ -94,21 +102,14 @@
         Raises:
             NoCodeFoundError: No code found in the response
 
         Returns:
             str: Extracted code from the response
         """
         code = response
-        match = re.search(
-            rf"{START_CODE_TAG}(.*)({END_CODE_TAG}|{END_CODE_TAG.replace('<', '</')})",
-            code,
-            re.DOTALL,
-        )
-        if match:
-            code = match.group(1).strip()
         if len(code.split(separator)) > 1:
             code = code.split(separator)[1]
         code = self._polish_code(code)
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
@@ -147,14 +148,16 @@
     api_token: str
     temperature: float = 0
     max_tokens: int = 512
     top_p: float = 1
     frequency_penalty: float = 0
     presence_penalty: float = 0.6
     stop: Optional[str] = None
+    # support explicit proxy for OpenAI
+    openai_proxy: Optional[str] = None
 
     def _set_params(self, **kwargs):
         """
         Set Parameters
         Args:
             **kwargs: ["model", "engine", "deployment_id", "temperature","max_tokens",
             "top_p", "frequency_penalty", "presence_penalty", "stop", ]
@@ -313,17 +316,17 @@
     """Base class to implement a new Google LLM
 
     LLM base class is extended to be used with Google Palm API.
     """
 
     genai: Any
     temperature: Optional[float] = 0
-    top_p: Optional[float] = None
-    top_k: Optional[float] = None
-    max_output_tokens: Optional[int] = None
+    top_p: Optional[float] = 0.8
+    top_k: Optional[float] = 0.3
+    max_output_tokens: Optional[int] = 1000
 
     def _configure(self, api_key: str):
         """
         Configure Google Palm API Key
         Args:
             api_key (str): A string of API keys generated from Google Cloud
 
@@ -331,19 +334,35 @@
 
         """
 
         if not api_key:
             raise APIKeyNotFoundError("Google Palm API key is required")
 
         err_msg = "Install google-generativeai >= 0.1 for Google Palm API"
-        genai = import_optional_dependency("google.generativeai", extra=err_msg)
+        genai = import_dependency("google.generativeai", extra=err_msg)
 
         genai.configure(api_key=api_key)
         self.genai = genai
 
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
     def _valid_params(self):
         return ["temperature", "top_p", "top_k", "max_output_tokens"]
 
     def _set_params(self, **kwargs):
         """
         Set Parameters
         Args:
@@ -387,17 +406,17 @@
         raise MethodNotImplementedError("method has not been implemented")
 
     def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
         """
         Call the Google LLM.
 
         Args:
-            instruction (str): Instruction to pass
+            instruction (object): Instruction to pass
             value (str): Value to pass
             suffix (str): Suffix to pass
 
         Returns:
             str: Response
         """
-        self.last_prompt = str(instruction) + str(value)
-        prompt = str(instruction) + str(value) + suffix
+        self.last_prompt = str(instruction) + value
+        prompt = str(instruction) + value + suffix
         return self._generate_text(prompt)
```

### Comparing `idoctorai-0.6.9/pandasai/llm/fake.py` & `idoctorai-0.7.0/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.9/pandasai/llm/open_assistant.py` & `idoctorai-0.7.0/pandasai/llm/open_assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Open Assistant LLM
 
-This module is to run the HuggingFace OpenAssistant API hosted and maintained by HuggingFace.co.
-To generate HF_TOKEN go to https://huggingface.co/settings/tokens after creating Account on
-the platform.
+This module is to run the HuggingFace OpenAssistant API hosted and maintained by
+HuggingFace.co. To generate HF_TOKEN go to https://huggingface.co/settings/tokens after
+creating Account on the platform.
 
 Example:
-    Use below example to call Starcoder Model
+    Use below example to call OpenAssistant Model
 
     >>> from pandasai.llm.open_assistant import OpenAssistant
 """
 
 import os
 from typing import Optional
 
@@ -19,29 +19,28 @@
 from .base import HuggingFaceLLM
 
 load_dotenv()
 
 
 class OpenAssistant(HuggingFaceLLM):
     """Open Assistant LLM
-     A base HuggingFaceLLM class is extended to use OpenAssistant Model via its API.
-     Currently `oasst-sft-1-pythia-12b` is supported via this module.
+    A base HuggingFaceLLM class is extended to use OpenAssistant Model via its API.
+    Currently `oasst-sft-1-pythia-12b` is supported via this module.
     """
 
     api_token: str
     _api_url: str = (
         "https://api-inference.huggingface.co/models/"
         "OpenAssistant/oasst-sft-1-pythia-12b"
     )
     _max_retries: int = 10
 
     def __init__(self, api_token: Optional[str] = None):
-
         """
-        __init__ method of OpenAssistant Calss
+        __init__ method of OpenAssistant Class
 
         Raises:
             APIKeyNotFoundError: HuggingFace Hub API key is required
 
         Args:
             api_token (str): API token from Huggingface platform
         """
```

### Comparing `idoctorai-0.6.9/pandasai/llm/openai.py` & `idoctorai-0.7.0/pandasai/llm/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,28 +23,30 @@
 load_dotenv()
 
 
 class OpenAI(BaseOpenAI):
     """OpenAI LLM using BaseOpenAI Class.
 
     An API call to OpenAi API is sent and response is recorded and returned.
-    The default chat model is **gpt-3.5-turbo** while **text-davinci-003** is only supported
-    completion model.
+    The default chat model is **gpt-3.5-turbo** while **text-davinci-003** is only
+    supported completion model.
     The list of supported Chat models includes ["gpt-4", "gpt-4-0314", "gpt-4-32k",
      "gpt-4-32k-0314","gpt-3.5-turbo", "gpt-3.5-turbo-0301"].
 
     """
 
     _supported_chat_models = [
         "gpt-4",
-        "gpt-4-0314",
+        "gpt-4-0613",
         "gpt-4-32k",
-        "gpt-4-32k-0314",
+        "gpt-4-32k-0613",
         "gpt-3.5-turbo",
-        "gpt-3.5-turbo-0301",
+        "gpt-3.5-turbo-16k",
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k-0613",
     ]
     _supported_completion_models = ["text-davinci-003"]
 
     model: str = "gpt-3.5-turbo"
     langchain: LangChain
 
     def __init__(
@@ -64,14 +66,21 @@
         self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
         if self.api_token is None:
             raise APIKeyNotFoundError("OpenAI API key is required")
         openai.api_key = self.api_token
 
         # # langchain 
         # self.langchain = LangChain(api_token=self.api_token)
+        
+        self.openai_proxy = kwargs.get("openai_proxy") or os.getenv("OPENAI_PROXY")
+        if self.openai_proxy:
+            openai.proxy = {
+                "http": self.openai_proxy,
+                "https": self.openai_proxy
+            }
 
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API"""
         return {
```

### Comparing `idoctorai-0.6.9/pandasai/llm/starcoder.py` & `idoctorai-0.7.0/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.9/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.7.0/pandasai/prompts/correct_error_prompt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,49 @@
 """ Prompt to correct Python Code on Error
 ```
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the result of `print(df.head({rows_to_display}))`:
+This is the metadata of the dataframe:
 {df_head}.
 
 The user asked the following question:
 {question}
 
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above
-mentioned error. Do not generate the same code again. Make sure to prefix the requested python
-code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
+mentioned error. Do not generate the same code again.
 ```
-"""
-# pylint:disable=duplicate-code
+"""  # noqa: E501
 from datetime import date
 
-from pandasai.constants import END_CODE_TAG, START_CODE_TAG
-
 from .base import Prompt
 
 
 class CorrectErrorPrompt(Prompt):
     """Prompt to Correct Python code on Error"""
-    # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the result of `print(df.head({rows_to_display}))`:
+This is the metadata of the dataframe:
 {df_head}.
 the columns are {df_columns}.
 
 The user asked the following question:
 {question}
 
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
-Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
-"""
+"""  # noqa: E501
 
     def __init__(self, **kwargs):
-        super().__init__(
-            **kwargs,
-            START_CODE_TAG=START_CODE_TAG,
-            END_CODE_TAG=END_CODE_TAG,
-            today_date=date.today()
-        )
+        super().__init__(**kwargs, today_date=date.today())
```

### Comparing `idoctorai-0.6.9/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.7.0/pandasai/prompts/correct_multiples_prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 """ Prompt to correct error """
 
 import pandas as pd
 
-from pandasai.constants import END_CODE_TAG, START_CODE_TAG
-
 from .base import Prompt
 
 
 class CorrectMultipleDataframesErrorPrompt(Prompt):
     """Prompt to generate Python code"""
-    # pylint: disable=too-few-public-methods
 
     text: str = """
 You are provided with the the example of pandas dataframes:"""
 
     def __init__(
         self,
         code: str,
         error_returned: Exception,
         question: str,
         df_head: list[pd.DataFrame],
-    ): # pylint: disable=super-init-not-called
+    ):
         for i, dataframe in enumerate(df_head, start=1):
             row, col = dataframe.shape
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
-This is the result of `print(df{i}.head())`:
+This is the metadata of the dataframe df{i}:
 {dataframe}"""
 
         instruction: str = f"""
 The user asked the following question:
 {question}
 
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
-Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
-"""
+"""  # noqa: E501
 
         self.text += instruction
 
     def __str__(self):
         return self.text
```

### Comparing `idoctorai-0.6.9/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.7.0/pandasai/prompts/multiple_dataframes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """ Prompt to generate Python code for multiple dataframes """
 
 from datetime import date
 
 import pandas as pd
 
-from pandasai.constants import END_CODE_TAG, START_CODE_TAG
-
 from .base import Prompt
 
 
 class MultipleDataframesPrompt(Prompt):
     """Prompt to generate Python code"""
-    # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
-You are provided with the example of pandas dataframes:"""
+You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
 Don't add too many code comments.The result must be printed at the end of the python code.If the data format is not standard, standardize and format the data first.
-Using the provided dataframes only and Do not create your own dataframe, return the python code(no duplicate) and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
-"""
+Using the provided dataframes and no other dataframes, return the python code to get the answer to the following question:
+"""  # noqa: E501
 
-    def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
+    def __init__(self, dataframes: list[pd.DataFrame]):
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
-            data_text = dataframe.head().to_string()
+            dfhead = dataframe.head(5).to_csv(index=False)
 
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
-This is the result of `print(df{i}.head())`:
-{data_text}"""
+This is the first 5 rows of the dataframe df{i}:
+{dfhead}"""
+
 
         self.text += self.instruction
         self.text = self.text.format(
             today_date=date.today(),
-            START_CODE_TAG=START_CODE_TAG,
-            END_CODE_TAG=END_CODE_TAG,
         )
 
     def __str__(self):
         return self.text
```

### Comparing `idoctorai-0.6.9/pyproject.toml` & `idoctorai-0.7.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.6.9"
-description = "idoctorai"
-authors = ["Gabriele Venturi"]
+version = "0.7.0"
+description = "Idoctor AI is a Python library that integrates generative artificial intelligence capabilities into Pandas."
+authors = ["FH"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "pandasai"},{include="pyproject.toml"}]
-
-
-
+packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 python-dotenv = "^1.0.0"
 pandas = "1.5.3"
-openpyxl = "3.1.2"
 astor = "^0.8.1"
 openai = "^0.27.5"
-langchain = "0.0.194"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
-toml = "^0.10.2"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
-
-scikit-learn = "^1.2.2"
-seaborn = "^0.12.2"
-statsmodels = "^0.14.0"
-plotly = "^5.14.1"
-ggplot = "^0.11.5"
-
+google-cloud-aiplatform = { version = "^1.26.1", optional = true }
+langchain = { version = "^0.0.199", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
-pylint = "^2.17.3"
+ruff = "^0.0.220"
 pytest = "^7.3.1"
-isort = "^5.12.0"
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 
+
+[tool.poetry.group.extras.dependencies]
+google-cloud-aiplatform = "^1.26.1"
+
 [tool.poetry.extras]
 google = ["google-generativeai"]
+tests = ["numpy", "seaborn"]
+langchain = ["langchain"]
+google-cloud = ["google-cloud-aiplatform"]
 
 [tool.poetry.group.whitelist.dependencies]
 statsmodels = {version = "^0.14.0", optional = true}
 scikit-learn = {version = "^1.2.2", optional = true}
 seaborn = {version = "^0.12.2", optional = true}
 plotly = {version = "^5.14.1", optional = true}
 ggplot = {version = "^0.11.5", optional = true}
+numpy = {version = "^1.17", optional = true}
+scipy = {version = "^1.9.0", optional = true}
+streamlit = { version = "^1.23.1", optional = true }
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.0"
 mkdocstrings-python = "0.7.1"
 markdown-include = "^0.6.0"
 
 [tool.poetry.scripts]
 pai = "pai.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.pylint]
-ignore = "tests_*"
+[tool.ruff]
+exclude = ["tests_*"]
 
 [tool.pytest.ini_options]
 env = [
     "HUGGINGFACE_API_KEY=",
     "OPENAI_API_KEY="
-]
+]
```

