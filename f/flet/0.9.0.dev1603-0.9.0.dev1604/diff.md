# Comparing `tmp/flet-0.9.0.dev1603.tar.gz` & `tmp/flet-0.9.0.dev1604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-0.9.0.dev1603.tar", max compression
+gzip compressed data, was "flet-0.9.0.dev1604.tar", max compression
```

## Comparing `flet-0.9.0.dev1603.tar` & `flet-0.9.0.dev1604.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     2145 2023-07-06 01:33:30.014795 flet-0.9.0.dev1603/README.md
--rw-r--r--   0        0        0     1085 2023-07-06 01:34:09.445680 flet-0.9.0.dev1603/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-06 01:33:30.014795 flet-0.9.0.dev1603/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2023-07-06 01:33:30.014795 flet-0.9.0.dev1603/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0       20 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2985 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      570 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3620 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0     7267 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/async_websocket_connection.py
--rw-r--r--   0        0        0       32 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/auth/__init__.py
--rw-r--r--   0        0        0       42 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/auth/providers/__init__.py
--rw-r--r--   0        0        0       31 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     3053 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/cli/cli.py
--rw-r--r--   0        0        0     1953 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0     1989 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/cli/commands/create.py
--rw-r--r--   0        0        0      673 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0     8473 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     9293 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0     9745 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0       52 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/constants.py
--rw-r--r--   0        0        0       55 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3212 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/reconnecting_websocket.py
--rw-r--r--   0        0        0     1272 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/security.py
--rw-r--r--   0        0        0     5461 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/sync_websocket_connection.py
--rw-r--r--   0        0        0      145 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/utils/__init__.py
--rw-r--r--   0        0        0     1469 2023-07-06 01:33:30.018794 flet-0.9.0.dev1603/src/flet/version.py
--rw-r--r--   0        0        0       32 2023-07-06 01:24:45.000000 flet-0.9.0.dev1603/src/flet/web/.last_build_id
--rw-r--r--   0        0        0      484 2023-07-06 01:24:41.000000 flet-0.9.0.dev1603/src/flet/web/assets/AssetManifest.bin
--rw-r--r--   0        0        0      455 2023-07-06 01:24:41.000000 flet-0.9.0.dev1603/src/flet/web/assets/AssetManifest.json
--rw-r--r--   0        0        0       82 2023-07-06 01:24:41.000000 flet-0.9.0.dev1603/src/flet/web/assets/FontManifest.json
--rw-r--r--   0        0        0  1738123 2023-07-06 01:24:41.000000 flet-0.9.0.dev1603/src/flet/web/assets/NOTICES
--rw-r--r--   0        0        0  1261080 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
--rw-r--r--   0        0        0      298 2023-07-06 01:24:40.000000 flet-0.9.0.dev1603/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
--rw-r--r--   0        0        0      271 2023-07-06 01:24:40.000000 flet-0.9.0.dev1603/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
--rw-r--r--   0        0        0      166 2023-07-06 01:24:40.000000 flet-0.9.0.dev1603/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
--rw-r--r--   0        0        0      366 2023-07-06 01:24:40.000000 flet-0.9.0.dev1603/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
--rw-r--r--   0        0        0     9242 2023-07-06 01:24:41.000000 flet-0.9.0.dev1603/src/flet/web/assets/shaders/ink_sparkle.frag
--rw-r--r--   0        0        0     1028 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/favicon.png
--rw-r--r--   0        0        0    14240 2023-07-06 01:23:21.000000 flet-0.9.0.dev1603/src/flet/web/flutter.js
--rw-r--r--   0        0        0     8316 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/flutter_service_worker.js
--rw-r--r--   0        0        0     4699 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/icons/apple-touch-icon-192.png
--rw-r--r--   0        0        0     6622 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/icons/icon-192.png
--rw-r--r--   0        0        0    18666 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/icons/icon-512.png
--rw-r--r--   0        0        0     4128 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    11906 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    17040 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/icons/loading-animation.png
--rw-r--r--   0        0        0     3158 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/index.html
--rw-r--r--   0        0        0  5449285 2023-07-06 01:24:40.000000 flet-0.9.0.dev1603/src/flet/web/main.dart.js
--rw-r--r--   0        0        0      789 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/manifest.json
--rw-r--r--   0        0        0     1573 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/python-worker.js
--rw-r--r--   0        0        0      744 2023-07-06 01:24:44.000000 flet-0.9.0.dev1603/src/flet/web/python.js
--rw-r--r--   0        0        0       92 2023-07-06 01:24:40.000000 flet-0.9.0.dev1603/src/flet/web/version.json
--rw-r--r--   0        0        0     3346 1970-01-01 00:00:00.000000 flet-0.9.0.dev1603/PKG-INFO
+-rw-r--r--   0        0        0     2145 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/README.md
+-rw-r--r--   0        0        0     1085 2023-07-06 16:34:12.508830 flet-0.9.0.dev1604/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0       20 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2985 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      570 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3620 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0     7267 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/async_websocket_connection.py
+-rw-r--r--   0        0        0       32 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/auth/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/auth/providers/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     3053 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     1953 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0     1989 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/cli/commands/create.py
+-rw-r--r--   0        0        0      673 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0     8473 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     9293 2023-07-06 16:33:37.320957 flet-0.9.0.dev1604/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0     9745 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0       52 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/constants.py
+-rw-r--r--   0        0        0       55 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3212 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/reconnecting_websocket.py
+-rw-r--r--   0        0        0     1272 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/security.py
+-rw-r--r--   0        0        0     5461 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/sync_websocket_connection.py
+-rw-r--r--   0        0        0      145 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/utils/__init__.py
+-rw-r--r--   0        0        0     1469 2023-07-06 16:33:37.324957 flet-0.9.0.dev1604/src/flet/version.py
+-rw-r--r--   0        0        0       32 2023-07-06 16:25:12.000000 flet-0.9.0.dev1604/src/flet/web/.last_build_id
+-rw-r--r--   0        0        0      484 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/AssetManifest.bin
+-rw-r--r--   0        0        0      455 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/AssetManifest.json
+-rw-r--r--   0        0        0       82 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/FontManifest.json
+-rw-r--r--   0        0        0  1738123 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/NOTICES
+-rw-r--r--   0        0        0  1261080 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
+-rw-r--r--   0        0        0      298 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
+-rw-r--r--   0        0        0      271 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
+-rw-r--r--   0        0        0      166 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
+-rw-r--r--   0        0        0      366 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
+-rw-r--r--   0        0        0     9242 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/assets/shaders/ink_sparkle.frag
+-rw-r--r--   0        0        0     1028 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/favicon.png
+-rw-r--r--   0        0        0    14240 2023-07-06 16:23:57.000000 flet-0.9.0.dev1604/src/flet/web/flutter.js
+-rw-r--r--   0        0        0     8316 2023-07-06 16:25:12.000000 flet-0.9.0.dev1604/src/flet/web/flutter_service_worker.js
+-rw-r--r--   0        0        0     4699 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/icons/apple-touch-icon-192.png
+-rw-r--r--   0        0        0     6622 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/icons/icon-192.png
+-rw-r--r--   0        0        0    18666 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/icons/icon-512.png
+-rw-r--r--   0        0        0     4128 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    11906 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    17040 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/icons/loading-animation.png
+-rw-r--r--   0        0        0     3158 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/index.html
+-rw-r--r--   0        0        0  5449285 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/main.dart.js
+-rw-r--r--   0        0        0      789 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/manifest.json
+-rw-r--r--   0        0        0     1573 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/python-worker.js
+-rw-r--r--   0        0        0      744 2023-07-06 16:25:11.000000 flet-0.9.0.dev1604/src/flet/web/python.js
+-rw-r--r--   0        0        0       92 2023-07-06 16:25:08.000000 flet-0.9.0.dev1604/src/flet/web/version.json
+-rw-r--r--   0        0        0     3346 1970-01-01 00:00:00.000000 flet-0.9.0.dev1604/PKG-INFO
```

### Comparing `flet-0.9.0.dev1603/README.md` & `flet-0.9.0.dev1604/README.md`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/pyproject.toml` & `flet-0.9.0.dev1604/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet"
-version = "0.9.0.dev1603"
+version = "0.9.0.dev1604"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-runtime = "0.9.0.dev1603"
+flet-runtime = "0.9.0.dev1604"
 python = "^3.7"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 websocket-client = "^1.5.2"
 watchdog = "^3.0.0"
 websockets = "^11.0.3"
 packaging = "^23.1"
 copier = "^8.0.0"
```

