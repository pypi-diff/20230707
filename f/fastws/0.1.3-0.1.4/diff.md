# Comparing `tmp/fastws-0.1.3.tar.gz` & `tmp/fastws-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastws-0.1.3.tar", max compression
+gzip compressed data, was "fastws-0.1.4.tar", max compression
```

## Comparing `fastws-0.1.3.tar` & `fastws-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-07-06 20:53:23.287732 fastws-0.1.3/LICENSE
--rw-r--r--   0        0        0    10110 2023-07-06 21:06:54.397590 fastws-0.1.3/README.md
--rw-r--r--   0        0        0      437 2023-07-06 21:07:37.737582 fastws-0.1.3/fastws/__init__.py
--rw-r--r--   0        0        0     6903 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/application.py
--rw-r--r--   0        0        0     1552 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/asyncapi.py
--rw-r--r--   0        0        0     4346 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/broker.py
--rw-r--r--   0        0        0     6172 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/docs.py
--rw-r--r--   0        0        0     6183 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/routing.py
--rw-r--r--   0        0        0     1231 2023-07-06 21:07:37.597582 fastws-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    11228 1970-01-01 00:00:00.000000 fastws-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 20:53:23.287732 fastws-0.1.4/LICENSE
+-rw-r--r--   0        0        0    10110 2023-07-06 21:06:54.397590 fastws-0.1.4/README.md
+-rw-r--r--   0        0        0      437 2023-07-06 21:50:32.707124 fastws-0.1.4/fastws/__init__.py
+-rw-r--r--   0        0        0     6890 2023-07-06 21:51:49.747110 fastws-0.1.4/fastws/application.py
+-rw-r--r--   0        0        0     1566 2023-07-06 21:48:56.247142 fastws-0.1.4/fastws/asyncapi.py
+-rw-r--r--   0        0        0     4346 2023-07-06 21:52:03.487107 fastws-0.1.4/fastws/broker.py
+-rw-r--r--   0        0        0     6160 2023-07-06 21:49:29.897135 fastws-0.1.4/fastws/docs.py
+-rw-r--r--   0        0        0     6183 2023-07-06 20:53:23.287732 fastws-0.1.4/fastws/routing.py
+-rw-r--r--   0        0        0     1231 2023-07-06 21:50:32.547124 fastws-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    11228 1970-01-01 00:00:00.000000 fastws-0.1.4/PKG-INFO
```

### Comparing `fastws-0.1.3/LICENSE` & `fastws-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastws-0.1.3/README.md` & `fastws-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fastws-0.1.3/fastws/application.py` & `fastws-0.1.4/fastws/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             yield Message.model_validate_json(message)
 
 
 class FastWS(Broker):
     def __init__(
         self,
         *,
-        title: str = "Event Driven Broker",
-        version: str = "1.0.0",
+        title: str = "FastWS",
+        version: str = "0.0.1",
         asyncapi_version: str = "2.4.0",
         description: str | None = None,
         terms_of_service: str | None = None,
         contact: dict[str, str] | None = None,
         license_info: dict[str, str] | None = None,
         servers: dict | None = None,
         asyncapi_url: str | None = "/asyncapi.json",
```

### Comparing `fastws-0.1.3/fastws/asyncapi.py` & `fastws-0.1.4/fastws/asyncapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     name: str | Enum
 
 
 class Message(BaseModel):
     messageId: str
     name: str
     title: str
-    summary: str
+    summary: str | None = None
     description: str
     contentType: str = "application/json"
     payload: dict | None = None
     tags: list[Tag] | None = None
     examples: list[dict] | None = None
```

### Comparing `fastws-0.1.3/fastws/broker.py` & `fastws-0.1.4/fastws/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return handler(**values)
 
 
 class Broker:
     def __init__(
         self,
         title: str = "Event Driven Broker",
-        version: str = "1.0.0",
+        version: str = "0.0.1",
         asyncapi_version: str = "2.4.0",
         description: str | None = None,
         terms_of_service: str | None = None,
         contact: dict[str, str] | None = None,
         license_info: dict[str, str] | None = None,
         servers: dict | None = None,
     ) -> None:
```

### Comparing `fastws-0.1.3/fastws/docs.py` & `fastws-0.1.4/fastws/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     messages = {}
     sub_messages = []
     pub_messages = []
 
     for route in routes:
         msg = asyncapi.Message(
             messageId=route.operation,
-            name=route.operation,
-            title=" ".join(route.operation.split("_")).title(),
-            summary=route.operation,
+            name=route.name,
+            title=" ".join(route.name.split("_")).title(),
+            summary=route.summary,
             description=route.description,
             tags=[asyncapi.Tag(name=t) for t in route.tags],
         )
         if route.method == "SEND":
             key = route.operation
             pub_messages.append(key)
             messages[key] = msg.model_copy(
```

### Comparing `fastws-0.1.3/fastws/routing.py` & `fastws-0.1.4/fastws/routing.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.3/pyproject.toml` & `fastws-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastws"
-version = "0.1.3"
+version = "0.1.4"
 description = "FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI."
 authors = ["Endre Krohn <endre@skript.no>"]
 readme = "README.md"
 packages = [{ include = "fastws" }]
 repository = "https://github.com/endrekrohn/fastws"
 documentation = "https://github.com/endrekrohn/fastws"
 keywords = ["fastapi", "pydantic", "starlette", "websockets", "asyncapi"]
```

### Comparing `fastws-0.1.3/PKG-INFO` & `fastws-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastws
-Version: 0.1.3
+Version: 0.1.4
 Summary: FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI.
 Home-page: https://github.com/endrekrohn/fastws
 Keywords: fastapi,pydantic,starlette,websockets,asyncapi
 Author: Endre Krohn
 Author-email: endre@skript.no
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

