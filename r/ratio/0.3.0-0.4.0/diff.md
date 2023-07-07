# Comparing `tmp/ratio-0.3.0.tar.gz` & `tmp/ratio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratio-0.3.0.tar", max compression
+gzip compressed data, was "ratio-0.4.0.tar", max compression
```

## Comparing `ratio-0.3.0.tar` & `ratio-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,74 @@
--rw-r--r--   0        0        0     1069 2023-01-11 12:56:40.363445 ratio-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     2212 2023-01-17 15:27:32.679191 ratio-0.3.0/README.md
--rw-r--r--   0        0        0     1682 2023-01-17 17:45:02.486322 ratio-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-14 13:32:53.995281 ratio-0.3.0/ratio/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 15:51:49.151042 ratio-0.3.0/ratio/application/__init__.py
--rw-r--r--   0        0        0     1547 2023-01-17 17:42:50.506181 ratio-0.3.0/ratio/application/application.py
--rw-r--r--   0        0        0     1269 2023-01-17 15:27:32.679411 ratio-0.3.0/ratio/application/discover_routes.py
--rw-r--r--   0        0        0      504 2023-01-17 15:27:32.679551 ratio-0.3.0/ratio/application/load_local_module.py
--rw-r--r--   0        0        0        0 2022-12-14 13:39:18.774501 ratio-0.3.0/ratio/database/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 14:18:24.938150 ratio-0.3.0/ratio/database/fields/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 13:39:56.925867 ratio-0.3.0/ratio/database/migrations/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 14:18:09.774439 ratio-0.3.0/ratio/database/models/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 13:40:02.365051 ratio-0.3.0/ratio/database/seeders/__init__.py
--rw-r--r--   0        0        0        0 2022-12-15 08:17:37.128086 ratio-0.3.0/ratio/http/__init__.py
--rw-r--r--   0        0        0      123 2022-12-19 12:05:06.045470 ratio-0.3.0/ratio/http/parameters.py
--rw-r--r--   0        0        0     1692 2023-01-17 15:27:32.679869 ratio-0.3.0/ratio/http/request.py
--rw-r--r--   0        0        0     2061 2023-01-17 17:42:50.506357 ratio-0.3.0/ratio/http/response.py
--rw-r--r--   0        0        0        0 2022-12-14 23:23:50.494736 ratio-0.3.0/ratio/router/__init__.py
--rw-r--r--   0        0        0      448 2022-12-19 22:51:28.652314 ratio-0.3.0/ratio/router/exceptions.py
--rw-r--r--   0        0        0      281 2023-01-17 15:27:32.680220 ratio-0.3.0/ratio/router/is_route.py
--rw-r--r--   0        0        0      369 2023-01-17 17:42:50.506488 ratio-0.3.0/ratio/router/redirect.py
--rw-r--r--   0        0        0        0 2022-12-20 18:53:20.080531 ratio-0.3.0/ratio/router/resolvers/__init__.py
--rw-r--r--   0        0        0     1522 2023-01-17 15:27:32.680547 ratio-0.3.0/ratio/router/resolvers/direct_resolver.py
--rw-r--r--   0        0        0     2205 2023-01-17 15:27:32.680908 ratio-0.3.0/ratio/router/resolvers/dynamic_resolver.py
--rw-r--r--   0        0        0      574 2023-01-09 22:22:09.700343 ratio-0.3.0/ratio/router/resolvers/generic_routes.py
--rw-r--r--   0        0        0      632 2023-01-09 22:23:07.179935 ratio-0.3.0/ratio/router/resolvers/resolver.py
--rw-r--r--   0        0        0      382 2023-01-16 14:11:13.895598 ratio-0.3.0/ratio/router/resolvers/util.py
--rw-r--r--   0        0        0     1395 2023-01-09 22:47:15.609383 ratio-0.3.0/ratio/router/route.py
--rw-r--r--   0        0        0     3994 2023-01-17 15:27:32.681253 ratio-0.3.0/ratio/router/route_path.py
--rw-r--r--   0        0        0       93 2022-12-22 11:07:32.453324 ratio-0.3.0/ratio/router/route_type.py
--rw-r--r--   0        0        0     1753 2023-01-12 15:28:01.966443 ratio-0.3.0/ratio/router/router.py
--rw-r--r--   0        0        0        0 2023-01-16 14:20:21.332091 ratio-0.3.0/ratio/util/__init__.py
--rw-r--r--   0        0        0      261 2023-01-16 14:20:21.332354 ratio-0.3.0/ratio/util/remove_none.py
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 ratio-0.3.0/setup.py
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 ratio-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-01-11 12:56:40.363445 ratio-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2212 2023-01-17 15:27:32.679191 ratio-0.4.0/README.md
+-rw-r--r--   0        0        0     1513 2023-07-07 14:35:21.784621 ratio-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-14 13:32:53.995281 ratio-0.4.0/ratio/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-12 15:51:49.151042 ratio-0.4.0/ratio/application/__init__.py
+-rw-r--r--   0        0        0      168 2023-01-12 16:00:57.802374 ratio-0.4.0/ratio/application/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2604 2023-01-27 17:28:11.759046 ratio-0.4.0/ratio/application/__pycache__/application.cpython-311.pyc
+-rw-r--r--   0        0        0     3004 2023-07-07 14:27:09.283377 ratio-0.4.0/ratio/application/__pycache__/discover_routes.cpython-311.pyc
+-rw-r--r--   0        0        0     1079 2023-01-17 15:37:48.494175 ratio-0.4.0/ratio/application/__pycache__/load_local_module.cpython-311.pyc
+-rw-r--r--   0        0        0     1563 2023-01-27 17:27:04.566661 ratio-0.4.0/ratio/application/application.py
+-rw-r--r--   0        0        0     1265 2023-07-07 14:32:39.374107 ratio-0.4.0/ratio/application/discover_routes.py
+-rw-r--r--   0        0        0      504 2023-01-17 15:27:32.679551 ratio-0.4.0/ratio/application/load_local_module.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:26:19.621309 ratio-0.4.0/ratio/authentication/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-07 14:27:09.285205 ratio-0.4.0/ratio/authentication/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3267 2023-07-07 14:27:09.285938 ratio-0.4.0/ratio/authentication/__pycache__/basic_authentication.cpython-311.pyc
+-rw-r--r--   0        0        0     1833 2023-07-07 09:26:19.621827 ratio-0.4.0/ratio/authentication/basic_authentication.py
+-rw-r--r--   0        0        0      164 2022-12-15 11:48:38.879022 ratio-0.4.0/ratio/console/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      675 2022-12-15 12:12:40.212235 ratio-0.4.0/ratio/console/__pycache__/_create_rich_console.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2022-12-14 13:39:18.774501 ratio-0.4.0/ratio/database/__init__.py
+-rw-r--r--   0        0        0      165 2022-12-14 23:33:58.428995 ratio-0.4.0/ratio/database/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2022-12-14 14:18:24.938150 ratio-0.4.0/ratio/database/fields/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-14 13:39:56.925867 ratio-0.4.0/ratio/database/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-14 14:18:09.774439 ratio-0.4.0/ratio/database/models/__init__.py
+-rw-r--r--   0        0        0      172 2022-12-15 08:12:18.657110 ratio-0.4.0/ratio/database/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      648 2022-12-15 08:12:18.657377 ratio-0.4.0/ratio/database/models/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2022-12-14 13:40:02.365051 ratio-0.4.0/ratio/database/seeders/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-15 08:17:37.128086 ratio-0.4.0/ratio/http/__init__.py
+-rw-r--r--   0        0        0      161 2022-12-15 18:52:23.846463 ratio-0.4.0/ratio/http/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5546 2023-07-07 14:27:09.276107 ratio-0.4.0/ratio/http/__pycache__/headers.cpython-311.pyc
+-rw-r--r--   0        0        0      620 2022-12-19 12:38:48.677400 ratio-0.4.0/ratio/http/__pycache__/parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     5169 2023-07-07 14:27:09.277439 ratio-0.4.0/ratio/http/__pycache__/request.cpython-311.pyc
+-rw-r--r--   0        0        0     2717 2023-07-07 14:27:09.274778 ratio-0.4.0/ratio/http/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0        0        0     2089 2023-07-07 14:32:39.374388 ratio-0.4.0/ratio/http/headers.py
+-rw-r--r--   0        0        0      123 2022-12-19 12:05:06.045470 ratio-0.4.0/ratio/http/parameters.py
+-rw-r--r--   0        0        0     2150 2023-07-07 09:26:19.622534 ratio-0.4.0/ratio/http/request.py
+-rw-r--r--   0        0        0     1231 2023-07-07 14:32:39.374616 ratio-0.4.0/ratio/http/response.py
+-rw-r--r--   0        0        0        0 2022-12-14 23:23:50.494736 ratio-0.4.0/ratio/router/__init__.py
+-rw-r--r--   0        0        0      163 2022-12-15 12:24:03.997719 ratio-0.4.0/ratio/router/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1321 2022-12-19 22:52:04.087484 ratio-0.4.0/ratio/router/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0      787 2023-01-17 15:37:48.494549 ratio-0.4.0/ratio/router/__pycache__/is_route.cpython-311.pyc
+-rw-r--r--   0        0        0     1351 2023-01-27 21:29:19.231865 ratio-0.4.0/ratio/router/__pycache__/redirect.cpython-311.pyc
+-rw-r--r--   0        0        0     2912 2023-07-07 14:27:09.273882 ratio-0.4.0/ratio/router/__pycache__/route.cpython-311.pyc
+-rw-r--r--   0        0        0     5751 2023-07-07 14:27:09.280315 ratio-0.4.0/ratio/router/__pycache__/route_path.cpython-311.pyc
+-rw-r--r--   0        0        0      486 2022-12-22 11:37:23.690170 ratio-0.4.0/ratio/router/__pycache__/route_type.cpython-311.pyc
+-rw-r--r--   0        0        0     2638 2023-01-12 16:00:57.804487 ratio-0.4.0/ratio/router/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0      448 2022-12-19 22:51:28.652314 ratio-0.4.0/ratio/router/exceptions.py
+-rw-r--r--   0        0        0      281 2023-01-17 15:27:32.680220 ratio-0.4.0/ratio/router/is_route.py
+-rw-r--r--   0        0        0      757 2023-07-07 14:32:39.374832 ratio-0.4.0/ratio/router/redirect.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:53:20.080531 ratio-0.4.0/ratio/router/resolvers/__init__.py
+-rw-r--r--   0        0        0      173 2022-12-20 18:57:54.440786 ratio-0.4.0/ratio/router/resolvers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2677 2023-01-17 15:37:48.482483 ratio-0.4.0/ratio/router/resolvers/__pycache__/direct_resolver.cpython-311.pyc
+-rw-r--r--   0        0        0     4118 2023-01-17 15:37:48.475145 ratio-0.4.0/ratio/router/resolvers/__pycache__/dynamic_resolver.cpython-311.pyc
+-rw-r--r--   0        0        0     1240 2023-01-09 22:43:10.227968 ratio-0.4.0/ratio/router/resolvers/__pycache__/generic_routes.cpython-311.pyc
+-rw-r--r--   0        0        0     1726 2023-01-20 15:32:12.371829 ratio-0.4.0/ratio/router/resolvers/__pycache__/resolver.cpython-311.pyc
+-rw-r--r--   0        0        0      978 2023-07-07 14:27:09.282003 ratio-0.4.0/ratio/router/resolvers/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0     1522 2023-01-17 15:27:32.680547 ratio-0.4.0/ratio/router/resolvers/direct_resolver.py
+-rw-r--r--   0        0        0     2205 2023-01-17 15:27:32.680908 ratio-0.4.0/ratio/router/resolvers/dynamic_resolver.py
+-rw-r--r--   0        0        0      574 2023-01-09 22:22:09.700343 ratio-0.4.0/ratio/router/resolvers/generic_routes.py
+-rw-r--r--   0        0        0      632 2023-01-18 21:41:14.746247 ratio-0.4.0/ratio/router/resolvers/resolver.py
+-rw-r--r--   0        0        0      398 2023-07-07 09:26:19.622829 ratio-0.4.0/ratio/router/resolvers/util.py
+-rw-r--r--   0        0        0     1487 2023-07-07 14:32:39.375062 ratio-0.4.0/ratio/router/route.py
+-rw-r--r--   0        0        0     4082 2023-07-07 14:32:39.375319 ratio-0.4.0/ratio/router/route_path.py
+-rw-r--r--   0        0        0       93 2022-12-22 11:07:32.453324 ratio-0.4.0/ratio/router/route_type.py
+-rw-r--r--   0        0        0     1753 2023-01-12 15:28:01.966443 ratio-0.4.0/ratio/router/router.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:20:21.332091 ratio-0.4.0/ratio/util/__init__.py
+-rw-r--r--   0        0        0      161 2023-01-16 14:21:44.927758 ratio-0.4.0/ratio/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      830 2023-01-16 14:21:44.928087 ratio-0.4.0/ratio/util/__pycache__/remove_none.cpython-311.pyc
+-rw-r--r--   0        0        0      261 2023-01-16 14:20:21.332354 ratio-0.4.0/ratio/util/remove_none.py
+-rw-r--r--   0        0        0      162 2023-01-17 22:27:56.720204 ratio-0.4.0/ratio/views/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1322 2023-01-17 23:07:02.591576 ratio-0.4.0/ratio/views/__pycache__/json_view.cpython-311.pyc
+-rw-r--r--   0        0        0     1080 2023-01-17 23:07:02.588822 ratio-0.4.0/ratio/views/__pycache__/simple_view.cpython-311.pyc
+-rw-r--r--   0        0        0      729 2023-01-17 23:07:02.588470 ratio-0.4.0/ratio/views/__pycache__/view.cpython-311.pyc
+-rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 ratio-0.4.0/setup.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 ratio-0.4.0/PKG-INFO
```

### Comparing `ratio-0.3.0/LICENSE.md` & `ratio-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ratio-0.3.0/README.md` & `ratio-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ratio-0.3.0/pyproject.toml` & `ratio-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "ratio"
-version = "0.3.0"
+version = "0.4.0"
 description = "The Python Web Framework for developers who like to get shit done"
 authors = ["Job Veldhuis <job@baukefrederik.me>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rich = "^12.6.0"
 
-
 [tool.poetry.group.dev.dependencies]
-black = {extras = ["d"], version = "^22.12.0"}
-pytest = "^7.2.0"
-pytest-asyncio = "^0.20.3"
-coverage = "^6.5.0"
+black = "^23.3.0"
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.0"
+coverage = "^7.2.7"
 asgiref = "^3.5.2"
-ruff = "^0.0.186"
-mypy = "^0.991"
-setuptools = "^65.6.3"
+ruff = "^0.0.277"
+mypy = "^1.4.1"
+setuptools = "^68.0.0"
 
 [tool.poetry.group.tmp.dependencies]
 uvicorn = "^0.20.0"
 
 [tool.pytest.ini_options]
 asyncio_mode="auto"
 
@@ -43,14 +42,15 @@
     "PLR",
     "PLW",
     "RUF"
 ]
 ignore = [
     "E501",     # Reason: the line length is checked and automatically formatted by Black
     "RET502",   # Reason: the return type is already enforced by Mypy type checking
+    "E999"      # Reason: syntax errors should already be caught by IDE, mypy and unit tests
 ]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
