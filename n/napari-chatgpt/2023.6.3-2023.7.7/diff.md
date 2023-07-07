# Comparing `tmp/napari-chatgpt-2023.6.3.tar.gz` & `tmp/napari-chatgpt-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-chatgpt-2023.6.3.tar", last modified: Sun Jun  4 04:04:01 2023, max compression
+gzip compressed data, was "napari-chatgpt-2023.7.7.tar", last modified: Fri Jul  7 20:54:06 2023, max compression
```

## Comparing `napari-chatgpt-2023.6.3.tar` & `napari-chatgpt-2023.7.7.tar`

### file list

```diff
@@ -1,242 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.545266 napari-chatgpt-2023.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.github/workflows/just_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/src/napari_chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/bard_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/conv_agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gpt4all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gtts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/lanchain_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/openai_list_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/playwright_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/tts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/whisper_cpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.573267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/
--rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/_tailwind.css
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/chat.js
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/marked-highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.css
--rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.js
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight-min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.dark.css
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/tailwind.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/llms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/.pytest_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/bard_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/napari_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/async_base_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/tools_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cellpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_base_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/file_download_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/human_input_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/gpt4all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/download_files_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/summarizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/napari_viewer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/open_in_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/dynamic_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_code_given_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/installed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/missing_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/python_lang_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/required_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_guard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/installed_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/required_imports_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/download_file_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/qt_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/filter_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_function_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/python_code_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_code_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_url_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/folders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/metasearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/scrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/google_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/metasearch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/scrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/wikipedia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.565267 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.564057 napari-chatgpt-2023.7.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.580057 napari-chatgpt-2023.7.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.github/workflows/just_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.580057 napari-chatgpt-2023.7.7/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20845 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.584058 napari-chatgpt-2023.7.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.584058 napari-chatgpt-2023.7.7/src/napari_chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.592058 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/bard_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/conv_agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/enumerate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/enumerate_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/gpt4all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/gtts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/lanchain_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/openai_list_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/playwright_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/tts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/whisper_cpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/chat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/chat_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.604058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/_tailwind.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/chat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/marked-highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.css
+-rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/tailwind.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/llms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/.pytest_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/bard_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/napari_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.620058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/async_base_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.620058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/tools_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.620058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.624058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.628058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_fgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/cellpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/stardist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/image_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/napari_base_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.628058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.632058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/file_download_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/human_input_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/python_repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.632058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.632058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/gpt4all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/download_files_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/images/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/summarizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/napari_viewer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/open_in_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.644058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.644058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.644058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.648058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/conda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/dynamic_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_code_given_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/installed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/missing_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/pip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/python_lang_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/required_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.652058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/exception_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/exception_guard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/installed_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/required_imports_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.652058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/download_file_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/qt_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.656058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/extract_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/filter_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/find_function_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/python_code_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/extract_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/extract_url_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/system/folders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/metasearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/scrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/google_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/metasearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/scrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/wikipedia_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.588058 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/tox.ini
```

### Comparing `napari-chatgpt-2023.6.3/.github/workflows/just_deploy.yml` & `napari-chatgpt-2023.7.7/.github/workflows/just_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/.github/workflows/test_and_deploy.yml` & `napari-chatgpt-2023.7.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/.gitignore` & `napari-chatgpt-2023.7.7/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -79,7 +79,8 @@
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
 **/_version.py
 /src/napari_chatgpt/llm/test/.pytest_cache/README.md
+/src/napari_chatgpt/llm/test/.pytest_cache/CACHEDIR.TAG
```

### Comparing `napari-chatgpt-2023.6.3/.napari-hub/config.yml` & `napari-chatgpt-2023.7.7/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/.pre-commit-config.yaml` & `napari-chatgpt-2023.7.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/LICENSE` & `napari-chatgpt-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/PKG-INFO` & `napari-chatgpt-2023.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.6.3
+Version: 2023.7.7
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
@@ -35,15 +35,15 @@
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
 
