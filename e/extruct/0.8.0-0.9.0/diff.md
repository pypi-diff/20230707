# Comparing `tmp/extruct-0.8.0.tar.gz` & `tmp/extruct-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/extruct-0.8.0.tar", last modified: Mon Oct  7 11:26:07 2019, max compression
+gzip compressed data, was "dist/extruct-0.9.0.tar", last modified: Mon Apr 20 15:01:16 2020, max compression
```

## Comparing `extruct-0.8.0.tar` & `extruct-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-07 11:26:07.000000 extruct-0.8.0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct/
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2175 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/tool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      345 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/microformat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7632 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/w3cmicrodata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4649 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/xmldom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2630 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/uniform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5682 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/_extruct.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1694 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/rdfa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/opengraph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      278 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1275 2019-10-07 11:25:27.000000 extruct-0.8.0/extruct/jsonld.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      910 2019-10-07 11:26:07.000000 extruct-0.8.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      910 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      484 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      109 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2019-10-07 11:26:07.000000 extruct-0.8.0/extruct.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2019-10-07 11:26:07.000000 extruct-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    35471 2019-10-07 11:25:27.000000 extruct-0.8.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1747 2019-10-07 11:25:27.000000 extruct-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-20 15:01:16.000000 extruct-0.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/VERSION
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2175 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/tool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      345 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/microformat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7632 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/w3cmicrodata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4649 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/xmldom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2630 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/uniform.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5682 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/_extruct.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1694 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/rdfa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/opengraph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      278 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1275 2020-04-20 15:00:46.000000 extruct-0.9.0/extruct/jsonld.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      886 2020-04-20 15:01:16.000000 extruct-0.9.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      886 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      465 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2020-04-20 15:01:16.000000 extruct-0.9.0/extruct.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-04-20 15:01:16.000000 extruct-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30527 2020-04-20 15:00:46.000000 extruct-0.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1649 2020-04-20 15:00:46.000000 extruct-0.9.0/setup.py
```

### Comparing `extruct-0.8.0/extruct/tool.py` & `extruct-0.9.0/extruct/tool.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/extruct/w3cmicrodata.py` & `extruct-0.9.0/extruct/w3cmicrodata.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/extruct/xmldom.py` & `extruct-0.9.0/extruct/xmldom.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/extruct/uniform.py` & `extruct-0.9.0/extruct/uniform.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/extruct/_extruct.py` & `extruct-0.9.0/extruct/_extruct.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/extruct/rdfa.py` & `extruct-0.9.0/extruct/rdfa.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/extruct/opengraph.py` & `extruct-0.9.0/extruct/opengraph.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/extruct/jsonld.py` & `extruct-0.9.0/extruct/jsonld.py`

 * *Files identical despite different names*

### Comparing `extruct-0.8.0/PKG-INFO` & `extruct-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extruct
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extract embedded metadata from HTML markup
 Home-page: https://github.com/scrapinghub/extruct
 Author: Scrapinghub
 Author-email: info@scrapinghub.com
 Maintainer: Scrapinghub
 Maintainer-email: info@scrapinghub.com
 License: UNKNOWN
@@ -19,8 +19,7 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: cli
-Provides-Extra: service
```

### Comparing `extruct-0.8.0/extruct.egg-info/PKG-INFO` & `extruct-0.9.0/extruct.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extruct
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extract embedded metadata from HTML markup
 Home-page: https://github.com/scrapinghub/extruct
 Author: Scrapinghub
 Author-email: info@scrapinghub.com
 Maintainer: Scrapinghub
 Maintainer-email: info@scrapinghub.com
 License: UNKNOWN
@@ -19,8 +19,7 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: cli
-Provides-Extra: service
```

### Comparing `extruct-0.8.0/README.rst` & `extruct-0.9.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 .. image:: https://img.shields.io/pypi/v/extruct.svg
    :target: https://pypi.python.org/pypi/extruct
    :alt: PyPI Version
 
 
 *extruct* is a library for extracting embedded metadata from HTML markup.
 
-It also has a built-in HTTP server to test its output as JSON.
-
 Currently, *extruct* supports:
 
 - `W3C's HTML Microdata`_
 - `embedded JSON-LD`_
 - `Microformat`_ via `mf2py`_
 - `Facebook's Open Graph`_
 - (experimental) `RDFa`_ via `rdflib`_
@@ -582,112 +580,14 @@
                 "html": "\n<p>Blah blah blah</p>\n",
                 "value": "\nBlah blah blah\n"
             }
         ]
       }
    }]
 