### Comparing `flet-0.9.0.dev1603/src/flet/__pyinstaller/macos_utils.py` & `flet-0.9.0.dev1604/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/__pyinstaller/utils.py` & `flet-0.9.0.dev1604/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/__pyinstaller/win_utils.py` & `flet-0.9.0.dev1604/src/flet/__pyinstaller/win_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/async_websocket_connection.py` & `flet-0.9.0.dev1604/src/flet/async_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/cli/cli.py` & `flet-0.9.0.dev1604/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/cli/commands/base.py` & `flet-0.9.0.dev1604/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/cli/commands/create.py` & `flet-0.9.0.dev1604/src/flet/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/cli/commands/options.py` & `flet-0.9.0.dev1604/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/cli/commands/pack.py` & `flet-0.9.0.dev1604/src/flet/cli/commands/pack.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/cli/commands/publish.py` & `flet-0.9.0.dev1604/src/flet/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/cli/commands/run.py` & `flet-0.9.0.dev1604/src/flet/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/reconnecting_websocket.py` & `flet-0.9.0.dev1604/src/flet/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/security.py` & `flet-0.9.0.dev1604/src/flet/security.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/sync_websocket_connection.py` & `flet-0.9.0.dev1604/src/flet/sync_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/version.py` & `flet-0.9.0.dev1604/src/flet/version.py`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/assets/NOTICES` & `flet-0.9.0.dev1604/src/flet/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/assets/fonts/MaterialIcons-Regular.otf` & `flet-0.9.0.dev1604/src/flet/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/assets/shaders/ink_sparkle.frag` & `flet-0.9.0.dev1604/src/flet/web/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/favicon.png` & `flet-0.9.0.dev1604/src/flet/web/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/flutter.js` & `flet-0.9.0.dev1604/src/flet/web/flutter.js`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/flutter_service_worker.js` & `flet-0.9.0.dev1604/src/flet/web/flutter_service_worker.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -30,16 +30,16 @@
     "canvaskit/skwasm.js": "1df4d741f441fa1a4d10530ced463ef8",
     "canvaskit/canvaskit.js": "76f7d822f42397160c5dfc69cbc9b2de",
     "canvaskit/skwasm.worker.js": "19659053a277272607529ef87acf9d8a",
     "canvaskit/skwasm.wasm": "6711032e17bf49924b2b001cef0d3ea3",
     "canvaskit/chromium/canvaskit.wasm": "fc18c3010856029414b70cae1afc5cd9",
     "canvaskit/chromium/canvaskit.js": "8c8392ce4a4364cbb240aa09b5652e05",
     "python-worker.js": "b961f261b9ad85e06369e83fd2e33bb7",