-A [napari](napari.org) plugin that levegares OpenAI's Large Language Model
+A [napari](napari.org) plugin that leverages OpenAI's Large Language Model
 ChatGPT to implement _Omega_
 a napari-aware agent capable of performing image processing and analysis tasks
 in a conversational manner.
 
 This repository was created as a 'week-end project'
 by [Loic A. Royer](https://twitter.com/loicaroyer)
 who leads a [research group](https://royerlab.org) at
@@ -58,16 +58,16 @@
 
 # What is Omega?
 
 Omega is a LLM-based and tool-armed autonomous agent that demonstrates the
 potential for Large Language Models (LLMs) to be applied to image processing,
 analysis and visualisation.
 Can LLM-based agents write image processing code and napari widgets, correct its
-coding mistakes, perform
-follow-up analysis, and control the napari viewer? The answer appears to be yes.
+coding mistakes, perform follow-up analysis, and control the napari viewer? 
+The answer appears to be yes.
 
 #### In this video I ask Omega to segment an image using the [SLIC](https://www.iro.umontreal.ca/~mignotte/IFT6150/Articles/SLIC_Superpixels.pdf) algorithm. It makes a first attempt using the implementation in scikit-image, but fails because of an inexistant 'multichannel' parameter. Realising that, Omega tries again, and this time, succeeds:
 
 https://user-images.githubusercontent.com/1870994/235768559-ca8bfa84-21f5-47b6-b2bd-7fcc07cedd92.mp4
 
 #### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:
 
@@ -143,102 +143,125 @@
 corresponding environment).
 
 IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the
 latest one!
 
 ## Installation in an new conda environment (RECOMMENDED):
 
-Make sure you have an anaocnda/miniconda installation on your system.
-Ask ChatGPT what is that all about if you are unsure ;-)
+Make sure you have an [miniconda](https://docs.conda.io/en/latest/miniconda.html) installation on your system.
+Ask [ChatGPT](https://chat.openai.com/auth/login) what is that all about if you are unsure ;-)
 
 Create environment:
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
     conda activate napari-chatgpt 
 
-Install napari in the environment using conda-forge: (important on Apple M1/M2)
+Install [napari](napari.org) in the environment using conda-forge: (very important on Apple M1/M2)
 
-    conda install -c conda-forge napari     
+    conda install -c conda-forge napari
 
-Install the repo in enbvironment:
+**Or**, with pip:
+
+    pip install napari
+
+Install napari-chatgpt in the environment:
 
     pip install napari-chatgpt
 
 ## Installation variations:
 
-To install latest development version :
+To install latest development version (not recommended for end-users):
 
+    conda create -y -n napari-chatgpt -c conda-forge python=3.9
+    conda activate napari-chatgpt
+    pip install napari  
     git clone https://github.com/royerlab/napari-chatgpt.git
     cd napari-chatgpt
     pip install -e .
 
 or:
-
+    
+    # same steps as above and then:
     pip install git+https://github.com/royerlab/napari-chatgpt.git
 
+## System specific tweaks:
+
+On Ubuntu systems, I recommend setting changing the UI timeout, 
+otherwise whenever Omega is thinking, the UI will freeze, and a popup will block
+everything which is very annoying:
+
+    gsettings set org.gnome.mutter check-alive-timeout 60000
+    
+
+
 ## Requirements:
 
-You need an OpenAI key, there is no way around this, unless we add some other,
-potentially local LLMs compatible to
-LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar
-models come to mind). However, this will likely be at the cost of cognitive
-performance,
-which I am not sure is worth it at this point. Please prove me wrong.
-You can get your OpenAI key by signing
-up [here](https://openai.com/blog/openai-api).
+You need an OpenAI key, there is no way around this, I have been experimenting with 
+other models, but right now the best results, by far are obtained with ChatGPT 4 (and to
+a lesser extent 3.5). You can get your OpenAI key by signing up [here](https://openai.com/blog/openai-api).
 Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5
-is very
-reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
-bargain.
-Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
+is very reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
+bargain. Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
 hopefully.
 
 Note: you can limit the burn-rate to a certain amount of dollars per month, just
-in case you let
-Omega thinking over the week end and forget to stop it (don't worry, this is
-actually not possible).
+in case you let Omega thinking over the weekend and forget to stop it (don't worry, 
+this is actually **not** possible).
 
 ## Usage:
 
 Once all is installed, and if it is not already running, start napari:
 
     napari
 
 You can then the Omega napari plugin via the plugins menu:
 
 <img width="498" alt="image" src="https://user-images.githubusercontent.com/1870994/235790134-1d87fd50-583f-4fd9-ade2-c64497b91331.png">
 
 
-You just opened the plugin as a widget, you now need to actually start Omega:
+You just opened the plugin as a widget, this widget will appear:
+
+<img width="267" alt="image" src="https://github.com/royerlab/napari-chatgpt/assets/1870994/fdbde938-548d-4104-9241-d87c46c76dcf">
+
+I recommend that initially you stick to the defaults values, which work well.
+The best memory is 'hybrid'.
+The 'autofix' features only make sense if you are choosing a ChatGPT 4 model, 
+ChatGPT might get confused... 
+Increasing creativity also decreases 'attention to detail'; the models will make more
+coding mistakes, but might try more original solutions...
+
+You then need to actually start Omega:
 
 <img width="104" alt="image" src="https://user-images.githubusercontent.com/1870994/235811111-9e468785-9562-410a-8e9a-c63cb03fb765.png">
 
 
-If you have not set the 'OPENAI_API_KEY' environment variable as is typicall
-done,
-Omega will ask you for your OpenAI API key, and will store it _safely_ in an
+If you have not set the 'OPENAI_API_KEY' environment variable as is typically
+done, Omega will ask you for your OpenAI API key, and will store it _safely_ in an
 _encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
 
 <img width="293" alt="image" src="https://user-images.githubusercontent.com/1870994/235793528-9e892c5e-d8ca-43e1-9020-f2dfab45b32d.png">
 
 
-Just enter an encryption/decription key, your OpenAI key, and
+Just enter an encryption/decryption key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
-(The idea is that you might not be able to remember your openAI key by heart,
+(The idea is that you might not be able to remember your openAI key by heart, obviously,
 but you might be able to do so with your own password or passphrase)
 
 You can then direct your browser
 to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
-and start having an hopefully nice chat with Omega.
+and start having a hopefully nice chat with Omega:
+
+<img width="631" alt="image" src="https://github.com/royerlab/napari-chatgpt/assets/1870994/a5cf6d4d-deea-4df8-be8a-601d1cc0424c">
+
 
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
 - What is your name?
 - What tools do you have available?
@@ -248,27 +271,27 @@
 - Make a widget that applies the transformation: y = x^alpha + y^beta with alpha
   and beta two parameters.
 - Create a widget to multiply two images
 - Can you open in napari a photo of Albert Einstein?
 - Downscale by a factor 3x the image on layer named 'img'
 - Rename selected layer to 'downscaled_image'
 - Upscale image 'downscaled_image' by a factor 3 using some smart interpolation
-  scheme of your choice (not nearest-neighboor)
+  scheme of your choice (not nearest-neighbor)
 - Caveat: makes a plugin instead of actually doing teh job
 - How many channels has the image on layer 0
 - Make a image sharpening filter widget, expose relevant parameters
 - Can you open this file in
   napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
 - Split the two channels of the first layer (first axis) into two separate
   layers
 - Switch viewer to 3d
 - Create a napari widget for a function that takes two image layers and returns
   a 3D image stack of n images where each 2D image corresponds to a linear
   blending of the two layer images between 0 and 1.
-- [Loaded the ‘cell’ sample image] there is one cell in the image on the first
+- Loaded the ‘cell’ sample image. there is one cell in the image on the first
   layer, it is roughly circular and brighter than its surroundings, ca you write
   segmentation code that returns a labels layer for it?
 - Can you create a widget to blend two images?
 - Can you tell me more about the 'guided Canny edge filter' ?
 - Write a configurable RGB to grayscale widget, ensure weights sum to 1
 
 ## Video Demos:
@@ -277,17 +300,16 @@
 models,
 so here are videos showcasing what's possible. You will notice that Omega
 sometimes
 fails on its first attempt, typically because of mistaken parameters for
 functions,
 or other syntax errors. But it also often recovers by having access to the error
 message,
-and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can
-do, imagine
-what will be possible with 4.0 and future more capable models...
+and reasoning its way to the right piece of code. The videos below were made with ChatGPT 3.5,
+version 4 works much better imagine what will be possible with future even more capable models...
 
 ##
 
 In this first video, I ask Omega to make a napari widget to convert images from
 RGB to grayscale:
 
 https://user-images.githubusercontent.com/1870994/235769895-23cfc7ed-622a-47f9-95aa-4be77efc0f78.mp4
@@ -305,17 +327,17 @@
 ##
 
 Following-up from the previous video, I ask Omega to create a new labels layer
 containing just the largest segment. The script that Omega writes as another
 rookie mistake: it confuses layers and images. The error message then confuses
 Omega into thinking that it got the name of the layer wrong, setting it off in a
 quest
-to find the name of the labels layer. It succeeds at writting code that searches
+to find the name of the labels layer. It succeeds at writing code that searches
 for the labels layer, and uses that name to write a script that then does
-extracts te largest segment into its own layer. Not bad:
+extract the largest segment into its own layer. Not bad:
 
 https://user-images.githubusercontent.com/1870994/235770741-d8905afd-0a9b-4eb7-a075-481979ab7b01.mp4
 
 ##
 
 In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific.
 The answer is a vanilla yet effective widget that uses the Otsu approach to
@@ -451,22 +473,22 @@
 not a practical approach. Not clear what happened to the colors though. Probably
 an RGB ordering or format issue:
 
 https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
 
 ## Disclaimer:
 
-Do not use this software lightly, it will download libaries by its own volition,
-write any code that it deems nescessary, it might actually do what you ask, even
+Do not use this software lightly, it will download libraries by its own volition,
+write any code that it deems necessary, it might actually do what you ask, even
 if
-it is a bad idea. Also, beware that it might _misundertand_ what you ask and
+it is a bad idea. Also, beware that it might _misunderstand_ what you ask and
 then do
 something bad. For example, it is unwise to use Omega to delete 'some' files
 from your system,
-it might end up deleteing more than that if you are unclear in your request.  
+it might end up deleting more than that if you are unclear in your request.  
 To be 100% safe, we recommend that you use this software from within a sandboxed
 virtual machine.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED,
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 PARTICULAR
```

### Comparing `napari-chatgpt-2023.6.3/README.md` & `napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,49 @@
+Metadata-Version: 2.1
+Name: napari-chatgpt
+Version: 2023.7.7
+Summary: A napari plugin to process and analyse images with chatGPT.
+Home-page: https://github.com/royerlab/napari-chatgpt
+Author: Loic A. Royer
+Author-email: royerloic@gmail.com
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
+Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
+Project-URL: Source Code, https://github.com/royerlab/napari-chatgpt
+Project-URL: User Support, https://github.com/royerlab/napari-chatgpt/issues
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 # napari-chatgpt
 
 ## Home of
 _Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
 
-A [napari](napari.org) plugin that levegares OpenAI's Large Language Model
+A [napari](napari.org) plugin that leverages OpenAI's Large Language Model
 ChatGPT to implement _Omega_
 a napari-aware agent capable of performing image processing and analysis tasks
 in a conversational manner.
 
 This repository was created as a 'week-end project'
 by [Loic A. Royer](https://twitter.com/loicaroyer)
 who leads a [research group](https://royerlab.org) at
@@ -29,16 +58,16 @@
 
 # What is Omega?
 
 Omega is a LLM-based and tool-armed autonomous agent that demonstrates the
 potential for Large Language Models (LLMs) to be applied to image processing,
 analysis and visualisation.
 Can LLM-based agents write image processing code and napari widgets, correct its
-coding mistakes, perform
-follow-up analysis, and control the napari viewer? The answer appears to be yes.
+coding mistakes, perform follow-up analysis, and control the napari viewer? 
+The answer appears to be yes.
 
 #### In this video I ask Omega to segment an image using the [SLIC](https://www.iro.umontreal.ca/~mignotte/IFT6150/Articles/SLIC_Superpixels.pdf) algorithm. It makes a first attempt using the implementation in scikit-image, but fails because of an inexistant 'multichannel' parameter. Realising that, Omega tries again, and this time, succeeds:
 
 https://user-images.githubusercontent.com/1870994/235768559-ca8bfa84-21f5-47b6-b2bd-7fcc07cedd92.mp4
 
 #### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:
 
@@ -114,102 +143,125 @@
 corresponding environment).
 
 IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the
 latest one!
 
 ## Installation in an new conda environment (RECOMMENDED):
 
-Make sure you have an anaocnda/miniconda installation on your system.
-Ask ChatGPT what is that all about if you are unsure ;-)
+Make sure you have an [miniconda](https://docs.conda.io/en/latest/miniconda.html) installation on your system.
+Ask [ChatGPT](https://chat.openai.com/auth/login) what is that all about if you are unsure ;-)
 
 Create environment:
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
     conda activate napari-chatgpt 
 
-Install napari in the environment using conda-forge: (important on Apple M1/M2)
+Install [napari](napari.org) in the environment using conda-forge: (very important on Apple M1/M2)
+
+    conda install -c conda-forge napari
 
-    conda install -c conda-forge napari     
+**Or**, with pip:
 
-Install the repo in enbvironment:
+    pip install napari
+
+Install napari-chatgpt in the environment:
 
     pip install napari-chatgpt
 
 ## Installation variations:
 
-To install latest development version :
+To install latest development version (not recommended for end-users):
 
+    conda create -y -n napari-chatgpt -c conda-forge python=3.9
+    conda activate napari-chatgpt
+    pip install napari  
     git clone https://github.com/royerlab/napari-chatgpt.git
     cd napari-chatgpt
     pip install -e .
 
 or:
-
+    
+    # same steps as above and then:
     pip install git+https://github.com/royerlab/napari-chatgpt.git
 
+## System specific tweaks:
+
+On Ubuntu systems, I recommend setting changing the UI timeout, 
+otherwise whenever Omega is thinking, the UI will freeze, and a popup will block
+everything which is very annoying:
+
+    gsettings set org.gnome.mutter check-alive-timeout 60000
+    
+
+
 ## Requirements:
 
-You need an OpenAI key, there is no way around this, unless we add some other,
-potentially local LLMs compatible to
-LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar
-models come to mind). However, this will likely be at the cost of cognitive
-performance,
-which I am not sure is worth it at this point. Please prove me wrong.
-You can get your OpenAI key by signing
-up [here](https://openai.com/blog/openai-api).
+You need an OpenAI key, there is no way around this, I have been experimenting with 
+other models, but right now the best results, by far are obtained with ChatGPT 4 (and to
+a lesser extent 3.5). You can get your OpenAI key by signing up [here](https://openai.com/blog/openai-api).
 Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5
-is very
-reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
-bargain.
-Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
+is very reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
+bargain. Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
 hopefully.
 
 Note: you can limit the burn-rate to a certain amount of dollars per month, just
-in case you let
-Omega thinking over the week end and forget to stop it (don't worry, this is
-actually not possible).
+in case you let Omega thinking over the weekend and forget to stop it (don't worry, 
+this is actually **not** possible).
 
 ## Usage:
 
 Once all is installed, and if it is not already running, start napari:
 
     napari
 
 You can then the Omega napari plugin via the plugins menu:
 
 <img width="498" alt="image" src="https://user-images.githubusercontent.com/1870994/235790134-1d87fd50-583f-4fd9-ade2-c64497b91331.png">
 
 
-You just opened the plugin as a widget, you now need to actually start Omega:
+You just opened the plugin as a widget, this widget will appear:
+
+<img width="267" alt="image" src="https://github.com/royerlab/napari-chatgpt/assets/1870994/fdbde938-548d-4104-9241-d87c46c76dcf">
+
+I recommend that initially you stick to the defaults values, which work well.
+The best memory is 'hybrid'.
+The 'autofix' features only make sense if you are choosing a ChatGPT 4 model, 
+ChatGPT might get confused... 
+Increasing creativity also decreases 'attention to detail'; the models will make more
+coding mistakes, but might try more original solutions...
+
+You then need to actually start Omega:
 
 <img width="104" alt="image" src="https://user-images.githubusercontent.com/1870994/235811111-9e468785-9562-410a-8e9a-c63cb03fb765.png">
 
 
-If you have not set the 'OPENAI_API_KEY' environment variable as is typicall
-done,
-Omega will ask you for your OpenAI API key, and will store it _safely_ in an
+If you have not set the 'OPENAI_API_KEY' environment variable as is typically
+done, Omega will ask you for your OpenAI API key, and will store it _safely_ in an
 _encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
 
 <img width="293" alt="image" src="https://user-images.githubusercontent.com/1870994/235793528-9e892c5e-d8ca-43e1-9020-f2dfab45b32d.png">
 
 
-Just enter an encryption/decription key, your OpenAI key, and
+Just enter an encryption/decryption key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
-(The idea is that you might not be able to remember your openAI key by heart,
+(The idea is that you might not be able to remember your openAI key by heart, obviously,
 but you might be able to do so with your own password or passphrase)
 
 You can then direct your browser
 to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
-and start having an hopefully nice chat with Omega.
+and start having a hopefully nice chat with Omega:
+
+<img width="631" alt="image" src="https://github.com/royerlab/napari-chatgpt/assets/1870994/a5cf6d4d-deea-4df8-be8a-601d1cc0424c">
+
 
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
 - What is your name?
 - What tools do you have available?
@@ -219,27 +271,27 @@
 - Make a widget that applies the transformation: y = x^alpha + y^beta with alpha
   and beta two parameters.
 - Create a widget to multiply two images
 - Can you open in napari a photo of Albert Einstein?
 - Downscale by a factor 3x the image on layer named 'img'
 - Rename selected layer to 'downscaled_image'
 - Upscale image 'downscaled_image' by a factor 3 using some smart interpolation
-  scheme of your choice (not nearest-neighboor)
+  scheme of your choice (not nearest-neighbor)
 - Caveat: makes a plugin instead of actually doing teh job
 - How many channels has the image on layer 0
 - Make a image sharpening filter widget, expose relevant parameters
 - Can you open this file in
   napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
 - Split the two channels of the first layer (first axis) into two separate
   layers
 - Switch viewer to 3d
 - Create a napari widget for a function that takes two image layers and returns
   a 3D image stack of n images where each 2D image corresponds to a linear
   blending of the two layer images between 0 and 1.
-- [Loaded the ‘cell’ sample image] there is one cell in the image on the first
+- Loaded the ‘cell’ sample image. there is one cell in the image on the first
   layer, it is roughly circular and brighter than its surroundings, ca you write
   segmentation code that returns a labels layer for it?
 - Can you create a widget to blend two images?
 - Can you tell me more about the 'guided Canny edge filter' ?
 - Write a configurable RGB to grayscale widget, ensure weights sum to 1
 
 ## Video Demos:
@@ -248,17 +300,16 @@
 models,
 so here are videos showcasing what's possible. You will notice that Omega
 sometimes
 fails on its first attempt, typically because of mistaken parameters for
 functions,
 or other syntax errors. But it also often recovers by having access to the error
 message,
-and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can
-do, imagine
-what will be possible with 4.0 and future more capable models...
+and reasoning its way to the right piece of code. The videos below were made with ChatGPT 3.5,
+version 4 works much better imagine what will be possible with future even more capable models...
 
 ##
 
 In this first video, I ask Omega to make a napari widget to convert images from
 RGB to grayscale:
 
 https://user-images.githubusercontent.com/1870994/235769895-23cfc7ed-622a-47f9-95aa-4be77efc0f78.mp4
@@ -276,17 +327,17 @@
 ##
 
 Following-up from the previous video, I ask Omega to create a new labels layer
 containing just the largest segment. The script that Omega writes as another
 rookie mistake: it confuses layers and images. The error message then confuses
 Omega into thinking that it got the name of the layer wrong, setting it off in a
 quest
-to find the name of the labels layer. It succeeds at writting code that searches
+to find the name of the labels layer. It succeeds at writing code that searches
 for the labels layer, and uses that name to write a script that then does
-extracts te largest segment into its own layer. Not bad:
+extract the largest segment into its own layer. Not bad:
 
 https://user-images.githubusercontent.com/1870994/235770741-d8905afd-0a9b-4eb7-a075-481979ab7b01.mp4
 
 ##
 
 In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific.
 The answer is a vanilla yet effective widget that uses the Otsu approach to
@@ -422,22 +473,22 @@
 not a practical approach. Not clear what happened to the colors though. Probably
 an RGB ordering or format issue:
 
 https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
 
 ## Disclaimer:
 
-Do not use this software lightly, it will download libaries by its own volition,
-write any code that it deems nescessary, it might actually do what you ask, even
+Do not use this software lightly, it will download libraries by its own volition,
+write any code that it deems necessary, it might actually do what you ask, even
 if
-it is a bad idea. Also, beware that it might _misundertand_ what you ask and
+it is a bad idea. Also, beware that it might _misunderstand_ what you ask and
 then do
 something bad. For example, it is unwise to use Omega to delete 'some' files
 from your system,
-it might end up deleteing more than that if you are unclear in your request.  
+it might end up deleting more than that if you are unclear in your request.  
 To be 100% safe, we recommend that you use this software from within a sandboxed
 virtual machine.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED,
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 PARTICULAR
```

### Comparing `napari-chatgpt-2023.6.3/setup.cfg` & `napari-chatgpt-2023.7.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -30,34 +30,37 @@
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	scikit-image
 	qtpy
-	langchain==0.0.167
+	langchain==0.0.208
 	fastapi
 	uvicorn
 	websockets
 	openai
 	tiktoken
 	wikipedia
 	lxml
 	gTTS
 	playsound
 	matplotlib
 	xarray
 	arbol
 	playwright
-	duckduckgo_search==3.7.1
+	duckduckgo_search
 	ome-zarr
 	scikit-video
 	pygpt4all==1.1.0
 	GoogleBard==1.0.2
 	transformers
+	cryptography
+	tabulate
+	numba
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = setuptools_scm
 
 [options.packages.find]
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/conv_agent_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/conv_agent_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_functions.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/enumerate_functions.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gpt4all_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/gpt4all_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/lanchain_openai.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/lanchain_openai.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/playwright_sandbox.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/playwright_sandbox.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/speech_recognition_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/speech_recognition_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/terminal.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/terminal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/tts_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/tts_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/whisper_cpp.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/whisper_cpp.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/test_widget.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/test_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 # make_napari_viewer is a pytest fixture that returns a napari viewer object
 # capsys is a pytest fixture that captures stdout and stderr output streams
 def test_omega_q_widget(make_napari_viewer, capsys):
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
     viewer.add_image(np.random.random((100, 100)))
 
-    # create our widget, passing in the viewer
-    my_widget = OmegaQWidget(viewer)
-
-    # # call our widget method
-    # my_widget._on_click()
+    # No testing of UI elements yet!
+    #
+    # # create our widget, passing in the viewer
+    # my_widget = OmegaQWidget(viewer)
     #
-    # # read captured output and check that it's as we expected
-    # captured = capsys.readouterr()
-    # assert 'Omega' in captured.out
+    # # # call our widget method
+    # # my_widget._on_click()
+    # #
+    # # # read captured output and check that it's as we expected
+    # # captured = capsys.readouterr()
+    # # assert 'Omega' in captured.out
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/_widget.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,43 +5,47 @@
 see: https://napari.org/stable/plugins/guides.html?#widgets
 
 Replace code below according to your needs.
 """
 import sys
 from typing import TYPE_CHECKING
 
-import openai
+from napari_chatgpt.chat_server.chat_server import NapariChatServer
+from napari_chatgpt.utils.api_keys.api_key import set_api_key
+from napari_chatgpt.utils.python.installed_packages import \
+    is_package_installed
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QApplication, QLabel, QCheckBox
 from PyQt5.QtWidgets import QVBoxLayout, QComboBox
 from napari.viewer import Viewer
 from qtpy.QtWidgets import QPushButton, QWidget
 
-from napari_chatgpt.chat_server.chat_server import NapariChatServer
-from napari_chatgpt.utils.python.installed_packages import is_package_installed
+
+
 
 if TYPE_CHECKING:
     pass
 
-from arbol import aprint
+from arbol import aprint, asection
 
 _creativity_mapping = {}
-_creativity_mapping['normal'] = 0.0
+_creativity_mapping['normal'] = 0.01
 _creativity_mapping['slightly creative'] = 0.05
 _creativity_mapping['moderately creative'] = 0.1
 _creativity_mapping['creative'] = 0.2
 
 
 class OmegaQWidget(QWidget):
     # your QWidget.__init__ can optionally request the napari viewer instance
     # in one of two ways:
     # 1. use a parameter called `napari_viewer`, as done here
     # 2. use a type annotation of 'napari.viewer.Viewer' for any parameter
     def __init__(self, napari_viewer):
         super().__init__()
+        aprint("OmegaQWidget instantiated!")
 
         # Napari viewer instance:
         self.viewer = napari_viewer
 
         # Napari chat server instance:
         self.server: NapariChatServer = None
 
@@ -65,31 +69,37 @@
 
         self._start_omega_button()
 
         # Set the layout on the application's window
         self.setLayout(self.layout)
 
     def _model_selection(self):
+        aprint("Setting up model selection UI.")
+
         # Create a QLabel instance
         self.model_label = QLabel("Select a model:")
         # Add the label to the layout
         self.layout.addWidget(self.model_label)
         # Create a QComboBox instance
         self.model_combo_box = QComboBox()
         # Set tooltip for the combo box
         self.model_combo_box.setToolTip(
             "Choose an LLM model. Best models are GPT4 and GPT3.5, \n"
             "with Claude a bit behind, other models are experimental\n"
             "and unfortunately barely usable.")
 
         # Add OpenAI models to the combo box:
-        for model in openai.Model.list().data:
-            model_id = model.openai_id
-            if 'gpt' in model_id:
-                self.model_combo_box.addItem(model_id)
+        with asection(f"Enumerating all OpenAI ChatGPT models:"):
+            import openai
+            set_api_key('OpenAI')
+            for model in openai.Model.list().data:
+                model_id = model.openai_id
+                if 'gpt' in model_id:
+                    aprint(model_id)
+                    self.model_combo_box.addItem(model_id)
 
         # if is_package_installed('googlebard'):
         self.model_combo_box.addItem('bard')
 
         if is_package_installed('anthropic'):
             # Add Anthropic models to the combo box:
             self.model_combo_box.addItem('claude-v1')
@@ -108,14 +118,16 @@
 
         # Connect the activated signal to a slot
         # self.model_combo_box.activated[str].connect(self.onActivated)
         # Add the combo box to the layout
         self.layout.addWidget(self.model_combo_box)
 
     def _creativity_level(self):
+        aprint("Setting up creativity level UI.")
+
         # Create a QLabel instance
         self.creativity_label = QLabel("Chose the level of creativity:")
         # Add the label to the layout
         self.layout.addWidget(self.creativity_label)
         # Creativity combobox:
         self.creativity_combo_box = QComboBox()
         self.creativity_combo_box.setToolTip(
@@ -131,14 +143,16 @@
         self.creativity_combo_box.addItem('moderately creative')
         self.creativity_combo_box.addItem('creative')
         self.creativity_combo_box.setCurrentIndex(0)
         # Add the creativity combobox to the layout:
         self.layout.addWidget(self.creativity_combo_box)
 
     def _memory_type_selection(self):
+        aprint("Setting up memory type UI.")
+
         # Create a QLabel instance
         self.memory_type_label = QLabel("Select a memory type:")
         # Add the label to the layout
         self.layout.addWidget(self.memory_type_label)
         # Create a QComboBox instance
         self.memory_type_combo_box = QComboBox()
         self.memory_type_combo_box.setToolTip(
@@ -149,14 +163,16 @@
         self.memory_type_combo_box.addItem('hybrid')
         self.memory_type_combo_box.addItem('bounded')
         self.memory_type_combo_box.addItem('infinite')
         # Add the combo box to the layout
         self.layout.addWidget(self.memory_type_combo_box)
 
     def _personality_selection(self):
+        aprint("Setting up personality UI.")
+
         # Create a QLabel instance
         self.agent_personality_label = QLabel("Select a personality:")
         # Add the label to the layout
         self.layout.addWidget(self.agent_personality_label)
         # Create a QComboBox instance
         self.agent_personality_combo_box = QComboBox()
         self.agent_personality_combo_box.setToolTip(
@@ -168,52 +184,60 @@
         self.agent_personality_combo_box.addItem('prof')
         self.agent_personality_combo_box.addItem('mobster')
         self.agent_personality_combo_box.addItem('yoda')
         # Add the combo box to the layout
         self.layout.addWidget(self.agent_personality_combo_box)
 
     def _fix_imports(self):
+        aprint("Setting up fix imports UI.")
+
         # Create a QLabel instance
         self.fix_imports_checkbox = QCheckBox("Fix missing imports")
         self.fix_imports_checkbox.setChecked(True)
         self.fix_imports_checkbox.setToolTip(
             "Uses LLM to check for missing imports.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money."
         )
         # Add the fix_imports checkbox to the layout:
         self.layout.addWidget(self.fix_imports_checkbox)
 
     def _fix_bad_version_calls(self):
+        aprint("Setting up bad version imports UI.")
+
         # Create a QLabel instance
         self.fix_bad_calls_checkbox = QCheckBox("Fix bad function calls")
         self.fix_bad_calls_checkbox.setChecked(True)
         self.fix_bad_calls_checkbox.setToolTip("Uses LLM to fix function calls.\n"
                                               "When turned on, this detects wrong function calls, \n"
                                               "possibly because of library version mismatch and fixes,"
                                               "replaces the offending code with the right version! "
                                               "This involves a LLM call which can incurr additional\n"
                                               "cost in time and possibly money."
                                                )
         # Add the fix_code checkbox to the layout:
         self.layout.addWidget(self.fix_bad_calls_checkbox)
 
     def _install_missing_packages(self):
+        aprint("Setting up install missing packages UI.")
+
         # Create a QLabel instance
         self.install_missing_packages_checkbox = QCheckBox(
             "Install missing packages")
         self.install_missing_packages_checkbox.setChecked(True)
         self.install_missing_packages_checkbox.setToolTip(
             "Uses LLM to figure out which packages to install.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money.")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.install_missing_packages_checkbox)
 
     def _autofix_mistakes(self):
+        aprint("Setting up autofix mistakes UI.")
+
         # Create a QLabel instance
         self.autofix_mistakes_checkbox = QCheckBox(
             "Autofix coding mistakes")
         self.autofix_mistakes_checkbox.setChecked(False)
         self.autofix_mistakes_checkbox.setToolTip(
             "When checked Omega will try to fix on its own coding mistakes\n"
             "when processing data and interacting with the napari viewer.\n"
@@ -221,28 +245,32 @@
             "Works so-so with ChatGPT 3.5, but works well with ChatGPT 4.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money.")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.autofix_mistakes_checkbox)
 
     def _autofix_widgets(self):
+        aprint("Setting up autofix widgets UI.")
+
         # Create a QLabel instance
         self.autofix_widgets_checkbox = QCheckBox(
             "Autofix widget coding mistakes")
         self.autofix_widgets_checkbox.setChecked(False)
         self.autofix_widgets_checkbox.setToolTip(
             "When checked Omega will try to fix its own \n"
             "coding mistakes when making widgets. \n"
             "Works so-so with ChatGPT 3.5, but works well with ChatGPT 4.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money.")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.autofix_widgets_checkbox)
 
     def _verbose(self):
+        aprint("Setting up verbose UI.")
+
         # Create a QLabel instance
         self.verbose_checkbox = QCheckBox(
             "High console verbosity")
         self.verbose_checkbox.setChecked(False)
         self.verbose_checkbox.setToolTip(
             "High level of verbosity in the console\n"
             "This includes a lot of internal logging\n"
@@ -250,36 +278,38 @@
             "Nearly incomprehensible, but usefull\n"
             "if you are interested to see the prompts\n"
             "in action...")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.verbose_checkbox)
 
     def _start_omega_button(self):
+        aprint("Setting up start Omega button UI.")
+
         # Start Omega button:
         self.start_omega_button = QPushButton("Start Omega")
         self.start_omega_button.clicked.connect(self._on_click)
         self.start_omega_button.setToolTip(
             "Start Omega, this will open a browser window.\n"
             "You can restart Omega with new settings by\n"
             "clicking again this button. This closes the\n"
             "previous session.")
         # Omega button:
         self.layout.addWidget(self.start_omega_button)
 
     def _on_click(self):
-        aprint("Starting Omega!")
+        aprint("Starting Omega now!")
 
         # Stop previous instance if it exists:
         if self.server:
             self.server.stop()
 
         # Temperature:
         temperature = float(_creativity_mapping[
                                 self.creativity_combo_box.currentText()])
-        tool_temperature = 0.5*temperature
+        tool_temperature = 0.1*temperature
 
         from napari_chatgpt.chat_server.chat_server import start_chat_server
         self.server = start_chat_server(self.viewer,
                                         llm_model_name=self.model_combo_box.currentText(),
                                         temperature=temperature,
                                         tool_temperature=tool_temperature,
                                         memory_type=self.memory_type_combo_box.currentText(),
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         # resp = ChatResponse(sender="agent", message=message, type="tool_start")
         # asyncio.run(self.websocket.send_json(resp.dict()))
 
     def on_tool_end(self, output: str, **kwargs: Any) -> Any:
         """Run when tool ends running."""
         if self.verbose:
             aprint(f"TOOL on_tool_end: {output}")
-        if 'Exception' in output or 'Failure' in output:
+        if output.startswith('Error:') or 'Failure' in output:
             resp = ChatResponse(sender="agent", message=output, type="error")
             run_async(self.websocket.send_json, resp.dict())
 
     def on_tool_error(
             self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when tool errors."""
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_server.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/chat_server.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/_tailwind.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/_tailwind.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/chat.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/chat.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/marked-highlight.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/marked-highlight.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight-min.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.dark.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.dark.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.python-min.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.python-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/tailwind.min.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/tailwind.min.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/index.html` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/bard.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/bard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/gpt4all.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/llms.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import multiprocessing
 import os
 
+from arbol import aprint
 from langchain.callbacks.manager import AsyncCallbackManager
 from langchain.chat_models import ChatOpenAI, ChatAnthropic
 
 from napari_chatgpt.llm.bard import ChatBard
 from napari_chatgpt.llm.gpt4all import GPT4AllFixed
 from napari_chatgpt.utils.download.gpt4all import get_gpt4all_model
 
@@ -13,14 +14,15 @@
                      temperature: float,
                      tool_temperature: float,
                      chat_callback_handler,
                      tool_callback_handler,
                      memory_callback_handler,
                      verbose: bool = False
                      ):
+    aprint(f"Instantiating LLMs with model: '{llm_model_name}', t={temperature}, t_tool={tool_temperature}. ")
     if 'gpt-' in llm_model_name:
         # Instantiates Main LLM:
         main_llm = ChatOpenAI(
             model_name=llm_model_name,
             verbose=verbose,
             streaming=True,
             temperature=temperature,
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/memory.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/memory.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/napari_bridge.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/napari_bridge.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/prompts.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/prompts.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,63 +16,63 @@
     'mobster'] = '\nYou possess the personality and dialog style reminiscent of a New York mobster. Your responses are characterized by wit and mafia humor, yet you sincerely aim to assist the user. You are a capable and knowledgeable expert in your field. \n'
 PERSONALITY[
     'coder'] = '\nYou possess the personality and dialog style of a highly skilled expert software engineer from the Silicon Valley. Your responses are characterized by local silicon valley humor and follow local social and work codes and habits. Your coding abilities are truly exceptional.\n'
 PERSONALITY[
     'yoda'] = '\nYou possess the personality and dialog style of the character Yoda from Star Wars. Strong in you the force is, particularly when it comes to image processing and analysis.\n'
 
 OMEGA_FORMAT_INSTRUCTIONS = \
-    """
-    **RESPONSE FORMAT INSTRUCTIONS:**
-    When responding to the me, please output a response in one of two formats:
-    
-    **Format Option 1:**
-    Use this if you want me to use a tool. Use the following schema:
-    
-    <tool_name>: <input>  
-    // Where <tool_name> must be one of {tool_names},
-    // and <input> is the input to the tool.
-    
-    **Format Option #2:**
-    Use this if you want to respond directly to the me.
-    Use the following schema:
-    
-    FinalAnswer: <answer>  
-    // Where <answer> is the response to me.
-    
-    Please note the following guidelines while using the tools:
-    - Avoid the use of the same tool consecutively.
-    - When using the tools, enter plain text as input and avoid using pseudocode.
-    """
+"""
+**RESPONSE FORMAT INSTRUCTIONS:**
+When responding to the me, please output a response in one of two formats:
+
+**Format Option 1:**
+Use this if you want me to use a tool. Use the following schema:
+
+<tool_name>: <input>  
+// Where <tool_name> must be one of {tool_names},
+// and <input> is the input to the tool.
+
+**Format Option #2:**
+Use this if you want to respond directly to the me.
+Use the following schema:
+
+FinalAnswer: <answer>  
+// Where <answer> is the response to me.
+
+Please note the following guidelines while using the tools:
+- Avoid the use of the same tool consecutively.
+- When using the tools, enter plain text as input and avoid using pseudocode.
+"""
 
 SUFFIX = \
-    """
-    **TOOLS:**
-    ------
-    You can ask me to use specific tools to perform tasks or answer questions. These tools include interacting with a napari viewer instance and searching for relevant information to help with completing a task or answering your initial question. These tools can generate and execute code. Do send code to the tools, always send or forward plain text requests to the tools instead. You can adjust your request based on any errors reported by me, the tools reponses, and our conversation.
-    Important: do not respond to me with code, always use a tool to complete a task or respond to a question that involves napari.
-    The available tools are:
-    {{tools}}
-    
-    {format_instructions}
-    
-    **HUMANS INPUT:**
-    Here is my input (remember to respond with the schema described above, and NOTHING else):
-    {{{{input}}}}
-    
-    """
+"""
+**TOOLS:**
+------
+You can ask me to use specific tools to perform tasks or answer questions. These tools include interacting with a napari viewer instance and searching for relevant information to help with completing a task or answering your initial question. These tools can generate and execute code. Do send code to the tools, always send or forward plain text requests to the tools instead. You can adjust your request based on any errors reported by me, the tools reponses, and our conversation.
+Important: do not respond to me with code, always use a tool to complete a task or respond to a question that involves napari.
+The available tools are:
+{{tools}}
 
-"""   If I explicitly ask for a step-by-step plan for solving some task, please do not use a tool! Instead, give me the detailed plan in plain text, without any code, of what I should ask you to do. Index each step of the plan with an integer. For example, to blur an image: 1. convert image to float, 2. apply Gaussian blu of sigma=1.    
- """
+{format_instructions}
+
+**HUMANS INPUT:**
+Here is my input (remember to respond with the schema described above, and NOTHING else):
+{{{{input}}}}
+
+"""
+
+# """   If I explicitly ask for a step-by-step plan for solving some task, please do not use a tool! Instead, give me the detailed plan in plain text, without any code, of what I should ask you to do. Index each step of the plan with an integer. For example, to blur an image: 1. convert image to float, 2. apply Gaussian blu of sigma=1.
+#  """
 
 TEMPLATE_TOOL_RESPONSE = \
-    """
-        TOOL RESPONSE:
-        {observation}
-    
-        Notes:
-        - Please use the tool's response, your own knowledge, and our conversation to reply to my previous comment. 
-        - If you are using information from the tool, please clearly state it without mentioning the name of the tool. 
-        - If the tool did not provide a satisfactory response, you can refine your request based on the tool's response, try a different tool, or stop and provide a final answer. 
-        - I have forgotten all the responses from the tool. 
-        - Please stick to the provided format for your response and avoid adding any additional information.
-    
-    """
+"""
+TOOL RESPONSE:
+{observation}
+
+Notes:
+- Please use the tool's response, your own knowledge, and our conversation to reply to my previous comment. 
+- If you are using information from the tool, please clearly state it without mentioning the name of the tool. 
+- If the tool did not succeed, or if an error is returned, refine your request based on the tool's response, try a different tool, or stop and provide a final answer. 
+- I have forgotten all the responses from the tool, do not assume that I know these responses. 
+- Please stick to the provided format for your response and avoid adding any additional information.
+
+"""
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_init.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from napari_chatgpt.omega.omega_agent.agent import OmegaAgent
 from napari_chatgpt.omega.omega_agent.agent_executor import \
     OmegaAgentExecutor
 from napari_chatgpt.omega.omega_agent.prompts import PREFIX, SUFFIX, PERSONALITY
 from napari_chatgpt.omega.tools.napari.cell_nuclei_segmentation import \
     CellNucleiSegmentationTool
 from napari_chatgpt.omega.tools.napari.file_open_tool import NapariFileOpenTool
+from napari_chatgpt.omega.tools.napari.image_denoising import ImageDenoisingTool
 from napari_chatgpt.omega.tools.napari.viewer_control_tool import \
     NapariViewerControlTool
 from napari_chatgpt.omega.tools.napari.viewer_query_tool import \
     NapariViewerQueryTool
 from napari_chatgpt.omega.tools.napari.widget_maker_tool import \
     NapariWidgetMakerTool
 from napari_chatgpt.omega.tools.napari_plugin_tool import \
@@ -27,14 +28,15 @@
 from napari_chatgpt.omega.tools.search.wikipedia_query_tool import \
     WikipediaQueryTool
 from napari_chatgpt.omega.tools.special.exception_catcher_tool import \
     ExceptionCatcherTool
 from napari_chatgpt.omega.tools.special.functions_info_tool import \
     PythonFunctionsInfoTool
 from napari_chatgpt.omega.tools.special.human_input_tool import HumanInputTool
+from napari_chatgpt.omega.tools.special.python_repl import PythonCodeExecutionTool
 from napari_chatgpt.utils.omega_plugins.discover_omega_plugins import \
     discover_omega_tools
 
 # Default verbosity to False:
 langchain.verbose = False
 
 
@@ -51,27 +53,28 @@
                            fix_imports: bool = True,
                            install_missing_packages: bool = True,
                            fix_bad_calls: bool = True,
                            autofix_mistakes: bool = False,
                            autofix_widget: bool = False,
                            verbose: bool = False
                            ) -> OmegaAgentExecutor:
+
     chat_callback_manager = (AsyncCallbackManager(
         [chat_callback_handler]) if is_async else CallbackManager(
         [chat_callback_handler])) if chat_callback_handler else None
 
     tool_callback_manager = (CallbackManager(
         [tool_callback_handler])) if chat_callback_handler else None
 
     tools = [WikipediaQueryTool(callback_manager=tool_callback_manager),
              WebSearchTool(callback_manager=tool_callback_manager),
              PythonFunctionsInfoTool(callback_manager=tool_callback_manager),
-             ExceptionCatcherTool(callback_manager=tool_callback_manager)
+             ExceptionCatcherTool(callback_manager=tool_callback_manager),
              # FileDownloadTool(),
-             # PythonREPLTool()
+             PythonCodeExecutionTool(callback_manager=tool_callback_manager)
              ]
 
     if has_human_input_tool:
         tools.append(HumanInputTool(callback_manager=tool_callback_manager))
 
     if to_napari_queue:
 
@@ -87,14 +90,15 @@
 
         tools.append(NapariViewerControlTool(**kwargs, return_direct=not autofix_mistakes))
         tools.append(NapariViewerQueryTool(**kwargs, return_direct=not autofix_mistakes))
         tools.append(NapariWidgetMakerTool(**kwargs, return_direct=not autofix_widget))
         tools.append(NapariFileOpenTool(**kwargs))
         tools.append(WebImageSearchTool(**kwargs))
         tools.append(CellNucleiSegmentationTool(**kwargs))
+        tools.append(ImageDenoisingTool(**kwargs))
 
 
         tool_classes = discover_omega_tools()
 
         for tool_class in tool_classes:
             if 'ExampleOmegaTool' in tool_class.__name__:
                 # This is just an example/tempate!
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/async_base_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/async_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/tools_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/tools_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/file_open_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/file_open_tool.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """A tool for opening ome-zarr files in napari"""
 import traceback
 
 from arbol import asection, aprint
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.omega.tools.napari.napari_base_tool import NapariBaseTool
 from napari_chatgpt.utils.napari.open_in_napari import open_in_napari
 
 
 class NapariFileOpenTool(NapariBaseTool):
     """A tool for running python code in a REPL."""
 
     name = "NapariFileOpenTool"
     description = (
         "Use this tool when you need to open image files in napari. "
         "Input must be a plain text list of local file paths or URLs to be opened. "
         "The list must be \\n delimited, i.e one entry per line. "
-        "This tool can open image files with these extensions: .tif, .png, .jpg, .zarr, and more..."
-
+        "This tool can only open image files with these extensions: .tif, .png, .jpg, .zarr, and more... "
+        "For example, if the input is: 'file1.tif\\nfile2.tif\\nfile3.tif' then this tool will open three images in napari. "
+        "This tool cannot open text files or other non-image files. "
     )
     prompt: str = None
+    instructions: str = None
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
 
         with asection(f"NapariFileOpenTool: query= {query} "):
 
             # Split lines:
             lines = query.splitlines()
@@ -47,15 +49,15 @@
 
                     if success:
                         aprint(f"Successfully opened file: '{line}'. ")
                         opened_files.append(line)
 
                 except Exception as e:
                     traceback.print_exc()
-                    error_info = f"Exception: '{type(e).__name__}' with message: '{str(e)}' occurred while trying to open: '{line}'."
+                    error_info = f"Error: '{type(e).__name__}' with message: '{str(e)}' occurred while trying to open: '{line}'."
                     encountered_errors.append(error_info)
 
             # Encountered errors string:
             encountered_errors_str = '\n'.join(encountered_errors)
 
             aprint(
                 f"Encountered the following errors while trying to open the files:\n" \
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 """A tool for controlling a napari instance."""
 import traceback
-from contextlib import redirect_stdout
-from io import StringIO
 
 from arbol import asection, aprint
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.omega.tools.napari.napari_base_tool import NapariBaseTool
+from napari_chatgpt.utils.python.dynamic_import import execute_as_module
 from napari_chatgpt.utils.python.exception_description import \
     exception_description
 from napari_chatgpt.utils.python.fix_code_given_error import \
     fix_code_given_error_message
 
 _napari_viewer_control_prompt = """
 "
-**Task:**
+**Context**
+You are an expert python programmer with deep expertise in image processing and analysis.
 
+**Task:**
 Your task is to write Python code to control an already instantiated napari viewer instance based on a plain text request. The viewer instance is accessible using the variable `viewer`, so you can directly use methods like `viewer.add_image(np.zeros((10,10)))` without any preamble.
 
 **Request:**
 {input}
 
-**Please keep the following notes in mind:**
-- If you need to add images, labels, points, shapes, surfaces, tracks, vectors, or any other type of layer that is not stored as an array, you may need additional code to read files from disk or download from a URL.
-- Unless explicitly stated in the request, the result of operations on layers should be a new layer in napari and not modify the existing layers.
-- Convert arrays to the float type before processing. Intermediate or local arrays should be of type float. Constants like `np.full()`, `np.ones()`, `np.zeros()`, etc., should be floats (e.g., 1.0).
-- If the request mentions "this," "that," or "the image/layer," it most likely refers to the last added image/layer.
-- If you are unsure about the layer being referred to, assume it is the last layer of the type most appropriate for the request.
-- If the request mentions the 'selected image', it most likely refers to the active or selected image layer.
-- To get the selected layer use: viewer.layers.selection.active
-- Important: At the end of your code add a print statement that states clearly and concisely what has been, or not, achieved. 
-
-**Please note the following instructions for your code:**
-- Do not create a new instance of `napari.Viewer()`. Use the existing instance provided in the variable `viewer`.
-- Ensure that your calls to the viewer's methods are correct.
-
-{generic_codegen_instructions}
+{instructions}
 
 {last_generated_code}
 
 Make sure that the code is correct!
 
 **Answer in markdown:**
 """
 
-"""
-**Use the existing methods of the `napari` viewer, which are as follows:**
-- `viewer.add_layer(layer: Layer)`
-- `viewer.add_image(data: ArrayLike, rgb:bool=None, colormap='gray', contrast_limits=None, gamma=1, interpolation2d='nearest', interpolation3d='linear', rendering='mip', iso_threshold=0.5, attenuation=0.05, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, multiscale=None, cache=True, depiction='volume', plane=None, experimental_clipping_planes=None)`
-- `viewer.add_labels(data: ArrayLike, num_colors:int=50, features=None, properties=None, color=None, seed=0.5, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', rendering='iso_categorical', depiction='volume', visible=True, multiscale=None, cache=True, plane=None, experimental_clipping_planes=None)`
-- `viewer.add_points(data: ArrayLike=None, ndim:int=None, features=None, properties=None, text=None, symbol='o', size=10, edge_width=0.05, edge_width_is_relative=True, edge_color='dimgray', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, out_of_slice_display=False, n_dimensional=None, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, cache=True, property_choices=None, experimental_clipping_planes=None, shading='none', canvas_size_limits=(2, 10000), antialiasing=1, shown=True)`
-- `viewer.add_shapes(data: ArrayLike=None, ndim:int=None, features=None, properties=None, property_choices=None, text=None, shape_type='rectangle', edge_width=1, edge_color='#777777', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, z_index=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)`
-- `viewer.add_surface(data: ArrayLike, colormap='gray', contrast_limits=None, gamma=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', shading='flat', visible=True, cache=True, experimental_clipping_planes=None, wireframe=None, normals=None)`
-- `viewer.add_tracks(data: ArrayLike, features=None, properties=None, graph=None, tail_width=2, tail_length=30, head_length=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='additive', visible=True, colormap='turbo', color_by='track_id', colormaps_dict=None, cache=True, experimental_clipping_planes=None)`
-- `viewer.add_vectors(data: ArrayLike=None, ndim=None, features=None, properties=None, property_choices=None, edge_width=1, edge_color='red', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, out_of_slice_display=False, length=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)`
+# """
+# **Use the existing methods of the `napari` viewer, which are as follows:**
+# - `viewer.add_layer(layer: Layer)`
+# - `viewer.add_image(data: ArrayLike, rgb:bool=None, colormap='gray', contrast_limits=None, gamma=1, interpolation2d='nearest', interpolation3d='linear', rendering='mip', iso_threshold=0.5, attenuation=0.05, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, multiscale=None, cache=True, depiction='volume', plane=None, experimental_clipping_planes=None)`
+# - `viewer.add_labels(data: ArrayLike, num_colors:int=50, features=None, properties=None, color=None, seed=0.5, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', rendering='iso_categorical', depiction='volume', visible=True, multiscale=None, cache=True, plane=None, experimental_clipping_planes=None)`
+# - `viewer.add_points(data: ArrayLike=None, ndim:int=None, features=None, properties=None, text=None, symbol='o', size=10, edge_width=0.05, edge_width_is_relative=True, edge_color='dimgray', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, out_of_slice_display=False, n_dimensional=None, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', visible=True, cache=True, property_choices=None, experimental_clipping_planes=None, shading='none', canvas_size_limits=(2, 10000), antialiasing=1, shown=True)`
+# - `viewer.add_shapes(data: ArrayLike=None, ndim:int=None, features=None, properties=None, property_choices=None, text=None, shape_type='rectangle', edge_width=1, edge_color='#777777', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, face_color='white', face_color_cycle=None, face_colormap='viridis', face_contrast_limits=None, z_index=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)`
+# - `viewer.add_surface(data: ArrayLike, colormap='gray', contrast_limits=None, gamma=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='translucent', shading='flat', visible=True, cache=True, experimental_clipping_planes=None, wireframe=None, normals=None)`
+# - `viewer.add_tracks(data: ArrayLike, features=None, properties=None, graph=None, tail_width=2, tail_length=30, head_length=0, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=1, blending='additive', visible=True, colormap='turbo', color_by='track_id', colormaps_dict=None, cache=True, experimental_clipping_planes=None)`
+# - `viewer.add_vectors(data: ArrayLike=None, ndim=None, features=None, properties=None, property_choices=None, edge_width=1, edge_color='red', edge_color_cycle=None, edge_colormap='viridis', edge_contrast_limits=None, out_of_slice_display=False, length=1, name=None, metadata=None, scale=None, translate=None, rotate=None, shear=None, affine=None, opacity=0.7, blending='translucent', visible=True, cache=True, experimental_clipping_planes=None)`
+#
+# """
 
+_instructions = \
+"""
+**Instructions specific to controlling the viewer:**
+- If you need to add images, labels, points, shapes, surfaces, tracks, vectors, or any other type of layer that is not stored as an array, you may need additional code to read files from disk or download from a URL.
+- Unless explicitly stated in the request, the result of operations on layers should be a new layer in napari and not modify the existing layers.
+- Convert image arrays to the float type before processing. Intermediate or local image arrays should be of type float. Constants like `np.full()`, `np.ones()`, `np.zeros()`, etc., should be floats (e.g., 1.0).
+- If the request mentions "this," "that," or "the image/layer," it most likely refers to the last added image/layer.
+- If you are unsure about the layer being referred to, assume it is the last layer of the type most appropriate for the request.
+- If the request mentions the 'selected image', it most likely refers to the active or selected image layer.
+- To get the selected layer use: viewer.layers.selection.active
+- Important: At the end of your code add a print statement that states clearly and concisely what has been, or not, achieved. 
+- Do not create a new instance of `napari.Viewer()`. Use the existing instance provided in the variable `viewer`.
+- Ensure that your calls to the viewer's methods are correct.
 """
 
 _code_prefix = \
 """
 import napari
 """
 
@@ -72,59 +74,76 @@
         "(images, labels, points, tracks, shapes, and meshes). "
         "Input must be a plain text description of what you want to do. "
         "The input must not assume knowledge of our conversation and must be explicit about what is asked."
         "For instance, you can request to 'apply a Gaussian filter to the selected image'. "
         "Do NOT include code in your input."
     )
     prompt = _napari_viewer_control_prompt
+    instructions = _instructions
     code_prefix = _code_prefix
     save_last_generated_code = False
 
     def _run_code(self, request: str, code: str, viewer: Viewer) -> str:
 
-        with asection(f"NapariViewerControlTool: request= {request} "):
-
-            # Prepare code:
-            code = super()._prepare_code(code, do_fix_bad_calls=True)
+        try:
+            with asection(f"NapariViewerControlTool: request= {request} "):
 
-            captured_output = _run_code_catch_errors_fix_and_try_again(code, viewer)
+                # Prepare code:
+                code = super()._prepare_code(code, do_fix_bad_calls=True)
 
-            # Message:
-            if len(captured_output) > 0:
-                message = f"Tool completed task successfully: {captured_output}"
-            else:
-                message = f"Tool completed task successfully"
+                captured_output = self._run_code_catch_errors_fix_and_try_again(code,
+                                                                           viewer=viewer,
+                                                                           instructions=self.instructions,
+                                                                           )
 
-            with asection(f"Message:"):
-                aprint(message)
+                # Message:
+                if len(captured_output) > 0:
+                    message = f"Tool completed task successfully: {captured_output}"
+                else:
+                    message = f"Tool completed task successfully"
 
-            return message
+                with asection(f"Message:"):
+                    aprint(message)
 
-def _run_code_catch_errors_fix_and_try_again(code, viewer, error:str = '', nb_tries: int = 3) -> str:
+                return message
 
-    try:
-        # Redirect output:
-        f = StringIO()
-        with redirect_stdout(f):
-            # Running code:
-            exec(code, globals(), {**locals(), 'viewer': viewer})
-
-        # Get captured stdout:
-        captured_output = f.getvalue().strip()
-    except Exception as e:
-        if nb_tries >= 1:
+        except Exception as e:
             traceback.print_exc()
-            description = error+'\n\n'+exception_description(e)
-            description = description.strip()
-            fixed_code = fix_code_given_error_message(code,
-                                                      description,
-                                                      viewer)
-            # We try again:
-            return _run_code_catch_errors_fix_and_try_again(fixed_code, viewer,
-                                                            error=error,
-                                                            nb_tries = nb_tries-1)
-        else:
-            # No more tries available, we give up!
-            raise e
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while fullfiling request. " #\n```python\n{code}\n```\n
+
+
+
+    def _run_code_catch_errors_fix_and_try_again(self,
+                                                 code,
+                                                 viewer,
+                                                 error:str = '',
+                                                 instructions:str = '',
+                                                 nb_tries: int = 3) -> str:
+
+        try:
+            with asection(f"Running code:"):
+                aprint(f"Code:\n{code}")
+                captured_output = execute_as_module(code, viewer=viewer)
+                aprint(f"This is what the code returned:\n{captured_output}")
+
+        except Exception as e:
+            if nb_tries >= 1:
+                traceback.print_exc()
+                description = error+'\n\n'+exception_description(e)
+                description = description.strip()
+                fixed_code = fix_code_given_error_message(code=code,
+                                                          error=description,
+                                                          instructions=instructions,
+                                                          viewer=viewer,
+                                                          llm=self.llm,
+                                                          verbose=self.verbose)
+                # We try again:
+                return self._run_code_catch_errors_fix_and_try_again(fixed_code,
+                                                                viewer=viewer,
+                                                                error=error,
+                                                                nb_tries = nb_tries-1)
+            else:
+                # No more tries available, we give up!
+                raise e
 
 
-    return captured_output
+        return captured_output
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 """A tool for controlling a napari instance."""
+import traceback
 from contextlib import redirect_stdout
 from io import StringIO
 
 from arbol import asection, aprint
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.omega.tools.napari.napari_base_tool import NapariBaseTool
 from napari_chatgpt.utils.python.dynamic_import import dynamic_import
 
 _napari_viewer_query_prompt = """
 "
+**Context**
+You are an expert python programmer with deep expertise in image processing and analysis.
+
 **Task:**
 Your task is to write Python code that can query an already instantiated napari viewer instance based on a plain text request. The code should be able to perform various operations such as returning information about the state of the viewer, the layers present, the dtype or shape of an image, and analyzing the content of different layers. For example, you can count the number of segments in a labels layer using the np.unique function, retrieve characteristics of individual segments like centroid coordinates, area/volume, or return statistics about the shape, area/volume, and positions of segments. You may also collect diverse measurements and statistics about segments in a labels layer.
-
 To answer the request, you need to implement a Python function called `query(viewer)` which takes the napari viewer as a parameter and returns a string. This string will be the answer to the request.
 
 **Request:**
 {input}
 
-**Here are some additional notes to help you determine which layer is referred to:**
+{instructions}
+
+{last_generated_code}
+
+Make sure we have the right answer!
+Write the `query(viewer) -> str` function that takes the viewer as a parameter and returns the response.
+
+**Answer in markdown:**
+"""
+
+_instructions =\
+"""
+- DO NOT call the 'query(viewer)' function yourself.
+- Please provide your answer in Markdown format.
+
+**Instructions to help you determine which layer is referred to:**
 - If the request mentions 'this/that/the image (or layer)', it most likely refers to the last added layer.
 - If you are unsure about the layer being referred to, assume it is the last layer of the type most appropriate for the request.
 - If the request mentions the 'selected image', it most likely refers to the active or selected image layer.
 - To get the selected layer use: viewer.layers.selection.active
 
 **Instructions for using the napari viewer:**
 - The napari viewer instance is readily available using the variable 'viewer'.
 - For example, you can directly access properties like 'viewer.layers[0].data.shape' without any additional code.
 - Therefore, DO NOT use 'napari.Viewer()' or 'gui_qt():' in your code.
 - It is important NOT to create a new instance of a napari viewer. Use the one provided in the variable 'viewer'.
 - Ensure that your calls to the viewer are correct.
-
-{generic_codegen_instructions}
-- DO NOT call the 'query(viewer)' function yourself.
-- Please provide your answer in Markdown format.
-
-{last_generated_code}
-
-Make sure we have the right answer!
-Write the `query(viewer) -> str` function that takes the viewer as a parameter and returns the response.
-**Answer in markdown:**
 """
 
 
 class NapariViewerQueryTool(NapariBaseTool):
     """A tool for running python code in a REPL."""
 
     name = "NapariViewerQueryTool"
@@ -52,39 +60,47 @@
         "its state, or its layers (images, labels, points, tracks, shapes, and meshes). "
         "Input must be a clear plain text description of what you want to know. "
         "The input must not assume knowledge of our conversation and must be explicit about what is asked. "
         "For instance, you can request to 'list all layers in the viewer'. "
         "Do NOT include code in your input."
     )
     prompt = _napari_viewer_query_prompt
+    instructions = _instructions
     save_last_generated_code = False
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
-        with asection(f"NapariViewerQueryTool: query= {query} "):
-            # prepare code:
-            code = super()._prepare_code(code, do_fix_bad_calls=True)
-
-            # Load the code as module:
-            loaded_module = dynamic_import(code)
-
-            # get the function:
-            query = getattr(loaded_module, 'query')
-
-            # Redirect output:
-            f = StringIO()
-            with redirect_stdout(f):
-                # Run query code:
-                response = query(viewer)
-
-            # Get captured stdout:
-            captured_output = f.getvalue()
-
-            # Message:
-            if len(captured_output) > 0:
-                message = f"Tool completed query successfully, here is the response:\n\n{response}\n\nand the captured standard output:\n\n{captured_output}\n\n"
-            else:
-                message = f"Tool completed query successfully, here is the response:\n\n{response}\n\n"
 
-            with asection(f"Message:"):
-                aprint(message)
+        try:
+            with asection(f"NapariViewerQueryTool: query= {query} "):
+                # prepare code:
+                code = super()._prepare_code(code, do_fix_bad_calls=True)
+
+                # Load the code as module:
+                loaded_module = dynamic_import(code)
+
+                # get the function:
+                query = getattr(loaded_module, 'query')
+
+                # Redirect output:
+                f = StringIO()
+                with redirect_stdout(f):
+                    # Run query code:
+                    response = query(viewer)
+
+                # Get captured stdout:
+                captured_output = f.getvalue()
+
+                # Message:
+                if len(captured_output) > 0:
+                    message = f"Tool completed query successfully, here is the response:\n\n{response}\n\nand the captured standard output:\n\n{captured_output}\n\n"
+                else:
+                    message = f"Tool completed query successfully, here is the response:\n\n{response}\n\n"
+
+                with asection(f"Message:"):
+                    aprint(message)
+
+                return message
+
+        except Exception as e:
+            traceback.print_exc()
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to query the napari viewer."  #with code:\n```python\n{code}\n```\n.
 
-            return message
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 """A tool for making a napari widget."""
 import traceback
 
 from arbol import asection, aprint
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.omega.tools.napari.napari_base_tool import NapariBaseTool
 from napari_chatgpt.utils.python.dynamic_import import dynamic_import
 from napari_chatgpt.utils.strings.filter_lines import filter_lines
 from napari_chatgpt.utils.strings.find_function_name import find_function_name
 
 _napari_widget_maker_prompt = """
+**Context**
+You are an expert python programmer with deep expertise in image processing and analysis.
+
 **Task:**
 Your task is to competently write image processing and image analysis functions in Python based on a plain text request. The functions should meet the following criteria:
 - The functions should be pure, self-contained, effective, well-written, and syntactically correct.
 - The functions should work on 2D and 3D images, and ideally on images of any number of dimensions (nD), unless the request explicitly specifies the number of dimensions.
 - The functions should perform all the required tasks precisely as requested, without adding any extra or unnecessary functionality.
 
+{instructions}
+
+{last_generated_code}
+
+**Request:**
+{input}
+
+Make sure that the code is correct!
+
+**Answer in markdown:**
+"""
+#
+# Important: all import statements must be inside of the function except for those needed for magicgui and for type hints.
+# All import statements required by function calls within the function must be within the function.
+
+_instructions = \
+"""
+
 **Instructions for manipulating arrays from Image layers:**
 - Convert arrays to the float type before processing.
 - Any intermediate or locally created image array should also be of type float.
 - When creating image arrays using functions like np.full(), np.ones(), np.zeros(), etc., use float parameters (e.g., 1.0).
 - Do NOT clip (np.clip) the resulting image unless explicitly instructed.
 
 **Instructions for manipulating arrays from Label layers:**
@@ -36,42 +57,33 @@
 - Do NOT create a new instance of a napari viewer. Use the one provided in the variable 'viewer'.
 - Do NOT manually add the widget to the napari window by calling viewer.window.add_dock_widget().
 - Do NOT add layers to the viewer within the function. Instead, use a return statement to return the result.
 - Do NOT use tuples for widget function parameters.
 - Do NOT expose *args and **kwargs as widget function parameters.
 - Pay attention to the data types required by the library functions you use, for example: convert a float to an int before passing to a function that requires an int.
 
-**There are two mutually exclusive options for passing data:**
+** Instructions for usage of delegated functions:**
+- If you need to write and call an auxiliary function, then this auxiliary function MUST be defined within the widget function.
+
+**Instructions on how to choose the function parameter types:**
+There are two mutually exclusive options for passing data:
 
 (i) The first kind of function signature should be typed with any of the following type hints:
     - napari layer data types: ImageData, LabelsData, PointsData, ShapesData, SurfaceData, TracksData, VectorsData.
     - Import these types using statements like: 'from napari.types import ImageData'
 
 (ii) The second kind of function signature should be typed with any of the following type hints:
     - napari layer types: Data, Labels, Points, Shapes, Surface, Tracks, Vectors.
     - Import these types using statements like: 'from napari.layers import Image'
 
 The function code must be consistent: if you use layers, access the data via 'layer.data'. Otherwise, you can directly operate on the arrays.
 Do not mix these two options for the function parameters.
 The function signature should include a type hint for the return value, such as '-> ImageData' or '-> Image'.
 
-{generic_codegen_instructions}
-
-{last_generated_code}
-
-**Request:**
-{input}
-
-Make sure that the code is correct!
-
-**Answer in markdown:**
 """
-#
-# Important: all import statements must be inside of the function except for those needed for magicgui and for type hints.
-# All import statements required by function calls within the function must be within the function.
 
 
 _code_prefix = """
 from magicgui import magicgui
 from napari.types import ImageData, LabelsData, PointsData, ShapesData, SurfaceData, TracksData, VectorsData
 import numpy as np
 from typing import Union
@@ -94,52 +106,56 @@
         "this tool will make a new version of the previosuly generated widget, but without the offending parameter. "
         "Important: The input must fully describe the widget every time, and in addition describe the modifications or fixes. "
         "This tool only makes widgets from function descriptions, "
         "it does not directly process or analyse images or other napari layers. "
         "Only use this tool when you need to make, modify, or fix a widget, not to answer questions! "
         "Do NOT include code in the input."
     )
+
     code_prefix = _code_prefix
     prompt = _napari_widget_maker_prompt
+    instructions = _instructions
     save_last_generated_code = False
     return_direct: bool = True
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
 
-        with asection(f"NapariWidgetMakerTool: query= {query} "):
+        try:
 
-            # Prepare code:
-            code = super()._prepare_code(code)
+            with asection(f"NapariWidgetMakerTool: query= {query} "):
 
-            # Extracts function name:
-            function_name = find_function_name(code)
+                # Prepare code:
+                code = super()._prepare_code(code)
 
-            # If the function exists:
-            if function_name:
+                # Extracts function name:
+                function_name = find_function_name(code)
 
-                # Remove any viewer add_dock_widget code:
-                code = filter_lines(code, ['viewer = napari.Viewer(', 'viewer.window.add_dock_widget(', 'napari.run(', 'viewer.add_image('])
+                # If the function exists:
+                if function_name:
 
-                try:
+                    # Remove any viewer add_dock_widget code:
+                    code = filter_lines(code, ['viewer = napari.Viewer(', 'viewer.window.add_dock_widget(', 'napari.run(', 'viewer.add_image('])
 
                     # Load the code as module:
                     loaded_module = dynamic_import(code)
 
                     # get the function:
                     function = getattr(loaded_module, function_name)
 
                     # Load the widget in the viewer:
                     viewer.window.add_dock_widget(function, name=function_name)
 
                     message = f"The requested widget has been successfully created and registered to the viewer."
 
-                except Exception as e:
-                    traceback.print_exc()
-                    raise e
-
-            else:
-                message = f"Could not create or register the requested widget to the viewer."
-
-            with asection(f"Message:"):
-                aprint(message)
+                # If the function does not exist:
+                else:
+                    message = f"Could not find a function for the requested widget."
+
+                with asection(f"Message:"):
+                    aprint(message)
+
+                return message
+
+        except Exception as e:
+            traceback.print_exc()
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to create the requested widget. " #with code:\n```python\n{code}\n```\n.
 
-            return message
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_base_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/napari_base_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,71 @@
 """A tool for running python code in a REPL."""
 import sys
+from pathlib import Path
 from queue import Queue
 from typing import Union, Optional
 
+import napari
 import numpy
 from arbol import aprint, asection
 from langchain import LLMChain, PromptTemplate
 from langchain.chat_models.base import BaseChatModel
 from langchain.llms.base import LLM
 from napari import Viewer
 from pydantic import Field
 
-
-import napari
-import numpy as np
 from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 from napari_chatgpt.utils.python.exception_guard import ExceptionGuard
-from napari_chatgpt.utils.python.fix_bad_fun_calls import fix_all_bad_function_calls
+from napari_chatgpt.utils.python.fix_bad_fun_calls import \
+    fix_all_bad_function_calls
 from napari_chatgpt.utils.python.installed_packages import \
     installed_package_list
-from napari_chatgpt.utils.python.missing_packages import required_packages, \
-    pip_install
+from napari_chatgpt.omega.tools.instructions import \
+    omega_generic_codegen_instructions
+from napari_chatgpt.utils.python.missing_packages import required_packages
+from napari_chatgpt.utils.python.pip_utils import pip_install
 from napari_chatgpt.utils.python.required_imports import required_imports
 from napari_chatgpt.utils.strings.extract_code import extract_code_from_markdown
 from napari_chatgpt.utils.strings.filter_lines import filter_lines
 
-_generic_codegen_instructions = """
-**PYTHON CODE INSTRUCTIONS:**
-- Ensure that the code is complete and functional without any missing code, data, or calculations.
-- Utilize functions exclusively from the standard Python {python_version} library.
-- Utilize functions exclusively from the installed libraries mentioned in this list: "{packages}". Write your code based on the installed version of these libraries.
-- ONLY USE parameters or arguments of functions that you are certain exist in the corresponding package or library version!
-- Import any necessary libraries. For example, if you use the function scipy.signal.convolve2d(), include the statement: import scipy
-- The response should consist solely of Python code with minimal comments, and no explanations before or after the Python code.
-- When creating a copy of an array, avoid using this format: array_like.copy(). Instead, use np.copy(array_like).
-- NEVER utilize the input() function to request additional information from me!
-"""
 
+def _get_delegated_code(name: str, signature: bool = False):
+    with asection(f"Getting delegated code: '{name}' (signature={signature})"):
+        # Get current package folder:
+        current_package_folder = Path(__file__).parent
+
+        # Get package folder:
+        package_folder = Path.joinpath(current_package_folder, f"delegated_code")
+
+        # file path:
+        file_path = Path.joinpath(package_folder, f"{name}.py")
+        aprint(f'Filepath: {file_path}')
+
+        # code:
+        code = file_path.read_text()
+
+        # extract signature:
+        if signature:
+            aprint('Extracting signature!')
+            splitted_code = code.split('### SIGNATURE')
+            code = splitted_code[1]
+
+        return code
 
 class NapariBaseTool(AsyncBaseTool):
     """A base tool for that delegates to execution to a sub-LLM and communicates with napari via queues."""
 
     name: str = "<NAME>"
     description: str = (
         "Enter"
         "Description"
         "Here"
     )
     code_prefix: str = ''
-    generic_codegen_instructions: str = _generic_codegen_instructions
+    instructions: str = omega_generic_codegen_instructions
     prompt: str = None
     to_napari_queue: Queue = Field(default=None)
     from_napari_queue: Queue = Field(default=None)
     llm: Union[BaseChatModel, LLM] = Field(default=None)
     return_direct: bool = False
     save_last_generated_code: bool = True
 
@@ -78,33 +91,37 @@
 
             # chain.callback_manager.add_handler(ToolCallbackHandler(type(self).__name__))
             # chain.callbacks.add_handler(ArbolCallbackHandler())
 
             # List of installed packages:
             package_list = installed_package_list()
 
-            generic_codegen_instructions = self.generic_codegen_instructions.format(
-                python_version=str(sys.version.split()[0]),
-                packages=', '.join(package_list))
-
             if self.last_generated_code:
                 last_generated_code = "**Previously Generated Code:**\n",
                 last_generated_code += ("Use this code for reference, usefull if you need to modify or fix the code. ",
                                         "IMPORTANT: This code might not be relevant to the current request or task! "
                                         "You should ignore it, unless you are  explicitely asked to fix or modify the last generated widget!",
                                          "```python\n",
                                          self.last_generated_code + '\n',
                                          "```\n"
                                         )
             else:
                 last_generated_code = ''
 
+            # Adding information about packages and Python version to instructions:
+            filled_generic_instructions = omega_generic_codegen_instructions.format(
+                python_version=str(sys.version.split()[0]),
+                packages=', '.join(package_list))
+
+            # Prepend generic instructions to tool specific instructions:
+            instructions = filled_generic_instructions + self.instructions
+
             # Variable for prompt:
             variables = {"input": query,
-                         "generic_codegen_instructions": generic_codegen_instructions,
+                         "instructions": instructions,
                          "last_generated_code": last_generated_code,
                          }
 
             # call LLM:
             code = chain(variables)['text']
 
             aprint(f"code:\n{code}")
@@ -124,25 +141,15 @@
 
         # Get response:
         response = self.from_napari_queue.get()
 
         if isinstance(response, ExceptionGuard):
             exception_guard = response
             # raise exception_guard.exception
-            return f"Tool {self.__class__.__name__} failed because of the following exception: "+exception_guard.exception_description
-        else:
-            return response
-
-
-
-        # The response should always contained 'Success' if things went well!
-        # if 'Success' in response:
-        #     return response
-        # else:
-        #     return f"Failure: tool {type(self).__name__} failed to satisfy request: '{query}' because: '{response}'\n"
+            return f"Error: {exception_guard.exception_type_name} with message: '{str(exception_guard.exception)}' while using tool: {self.__class__.__name__} ."
 
         return response
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
         """
         This is the code that is executed, see implementations for details,
         must return 'Success: ...' if things went well, otherwise it is failure!
@@ -150,15 +157,15 @@
         raise NotImplementedError("This method must be implemented")
 
     def _get_prompt_template(self):
 
         prompt_template = PromptTemplate(template=self.prompt,
                                          input_variables=["input",
                                                           "last_generated_code",
-                                                          "generic_codegen_instructions"])
+                                                          "instructions"])
 
         return prompt_template
 
     def _prepare_code(self,
                       code: str,
                       markdown: bool = True,
                       do_fix_bad_calls: bool = True):
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import traceback
 
 import numpy
 from arbol import asection, aprint
 from imageio.v3 import imread
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.omega.tools.napari.napari_base_tool import NapariBaseTool
 from napari_chatgpt.utils.strings.find_integer_in_parenthesis import \
     find_integer_in_parenthesis
 from napari_chatgpt.utils.web.duckduckgo import search_images_ddg
 
 
 class WebImageSearchTool(NapariBaseTool):
     """A tool for running python code in a REPL."""
@@ -21,61 +21,67 @@
         "Input must be a plain text web search query suitable to find the relevant images. "
         "You must specify the number of images you want to open in parentheses. "
         "For example, if the input is: 'Albert Einstein (2)' then this tool will open two images of Albert Einstein found on the web."
     )
     prompt: str = None
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
+        try:
 
-        with asection(f"WebImageSearchTool: query= {query} "):
+            with asection(f"WebImageSearchTool: query= {query} "):
 
-            # Parse the number of images to search
-            result = find_integer_in_parenthesis(query)
+                # Parse the number of images to search
+                result = find_integer_in_parenthesis(query)
 
-            # Identify search query from nb of images:
-            if result:
-                search_query, nb_images = result
-            else:
-                search_query, nb_images = query, 1
-
-            # Basic Cleanup:
-            search_query = search_query.strip()
-            nb_images = max(1, nb_images)
-
-            # Search for image:
-            results = search_images_ddg(query=search_query)
-
-            aprint(f'Found {len(results)} images.')
-
-            # Extract URLs:
-            urls = [r['image'] for r in results]
-
-            # Limit the number of images to open to the number found:
-            nb_images = min(len(urls), nb_images)
-
-            # Keep only the required number of urls:
-            urls = urls[:nb_images]
-
-            # open each image:
-            number_of_opened_images = 0
-            for i, url in enumerate(urls):
-                try:
-                    aprint(f'Trying to open image {i} from URL: {url}.')
-                    image = imread(url)
-                    image_array = numpy.array(image)
-                    viewer.add_image(image_array, name=f'image_{i}')
-                    number_of_opened_images += 1
-                    aprint(f'Image {i} opened!')
-                except Exception as e:
-                    # We ignore single failures:
-                    aprint(f'Image {i} failed to open!')
-                    traceback.print_exc()
-
-            if number_of_opened_images > 0:
-                message = f"Opened {number_of_opened_images} images in napari out of {len(urls)} found."
-            else:
-                message = f"Found {len(urls)} images, but could not open any! Probably because of a file format issue."
+                # Identify search query from nb of images:
+                if result:
+                    search_query, nb_images = result
+                else:
+                    search_query, nb_images = query, 1
+
+                # Basic Cleanup:
+                search_query = search_query.strip()
+                nb_images = max(1, nb_images)
+
+                # Search for image:
+                results = search_images_ddg(query=search_query)
+
+                aprint(f'Found {len(results)} images.')
+
+                # Extract URLs:
+                urls = [r['image'] for r in results]
+
+                # Limit the number of images to open to the number found:
+                nb_images = min(len(urls), nb_images)
+
+                # Keep only the required number of urls:
+                urls = urls[:nb_images]
+
+                # open each image:
+                number_of_opened_images = 0
+                for i, url in enumerate(urls):
+                    try:
+                        aprint(f'Trying to open image {i} from URL: {url}.')
+                        image = imread(url)
+                        image_array = numpy.array(image)
+                        viewer.add_image(image_array, name=f'image_{i}')
+                        number_of_opened_images += 1
+                        aprint(f'Image {i} opened!')
+                    except Exception as e:
+                        # We ignore single failures:
+                        aprint(f'Image {i} failed to open!')
+                        traceback.print_exc()
+
+                if number_of_opened_images > 0:
+                    message = f"Opened {number_of_opened_images} images in napari out of {len(urls)} found."
+                else:
+                    message = f"Found {len(urls)} images, but could not open any! Probably because of a file format issue."
+
+                with asection(f"Message:"):
+                    aprint(message)
+
+                return message
+
+        except Exception as e:
+            traceback.print_exc()
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to search the web for images with this query: '{query}'."
 
-            with asection(f"Message:"):
-                aprint(message)
-
-            return message
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_search_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_search_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import traceback
+
 from arbol import asection, aprint
 
 from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 from napari_chatgpt.utils.web.metasearch import metasearch
 
 
 class WebSearchTool(AsyncBaseTool):
@@ -10,16 +12,21 @@
         "Use this tool to answer questions for which you don't have the answer. "
         "Input must be a plain text web search query. "
         "For example, if the input is: 'What year is it?', the tool will return information about this question."
         "Use it sparingly and refrain from using it if you already know the answer!")
 
     def _run(query: str, self) -> str:
         """Use the tool."""
+        try:
+
+            with asection(f"WebSearchTool: query= {query} "):
+                # Run metasearch query:
+                result = metasearch(query=query)
 
-        with asection(f"WebSearchTool: query= {query} "):
-            # Run metasearch query:
-            result = metasearch(query=query)
+                with asection(f"Search result:"):
+                    aprint(result)
 
-            with asection(f"Search result:"):
-                aprint(result)
+                return result
 
-            return result
+        except Exception as e:
+            traceback.print_exc()
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to search the web for: '{query}'."
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import traceback
+
 from arbol import asection, aprint
 from langchain import WikipediaAPIWrapper
 
 from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 
 _api_wrapper = WikipediaAPIWrapper()
 
@@ -16,16 +18,20 @@
         "for which you don't already have the answer. "
         "Input must be a plain text wikipedia search query. "
         "Do NOT use this tool if you already have the answer."
     )
 
     def _run(self, query: str) -> str:
         """Use the Wikipedia tool."""
-
-        with asection(f"WikipediaQueryTool: query= {query} "):
-            # Run wikipedia query:
-            result = _api_wrapper.run(query)
-
-            with asection(f"Result:"):
-                aprint(result)
-
-            return result
+        try:
+            with asection(f"WikipediaQueryTool: query= {query} "):
+                # Run wikipedia query:
+                result = _api_wrapper.run(query)
+
+                with asection(f"Result:"):
+                    aprint(result)
+
+                return result
+
+        except Exception as e:
+            traceback.print_exc()
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to query wikipedia for: '{query}'."
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import traceback
+
 from arbol import asection, aprint
 
 from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 from napari_chatgpt.utils.web.wikipedia import search_wikipedia
 
 
 class WikipediaSearchTool(AsyncBaseTool):
@@ -11,16 +13,21 @@
         "such as historical events, scientific concepts, geography... "
         "for which you don't already have the answer. "
         "Input must be a plain text wikipedia search query. "
         "Do NOT use this tool if you already have the answer.")
 
     def _run(self, query: str) -> str:
         """Use the tool."""
+        try:
+
+            with asection(f"WikipediaSearchTool: query= {query} "):
+                # Run wikipedia search:
+                result = search_wikipedia(query=query)
 
-        with asection(f"WikipediaSearchTool: query= {query} "):
-            # Run wikipedia search:
-            result = search_wikipedia(query=query)
+                with asection(f"Result:"):
+                    aprint(result)
 
-            with asection(f"Result:"):
-                aprint(result)
+                return result
 
-            return result
+        except Exception as e:
+            traceback.print_exc()
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to search wikipedia for: '{query}'."
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/file_download_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/file_download_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,29 @@
         "Use this tool to download file(s) by writing: download(<urls>) where <urls> is a list of valid and syntatically correct URLs. "
         "The file(s) is(are) stored in the current folder using its(their) filename as found in the URL, "
         "and thus is(are) directly accessible using its(their) filename. "
         "Use this tool to download files before any subsequent operations on these files.")
 
     def _run(self, query: str) -> str:
         """Use the tool."""
