# Comparing `tmp/hubotlibs-0.2.6.tar.gz` & `tmp/hubotlibs-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubotlibs-0.2.6.tar", last modified: Fri Jul  7 02:01:22 2023, max compression
+gzip compressed data, was "hubotlibs-0.2.7.tar", last modified: Fri Jul  7 02:17:50 2023, max compression
```

## Comparing `hubotlibs-0.2.6.tar` & `hubotlibs-0.2.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:01:22.881436 hubotlibs-0.2.6/
--rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     2623 2023-07-07 02:01:22.881436 hubotlibs-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 02:01:22.828578 hubotlibs-0.2.6/hubotlibs/
--rw-rw-rw-   0        0        0     1110 2023-06-23 17:33:54.000000 hubotlibs-0.2.6/hubotlibs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:01:22.852514 hubotlibs-0.2.6/hubotlibs/dar/
--rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.2.6/hubotlibs/dar/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.2.6/hubotlibs/dar/load.py
--rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/log.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:01:22.876450 hubotlibs-0.2.6/hubotlibs/dar/utils/
--rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/PyroHelpers.py
--rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/adminHelpers.py
--rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/ai.py
--rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/aiohttp_helper.py
--rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/basic.py
--rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:01:22.879443 hubotlibs-0.2.6/hubotlibs/dar/utils/db/
--rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/db/__init__.py
--rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/db/permit.py
--rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/function.py
--rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/get_id.py
--rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/http.py
--rw-rw-rw-   0        0        0     3696 2023-07-07 01:45:07.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/inline.py
--rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/interval.py
--rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/misc.py
--rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/parser.py
--rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/pilter.py
--rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/tools.py
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/unpack.py
--rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.2.6/hubotlibs/dar/utils/utility.py
--rw-rw-rw-   0        0        0       47 2023-07-07 01:42:39.000000 hubotlibs-0.2.6/hubotlibs/version.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:01:22.846530 hubotlibs-0.2.6/hubotlibs.egg-info/
--rw-rw-rw-   0        0        0     2623 2023-07-07 02:01:22.000000 hubotlibs-0.2.6/hubotlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-07-07 02:01:22.000000 hubotlibs-0.2.6/hubotlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:01:22.000000 hubotlibs-0.2.6/hubotlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-07 02:01:22.000000 hubotlibs-0.2.6/hubotlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 02:01:22.000000 hubotlibs-0.2.6/hubotlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 02:01:22.884430 hubotlibs-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:17:50.350936 hubotlibs-0.2.7/
+-rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     2623 2023-07-07 02:17:50.350936 hubotlibs-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 02:17:50.299600 hubotlibs-0.2.7/hubotlibs/
+-rw-rw-rw-   0        0        0     1110 2023-06-23 17:33:54.000000 hubotlibs-0.2.7/hubotlibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:17:50.317552 hubotlibs-0.2.7/hubotlibs/dar/
+-rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.2.7/hubotlibs/dar/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.2.7/hubotlibs/dar/load.py
+-rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/log.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:17:50.346750 hubotlibs-0.2.7/hubotlibs/dar/utils/
+-rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/PyroHelpers.py
+-rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/adminHelpers.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/ai.py
+-rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/aiohttp_helper.py
+-rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/basic.py
+-rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:17:50.348744 hubotlibs-0.2.7/hubotlibs/dar/utils/db/
+-rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/db/__init__.py
+-rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/db/permit.py
+-rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/function.py
+-rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/get_id.py
+-rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/http.py
+-rw-rw-rw-   0        0        0     4708 2023-07-07 02:12:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/inline.py
+-rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/interval.py
+-rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/misc.py
+-rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/parser.py
+-rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/pilter.py
+-rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/tools.py
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/unpack.py
+-rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.2.7/hubotlibs/dar/utils/utility.py
+-rw-rw-rw-   0        0        0       47 2023-07-07 02:13:03.000000 hubotlibs-0.2.7/hubotlibs/version.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:17:50.314559 hubotlibs-0.2.7/hubotlibs.egg-info/
+-rw-rw-rw-   0        0        0     2623 2023-07-07 02:17:50.000000 hubotlibs-0.2.7/hubotlibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-07-07 02:17:50.000000 hubotlibs-0.2.7/hubotlibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:17:50.000000 hubotlibs-0.2.7/hubotlibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-07 02:17:50.000000 hubotlibs-0.2.7/hubotlibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 02:17:50.000000 hubotlibs-0.2.7/hubotlibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:17:50.356922 hubotlibs-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.2.7/setup.py
```

### Comparing `hubotlibs-0.2.6/LICENSE` & `hubotlibs-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/PKG-INFO` & `hubotlibs-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.2.6/README.md` & `hubotlibs-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/__init__.py` & `hubotlibs-0.2.7/hubotlibs/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/__init__.py` & `hubotlibs-0.2.7/hubotlibs/dar/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/load.py` & `hubotlibs-0.2.7/hubotlibs/dar/load.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/log.py` & `hubotlibs-0.2.7/hubotlibs/dar/log.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/PyroHelpers.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/adminHelpers.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/ai.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/ai.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/aiohttp_helper.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/basic.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/basic.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/constants.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/db/__init__.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/db/permit.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/function.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/function.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/get_id.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/http.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/http.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/inline.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/inline.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,124 +12,151 @@
     def __lt__(self, other):
         return self.text < other.text
 
     def __gt__(self, other):
         return self.text > other.text
 
 
