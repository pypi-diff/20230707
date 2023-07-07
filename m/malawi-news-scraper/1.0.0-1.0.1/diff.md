# Comparing `tmp/malawi-news-scraper-1.0.0.tar.gz` & `tmp/malawi-news-scraper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malawi-news-scraper-1.0.0.tar", last modified: Fri Jul  7 17:37:57 2023, max compression
+gzip compressed data, was "malawi-news-scraper-1.0.1.tar", last modified: Fri Jul  7 19:04:04 2023, max compression
```

## Comparing `malawi-news-scraper-1.0.0.tar` & `malawi-news-scraper-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 17:37:57.695643 malawi-news-scraper-1.0.0/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1069 2023-07-07 16:47:56.000000 malawi-news-scraper-1.0.0/LICENSE
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 17:37:57.691643 malawi-news-scraper-1.0.0/PKG-INFO
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       69 2023-07-07 16:47:56.000000 malawi-news-scraper-1.0.0/README.md
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1125 2023-07-07 17:29:30.000000 malawi-news-scraper-1.0.0/pyproject.toml
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       38 2023-07-07 17:37:57.695643 malawi-news-scraper-1.0.0/setup.cfg
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 17:37:57.691643 malawi-news-scraper-1.0.0/src/
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 17:37:57.691643 malawi-news-scraper-1.0.0/src/malawi_news_scraper.egg-info/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 17:37:57.000000 malawi-news-scraper-1.0.0/src/malawi_news_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      341 2023-07-07 17:37:57.000000 malawi-news-scraper-1.0.0/src/malawi_news_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        1 2023-07-07 17:37:57.000000 malawi-news-scraper-1.0.0/src/malawi_news_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       88 2023-07-07 17:37:57.000000 malawi-news-scraper-1.0.0/src/malawi_news_scraper.egg-info/requires.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        9 2023-07-07 17:37:57.000000 malawi-news-scraper-1.0.0/src/malawi_news_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 17:37:57.691643 malawi-news-scraper-1.0.0/src/scrapers/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      233 2023-07-07 17:29:40.000000 malawi-news-scraper-1.0.0/src/scrapers/__init__.py
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      133 2023-07-07 16:34:58.000000 malawi-news-scraper-1.0.0/src/scrapers/main.py
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1989 2023-07-07 16:55:45.000000 malawi-news-scraper-1.0.0/src/scrapers/malawi_voice.py
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1069 2023-07-07 16:47:56.000000 malawi-news-scraper-1.0.1/LICENSE
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       27 2023-07-07 18:00:31.000000 malawi-news-scraper-1.0.1/MANIFEST.in
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/PKG-INFO
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       69 2023-07-07 16:47:56.000000 malawi-news-scraper-1.0.1/README.md
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1130 2023-07-07 19:01:54.000000 malawi-news-scraper-1.0.1/pyproject.toml
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       38 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/setup.cfg
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.111206 malawi-news-scraper-1.0.1/src/
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      357 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        1 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       87 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/requires.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        9 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/src/scrapers/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      233 2023-07-07 19:01:54.000000 malawi-news-scraper-1.0.1/src/scrapers/__init__.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       65 2023-07-07 16:17:05.000000 malawi-news-scraper-1.0.1/src/scrapers/config.toml
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1989 2023-07-07 16:55:45.000000 malawi-news-scraper-1.0.1/src/scrapers/malawi_voice.py
```

### Comparing `malawi-news-scraper-1.0.0/LICENSE` & `malawi-news-scraper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `malawi-news-scraper-1.0.0/PKG-INFO` & `malawi-news-scraper-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malawi-news-scraper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scrape news from known news outlets in Malawi
 Author-email: Hopson Gausi <hopgausi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hopson Gausi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `malawi-news-scraper-1.0.0/pyproject.toml` & `malawi-news-scraper-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 [build-system]
-requires = ['setuptools>=61.0.0', 'wheel']
+requires = ['setuptools>=1.0.1', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'malawi-news-scraper'
-version = '1.0.0'
+version = '1.0.1'
 description = 'Scrape news from known news outlets in Malawi'
 readme = 'README.md'
 authors = [{ name = 'Hopson Gausi', email = 'hopgausi@gmail.com' }]
 license = { file = 'LICENSE' }
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
 ]
 keywords = ['News scraper', 'scraper', 'malawi']
 dependencies = [
-    'feedparser >= 6.0.10',
+    'feedparser >= 1.0.1',
     'html2text',
     'beautifulsoup4'
 ]
 requires-python = '>=3.11'
 
 [project.optional-dependencies]
 dev = ['black', 'bumpver', 'isort', 'pip-tools', 'pytest']
 
 [project.urls]
 Homepage = 'https://github.com/hopgausi/malawi-news-scraper'
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = 'MAJOR.MINOR.PATCH'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
-push = true
+push = false
 
 [tool.bumpver.file_patterns]
-"pyproject.toml" = [
-    'current_version = "{version}"',
-]
+"pyproject.toml" = ['current_version = "{version}"', "{version}"]
 "src/scrapers/__init__.py" = ["{version}"]
```

### Comparing `malawi-news-scraper-1.0.0/src/malawi_news_scraper.egg-info/PKG-INFO` & `malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malawi-news-scraper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scrape news from known news outlets in Malawi
 Author-email: Hopson Gausi <hopgausi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hopson Gausi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `malawi-news-scraper-1.0.0/src/scrapers/malawi_voice.py` & `malawi-news-scraper-1.0.1/src/scrapers/malawi_voice.py`

 * *Files identical despite different names*

