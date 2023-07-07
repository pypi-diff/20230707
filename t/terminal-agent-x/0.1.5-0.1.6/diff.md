# Comparing `tmp/terminal-agent-x-0.1.5.tar.gz` & `tmp/terminal-agent-x-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal-agent-x-0.1.5.tar", last modified: Sun Jul  2 16:51:48 2023, max compression
+gzip compressed data, was "terminal-agent-x-0.1.6.tar", last modified: Fri Jul  7 09:43:08 2023, max compression
```

## Comparing `terminal-agent-x-0.1.5.tar` & `terminal-agent-x-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.5/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4099 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3217 2023-07-02 16:48:43.000000 terminal-agent-x-0.1.5/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      976 2023-07-02 16:41:45.000000 terminal-agent-x-0.1.5/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.646097 terminal-agent-x-0.1.5/terminal_agent_x/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.5/terminal_agent_x/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7077 2023-07-02 16:37:25.000000 terminal-agent-x-0.1.5/terminal_agent_x/tax.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4099 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      498 2023-06-06 16:47:27.000000 terminal-agent-x-0.1.5/tests/test.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 09:43:08.230202 terminal-agent-x-0.1.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.6/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3712 2023-07-07 09:43:08.230202 terminal-agent-x-0.1.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2830 2023-07-07 09:42:02.000000 terminal-agent-x-0.1.6/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      976 2023-07-07 09:36:02.000000 terminal-agent-x-0.1.6/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 09:43:08.230202 terminal-agent-x-0.1.6/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 09:43:08.230202 terminal-agent-x-0.1.6/terminal_agent_x/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.6/terminal_agent_x/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10029 2023-07-07 09:32:16.000000 terminal-agent-x-0.1.6/terminal_agent_x/tax.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 09:43:08.230202 terminal-agent-x-0.1.6/terminal_agent_x.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3712 2023-07-07 09:43:08.000000 terminal-agent-x-0.1.6/terminal_agent_x.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-07-07 09:43:08.000000 terminal-agent-x-0.1.6/terminal_agent_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 09:43:08.000000 terminal-agent-x-0.1.6/terminal_agent_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-07-07 09:43:08.000000 terminal-agent-x-0.1.6/terminal_agent_x.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-07-07 09:43:08.000000 terminal-agent-x-0.1.6/terminal_agent_x.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 09:43:08.230202 terminal-agent-x-0.1.6/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      498 2023-06-06 16:47:27.000000 terminal-agent-x-0.1.6/tests/test.py
```

### Comparing `terminal-agent-x-0.1.5/LICENSE` & `terminal-agent-x-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal-agent-x-0.1.5/PKG-INFO` & `terminal-agent-x-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.5
+Version: 0.1.6
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Project-URL: Wiki, https://github.com/LyuLumos/Terminal-Agent-X/wiki
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal-Agent-X
 
 [EN](README.md) / [中文](https://github.com/LyuLumos/Terminal-Agent-X/blob/main/README_cn.md) / [Wiki](https://github.com/LyuLumos/Terminal-Agent-X/wiki)
 
+## Features
+
+- 👻 Easy installation and usage with a single command.
+- 🎈 Small size, no additional dependencies required.
+- 🐼 Supports English and Chinese on Windows CMD, Powershell, Linux shell, etc.
+- 🤖 Compatible with OpenAI GPT-3.5/4s, DALL·E, and Claude API in Chinese Mainland and other countries.
+
+
 ## Install
 
 ```bash
 pip install terminal-agent-x
 ```
 
 ## Config
@@ -39,90 +47,74 @@
 
 You can use the `tax <prompt>` to interact with the model, like:
 
 ```
 $ tax write a python code for fibonacci
 ```
 
-Use `tax -h` to get more information.
-```bash
-usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
-
-Tax: A terminal agent using OpenAI/Claude API
-
-positional arguments:
-  prompt                Prompt
-
-options:
-  -h, --help            show this help message and exit
-  -k KEY, --key KEY     Your key for OpenAI/Claude.
-  --model MODEL         Model name. Choose from gpt-3.5/4s or DALLE.
-  -i INPUT, --input INPUT
-                        Input file. If specified, the prompt will be read from the file.
-  -o OUTPUT, --output OUTPUT
-                        Output file. If specified, the response will be saved to the file.
-  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.
-  --show_all            Show all contents in the response.
+or use `tax --chat` to chat with the model.
+```
+$ tax --chat
+> hi
+Tax: Hello! How can I assist you today?
 ```
 
+Use `tax -h` to get more information.
+
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
-Anthropic Claude API in not available since July 2023. Please use OpenAI API instead.
-
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
-<summary>0.1.0</summary>
+<summary>0.1.x</summary>
+
+#### 0.1.0
 
 - Implement basic functions
 - Support for Windows cmd and Linux shell
 - Add `--file` option for saving the response to a file
-</details>
 
-<details>
-<summary>0.1.1</summary>
+#### 0.1.1
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
-</details>
 
-<details>
-<summary>0.1.2</summary>
+#### 0.1.2
 
-- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt). (deprecated in 0.1.5) 
 - Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
 - Add a timeout function.
 - Fix: C++ code block prefix.
-</details>
 
-<details>
-<summary>0.1.3</summary>
+#### 0.1.3
 
 - Fix: code block prefix bug (tax will act maybe a little faster).
 - Modify: simplify the code.
 - Test: test for multi-process. Now you can use tax more efficiently in terminal.
-</details>
 
-<details>
-<summary>0.1.4</summary>
+#### 0.1.4
 
 - Feat: Add support for reading prompt from file.
 - Feat: Add support for OpenAI DALL·E.
 - Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
-</details>
 
-<details>
-<summary>0.1.5</summary>
+#### 0.1.5
+
+- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable. `claude-to-chatgpt` is unavailable.
+
+#### 0.1.6
+
+- Feat: Add support for **Chat** on Linux. Now you can use tax as **ChatGPT CLI**!
+- Feat: Add support for native Anthropic Claude API on Linux Shell, Windows cmd and Powershell.
 
-- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable.
 </details>
```

### Comparing `terminal-agent-x-0.1.5/README.md` & `terminal-agent-x-0.1.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Terminal-Agent-X
 
 [EN](README.md) / [中文](https://github.com/LyuLumos/Terminal-Agent-X/blob/main/README_cn.md) / [Wiki](https://github.com/LyuLumos/Terminal-Agent-X/wiki)
 
+## Features
+
+- 👻 Easy installation and usage with a single command.
+- 🎈 Small size, no additional dependencies required.
+- 🐼 Supports English and Chinese on Windows CMD, Powershell, Linux shell, etc.
+- 🤖 Compatible with OpenAI GPT-3.5/4s, DALL·E, and Claude API in Chinese Mainland and other countries.
+
+
 ## Install
 
 ```bash
 pip install terminal-agent-x
 ```
 
 ## Config
@@ -19,90 +27,74 @@
 
 You can use the `tax <prompt>` to interact with the model, like:
 
 ```
 $ tax write a python code for fibonacci
 ```
 
-Use `tax -h` to get more information.
-```bash
-usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
-
-Tax: A terminal agent using OpenAI/Claude API
-
-positional arguments:
-  prompt                Prompt
-
-options:
-  -h, --help            show this help message and exit
-  -k KEY, --key KEY     Your key for OpenAI/Claude.
-  --model MODEL         Model name. Choose from gpt-3.5/4s or DALLE.
-  -i INPUT, --input INPUT
-                        Input file. If specified, the prompt will be read from the file.
-  -o OUTPUT, --output OUTPUT
-                        Output file. If specified, the response will be saved to the file.
-  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.
-  --show_all            Show all contents in the response.
+or use `tax --chat` to chat with the model.
+```
+$ tax --chat
+> hi
+Tax: Hello! How can I assist you today?
 ```
 
+Use `tax -h` to get more information.
+
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
-Anthropic Claude API in not available since July 2023. Please use OpenAI API instead.
-
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
-<summary>0.1.0</summary>
+<summary>0.1.x</summary>
+
+#### 0.1.0
 
 - Implement basic functions
 - Support for Windows cmd and Linux shell
 - Add `--file` option for saving the response to a file
-</details>
 
-<details>
-<summary>0.1.1</summary>
+#### 0.1.1
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
-</details>
 
-<details>
-<summary>0.1.2</summary>
+#### 0.1.2
 
-- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt). (deprecated in 0.1.5) 
 - Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
 - Add a timeout function.
 - Fix: C++ code block prefix.
-</details>
 
-<details>
-<summary>0.1.3</summary>
+#### 0.1.3
 
 - Fix: code block prefix bug (tax will act maybe a little faster).
 - Modify: simplify the code.
 - Test: test for multi-process. Now you can use tax more efficiently in terminal.
-</details>
 
-<details>
-<summary>0.1.4</summary>
+#### 0.1.4
 
 - Feat: Add support for reading prompt from file.
 - Feat: Add support for OpenAI DALL·E.
 - Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
-</details>
 
-<details>
-<summary>0.1.5</summary>
+#### 0.1.5
+
+- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable. `claude-to-chatgpt` is unavailable.
+
+#### 0.1.6
+
+- Feat: Add support for **Chat** on Linux. Now you can use tax as **ChatGPT CLI**!
+- Feat: Add support for native Anthropic Claude API on Linux Shell, Windows cmd and Powershell.
 
-- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable.
 </details>
```

### Comparing `terminal-agent-x-0.1.5/pyproject.toml` & `terminal-agent-x-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal-agent-x"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="LyuLumos", email="lyujiuyang0@gmail.com" },
 ]
 
 description = "A terminal agent for terminal users."
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `terminal-agent-x-0.1.5/terminal_agent_x/tax.py` & `terminal-agent-x-0.1.6/terminal_agent_x/tax.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import subprocess
 import os
 import argparse
 import re
 import json
 from typing import Tuple
 import psutil
+import datetime
 
 
 def check_terminal() -> str:
     # check the terminal type
     parent_process_name = psutil.Process(os.getppid()).name()
     if parent_process_name in ['pwsh', 'powershell', 'powershell.exe']:
         return 'powershell'
@@ -40,73 +41,106 @@
         for child in children:
             child.kill()
         parent.kill()
     except psutil.NoSuchProcess:
         pass
 
 
-def fetch_code(openai_key: str, model: str, prompt: str, url_option: str) -> str:
-    url, headers, terminal_headers, data = req_info(openai_key, model, prompt, url_option)
+def fetch_code(openai_key: str, model: str, prompt: str, url_option: str, chat_flag: bool) -> str:
+    url, headers, terminal_headers, data = req_info(
+        openai_key, model, prompt, url_option, chat_flag)
     if os.name == 'nt':  # Windows
         if check_terminal() == 'powershell':
             wt_command = f'Invoke-WebRequest -Uri "{url}" -Method POST -Headers @{{{terminal_headers[0]};{terminal_headers[1]}}} -Body \'{data}\' -UseBasicParsing | Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty choices | Select-Object -First 1 | Select-Object -ExpandProperty message | Select-Object -ExpandProperty content'
             print(
                 f'Current version does not fully support Windows PowerShell. Please copy command below and paste:\n\n{wt_command}')
             return ''
-        # Windows cmd
+        # Windows cmdtax
         headers = [h.replace('"', '\\"') for h in headers]
         data = data.replace('"', '\\"')
         command = f'curl -s "{url}" -H "{headers[0]}" -H "{headers[1]}" -d "{data}"'
-        command = f'{command} --ipv4' if model == 'claude' else command  # The claude API worker is not IPv6 compatible
+        # The claude API worker is not IPv6 compatible
+        command = f'{command} --ipv4' if model == 'claude' else command
     else:  # Linux
         command = f"curl -s --location '{url}' --header '{headers[0]}' --header '{headers[1]}' --data '{data}'"
     # print(command)
 
     try:
         res, err = run_command_with_timeout(command, 60)
-        # print(res, err)
         # res = os.popen(command).read().encode('utf-8').decode('utf-8', 'ignore')
         if model.lower() == 'dalle':
             return json.loads(res)['data'][0]['url']
         return json.loads(res)['choices'][0]['message']['content']
-    except KeyError:
-        assert False, 'This is most likely due to poor internet or invalid key. Please retry.'
-    except json.decoder.JSONDecodeError:
-        assert False, 'This URL may be invalid or the response cannot be parsed'
+    except:
+        return 'Error', res, err
+
+
+def chat_data_wrapper(model: str, prompt: str, chat_flag: bool) -> str:
+    if chat_flag:
+        return f'{{"model": "{model}","messages":{prompt}}}'  # 组装数据的部分在函数之外完成
+    if model.lower() == 'dalle':
+        return f'{{"prompt": "{prompt}"}}'
+    return f'{{"model": "{model}","messages": [{{"role": "user", "content": "{prompt}"}}]}}'
 
 
-def req_info(openai_key: str, model: str, prompt: str, url_option: str) -> Tuple[str, str, str, str]:
+def req_info(openai_key: str, model: str, prompt: str, url_option: str, chat_flag: bool) -> Tuple[str, str, str, str]:
     headers = [
         f"Authorization: Bearer {openai_key}",
         "Content-Type: application/json"
     ]
     terminal_headers = [
         f"Authorization='Bearer {openai_key}'",
         "'Content-Type'='application/json'"
     ]
-
     urls = {
         'openai_gfw': 'https://api.openai-proxy.com/v1/chat/completions',
         'openai': 'https://api.openai.com/v1/chat/completions',
-        # 'claude': 'https://claude-api.lyulumos.space/v1/chat/completions'
     }
-    # url_option = 'claude' if model == 'claude' else url_option
-    # claude API is not accessible
-    if model == 'claude':
-        assert False, 'Claude API is not accessible now. Please use OpenAI API instead.'
     url = urls[url_option] if url_option in urls else url_option
 
     if model.lower() == 'dalle':
         url = 'https://api.openai-proxy.com/v1/images/generations' if url_option == 'openai_gfw' else 'https://api.openai.com/v1/images/generations'
-        data = f'{{"prompt": "{prompt}"}}'
-    else:
-        data = f'{{"model": "{model}","messages": [{{"role": "user", "content": "{prompt}"}}]}}'
+    data = chat_data_wrapper(model, prompt, chat_flag)
     return url, headers, terminal_headers, data
 
 
+def single_claude(anthropic_api_key: str, model: str, prompt: str) -> str:
+    url = 'https://api.anthropic.com/v1/complete'
+    model = 'claude-1' if model == 'claude' else model
+    headers = [
+        "anthropic-version: 2023-06-01",
+        "content-type: application/json",
+        f"x-api-key: {anthropic_api_key}"
+    ]
+    terminal_headers = [
+        "'anthropic-version'='2023-06-01'",
+        "'content-type'='application/json'",
+        f"'x-api-key'='{anthropic_api_key}'"
+    ]
+    data = f'{{"model": "{model}","prompt": "\\n\\nHuman: {prompt}\\n\\nAssistant:","max_tokens_to_sample": 256,"stream": false}}'
+    if os.name == 'nt':
+        if check_terminal() == 'powershell':
+            wt_command = f'Invoke-WebRequest -Uri "{url}" -Method POST -Headers @{{{terminal_headers[0]};{terminal_headers[1]};{terminal_headers[2]}}} -Body \'{data}\' -UseBasicParsing | Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty completion'
+            print(
+                f'Current version does not fully support Windows PowerShell. Please copy command below and paste:\n\n{wt_command}')
+            return ''
+        # Windows cmd
+        headers = [h.replace('"', '\\"') for h in headers]
+        data = data.replace('"', '\\"')
+        command = f'curl -s {url} -H "{headers[0]}" -H "{headers[1]}" -H "{headers[2]}" -d "{data}"'
+    else:
+        command = f"curl --request POST --url '{url}' --header '{headers[0]}' --header '{headers[1]}' --header '{headers[2]}' --data '{data}'"
+    # print(command)
+    try:
+        res, err = run_command_with_timeout(command, 60)
+        return json.loads(res)['completion']
+    except:
+        return 'Error', res, err
+
+
 def find_code(text: str) -> str:
     pattern = r"```(.*?)```"
     match = re.search(pattern, text, re.DOTALL)
     if match:
         codes = match.group(0)
         first_n = codes.find('\n')
         return codes[first_n+1:-3].strip()  # without ``` pairs
@@ -115,41 +149,72 @@
 
 def load_file(path: str) -> str:
     with open(path, 'r', encoding='utf-8') as f:
         text = f.read()
     return text.replace('\\', '\\\\').replace('"', '\\"').replace('\n', '\\n')
 
 
+def chat(openai_key: str, model: str, url_option: str):
+    current_date = datetime.datetime.now().strftime("%Y-%m-%d")
+    conversation = [
+        {"role": "system", "content": f"You are ChatGPT, a large language model trained by OpenAI.\nKnowledge cutoff: 2021-09\nCurrent date: {current_date}"},
+    ]
+    # print(conversation)
+
+    while True:
+        user_input = input("> ")
+        if user_input == "exit":
+            break
+        conversation.append({"role": "user", "content": user_input})
+        response = fetch_code(openai_key, model, json.dumps(
+            conversation), url_option, True)
+        print(f'Tax: {response}')
+        conversation.append({"role": "assistant", "content": response.encode(
+            'unicode-escape').decode('utf8').replace("'", "")})
+        # The bash command sent cannot contain single quotes, escaping has no effect. So the single quotes in the conversation will be deleted and the user will not see it.
+        # print(conversation)
+
+
 def main() -> None:
     parser = argparse.ArgumentParser(
         description='Tax: A terminal agent using OpenAI/Claude API')
-    parser.add_argument("prompt", nargs='+', type=str, help="Prompt")
+    parser.add_argument("prompt", nargs='*', type=str, help="Prompt")
     parser.add_argument('-k', '--key', type=str,
                         help='Your key for OpenAI/Claude.')
-    parser.add_argument('--model', type=str,
-                        default='gpt-3.5-turbo', help='Model name. Choose from gpt-3.5/4s or DALLE.')
+    parser.add_argument('-m', '--model', type=str,
+                        default='gpt-3.5-turbo', help='Model name. Choose from gpt-3.5/4s, Claude API or DALLE.')
     parser.add_argument('-i', '--input', type=str,
                         help='Input file. If specified, the prompt will be read from the file.')
     parser.add_argument('-o', '--output', type=str,
                         help='Output file. If specified, the response will be saved to the file.')
-    parser.add_argument('--url', type=str, default='openai',
+    parser.add_argument('-c', '--chat', action='store_true',
+                        help='Chat mode. Tax will act like ChatGPT. Enter "exit" to quit.')
+    parser.add_argument('-u', '--url', type=str, default='openai',
                         help="URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.")
-    parser.add_argument('--show_all', action='store_true',
+    parser.add_argument('-a', '--show_all', action='store_true',
                         help='Show all contents in the response.')
     args = parser.parse_args()
 
     prompt = ' '.join(args.prompt)
     prompt = f'{prompt}\\n{load_file(args.input)}' if args.input else prompt
 
     key = args.key or os.environ.get('OpenAI_KEY')
     if not key:
         assert False, 'Error: OpenAI key not found. Please specify it in system environment variables or pass it as an argument.'
+    if args.chat:
+        chat(key, args.model, args.url)
+        return
+
+    if args.model.lower() == 'claude' or args.url == 'claude':
+        res = single_claude(key, 'claude-1', prompt)
+        print(res)
+        return
 
     # res = get_model_response(openai_key, args.model, prompt)
-    res = fetch_code(key, args.model, prompt, args.url)
+    res = fetch_code(key, args.model, prompt, args.url, False)
 
     if args.output:
         with open(args.output, 'w', encoding='utf-8') as f:
             f.write(res)
         f.close()
     elif args.show_all or args.model.lower() == 'dalle':
         print(res)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `terminal-agent-x-0.1.5/terminal_agent_x.egg-info/PKG-INFO` & `terminal-agent-x-0.1.6/terminal_agent_x.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.5
+Version: 0.1.6
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Project-URL: Wiki, https://github.com/LyuLumos/Terminal-Agent-X/wiki
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal-Agent-X
 
 [EN](README.md) / [中文](https://github.com/LyuLumos/Terminal-Agent-X/blob/main/README_cn.md) / [Wiki](https://github.com/LyuLumos/Terminal-Agent-X/wiki)
 
+## Features
+
+- 👻 Easy installation and usage with a single command.
+- 🎈 Small size, no additional dependencies required.
+- 🐼 Supports English and Chinese on Windows CMD, Powershell, Linux shell, etc.
+- 🤖 Compatible with OpenAI GPT-3.5/4s, DALL·E, and Claude API in Chinese Mainland and other countries.
+
+
 ## Install
 
 ```bash
 pip install terminal-agent-x
 ```
 
 ## Config
@@ -39,90 +47,74 @@
 
 You can use the `tax <prompt>` to interact with the model, like:
 
 ```
 $ tax write a python code for fibonacci
 ```
 
-Use `tax -h` to get more information.
-```bash
-usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
-
-Tax: A terminal agent using OpenAI/Claude API
-
-positional arguments:
-  prompt                Prompt
-
-options:
-  -h, --help            show this help message and exit
-  -k KEY, --key KEY     Your key for OpenAI/Claude.
-  --model MODEL         Model name. Choose from gpt-3.5/4s or DALLE.
-  -i INPUT, --input INPUT
-                        Input file. If specified, the prompt will be read from the file.
-  -o OUTPUT, --output OUTPUT
-                        Output file. If specified, the response will be saved to the file.
-  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.
-  --show_all            Show all contents in the response.
+or use `tax --chat` to chat with the model.
+```
+$ tax --chat
+> hi
+Tax: Hello! How can I assist you today?
 ```
 
+Use `tax -h` to get more information.
+
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
-Anthropic Claude API in not available since July 2023. Please use OpenAI API instead.
-
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
-<summary>0.1.0</summary>
+<summary>0.1.x</summary>
+
+#### 0.1.0
 
 - Implement basic functions
 - Support for Windows cmd and Linux shell
 - Add `--file` option for saving the response to a file
-</details>
 
-<details>
-<summary>0.1.1</summary>
+#### 0.1.1
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
-</details>
 
-<details>
-<summary>0.1.2</summary>
+#### 0.1.2
 
-- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt). (deprecated in 0.1.5) 
 - Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
 - Add a timeout function.
 - Fix: C++ code block prefix.
-</details>
 
-<details>
-<summary>0.1.3</summary>
+#### 0.1.3
 
 - Fix: code block prefix bug (tax will act maybe a little faster).
 - Modify: simplify the code.
 - Test: test for multi-process. Now you can use tax more efficiently in terminal.
-</details>
 
-<details>
-<summary>0.1.4</summary>
+#### 0.1.4
 
 - Feat: Add support for reading prompt from file.
 - Feat: Add support for OpenAI DALL·E.
 - Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
-</details>
 
-<details>
-<summary>0.1.5</summary>
+#### 0.1.5
+
+- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable. `claude-to-chatgpt` is unavailable.
+
+#### 0.1.6
+
+- Feat: Add support for **Chat** on Linux. Now you can use tax as **ChatGPT CLI**!
+- Feat: Add support for native Anthropic Claude API on Linux Shell, Windows cmd and Powershell.
 
-- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable.
 </details>
```

