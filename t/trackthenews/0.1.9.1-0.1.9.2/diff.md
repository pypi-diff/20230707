# Comparing `tmp/trackthenews-0.1.9.1.tar.gz` & `tmp/trackthenews-0.1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trackthenews-0.1.9.1.tar", last modified: Tue Jul  3 19:33:37 2018, max compression
+gzip compressed data, was "dist/trackthenews-0.1.9.2.tar", last modified: Mon Jul 23 21:38:42 2018, max compression
```

## Comparing `trackthenews-0.1.9.1.tar` & `trackthenews-0.1.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/
--rw-rw-r--   0 parker    (1000) parker    (1000)     3887 2018-07-03 14:08:30.000000 trackthenews-0.1.9.1/README.md
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews/
--rw-rw-r--   0 parker    (1000) parker    (1000)       20 2018-06-18 23:07:44.000000 trackthenews-0.1.9.1/trackthenews/__init__.py
--rwxrwxr-x   0 parker    (1000) parker    (1000)    15422 2018-07-03 19:23:11.000000 trackthenews-0.1.9.1/trackthenews/core.py
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews/fonts/
--rw-rw-r--   0 parker    (1000) parker    (1000)     4301 2018-06-18 23:07:44.000000 trackthenews-0.1.9.1/trackthenews/fonts/LICENSE_OFL.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)   552144 2018-06-18 23:07:44.000000 trackthenews-0.1.9.1/trackthenews/fonts/NotoSerif-Regular.ttf
--rwxrwxr-x   0 parker    (1000) parker    (1000)     1049 2018-07-03 19:32:09.000000 trackthenews-0.1.9.1/setup.py
--rw-rw-r--   0 parker    (1000) parker    (1000)       29 2018-06-19 20:58:47.000000 trackthenews-0.1.9.1/MANIFEST.in
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews.egg-info/
--rw-rw-r--   0 parker    (1000) parker    (1000)       13 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews.egg-info/top_level.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)        1 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews.egg-info/dependency_links.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)     5001 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews.egg-info/PKG-INFO
--rw-rw-r--   0 parker    (1000) parker    (1000)       52 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews.egg-info/entry_points.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)      171 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews.egg-info/requires.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)      370 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/trackthenews.egg-info/SOURCES.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)     5001 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/PKG-INFO
--rw-rw-r--   0 parker    (1000) parker    (1000)       38 2018-07-03 19:33:37.000000 trackthenews-0.1.9.1/setup.cfg
+drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/
+-rw-rw-r--   0 parker    (1000) parker    (1000)     3887 2018-07-03 14:08:30.000000 trackthenews-0.1.9.2/README.md
+drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews/
+-rw-rw-r--   0 parker    (1000) parker    (1000)       20 2018-06-18 23:07:44.000000 trackthenews-0.1.9.2/trackthenews/__init__.py
+-rwxrwxr-x   0 parker    (1000) parker    (1000)    15371 2018-07-23 21:30:57.000000 trackthenews-0.1.9.2/trackthenews/core.py
+drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews/fonts/
+-rw-rw-r--   0 parker    (1000) parker    (1000)     4301 2018-06-18 23:07:44.000000 trackthenews-0.1.9.2/trackthenews/fonts/LICENSE_OFL.txt
+-rw-rw-r--   0 parker    (1000) parker    (1000)   552144 2018-06-18 23:07:44.000000 trackthenews-0.1.9.2/trackthenews/fonts/NotoSerif-Regular.ttf
+-rwxrwxr-x   0 parker    (1000) parker    (1000)     1049 2018-07-23 21:34:43.000000 trackthenews-0.1.9.2/setup.py
+-rw-rw-r--   0 parker    (1000) parker    (1000)       29 2018-06-19 20:58:47.000000 trackthenews-0.1.9.2/MANIFEST.in
+drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/
+-rw-rw-r--   0 parker    (1000) parker    (1000)       13 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/top_level.txt
+-rw-rw-r--   0 parker    (1000) parker    (1000)        1 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/dependency_links.txt
+-rw-rw-r--   0 parker    (1000) parker    (1000)     5001 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/PKG-INFO
+-rw-rw-r--   0 parker    (1000) parker    (1000)       52 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/entry_points.txt
+-rw-rw-r--   0 parker    (1000) parker    (1000)      171 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/requires.txt
+-rw-rw-r--   0 parker    (1000) parker    (1000)      370 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/SOURCES.txt
+-rw-rw-r--   0 parker    (1000) parker    (1000)     5001 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/PKG-INFO
+-rw-rw-r--   0 parker    (1000) parker    (1000)       38 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/setup.cfg
```

### Comparing `trackthenews-0.1.9.1/README.md` & `trackthenews-0.1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `trackthenews-0.1.9.1/trackthenews/core.py` & `trackthenews-0.1.9.2/trackthenews/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import sqlite3
 import time
 import textwrap
 import sys
 
 from datetime import datetime
-from io import BytesIO
+from io import BytesIO, open
 from builtins import input
 
 import feedparser
 import html2text
 import requests
 import yaml
 
@@ -228,15 +228,15 @@
     return config
 
 def setup_db(config):
     database = os.path.join(home, config['db'])
     if not os.path.isfile(database):
         conn = sqlite3.connect(database)
         schema_script = """create table articles (
-            id          integer primary key autoincrement not null,
+            id          integer primary key not null,
             title       text,
             outlet      text,
             url         text,
             tweeted     boolean,
             recorded_at datetime
         );"""
         conn.executescript(schema_script)
@@ -279,15 +279,15 @@
     return
 
 
 def initial_setup():
     configfile = os.path.join(home, 'config.yaml')
 
     if os.path.isfile(configfile):
-        with open(configfile, 'r') as f:
+        with open(configfile, 'r', encoding="utf-8") as f:
             config = yaml.load(f)
     else:
         to_configure = input("It looks like this is the first time you've run trackthenews, or you've moved or deleted its configuration files.\nWould you like to create a new configuration in {}? (Y/n) ".format(home))
 
         config = {}
     
         if to_configure.lower() in ['n','no','q','exit','quit']:
@@ -349,15 +349,15 @@
         sys.exit("Created new configuration files. Now go populate the RSS Feed file and the list of matchwords!")
 
     configfile = os.path.join(home, 'config.yaml')
     if not os.path.isfile(configfile):
         initial_setup()
 
     global config
-    with open(configfile) as f:
+    with open(configfile, encoding="utf-8") as f:
         config = yaml.load(f)
 
     global ua
     ua = config['user-agent']
 
     database = os.path.join(home, config['db'])
     if not os.path.isfile(database):
@@ -370,17 +370,17 @@
     matchlist_case_sensitive = os.path.join(home, 'matchlist_case_sensitive.txt')
     if not (os.path.isfile(matchlist) and \
             os.path.isfile(matchlist_case_sensitive)):
         setup_matchlist()
 
     global matchwords
     global matchwords_case_sensitive
-    with open(matchlist, 'r') as f:
+    with open(matchlist, 'r', encoding="utf-8") as f:
         matchwords = [w for w in f.read().split('\n') if w]
-    with open(matchlist_case_sensitive, 'r') as f:
+    with open(matchlist_case_sensitive, 'r', encoding="utf-8") as f:
         matchwords_case_sensitive = [w for w in f.read().split('\n') if w]
  
     if not (matchwords or matchwords_case_sensitive):
             sys.exit("You must add words to at least one of the matchwords lists, located at {} and {}.".format(matchlist, matchlist_case_sensitive))
 
     sys.path.append(home)
     global blocklist_loaded
@@ -399,15 +399,15 @@
         print("Matching against the following case-sensitive words: {}".format(
             matchwords_case_sensitive))
 
     rssfeedsfile = os.path.join(home, 'rssfeeds.json')
     if not os.path.isfile(rssfeedsfile):
         setup_rssfeedsfile()
 
-    with open(rssfeedsfile, 'r') as f:
+    with open(rssfeedsfile, 'r', encoding="utf-8") as f:
         try:
             rss_feeds = json.load(f)
         except json.JSONDecodeError:
             sys.exit("You must add RSS feeds to the RSS feeds list, located at {}.".format(rssfeedsfile))
 
     for feed in rss_feeds:
         outlet = feed['outlet'] if 'outlet' in feed else ''
@@ -423,17 +423,14 @@
         for article in articles:
             article_exists = conn.execute('select * from articles where url = ?',
                     (article.url,)).fetchall()
             if not article_exists:
                 deduped.append(article)
 
         for counter, article in enumerate(deduped, 1):
-            # aquire exclusive access here since changes are commited later int he loop
-            conn.execute('BEGIN EXCLUSIVE')
-
             print('Checking {} article {}/{}'.format(
                 article.outlet, counter, len(deduped)))
 
             try:
                 article.check_for_matches()
             except:
                 print('Having trouble with that article. Skipping for now.')
```

