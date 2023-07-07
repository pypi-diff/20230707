# Comparing `tmp/mkdocs-typedoc-1.0.0.tar.gz` & `tmp/mkdocs-typedoc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-typedoc-1.0.0.tar", last modified: Sun Jul  2 21:17:37 2023, max compression
+gzip compressed data, was "mkdocs-typedoc-1.0.1.tar", last modified: Fri Jul  7 07:35:35 2023, max compression
```

## Comparing `mkdocs-typedoc-1.0.0.tar` & `mkdocs-typedoc-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-02 21:17:37.307174 mkdocs-typedoc-1.0.0/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-07-02 15:55:15.000000 mkdocs-typedoc-1.0.0/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     4363 2023-07-02 21:17:37.307252 mkdocs-typedoc-1.0.0/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     3329 2023-07-02 21:02:49.000000 mkdocs-typedoc-1.0.0/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-02 21:17:37.306568 mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     4363 2023-07-02 21:17:37.000000 mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)      304 2023-07-02 21:17:37.000000 mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2023-07-02 21:17:37.000000 mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)       56 2023-07-02 21:17:37.000000 mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/entry_points.txt
--rw-r--r--   0 kuba       (501) staff       (20)      128 2023-07-02 21:17:37.000000 mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)        8 2023-07-02 21:17:37.000000 mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)     1214 2023-07-02 21:17:37.307561 mkdocs-typedoc-1.0.0/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)      192 2023-07-02 21:14:13.000000 mkdocs-typedoc-1.0.0/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-02 21:17:37.306812 mkdocs-typedoc-1.0.0/typedoc/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-03-26 20:51:00.000000 mkdocs-typedoc-1.0.0/typedoc/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     3215 2023-07-02 20:38:50.000000 mkdocs-typedoc-1.0.0/typedoc/plugin.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-07 07:35:35.887707 mkdocs-typedoc-1.0.1/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-07-02 15:55:15.000000 mkdocs-typedoc-1.0.1/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     4929 2023-07-07 07:35:35.887810 mkdocs-typedoc-1.0.1/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     3895 2023-07-07 07:27:27.000000 mkdocs-typedoc-1.0.1/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-07 07:35:35.886856 mkdocs-typedoc-1.0.1/mkdocs_typedoc.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     4929 2023-07-07 07:35:35.000000 mkdocs-typedoc-1.0.1/mkdocs_typedoc.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)      304 2023-07-07 07:35:35.000000 mkdocs-typedoc-1.0.1/mkdocs_typedoc.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2023-07-07 07:35:35.000000 mkdocs-typedoc-1.0.1/mkdocs_typedoc.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       56 2023-07-07 07:35:35.000000 mkdocs-typedoc-1.0.1/mkdocs_typedoc.egg-info/entry_points.txt
+-rw-r--r--   0 kuba       (501) staff       (20)      112 2023-07-07 07:35:35.000000 mkdocs-typedoc-1.0.1/mkdocs_typedoc.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        8 2023-07-07 07:35:35.000000 mkdocs-typedoc-1.0.1/mkdocs_typedoc.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)     1196 2023-07-07 07:35:35.888206 mkdocs-typedoc-1.0.1/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)      192 2023-07-02 21:14:13.000000 mkdocs-typedoc-1.0.1/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-07 07:35:35.887330 mkdocs-typedoc-1.0.1/typedoc/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-03-26 20:51:00.000000 mkdocs-typedoc-1.0.1/typedoc/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4707 2023-07-07 07:20:58.000000 mkdocs-typedoc-1.0.1/typedoc/plugin.py
```

### Comparing `mkdocs-typedoc-1.0.0/LICENSE` & `mkdocs-typedoc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-typedoc-1.0.0/PKG-INFO` & `mkdocs-typedoc-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: mkdocs-typedoc
-Version: 1.0.0
-Summary: MkDocs plugin to generate documentation from TypeScript source code using TypeDoc.
-Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc
-Author: Jakub Andrýsek
-Author-email: email@kubaandrysek.cz
-License: MIT
-Project-URL: Source, https://github.com/JakubAndrysek/mkdocs-typedoc
-Project-URL: Documentation, https://typedoc.kubaandrysek.cz/
-Project-URL: Tracker, https://github.com/JakubAndrysek/mkdocs-typedoc/issues
-Project-URL: Funding, https://github.com/sponsors/jakubandrysek
-Keywords: mkdocs plugin
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Mkdocs-Typedoc Plugin
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-typedoc&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <a href="https://github.com/JakubAndrysek/mkdocs-typedoc/blob/main/LICENSE" target="_blank"><img src="https://img.shields.io/github/license/JakubAndrysek/mkdocs-typedoc?style=flat-square"></a>
 <a href="https://pypi.org/project/mkdocs-typedoc/" target="_blank"><img alt="PyPI" src="https://img.shields.io/pypi/v/mkdocs-typedoc?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/mkdocs-typedoc/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/JakubAndrysek/mkdocs-typedoc?style=flat-square"></a>
