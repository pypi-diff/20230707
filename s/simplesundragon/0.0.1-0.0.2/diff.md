# Comparing `tmp/simplesundragon-0.0.1.tar.gz` & `tmp/simplesundragon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesundragon-0.0.1.tar", last modified: Fri Jul  7 07:57:04 2023, max compression
+gzip compressed data, was "simplesundragon-0.0.2.tar", last modified: Fri Jul  7 09:35:39 2023, max compression
```

## Comparing `simplesundragon-0.0.1.tar` & `simplesundragon-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:57:04.753757 simplesundragon-0.0.1/
--rw-rw-rw-   0        0        0      475 2023-07-07 07:57:04.753757 simplesundragon-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2023-07-07 07:26:54.000000 simplesundragon-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 07:57:04.753757 simplesundragon-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-07-07 07:55:41.000000 simplesundragon-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:57:04.737415 simplesundragon-0.0.1/simplesundragon/
--rw-rw-rw-   0        0        0     1689 2023-07-07 07:23:21.000000 simplesundragon-0.0.1/simplesundragon/simplesundragon.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:57:04.753757 simplesundragon-0.0.1/simplesundragon.egg-info/
--rw-rw-rw-   0        0        0      475 2023-07-07 07:57:04.000000 simplesundragon-0.0.1/simplesundragon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-07 07:57:04.000000 simplesundragon-0.0.1/simplesundragon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:57:04.000000 simplesundragon-0.0.1/simplesundragon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-07 07:57:04.000000 simplesundragon-0.0.1/simplesundragon.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-07-07 07:57:04.000000 simplesundragon-0.0.1/simplesundragon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 09:35:39.696165 simplesundragon-0.0.2/
+-rw-rw-rw-   0        0        0      475 2023-07-07 09:35:39.695160 simplesundragon-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2023-07-07 09:22:25.000000 simplesundragon-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 09:35:39.696165 simplesundragon-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-07-07 09:32:43.000000 simplesundragon-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:35:39.686193 simplesundragon-0.0.2/simplesundragon/
+-rw-rw-rw-   0        0        0     1689 2023-07-07 07:23:21.000000 simplesundragon-0.0.2/simplesundragon/simplesundragon.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:35:39.694158 simplesundragon-0.0.2/simplesundragon.egg-info/
+-rw-rw-rw-   0        0        0      475 2023-07-07 09:35:39.000000 simplesundragon-0.0.2/simplesundragon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-07 09:35:39.000000 simplesundragon-0.0.2/simplesundragon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 09:35:39.000000 simplesundragon-0.0.2/simplesundragon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-07 07:57:04.000000 simplesundragon-0.0.2/simplesundragon.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-07-07 09:35:39.000000 simplesundragon-0.0.2/simplesundragon.egg-info/top_level.txt
```

### Comparing `simplesundragon-0.0.1/setup.py` & `simplesundragon-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='simplesundragon', # 패키지 명
-    version='0.0.1',
+    version='0.0.2',
     description='study first Package',
     author='Jeongdongki',
     author_email='dkrhank45@skuniv.ac.kr',
     url='https://github.com/jeongdonggi/SimpleSunDragon',
     python_requires='>=3',
     install_requires=[],
     keywords=['Jeongdongki', 'simplesundragon'],
```

### Comparing `simplesundragon-0.0.1/simplesundragon/simplesundragon.py` & `simplesundragon-0.0.2/simplesundragon/simplesundragon.py`

 * *Files identical despite different names*

