# Comparing `tmp/oobabot-0.1.9.tar.gz` & `tmp/oobabot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.9.tar", max compression
+gzip compressed data, was "oobabot-0.2.0.tar", max compression
```

## Comparing `oobabot-0.1.9.tar` & `oobabot-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,31 @@
--rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.9/LICENSE
--rw-r--r--   0        0        0    15491 2023-05-24 05:41:27.585006 oobabot-0.1.9/README.md
--rw-r--r--   0        0        0     1222 2023-05-26 15:58:27.461799 oobabot-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-26 15:58:34.741799 oobabot-0.1.9/src/oobabot/__init__.py
--rw-r--r--   0        0        0      121 2023-05-20 20:17:19.345668 oobabot-0.1.9/src/oobabot/__main__.py
--rw-r--r--   0        0        0     6457 2023-05-26 15:20:56.341750 oobabot-0.1.9/src/oobabot/bot_commands.py
--rw-r--r--   0        0        0     7616 2023-05-25 21:00:13.017091 oobabot-0.1.9/src/oobabot/decide_to_respond.py
--rw-r--r--   0        0        0    29410 2023-05-25 21:00:13.017091 oobabot-0.1.9/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     6991 2023-05-25 16:33:50.006742 oobabot-0.1.9/src/oobabot/discord_utils.py
--rw-r--r--   0        0        0     8993 2023-05-26 15:20:56.341750 oobabot-0.1.9/src/oobabot/fancy_logger.py
--rw-r--r--   0        0        0     3106 2023-05-22 16:17:18.271389 oobabot-0.1.9/src/oobabot/http_client.py
--rw-r--r--   0        0        0    13406 2023-05-22 16:25:27.421377 oobabot-0.1.9/src/oobabot/image_generator.py
--rw-r--r--   0        0        0    10297 2023-05-25 16:33:50.006742 oobabot-0.1.9/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0    13851 2023-05-26 15:21:06.401750 oobabot-0.1.9/src/oobabot/oobabot.py
--rw-r--r--   0        0        0    13391 2023-05-26 15:21:06.401750 oobabot-0.1.9/src/oobabot/overengineered_settings_parser.py
--rw-r--r--   0        0        0     4353 2023-05-22 16:16:39.311390 oobabot-0.1.9/src/oobabot/persona.py
--rw-r--r--   0        0        0     7774 2023-05-22 23:19:07.950798 oobabot-0.1.9/src/oobabot/prompt_generator.py
--rw-r--r--   0        0        0     3243 2023-05-20 20:44:28.735288 oobabot-0.1.9/src/oobabot/repetition_tracker.py
--rw-r--r--   0        0        0     6736 2023-05-22 16:25:27.421377 oobabot-0.1.9/src/oobabot/response_stats.py
--rw-r--r--   0        0        0     9758 2023-05-20 20:33:38.965441 oobabot-0.1.9/src/oobabot/sd_client.py
--rw-r--r--   0        0        0    26244 2023-05-26 15:36:23.871770 oobabot-0.1.9/src/oobabot/settings.py
--rw-r--r--   0        0        0    10906 2023-05-20 20:17:19.345668 oobabot-0.1.9/src/oobabot/templates.py
--rw-r--r--   0        0        0     1481 2023-05-20 20:17:19.345668 oobabot-0.1.9/src/oobabot/types.py
--rw-r--r--   0        0        0    16328 1970-01-01 00:00:00.000000 oobabot-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-04 16:32:46.838921 oobabot-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14771 2023-07-07 09:39:36.542311 oobabot-0.2.0/README.md
+-rw-r--r--   0        0        0     1242 2023-06-28 06:17:56.191776 oobabot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-06-22 17:46:43.191778 oobabot-0.2.0/src/oobabot/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-04 16:34:13.130150 oobabot-0.2.0/src/oobabot/__main__.py
+-rw-r--r--   0        0        0     5701 2023-06-25 07:35:53.143740 oobabot-0.2.0/src/oobabot/audio_commands.py
+-rw-r--r--   0        0        0     4255 2023-06-28 03:58:01.057680 oobabot-0.2.0/src/oobabot/audio_responder.py
+-rw-r--r--   0        0        0     6715 2023-06-24 10:16:43.418003 oobabot-0.2.0/src/oobabot/bot_commands.py
+-rw-r--r--   0        0        0     7616 2023-06-04 16:34:13.130476 oobabot-0.2.0/src/oobabot/decide_to_respond.py
+-rw-r--r--   0        0        0    30180 2023-06-27 18:17:06.105806 oobabot-0.2.0/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0    13538 2023-06-28 06:17:56.192524 oobabot-0.2.0/src/oobabot/discord_utils.py
+-rw-r--r--   0        0        0     7398 2023-06-28 06:17:56.193881 oobabot-0.2.0/src/oobabot/discrivener.py
+-rw-r--r--   0        0        0     7696 2023-06-28 06:17:56.195692 oobabot-0.2.0/src/oobabot/discrivener_message.py
+-rw-r--r--   0        0        0     9954 2023-06-30 16:20:06.306446 oobabot-0.2.0/src/oobabot/fancy_logger.py
+-rw-r--r--   0        0        0     3106 2023-06-25 08:04:52.621295 oobabot-0.2.0/src/oobabot/http_client.py
+-rw-r--r--   0        0        0    13441 2023-06-28 02:27:36.169389 oobabot-0.2.0/src/oobabot/image_generator.py
+-rw-r--r--   0        0        0    10232 2023-06-27 19:34:35.425514 oobabot-0.2.0/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0     8344 2023-06-30 16:20:06.306774 oobabot-0.2.0/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0    13657 2023-07-05 22:59:35.084527 oobabot-0.2.0/src/oobabot/overengineered_settings_parser.py
+-rw-r--r--   0        0        0     4145 2023-07-05 22:59:35.086048 oobabot-0.2.0/src/oobabot/persona.py
+-rw-r--r--   0        0        0     7774 2023-06-04 16:34:13.132066 oobabot-0.2.0/src/oobabot/prompt_generator.py
+-rw-r--r--   0        0        0     3243 2023-06-04 16:34:13.132218 oobabot-0.2.0/src/oobabot/repetition_tracker.py
+-rw-r--r--   0        0        0     6736 2023-06-04 16:34:13.132382 oobabot-0.2.0/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0     9963 2023-06-27 16:19:38.608247 oobabot-0.2.0/src/oobabot/runtime.py
+-rw-r--r--   0        0        0    11466 2023-06-27 18:16:30.917288 oobabot-0.2.0/src/oobabot/sd_client.py
+-rw-r--r--   0        0        0    30574 2023-07-07 09:39:36.544798 oobabot-0.2.0/src/oobabot/settings.py
+-rw-r--r--   0        0        0    10905 2023-07-02 22:19:21.886909 oobabot-0.2.0/src/oobabot/templates.py
+-rw-r--r--   0        0        0     3744 2023-06-28 03:58:01.058041 oobabot-0.2.0/src/oobabot/transcript.py
+-rw-r--r--   0        0        0     5191 2023-06-28 06:17:56.198342 oobabot-0.2.0/src/oobabot/types.py
+-rw-r--r--   0        0        0    12730 2023-06-28 06:17:56.198871 oobabot-0.2.0/src/oobabot/voice_client.py
+-rw-r--r--   0        0        0    15608 1970-01-01 00:00:00.000000 oobabot-0.2.0/PKG-INFO
```

### Comparing `oobabot-0.1.9/LICENSE` & `oobabot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.9/README.md` & `oobabot-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 Real motivation: I wanted a chatbot in my discord that would act like my cat.  A "catbot" if you will.
 
 ## Features
 
 | **`oobabot`**  | how that's awesome |
 |---------------|------------------|
 | **user-supplied persona** | you supply the persona on how would like the bot to behave |
-| **multiple converations** | can track multiple conversational threads, and reply to each in a contextually appropriate way |
+| **multiple conversations** | can track multiple conversational threads, and reply to each in a contextually appropriate way |
 | **watchwords** | can monitor all channels in a server for one or more wakewords or @-mentions |
 | **private conversations** | can chat with you 1:1 in a DM |
 | **good Discord hygiene** | splits messages into independent sentences, pings the author in the first one |
 | **low-latency** | streams the reply live, sentence by sentence.  Provides lower latency, especially on longer responses. |
 | **stats** | track token generation speed, latency, failures and usage |
 | **easy networking** | connects to discord from your machine using websockets, so no need to expose a server to the internet |
 | ✨**Stable Diffusion** | new in v0.1.4!  Optional image generation with AUTOMATIC1111 |
