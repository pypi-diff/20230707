# Comparing `tmp/LolzteamApi-1.0.8.tar.gz` & `tmp/LolzteamApi-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.8.tar", last modified: Fri Jul  7 15:03:11 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.9.tar", last modified: Fri Jul  7 15:34:04 2023, max compression
```

## Comparing `LolzteamApi-1.0.8.tar` & `LolzteamApi-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:03:11.391167 LolzteamApi-1.0.8/
--rw-rw-rw-   0        0        0     1082 2023-07-07 14:49:03.000000 LolzteamApi-1.0.8/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-07 15:03:11.375153 LolzteamApi-1.0.8/LolzteamApi/
--rw-rw-rw-   0        0        0        0 2023-07-07 14:50:53.000000 LolzteamApi-1.0.8/LolzteamApi/__init__.py
--rw-rw-rw-   0        0        0   163271 2023-07-07 11:33:39.000000 LolzteamApi-1.0.8/LolzteamApi/main.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:03:11.389170 LolzteamApi-1.0.8/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     1649 2023-07-07 15:03:11.000000 LolzteamApi-1.0.8/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-07 15:03:11.000000 LolzteamApi-1.0.8/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:03:11.000000 LolzteamApi-1.0.8/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 15:03:11.000000 LolzteamApi-1.0.8/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 15:03:11.000000 LolzteamApi-1.0.8/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1649 2023-07-07 15:03:11.391167 LolzteamApi-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-07-06 22:34:30.000000 LolzteamApi-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 15:03:11.392169 LolzteamApi-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-07-07 14:46:22.000000 LolzteamApi-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:34:04.907202 LolzteamApi-1.0.9/
+-rw-rw-rw-   0        0        0     1082 2023-07-07 14:49:03.000000 LolzteamApi-1.0.9/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-07 15:34:04.899204 LolzteamApi-1.0.9/LolzteamApi/
+-rw-rw-rw-   0        0        0        0 2023-07-07 14:50:53.000000 LolzteamApi-1.0.9/LolzteamApi/__init__.py
+-rw-rw-rw-   0        0        0   163271 2023-07-07 11:33:39.000000 LolzteamApi-1.0.9/LolzteamApi/main.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:34:04.904201 LolzteamApi-1.0.9/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     1649 2023-07-07 15:34:04.000000 LolzteamApi-1.0.9/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-07 15:34:04.000000 LolzteamApi-1.0.9/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:34:04.000000 LolzteamApi-1.0.9/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 15:34:04.000000 LolzteamApi-1.0.9/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 15:34:04.000000 LolzteamApi-1.0.9/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1649 2023-07-07 15:34:04.906202 LolzteamApi-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-07-06 22:34:30.000000 LolzteamApi-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:34:04.907202 LolzteamApi-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-07-07 15:33:26.000000 LolzteamApi-1.0.9/setup.py
```

### Comparing `LolzteamApi-1.0.8/LICENSE` & `LolzteamApi-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.8/LolzteamApi/main.py` & `LolzteamApi-1.0.9/LolzteamApi/main.py`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.8/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.9/LolzteamApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `LolzteamApi-1.0.8/PKG-INFO` & `LolzteamApi-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `LolzteamApi-1.0.8/README.md` & `LolzteamApi-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.8/setup.py` & `LolzteamApi-1.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.8",
+    version="1.0.9",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
```

