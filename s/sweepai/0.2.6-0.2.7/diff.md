# Comparing `tmp/sweepai-0.2.6.tar.gz` & `tmp/sweepai-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.6.tar", max compression
+gzip compressed data, was "sweepai-0.2.7.tar", max compression
```

## Comparing `sweepai-0.2.6.tar` & `sweepai-0.2.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.6/LICENSE
--rw-r--r--   0        0        0     4541 2023-07-05 21:28:16.687295 sweepai-0.2.6/README.md
--rw-r--r--   0        0        0     1375 2023-07-06 00:41:14.976558 sweepai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.6/sweepai/__init__.py
--rw-r--r--   0        0        0    10754 2023-07-05 21:28:16.690628 sweepai-0.2.6/sweepai/api.py
--rw-r--r--   0        0        0     5974 2023-07-06 00:23:49.508003 sweepai-0.2.6/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10163 2023-07-06 00:23:49.508003 sweepai-0.2.6/sweepai/app/backend.py
--rw-r--r--   0        0        0     1185 2023-07-06 00:38:30.156451 sweepai-0.2.6/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.6/sweepai/app/config.py
--rw-r--r--   0        0        0    10897 2023-07-06 00:23:49.508003 sweepai-0.2.6/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.6/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17168 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/core/chat.py
--rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.6/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     7435 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/core/entities.py
--rw-r--r--   0        0        0    13102 2023-07-06 00:23:49.508003 sweepai-0.2.6/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/core/react.py
--rw-r--r--   0        0        0    16575 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    14461 2023-07-06 00:23:49.508003 sweepai-0.2.6/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.6/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     1430 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/utils/config.py
--rw-r--r--   0        0        0      671 2023-07-06 00:14:22.909920 sweepai-0.2.6/sweepai/utils/constants.py
--rw-r--r--   0        0        0     4072 2023-07-03 00:42:21.645402 sweepai-0.2.6/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.6/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.6/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.6/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.6/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.6/sweepai/utils/utils.py
--rw-r--r--   0        0        0     5612 2023-07-06 00:41:17.985534 sweepai-0.2.6/setup.py
--rw-r--r--   0        0        0     5408 2023-07-06 00:41:17.985849 sweepai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4541 2023-07-05 21:28:16.687295 sweepai-0.2.7/README.md
+-rw-r--r--   0        0        0     1395 2023-07-06 23:13:25.698058 sweepai-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.7/sweepai/__init__.py
+-rw-r--r--   0        0        0    10759 2023-07-06 22:37:11.532073 sweepai-0.2.7/sweepai/api.py
+-rw-r--r--   0        0        0     5974 2023-07-06 00:23:49.508003 sweepai-0.2.7/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10163 2023-07-06 00:23:49.508003 sweepai-0.2.7/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1185 2023-07-06 22:37:11.532073 sweepai-0.2.7/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.7/sweepai/app/config.py
+-rw-r--r--   0        0        0    11762 2023-07-06 23:10:05.104469 sweepai-0.2.7/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.7/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17168 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.7/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8120 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13065 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/core/react.py
+-rw-r--r--   0        0        0    17298 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    15419 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.7/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     1808 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/config.py
+-rw-r--r--   0        0        0      671 2023-07-06 23:10:39.614513 sweepai-0.2.7/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     4337 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.7/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.7/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.7/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     5640 2023-07-06 23:13:27.847816 sweepai-0.2.7/setup.py
+-rw-r--r--   0        0        0     5450 2023-07-06 23:13:27.848311 sweepai-0.2.7/PKG-INFO
```

### Comparing `sweepai-0.2.6/LICENSE` & `sweepai-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/README.md` & `sweepai-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/pyproject.toml` & `sweepai-0.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.6"
+version = "0.2.7"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
@@ -19,14 +19,15 @@
 PyGithub = "1.58.2"
 loguru = "^0.6.0"
 requests = "^2.28.2"
 urllib3 = "^2.0.3"
 gradio = "^3.35.2"
 config-path = "^1.0.3"
 typer = "^0.9.0"
+tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 commit5 = "^0.1.1"
 jupyter = "^1.0.0"
 ipykernel = "^6.23.1"
 build = "^0.10.0"
```

### Comparing `sweepai-0.2.6/sweepai/api.py` & `sweepai-0.2.7/sweepai/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,26 @@
         "backoff",
         "tiktoken",
         "highlight-io",
         "GitPython",
         "posthog",
         "tqdm",
         "pyyaml",
