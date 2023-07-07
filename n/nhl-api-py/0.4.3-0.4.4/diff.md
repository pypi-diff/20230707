# Comparing `tmp/nhl_api_py-0.4.3.tar.gz` & `tmp/nhl_api_py-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.4.3.tar", max compression
+gzip compressed data, was "nhl_api_py-0.4.4.tar", max compression
```

## Comparing `nhl_api_py-0.4.3.tar` & `nhl_api_py-0.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4940 2023-06-18 13:41:39.289397 nhl_api_py-0.4.3/README.md
--rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.4.3/nhlpy/__init__.py
--rw-r--r--   0        0        0      315 2023-06-21 16:19:03.961354 nhl_api_py-0.4.3/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.4.3/nhlpy/api/core.py
--rw-r--r--   0        0        0     4213 2023-06-16 18:35:41.424465 nhl_api_py-0.4.3/nhlpy/api/games.py
--rw-r--r--   0        0        0     8696 2023-06-29 12:52:27.845826 nhl_api_py-0.4.3/nhlpy/api/helpers.py
--rw-r--r--   0        0        0     2035 2023-06-16 18:35:41.424465 nhl_api_py-0.4.3/nhlpy/api/players.py
--rw-r--r--   0        0        0      910 2023-06-16 18:35:41.424465 nhl_api_py-0.4.3/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     1942 2023-06-18 13:41:39.289397 nhl_api_py-0.4.3/nhlpy/api/standings.py
--rw-r--r--   0        0        0     2146 2023-06-16 18:35:41.424465 nhl_api_py-0.4.3/nhlpy/api/teams.py
--rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.4.3/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1390 2023-06-29 12:55:44.735826 nhl_api_py-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 nhl_api_py-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     4940 2023-06-18 13:41:39.289397 nhl_api_py-0.4.4/README.md
+-rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.4.4/nhlpy/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-21 16:19:03.961354 nhl_api_py-0.4.4/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.4.4/nhlpy/api/core.py
+-rw-r--r--   0        0        0     4213 2023-06-16 18:35:41.424465 nhl_api_py-0.4.4/nhlpy/api/games.py
+-rw-r--r--   0        0        0     9046 2023-07-07 18:27:10.203733 nhl_api_py-0.4.4/nhlpy/api/helpers.py
+-rw-r--r--   0        0        0     2035 2023-06-16 18:35:41.424465 nhl_api_py-0.4.4/nhlpy/api/players.py
+-rw-r--r--   0        0        0      910 2023-06-16 18:35:41.424465 nhl_api_py-0.4.4/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1942 2023-06-18 13:41:39.289397 nhl_api_py-0.4.4/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     2146 2023-06-16 18:35:41.424465 nhl_api_py-0.4.4/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.4.4/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1390 2023-07-07 18:28:36.203734 nhl_api_py-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 nhl_api_py-0.4.4/PKG-INFO
```

### Comparing `nhl_api_py-0.4.3/README.md` & `nhl_api_py-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/nhlpy/api/core.py` & `nhl_api_py-0.4.4/nhlpy/api/core.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/nhlpy/api/games.py` & `nhl_api_py-0.4.4/nhlpy/api/games.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/nhlpy/api/helpers.py` & `nhl_api_py-0.4.4/nhlpy/api/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import warnings
 from typing import List, Optional
 
 from nhlpy.api.standings import Standings
 from nhlpy.api.schedule import Schedule
 from nhlpy.api.games import Games
 
@@ -181,29 +182,35 @@
         away_team = game_data["gameData"]["teams"]["away"]["id"]
         game_start = game_data["gameData"]["datetime"]["dateTime"]
 
         for event_type in game_data["liveData"]["plays"]["allPlays"]:
             if event_type["result"]["event"] != "Shot":
                 continue
             player_id, player_name = _get_shooter(event_type)
-            shot = {
-                "game_id": game_id,
-                "game_start": game_start,
-                "player_id": player_id,
-                "player_name": player_name,
-                "player_side": "HOME"
-                if home_team == event_type["team"]["id"]
-                else "AWAY",
-                "shot_type": event_type["result"]["secondaryType"],
-                "home_team": home_team,
-                "away_team": away_team,
-                "event": event_type["result"]["event"],
-                "event_type_id": event_type["result"]["eventTypeId"],
-                "event_descr": event_type["result"]["description"],
-                "period": event_type["about"]["period"],
-                "period_time": event_type["about"]["periodTime"],
-                "x_cord": event_type["coordinates"]["x"],
-                "y_cord": event_type["coordinates"]["y"]
-            }
-            shot_data.append(shot)
+            try:
+                shot = {
+                    "game_id": game_id,
+                    "game_start": game_start,
+                    "player_id": player_id,
+                    "player_name": player_name,
+                    "player_side": "HOME"
+                    if home_team == event_type["team"]["id"]
+                    else "AWAY",
+                    "shot_type": event_type["result"]["secondaryType"],
+                    "home_team": home_team,
+                    "away_team": away_team,
+                    "event": event_type["result"]["event"],
+                    "event_type_id": event_type["result"]["eventTypeId"],
+                    "event_descr": event_type["result"]["description"],
+                    "period": event_type["about"]["period"],
+                    "period_time": event_type["about"]["periodTime"],
+                    "x_cord": event_type["coordinates"]["x"],
+                    "y_cord": event_type["coordinates"]["y"],
+                }
+                shot_data.append(shot)
+            except KeyError:
+                logging.warning(
+                    f"KeyError for event: {event_type}, game_id: {game_id}, event code: {event_type['result']['eventCode']}"
+                )
+                continue
 
         return shot_data
```

### Comparing `nhl_api_py-0.4.3/nhlpy/api/players.py` & `nhl_api_py-0.4.4/nhlpy/api/players.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/nhlpy/api/schedule.py` & `nhl_api_py-0.4.4/nhlpy/api/schedule.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/nhlpy/api/standings.py` & `nhl_api_py-0.4.4/nhlpy/api/standings.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/nhlpy/api/teams.py` & `nhl_api_py-0.4.4/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/nhlpy/nhl_client.py` & `nhl_api_py-0.4.4/nhlpy/nhl_client.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.3/pyproject.toml` & `nhl_api_py-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.4.3"
+version = "0.4.4"
 description = "NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
```

### Comparing `nhl_api_py-0.4.3/PKG-INFO` & `nhl_api_py-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 0.4.3
+Version: 0.4.4
 Summary: NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications.
 Home-page: https://github.com/coreyjs/nhl-api-py
 License: GPL-3.0-or-later
 Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.10,<4.0
```