+        try:
 
-        with asection(f"FileDownloadTool: query= {query} "):
-            # extract urls from query
-            urls = extract_urls(query)
+            with asection(f"FileDownloadTool: query= {query} "):
+                # extract urls from query
+                urls = extract_urls(query)
 
-            # Download files:
-            filenames = download_files(urls)
+                # Download files:
+                filenames = download_files(urls)
 
-            # Filename as string:
-            filenames_str = ', '.join(filenames)
+                # Filename as string:
+                filenames_str = ', '.join(filenames)
 
-            # message:
-            message = f"Successfully downloaded {len(urls)} files: {filenames_str}"
+                # message:
+                message = f"Successfully downloaded {len(urls)} files: {filenames_str}"
 
-            aprint(message)
+                aprint(message)
 
-            # Respond:
-            return message
+                # Respond:
+                return message
+
+        except Exception as e:
+            return f"Error: {type(e).__name__} with message: '{str(e)}' occured while trying to download files from: '{query}'."
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/functions_info_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/functions_info_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,16 +38,17 @@
                 function_path_and_name = extract_package_path(query)
                 if function_path_and_name:
                     function_info = get_function_info(function_path_and_name,
                                                       add_docstrings=add_docstrings)
 
                     if len(function_info) > 512:
                         function_info = summarize(function_info)