### Comparing `trackthenews-0.1.9.1/trackthenews/fonts/LICENSE_OFL.txt` & `trackthenews-0.1.9.2/trackthenews/fonts/LICENSE_OFL.txt`

 * *Files identical despite different names*

### Comparing `trackthenews-0.1.9.1/trackthenews/fonts/NotoSerif-Regular.ttf` & `trackthenews-0.1.9.2/trackthenews/fonts/NotoSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `trackthenews-0.1.9.1/setup.py` & `trackthenews-0.1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = f.read().split()
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='trackthenews',
-    version='0.1.9.1',
+    version='0.1.9.2',
     description='Monitor RSS feeds for keywords and act on matching results. A special project of the Freedom of the Press Foundation.',
     long_description=readme,
     long_description_content_type='text/markdown',
     install_requires=reqs,
     author='Parker Higgins',
     author_email='parker@freedom.press',
     url='https://github.com/freedomofpress/trackthenews',
```

### Comparing `trackthenews-0.1.9.1/trackthenews.egg-info/PKG-INFO` & `trackthenews-0.1.9.2/trackthenews.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackthenews
-Version: 0.1.9.1
+Version: 0.1.9.2
 Summary: Monitor RSS feeds for keywords and act on matching results. A special project of the Freedom of the Press Foundation.
 Home-page: https://github.com/freedomofpress/trackthenews
 Author: Parker Higgins
 Author-email: parker@freedom.press
 License: MIT
 Description: # Track The News
```

### Comparing `trackthenews-0.1.9.1/PKG-INFO` & `trackthenews-0.1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackthenews
-Version: 0.1.9.1
+Version: 0.1.9.2
 Summary: Monitor RSS feeds for keywords and act on matching results. A special project of the Freedom of the Press Foundation.
 Home-page: https://github.com/freedomofpress/trackthenews
 Author: Parker Higgins
 Author-email: parker@freedom.press
 License: MIT
 Description: # Track The News
```

