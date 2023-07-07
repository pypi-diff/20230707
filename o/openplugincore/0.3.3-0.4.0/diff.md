# Comparing `tmp/openplugincore-0.3.3.tar.gz` & `tmp/openplugincore-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugincore-0.3.3.tar", last modified: Sat Jul  1 19:33:22 2023, max compression
+gzip compressed data, was "openplugincore-0.4.0.tar", last modified: Thu Jul  6 05:30:46 2023, max compression
```

## Comparing `openplugincore-0.3.3.tar` & `openplugincore-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.414908 openplugincore-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-01 19:33:22.410908 openplugincore-0.3.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.410908 openplugincore-0.3.3/openplugincore/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/openplugincore.py
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/plugins.json
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.410908 openplugincore-0.3.3/openplugincore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 19:33:22.414908 openplugincore-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-01 19:33:07.000000 openplugincore-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.410908 openplugincore-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/test_basicTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:30:46.755294 openplugincore-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-06 05:30:46.755294 openplugincore-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:30:46.751294 openplugincore-0.4.0/openplugincore/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 05:30:37.000000 openplugincore-0.4.0/openplugincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-06 05:30:37.000000 openplugincore-0.4.0/openplugincore/openplugincore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 05:30:37.000000 openplugincore-0.4.0/openplugincore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:30:46.751294 openplugincore-0.4.0/openplugincore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-06 05:30:46.000000 openplugincore-0.4.0/openplugincore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-06 05:30:46.000000 openplugincore-0.4.0/openplugincore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:30:46.000000 openplugincore-0.4.0/openplugincore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 05:30:46.000000 openplugincore-0.4.0/openplugincore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 05:30:46.000000 openplugincore-0.4.0/openplugincore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:30:46.755294 openplugincore-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-06 05:30:37.000000 openplugincore-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:30:46.751294 openplugincore-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:30:37.000000 openplugincore-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-06 05:30:37.000000 openplugincore-0.4.0/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-06 05:30:37.000000 openplugincore-0.4.0/tests/test_basicTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-06 05:30:37.000000 openplugincore-0.4.0/tests/test_e2e.py
```

### Comparing `openplugincore-0.3.3/PKG-INFO` & `openplugincore-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.3.3
+Version: 0.4.0
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.3.3/openplugincore/openplugincore.py` & `openplugincore-0.4.0/openplugincore/openplugincore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from urllib.error import HTTPError
 import requests
 from typing import Any, List, Dict, Union, Tuple, Callable
 import os
 from .types import ChatgptAssistantMessage, ChatgptFunctionMessage, PluginConfigs
 from langchain.chains.openai_functions.openapi import openapi_spec_to_openai_fn
 from langchain.utilities.openapi import OpenAPISpec
 from langchain.output_parsers.openai_functions import JsonOutputFunctionsParser
@@ -52,38 +53,46 @@
             function_response
         ]
     }
     summarize = openai.ChatCompletion.create(**all_chatgpt_args)
     return summarize
 
 class OpenPlugin:
-    def __init__(self, plugin_name: str, openai_api_key: str = None, root_url: str = None, verbose: bool = False):
+    def __init__(self, plugin_name: str = None, openai_api_key: str = None, root_url: str = None, verbose: bool = False):
         self.name: str = plugin_name
         self.root_url: str = root_url
         self.description: str = None
         self.manifest: Any = None
         self.functions: List[Dict[str, Any]] = None
         self.call_api_fn: Callable = None
         self.verbose: bool = verbose
-
+        if self.name is None and self.root_url is None:
+            raise ValueError("Either plugin_name or root_url must be passed in as a parameter")
         if openai_api_key is None:
             openai_api_key = os.getenv('OPENAI_API_KEY')
             if openai_api_key is None:
                 raise ValueError("OPENAI_API_KEY not found. You can pass in the parameter openai_api_key. You can also set the environment variable OPENAI_API_KEY=<API-KEY>.")
         os.environ["OPENAI_API_KEY"] = openai_api_key
         openai.api_key = openai_api_key
         self.init(plugin_name)
-        self.name: str = self.manifest["name_for_model"]
         self.description: str = self.manifest["description_for_model"]
 
-    def init(self, plugin_name: str) -> None:
+    def init(self, plugin_name: str = None) -> None:
         base_dir = os.path.dirname(os.path.realpath(__file__))
         plugins_file_path = os.path.join(base_dir, "plugins.json")
-        with open(plugins_file_path) as f:
-            plugins = json.load(f)
+        
+        # fetch plugins from github
+        try:
+            plugins_url = "https://raw.githubusercontent.com/CakeCrusher/openplugin/main/migrations/plugin_store/openplugins.json"
+            response = requests.get(plugins_url)
+            response.raise_for_status()
+            plugins = response.json()
+        except Exception as e:
+            raise HTTPError(f"Unable to fetch plugins from github url '{plugins_url}'")
+    
         # if self.root_url has a value
         if self.root_url is None:
             try:
                 self.root_url = plugins[plugin_name]
             except KeyError:
                 # throw error
                 raise KeyError("Plugin not found")
@@ -93,14 +102,16 @@
     def fetch_manifest(self, root_url: str) -> Any:
         if plugin_configs.get(self.name, {}).get("manifest", None) is not None:
             return plugin_configs[self.name]["manifest"]
         
         response = requests.get(root_url + "/.well-known/ai-plugin.json")
         response.raise_for_status()  # Raise exception if the request failed
         manifest = response.json()