@@ -47,44 +22,60 @@
 ```
 
 Ensure that you have [Node.js](https://nodejs.org/en/) installed in your system. If not, you can download it from the official website.
 
 Also, install [TypeDoc](https://typedoc.org/) using [NPM](https://www.npmjs.com/):
 
 ```bash
-npm install typedoc --save-dev
+npm install typedoc typescript --save-dev
 ```
 
 ## Usage
 
 Add the following lines to your mkdocs.yml:
 
 ```yaml
 plugins:
   - typedoc:
       source: './ts-examples/@types/*.d.ts'
       output_dir: 'typedocApi'
       tsconfig: './ts-examples/tsconfig.json'
       options: 'typedoc.json'
       name: 'API Doc'
+      disable_system_check: False
 ```
 
 - `source` (required): The path to your TypeScript source code.
 - `output_dir` (optional): The directory where you want to output your docs. Default is "typedoc".
 - `tsconfig` (required): The path to the tsconfig file for your project.
 - `options` (optional): The path to the typedoc.json options file with more options.
 - `name` (optional): The name for the generated documentation. Default is "TypeDoc API".
+- `disable_system_check` (optional): Disable the TypeScript system check. Default is False.
 
 The plugin will generate TypeDoc documentation into the output directory specified.
 
+## Windows machines
+
+System might not work on Windows machines, if you would like to test it on Windows, set `disable_system_check` to `True`.
+
+Error message:
+
+```bash
+INFO     -  Building documentation...
+INFO     -  Cleaning site directory
+ERROR    -  TypeDoc: TypeDoc failed with error: [WinError 2] The system cannot find the file specified
+```
+
+If anyone knows how to fix this, please let me know or create a pull request.
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Do You Enjoy My Work?
 Then definitely consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
 
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://choosealicense.com/licenses/mit/)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,21 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-typedoc Version: 1.0.0 Summary: MkDocs
-plugin to generate documentation from TypeScript source code using TypeDoc.
-Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc Author: Jakub
-AndrÃ½sek Author-email: email@kubaandrysek.cz License: MIT Project-URL: Source,
-https://github.com/JakubAndrysek/mkdocs-typedoc Project-URL: Documentation,
-https://typedoc.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/
-JakubAndrysek/mkdocs-typedoc/issues Project-URL: Funding, https://github.com/
-sponsors/jakubandrysek Keywords: mkdocs plugin Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE # Mkdocs-Typedoc Plugin
+# Mkdocs-Typedoc Plugin
                  [https://hits.seeyoufarm.com/api/count/incr/
        badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-
 typedoc&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]
 [https://img.shields.io/github/license/JakubAndrysek/mkdocs-typedoc?style=flat-
    square] [PyPI] [https://img.shields.io/github/stars/JakubAndrysek/mkdocs-
 typedoc?style=flat-square] [https://img.shields.io/github/forks/JakubAndrysek/
    mkdocs-typedoc?style=flat-square] [https://img.shields.io/github/issues/
@@ -25,23 +12,31 @@
 typedoc?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads]
 The Mkdocs-Typedoc Plugin is designed to integrate TypeDoc documentation with
 your MkDocs project. ## Installation Install the plugin using pip from [PyPI]
 (https://pypi.org/project/mkdocs-typedoc/): ```bash pip install mkdocs-typedoc
 ``` Ensure that you have [Node.js](https://nodejs.org/en/) installed in your
 system. If not, you can download it from the official website. Also, install
 [TypeDoc](https://typedoc.org/) using [NPM](https://www.npmjs.com/): ```bash
