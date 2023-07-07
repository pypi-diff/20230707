# Comparing `tmp/twscrape-0.4.1.tar.gz` & `tmp/twscrape-0.4.2.tar.gz`

## Comparing `twscrape-0.4.1.tar` & `twscrape-0.4.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.4.1/.gitattributes
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.4.1/Dockerfile-test
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 twscrape-0.4.1/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.4.1/.github/CODEOWNERS
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.4.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.4.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.4.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.4.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/test_api.py
--rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/test_parser.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/test_pool.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/test_queue_client.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/manual_tweet_with_video_1.json
--rw-r--r--   0        0        0    84696 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/manual_tweet_with_video_2.json
--rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   110556 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.4.1/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/account.py
--rw-r--r--   0        0        0     8859 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/accounts_pool.py
--rw-r--r--   0        0        0     9734 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/api.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/cli.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/constants.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/db.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/logger.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/login.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/models.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/queue_client.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 twscrape-0.4.1/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.4.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.4.1/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.4.1/readme.md
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.4.2/.gitattributes
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.4.2/Dockerfile-test
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 twscrape-0.4.2/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.4.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 twscrape-0.4.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.4.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.4.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.4.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/test_api.py
+-rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/test_parser.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/test_pool.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/test_queue_client.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/manual_tweet_with_video_1.json
+-rw-r--r--   0        0        0    84696 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/manual_tweet_with_video_2.json
+-rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   110556 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.4.2/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/account.py
+-rw-r--r--   0        0        0     8983 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0     9781 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/api.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/cli.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/constants.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/db.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/logger.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/login.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/models.py
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/queue_client.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 twscrape-0.4.2/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 twscrape-0.4.2/readme.md
+-rw-r--r--   0        0        0     8090 2020-02-02 00:00:00.000000 twscrape-0.4.2/PKG-INFO
```

### Comparing `twscrape-0.4.1/Dockerfile-test` & `twscrape-0.4.2/Dockerfile-test`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/Makefile` & `twscrape-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/.github/workflows/publish.yml` & `twscrape-0.4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/conftest.py` & `twscrape-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/test_api.py` & `twscrape-0.4.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/test_parser.py` & `twscrape-0.4.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/test_pool.py` & `twscrape-0.4.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/test_queue_client.py` & `twscrape-0.4.2/tests/test_queue_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from contextlib import aclosing
+
 import httpx
 from pytest_httpx import HTTPXMock
 
 from twscrape.accounts_pool import AccountsPool
 from twscrape.logger import set_log_level
 from twscrape.queue_client import QueueClient
 
@@ -88,15 +90,15 @@
     # unlock on exit (failed account still should locked)
     await client.__aexit__(None, None, None)
     locked3 = await get_locked(pool)
     assert len(locked3) == 1
     assert locked1 == locked3  # failed account locked
 
 
-async def test_retry_with_same_acc_on_network_error(httpx_mock: HTTPXMock, client_fixture):
+async def test_retry_with_same_acc_on_network_error(httpx_mock: HTTPXMock, client_fixture: CF):
     pool, client = client_fixture
 
     # locked account on enter
     await client.__aenter__()
     locked1 = await get_locked(pool)
     assert len(locked1) == 1
 
@@ -109,7 +111,47 @@
 
     locked2 = await get_locked(pool)
     assert locked2 == locked1
 
     # check username added to request obj (for logging)
     username = getattr(rep, "__username", None)
     assert username is not None
+
+
+async def test_ctx_closed_on_break(httpx_mock: HTTPXMock, client_fixture: CF):
+    pool, client = client_fixture
+
+    async def get_data_stream():
+        async with client as c:
+            counter = 0
+            while True:
+                counter += 1
+                check_retry = counter == 2
+                before_ctx = c.ctx
+
+                if check_retry:
+                    httpx_mock.add_response(url=URL, json={"counter": counter}, status_code=403)
+                    httpx_mock.add_response(url=URL, json={"counter": counter}, status_code=200)
+                else:
+                    httpx_mock.add_response(url=URL, json={"counter": counter}, status_code=200)
+
+                rep = await c.get(URL)
+
+                if check_retry:
+                    assert before_ctx != c.ctx
+                elif before_ctx is not None:
+                    assert before_ctx == c.ctx
+
+                assert rep.json() == {"counter": counter}
+                yield rep.json()["counter"]
+
+                if counter == 9:
+                    return
+
+    # need to use async with to break to work
+    async with aclosing(get_data_stream()) as gen:
+        async for x in gen:
+            if x == 3:
+                break
+
+    # ctx should be None after break
+    assert client.ctx is None
```

