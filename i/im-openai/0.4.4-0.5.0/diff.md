# Comparing `tmp/im_openai-0.4.4.tar.gz` & `tmp/im_openai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.4.4.tar", last modified: Sat Jul  1 00:14:12 2023, max compression
+gzip compressed data, was "im_openai-0.5.0.tar", last modified: Fri Jul  7 00:55:05 2023, max compression
```

## Comparing `im_openai-0.4.4.tar` & `im_openai-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-01 00:14:12.848961 im_openai-0.4.4/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.4.4/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.4.4/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.4.4/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.4.4/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3068 2023-07-01 00:14:12.849566 im_openai-0.4.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.4.4/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-01 00:14:12.803090 im_openai-0.4.4/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.4.4/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.4.4/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-01 00:14:12.818792 im_openai-0.4.4/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.4.4/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4746 2023-07-01 00:12:14.000000 im_openai-0.4.4/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2100 2023-06-30 20:10:17.000000 im_openai-0.4.4/im_openai/langchain_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3048 2023-06-30 23:20:06.000000 im_openai-0.4.4/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.4.4/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-01 00:14:12.839615 im_openai-0.4.4/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3068 2023-07-01 00:14:12.000000 im_openai-0.4.4/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-07-01 00:14:12.000000 im_openai-0.4.4/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-01 00:14:12.000000 im_openai-0.4.4/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-01 00:14:12.000000 im_openai-0.4.4/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-01 00:14:12.000000 im_openai-0.4.4/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-07-01 00:14:12.851485 im_openai-0.4.4/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-01 00:13:54.000000 im_openai-0.4.4/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-01 00:14:12.846886 im_openai-0.4.4/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.4.4/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.4.4/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.573552 im_openai-0.5.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.5.0/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.5.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.5.0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3128 2023-07-07 00:55:05.574272 im_openai-0.5.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.5.0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.493967 im_openai-0.5.0/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.5.0/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.516556 im_openai-0.5.0/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-06 21:35:09.000000 im_openai-0.5.0/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4746 2023-07-07 00:30:31.000000 im_openai-0.5.0/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8835 2023-07-07 00:33:17.000000 im_openai-0.5.0/im_openai/langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3353 2023-07-07 00:30:57.000000 im_openai-0.5.0/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.5.0/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.561558 im_openai-0.5.0/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3128 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-07-07 00:55:05.576660 im_openai-0.5.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-07 00:33:18.000000 im_openai-0.5.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.570632 im_openai-0.5.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.5.0/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.5.0/tests/test_im_openai.py
```

### Comparing `im_openai-0.4.4/CONTRIBUTING.rst` & `im_openai-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/LICENSE` & `im_openai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/PKG-INFO` & `im_openai-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.4.4
+Version: 0.5.0
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -118,9 +118,14 @@
 - pass along chat_id
 - attempt to auto-convert langchain prompt templates
 
 ## 0.4.4 (2023-06-30)
 
 - remove stray prints
 
+## 0.5.0 (2023-07-06)
+
+- Add langchain callbacks handlers
+
+
```

### Comparing `im_openai-0.4.4/README.md` & `im_openai-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/docs/Makefile` & `im_openai-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/docs/conf.py` & `im_openai-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/docs/installation.rst` & `im_openai-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/docs/make.bat` & `im_openai-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/im_openai/client.py` & `im_openai-0.5.0/im_openai/client.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/im_openai/patch.py` & `im_openai-0.5.0/im_openai/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,21 @@
         **kwargs
     ):
         if ip_project_key is None:
             ip_project_key = os.environ.get("PROMPT_PROJECT_KEY")
         if ip_project_key is None:
             return oldcreate(*args, **kwargs)
 
+        if "messages" in kwargs:
+            template_params = {}
+            for message in kwargs["messages"]:
+                if hasattr(message["content"], "template_args"):
+                    template_params.update(message["content"].template_args)
+            ip_template_params = template_params
+
         if ip_template_text is None and ip_template_chat is None:
             ip_template = get_prompt_template(*args, **kwargs)
             if isinstance(ip_template, str):
                 ip_template_text = ip_template
             elif isinstance(ip_template, list):
                 ip_template_chat = ip_template
```

### Comparing `im_openai-0.4.4/im_openai.egg-info/PKG-INFO` & `im_openai-0.5.0/im_openai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.4.4
+Version: 0.5.0
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -118,9 +118,14 @@
 - pass along chat_id
 - attempt to auto-convert langchain prompt templates
 
 ## 0.4.4 (2023-06-30)
 
 - remove stray prints
 
+## 0.5.0 (2023-07-06)
+
+- Add langchain callbacks handlers
+
+
```

### Comparing `im_openai-0.4.4/im_openai.egg-info/SOURCES.txt` & `im_openai-0.5.0/im_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.4/setup.py` & `im_openai-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.4.4",
+    version="0.5.0",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.4.4/tests/test_im_openai.py` & `im_openai-0.5.0/tests/test_im_openai.py`

 * *Files identical despite different names*

