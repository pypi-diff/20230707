# Comparing `tmp/oobabot_plugin-0.1.9.tar.gz` & `tmp/oobabot_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot_plugin-0.1.9.tar", max compression
+gzip compressed data, was "oobabot_plugin-0.2.0.tar", max compression
```

## Comparing `oobabot_plugin-0.1.9.tar` & `oobabot_plugin-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-05-23 18:45:53.519115 oobabot_plugin-0.1.9/LICENSE
--rw-r--r--   0        0        0     1951 2023-05-24 06:06:57.334971 oobabot_plugin-0.1.9/README.md
--rw-r--r--   0        0        0     1181 2023-05-26 18:44:59.392017 oobabot_plugin-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-24 16:52:38.642666 oobabot_plugin-0.1.9/src/oobabot_plugin/__init__.py
--rw-r--r--   0        0        0   920346 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/ace.js
--rw-r--r--   0        0        0    12073 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_mode_yaml.js
--rw-r--r--   0        0        0     1572 2023-05-26 18:39:06.122009 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_oobabot.js
--rw-r--r--   0        0        0     3509 2023-05-26 18:42:31.352014 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_theme_github.js
--rw-r--r--   0        0        0     3800 2023-05-26 18:42:31.352014 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_theme_github_dark.js
--rw-r--r--   0        0        0     3511 2023-05-26 18:39:02.492009 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_theme_twilight.js
--rw-r--r--   0        0        0     7676 2023-05-26 18:40:18.922011 oobabot_plugin-0.1.9/src/oobabot_plugin/bootstrap.py
--rw-r--r--   0        0        0    16913 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/controller.py
--rw-r--r--   0        0        0      172 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/editor.html
--rw-r--r--   0        0        0     9903 2023-05-25 16:33:44.756742 oobabot_plugin-0.1.9/src/oobabot_plugin/input_handlers.py
--rw-r--r--   0        0        0     3305 2023-05-25 16:33:44.756742 oobabot_plugin-0.1.9/src/oobabot_plugin/install.py
--rw-r--r--   0        0        0      806 2023-05-23 19:32:11.169051 oobabot_plugin-0.1.9/src/oobabot_plugin/instructions.md
--rw-r--r--   0        0        0    13529 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/layout.py
--rw-r--r--   0        0        0     2935 2023-05-26 18:42:15.202013 oobabot_plugin-0.1.9/src/oobabot_plugin/oobabot_log.css
--rw-r--r--   0        0        0     1144 2023-05-24 17:50:51.222742 oobabot_plugin-0.1.9/src/oobabot_plugin/script.py
--rw-r--r--   0        0        0      783 2023-05-26 18:41:48.302013 oobabot_plugin-0.1.9/src/oobabot_plugin/server.py
--rw-r--r--   0        0        0     4728 2023-05-26 18:42:11.702013 oobabot_plugin-0.1.9/src/oobabot_plugin/strings.py
--rw-r--r--   0        0        0     8509 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/worker.py
--rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 oobabot_plugin-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-24 23:25:59.529104 oobabot_plugin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1951 2023-05-24 23:25:59.529239 oobabot_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0     1871 2023-07-07 10:24:51.238182 oobabot_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-06-24 23:44:13.221133 oobabot_plugin-0.2.0/src/oobabot_plugin/__init__.py
+-rw-r--r--   0        0        0     7536 2023-06-24 09:50:54.210004 oobabot_plugin-0.2.0/src/oobabot_plugin/bootstrap.py
+-rw-r--r--   0        0        0     7784 2023-07-07 10:24:51.240296 oobabot_plugin-0.2.0/src/oobabot_plugin/button_enablers.py
+-rw-r--r--   0        0        0     9560 2023-07-07 10:24:51.240670 oobabot_plugin-0.2.0/src/oobabot_plugin/button_handlers.py
+-rw-r--r--   0        0        0     3039 2023-07-07 10:24:51.241673 oobabot_plugin-0.2.0/src/oobabot_plugin/controller.py
+-rw-r--r--   0        0        0     9903 2023-05-25 05:24:15.485352 oobabot_plugin-0.2.0/src/oobabot_plugin/input_handlers.py
+-rw-r--r--   0        0        0     3305 2023-05-25 06:56:54.200392 oobabot_plugin-0.2.0/src/oobabot_plugin/install.py
+-rw-r--r--   0        0        0      806 2023-05-24 23:25:59.534874 oobabot_plugin-0.2.0/src/oobabot_plugin/instructions.md
+-rw-r--r--   0        0        0    15924 2023-07-07 10:24:51.242055 oobabot_plugin-0.2.0/src/oobabot_plugin/layout.py
+-rw-r--r--   0        0        0     4826 2023-07-07 10:26:33.202649 oobabot_plugin-0.2.0/src/oobabot_plugin/oobabot_log.css
+-rw-r--r--   0        0        0      498 2023-06-26 15:36:57.565953 oobabot_plugin-0.2.0/src/oobabot_plugin/oobabot_log.js
+-rw-r--r--   0        0        0     1144 2023-06-24 06:51:19.539687 oobabot_plugin-0.2.0/src/oobabot_plugin/script.py
+-rw-r--r--   0        0        0      783 2023-06-22 12:29:04.858021 oobabot_plugin-0.2.0/src/oobabot_plugin/server.py
+-rw-r--r--   0        0        0     4446 2023-07-07 10:24:51.243563 oobabot_plugin-0.2.0/src/oobabot_plugin/strings.py
+-rw-r--r--   0        0        0      211 2023-07-07 10:24:51.243788 oobabot_plugin-0.2.0/src/oobabot_plugin/transcript.md
+-rw-r--r--   0        0        0     5702 2023-07-07 10:24:51.244597 oobabot_plugin-0.2.0/src/oobabot_plugin/transcript_view.py
+-rw-r--r--   0        0        0     8867 2023-07-05 22:59:41.850315 oobabot_plugin-0.2.0/src/oobabot_plugin/worker.py
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 oobabot_plugin-0.2.0/PKG-INFO
```

### Comparing `oobabot_plugin-0.1.9/LICENSE` & `oobabot_plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.9/README.md` & `oobabot_plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.9/pyproject.toml` & `oobabot_plugin-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 [tool.poetry]
 name = "oobabot-plugin"
