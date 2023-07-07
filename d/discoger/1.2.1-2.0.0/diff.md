# Comparing `tmp/discoger-1.2.1.tar.gz` & `tmp/discoger-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.2.1.tar", last modified: Sun May 21 20:44:54 2023, max compression
+gzip compressed data, was "discoger-2.0.0.tar", last modified: Fri Jul  7 13:42:52 2023, max compression
```

## Comparing `discoger-1.2.1.tar` & `discoger-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:44:54.335148 discoger-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 20:44:39.000000 discoger-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-21 20:44:54.335148 discoger-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-21 20:44:39.000000 discoger-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:44:54.331148 discoger-1.2.1/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:44:39.000000 discoger-1.2.1/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-21 20:44:39.000000 discoger-1.2.1/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-21 20:44:39.000000 discoger-1.2.1/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:44:54.335148 discoger-1.2.1/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-21 20:44:54.000000 discoger-1.2.1/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-21 20:44:54.000000 discoger-1.2.1/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:44:54.000000 discoger-1.2.1/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 20:44:54.000000 discoger-1.2.1/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-21 20:44:54.000000 discoger-1.2.1/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 20:44:54.000000 discoger-1.2.1/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 20:44:54.335148 discoger-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-21 20:44:39.000000 discoger-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:52.258410 discoger-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 13:42:29.000000 discoger-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-07 13:42:52.258410 discoger-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-07 13:42:29.000000 discoger-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:52.254410 discoger-2.0.0/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:52.254410 discoger-2.0.0/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 13:42:52.258410 discoger-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-07 13:42:29.000000 discoger-2.0.0/setup.py
```

### Comparing `discoger-1.2.1/LICENSE` & `discoger-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.2.1/PKG-INFO` & `discoger-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.2.1
+Version: 2.0.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.2.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.0.0.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
@@ -27,14 +27,16 @@
         ### Configuration
         
         After that you need create config.ini file
         
         ```
         [DEFAULT]
         schedule_time = 30
+        disable_unofficial = True
+        log_level = INFO
         
         [discogs]
         secret = dbPVkGbCVVffggfgkdfgmlkknzezsbhmscskncno
         
         [telegram]
         token = 1766763279:AAFwufBsdfdsfgdfsgfgsfsgdfgsdf
         ```
```

### Comparing `discoger-1.2.1/README.md` & `discoger-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 ### Configuration
 
 After that you need create config.ini file
 
 ```
 [DEFAULT]
 schedule_time = 30
+disable_unofficial = True
+log_level = INFO
 
 [discogs]
 secret = dbPVkGbCVVffggfgkdfgmlkknzezsbhmscskncno
 
 [telegram]
 token = 1766763279:AAFwufBsdfdsfgdfsgfgsfsgdfgsdf
 ```
```

### Comparing `discoger-1.2.1/discoger/discoger.py` & `discoger-2.0.0/discoger/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,257 +1,220 @@
 #!/usr/bin/env python3
 
 import configparser
 import discogs_client
 import logging
-import feedparser
 import threading
 import schedule
-import telebot
 import time
 import re
 
 from yamldb.YamlDB import YamlDB
 from pathlib import Path
 from time import sleep
-from telebot import types, util
+from telebot import types, util, telebot
+from discoger import scrap, utils
 
-logging.basicConfig(format='%(asctime)s %(levelname)s - %(message)s', level=logging.INFO)
 
