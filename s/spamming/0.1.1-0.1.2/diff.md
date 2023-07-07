# Comparing `tmp/spamming-0.1.1.tar.gz` & `tmp/spamming-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spamming-0.1.1.tar", last modified: Fri Jul  7 18:11:59 2023, max compression
+gzip compressed data, was "spamming-0.1.2.tar", last modified: Fri Jul  7 18:16:45 2023, max compression
```

## Comparing `spamming-0.1.1.tar` & `spamming-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:11:59.348459 spamming-0.1.1/
--rw-rw-rw-   0        0        0     1099 2023-07-04 18:01:23.000000 spamming-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      777 2023-07-07 18:11:59.345465 spamming-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-07-07 18:04:13.000000 spamming-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 18:11:59.348459 spamming-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-07-07 18:11:27.000000 spamming-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:11:59.294270 spamming-0.1.1/spamming/
--rw-rw-rw-   0        0        0      180 2023-07-07 18:11:25.000000 spamming-0.1.1/spamming/__init__.py
--rw-rw-rw-   0        0        0      732 2023-07-07 17:54:42.000000 spamming-0.1.1/spamming/nonsense.py
--rw-rw-rw-   0        0        0      387 2023-07-07 17:54:14.000000 spamming-0.1.1/spamming/spamclick.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:11:59.338852 spamming-0.1.1/spamming.egg-info/
--rw-rw-rw-   0        0        0      777 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-07 18:11:59.000000 spamming-0.1.1/spamming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 18:16:45.922971 spamming-0.1.2/
+-rw-rw-rw-   0        0        0     1099 2023-07-04 18:01:23.000000 spamming-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      777 2023-07-07 18:16:45.918388 spamming-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-07-07 18:04:13.000000 spamming-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 18:16:45.923969 spamming-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-07-07 18:14:56.000000 spamming-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:16:45.875828 spamming-0.1.2/spamming/
+-rw-rw-rw-   0        0        0      205 2023-07-07 18:15:41.000000 spamming-0.1.2/spamming/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-07-07 17:54:42.000000 spamming-0.1.2/spamming/nonsense.py
+-rw-rw-rw-   0        0        0      387 2023-07-07 17:54:14.000000 spamming-0.1.2/spamming/spamclick.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:16:45.914398 spamming-0.1.2/spamming.egg-info/
+-rw-rw-rw-   0        0        0      777 2023-07-07 18:16:45.000000 spamming-0.1.2/spamming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-07 18:16:45.000000 spamming-0.1.2/spamming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:16:45.000000 spamming-0.1.2/spamming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 18:16:45.000000 spamming-0.1.2/spamming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 18:16:45.000000 spamming-0.1.2/spamming.egg-info/top_level.txt
```

### Comparing `spamming-0.1.1/LICENSE` & `spamming-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spamming-0.1.1/setup.py` & `spamming-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='spamming',
-    version='0.1.1',
+    version='0.1.2',
     license='MIT',
     description= "A spamming package",
     long_description= open("README.md").read(),
     long_description_content_type= "text/markdown",
     author="gugu256",
     author_email='gugu256@mail.com',
     keywords=["spamming", "spam", "automation", "pyautogui"],
```

### Comparing `spamming-0.1.1/spamming/nonsense.py` & `spamming-0.1.2/spamming/nonsense.py`

 * *Files identical despite different names*

