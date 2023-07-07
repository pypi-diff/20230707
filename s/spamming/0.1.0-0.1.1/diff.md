# Comparing `tmp/spamming-0.1.0.tar.gz` & `tmp/spamming-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spamming-0.1.0.tar", last modified: Fri Jul  7 18:08:29 2023, max compression
+gzip compressed data, was "spamming-0.1.1.tar", last modified: Fri Jul  7 18:11:59 2023, max compression
```

## Comparing `spamming-0.1.0.tar` & `spamming-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:08:29.175234 spamming-0.1.0/
--rw-rw-rw-   0        0        0     1099 2023-07-04 18:01:23.000000 spamming-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      777 2023-07-07 18:08:29.174227 spamming-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-07-07 18:04:13.000000 spamming-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 18:08:29.176232 spamming-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-07-07 18:08:13.000000 spamming-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:08:29.139175 spamming-0.1.0/spamming/
--rw-rw-rw-   0        0        0      162 2023-07-07 18:07:50.000000 spamming-0.1.0/spamming/__init__.py
--rw-rw-rw-   0        0        0      732 2023-07-07 17:54:42.000000 spamming-0.1.0/spamming/nonsense.py
--rw-rw-rw-   0        0        0      387 2023-07-07 17:54:14.000000 spamming-0.1.0/spamming/spamclick.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:08:29.169685 spamming-0.1.0/spamming.egg-info/
--rw-rw-rw-   0        0        0      777 2023-07-07 18:08:28.000000 spamming-0.1.0/spamming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-07 18:08:29.000000 spamming-0.1.0/spamming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:08:28.000000 spamming-0.1.0/spamming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 18:08:28.000000 spamming-0.1.0/spamming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 18:08:28.000000 spamming-0.1.0/spamming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 18:11:59.348459 spamming-0.1.1/
+-rw-rw-rw-   0        0        0     1099 2023-07-04 18:01:23.000000 spamming-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      777 2023-07-07 18:11:59.345465 spamming-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-07-07 18:04:13.000000 spamming-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 18:11:59.348459 spamming-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-07-07 18:11:27.000000 spamming-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:11:59.294270 spamming-0.1.1/spamming/
+-rw-rw-rw-   0        0        0      180 2023-07-07 18:11:25.000000 spamming-0.1.1/spamming/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-07-07 17:54:42.000000 spamming-0.1.1/spamming/nonsense.py
+-rw-rw-rw-   0        0        0      387 2023-07-07 17:54:14.000000 spamming-0.1.1/spamming/spamclick.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:11:59.338852 spamming-0.1.1/spamming.egg-info/
+-rw-rw-rw-   0        0        0      777 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-07 18:11:59.000000 spamming-0.1.1/spamming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 18:11:58.000000 spamming-0.1.1/spamming.egg-info/top_level.txt
```

### Comparing `spamming-0.1.0/LICENSE` & `spamming-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spamming-0.1.0/setup.py` & `spamming-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='spamming',
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
     description= "A spamming package",
     long_description= open("README.md").read(),
     long_description_content_type= "text/markdown",
     author="gugu256",
     author_email='gugu256@mail.com',
     keywords=["spamming", "spam", "automation", "pyautogui"],
```

### Comparing `spamming-0.1.0/spamming/nonsense.py` & `spamming-0.1.1/spamming/nonsense.py`

 * *Files identical despite different names*

