# Comparing `tmp/synonym_cli-0.2.1.tar.gz` & `tmp/synonym_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synonym_cli-0.2.1.tar", max compression
+gzip compressed data, was "synonym_cli-0.3.0.tar", max compression
```

## Comparing `synonym_cli-0.2.1.tar` & `synonym_cli-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1150 2022-12-24 21:18:07.853065 synonym_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2562 2022-12-22 13:49:27.335566 synonym_cli-0.2.1/README.md
--rw-r--r--   0        0        0        0 2022-12-21 22:20:42.204585 synonym_cli-0.2.1/src/synonym_cli/__init__.py
--rw-r--r--   0        0        0     2027 2022-12-24 21:37:10.794181 synonym_cli-0.2.1/src/synonym_cli/__main__.py
--rw-r--r--   0        0        0     2716 2022-12-22 13:38:51.956631 synonym_cli-0.2.1/src/synonym_cli/altervista.py
--rw-r--r--   0        0        0     4527 2022-12-24 21:45:17.226851 synonym_cli-0.2.1/src/synonym_cli/cli.py
--rw-r--r--   0        0        0     3299 2022-12-22 13:38:51.974631 synonym_cli-0.2.1/src/synonym_cli/datamuse.py
--rw-r--r--   0        0        0     1450 2022-12-21 23:21:36.554550 synonym_cli-0.2.1/src/synonym_cli/settings.py
--rw-r--r--   0        0        0      378 2022-12-21 22:20:01.825003 synonym_cli-0.2.1/src/synonym_cli/tur.py
--rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 synonym_cli-0.2.1/setup.py
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 synonym_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1158 2023-07-07 09:31:56.697386 synonym_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2721 2023-07-07 08:34:55.649887 synonym_cli-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-21 22:20:42.204585 synonym_cli-0.3.0/src/synonym_cli/__init__.py
+-rw-r--r--   0        0        0     2027 2022-12-24 21:37:10.794181 synonym_cli-0.3.0/src/synonym_cli/__main__.py
+-rw-r--r--   0        0        0     2716 2022-12-22 13:38:51.956631 synonym_cli-0.3.0/src/synonym_cli/altervista.py
+-rw-r--r--   0        0        0     3989 2023-07-07 10:01:57.273803 synonym_cli-0.3.0/src/synonym_cli/cli.py
+-rw-r--r--   0        0        0     3299 2022-12-22 13:38:51.974631 synonym_cli-0.3.0/src/synonym_cli/datamuse.py
+-rw-r--r--   0        0        0     1450 2022-12-21 23:21:36.554550 synonym_cli-0.3.0/src/synonym_cli/settings.py
+-rw-r--r--   0        0        0      457 2023-07-07 10:07:19.107300 synonym_cli-0.3.0/src/synonym_cli/tur.py
+-rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 synonym_cli-0.3.0/setup.py
+-rw-r--r--   0        0        0     3940 1970-01-01 00:00:00.000000 synonym_cli-0.3.0/PKG-INFO
```

### Comparing `synonym_cli-0.2.1/pyproject.toml` & `synonym_cli-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "synonym-cli"
 description = "🌾Get synonyms and antonyms of words from Thesaurus.com and other sources in your terminal, with rich output."
 authors = ["agmmnn <agmmnn@gmail.com>"]
