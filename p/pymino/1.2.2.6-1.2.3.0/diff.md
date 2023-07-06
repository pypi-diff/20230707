# Comparing `tmp/pymino-1.2.2.6.tar.gz` & `tmp/pymino-1.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymino-1.2.2.6.tar", last modified: Sun Jul  2 23:12:28 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\gss\pymino\dist\.tmp-_2x2yroa\pymino-1.2.3.0.tar", last modified: Thu Jul  6 03:46:26 2023, max compression
```

## Comparing `pymino-1.2.2.6.tar` & `pymino-1.2.3.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.399698 pymino-1.2.2.6/
--rw-rw-rw-   0        0        0     1085 2023-06-27 02:23:25.000000 pymino-1.2.2.6/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-07-02 23:12:28.399698 pymino-1.2.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-07-02 23:10:10.000000 pymino-1.2.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.019991 pymino-1.2.2.6/pymino/
--rw-rw-rw-   0        0        0      721 2023-07-02 22:29:02.000000 pymino-1.2.2.6/pymino/__init__.py
--rw-rw-rw-   0        0        0    11727 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30988 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/bot.py
--rw-rw-rw-   0        0        0    36824 2023-06-28 06:25:49.000000 pymino-1.2.2.6/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.188642 pymino-1.2.2.6/pymino/ext/
--rw-rw-rw-   0        0        0      528 2023-06-27 04:04:07.000000 pymino-1.2.2.6/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-17 07:35:45.000000 pymino-1.2.2.6/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    11196 2023-06-28 06:25:45.000000 pymino-1.2.2.6/pymino/ext/account.py
--rw-rw-rw-   0        0        0   345265 2023-07-02 22:55:58.000000 pymino-1.2.2.6/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21408 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25886 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   344166 2023-07-02 22:55:07.000000 pymino-1.2.2.6/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45526 2023-07-02 22:27:53.000000 pymino-1.2.2.6/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1856 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.316653 pymino-1.2.2.6/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15825 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    70299 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6657 2023-06-27 07:21:56.000000 pymino-1.2.2.6/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.398700 pymino-1.2.2.6/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11357 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10322 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.035118 pymino-1.2.2.6/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1555 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-07-02 23:12:28.401692 pymino-1.2.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-06-27 04:33:02.000000 pymino-1.2.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:26.720507 pymino-1.2.3.0/
+-rw-rw-rw-   0        0        0     1085 2023-07-05 01:41:18.000000 pymino-1.2.3.0/LICENSE
+-rw-rw-rw-   0        0        0     7426 2023-07-06 03:46:26.721500 pymino-1.2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6708 2023-07-06 03:46:03.000000 pymino-1.2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:26.617340 pymino-1.2.3.0/pymino/
+-rw-rw-rw-   0        0        0      775 2023-07-06 03:37:57.000000 pymino-1.2.3.0/pymino/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-07-06 03:43:42.000000 pymino-1.2.3.0/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    37317 2023-07-06 02:21:48.000000 pymino-1.2.3.0/pymino/async_client.py
+-rw-rw-rw-   0        0        0    31005 2023-07-06 01:18:58.000000 pymino-1.2.3.0/pymino/bot.py
+-rw-rw-rw-   0        0        0    36840 2023-07-06 01:19:00.000000 pymino-1.2.3.0/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:26.674379 pymino-1.2.3.0/pymino/ext/
+-rw-rw-rw-   0        0        0      651 2023-07-05 02:49:00.000000 pymino-1.2.3.0/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    11196 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/account.py
+-rw-rw-rw-   0        0        0    11496 2023-07-06 02:20:56.000000 pymino-1.2.3.0/pymino/ext/async_account.py
+-rw-rw-rw-   0        0        0   345249 2023-07-06 02:59:58.000000 pymino-1.2.3.0/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21402 2023-07-05 01:57:26.000000 pymino-1.2.3.0/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25878 2023-07-06 01:26:00.000000 pymino-1.2.3.0/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0    67975 2023-07-06 02:49:53.000000 pymino-1.2.3.0/pymino/ext/async_global_client.py
+-rw-rw-rw-   0        0        0     7233 2023-07-05 01:53:43.000000 pymino-1.2.3.0/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344155 2023-07-06 01:26:00.000000 pymino-1.2.3.0/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    45520 2023-07-05 01:57:13.000000 pymino-1.2.3.0/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1856 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:26.702652 pymino-1.2.3.0/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-07-06 02:42:55.000000 pymino-1.2.3.0/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    70299 2023-07-05 02:42:02.000000 pymino-1.2.3.0/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6657 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:26.719516 pymino-1.2.3.0/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11544 2023-07-06 02:13:14.000000 pymino-1.2.3.0/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-07-05 01:41:18.000000 pymino-1.2.3.0/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10404 2023-07-06 02:03:53.000000 pymino-1.2.3.0/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:26.639660 pymino-1.2.3.0/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7426 2023-07-06 03:46:26.000000 pymino-1.2.3.0/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1640 2023-07-06 03:46:26.000000 pymino-1.2.3.0/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:46:26.000000 pymino-1.2.3.0/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-06 03:46:26.000000 pymino-1.2.3.0/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 03:46:26.000000 pymino-1.2.3.0/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-07-06 03:46:26.723483 pymino-1.2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-07-05 01:41:18.000000 pymino-1.2.3.0/setup.py
```

### Comparing `pymino-1.2.2.6/LICENSE` & `pymino-1.2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/PKG-INFO` & `pymino-1.2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.2.6
+Version: 1.2.3.0
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
   <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
