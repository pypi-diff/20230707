# Comparing `tmp/songline-0.0.1.tar.gz` & `tmp/songline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\songline-0.0.1.tar", last modified: Mon May 20 13:37:37 2019, max compression
+gzip compressed data, was "songline-0.0.2.tar", last modified: Fri Jul  7 06:04:13 2023, max compression
```

## Comparing `songline-0.0.1.tar` & `songline-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,16 @@
-drwxrwxrwx   0        0        0        0 2019-05-20 13:37:37.000000 songline-0.0.1/
--rw-rw-rw-   0        0        0     1305 2019-05-20 13:37:37.000000 songline-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      313 2019-05-20 13:36:02.000000 songline-0.0.1/README.txt
--rw-rw-rw-   0        0        0       40 2019-05-19 07:28:32.000000 songline-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1959 2019-05-20 13:34:43.000000 songline-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2019-05-20 13:37:37.000000 songline-0.0.1/songline/
--rw-rw-rw-   0        0        0       38 2019-05-20 13:06:26.000000 songline-0.0.1/songline/__init__.py
--rw-rw-rw-   0        0        0     1543 2019-05-20 13:06:23.000000 songline-0.0.1/songline/sendline.py
+drwxrwxrwx   0        0        0        0 2023-07-07 06:04:13.440214 songline-0.0.2/
+-rw-rw-rw-   0        0        0     1071 2023-07-07 01:51:10.000000 songline-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1082 2023-07-07 01:51:10.000000 songline-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2445 2023-07-07 06:04:13.440214 songline-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1522 2023-07-07 01:51:10.000000 songline-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-07 06:04:13.444205 songline-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1948 2023-07-07 03:52:07.000000 songline-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 06:04:13.412289 songline-0.0.2/songline/
+-rw-rw-rw-   0        0        0       39 2023-07-07 01:51:10.000000 songline-0.0.2/songline/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-07-07 03:51:55.000000 songline-0.0.2/songline/sendline.py
+drwxrwxrwx   0        0        0        0 2023-07-07 06:04:13.439217 songline-0.0.2/songline.egg-info/
+-rw-rw-rw-   0        0        0     2445 2023-07-07 06:04:13.000000 songline-0.0.2/songline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-07 06:04:13.000000 songline-0.0.2/songline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 06:04:13.000000 songline-0.0.2/songline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 06:04:13.000000 songline-0.0.2/songline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 06:04:13.000000 songline-0.0.2/songline.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `songline-0.0.1/setup.py` & `songline-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from distutils.core import setup
-
 from os import path
-
-here = path.abspath(path.dirname(__file__))
-
-# Get the long description from the README file
-with open(path.join(here, 'README.txt'), encoding='utf-8') as f:
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
-    print(long_description)
 
 setup(
   name = 'songline',         # How you named your package folder (MyLib)
   packages = ['songline'],   # Chose the same as "name"
-  version = '0.0.1',      # Start with a small number and increase it with every change you make
+  version = '0.0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Send Message, Sticker ,Image to LINE',   # Give a short description about your library
   long_description=long_description,
+  long_description_content_type="text/markdown",
   author = 'Loong Wissawakorn (Uncle Engineer)',                   # Type in your name
   author_email = 'loong.wissawakorn@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/UncleEngineer/songline',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/UncleEngineer/songline/archive/v_001.tar.gz',    # I explain this later on
   keywords = ['Python', 'Uncle Engineer','LINE API'],   # Keywords that define your package best
   install_requires=[
           'requests',
```