### Comparing `twscrape-0.4.1/tests/mocked-data/favoriters_raw.json` & `twscrape-0.4.2/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/followers_raw.json` & `twscrape-0.4.2/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/following_raw.json` & `twscrape-0.4.2/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/manual_tweet_with_video_1.json` & `twscrape-0.4.2/tests/mocked-data/manual_tweet_with_video_1.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/manual_tweet_with_video_2.json` & `twscrape-0.4.2/tests/mocked-data/manual_tweet_with_video_2.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/retweeters_raw.json` & `twscrape-0.4.2/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/search_raw.json` & `twscrape-0.4.2/tests/mocked-data/search_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.4.2/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.4.2/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.4.2/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.4.2/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.4.2/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/account.py` & `twscrape-0.4.2/twscrape/account.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/accounts_pool.py` & `twscrape-0.4.2/twscrape/accounts_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,18 +129,19 @@
             logger.info(f"[{i}/{len(accounts)}] Logging in {x.username} - {x.email}")
             await self.login(x)
 
     async def set_active(self, username: str, active: bool):
         qs = "UPDATE accounts SET active = :active WHERE username = :username"
         await execute(self._db_file, qs, {"username": username, "active": active})
 
-    async def lock_until(self, username: str, queue: str, unlock_at: int):
+    async def lock_until(self, username: str, queue: str, unlock_at: int, req_count=0):
         qs = f"""
         UPDATE accounts SET
             locks = json_set(locks, '$.{queue}', datetime({unlock_at}, 'unixepoch')),
+            stats = json_set(stats, '$.{queue}', COALESCE(json_extract(stats, '$.{queue}'), 0) + {req_count}),
             last_used = datetime({utc_ts()}, 'unixepoch')
         WHERE username = :username
         """
         await execute(self._db_file, qs, {"username": username})
 
     async def unlock(self, username: str, queue: str, req_count=0):
         qs = f"""
```

### Comparing `twscrape-0.4.1/twscrape/api.py` & `twscrape-0.4.2/twscrape/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from .logger import logger
 from .models import Tweet, User
 from .queue_client import QueueClient, req_id
 from .utils import encode_params, find_obj, get_by_path, to_old_obj, to_old_rep
 
 
 class API:
-    def __init__(self, pool: AccountsPool, debug=False):
-        self.pool = pool
+    def __init__(self, pool: AccountsPool | None, debug=False):
+        self.pool = pool if pool is not None else AccountsPool()
         self.debug = debug
 
     # general helpers
 
     def _is_end(self, rep: Response, q: str, res: list, cur: str | None, cnt: int, lim: int):
         new_count = len(res)
         new_total = cnt + new_count
```

### Comparing `twscrape-0.4.1/twscrape/cli.py` & `twscrape-0.4.2/twscrape/cli.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/constants.py` & `twscrape-0.4.2/twscrape/constants.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/db.py` & `twscrape-0.4.2/twscrape/db.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/imap.py` & `twscrape-0.4.2/twscrape/imap.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/login.py` & `twscrape-0.4.2/twscrape/login.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/models.py` & `twscrape-0.4.2/twscrape/models.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/twscrape/queue_client.py` & `twscrape-0.4.2/twscrape/queue_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,28 +35,31 @@
 
     async def __aenter__(self):
         await self._get_ctx()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self._close_ctx()
-        return self
 
-    async def _close_ctx(self):
-        if self.ctx is not None:
-            await self.ctx.clt.aclose()
-            await self.pool.unlock(self.ctx.acc.username, self.queue, self.ctx.req_count)
+    async def _close_ctx(self, reset_at=-1):
+        if self.ctx is None:
+            return
+
+        ctx, self.ctx, self.req_count = self.ctx, None, 0
+        await ctx.clt.aclose()
+
+        if reset_at <= 0:
+            await self.pool.unlock(ctx.acc.username, self.queue, ctx.req_count)
+        else:
+            await self.pool.lock_until(ctx.acc.username, self.queue, reset_at, ctx.req_count)
 
     async def _get_ctx(self) -> Ctx:
         if self.ctx:
             return self.ctx
 
-        if self.ctx is not None:
-            await self._close_ctx()
-
         acc = await self.pool.get_for_queue_or_wait(self.queue)
         clt = acc.make_client()
         self.ctx = Ctx(acc, clt)
         return self.ctx
 
     def _push_history(self, rep: httpx.Response):
         self.history.append(rep)
@@ -101,24 +104,22 @@
                 rep = e.response
                 log_id = f"{req_id(rep)} on queue={self.queue}"
 
                 # rate limit
                 if rep.status_code == 429:
                     logger.debug(f"Rate limit for {log_id}")
                     reset_ts = int(rep.headers.get("x-rate-limit-reset", 0))
-                    await self.pool.lock_until(ctx.acc.username, self.queue, reset_ts)
-                    self.ctx = None  # get next account
+                    await self._close_ctx(reset_ts)  # get next account on next iteration
                     continue
 
                 # possible account banned
                 if rep.status_code in (401, 403):
                     reset_ts = utc_ts() + 60 * 60  # + 1 hour
                     logger.warning(f"Code {rep.status_code} for {log_id} – frozen for 1h")
-                    await self.pool.lock_until(ctx.acc.username, self.queue, reset_ts)
-                    self.ctx = None  # get next account
+                    await self._close_ctx(reset_ts)  # get next account on next iteration
                     continue
 
                 # twitter can return different types of cursors that not transfers between accounts
                 # just take the next account, the current cursor can work in it
                 if rep.status_code == 400:
                     logger.debug(f"Cursor not valid for {log_id}")
                     continue
```

### Comparing `twscrape-0.4.1/twscrape/utils.py` & `twscrape-0.4.2/twscrape/utils.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/.gitignore` & `twscrape-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/LICENSE` & `twscrape-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.4.1/pyproject.toml` & `twscrape-0.4.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.4.1"
+version = "0.4.2"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
```

### Comparing `twscrape-0.4.1/readme.md` & `twscrape-0.4.2/readme.md`

 * *Files 20% similar despite different names*

```diff
@@ -97,14 +97,27 @@
     doc.dict()  # -> python dict
     doc.json()  # -> json string
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+### Stoping iteration with break
+
+In order to correctly release an account in case of `break` in loop, a special syntax must be used. Otherwise, Python's events loop will release lock on the account sometime in the future. See explanation [here](https://github.com/vladkens/twscrape/issues/27#issuecomment-1623395424).
+
+```python
+from contextlib import aclosing
+
+async with aclosing(api.search("elon musk")) as gen:
+    async for tweet in gen:
+        if tweet.id < 200:
+            break
+```
+
 ## CLI
 
 ### Get help on CLI commands
 
 ```sh
 # show all commands
 twscrape
@@ -134,17 +147,15 @@
 
 ### Get list of accounts and their statuses
 
 ```sh
 twscrape accounts
 
 # Output:
-# ───────────────────────────────────────────────────────────────────────────────────
 # username  logged_in  active  last_used            total_req  error_msg
-# ───────────────────────────────────────────────────────────────────────────────────
 # user1     True       True    2023-05-20 03:20:40  100        None
 # user2     True       True    2023-05-20 03:25:45  120        None
 # user3     False      False   None                 120        Login error
 ```
 
 ### Use different accounts file
 
@@ -179,14 +190,16 @@
 
 ```sh
 twscrape search "elon mask lang:es" --limit=20 --raw
 ```
 
 ## Limitations
 
+NOTE: After 1 July 2023 Twitter [introduced limits](https://twitter.com/elonmusk/status/1675187969420828672) on the number of tweets per day per account (and these continue to change), so the values below may not be fully correct.
+
 API rate limits (per account):
 - Search API – 250 req / 15 min
 - GraphQL API – has individual rate limits per operation (in most cases this is 500 req / 15 min)
 
 API data limits:
 - `user_tweets` & `user_tweets_and_replies` – can return ~3200 tweets maximum
```

### Comparing `twscrape-0.4.1/PKG-INFO` & `twscrape-0.4.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twscrape
-Version: 0.4.1
+Version: 0.4.2
 Summary: Twitter GraphQL and Search API implementation with SNScrape data models
 Project-URL: repository, https://github.com/vladkens/twscrape
 Author-email: vladkens <v.pronsky@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: api,scrape,scrapper,snscrape,twitter
 Classifier: Development Status :: 4 - Beta
@@ -124,14 +124,27 @@
     doc.dict()  # -> python dict
     doc.json()  # -> json string
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+### Stoping iteration with break
+
+In order to correctly release an account in case of `break` in loop, a special syntax must be used. Otherwise, Python's events loop will release lock on the account sometime in the future. See explanation [here](https://github.com/vladkens/twscrape/issues/27#issuecomment-1623395424).
+
+```python
+from contextlib import aclosing
+
+async with aclosing(api.search("elon musk")) as gen:
+    async for tweet in gen:
+        if tweet.id < 200:
+            break
+```
+
 ## CLI
 
 ### Get help on CLI commands
 
 ```sh
 # show all commands
 twscrape
@@ -161,17 +174,15 @@
 
 ### Get list of accounts and their statuses
 
 ```sh
 twscrape accounts
 
 # Output:
-# ───────────────────────────────────────────────────────────────────────────────────
 # username  logged_in  active  last_used            total_req  error_msg
-# ───────────────────────────────────────────────────────────────────────────────────
 # user1     True       True    2023-05-20 03:20:40  100        None
 # user2     True       True    2023-05-20 03:25:45  120        None
 # user3     False      False   None                 120        Login error
 ```
 
 ### Use different accounts file
 
@@ -206,14 +217,16 @@
 
 ```sh
 twscrape search "elon mask lang:es" --limit=20 --raw
 ```
 
 ## Limitations
 
+NOTE: After 1 July 2023 Twitter [introduced limits](https://twitter.com/elonmusk/status/1675187969420828672) on the number of tweets per day per account (and these continue to change), so the values below may not be fully correct.
+
 API rate limits (per account):
 - Search API – 250 req / 15 min
 - GraphQL API – has individual rate limits per operation (in most cases this is 500 req / 15 min)
 
 API data limits:
 - `user_tweets` & `user_tweets_and_replies` – can return ~3200 tweets maximum
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twscrape Version: 0.4.1 Summary: Twitter GraphQL
+Metadata-Version: 2.1 Name: twscrape Version: 0.4.2 Summary: Twitter GraphQL
 and Search API implementation with SNScrape data models Project-URL:
 repository, https://github.com/vladkens/twscrape Author-email: vladkens
 pronsky@gmail.com> License: MIT License-File: LICENSE Keywords:
 api,scrape,scrapper,snscrape,twitter Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Requires-Dist: aiosqlite==0.17.0 Requires-Dist: fake-
@@ -45,42 +45,49 @@
 (no limit) # note 2: all methods have `raw` version e.g.: async for tweet in
 api.search("elon musk"): print(tweet.id, tweet.user.username, tweet.rawContent)
 # tweet is `Tweet` object async for rep in api.search_raw("elon musk"): print
 (rep.status_code, rep.json()) # rep is `httpx.Response` object # change log
 level, default info set_log_level("DEBUG") # Tweet & User model can be
 converted to regular dict or json, e.g.: doc = await api.user_by_id(user_id) #
 User doc.dict() # -> python dict doc.json() # -> json string if __name__ ==
-"__main__": asyncio.run(main()) ``` ## CLI ### Get help on CLI commands ```sh #
-show all commands twscrape # help on specific comand twscrape search --help ```
-### Add accounts & login First add accounts from file: ```sh # twscrape
+"__main__": asyncio.run(main()) ``` ### Stoping iteration with break In order
+to correctly release an account in case of `break` in loop, a special syntax
+must be used. Otherwise, Python's events loop will release lock on the account
+sometime in the future. See explanation [here](https://github.com/vladkens/
+twscrape/issues/27#issuecomment-1623395424). ```python from contextlib import
+aclosing async with aclosing(api.search("elon musk")) as gen: async for tweet
+in gen: if tweet.id < 200: break ``` ## CLI ### Get help on CLI commands ```sh
+# show all commands twscrape # help on specific comand twscrape search --help
+``` ### Add accounts & login First add accounts from file: ```sh # twscrape
 add_accounts   # line_format should have "username", "password", "email",
 "email_password" tokens # tokens delimeter should be same as an file twscrape
 add_accounts accounts.txt username:password:email:email_password ``` The call
 login: ```sh twscrape login_accounts ``` Accounts and their sessions will be
 saved, so they can be reused for future requests ### Get list of accounts and
-their statuses ```sh twscrape accounts # Output: #
-âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
-# username logged_in active last_used total_req error_msg #
-âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
-# user1 True True 2023-05-20 03:20:40 100 None # user2 True True 2023-05-20 03:
-25:45 120 None # user3 False False None 120 Login error ``` ### Use different
-accounts file Useful if using a different set of accounts for different actions
-``` twscrape --db test-accounts.db  ``` ### Search commands ```sh twscrape
-search "QUERY" --limit=20 twscrape tweet_details TWEET_ID twscrape retweeters
-TWEET_ID --limit=20 twscrape favoriters TWEET_ID --limit=20 twscrape user_by_id
-USER_ID twscrape user_by_login USERNAME twscrape followers USER_ID --limit=20
-twscrape following USER_ID --limit=20 twscrape user_tweets USER_ID --limit=20
-twscrape user_tweets_and_replies USER_ID --limit=20 ``` The default output is
-in the console (stdout), one document per line. So it can be redirected to the
-file. ```sh twscrape search "elon mask lang:es" --limit=20 > data.txt ``` By
-default, parsed data is returned. The original tweet responses can be retrieved
-with `--raw` ```sh twscrape search "elon mask lang:es" --limit=20 --raw ``` ##
-Limitations API rate limits (per account): - Search API â 250 req / 15 min -
-GraphQL API â has individual rate limits per operation (in most cases this is
-500 req / 15 min) API data limits: - `user_tweets` & `user_tweets_and_replies`
-â can return ~3200 tweets maximum ## See also - [twitter-advanced-search]
-(https://github.com/igorbrigadir/twitter-advanced-search) â guide on search
-filters - [twitter-api-client](https://github.com/trevorhobenshield/twitter-
-api-client) â Implementation of Twitter's v1, v2, and GraphQL APIs -
-[snscrape](https://github.com/JustAnotherArchivist/snscrape) â is a scraper
-for social networking services (SNS) - [twint](https://github.com/twintproject/
-twint) â Twitter Intelligence Tool
+their statuses ```sh twscrape accounts # Output: # username logged_in active
+last_used total_req error_msg # user1 True True 2023-05-20 03:20:40 100 None #
+user2 True True 2023-05-20 03:25:45 120 None # user3 False False None 120 Login
+error ``` ### Use different accounts file Useful if using a different set of
+accounts for different actions ``` twscrape --db test-accounts.db  ``` ###
+Search commands ```sh twscrape search "QUERY" --limit=20 twscrape tweet_details
+TWEET_ID twscrape retweeters TWEET_ID --limit=20 twscrape favoriters TWEET_ID -
+-limit=20 twscrape user_by_id USER_ID twscrape user_by_login USERNAME twscrape
+followers USER_ID --limit=20 twscrape following USER_ID --limit=20 twscrape
+user_tweets USER_ID --limit=20 twscrape user_tweets_and_replies USER_ID --
+limit=20 ``` The default output is in the console (stdout), one document per
+line. So it can be redirected to the file. ```sh twscrape search "elon mask
+lang:es" --limit=20 > data.txt ``` By default, parsed data is returned. The
+original tweet responses can be retrieved with `--raw` ```sh twscrape search
+"elon mask lang:es" --limit=20 --raw ``` ## Limitations NOTE: After 1 July 2023
+Twitter [introduced limits](https://twitter.com/elonmusk/status/
+1675187969420828672) on the number of tweets per day per account (and these
+continue to change), so the values below may not be fully correct. API rate
+limits (per account): - Search API â 250 req / 15 min - GraphQL API â has
+individual rate limits per operation (in most cases this is 500 req / 15 min)
+API data limits: - `user_tweets` & `user_tweets_and_replies` â can return
+~3200 tweets maximum ## See also - [twitter-advanced-search](https://
+github.com/igorbrigadir/twitter-advanced-search) â guide on search filters -
+[twitter-api-client](https://github.com/trevorhobenshield/twitter-api-client)
+â Implementation of Twitter's v1, v2, and GraphQL APIs - [snscrape](https://
+github.com/JustAnotherArchivist/snscrape) â is a scraper for social
+networking services (SNS) - [twint](https://github.com/twintproject/twint) â
+Twitter Intelligence Tool
```