@@ -69,25 +69,24 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-  ³ oobabot  ~/oobabot        oobabot --help         383ms  Tue May 23 18:56:42 2023
 usage: oobabot [-h] [-c CONFIG] [--generate-config] [--invite-url] [--ai-name AI_NAME]
                [--persona PERSONA] [--wakewords [WAKEWORDS ...]]
                [--discord-token DISCORD_TOKEN] [--dont-split-responses]
                [--history-lines HISTORY_LINES] [--ignore-dms] [--reply-in-thread]
                [--stream-responses] [--base-url BASE_URL] [--log-all-the-things]
                [--message-regex MESSAGE_REGEX] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
-               [--extra-prompt-text EXTRA_PROMPT_TEXT] [--use-ai-generated-keywords]
+               [--extra-prompt-text EXTRA_PROMPT_TEXT]
 
-oobabot v0.1.8: Discord bot for oobabooga's text-generation-webui
+oobabot v0.2.0: Discord bot for oobabooga's text-generation-webui
 
 General Settings:
 
   -h, --help
   -c CONFIG, --config CONFIG
                         Path to a config file to read settings from. Command line settings
                         will override settings in this file. (default: config.yml)
@@ -112,15 +111,15 @@
                         if no wakewords are supplied. (default: ['oobabot'])
 
 Discord:
 
   --discord-token DISCORD_TOKEN
                         Token to log into Discord with. For security purposes it's strongly
                         recommended that you set this via the DISCORD_TOKEN environment
-                        variable instead, if possible. (default: )
+                        variable instead, if possible. (default: None)
   --dont-split-responses
                         Post the entire response as a single message, rather than splitting
                         it into separate messages by sentence. (default: False)
   --history-lines HISTORY_LINES
                         Number of lines of chat history the AI will see when generating a
                         response. (default: 7)
   --ignore-dms          If set, the bot will not respond to direct messages. (default:
@@ -150,27 +149,18 @@
                         an image. (default: ['draw me', 'drawing', 'photo', 'pic',
                         'picture', 'image', 'sketch'])
   --stable-diffusion-url STABLE_DIFFUSION_URL
                         URL for an AUTOMATIC1111 Stable Diffusion server. (default: )
   --extra-prompt-text EXTRA_PROMPT_TEXT
                         This will be appended to every image generation prompt sent to
                         Stable Diffusion. (default: )
-  --use-ai-generated-keywords
-                        FEATURE PREVIEW: If set, the bot will ask Oobabooga to generate
-                        image keywords from a user's message. It will then pass the
-                        keywords that Oobabooga produces to Stable Diffusion to finally
-                        generate an image. Otherwise, the bot will simply extract keywords
-                        directly from the user's message using a simple regex. (default:
-                        False)
 
 
 Additional settings can be set in config.yml.  Use the --generate-config option to print a
 new copy of this file to STDOUT.
-
-Please set the 'DISCORD_TOKEN' environment variable to your bot's discord token.
 ```
 
 There are **a lot more settings** in the [config.yml file (sample)](./docs/config.sample.yml) here.
 
 ## Required settings
 
 - **`DISCORD_TOKEN`** environment variable
@@ -186,15 +176,15 @@
     **fish example**
 
     ``` fish
     set -Ux DISCORD_TOKEN ___YOUR_TOKEN___
     ```
 
     In certain environments, it may be difficult to set an environment variable.  In that case, you can also pass the token in as a command-line argument using `--discord-token`.  But doing so might leak the token to other
-    users on a shared sysem, as it will be visible to anyone who can run `ps`.
+    users on a shared system, as it will be visible to anyone who can run `ps`.
 
 - **`--base-url`**
 
     The base URL of oobabooga's streaming web API.  This is
     required if the oobabooga machine is different than where you're running **`oobabot`**.
 
     By default, this will be port 5005 (even though the HTML UI runs on a different port).  The protocol should typically be ws://.
```

### Comparing `oobabot-0.1.9/pyproject.toml` & `oobabot-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oobabot"
-version = "0.1.9"
+version = "0.2.0"
 description = "A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui"
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot"
 
 [tool.poetry.dependencies]
