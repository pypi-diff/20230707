# Comparing `tmp/gpt_fn-0.0.8.tar.gz` & `tmp/gpt_fn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.0.8.tar", max compression
+gzip compressed data, was "gpt_fn-0.0.9.tar", max compression
```

## Comparing `gpt_fn-0.0.8.tar` & `gpt_fn-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1066 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/LICENSE
--rw-r--r--   0        0        0     4119 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/README.md
--rw-r--r--   0        0        0      852 2023-07-06 05:52:36.856174 gpt_fn-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/__init__.py
--rw-r--r--   0        0        0      767 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/ai_function.py
--rw-r--r--   0        0        0     4278 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/completion.py
--rw-r--r--   0        0        0      537 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/conftest.py
--rw-r--r--   0        0        0      342 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/exceptions.py
--rw-r--r--   0        0        0      878 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/prompt.py
--rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/py.typed
--rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__init__.py
--rw-r--r--   0        0        0      271 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0     9184 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_completion.ambr
--rw-r--r--   0        0        0      330 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0     3457 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0     4059 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0    16256 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0    15664 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
--rw-r--r--   0        0        0     9246 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion.yaml
--rw-r--r--   0        0        0     6251 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml
--rw-r--r--   0        0        0     6530 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml
--rw-r--r--   0        0        0     7869 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_structural_completion.yaml
--rw-r--r--   0        0        0     6611 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml
--rw-r--r--   0        0        0      872 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/test_ai_function.py
--rw-r--r--   0        0        0     4151 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/test_completion.py
--rw-r--r--   0        0        0      522 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/__init__.py
--rw-r--r--   0        0        0     1951 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     3560 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/signature.py
--rw-r--r--   0        0        0        0 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/__init__.py
--rw-r--r--   0        0        0     4717 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0    14060 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0     7162 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser_with_prompt[email.txt-Email].yaml
--rw-r--r--   0        0        0     2186 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt
--rw-r--r--   0        0        0     1734 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     2647 2023-07-06 05:52:16.640026 gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 gpt_fn-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-07 14:26:09.101130 gpt_fn-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4102 2023-07-07 14:26:09.101130 gpt_fn-0.0.9/README.md
+-rw-r--r--   0        0        0      852 2023-07-07 14:26:37.569792 gpt_fn-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0      767 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0     4278 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/completion.py
+-rw-r--r--   0        0        0      537 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      342 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/exceptions.py
+-rw-r--r--   0        0        0      883 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0     9184 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/__snapshots__/test_completion.ambr
+-rw-r--r--   0        0        0      713 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0     3457 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0     4059 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0    16256 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0    15664 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
+-rw-r--r--   0        0        0     9246 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_function_completion.yaml
+-rw-r--r--   0        0        0     6251 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml
+-rw-r--r--   0        0        0     6530 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml
+-rw-r--r--   0        0        0     7869 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_structural_completion.yaml
+-rw-r--r--   0        0        0     6611 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml
+-rw-r--r--   0        0        0      872 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0     4151 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/test_completion.py
+-rw-r--r--   0        0        0     1557 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1951 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     3560 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0     4717 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0    14060 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0     7162 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser_with_prompt[email.txt-Email].yaml
+-rw-r--r--   0        0        0     2186 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt
+-rw-r--r--   0        0        0     1734 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     2647 2023-07-07 14:26:09.105130 gpt_fn-0.0.9/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 gpt_fn-0.0.9/PKG-INFO
```

### Comparing `gpt_fn-0.0.8/LICENSE` & `gpt_fn-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/README.md` & `gpt_fn-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,37 +29,32 @@
 
 You can install GPT-Fn using pip, the Python package manager:
 
 ```bash
 pip install gpt-fn
 ```
 
-Alternatively, you can clone the repository and install it manually:
-
-```bash
-git clone https://github.com/your-username/gpt-fn.git
-cd gpt-fn
-pip install -r requirements.txt
-python setup.py install
-```
-
 ## Getting Started
 
-To start using GPT-Fn in your project, import the library and call the desired AI function:
+To start using GPT-Fn in your project, import the library and call the desired function:
 
 ```python
-from gpt_fn import text_generation
+from gpt_fn.completion import chat_completion
 
-input_text = "Once upon a time"
-generated_text = text_generation.generate_text(input_text, max_length=100)
+generated_text = chat_completion(
+    [
+        {"role": "system", "content": "You are a helpful assistant."},
+        {"role": "user", "content": "Hello, who are you?"},
+    ],
+)
 
 print(generated_text)
 ```
 
-In the example above, we use the `text_generation.generate_text` function to generate additional text based on an initial input. You can explore other available AI functions in the GPT-Fn documentation for a wide range of AI tasks.
+In the example above, we use the `chat_completion` function to generate response by AI. `chat_completion` also raises error on incomplete responses. The implementation of `chat_completion` makes the most common use case easy. You can explore other available functions in the GPT-Fn documentation/[tests](src/gpt_fn/tests/) for a wide range of AI tasks.
 
 ## Contributing
 
 We welcome contributions from the developer community to help improve GPT-Fn. If you encounter any issues, have ideas for new features, or would like to contribute code, please check out our [contribution guidelines](CONTRIBUTING.md). We appreciate your support!
 
 ## License
 