-        "pymongo"
+        "pymongo",
+        "tabulate"
     )
 )
 secrets = [
     modal.Secret.from_name(BOT_TOKEN_NAME),
     modal.Secret.from_name("openai-secret"),
     modal.Secret.from_name("anthropic"),
     modal.Secret.from_name("posthog"),
     modal.Secret.from_name("highlight"),
     modal.Secret.from_name("mongodb"),
+    modal.Secret.from_name("discord")
 ]
 
 FUNCTION_SETTINGS = {
     "image": image,
     "secrets": secrets,
     "timeout": 30 * 60,
 }
@@ -97,17 +99,15 @@
                     #         description=LABEL_DESCRIPTION
                     #     )
                     
                     current_issue = repo.get_issue(number=request.issue.number)
                     current_issue.add_to_labels(LABEL_NAME)
             case "issues", "labeled":
                 request = IssueRequest(**request_dict)
-                if request.issue is not None and (
-                    "sweep" in [label.name.lower() for label in request.issue.labels]
-                ):
+                if 'label' in request_dict and str.lower(request_dict['label']['name']) == LABEL_NAME:
                     request.issue.body = request.issue.body or ""
                     request.repository.description = (
                         request.repository.description or ""
                     )
                     # Update before we handle the ticket to make sure index is up to date
                     # other ways suboptimal
                     handle_ticket.spawn(
```

### Comparing `sweepai-0.2.6/sweepai/app/api_client.py` & `sweepai-0.2.7/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/app/backend.py` & `sweepai-0.2.7/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/app/cli.py` & `sweepai-0.2.7/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/app/config.py` & `sweepai-0.2.7/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/app/ui.py` & `sweepai-0.2.7/sweepai/app/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,34 @@
 {summary}
 
 Here is my plan:
 {plan}
 
 Reply with "ok" to create the PR or anything else to propose changes.'''
 
+print("Getting list of repos...")
 github_client = Github(config.github_pat)
 repos = list(github_client.get_user().get_repos())
+print("Done.")
 
 css = '''
 footer {
     visibility: hidden;
 }
 pre, code {
     white-space: pre-wrap !important;
     word-break: break-all !important;
 }
 #snippets {
     height: 750px;
     overflow-y: scroll;
 }