-version = "0.2.1"
+version = "0.3.0"
 readme = "README.md"
 homepage = "https://github.com/agmmnn/syn"
 repository = "https://github.com/agmmnn/syn"
 keywords = ["synonym", "antonym", "thesaurus", "cli"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
@@ -16,24 +16,24 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/agmmnn/syn/releases"
 Source = "https://github.com/agmmnn/syn"
 "Bug Tracker" = "https://github.com/agmmnn/syn/issues"
 
 [tool.poetry.dependencies]
-gazpacho = "^1.1"
 python = "^3.7"
 requests = "^2.28.1"
-rich = "^12.6.0"
-importlib-metadata = "^5.2.0"
-aiohttp = "^3.8.3"
+rich = "^13.4.2"
+importlib-metadata = "^6.7.0"
+aiohttp = "^3.8.4"
+beautifulsoup4 = "^4.12.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
-pytest = "^7.2.0"
+black = "^23.3.0"
+pytest = "^7.4.0"
 
 [tool.poetry.scripts]
 syn = "synonym_cli.__main__:cli"
 
 [tool.black]
 includes = "src"
```

### Comparing `synonym_cli-0.2.1/README.md` & `synonym_cli-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<div align="center"><img src="https://user-images.githubusercontent.com/16024979/162848437-8da9d5d4-a234-44d3-94d8-048f92b015a6.png" alt="syn"><a alt="Github" href="https://github.com/agmmnn/syn"><img alt="GitHub release" src="https://img.shields.io/github/v/release/agmmnn/syn"></a> <a href="https://pypi.org/project/synonym-cli/"><img alt="PyPI" src="https://img.shields.io/pypi/v/synonym-cli"></a></div>
+<div align="center"><img src="https://user-images.githubusercontent.com/16024979/162848437-8da9d5d4-a234-44d3-94d8-048f92b015a6.png" alt="syn"><a alt="Github" href="https://github.com/agmmnn/syn"><img alt="GitHub release" src="https://img.shields.io/github/v/release/agmmnn/syn"></a> <a href="https://pypi.org/project/synonym-cli/"><img alt="PyPI" src="https://img.shields.io/pypi/v/synonym-cli"></a> <a href="https://pepy.tech/project/synonym-cli"><img alt="PyPI" src="https://pepy.tech/badge/synonym-cli"></a></div>
 
 # 🌾 syn
 
 Get synonyms and antonyms of words from [Thesaurus.com](https://www.thesaurus.com/), [Datamuse API](https://www.datamuse.com/api/) and [AlterVista](https://thesaurus.altervista.org/) in your terminal, with [rich](https://github.com/Textualize/rich) output.
 
 # Install:
 
@@ -16,14 +16,16 @@
 syn <word>
 ```
 
 ### Explore Mode
 
 Returns more particular results about the given word. Uses [Datamuse API](https://www.datamuse.com/api/).
 
+> for Web UI: https://wordwhisper.vercel.app
+
 `$ syn dominant -d`
 ![](https://user-images.githubusercontent.com/16024979/209148078-309ba28e-dc59-459f-9035-b6d3d75b710f.png)
 
 ### Other Languages
 
 For other languages you can use `--lang`, `-l` command. To use this feature, you need to get an api key from [here](https://thesaurus.altervista.org/openapi).
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-                         [syn][GitHub_release] [PyPI]
+                      [syn][GitHub_release] [PyPI] [PyPI]
 # ð¾ syn Get synonyms and antonyms of words from [Thesaurus.com](https://
 www.thesaurus.com/), [Datamuse API](https://www.datamuse.com/api/) and
 [AlterVista](https://thesaurus.altervista.org/) in your terminal, with [rich]
 (https://github.com/Textualize/rich) output. # Install: ``` pip install
 synonym-cli ``` ## Usage: ``` syn  ``` ### Explore Mode Returns more particular
 results about the given word. Uses [Datamuse API](https://www.datamuse.com/api/
-). `$ syn dominant -d` ![](https://user-images.githubusercontent.com/16024979/
-209148078-309ba28e-dc59-459f-9035-b6d3d75b710f.png) ### Other Languages For
-other languages you can use `--lang`, `-l` command. To use this feature, you
-need to get an api key from [here](https://thesaurus.altervista.org/openapi).
-`$ syn -l fr belle` ![](https://user-images.githubusercontent.com/16024979/
-209144768-0cde6709-65d9-4142-9eae-bb4bc38e4a13.png) `$ syn -l ru ÑÑÐ°Ð·Ð°` !
-[](https://user-images.githubusercontent.com/16024979/209144765-abca9b54-5495-
-4295-98f7-15acdbde7623.png) > AlterVista's Thesaurus API supports the following
+). > for Web UI: https://wordwhisper.vercel.app `$ syn dominant -d` ![](https:/
+/user-images.githubusercontent.com/16024979/209148078-309ba28e-dc59-459f-9035-
+b6d3d75b710f.png) ### Other Languages For other languages you can use `--lang`,
+`-l` command. To use this feature, you need to get an api key from [here]
+(https://thesaurus.altervista.org/openapi). `$ syn -l fr belle` ![](https://
+user-images.githubusercontent.com/16024979/209144768-0cde6709-65d9-4142-9eae-
+bb4bc38e4a13.png) `$ syn -l ru ÑÑÐ°Ð·Ð°` ![](https://user-
+images.githubusercontent.com/16024979/209144765-abca9b54-5495-4295-98f7-
+15acdbde7623.png) > AlterVista's Thesaurus API supports the following
 languages: > Czech: `cs`, Danish: `da`, English (US): `en`, French: `fr`,
 German (Germany): `de`, German (Switzerland): `de`, Greek: `el`, Hungarian:
 `hu`, Italian: `it`, Norwegian: `no`, Polish: `pl`, Portuguese: `pt`, Romanian:
 `ro`, Russian: `ru`, Slovak: `sk`, Spanish: `es`. ### Set Default Language You
 can set the default language with the `--setlang ` argument, so you don't have
 to give the `-l` argument every time. ``` $ syn --setlang fr > default language
 is: fr $ syn belle > ... ``` ## Arguments ``` -h, --help show this help message
```

### Comparing `synonym_cli-0.2.1/src/synonym_cli/__main__.py` & `synonym_cli-0.3.0/src/synonym_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `synonym_cli-0.2.1/src/synonym_cli/altervista.py` & `synonym_cli-0.3.0/src/synonym_cli/altervista.py`

 * *Files identical despite different names*

### Comparing `synonym_cli-0.2.1/src/synonym_cli/datamuse.py` & `synonym_cli-0.3.0/src/synonym_cli/datamuse.py`

 * *Files identical despite different names*

### Comparing `synonym_cli-0.2.1/src/synonym_cli/settings.py` & `synonym_cli-0.3.0/src/synonym_cli/settings.py`

 * *Files identical despite different names*

### Comparing `synonym_cli-0.2.1/setup.py` & `synonym_cli-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 packages = \
 ['synonym_cli']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiohttp>=3.8.3,<4.0.0',
- 'gazpacho>=1.1,<2.0',
- 'importlib-metadata>=5.2.0,<6.0.0',
+['aiohttp>=3.8.4,<4.0.0',
+ 'beautifulsoup4>=4.12.2,<5.0.0',
+ 'importlib-metadata>=6.7.0,<7.0.0',
  'requests>=2.28.1,<3.0.0',
- 'rich>=12.6.0,<13.0.0']
+ 'rich>=13.4.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['syn = synonym_cli.__main__:cli']}
 
 setup_kwargs = {
     'name': 'synonym-cli',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': '🌾Get synonyms and antonyms of words from Thesaurus.com and other sources in your terminal, with rich output.',
-    'long_description': '<div align="center"><img src="https://user-images.githubusercontent.com/16024979/162848437-8da9d5d4-a234-44d3-94d8-048f92b015a6.png" alt="syn"><a alt="Github" href="https://github.com/agmmnn/syn"><img alt="GitHub release" src="https://img.shields.io/github/v/release/agmmnn/syn"></a> <a href="https://pypi.org/project/synonym-cli/"><img alt="PyPI" src="https://img.shields.io/pypi/v/synonym-cli"></a></div>\n\n# 🌾 syn\n\nGet synonyms and antonyms of words from [Thesaurus.com](https://www.thesaurus.com/), [Datamuse API](https://www.datamuse.com/api/) and [AlterVista](https://thesaurus.altervista.org/) in your terminal, with [rich](https://github.com/Textualize/rich) output.\n\n# Install:\n\n```\npip install synonym-cli\n```\n\n## Usage:\n\n```\nsyn <word>\n```\n\n### Explore Mode\n\nReturns more particular results about the given word. Uses [Datamuse API](https://www.datamuse.com/api/).\n\n`$ syn dominant -d`\n![](https://user-images.githubusercontent.com/16024979/209148078-309ba28e-dc59-459f-9035-b6d3d75b710f.png)\n\n### Other Languages\n\nFor other languages you can use `--lang`, `-l` command. To use this feature, you need to get an api key from [here](https://thesaurus.altervista.org/openapi).\n\n`$ syn -l fr belle`\n![](https://user-images.githubusercontent.com/16024979/209144768-0cde6709-65d9-4142-9eae-bb4bc38e4a13.png)\n\n`$ syn -l ru фраза`\n![](https://user-images.githubusercontent.com/16024979/209144765-abca9b54-5495-4295-98f7-15acdbde7623.png)\n\n> AlterVista\'s Thesaurus API supports the following languages:\n\n> Czech: `cs`, Danish: `da`, English (US): `en`, French: `fr`, German (Germany): `de`, German (Switzerland): `de`, Greek: `el`, Hungarian: `hu`, Italian: `it`, Norwegian: `no`, Polish: `pl`, Portuguese: `pt`, Romanian: `ro`, Russian: `ru`, Slovak: `sk`, Spanish: `es`.\n\n### Set Default Language\n\nYou can set the default language with the `--setlang <lang_code>` argument, so you don\'t have to give the `-l` argument every time.\n\n```\n$ syn --setlang fr\n> default language is: fr\n$ syn belle\n> ...\n```\n\n## Arguments\n\n```\n  -h, --help      show this help message and exit\n  -p, --plain     returns plain text output\n  -l, --lang      <language>\n  --setkey        set apikey for altervista api\n  --setlang       set default language (currently default is \'en\')\n  --show          show settings file\n  -v, --version   show program\'s version number and exit\n```\n\n# Contrubuting\n\nContributions are welcome. If you want to contribute to this list send a pull request or just open a new issue.\n',
+    'long_description': '<div align="center"><img src="https://user-images.githubusercontent.com/16024979/162848437-8da9d5d4-a234-44d3-94d8-048f92b015a6.png" alt="syn"><a alt="Github" href="https://github.com/agmmnn/syn"><img alt="GitHub release" src="https://img.shields.io/github/v/release/agmmnn/syn"></a> <a href="https://pypi.org/project/synonym-cli/"><img alt="PyPI" src="https://img.shields.io/pypi/v/synonym-cli"></a> <a href="https://pepy.tech/project/synonym-cli"><img alt="PyPI" src="https://pepy.tech/badge/synonym-cli"></a></div>\n\n# 🌾 syn\n\nGet synonyms and antonyms of words from [Thesaurus.com](https://www.thesaurus.com/), [Datamuse API](https://www.datamuse.com/api/) and [AlterVista](https://thesaurus.altervista.org/) in your terminal, with [rich](https://github.com/Textualize/rich) output.\n\n# Install:\n\n```\npip install synonym-cli\n```\n\n## Usage:\n\n```\nsyn <word>\n```\n\n### Explore Mode\n\nReturns more particular results about the given word. Uses [Datamuse API](https://www.datamuse.com/api/).\n\n> for Web UI: https://wordwhisper.vercel.app\n\n`$ syn dominant -d`\n![](https://user-images.githubusercontent.com/16024979/209148078-309ba28e-dc59-459f-9035-b6d3d75b710f.png)\n\n### Other Languages\n\nFor other languages you can use `--lang`, `-l` command. To use this feature, you need to get an api key from [here](https://thesaurus.altervista.org/openapi).\n\n`$ syn -l fr belle`\n![](https://user-images.githubusercontent.com/16024979/209144768-0cde6709-65d9-4142-9eae-bb4bc38e4a13.png)\n\n`$ syn -l ru фраза`\n![](https://user-images.githubusercontent.com/16024979/209144765-abca9b54-5495-4295-98f7-15acdbde7623.png)\n\n> AlterVista\'s Thesaurus API supports the following languages:\n\n> Czech: `cs`, Danish: `da`, English (US): `en`, French: `fr`, German (Germany): `de`, German (Switzerland): `de`, Greek: `el`, Hungarian: `hu`, Italian: `it`, Norwegian: `no`, Polish: `pl`, Portuguese: `pt`, Romanian: `ro`, Russian: `ru`, Slovak: `sk`, Spanish: `es`.\n\n### Set Default Language\n\nYou can set the default language with the `--setlang <lang_code>` argument, so you don\'t have to give the `-l` argument every time.\n\n```\n$ syn --setlang fr\n> default language is: fr\n$ syn belle\n> ...\n```\n\n## Arguments\n\n```\n  -h, --help      show this help message and exit\n  -p, --plain     returns plain text output\n  -l, --lang      <language>\n  --setkey        set apikey for altervista api\n  --setlang       set default language (currently default is \'en\')\n  --show          show settings file\n  -v, --version   show program\'s version number and exit\n```\n\n# Contrubuting\n\nContributions are welcome. If you want to contribute to this list send a pull request or just open a new issue.\n',
     'author': 'agmmnn',
     'author_email': 'agmmnn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/agmmnn/syn',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['synonym_cli'] package_data = \ {'': ['*']}
-install_requires = \ ['aiohttp>=3.8.3,<4.0.0', 'gazpacho>=1.1,<2.0',
-'importlib-metadata>=5.2.0,<6.0.0', 'requests>=2.28.1,<3.0.0',
-'rich>=12.6.0,<13.0.0'] entry_points = \ {'console_scripts': ['syn =
+install_requires = \ ['aiohttp>=3.8.4,<4.0.0', 'beautifulsoup4>=4.12.2,<5.0.0',
+'importlib-metadata>=6.7.0,<7.0.0', 'requests>=2.28.1,<3.0.0',
+'rich>=13.4.2,<14.0.0'] entry_points = \ {'console_scripts': ['syn =
 synonym_cli.__main__:cli']} setup_kwargs = { 'name': 'synonym-cli', 'version':
-'0.2.1', 'description': 'ð¾Get synonyms and antonyms of words from
+'0.3.0', 'description': 'ð¾Get synonyms and antonyms of words from
 Thesaurus.com and other sources in your terminal, with rich output.',
 'long_description': '
-                         [syn][GitHub_release] [PyPI]
+                      [syn][GitHub_release] [PyPI] [PyPI]
 \n\n# ð¾ syn\n\nGet synonyms and antonyms of words from [Thesaurus.com]
 (https://www.thesaurus.com/), [Datamuse API](https://www.datamuse.com/api/) and
 [AlterVista](https://thesaurus.altervista.org/) in your terminal, with [rich]
 (https://github.com/Textualize/rich) output.\n\n# Install:\n\n```\npip install
 synonym-cli\n```\n\n## Usage:\n\n```\nsyn \n```\n\n### Explore Mode\n\nReturns
 more particular results about the given word. Uses [Datamuse API](https://
-www.datamuse.com/api/).\n\n`$ syn dominant -d`\n![](https://user-
-images.githubusercontent.com/16024979/209148078-309ba28e-dc59-459f-9035-
-b6d3d75b710f.png)\n\n### Other Languages\n\nFor other languages you can use `--
-lang`, `-l` command. To use this feature, you need to get an api key from
-[here](https://thesaurus.altervista.org/openapi).\n\n`$ syn -l fr belle`\n![]
-(https://user-images.githubusercontent.com/16024979/209144768-0cde6709-65d9-
-4142-9eae-bb4bc38e4a13.png)\n\n`$ syn -l ru ÑÑÐ°Ð·Ð°`\n![](https://user-
+www.datamuse.com/api/).\n\n> for Web UI: https://wordwhisper.vercel.app\n\n`$
+syn dominant -d`\n![](https://user-images.githubusercontent.com/16024979/
+209148078-309ba28e-dc59-459f-9035-b6d3d75b710f.png)\n\n### Other
+Languages\n\nFor other languages you can use `--lang`, `-l` command. To use
+this feature, you need to get an api key from [here](https://
+thesaurus.altervista.org/openapi).\n\n`$ syn -l fr belle`\n![](https://user-
+images.githubusercontent.com/16024979/209144768-0cde6709-65d9-4142-9eae-
+bb4bc38e4a13.png)\n\n`$ syn -l ru ÑÑÐ°Ð·Ð°`\n![](https://user-
 images.githubusercontent.com/16024979/209144765-abca9b54-5495-4295-98f7-
 15acdbde7623.png)\n\n> AlterVista\'s Thesaurus API supports the following
 languages:\n\n> Czech: `cs`, Danish: `da`, English (US): `en`, French: `fr`,
 German (Germany): `de`, German (Switzerland): `de`, Greek: `el`, Hungarian:
 `hu`, Italian: `it`, Norwegian: `no`, Polish: `pl`, Portuguese: `pt`, Romanian:
 `ro`, Russian: `ru`, Slovak: `sk`, Spanish: `es`.\n\n### Set Default
 Language\n\nYou can set the default language with the `--setlang ` argument, so
```

### Comparing `synonym_cli-0.2.1/PKG-INFO` & `synonym_cli-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synonym-cli
-Version: 0.2.1
+Version: 0.3.0
 Summary: 🌾Get synonyms and antonyms of words from Thesaurus.com and other sources in your terminal, with rich output.
 Home-page: https://github.com/agmmnn/syn
 Keywords: synonym,antonym,thesaurus,cli
 Author: agmmnn
 Author-email: agmmnn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
@@ -13,26 +13,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: gazpacho (>=1.1,<2.0)
-Requires-Dist: importlib-metadata (>=5.2.0,<6.0.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: importlib-metadata (>=6.7.0,<7.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Bug Tracker, https://github.com/agmmnn/syn/issues
 Project-URL: Changelog, https://github.com/agmmnn/syn/releases
 Project-URL: Repository, https://github.com/agmmnn/syn
 Project-URL: Source, https://github.com/agmmnn/syn
 Description-Content-Type: text/markdown
 
-<div align="center"><img src="https://user-images.githubusercontent.com/16024979/162848437-8da9d5d4-a234-44d3-94d8-048f92b015a6.png" alt="syn"><a alt="Github" href="https://github.com/agmmnn/syn"><img alt="GitHub release" src="https://img.shields.io/github/v/release/agmmnn/syn"></a> <a href="https://pypi.org/project/synonym-cli/"><img alt="PyPI" src="https://img.shields.io/pypi/v/synonym-cli"></a></div>
+<div align="center"><img src="https://user-images.githubusercontent.com/16024979/162848437-8da9d5d4-a234-44d3-94d8-048f92b015a6.png" alt="syn"><a alt="Github" href="https://github.com/agmmnn/syn"><img alt="GitHub release" src="https://img.shields.io/github/v/release/agmmnn/syn"></a> <a href="https://pypi.org/project/synonym-cli/"><img alt="PyPI" src="https://img.shields.io/pypi/v/synonym-cli"></a> <a href="https://pepy.tech/project/synonym-cli"><img alt="PyPI" src="https://pepy.tech/badge/synonym-cli"></a></div>
 
 # 🌾 syn
 
 Get synonyms and antonyms of words from [Thesaurus.com](https://www.thesaurus.com/), [Datamuse API](https://www.datamuse.com/api/) and [AlterVista](https://thesaurus.altervista.org/) in your terminal, with [rich](https://github.com/Textualize/rich) output.
 
 # Install:
 
@@ -46,14 +46,16 @@
 syn <word>
 ```
 
 ### Explore Mode
 
 Returns more particular results about the given word. Uses [Datamuse API](https://www.datamuse.com/api/).
 
+> for Web UI: https://wordwhisper.vercel.app
+
 `$ syn dominant -d`
 ![](https://user-images.githubusercontent.com/16024979/209148078-309ba28e-dc59-459f-9035-b6d3d75b710f.png)
 
 ### Other Languages
 
 For other languages you can use `--lang`, `-l` command. To use this feature, you need to get an api key from [here](https://thesaurus.altervista.org/openapi).
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1 Name: synonym-cli Version: 0.2.1 Summary: ð¾Get
+Metadata-Version: 2.1 Name: synonym-cli Version: 0.3.0 Summary: ð¾Get
 synonyms and antonyms of words from Thesaurus.com and other sources in your
 terminal, with rich output. Home-page: https://github.com/agmmnn/syn Keywords:
 synonym,antonym,thesaurus,cli Author: agmmnn Author-email: agmmnn@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: Environment :: Console Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Utilities Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: gazpacho (>=1.1,<2.0) Requires-Dist: importlib-metadata
-(>=5.2.0,<6.0.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: rich
-(>=12.6.0,<13.0.0) Project-URL: Bug Tracker, https://github.com/agmmnn/syn/
-issues Project-URL: Changelog, https://github.com/agmmnn/syn/releases Project-
-URL: Repository, https://github.com/agmmnn/syn Project-URL: Source, https://
-github.com/agmmnn/syn Description-Content-Type: text/markdown
-                         [syn][GitHub_release] [PyPI]
+Classifier: Topic :: Utilities Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: importlib-
+metadata (>=6.7.0,<7.0.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-
+Dist: rich (>=13.4.2,<14.0.0) Project-URL: Bug Tracker, https://github.com/
+agmmnn/syn/issues Project-URL: Changelog, https://github.com/agmmnn/syn/
+releases Project-URL: Repository, https://github.com/agmmnn/syn Project-URL:
+Source, https://github.com/agmmnn/syn Description-Content-Type: text/markdown
+                      [syn][GitHub_release] [PyPI] [PyPI]
 # ð¾ syn Get synonyms and antonyms of words from [Thesaurus.com](https://
 www.thesaurus.com/), [Datamuse API](https://www.datamuse.com/api/) and
 [AlterVista](https://thesaurus.altervista.org/) in your terminal, with [rich]
 (https://github.com/Textualize/rich) output. # Install: ``` pip install
 synonym-cli ``` ## Usage: ``` syn  ``` ### Explore Mode Returns more particular
 results about the given word. Uses [Datamuse API](https://www.datamuse.com/api/
-). `$ syn dominant -d` ![](https://user-images.githubusercontent.com/16024979/
-209148078-309ba28e-dc59-459f-9035-b6d3d75b710f.png) ### Other Languages For
-other languages you can use `--lang`, `-l` command. To use this feature, you
-need to get an api key from [here](https://thesaurus.altervista.org/openapi).
-`$ syn -l fr belle` ![](https://user-images.githubusercontent.com/16024979/
-209144768-0cde6709-65d9-4142-9eae-bb4bc38e4a13.png) `$ syn -l ru ÑÑÐ°Ð·Ð°` !
-[](https://user-images.githubusercontent.com/16024979/209144765-abca9b54-5495-
-4295-98f7-15acdbde7623.png) > AlterVista's Thesaurus API supports the following
+). > for Web UI: https://wordwhisper.vercel.app `$ syn dominant -d` ![](https:/
+/user-images.githubusercontent.com/16024979/209148078-309ba28e-dc59-459f-9035-
+b6d3d75b710f.png) ### Other Languages For other languages you can use `--lang`,
+`-l` command. To use this feature, you need to get an api key from [here]
+(https://thesaurus.altervista.org/openapi). `$ syn -l fr belle` ![](https://
+user-images.githubusercontent.com/16024979/209144768-0cde6709-65d9-4142-9eae-
+bb4bc38e4a13.png) `$ syn -l ru ÑÑÐ°Ð·Ð°` ![](https://user-
+images.githubusercontent.com/16024979/209144765-abca9b54-5495-4295-98f7-
+15acdbde7623.png) > AlterVista's Thesaurus API supports the following
 languages: > Czech: `cs`, Danish: `da`, English (US): `en`, French: `fr`,
 German (Germany): `de`, German (Switzerland): `de`, Greek: `el`, Hungarian:
 `hu`, Italian: `it`, Norwegian: `no`, Polish: `pl`, Portuguese: `pt`, Romanian:
 `ro`, Russian: `ru`, Slovak: `sk`, Spanish: `es`. ### Set Default Language You
 can set the default language with the `--setlang ` argument, so you don't have
 to give the `-l` argument every time. ``` $ syn --setlang fr > default language
 is: fr $ syn belle > ... ``` ## Arguments ``` -h, --help show this help message
```