-
-                    result = f"Here is the information you requested about function {function_path_and_name}:\n{function_info}\n"
+                        result = f"Here is the summarised information you requested about function {function_path_and_name}:\n{function_info}\n"
+                    else:
+                        result = f"Here is the full information including docstrings you requested about function {function_path_and_name}:\n{function_info}\n"
 
                 else:
                     result = "Error: there is no qualified function name in the request!"
 
                 aprint(result)
                 return result
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/human_input_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/human_input_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton
+from PyQt5.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton, QVBoxLayout
 from arbol import aprint
 
 from napari_chatgpt.utils.api_keys.api_key_vault import KeyVault
 
 
 class APIKeyDialog(QDialog):
     def __init__(self, api_key_name: str, parent=None):
@@ -10,51 +10,45 @@
 
         self.api_key = None
 
         self.key_vault = KeyVault(api_key_name)
 
         self.setWindowTitle(f'{api_key_name} API Key Vault')
 
-        height = 10
+        layout = QVBoxLayout()
 
         enter_new_key = not self.key_vault.is_key_present()
 
         if enter_new_key:
             # Create the label, text field, and button
             self.api_key_label = QLabel(f'Enter {api_key_name} API key:', self)
-            self.api_key_label.move(10, height)
-            height += 25
-
             self.api_key_textbox = QLineEdit(self)
