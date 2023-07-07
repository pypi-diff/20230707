# Comparing `tmp/spamming-0.1.0.tar.gz` & `tmp/spamming-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spamming-0.1.tar", last modified: Fri Jul  7 18:00:09 2023, max compression
+gzip compressed data, was "spamming-1.0.tar", last modified: Fri Jul  7 18:01:54 2023, max compression
```

## Comparing `spamming-0.1.0.tar` & `spamming-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:00:09.817297 spamming-0.1/
--rw-rw-rw-   0        0        0     1099 2023-07-04 18:01:23.000000 spamming-0.1/LICENSE
--rw-rw-rw-   0        0        0      764 2023-07-07 18:00:09.815280 spamming-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-07-07 17:58:57.000000 spamming-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 18:00:09.817297 spamming-0.1/setup.cfg
--rw-rw-rw-   0        0        0      701 2023-07-07 17:58:52.000000 spamming-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:00:09.790723 spamming-0.1/spamming/
--rw-rw-rw-   0        0        0      134 2023-07-07 17:59:09.000000 spamming-0.1/spamming/__init__.py
--rw-rw-rw-   0        0        0      732 2023-07-07 17:54:42.000000 spamming-0.1/spamming/nonsense.py
--rw-rw-rw-   0        0        0      387 2023-07-07 17:54:14.000000 spamming-0.1/spamming/spamclick.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:00:09.810743 spamming-0.1/spamming.egg-info/
--rw-rw-rw-   0        0        0      764 2023-07-07 18:00:09.000000 spamming-0.1/spamming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-07 18:00:09.000000 spamming-0.1/spamming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:00:09.000000 spamming-0.1/spamming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 18:00:09.000000 spamming-0.1/spamming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 18:00:09.000000 spamming-0.1/spamming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 18:01:54.180449 spamming-1.0/
+-rw-rw-rw-   0        0        0     1099 2023-07-04 18:01:23.000000 spamming-1.0/LICENSE
+-rw-rw-rw-   0        0        0      763 2023-07-07 18:01:54.178075 spamming-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-07-07 18:00:53.000000 spamming-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 18:01:54.180449 spamming-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      701 2023-07-07 18:00:49.000000 spamming-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:01:54.146069 spamming-1.0/spamming/
+-rw-rw-rw-   0        0        0      160 2023-07-07 18:01:15.000000 spamming-1.0/spamming/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-07-07 17:54:42.000000 spamming-1.0/spamming/nonsense.py
+-rw-rw-rw-   0        0        0      387 2023-07-07 17:54:14.000000 spamming-1.0/spamming/spamclick.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:01:54.175064 spamming-1.0/spamming.egg-info/
+-rw-rw-rw-   0        0        0      763 2023-07-07 18:01:53.000000 spamming-1.0/spamming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-07 18:01:54.000000 spamming-1.0/spamming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:01:53.000000 spamming-1.0/spamming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 18:01:53.000000 spamming-1.0/spamming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 18:01:53.000000 spamming-1.0/spamming.egg-info/top_level.txt
```

### Comparing `spamming-0.1/LICENSE` & `spamming-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spamming-0.1/setup.py` & `spamming-1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='spamming',
-    version='0.1',
+    version='1.0',
     license='MIT',
     description= "A spamming package",
     long_description= open("README.md").read(),
     long_description_content_type= "text/markdown",
     author="gugu256",
     author_email='gugu256@mail.com',
     keywords=["spamming", "spam", "automation", "pyautogui"],
```

### Comparing `spamming-0.1/spamming/nonsense.py` & `spamming-1.0/spamming/nonsense.py`

 * *Files identical despite different names*

