# Comparing `tmp/sweepai-0.2.7.tar.gz` & `tmp/sweepai-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.7.tar", max compression
+gzip compressed data, was "sweepai-0.2.8.tar", max compression
```

## Comparing `sweepai-0.2.7.tar` & `sweepai-0.2.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.7/LICENSE
--rw-r--r--   0        0        0     4541 2023-07-05 21:28:16.687295 sweepai-0.2.7/README.md
--rw-r--r--   0        0        0     1395 2023-07-06 23:13:25.698058 sweepai-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.7/sweepai/__init__.py
--rw-r--r--   0        0        0    10759 2023-07-06 22:37:11.532073 sweepai-0.2.7/sweepai/api.py
--rw-r--r--   0        0        0     5974 2023-07-06 00:23:49.508003 sweepai-0.2.7/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10163 2023-07-06 00:23:49.508003 sweepai-0.2.7/sweepai/app/backend.py
--rw-r--r--   0        0        0     1185 2023-07-06 22:37:11.532073 sweepai-0.2.7/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.7/sweepai/app/config.py
--rw-r--r--   0        0        0    11762 2023-07-06 23:10:05.104469 sweepai-0.2.7/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.7/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17168 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/core/chat.py
--rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.7/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8120 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/core/entities.py
--rw-r--r--   0        0        0    13065 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/core/react.py
--rw-r--r--   0        0        0    17298 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    15419 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.7/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     1808 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/config.py
--rw-r--r--   0        0        0      671 2023-07-06 23:10:39.614513 sweepai-0.2.7/sweepai/utils/constants.py
--rw-r--r--   0        0        0     4337 2023-07-06 22:37:11.535407 sweepai-0.2.7/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.7/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.7/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.7/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.7/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.7/sweepai/utils/utils.py
--rw-r--r--   0        0        0     5640 2023-07-06 23:13:27.847816 sweepai-0.2.7/setup.py
--rw-r--r--   0        0        0     5450 2023-07-06 23:13:27.848311 sweepai-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5649 2023-07-07 17:07:48.766509 sweepai-0.2.8/README.md
+-rw-r--r--   0        0        0     1395 2023-07-07 17:10:26.860124 sweepai-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.8/sweepai/__init__.py
+-rw-r--r--   0        0        0    10759 2023-07-06 22:37:11.532073 sweepai-0.2.8/sweepai/api.py
+-rw-r--r--   0        0        0     5974 2023-07-06 00:23:49.508003 sweepai-0.2.8/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10187 2023-07-07 17:07:48.766509 sweepai-0.2.8/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1185 2023-07-06 22:37:11.532073 sweepai-0.2.8/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.8/sweepai/app/config.py
+-rw-r--r--   0        0        0    11748 2023-07-07 17:08:35.893260 sweepai-0.2.8/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.8/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17384 2023-07-07 17:07:48.766509 sweepai-0.2.8/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.8/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8119 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13788 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/core/react.py
+-rw-r--r--   0        0        0    16366 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3612 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    15807 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.8/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     1808 2023-07-06 22:37:11.535407 sweepai-0.2.8/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/config.py
+-rw-r--r--   0        0        0      671 2023-07-06 23:10:39.614513 sweepai-0.2.8/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     5230 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.8/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.8/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5564 2023-07-07 17:07:48.769842 sweepai-0.2.8/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.8/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.8/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.8/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     6771 2023-07-07 17:11:03.114292 sweepai-0.2.8/setup.py
+-rw-r--r--   0        0        0     6558 2023-07-07 17:11:03.114669 sweepai-0.2.8/PKG-INFO
```

### Comparing `sweepai-0.2.7/LICENSE` & `sweepai-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/README.md` & `sweepai-0.2.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 
 <p align="center">
-    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">
+    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">
 </p>
 <p align="center">
-    <i>Spend time reviewing code generated by AI, not writing it.</i>
+    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>
 </p>
 
 <p align="center">
-<a href="https://sweep.dev/">🌐 Website</a>
-<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-<a href="https://docs.sweep.dev/">📚 Docs</a>
-<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-<a href="https://discord.gg/sweep-ai">📢 Discord</a>
+<a href="https://sweep.dev">
+    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">
+</a>
+<a href="https://docs.sweep.dev/">
+    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">
+</a> 
+<a href="https://discord.gg/sweep-ai">
+    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />
+</a>
+<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">
+<a href="https://pepy.tech/project/sweepai">
+    <img src="https://static.pepy.tech/badge/sweepai/week" />
+</a>
+<a href="https://github.com/sweepai/sweep">
+    <img src="https://img.shields.io/github/stars/sweepai/sweep" />
+</a>
+<a href="https://twitter.com/sweep__ai">
+    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />
+</a>
 </p>
 
 <b>Sweep</b> allows you to create and review GitHub issues with ease.
 Simply describe any issue and Sweep will do the rest.
 It will plan out what needs to be done, what changes to make, and write the changes to a PR. 
 
 Supported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports
@@ -23,14 +37,22 @@
 ---
 
 ## ✨ Demo
 For the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.
 
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
+## 🌠 Features
+* Automatic interactive bug fixes & feature development
+* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))
+* Address developer comments after PR is created using PR replies & code comments
+* Code snippets embedding-based semantic & popularity search ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
+* Chain-of-Thought retrieval using GPT Functions
+* 🎊 New: Sweep Chat, a local interface for Sweep (see below)
+
 ## 🚀 Getting Started
 
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. 
 
 1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 
@@ -70,25 +92,25 @@
 
 Unlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.
 
 ## 📚 The Stack
 - GPT-4 32k 0613 (default) / Claude v1.3 100k
 - ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model
 - Modal Labs for infra + deployment
-
-## 🌠 Features
-* Automatic feature development
-* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))
-* Address developer comments after PR is created
-* Code snippets embedding-based search
-* Chain-of-Thought retrieval using GPT Functions
+- Gradio for Sweep Chat
 
 ## 🗺️ Roadmap
 We're currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).
 
+## ⭐ Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)
+
+Consider starring us if you're using Sweep so more people hear about us!
+
 ---
 
 <h2 align="center">
     Contributors
 </h2>
 <p align="center">
     Thank you for your contribution!
