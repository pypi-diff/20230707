# Comparing `tmp/hubotlibs-0.2.9.tar.gz` & `tmp/hubotlibs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubotlibs-0.2.9.tar", last modified: Fri Jul  7 02:33:00 2023, max compression
+gzip compressed data, was "hubotlibs-0.3.0.tar", last modified: Fri Jul  7 02:39:24 2023, max compression
```

## Comparing `hubotlibs-0.2.9.tar` & `hubotlibs-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:33:00.070341 hubotlibs-0.2.9/
--rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     2623 2023-07-07 02:33:00.070341 hubotlibs-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 02:33:00.019477 hubotlibs-0.2.9/hubotlibs/
--rw-rw-rw-   0        0        0     1110 2023-06-23 17:33:54.000000 hubotlibs-0.2.9/hubotlibs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:33:00.037429 hubotlibs-0.2.9/hubotlibs/dar/
--rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.2.9/hubotlibs/dar/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.2.9/hubotlibs/dar/load.py
--rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/log.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:33:00.066352 hubotlibs-0.2.9/hubotlibs/dar/utils/
--rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/PyroHelpers.py
--rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/adminHelpers.py
--rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/ai.py
--rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/aiohttp_helper.py
--rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/basic.py
--rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:33:00.068346 hubotlibs-0.2.9/hubotlibs/dar/utils/db/
--rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/db/__init__.py
--rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/db/permit.py
--rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/function.py
--rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/get_id.py
--rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/http.py
--rw-rw-rw-   0        0        0     4452 2023-07-07 02:32:30.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/inline.py
--rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/interval.py
--rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/misc.py
--rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/parser.py
--rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/pilter.py
--rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/tools.py
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/unpack.py
--rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.2.9/hubotlibs/dar/utils/utility.py
--rw-rw-rw-   0        0        0       47 2023-07-07 02:28:42.000000 hubotlibs-0.2.9/hubotlibs/version.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:33:00.034438 hubotlibs-0.2.9/hubotlibs.egg-info/
--rw-rw-rw-   0        0        0     2623 2023-07-07 02:32:59.000000 hubotlibs-0.2.9/hubotlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-07-07 02:32:59.000000 hubotlibs-0.2.9/hubotlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:32:59.000000 hubotlibs-0.2.9/hubotlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-07 02:32:59.000000 hubotlibs-0.2.9/hubotlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 02:32:59.000000 hubotlibs-0.2.9/hubotlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 02:33:00.072336 hubotlibs-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:39:24.208869 hubotlibs-0.3.0/
+-rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2623 2023-07-07 02:39:24.208869 hubotlibs-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 02:39:24.159752 hubotlibs-0.3.0/hubotlibs/
+-rw-rw-rw-   0        0        0     1110 2023-06-23 17:33:54.000000 hubotlibs-0.3.0/hubotlibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:39:24.177704 hubotlibs-0.3.0/hubotlibs/dar/
+-rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.3.0/hubotlibs/dar/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.3.0/hubotlibs/dar/load.py
+-rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/log.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:39:24.204879 hubotlibs-0.3.0/hubotlibs/dar/utils/
+-rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/PyroHelpers.py
+-rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/adminHelpers.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/ai.py
+-rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/aiohttp_helper.py
+-rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/basic.py
+-rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:39:24.207871 hubotlibs-0.3.0/hubotlibs/dar/utils/db/
+-rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/db/__init__.py
+-rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/db/permit.py
+-rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/function.py
+-rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/get_id.py
+-rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/http.py
+-rw-rw-rw-   0        0        0     4289 2023-07-07 02:38:58.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/inline.py
+-rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/interval.py
+-rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/misc.py
+-rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/parser.py
+-rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/pilter.py
+-rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/tools.py
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/unpack.py
+-rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.3.0/hubotlibs/dar/utils/utility.py
+-rw-rw-rw-   0        0        0       47 2023-07-07 02:39:08.000000 hubotlibs-0.3.0/hubotlibs/version.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:39:24.173714 hubotlibs-0.3.0/hubotlibs.egg-info/
+-rw-rw-rw-   0        0        0     2623 2023-07-07 02:39:24.000000 hubotlibs-0.3.0/hubotlibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-07-07 02:39:24.000000 hubotlibs-0.3.0/hubotlibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:39:24.000000 hubotlibs-0.3.0/hubotlibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-07 02:39:24.000000 hubotlibs-0.3.0/hubotlibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 02:39:24.000000 hubotlibs-0.3.0/hubotlibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:39:24.210876 hubotlibs-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.3.0/setup.py
```

### Comparing `hubotlibs-0.2.9/LICENSE` & `hubotlibs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/PKG-INFO` & `hubotlibs-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.2.9/README.md` & `hubotlibs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/__init__.py` & `hubotlibs-0.3.0/hubotlibs/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/__init__.py` & `hubotlibs-0.3.0/hubotlibs/dar/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/load.py` & `hubotlibs-0.3.0/hubotlibs/dar/load.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/log.py` & `hubotlibs-0.3.0/hubotlibs/dar/log.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/PyroHelpers.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/adminHelpers.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/ai.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/ai.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/aiohttp_helper.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/basic.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/basic.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/constants.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/db/__init__.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/db/permit.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/function.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/function.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/get_id.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/http.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/http.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/inline.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/inline.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,47 +96,40 @@
             [
                 EqInlineKeyboardButton(
                     x.__MODULE__,
                     callback_data="{}_module({})".format(
                         prefix, x.__MODULE__.replace(" ", "_").lower()
                     ),
                 )
-                for x in module_dict.values()
+                for x in data.values()
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
-                for x in module_dict.values()
+                for x in data.values()
             ]
         )
         
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
-    if user_id in PREMIUMID:
+    if user_id in BASICID:
+        
+        return modules
+            
+    elif user_id in MEDIUMID:
+        pairs = list(zip(modules[::2], modules[1::2]))
         
+        return pairs
+                
+    elif user_id in PREMIUMID:
         max_num_pages = ceil(len(pairs) / line)
         modulo_page = page_n % max_num_pages
 
         if len(pairs) > line:
             pairs = pairs[modulo_page * line : line * (modulo_page + 1)] + [
                 (
                     EqInlineKeyboardButton(
@@ -146,8 +139,8 @@
                     EqInlineKeyboardButton(
                         "❯",
                         callback_data="{}_next({})".format(prefix, modulo_page),
                     ),
                 )
             ]
 
-    return pairs
+        return pairs
```

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/interval.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/interval.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/misc.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/parser.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/parser.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/pilter.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/tools.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/unpack.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs/dar/utils/utility.py` & `hubotlibs-0.3.0/hubotlibs/dar/utils/utility.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/hubotlibs.egg-info/PKG-INFO` & `hubotlibs-0.3.0/hubotlibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.2.9/hubotlibs.egg-info/SOURCES.txt` & `hubotlibs-0.3.0/hubotlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.2.9/setup.py` & `hubotlibs-0.3.0/setup.py`

 * *Files identical despite different names*