-npm install typedoc --save-dev ``` ## Usage Add the following lines to your
-mkdocs.yml: ```yaml plugins: - typedoc: source: './ts-examples/@types/*.d.ts'
-output_dir: 'typedocApi' tsconfig: './ts-examples/tsconfig.json' options:
-'typedoc.json' name: 'API Doc' ``` - `source` (required): The path to your
-TypeScript source code. - `output_dir` (optional): The directory where you want
-to output your docs. Default is "typedoc". - `tsconfig` (required): The path to
-the tsconfig file for your project. - `options` (optional): The path to the
-typedoc.json options file with more options. - `name` (optional): The name for
-the generated documentation. Default is "TypeDoc API". The plugin will generate
-TypeDoc documentation into the output directory specified. ## Contributing Pull
-requests are welcome. For major changes, please open an issue first to discuss
-what you would like to change. ## Do You Enjoy My Work? Then definitely
-consider: - supporting me on GitHub Sponsors: [![](https://img.shields.io/
-static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https:/
-/github.com/sponsors/jakubandrysek) ## License [MIT](https://
-choosealicense.com/licenses/mit/)
+npm install typedoc typescript --save-dev ``` ## Usage Add the following lines
+to your mkdocs.yml: ```yaml plugins: - typedoc: source: './ts-examples/@types/
+*.d.ts' output_dir: 'typedocApi' tsconfig: './ts-examples/tsconfig.json'
+options: 'typedoc.json' name: 'API Doc' disable_system_check: False ``` -
+`source` (required): The path to your TypeScript source code. - `output_dir`
+(optional): The directory where you want to output your docs. Default is
+"typedoc". - `tsconfig` (required): The path to the tsconfig file for your
+project. - `options` (optional): The path to the typedoc.json options file with
+more options. - `name` (optional): The name for the generated documentation.
+Default is "TypeDoc API". - `disable_system_check` (optional): Disable the
+TypeScript system check. Default is False. The plugin will generate TypeDoc
+documentation into the output directory specified. ## Windows machines System
+might not work on Windows machines, if you would like to test it on Windows,
+set `disable_system_check` to `True`. Error message: ```bash INFO - Building
+documentation... INFO - Cleaning site directory ERROR - TypeDoc: TypeDoc failed
+with error: [WinError 2] The system cannot find the file specified ``` If
+anyone knows how to fix this, please let me know or create a pull request. ##
+Contributing Pull requests are welcome. For major changes, please open an issue
+first to discuss what you would like to change. ## Do You Enjoy My Work? Then
+definitely consider: - supporting me on GitHub Sponsors: [![](https://
+img.shields.io/static/
+v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
+github.com/sponsors/jakubandrysek) ## License [MIT](https://choosealicense.com/
+licenses/mit/)
```

### Comparing `mkdocs-typedoc-1.0.0/mkdocs_typedoc.egg-info/PKG-INFO` & `mkdocs-typedoc-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-typedoc
-Version: 1.0.0
+Version: 1.0.1
 Summary: MkDocs plugin to generate documentation from TypeScript source code using TypeDoc.
 Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/mkdocs-typedoc
 Project-URL: Documentation, https://typedoc.kubaandrysek.cz/
@@ -47,39 +47,55 @@
 ```
 
 Ensure that you have [Node.js](https://nodejs.org/en/) installed in your system. If not, you can download it from the official website.
 
 Also, install [TypeDoc](https://typedoc.org/) using [NPM](https://www.npmjs.com/):
 
 ```bash
-npm install typedoc --save-dev
+npm install typedoc typescript --save-dev
 ```
 
 ## Usage
 
 Add the following lines to your mkdocs.yml:
 
 ```yaml
 plugins:
   - typedoc:
       source: './ts-examples/@types/*.d.ts'
       output_dir: 'typedocApi'
       tsconfig: './ts-examples/tsconfig.json'
       options: 'typedoc.json'
       name: 'API Doc'
+      disable_system_check: False
 ```
 
 - `source` (required): The path to your TypeScript source code.
 - `output_dir` (optional): The directory where you want to output your docs. Default is "typedoc".
 - `tsconfig` (required): The path to the tsconfig file for your project.
 - `options` (optional): The path to the typedoc.json options file with more options.
 - `name` (optional): The name for the generated documentation. Default is "TypeDoc API".
+- `disable_system_check` (optional): Disable the TypeScript system check. Default is False.
 
 The plugin will generate TypeDoc documentation into the output directory specified.
 
+## Windows machines
+
+System might not work on Windows machines, if you would like to test it on Windows, set `disable_system_check` to `True`.
+
+Error message:
+
+```bash
+INFO     -  Building documentation...
+INFO     -  Cleaning site directory
+ERROR    -  TypeDoc: TypeDoc failed with error: [WinError 2] The system cannot find the file specified
+```
+
+If anyone knows how to fix this, please let me know or create a pull request.
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Do You Enjoy My Work?
 Then definitely consider:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-typedoc Version: 1.0.0 Summary: MkDocs
+Metadata-Version: 2.1 Name: mkdocs-typedoc Version: 1.0.1 Summary: MkDocs
 plugin to generate documentation from TypeScript source code using TypeDoc.
 Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc Author: Jakub
 AndrÃ½sek Author-email: email@kubaandrysek.cz License: MIT Project-URL: Source,
 https://github.com/JakubAndrysek/mkdocs-typedoc Project-URL: Documentation,
 https://typedoc.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/
 JakubAndrysek/mkdocs-typedoc/issues Project-URL: Funding, https://github.com/
 sponsors/jakubandrysek Keywords: mkdocs plugin Classifier: License :: OSI
@@ -25,23 +25,31 @@
 typedoc?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads]
 The Mkdocs-Typedoc Plugin is designed to integrate TypeDoc documentation with
 your MkDocs project. ## Installation Install the plugin using pip from [PyPI]
 (https://pypi.org/project/mkdocs-typedoc/): ```bash pip install mkdocs-typedoc
 ``` Ensure that you have [Node.js](https://nodejs.org/en/) installed in your
 system. If not, you can download it from the official website. Also, install
 [TypeDoc](https://typedoc.org/) using [NPM](https://www.npmjs.com/): ```bash
