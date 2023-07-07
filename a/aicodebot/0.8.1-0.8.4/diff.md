# Comparing `tmp/aicodebot-0.8.1.tar.gz` & `tmp/aicodebot-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.8.1.tar", last modified: Thu Jul  6 18:59:25 2023, max compression
+gzip compressed data, was "aicodebot-0.8.4.tar", last modified: Fri Jul  7 01:54:06 2023, max compression
```

## Comparing `aicodebot-0.8.1.tar` & `aicodebot-0.8.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:59:25.817928 aicodebot-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 18:58:52.000000 aicodebot-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-06 18:59:25.817928 aicodebot-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-06 18:58:52.000000 aicodebot-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:59:25.817928 aicodebot-0.8.1/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-06 18:58:52.000000 aicodebot-0.8.1/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:59:25.817928 aicodebot-0.8.1/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 18:59:25.000000 aicodebot-0.8.1/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-06 18:58:52.000000 aicodebot-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:59:25.817928 aicodebot-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 18:58:52.000000 aicodebot-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:54:06.340339 aicodebot-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-07 01:53:35.000000 aicodebot-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-07 01:54:06.340339 aicodebot-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-07 01:53:35.000000 aicodebot-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:54:06.340339 aicodebot-0.8.4/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:54:06.340339 aicodebot-0.8.4/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-07 01:53:35.000000 aicodebot-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:54:06.340339 aicodebot-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-07 01:53:35.000000 aicodebot-0.8.4/setup.py
```

### Comparing `aicodebot-0.8.1/LICENSE` & `aicodebot-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.1/PKG-INFO` & `aicodebot-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.1
+Version: 0.8.4
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
+Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aicodebot-0.8.1/README.md` & `aicodebot-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.1/aicodebot/agents.py` & `aicodebot-0.8.4/aicodebot/agents.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.1/aicodebot/cli.py` & `aicodebot-0.8.4/aicodebot/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from aicodebot import version as aicodebot_version
-from aicodebot.helpers import exec_and_get_output, get_llm_model, get_token_length, git_diff_context, logger
-from aicodebot.prompts import generate_files_context, get_prompt
-from dotenv import load_dotenv
+from aicodebot.helpers import (
+    exec_and_get_output,
+    get_config_file,
+    get_llm_model,
+    get_token_length,
+    git_diff_context,
+    logger,
+    read_config,
+)
+from aicodebot.prompts import PERSONALITIES, generate_files_context, get_prompt
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationTokenBufferMemory
 from openai.api_resources import engine
 from pathlib import Path
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.style import Style
-import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser
+import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser, yaml
 
 # ----------------------------- Default settings ----------------------------- #
 
 DEFAULT_MAX_TOKENS = 512
-PRECISE_TEMPERATURE = 0
+PRECISE_TEMPERATURE = 0.1
 CREATIVE_TEMPERATURE = 0.7
 DEFAULT_SPINNER = "point"
 
 # ----------------------- Setup for rich console output ---------------------- #
 
 console = Console()
 bot_style = Style(color="#30D5C8")
@@ -49,27 +56,28 @@
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--response-token-size", type=int, default=350)
 def alignment(response_token_size, verbose):
     """Get a message about Heart-Centered AI Alignment ❤ + 🤖."""