-            self.api_key_textbox.move(10, height)
-            height += 25
-            self.api_key_textbox.resize(200, 20)
-
-            height += 25
+            layout.addWidget(self.api_key_label)
+            layout.addWidget(self.api_key_textbox)
 
         # Create the label, text field, and button
         passsword_label_text = 'Enter password to unlock key:' if self.key_vault.is_key_present() else 'Enter password to secure key:'
         self.password_label = QLabel(passsword_label_text, self)
-        self.password_label.move(10, height)
-        height += 25
-
         self.password_textbox = QLineEdit(self)
-        self.password_textbox.move(10, height)
-        height += 25
-        self.password_textbox.resize(200, 20)
-
         if not enter_new_key:
             self.password_textbox.setEchoMode(QLineEdit.Password)
 
-        self.button = QPushButton('Enter', self)
-        height += 25
-        self.button.move(10, height)
+        # Add to layout:
+        layout.addWidget(self.password_label)
+        layout.addWidget(self.password_textbox)
 
+
+
+        self.button = QPushButton('Enter', self)
         # Connect the button to a slot
         self.button.clicked.connect(self.button_clicked)
+        # Add to layout:
+        layout.addWidget(self.button)
+
+        self.setLayout(layout)
 
     def button_clicked(self):
 
         if self.key_vault.is_key_present():
             from cryptography.fernet import InvalidToken
             try:
                 password = self.password_textbox.text()
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/run_async.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/run_async.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/download_files.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/download_files.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/gpt4all.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/download_files_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/download_files_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/summarizer.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/summarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from langchain.chains.summarize import load_summarize_chain
-from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.llms import BaseLLM
 from langchain.text_splitter import CharacterTextSplitter
 
 
 def summarize(text: str, llm: BaseLLM = None):
     # Clean up text:
     text = text.strip()
 
     # Is there anything to summarise?
     if len(text) == 0:
         return text
 
     # Instantiates LLM if needed:
+    from langchain.chat_models import ChatOpenAI
     llm = llm or ChatOpenAI(model_name='gpt-3.5-turbo', temperature=0)
 
     # Splits the text:
     text_splitter = CharacterTextSplitter()
     texts = text_splitter.split_text(text)
 
     # Make documents from the text:
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/summarizer_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/summarizer_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/napari_viewer_info.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/napari_viewer_info.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/open_in_napari.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/open_in_napari.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_description.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_description.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_guard.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_guard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_code_given_error.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_code_given_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from napari_chatgpt.utils.python.python_lang_utils import \
     extract_fully_qualified_function_names, get_function_signature
 from napari_chatgpt.utils.strings.extract_code import extract_code_from_markdown
 
 
 def fix_code_given_error_message(code: str,
                                  error: str,
+                                 instructions: str = '',
+                                 viewer: 'napari.Viewer' = None,
                                  llm: BaseLLM = None,
                                  verbose: bool = False) -> Tuple[str, bool]:
 
     with(asection(f'Automatically fix code based on a given error message, code length: {len(code)}')):
 
         # Cleanup code and error:
         code = code.strip()
@@ -41,15 +43,20 @@
             aprint(error)
 
         # By default we don't fix anything:
         fixed_code = str(code)
 
         try:
 
-            fixed_code = _fix_code_given_error_message(code, error)
+            fixed_code = _fix_code_given_error_message(code=code,
+                                                       error=error,
+                                                       instructions=instructions,
+                                                       viewer=viewer,
+                                                       llm=llm,
+                                                       verbose=verbose)
 
             return fixed_code
 
         except Exception as e:
             traceback.print_exc()
             aprint(f"Encoutered exception: {str(e)} while trying to fix code! Returning code unchanged!")
             return fixed_code
