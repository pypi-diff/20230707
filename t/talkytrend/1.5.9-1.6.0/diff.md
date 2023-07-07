# Comparing `tmp/talkytrend-1.5.9.tar.gz` & `tmp/talkytrend-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.5.9.tar", max compression
+gzip compressed data, was "talkytrend-1.6.0.tar", max compression
```

## Comparing `talkytrend-1.5.9.tar` & `talkytrend-1.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-06 13:13:33.559704 talkytrend-1.5.9/LICENSE
--rw-r--r--   0        0        0     3444 2023-07-06 13:13:33.559704 talkytrend-1.5.9/README.md
--rw-r--r--   0        0        0     2178 2023-07-06 13:13:34.511702 talkytrend-1.5.9/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-06 13:13:34.511702 talkytrend-1.5.9/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-07-06 13:13:33.559704 talkytrend-1.5.9/talkytrend/config.py
--rw-r--r--   0        0        0     2087 2023-07-06 13:13:33.559704 talkytrend-1.5.9/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6551 2023-07-06 13:13:33.559704 talkytrend-1.5.9/talkytrend/main.py
--rw-r--r--   0        0        0     4387 1970-01-01 00:00:00.000000 talkytrend-1.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-07 16:02:48.571368 talkytrend-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3444 2023-07-07 16:02:48.571368 talkytrend-1.6.0/README.md
+-rw-r--r--   0        0        0     2178 2023-07-07 16:02:49.383386 talkytrend-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-07 16:02:49.383386 talkytrend-1.6.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-07 16:02:48.571368 talkytrend-1.6.0/talkytrend/config.py
+-rw-r--r--   0        0        0     2087 2023-07-07 16:02:48.571368 talkytrend-1.6.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6714 2023-07-07 16:02:48.571368 talkytrend-1.6.0/talkytrend/main.py
+-rw-r--r--   0        0        0     4387 1970-01-01 00:00:00.000000 talkytrend-1.6.0/PKG-INFO
```

### Comparing `talkytrend-1.5.9/LICENSE` & `talkytrend-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.9/README.md` & `talkytrend-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.9/pyproject.toml` & `talkytrend-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.5.9"
+version = "1.6.0"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.5.9/talkytrend/config.py` & `talkytrend-1.6.0/talkytrend/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,13 +19,13 @@
         'talky_settings.toml',
         'settings.toml',
         '.secrets.toml'
     ],
     # Load the.env file
     load_dotenv=True,
     # merge=True,
-    # merge_enabled=True,
+    merge_enabled=True,
     # Set the environments to True
     environments=True,
     # Set the default environment
     default_env="default",)
```

### Comparing `talkytrend-1.5.9/talkytrend/default_settings.toml` & `talkytrend-1.6.0/talkytrend/default_settings.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 # export TT_SCANNER_FREQUENCY=3600
 
 
 [default]
 VALUE = "On Default"
 talkytrend_enabled = true
 talkytrend_mode = "scanner"