+#message_box > label > span {
+    display: none;
+}
 '''
 
 def get_files_recursively(root_path, path=''):
     files = []
     path_to_contents = {}
 
     if path == '.git':
@@ -104,27 +109,35 @@
         repo = args[0]
     else:
         repo = config.repo_full_name
     return gr.Dropdown.update(choices=get_files(repo))
 
 
 with gr.Blocks(theme=gr.themes.Soft(), title="Sweep Chat", css=css) as demo:
+    print("Launching gradio!")
     with gr.Row():
         with gr.Column():
             repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name", value=config.repo_full_name or "")
+        print("Indexing files...")
         with gr.Column(scale=2):
             file_names = gr.Dropdown(choices=get_files(config.repo_full_name), multiselect=True, label="Files")
+        print("Indexed files!")
         repo_full_name.change(get_files_update, repo_full_name, file_names)
 
     with gr.Row():
         with gr.Column(scale=2):
             chatbot = gr.Chatbot(height=750)
         with gr.Column():
             snippets_text = gr.Markdown(value="### Relevant snippets", elem_id="snippets")
-    msg = gr.Textbox(label="Message to Sweep", placeholder="Send a message to Sweep")
+    
+    with gr.Row():
+        with gr.Column(scale=0.5):
+            create_pr_button = gr.Button(value="Create PR", color="blue", interactive=False)
+        with gr.Column(scale=8):
+            msg = gr.Textbox(placeholder="Send a message to Sweep", label=None, elem_id="message_box")
 
     proposed_pr: str | None = None
     searched = False
     selected_snippets = []
     file_to_str = {}
 
     def repo_name_change(repo_full_name):
@@ -177,15 +190,15 @@
         return file_names, build_string()
     
     file_names.change(file_names_change, [file_names], [file_names, snippets_text])
     
     def handle_message_submit(repo_full_name: str, user_message: str, history: list[tuple[str | None, str | None]]):
         if not repo_full_name:
             raise Exception("Set the repository name first")
-        return gr.update(value="", interactive=False), history + [[user_message, None]]
+        return gr.update(value="", interactive=False), history + [[user_message, None]], gr.Button.update(interactive=True)
 
     def handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_names):
         global selected_snippets
         global searched
         message = chat_history[-1][0]
         yield chat_history, snippets_text, file_names
         if not selected_snippets:
@@ -215,15 +228,15 @@
                     "title": proposed_pr["title"],
                     "content": proposed_pr["summary"],
                     "branch_name": proposed_pr["branch"],
                 },
                 messages=chat_history,
             )
             chat_history[-1][1] = f"✅ PR created at {pull_request['html_url']}"
-            yield chat_history, snippets_text, file_names
+            yield chat_history, snippets_text, file_names, "Create PR"
             return
 
         # Generate response
         logger.info("...")
         chat_history.append([None, "..."])
         yield chat_history, snippets_text, file_names
         chat_history[-1][1] = ""
@@ -239,15 +252,15 @@
             stream = api_client.stream_chat(chat_history, selected_snippets)
         function_name = ""
         raw_arguments = ""
         for chunk in stream:
             if chunk.get("content"):
                 token = chunk["content"]
                 chat_history[-1][1] += token
-                yield chat_history, snippets_text, file_names
+                yield chat_history, snippets_text, file_names, "Create PR"
             if chunk.get("function_call"):
                 function_call = chunk["function_call"]
                 function_name = function_name or function_call.get("name")
                 raw_arguments += function_call.get("arguments")
                 chat_history[-1][1] = f"Calling function: `{function_name}`\n```json\n{raw_arguments}\n```"
                 yield chat_history, snippets_text, file_names
         if function_name:
@@ -264,14 +277,21 @@
                     plan="\n".join([f"* `{item['file_path']}`: {item['instructions']}" for item in arguments["plan"]])
                 )
                 yield chat_history, snippets_text, file_names
                 proposed_pr = arguments
             else:
                 raise NotImplementedError
 
-    response = msg.submit(handle_message_submit, [repo_full_name, msg, chatbot], [msg, chatbot], queue=False).then(handle_message_stream, [chatbot, snippets_text, file_names], [chatbot, snippets_text, file_names])
+    response = msg \
+        .submit(handle_message_submit, [repo_full_name, msg, chatbot], [msg, chatbot, create_pr_button], queue=False)\
+        .then(handle_message_stream, [chatbot, snippets_text, file_names], [chatbot, snippets_text, file_names])
     response.then(lambda: gr.update(interactive=True), None, [msg], queue=False)
 
+    def on_create_pr_button_click(chat_history: list[tuple[str | None, str | None]], create_pr_button: str):
+        return chat_history + [(create_pr_button, None)]
+
+    create_pr_button.click(on_create_pr_button_click, [chatbot, create_pr_button], chatbot).then(handle_message_stream, [chatbot, snippets_text, file_names], [chatbot, snippets_text, file_names])
+
 
 if __name__ == "__main__":
     demo.queue()
     demo.launch()
```

### Comparing `sweepai-0.2.6/sweepai/core/chat.py` & `sweepai-0.2.7/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/core/code_repair.py` & `sweepai-0.2.7/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/core/entities.py` & `sweepai-0.2.7/sweepai/core/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 import re
+import string
 from typing import ClassVar, Literal, Type, TypeVar
 from loguru import logger
 from pydantic import BaseModel
 
 try:   # Python 3.11+
     from typing import Self
 except ImportError:  # Python 3.10
@@ -64,25 +66,41 @@
 
 class FilesToChange(RegexMatchableBaseModel):
     files_to_modify: str
     files_to_create: str
     _regex = r"""<create>(?P<files_to_create>.*)</create>\s*<modify>(?P<files_to_modify>.*)</modify>"""
 
 
+# todo (fix double colon regex): Update the split from "file_tree.py : desc" to "file_tree.py\tdesc"
+# tab supremacy 
+def clean_filename(file_name: str):
+    valid_chars = "-_./%s%s" % (string.ascii_letters, string.digits)
+    file_name = ''.join(c for c in file_name if c in valid_chars)
+    file_name = file_name.replace(' ', '')
+    return os.path.normpath(file_name)
+
+def clean_instructions(instructions: str):
+    return instructions.strip()
+
 class FileChangeRequest(RegexMatchableBaseModel):
     filename: str
     instructions: str
     change_type: Literal["modify"] | Literal["create"]
-    _regex = r"""^ *`?(?P<filename>\S*)`?:(?P<instructions>.*)"""
 
     @classmethod
     def from_string(cls: Type[Self], string: str, **kwargs) -> Self:
-        result = super().from_string(string, **kwargs)
-        result.filename = result.filename.strip('`')
-        return result
+        colon_idx = string.find(':')
+        file_name = string[:colon_idx]
+        instructions = string[colon_idx + 1:]
+        file_name = clean_filename(file_name)
+        instructions = clean_instructions(instructions)
+        res = FileChangeRequest(filename=file_name, 
+                                instructions=instructions,
+                                change_type="modify")
+        return res
 
 
 class FileChange(RegexMatchableBaseModel):
     commit_message: str
     code: str
     _regex = r"""Commit Message:(?P<commit_message>.*)<new_file>(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)$"""
     # _regex = r"""Commit Message:(?P<commit_message>.*)(<new_file>|```)(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)($|```)"""
```

### Comparing `sweepai-0.2.6/sweepai/core/prompts.py` & `sweepai-0.2.7/sweepai/core/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,19 +190,17 @@
 * filename_3: instructions_3
 * filename_4: instructions_4
 ...
 </modify>
 """
 
 reply_prompt = """
-Write a response to this user:
-* Ping the user.
+Write a 1-paragraph response to this user:
 * Tell them you have started working on this PR and a rough summary of your plan. 
 * Do not start with "Here is a draft", just write the response.
-* End with "Give me a minute!".
 * Use github markdown to format the response.
 """
 
 create_file_prompt = """
 Think step-by-step regarding the instructions and what should be added to the new file.
 Then create a plan of parts of the code to create, with low-level, detailed references to functions and variable to create, and what each function does.
 Then create the following file using the following instructions:
```

### Comparing `sweepai-0.2.6/sweepai/core/react.py` & `sweepai-0.2.7/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/core/sweep_bot.py` & `sweepai-0.2.7/sweepai/core/sweep_bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     def get_files_to_change(self):
         file_change_requests: list[FileChangeRequest] = []
         for count in range(5):
             try:
                 logger.info(f"Generating for the {count}th time...")
                 files_to_change_response = self.chat(files_to_change_prompt, message_key="files_to_change") # Dedup files to change here
                 files_to_change = FilesToChange.from_string(files_to_change_response)
-                files_to_create: list[str] = files_to_change.files_to_create.split("*")
-                files_to_modify: list[str] = files_to_change.files_to_modify.split("*")
+                files_to_create: list[str] = files_to_change.files_to_create.split("\n*")
+                files_to_modify: list[str] = files_to_change.files_to_modify.split("\n*")
                 for file_change_request, change_type in zip(
                     files_to_create + files_to_modify,
                     ["create"] * len(files_to_create)
                     + ["modify"] * len(files_to_modify),
                 ):
                     file_change_request = file_change_request.strip()
                     if not file_change_request or file_change_request == "None":
@@ -70,20 +70,20 @@
                     return file_change_requests
             except RegexMatchError:
                 logger.warning("Failed to parse! Retrying...")
                 self.delete_messages_from_chat("files_to_change")
                 continue
         raise Exception("Could not generate files to change")
 
-    def generate_pull_request(self):
+    def generate_pull_request(self) -> PullRequest:
         pull_request = None
         for count in range(5):
             try:
                 logger.info(f"Generating for the {count}th time...")
-                pr_text_response = self.chat(pull_request_prompt, message_key="pull_request")
+                pr_text_response = self.chat(pull_request_prompt, message_key="pull_request", model="gpt-3.5-turbo-16k-0613")
             except Exception:
                 logger.warning("Failed to parse! Retrying...")
                 self.undo()
                 continue
             pull_request = PullRequest.from_string(pr_text_response)
             pull_request.branch_name = "sweep/" + pull_request.branch_name[:250]
             return pull_request
@@ -154,15 +154,26 @@
             self.repo.full_name, 
             query=query,
             n_results=num_snippets,
             installation_id=installation_id,
         )
         self.populate_snippets(snippets)
         return snippets
-
+    
+    def validate_file_change_requests(self, file_change_requests: list[FileChangeRequest]):
+        for file_change_request in file_change_requests:
+            try:
+                contents = self.repo.get_contents(file_change_request.filename)
+                if contents:
+                    file_change_request.change_type = "modify"
+                else:
+                    file_change_request.change_type = "create"
+            except:
+                file_change_request.change_type = "create"
+        return file_change_requests
 
 class SweepBot(CodeGenBot, GithubBot):
     def cot_retrieval(self):
         # TODO(sweep): add semantic search using vector db
         # TODO(sweep): add search using webpilot + github
         functions = [
             Function(
@@ -354,14 +365,16 @@
                         branch=branch,
                     )
                 else:
                     new_file_contents, file_name = self.modify_file(
                         file_change_request, contents.decoded_content.decode("utf-8")
                     )
                     new_file_contents = format_contents(new_file_contents, file_markdown)
+                    if contents.decoded_content.decode("utf-8").endswith("\n"):
+                        new_file_contents += "\n"
                     logger.debug(
                         f"{file_name}, {f'Update {file_name}'}, {new_file_contents}, {branch}"
                     )
                     self.repo.update_file(
                         file_name,
                         f'Update {file_name}',
                         new_file_contents,
```

### Comparing `sweepai-0.2.6/sweepai/core/vector_db.py` & `sweepai-0.2.7/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/events.py` & `sweepai-0.2.7/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/handlers/create_pr.py` & `sweepai-0.2.7/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/handlers/on_comment.py` & `sweepai-0.2.7/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/handlers/on_review.py` & `sweepai-0.2.7/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/handlers/on_ticket.py` & `sweepai-0.2.7/sweepai/handlers/on_ticket.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,38 +5,41 @@
 # TODO: Add file validation
 
 import os
 import openai
 
 from loguru import logger
 import modal
+from tabulate import tabulate
 
 from sweepai.core.entities import FileChangeRequest, Snippet
 from sweepai.core.prompts import (
     reply_prompt,
 )
 from sweepai.core.sweep_bot import SweepBot
 from sweepai.core.prompts import issue_comment_prompt
 from sweepai.handlers.create_pr import create_pr
 from sweepai.handlers.on_comment import on_comment
 from sweepai.handlers.on_review import review_pr
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, search_snippets
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
 from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME
-from sweepai.utils.chat_logger import ChatLogger
+from sweepai.utils.chat_logger import ChatLogger, discord_log_error
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 sep = "\n---\n"
-bot_suffix = f"\n{sep}I'm a bot that handles simple bugs and feature requests \
-but I might make mistakes. Please be kind!"
+bot_suffix_starring = "⭐ If you are enjoying Sweep, please [star our repo](https://github.com/sweepai/sweep) so more people can hear about us!"
+bot_suffix = f"\n{sep}I'm a bot that handles simple bugs and feature requests but I might make mistakes. Please be kind!\n<sup>[Join Our Discord](https://discord.com/invite/sweep-ai)"
+
+stars_suffix = "⭐ In the meantime, consider [starring our repo](https://github.com/sweepai/sweep) so more people can hear about us!"
 
 collapsible_template = '''
 <details>
   <summary>{summary}</summary>
 
   {body}
 </details>