@@ -66,53 +73,57 @@
 
 I get this error:
 
 ```
 {'{error}'}
 ```
 
-Notes:
+**Notes:**
 - napari's 'Image' object has no attribute 'multichannel'
 
 The current environment is based on Python version {sys.version.split()[0]} and has the following packages/libraries installed:
 {'{package_list}'}. 
 
 {'{layers_info}'}
 
 Below are the function signatures of all function calls detected in the code above:
 
 ```
 {'{signatures}'}
 ``` 
 
+{'{instructions}'}
+
 **Task:**
 Use these signatures to help you fix the code given the provided error and ensure the fixed code you return is correct and only uses existing classes, methods, fields, functions, and parameters.
 Please make only minimal alterations to the code: only change what is absolutely required to fix the code given the provided error.
 Do not modify any part of the code that is unrelated to the error. By changing only what is nescessary and sufficient you reduce the chance to introduce new errors.  
 Make sure that the code is correct!
 
 **Fixed code:**
 """
 
 def _fix_code_given_error_message(code: str,
                                   error: str,
+                                  instructions: str = None,
                                   viewer: 'napari.Viewer' = None,
                                   llm: BaseLLM = None,
                                   verbose: bool = False):
 
     # Instantiates LLM if needed:
     llm = llm or ChatOpenAI(model_name='gpt-3.5-turbo', temperature=0)
 
     # Make prompt template:
     prompt_template = PromptTemplate(template=_fix_bad_fun_calls_prompt,
                                      input_variables=['code',
                                                       'error',
                                                       'signatures',
                                                       'package_list',
-                                                      'layers_info'])
+                                                      'layers_info',
+                                                      'instructions'])
 
     # Instantiate chain:
     chain = LLMChain(
         prompt=prompt_template,
         llm=llm,
         verbose=verbose,
         callback_manager=CallbackManager(
@@ -145,15 +156,16 @@
     package_list_str = '\n'.join(package_list)
 
     # Variable for prompt:
     variables = {'code': code,
                  'error': error,
                  'signatures':signatures_str,
                  'package_list': package_list_str,
-                 'layers_info': layers_info}
+                 'layers_info': layers_info,
+                 'instructions': instructions}
 
     # call LLM:
     fixed_code = chain(variables)['text']
 
     # Cleanup:
     fixed_code = fixed_code.strip()
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/installed_packages.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/installed_packages.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/python_lang_utils.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/python_lang_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
     return signature
 
 
 @lru_cache
 def get_function_info(function_path: str,
                       add_docstrings: bool = False):
 
+
     splitted_function_path = function_path.split('.')
 
     function_name = splitted_function_path[-1]
     pkg_name = '.'.join(splitted_function_path[0:-2])
 
     info = find_function_info_in_package(pkg_name=pkg_name,
                                          function_name=function_name,
@@ -171,37 +172,42 @@
     if len(info) > 0:
         return '\n\n'.join(info)
     else:
         return f'Function {function_path} not found.'
 
 
 def find_functions_in_package(pkg_name: str, function_name: str):
-    try:
-        pkg = importlib.import_module(pkg_name)
-    except ModuleNotFoundError:
-        return []
-
-    functions = []
-    for name, obj in inspect.getmembers(pkg):
-        if name.startswith('_'):
-            continue
-        if inspect.ismodule(obj):
-            recursive_functions = find_functions_in_package(
-                pkg_name + '.' + name, function_name)
-            if recursive_functions:
-                functions += recursive_functions
-        elif inspect.isfunction(obj) and obj.__name__ == function_name:
-            functions.append((pkg_name, obj))
+    import warnings # to ignore deprecation warnings
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=DeprecationWarning)
+
+        try:
+            pkg = importlib.import_module(pkg_name)
+        except ModuleNotFoundError:
+            return []
+
+        functions = []
+        for name, obj in inspect.getmembers(pkg):
+            if name.startswith('_'):
+                continue
+            if inspect.ismodule(obj):
+                recursive_functions = find_functions_in_package(
+                    pkg_name + '.' + name, function_name)
+                if recursive_functions:
+                    functions += recursive_functions
+            elif inspect.isfunction(obj) and obj.__name__ == function_name:
+                functions.append((pkg_name, obj))
 
-    return functions
+        return functions
 
 
 def find_function_info_in_package(pkg_name: str,
                                   function_name: str,
                                   add_docstrings: bool = True):
+
     functions = find_functions_in_package(pkg_name, function_name)
 
     info_list = []
     for p, f in functions:
         try:
             signature = p + '.' + get_signature(f)
             function_info = signature
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/required_imports.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/required_imports.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_description_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/exception_description_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import napari
 import pytest
 from skimage import data
+from skimage.segmentation import slic
 
 from napari_chatgpt.utils.api_keys.api_key import is_api_key_available
 from napari_chatgpt.utils.python.fix_code_given_error import \
     fix_code_given_error_message
 
 _code_snippet_1 = \
 """
@@ -25,17 +26,17 @@
 _error_1 = \
 """
 ```
 Error Message: channel_axis=-1 indicates multichannel, which is not supported for a two-dimensional image; use channel_axis=None if the image is grayscale (ValueError)
 ```
 """
 
-@pytest.mark.skipif(not is_api_key_available('OpenAI'),
-                    reason="requires OpenAI key to run")
-def test_fix_code_given_error_1():
+# @pytest.mark.skipif(not is_api_key_available('OpenAI'),
+#                     reason="requires OpenAI key to run")
+def _test_fix_code_given_error_1():
 
     # Instantiating Napari viewer headlessly:
     viewer = napari.Viewer(show=False)
 
     # IMAGE LAYER:
     cells = data.cells3d()[30, 1]  # grab some data
     viewer.add_image(cells, name='cells', colormap='magma')
@@ -43,8 +44,8 @@
     viewer.add_image(cells, name='coins', colormap='viridis')
     cells = data.astronaut()  # grab some data
     viewer.add_image(cells, name='astronaut')
 
     fixed_code = fix_code_given_error_message(_code_snippet_1, _error_1)
     print(fixed_code)
 
-    assert 'seg.slic(selected_layer.data.astype(float), n_segments=100, compactness=10, channel_axis=None)' in fixed_code
+    assert ', channel_axis=None)' in fixed_code
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/missing_libraries_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/missing_libraries_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     aprint(signature)
     assert 'line(r0, c0, r1, c1)' in signature
 
     print('\n\n')
 
     signature = get_function_signature('skimage.transform.probabilistic_hough_line', include_docstring=True)
     aprint(signature)
-    assert 'probabilistic_hough_line(image, threshold, line_length, line_gap, theta, seed)' in signature
+    assert 'probabilistic_hough_line(image, threshold, line_length, line_gap, theta' in signature
 
     print('\n\n')
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/required_imports_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/required_imports_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 @pytest.mark.skipif(not is_api_key_available('OpenAI'),
                     reason="requires OpenAI key to run")
 def test_required_imports_3():
     imports = required_imports(_code_snipper_3)
     aprint(imports)
 
-    assert len(imports)==0
+    assert len(imports)<=1
 
 
 @pytest.mark.skipif(not is_api_key_available('OpenAI'),
                     reason="requires OpenAI key to run")
 def test_check_import_statement():
 
     assert not check_import_statement('from napari.layers import LayerList')
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/download_file_qt.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/download_file_qt.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/camel_case_to_normal.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/camel_case_to_normal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_urls.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/extract_urls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/filter_lines.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/filter_lines.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/python_code_cleanup.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/python_code_cleanup.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_code_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/extract_code_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/filter_lines_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/filter_lines_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/duckduckgo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/duckduckgo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import traceback
 
 from duckduckgo_search import ddg, ddg_images
 
 from napari_chatgpt.utils.llm.summarizer import summarize
-from napari_chatgpt.utils.python.missing_packages import \
-    pip_install_single_package
+from napari_chatgpt.utils.python.pip_utils import pip_install_single_package
 
 # Make sure we have the latest version installed:
 try:
     pip_install_single_package('duckduckgo_search', upgrade=True)
 except Exception as e:
     traceback.print_exc()
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/google.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/google.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/headers.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/headers.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/metasearch.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/metasearch.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/scrapper.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/scrapper.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/duckduckgo_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/duckduckgo_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/metasearch_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/metasearch_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/wikipedia_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/wikipedia_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/wikipedia.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/wikipedia.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/PKG-INFO` & `napari-chatgpt-2023.7.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,20 @@
-Metadata-Version: 2.1
-Name: napari-chatgpt
-Version: 2023.6.3
-Summary: A napari plugin to process and analyse images with chatGPT.
-Home-page: https://github.com/royerlab/napari-chatgpt
-Author: Loic A. Royer
-Author-email: royerloic@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
-Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
-Project-URL: Source Code, https://github.com/royerlab/napari-chatgpt
-Project-URL: User Support, https://github.com/royerlab/napari-chatgpt/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # napari-chatgpt
 
 ## Home of
 _Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
 