-def basic_medium_modules(user_id, datadict, prefix, chat=None):
+# def basic_medium_modules(user_id, datadict, prefix, chat=None):
     
+#     data = {}
+#     if user_id in BASICID:
+#         filter_set = {'limit', 'broadcast', 'help'}
+#         for key, value in datadict.items():
+#             if key in filter_set:
+#                 data[key] = value
+            
+#     elif user_id in MEDIUMID:
+#         filter_set = {'limit', 'broadcast', 'pilter', 'help', 'afk', 'antipm', 'botlog'}
+#         for key, value in datadict.items():
+#             if key in filter_set:
+#                 data[key] = value
+
+#     if not chat:
+#         modules = sorted(
+#             [
+#                 EqInlineKeyboardButton(
+#                     x.__MODULE__,
+#                     callback_data="{}_module({})".format(
+#                         prefix, x.__MODULE__.replace(" ", "_").lower()
+#                     ),
+#                 )
+#                 for x in data.values()
+#             ]
+#         )
+#     else:
+#         modules = sorted(
+#             [
+#                 EqInlineKeyboardButton(
+#                     x.__MODULE__,
+#                     callback_data="{}_module({},{})".format(
+#                         prefix, chat, x.__MODULE__.replace(" ", "_").lower()
+#                     ),
+#                 )
+#                 for x in data.values()
+#             ]
+#         )
+        
+#     pairs = list(zip(modules[::2], modules[1::2]))
+#     i = 0
+#     for m in pairs:
+#         for _ in m:
+#             i += 1
+#     if len(modules) - i == 1:
+#         pairs.append((modules[-1],))
+#     elif len(modules) - i == 2:
+#         pairs.append(
+#             (
+#                 modules[-2],
+#                 modules[-1],
+#             )
+#         )
+        
+#     return pairs
+
+
+def prem_modules(user_id, page_n, module_dict, prefix, chat=None):
     data = {}
     if user_id in BASICID:
         filter_set = {'limit', 'broadcast', 'help'}
         for key, value in datadict.items():
             if key in filter_set:
                 data[key] = value
             
     elif user_id in MEDIUMID:
         filter_set = {'limit', 'broadcast', 'pilter', 'help', 'afk', 'antipm', 'botlog'}
         for key, value in datadict.items():
             if key in filter_set:
                 data[key] = value
-
+                
+    elif user_id in PREMIUMID:
+        data = module_dict
+        
     if not chat:
         modules = sorted(
             [
                 EqInlineKeyboardButton(
                     x.__MODULE__,
                     callback_data="{}_module({})".format(
                         prefix, x.__MODULE__.replace(" ", "_").lower()
                     ),
                 )
-                for x in data.values()
+                for x in module_dict.values()
             ]
         )
     else:
         modules = sorted(
             [
                 EqInlineKeyboardButton(
                     x.__MODULE__,
                     callback_data="{}_module({},{})".format(
                         prefix, chat, x.__MODULE__.replace(" ", "_").lower()
                     ),
                 )
-                for x in data.values()
+                for x in module_dict.values()
             ]
         )
         