@@ -100,57 +103,51 @@
 
     # Add emojis
     eyes_reaction = item_to_react_to.create_reaction("eyes")
 
     # Creates progress bar ASCII for 0-5 states
     progress_headers = [
         None,
-        "Step 1: Code Search",
-        "Step 2: Snippet Analysis",
-        "Step 3: Planning",
-        "Step 4: Coding",
-        "Step 5: Code Review"
-    ]
-    progress_bars = [
-        "[#----------------------------------] 0% Complete",
-        "[#######----------------------------] 20% Complete",
-        "[##############---------------------] 40% Complete",
-        "[#####################--------------] 60% Complete",
-        "[############################-------] 80% Complete",
-        "[###################################] 100% Complete",
+        "Step 1: 🔍 Code Search",
+        "Step 2: 🧐 Snippet Analysis",
+        "Step 3: 📝 Planning",
+        "Step 4: ⌨️ Coding",
+        "Step 5: 🔁 Code Review"
     ]
     def get_progress_bar(index, errored=False):
         if index < 0: index = 0
-        if index >= len(progress_bars): index = -1
+        index *= 20
+        index = min(100, index)
         if errored:
-            return f"## Progress\n{progress_bars[index]} 🚫"
-        return f"## Progress\n{progress_bars[index]}"
+            return f"![{index}%](https://progress-bar.dev/{index}/?&title=Errored&width=600)"
+        return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + ("\n" + stars_suffix if index != -1 else "")
 
     issue_comment = current_issue.create_comment(f"{get_progress_bar(0)}\n{sep}I am currently looking into this ticket! I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.{bot_suffix}")