-home = str(Path.home())
-config_file = Path(home + "/.config/discoger/config.ini")
-database_dir = Path(home + "/.config/discoger/databases")
-discogs_url = 'https://www.discogs.com'
-
-if config_file.exists():
-    config = configparser.ConfigParser()
-    config.read(config_file)
-else:
-    logging.error("No config file, please create a config file follwing example")
-    raise SystemExit()
-
-if not database_dir.exists():
-    database_dir.mkdir(parents=True, exist_ok=True)
-
-token = config["telegram"]["token"]
-secret = config["discogs"]["secret"]
-disable_unofficial = config["DEFAULT"].getboolean('disable_unofficial', fallback=True)
-bot = telebot.TeleBot(token)
-
-commands = {  # command description used in the "help" command
-    '/start': 'Get used to the bot',
-    '/help': 'Gives you information about the available commands',
-    '/list': 'Show all items in your following list',
-    '/delete': 'Delete item from the following list',
-    'https://www.discogs.com/release|master/.*': 'Add release or master release in following list (ex: https://www.discogs.com/release/26741825)'
-}
-
-try:
-    d = discogs_client.Client('DiscogsAlert/0.1', user_token=secret)
-    me = d.identity()
-except discogs_client.exceptions.HTTPError as e:
-    logging.error('Error: Unable to authenticate.')
-    raise SystemExit(e)
-
-
-@bot.message_handler(commands=['help', 'start'])
-def send_welcome(message):
-    chat_id = message.chat.id
-    msg = "Hi there, I am Discoger bot"
-    db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    if not db.get("release_list"):
-        db["release_list"] = list()
-        db["chat_id"] = chat_id
-        db.save()
-    bot.reply_to(message, msg)
-    process_hi_step(chat_id)
-
-
-def process_hi_step(chat_id):
-    markup = types.ReplyKeyboardMarkup()
-    itembtna = types.KeyboardButton('/help')
-    itembtnb = types.KeyboardButton('/check')
-    itembtnc = types.KeyboardButton('/list')
-    itembtnd = types.KeyboardButton('/delete')
-    markup.row(itembtna, itembtnb)
-    markup.row(itembtnc, itembtnd)
-    help_text = "What do you want?\n"
-    for key in commands:
-        help_text += key + " "
-        help_text += commands[key] + "\n"
-    bot.send_message(chat_id, help_text, reply_markup=markup, disable_web_page_preview=True)
-
-
-@bot.message_handler(commands=['check'])
-def get_check(message):
-    chat_id = message.chat.id
-    db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    if db.get("release_list"):
-        bot.send_message(chat_id, "Okay i'm checkng your following list")
-        check_discogs(chat_id)
-    else:
-        bot.send_message(chat_id, "Your discoger following list is empty, send me a url first")
-
-
-@bot.message_handler(regexp="^https://www.discogs.com/.*(release|master)/.*")
-def handle_message(message):
-    release_info = dict()
-    chat_id = message.chat.id
-    release_id = re.findall(r'\d+', message.text)[0]
-    db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    if not db.search("release_list[?release_id=='%s']" % (release_id)):
-        if len(re.findall(r'\/master\/\d+', message.text)) == 1:
-            master_release_info = d.master(release_id)
-            release_all_info = d.release(master_release_info.main_release.id)
+class Discoger:
+    def __init__(self):
+        self.home = str(Path.home())
+        self.config_file = Path(self.home + "/.config/discoger/config.ini")
+        self.database_dir = Path(self.home + "/.config/discoger/databases")
+        self.discogs_url = "https://www.discogs.com"
+
+        if self.config_file.exists():
+            self.config = configparser.ConfigParser()
+            self.config.read(self.config_file)
         else:
-            release_all_info = d.release(release_id)
-        db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-        release_info["release_id"] = release_id
-        release_info["artist"] = release_all_info.artists[0].name
-        release_info["title"] = release_all_info.title
-        release_info["url"] = message.text
-        if len(re.findall(r'\/master\/\d+', message.text)) == 1:
-            release_info["type"] = "master"
-        else:
-            release_info["type"] = "release"
-        release_info["last_sell"] = dict()
-        db["release_list"].append(release_info)
-        db.save()
-        bot.send_message(chat_id, "%s is added in following list" % (release_id))
-    else:
-        bot.send_message(chat_id, "%s is already in following list" % (release_id))
-
-
-@bot.message_handler(commands=['list'])
-def get_list(message):
-    chat_id = message.chat.id
-    db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    if not db.get("release_list"):
-        bot.send_message(chat_id, "Your discoger following list is empty, send me a url first")
-    else:
-        id_list = 0
-        all_text = ""
-        for i in db["release_list"]:
-            sell_type = i.get("type")
-            if sell_type is None:
-                sell_type = "release"
-            text = "%s: %s - %s %s/%s/%s" % (id_list, i["artist"], i["title"], discogs_url, sell_type, i["release_id"])
-            all_text = all_text + "\n" + text
-            id_list = id_list + 1
-        splitted_text = util.split_string(all_text, 3000)
-        for text in splitted_text:
-            bot.send_message(chat_id, text, disable_web_page_preview=True)
-
-
-@bot.message_handler(commands=['delete'])
-def delete_release(message):
-    msg = "Which item do you want delete in your list?"
-    answer = bot.reply_to(message, msg)
-    bot.register_next_step_handler(answer, process_delete_step)
-
-
-def process_delete_step(message):
-    chat_id = message.chat.id
-    id_item = message.text
-    db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    db["release_list"].pop(int(id_item))
-    db.save()
-    bot.send_message(chat_id, "%s is deleted in following list" % (id_item))
-
-
-def check_sales(release_id, type_sell):
-    data_last_sell = dict()
-    if type_sell == 'master':
-        url = f"{discogs_url}/sell/mplistrss?output=rss&master_id={release_id}&ev=mb&format=Vinyl"
-    else:
-        url = f"{discogs_url}/sell/mplistrss?output=rss&release_id={release_id}"
-    feed = feedparser.parse(url)
-    try:
-        entry = feed.entries[-1]
-        data_last_sell["id"] = re.findall(r'\d+', entry["link"])[0]
-        data_last_sell["date"] = entry["updated"]
-        data_last_sell["url"] = entry["link"]
-        data_last_sell["price"] = re.findall(r'... \d?\d?\d\d.\d\d', entry["summary_detail"]["value"])[0]
-        if disable_unofficial and len(re.findall('Unofficial', entry["title"])) > 0:
-            return None
-        else:
-            return data_last_sell
-    except Exception as e:
-        logging.debug("%s: for %s item" % (e, release_id))
-        return None
-
-
-def check_price(release_id, type_sell):
-    if type_sell == 'master':
-        return None
-    else:
-        _info = d.release(release_id)
-    return "%s %s" % (round(_info.price_suggestions.mint.value, 2), _info.price_suggestions.mint.currency)
-
-
-def check_discogs(chat_id=None):
-    if chat_id:
-        logging.info("Check user list %s" % (chat_id))
-        scrap_data(chat_id)
-    else:
-        logging.info("Check all list")
-        for x in database_dir.iterdir():
-            chat_id = re.findall(r'\d+', str(x))[0]
-            logging.info("Check user list %s" % (chat_id))
-            scrap_data(chat_id)
-
-
-def scrap_data(chat_id):
-    db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    chat_id = db.get("chat_id")
-    for i in range(len(db["release_list"])):
-        item = db.search("release_list[%s]" % (str(i)))
-        sell_type = item.get("type")
-        if sell_type is None:
-            sell_type = "release"
-        data_last_sell = check_sales(item["release_id"], sell_type)
-        if data_last_sell:
-            if not item["last_sell"] or (item["last_sell"]["id"] != data_last_sell["id"] and item["last_sell"]["date"] < data_last_sell["date"]):
-                good_price = check_price(item["release_id"], sell_type)
-                logging.info("New item for %s - %s" % (item["artist"], item["title"]))
-                text = "New release for:\n%s - %s\nDate: %s\nPrice: %s\nGood price: %s\n%s" % (item["artist"], item["title"], data_last_sell["date"], data_last_sell["price"], good_price, data_last_sell["url"])
-                bot.send_message(chat_id, text, disable_web_page_preview=True)
-                db["release_list"][i]["last_sell"] = data_last_sell
-            else:
-                logging.info("Not new item for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
-        else:
-            logging.info("Nothing available for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
-    db.save()
-
+            logging.error(
+                "No config file, please create a config file follwing example"
+            )
+            raise SystemExit()
+
+        if not self.database_dir.exists():
+            self.database_dir.mkdir(parents=True, exist_ok=True)
+
+        self.token = self.config["telegram"]["token"]
+        self.secret = self.config["discogs"]["secret"]
+        self.disable_unofficial = self.config["DEFAULT"].getboolean(
+            "disable_unofficial", fallback=True
+        )
+        self.bot = telebot.TeleBot(self.token)
+        self.log_level = self.config["DEFAULT"]["log_level"]
+
+        handler = logging.StreamHandler()
+        handler.setFormatter(utils.CustomFormatter())
+        logger = logging.getLogger()
+        logger.addHandler(handler)
+        logger.setLevel(self.log_level)
+
+        self.commands = {  # command description used in the "help" command
+            "/start": "Get used to the bot",
+            "/help": "Gives you information about the available commands",
+            "/list": "Show all items in your following list",
+            "/delete": "Delete item from the following list",
+            "https://www.discogs.com/release|master/.*": "Add release or master release in following list (ex: https://www.discogs.com/release/26741825)",
+        }
 
-def bot_polling():
-    while True:
         try:
-            logging.info("Starting bot polling now. New bot instance started!")
-            bot.polling(none_stop=True, interval=3, timeout=30)
-        except Exception as ex:
-            logging.error("Bot polling failed, restarting in {}sec. Error:\n{}".format(30, ex))
-            bot.stop_polling()
-            sleep(30)
-        else:
-            bot.stop_polling()
-            logging.info("Bot polling loop finished.")
-            break
-
-
-def run_threaded(job_func):
-    job_thread = threading.Thread(target=job_func)
-    job_thread.start()
-
-
-def main():
-    schedule.every(int(config["DEFAULT"]["schedule_time"])).minutes.do(run_threaded, check_discogs)
-    polling_thread = threading.Thread(target=bot_polling)
-    polling_thread.daemon = True
-    polling_thread.start()
-    while 1:
-        schedule.run_pending()
-        time.sleep(1)
+            self.d = discogs_client.Client("DiscogsAlert/0.1", user_token=self.secret)
+            self.me = self.d.identity()
+        except discogs_client.exceptions.HTTPError as e:
+            logging.error("Error: Unable to authenticate.")
+            raise SystemExit(e)
+
+        @self.bot.message_handler(commands=["help", "start"])
+        def send_welcome(message):
+            chat_id = message.chat.id
+            msg = "Hi there, I am Discoger bot"
+            db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, self.home, chat_id))
+            if not db.get("release_list"):
+                db["release_list"] = list()
+                db["chat_id"] = chat_id
+                db.save()
+            self.bot.reply_to(message, msg)
+            process_hi_step(chat_id)
+
+        def process_hi_step(chat_id):
+            markup = types.ReplyKeyboardMarkup()
+            itembtna = types.KeyboardButton("/help")
+            itembtnb = types.KeyboardButton("/check")
+            itembtnc = types.KeyboardButton("/list")
+            itembtnd = types.KeyboardButton("/delete")
+            markup.row(itembtna, itembtnb)
+            markup.row(itembtnc, itembtnd)
+            help_text = "What do you want?\n"
+            for key in self.commands:
+                help_text += key + " "
+                help_text += self.commands[key] + "\n"
+            self.bot.send_message(
+                chat_id, help_text, reply_markup=markup, disable_web_page_preview=True
+            )
+
+        @self.bot.message_handler(commands=["check"])
+        def get_check(message):
+            chat_id = message.chat.id
+            db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
+            if db.get("release_list"):
+                self.bot.send_message(chat_id, "Okay i'm checkng your following list")
+                check_discogs(chat_id)
+            else:
+                self.bot.send_message(
+                    chat_id,
+                    "Your discoger following list is empty, send me a url first",
+                )
+
+        @self.bot.message_handler(
+            regexp="^https://www.discogs.com/.*(release|master)/.*"
+        )
+        def handle_message(message):
+            chat_id = message.chat.id
+            url = message.text
+            release_id = re.findall(r"\d+", url)[0]
+            db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
+            if not db.search("release_list[?release_id=='%s']" % (release_id)):
+                release = scrap.DiscogerInfo(url, self.d, release_id)
+                db["release_list"].append(release.release_info)
+                db.save()
+                self.bot.send_message(
+                    chat_id, "%s is added in following list" % (release_id)
+                )
+            else:
+                self.bot.send_message(
+                    chat_id, "%s is already in following list" % (release_id)
+                )
+
+        @self.bot.message_handler(commands=["list"])
+        def get_list(message):
+            chat_id = message.chat.id
+            db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, self.home, chat_id))
+            if not db.get("release_list"):
+                self.bot.send_message(
+                    chat_id,
+                    "Your discoger following list is empty, send me a url first",
+                )
+            else:
+                id_list = 0
+                all_text = ""
+                for i in db["release_list"]:
+                    sell_type = i.get("type")
+                    if sell_type is None:
+                        sell_type = "release"
+                    text = "%s: %s - %s %s/%s/%s" % (
+                        id_list,
+                        i["artist"],
+                        i["title"],
+                        self.discogs_url,
+                        sell_type,
+                        i["release_id"],
+                    )
+                    all_text = all_text + "\n" + text
+                    id_list = id_list + 1
+                splitted_text = util.split_string(all_text, 3000)
+                for text in splitted_text:
+                    self.bot.send_message(chat_id, text, disable_web_page_preview=True)
+
+        @self.bot.message_handler(commands=["delete"])
+        def delete_release(message):
+            msg = "Which item do you want delete in your list?"
+            answer = self.bot.reply_to(message, msg)
+            self.bot.register_next_step_handler(answer, process_delete_step)
+
+        def process_delete_step(message):
+            chat_id = message.chat.id
+            id_item = message.text
+            db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
+            db["release_list"].pop(int(id_item))
+            db.save()
+            self.bot.send_message(
+                chat_id, "%s is deleted in following list" % (id_item)
+            )
+
+        def check_discogs(chat_id=None):
+            if chat_id:
+                logging.info("Check user list %s" % (chat_id))
+                db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
+                utils.scrap_data(self, chat_id, db)
+            else:
+                logging.info("Check all list")
+                for x in self.database_dir.iterdir():
+                    chat_id = re.findall(r"\d+", str(x))[0]
+                    logging.info("Check user list %s" % (chat_id))
+                    db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
+                    utils.scrap_data(self, chat_id, db)
+
+        def bot_polling():
+            while True:
+                try:
+                    logging.info("Starting bot polling now. New bot instance started!")
+                    self.bot.polling(none_stop=True, interval=3, timeout=30)
+                except Exception as ex:
+                    logging.error(
+                        "Bot polling failed, restarting in {}sec. Error:\n{}".format(
+                            30, ex
+                        )
+                    )
+                    self.bot.stop_polling()
+                    sleep(30)
+                else:
+                    self.bot.stop_polling()
+                    logging.info("Bot polling loop finished.")
+                    break
+
+        def run_threaded(job_func):
+            job_thread = threading.Thread(target=job_func)
+            job_thread.start()
+
+        schedule.every(int(self.config["DEFAULT"]["schedule_time"])).minutes.do(
+            run_threaded, check_discogs
+        )
+        polling_thread = threading.Thread(target=bot_polling)
+        polling_thread.daemon = True
+        polling_thread.start()
+        while 1:
+            schedule.run_pending()
+            time.sleep(1)
 
 
 if __name__ == "__main__":