-REST API service
-----------------
-
-*extruct* also ships with a REST API service to test its output from URLs.
-
-Dependencies
-++++++++++++
-
-* bottle_ (Web framework)
-* gevent_ (Aysnc framework)
-* requests_
-
-.. _bottle: https://pypi.python.org/pypi/bottle
-.. _gevent: http://www.gevent.org/
-.. _requests: http://docs.python-requests.org/
-
-Usage
-+++++
-
-::
-
-    python -m extruct.service
-
-launches an HTTP server listening on port 10005.
-
-Methods supported
-+++++++++++++++++
-
-::
-
-    /extruct/<URL>
-    method = GET
-
-
-    /extruct/batch
-    method = POST
-    params:
-        urls - a list of URLs separted by newlines
-        urlsfile - a file with one URL per line
-
-E.g. http://localhost:10005/extruct/http://www.sarenza.com/i-love-shoes-susket-s767163-p0000119412
-
-will output something like this:
-
->>>
-{ 'json-ld': [ { '@context': 'http://schema.org',
-                 '@id': 'FP',
-                 '@type': 'Product',
-                 'brand': { '@type': 'Brand',
-                            'url': 'https://www.sarenza.com/i-love-shoes'},
-                 'color': ['Lava', 'Black', 'Lt grey'],
-                 'image': [ 'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_09.jpg?201509221045&v=20180313113923',
-                            'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_02.jpg?201509291747&v=20180313113923',
-                            'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_03.jpg?201509221045&v=20180313113923',
-                            'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_04.jpg?201509221045&v=20180313113923',
-                            'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_05.jpg?201509221045&v=20180313113923',
-                            'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_06.jpg?201509221045&v=20180313113923',
-                            'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_07.jpg?201509221045&v=20180313113923',
-                            'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_08.jpg?201509221045&v=20180313113923'],
-                 'name': 'Susket',
-                 'offers': { '@type': 'AggregateOffer',
-                             'availability': 'InStock',
-                             'highPrice': '49.00',
-                             'lowPrice': '0.00',
-                             'price': '0.00',
-                             'priceCurrency': 'EUR'}}],
-  'microdata': [ { 'properties': { 'average': '4.7',
-                                   'best': '5',
-                                   'itemreviewed': 'Sarenza',
-                                   'rating': '4.7 / 5\n\t\t  (4 066 avis)',
-                                   'votes': '4 066'},
-                   'type': 'http://data-vocabulary.org/Review-aggregate'}],
-  'microformat': [],
-  'opengraph': [ { 'namespace': {'og': 'http://ogp.me/ns#'},
-                   'properties': [ ( 'og:title',
-                                     'I Love Shoes Susket @sarenza.com'),
-                                   ( 'og:image',
-                                     'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_09.jpg?201509221045&v=20180313113923'),
-                                   ('og:site_name', 'sarenza.com'),
-                                   ('og:type', 'product'),
-                                   ('og:description', '...'),
-                                   ( 'og:url',
-                                     'https://www.sarenza.com/i-love-shoes-susket-s767163-p0000119412'),
-                                   ('og:country-name', 'FRA')]}],
-  'rdfa': [ { '@id': 'https://www.sarenza.com/i-love-shoes-susket-s767163-p0000119412',
-              'http://ogp.me/ns#country-name': [{'@value': 'FRA'}],
-              'http://ogp.me/ns#description': [{'@value': '...'}],
-              'http://ogp.me/ns#image': [ { '@value': 'https://cdn.sarenza.net/_img/productsv4/0000119412/MD_0000119412_223992_09.jpg?201509221045&v=20180313113923'}],
-              'http://ogp.me/ns#site_name': [{'@value': 'sarenza.com'}],
-              'http://ogp.me/ns#title': [ { '@value': 'I Love Shoes Susket '
-                                                      '@sarenza.com'}],
-              'http://ogp.me/ns#type': [{'@value': 'product'}],
-              'http://ogp.me/ns#url': [ { '@value': 'https://www.sarenza.com/i-love-shoes-susket-s767163-p0000119412'}],
-              'http://ogp.me/ns/fb#admins': [{'@value': '100001934697625'}],
-              'http://ogp.me/ns/fb#app_id': [{'@value': '148128758532914'}]},
-            { '@id': '_:Ncf1962068aa142b29000813372db7841',
-              'http://www.w3.org/1999/xhtml/vocab#role': [ { '@id': 'http://www.w3.org/1999/xhtml/vocab#navigation'}]}]}
-
 
 Command Line Tool
 -----------------
 
 *extruct* provides a command line tool that allows you to fetch a page and
 extract the metadata from it directly from the command line.
```

### Comparing `extruct-0.8.0/setup.py` & `extruct-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,27 +24,22 @@
     entry_points={
         'console_scripts': {
             'extruct = extruct.tool:main',
         }
     },
     packages=find_packages(exclude=['tests',]),
     package_data={'extruct': ['VERSION']},
-    install_requires=['lxml', 
-                      'rdflib', 
-                      'rdflib-jsonld', 
-                      'mf2py', 
+    install_requires=['lxml',
+                      'rdflib<5.0.0',
+                      'rdflib-jsonld',
+                      'mf2py',
                       'w3lib',
                       'html-text>=0.5.1',
                       'six'],
     extras_require={
-        'service': [
-            'bottle',
-            'gevent',
-            'requests',
-        ],
         'cli': [
             'requests',
         ],
     },
     keywords='extruct',
     classifiers=[
         'Development Status :: 4 - Beta',
```