@@ -67,8 +62,8 @@
 
 ## Acknowledgements
 
 We would like to thank the open-source community for their valuable contributions and the creators of the underlying AI models that power GPT-Fn.
 
 ## Contact
 
-If you have any questions, suggestions, or feedback, please don't hesitate to contact us at [email protected]
+If you have any questions, suggestions, or feedback, please don't hesitate to opena an issue.
```

### Comparing `gpt_fn-0.0.8/pyproject.toml` & `gpt_fn-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `gpt_fn-0.0.8/src/gpt_fn/ai_function.py` & `gpt_fn-0.0.9/src/gpt_fn/ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/completion.py` & `gpt_fn-0.0.9/src/gpt_fn/completion.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/conftest.py` & `gpt_fn-0.0.9/src/gpt_fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/prompt.py` & `gpt_fn-0.0.9/src/gpt_fn/prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Literal
+from typing import Any, Literal
 
 import jinja2
 from pydantic import BaseModel
 
 from .completion import FunctionMessage, Message
 
 
 class MessageTemplate(BaseModel):
     role: Literal["system", "user", "assistant", "function"]
     content: str
     name: str = ""
 
-    def render(self, **kwargs: str) -> Message:
+    def render(self, **kwargs: Any) -> Message:
         content = jinja2.Template(self.content).render(**kwargs)
         if self.role == "function":
             return FunctionMessage(
                 role=self.role,
                 content=content,
                 name=self.name,
             )
@@ -25,9 +25,9 @@
         # remove whitespace
         anystr_strip_whitespace = True
 
 
 class ChatTemplate(BaseModel):
     messages: list[MessageTemplate]
 
-    def render(self, **kwargs: str) -> list[Message]:
+    def render(self, **kwargs: Any) -> list[Message]:
         return [m.render(**kwargs) for m in self.messages]
```

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/__snapshots__/test_completion.ambr` & `gpt_fn-0.0.9/src/gpt_fn/tests/__snapshots__/test_completion.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_function_completion.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_structural_completion.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_structural_completion.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml` & `gpt_fn-0.0.9/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/test_ai_function.py` & `gpt_fn-0.0.9/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/tests/test_completion.py` & `gpt_fn-0.0.9/src/gpt_fn/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/pydantic_parser.py` & `gpt_fn-0.0.9/src/gpt_fn/utils/pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/signature.py` & `gpt_fn-0.0.9/src/gpt_fn/utils/signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.0.9/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.0.9/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser_with_prompt[email.txt-Email].yaml` & `gpt_fn-0.0.9/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser_with_prompt[email.txt-Email].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt` & `gpt_fn-0.0.9/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.0.9/src/gpt_fn/utils/tests/test_pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/src/gpt_fn/utils/tests/test_signature.py` & `gpt_fn-0.0.9/src/gpt_fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.8/PKG-INFO` & `gpt_fn-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -45,37 +45,32 @@
 
 You can install GPT-Fn using pip, the Python package manager:
 
 ```bash
 pip install gpt-fn
 ```
 
-Alternatively, you can clone the repository and install it manually:
-
-```bash
-git clone https://github.com/your-username/gpt-fn.git
-cd gpt-fn
-pip install -r requirements.txt
-python setup.py install
-```
-
 ## Getting Started
 
-To start using GPT-Fn in your project, import the library and call the desired AI function:
+To start using GPT-Fn in your project, import the library and call the desired function:
 
 ```python
-from gpt_fn import text_generation
+from gpt_fn.completion import chat_completion
 
-input_text = "Once upon a time"
-generated_text = text_generation.generate_text(input_text, max_length=100)
+generated_text = chat_completion(
+    [
+        {"role": "system", "content": "You are a helpful assistant."},
+        {"role": "user", "content": "Hello, who are you?"},
+    ],
+)
 
 print(generated_text)
 ```
 
-In the example above, we use the `text_generation.generate_text` function to generate additional text based on an initial input. You can explore other available AI functions in the GPT-Fn documentation for a wide range of AI tasks.
+In the example above, we use the `chat_completion` function to generate response by AI. `chat_completion` also raises error on incomplete responses. The implementation of `chat_completion` makes the most common use case easy. You can explore other available functions in the GPT-Fn documentation/[tests](src/gpt_fn/tests/) for a wide range of AI tasks.
 
 ## Contributing
 
 We welcome contributions from the developer community to help improve GPT-Fn. If you encounter any issues, have ideas for new features, or would like to contribute code, please check out our [contribution guidelines](CONTRIBUTING.md). We appreciate your support!
 
 ## License
 
@@ -83,9 +78,9 @@
 
 ## Acknowledgements
 
 We would like to thank the open-source community for their valuable contributions and the creators of the underlying AI models that power GPT-Fn.
 
 ## Contact
 
-If you have any questions, suggestions, or feedback, please don't hesitate to contact us at [email protected]
+If you have any questions, suggestions, or feedback, please don't hesitate to opena an issue.
```