@@ -69,22 +69,11 @@
     "node_modules",
     "venv",
 ]
 per-file-ignores = {}
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 target-version = "py311"
 
-[tool.mypy]
-python_version = "3.11"
-disallow_untyped_defs = true
-disallow_incomplete_defs = true
-disallow_any_unimported = true
-show_error_codes = true
-no_implicit_optional = true
-warn_return_any = true
-warn_unused_ignores = true
-
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ratio-0.3.0/ratio/application/application.py` & `ratio-0.4.0/ratio/application/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 
 class Ratio:
     application_root: pathlib.Path
     router: Router
 
-    def __init__(self, root: pathlib.Path | None):
+    def __init__(self, root: pathlib.Path | None = None):
         self.application_root = root if root is not None else pathlib.Path.cwd()
 
         routes = discover_routes(self.application_root)
         self.router = Router(routes)
 
     async def __call__(
         self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
@@ -34,15 +34,15 @@
         request = Request.from_http_scope(scope)
         route = await self.router.resolve(request)
         response = await route()
 
         start: HTTPResponseStartEvent = {
             "type": "http.response.start",
             "status": response.code,
-            "headers": response.headers,
+            "headers": response.headers.encode(),
             "trailers": False,
         }
 
         await send(start)
 
         body: HTTPResponseBodyEvent = {
             "type": "http.response.body",
```

### Comparing `ratio-0.3.0/ratio/application/discover_routes.py` & `ratio-0.4.0/ratio/application/discover_routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     module = load_local_module("route", resolved_path)
     module_attributes = [getattr(module, item) for item in dir(module)]
     potential_routes = [
         attribute for attribute in module_attributes if is_route(attribute)
     ]
 
-    if not len(potential_routes) == 1:
+    if len(potential_routes) != 1:
         return None
 
     return potential_routes[0]
 
 
 def discover_routes(
     application_root: pathlib.Path,
```

### Comparing `ratio-0.3.0/ratio/http/request.py` & `ratio-0.4.0/ratio/http/request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 from ratio.http.parameters import Parameters
+from ratio.http.headers import Headers
 import urllib.parse
 from asgiref.typing import HTTPScope
-from typing import Self
+from typing import Iterable, TypedDict, NotRequired
+
+
+class RequestData(TypedDict):
+    method: str
+    url: str
+    headers: NotRequired[Iterable[tuple[str, str]]]
 
 
 class Request:
     method: str
     url: str
     body: list[str]
     cookies: dict[str, str]
+    headers: Headers
     fresh: bool
     path_parameters: dict[str, str]
 
     __parsed_url: urllib.parse.ParseResult
 
-    def __init__(self, method: str, url: str) -> None:
-        self.__parsed_url = urllib.parse.urlparse(url)
-        self.method = method
+    def __init__(self, data: RequestData) -> None:
+        self.__parsed_url = urllib.parse.urlparse(data["url"])
+        self.method = data["method"]
         self.path_parameters = {}
+        self.headers = Headers()
+
+        for header in data.get("headers", []):
+            self.headers.add(header[0], header[1])
 
     @property
     def url_hostname(self) -> str | None:
         return self.__parsed_url.hostname
 
     @property
     def url_port(self) -> int | None:
@@ -51,11 +63,18 @@
             for (key, value) in parsed_query_parameters.items()
         }
 
     @property
     def parameters(self) -> Parameters:
         return {"query": self.query_parameters, "path": self.path_parameters}
 
-    # Reason for ignoring type: Self is actually valid. In new version of Mypy this will be supported.
     @classmethod
-    def from_http_scope(cls, scope: HTTPScope) -> Self:  # type: ignore
-        return cls(scope["method"], scope["path"])
+    def from_http_scope(cls, scope: HTTPScope) -> "Request":
+        return cls(
+            {
+                "method": scope["method"],
+                "url": scope["path"],
+                "headers": map(
+                    lambda item: (item[0].decode(), item[1].decode()), scope["headers"]
+                ),
+            }
+        )
```

### Comparing `ratio-0.3.0/ratio/router/resolvers/direct_resolver.py` & `ratio-0.4.0/ratio/router/resolvers/direct_resolver.py`

 * *Files identical despite different names*

### Comparing `ratio-0.3.0/ratio/router/resolvers/dynamic_resolver.py` & `ratio-0.4.0/ratio/router/resolvers/dynamic_resolver.py`

 * *Files identical despite different names*

### Comparing `ratio-0.3.0/ratio/router/resolvers/generic_routes.py` & `ratio-0.4.0/ratio/router/resolvers/generic_routes.py`

 * *Files identical despite different names*

### Comparing `ratio-0.3.0/ratio/router/resolvers/resolver.py` & `ratio-0.4.0/ratio/router/resolvers/resolver.py`

 * *Files identical despite different names*

### Comparing `ratio-0.3.0/ratio/router/route.py` & `ratio-0.4.0/ratio/router/route.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from ratio.http.response import Response
 from ratio.http.request import Request
-from typing import Awaitable, Callable
+from typing import Awaitable, Callable, TypeVar
 from http import HTTPStatus
 
-RouteMethod = Callable[[Request], Awaitable[Response]]
+_T = TypeVar("_T")
+RouteMethod = Callable[[_T, Request], Awaitable[Response]]
+BoundRouteMethod = Callable[[Request], Awaitable[Response]]
 
 
 class Route:
     async def get(self, _request: Request) -> Response:
         return Response.from_http_status(HTTPStatus.METHOD_NOT_ALLOWED)
 
     async def head(self, _request: Request) -> Response:
```

### Comparing `ratio-0.3.0/ratio/router/route_path.py` & `ratio-0.4.0/ratio/router/route_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from ratio.router.route_type import RouteType
 from ratio.router.exceptions import InvalidRouteError
 import re
 import pathlib
-from typing import Self
 
 ROUTE_ALLOWED_CHARACTERS = r"^[A-Za-z0-9_\/\[\]]+$"
 DIRECT_ROUTE_ALLOWED_CHARACTERS = r"^[A-Za-z0-9_\/]+$"
 DYNAMIC_ROUTE_KEY_ALLOWED_CHARACTERS = r"[A-Za-z0-9_]+"
 DYNAMIC_PATH_PARAMETER_REGEX = r"\[([A-Za-z0-9_]+?)]"
 INVALID_DYNAMIC_PARAMETER_REGEX = r"(.*?)\[([^A-Za-z0-9_]+)](.*?)$"
 
+# The minimum amount of slashes needed for a nested route
+# e.g. /test/ is not nested, while /test/something/ is
+MINIMUM_SEPARATORS_FOR_NESTED_ROUTE = 3
+
 
 class RoutePath:
     __path: str
 
     def __init__(self, path: str):
         if path == "/":
             path = "/index"
         self.__path = path
         self.assert_is_valid()
 
     def __str__(self) -> str:
         return self.__path
 
-    # Reason for ignoring type: Self is actually valid. In new version of Mypy this will be supported.
     @classmethod
-    def from_path(cls, path: pathlib.Path) -> Self:  # type: ignore
+    def from_path(cls, path: pathlib.Path) -> "RoutePath":
         return cls("/" + str(path))
 
     @property
     def route_type(self) -> RouteType:
         if len(self.parameter_keys) == 0:
             return RouteType.DIRECT
 
@@ -74,15 +76,18 @@
             is None
         ):
             raise InvalidRouteError(
                 "Some parameters are specified incorrectly. Make sure you close your brackets appropriately."
             )
 
         # For intuitive custom error routes to work, we cannot have `/[id]` as route.
-        if len(self.parameter_keys) == 1 and len(self.__path.split("/")) < 3:
+        if (
+            len(self.parameter_keys) == 1
+            and len(self.__path.split("/")) < MINIMUM_SEPARATORS_FOR_NESTED_ROUTE
+        ):
             raise InvalidRouteError("Top-level dynamic routes are not allowed.")
 
     @property
     def parameter_keys(self) -> list[str]:
         return re.findall(DYNAMIC_PATH_PARAMETER_REGEX, self.__path)
 
     def as_simple_regex(self) -> str:
```

### Comparing `ratio-0.3.0/ratio/router/router.py` & `ratio-0.4.0/ratio/router/router.py`

 * *Files identical despite different names*

### Comparing `ratio-0.3.0/setup.py` & `ratio-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['ratio',
  'ratio.application',
+ 'ratio.authentication',
  'ratio.database',
  'ratio.database.fields',
  'ratio.database.migrations',
  'ratio.database.models',
  'ratio.database.seeders',
  'ratio.http',
  'ratio.router',
@@ -18,15 +19,15 @@
 {'': ['*']}
 
 install_requires = \
 ['rich>=12.6.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'ratio',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'The Python Web Framework for developers who like to get shit done',
     'long_description': '<h1 align="center">Ratio</h1>\n<p align="center">\n  The Python web framework for developers who want to get shit done.\n</p>\n\n---\n\n**Ratio is currently being developed and all releases in this phase may introduce breaking changes until further notice.\nPlease do not use Ratio in production without carefully considering the consequences.**\n\n---\n\n## What is Ratio?\nRatio is an asynchronous Python web framework that was built with developer experience in mind. Quick to learn for those\nwho just start out with programming and powerful so that senior developers can build high performance web applications \nwith it. The framework is designed with the Goldilocks principle in mind: just enough. Enough power to run high performance\nweb applications, enough intuitive design, so that developers can easily pick up on the principles.\n\nRatio borrows ideas from great frameworks, like [Django](https://github.com/django/django), [FastAPI](https://github.com/tiangolo/fastapi)\nand [Next.js](https://github.com/vercel/next.js). It combines those ideas with original concepts to improve the life of \na developer when building web applications for any purpose.\n\n## Ready out of the box \nRatio will be shipped with a custom and extensible command line interface, which can be used to perform actions within a\nproject.\n  \nThis is what we aim Ratio to do:\n\n- **File based routing:** Intuitive routing for each incoming request, based on file system.\n- **Integrates with databases:** Connect to SQL or SQLite databases from within the application controllers.\n- **Write once, use everywhere:** Do not repeat yourself, by defining models, routes and actions you can use them throughout the application.\n- **Adheres to standards:** API views are based on [OpenAPI]() and the [JSON schema standard]().\n\n_This list is not complete and will be extended after certain releases in the pre-release phase._\n\n\n## Minimal external dependencies\nCurrently, Ratio only requires the `rich` package from outside the Python standard library, which is used \nfor rendering beautiful output to the command line. In a future version of Ratio, we might want to remove this direct\ndependency for users who really want to have no external dependencies.\n',
     'author': 'Job Veldhuis',
     'author_email': 'job@baukefrederik.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ratio-0.3.0/PKG-INFO` & `ratio-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratio
-Version: 0.3.0
+Version: 0.4.0
 Summary: The Python Web Framework for developers who like to get shit done
 Author: Job Veldhuis
 Author-email: job@baukefrederik.me
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rich (>=12.6.0,<13.0.0)
```