-    <h3 style="color: red;"><strong>WARNING</strong></h3>
+    <h3 style="color: red;"><strong> WARNING </strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
   <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.2.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.0 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.2.6/README.md` & `pymino-1.2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
   <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
-    <h3 style="color: red;"><strong>WARNING</strong></h3>
+    <h3 style="color: red;"><strong> WARNING </strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
   <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
```

### Comparing `pymino-1.2.2.6/pymino/async_bot.py` & `pymino-1.2.3.0/pymino/async_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         self.request.userId: str = self.userId
         self.is_authenticated: bool = True
 
         if hasattr(self.request, "email") and self._cached:
             cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
 
         if not self.is_ready:
-            self.is_ready = True
+            self._is_ready = True
             await self.run_forever()
 
 
     async def fetch_account(self) -> dict:
         self.profile: UserProfile = UserProfile(
             await self.request.handler(
                 method="GET",
@@ -303,15 +303,15 @@
                 "longitude": 0,
                 "mediaList": None,
                 "eventSource": "UserProfileView",
                 "timestamp": int(time() * 1000),
         }
 
         if nickname: data['nickname'] = nickname
-        if icon: data['icon'] = self.upload_image(icon)
+        if icon: data['icon'] = self.upload_image(icon) # Human is gay.
         if content: data['content'] = content
         if backgroundColor:
             data["extensions"] = {
                 "style": {
                     "backgroundColor": backgroundColor
                     if backgroundColor.startswith("#")
                     else f"#{backgroundColor}"
```

### Comparing `pymino-1.2.2.6/pymino/bot.py` & `pymino-1.2.3.0/pymino/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
         **Note:** This property only returns the user ID and cannot be used to set the user ID. To set the user ID, use the
         `self._userId` attribute directly.
         """
         return self._userId
 
 
     @userId.setter
-    def userId(self, value: str) -> None:
+    def userId(self, value: str) -> None: # Human is gay.
         """
         Sets the ID of the user associated with the client.
 
         :param value: The ID of the user to set.
         :type value: str
         :return: None
 
@@ -664,15 +664,15 @@
         self.request.userId: str = self.userId
         self.is_authenticated: bool = True
 
         if hasattr(self.request, "email") and self._cached:
             cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
 
         if not self.is_ready:
-            self.is_ready = True
+            self._is_ready = True
             self.connect()
 
         if self.debug:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
 
         Thread(target=self.__run_console__).start()
         return response
```

### Comparing `pymino-1.2.2.6/pymino/client.py` & `pymino-1.2.3.0/pymino/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
         >>> client = Client()
         >>> response = client.authenticate(email="example@example.com", password="password")
         >>> client._run(response)
         """
         if response["api:statuscode"] != 0: input(response), exit()
 
         if not hasattr(self, "profile"): 
-            self.profile: UserProfile = UserProfile(response)
+            self.profile: UserProfile = UserProfile(response) # Human is gay.
 
         if not self.sid:
             self.sid: str = response["sid"]
 
         self.userId: str = self.profile.userId
         self.community.userId: str = self.userId
         self.request.sid: str = self.sid
```

### Comparing `pymino-1.2.2.6/pymino/ext/__init__.py` & `pymino-1.2.3.0/pymino/ext/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,9 +10,12 @@
 from .account import *
 from .context import *
 from .global_client import *
 from .community import *
 from .async_community import *
 from .dispatcher import *
 from .handle_queue import *
+from .async_account import *
 from .async_event_handler import *
-from .utilities.request_handler import *
+from .async_community import AsyncCommunity
+from .utilities.request_handler import *
+from .utilities.async_request_handler import *
```

### Comparing `pymino-1.2.2.6/pymino/ext/account.py` & `pymino-1.2.3.0/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/async_community.py` & `pymino-1.2.3.0/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
         """
         async def community_func(*args, **kwargs) -> Any:
             if not args[0].userId:
                 raise NotLoggedIn("You are not logged in. Please login before using this function.")
             if not any([args[0].community_id, kwargs.get("comId")]):
                 raise MissingCommunityId()
             return await func(*args, **kwargs)
+
         community_func.__annotations__ = func.__annotations__
         return community_func
 
 
     @community
     async def invite_code(self, comId: Union[str, int] = None) -> CommunityInvitation:
         """
@@ -248,15 +249,15 @@
                 "objectType": objectType.value if isinstance(objectType, ObjectTypes) else objectType,
                 "timestamp": int(time() * 1000)
                 }
             )
         return LinkInfo(response)
     
 
-    def fetch_object_id(self, link: str) -> str:
+    async def fetch_object_id(self, link: str) -> str:
         """
         Fetches the object ID given a link to the object.
 
         :param link: The link to the object.
         :type link: str
         :raises NotLoggedIn: If the user is not logged in.
         :raises MissingCommunityId: If the community ID is missing.
@@ -270,15 +271,15 @@
 
         >>> object_id = client.community.fetch_object_id(link="https://aminoapps.com/p/w2Fs6H")
         >>> print(object_id)
         """
 
         KEY = str((link, "OBJECT_ID"))
         if not self.cache.get(KEY):
-            response = self.session.handler(
+            response = await self.session.handler(
                 method="GET",
                 url=f"/g/s/link-resolution?q={link}"
             )
             self.cache.set(KEY, response)
 
         return LinkInfo(self.cache.get(KEY)).objectId
 
@@ -3910,26 +3911,26 @@
             print("background_image is deprecated, please use backgroundImage instead.")
 
         data: dict = {"timestamp": int(time() * 1000), "extensions": {}}
 
         [data.update({key: value}) for key, value in {
             "nickname": nickname,
             "content": content,
-            "icon": self.__handle_media__(media=icon, media_value=True) if icon is not None else None,
-            "mediaList": [[100, self.__handle_media__(media=cover_image, media_value=True), None, None, None, None]] if cover_image is not None else None
+            "icon": await self.__handle_media__(media=icon, media_value=True) if icon is not None else None,
+            "mediaList": [[100, await self.__handle_media__(media=cover_image, media_value=True), None, None, None, None]] if cover_image is not None else None
             }.items() if value is not None]
 
         if backgroundColor:
             data["extensions"]["style"] = {"backgroundColor": backgroundColor}
 
         if backgroundImage:
-            data["extensions"]["style"] = {"backgroundMediaList": [[100, self.__handle_media__(media=backgroundImage, media_value=True), None, None, None, None]]}
+            data["extensions"]["style"] = {"backgroundMediaList": [[100, await self.__handle_media__(media=backgroundImage, media_value=True), None, None, None, None]]}
 
         return UserProfile(
-            self.session.handler(
+            await self.session.handler(
                 method="POST",
                 url=f"/x{self.community_id if comId is None else comId}/s/user-profile/{self.userId}",
                 data=data
                 ))
 
     @community
     async def fetch_user_blogs(self, userId: str, start: int = 0, size: int = 5, comId: Union[str, int] = None) -> CBlogList:
@@ -4118,16 +4119,16 @@
             method="POST",
             url=f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/message",
             data = PrepareMessage(content=message,
             extensions = {
             "linkSnippetList": [{
                 "link": link,
                 "mediaType": 100,
-                "mediaUploadValue": self.encode_media(
-                    self.__handle_media__(
+                "mediaUploadValue": await self.encode_media(
+                    await self.__handle_media__(
                         media=image,
                         content_type="image/jpg",
                         media_value=False
                     )
                 ),
                 "mediaUploadValueContentType": "image/png",
                 "mentionedArray": [
@@ -4152,15 +4153,15 @@
     async def send_image(self, chatId: str, image: BinaryIO = None, comId: Union[str, int] = None) -> CMessage:
         return CMessage(
             await self.session.handler(
             method="POST",
             url=f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/message",
             data = PrepareMessage(
                 mediaType = 100,
-                mediaUploadValue=self.encode_media(self.__handle_media__(media=image, content_type="image/jpg", media_value=False)),
+                mediaUploadValue= await self.encode_media(self.__handle_media__(media=image, content_type="image/jpg", media_value=False)),
                 mediaUploadValueContentType = "image/jpg",
                 mediaUhqEnabled = True
                 ).json()
             ))
 
 
     @community
@@ -4192,15 +4193,15 @@
         return CMessage(
             await self.session.handler(
             method="POST",
             url=f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/message",
             data = PrepareMessage(
                 type=2,
                 mediaType=110,
-                mediaUploadValue=self.encode_media(self.__handle_media__(media=audio, content_type="audio/aac", media_value=False)
+                mediaUploadValue=await self.encode_media(self.__handle_media__(media=audio, content_type="audio/aac", media_value=False)
                 )).json()
             ))
 
 
     @community
     async def send_sticker(self, chatId: str, stickerId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
@@ -5195,52 +5196,14 @@
                 } if reason is None else {
                     "adminOpNote": {"content": reason},
                     "adminOpName": 110,
                     "adminOpValue": 9,
                     "timestamp": int(time() * 1000)
                 }))
 
-    @community
-    async def enable_chat(self, chatId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
-        """
-        Enables a chat in the community.
-
-        :param chatId: The ID of the chat to enable.
-        :type chatId: str
-        :param reason: The reason for enabling the chat. (Optional)
-        :type reason: str, optional
-        :param comId: The ID of the community where the chat is located. If not provided, the current community ID is used.
-        :type comId: Union[str, int], optional
-        :return: An `ApiResponse` object representing the response from the API.
-        :rtype: ApiResponse
-
-        This function enables a chat in the specified community.
-
-        `ApiResponse` represents a response from the API.
-
-        **Example usage:**
-
-        >>> response = client.community.enable_chat("chat123")
-        ... print(response.status_code)
-        ... print(response.json())
-        """
-        return ApiResponse(await self.session.handler(
-            method = "POST",
-            url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/admin",
-            data = {
-            "adminOpName": 110,
-            "adminOpValue": 0,
-            "timestamp": int(time() * 1000)
-            } if reason is None else {
-            "adminOpNote": {"content": reason},
-            "adminOpName": 110,
-            "adminOpValue": 0,
-            "timestamp": int(time() * 1000)
-            }
-        ))
 
     @community
     async def disable_blog(self, blogId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
         """
         Disables a blog in the current or specified community.
 
         :param blogId: The ID of the blog to disable.
@@ -6034,15 +5997,15 @@
         ...     else:
         ...         print("Edit failed.")
         """
         data = dict(timestamp = int(time() * 1000))
 
         if title: data               .update(dict(title = title))
         if content: data             .update(dict(content = content))
-        if icon: data                .update(dict(icon = self.upload_media(open(icon, "rb").read()), content_type = "image/jpg"))
+        if icon: data                .update(dict(icon = await self.upload_media(open(icon, "rb").read()), content_type = "image/jpg"))
         if keywords: data            .update(dict(keywords = keywords))
         if announcement: data        .update(dict(extensions = dict(announcement = announcement)))
         if pinAnnouncement: data     .update(dict(extensions = dict(pinAnnouncement = pinAnnouncement)))
         if fansOnly: data            .update(dict(extensions = dict(fansOnly = fansOnly)))
         if publishToGlobal: data     .update(dict(publishToGlobal = 0))
         if not publishToGlobal: data .update(dict(publishToGlobal = 1))
 
@@ -7473,8 +7436,46 @@
         if pageToken: return AdminLogList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pageToken={pageToken}&pagingType=t"
         ))
         else: return AdminLogList(await self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pagingType=t"
+        ))
+
+    @community
+    async def apply_bubble(self, bubbleId: str, chatId: str = None, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Applies the specified bubble to the community.
+
+        :param bubbleId: The ID of the bubble to apply.
+        :type bubbleId: str
+        :param comId: The ID of the community to apply the bubble to. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The response of the request.
+        :rtype: response object
+
+        This function applies the specified bubble to the community.
+
+        Note: The response object may vary based on the implementation.
+
+        **Example usage:**
+
+        >>> client.community.apply_bubble("000000")
+        """
+        if bubbleId is None:
+            raise ValueError("bubbleId cannot be None.")
+        
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/chat/thread/apply-bubble",
+            data = {
+                "applyToAll": False,
+                "bubbleId": bubbleId,
+                "threadId": chatId,
+                "timestamp": int(time() * 1000)
+            } if chatId else {
+                "applyToAll": True,
+                "bubbleId": bubbleId,
+                "timestamp": int(time() * 1000)
+            }
         ))
```

### Comparing `pymino-1.2.2.6/pymino/ext/async_context.py` & `pymino-1.2.3.0/pymino/ext/async_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,24 +226,24 @@
         start = time()
 
         with self.bot.cache as cache:
             while time() - start < timeout:
                 cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
 
                 if cached_message == message:
-                    cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                    cache.pop(f"{self.message.chatId}_{self.message.author.userId}")
                     return 200
 
                 if all([cached_message is not None, cached_message != message]):
-                    cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                    cache.pop(f"{self.message.chatId}_{self.message.author.userId}")
                     return 404
 
                 await asyncio.sleep(0.1)
 
-            cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+            cache.pop(f"{self.message.chatId}_{self.message.author.userId}")
             return 500
 
 
     @_run
     @__typing__
     async def send(self, content: str, delete_after: int= None, mentioned: Union[str, List[str]]= None) -> CMessage:
         """
```

### Comparing `pymino-1.2.2.6/pymino/ext/async_event_handler.py` & `pymino-1.2.3.0/pymino/ext/async_event_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             potential_parameters.get(parameter)
             for parameter in inspect_signature(func).parameters
         )
 
 
     async def emit(self, name: str, *args) -> None:
         """`emit` is a function that emits an event."""
-        await self._events[name](*args) if name in self._events else None
+        self._events[name](*args) if name in self._events else None
 
 
     def command(
         self,
         name: str=None,
         description: str=None,
         usage: str=None,
@@ -259,15 +259,15 @@
 
         return 200
 
 
     def _add_cache(self, chatId: str, userId: str, content: str):
         with self.cache as cache:
             if cache.get(f"{chatId}_{userId}") is not None:
-                self.cache.clear(f"{chatId}_{userId}")
+                self.cache.pop(f"{chatId}_{userId}")
 
             cache.add(
                 key=f"{chatId}_{userId}",
                 value=content,
                 expire=90
                 )
```

### Comparing `pymino-1.2.2.6/pymino/ext/async_socket.py` & `pymino-1.2.3.0/pymino/ext/async_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         workers = [QueueHandler(self.message_queue, self.dispatcher) for _ in range(self.pool_size)]
         worker_tasks = [asyncio.create_task(worker.process_messages()) for worker in workers]
         await asyncio.gather(*worker_tasks)
 
 
     async def _ready(self) -> None:
         if "ready" in self._events:
-            await self._events["ready"]()
+            await self.emit("ready")
         else:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
 
 
     async def reconnect(self) -> None:
         self.reconnecting = True
         await asyncio.sleep(0)
```

### Comparing `pymino-1.2.2.6/pymino/ext/community.py` & `pymino-1.2.3.0/pymino/ext/community.py`

 * *Files 1% similar despite different names*

```diff
@@ -5128,52 +5128,14 @@
             } if reason is None else {
             "adminOpNote": {"content": reason},
             "adminOpName": 110,
             "adminOpValue": 9,
             "timestamp": int(time() * 1000)
             }))
 
-    @community
-    def enable_chat(self, chatId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
-        """
-        Enables a chat in the community.
-
-        :param chatId: The ID of the chat to enable.
-        :type chatId: str
-        :param reason: The reason for enabling the chat. (Optional)
-        :type reason: str, optional
-        :param comId: The ID of the community where the chat is located. If not provided, the current community ID is used.
-        :type comId: Union[str, int], optional
-        :return: An `ApiResponse` object representing the response from the API.
-        :rtype: ApiResponse
-
-        This function enables a chat in the specified community.
-
-        `ApiResponse` represents a response from the API.
-
-        **Example usage:**
-
-        >>> response = client.community.enable_chat("chat123")
-        ... print(response.status_code)
-        ... print(response.json())
-        """
-        return ApiResponse(self.session.handler(
-            method = "POST",
-            url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/admin",
-            data = {
-            "adminOpName": 110,
-            "adminOpValue": 0,
-            "timestamp": int(time() * 1000)
-            } if reason is None else {
-            "adminOpNote": {"content": reason},
-            "adminOpName": 110,
-            "adminOpValue": 0,
-            "timestamp": int(time() * 1000)
-            }
-        ))
 
     @community
     def disable_blog(self, blogId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
         """
         Disables a blog in the current or specified community.
 
         :param blogId: The ID of the blog to disable.
@@ -7403,8 +7365,48 @@
         if pageToken: return AdminLogList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pageToken={pageToken}&pagingType=t"
         ))
         else: return AdminLogList(self.session.handler(
             method = "GET",
             url = f"/x{comId or self.community_id}/s/admin/operation?size={size}&operatorUid={userId}&pagingType=t"
+        ))
+# {"timestamp": , "applyToAll": true, "bubbleId": "000000"} All
+#
+
+    @community
+    def apply_bubble(self, bubbleId: str, chatId: str = None, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Applies the specified bubble to the community.
+
+        :param bubbleId: The ID of the bubble to apply.
+        :type bubbleId: str
+        :param comId: The ID of the community to apply the bubble to. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The response of the request.
+        :rtype: response object
+
+        This function applies the specified bubble to the community.
+
+        Note: The response object may vary based on the implementation.
+
+        **Example usage:**
+
+        >>> client.community.apply_bubble("000000")
+        """
+        if bubbleId is None:
+            raise ValueError("bubbleId cannot be None.")
+        
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/chat/thread/apply-bubble",
+            data = {
+                "applyToAll": False,
+                "bubbleId": bubbleId,
+                "threadId": chatId,
+                "timestamp": int(time() * 1000)
+            } if chatId else {
+                "applyToAll": True,
+                "bubbleId": bubbleId,
+                "timestamp": int(time() * 1000)
+            }
         ))
```

### Comparing `pymino-1.2.2.6/pymino/ext/console.py` & `pymino-1.2.3.0/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/context.py` & `pymino-1.2.3.0/pymino/ext/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,22 +221,22 @@
         start = time()
 
         with self.bot.cache as cache:
             while time() - start < timeout:
                 cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
 
                 if cached_message == message:
-                    cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                    cache.pop(f"{self.message.chatId}_{self.message.author.userId}")
                     return 200
 
                 if all([cached_message is not None, cached_message != message]):
-                    cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                    cache.pop(f"{self.message.chatId}_{self.message.author.userId}")
                     return 404
 
-            cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+            cache.pop(f"{self.message.chatId}_{self.message.author.userId}")
             return 500
 
 
     @_run
     @__typing__
     def send(self, content: str, delete_after: int= None, mentioned: Union[str, List[str]]= None) -> CMessage:
         """
```

### Comparing `pymino-1.2.2.6/pymino/ext/dispatcher.py` & `pymino-1.2.3.0/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/acm.py` & `pymino-1.2.3.0/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/admin_log.py` & `pymino-1.2.3.0/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/api_response.py` & `pymino-1.2.3.0/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/bubble.py` & `pymino-1.2.3.0/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/chat_threads.py` & `pymino-1.2.3.0/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/comments.py` & `pymino-1.2.3.0/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/enums.py` & `pymino-1.2.3.0/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/exceptions.py` & `pymino-1.2.3.0/pymino/ext/entities/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,8 +498,14 @@
             "Intents are not enabled. Please enable them in your Bot instance and try again."
             )
 
 class InvalidCommandPrefix(Exception):
     def __init__(self):
         super().__init__(
             "Invalid command prefix. Please provide a valid command prefix."
+            )
+        
+class MissingAwaitError(Exception):
+    def __init__(self):
+        super().__init__(
+            "Missing await error. Please add `await` before your function call."
             )