-    current_index = 0
     past_messages = {}
     def comment_reply(message: str, index: int):
         # Only update the progress bar if the issue generation errors.
         errored = (index == -1)
+        current_index = index
         if index >= 0:
-            current_index = index
             past_messages[index] = message
 
         # Include progress history
         agg_message = None
-        for i in range(current_index+1):
+        for i in range(current_index + 1):
             if i in past_messages:
                 header = progress_headers[i]
                 if header is not None: header = "## " + header + "\n"
                 else: header = "No header\n"
                 msg = header + past_messages[i]
                 if agg_message is None:
                     agg_message = msg
                 else:
                     agg_message = agg_message + f"\n{sep}" + msg
+        if errored:
+            agg_message = "## Error: 🚫 Unable to Complete PR\nIf you would like to report this bug, please join our **[Discord](https://discord.com/invite/sweep-ai)**."
 
         # Update the issue comment
         issue_comment.edit(f"{get_progress_bar(current_index, errored)}\n{sep}{agg_message}{bot_suffix}")
 
     comments = current_issue.get_comments()
     replies_text = ""
     if comment_id:
@@ -159,14 +156,18 @@
                 issue_comment_prompt.format(
                     username=comment.user.login,
                     reply=comment.body,
                 ) for comment in comments
             ]
         )
 
