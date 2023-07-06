# Comparing `tmp/tarvis-tradingbot-0.9.6.tar.gz` & `tmp/tarvis-tradingbot-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-tradingbot-0.9.6.tar", last modified: Sun May 14 09:51:20 2023, max compression
+gzip compressed data, was "tarvis-tradingbot-0.9.9.tar", last modified: Thu Jul  6 23:14:38 2023, max compression
```

## Comparing `tarvis-tradingbot-0.9.6.tar` & `tarvis-tradingbot-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.572299 tarvis-tradingbot-0.9.6/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:51:20.572299 tarvis-tradingbot-0.9.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      842 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/tarvis/tradingbot/
--rw-r--r--   0 root         (0) root         (0)      526 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/tarvis/tradingbot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:14:38.697333 tarvis-tradingbot-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-06 23:14:28.000000 tarvis-tradingbot-0.9.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2023-07-06 23:14:38.697333 tarvis-tradingbot-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-06 23:14:28.000000 tarvis-tradingbot-0.9.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 23:14:38.697333 tarvis-tradingbot-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      836 2023-07-06 23:14:28.000000 tarvis-tradingbot-0.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:14:38.693333 tarvis-tradingbot-0.9.9/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:14:38.697333 tarvis-tradingbot-0.9.9/tarvis/tradingbot/
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-06 23:14:28.000000 tarvis-tradingbot-0.9.9/tarvis/tradingbot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:14:38.697333 tarvis-tradingbot-0.9.9/tarvis_tradingbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-07-06 23:14:38.000000 tarvis-tradingbot-0.9.9/tarvis_tradingbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-06 23:14:38.000000 tarvis-tradingbot-0.9.9/tarvis_tradingbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 23:14:38.000000 tarvis-tradingbot-0.9.9/tarvis_tradingbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-06 23:14:38.000000 tarvis-tradingbot-0.9.9/tarvis_tradingbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-06 23:14:38.000000 tarvis-tradingbot-0.9.9/tarvis_tradingbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 23:14:38.000000 tarvis-tradingbot-0.9.9/tarvis_tradingbot.egg-info/top_level.txt
```

### Comparing `tarvis-tradingbot-0.9.6/LICENSE.txt` & `tarvis-tradingbot-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-tradingbot-0.9.6/setup.py` & `tarvis-tradingbot-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-tradingbot",
-    version="0.9.6",
+    version="0.9.9",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
-    description="Tarvis Basic Trading Bot",
+    description="Tarvis Trading Bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=["License :: OSI Approved :: MIT License"],
     packages=find_namespace_packages(include=["tarvis.*"]),
     entry_points={"console_scripts": ["tarvis-tradingbot=tarvis.tradingbot:main"]},
     python_requires=">=3.10",
```

### Comparing `tarvis-tradingbot-0.9.6/tarvis/tradingbot/__init__.py` & `tarvis-tradingbot-0.9.9/tarvis/tradingbot/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from tarvis.btb import btbs
+from tarvis.atb import atbs
+import tarvis.exchange.binance
 import tarvis.exchange.dydx
 import tarvis.exchange.woo
 import tarvis.indicators.webapi
 from tarvis.indicators.webapi import WebAPIIndicatorSource
 
 
 def main():
-    btbs.run(
+    atbs.run(
         indicator_source_classes=[WebAPIIndicatorSource],
         exchange_classes=[
+            tarvis.exchange.binance.BinanceExchange,
             tarvis.exchange.dydx.DYDXExchange,
             tarvis.exchange.woo.WooExchange,
         ],
         additional_providers=None,
         additional_modules=[tarvis.indicators.webapi],
     )
```

