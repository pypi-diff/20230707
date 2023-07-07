# Comparing `tmp/malawi-news-scraper-1.0.1.tar.gz` & `tmp/malawi-news-scraper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malawi-news-scraper-1.0.1.tar", last modified: Fri Jul  7 19:04:04 2023, max compression
+gzip compressed data, was "malawi-news-scraper-1.1.0.tar", last modified: Fri Jul  7 20:12:51 2023, max compression
```

## Comparing `malawi-news-scraper-1.0.1.tar` & `malawi-news-scraper-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1069 2023-07-07 16:47:56.000000 malawi-news-scraper-1.0.1/LICENSE
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       27 2023-07-07 18:00:31.000000 malawi-news-scraper-1.0.1/MANIFEST.in
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/PKG-INFO
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       69 2023-07-07 16:47:56.000000 malawi-news-scraper-1.0.1/README.md
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1130 2023-07-07 19:01:54.000000 malawi-news-scraper-1.0.1/pyproject.toml
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       38 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/setup.cfg
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.111206 malawi-news-scraper-1.0.1/src/
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      357 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        1 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       87 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/requires.txt
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        9 2023-07-07 19:04:04.000000 malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 19:04:04.115206 malawi-news-scraper-1.0.1/src/scrapers/
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      233 2023-07-07 19:01:54.000000 malawi-news-scraper-1.0.1/src/scrapers/__init__.py
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       65 2023-07-07 16:17:05.000000 malawi-news-scraper-1.0.1/src/scrapers/config.toml
--rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1989 2023-07-07 16:55:45.000000 malawi-news-scraper-1.0.1/src/scrapers/malawi_voice.py
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:12:51.201443 malawi-news-scraper-1.1.0/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1069 2023-07-07 16:47:56.000000 malawi-news-scraper-1.1.0/LICENSE
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       27 2023-07-07 18:00:31.000000 malawi-news-scraper-1.1.0/MANIFEST.in
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 20:12:51.201443 malawi-news-scraper-1.1.0/PKG-INFO
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       69 2023-07-07 16:47:56.000000 malawi-news-scraper-1.1.0/README.md
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1129 2023-07-07 20:09:19.000000 malawi-news-scraper-1.1.0/pyproject.toml
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       38 2023-07-07 20:12:51.201443 malawi-news-scraper-1.1.0/setup.cfg
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:12:51.197443 malawi-news-scraper-1.1.0/src/
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:12:51.201443 malawi-news-scraper-1.1.0/src/malawi_news_scraper.egg-info/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     1840 2023-07-07 20:12:51.000000 malawi-news-scraper-1.1.0/src/malawi_news_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      447 2023-07-07 20:12:51.000000 malawi-news-scraper-1.1.0/src/malawi_news_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        1 2023-07-07 20:12:51.000000 malawi-news-scraper-1.1.0/src/malawi_news_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)       87 2023-07-07 20:12:51.000000 malawi-news-scraper-1.1.0/src/malawi_news_scraper.egg-info/requires.txt
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)        9 2023-07-07 20:12:51.000000 malawi-news-scraper-1.1.0/src/malawi_news_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 hopgausi  (1000) hopgausi  (1000)        0 2023-07-07 20:12:51.201443 malawi-news-scraper-1.1.0/src/scrapers/
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      287 2023-07-07 20:09:19.000000 malawi-news-scraper-1.1.0/src/scrapers/__init__.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)     2044 2023-07-07 20:01:58.000000 malawi-news-scraper-1.1.0/src/scrapers/base_feed_scraper.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      298 2023-07-07 20:02:31.000000 malawi-news-scraper-1.1.0/src/scrapers/base_parser.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      114 2023-07-07 19:36:50.000000 malawi-news-scraper-1.1.0/src/scrapers/config.toml
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      153 2023-07-07 20:11:38.000000 malawi-news-scraper-1.1.0/src/scrapers/malawi_voice.py
+-rw-rw-r--   0 hopgausi  (1000) hopgausi  (1000)      151 2023-07-07 20:07:23.000000 malawi-news-scraper-1.1.0/src/scrapers/maravi_post.py
```

### Comparing `malawi-news-scraper-1.0.1/LICENSE` & `malawi-news-scraper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malawi-news-scraper-1.0.1/PKG-INFO` & `malawi-news-scraper-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malawi-news-scraper
-Version: 1.0.1
+Version: 1.1.0
 Summary: Scrape news from known news outlets in Malawi
 Author-email: Hopson Gausi <hopgausi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hopson Gausi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `malawi-news-scraper-1.0.1/pyproject.toml` & `malawi-news-scraper-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
-requires = ['setuptools>=1.0.1', 'wheel']
+requires = ['setuptools>=1.1.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'malawi-news-scraper'
-version = '1.0.1'
+version = '1.1.0'
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
-    'feedparser >= 1.0.1',
+    'feedparser >= 1.1.0',
     'html2text',
     'beautifulsoup4'
 ]
 requires-python = '>=3.11'
 
 [project.optional-dependencies]
 dev = ['black', 'bumpver', 'isort', 'pip-tools', 'pytest']
 
 [project.urls]
 Homepage = 'https://github.com/hopgausi/malawi-news-scraper'
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.1.0"
 version_pattern = 'MAJOR.MINOR.PATCH'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
-push = false
+push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', "{version}"]
 "src/scrapers/__init__.py" = ["{version}"]
```

### Comparing `malawi-news-scraper-1.0.1/src/malawi_news_scraper.egg-info/PKG-INFO` & `malawi-news-scraper-1.1.0/src/malawi_news_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malawi-news-scraper
-Version: 1.0.1
+Version: 1.1.0
 Summary: Scrape news from known news outlets in Malawi
 Author-email: Hopson Gausi <hopgausi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hopson Gausi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `malawi-news-scraper-1.0.1/src/scrapers/malawi_voice.py` & `malawi-news-scraper-1.1.0/src/scrapers/base_feed_scraper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import feedparser
 from bs4 import BeautifulSoup
-import scrapers
 from functools import cache
 
-class MalawiVoiceScraper:
+class BaseFeedScraper:
     def __init__(self):
-        self.link = scrapers.MALAWI_VOICE_URL
+        self.link = self.get_link()
+
+    def get_link(self):
+        return None 
     
     def scrape_news(self)-> dict:
         """ Scrape the news feed, and return a list of news articles and source details."""
         parsed_xml_news = self._get_xml_news()
         return self._sanitize_news(parsed_xml_news)
     
     @cache
@@ -38,16 +40,17 @@
             'data': sanitized_news,
             'source': self._get_source_details(parsed_xml_news.feed)
         }
             
     def _get_image_url(self, content: str)->str:
         """Returns the image url for the given content news feed"""
         soup = BeautifulSoup(content, 'html.parser')
-        img_tag = soup.find('figure').find('img')
-        return img_tag['src']
+        img_tag = soup.find_all('img')
+        img = img_tag[0]['src'] if len(img_tag) > 0 else ''
+        return img
     
     def _get_source_details(self, feed: dict) -> dict:
         """Returns the source details for the news, that is, the site the feed is being scraped from"""
         source_details = {
             'name': feed['title'],
             'url': feed['link'],
             'mission_statement': feed['subtitle'],
```