-    "index.html": "949910a95f13198a75b85451c6641204",
-    "/": "949910a95f13198a75b85451c6641204"
+    "index.html": "8d213814b6f52ea5f4857b109f1f2503",
+    "/": "8d213814b6f52ea5f4857b109f1f2503"
 };
 // The application shell files that are downloaded before a service worker can
 // start.
 const CORE = ["main.dart.js",
     "index.html",
     "assets/AssetManifest.json",
     "assets/FontManifest.json"
```

### Comparing `flet-0.9.0.dev1603/src/flet/web/icons/apple-touch-icon-192.png` & `flet-0.9.0.dev1604/src/flet/web/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/icons/icon-192.png` & `flet-0.9.0.dev1604/src/flet/web/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/icons/icon-512.png` & `flet-0.9.0.dev1604/src/flet/web/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/icons/icon-maskable-192.png` & `flet-0.9.0.dev1604/src/flet/web/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/icons/icon-maskable-512.png` & `flet-0.9.0.dev1604/src/flet/web/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/icons/loading-animation.png` & `flet-0.9.0.dev1604/src/flet/web/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/index.html` & `flet-0.9.0.dev1604/src/flet/web/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   <!-- webRenderer -->
   <!-- useColorEmoji -->
 
   <!-- pyodideCode -->
 
   <script>
     // The value below is injected by flutter build, do not touch.
-    var serviceWorkerVersion = "468383805";
+    var serviceWorkerVersion = "802957387";
   </script>
   <!-- This script adds the flutter initialization JS code -->
   <script src="flutter.js" defer></script>
 </head>
 
 <body>
   <div id="loading">
```

### Comparing `flet-0.9.0.dev1603/src/flet/web/main.dart.js` & `flet-0.9.0.dev1604/src/flet/web/main.dart.js`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/manifest.json` & `flet-0.9.0.dev1604/src/flet/web/manifest.json`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/python-worker.js` & `flet-0.9.0.dev1604/src/flet/web/python-worker.js`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/src/flet/web/python.js` & `flet-0.9.0.dev1604/src/flet/web/python.js`

 * *Files identical despite different names*

### Comparing `flet-0.9.0.dev1603/PKG-INFO` & `flet-0.9.0.dev1604/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: flet
-Version: 0.9.0.dev1603
+Version: 0.9.0.dev1604
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: copier (>=8.0.0,<9.0.0)
-Requires-Dist: flet-runtime (==0.9.0.dev1603)
+Requires-Dist: flet-runtime (==0.9.0.dev1604)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pydantic (<2)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Requires-Dist: websocket-client (>=1.5.2,<2.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
```