-version = "0.1.9"
+version = "0.2.0"
 description = "A Discord bot plugin to oobabooga's text-generation-webui, based on oobabot."
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot-plugin"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-oobabot = "^0.1.9"
-gradio = "^3.31.0"
+oobabot = "^0.2.0"
+# oobabot = { path = "../oobabot" }
+# we can't use the latest version of gradio, since a range of
+# text-generation-webui versions are incompatible with it.  But
+# we don't want to use a version older than 3.34.0, since those
+# have serious security issues.  So this version seems like the
+# only compromise, until at least text-generation-webui supports
+# a newer version of gradio.
+gradio = "~3.34.0"
+# we don't actually use fastapi, but it's a dependency of gradio
+# and if this isn't specified, poetry will install a very old version
+# (0.1.17) instead of the latest (0.99.1).  This older version won't
+# work with gradio.  Remove this when either gradio or poetry fixes
+# this issue.
+fastapi = "^0.99.1"
 
 [tool.poetry.scripts]
 oobabot-plugin = 'oobabot_plugin.install:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/bootstrap.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 
 import oobabot
 
 import oobabot_plugin
 from oobabot_plugin import controller
 from oobabot_plugin import strings
 
-# we'll try to discover what the user has actually set the
-# port to, but if we fail for some reason, fall back to this
-DEFAULT_STREAMING_API_PORT = 5005
-
 # standard config file name, can be overridden in settings.json
 DEFAULT_CONFIG_FILE = "oobabot-config.yml"
 
 
 # allow our logging to use the original version of StreamHandler.emit,
 # then reapply the monkey-patch so it doesn't affect anyone else
 oobabot_logger = strings.repair_logging()
@@ -58,15 +54,15 @@
 def plugin_ui(
     script_py_version: str = "",
     params: typing.Optional[dict] = None,
 ) -> None:
     """
     Creates custom gradio elements when the UI is launched.
     """
-    streaming_port = DEFAULT_STREAMING_API_PORT
+    streaming_port = oobabot_plugin.DEFAULT_STREAMING_API_PORT
     api_extension_loaded = True
 
     if script_py_version:
         log_script_py_version(script_py_version)
 
         # use optimistic defaults, in case the probing process
         # fails for some reason.  If either of these fail, the
