# Comparing `tmp/unbelievaboat-1.2.0.tar.gz` & `tmp/unbelievaboat-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.2.0.tar", last modified: Fri Jul  7 13:27:20 2023, max compression
+gzip compressed data, was "unbelievaboat-1.2.1.tar", last modified: Fri Jul  7 14:03:53 2023, max compression
```

## Comparing `unbelievaboat-1.2.0.tar` & `unbelievaboat-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:27:20.146618 unbelievaboat-1.2.0/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3940 2023-07-07 13:27:20.146618 unbelievaboat-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3199 2023-07-06 17:33:53.000000 unbelievaboat-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 13:27:20.147618 unbelievaboat-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-07 13:26:58.000000 unbelievaboat-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:27:20.086937 unbelievaboat-1.2.0/unbelievaboat/
--rw-rw-rw-   0        0        0     7907 2023-07-07 13:25:42.000000 unbelievaboat-1.2.0/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3987 2023-07-07 12:24:42.000000 unbelievaboat-1.2.0/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.2.0/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:27:20.122913 unbelievaboat-1.2.0/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.2.0/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.2.0/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.2.0/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:27:20.133334 unbelievaboat-1.2.0/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.2.0/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      969 2023-07-07 13:16:24.000000 unbelievaboat-1.2.0/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.2.0/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.2.0/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1532 2023-07-07 13:25:58.000000 unbelievaboat-1.2.0/unbelievaboat/structures/UserBalance.py
--rw-rw-rw-   0        0        0     2357 2023-07-07 13:21:13.000000 unbelievaboat-1.2.0/unbelievaboat/structures/UserInventory.py
--rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.2.0/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:27:20.140564 unbelievaboat-1.2.0/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1322 2023-07-02 15:20:48.000000 unbelievaboat-1.2.0/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0     1169 2023-07-02 15:20:05.000000 unbelievaboat-1.2.0/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1623 2023-07-02 15:21:56.000000 unbelievaboat-1.2.0/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1320 2023-07-02 15:27:56.000000 unbelievaboat-1.2.0/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1487 2023-07-02 15:27:17.000000 unbelievaboat-1.2.0/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.2.0/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:27:20.144621 unbelievaboat-1.2.0/unbelievaboat/util/
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.2.0/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.2.0/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.2.0/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:27:20.117898 unbelievaboat-1.2.0/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3940 2023-07-07 13:27:19.000000 unbelievaboat-1.2.0/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-07-07 13:27:20.000000 unbelievaboat-1.2.0/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:27:19.000000 unbelievaboat-1.2.0/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-07 13:27:19.000000 unbelievaboat-1.2.0/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 13:27:19.000000 unbelievaboat-1.2.0/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 14:03:53.321267 unbelievaboat-1.2.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3940 2023-07-07 14:03:53.321267 unbelievaboat-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3199 2023-07-06 17:33:53.000000 unbelievaboat-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:03:53.322274 unbelievaboat-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-07 14:00:36.000000 unbelievaboat-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:03:53.284640 unbelievaboat-1.2.1/unbelievaboat/
+-rw-rw-rw-   0        0        0     8661 2023-07-07 14:03:38.000000 unbelievaboat-1.2.1/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3987 2023-07-07 12:24:42.000000 unbelievaboat-1.2.1/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.2.1/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:03:53.298662 unbelievaboat-1.2.1/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.2.1/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.2.1/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.2.1/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:03:53.307576 unbelievaboat-1.2.1/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.2.1/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      766 2023-07-07 13:57:39.000000 unbelievaboat-1.2.1/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.2.1/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      711 2023-07-07 14:00:21.000000 unbelievaboat-1.2.1/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1532 2023-07-07 13:25:58.000000 unbelievaboat-1.2.1/unbelievaboat/structures/UserBalance.py
+-rw-rw-rw-   0        0        0     2343 2023-07-07 14:00:16.000000 unbelievaboat-1.2.1/unbelievaboat/structures/UserInventory.py
+-rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.2.1/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:03:53.316211 unbelievaboat-1.2.1/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1322 2023-07-02 15:20:48.000000 unbelievaboat-1.2.1/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0     1169 2023-07-02 15:20:05.000000 unbelievaboat-1.2.1/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1623 2023-07-02 15:21:56.000000 unbelievaboat-1.2.1/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1320 2023-07-02 15:27:56.000000 unbelievaboat-1.2.1/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1487 2023-07-02 15:27:17.000000 unbelievaboat-1.2.1/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.2.1/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:03:53.319234 unbelievaboat-1.2.1/unbelievaboat/util/
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.2.1/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.2.1/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.2.1/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:03:53.295153 unbelievaboat-1.2.1/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3940 2023-07-07 14:03:53.000000 unbelievaboat-1.2.1/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-07-07 14:03:53.000000 unbelievaboat-1.2.1/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:03:53.000000 unbelievaboat-1.2.1/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-07 14:03:53.000000 unbelievaboat-1.2.1/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 14:03:53.000000 unbelievaboat-1.2.1/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.2.0/LICENSE` & `unbelievaboat-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/PKG-INFO` & `unbelievaboat-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.2.0
+Version: 1.2.1
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.2.0/README.md` & `unbelievaboat-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/setup.py` & `unbelievaboat-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.2.0",
+    version="1.2.1",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.2.0/unbelievaboat/Client.py` & `unbelievaboat-1.2.1/unbelievaboat/Client.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,27 +94,37 @@
     async def get_guild_leaderboard(
         self, guild_id: int, params: Dict[str, Any] = {}
     ) -> Leaderboard:
         endpoint: str = f"guilds/{guild_id}/users"
         response: Dict[str, Any] = await self._request_handler.request(
             "GET", endpoint, params=params
         )
