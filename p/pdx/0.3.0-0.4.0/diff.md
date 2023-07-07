# Comparing `tmp/pdx-0.3.0.tar.gz` & `tmp/pdx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdx-0.3.0.tar", max compression
+gzip compressed data, was "pdx-0.4.0.tar", max compression
```

## Comparing `pdx-0.3.0.tar` & `pdx-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.3.0/LICENSE
--rw-r--r--   0        0        0      147 2023-06-17 06:12:09.825905 pdx-0.3.0/README.md
--rw-r--r--   0        0        0      832 2023-07-02 16:26:51.942285 pdx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-02 10:21:05.627006 pdx-0.3.0/src/pdx/__init__.py
--rw-r--r--   0        0        0     1655 2023-07-02 10:40:15.375462 pdx-0.3.0/src/pdx/agent/__init__.py
--rw-r--r--   0        0        0     2843 2023-07-02 10:40:49.397512 pdx-0.3.0/src/pdx/agent/completer.py
--rw-r--r--   0        0        0     4155 2023-06-17 06:01:30.639029 pdx-0.3.0/src/pdx/agent/config.py
--rw-r--r--   0        0        0     1971 2023-07-02 10:37:06.519366 pdx-0.3.0/src/pdx/agent/metadata.py
--rw-r--r--   0        0        0     5005 2023-06-17 06:01:28.170575 pdx-0.3.0/src/pdx/agent/prompt.py
--rw-r--r--   0        0        0     2036 2023-06-17 06:00:09.706566 pdx-0.3.0/src/pdx/agent/prompt_session.py
--rw-r--r--   0        0        0     1894 2023-06-17 06:01:26.871641 pdx-0.3.0/src/pdx/agent/templater.py
--rw-r--r--   0        0        0     1965 2023-07-02 13:36:16.141378 pdx-0.3.0/src/pdx/agent/tester.py
--rw-r--r--   0        0        0     1746 2023-07-02 10:42:19.914775 pdx-0.3.0/src/pdx/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.3.0/src/pdx/commands/__init__.py
--rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.3.0/src/pdx/commands/create.py
--rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.3.0/src/pdx/exceptions.py
--rw-r--r--   0        0        0     2162 2023-06-17 06:03:02.108872 pdx-0.3.0/src/pdx/logger.py
--rw-r--r--   0        0        0     1951 2023-06-17 06:01:22.481929 pdx-0.3.0/src/pdx/models/__init__.py
--rw-r--r--   0        0        0     2913 2023-07-02 10:45:38.216714 pdx-0.3.0/src/pdx/models/anthropic/__init__.py
--rw-r--r--   0        0        0     4202 2023-06-17 06:01:17.123209 pdx-0.3.0/src/pdx/models/anthropic/client.py
--rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.3.0/src/pdx/models/anthropic/constants.py
--rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.3.0/src/pdx/models/anthropic/exceptions.py
--rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.3.0/src/pdx/models/api_client.py
--rw-r--r--   0        0        0      478 2023-06-17 06:00:09.711427 pdx-0.3.0/src/pdx/models/metadata.py
--rw-r--r--   0        0        0     4639 2023-07-02 10:45:47.318103 pdx-0.3.0/src/pdx/models/openai/__init__.py
--rw-r--r--   0        0        0     2892 2023-06-17 06:01:10.182094 pdx-0.3.0/src/pdx/models/openai/client.py
--rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.3.0/src/pdx/models/openai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.3.0/src/pdx/models/utils.py
--rw-r--r--   0        0        0      252 2023-06-17 06:00:09.713261 pdx-0.3.0/src/pdx/settings.py
--rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.3.0/src/pdx/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.3.0/src/pdx/templates/simple/Readme.md
--rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.3.0/src/pdx/templates/simple/__init__.py
--rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.3.0/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
--rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.3.0/src/pdx/templates/simple/templates/1_prompt.jinja
--rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.3.0/src/pdx/templates/simple/tests/test_1.yaml
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.3.0/src/pdx/utils/__init__.py
--rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.3.0/src/pdx/utils/rw.py
--rw-r--r--   0        0        0       22 2023-07-02 16:26:56.721767 pdx-0.3.0/src/pdx/version.py
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pdx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1676 2023-07-04 20:25:52.208721 pdx-0.4.0/README.md
+-rw-r--r--   0        0        0      832 2023-07-07 16:24:08.269082 pdx-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-02 10:21:05.627006 pdx-0.4.0/src/pdx/__init__.py
+-rw-r--r--   0        0        0     1655 2023-07-02 10:40:15.375462 pdx-0.4.0/src/pdx/agent/__init__.py
+-rw-r--r--   0        0        0     2843 2023-07-02 10:40:49.397512 pdx-0.4.0/src/pdx/agent/completer.py
+-rw-r--r--   0        0        0     4155 2023-06-17 06:01:30.639029 pdx-0.4.0/src/pdx/agent/config.py
+-rw-r--r--   0        0        0     1971 2023-07-02 10:37:06.519366 pdx-0.4.0/src/pdx/agent/metadata.py
+-rw-r--r--   0        0        0     5005 2023-06-17 06:01:28.170575 pdx-0.4.0/src/pdx/agent/prompt.py
+-rw-r--r--   0        0        0     2036 2023-06-17 06:00:09.706566 pdx-0.4.0/src/pdx/agent/prompt_session.py
+-rw-r--r--   0        0        0     1894 2023-06-17 06:01:26.871641 pdx-0.4.0/src/pdx/agent/templater.py
+-rw-r--r--   0        0        0     1965 2023-07-02 13:36:16.141378 pdx-0.4.0/src/pdx/agent/tester.py
+-rw-r--r--   0        0        0     1746 2023-07-02 10:42:19.914775 pdx-0.4.0/src/pdx/cli.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.4.0/src/pdx/commands/__init__.py
+-rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.4.0/src/pdx/commands/create.py
+-rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.4.0/src/pdx/exceptions.py
+-rw-r--r--   0        0        0     2162 2023-06-17 06:03:02.108872 pdx-0.4.0/src/pdx/logger.py
+-rw-r--r--   0        0        0     1951 2023-06-17 06:01:22.481929 pdx-0.4.0/src/pdx/models/__init__.py
+-rw-r--r--   0        0        0     2913 2023-07-02 10:45:38.216714 pdx-0.4.0/src/pdx/models/anthropic/__init__.py
+-rw-r--r--   0        0        0     4202 2023-06-17 06:01:17.123209 pdx-0.4.0/src/pdx/models/anthropic/client.py
+-rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.4.0/src/pdx/models/anthropic/constants.py
+-rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.4.0/src/pdx/models/anthropic/exceptions.py
+-rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.4.0/src/pdx/models/api_client.py
+-rw-r--r--   0        0        0      478 2023-06-17 06:00:09.711427 pdx-0.4.0/src/pdx/models/metadata.py
+-rw-r--r--   0        0        0     4639 2023-07-02 10:45:47.318103 pdx-0.4.0/src/pdx/models/openai/__init__.py
+-rw-r--r--   0        0        0     2892 2023-06-17 06:01:10.182094 pdx-0.4.0/src/pdx/models/openai/client.py
+-rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.4.0/src/pdx/models/openai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.4.0/src/pdx/models/utils.py
+-rw-r--r--   0        0        0      252 2023-06-17 06:00:09.713261 pdx-0.4.0/src/pdx/settings.py
+-rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.4.0/src/pdx/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.4.0/src/pdx/templates/simple/Readme.md
+-rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.4.0/src/pdx/templates/simple/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.4.0/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
+-rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.4.0/src/pdx/templates/simple/templates/1_prompt.jinja
+-rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.4.0/src/pdx/templates/simple/tests/test_1.yaml
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.4.0/src/pdx/utils/__init__.py
+-rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.4.0/src/pdx/utils/rw.py
+-rw-r--r--   0        0        0       22 2023-07-02 16:26:56.721767 pdx-0.4.0/src/pdx/version.py
+-rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 pdx-0.4.0/PKG-INFO
```

### Comparing `pdx-0.3.0/LICENSE` & `pdx-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/pyproject.toml` & `pdx-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdx"
-version = "0.3.0"
+version = "0.4.0"
 description = "Prompt Engineering and Dev-Ops toolkits. A faster way to build and manage applications powered by Language Models."
 keywords = ["prompt", "LLM", "prompt engineering", "dev-ops", "observability", "apps"]
 authors = ["Adithya Krishnan <krishsandeep@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "pdx", from = "src"}]
```

### Comparing `pdx-0.3.0/src/pdx/agent/__init__.py` & `pdx-0.4.0/src/pdx/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/agent/completer.py` & `pdx-0.4.0/src/pdx/agent/completer.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/agent/config.py` & `pdx-0.4.0/src/pdx/agent/config.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/agent/metadata.py` & `pdx-0.4.0/src/pdx/agent/metadata.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/agent/prompt.py` & `pdx-0.4.0/src/pdx/agent/prompt.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/agent/prompt_session.py` & `pdx-0.4.0/src/pdx/agent/prompt_session.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/agent/templater.py` & `pdx-0.4.0/src/pdx/agent/templater.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/agent/tester.py` & `pdx-0.4.0/src/pdx/agent/tester.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/cli.py` & `pdx-0.4.0/src/pdx/cli.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/commands/create.py` & `pdx-0.4.0/src/pdx/commands/create.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/exceptions.py` & `pdx-0.4.0/src/pdx/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/logger.py` & `pdx-0.4.0/src/pdx/logger.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/__init__.py` & `pdx-0.4.0/src/pdx/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/anthropic/__init__.py` & `pdx-0.4.0/src/pdx/models/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/anthropic/client.py` & `pdx-0.4.0/src/pdx/models/anthropic/client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/anthropic/exceptions.py` & `pdx-0.4.0/src/pdx/models/anthropic/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/api_client.py` & `pdx-0.4.0/src/pdx/models/api_client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/openai/__init__.py` & `pdx-0.4.0/src/pdx/models/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/openai/client.py` & `pdx-0.4.0/src/pdx/models/openai/client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/models/openai/exceptions.py` & `pdx-0.4.0/src/pdx/models/openai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.3.0/src/pdx/utils/rw.py` & `pdx-0.4.0/src/pdx/utils/rw.py`

 * *Files identical despite different names*