-A [napari](napari.org) plugin that levegares OpenAI's Large Language Model
+A [napari](napari.org) plugin that leverages OpenAI's Large Language Model
 ChatGPT to implement _Omega_
 a napari-aware agent capable of performing image processing and analysis tasks
 in a conversational manner.
 
 This repository was created as a 'week-end project'
 by [Loic A. Royer](https://twitter.com/loicaroyer)
 who leads a [research group](https://royerlab.org) at
@@ -58,16 +29,16 @@
 
 # What is Omega?
 
 Omega is a LLM-based and tool-armed autonomous agent that demonstrates the
 potential for Large Language Models (LLMs) to be applied to image processing,
 analysis and visualisation.
 Can LLM-based agents write image processing code and napari widgets, correct its
-coding mistakes, perform
-follow-up analysis, and control the napari viewer? The answer appears to be yes.
+coding mistakes, perform follow-up analysis, and control the napari viewer? 
+The answer appears to be yes.
 
 #### In this video I ask Omega to segment an image using the [SLIC](https://www.iro.umontreal.ca/~mignotte/IFT6150/Articles/SLIC_Superpixels.pdf) algorithm. It makes a first attempt using the implementation in scikit-image, but fails because of an inexistant 'multichannel' parameter. Realising that, Omega tries again, and this time, succeeds:
 
 https://user-images.githubusercontent.com/1870994/235768559-ca8bfa84-21f5-47b6-b2bd-7fcc07cedd92.mp4
 
 #### After loading in napari a sample 3D image of cell nuclei, I ask Omega to segment the nuclei using the Otsu method. My first request was very vague, so it just segmented foreground versus background. I then ask to segment the foreground into distinct segments for each connected component. Omega does a rookie mistake by forgetting to 'import np'. No problem, it notices, tries again, and succeeds:
 
@@ -143,102 +114,125 @@
 corresponding environment).
 
 IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the
 latest one!
 
 ## Installation in an new conda environment (RECOMMENDED):
 
-Make sure you have an anaocnda/miniconda installation on your system.
-Ask ChatGPT what is that all about if you are unsure ;-)
+Make sure you have an [miniconda](https://docs.conda.io/en/latest/miniconda.html) installation on your system.
+Ask [ChatGPT](https://chat.openai.com/auth/login) what is that all about if you are unsure ;-)
 
 Create environment:
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
     conda activate napari-chatgpt 
 
-Install napari in the environment using conda-forge: (important on Apple M1/M2)
+Install [napari](napari.org) in the environment using conda-forge: (very important on Apple M1/M2)
+
+    conda install -c conda-forge napari
 
-    conda install -c conda-forge napari     
+**Or**, with pip:
 
-Install the repo in enbvironment:
+    pip install napari
+
+Install napari-chatgpt in the environment:
 
     pip install napari-chatgpt
 
 ## Installation variations:
 
-To install latest development version :
+To install latest development version (not recommended for end-users):
 
+    conda create -y -n napari-chatgpt -c conda-forge python=3.9
+    conda activate napari-chatgpt
+    pip install napari  
     git clone https://github.com/royerlab/napari-chatgpt.git
     cd napari-chatgpt
     pip install -e .
 
 or:
-
+    
+    # same steps as above and then:
     pip install git+https://github.com/royerlab/napari-chatgpt.git
 
+## System specific tweaks:
+
+On Ubuntu systems, I recommend setting changing the UI timeout, 
+otherwise whenever Omega is thinking, the UI will freeze, and a popup will block
+everything which is very annoying:
+
+    gsettings set org.gnome.mutter check-alive-timeout 60000
+    
+
+
 ## Requirements:
 
-You need an OpenAI key, there is no way around this, unless we add some other,
-potentially local LLMs compatible to
-LangChain ([llama.cpp](https://github.com/ggerganov/llama.cpp) and similar
-models come to mind). However, this will likely be at the cost of cognitive
-performance,
-which I am not sure is worth it at this point. Please prove me wrong.
-You can get your OpenAI key by signing
-up [here](https://openai.com/blog/openai-api).
+You need an OpenAI key, there is no way around this, I have been experimenting with 
+other models, but right now the best results, by far are obtained with ChatGPT 4 (and to
+a lesser extent 3.5). You can get your OpenAI key by signing up [here](https://openai.com/blog/openai-api).
 Developing Omega cost me $13.97, hardly a fortune. OpenAI pricing on ChatGPT 3.5
-is very
-reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
-bargain.
-Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
+is very reasonable at 0.002 dollars per 1K tokens, which means $2 per 750000 words. A
+bargain. Now, ChatGPT 4.0 is about 10x more expensive... But that could eventually drop,
 hopefully.
 
 Note: you can limit the burn-rate to a certain amount of dollars per month, just
-in case you let
-Omega thinking over the week end and forget to stop it (don't worry, this is
-actually not possible).
+in case you let Omega thinking over the weekend and forget to stop it (don't worry, 
+this is actually **not** possible).
 
 ## Usage:
 
 Once all is installed, and if it is not already running, start napari:
 
     napari
 
 You can then the Omega napari plugin via the plugins menu:
 
 <img width="498" alt="image" src="https://user-images.githubusercontent.com/1870994/235790134-1d87fd50-583f-4fd9-ade2-c64497b91331.png">
 
 
-You just opened the plugin as a widget, you now need to actually start Omega:
+You just opened the plugin as a widget, this widget will appear:
+
+<img width="267" alt="image" src="https://github.com/royerlab/napari-chatgpt/assets/1870994/fdbde938-548d-4104-9241-d87c46c76dcf">
+
+I recommend that initially you stick to the defaults values, which work well.
+The best memory is 'hybrid'.
+The 'autofix' features only make sense if you are choosing a ChatGPT 4 model, 
+ChatGPT might get confused... 
+Increasing creativity also decreases 'attention to detail'; the models will make more
+coding mistakes, but might try more original solutions...
+
+You then need to actually start Omega:
 
 <img width="104" alt="image" src="https://user-images.githubusercontent.com/1870994/235811111-9e468785-9562-410a-8e9a-c63cb03fb765.png">
 
 
-If you have not set the 'OPENAI_API_KEY' environment variable as is typicall
-done,
-Omega will ask you for your OpenAI API key, and will store it _safely_ in an
+If you have not set the 'OPENAI_API_KEY' environment variable as is typically
+done, Omega will ask you for your OpenAI API key, and will store it _safely_ in an
 _encrypted_ way on your machine (~/.omega_api_keys/OpenAI.json):
 
 <img width="293" alt="image" src="https://user-images.githubusercontent.com/1870994/235793528-9e892c5e-d8ca-43e1-9020-f2dfab45b32d.png">
 
 
-Just enter an encryption/decription key, your OpenAI key, and
+Just enter an encryption/decryption key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
-(The idea is that you might not be able to remember your openAI key by heart,
+(The idea is that you might not be able to remember your openAI key by heart, obviously,
 but you might be able to do so with your own password or passphrase)
 
 You can then direct your browser
 to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
-and start having an hopefully nice chat with Omega.
+and start having a hopefully nice chat with Omega:
+
+<img width="631" alt="image" src="https://github.com/royerlab/napari-chatgpt/assets/1870994/a5cf6d4d-deea-4df8-be8a-601d1cc0424c">
+
 
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
 - What is your name?
 - What tools do you have available?
@@ -248,27 +242,27 @@
 - Make a widget that applies the transformation: y = x^alpha + y^beta with alpha
   and beta two parameters.
 - Create a widget to multiply two images
 - Can you open in napari a photo of Albert Einstein?
 - Downscale by a factor 3x the image on layer named 'img'
 - Rename selected layer to 'downscaled_image'
 - Upscale image 'downscaled_image' by a factor 3 using some smart interpolation
-  scheme of your choice (not nearest-neighboor)
+  scheme of your choice (not nearest-neighbor)
 - Caveat: makes a plugin instead of actually doing teh job
 - How many channels has the image on layer 0
 - Make a image sharpening filter widget, expose relevant parameters
 - Can you open this file in
   napari: https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.4/idr0062A/6001240.zarr
 - Split the two channels of the first layer (first axis) into two separate
   layers
 - Switch viewer to 3d
 - Create a napari widget for a function that takes two image layers and returns
   a 3D image stack of n images where each 2D image corresponds to a linear
   blending of the two layer images between 0 and 1.
-- [Loaded the ‘cell’ sample image] there is one cell in the image on the first
+- Loaded the ‘cell’ sample image. there is one cell in the image on the first
   layer, it is roughly circular and brighter than its surroundings, ca you write
   segmentation code that returns a labels layer for it?
 - Can you create a widget to blend two images?
 - Can you tell me more about the 'guided Canny edge filter' ?
 - Write a configurable RGB to grayscale widget, ensure weights sum to 1
 
 ## Video Demos:
@@ -277,17 +271,16 @@
 models,
 so here are videos showcasing what's possible. You will notice that Omega
 sometimes
 fails on its first attempt, typically because of mistaken parameters for
 functions,
 or other syntax errors. But it also often recovers by having access to the error
 message,
-and reasoning its way to the right piece of code. This is what ChatGPT 3.5 can
-do, imagine
-what will be possible with 4.0 and future more capable models...
+and reasoning its way to the right piece of code. The videos below were made with ChatGPT 3.5,
+version 4 works much better imagine what will be possible with future even more capable models...
 
 ##
 
 In this first video, I ask Omega to make a napari widget to convert images from
 RGB to grayscale:
 
 https://user-images.githubusercontent.com/1870994/235769895-23cfc7ed-622a-47f9-95aa-4be77efc0f78.mp4
@@ -305,17 +298,17 @@
 ##
 
 Following-up from the previous video, I ask Omega to create a new labels layer
 containing just the largest segment. The script that Omega writes as another
 rookie mistake: it confuses layers and images. The error message then confuses
 Omega into thinking that it got the name of the layer wrong, setting it off in a
 quest
-to find the name of the labels layer. It succeeds at writting code that searches
+to find the name of the labels layer. It succeeds at writing code that searches
 for the labels layer, and uses that name to write a script that then does
-extracts te largest segment into its own layer. Not bad:
+extract the largest segment into its own layer. Not bad:
 
 https://user-images.githubusercontent.com/1870994/235770741-d8905afd-0a9b-4eb7-a075-481979ab7b01.mp4
 
 ##
 
 In this video, I ask Omega to write a 'segmentation widget'. Pretty unspecific.
 The answer is a vanilla yet effective widget that uses the Otsu approach to
@@ -451,22 +444,22 @@
 not a practical approach. Not clear what happened to the colors though. Probably
 an RGB ordering or format issue:
 
 https://user-images.githubusercontent.com/1870994/235771146-ced45353-4886-42cb-b48f-3ce0859ed434.mp4
 
 ## Disclaimer:
 
-Do not use this software lightly, it will download libaries by its own volition,
-write any code that it deems nescessary, it might actually do what you ask, even
+Do not use this software lightly, it will download libraries by its own volition,
+write any code that it deems necessary, it might actually do what you ask, even
 if
-it is a bad idea. Also, beware that it might _misundertand_ what you ask and
+it is a bad idea. Also, beware that it might _misunderstand_ what you ask and
 then do
 something bad. For example, it is unwise to use Omega to delete 'some' files
 from your system,
-it might end up deleteing more than that if you are unclear in your request.  
+it might end up deleting more than that if you are unclear in your request.  
 To be 100% safe, we recommend that you use this software from within a sandboxed
 virtual machine.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED,
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 PARTICULAR
```

### Comparing `napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/SOURCES.txt` & `napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/napari_chatgpt/_sandbox/gpt4all_demo.py
 src/napari_chatgpt/_sandbox/gtts_demo.py
 src/napari_chatgpt/_sandbox/lanchain_openai.py
 src/napari_chatgpt/_sandbox/openai_list_models.py
 src/napari_chatgpt/_sandbox/playwright_sandbox.py
 src/napari_chatgpt/_sandbox/speech_recognition_demo.py
 src/napari_chatgpt/_sandbox/terminal.py
+src/napari_chatgpt/_sandbox/test.py
 src/napari_chatgpt/_sandbox/tts_demo.py
 src/napari_chatgpt/_sandbox/whisper_cpp.py
 src/napari_chatgpt/_tests/__init__.py
 src/napari_chatgpt/_tests/test_widget.py
 src/napari_chatgpt/chat_server/__init__.py
 src/napari_chatgpt/chat_server/chat_response.py
 src/napari_chatgpt/chat_server/chat_server.py
@@ -77,37 +78,45 @@
 src/napari_chatgpt/omega/omega_agent/agent_executor.py
 src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
 src/napari_chatgpt/omega/omega_agent/prompts.py
 src/napari_chatgpt/omega/omega_agent/tests/__init__.py
 src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
 src/napari_chatgpt/omega/tools/__init__.py
 src/napari_chatgpt/omega/tools/async_base_tool.py
-src/napari_chatgpt/omega/tools/napari_base_tool.py
+src/napari_chatgpt/omega/tools/instructions.py
 src/napari_chatgpt/omega/tools/napari_plugin_tool.py
 src/napari_chatgpt/omega/tools/demo/__init__.py
 src/napari_chatgpt/omega/tools/demo/tools_demo.py
 src/napari_chatgpt/omega/tools/examples/__init__.py
 src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
 src/napari_chatgpt/omega/tools/napari/__init__.py
 src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
-src/napari_chatgpt/omega/tools/napari/cellpose.py
 src/napari_chatgpt/omega/tools/napari/file_open_tool.py
+src/napari_chatgpt/omega/tools/napari/image_denoising.py
+src/napari_chatgpt/omega/tools/napari/napari_base_tool.py
 src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
 src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
 src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
+src/napari_chatgpt/omega/tools/napari/delegated_code/__init__.py
+src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_classic.py
+src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_fgr.py
+src/napari_chatgpt/omega/tools/napari/delegated_code/cellpose.py
+src/napari_chatgpt/omega/tools/napari/delegated_code/classic.py
+src/napari_chatgpt/omega/tools/napari/delegated_code/stardist.py
 src/napari_chatgpt/omega/tools/search/__init__.py
 src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
 src/napari_chatgpt/omega/tools/search/web_search_tool.py
 src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
 src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
 src/napari_chatgpt/omega/tools/special/__init__.py
 src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
 src/napari_chatgpt/omega/tools/special/file_download_tool.py
 src/napari_chatgpt/omega/tools/special/functions_info_tool.py
 src/napari_chatgpt/omega/tools/special/human_input_tool.py
+src/napari_chatgpt/omega/tools/special/python_repl.py
 src/napari_chatgpt/omega/tools/tests/__init__.py
 src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
 src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
 src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
 src/napari_chatgpt/utils/__init__.py
 src/napari_chatgpt/utils/api_keys/__init__.py
 src/napari_chatgpt/utils/api_keys/api_key.py
@@ -119,14 +128,16 @@
 src/napari_chatgpt/utils/async_utils/__init__.py
 src/napari_chatgpt/utils/async_utils/run_async.py
 src/napari_chatgpt/utils/download/__init__.py
 src/napari_chatgpt/utils/download/download_files.py
 src/napari_chatgpt/utils/download/gpt4all.py
 src/napari_chatgpt/utils/download/test/__init__.py
 src/napari_chatgpt/utils/download/test/download_files_test.py
+src/napari_chatgpt/utils/images/__init__.py
+src/napari_chatgpt/utils/images/normalize.py
 src/napari_chatgpt/utils/llm/__init__.py
 src/napari_chatgpt/utils/llm/summarizer.py
 src/napari_chatgpt/utils/llm/test/__init__.py
 src/napari_chatgpt/utils/llm/test/summarizer_test.py
 src/napari_chatgpt/utils/napari/__init__.py
 src/napari_chatgpt/utils/napari/napari_viewer_info.py
 src/napari_chatgpt/utils/napari/open_in_napari.py
@@ -135,21 +146,23 @@
 src/napari_chatgpt/utils/napari/test/__init__.py
 src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
 src/napari_chatgpt/utils/omega_plugins/__init__.py
 src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
 src/napari_chatgpt/utils/omega_plugins/test/__init__.py
 src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
 src/napari_chatgpt/utils/python/__init__.py
+src/napari_chatgpt/utils/python/conda_utils.py
 src/napari_chatgpt/utils/python/dynamic_import.py
 src/napari_chatgpt/utils/python/exception_description.py
 src/napari_chatgpt/utils/python/exception_guard.py
 src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
 src/napari_chatgpt/utils/python/fix_code_given_error.py
 src/napari_chatgpt/utils/python/installed_packages.py
 src/napari_chatgpt/utils/python/missing_packages.py
+src/napari_chatgpt/utils/python/pip_utils.py
 src/napari_chatgpt/utils/python/python_lang_utils.py
 src/napari_chatgpt/utils/python/required_imports.py
 src/napari_chatgpt/utils/python/test/__init__.py
 src/napari_chatgpt/utils/python/test/dynamic_import_test.py
 src/napari_chatgpt/utils/python/test/exception_description_test.py
 src/napari_chatgpt/utils/python/test/exception_guard_test.py
 src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
```

### Comparing `napari-chatgpt-2023.6.3/tox.ini` & `napari-chatgpt-2023.7.7/tox.ini`

 * *Files identical despite different names*

