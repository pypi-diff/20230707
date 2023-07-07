# Comparing `tmp/sweepai-0.2.8.tar.gz` & `tmp/sweepai-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.8.tar", max compression
+gzip compressed data, was "sweepai-0.2.9.tar", max compression
```

## Comparing `sweepai-0.2.8.tar` & `sweepai-0.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.8/LICENSE
--rw-r--r--   0        0        0     5649 2023-07-07 17:07:48.766509 sweepai-0.2.8/README.md
--rw-r--r--   0        0        0     1395 2023-07-07 17:10:26.860124 sweepai-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.8/sweepai/__init__.py
--rw-r--r--   0        0        0    10759 2023-07-06 22:37:11.532073 sweepai-0.2.8/sweepai/api.py
--rw-r--r--   0        0        0     5974 2023-07-06 00:23:49.508003 sweepai-0.2.8/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10187 2023-07-07 17:07:48.766509 sweepai-0.2.8/sweepai/app/backend.py
--rw-r--r--   0        0        0     1185 2023-07-06 22:37:11.532073 sweepai-0.2.8/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.8/sweepai/app/config.py
--rw-r--r--   0        0        0    11748 2023-07-07 17:08:35.893260 sweepai-0.2.8/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.8/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17384 2023-07-07 17:07:48.766509 sweepai-0.2.8/sweepai/core/chat.py
--rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.8/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8119 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/core/entities.py
--rw-r--r--   0        0        0    13788 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/core/react.py
--rw-r--r--   0        0        0    16366 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3612 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    15807 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.8/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     1808 2023-07-06 22:37:11.535407 sweepai-0.2.8/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/config.py
--rw-r--r--   0        0        0      671 2023-07-06 23:10:39.614513 sweepai-0.2.8/sweepai/utils/constants.py
--rw-r--r--   0        0        0     5230 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.8/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5564 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.8/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.8/sweepai/utils/utils.py
--rw-r--r--   0        0        0     6771 2023-07-07 17:11:03.114292 sweepai-0.2.8/setup.py
--rw-r--r--   0        0        0     6558 2023-07-07 17:11:03.114669 sweepai-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5649 2023-07-07 17:07:48.766509 sweepai-0.2.9/README.md
+-rw-r--r--   0        0        0     1395 2023-07-07 19:43:15.812873 sweepai-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.9/sweepai/__init__.py
+-rw-r--r--   0        0        0    10759 2023-07-06 22:37:11.532073 sweepai-0.2.9/sweepai/api.py
+-rw-r--r--   0        0        0     5979 2023-07-07 19:36:37.902025 sweepai-0.2.9/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10163 2023-07-07 17:21:31.731293 sweepai-0.2.9/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1185 2023-07-06 22:37:11.532073 sweepai-0.2.9/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.9/sweepai/app/config.py
+-rw-r--r--   0        0        0    11493 2023-07-07 19:31:43.131206 sweepai-0.2.9/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.9/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17384 2023-07-07 17:07:48.766509 sweepai-0.2.9/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.9/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8121 2023-07-07 19:15:26.680881 sweepai-0.2.9/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13788 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/core/react.py
+-rw-r--r--   0        0        0    16366 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3612 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    15807 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.9/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     1808 2023-07-06 22:37:11.535407 sweepai-0.2.9/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/config.py
+-rw-r--r--   0        0        0      670 2023-07-07 18:46:43.059593 sweepai-0.2.9/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     5230 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8409 2023-07-07 19:15:26.680881 sweepai-0.2.9/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5564 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.9/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.9/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     6771 2023-07-07 19:43:18.987431 sweepai-0.2.9/setup.py
+-rw-r--r--   0        0        0     6558 2023-07-07 19:43:18.987821 sweepai-0.2.9/PKG-INFO
```

### Comparing `sweepai-0.2.8/LICENSE` & `sweepai-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/README.md` & `sweepai-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/pyproject.toml` & `sweepai-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.8"
+version = "0.2.9"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.2.8/sweepai/api.py` & `sweepai-0.2.9/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/app/api_client.py` & `sweepai-0.2.9/sweepai/app/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                     yield item
                 break
             except json.JSONDecodeError:
                 pass
 
 class APIClient(BaseModel):
     config: SweepChatConfig