+    def log_error(error_type, exception):
+        content = f"**{error_type} Error**\n{username}: {issue_url}\n```{exception}```"
+        discord_log_error(content)
+
     def fetch_file_contents_with_retry():
         retries = 3
         error = None
         for i in range(retries):
             try:
                 logger.info(f"Fetching relevant files for the {i}th time...")
                 return search_snippets(
@@ -190,26 +191,27 @@
         assert len(snippets) > 0
     except Exception as e:
         logger.error(e)
         comment_reply(
             "It looks like an issue has occured around fetching the files. Perhaps the repo has not been initialized: try removing this repo and adding it back. I'll try again in a minute. If this error persists contact team@sweep.dev.",
             -1
         )
+        log_error("File Fetch", str(e))
         raise e
 
     num_full_files = 2
     num_extended_snippets = 2
 
     most_relevant_snippets = snippets[:num_full_files]
     snippets = snippets[:-num_full_files]
     logger.info("Expanding snippets...")
     for snippet in most_relevant_snippets:
         current_snippet = snippet
         _chunks, metadatas, _ids = chunker.call(
-            current_snippet.content, 
+            current_snippet.content,
             current_snippet.file_path
         )
         segmented_snippets = [
             Snippet(
                 content=current_snippet.content,
                 start=metadata["start"],
                 end=metadata["end"],
@@ -249,72 +251,75 @@
         summary=summary + replies_text,
         snippets=snippets,
         tree=tree, # TODO: Anything in repo tree that has something going through is expanded
     )
 
     chat_logger = ChatLogger({
         'repo_name': repo_name,
-        'issue_url': issue_url,
-        'username': username,
         'title': title,
         'summary': summary + replies_text,
+        "issue_number": issue_number,
+        "issue_url": issue_url,
+        "username": username,
+        "repo_full_name": repo_full_name,
+        "repo_description": repo_description,
+        "installation_id": installation_id,
+        "comment_id": comment_id,
     })
     sweep_bot = SweepBot.from_system_message_content(
         human_message=human_message, repo=repo, is_reply=bool(comments), chat_logger=chat_logger
     )
     sweepbot_retries = 3
     try:
         for i in range(sweepbot_retries):
             # ANALYZE SNIPPETS
             logger.info("CoT retrieval...")
             if sweep_bot.model == "gpt-4-32k-0613":
                 sweep_bot.cot_retrieval()
-            logger.info("Fetching files to modify/create...")
-            file_change_requests = sweep_bot.get_files_to_change()
-            for file_change_request in file_change_requests:
-                try:
-                    contents = repo.get_contents(file_change_request.filename)
-                    if contents:
-                        file_change_request.change_type = "modify"
-                    else:
-                        file_change_request.change_type = "create"
-                except:
-                    file_change_request.change_type = "create"
 
             newline = '\n'
             comment_reply(
-                "I found the following snippets in your repository. I will now analyze this snippets."
+                "I found the following snippets in your repository. I will now analyze this snippets and come up with a plan."
                 + "\n\n"
                 + collapsible_template.format(
                     summary="Some code snippets I looked at (click to expand). If some file is missing from here, you can mention the path in the ticket description.",
                     body="\n".join(
                         [
                             f"https://github.com/{organization}/{repo_name}/blob/{repo.get_commits()[0].sha}/{snippet.file_path}#L{max(snippet.start, 1)}-L{min(snippet.end, snippet.content.count(newline))}\n"
                             for snippet in snippets
                         ]
                     ),
                 ),
                 1
             )
 
             # COMMENT ON ISSUE
-            logger.info("Getting response from ChatGPT...")
-            reply = sweep_bot.chat(reply_prompt, message_key="reply")
-            sweep_bot.delete_messages_from_chat("reply")
-            logger.info("Sending response...")
+            # TODO: removed issue commenting here
+            logger.info("Fetching files to modify/create...")
+            file_change_requests = sweep_bot.get_files_to_change()
+            file_change_requests = sweep_bot.validate_file_change_requests(file_change_requests)
+            table = tabulate(
+                [[f"`{file_change_request.filename}`", file_change_request.instructions] for file_change_request in file_change_requests],
+                headers=["File Path", "Proposed Changes"],
+                tablefmt="pipe"
+            )
+            print(table)
             comment_reply(
-                reply,
+                "From looking through the relevant snippets, I decided to make the following modifications:\n\n" + table + "\n\n",
                 2
             )
 
             # CREATE PR METADATA
             logger.info("Generating PR...")
             pull_request = sweep_bot.generate_pull_request()
+            pull_request_content = pull_request.content.strip().replace("\n", "\n>")
+            pull_request_summary = f"**{pull_request.title}**\n`{pull_request.branch_name}`\n>{pull_request_content}\n"
+
             comment_reply(
-                "I have created a plan for writing the pull request. I am now working on executing my plan and coding the required changes to address this issue.",
+                f"I have created a plan for writing the pull request. I am now working on executing my plan and coding the required changes to address this issue. Here is the planned pull request:\n\n{pull_request_summary}",
                 3
             )
 
             # WRITE PULL REQUEST
             logger.info("Making PR...")
             response = create_pr(file_change_requests, pull_request, sweep_bot, username, installation_id, issue_number)
             if not response or not response["success"]: raise Exception("Failed to create PR")
@@ -327,23 +332,23 @@
 
             try:
                 current_issue.delete_reaction(eyes_reaction.id)
             except:
                 pass
             try:
                 # CODE REVIEW
-                changes_required, review_comment = review_pr(repo=repo, pr=pr, issue_url=issue_url, username=username, 
-                        repo_description=repo_description, title=title, 
+                changes_required, review_comment = review_pr(repo=repo, pr=pr, issue_url=issue_url, username=username,
+                        repo_description=repo_description, title=title,
                         summary=summary, replies_text=replies_text, tree=tree)
                 logger.info(f"Addressing review comment {review_comment}")
                 if changes_required:
-                    on_comment(repo_full_name=repo_full_name, 
-                            repo_description=repo_description, 
+                    on_comment(repo_full_name=repo_full_name,
+                            repo_description=repo_description,
                             comment=review_comment,
-                            username=username, 
+                            username=username,
                             installation_id=installation_id,
                             pr_path=None,
                             pr_line_position=None,
                             pr_number=pr.number)
             except Exception as e:
                 logger.error(e)
 
@@ -355,14 +360,15 @@
             break
     except openai.error.InvalidRequestError as e:
         logger.error(e)
         comment_reply(
             "I'm sorry, but it looks our model has ran out of context length. We're trying to make this happen less, but one way to mitigate this is to code smaller files. If this error persists contact team@sweep.dev.",
             -1
         )
+        log_error("Context Length", str(e))
         posthog.capture(
             username,
             "failed",
             properties={
                 "error": str(e),
                 "reason": "Invalid request error / context length",
                 **metadata,
@@ -371,14 +377,15 @@
         raise e
     except Exception as e:
         logger.error(e)
         comment_reply(
             "I'm sorry, but it looks like an error has occured. Try removing and re-adding the sweep label. If this error persists contact team@sweep.dev.",
             -1
         )
+        log_error("Workflow", str(e))
         posthog.capture(
             username,
             "failed",
             properties={"error": str(e), "reason": "Generic error", **metadata},
         )
         raise e
     else:
```

### Comparing `sweepai-0.2.6/sweepai/slack.py` & `sweepai-0.2.7/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/constants.py` & `sweepai-0.2.7/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/diff.py` & `sweepai-0.2.7/sweepai/utils/diff.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,20 +71,26 @@
     last_section = ""
     if last_section_idx < len(new_file) - 1:
         last_section = new_file[last_section_idx + len("</copied>"):]
         new_file = new_file[:last_section_idx + len("</copied>")] # remove the last section from new_file
     
     # Parse copied sections, first copying the content and then adding whatever is after the copied section
     for copied_section in copied_sections:
-        start_line, end_line = copied_section.split("-")
+        if "-" in copied_section:
+            start_line, end_line = copied_section.split("-")
+        else: # <copied>num</copied>
+            start_line = copied_sections
+            end_line = start_line
+
         start_line = int(start_line) - 1 if int(start_line) - 1 > 0 else 0
         end_line = int(end_line)
         # Check for duplicate lines
         k = 30
         result_file = join_contents_k(result_file, "\n".join(old_file_lines[start_line:end_line]), k)
+        # TODO: Use replace first instead of .replace, since duplicated <copied> sections might cause faulty copy
         new_file = new_file.replace(f"<copied>{copied_section}</copied>\n", "")
         next_section_idx = new_file.index("<copied>") if "<copied>" in new_file else len(new_file)
         # Check for duplicate lines
         result_file = join_contents_k(result_file, new_file[:next_section_idx], k)
         new_file = new_file[next_section_idx:] # remove the first section from new_file
     return result_file + last_section
```

### Comparing `sweepai-0.2.6/sweepai/utils/event_logger.py` & `sweepai-0.2.7/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/file_change_functions.py` & `sweepai-0.2.7/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/github_utils.py` & `sweepai-0.2.7/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/huggingface.py` & `sweepai-0.2.7/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/prompt_constructor.py` & `sweepai-0.2.7/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/scorer.py` & `sweepai-0.2.7/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/snippets.py` & `sweepai-0.2.7/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/sweepai/utils/utils.py` & `sweepai-0.2.7/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.6/setup.py` & `sweepai-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 
 install_requires = \
 ['PyGithub==1.58.2',
  'config-path>=1.0.3,<2.0.0',
  'gradio>=3.35.2,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'requests>=2.28.2,<3.0.0',
+ 'tabulate>=0.9.0,<0.10.0',
  'typer>=0.9.0,<0.10.0',
  'urllib3>=2.0.3,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'Sweep software chores',
     'long_description': '\n<p align="center">\n    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
 path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
-'requests>=2.28.2,<3.0.0', 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0']
-entry_points = \ {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai =
-sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.6',
-'description': 'Sweep software chores', 'long_description': '\n
+'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
+'urllib3>=2.0.3,<3.0.0'] entry_points = \ {'console_scripts': ['sweep =
+sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
+{ 'name': 'sweepai', 'version': '0.2.7', 'description': 'Sweep software
+chores', 'long_description': '\n
                   \n [https://github.com/sweepai/sweep/blob/
   856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]\n
 \n
         \n Spend time reviewing code generated by AI, not writing it.\n
 \n\n
           \nð_Website\n  â¢  \nð_Docs\n  â¢  \nð¢_Discord\n
 \n\nSweep allows you to create and review GitHub issues with ease.\nSimply
```

### Comparing `sweepai-0.2.6/PKG-INFO` & `sweepai-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.2.6
+Version: 0.2.7
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: config-path (>=1.0.3,<2.0.0)
 Requires-Dist: gradio (>=3.35.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/sweepai/sweep/issues
 Project-URL: Community, https://discord.gg/sweep-ai
 Project-URL: documentation, https://docs.sweep.dev
 Project-URL: homepage, https://sweep.dev
 Project-URL: repository, https://github.com/sweepai/sweep
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.2.6 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.2.7 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: PyGithub
 (==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0) Requires-Dist: gradio
 (>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
-requests (>=2.28.2,<3.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
-Dist: urllib3 (>=2.0.3,<3.0.0) Project-URL: Bug Tracker, https://github.com/
-sweepai/sweep/issues Project-URL: Community, https://discord.gg/sweep-ai
-Project-URL: documentation, https://docs.sweep.dev Project-URL: homepage,
-https://sweep.dev Project-URL: repository, https://github.com/sweepai/sweep
-Description-Content-Type: text/markdown
+requests (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-
+Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: urllib3 (>=2.0.3,<3.0.0) Project-
+URL: Bug Tracker, https://github.com/sweepai/sweep/issues Project-URL:
+Community, https://discord.gg/sweep-ai Project-URL: documentation, https://
+docs.sweep.dev Project-URL: homepage, https://sweep.dev Project-URL:
+repository, https://github.com/sweepai/sweep Description-Content-Type: text/
+markdown
                     [https://github.com/sweepai/sweep/blob/
    856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]
           Spend time reviewing code generated by AI, not writing it.
               ð_Website   â¢   ð_Docs   â¢   ð¢_Discord
 Sweep allows you to create and review GitHub issues with ease. Simply describe
 any issue and Sweep will do the rest. It will plan out what needs to be done,
 what changes to make, and write the changes to a PR. Supported languages:
```

