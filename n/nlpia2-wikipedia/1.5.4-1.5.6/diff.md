# Comparing `tmp/nlpia2_wikipedia-1.5.4.tar.gz` & `tmp/nlpia2_wikipedia-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpia2_wikipedia-1.5.4.tar", max compression
+gzip compressed data, was "nlpia2_wikipedia-1.5.6.tar", max compression
```

## Comparing `nlpia2_wikipedia-1.5.4.tar` & `nlpia2_wikipedia-1.5.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1057 2022-02-24 21:47:29.044908 nlpia2_wikipedia-1.5.4/LICENSE
--rw-r--r--   0        0        0     3798 2022-05-04 23:25:18.637807 nlpia2_wikipedia-1.5.4/README.md
--rw-r--r--   0        0        0     1633 2023-07-04 22:26:53.425674 nlpia2_wikipedia-1.5.4/pyproject.toml
--rw-r--r--   0        0        0       99 2023-07-01 00:11:01.060006 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/__init__.py
--rw-r--r--   0        0        0     2420 2023-06-30 23:36:01.865166 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/exceptions.py
--rw-r--r--   0        0        0      184 2023-07-04 20:01:10.064999 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/parsers.py
--rw-r--r--   0        0        0     2873 2023-07-04 22:12:15.959850 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/util.py
--rw-r--r--   0        0        0    26553 2023-07-04 21:56:30.536368 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/wikipedia.py
--rw-r--r--   0        0        0     4788 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.4/setup.py
--rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-02-24 21:47:29.044908 nlpia2_wikipedia-1.5.6/LICENSE
+-rw-r--r--   0        0        0     3798 2022-05-04 23:25:18.637807 nlpia2_wikipedia-1.5.6/README.md
+-rw-r--r--   0        0        0     1635 2023-07-07 00:23:31.596193 nlpia2_wikipedia-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-07-06 23:18:10.526524 nlpia2_wikipedia-1.5.6/src/wikipedia/__init__.py
+-rw-r--r--   0        0        0     2420 2023-06-30 23:36:01.865166 nlpia2_wikipedia-1.5.6/src/wikipedia/exceptions.py
+-rw-r--r--   0        0        0      184 2023-07-04 20:01:10.064999 nlpia2_wikipedia-1.5.6/src/wikipedia/parsers.py
+-rw-r--r--   0        0        0     2873 2023-07-04 22:12:15.959850 nlpia2_wikipedia-1.5.6/src/wikipedia/util.py
+-rw-r--r--   0        0        0    28098 2023-07-06 23:20:48.523524 nlpia2_wikipedia-1.5.6/src/wikipedia/wikipedia.py
+-rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.6/setup.py
+-rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.6/PKG-INFO
```

### Comparing `nlpia2_wikipedia-1.5.4/LICENSE` & `nlpia2_wikipedia-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.4/README.md` & `nlpia2_wikipedia-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.4/pyproject.toml` & `nlpia2_wikipedia-1.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nlpia2_wikipedia"
-version = "1.5.4"
+version = "1.5.6"
 description = "Updated version of `wikipedia` package because original repo has been abandoned since 2014."
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 authors = [
     "Hobson Lane <hobson@tangibleai.com>",
     ]
 homepage = "https://gitlab.com/tangibleai/community/nlpia2_wikipedia"
 repository = "https://gitlab.com/tangibleai/community/nlpia2_wikipedia"
 documentation = "https://gitlab.com/tangibleai/community/nlpia2_wikipedia"
 packages = [
-    {include="nlpia2_wikipedia", from="src"},
+    {include="wikipedia", from="src"},
     ]
 
 
 
 keywords = [
     'wiki',
     'Wikipedia',
@@ -49,15 +49,15 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 poetry = ">=1.1"
 beautifulsoup4 = ">=4.11"
 requests = ">=2.0,<3.0.0"
-pandas = ">=2.0"
+pandas = ">=1.5.3,<2.0.0"
 
 [tool.poetry.dev-dependencies]
 tox = ">=3.18"
 pytest = ">=6.2.0"
 pytest-cov = ">=3.0.0"
 pydocstyle = ">=5.1.1"
 Sphinx = ">=4.4.0"
```

### Comparing `nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/exceptions.py` & `nlpia2_wikipedia-1.5.6/src/wikipedia/exceptions.py`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/util.py` & `nlpia2_wikipedia-1.5.6/src/wikipedia/util.py`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/wikipedia.py` & `nlpia2_wikipedia-1.5.6/src/wikipedia/wikipedia.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import unicode_literals
 
 import logging
 import requests
 import time
-from bs4 import BeautifulSoup
 from datetime import datetime, timedelta
 from decimal import Decimal
 
 from .exceptions import (
     PageError, DisambiguationError, RedirectError, HTTPTimeoutError,
     WikipediaException, ODD_ERROR_MESSAGE
 )
+from bs4 import BeautifulSoup
 from .util import cache, stdout_encode
 from .util import debug  # noqa
 import pandas as pd
 import re
 
 log = logging.getLogger(__name__)
 
@@ -314,15 +314,16 @@
 
 class WikipediaPage(object):
     '''
     Contains data from a Wikipedia page.
     Uses property methods to filter data from the raw HTML.
     '''
 
-    def __init__(self, title=None, pageid=None, redirect=True, preload=False, original_title='', markdown=False):
+    def __init__(self, title=None, pageid=None, redirect=True, preload=False, original_title='', format='wikitext', version=1):
+        """ `format` and `version` ignored but will reflect package version major version so bump default version when improved parsers available"""
         # FIXME: parse page.content as markdown (headings with ## instead of ==
         if title is not None:
             self.title = title
             self.original_title = original_title or title
         elif pageid is not None:
             self.pageid = pageid
         else:
@@ -507,14 +508,44 @@
             request = _wiki_request(query_params)
             self._content = request['query']['pages'][self.pageid]['extract']
             self._revision_id = request['query']['pages'][self.pageid]['revisions'][0]['revid']
             self._parent_id = request['query']['pages'][self.pageid]['revisions'][0]['parentid']
 
         return self._content
 
+    def get_content(self):
+        """ Stub to allow improved parsing (sentence separating whitespace in HTML is deleted)
+
+        TODO:
+          - [ ] wiki.get_content() with improved parsing of sentence separators in HTML
+          - [ ] improved parsing to create .json()
+          - [ ] improved @property .json used within .content and .get_content
+            - .content utilizes __init__ setting that defaults to old parsing
+            - .get_content defaults to new parsing always (ignoring .__init__ setting
+          - [ ] with options in Wikipedia.__init__
+          - [ ] @property for md/markdown
+          - [ ] @property for adoc
+          - [ ] @property .rst/restructured_text
+          - [ ] @property .rtf/rich_text
+          - [ ] @property .wiki/wikitext
+          - [ ] get_content defaults to markdown instead of RST or wikitext
+          - [ ] __init__ options to control HTML parsing for json and default content format
+        """
+
+        return self.content
+
+
+    def get_html_paragraphs(self, html=None):
+        html = html or self.html()
+        soup = BeautifulSoup(html, 'html.parser')
+        self.paragraphs = [p.text for p in soup.select("p")]
+        soup_filtered = soup.find_all(['h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'p'])
+        self.paragraphs_with_headings = [x.text for x in soup_filtered] 
+        return self.paragraphs_with_headings
+
     @property
     def revision_id(self):
         '''
         Revision ID of the page.
 
         The revision ID is a number that uniquely identifies the current
         version of the page. It can be used to create the permalink or for
```

### Comparing `nlpia2_wikipedia-1.5.4/setup.py` & `nlpia2_wikipedia-1.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['nlpia2_wikipedia']
+['wikipedia']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beautifulsoup4>=4.11', 'pandas>=2.0', 'poetry>=1.1', 'requests>=2.0,<3.0.0']
+['beautifulsoup4>=4.11',
+ 'pandas>=1.5.3,<2.0.0',
+ 'poetry>=1.1',
+ 'requests>=2.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'nlpia2-wikipedia',
-    'version': '1.5.4',
+    'version': '1.5.6',
     'description': 'Updated version of `wikipedia` package because original repo has been abandoned since 2014.',
     'long_description': '# Wikipedia\n\n[![image](https://travis-ci.org/goldsmith/Wikipedia.png?branch=master)](https://travis-ci.org/goldsmith/Wikipedia)\n\n[![image](https://pypip.in/d/wikipedia/badge.png)](https://crate.io/packages/wikipedia)\n\n[![image](https://pypip.in/v/wikipedia/badge.png)](https://crate.io/packages/wikipedia)\n\n[![License](https://pypip.in/license/wikipedia/badge.png)](https://pypi.python.org/pypi/wikipedia/)\n\n**Wikipedia** is a Python library that makes it easy to access and parse\ndata from Wikipedia.\n\nSearch Wikipedia, get article summaries, get data like links and images\nfrom a page, and more. Wikipedia wraps the [MediaWiki\nAPI](https://www.mediawiki.org/wiki/API) so you can focus on using\nWikipedia data, not getting it.\n\n``` {.python}\n>>> import wikipedia\n>>> print wikipedia.summary("Wikipedia")\n# Wikipedia (/ˌwɪkɨˈpiːdiə/ or /ˌwɪkiˈpiːdiə/ WIK-i-PEE-dee-ə) is a collaboratively edited, multilingual, free Internet encyclopedia supported by the non-profit Wikimedia Foundation...\n\n>>> wikipedia.search("Barack")\n# [u\'Barak (given name)\', u\'Barack Obama\', u\'Barack (brandy)\', u\'Presidency of Barack Obama\', u\'Family of Barack Obama\', u\'First inauguration of Barack Obama\', u\'Barack Obama presidential campaign, 2008\', u\'Barack Obama, Sr.\', u\'Barack Obama citizenship conspiracy theories\', u\'Presidential transition of Barack Obama\']\n\n>>> ny = wikipedia.page("New York")\n>>> ny.title\n# u\'New York\'\n>>> ny.url\n# u\'http://en.wikipedia.org/wiki/New_York\'\n>>> ny.content\n# u\'New York is a state in the Northeastern region of the United States. New York is the 27th-most exten\'...\n>>> ny.links[0]\n# u\'1790 United States Census\'\n\n>>> wikipedia.set_lang("fr")\n>>> wikipedia.summary("Facebook", sentences=1)\n# Facebook est un service de réseautage social en ligne sur Internet permettant d\'y publier des informations (photographies, liens, textes, etc.) en contrôlant leur visibilité par différentes catégories de personnes.\n```\n\nNote: this library was designed for ease of use and simplicity, not for\nadvanced use. If you plan on doing serious scraping or automated\nrequests, please use\n[Pywikipediabot](http://www.mediawiki.org/wiki/Manual:Pywikipediabot)\n(or one of the other more advanced [Python MediaWiki API\nwrappers](http://en.wikipedia.org/wiki/Wikipedia:Creating_a_bot#Python)),\nwhich has a larger API, rate limiting, and other features so we can be\nconsiderate of the MediaWiki infrastructure.\n\n## Installation\n\nTo install Wikipedia, simply run:\n\n    $ pip install wikipedia\n\nWikipedia is compatible with Python 2.6+ (2.7+ to run unittest discover)\nand Python 3.3+.\n\n## Documentation\n\nRead the docs at <https://wikipedia.readthedocs.org/en/latest/>.\n\n-   [Quickstart](https://wikipedia.readthedocs.org/en/latest/quickstart.html)\n-   [Full API](https://wikipedia.readthedocs.org/en/latest/code.html)\n\nTo run tests, clone the [repository on\nGitHub](https://github.com/goldsmith/Wikipedia), then run:\n\n    $ pip install -r requirements.txt\n    $ bash runtests  # will run tests for python and python3\n    $ python -m unittest discover tests/ \'*test.py\'  # manual style\n\nin the root project directory.\n\nTo build the documentation yourself, after installing requirements.txt,\nrun:\n\n    $ pip install sphinx\n    $ cd docs/\n    $ make html\n\n## License\n\nMIT licensed. See the [LICENSE\nfile](https://github.com/goldsmith/Wikipedia/blob/master/LICENSE) for\nfull details.\n\n## Credits\n\n-   [wiki-api](https://github.com/richardasaurus/wiki-api) by\n    \\@richardasaurus for inspiration\n-   \\@nmoroze and \\@themichaelyang for feedback and suggestions\n-   The [Wikimedia Foundation](http://wikimediafoundation.org/wiki/Home)\n    for giving the world free access to data\n\n[![Bitdeli badge](https://d2weczhvl823v0.cloudfront.net/goldsmith/wikipedia/trend.png)](https://bitdeli.com/free)\n',
     'author': 'Hobson Lane',
     'author_email': 'hobson@tangibleai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tangibleai/community/nlpia2_wikipedia',
```

### Comparing `nlpia2_wikipedia-1.5.4/PKG-INFO` & `nlpia2_wikipedia-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpia2-wikipedia
-Version: 1.5.4
+Version: 1.5.6
 Summary: Updated version of `wikipedia` package because original repo has been abandoned since 2014.
 Home-page: https://gitlab.com/tangibleai/community/nlpia2_wikipedia
 License: AGPL-3.0-or-later
 Keywords: wiki,Wikipedia,scraping,api,wrapper,crawler,markdown,html,parser
 Author: Hobson Lane
 Author-email: hobson@tangibleai.com
 Requires-Python: >=3.8
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: beautifulsoup4 (>=4.11)
-Requires-Dist: pandas (>=2.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: poetry (>=1.1)
 Requires-Dist: requests (>=2.0,<3.0.0)
 Project-URL: Documentation, https://gitlab.com/tangibleai/community/nlpia2_wikipedia
 Project-URL: Repository, https://gitlab.com/tangibleai/community/nlpia2_wikipedia
 Description-Content-Type: text/markdown
 
 # Wikipedia
```