@@ -30,14 +30,15 @@
 pycodestyle = ["-E203", "-W503", "-W504"]
 
 [tool.poetry.group.test.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pre-commit = "^3.2.0"
+pyright = "1.1.315"
 pytest = "^7.1"
 pylint = "^2.17.4"
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 force_sort_within_sections = true
```

### Comparing `oobabot-0.1.9/src/oobabot/bot_commands.py` & `oobabot-0.2.0/src/oobabot/bot_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 """
 Implementation of the bot's slash commands.
 """
 import typing
 
 import discord
 
+from oobabot import audio_commands
 from oobabot import decide_to_respond
 from oobabot import discord_utils
 from oobabot import fancy_logger
+from oobabot import ooba_client
 from oobabot import persona
+from oobabot import prompt_generator
 from oobabot import repetition_tracker
 from oobabot import templates
 
 
 class BotCommands:
     """
     Implementation of the bot's slash commands.
@@ -22,42 +25,37 @@
     def __init__(
         self,
         decide_to_respond: decide_to_respond.DecideToRespond,
         repetition_tracker: repetition_tracker.RepetitionTracker,
         persona: persona.Persona,
         discord_settings: dict,
         template_store: templates.TemplateStore,
+        ooba_client: ooba_client.OobaClient,
+        prompt_generator: prompt_generator.PromptGenerator,
     ):
         self.decide_to_respond = decide_to_respond
         self.repetition_tracker = repetition_tracker
         self.persona = persona
         self.reply_in_thread = discord_settings["reply_in_thread"]
         self.template_store = template_store
+        self.discrivener_location = discord_settings["discrivener_location"]
+        self.discrivener_model_location = discord_settings["discrivener_model_location"]
+        self.audio_commands = audio_commands.AudioCommands(
+            persona,
+            ooba_client,
+            prompt_generator,
+            self.discrivener_location,
+            self.discrivener_model_location,
+        )
 
     async def on_ready(self, client: discord.Client):
         """
         Register commands with Discord.
         """
 
-        async def fail(
-            interaction: discord.Interaction, reason: typing.Optional[str] = None
-        ):
-            msg = reason
-            if msg is None:
-                command = "command"
-                if interaction.command is not None:
-                    command = interaction.command.name
-                fancy_logger.get().warning(
-                    f"{command} called from an unexpected channel: "
-                    + f"{interaction.channel_id}"
-                )
-                msg = f"{command} failed"
-
-            await interaction.response.send_message(msg, ephemeral=True, silent=True)
-
         async def get_messageable(
             interaction: discord.Interaction,
         ) -> (
             typing.Optional[
                 typing.Union[
                     discord.TextChannel,
                     discord.Thread,
@@ -88,23 +86,23 @@
         )
         @discord.app_commands.rename(text_to_send="message")
         @discord.app_commands.describe(
             text_to_send=f"Message to force {self.persona.ai_name} to say."
         )
         async def say(interaction: discord.Interaction, text_to_send: str):
             if interaction.channel_id is None:
-                await fail(interaction)
+                await discord_utils.fail_interaction(interaction)
                 return
 
             # if reply_in_thread is True, we don't want our bot to
             # speak in guild channels, only threads and private messages
             if self.reply_in_thread:
                 channel = await get_messageable(interaction)
                 if channel is None or isinstance(channel, discord.TextChannel):
-                    await fail(
+                    await discord_utils.fail_interaction(
                         interaction, f"{self.persona.ai_name} may only speak in threads"
                     )
                     return
 
             fancy_logger.get().debug(
                 "/say called by user '%s' in channel #%d",
                 interaction.user.name,
@@ -125,15 +123,15 @@
             name="lobotomize",
             description=f"Erase {self.persona.ai_name}'s memory of any message "
             + "before now in this channel.",
         )
         async def lobotomize(interaction: discord.Interaction):
             channel = await get_messageable(interaction)
             if channel is None:
-                await fail(interaction)
+                await discord_utils.fail_interaction(interaction)
                 return
 
             # find the current message in this channel
             # tell the Repetition Tracker to hide messages
             # before this message
             async for message in channel.history(limit=1):
                 channel_name = discord_utils.get_channel_name(channel)
@@ -163,12 +161,19 @@
         fancy_logger.get().debug(
             "Registering commands, sometimes this takes a while..."
         )
 
         tree = discord.app_commands.CommandTree(client)
         tree.add_command(lobotomize)
         tree.add_command(say)
+
+        if discord_utils.is_discrivener_installed(
+            self.discrivener_location,
+            self.discrivener_model_location,
+        ):
+            self.audio_commands.add_commands(tree)
+
         commands = await tree.sync(guild=None)
         for command in commands:
             fancy_logger.get().info(
                 "Registered command: %s: %s", command.name, command.description
             )
```

### Comparing `oobabot-0.1.9/src/oobabot/decide_to_respond.py` & `oobabot-0.2.0/src/oobabot/decide_to_respond.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.9/src/oobabot/discord_bot.py` & `oobabot-0.2.0/src/oobabot/discord_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         self.ai_user_id = -1
 
         self.dont_split_responses = discord_settings["dont_split_responses"]
         self.ignore_dms = discord_settings["ignore_dms"]
         self.reply_in_thread = discord_settings["reply_in_thread"]
         self.stop_markers = discord_settings["stop_markers"]
         self.stream_responses = discord_settings["stream_responses"]
+        self.stream_responses_speed_limit = discord_settings[
+            "stream_responses_speed_limit"
+        ]
 
         # add stopping_strings to stop_markers
         self.stop_markers.extend(self.ooba_client.get_stopping_strings())
 
         super().__init__(intents=discord_utils.get_intents())
 
     async def on_ready(self) -> None:
@@ -326,14 +329,18 @@
             "Request from %s in %s", message.author_name, message.channel_name
         )
 
         repeated_id = self.repetition_tracker.get_throttle_message_id(
             response_channel_id
         )
 
+        # determine if we're responding to a specific message that
+        # summoned us.  If so, find out what message ID that was, so
+        # that we can ignore all messages sent after it (as not to
+        # confuse the AI about what to reply to)
         reference = None
         ignore_all_until_message_id = None
         if is_summon_in_public_channel:
             # we can't use the message reference if we're starting a new thread
             if message.channel_id == response_channel_id:
                 reference = raw_message.to_reference()
             ignore_all_until_message_id = raw_message.id
@@ -365,15 +372,17 @@
         # will be set to true when we abort the response because:
         #  it was empty
         #  it repeated a previous response and we're throttling it
         aborted_by_us = False
         sent_message_count = 0
         try:
             if self.stream_responses:
-                generator = self.ooba_client.request_as_grouped_tokens(prompt_prefix)
+                generator = self.ooba_client.request_as_grouped_tokens(
+                    prompt_prefix, interval=self.stream_responses_speed_limit
+                )
                 last_sent_message = await self._render_streaming_response(
                     generator,
                     this_response_stat,
                     response_channel,
                     response_channel_id,
                     allowed_mentions,
                     reference,
@@ -412,14 +421,17 @@
                             response_channel_id,
                             allowed_mentions=allowed_mentions,
                             reference=reference,
                         )
                         if sent_message is not None:
                             last_sent_message = sent_message
                             sent_message_count += 1
+                            # only use the reference for the first
+                            # message in a multi-message chain
+                            reference = None
                         if abort_response:
                             aborted_by_us = True
                             break
 
         except discord.DiscordException as err:
             fancy_logger.get().error("Error: %s", err, exc_info=True)
             self.response_stats.log_response_failure()
@@ -585,14 +597,18 @@
                     abort_response = True
                     break
 
             if not line and not previous_line:
                 # filter out multiple blank lines in a row
                 continue
 
+            if not line.strip():
+                # filter out lines that are entirely made of whitespace
+                continue
+
             good_lines.append(line)
         return ("\n".join(good_lines), abort_response)
 
     ########
     async def _filter_history_message(
         self,
         message: discord.Message,
@@ -672,19 +688,18 @@
             if items >= limit:
                 return
 
             if ignoring_all:
                 if item.id == ignore_all_until_message_id:
                     ignoring_all = False
                 else:
-                    fancy_logger.get().debug(
-                        "Ignoring message %d because it was sent after %d",
-                        item.id,
-                        ignore_all_until_message_id,
-                    )
+                    # this message was sent after the message we're
+                    # responding to.  So filter out it as to not confuse
+                    # the AI into responding to content from that message
+                    # instead
                     continue
 
             last_returned = item
             (sanitized_message, allow_more) = await self._filter_history_message(
                 item,
                 stop_before_message_id=stop_before_message_id,
             )
```

### Comparing `oobabot-0.1.9/src/oobabot/fancy_logger.py` & `oobabot-0.2.0/src/oobabot/fancy_logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Logging with colors
 """
 
 import html
 import logging
+import sys
 import textwrap
 import typing
 
 from oobabot import discord_utils
 
 FOREGROUND_COLORS = {
     "black": 30,
@@ -138,20 +139,20 @@
         return msg
     result = html.escape(msg)
     return result
 
 
 def init_logging(
     level: typing.Union[int, str],
-    log_to_console: bool = True,
+    running_from_cli: bool = True,
 ) -> None:
     logger = get()
     logger.setLevel(level)
 
-    if log_to_console:
+    if running_from_cli:
         console_handler = logging.StreamHandler()
         console_handler.setLevel(level)
         console_handler.setFormatter(
             ColorfulLoggingFormatter(
                 coloring_book=make_coloring_book(apply_color_console),
             )
         )
@@ -284,7 +285,36 @@
         self.buffer.append(self.format(record))
 
     def get_all(self) -> typing.List[str]:
         return self.buffer.get()
 
 
 recent_logs = RingBufferedHandler()
+
+
+# def log_async_task(fn_inner):
+#     """
+#     Decorator for async tasks that logs unhandled exceptions.
+#     This is useful for tasks that won't be awaited until the
+#     program exits.  With this, the error will be logged as it
+#     happens, rather than when the task is awaited.
+#     """
+
+#     @functools.wraps(fn_inner)
+#     async def wrapper(*args, **kwargs):
+#         try:
+#             return await fn_inner(*args, **kwargs)
+#         except (KeyboardInterrupt, SystemExit):
+#             get().info("Exiting async task due to interrupt")
+#             raise
+#         except Exception as err:
+#             get().error("Unhandled exception from async task", exc_info=err)
+#             raise
+
+#     return wrapper
+
+
+def excepthook(*exc_info):
+    exc_type = exc_info[0]
+    if issubclass(exc_type, (KeyboardInterrupt, SystemExit)):
+        sys.__excepthook__(*exc_info)
+    get().error("Unhandled exception", exc_info=exc_info)
```

### Comparing `oobabot-0.1.9/src/oobabot/http_client.py` & `oobabot-0.2.0/src/oobabot/http_client.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.9/src/oobabot/image_generator.py` & `oobabot-0.2.0/src/oobabot/image_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,14 +264,15 @@
             )
 
         fancy_logger.get().debug(
             "Stable Diffusion: image keywords: %s",
             ", ".join(self.image_words),
         )
 
+    # @fancy_logger.log_async_task
     async def _generate_image(
         self,
         image_prompt: str,
         raw_message: discord.Message,
         response_channel: discord.abc.Messageable,
     ) -> discord.Message:
         is_channel_nsfw = False
```

### Comparing `oobabot-0.1.9/src/oobabot/ooba_client.py` & `oobabot-0.2.0/src/oobabot/ooba_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,14 @@
                 #
                 # {"event": "text_stream", "message_num": 0, "text": ""}
                 # {"event": "text_stream", "message_num": 1, "text": "Oh"}
                 # {"event": "text_stream", "message_num": 2, "text": ","}
                 # {"event": "text_stream", "message_num": 3, "text": " okay"}
                 # {"event": "text_stream", "message_num": 4, "text": "."}
                 # {"event": "stream_end", "message_num": 5}
-                # get_logger().debug(f"Received message: {msg}")
                 if msg.type == aiohttp.WSMsgType.TEXT:
                     # bdata = typing.cast(bytes, msg.data)
                     # get_logger().debug(f"Received data: {bdata}")
 
                     incoming_data = msg.json()
                     if "text_stream" == incoming_data["event"]:
                         self.total_response_tokens += 1
```

### Comparing `oobabot-0.1.9/src/oobabot/oobabot.py` & `oobabot-0.2.0/src/oobabot/runtime.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,94 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-#
 """
-Bot entrypoint.
+Contains all runtime state of the bot.
 """
 
 import asyncio
-import concurrent.futures
+from concurrent import futures
 import contextlib
-import signal
-import sys
 import threading
 import typing
 
 import discord
 
 from oobabot import bot_commands
 from oobabot import decide_to_respond
 from oobabot import discord_bot
-from oobabot import discord_utils
 from oobabot import fancy_logger
 from oobabot import http_client
 from oobabot import image_generator
 from oobabot import ooba_client
 from oobabot import persona
 from oobabot import prompt_generator
 from oobabot import repetition_tracker
 from oobabot import response_stats
 from oobabot import sd_client
 from oobabot import settings
 from oobabot import templates
 
 
-# this warning causes more harm than good here
-# pylint: disable=W0201
-class Oobabot:
+class OobabotRuntimeError(Exception):
     """
-    Main bot class.  Load settings, creates helper objects,
-    and invokes the bot loop.
-
-    Methods:
-        constructor: Loads settings from the command line, environment
-            variables, and config file.  This config may be changed
-            before calling start().
-        start: Start the bot.  Blocks until the bot exits.
-        stop: Stop the bot.  Blocks until the bot exits.
-
-    Class Methods:
-        test_discord_token: Test a discord token to see if it's valid.
-            Requires Internet access.
-        generate_invite_url: Generate a URL that can be used to invite
-            the bot to a server.
+    Raised when the bot encounters an error that it can't recover from.
     """
 
-    def __init__(
-        self,
-        cli_args: typing.List[str],
-    ):
-        """
-        Initialize the bot, and load settings from the command line,
-        environment variables, and config file.  These will be
-        available in self.settings.
-
-        self.settings is an :py:class:`oobabot.settings.Settings` object.
-        """
-        self.startup_lock = threading.Lock()
-        self.settings = settings.Settings()
-
-        self.settings.load(cli_args)
-
-    def start(self):
-        """
-        Start the bot.  Blocks until the bot exits.
-
-        When running from the CLI, the bot would normally exit
-        when the user presses Ctrl-C.  Or otherwise sends a SIGINT
-        or SIGTERM signal.
-
-        This is also where one-off commands are run in CLI mode:
-         - help: Print help and exit
-         - generate_config: Print a the config file and exit
-         - invite_url: Print a URL that can be used to invite the bot
-
-        When running inside another process, the bot will exit
-        when another thread calls stop().
-        """
-
-        with self.startup_lock:
-            self._begin()
-
-            if self.settings.general_settings.get("help"):
-                self.settings.print_help()
-                return
-
-            if self.settings.general_settings.get("generate_config"):
-                self.settings.write_to_stream(out_stream=sys.stdout)
-                if sys.stdout.isatty():
-                    print(self.settings.META_INSTRUCTION, file=sys.stderr)
-                else:
-                    print("# oobabot: config.yml output successfully", file=sys.stderr)
-                return
-
-            if not self.settings.discord_settings.get("discord_token"):
-                msg = (
-                    f"Please set the '{self.settings.DISCORD_TOKEN_ENV_VAR}' "
-                    + "environment variable to your bot's discord token."
-                )
-                print(msg, file=sys.stderr)
-                if self._our_own_main():
-                    sys.exit(1)
-                else:
-                    raise RuntimeError(msg)
-
-            if self.settings.general_settings.get("invite_url"):
-                url = self.generate_invite_url(
-                    self.settings.discord_settings.get_str("discord_token")
-                )
-                print(url)
-                return
-
-            self._prepare_connections()
-
-        asyncio.run(self._init_then_start())
-
-    def _our_own_main(self) -> bool:
-        """
-        Returns True if we're running from the CLI, False if we're
-        running inside another process.
-        """
-        return threading.current_thread() == threading.main_thread()
-
-    def _begin(self):
-        """
-        Called after we've loaded our configuration but before we
-        start the bot.  This is a good place to do any one-time setup
-        for helper objects.
-        """
 
-        fancy_logger.init_logging(
-            level=self.settings.discord_settings.get_str("log_level"),
-            log_to_console=self._our_own_main(),
-        )
+class Runtime:
+    """
+    Contains all the runtime state of the bot.  It should be
+    created once the configuration is known.
+    """
 
+    def __init__(self, settings: settings.Settings):
         # templates used to generate prompts to send to the AI
         # as well as for some UI elements
         self.template_store = templates.TemplateStore(
-            settings=self.settings.template_settings.get_all()
+            settings=settings.template_settings.get_all()
         )
 
         ########################################################
         # Connect to Oobabooga
 
         self.ooba_client = ooba_client.OobaClient(
-            settings=self.settings.oobabooga_settings.get_all(),
+            settings=settings.oobabooga_settings.get_all(),
         )
 
         ########################################################
         # Connect to Stable Diffusion, if configured
 
-        self.stable_diffusion_client = None
-        sd_settings = self.settings.stable_diffusion_settings.get_all()
+        self.stable_diffusion_client: typing.Optional[
+            sd_client.StableDiffusionClient
+        ] = None
+        sd_settings = settings.stable_diffusion_settings.get_all()
         if sd_settings["stable_diffusion_url"]:
             self.stable_diffusion_client = sd_client.StableDiffusionClient(
                 settings=sd_settings,
             )
 
         ########################################################
         # Bot logic
 
         self.persona = persona.Persona(
-            persona_settings=self.settings.persona_settings.get_all()
+            persona_settings=settings.persona_settings.get_all()
         )
 
         # decides which messages the bot will respond to
         self.decide_to_respond = decide_to_respond.DecideToRespond(
-            discord_settings=self.settings.discord_settings.get_all(),
+            discord_settings=settings.discord_settings.get_all(),
             persona=self.persona,
-            interrobang_bonus=self.settings.DECIDE_TO_RESPOND_INTERROBANG_BONUS,
-            time_vs_response_chance=self.settings.TIME_VS_RESPONSE_CHANCE,
+            interrobang_bonus=settings.DECIDE_TO_RESPOND_INTERROBANG_BONUS,
+            time_vs_response_chance=settings.TIME_VS_RESPONSE_CHANCE,
         )
 
         # once we decide to respond, this generates a prompt
         # to send to the AI, given a message history
         self.prompt_generator = prompt_generator.PromptGenerator(
-            discord_settings=self.settings.discord_settings.get_all(),
-            oobabooga_settings=self.settings.oobabooga_settings.get_all(),
+            discord_settings=settings.discord_settings.get_all(),
+            oobabooga_settings=settings.oobabooga_settings.get_all(),
             persona=self.persona,
             template_store=self.template_store,
         )
 
         # tracks of the time spent on responding, success rate, etc.
         self.response_stats = response_stats.AggregateResponseStats(
             fn_get_total_tokens=lambda: self.ooba_client.total_response_tokens
@@ -196,180 +96,160 @@
 
         # generates images, if stable diffusion is configured
         # also includes a UI to regenerate images on demand
         self.image_generator = None
         if self.stable_diffusion_client is not None:
             self.image_generator = image_generator.ImageGenerator(
                 ooba_client=self.ooba_client,
-                persona_settings=self.settings.persona_settings.get_all(),
+                persona_settings=settings.persona_settings.get_all(),
                 prompt_generator=self.prompt_generator,
-                sd_settings=self.settings.stable_diffusion_settings.get_all(),
+                sd_settings=settings.stable_diffusion_settings.get_all(),
                 stable_diffusion_client=self.stable_diffusion_client,
                 template_store=self.template_store,
             )
 
         # if a bot sees itself repeating a message over and over,
         # it will keep doing so forever.  This attempts to fix that.
         # by looking for repeated responses, and deciding how far
         # back in history the bot can see.
         self.repetition_tracker = repetition_tracker.RepetitionTracker(
-            repetition_threshold=self.settings.REPETITION_TRACKER_THRESHOLD
+            repetition_threshold=settings.REPETITION_TRACKER_THRESHOLD
         )
 
         self.bot_commands = bot_commands.BotCommands(
             decide_to_respond=self.decide_to_respond,
             repetition_tracker=self.repetition_tracker,
             persona=self.persona,
-            discord_settings=self.settings.discord_settings.get_all(),
+            discord_settings=settings.discord_settings.get_all(),
             template_store=self.template_store,
+            ooba_client=self.ooba_client,
+            prompt_generator=self.prompt_generator,
         )
 
-        self.discord_bot = None
+        ########################################################
+        # Connect to Discord
 
-        if self._our_own_main():
-            # if we're running as a worker thread in another process,
-            # we can't (and shouldn't) register
-            def exit_handler(signum, _frame):
-                sig_name = signal.Signals(signum).name
-                fancy_logger.get().info("Received signal %s, exiting...", sig_name)
-                self.response_stats.write_stat_summary_to_log()
-                sys.exit(0)
+        self.discord_bot = discord_bot.DiscordBot(
+            bot_commands=self.bot_commands,
+            decide_to_respond=self.decide_to_respond,
+            discord_settings=settings.discord_settings.get_all(),
+            ooba_client=self.ooba_client,
+            image_generator=self.image_generator,
+            persona=self.persona,
+            prompt_generator=self.prompt_generator,
+            repetition_tracker=self.repetition_tracker,
+            response_stats=self.response_stats,
+        )
 
-            signal.signal(signal.SIGINT, exit_handler)
-            signal.signal(signal.SIGTERM, exit_handler)
+        self.discord_token = settings.discord_settings.get_str("discord_token")
+
+    def test_connections(self) -> bool:
+        """
+        Tests that we can connect to all services we depend on.
+        Does not test Discord connectivity.
+
+        Returns True if all configured connections succeeded,
+        False otherwise.
+        """
 
-    def _prepare_connections(self):
-        ########################################################
-        # Test connection to services
         for client in [self.ooba_client, self.stable_diffusion_client]:
             if client is None:
                 continue
 
             fancy_logger.get().info("%s is at %s", client.service_name, client.base_url)
             try:
                 client.test_connection()
                 fancy_logger.get().info("Connected to %s!", client.service_name)
             except (ValueError, http_client.OobaHttpClientError) as err:
-                fancy_logger.get().error(
+                fancy_logger.get().warning(
                     "Could not connect to %s server: [%s]",
                     client.service_name,
                     client.base_url,
                 )
-                fancy_logger.get().error("Please check the URL and try again.")
+                fancy_logger.get().warning("Please check the URL and try again.")
                 if err.__cause__ is not None:
                     fancy_logger.get().error("Reason: %s", err.__cause__)
-                if self._our_own_main():
-                    sys.exit(1)
-                else:
-                    raise
-
-        ########################################################
-        # Connect to Discord
+                return False
+        return True
 
-        fancy_logger.get().info("Connecting to Discord... ")
-        self.discord_bot = discord_bot.DiscordBot(
-            bot_commands=self.bot_commands,
-            decide_to_respond=self.decide_to_respond,
-            discord_settings=self.settings.discord_settings.get_all(),
-            ooba_client=self.ooba_client,
-            image_generator=self.image_generator,
-            persona=self.persona,
-            prompt_generator=self.prompt_generator,
-            repetition_tracker=self.repetition_tracker,
-            response_stats=self.response_stats,
-        )
-
-    async def _init_then_start(self):
+    async def run(self):
         """
         Opens HTTP connections to oobabooga and stable diffusion,
         then connects to Discord.  Blocks until the bot is stopped.
+
+        Raises OobabotRuntimeError if the bot cannot connect to Discord.
         """
-        if self.discord_bot is None:
-            raise RuntimeError("Discord bot not initialized")
 
         async with contextlib.AsyncExitStack() as stack:
             for context_manager in [
                 self.ooba_client,
                 self.stable_diffusion_client,
             ]:
                 if context_manager is not None:
                     await stack.enter_async_context(context_manager)
 
             try:
-                await self.discord_bot.start(
-                    self.settings.discord_settings.get_str("discord_token")
-                )
+                fancy_logger.get().info("Connecting to Discord... ")
+                await self.discord_bot.start(self.discord_token)
+                fancy_logger.get().info("Discord bot exited.")
+
+            except discord.errors.PrivilegedIntentsRequired as err:
+                fancy_logger.get().warning("Could not log in to Discord: %s", err)
+                fancy_logger.get().warning(
+                    "The bot token you provided does not have the required "
+                    + "gateway intents.  Did you remember to enable both "
+                    + "'SERVER MEMBERS INTENT' and 'MESSAGE CONTENT INTENT' "
+                    + "in the bot's settings on Discord?"
+                )
+                raise OobabotRuntimeError(
+                    "Could not log in to Discord: intents not set"
+                ) from err
+
             except discord.LoginFailure as err:
-                fancy_logger.get().error("Could not log in to Discord: %s", err)
-                fancy_logger.get().error("Please check the token and try again.")
-                if self._our_own_main():
-                    sys.exit(1)
+                fancy_logger.get().warning("Could not log in to Discord: %s", err)
+                fancy_logger.get().warning("Please check the token and try again.")
+                raise OobabotRuntimeError(
+                    "Could not log in to Discord: invalid token"
+                ) from err
+
             finally:
                 await self.discord_bot.close()
         fancy_logger.get().info("Disconnected from Discord.")
 
     def stop(self, wait_timeout: float = 5.0) -> None:
         """
         Stops the bot, if it's running.  Safe to be called
         from a separate thread from the one that called run().
 
-        Blocks until the bot is gracefully stopped.
-        """
-        if self.discord_bot is None:
-            return
-
-        async def close_and_set() -> None:
-            if self.discord_bot is None:
-                return
-            await self.discord_bot.close()
-
-        with self.startup_lock:
-            try:
-                # if discord is already stopped, then their .loop is set
-                # _MissingSentinel.  So instead check if it's still connected.
-                if self.discord_bot.is_closed():
-                    fancy_logger.get().info("Discord bot already stopped.")
-                    return
-
-                future = asyncio.run_coroutine_threadsafe(
-                    close_and_set(),
-                    self.discord_bot.loop,
-                )
-                future.result(timeout=wait_timeout)
-            except RuntimeError:
-                # this can happen if the main application is shutting down
-                fancy_logger.get().warning("Discord bot is already stopped.")
-            except concurrent.futures.TimeoutError:
-                fancy_logger.get().warning(
-                    "Discord bot did not stop in time, it might be busted."
-                )
-
-    @classmethod
-    def test_discord_token(cls, discord_token: str) -> bool:
+        Blocks until the bot is gracefully stopped, or until
+        wait_timeout seconds have passed, whichever comes first.
         """
-        Tests a discord token to see if it's valid.  Can be called from any thread.
 
-        Requires Internet connectivity.
+        self.response_stats.write_stat_summary_to_log()
 
-        Returns True if it was able to connect with the token, False if it isn't.
-        """
-        return asyncio.run(discord_utils.test_discord_token(discord_token))
-
-    @classmethod
-    def generate_invite_url(cls, discord_token: str) -> str:
-        """
-        Generates an invite URL for the bot with the given token.
-
-        Can be called from any thread.  Does not require Internet connectivity.
-        """
-        ai_user_id = discord_utils.get_user_id_from_token(discord_token)
-        return discord_utils.generate_invite_url(ai_user_id)
-
-
-# pylint: enable=W0201
+        # if we're on our main thread, then we can just terminate
+        # the bot loop directly.  But if we're on a separate thread,
+        # then we need to call it from the  discord bot's event loop.
+        if threading.current_thread() == threading.main_thread():
+            self.discord_bot.loop.stop()
+            return
 
+        try:
+            # if discord is already stopped, then their .loop is set
+            # _MissingSentinel.  So instead check if it's still connected.
+            if self.discord_bot.is_closed():
+                fancy_logger.get().info("Discord bot already stopped.")
+                return
 
-def main():
-    # create the object and load our settings
-    oobabot = Oobabot(sys.argv[1:])
-    # start the loop
-    oobabot.start()
+            future = asyncio.run_coroutine_threadsafe(
+                self.discord_bot.close(),
+                self.discord_bot.loop,
+            )
+            future.result(timeout=wait_timeout)
+        except RuntimeError as err:
+            # this can happen if the main application is shutting down
+            fancy_logger.get().error("Could not stop Discord bot: %s", err)
+            raise OobabotRuntimeError("Discord bot is already stopped.") from err
+        except futures.TimeoutError:
+            fancy_logger.get().warning(
+                "Discord bot did not stop in time, it might be busted."
+            )
```

### Comparing `oobabot-0.1.9/src/oobabot/overengineered_settings_parser.py` & `oobabot-0.2.0/src/oobabot/overengineered_settings_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 
 import oobabot
 
 YAML_WIDTH = 88
 DIVIDER = "# " * (YAML_WIDTH >> 1)
 INDENT_UNIT = 2
 
+
+class ConfigFileMissingError(Exception):
+    """
+    Raised when the config file is missing.
+    """
+
+
 SettingDictType = typing.Dict[
     str, typing.Union[bool, int, float, str, typing.List[str]]
 ]
 
 SettingValueType = typing.Union[
     bool, int, float, str, typing.List[str], SettingDictType
 ]
@@ -60,22 +67,14 @@
 
 
 class ConfigSetting(typing.Generic[T]):
     """
     An individual setting that can be exposed through CLI and/or YAML
     """
 
-    data_type: T
-    description_lines: typing.List[str]
-    cli_args: typing.List[str]
-    include_in_argparse: bool
-    include_in_yaml: bool
-    show_default_in_yaml: bool
-    fn_on_set: typing.Callable[[T], None]
-
     def __init__(
         self,
         name: str,
         default: T,
         description_lines: typing.List[str],
         cli_args: typing.Optional[typing.List[str]] = None,
         place_default_in_yaml: bool = False,
@@ -182,32 +181,36 @@
         # note: keeping the type checker happy across python versions
         # here is actually kinda hard.  It's worried about what the
         # values in the combined dict might be.  But really it's fine,
         # so just tell it to chill.
         self.set_value(value)  # type: ignore
 
     def set_value(self, value: T) -> None:
+        if isinstance(self.default, bool) and isinstance(value, str):
+            if value.lower() in ["true", "yes", "1"]:
+                value = True  # type: ignore
+            elif value.lower() in ["false", "no", "0"]:
+                value = False  # type: ignore
+            else:
+                value = bool(value)  # type: ignore
+
         self.value = value
         self.fn_on_set(value)
 
     def get(self) -> T:
         if isinstance(self.value, dict):
             return self.value.copy()
         return self.value
 
 
 class ConfigSettingGroup:
     """
     A group of related settings that can be exposed through CLI and/or YAML
     """
 
-    name: str
-    description: str
-    settings: typing.Dict[str, ConfigSetting]
-
     def __init__(
         self,
         name: str,
         description: str = "",
         include_in_argparse: bool = True,
         include_in_yaml: bool = True,
     ):
@@ -355,32 +358,35 @@
 def load_from_dict(
     setting_groups: typing.List["ConfigSettingGroup"],
     settings_dict: dict,
 ) -> None:
     """
     Load settings from a dictionary
     """
-    print(f"settings_dict: {settings_dict}")
     for group in setting_groups:
         group.set_values_from_dict(settings_dict)
 
 
 def load(
     cli_args: typing.List[str],
     setting_groups: typing.List["ConfigSettingGroup"],
     config_file: str,
+    raise_if_file_missing: bool,
 ) -> argparse.ArgumentParser:
     """
     Load settings from defaults, config.yml, and command line arguments
     in that order.  Later sources will overwrite earlier ones.
 
     Returns the argparse parser, which can be used to print out the help
     message.
     """
-    load_from_yaml(config_file, setting_groups)
+    load_error_message = load_from_yaml(config_file, setting_groups)
+    if load_error_message and raise_if_file_missing:
+        raise ConfigFileMissingError(load_error_message)
+
     namespace = load_from_cli(cli_args, setting_groups)
 
     # returning this since it can print out the help message
     return namespace
 
 
 START_COMMENT = textwrap.dedent(
```

### Comparing `oobabot-0.1.9/src/oobabot/persona.py` & `oobabot-0.2.0/src/oobabot/persona.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,41 +13,26 @@
 
 
 class Persona:
     """
     Handles retrieving persona data from a variety of formats
     """
 
-    ai_name: str
-    """
-    The name of the AI.
-    """
-
-    persona: str
-    """
-    The persona of the AI.
-    """
-
-    wakewords: typing.List[str]
-    """
-    If we see one of these words in a message, we'll respond to it.
-    """
-
     # list of keys that, depending on the json/yaml schema, might
     # contain the AI's name.  Take the first one found, in order.
     NAME_KEYS = ["char_name", "name"]
 
     # list of keys that, depending on the json/yaml schema, might
     # contain the AI's persona.  Take the first one found, in order.
     PERSONA_KEYS = ["char_persona", "description", "context", "personality"]
 
     def __init__(self, persona_settings: dict) -> None:
-        self.ai_name = persona_settings["ai_name"]
-        self.persona = persona_settings["persona"]
-        self.wakewords = persona_settings["wakewords"].copy()
+        self.ai_name: str = persona_settings["ai_name"]
+        self.persona: str = persona_settings["persona"]
+        self.wakewords: typing.List[str] = persona_settings["wakewords"].copy()
 
         # if a json file is specified, load it and have
         # that overwrite everything else
         if "persona_file" in persona_settings:
             filename = persona_settings["persona_file"]
             try:
                 self.load_from_file(filename)
```

### Comparing `oobabot-0.1.9/src/oobabot/prompt_generator.py` & `oobabot-0.2.0/src/oobabot/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.9/src/oobabot/repetition_tracker.py` & `oobabot-0.2.0/src/oobabot/repetition_tracker.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.9/src/oobabot/response_stats.py` & `oobabot-0.2.0/src/oobabot/response_stats.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.9/src/oobabot/sd_client.py` & `oobabot-0.2.0/src/oobabot/sd_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,24 +38,38 @@
         #   and also a few privacy-related fields.
         "progress": STABLE_DIFFUSION_API_URI_PATH + "progress",
         # progress: GET only
         #   returns the progress of the current image generation
         "txt2img": STABLE_DIFFUSION_API_URI_PATH + "txt2img",
         # txt2img: POST only
         #   takes a prompt, generates an image and returns it
+        "sd-models": STABLE_DIFFUSION_API_URI_PATH + "sd-models",
+        # sd-models: GET only
+        # [
+        #   {
+        #     "title": "Anything-V3.0.ckpt [812cd9f9d9]",
+        #     "model_name": "Anything-V3.0",
+        #     "hash": "812cd9f9d9",
+        #     "sha256": "812cd9f9d9a0cb62aaad605173fd64dea1....",
+        #     "filename": "...long..path.../models/Stable-diffusion/Anything-V3.0.ckpt",
+        #     "config": null
+        #   },
+        # ...
+        # ]
     }
 
     def __init__(
         self,
         settings: typing.Dict[str, typing.Any],
     ):
         super().__init__(self.SERVICE_NAME, settings["stable_diffusion_url"])
 
         self.extra_prompt_text = settings["extra_prompt_text"]
         self.request_params = settings["request_params"]
+        self.sd_models = []
 
         # when we're in a "age restricted" channel, we'll swap
         # the "negative_prompt" in the request_params with this
         # value.  Otherwise we'll use the one already in
         # request_params["negative_prompt"]
         self.negative_prompt_nsfw = self.request_params.pop("negative_prompt_nsfw", "")
 
@@ -126,22 +140,30 @@
             return
 
         async with self._get_session().post(url, json=options_to_set) as response:
             if response.status != 200:
                 raise http_client.OobaHttpClientError(response)
             await response.json()
 
-    async def get_samplers(self) -> typing.List[str]:
-        url = self.API_COMMAND_URLS["get_samplers"]
+    async def _call_and_extract_field(
+        self, command: str, field: str
+    ) -> typing.List[str]:
+        url = self.API_COMMAND_URLS[command]
         async with self._get_session().get(url) as response:
             if response.status != 200:
                 raise http_client.OobaHttpClientError(response)
             response = await response.json()
-            samplers = [str(sampler["name"]) for sampler in response]
-            return samplers
+            values = [str(value[field]) for value in response]
+            return values
+
+    async def get_samplers(self) -> typing.List[str]:
+        return await self._call_and_extract_field("get_samplers", "name")
+
+    async def get_models(self) -> typing.List[str]:
+        return await self._call_and_extract_field("sd-models", "model_name")
 
     def generate_image(
         self,
         prompt: str,
         is_channel_nsfw: bool = False,
     ) -> "asyncio.Task[bytes]":
         """
@@ -156,14 +178,30 @@
             OobaHttpClientError, if the request fails.
         """
         request = self.request_params.copy()
         request["prompt"] = prompt
         if is_channel_nsfw:
             request["negative_prompt"] = self.negative_prompt_nsfw
 
+        # try to extract a model name from the prompt.  If we do,
+        # set it via ['override_settings']['sd_model_checkpoint']
+        lower_prompt = prompt.lower()
+        for model in self.sd_models:
+            if model.lower() in lower_prompt:
+                if "override_settings" not in request:
+                    request["override_settings"] = {}
+                request["override_settings"]["sd_model_checkpoint"] = model
+
+                fancy_logger.get().debug(
+                    "Stable Diffusion:  setting model to '%s'", model
+                )
+                # remove the model name from the prompt itself
+                request["prompt"] = request["prompt"].replace(model, "")
+                break
+
         if self.extra_prompt_text:
             request["prompt"] += ", " + self.extra_prompt_text
 
         async def do_post() -> bytes:
             fancy_logger.get().debug(
                 "Stable Diffusion: Image request (nsfw: %r): %s",
                 is_channel_nsfw,
@@ -242,14 +280,18 @@
             "Stable Diffusion: Available samplers: %s", ", ".join(samplers)
         )
         self.request_params["sampler"] = ""
 
     async def _setup(self):
         await self.verify_sampler_available()
         await self.set_options()
+        self.sd_models = await self.get_models()
+        fancy_logger.get().info(
+            "Stable Diffusion: Available models: %s", ", ".join(self.sd_models)
+        )
         fancy_logger.get().debug(
             "Stable Diffusion: Using negative prompt: %s...",
             str(self.request_params.get("negative_prompt", ""))[:20],
         )
         if self.extra_prompt_text:
             fancy_logger.get().debug(
                 "Stable Diffusion: will append to every prompt: '%s'",
```

### Comparing `oobabot-0.1.9/src/oobabot/settings.py` & `oobabot-0.2.0/src/oobabot/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,24 @@
 import textwrap
 import typing
 
 from oobabot import templates
 import oobabot.overengineered_settings_parser as oesp
 
 
+class SettingsError(Exception):
+    """
+    Base class for exceptions in this module.
+    """
+
+    def __init__(self, message: str, cause: Exception):
+        self.message = message
+        super().__init__(message, cause)
+
+
 def _console_wrapped(message):
     width = shutil.get_terminal_size().columns
     return "\n".join(textwrap.wrap(message, width))
 
 
 def _make_template_comment(
     tokens_desc_tuple: typing.Tuple[typing.List[templates.TemplateToken], str, bool],
@@ -60,14 +70,18 @@
     environment variables and command line arguments.
     """
 
     ############################################################
     # This section is for constants which are not yet
     # customizable by the user.
 
+    # when trying to stop the bot, wait this long before
+    # giving up and just exiting
+    STOP_LOCK_TIMEOUT: float = 5.0
+
     # This is a table of the probability that the bot will respond
     # in an unsolicited manner (i.e. it isn't specifically pinged)
     # to a message, based on how long ago it was pinged in that
     # same channel.
     TIME_VS_RESPONSE_CHANCE: typing.List[typing.Tuple[float, float]] = [
         # (seconds, base % chance of an unsolicited response)
         (60.0, 0.90),
@@ -85,25 +99,32 @@
 
     OOBABOOGA_DEFAULT_REQUEST_PARAMS: oesp.SettingDictType = {
         "max_new_tokens": 250,
         "do_sample": True,
         "temperature": 1.3,
         "top_p": 0.1,
         "typical_p": 1,
+        "epsilon_cutoff": 0,  # In units of 1e-4
+        "eta_cutoff": 0,  # In units of 1e-4
+        "tfs": 1,
+        "top_a": 0,
         "repetition_penalty": 1.18,
         "top_k": 40,
         "min_length": 0,
         "no_repeat_ngram_size": 0,
         "num_beams": 1,
         "penalty_alpha": 0,
         "length_penalty": 1,
         "early_stopping": False,
+        "mirostat_mode": 0,
+        "mirostat_tau": 5,
+        "mirostat_eta": 0.1,
         "seed": -1,
         "add_bos_token": True,
-        "truncation_length": 730,
+        "truncation_length": 2048,
         "ban_eos_token": False,
         "skip_special_tokens": True,
         "stopping_strings": [],
     }
 
     # set default negative prompts to make it more difficult
     # to create content against the discord TOS
@@ -415,14 +436,41 @@
                         Note: may be janky
                         """
                     )
                 ],
             )
         )
         self.discord_settings.add_setting(
+            oesp.ConfigSetting[float](
+                name="stream_responses_speed_limit",
+                default=0.7,
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        FEATURE PREVIEW: When streaming responses, cap the
+                        rate at which we send updates to Discord to be no
+                        more than once per this many seconds.
+
+                        This does not guarantee that updates will be sent
+                        this fast.  Only that they will not be sent any
+                        faster than this rate.
+
+                        This is useful because Discord has a rate limit on
+                        how often you can send messages, and if you exceed
+                        it, the updates will suddenly become slow.
+
+                        Example: 0.2 means we will send updates no faster
+                        than 5 times per second.
+                        """
+                    )
+                ],
+                include_in_argparse=False,
+            )
+        )
+        self.discord_settings.add_setting(
             oesp.ConfigSetting[int](
                 name="unsolicited_channel_cap",
                 default=3,
                 description_lines=[
                     textwrap.dedent(
                         """
                         FEATURE PREVIEW: Adds a limit to the number of channels
@@ -435,17 +483,48 @@
                         unsolicited message.  The bot will still respond to
                         @-mentions and wake words in any channel it can access.
 
                         Set to 0 to disable this feature.
                         """
                     )
                 ],
+                include_in_argparse=False,
+            )
+        )
+        self.discord_settings.add_setting(
+            oesp.ConfigSetting[str](
+                name="discrivener_location",
+                default="",
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        FEATURE PREVIEW: Path to the Discrivener executable.
+                        Will enable prototype voice integration.
+                        """
+                    )
+                ],
+                include_in_argparse=False,
             )
         )
 