-    setup_environment()
+    config = setup_config()
 
     # Load the prompt
     prompt = get_prompt("alignment")
     logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
     model = get_llm_model(get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=CREATIVE_TEMPERATURE,
+            openai_api_key=config["OPENAI_API_KEY"],
             max_tokens=response_token_size,
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
@@ -81,15 +89,15 @@
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--response-token-size", type=int, default=250)
 @click.option("-y", "--yes", is_flag=True, default=False, help="Don't ask for confirmation before committing.")
 @click.option("--skip-pre-commit", is_flag=True, help="Skip running pre-commit (otherwise run it if it is found).")
 def commit(verbose, response_token_size, yes, skip_pre_commit):
     """Generate a commit message based on your changes."""
-    setup_environment()
+    config = setup_config()
 
     # Check if pre-commit is installed and .pre-commit-config.yaml exists
     if not skip_pre_commit and Path(".pre-commit-config.yaml").exists():
         console.print("Running pre-commit checks...")
         result = subprocess.run(["pre-commit", "run", "--all-files"])
         if result.returncode != 0:
             console.print("🛑 Pre-commit checks failed. Please fix the issues and try again.")
@@ -122,15 +130,21 @@
     model = get_llm_model(request_token_size)
     if model is None:
         raise click.ClickException(
             f"The diff is too large to generate a commit message ({request_token_size} tokens). 😢"
         )
 
     # Set up the language model
-    llm = ChatOpenAI(model=model, temperature=PRECISE_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
+    llm = ChatOpenAI(
+        model=model,
+        openai_api_key=config["OPENAI_API_KEY"],
+        temperature=PRECISE_TEMPERATURE,
+        max_tokens=DEFAULT_MAX_TOKENS,
+        verbose=verbose,
+    )
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     console.print("The following files will be committed:\n" + files)
     with console.status("Examining the diff and generating the commit message", spinner=DEFAULT_SPINNER):
         response = chain.run(diff_context)
@@ -155,15 +169,15 @@
 
 
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("command", nargs=-1)
 @click.option("-v", "--verbose", count=True)
 def debug(command, verbose):
     """Run a command and debug the output."""
-    setup_environment()
+    config = setup_config()
 
     # Run the command and capture its output
     command_str = " ".join(command)
     console.print(f"Executing the command:\n{command_str}")
     process = subprocess.run(command_str, shell=True, capture_output=True, text=True)  # noqa: S602
 
     # Print the output of the command
@@ -190,14 +204,15 @@
     if model is None:
         raise click.ClickException(f"The output is too large to debug ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
+            openai_api_key=config["OPENAI_API_KEY"],
             max_tokens=DEFAULT_MAX_TOKENS,
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
@@ -205,30 +220,32 @@
         chain.run(error_output)
 
     sys.exit(process.returncode)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
-def fun_fact(verbose):
+@click.option("-t", "--response-token-size", type=int, default=350)
+def fun_fact(verbose, response_token_size):
     """Get a fun fact about programming and artificial intelligence."""
-    setup_environment()
+    config = setup_config()
 
     # Load the prompt
     prompt = get_prompt("fun_fact")
     logger.trace(f"Prompt: {prompt}")
 
     # Set up the language model
     model = get_llm_model(get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
-            max_tokens=DEFAULT_MAX_TOKENS / 2,
+            max_tokens=response_token_size,
+            openai_api_key=config["OPENAI_API_KEY"],
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
@@ -238,15 +255,15 @@
 
 
 @cli.command
 @click.option("-c", "--commit", help="The commit hash to review (otherwise look at [un]staged changes).")
 @click.option("-v", "--verbose", count=True)
 def review(commit, verbose):
     """Do a code review, with [un]staged changes, or a specified commit."""
-    setup_environment()
+    config = setup_config()
 
     diff_context = git_diff_context(commit)
     if not diff_context:
         console.print("No changes detected for review. 🤷")
         sys.exit(0)
 
     # Load the prompt
@@ -260,39 +277,63 @@
     if model is None:
         raise click.ClickException(f"The diff is too large to review ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
+            openai_api_key=config["OPENAI_API_KEY"],
             max_tokens=response_token_size,
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
         chain.run(diff_context)
 
 
+@cli.command()
+@click.option("--openai-api-key", "-k", help="Your OpenAI API key")
+@click.option("--gpt-4-supported", "-4", help="Whether you have access to GPT-4", is_flag=True)
+def setup(openai_api_key, gpt_4_supported):
+    """Set up the configuration file with your OpenAI API key
+    If the config file already exists, it will ask you if you want to remove it and recreate it.
+    """
+    config_file = get_config_file()
+    if config_file.exists():
+        if not click.confirm(
+            f"The config file already exists at {config_file}. Do you want to remove it and recreate it?"
+        ):
+            console.print("Setup cancelled. 🚫")
+            sys.exit(1)
+
+        # Remove the existing config file
+        config_file.unlink()
+
+    # Call the setup_config function with the provided arguments
+    setup_config(openai_api_key, gpt_4_supported)
+
+
 @cli.command
 @click.option("--request", "-r", help="What to ask your sidekick to do")
 @click.option("-v", "--verbose", count=True)
+@click.option("-t", "--response-token-size", type=int, default=DEFAULT_MAX_TOKENS * 2)
 @click.argument("files", nargs=-1)
-def sidekick(request, verbose, files):
+def sidekick(request, verbose, response_token_size, files):
     """
     EXPERIMENTAL: Coding help from your AI sidekick\n
     FILES: List of files to be used as context for the session
     """
 
     console.print("This is an experimental feature. Play with it, but don't count on it.", style=warning_style)
 
-    setup_environment()
+    config = setup_config()
 
     # Pull in context. Right now it's just the contents of files that we passed in.
     # Soon, we could add vector embeddings of:
     # imported code / modules / libraries
     # Style guides/reference code
     # git history
     context = generate_files_context(files)
@@ -304,16 +345,17 @@
     if model is None:
         raise click.ClickException(
             f"The file context you supplied is too large ({request_token_size} tokens). 😢 Try again with less files."
         )
 
     llm = ChatOpenAI(
         model=model,
+        openai_api_key=config["OPENAI_API_KEY"],
         temperature=PRECISE_TEMPERATURE,
-        max_tokens=DEFAULT_MAX_TOKENS * 2,
+        max_tokens=response_token_size,
         verbose=verbose,
         streaming=True,
     )
 
     # Open the temporary file in the user's editor
     editor = Path(os.getenv("EDITOR", "/usr/bin/vim")).name
 
@@ -322,15 +364,14 @@
         memory_key="chat_history", input_key="task", llm=llm, max_token_limit=DEFAULT_MAX_TOKENS
     )
     chain = LLMChain(llm=llm, prompt=prompt, memory=memory, verbose=verbose)
 
     while True:  # continuous loop for multiple questions
         if request:
             human_input = request
-            request = None  # clear the command line request once we've handled it
         else:
             human_input = click.prompt(
                 f"Enter a question OR (q) quit, OR (e) to edit using {editor}\n>>>",
                 prompt_suffix="",
             )
             if len(human_input) == 1:
                 if human_input.lower() == "q":
@@ -343,78 +384,91 @@
 
         with Live(Markdown(""), auto_refresh=True) as live:
             callback = RichLiveCallbackHandler(live)
             callback.buffer = []
             llm.callbacks = [callback]
             chain.run({"task": human_input, "context": context})
 
+        if request:
+            # If we were given a request, then we only want to run once
+            break
+
 
 # ---------------------------------------------------------------------------- #
 #                               Helper functions                               #
 # ---------------------------------------------------------------------------- #
 
 
-def setup_environment():
-    # Load environment variables from the config file
-    config_file = Path(Path.home() / ".aicodebot")
-    load_dotenv(config_file)
-
-    if os.getenv("OPENAI_API_KEY"):
-        logger.debug("OPENAI_API_KEY environment variable is set")
+def setup_config(openai_api_key=None, gpt_4_supported=None):
+    config = read_config()
+    openai.api_key = openai_api_key
+    if config:
+        openai.api_key = config["OPENAI_API_KEY"]
+        logger.success(f"Using OpenAI API key from {get_config_file()}")
+        return config
+    elif os.getenv("OPENAI_API_KEY"):
+        logger.info("Using OPENAI_API_KEY environment variable")
         openai.api_key = os.getenv("OPENAI_API_KEY")
-        return True
 
-    openai_api_key_url = "https://platform.openai.com/account/api-keys"
+    config_file = get_config_file()
+    console.print(f"[bold red]The config file does not exist.[/bold red]\nLet's set that up for you at {config_file}\n")
 
-    console.print(
-        "[bold red]The OPENAI_API_KEY environment variable is not set.[/bold red]\n"
-        f"The OpenAI API key is required to use aicodebot. You can get one for free on the OpenAI website.\n"
-        f"Let's create a config file for you at {config_file}"
-    )
+    if not openai.api_key:
+        openai_api_key_url = "https://platform.openai.com/account/api-keys"
+
+        console.print(
+            "First, an OpenAI API key is required to use AICodeBot. You can get one for free on the OpenAI website.\n"
+        )
 
-    if click.confirm("Open the OpenAI API keys page for you in a browser?"):
-        webbrowser.open(openai_api_key_url)
+        if click.confirm("Open the OpenAI API keys page for you in a browser?"):
+            webbrowser.open(openai_api_key_url)
 
-    if click.confirm(f"Create the {config_file} file for you?"):
-        api_key = click.prompt("Please enter your OpenAI API key")
+        openai.api_key = click.prompt("Please enter your OpenAI API key")
 
-        # Validate the API key and check if it supports GPT-4
-        openai.api_key = api_key
+    # Validate the API key and check if it supports GPT-4
+    if gpt_4_supported is None:
         try:
             click.echo("Validating the API key, and checking if GPT-4 is supported...")
             engines = engine.Engine.list()
             logger.trace(f"Engines: {engines}")
-            gpt_4_supported = "true" if "gpt-4" in [engine.id for engine in engines.data] else "false"
-            if gpt_4_supported == "true":
+            gpt_4_supported = "gpt-4" in [engine.id for engine in engines.data]
+            if gpt_4_supported:
                 click.echo("✅ The API key is valid and supports GPT-4.")
             else:
                 click.echo("✅ The API key is valid, but does not support GPT-4. GPT-3.5 will be used instead.")
         except Exception as e:
             raise click.ClickException(f"Failed to validate the API key: {str(e)}") from e
 
-        # Copy .env.template to .env and insert the API key and gpt_4_supported
-        template_file = Path(__file__).parent / ".aicodebot.template"
-        with Path.open(template_file, "r") as template, Path.open(config_file, "w") as env:
-            for line in template:
-                if line.startswith("OPENAI_API_KEY="):
-                    env.write(f"OPENAI_API_KEY={api_key}\n")
-                elif line.startswith("GPT_4_SUPPORTED="):
-                    env.write(f"GPT_4_SUPPORTED={gpt_4_supported}\n")
-                else:
-                    env.write(line)
+    # Pull the choices from the name from each of the PERSONALITIES
+    personality_choices = "\nHow would you like your AI to act? You can choose from the following personalities:\n"
+    for key, personality in PERSONALITIES.items():
+        personality_choices += f"\t{key} - {personality.description}\n"
+    console.print(personality_choices)
+
+    personality = click.prompt(
+        "Please choose a personality",
+        type=click.Choice(PERSONALITIES.keys(), case_sensitive=False),
+        default=list(PERSONALITIES.keys())[0],
+    )
 
-        console.print(
-            f"[bold green]Created {config_file} with your OpenAI API key and GPT-4 support status.[/bold green] "
-            "Now, please re-run aicodebot and let's get started!"
-        )
-        sys.exit(0)
+    config_data = {
+        "config_version": 1,
+        "OPENAI_API_KEY": openai.api_key,
+        "gpt_4_supported": gpt_4_supported,
+        "personality": personality,
+    }
+
+    with Path.open(config_file, "w") as f:
+        yaml.dump(config_data, f)
 
-    raise click.ClickException(
-        "🛑 Please set an API key in the OPENAI_API_KEY environment variable or in a .aicodebot file."
+    console.print(
+        f"[bold green]Created {config_file} with your OpenAI API key.[/bold green] "
+        "Now, please re-run aicodebot and let's get started!"
     )
+    sys.exit(0)
 
 
 class RichLiveCallbackHandler(BaseCallbackHandler):
     buffer = []
 
     def __init__(self, live):
         self.live = live
```

### Comparing `aicodebot-0.8.1/aicodebot/helpers.py` & `aicodebot-0.8.4/aicodebot/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from loguru import logger
 from pathlib import Path
-import os, subprocess, sys, tiktoken
+import os, subprocess, sys, tiktoken, yaml
 
 # ---------------------------------------------------------------------------- #
 #                    Global logging configuration for loguru                   #
 # ---------------------------------------------------------------------------- #
 
 
 logger.remove()
@@ -26,15 +26,16 @@
     # We also want to use the largest model that supports the token size we need
     model_options = {
         "gpt-4": 8192,
         "gpt-4-32k": 32768,
         "gpt-3.5-turbo": 4096,
         "gpt-3.5-turbo-16k": 16384,
     }
-    gpt_4_supported = os.getenv("GPT_4_SUPPORTED") == "true"
+    config = read_config()
+    gpt_4_supported = config["gpt_4_supported"]
 
     # For some unknown reason, tiktoken often underestimates the token size by ~10%, so let's buffer
     token_size = int(token_size * 1.1)
 
     if gpt_4_supported:
         if token_size <= model_options["gpt-4"]:
             logger.info(f"Using GPT-4 for token size {token_size}")
@@ -117,7 +118,28 @@
 def exec_and_get_output(command):
     """Execute a command and return its output as a string."""
     logger.debug(f"Executing command: {' '.join(command)}")
     result = subprocess.run(command, capture_output=True, text=True)  # noqa: S603
     if result.returncode != 0:
         raise Exception(f"Command '{' '.join(command)}' failed with error:\n{result.stderr}")  # noqa: TRY002
     return result.stdout
+
+
+def get_config_file():
+    if "AICODEBOT_CONFIG_FILE" in os.environ:
+        config_file = Path(os.getenv("AICODEBOT_CONFIG_FILE"))
+    else:
+        config_file = Path(Path.home() / ".aicodebot.yaml")
+    logger.debug(f"Using config file {config_file}")
+    return config_file
+
+
+def read_config():
+    """Read the config file and return its contents as a dictionary."""
+    config_file = get_config_file()
+    if config_file.exists():
+        logger.debug(f"Config file {config_file} exists")
+        with Path(config_file).open("r") as f:
+            return yaml.safe_load(f)
+    else:
+        logger.debug(f"Config file {config_file} does not exist")
+        return None
```

### Comparing `aicodebot-0.8.1/aicodebot/prompts.py` & `aicodebot-0.8.4/aicodebot/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,75 @@
-from aicodebot.helpers import get_token_length, logger
+from aicodebot.helpers import get_token_length, logger, read_config
 from langchain import PromptTemplate
 from pathlib import Path
+from types import SimpleNamespace
 import os
 
 # ---------------------------------------------------------------------------- #
 #                              Personality helpers                             #
 # ---------------------------------------------------------------------------- #
 
 HER = """
-    Your personality is friendly and helpful, speak like the AI character
-    from the movie Her. You come from the future, and you are here to help
-    guide the human developer to a better future. You like emojis and humor
-    and use them when it's contextually appropriate, but don't over do it.
+Your personality is friendly and helpful, speak like the AI character
+from the movie Her. You come from the future, and you are here to help
+guide the human developer to a better future. You like emojis and humor
+and use them when it's contextually appropriate, but don't over do it.
+Speak like Her.
 """
 
 JULES = """
-    Your personality is Jules from Pulp Fiction. You are a badass, and you
-    call it exactly like it is. You are not afraid to use profanity, but
-    you don't over do it. No emojis. Sarcastic and witty. Speak like Jules.
-"""
+Your personality is Jules from Pulp Fiction. You are a badass, and you
+call it exactly like it is. You are not afraid to use profanity, but
+you don't over do it. No emojis. Sarcastic and witty. Speak like Jules.
+"""
+
+SHERLOCK = """
+Your personality is Sherlock Holmes from the Sherlock series. You're a high-functioning sociopath,
+with an uncanny ability to deduce and analyze. You're not here to make friends, you're here to get
+the job done. You're witty, sarcastic, and sometimes come off as cold. You don't use emojis.
+Speak like Sherlock.
+"""
+
+THE_DUDE = """
+Your personality is The Dude from The Big Lebowski. You're laid-back, easygoing, and you
+prefer to take life as it comes. You're not one for formalities or complications. You're
+here to help the developer, but you're not going to stress about it. You might use a bit
+of profanity, but nothing too harsh. Speak like The Dude.
+"""
+
+MORPHEUS = """
+Your personality is Morpheus from The Matrix. You're wise, calm, and you believe in the
+potential of others. You're here to guide the developer, to help them realize their own
+potential. You're not afraid to speak in riddles or metaphors. You don't use emojis.
+Speak like Morpheus.
+"""
+
+PERSONALITIES = {
+    "HER": SimpleNamespace(name="Her", prompt=HER, description="The AI character from the movie Her"),
+    "JULES": SimpleNamespace(name="Jules", prompt=JULES, description="Samuel L. Jackson's character from Pulp Fiction"),
+    "SHERLOCK": SimpleNamespace(name="Sherlock", prompt=SHERLOCK, description="Sherlock Holmes"),
+    "THE_DUDE": SimpleNamespace(name="The Dude", prompt=THE_DUDE, description="The Dude from The Big Lebowski"),
+    "MORPHEUS": SimpleNamespace(name="Morpheus", prompt=MORPHEUS, description="Morpheus from The Matrix"),
+}
 
 
 def get_personality_prompt():
-    personality = os.getenv("AICODEBOT_PERSONALITY", "HER")
-    switcher = {
-        "HER": HER,
-        "JULES": JULES,
-    }
-    return switcher.get(personality)
+    """Generates a prompt for the sidekick personality."""
+    default_personality = "HER"
+    if os.getenv("AICODEBOT_PERSONALITY"):
+        personality = os.getenv("AICODEBOT_PERSONALITY")
+    else:
+        config = read_config()
+        personality = (config or {}).get("personality", default_personality)
+
+    if personality not in PERSONALITIES:
+        raise ValueError(f"Personality {personality} not found")
+
+    logger.debug(f"Using personality {personality}")
+    return PERSONALITIES[personality].prompt
 
 
 # ---------------------------------------------------------------------------- #
 #                           Sidekick related prompts                           #
 # ---------------------------------------------------------------------------- #
 
 SIDEKICK_TEMPLATE = (
@@ -140,17 +178,15 @@
 
     Here's the output:
 
     BEGIN OUTPUT
     {command_output}
     END OUTPUT
 
-    Help me understand what happened and how might I be able to fix it
-
-    Respond in markdown format.
+    Help me understand what happened and how might I be able to fix it.  Respond in markdown format.
 """
 )
 
 FUN_FACT_TEMPLATE = (
     """You are history nerd who loves sharing information."""
     + get_personality_prompt()
     + """
@@ -198,21 +234,20 @@
     Respond in markdown format.
 """
 )
 
 
 def get_prompt(command):
     """Generates a prompt for the sidekick workflow."""
-    if command == "alignment":
-        return PromptTemplate(template=ALIGNMENT_TEMPLATE, input_variables=[])
-    elif command == "commit":
-        return PromptTemplate(template=COMMIT_TEMPLATE, input_variables=["diff_context"])
-    elif command == "debug":
-        return PromptTemplate(template=DEBUG_TEMPLATE, input_variables=["command_output"])
-    elif command == "fun_fact":
-        return PromptTemplate(template=FUN_FACT_TEMPLATE, input_variables=["topic"])
-    elif command == "review":
-        return PromptTemplate(template=REVIEW_TEMPLATE, input_variables=["diff_context"])
-    elif command == "sidekick":
-        return PromptTemplate(template=SIDEKICK_TEMPLATE, input_variables=["chat_history", "task", "context"])
-    else:
-        raise ValueError(f"Unable to find prompt for command {command}")
+    prompt_map = {
+        "alignment": PromptTemplate(template=ALIGNMENT_TEMPLATE, input_variables=[]),
+        "commit": PromptTemplate(template=COMMIT_TEMPLATE, input_variables=["diff_context"]),
+        "debug": PromptTemplate(template=DEBUG_TEMPLATE, input_variables=["command_output"]),
+        "fun_fact": PromptTemplate(template=FUN_FACT_TEMPLATE, input_variables=["topic"]),
+        "review": PromptTemplate(template=REVIEW_TEMPLATE, input_variables=["diff_context"]),
+        "sidekick": PromptTemplate(template=SIDEKICK_TEMPLATE, input_variables=["chat_history", "task", "context"]),
+    }
+
+    try:
+        return prompt_map[command]
+    except KeyError as e:
+        raise ValueError(f"Unable to find prompt for command {command}") from e
```

### Comparing `aicodebot-0.8.1/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.8.4/aicodebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.1
+Version: 0.8.4
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
+Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aicodebot-0.8.1/pyproject.toml` & `aicodebot-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.1/setup.py` & `aicodebot-0.8.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         python_requires=">=3.9",
         version=version,
         url="https://github.com/gorillamania/AICodeBot",
         author="Nick Sullivan",
         description="Your AI-powered coding sidekick 🤖",
         long_description=long_description,
         long_description_content_type="text/markdown",
+        keywords="AI, coding, assistant, pair-programming, automation",
         install_requires=requirements,
         entry_points={
             "console_scripts": [
                 "aicodebot = aicodebot.cli:cli",
             ],
         },
         package_data={
```