+        if not self.name:
+            self.name: str = manifest["name_for_model"]
         if self.verbose:
             print(f"\"{self.name}\" manifest: ", json.dumps(manifest, indent=2))
 
         # add manifest to plugin_configs
         plugin_configs[self.name] = {
             **plugin_configs.get(self.name, {}),
             "manifest": manifest
@@ -111,14 +122,15 @@
         openapi_url = manifest.get("api", {}).get("url")
         if self.verbose:
             print(f"\"{self.name}\" openapi_url: ", openapi_url)
         if openapi_url == None:
             raise ValueError("OpenAPI URL not found in manifest")
         if isinstance(openapi_url, Union[OpenAPISpec, str]):
             for conversion in (
+                # each of the below specs can get stuck in a while loop
                 OpenAPISpec.from_url,
                 OpenAPISpec.from_file,
                 OpenAPISpec.from_text,
             ):
                 try:
                     openapi_url = conversion(openapi_url)  # type: ignore[arg-type]
                     break
@@ -204,8 +216,8 @@
         try:
             return ChatgptFunctionMessage(
                 role="function",
                 name=llm_chain_out["name"],
                 content=json.dumps(json_response)
             )
         except json.decoder.JSONDecodeError:
-            raise json.decoder.JSONDecodeError(f"API call failed, API returned the following non-JSON response:\n{json_response.content}")
+            raise json.decoder.JSONDecodeError(f"API call failed, API returned the following non-JSON response:\n{response.content}")
```

### Comparing `openplugincore-0.3.3/openplugincore/types.py` & `openplugincore-0.4.0/openplugincore/types.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.3.3/openplugincore.egg-info/PKG-INFO` & `openplugincore-0.4.0/openplugincore.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.3.3
+Version: 0.4.0
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.3.3/setup.py` & `openplugincore-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugincore', 
-        version="0.3.3",
+        version="0.4.0",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         packages=find_packages(),
         package_data={
             "openplugincore": ["*.json"],  # include all .json files in the openplugin package
```

### Comparing `openplugincore-0.3.3/tests/mock_data.py` & `openplugincore-0.4.0/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.3.3/tests/test_basicTest.py` & `openplugincore-0.4.0/tests/test_basicTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import requests
 from dotenv import load_dotenv
 load_dotenv()
 
 OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
 
 def test_initiate_todo_with_url():
-    plugin = OpenPlugin("NA", root_url="http://localhost:3333")
+    plugin = OpenPlugin(root_url="http://localhost:3333")
     assert plugin.manifest is not None
     assert plugin.manifest.get("name_for_model") == "todo"
 
 @pytest.fixture
 def todo_openplugin():
     plugin = OpenPlugin("__testing__")
     return plugin
```

### Comparing `openplugincore-0.3.3/tests/test_e2e.py` & `openplugincore-0.4.0/tests/test_e2e.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,32 +51,14 @@
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
     # # ensure that the json_content has a key of image_url and that is starts with https://lgtm.lol
     assert "image_url" in json_content
     assert json_content["image_url"].startswith("https://lgtm.lol")
 
-if False: # server too inconsistent
-    def test_initiate_and_fetch_Figlet():
-        plugin = OpenPlugin("Figlet")
-        assert plugin.manifest is not None
-
-        # create chatgpt request that will call the addTodo function
-        chatgpt_prompt = 'Convert "Testing" to the Doom ASCII font.'
-        response = plugin.fetch_plugin(
-            prompt=chatgpt_prompt,
-            model="gpt-3.5-turbo-0613",
-            temperature=0,
-        )
-
-        assert response is not None
-        assert response["role"] == "function"
-
-        json_content = json.loads(response["content"])
-        assert json_content["font"] == "doom"
 
 def test_initiate_and_fetch_yt_caption_retriever():
     plugin = OpenPlugin("yt_caption_retriever")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'give me a 2 sentence summary of the following yt video https://www.youtube.com/watch?v=P310I19L3Ko'
@@ -165,55 +147,14 @@
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
 
     # Replace the line below with a test for the final output in json_content
     assert isinstance(json_content["blog"], str)
 
-def test_initiate_and_fetch_socialsearch():
-    plugin = OpenPlugin("socialsearch")
-    assert plugin.manifest is not None
-    print("plugin.manifest: ", json.dumps(plugin.manifest, indent=2))
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'show me elon musk latest tweet'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        verbose=True,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["message"], str)
-
-if False: # unable to convert url
-    def test_initiate_and_fetch_show_me_diagrams():
-        plugin = OpenPlugin("show_me_diagrams")
-        plugin.verbose = True
-        assert plugin.manifest is not None
-
-        # create chatgpt request that will call the addTodo function
-        chatgpt_prompt = 'make a diagram of one node connected to two others that will be yes or no'
-        response = plugin.fetch_plugin(
-            prompt=chatgpt_prompt,
-            model="gpt-3.5-turbo-0613",
-            temperature=0,
-        )
-
-        assert response is not None
-        assert response["role"] == "function"
-        json_content = json.loads(response["content"])
-
-        # Replace the line below with a test for the final output in json_content
-        assert isinstance(json_content["results"][0]["image"], str)
-
 def test_initiate_and_fetch_scholarai():
     plugin = OpenPlugin("scholarai")
     assert plugin.manifest is not None
 
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'What scientific research exists for semantic representation of language through brain waves. dont sort.'
```