-    pairs = list(zip(modules[::2], modules[1::2]))
-    i = 0
-    for m in pairs:
-        for _ in m:
-            i += 1
-    if len(modules) - i == 1:
-        pairs.append((modules[-1],))
-    elif len(modules) - i == 2:
-        pairs.append(
-            (
-                modules[-2],
-                modules[-1],
-            )
-        )
+    if user_id in BASICID:
+        
+        return modules
+            
+    elif user_id in MEDIUMID:
+        pairs = list(zip(modules[::2], modules[1::2]))
         
-    return pairs
+        return pairs
+                
+    elif user_id in PREMIUMID:
+        line = 4
+        pairs = list(zip(modules[::2], modules[1::2]))
+        i = 0
+        for m in pairs:
+            for _ in m:
+                i += 1
+        if len(modules) - i == 1:
+            pairs.append((modules[-1],))
+        elif len(modules) - i == 2:
+            pairs.append(
+                (
+                    modules[-2],
+                    modules[-1],
+                )
+            )
 
+        max_num_pages = ceil(len(pairs) / line)
+        modulo_page = page_n % max_num_pages
 
-def prem_modules(page_n, module_dict, prefix, chat=None):
-    if not chat:
-        modules = sorted(
-            [
-                EqInlineKeyboardButton(
-                    x.__MODULE__,
-                    callback_data="{}_module({})".format(
-                        prefix, x.__MODULE__.replace(" ", "_").lower()
+        if len(pairs) > line:
+            pairs = pairs[modulo_page * line : line * (modulo_page + 1)] + [
+                (
+                    EqInlineKeyboardButton(
+                        "❮",
+                        callback_data="{}_prev({})".format(prefix, modulo_page),
                     ),
-                )
-                for x in module_dict.values()
-            ]
-        )
-    else:
-        modules = sorted(
-            [
-                EqInlineKeyboardButton(
-                    x.__MODULE__,
-                    callback_data="{}_module({},{})".format(
-                        prefix, chat, x.__MODULE__.replace(" ", "_").lower()
+                    EqInlineKeyboardButton(
+                        "❯",
+                        callback_data="{}_next({})".format(prefix, modulo_page),
                     ),
                 )
-                for x in module_dict.values()
             ]
-        )
-    line = 4
-    pairs = list(zip(modules[::2], modules[1::2]))
-    i = 0
-    for m in pairs:
-        for _ in m:
-            i += 1
-    if len(modules) - i == 1:
-        pairs.append((modules[-1],))
-    elif len(modules) - i == 2:
-        pairs.append(
-            (
-                modules[-2],
-                modules[-1],
-            )
-        )
-
-    max_num_pages = ceil(len(pairs) / line)
-    modulo_page = page_n % max_num_pages
-
-    if len(pairs) > line:
-        pairs = pairs[modulo_page * line : line * (modulo_page + 1)] + [
-            (
-                EqInlineKeyboardButton(
-                    "❮",
-                    callback_data="{}_prev({})".format(prefix, modulo_page),
-                ),
-                EqInlineKeyboardButton(
-                    "❯",
-                    callback_data="{}_next({})".format(prefix, modulo_page),
-                ),
-            )
-        ]
 
-    return pairs
+        return pairs
```

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/interval.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/interval.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/misc.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/parser.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/parser.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/pilter.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/tools.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/unpack.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs/dar/utils/utility.py` & `hubotlibs-0.2.7/hubotlibs/dar/utils/utility.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/hubotlibs.egg-info/PKG-INFO` & `hubotlibs-0.2.7/hubotlibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.2.6/hubotlibs.egg-info/SOURCES.txt` & `hubotlibs-0.2.7/hubotlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.6/setup.py` & `hubotlibs-0.2.7/setup.py`

 * *Files identical despite different names*