```

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/input_handlers.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/input_handlers.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/install.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/install.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/instructions.md` & `oobabot_plugin-0.2.0/src/oobabot_plugin/instructions.md`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/layout.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/layout.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,89 +16,110 @@
     """
     This class is responsible for creating the oobabot UI frame.
 
     It should create all of the UI components, but not set any
     behaviors or values.
     """
 
-    # outer navigation elements
-    tab_config: gr.Tab
-    tab_advanced: gr.Tab
-
-    #############################################
-    # Configuration tab
-    #############################################
-
-    # discord token widgets
-    welcome_accordion: gr.Accordion
-    discord_token_textbox: gr.Textbox
-    discord_token_save_button: gr.Button
-    discord_invite_link_html: gr.HTML
-    ive_done_all_this_button: gr.Button
-
-    # persona widgets
-    character_dropdown: gr.Dropdown
-
-    ai_name_textbox: gr.Textbox
-    persona_textbox: gr.Textbox
-
-    # the _character ones are only shown when we are
-    # using a character, when they're shown, the other
-    # ones are hidden.
-    ai_name_textbox_character: gr.Textbox
-    persona_textbox_character: gr.Textbox
-
-    wake_words_textbox: gr.Textbox
-
-    # discord behavior widgets
-    split_responses_radio_group: gr.Radio
-    history_lines_slider: gr.Slider
-    discord_behavior_checkbox_group: gr.CheckboxGroup
-
-    # stable diffusion settings
-    stable_diffusion_url_textbox: gr.Textbox
-    stable_diffusion_prefix: gr.Textbox
-    stable_diffusion_params: gr.Textbox
-
-    save_settings_button: gr.Button
-
-    #############################################
-    # Advanced tab
-    #############################################
-
-    advanced_settings_html: gr.HTML
-    advanced_save_result: gr.Markdown
-    advanced_save_settings_button: gr.Button
-
-    #############################################
-    # Runtime section
-    #############################################
-
-    # runtime widgets
-    start_button: gr.Button
-    stop_button: gr.Button
-    log_output_html: gr.HTML
+    def __init__(self) -> None:
+        # outer navigation elements
+        self.tab_config: gr.Tab
+        self.tab_audio: typing.Optional[gr.Tab]
+        self.tab_advanced: gr.Tab
+
+        #############################################
+        # Configuration tab
+        #############################################
+
+        # discord token widgets
+        self.welcome_accordion: gr.Accordion
+        self.discord_token_textbox: gr.Textbox
+        self.discord_token_save_button: gr.Button
+        self.discord_invite_link_html: gr.HTML
+        self.ive_done_all_this_button: gr.Button
+
+        # persona widgets
+        self.character_dropdown: gr.Dropdown
+
+        self.ai_name_textbox: gr.Textbox
+        self.persona_textbox: gr.Textbox
+
+        # the _character ones are only shown when we are
+        # using a character, when they're shown, the other
+        # ones are hidden.
+        self.ai_name_textbox_character: gr.Textbox
+        self.persona_textbox_character: gr.Textbox
+
+        self.wake_words_textbox: gr.Textbox
+
+        # discord behavior widgets
+        self.split_responses_radio_group: gr.Radio
+        self.history_lines_slider: gr.Slider
+        self.discord_behavior_checkbox_group: gr.CheckboxGroup
+
+        # stable diffusion settings
+        self.stable_diffusion_url_textbox: gr.Textbox
+        self.stable_diffusion_prefix: gr.Textbox
+        self.stable_diffusion_params: gr.Textbox
+
+        self.save_settings_button: gr.Button
+
+        #############################################
+        # Advanced tab
+        #############################################
+
+        self.advanced_save_result: gr.Markdown
+        self.advanced_save_settings_button: gr.Button
+        self.advanced_yaml_editor: gr.Code
+
+        #############################################
+        # Audio tab
+        #############################################
+
+        self.transcript_markdown: typing.Optional[gr.Markdown]
+        self.transcript_html: typing.Optional[gr.HTML]
+
+        #############################################
+        # Runtime section
+        #############################################
+
+        # runtime widgets
+        self.start_button: gr.Button
+        self.plugin_auto_start_checkbox: gr.Checkbox
+        self.stop_button: gr.Button
+        self.log_output_html: gr.HTML
+        self.running_state_textbox: gr.Textbox
 
     def layout_ui(
         self,
         get_logs: typing.Callable[[], str],
         has_plausible_token: bool,
         stable_diffusion_keywords: typing.List[str],
         api_extension_loaded: bool,
         is_using_character: bool,
+        get_transcript_html: typing.Callable[[], str],
+        is_voice_enabled: bool,
     ) -> None:
         with gr.Blocks():
             self.tab_config = gr.Tab(
                 label="Configuration",
                 elem_id="oobabot-tab-config",
             )
             self.tab_advanced = gr.Tab(
                 label="Advanced",
                 elem_id="oobabot-tab-advanced",
             )
