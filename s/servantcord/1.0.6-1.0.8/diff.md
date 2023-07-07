# Comparing `tmp/servantcord-1.0.6.tar.gz` & `tmp/servantcord-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servantcord-1.0.6.tar", last modified: Fri Jul  7 13:05:20 2023, max compression
+gzip compressed data, was "servantcord-1.0.8.tar", last modified: Fri Jul  7 13:16:35 2023, max compression
```

## Comparing `servantcord-1.0.6.tar` & `servantcord-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.389366 servantcord-1.0.6/
--rw-rw-rw-   0        0        0      591 2023-07-07 13:05:20.388368 servantcord-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 13:05:20.389366 servantcord-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-07-07 13:05:11.000000 servantcord-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.377900 servantcord-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.380886 servantcord-1.0.6/src/servantcord/
--rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.6/src/servantcord/__init__.py
--rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.6/src/servantcord/lol.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.387434 servantcord-1.0.6/src/servantcord.egg-info/
--rw-rw-rw-   0        0        0      591 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 13:16:35.504834 servantcord-1.0.8/
+-rw-rw-rw-   0        0        0      591 2023-07-07 13:16:35.504834 servantcord-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:16:35.505799 servantcord-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2023-07-07 13:16:22.000000 servantcord-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:16:35.496569 servantcord-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:16:35.499982 servantcord-1.0.8/src/servantcord/
+-rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.8/src/servantcord/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.8/src/servantcord/lol.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:16:35.503854 servantcord-1.0.8/src/servantcord.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-07-07 13:16:35.000000 servantcord-1.0.8/src/servantcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-07 13:16:35.000000 servantcord-1.0.8/src/servantcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:16:35.000000 servantcord-1.0.8/src/servantcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 13:16:35.000000 servantcord-1.0.8/src/servantcord.egg-info/top_level.txt
```

### Comparing `servantcord-1.0.6/PKG-INFO` & `servantcord-1.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.6
+Version: 1.0.8
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `servantcord-1.0.6/src/servantcord.egg-info/PKG-INFO` & `servantcord-1.0.8/src/servantcord.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.6
+Version: 1.0.8
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