-    main()
+    Discoger()
```

### Comparing `discoger-1.2.1/discoger.egg-info/PKG-INFO` & `discoger-2.0.0/discoger.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.2.1
+Version: 2.0.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.2.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.0.0.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
@@ -27,14 +27,16 @@
         ### Configuration
         
         After that you need create config.ini file
         
         ```
         [DEFAULT]
         schedule_time = 30
+        disable_unofficial = True
+        log_level = INFO
         
         [discogs]
         secret = dbPVkGbCVVffggfgkdfgmlkknzezsbhmscskncno
         
         [telegram]
         token = 1766763279:AAFwufBsdfdsfgdfsgfgsfsgdfgsdf
         ```
```

### Comparing `discoger-1.2.1/setup.py` & `discoger-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 import setuptools
 import discoger._info as package_info
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-with open("requirements.txt", 'r') as fh:
-    requirements = fh.read().splitlines()
-
 setuptools.setup(
     name=package_info.__title__,  # How you named your package folder (MyLib)
     packages=setuptools.find_packages(),
     version=package_info.__version__,  # Start with a small number and increase it with every
     license=package_info.__license__,
     description=package_info.__description__,  # Give a short description about your library
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=package_info.__author__,  # Type in your name
     author_email=package_info.__author_email__,  # Type in your E-Mail
-    url=f'https://github.com/{package_info.__github_username__}/{package_info.__title__}',  #
-    download_url=f'https://github.com/{package_info.__github_username__}/{package_info.__title__}/archive/{package_info.__version__}.tar.gz',
+    url=f"https://github.com/{package_info.__github_username__}/{package_info.__title__}",  #
+    download_url=f"https://github.com/{package_info.__github_username__}/{package_info.__title__}/archive/{package_info.__version__}.tar.gz",
     keywords=package_info.__keywords__,
-    install_requires=requirements,
-    entry_points={"console_scripts": ["discoger = discoger.discoger:main"]},
+    entry_points={"console_scripts": ["discoger = discoger.client:main"]},
     classifiers=[
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Development Status :: 5 - Production/Stable',
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Development Status :: 5 - Production/Stable",
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state
-        'Programming Language :: Python :: 3',  # Specify which python versions that you want
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Internet :: WWW/HTTP',
-        'Operating System :: OS Independent'
+        "Programming Language :: Python :: 3",  # Specify which python versions that you want
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Topic :: Internet :: WWW/HTTP",
+        "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7'
+    python_requires=">=3.7",
 )
```