```

### Comparing `pymino-1.2.2.6/pymino/ext/entities/general.py` & `pymino-1.2.3.0/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/handlers.py` & `pymino-1.2.3.0/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/link_info.py` & `pymino-1.2.3.0/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/member.py` & `pymino-1.2.3.0/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/messages.py` & `pymino-1.2.3.0/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/notification.py` & `pymino-1.2.3.0/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/sticker.py` & `pymino-1.2.3.0/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/threads.py` & `pymino-1.2.3.0/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/userprofile.py` & `pymino-1.2.3.0/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/entities/wsevents.py` & `pymino-1.2.3.0/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/global_client.py` & `pymino-1.2.3.0/pymino/ext/global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/handle_queue.py` & `pymino-1.2.3.0/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/socket.py` & `pymino-1.2.3.0/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.3.0/pymino/ext/utilities/async_request_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,33 +115,35 @@
             data: Union[dict, bytes, None],
             headers: dict,
             content_type: Optional[str]
     ) -> Union[int, str]:
         """
         `send_request` - Sends a request
 
-        `**Parameters**``
+        `**Parameters**`
         - `method` - The request method to use.
         - `url` - The url to send the request to.
         - `data` - The data to send with the request.
         - `headers` - The headers to send with the request.
         - `content_type` - The content type of the data.
 
-        `**Returns**``
+        `**Returns**`
         - `Union[int, str]` - The status code and response from the request.
 
         """
         if self.session is None:
             await self.initialize_session()
 
         try:
             async with self.session.request(
                 method, url, data=data, headers=headers, proxy=self.proxy
             ) as response:
