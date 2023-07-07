# Comparing `tmp/langchain_interpreter-0.0.5.tar.gz` & `tmp/langchain_interpreter-0.0.6.tar.gz`

## Comparing `langchain_interpreter-0.0.5.tar` & `langchain_interpreter-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/Makefile
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/conf.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/index.rst
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/langchain_interpreter.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/make.bat
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/modules.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/requirements.txt
--rw-r--r--   0        0        0    17907 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/examples/chains_from_json.ipynb
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/examples/json_from_chains.ipynb
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/examples/validation.ipynb
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/conv_buffer_memory.json
--rwxr-xr-x   0        0        0      403 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/llmchain.json
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/seq_chain.json
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/seq_chain_memory.json
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/simple_seq_chain.json
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/langchain_interpreter/__init__.py
--rwxr-xr-x   0        0        0     4767 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/langchain_interpreter/main.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/langchain_interpreter/validation.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/LICENSE
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/index.rst
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/langchain_interpreter.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/modules.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/requirements.txt
+-rw-r--r--   0        0        0    17907 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/examples/chains_from_json.ipynb
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/examples/json_from_chains.ipynb
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/examples/validation.ipynb
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/conv_buffer_memory.json
+-rwxr-xr-x   0        0        0      403 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/llmchain.json
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/seq_chain.json
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/seq_chain_memory.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/simple_seq_chain.json
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/langchain_interpreter/__init__.py
+-rwxr-xr-x   0        0        0     4785 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/langchain_interpreter/main.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/langchain_interpreter/validation.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/LICENSE
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/PKG-INFO
```

### Comparing `langchain_interpreter-0.0.5/.readthedocs.yaml` & `langchain_interpreter-0.0.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/docs/Makefile` & `langchain_interpreter-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/docs/conf.py` & `langchain_interpreter-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/docs/index.rst` & `langchain_interpreter-0.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/docs/langchain_interpreter.rst` & `langchain_interpreter-0.0.6/docs/langchain_interpreter.rst`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/docs/make.bat` & `langchain_interpreter-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/src/examples/chains_from_json.ipynb` & `langchain_interpreter-0.0.6/src/examples/chains_from_json.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/src/examples/json_from_chains.ipynb` & `langchain_interpreter-0.0.6/src/examples/json_from_chains.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/src/examples/validation.ipynb` & `langchain_interpreter-0.0.6/src/examples/validation.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/src/json/seq_chain.json` & `langchain_interpreter-0.0.6/src/json/seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/src/json/seq_chain_memory.json` & `langchain_interpreter-0.0.6/src/json/seq_chain_memory.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/src/json/simple_seq_chain.json` & `langchain_interpreter-0.0.6/src/json/simple_seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/src/langchain_interpreter/main.py` & `langchain_interpreter-0.0.6/src/langchain_interpreter/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,30 +23,30 @@
     Raises:
         ValidationError:
     """
 
     with open(filename) as f:
         cfg = json.load(f)
     validate_chain(cfg)
-    return get_chain(cfg, **kwargs)
+    return get_chain(cfg["chain"], **kwargs)
 
 
 def chain_from_str(s, **kwargs):
     """Generate a LangChain Chain from a json string.
 
     Args:
         s (str): the json string to turn into a chain
 
     Returns:
         chain: the chain specified by the json template.
     """
 
     cfg = json.loads(s)
     validate_chain(cfg)
-    return get_chain(cfg, **kwargs)
+    return get_chain(cfg["chain"], **kwargs)
 
 
 def get_chain(cfg, **kwargs):
     if cfg["type"] == "LLMChain":
         return get_llm_chain(cfg, **kwargs)
     if cfg["type"] == "SimpleSequentialChain":
         return get_simple_sequential_chain(cfg, **kwargs)
```

### Comparing `langchain_interpreter-0.0.5/src/langchain_interpreter/validation.py` & `langchain_interpreter-0.0.6/src/langchain_interpreter/validation.py`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/.gitignore` & `langchain_interpreter-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/LICENSE` & `langchain_interpreter-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/README.md` & `langchain_interpreter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.5/pyproject.toml` & `langchain_interpreter-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "langchain_interpreter"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Elijah Tarr", email="elijahotarr@gmail.com" },
 ]
 description = "A way to turn json into langchain pipelines."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `langchain_interpreter-0.0.5/PKG-INFO` & `langchain_interpreter-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_interpreter
-Version: 0.0.5
+Version: 0.0.6
 Summary: A way to turn json into langchain pipelines.
 Project-URL: Homepage, https://github.com/eoriont/langchain_interpreter
 Project-URL: Bug Tracker, https://github.com/eoriont/langchain_interpreter/issues
 Author-email: Elijah Tarr <elijahotarr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