-npm install typedoc --save-dev ``` ## Usage Add the following lines to your
-mkdocs.yml: ```yaml plugins: - typedoc: source: './ts-examples/@types/*.d.ts'
-output_dir: 'typedocApi' tsconfig: './ts-examples/tsconfig.json' options:
-'typedoc.json' name: 'API Doc' ``` - `source` (required): The path to your
-TypeScript source code. - `output_dir` (optional): The directory where you want
-to output your docs. Default is "typedoc". - `tsconfig` (required): The path to
-the tsconfig file for your project. - `options` (optional): The path to the
-typedoc.json options file with more options. - `name` (optional): The name for
-the generated documentation. Default is "TypeDoc API". The plugin will generate
-TypeDoc documentation into the output directory specified. ## Contributing Pull
-requests are welcome. For major changes, please open an issue first to discuss
-what you would like to change. ## Do You Enjoy My Work? Then definitely
-consider: - supporting me on GitHub Sponsors: [![](https://img.shields.io/
-static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https:/
-/github.com/sponsors/jakubandrysek) ## License [MIT](https://
-choosealicense.com/licenses/mit/)
+npm install typedoc typescript --save-dev ``` ## Usage Add the following lines
+to your mkdocs.yml: ```yaml plugins: - typedoc: source: './ts-examples/@types/
+*.d.ts' output_dir: 'typedocApi' tsconfig: './ts-examples/tsconfig.json'
+options: 'typedoc.json' name: 'API Doc' disable_system_check: False ``` -
+`source` (required): The path to your TypeScript source code. - `output_dir`
+(optional): The directory where you want to output your docs. Default is
+"typedoc". - `tsconfig` (required): The path to the tsconfig file for your
+project. - `options` (optional): The path to the typedoc.json options file with
+more options. - `name` (optional): The name for the generated documentation.
+Default is "TypeDoc API". - `disable_system_check` (optional): Disable the
+TypeScript system check. Default is False. The plugin will generate TypeDoc
+documentation into the output directory specified. ## Windows machines System
+might not work on Windows machines, if you would like to test it on Windows,
+set `disable_system_check` to `True`. Error message: ```bash INFO - Building
+documentation... INFO - Cleaning site directory ERROR - TypeDoc: TypeDoc failed
+with error: [WinError 2] The system cannot find the file specified ``` If
+anyone knows how to fix this, please let me know or create a pull request. ##
+Contributing Pull requests are welcome. For major changes, please open an issue
+first to discuss what you would like to change. ## Do You Enjoy My Work? Then
+definitely consider: - supporting me on GitHub Sponsors: [![](https://
+img.shields.io/static/
+v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
+github.com/sponsors/jakubandrysek) ## License [MIT](https://choosealicense.com/
+licenses/mit/)
```

### Comparing `mkdocs-typedoc-1.0.0/setup.cfg` & `mkdocs-typedoc-1.0.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-typedoc
-version = 1.0.0
+version = 1.0.1
 description = MkDocs plugin to generate documentation from TypeScript source code using TypeDoc.
 keywords = mkdocs plugin
 url = https://github.com/JakubAndrysek/mkdocs-typedoc
 author = Jakub Andrýsek
 author_email = email@kubaandrysek.cz
 project_urls = 
 	Source = https://github.com/JakubAndrysek/mkdocs-typedoc
@@ -34,14 +34,12 @@
 
 [options.extras_require]
 dev = 
 	mkdocs-material
 	mkdocs-open-in-new-tab
 	mkdocs-glightbox
 	mkdocs-git-revision-date-localized-plugin
-	cairosvg
-	pillow
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

