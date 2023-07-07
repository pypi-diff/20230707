# Comparing `tmp/LLM-Toolbox-0.1.7.tar.gz` & `tmp/LLM-Toolbox-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.7.tar", last modified: Wed Jun 28 09:57:01 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.8.tar", last modified: Fri Jul  7 06:21:13 2023, max compression
```

## Comparing `LLM-Toolbox-0.1.7.tar` & `LLM-Toolbox-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-28 09:57:01.097065 LLM-Toolbox-0.1.7/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.7/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-28 09:57:01.087065 LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17184 2023-06-28 09:57:01.000000 LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-06-28 09:57:01.000000 LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-28 09:57:01.000000 LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-06-28 09:57:01.000000 LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-06-28 09:57:01.000000 LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-28 09:57:01.000000 LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17184 2023-06-28 09:57:01.097065 LLM-Toolbox-0.1.7/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16646 2023-06-28 09:54:05.000000 LLM-Toolbox-0.1.7/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-28 09:57:01.087065 LLM-Toolbox-0.1.7/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.7/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15872 2023-06-27 10:19:56.000000 LLM-Toolbox-0.1.7/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-28 09:57:01.087065 LLM-Toolbox-0.1.7/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-28 09:57:01.097065 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      831 2023-06-27 10:28:40.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/life.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-28 09:57:01.097065 LLM-Toolbox-0.1.7/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2173 2023-06-28 09:45:49.000000 LLM-Toolbox-0.1.7/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.8/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.676696 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16662 2023-06-28 10:02:44.000000 LLM-Toolbox-0.1.8/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.676696 LLM-Toolbox-0.1.8/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.8/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16246 2023-07-07 06:16:50.000000 LLM-Toolbox-0.1.8/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.676696 LLM-Toolbox-0.1.8/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      831 2023-06-27 10:28:40.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/life.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2173 2023-07-07 06:20:12.000000 LLM-Toolbox-0.1.8/setup.py
```

### Comparing `LLM-Toolbox-0.1.7/LICENSE` & `LLM-Toolbox-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.7
+Version: 0.1.8
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -36,15 +36,15 @@
     1. [Current Costs](#current-costs)
 1. [Installation](#installation)
     1. [pip](#pip)
     1. [`pipx`, the Easy Way](#pipx-the-easy-way)
     1. [Installing the LLM-Toolbox](#installing-the-llm-toolbox)
     1. [Cloning the LLM-Toolbox Repository](#cloning-the-llm-toolbox-repository)
 1. [Getting Started](#getting-started)
-    1. [Set your OpenAI API key](#set-your-openai-api-key)
+    1. [Configuring your OpenAI API key](#configuring-your-openai-api-key)
 1. [Tools](#tools)
     1. [LMT](#lmt)
     1. [ShellGenius](#shellgenius)
     1. [Commitgen](#commitgen)
     1. [Codereview](#codereview)
     1. [VocabMaster](#vocabmaster)
     1. [Thesaurus](#thesaurus)
```

### Comparing `LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/SOURCES.txt` & `LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/PKG-INFO` & `LLM-Toolbox-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.7
+Version: 0.1.8
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -36,15 +36,15 @@
     1. [Current Costs](#current-costs)
 1. [Installation](#installation)
     1. [pip](#pip)
     1. [`pipx`, the Easy Way](#pipx-the-easy-way)
     1. [Installing the LLM-Toolbox](#installing-the-llm-toolbox)
     1. [Cloning the LLM-Toolbox Repository](#cloning-the-llm-toolbox-repository)
 1. [Getting Started](#getting-started)
-    1. [Set your OpenAI API key](#set-your-openai-api-key)
+    1. [Configuring your OpenAI API key](#configuring-your-openai-api-key)
 1. [Tools](#tools)
     1. [LMT](#lmt)
     1. [ShellGenius](#shellgenius)
     1. [Commitgen](#commitgen)
     1. [Codereview](#codereview)
     1. [VocabMaster](#vocabmaster)
     1. [Thesaurus](#thesaurus)
```

### Comparing `LLM-Toolbox-0.1.7/README.md` & `LLM-Toolbox-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     1. [Current Costs](#current-costs)
 1. [Installation](#installation)
     1. [pip](#pip)
     1. [`pipx`, the Easy Way](#pipx-the-easy-way)
     1. [Installing the LLM-Toolbox](#installing-the-llm-toolbox)
     1. [Cloning the LLM-Toolbox Repository](#cloning-the-llm-toolbox-repository)
 1. [Getting Started](#getting-started)
-    1. [Set your OpenAI API key](#set-your-openai-api-key)
+    1. [Configuring your OpenAI API key](#configuring-your-openai-api-key)
 1. [Tools](#tools)
     1. [LMT](#lmt)
     1. [ShellGenius](#shellgenius)
     1. [Commitgen](#commitgen)
     1. [Codereview](#codereview)
     1. [VocabMaster](#vocabmaster)
     1. [Thesaurus](#thesaurus)
```

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.8/llm_toolbox/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import os
-import re
-import requests
 import shutil
 import subprocess
 import sys
 import tempfile
+import requests
 from datetime import datetime
 from functools import wraps
 from pathlib import Path
 
 import click
 import validators
 from strip_tags.lib import strip_tags
@@ -24,18 +23,18 @@
     """
     dest_path = Path.home() / ".config/lmt/templates"
     dest_path.mkdir(parents=True, exist_ok=True)
 
     config_file = Path.home() / ".config/lmt/config.json"
     config_file.touch(exist_ok=True)
 
-    # Load existing config if it exists, else start with empty dictionary
-    with config_file.open("r") as f:
+    # Load existing config if it exists, else create an empty config
+    with config_file.open("r") as file:
         try:
-            config = json.load(f)
+            config = json.load(file)
         except json.JSONDecodeError:
             click.echo(f"{click.style('Installing templates...', fg='yellow')}")
             config = {}
 
     src_path = Path(__file__).parent / "tools/templates"
     for file in src_path.glob("*.yaml"):
         destination = dest_path / file.name
@@ -48,58 +47,59 @@
             template_name = file.stem
             config[template_name] = str(dest_path / file.name)
             click.echo(
                 f"{click.style(f'Installed `{template_name}` template.', fg='green')}"
             )
 
     # Write the updated config back to the file
-    with config_file.open("w") as f:
-        json.dump(config, f, indent=4)
+    with config_file.open("w") as file:
+        json.dump(config, file, indent=4)
     print()
 
 
 install_templates()
 
 
 def validate_model_name(ctx, param, value):
     """
     Validates the model name parameter.
     """
     model_name = value.lower()
     if model_name in VALID_MODELS:
         return VALID_MODELS[model_name]
-    elif model_name in VALID_MODELS.values():
+
+    if model_name in VALID_MODELS.values():
         return model_name
-    else:
+
+    if not any(model_name in items for items in VALID_MODELS.items()):
         raise click.BadParameter(f"Invalid model: {model_name}")
 
 
 def validate_temperature(ctx, param, value):
     """
     Validates the temperature parameter.
     """
     if 0 <= value <= 2:
         return value
-    else:
-        raise click.BadParameter("Temperature must be between 0 and 2.")
+    raise click.BadParameter("Temperature must be between 0 and 2.")
 
 
 @click.group()
 @click.pass_context
 @click.version_option()
 def cli():
     pass
 
 
-def common_options(f):
+def common_options(function):
     """
     Common options for all commands.
     """
 
-    @wraps(f)
+    @wraps(function)
     @click.option("--emoji", is_flag=True, help="Add emotions and emojis.")
     @click.option(
         "-m",
         "--model",
         default="gpt-3.5-turbo",
         help="The model to use for the requests.",
         callback=validate_model_name,
@@ -136,15 +136,15 @@
     @click.option(
         "--debug",
         is_flag=True,
         default=False,
         help="Print debug information.",
     )
     def wrapper(*args, **kwargs):
-        return f(*args, **kwargs)
+        return function(*args, **kwargs)
 
     return wrapper
 
 
 @cli.command()
 @click.argument("words", nargs=-1, required=False)
 @click.pass_context
@@ -295,15 +295,14 @@
     except IndexError as error:
         click.echo(f"{click.style('Error occurred: {error}', fg='red')}", err=True)
         return
     except TypeError:
         click.echo("No commit message generated. Aborting commit.")
         return
 
-
     # Clean `^M` characters
     commit_message = commit_message.replace("\r", "")
 
     click.echo("\n---\n")
 
     choice = click.prompt(
         "Do you want to use this commit message? (yes/edit/no)",
@@ -528,45 +527,53 @@
         raw,
         debug,
     )
 
 
 @cli.command()
 @click.pass_context
+@click.option("--reset", is_flag=True, help="Reset the template file.")
 @common_options
-def life(ctx, model, emoji, temperature, tokens, no_stream, raw, debug):
+def life(ctx, reset, model, emoji, temperature, tokens, no_stream, raw, debug):
     """
     Comment on the remaining lifespan of a person.
     """
     template_file = get_template_content("life")
     user_info = template_file["user_info"]
 
-    if user_info["name"] is None:
+    if user_info["name"] is None or reset:
         user_name = click.prompt("What is your name?", type=str)
     else:
         user_name = user_info["name"]
 
-    if user_info["date_of_birth"] is None:
-        date_of_birth = click.prompt(
-            "What is your date of birth? (YYYY-MM-DD)", type=str
-        )
-    else:
-        date_of_birth = user_info["date_of_birth"]
+    while True:
+        try:
+            if user_info["date_of_birth"] is None or reset:
+                date_of_birth_str = click.prompt(
+                    "What is your date of birth? (YYYY-MM-DD)", type=str
+                )
+            else:
+                date_of_birth_str = user_info["date_of_birth"]
+            date_of_birth = datetime.strptime(date_of_birth_str, "%Y-%m-%d")
+
+        except ValueError:
+            click.echo("Please enter a valid date.")
+        else:
+            break
 
     life_expectancy = user_info["life_expectancy"]
     system = template_file["system"]
 
     # Update the template file
     template_file["user_info"]["name"] = user_name
-    template_file["user_info"]["date_of_birth"] = date_of_birth
+    template_file["user_info"]["date_of_birth"] = date_of_birth_str
     template_path = TEMPLATES_DIR / "life.yaml"
-    with open(template_path, "w") as outfile:
-        yaml.dump(template_file, outfile, default_flow_style=False)
+    with open(template_path, "w", encoding="UTF-8") as file:
+        yaml.dump(template_file, file, default_flow_style=False)
 
-    date_of_birth = datetime.strptime(user_info["date_of_birth"], "%Y-%m-%d")
     remaining_days = life_expectancy - (datetime.now() - date_of_birth).days
     percentage = f"{(remaining_days / life_expectancy) * 100:.2f}"
 
     system = f"{system}".format(
         user_name=user_name, remaining_days=remaining_days, percentage=percentage
     )
```

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/codereview.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/critique.yaml` & `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/critique.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/life.yaml` & `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/life.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.7/setup.py` & `LLM-Toolbox-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 from pathlib import Path
 import shutil
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