+            if is_voice_enabled:
+                self.tab_audio = gr.Tab(
+                    label="Audio",
+                    elem_id="oobabot-tab-audio",
+                )
+            else:
+                self.tab_audio = None
+
             with self.tab_config:
                 with gr.Row():
                     with gr.Column(min_width=400):
                         self._init_config_ui(
                             has_plausible_token,
                             stable_diffusion_keywords,
                             is_using_character,
@@ -108,14 +129,31 @@
                             get_logs,
                             api_extension_loaded,
                         )
 
             with self.tab_advanced:
                 self._init_advanced_ui()
 
+            if self.tab_audio is None:
+                self.transcript_markdown = None
+                self.transcript_html = None
+            else:
+                with self.tab_audio:
+                    with gr.Column():
+                        self.transcript_markdown = gr.Markdown(
+                            strings.get_transcript_markdown(),
+                            elem_classes="oobabot-transcript-markdown",
+                        )
+                        self.transcript_html = gr.HTML(
+                            label="Oobabot Transcript",
+                            value=get_transcript_html,
+                            every=strings.QUICK_UPDATE_INTERVAL_SECONDS,
+                            elem_classes=["oobabot-audio-output"],
+                        )
+
     #############################################
     # Configuration tab
     #############################################
 
     BY_SENTENCE = "by sentence"
     SINGLE_MESSAGE = "single message"
     STREAMING = "streaming [beta feature]"
@@ -141,14 +179,15 @@
                 with gr.Row():
                     self.discord_token_textbox = gr.Textbox(
                         label="Discord Token",
                         show_label=False,
                         placeholder="Paste your Discord bot token here.",
                         # ugh. this is so gradio fires a change when the value's set
                         value=" ",
+                        elem_id="oobabot-token-textbox",
                     )
                     self.discord_token_save_button = gr.Button(
                         value="💾 Save", elem_id="oobabot-save-token"
                     )
                 gr.Markdown(instructions_2, elem_classes=["oobabot_instructions"])
                 self.discord_invite_link_html = gr.HTML()
                 self.ive_done_all_this_button = gr.Button(
@@ -228,15 +267,15 @@
                     elem_id="oobabot-wake-words",
                 )
 
         def _init_discord_behavior_widgets() -> None:
             gr.Markdown("### Discord Behavior")
 
             self.split_responses_radio_group = gr.Radio(
-                [self.BY_SENTENCE, self.SINGLE_MESSAGE],
+                [self.BY_SENTENCE, self.SINGLE_MESSAGE, self.STREAMING],
                 label="Split Responses",
                 info="How should `oobabot` split responses into messages?",
                 value=self.BY_SENTENCE,
                 interactive=True,
                 elem_id="oobabot-split-responses",
             )
             self.history_lines_slider = gr.Slider(
@@ -329,17 +368,16 @@
                 elem_id="oobabot-advanced-save-result",
             )
             self.advanced_save_settings_button = gr.Button(
                 value="💾 Save Settings",
                 elem_id="oobabot-advanced-save-settings",
                 interactive=True,
             )
