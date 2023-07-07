# Comparing `tmp/LIB-ADTECH-1.0.6.tar.gz` & `tmp/LIB-ADTECH-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LIB-ADTECH-1.0.6.tar", last modified: Fri Jul  7 14:06:43 2023, max compression
+gzip compressed data, was "LIB-ADTECH-1.0.7.tar", last modified: Fri Jul  7 14:14:57 2023, max compression
```

## Comparing `LIB-ADTECH-1.0.6.tar` & `LIB-ADTECH-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:43.400939 LIB-ADTECH-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:43.385429 LIB-ADTECH-1.0.6/Adlib/
--rw-rw-rw-   0        0        0       26 2023-07-07 12:20:05.000000 LIB-ADTECH-1.0.6/Adlib/__ini__.py
--rw-rw-rw-   0        0        0     3640 2023-07-07 12:20:05.000000 LIB-ADTECH-1.0.6/Adlib/funcoes.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:43.396488 LIB-ADTECH-1.0.6/LIB_ADTECH.egg-info/
--rw-rw-rw-   0        0        0      313 2023-07-07 14:06:43.000000 LIB-ADTECH-1.0.6/LIB_ADTECH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-07 14:06:43.000000 LIB-ADTECH-1.0.6/LIB_ADTECH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:06:43.000000 LIB-ADTECH-1.0.6/LIB_ADTECH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-07-07 14:06:43.000000 LIB-ADTECH-1.0.6/LIB_ADTECH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 14:06:43.000000 LIB-ADTECH-1.0.6/LIB_ADTECH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-07-07 12:20:58.000000 LIB-ADTECH-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      313 2023-07-07 14:06:43.398492 LIB-ADTECH-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 12:22:07.000000 LIB-ADTECH-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 14:06:43.402181 LIB-ADTECH-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-07-07 14:06:36.000000 LIB-ADTECH-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:14:57.300488 LIB-ADTECH-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-07 14:14:57.280728 LIB-ADTECH-1.0.7/Adlib/
+-rw-rw-rw-   0        0        0       26 2023-07-07 12:20:05.000000 LIB-ADTECH-1.0.7/Adlib/__ini__.py
+-rw-rw-rw-   0        0        0     3640 2023-07-07 14:13:34.000000 LIB-ADTECH-1.0.7/Adlib/funcoes.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:14:57.295496 LIB-ADTECH-1.0.7/LIB_ADTECH.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-07-07 14:14:57.000000 LIB-ADTECH-1.0.7/LIB_ADTECH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-07 14:14:57.000000 LIB-ADTECH-1.0.7/LIB_ADTECH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:14:57.000000 LIB-ADTECH-1.0.7/LIB_ADTECH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-07-07 14:14:57.000000 LIB-ADTECH-1.0.7/LIB_ADTECH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 14:14:57.000000 LIB-ADTECH-1.0.7/LIB_ADTECH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-07-07 12:20:58.000000 LIB-ADTECH-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      313 2023-07-07 14:14:57.295496 LIB-ADTECH-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:22:07.000000 LIB-ADTECH-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:14:57.300488 LIB-ADTECH-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-07-07 14:14:46.000000 LIB-ADTECH-1.0.7/setup.py
```

### Comparing `LIB-ADTECH-1.0.6/Adlib/funcoes.py` & `LIB-ADTECH-1.0.7/Adlib/funcoes.py`

 * *Files identical despite different names*

### Comparing `LIB-ADTECH-1.0.6/LICENSE` & `LIB-ADTECH-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LIB-ADTECH-1.0.6/setup.py` & `LIB-ADTECH-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
+with open("requirements.txt", "r") as arq:
+    requisitos = [linha.strip()[1:-1] for linha in arq.readlines()]
+
 setup(
     name='LIB-ADTECH',
-    version='1.0.6',
+    version='1.0.7',
     license='MIT License',
     author='Alan, Fabiano e Yan',
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='driverWait, librarySelenium',
     description=u'Funções úteis para desenvolvimento web.',
     packages=['Adlib'],
-    install_requires=['requests', 'selenium',
-'pandas'
-'numpy'
-'selenium'
-'beautifulsoup4'
-'openpyxl'
-'datetime'
-'chromedriver-autoinstaller'
-'tkinter'
-'discord-webhook'
- ]
+    install_requires=requisitos,
 )
```