-                return response.status, await response.text()
+                status_code = response.status
+                response_text = await response.text()
+            return status_code, response_text
         except (
             TypeError,
             ClientError,
             ClientConnectionError,
             ClientOSError,
             ClientConnectorError,
             ClientProxyConnectionError,
@@ -153,14 +155,17 @@
             ServerDisconnectedError,
             ServerFingerprintMismatch,
             ClientResponseError,
             ClientHttpProxyError,
             WSServerHandshakeError,
         ):
             return await self.handler(method, url, data, content_type)
+        
+        finally:
+            await self.close_session()
 
 
     async def handler(
             self,
             method: str,
             url: str,
             data: Union[dict, bytes, None] = None,
@@ -370,10 +375,11 @@
                     "DELETE": Fore.MAGENTA,
                     "LITE": Fore.YELLOW,
                 }.get(method, Fore.RED)
             )
             print(f"{color}{Style.BRIGHT}{method}{Style.RESET_ALL} - {url}")
 
 
-    async def close(self) -> None:
-        """Closes the HTTP session."""
-        await self.session.close()
+    async def close_session(self):
+        if self.session is not None:
+            await self.session.close()
+            self.session = None
```

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/chat_console.py` & `pymino-1.2.3.0/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/commands.py` & `pymino-1.2.3.0/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/community_console.py` & `pymino-1.2.3.0/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/generate.py` & `pymino-1.2.3.0/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/menu.py` & `pymino-1.2.3.0/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/profile_console.py` & `pymino-1.2.3.0/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.6/pymino/ext/utilities/request_handler.py` & `pymino-1.2.3.0/pymino/ext/utilities/request_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,17 @@
         - `None` - Raises an error if the status code is in the response map.
         
         """
         if all([
             response.get("api:statuscode", 200) == 105,
             hasattr(self, "email"),
             hasattr(self, "password")
-            ]): return self.bot.run(self.email, self.password, use_cache=False)
+            ]):
+            # NOTE: Login expired will have to run request manually
+            return self.bot.run(self.email, self.password, use_cache=False)
         
         else: raise APIException(response)
         
     def handle_response(self, status_code: int, response: str) -> dict:
         """
         `handle_response` - Handles the response and returns the response as a dict
```