+        self.discord_settings.add_setting(
+            oesp.ConfigSetting[str](
+                name="discrivener_model_location",
+                default="",
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        FEATURE PREVIEW: Path to the Discrivener model to
+                        load.  Required if discrivener_location is set.
+                        """
+                    )
+                ],
+                include_in_argparse=False,
+            )
+        )
         ###########################################################
         # Oobabooga Settings
 
         self.oobabooga_settings = oesp.ConfigSettingGroup("Oobabooga")
         self.setting_groups.append(self.oobabooga_settings)
 
         self.oobabooga_settings.add_setting(
@@ -509,14 +588,30 @@
                     )
                 ],
                 include_in_argparse=False,
                 show_default_in_yaml=False,
                 place_default_in_yaml=True,
             )
         )
+        self.oobabooga_settings.add_setting(
+            oesp.ConfigSetting[bool](
+                name="plugin_auto_start",
+                default=False,
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        When running inside the Oobabooga plugin, automatically
+                        connect to Discord when Oobabooga starts.  This has no effect
+                        when running from the command line.
+                        """
+                    )
+                ],
+                include_in_argparse=False,
+            )
+        )
 
         ###########################################################
         # Stable Diffusion Settings
 
         self.stable_diffusion_settings = oesp.ConfigSettingGroup("Stable Diffusion")
         self.setting_groups.append(self.stable_diffusion_settings)
 