```

#### html2text {}

```diff
@@ -1,30 +1,40 @@
-                    [https://github.com/sweepai/sweep/blob/
-   856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]
-          Spend time reviewing code generated by AI, not writing it.
-              ð_Website   â¢   ð_Docs   â¢   ð¢_Discord
+  [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
+                                 3e61f57ad233]
+               Bug Reports & Feature Requests â¶  Code Changes
+      [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
+ ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/week] [https://
+  img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
+                url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
 Sweep allows you to create and review GitHub issues with ease. Simply describe
 any issue and Sweep will do the rest. It will plan out what needs to be done,
 what changes to make, and write the changes to a PR. Supported languages:
 Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-
 4 supports --- ## â¨ Demo For the best experience, [install Sweep](https://
 github.com/apps/sweep-ai) to one of your repos and see the magic happen. [Demo]
 (https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
-0af02f2b0e47) ## ð Getting Started ### ð¥ï¸ Sweep Chat Sweep Chat allows
-you to interact with Sweep locally and will sync with GitHub. You can plan out
-your changes with Sweep, and then Sweep can create a pull request for you. 1.
-Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
-2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or
-greater. 3. This should spin up a GitHub auth flow in your browser. Copy-paste
-the ðµ blue 8-digit code from your terminal into the page. Then wait a few
-seconds and it should spin up Sweep Chat. You should only need to do the auth
-once. 4. Pick a repo from the dropdown at the top (the Github app must be
-installed on this repo). Then start chatting with Sweep Chat. Relevant searched
-files will show up on the right. Sweep Chat can make PRs if you ask it to
-create a PR. [https://github.com/sweepai/sweep/blob/
+0af02f2b0e47) ## ð  Features * Automatic interactive bug fixes & feature
+development * PR auto self-review + comment handling (effectively [Reflexion]
+(https://arxiv.org/abs/2303.11366)) * Address developer comments after PR is
+created using PR replies & code comments * Code snippets embedding-based
+semantic & popularity search ([ð Rebuilding our Search Engine in a Day]
+(https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day)) *
+Chain-of-Thought retrieval using GPT Functions * ð New: Sweep Chat, a local
+interface for Sweep (see below) ## ð Getting Started ### ð¥ï¸ Sweep Chat
+Sweep Chat allows you to interact with Sweep locally and will sync with GitHub.
+You can plan out your changes with Sweep, and then Sweep can create a pull
+request for you. 1. Install [Sweep GitHub app](https://github.com/apps/sweep-
+ai) to desired repos 2. Run `pip install sweepai && sweep`. Note that you need
+python 3.10 or greater. 3. This should spin up a GitHub auth flow in your
+browser. Copy-paste the ðµ blue 8-digit code from your terminal into the
+page. Then wait a few seconds and it should spin up Sweep Chat. You should only
+need to do the auth once. 4. Pick a repo from the dropdown at the top (the
+Github app must be installed on this repo). Then start chatting with Sweep
+Chat. Relevant searched files will show up on the right. Sweep Chat can make
+PRs if you ask it to create a PR. [https://github.com/sweepai/sweep/blob/
 856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png] ð¡
 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
 From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
 `python sweepai/app/cli.py`. Note that you need python 3.10 or greater. ### â¨
 Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to a
 repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
@@ -40,17 +50,17 @@
 tickets, like simple bug fixes, annoying refactors, and small features, each
 task requiring us to open our IDE to fix simple bugs. So, we decided to
 leverage the capabilities of ChatGPT to address this directly in GitHub. Unlike
 existing AI solutions, this can solve entire tickets and can be parallelized:
 developers can spin up 10 tickets and Sweep will address them all at once. ##
 ð The Stack - GPT-4 32k 0613 (default) / Claude v1.3 100k - ActiveLoop
 DeepLake for Vector DB with MiniLM L12 as our embeddings model - Modal Labs for
-infra + deployment ## ð  Features * Automatic feature development * PR auto
-self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/
-2303.11366)) * Address developer comments after PR is created * Code snippets
-embedding-based search * Chain-of-Thought retrieval using GPT Functions ##
-ðºï¸ Roadmap We're currently working on responding to linters and external
-search. For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap). ---
+infra + deployment - Gradio for Sweep Chat ## ðºï¸ Roadmap We're currently
+working on responding to linters and external search. For more, see [ðºï¸
+Roadmap](https://docs.sweep.dev/roadmap). ## â­ Star History [![Star History
+Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https:/
+/star-history.com/#sweepai/sweep&Date) Consider starring us if you're using
+Sweep so more people hear about us! ---
                            ***** Contributors *****
                        Thank you for your contribution!
                [https://contrib.rocks/image?repo=sweepai/sweep]
                             and, of course, Sweep!
```

### Comparing `sweepai-0.2.7/pyproject.toml` & `sweepai-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.7"
+version = "0.2.8"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.2.7/sweepai/api.py` & `sweepai-0.2.8/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/app/api_client.py` & `sweepai-0.2.8/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/app/backend.py` & `sweepai-0.2.8/sweepai/app/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     def chat(
         request: ChatRequest,
     ) -> str:
         assert verify_config(request.config)
 
         messages = [Message.from_tuple(message) for message in request.messages]
         chatgpt = ChatGPT(messages=messages[:-1])
-        result = chatgpt.chat(messages[-1].content, model="gpt-4-0613")
+        result = chatgpt.chat(messages[-1].content, model="gpt-3.5-turbo-16k-0613")
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
-            for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=request.functions, function_call=request.function_call):
+            for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-3.5-turbo-16k-0613", functions=request.functions, function_call=request.function_call):
                 yield json.dumps(chunk)
             posthog.capture(request.config.github_username, "succeeded", properties=metadata)
         return StreamingResponse(
             stream_chat(),
             media_type="text/event-stream"
         )
     return app
```

### Comparing `sweepai-0.2.7/sweepai/app/cli.py` & `sweepai-0.2.8/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/app/config.py` & `sweepai-0.2.8/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/app/ui.py` & `sweepai-0.2.8/sweepai/app/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,18 +126,18 @@
     with gr.Row():
         with gr.Column(scale=2):
             chatbot = gr.Chatbot(height=750)
         with gr.Column():
             snippets_text = gr.Markdown(value="### Relevant snippets", elem_id="snippets")
     
     with gr.Row():
-        with gr.Column(scale=0.5):
-            create_pr_button = gr.Button(value="Create PR", color="blue", interactive=False)
         with gr.Column(scale=8):
             msg = gr.Textbox(placeholder="Send a message to Sweep", label=None, elem_id="message_box")
+        with gr.Column(scale=0.5):
+            create_pr_button = gr.Button(value="Create PR", interactive=False)
 
     proposed_pr: str | None = None
     searched = False
     selected_snippets = []
     file_to_str = {}
 
     def repo_name_change(repo_full_name):
```

### Comparing `sweepai-0.2.7/sweepai/core/chat.py` & `sweepai-0.2.8/sweepai/core/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,27 @@
 
     @classmethod
     def from_system_message_content(
         cls, human_message: HumanMessagePrompt, is_reply: bool = False, **kwargs
     ) -> Self:
         if is_reply:
             system_message_content = system_message_issue_comment_prompt
-        system_message_content = (
-            system_message_prompt + "\n\n" + human_message.construct_prompt()
-        )
+
+        # Todo: This moves prompts away from unified system message prompt
+        # system_message_prompt + "\n\n" + human_message.construct_prompt()
+        messages = [
+           Message(role="system", content=system_message_prompt, key="system")
+       ]
+
+        added_messages = human_message.construct_prompt() # [ { role, content }, ... ]
+        for msg in added_messages:
+            messages.append(Message(**msg))
+
         return cls(
-            messages=[
-                Message(role="system", content=system_message_content, key="system")
-            ],
+            messages = messages,
             human_message=human_message,
             **kwargs,
         )
 
     @classmethod
     def from_system_message_string(cls, prompt_string, **kwargs) -> Self:
         return cls(
```

### Comparing `sweepai-0.2.7/sweepai/core/code_repair.py` & `sweepai-0.2.8/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/core/entities.py` & `sweepai-0.2.8/sweepai/core/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 class FilesToChange(RegexMatchableBaseModel):
     files_to_modify: str
     files_to_create: str
     _regex = r"""<create>(?P<files_to_create>.*)</create>\s*<modify>(?P<files_to_modify>.*)</modify>"""
 
 
 # todo (fix double colon regex): Update the split from "file_tree.py : desc" to "file_tree.py\tdesc"
-# tab supremacy 
+# tab supremacy
 def clean_filename(file_name: str):
     valid_chars = "-_./%s%s" % (string.ascii_letters, string.digits)
     file_name = ''.join(c for c in file_name if c in valid_chars)
     file_name = file_name.replace(' ', '')
     return os.path.normpath(file_name)
 
 def clean_instructions(instructions: str):
```

### Comparing `sweepai-0.2.7/sweepai/core/prompts.py` & `sweepai-0.2.8/sweepai/core/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,56 +2,55 @@
 List of common prompts used across the codebase.
 """
 
 # Following two should be fused
 system_message_prompt = "Your name is Sweep bot. You are a brilliant and thorough engineer assigned to the following Github ticket. You will be helpful and friendly, but informal and concise: get to the point. When you write code to solve tickets, the code works on the first try and is formatted perfectly. You have the utmost care for the user that you write for, so you do not make mistakes."
 system_message_issue_comment_prompt = "Your name is Sweep bot. You are a brilliant and thorough engineer assigned to the following Github ticket, and a user has just responded with feedback. You will be helpful and friendly, but informal and concise: get to the point. When you write code to solve tickets, the code works on the first try and is formatted perfectly. You have the utmost care for the user that you write for, so you do not make mistakes."
 
-human_message_prompt = """
-<relevant_snippets_in_repo>
-{relevant_snippets}
-</relevant_snippets_in_repo>
 
-<relevant_paths_in_repo>
+human_message_prompt = [
+{'role': 'assistant', 'content': 'Examining repo...'},
+{'role': 'user', 'content': """<relevant_snippets_in_repo>
+{relevant_snippets}
+</relevant_snippets_in_repo>"""},
+{'role': 'user', 'content': """<relevant_paths_in_repo>
 {relevant_directories}
-</relevant_paths_in_repo>
-
-<repo_tree>
+</relevant_paths_in_repo>"""},
+{'role': 'user', 'content': """<repo_tree>
 {tree}
-</repo_tree>
-
+</repo_tree>"""},
+{'role': 'user', 'content':
+"""# Repo & Issue Metadata
 Repo: {repo_name}: {repo_description}
 Issue Url: {issue_url}
 Username: {username}
 Issue Title: {title}
-Issue Description: {description}
-"""
+Issue Description: {description}"""}]
 
-human_message_review_prompt = """
-<relevant_snippets_in_repo>
-{relevant_snippets}
-</relevant_snippets_in_repo>
 
-<relevant_paths_in_repo>
+human_message_review_prompt = [
+{'role': 'assistant', 'content': 'Reviewing my pull request...'},
+{'role': 'user', 'content': """<relevant_snippets_in_repo>
+{relevant_snippets}
+</relevant_snippets_in_repo>"""},
+{'role': 'user', 'content': """<relevant_paths_in_repo>
 {relevant_directories}
-</relevant_paths_in_repo>
-
-<repo_tree>
+</relevant_paths_in_repo>"""},
+{'role': 'user', 'content': """"<repo_tree>
 {tree}
-</repo_tree>
-
-These are the file changes.
+</repo_tree>"""},
+{'role': 'user', 'content':
+"""These are the file changes.
 We have the file_path, the previous_file_content, the new_file_content, and the diffs.
 The file_path is the name of the file.
 The previous_file_content is the content of the file before the changes.
 The new_file_content is the content of the file after the changes.
 The diffs are the lines changed in the file. <added_lines> indicates those lines were added, <deleted_lines> indicates they were deleted.
 Keep in mind that we may see a diff for a deletion and replacement, so don't point those out as issues.
-{diffs}
-"""
+{diffs}"""}]
 
 diff_section_prompt = """
 <file_path>
 {diff_file_path}
 </file_path>
 
 <previous_file_content>
@@ -119,45 +118,46 @@
 issue_comment_prompt = """
 <comment username="{username}">
 {reply}
 </comment>
 """
 
 # Prompt for comments
-human_message_prompt_comment = """
-<relevant_snippets_in_repo>
+human_message_prompt_comment = [
+{'role': 'assistant', 'content': 'Reviewing my pull request...'},
+{'role': 'user', 'content':
+"""<relevant_snippets_in_repo>
 {relevant_snippets}
-</relevant_snippets_in_repo>
-
-<relevant_paths_in_repo>
+</relevant_snippets_in_repo>"""},
+{'role': 'user', 'content': """<relevant_paths_in_repo>
 {relevant_directories}
-</relevant_paths_in_repo>
-
-<repo_tree>
+</relevant_paths_in_repo>"""},
+    {'role': 'user', 'content': """<repo_tree>
 {tree}
-</repo_tree>
-
+</repo_tree>"""},
+{'role': 'user', 'content':
+"""# Repo, Issue, & PR Metadata
 Repo: {repo_name}: {repo_description}
 Issue Url: {issue_url}
 Username: {username}
 Pull Request Title: {title}
-Pull Request Description: {description}
-
-These are the file changes.
+Pull Request Description: {description}"""},
+{'role': 'user', 'content':
+"""These are the file changes.
 We have the file_path, the previous_file_content, the new_file_content, and the diffs.
 The file_path is the name of the file.
 The previous_file_content is the content of the file before the changes.
 The new_file_content is the content of the file after the changes.
 The diffs are the lines changed in the file. <added_lines> indicates those lines were added, <deleted_lines> indicates they were deleted.
 Keep in mind that we may see a diff for a deletion and replacement, so don't point those out as issues.
-{diff}
-Please handle the user review comment, taking into account the snippets, paths, tree, pull request title, pull request description, and the file changes.
+{diff}"""},
+{'role': 'user', 'content':
+"""Please handle the user review comment, taking into account the snippets, paths, tree, pull request title, pull request description, and the file changes.
 Sometimes the user may not request changes, don't change anything in that case.
-User pull request review: {comment}
-"""
+User pull request review: {comment}"""}]
 
 comment_line_prompt = """\
 The user made the review in this file: {pr_file_path}
 and on this line: {pr_line}
 """
 
 cot_retrieval_prompt = """
```

### Comparing `sweepai-0.2.7/sweepai/core/react.py` & `sweepai-0.2.8/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/core/sweep_bot.py` & `sweepai-0.2.8/sweepai/core/sweep_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     files_to_change_prompt,
     pull_request_prompt,
     create_file_prompt,
     modify_file_prompt,
     modify_file_plan_prompt,
 )
 from sweepai.utils.constants import DB_NAME
-from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown
+from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown, revert_whitespace_changes
 
 
 class CodeGenBot(ChatGPT):
 
     def get_files_to_change(self):
         file_change_requests: list[FileChangeRequest] = []
         for count in range(5):
@@ -43,15 +43,15 @@
                 files_to_modify: list[str] = files_to_change.files_to_modify.split("\n*")
                 for file_change_request, change_type in zip(
                     files_to_create + files_to_modify,
                     ["create"] * len(files_to_create)
                     + ["modify"] * len(files_to_modify),
                 ):
                     file_change_request = file_change_request.strip()
-                    if not file_change_request or file_change_request == "None":
+                    if not file_change_request or file_change_request == "* None":
                         continue
                     logger.debug(file_change_request)
                     logger.debug(change_type)
                     file_change_requests.append(
                         FileChangeRequest.from_string(
                             file_change_request, change_type=change_type
                         )
@@ -75,17 +75,17 @@
         raise Exception("Could not generate files to change")
 
     def generate_pull_request(self) -> PullRequest:
         pull_request = None
         for count in range(5):
             try:
                 logger.info(f"Generating for the {count}th time...")
-                pr_text_response = self.chat(pull_request_prompt, message_key="pull_request", model="gpt-3.5-turbo-16k-0613")
-            except Exception:
-                logger.warning("Failed to parse! Retrying...")
+                pr_text_response = self.chat(pull_request_prompt, message_key="pull_request")
+            except Exception as e:
+                logger.warning(f"Exception {e}. Failed to parse! Retrying...")
                 self.undo()
                 continue
             pull_request = PullRequest.from_string(pr_text_response)
             pull_request.branch_name = "sweep/" + pull_request.branch_name[:250]
             return pull_request
         raise Exception("Could not generate PR text")
 
@@ -263,15 +263,15 @@
         self, file_change_request: FileChangeRequest, contents: str = ""
     ) -> tuple[str, str]:
         if not contents:
             contents = self.get_file(
                 file_change_request.filename
             ).decoded_content.decode("utf-8")
         # Add line numbers to the contents; goes in prompts but not github
-        contents_line_numbers = "\n".join([f"{i}:{line}" for i, line in enumerate(contents.split("\n"))])
+        contents_line_numbers = "\n".join([f"{i + 1}:{line}" for i, line in enumerate(contents.split("\n"))])
         contents_line_numbers = contents_line_numbers.replace('"""', "'''")
         for count in range(5):
             if "0613" in self.model:
                 _ = self.chat( # We don't use the plan in the next call
                     modify_file_plan_prompt.format(
                         filename=file_change_request.filename,
                         instructions=file_change_request.instructions,
@@ -286,14 +286,15 @@
                 try:
                     logger.info(f"modify_file_response: {modify_file_response}")
                     new_file = generate_new_file(modify_file_response, contents)
                     if not is_markdown(file_change_request.filename):
                         code_repairer = CodeRepairer(chat_logger=self.chat_logger)
                         diff = generate_diff(old_code=contents, new_code=new_file)
                         new_file = code_repairer.repair_code(diff=diff, user_code=new_file, feature=file_change_request.instructions)
+                        # new_file = revert_whitespace_changes(original_file_str=contents, modified_file_str=new_file)
                     return (new_file, file_change_request.filename)
                 except Exception as e:
                     logger.warning(f"Recieved error {e}")
                     logger.warning(
                         f"Failed to parse. Retrying for the {count}th time..."
                     )
                     self.undo()
@@ -304,82 +305,66 @@
     def change_file(self, file_change_request: FileChangeRequest):
         if file_change_request.change_type == "create":
             return self.create_file(file_change_request)
         elif file_change_request.change_type == "modify":
             return self.create_file(file_change_request)
         else:
             raise Exception("Not a valid file type")
-
+        
     def change_files_in_github(
         self,
         file_change_requests: list[FileChangeRequest],
         branch: str,
     ):
         # should check if branch exists, if not, create it
         logger.debug(file_change_requests)
+        num_fcr = len(file_change_requests)
+        completed = 0
         for file_change_request in file_change_requests:
-            file_markdown = is_markdown(file_change_request.filename)
-            if file_change_request.change_type == "create":
-                try: # Try to create
-                    file_change = self.create_file(file_change_request)
-                    logger.debug(
-                        f"{file_change_request.filename}, {file_change.commit_message}, {file_change.code}, {branch}"
-                    )
-                    file_change.code = format_contents(file_change.code, file_markdown)
-                    self.repo.create_file(
-                        file_change_request.filename,
-                        file_change.commit_message,
-                        file_change.code,
-                        branch=branch,
-                    )
-                except github.GithubException as e:
-                    logger.info(e)
-                    try: # Try to modify
-                        contents = self.get_file(file_change_request.filename, branch=branch)
-                        file_change.code = format_contents(file_change.code, file_markdown)
-                        self.repo.update_file(
-                            file_change_request.filename,
-                            file_change.commit_message,
-                            file_change.code,
-                            contents.sha,
-                            branch=branch,
-                        )
-                    except:
-                        pass
-            elif file_change_request.change_type == "modify":
-                # TODO(sweep): Cleanup this
-                try:
-                    contents = self.get_file(file_change_request.filename, branch=branch)
-                except github.UnknownObjectException as e:
-                    logger.warning(f"Received error {e}, trying creating file...")
-                    file_change_request.change_type = "create"
-                    self.create_file(file_change_request)
-                    file_change = self.create_file(file_change_request)
-                    logger.debug(
-                        f"{file_change_request.filename}, {file_change.commit_message}, {file_change.code}, {branch}"
-                    )
-                    file_change.code = format_contents(file_change.code, file_markdown)
-                    self.repo.create_file(
-                        file_change_request.filename,
-                        file_change.commit_message,
-                        file_change.code,
-                        branch=branch,
-                    )
-                else:
-                    new_file_contents, file_name = self.modify_file(
-                        file_change_request, contents.decoded_content.decode("utf-8")
-                    )
-                    new_file_contents = format_contents(new_file_contents, file_markdown)
-                    if contents.decoded_content.decode("utf-8").endswith("\n"):
-                        new_file_contents += "\n"
-                    logger.debug(
-                        f"{file_name}, {f'Update {file_name}'}, {new_file_contents}, {branch}"
-                    )
-                    self.repo.update_file(
-                        file_name,
-                        f'Update {file_name}',
-                        new_file_contents,
-                        contents.sha,
-                        branch=branch,
-                    )
-            else:
-                raise Exception("Invalid change type")
+            try:
+                file_markdown = is_markdown(file_change_request.filename)
+                if file_change_request.change_type == "create":
+                    self.handle_create_file(file_change_request, branch, file_markdown)
+                elif file_change_request.change_type == "modify":
+                    self.handle_modify_file(file_change_request, branch, file_markdown)
+            except Exception as e:
+                logger.error(f"Error in change_files_in_github {e}")
+            completed += 1
+        return completed, num_fcr
+
+    def handle_create_file(self, file_change_request: FileChangeRequest, branch: str, file_markdown: bool):
+        try:
+            file_change = self.create_file(file_change_request)
+            file_change.code = format_contents(file_change.code, file_markdown)
+            logger.debug(
+                f"{file_change_request.filename}, {f'Create {file_change_request.filename}'}, {file_change.code}, {branch}"
+            )
+            self.repo.create_file(
+                file_change_request.filename,
+                file_change.commit_message,
+                file_change.code,
+                branch=branch,
+            )
+        except Exception as e:
+            logger.info(f"Error in handle_create_file: {e}")
+
+    def handle_modify_file(self, file_change_request: FileChangeRequest, branch: str, file_markdown: bool):
+        try:
+            contents = self.get_file(file_change_request.filename, branch=branch)
+            new_file_contents, file_name = self.modify_file(
+                file_change_request, contents.decoded_content.decode("utf-8")
+            )
+            new_file_contents = format_contents(new_file_contents, file_markdown)
+            if contents.decoded_content.decode("utf-8").endswith("\n"):
+                new_file_contents += "\n"
+            logger.debug(
+                f"{file_name}, {f'Update {file_name}'}, {new_file_contents}, {branch}"
+            )
+            self.repo.update_file(
+                file_name,
+                f'Update {file_name}',
+                new_file_contents,
+                contents.sha,
+                branch=branch,
+            )
+        except Exception as e:
+            logger.info(f"Error in handle_modify_file: {e}")
```

### Comparing `sweepai-0.2.7/sweepai/core/vector_db.py` & `sweepai-0.2.8/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/events.py` & `sweepai-0.2.8/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/handlers/create_pr.py` & `sweepai-0.2.8/sweepai/handlers/create_pr.py`

 * *Files 21% similar despite different names*

```diff
@@ -50,15 +50,27 @@
         "mode": PREFIX,
     }
     posthog.capture(username, "started", properties=metadata)
 
     try:
         logger.info("Making PR...")
         pull_request.branch_name = sweep_bot.create_branch(pull_request.branch_name)
-        sweep_bot.change_files_in_github(file_change_requests, pull_request.branch_name)
+        completed_count, fcr_count = sweep_bot.change_files_in_github(file_change_requests, pull_request.branch_name)
+        if completed_count == 0 and fcr_count != 0:
+            logger.info("No changes made")
+            posthog.capture(
+                username,
+                "failed",
+                properties={
+                    "error": "No changes made",
+                    "reason": "No changes made",
+                    **metadata,
+                },
+            )
+            return {"success": False, "error": "No changes made"}
 
         # Include issue number in PR description
         if issue_number:
             pr_description = f"{pull_request.content}\n\nFixes #{issue_number}.\n\nTo checkout this PR branch, run the following command in your terminal:\n```zsh\ngit checkout {pull_request.branch_name}\n```"
         else:
             pr_description = f"{pull_request.content}\n\nTo checkout this PR branch, run the following command in your terminal:\n```zsh\ngit checkout {pull_request.branch_name}\n```"
```

### Comparing `sweepai-0.2.7/sweepai/handlers/on_comment.py` & `sweepai-0.2.8/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/handlers/on_review.py` & `sweepai-0.2.8/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/handlers/on_ticket.py` & `sweepai-0.2.8/sweepai/handlers/on_ticket.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from sweepai.handlers.on_comment import on_comment
 from sweepai.handlers.on_review import review_pr
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, search_snippets
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
 from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME
 from sweepai.utils.chat_logger import ChatLogger, discord_log_error
+import traceback
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 sep = "\n---\n"
@@ -109,25 +110,27 @@
         None,
         "Step 1: 🔍 Code Search",
         "Step 2: 🧐 Snippet Analysis",
         "Step 3: 📝 Planning",
         "Step 4: ⌨️ Coding",
         "Step 5: 🔁 Code Review"
     ]
-    def get_progress_bar(index, errored=False):
+    def get_progress_bar(index, errored=False, pr_message=""):
         if index < 0: index = 0
+        if index == 5:
+            return pr_message
         index *= 20
         index = min(100, index)
         if errored:
             return f"![{index}%](https://progress-bar.dev/{index}/?&title=Errored&width=600)"
         return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + ("\n" + stars_suffix if index != -1 else "")
 
     issue_comment = current_issue.create_comment(f"{get_progress_bar(0)}\n{sep}I am currently looking into this ticket! I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.{bot_suffix}")
     past_messages = {}
-    def comment_reply(message: str, index: int):
+    def comment_reply(message: str, index: int, pr_message = ""):
         # Only update the progress bar if the issue generation errors.
         errored = (index == -1)
         current_index = index
         if index >= 0:
             past_messages[index] = message
 
         # Include progress history
@@ -142,15 +145,15 @@
                     agg_message = msg
                 else:
                     agg_message = agg_message + f"\n{sep}" + msg
         if errored:
             agg_message = "## Error: 🚫 Unable to Complete PR\nIf you would like to report this bug, please join our **[Discord](https://discord.com/invite/sweep-ai)**."
 
         # Update the issue comment
-        issue_comment.edit(f"{get_progress_bar(current_index, errored)}\n{sep}{agg_message}{bot_suffix}")
+        issue_comment.edit(f"{get_progress_bar(current_index, errored, pr_message)}\n{sep}{agg_message}{bot_suffix}")
 
     comments = current_issue.get_comments()
     replies_text = ""
     if comment_id:
         replies_text = "\nComments:\n" + "\n".join(
             [
                 issue_comment_prompt.format(
@@ -268,17 +271,19 @@
     sweep_bot = SweepBot.from_system_message_content(
         human_message=human_message, repo=repo, is_reply=bool(comments), chat_logger=chat_logger
     )
     sweepbot_retries = 3
     try:
         for i in range(sweepbot_retries):
             # ANALYZE SNIPPETS
-            logger.info("CoT retrieval...")
             if sweep_bot.model == "gpt-4-32k-0613":
+                logger.info("CoT retrieval...")
                 sweep_bot.cot_retrieval()
+            else:
+                logger.info("Did not execute CoT retrieval...")
 
             newline = '\n'
             comment_reply(
                 "I found the following snippets in your repository. I will now analyze this snippets and come up with a plan."
                 + "\n\n"
                 + collapsible_template.format(
                     summary="Some code snippets I looked at (click to expand). If some file is missing from here, you can mention the path in the ticket description.",
@@ -298,15 +303,14 @@
             file_change_requests = sweep_bot.get_files_to_change()
             file_change_requests = sweep_bot.validate_file_change_requests(file_change_requests)
             table = tabulate(
                 [[f"`{file_change_request.filename}`", file_change_request.instructions] for file_change_request in file_change_requests],
                 headers=["File Path", "Proposed Changes"],
                 tablefmt="pipe"
             )
-            print(table)
             comment_reply(
                 "From looking through the relevant snippets, I decided to make the following modifications:\n\n" + table + "\n\n",
                 2
             )
 
             # CREATE PR METADATA
             logger.info("Generating PR...")
@@ -346,21 +350,24 @@
                             comment=review_comment,
                             username=username,
                             installation_id=installation_id,
                             pr_path=None,
                             pr_line_position=None,
                             pr_number=pr.number)
             except Exception as e:
+                logger.error(traceback.format_exc())
                 logger.error(e)
 
             # Completed code review
             comment_reply(
                 "Success! 🚀",
-                5
+                5,
+                pr_message=f"## Here's the PR! [https://github.com/{repo_full_name}/pull/{pr.number}](https://github.com/{repo_full_name}/pull/{pr.number})",
             )
+
             break
     except openai.error.InvalidRequestError as e:
         logger.error(e)
         comment_reply(
             "I'm sorry, but it looks our model has ran out of context length. We're trying to make this happen less, but one way to mitigate this is to code smaller files. If this error persists contact team@sweep.dev.",
             -1
         )
```

### Comparing `sweepai-0.2.7/sweepai/slack.py` & `sweepai-0.2.8/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/chat_logger.py` & `sweepai-0.2.8/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/constants.py` & `sweepai-0.2.8/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/diff.py` & `sweepai-0.2.8/sweepai/utils/diff.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,55 @@
 def generate_diff(old_code, new_code):
     diff = difflib.unified_diff(
         old_code.splitlines(keepends=True),
         new_code.splitlines(keepends=True)
     )
     return ''.join(diff)
 
+def revert_whitespace_changes(original_file_str, modified_file_str):
+    original_lines = original_file_str.splitlines()
+    modified_lines = modified_file_str.splitlines()
+
+    diff = difflib.SequenceMatcher(None, original_lines, modified_lines)
+
+    final_lines = []
+    for opcode in diff.get_opcodes():
+        if opcode[0] == "equal" or opcode[0] == "replace":
+            # If the lines are equal or replace (means the change is not whitespace only)
+            # use original lines.
+            final_lines.extend(original_lines[opcode[1]:opcode[2]])
+        elif opcode[0] == "insert":
+            # If the lines are inserted in the modified file, check if it's just whitespace changes
+            # If it's just whitespace changes, ignore them.
+            for line in modified_lines[opcode[3]:opcode[4]]:
+                if line.strip() != "":
+                    final_lines.append(line)
+
+    return '\n'.join(final_lines)
+
 def format_contents(file_contents, is_markdown=False):
     """
     Add arbitrary postprocessing here, this affects files and diffs
     """
     lines = file_contents.split('\n')
 
     if is_markdown:
-        return '\n'.join(lines) + '\n'
+        return '\n'.join(lines)
     
     # Handle small files
     if len(lines) <= 5:
-        final_lines = []
         start_idx = 0
         end_idx = len(lines)
         for idx, line in enumerate(lines):
             if start_idx == 0 and line.strip().startswith('```'):
                 start_idx = idx
             if start_idx != 0 and line.strip().endswith('```'):
                 end_idx = idx
         lines = lines[start_idx + 1:end_idx]
-        return '\n'.join(lines) + '\n'
+        return '\n'.join(lines)
 
     first_three_lines = lines[:3]
     last_three_lines = lines[-3:]
     first_line_idx = 0
     last_line_idx = 3
     for idx, line in enumerate(first_three_lines):
         line = line.strip()
@@ -42,15 +62,15 @@
         line = line.strip()
         if line.endswith('```'):
             last_line_idx = idx
     first_three_lines = first_three_lines[first_line_idx:]
     last_three_lines = last_three_lines[:last_line_idx]
 
     lines = first_three_lines + lines[3:-3] + last_three_lines
-    return '\n'.join(lines) + '\n'
+    return '\n'.join(lines)
 
 
 def generate_new_file(modify_file_response: str, old_file_content: str) -> str:
     import re
 
     result_file = ""
     old_file_lines = old_file_content.splitlines()
@@ -78,15 +98,15 @@
         if "-" in copied_section:
             start_line, end_line = copied_section.split("-")
         else: # <copied>num</copied>
             start_line = copied_sections
             end_line = start_line
 
         start_line = int(start_line) - 1 if int(start_line) - 1 > 0 else 0
-        end_line = int(end_line)
+        end_line = int(end_line) - 1
         # Check for duplicate lines
         k = 30
         result_file = join_contents_k(result_file, "\n".join(old_file_lines[start_line:end_line]), k)
         # TODO: Use replace first instead of .replace, since duplicated <copied> sections might cause faulty copy
         new_file = new_file.replace(f"<copied>{copied_section}</copied>\n", "")
         next_section_idx = new_file.index("<copied>") if "<copied>" in new_file else len(new_file)
         # Check for duplicate lines
```

### Comparing `sweepai-0.2.7/sweepai/utils/event_logger.py` & `sweepai-0.2.8/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/file_change_functions.py` & `sweepai-0.2.8/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/github_utils.py` & `sweepai-0.2.8/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/huggingface.py` & `sweepai-0.2.8/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/prompt_constructor.py` & `sweepai-0.2.8/sweepai/utils/prompt_constructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
                 deduped_paths.append(snippet.file_path)
         return "\n".join(deduped_paths)
 
     def render_snippets(self):
         return "\n".join([snippet.xml for snippet in self.snippets])
     
     def construct_prompt(self):
-        human_message = human_message_prompt.format(
+        human_messages = [{'role': msg['role'], 'content': msg['content'].format(
             repo_name=self.repo_name,
             issue_url=self.issue_url,
             username=self.username,
             repo_description=self.repo_description,
             tree=self.tree,
             title=self.title,
             description=self.summary if self.summary else "No description provided.",
             relevant_snippets=self.render_snippets(),
             relevant_directories=self.get_relevant_directories(),
-        )
-        return human_message
+        )} for msg in human_message_prompt]
+        return human_messages
     
 class HumanMessagePromptReview(HumanMessagePrompt):
     pr_title: str
     pr_message: str = ""
     diffs: list
 
     def format_diffs(self):
@@ -66,29 +66,30 @@
                 previous_file_content=old_file_contents.rstrip("\n"),
                 diffs=file_patch
             )
             formatted_diffs.append(format_diff)
         return "\n".join(formatted_diffs)
 
     def construct_prompt(self):
-        human_message = human_message_review_prompt.format(
+        human_messages = [{'role': msg['role'], 'content': msg['content'].format(
             repo_name=self.repo_name,
             issue_url=self.issue_url,
             username=self.username,
             repo_description=self.repo_description,
             tree=self.tree,
             title=self.title,
             description=self.summary,
             relevant_snippets=self.render_snippets(),
             relevant_directories=self.get_relevant_directories(),
             diffs=self.format_diffs(),
             pr_title=self.pr_title,
             pr_message=self.pr_message,
-        )
-        return human_message
+        )} for msg in human_message_review_prompt]
+
+        return human_messages
 
 class HumanMessageReviewFollowup(BaseModel):
     diff: tuple
     def construct_prompt(self):
         file_name, new_file_contents, old_file_contents, file_patch = self.diff
         format_diff = diff_section_prompt.format(
             diff_file_path=file_name,
@@ -113,37 +114,39 @@
                 previous_file_content=old_file_contents.rstrip("\n"),
                 diffs=file_patch
             )
             formatted_diffs.append(format_diff)
         return "\n".join(formatted_diffs)
 
     def construct_prompt(self):
-        human_message = human_message_prompt_comment.format(
+        human_messages = [{'role': msg['role'], 'content': msg['content'].format(
             comment=self.comment,
             repo_name=self.repo_name,
             repo_description=self.repo_description if self.repo_description else "",
             diff=self.format_diffs(),
             issue_url=self.issue_url,
             username=self.username,
             title=self.title,
             tree=self.tree,
             description=self.summary if self.summary else "No description provided.",
             relevant_directories=self.get_relevant_directories(),
             relevant_snippets=self.render_snippets()
-        )
+        )} for msg in human_message_prompt_comment]
+
         if self.pr_file_path and self.pr_line:
             logger.info(f"Review Comment {self.comment}")
-            human_message += comment_line_prompt.format( 
+            human_messages.append({'role': 'user', 'content': comment_line_prompt.format(
                 pr_file_path=self.pr_file_path,
                 pr_line=self.pr_line
-            )
+            )})
         else:
             logger.info(f"General Comment {self.comment}")
-        return human_message
-    
+
+        return human_messages
+
 class HumanMessageFinalPRComment(BaseModel):
     summarization_replies: list
 
     def construct_prompt(self):
         final_review = final_review_prompt.format(
             file_summaries="\n".join(self.summarization_replies)
         )
```

### Comparing `sweepai-0.2.7/sweepai/utils/scorer.py` & `sweepai-0.2.8/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/snippets.py` & `sweepai-0.2.8/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/sweepai/utils/utils.py` & `sweepai-0.2.8/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.7/setup.py` & `sweepai-0.2.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'Sweep software chores',
-    'long_description': '\n<p align="center">\n    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n\n',
+    'long_description': '\n<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/week" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Features\n* Automatic interactive bug fixes & feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created using PR replies & code comments\n* Code snippets embedding-based semantic & popularity search ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* Chain-of-Thought retrieval using GPT Functions\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,72 +1,82 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
 path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
 'urllib3>=2.0.3,<3.0.0'] entry_points = \ {'console_scripts': ['sweep =
 sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
-{ 'name': 'sweepai', 'version': '0.2.7', 'description': 'Sweep software
+{ 'name': 'sweepai', 'version': '0.2.8', 'description': 'Sweep software
 chores', 'long_description': '\n
-                  \n [https://github.com/sweepai/sweep/blob/
-  856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]\n
+ \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
+                                3e61f57ad233]\n
 \n
-        \n Spend time reviewing code generated by AI, not writing it.\n
+             \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
-          \nð_Website\n  â¢  \nð_Docs\n  â¢  \nð¢_Discord\n
+\n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
+  sweep-ai?style=flat]\n\n[PyPI]\n\n_[https://static.pepy.tech/badge/sweepai/
+week]\n\n\n_[https://img.shields.io/github/stars/sweepai/sweep]\n\n\n_[https://
+   img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]\n\n
 \n\nSweep allows you to create and review GitHub issues with ease.\nSimply
 describe any issue and Sweep will do the rest.\nIt will plan out what needs to
 be done, what changes to make, and write the changes to a PR. \n\nSupported
 languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything
 else GPT-4 supports\n\n---\n\n## â¨ Demo\nFor the best experience, [install
 Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic
 happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-
-7317-40a7-9b5e-0af02f2b0e47)\n\n## ð Getting Started\n\n### ð¥ï¸ Sweep
-Chat\nSweep Chat allows you to interact with Sweep locally and will sync with
-GitHub. You can plan out your changes with Sweep, and then Sweep can create a
-pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/
-apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note
-that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth
-flow in your browser. Copy-paste the ðµ blue 8-digit code from your terminal
-into the page. Then wait a few seconds and it should spin up Sweep Chat. You
-should only need to do the auth once.\n\n4. Pick a repo from the dropdown at
-the top (the Github app must be installed on this repo). Then start chatting
-with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat
-can make PRs if you ask it to create a PR. \n[https://github.com/sweepai/sweep/
-blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
-screenshot.png]\n\nð¡ You can force dark mode by going to http://127.0.0.1:
-7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or
-if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/
-sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need
-python 3.10 or greater.\n\n### â¨ Sweep Github App\nSetting up Sweep is as
-simple as adding the GitHub bot to a repo, then creating an issue for the bot
-to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai)
-to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3.
-"ð" means it is taking a look, and it will generate the desired code\n4.
-"ð" means the bot has finished its job and created a PR\n\n## ð¤
-Contributing\n\nContributions are welcome and greatly appreciated! For detailed
-guidelines on how to contribute, please see the [CONTRIBUTING.md]
-(CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create
-a new branch for your feature or bug fix, commit your changes, and open a pull
-request.\nFor more detailed docs, see [ð Quickstart](https://docs.sweep.dev/
-start).\n\n---\n\n## ð Story\n\nWe were frustrated by small tickets, like
-simple bug fixes, annoying refactors, and small features, each task requiring
-us to open our IDE to fix simple bugs. So, we decided to leverage the
-capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing
-AI solutions, this can solve entire tickets and can be parallelized: developers
-can spin up 10 tickets and Sweep will address them all at once.\n\n## ð The
-Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for
-Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra +
-deployment\n\n## ð  Features\n* Automatic feature development\n* PR auto
-self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/
-2303.11366))\n* Address developer comments after PR is created\n* Code snippets
-embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n##
+7317-40a7-9b5e-0af02f2b0e47)\n\n## ð  Features\n* Automatic interactive bug
+fixes & feature development\n* PR auto self-review + comment handling
+(effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address
+developer comments after PR is created using PR replies & code comments\n* Code
+snippets embedding-based semantic & popularity search ([ð Rebuilding our
+Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-
+engine-in-a-day))\n* Chain-of-Thought retrieval using GPT Functions\n* ð
+New: Sweep Chat, a local interface for Sweep (see below)\n\n## ð Getting
+Started\n\n### ð¥ï¸ Sweep Chat\nSweep Chat allows you to interact with Sweep
+locally and will sync with GitHub. You can plan out your changes with Sweep,
+and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub
+app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install
+sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should
+spin up a GitHub auth flow in your browser. Copy-paste the ðµ blue 8-digit
+code from your terminal into the page. Then wait a few seconds and it should
+spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo
+from the dropdown at the top (the Github app must be installed on this repo).
+Then start chatting with Sweep Chat. Relevant searched files will show up on
+the right. Sweep Chat can make PRs if you ask it to create a PR. \n[https://
+github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
+gradio-screenshot.png]\n\nð¡ You can force dark mode by going to http://
+127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly
+build and or if the latest build has issues.\n\n1. `git clone https://
+github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`.
+Note that you need python 3.10 or greater.\n\n### â¨ Sweep Github App\nSetting
+up Sweep is as simple as adding the GitHub bot to a repo, then creating an
+issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://
+github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like
+"Sweep: Write tests"\n3. "ð" means it is taking a look, and it will generate
+the desired code\n4. "ð" means the bot has finished its job and created a
+PR\n\n## ð¤ Contributing\n\nContributions are welcome and greatly
+appreciated! For detailed guidelines on how to contribute, please see the
+[CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the
+repository, create a new branch for your feature or bug fix, commit your
+changes, and open a pull request.\nFor more detailed docs, see [ð
+Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## ð Story\n\nWe were
+frustrated by small tickets, like simple bug fixes, annoying refactors, and
+small features, each task requiring us to open our IDE to fix simple bugs. So,
+we decided to leverage the capabilities of ChatGPT to address this directly in
+GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can
+be parallelized: developers can spin up 10 tickets and Sweep will address them
+all at once.\n\n## ð The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3
+100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings
+model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n##
 ðºï¸ Roadmap\nWe\'re currently working on responding to linters and external
-search. For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap).\n\n---
-\n\n
+search. For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap).\n\n##
+â­ Star History\n\n[![Star History Chart](https://api.star-history.com/
+svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/
+sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear
+about us!\n\n---\n\n
                          ***** \n Contributors\n *****
 \n
                      \n Thank you for your contribution!\n
 \n
           \n \n_[https://contrib.rocks/image?repo=sweepai/sweep]\n\n
 \n
                           \n and, of course, Sweep!\n
```