-        
+
         data: Dict[str, Any] = {
             "guild_id": guild_id,
         }
-        
+
         if isinstance(response, list):
             data["users"] = response
         else:
-            data.update(**{            "users": response.get("users", []),
-            "page": params.get("page", 1),
-            "total_pages": response.get("total_pages", 1)})
+            data.update(
+                **{
+                    "users": response.get("users", []),
+                    "page": params.get("page", 1),
+                    "total_pages": response.get("total_pages", 1),
+                }
+            )
         return Leaderboard(self, data)
 
+    async def get_guild_leaderboard_all(
+        self, guild_id: int, params: Dict[str, Any] = {}
+    ) -> Leaderboard:
+        params["limit"] = 2147483647
+        return await self.get_guild_leaderboard(guild_id, params)
+
     async def get_guild(self, guild_id: int) -> Guild:
         endpoint: str = f"guilds/{guild_id}"
         response: Dict[str, Any] = await self._request_handler.request("GET", endpoint)
         return Guild(response)
 
     async def get_application_permission(self, guild_id: int) -> Permission:
         endpoint: str = f"applications/@me/guilds/{guild_id}"
@@ -127,14 +137,20 @@
         endpoint: str = f"guilds/{guild_id}/items"
         response: Dict[str, Any] = await self._request_handler.request(
             "GET", endpoint, params=params
         )
         response["guild_id"] = guild_id
         return Store(self, response)
 
+    async def get_store_items_all(
+        self, guild_id: int, params: Dict[str, Any] = {}
+    ) -> Store:
+        params["limit"] = 2147483647
+        return await self.get_store_items(guild_id, params)
+
     async def get_store_item(self, guild_id: int, item_id: int) -> StoreItem:
         endpoint: str = f"guilds/{guild_id}/items/{item_id}"
         response: Dict[str, Any] = await self._request_handler.request("GET", endpoint)
         response["guild_id"] = guild_id
         return StoreItem(self, response)
 
     async def edit_store_item(
@@ -169,14 +185,20 @@
         response: Dict[str, Any] = await self._request_handler.request(
             "GET", endpoint, params=params
         )
         response["guild_id"] = guild_id
         response["user_id"] = user_id
         return UserInventory(self, response)
 
+    async def get_inventory_items_all(
+        self, guild_id: int, user_id: int, params: Dict[str, Any] = {}
+    ) -> UserInventory:
+        params["limit"] = 2147483647
+        return await self.get_inventory_items(guild_id, user_id, params)
+
     async def get_inventory_item(
         self, guild_id: int, user_id: int, item_id: int
     ) -> InventoryItem:
         endpoint: str = f"guilds/{guild_id}/users/{user_id}/inventory/{item_id}"
         response: Dict[str, Any] = await self._request_handler.request("GET", endpoint)
         response["guild_id"] = guild_id
         response["user_id"] = user_id
```

### Comparing `unbelievaboat-1.2.0/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.2.1/unbelievaboat/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.2.1/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/Store.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/UserBalance.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/UserBalance.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/UserInventory.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/UserInventory.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         self.guild_id: str = data.get("guild_id")
         self.items: List[InventoryItem] = [
             InventoryItem(
                 client, {**item, "guild_id": self.guild_id, "user_id": self.user_id}
             )
             for item in data.get("items", [])
         ]
-        self.total_pages: Optional[int] = data.get("total_pages")
-        self.page: Optional[int] = data.get("page")
+        self.total_pages: int = data.get("total_pages", 1)
+        self.page: int = data.get("page", 1)
 
         self._client = client
 
     def __str__(self) -> str:
         return "<UserInventory guild_id={} items={} total_pages={} page={}>".format(
             self.guild_id,
             [str(item) for item in self.items],
```

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/items/InventoryItem.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/items/InventoryItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.2.1/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.2.1/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.2.0/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.2.1/unbelievaboat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.2.0
+Version: 1.2.1
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.2.0/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.2.1/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