@@ -593,14 +688,15 @@
                         keywords that Oobabooga produces to Stable Diffusion to finally
                         generate an image.
                         Otherwise, the bot will simply extract keywords directly
                         from the user's message using a simple regex.
                         """
                     )
                 ],
+                include_in_argparse=False,
             )
         )
 
         ###########################################################
         # Template Settings
 
         self.template_settings = oesp.ConfigSettingGroup(
@@ -638,32 +734,35 @@
 
     def write_to_stream(self, out_stream) -> None:
         oesp.write_to_stream(self.setting_groups, out_stream)
 
     def write_to_file(self, filename: str) -> None:
         oesp.write_to_file(self.setting_groups, filename)
 
-    def _filename_from_args(self, args: typing.List[str]) -> str:
+    def _filename_from_args(self, args: typing.List[str]) -> typing.Tuple[str, bool]:
         """
         Get the configuration filename from the command line arguments.
         If none is supplied, return the default.
+
+        Returns a tuple with the file to open, and True if it came
+        from the default, rather than a CLI argument.
         """
 
         # we need to hack this in here because we want to know the filename
         # before we parse the args, so that we can load the config file
         # first and then have the arguments overwrite the config file.
         config_setting = self.general_settings.get_setting("config")
         if args is not None:
             for config_flag in config_setting.cli_args:
                 # find the element after config_flag in args
                 try:
-                    return args[args.index(config_flag) + 1]
+                    return (args[args.index(config_flag) + 1], False)
                 except (ValueError, IndexError):
                     continue
-        return config_setting.default
+        return (config_setting.default, True)
 
     def load_from_yaml_stream(self, stream: typing.TextIO) -> typing.Optional[str]:
         """
         Load the config from a YAML stream.
 
         params:
             stream: stream to load the config from