-        self.advanced_settings_html = gr.HTML(
-            value="",
-            elem_id="oobabot-config-giant-html",
+        self.advanced_yaml_editor = gr.Code(
+            language="yaml",
         )
 
     #############################################
     # Runtime tab
     #############################################
 
     def _init_runtime_ui(
@@ -348,25 +386,39 @@
         api_extension_loaded: bool,
     ) -> None:
         with gr.Row():
             self.start_button = gr.Button(
                 value="Start Oobabot",
                 interactive=False,
             )
+            self.plugin_auto_start_checkbox = gr.Checkbox(
+                label="Start automatically when Oobabooga starts",
+                value=False,
+                interactive=True,
+                elem_id="oobabot-plugin-auto-start",
+            )
             self.stop_button = gr.Button(
                 value="Stop Oobabot",
                 interactive=False,
             )
+            self.running_state_textbox = gr.Textbox(
+                "",
+                interactive=False,
+                visible=False,
+                elem_id="oobabot-is-running",
+            )
+            # visible=False,  TODO: HIDE
+
         gr.Markdown("### Oobabot Status", elem_id="oobabot-status-heading")
         if not api_extension_loaded:
             gr.Markdown(
                 "**Warning**: The API extension is not loaded.  "
                 + "`Oobabot` will not work unless it is enabled.",
                 elem_id="oobabot-api-not-loaded",
             )
         with gr.Row():
             self.log_output_html = gr.HTML(
                 label="Oobabot Log",
                 value=get_logs,
-                every=0.5,
+                every=strings.QUICK_UPDATE_INTERVAL_SECONDS,
                 elem_classes=["oobabot-output"],
             )
```

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/script.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/script.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/server.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/server.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/strings.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/strings.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import types
 import typing
 
 import oobabot.fancy_logger
 
 TOKEN_LEN_CHARS = 72
 
+QUICK_UPDATE_INTERVAL_SECONDS: float = 0.5
+
 
 def resource(name: str) -> str:
     # return importlib.resources.read_text("oobabot_plugin", name)
     return pathlib.Path(os.path.join(os.path.dirname(__file__), name)).read_text(
         encoding="utf-8"
     )
 
@@ -34,37 +36,30 @@
     Returns markdown in two parts, before and after the
     token input box.
     """
     md_text = resource("instructions.md")
     return tuple(md_text.split("{{TOKEN_INPUT_BOX}}", 1))
 
 
+def get_transcript_markdown() -> str:
+    return resource("transcript.md")
+
+
 def get_css() -> str:
     return resource("oobabot_log.css")
 
 
 def get_js() -> str:
-    custom_js = resource("ace.js")
-    custom_js += resource("ace_theme_github.js")
-    custom_js += resource("ace_theme_github_dark.js")
-    custom_js += resource("ace_mode_yaml.js")
-    custom_js += resource("ace_oobabot.js")
-    return custom_js
+    return resource("oobabot_log.js")
 
 
 def token_is_plausible(token: str) -> bool:
     return len(token.strip()) >= TOKEN_LEN_CHARS
 
 
-def format_yaml_for_html(yaml: str) -> str:
-    template = resource("editor.html")
-    # replace {{OOBABOT-CONFIG-YML}} with yaml
-    return template.replace("{{OOBABOT-CONFIG-YML}}", yaml)
-
-
 def format_save_result(yaml_error: typing.Optional[str]) -> str:
     if yaml_error:
         return "❌ **Error**: " + yaml_error
     return "✔️ **Saved**"
 
 
 def make_link_from_token(
```

### Comparing `oobabot_plugin-0.1.9/src/oobabot_plugin/worker.py` & `oobabot_plugin-0.2.0/src/oobabot_plugin/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import threading
 import typing
 
 import gradio as gr
 from oobabot import oobabot
 
+import oobabot_plugin
 from oobabot_plugin import input_handlers
 from oobabot_plugin import layout
 
 
 class OobabotWorker:
     """
     This class is responsible for running oobabot in a worker thread.
@@ -54,17 +55,18 @@
             self.thread.join()
             self.stopping = False
             self.thread = None
 
         args = [
             "--config",
             os.path.abspath(self.config_file),
-            "--base-url",
-            f"ws://localhost:{self.port}/",
         ]
+        if self.port != oobabot_plugin.DEFAULT_STREAMING_API_PORT:
+            args.extend(["--base-url", f"ws://localhost:{str(self.port)}"])
+
         self.bot = oobabot.Oobabot(args)
         self.handlers = {}
 
     def start(self) -> None:
         """
         Stops the oobabot if it's running, then starts it.
         """
@@ -97,16 +99,43 @@
 
         lines = oobabot.fancy_logger.recent_logs.get_all()
         return (
             '<div class="oobabot-log">' + "\n<br>".join(lines) + "</div></body></html>"
         )
 
     def save_settings(self):
+        if self.bot is None:
+            return
         self.bot.settings.write_to_file(self.config_file)
 
+    def is_voice_enabled(self) -> bool:
+        if self.bot is None:
+            return False
+        return self.bot.is_voice_enabled()
+
+    def get_transcript(self) -> typing.List["oobabot.types.VoiceMessage"]:
+        """
+        Returns the transcript of the latest voice call from the oobabot,
+        or None if there is no transcript.
+        """
+        if self.bot is None:
+            return []
+        return self.bot.current_voice_transcript
+
+    def get_fancy_author(
+        self, user_id: int
+    ) -> typing.Optional["oobabot.types.FancyAuthor"]:
+        """
+        Returns display information about the given user id,
+        or None if the user id could not be found.
+        """
+        if self.bot is None:
+            return None
+        return self.bot.fancy_author_info(user_id)
+
     def get_input_handlers(
         self,
         fn_get_character_list: typing.Callable[[], typing.List[str]],
     ) -> typing.Dict[gr.components.IOComponent, input_handlers.ComponentToSetting]:
         if self.handlers:
             return self.handlers
 
@@ -166,70 +195,55 @@
                 "stable_diffusion_url",
             ),
             input_handlers.SimpleComponentToSetting(
                 layout.stable_diffusion_prefix,
                 settings.stable_diffusion_settings,
                 "extra_prompt_text",
             ),
+            input_handlers.SimpleComponentToSetting(
+                layout.plugin_auto_start_checkbox,
+                settings.oobabooga_settings,
+                "plugin_auto_start",
+            ),
         ]
 
         # make a map from component to setting
         self.handlers = {c.component: c for c in components_to_settings}
         return self.handlers
 
     def preview_persona(
         self,
         character: str,
         ai_name: str,
         persona: str,
-        wakewords_str: str,
-    ) -> typing.Tuple[str, str, str]:
+    ) -> typing.Tuple[str, str]:
         """
         Takes the persona settings and returns what the bot will
         end up using, given the settings.
 
-        Returns: (ai_name, persona, wakewords)
+        Returns: (ai_name, persona)
         """
         persona_file = (
             input_handlers.CharacterComponentToSetting.character_name_to_filepath(
                 character=character
             )
         )
 
-        # we need to turn wakewords into a list, then back again
-        wakewords_list = input_handlers.ListComponentToSetting.string_to_list(
-            wakewords_str
-        )
-
-        # if we change from a manually entered ai name to one
-        # from the persona file, we probably should remove the old
-        # ai name from the wakewords.
-        # if it turns out this *is* the new persona name, that's ok,
-        # since the persona handler will add it back in.
-        if persona_file:
-            if ai_name in wakewords_list:
-                wakewords_list.remove(ai_name)
-
-        persona_handler = oobabot.persona.Persona(
+        persona_handler = oobabot.runtime.persona.Persona(
             {
                 "ai_name": ai_name,
                 "persona": persona,
-                "wakewords": wakewords_list,
+                "wakewords": [],
                 "persona_file": persona_file,
             }
         )
 
-        new_wakewords = input_handlers.ListComponentToSetting.list_to_string(
-            persona_handler.wakewords
-        )
-
         return (
             persona_handler.ai_name,
             persona_handler.persona,
-            new_wakewords,
         )
 
     def is_using_character(
         self,
         fn_get_character_list: typing.Callable[[], typing.List[str]],
     ) -> bool:
         # get the filename out of the settings.  If it is
```

### Comparing `oobabot_plugin-0.1.9/PKG-INFO` & `oobabot_plugin-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: oobabot-plugin
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Discord bot plugin to oobabooga's text-generation-webui, based on oobabot.
 Home-page: https://github.com/chrisrude/oobabot-plugin
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gradio (>=3.31.0,<4.0.0)
-Requires-Dist: oobabot (>=0.1.9,<0.2.0)
+Requires-Dist: fastapi (>=0.99.1,<0.100.0)
+Requires-Dist: gradio (>=3.34.0,<3.35.0)
+Requires-Dist: oobabot (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/chrisrude/oobabot-plugin
 Description-Content-Type: text/markdown
 
 # Oobabot-plugin
 
 [**`oobabot`**](https://github.com/chrisrude/oobabot) is a Discord bot which talks to a Large Language Model AIs (like LLaMA, llama.cpp, etc...), running on [oobabooga's text-generation-webui](https://github.com/oobabooga/text-generation-webui).
```