-    api_endpoint = f"https://sweepai--{PREFIX}-ui.modal.run"
+    api_endpoint: str = f"https://sweepai--{PREFIX}-ui.modal.run"
 
     def get_installation_id(self):
         results = requests.post(
             self.api_endpoint + "/installation_id",
             json= self.config.dict(),
         )
         if results.status_code == 401:
```

### Comparing `sweepai-0.2.8/sweepai/app/backend.py` & `sweepai-0.2.9/sweepai/app/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     def chat(
         request: ChatRequest,
     ) -> str:
         assert verify_config(request.config)
 
         messages = [Message.from_tuple(message) for message in request.messages]
         chatgpt = ChatGPT(messages=messages[:-1])
-        result = chatgpt.chat(messages[-1].content, model="gpt-3.5-turbo-16k-0613")
+        result = chatgpt.chat(messages[-1].content, model="gpt-4-0613")
         return result
     
     @app.post("/chat_stream")
     def chat_stream(request: ChatRequest):
         assert verify_config(request.config)
         metadata = {
             "function": "ui_create_pr",
@@ -256,15 +256,15 @@
                 repo_description="" # TODO: fill this
             )
             chatgpt = ChatGPT(messages=[Message(role="system", content=system_message, key="system")] + messages[:-1])
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
             raise e
         def stream_chat():
-            for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-3.5-turbo-16k-0613", functions=request.functions, function_call=request.function_call):
+            for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=request.functions, function_call=request.function_call):
                 yield json.dumps(chunk)
             posthog.capture(request.config.github_username, "succeeded", properties=metadata)
         return StreamingResponse(
             stream_chat(),
             media_type="text/event-stream"
         )
     return app
```

### Comparing `sweepai-0.2.8/sweepai/app/cli.py` & `sweepai-0.2.9/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/app/config.py` & `sweepai-0.2.9/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/app/ui.py` & `sweepai-0.2.9/sweepai/app/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from sweepai.app.config import SweepChatConfig
 from sweepai.core.entities import Snippet
 
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
 
-pr_summary_template = '''💡 I'll create the following PR:
+pr_summary_template = '''⏳ I'm creating the following PR...
 
 **{title}**
 {summary}
 
 Here is my plan:
 {plan}
 