-talkytrend_scanner = false
+talkytrend_scanner = true
 talkytrend_scheduler = false
 scanner_frequency = 86400
 enable_signals = true
 assets = [
     { id ="EURUSD", exchange='FX_IDC',screener="forex", interval = "4h" },
     { id ="BTCUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
-    #use https://tvdb.brianthe.dev/ to get details
     # { id ="GOLD",exchange="TVC",screener="cfd", interval = "4h"},
     # { id ="USOIL",exchange="FX",screener="cfd", interval = "4h"},
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
+    #use https://tvdb.brianthe.dev/ to get details
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
-enable_news = true
+enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&max=2&apikey="
 news_api_key = ""
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 
 
 
 [testing]
```

### Comparing `talkytrend-1.5.9/talkytrend/main.py` & `talkytrend-1.6.0/talkytrend/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 from datetime import date
 import aiohttp
 from prettytable import PrettyTable, MARKDOWN
 from tradingview_ta import TA_Handler
 from talkytrend import __version__
 from talkytrend.config import settings
 
+
 class TalkyTrend:
     def __init__(self):
         try:
             self.logger = logging.getLogger("TalkyTrend")
             self.enabled = settings.talkytrend_enabled
             if not self.enabled:
                 return
             self.mode = settings.talkytrend_mode
             self.assets = settings.assets
             self.asset_signals = {}
             self.economic_calendar = settings.economic_calendar
-            self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
+            self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else settings.news_url
             self.live_tv = settings.live_tv_url
+            print(self.news_url)
         except Exception as error:
-            self.logger.error("TalkyTrend init error %s",error)
+            self.logger.error("TalkyTrend init error %s", error)
 
     async def fetch_analysis(
         self,
         asset_id,
         exchange,
         screener,
         interval):
@@ -37,23 +39,33 @@
             handler = TA_Handler(
                 symbol=asset_id,
                 exchange=exchange,
                 screener=screener,
                 interval=interval
             )
             analysis = handler.get_analysis()
-            return analysis.summary["RECOMMENDATION"]
+            # return analysis.summary["RECOMMENDATION"] as str
+            if analysis.summary["RECOMMENDATION"] == 'BUY':
+                return "🔼"
+            elif analysis.summary["RECOMMENDATION"] == 'STRONG_BUY':
+                return "⏫"
+            elif analysis.summary["RECOMMENDATION"] == 'SELL':
+                return "🔽"
+            elif analysis.summary["RECOMMENDATION"] == 'STRONG_SELL':
+                return "⏬"
+            else:
+                return "▶️"
         except Exception as error:
-            self.logger.error("event %s",error)
+            self.logger.error("event %s", error)
 
     async def check_signal(self):
         try:
             signals = []
             table = PrettyTable()
-            table.field_names = ["Asset", "4h"]
+            table.field_names = ["   Asset  ","   4h  "]
             for asset in self.assets:
                 current_signal = await self.fetch_analysis(
                     asset_id=asset["id"],
                     exchange=asset["exchange"],
                     screener=asset["screener"],
                     interval=asset["interval"]
                 )
@@ -62,39 +74,34 @@
                         "symbol": asset["id"],
                         "interval": asset["interval"],
                         "signal": current_signal
                     }
                     self.update_signal(asset["id"], asset["interval"], current_signal)
                     table.add_row([asset["id"], current_signal])
                     signals.append(signal_item)
-            #return signals
-            #return str(table)
-            # table.border = False
             table.set_style(MARKDOWN)
 
             return table.get_string()
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
 
-
     def is_new_signal(self, asset_id, interval, current_signal):
         if self.asset_signals.get(asset_id):
             if self.asset_signals[asset_id].get(interval) and current_signal != self.asset_signals[asset_id][interval]:
                 self.asset_signals[asset_id][interval] = current_signal
                 return True
         else:
             self.asset_signals[asset_id] = {interval: current_signal}
             return True
         return False
 
     def update_signal(self, asset_id, interval, current_signal):
         self.asset_signals[asset_id][interval] = current_signal
 
-
     def get_asset_signals(self):
         return self.asset_signals
 
     async def fetch_key_events(self):
         def filter_events(data, today):
             return [event for event in data if event.get('date', '').startswith(today)]
 
@@ -105,71 +112,65 @@
             return event.get('impact') == 'High' and event.get('country') == 'ALL'
 
         def is_opec_or_fomc(event):
             return "OPEC" in event.get('title') or "FOMC" in event.get('title')
 
         def format_event(event):
             return f"💬 {event['title']}\n⏰ {event['date']}"
-    
+
         async with aiohttp.ClientSession() as session:
             async with session.get(self.economic_calendar, timeout=10) as response:
                 response.raise_for_status()
                 data = await response.json()
                 today = date.today().isoformat()
                 events = filter_events(data, today)
                 for event in events:
                     if is_usd_high_impact(event) or is_all_high_impact(event):
                         return format_event(event)
                     if is_opec_or_fomc(event):
                         return format_event(event)
         return None
 
-
-
     async def fetch_key_news(self):
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(self.news_url, timeout=10) as response:
                     data = await response.json()
                     articles = data.get('articles', [])
                     key_news = [{'title': article['title'], 'url': article['url']} for article in articles]
                     last_item = key_news[-1]
-                    return f"📰 <a href='{last_item['url']}'>{last_item['title']}</a>"
-                    
+                    return str(f"📰 <a href='{last_item['url']}'>{last_item['title']}</a>")
+
         except aiohttp.ClientError as error:
             self.logger.error("news %s", error)
             return None
 
-            
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
         return any(event.startswith(current_date) for event in event_dates)
 
-
     async def scanner(self):
         while True:
             try:
                 if settings.enable_events:
                     key_events = await self.fetch_key_events()
                     if key_events is not None:
-                        self.logger.debug("Key event\n%s", key_events)
                         yield key_events
                 if settings.enable_news:
                     key_news = await self.fetch_key_news()
                     if key_news is not None:
-                        self.logger.debug("Key news\n%s", key_news)
                         yield key_news
 
                 if settings.enable_signals:
                     signals = await self.check_signal()
                     if signals is not None:
-                        self.logger.debug("Signals\n%s", signals)
                         yield signals
 
             except Exception as error:
-                self.logger.error("scanner %s", error)
+                print(error)
+                raise error
 
             await asyncio.sleep(settings.scanner_frequency)
 
     async def get_info(self):
         return f"{__class__.__name__} {__version__}\n"
```

### Comparing `talkytrend-1.5.9/PKG-INFO` & `talkytrend-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.5.9
+Version: 1.6.0
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.5.9 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.6.0 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: dynaconf (>=3.1.12,<4.0.0) Requires-Dist:
```

