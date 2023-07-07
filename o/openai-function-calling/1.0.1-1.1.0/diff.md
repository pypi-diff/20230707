# Comparing `tmp/openai_function_calling-1.0.1.tar.gz` & `tmp/openai_function_calling-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_calling-1.0.1.tar", max compression
+gzip compressed data, was "openai_function_calling-1.1.0.tar", max compression
```

## Comparing `openai_function_calling-1.0.1.tar` & `openai_function_calling-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     2210 2023-06-28 04:20:47.915657 openai_function_calling-1.0.1/README.md
--rw-r--r--   0        0        0      407 2023-06-28 04:20:47.916273 openai_function_calling-1.0.1/openai_function_calling/__init__.py
--rw-r--r--   0        0        0     3410 2023-06-30 18:14:11.747488 openai_function_calling-1.0.1/openai_function_calling/function.py
--rw-r--r--   0        0        0      330 2023-06-28 04:20:47.916650 openai_function_calling-1.0.1/openai_function_calling/json_schema_type.py
--rw-r--r--   0        0        0     3147 2023-06-28 04:20:47.916870 openai_function_calling-1.0.1/openai_function_calling/parameter.py
--rw-r--r--   0        0        0        0 2023-06-28 04:20:47.916908 openai_function_calling-1.0.1/openai_function_calling/py.typed
--rw-r--r--   0        0        0      625 2023-06-30 18:17:45.444765 openai_function_calling-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 openai_function_calling-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3409 2023-07-07 04:39:21.036437 openai_function_calling-1.1.0/README.md
+-rw-r--r--   0        0        0      499 2023-07-07 04:39:21.036852 openai_function_calling-1.1.0/openai_function_calling/__init__.py
+-rw-r--r--   0        0        0     5209 2023-07-07 04:39:21.037043 openai_function_calling-1.1.0/openai_function_calling/function.py
+-rw-r--r--   0        0        0     4754 2023-07-07 04:39:21.037184 openai_function_calling-1.1.0/openai_function_calling/function_inferer.py
+-rw-r--r--   0        0        0     1096 2023-07-07 04:39:21.037313 openai_function_calling-1.1.0/openai_function_calling/helper_functions.py
+-rw-r--r--   0        0        0      330 2023-06-28 04:20:47.916650 openai_function_calling-1.1.0/openai_function_calling/json_schema_type.py
+-rw-r--r--   0        0        0     4756 2023-07-07 04:39:21.037506 openai_function_calling-1.1.0/openai_function_calling/parameter.py
+-rw-r--r--   0        0        0        0 2023-06-28 04:20:47.916908 openai_function_calling-1.1.0/openai_function_calling/py.typed
+-rw-r--r--   0        0        0      759 2023-07-07 04:39:29.301304 openai_function_calling-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4055 1970-01-01 00:00:00.000000 openai_function_calling-1.1.0/PKG-INFO
```

### Comparing `openai_function_calling-1.0.1/README.md` & `openai_function_calling-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -12,48 +12,80 @@
 pip install openai-function-calling
 ```
 
 **The openai-function-calling package does come with the openai package. It must be installed separately with `pip install openai`**
 
 ## Usage
 
+### Auto-Infer the Function Definition (Beta)
+
+Automatically infer your function name, description, and parameters given a reference to the function. A `Function` instance is returned which can be converted to JSON schema with `.to_json_schema()` and then passed to the OpenAI chat completion API:
+
+```python
+def get_current_weather(location: str, unit: str) -> str:
+    """Get the current weather and return a summary."""
+    return f"It is currently sunny in {location} and 75 degrees {unit}."
+
+get_current_weather_json_schema = Function.from_function(get_current_weather).to_json_schema()
+
+# Get the function to call from ChatGPT (you would normally have more than one).
+response = openai.ChatCompletion.create(
+    model="gpt-3.5-turbo-0613",
+    messages=[
+        {
+            "role": "user",
+            "content": "What will the weather be like in Boston, MA today?",
+        }
+    ],
+    functions=[get_current_weather_json_schema],
+)
+```
+
+### Define Functions with Objects
+
+Define your function definitions using typed classes `Function` and `Parameter` which automatically convert to JSON schema with `.to_json_schema` methods. See an example below:
+
 ```python
 from openai_function_calling import Function, FunctionDict, Parameter, JsonSchemaType
 
+
 def get_current_weather(location: str, unit: str) -> str:
-  # Do some stuff here...
+    """Do some stuff in here."""
 
-# Define the function parameters.
-location_parameter = Parameter(
-    name="location",
-    type=JsonSchemaType.STRING,
-    description="The city and state, e.g. San Francisco, CA"
-)
-unit_parameter = Parameter(
-    name="unit",
-    type=JsonSchemaType.STRING,
-    description="The temperature unit to use.",
-    enum=["celsius", "fahrenheit"]
-)
 
 # Define the function.
 get_current_weather_function = Function(
     "get_current_weather",
     "Get the current weather",
-    [location_parameter, unit_parameter],
+    [
+        Parameter(
+            name="location",
+            type=JsonSchemaType.STRING,
+            description="The city and state, e.g. San Francisco, CA",
+        ),
+        Parameter(
+            name="unit",
+            type=JsonSchemaType.STRING,
+            description="The temperature unit to use.",
+            enum=["celsius", "fahrenheit"],
+        ),
+    ],
 )
 
 # Convert to a JSON schema dict to send to OpenAI.
 get_current_weather_function_dict = get_current_weather_function.to_json_schema()
 
 # Get the function to call from ChatGPT.
 response = openai.ChatCompletion.create(
     model="gpt-3.5-turbo-0613",
     messages=[
-      {"role": "user", "content": "What will the weather be like in Boston, MA tomorrow?"}
+        {
+            "role": "user",
+            "content": "What will the weather be like in Boston, MA tomorrow?",
+        }
     ],
     functions=[get_current_weather_function_dict],
 )
 ```
 
 ## Examples
```

### Comparing `openai_function_calling-1.0.1/pyproject.toml` & `openai_function_calling-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [tool.poetry]
 name = "openai-function-calling"
-version = "1.0.1"
+version = "1.1.0"
 description = "Helper functions to generate OpenAI GPT function calling requests."
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_function_calling"}]
 include = ["openai_function_calling/py.typed"]
+repository = "https://github.com/jakecyr/openai-function-calling"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <=3.12"
 typing-extensions = "^4.0"
+docstring-parser = "^0.15"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 openai = "^0.27.8"
 black = "^23.3.0"
 pytest = "^7.4.0"
 ruff = "~0.0.275"
 coverage = "^7.2.7"
```