### Comparing `pymino-1.2.2.6/pymino.egg-info/PKG-INFO` & `pymino-1.2.3.0/pymino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.2.6
+Version: 1.2.3.0
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
   <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
-    <h3 style="color: red;"><strong>WARNING</strong></h3>
+    <h3 style="color: red;"><strong> WARNING </strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
   <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.2.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.0 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.2.6/pymino.egg-info/SOURCES.txt` & `pymino-1.2.3.0/pymino.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 pymino/__init__.py
 pymino/async_bot.py
+pymino/async_client.py
 pymino/bot.py
 pymino/client.py
 pymino.egg-info/PKG-INFO
 pymino.egg-info/SOURCES.txt
 pymino.egg-info/dependency_links.txt
 pymino.egg-info/requires.txt
 pymino.egg-info/top_level.txt
 pymino/ext/__init__.py
 pymino/ext/_global.py
 pymino/ext/account.py
+pymino/ext/async_account.py
 pymino/ext/async_community.py
 pymino/ext/async_context.py
 pymino/ext/async_event_handler.py
+pymino/ext/async_global_client.py
 pymino/ext/async_socket.py
 pymino/ext/community.py
 pymino/ext/console.py
 pymino/ext/context.py
 pymino/ext/dispatcher.py
 pymino/ext/global_client.py
 pymino/ext/handle_queue.py
```

### Comparing `pymino-1.2.2.6/setup.cfg` & `pymino-1.2.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e32 2e36 0d0a 6175  on = 1.2.2.6..au
+00000020: 6f6e 203d 2031 2e32 2e33 2e30 0d0a 6175  on = 1.2.3.0..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.2.6/setup.py` & `pymino-1.2.3.0/setup.py`

 * *Files identical despite different names*