-Reply with "ok" to create the PR or anything else to propose changes.'''
+Reply to propose changes to the plan.'''
 
 print("Getting list of repos...")
 github_client = Github(config.github_pat)
 repos = list(github_client.get_user().get_repos())
 print("Done.")
 
 css = '''
@@ -131,15 +131,15 @@
     
     with gr.Row():
         with gr.Column(scale=8):
             msg = gr.Textbox(placeholder="Send a message to Sweep", label=None, elem_id="message_box")
         with gr.Column(scale=0.5):
             create_pr_button = gr.Button(value="Create PR", interactive=False)
 
-    proposed_pr: str | None = None
+    # proposed_pr: str | None = None
     searched = False
     selected_snippets = []
     file_to_str = {}
 
     def repo_name_change(repo_full_name):
         global installation_id
         try:
@@ -214,31 +214,14 @@
             yield chat_history, snippets_text, file_names
             logger.info("Fetched relevant snippets.")
             chat_history[-1][1] = "Found relevant snippets."
             # Update using chat_history
             snippets_text = build_string()
             yield chat_history, snippets_text, file_names
         
-        global proposed_pr
-        if proposed_pr and chat_history[-1][0].strip().lower() in ("okay", "ok"):
-            chat_history[-1][1] = f"⏳ Creating PR..."
-            yield chat_history, snippets_text, file_names
-            pull_request = api_client.create_pr(
-                file_change_requests=[(item["file_path"], item["instructions"]) for item in proposed_pr["plan"]],
-                pull_request={
-                    "title": proposed_pr["title"],
-                    "content": proposed_pr["summary"],
-                    "branch_name": proposed_pr["branch"],
-                },
-                messages=chat_history,
-            )
-            chat_history[-1][1] = f"✅ PR created at {pull_request['html_url']}"
-            yield chat_history, snippets_text, file_names, "Create PR"
-            return
-
         # Generate response
         logger.info("...")
         chat_history.append([None, "..."])
         yield chat_history, snippets_text, file_names
         chat_history[-1][1] = ""
         logger.info("Starting to generate response...")
         if len(chat_history) > 1 and "create pr" in message.lower():
@@ -272,16 +255,26 @@
                 if "branch" not in arguments:
                     arguments["branch"] = arguments["title"].lower().replace(" ", "_").replace("-", "_")[:50]
                 chat_history[-1][1] = pr_summary_template.format(
                     title=arguments["title"],
                     summary=arguments["summary"],
                     plan="\n".join([f"* `{item['file_path']}`: {item['instructions']}" for item in arguments["plan"]])
                 )
-                yield chat_history, snippets_text, file_names
-                proposed_pr = arguments
+                yield chat_history, snippets_text, file_names, "Create PR"
+                pull_request = api_client.create_pr(
+                    file_change_requests=[(item["file_path"], item["instructions"]) for item in arguments["plan"]],
+                    pull_request={
+                        "title": arguments["title"],
+                        "content": arguments["summary"],
+                        "branch_name": arguments["branch"],
+                    },
+                    messages=chat_history,
+                )
+                chat_history.append((None, f"✅ PR created at {pull_request['html_url']}"))
+                yield chat_history, snippets_text, file_names, "Create PR"
             else:
                 raise NotImplementedError
 
     response = msg \
         .submit(handle_message_submit, [repo_full_name, msg, chatbot], [msg, chatbot, create_pr_button], queue=False)\
         .then(handle_message_stream, [chatbot, snippets_text, file_names], [chatbot, snippets_text, file_names])
     response.then(lambda: gr.update(interactive=True), None, [msg], queue=False)
```

### Comparing `sweepai-0.2.8/sweepai/core/chat.py` & `sweepai-0.2.9/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/core/code_repair.py` & `sweepai-0.2.9/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/core/entities.py` & `sweepai-0.2.9/sweepai/core/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     files_to_create: str
     _regex = r"""<create>(?P<files_to_create>.*)</create>\s*<modify>(?P<files_to_modify>.*)</modify>"""
 
 
 # todo (fix double colon regex): Update the split from "file_tree.py : desc" to "file_tree.py\tdesc"
 # tab supremacy
 def clean_filename(file_name: str):
-    valid_chars = "-_./%s%s" % (string.ascii_letters, string.digits)
+    valid_chars = "-_./[]%s%s" % (string.ascii_letters, string.digits)
     file_name = ''.join(c for c in file_name if c in valid_chars)
     file_name = file_name.replace(' ', '')
     return os.path.normpath(file_name)
 
 def clean_instructions(instructions: str):
     return instructions.strip()
```

### Comparing `sweepai-0.2.8/sweepai/core/prompts.py` & `sweepai-0.2.9/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/core/react.py` & `sweepai-0.2.9/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/core/sweep_bot.py` & `sweepai-0.2.9/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/core/vector_db.py` & `sweepai-0.2.9/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/events.py` & `sweepai-0.2.9/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/handlers/create_pr.py` & `sweepai-0.2.9/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/handlers/on_comment.py` & `sweepai-0.2.9/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/handlers/on_review.py` & `sweepai-0.2.9/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/handlers/on_ticket.py` & `sweepai-0.2.9/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/slack.py` & `sweepai-0.2.9/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/chat_logger.py` & `sweepai-0.2.9/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/constants.py` & `sweepai-0.2.9/sweepai/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     ENV = PREFIX
     SWEEP_LOGIN = "sweep-canary[bot]"
 elif PREFIX == "dev":
     APP_ID = 324098
     ENV = PREFIX
     SWEEP_LOGIN = "sweep-nightly[bot]"
 LABEL_NAME = "sweep"
-LABEL_COLOR = "#9400D3"
+LABEL_COLOR = "9400D3"
 LABEL_DESCRIPTION = "Sweep your software chores"
```

### Comparing `sweepai-0.2.8/sweepai/utils/diff.py` & `sweepai-0.2.9/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/event_logger.py` & `sweepai-0.2.9/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/file_change_functions.py` & `sweepai-0.2.9/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/github_utils.py` & `sweepai-0.2.9/sweepai/utils/github_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,22 +171,26 @@
 ) -> tuple[Snippet, str]:
     # Initialize the relevant directories string
     get_relevant_snippets = modal.Function.lookup(DB_NAME, "get_relevant_snippets")
     snippets: list[Snippet] = get_relevant_snippets.call(
         repo.full_name, query, num_files, installation_id=installation_id
     )
     logger.info(f"Snippets: {snippets}")
+    total_file_contents = 0
+    # TODO: We should prioritize the mentioned files
     for snippet in snippets:
         try:
             file_contents = get_file_contents(repo, snippet.file_path, ref=branch)
             if (
-                len(file_contents) > sweep_config.max_file_limit
+                total_file_contents > sweep_config.max_file_limit
             ):  # more than 10000 tokens
                 logger.warning(f"Skipping {snippet.file_path}, too many tokens")
                 continue
+            else:
+                total_file_contents += len(file_contents)
         except github.UnknownObjectException as e:
             logger.warning(f"Error: {e}")
             logger.warning(f"Skipping {snippet.file_path}")
         else:
             snippet.content = file_contents
     tree, file_list = get_tree_and_file_list(
         repo.full_name, 
@@ -194,18 +198,20 @@
         snippet_paths=[snippet.file_path for snippet in snippets]
     )
     for file_path in tqdm(file_list):
         if file_path in query:
             try:
                 file_contents = get_file_contents(repo, file_path, ref=branch)
                 if (
-                    len(file_contents) > sweep_config.max_file_limit
+                    total_file_contents > sweep_config.max_file_limit
                 ):  # more than 10000 tokens
                     logger.warning(f"Skipping {file_path}, too many tokens")
                     continue
+                else:
+                    total_file_contents += len(file_contents)
             except github.UnknownObjectException as e:
                 logger.warning(f"Error: {e}")
                 logger.warning(f"Skipping {file_path}")
             else:
                 snippets.append(
                     Snippet(
                         content=file_contents,
```

### Comparing `sweepai-0.2.8/sweepai/utils/huggingface.py` & `sweepai-0.2.9/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/prompt_constructor.py` & `sweepai-0.2.9/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/scorer.py` & `sweepai-0.2.9/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/snippets.py` & `sweepai-0.2.9/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/sweepai/utils/utils.py` & `sweepai-0.2.9/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.8/setup.py` & `sweepai-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Sweep software chores',
     'long_description': '\n<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/week" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Features\n* Automatic interactive bug fixes & feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created using PR replies & code comments\n* Code snippets embedding-based semantic & popularity search ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* Chain-of-Thought retrieval using GPT Functions\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
 path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
 'urllib3>=2.0.3,<3.0.0'] entry_points = \ {'console_scripts': ['sweep =
 sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
-{ 'name': 'sweepai', 'version': '0.2.8', 'description': 'Sweep software
+{ 'name': 'sweepai', 'version': '0.2.9', 'description': 'Sweep software
 chores', 'long_description': '\n
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
```

### Comparing `sweepai-0.2.8/PKG-INFO` & `sweepai-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.2.8
+Version: 0.2.9
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.2.8 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.2.9 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: PyGithub
 (==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0) Requires-Dist: gradio
 (>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
 requests (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-
 Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: urllib3 (>=2.0.3,<3.0.0) Project-
```

