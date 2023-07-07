# Comparing `tmp/biochatter-0.1.4.tar.gz` & `tmp/biochatter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biochatter-0.1.4.tar", max compression
+gzip compressed data, was "biochatter-0.1.5.tar", max compression
```

## Comparing `biochatter-0.1.4.tar` & `biochatter-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.4/LICENSE
--rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.4/biochatter/__init__.py
--rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.4/biochatter/_stats.py
--rw-r--r--   0        0        0    18229 2023-07-06 14:40:38.478751 biochatter-0.1.4/biochatter/llm_connect.py
--rw-r--r--   0        0        0     5839 2023-07-06 14:40:38.478959 biochatter-0.1.4/biochatter/podcast.py
--rw-r--r--   0        0        0     5788 2023-07-06 14:40:38.479205 biochatter-0.1.4/biochatter/vectorstore.py
--rw-r--r--   0        0        0      740 2023-07-06 14:40:38.480642 biochatter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 biochatter-0.1.4/setup.py
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 biochatter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.5/LICENSE
+-rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.5/biochatter/__init__.py
+-rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.5/biochatter/_stats.py
+-rw-r--r--   0        0        0    18302 2023-07-07 08:35:59.679816 biochatter-0.1.5/biochatter/llm_connect.py
+-rw-r--r--   0        0        0     5839 2023-07-06 14:40:38.478959 biochatter-0.1.5/biochatter/podcast.py
+-rw-r--r--   0        0        0     5788 2023-07-06 14:40:38.479205 biochatter-0.1.5/biochatter/vectorstore.py
+-rw-r--r--   0        0        0      740 2023-07-07 08:36:14.273345 biochatter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 biochatter-0.1.5/setup.py
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 biochatter-0.1.5/PKG-INFO
```

### Comparing `biochatter-0.1.4/LICENSE` & `biochatter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.4/biochatter/_stats.py` & `biochatter-0.1.5/biochatter/_stats.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.4/biochatter/llm_connect.py` & `biochatter-0.1.5/biochatter/llm_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.ca_messages = []
         self.current_statements = []
 
     def set_user_name(self, user_name: str):
         self.user_name = user_name
 
     @abstractmethod
-    def set_api_key(self, api_key: str):
+    def set_api_key(self, api_key: str, user: Optional[str] = None):
         pass
 
     def get_prompts(self):
         return self.prompts
 
     def set_prompts(self, prompts: dict):
         self.prompts = prompts
@@ -488,15 +488,15 @@
             docsum=docsum,
         )
 
         self.version = version
         self.base = base
         self.deployment_name = deployment_name
 
-    def set_api_key(self, api_key: str):
+    def set_api_key(self, api_key: str, user: Optional[str] = None):
         """
         Set the API key for the Azure API. If the key is valid, initialise the
         conversational agent. No user stats on Azure.
 
         Args:
             api_key (str): The API key for the Azure API.
 
@@ -545,15 +545,15 @@
             prompts=prompts,
             split_correction=split_correction,
             docsum=docsum,
         )
 
         self.messages = []
 
-    def set_api_key(self, api_key: str, user: str):
+    def set_api_key(self, api_key: str, user: Optional[str] = None):
         self.chat = HuggingFaceHub(
             repo_id=self.model_name,
             model_kwargs={"temperature": 1.0},  # "regular sampling"
             # as per https://huggingface.co/docs/api-inference/detailed_parameters
             huggingfacehub_api_token=api_key,
         )
```

### Comparing `biochatter-0.1.4/biochatter/podcast.py` & `biochatter-0.1.5/biochatter/podcast.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.4/biochatter/vectorstore.py` & `biochatter-0.1.5/biochatter/vectorstore.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.4/pyproject.toml` & `biochatter-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biochatter"
-version = "0.1.4"
+version = "0.1.5"
 description = "Backend library for conversational AI in biomedicine"
 authors = ["Sebastian Lobentanzer <sebastian.lobentanzer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `biochatter-0.1.4/setup.py` & `biochatter-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tiktoken>=0.4.0,<0.5.0']
 
 extras_require = \
 {'podcast': ['gTTS>=2.3.2,<3.0.0'], 'streamlit': ['streamlit>=1.23.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'biochatter',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Backend library for conversational AI in biomedicine',
     'long_description': '# biochatter\nThis repository contains the `biochatter` Python package, a generic backend library for the connection of biomedical applications to conversational AI. Used in [ChatGSE](https://chat.biocypher.org), which is being developed at https://github.com/biocypher/ChatGSE. More to come, so stay tuned!\n\n## Installation\nTo use the package, install it from PyPI, for instance using pip (`pip install biochatter`) or Poetry (`poetry add biochatter`).\n',
     'author': 'Sebastian Lobentanzer',
     'author_email': 'sebastian.lobentanzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `biochatter-0.1.4/PKG-INFO` & `biochatter-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biochatter
-Version: 0.1.4
+Version: 0.1.5
 Summary: Backend library for conversational AI in biomedicine
 License: MIT
 Author: Sebastian Lobentanzer
 Author-email: sebastian.lobentanzer@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