@@ -674,35 +773,49 @@
         """
         return oesp.load_from_yaml_stream(stream, setting_groups=self.setting_groups)
 
     def load(
         self,
         cli_args: typing.List[str],
         config_file: typing.Optional[str] = None,
+        running_from_cli: bool = False,
     ) -> None:
         """
         Load the config from the command line arguments and config file.
 
         params:
             cli_args: list of command line arguments to parse
             config_file: path to the config file to load
 
         cli_args is intended to be used when running from a standalone
         application, while config_file is intended to be used when
         running from inside another process.
+
+        raises SettingsError if a specific configuration file
+        was requested (either by the config_file argument or the CLI),
+        but it could not be found.
         """
 
+        is_default = False
         if config_file is None:
-            config_file = self._filename_from_args(cli_args)
+            config_file, is_default = self._filename_from_args(cli_args)
+        raise_if_file_missing = not is_default and running_from_cli
 
-        self.arg_parser = oesp.load(
-            cli_args=cli_args,
-            setting_groups=self.setting_groups,
-            config_file=config_file,
-        )
+        try:
+            self.arg_parser = oesp.load(
+                cli_args=cli_args,
+                setting_groups=self.setting_groups,
+                config_file=config_file,
+                raise_if_file_missing=raise_if_file_missing,
+            )
+        except oesp.ConfigFileMissingError as err:
+            # get full path to config_file
+            config_file = os.path.abspath(config_file)
+            msg = f"Could not load config file at: {config_file}"
+            raise SettingsError(msg, err) from err
 
     def print_help(self):
         """
         Prints CLI usage information to STDOUT.
         """
         if self.arg_parser is None:
             raise ValueError("display_help called before load")
```

### Comparing `oobabot-0.1.9/src/oobabot/templates.py` & `oobabot-0.2.0/src/oobabot/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         Templates.COMMAND_LOBOTOMIZE_RESPONSE: (
             [
                 TemplateToken.AI_NAME,
                 TemplateToken.USER_NAME,
             ],
             "Displayed in Discord after a successful /lobotomize command.  "
             + "Both the discord users and the bot AI will see this message.",
-            False,
+            True,
         ),
         Templates.PROMPT: (
             [
                 TemplateToken.AI_NAME,
                 TemplateToken.IMAGE_COMING,
                 TemplateToken.MESSAGE_HISTORY,
                 TemplateToken.PERSONA,
```

### Comparing `oobabot-0.1.9/PKG-INFO` & `oobabot-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -59,15 +59,15 @@
 Real motivation: I wanted a chatbot in my discord that would act like my cat.  A "catbot" if you will.
 
 ## Features
 
 | **`oobabot`**  | how that's awesome |
 |---------------|------------------|
 | **user-supplied persona** | you supply the persona on how would like the bot to behave |
-| **multiple converations** | can track multiple conversational threads, and reply to each in a contextually appropriate way |
+| **multiple conversations** | can track multiple conversational threads, and reply to each in a contextually appropriate way |
 | **watchwords** | can monitor all channels in a server for one or more wakewords or @-mentions |
 | **private conversations** | can chat with you 1:1 in a DM |
 | **good Discord hygiene** | splits messages into independent sentences, pings the author in the first one |
 | **low-latency** | streams the reply live, sentence by sentence.  Provides lower latency, especially on longer responses. |
 | **stats** | track token generation speed, latency, failures and usage |
 | **easy networking** | connects to discord from your machine using websockets, so no need to expose a server to the internet |
 | ✨**Stable Diffusion** | new in v0.1.4!  Optional image generation with AUTOMATIC1111 |
@@ -90,25 +90,24 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-  ³ oobabot  ~/oobabot        oobabot --help         383ms  Tue May 23 18:56:42 2023
 usage: oobabot [-h] [-c CONFIG] [--generate-config] [--invite-url] [--ai-name AI_NAME]
                [--persona PERSONA] [--wakewords [WAKEWORDS ...]]
                [--discord-token DISCORD_TOKEN] [--dont-split-responses]
                [--history-lines HISTORY_LINES] [--ignore-dms] [--reply-in-thread]
                [--stream-responses] [--base-url BASE_URL] [--log-all-the-things]
                [--message-regex MESSAGE_REGEX] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
-               [--extra-prompt-text EXTRA_PROMPT_TEXT] [--use-ai-generated-keywords]
+               [--extra-prompt-text EXTRA_PROMPT_TEXT]
 
-oobabot v0.1.8: Discord bot for oobabooga's text-generation-webui
+oobabot v0.2.0: Discord bot for oobabooga's text-generation-webui
 
 General Settings:
 
   -h, --help
   -c CONFIG, --config CONFIG
                         Path to a config file to read settings from. Command line settings
                         will override settings in this file. (default: config.yml)
@@ -133,15 +132,15 @@
                         if no wakewords are supplied. (default: ['oobabot'])
 
 Discord:
 
   --discord-token DISCORD_TOKEN
                         Token to log into Discord with. For security purposes it's strongly
                         recommended that you set this via the DISCORD_TOKEN environment
-                        variable instead, if possible. (default: )
+                        variable instead, if possible. (default: None)
   --dont-split-responses
                         Post the entire response as a single message, rather than splitting
                         it into separate messages by sentence. (default: False)
   --history-lines HISTORY_LINES
                         Number of lines of chat history the AI will see when generating a
                         response. (default: 7)
   --ignore-dms          If set, the bot will not respond to direct messages. (default:
@@ -171,27 +170,18 @@
                         an image. (default: ['draw me', 'drawing', 'photo', 'pic',
                         'picture', 'image', 'sketch'])
   --stable-diffusion-url STABLE_DIFFUSION_URL
                         URL for an AUTOMATIC1111 Stable Diffusion server. (default: )
   --extra-prompt-text EXTRA_PROMPT_TEXT
                         This will be appended to every image generation prompt sent to
                         Stable Diffusion. (default: )
-  --use-ai-generated-keywords
-                        FEATURE PREVIEW: If set, the bot will ask Oobabooga to generate
-                        image keywords from a user's message. It will then pass the
-                        keywords that Oobabooga produces to Stable Diffusion to finally
-                        generate an image. Otherwise, the bot will simply extract keywords
-                        directly from the user's message using a simple regex. (default:
-                        False)
 
 
 Additional settings can be set in config.yml.  Use the --generate-config option to print a
 new copy of this file to STDOUT.
-
-Please set the 'DISCORD_TOKEN' environment variable to your bot's discord token.
 ```
 
 There are **a lot more settings** in the [config.yml file (sample)](./docs/config.sample.yml) here.
 
 ## Required settings
 
 - **`DISCORD_TOKEN`** environment variable
@@ -207,15 +197,15 @@
     **fish example**
 
     ``` fish
     set -Ux DISCORD_TOKEN ___YOUR_TOKEN___
     ```
 
     In certain environments, it may be difficult to set an environment variable.  In that case, you can also pass the token in as a command-line argument using `--discord-token`.  But doing so might leak the token to other
-    users on a shared sysem, as it will be visible to anyone who can run `ps`.
+    users on a shared system, as it will be visible to anyone who can run `ps`.
 
 - **`--base-url`**
 
     The base URL of oobabooga's streaming web API.  This is
     required if the oobabooga machine is different than where you're running **`oobabot`**.
 
     By default, this will be port 5005 (even though the HTML UI runs on a different port).  The protocol should typically be ws://.
```

