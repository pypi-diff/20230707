# Comparing `tmp/dry_scraper-0.1.8.7.tar.gz` & `tmp/dry_scraper-0.1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.8.7.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.8.8.tar", max compression
```

## Comparing `dry_scraper-0.1.8.7.tar` & `dry_scraper-0.1.8.8.tar`

### file list

```diff
@@ -1,27 +1,18 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.7/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.7/README.md
--rw-r--r--   0        0        0      550 2023-07-04 23:32:13.053047 dry_scraper-0.1.8.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.7/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.7/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.7/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0      178 2023-07-03 00:35:36.672352 dry_scraper-0.1.8.7/src/dry_scraper/nhl/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    42983 2023-07-04 23:12:54.332263 dry_scraper-0.1.8.7/src/dry_scraper/nhl/__pycache__/nhl_api_sources.cpython-311.pyc
--rw-r--r--   0        0        0    29655 2023-07-04 23:12:43.115480 dry_scraper-0.1.8.7/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0     4223 2023-07-04 23:30:26.748776 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/__pycache__/base_model.cpython-311.pyc
--rw-r--r--   0        0        0     1906 2023-07-04 23:30:26.752109 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/__pycache__/nhl_conferences_api_source.cpython-311.pyc
--rw-r--r--   0        0        0     2785 2023-07-04 23:30:26.752109 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/__pycache__/nhl_divisions_api_source.cpython-311.pyc
--rw-r--r--   0        0        0    30946 2023-07-04 23:30:26.748776 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/__pycache__/nhl_game_live_feed_api_source.cpython-311.pyc
--rw-r--r--   0        0        0     4174 2023-07-04 23:30:26.752109 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/__pycache__/nhl_people_api_source.cpython-311.pyc
--rw-r--r--   0        0        0     4649 2023-07-04 20:06:29.943027 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/__pycache__/nhl_schedule_api_source.cpython-311.pyc
--rw-r--r--   0        0        0     5103 2023-07-04 23:30:26.752109 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/__pycache__/nhl_teams_api_source.cpython-311.pyc
--rw-r--r--   0        0        0     2103 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/base_model.py
--rw-r--r--   0        0        0      688 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0     1044 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     6823 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    14863 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1874 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     2273 2023-07-04 02:50:05.226525 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     2186 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.7/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.7/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.8/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.8/README.md
+-rw-r--r--   0        0        0      550 2023-07-07 00:19:41.025172 dry_scraper-0.1.8.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.8/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.8/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.8/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    29866 2023-07-05 22:33:14.060482 dry_scraper-0.1.8.8/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0     2103 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/base_model.py
+-rw-r--r--   0        0        0      688 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0     1044 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     6823 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    14863 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1874 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     2273 2023-07-04 02:50:05.226525 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     2186 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.8/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.8/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.8/PKG-INFO
```

### Comparing `dry_scraper-0.1.8.7/LICENSE` & `dry_scraper-0.1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/README.md` & `dry_scraper-0.1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/pyproject.toml` & `dry_scraper-0.1.8.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.8.7"
+version = "0.1.8.8"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/data_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/data_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -520,35 +520,37 @@
             f"{self.season[:4]}"
             "0"
             f"{self.gamePk}"
             "/linescore"
         )
 
 
-def determine_team_decision(team_win: bool, ordinal: str) -> str:
+def determine_team_decision(team_goal_differential: int, ordinal: str) -> str:
     """
     Determine the decision of the game from the perspective of one team
     e.g., RW, OTL, SOW, etc.
 
     Parameters
     ----------
-    team_win : bool
-        bool describing if the team in question won or not
+    team_goal_differential : int
+        goal differential from the perspective of one team
     ordinal : str
         ordinal str describing the most recent period played
         e.g., 3rd, OT, SO
 
     Returns
     -------
     decision : str
         string describing decision of game from the perspective of one team
         e.g., RW, OTL, SOW, etc.
     """
+    if team_goal_differential == 0:
+        return "T"
     decision = "R" if ordinal == "3rd" else ordinal
-    return decision + "W" if team_win else decision + "L"
+    return decision + "W" if team_goal_differential > 0 else decision + "L"
 
 
 class NhlGameLiveFeedApiSource(NhlGameApiSource):
     """
     Subclass of NhlApiSource that represents a request from the NHL live feed API
 
     ...
@@ -771,17 +773,17 @@
         away_team_info = self.content_pyd.game_data.teams.away
         team_stats_df = pd.DataFrame(
             {
                 col: pd.Series(dtype=typ)
                 for col, typ in nhl_game_live_feed_api_source.team_stats_df_model.items()
             }
         )
-        home_win = (
+        home_line_score_goal_differential = (
             self.content_pyd.live_data.line_score.teams.home.goals
-            > self.content_pyd.live_data.line_score.teams.away.goals
+            - self.content_pyd.live_data.line_score.teams.away.goals
         )
         start = self.content_pyd.game_data.date_time.date_time
         end = self.content_pyd.game_data.date_time.end_date_time
         for home, team_stats, oppo_stats, team_info, oppo_info in [
             (True, home_stats, away_stats, home_team_info, away_team_info),
             (False, away_stats, home_stats, away_team_info, home_team_info),
         ]:
@@ -831,15 +833,17 @@
                 ),
                 "oppo_blocked_shots": not_none(oppo_stats.blocked, int),
                 "oppo_takeaways": not_none(oppo_stats.takeaways, int),
                 "oppo_giveaways": not_none(oppo_stats.giveaways, int),
                 "oppo_hits": not_none(oppo_stats.hits, int),
                 "team_goal_differential": int(team_stats.goals) - int(oppo_stats.goals),
                 "team_decision": determine_team_decision(
-                    home_win if home else not home_win,
+                    home_line_score_goal_differential
+                    if home
+                    else -home_line_score_goal_differential,
                     self.content_pyd.live_data.line_score.current_period_ordinal,
                 ),
             }
             team_stats_df.loc[
                 f"{self.gamePk} Home" if home else f"{self.gamePk} Away"
             ] = team_dict
         return team_stats_df
```

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/base_model.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/base_model.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/shared.py` & `dry_scraper-0.1.8.8/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/src/dry_scraper/teams.py` & `dry_scraper-0.1.8.8/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.7/PKG-INFO` & `dry_scraper-0.1.8.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.8.7
+Version: 0.1.8.8
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

