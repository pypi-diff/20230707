# Comparing `tmp/trilium_py-0.8.0-py3-none-any.whl.zip` & `tmp/trilium_py-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 27780 bytes, number of entries: 12
+Zip file size: 29215 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      141 b- defN 23-Apr-04 07:07 trilium_py/__init__.py
--rw-r--r--  2.0 unx    32257 b- defN 23-Jun-30 07:11 trilium_py/client.py
+-rw-r--r--  2.0 unx    33110 b- defN 23-Jul-06 09:30 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 07:07 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     8656 b- defN 23-Apr-04 07:07 trilium_py/utils/markdown_math.py
+-rw-r--r--  2.0 unx     2066 b- defN 23-Jul-06 09:30 trilium_py/utils/note_util.py
 -rw-r--r--  2.0 unx      675 b- defN 23-Apr-04 07:07 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 23-Apr-04 07:07 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      470 b- defN 23-Apr-04 07:07 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    11046 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      990 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/RECORD
-12 files, 89730 bytes uncompressed, 26110 bytes compressed:  70.9%
+-rwxrwx---  2.0 unx    35184 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    12365 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1076 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/RECORD
+13 files, 94054 bytes uncompressed, 27411 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -6,32 +6,35 @@
 
 Filename: trilium_py/utils/__init__.py
 Comment: 
 
 Filename: trilium_py/utils/markdown_math.py
 Comment: 
 
+Filename: trilium_py/utils/note_util.py
+Comment: 
+
 Filename: trilium_py/utils/param_util.py
 Comment: 
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.8.0.dist-info/LICENSE.txt
+Filename: trilium_py-0.8.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.8.0.dist-info/METADATA
+Filename: trilium_py-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.8.0.dist-info/WHEEL
+Filename: trilium_py-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.8.0.dist-info/top_level.txt
+Filename: trilium_py-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.8.0.dist-info/RECORD
+Filename: trilium_py-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -6,14 +6,15 @@
 import markdown2
 import requests
 from bs4 import BeautifulSoup
 from loguru import logger
 from natsort import natsort
 
 from .utils.markdown_math import sanitizeInput, reconstructMath
+from .utils.note_util import beautify_content
 from .utils.param_util import format_query_string, clean_param
 from .utils.time_util import get_yesterday, get_today
 
 
 class ETAPI:
 
     def __init__(self, server_url: str, token: str = None):
@@ -877,7 +878,36 @@
         url = f'{self.server_url}/etapi/backup/{backup_name}'
 
         res = requests.put(url, headers=self.get_header())
         if res.status_code == 204:
             logger.info('backup successfully')
             return True
         return False
+
+    def beautify_note(self, noteId: str) -> str:
+        """
+        beautify note content, add new lines and remove redundant lines, etc.
+
+        :param noteId:
+        :return:
+        """
+        content = self.get_note_content(noteId)
+        new_content = beautify_content(content)
+        res = self.update_note_content(noteId, new_content)
+        return res
+
+    def beautify_sub_notes(self, noteId: str):
+        """
+        beautify note and its child notes
+
+        :param noteId:
+        :return:
+        """
+        note = self.get_note(noteId)
+        logger.info(f"{noteId} {note['type']} {note['title']}")
+
+        if note['type'] == 'text':
+            self.beautify_note(noteId)
+
+        for x in note['childNoteIds']:
+            # logger.info(x)
+            self.beautify_sub_notes(x)
```

## Comparing `trilium_py-0.8.0.dist-info/LICENSE.txt` & `trilium_py-0.8.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.8.0.dist-info/METADATA` & `trilium_py-0.8.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -26,14 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: BeautifulSoup4
 Requires-Dist: requests
 Requires-Dist: markdown2[all]
 Requires-Dist: natsort
 Requires-Dist: loguru
+Requires-Dist: minify-html
 Requires-Dist: python-magic-bin ; platform_system == "Windows"
 Requires-Dist: python-magic ; sys_platform == "darwin"
 Requires-Dist: python-magic ; sys_platform == "linux"
 
 # 🐍 trilium-py
 
 Python client for ETAPI of Trilium Note.
@@ -75,15 +76,19 @@
     - [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
     - [Bulk upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder)
         - [Import from VNote](#import-from-vnote)
         - [Import from Joplin](#import-from-joplin)
         - [Import from Logseq](#import-from-logseq)
         - [Import from Obsidian](#import-from-obsidian)
         - [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
+        - [Import from Turtl](#import-from-turtl)
         - [Import from other markdown software](#import-from-other-markdown-software)
+- [(Advanced Usage) 🎨 Beautify notes](#advanced-usage--beautify-notes)
+    - [Beautify a note](#beautify-a-note)
+    - [Beautify a note and its child notes](#beautify-a-note-and-its-child-notes)
 - [🛠️ Develop](#️-develop)
 - [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
 
 <!--te-->
 
 # 🔧 Installation
 
@@ -379,27 +384,65 @@
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/gitRepo/youdaonote-pull/out/",
 )
 ```
 
+### Import from Turtl
+
+You need to convert Turtl from json to markdown first.
+See [turtl-to-markdown](https://github.com/Nriver/trilium-py/tree/main/examples/turtl-to-markdown) for details.
+
+Then you can import with trilium-py like this:
+
+```python
+res = ea.upload_md_folder(
+    parentNoteId="root",
+    mdFolder="/home/nate/gitRepo/turtl-to-markdown/out/",
+    ignoreFolder=['_resources'],
+)
+```
+
 ### Import from other markdown software
 
 In general, markdown files have variety of standards. You can always try import them with
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/data/your_markdown_files/",
 )
 ```
 
 If there is any problem, please feel free to create an [issue](https://github.com/Nriver/trilium-py/issues/new).
 
+## (Advanced Usage) 🎨 Beautify notes
+
+Because of the constraints imposed by the library utilized by Trilium, imported notes may experience minor formatting
+problems. These issues include an additional line appearing at the end of code blocks, images becoming integrated with
+the note content, and the absence of line breaks between headings, resulting in a cramped appearance of the note
+content.
+
+Here is what you can do to beautify your note.
+
+### Beautify a note
+
+Specify a note id to beautify note content.
+
+```
+ea.beautify_note('krm8B9JthNfi')
+```
+
+### Beautify a note and its child notes
+
+```
+ea.beautify_sub_notes('tlPuzU2szLJh')
+```
+
 # 🛠️ Develop
 
 Install with pip egg link to make package change without reinstall.
 
 ```python
 python -m pip install --user -e .
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.8.0 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.8.1 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
@@ -12,21 +12,21 @@
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: BeautifulSoup4 Requires-Dist: requests
 Requires-Dist: markdown2[all] Requires-Dist: natsort Requires-Dist: loguru
-Requires-Dist: python-magic-bin ; platform_system == "Windows" Requires-Dist:
-python-magic ; sys_platform == "darwin" Requires-Dist: python-magic ;
-sys_platform == "linux" # ð trilium-py Python client for ETAPI of Trilium
-Note. [![Downloads](https://static.pepy.tech/badge/trilium-py)](https://
-pepy.tech/project/trilium-py) [![Supported Versions](https://img.shields.io/
-pypi/pyversions/trilium-py.svg)](https://pypi.org/project/trilium-py) [!
-[Supported Versions](https://img.shields.io/pypi/v/trilium-
+Requires-Dist: minify-html Requires-Dist: python-magic-bin ; platform_system ==
+"Windows" Requires-Dist: python-magic ; sys_platform == "darwin" Requires-Dist:
+python-magic ; sys_platform == "linux" # ð trilium-py Python client for
+ETAPI of Trilium Note. [![Downloads](https://static.pepy.tech/badge/trilium-
+py)](https://pepy.tech/project/trilium-py) [![Supported Versions](https://
+img.shields.io/pypi/pyversions/trilium-py.svg)](https://pypi.org/project/
+trilium-py) [![Supported Versions](https://img.shields.io/pypi/v/trilium-
 py?color=%2334D058&label=pypi%20package)](https://pypi.org/project/trilium-py)
 [![PyPI license](https://img.shields.io/pypi/l/trilium-py.svg)](https://
 pypi.python.org/pypi/trilium-py/) [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [https://moe-counter--nriver1.repl.co/get/@Nriver_trilium-py]
 # ð¦® Table of Contents  - [ð trilium-py](#-trilium-py) - [ð¦® Table of
 Contents](#-table-of-contents) - [ð§ Installation](#-installation) - [ð
@@ -43,16 +43,19 @@
 yesterdays-unfinished-todo-to-today) - [(Advanced Usage) ð Upload Markdown
 files](#advanced-usage--upload-markdown-files) - [Upload single Markdown file
 with images](#upload-single-markdown-file-with-images) - [Bulk upload Markdown
 files in a folder](#bulk-upload-markdown-files-in-a-folder) - [Import from
 VNote](#import-from-vnote) - [Import from Joplin](#import-from-joplin) -
 [Import from Logseq](#import-from-logseq) - [Import from Obsidian](#import-
 from-obsidian) - [Import from Youdao Note/æéäºç¬è®°](#import-from-youdao-
-noteæéäºç¬è®°) - [Import from other markdown software](#import-from-
-other-markdown-software) - [ð ï¸ Develop](#ï¸-develop) - [ð Original
+noteæéäºç¬è®°) - [Import from Turtl](#import-from-turtl) - [Import from
+other markdown software](#import-from-other-markdown-software) - [(Advanced
+Usage) ð¨ Beautify notes](#advanced-usage--beautify-notes) - [Beautify a
+note](#beautify-a-note) - [Beautify a note and its child notes](#beautify-a-
+note-and-its-child-notes) - [ð ï¸ Develop](#ï¸-develop) - [ð Original
 OpenAPI Documentation](#-original-openapi-documentation)  # ð§ Installation
 ```bash python3 -m pip install trilium-py --user ``` # ð (Basic) Usage These
 are basic function that Trilium's ETAPI provides. Down below are some simple
 example code to use this package. ## ð Initialization If you have a ETAPI
 token, change the `server_url` and `token` to yours. ```python from
 trilium_py.client import ETAPI server_url = 'http://localhost:8080' token =
 'YOUR_TOKEN' ea = ETAPI(server_url, token) ``` If you haven't created ETAPI
@@ -124,17 +127,31 @@
 import just like a normal markdown, trilium-py will handle the images for you.
 ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="E:/data/
 out", ) ``` ### Import from Youdao Note/æéäºç¬è®° Youdao does not provide
 an export feature anymore. Luckily, you can use
 github.com/DeppWang/youdaonote-pull> to download your notes and convert them
 into markdown files. After that, trilium-py should be able to help you import
 them. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/
-home/nate/gitRepo/youdaonote-pull/out/", ) ``` ### Import from other markdown
-software In general, markdown files have variety of standards. You can always
-try import them with ```python res = ea.upload_md_folder( parentNoteId="root",
-mdFolder="/home/nate/data/your_markdown_files/", ) ``` If there is any problem,
-please feel free to create an [issue](https://github.com/Nriver/trilium-py/
-issues/new). # ð ï¸ Develop Install with pip egg link to make package change
-without reinstall. ```python python -m pip install --user -e . ``` # ð
-Original OpenAPI Documentation The original OpenAPI document is [here](https://
+home/nate/gitRepo/youdaonote-pull/out/", ) ``` ### Import from Turtl You need
+to convert Turtl from json to markdown first. See [turtl-to-markdown](https://
+github.com/Nriver/trilium-py/tree/main/examples/turtl-to-markdown) for details.
+Then you can import with trilium-py like this: ```python res =
+ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/gitRepo/turtl-
+to-markdown/out/", ignoreFolder=['_resources'], ) ``` ### Import from other
+markdown software In general, markdown files have variety of standards. You can
+always try import them with ```python res = ea.upload_md_folder
+( parentNoteId="root", mdFolder="/home/nate/data/your_markdown_files/", ) ```
+If there is any problem, please feel free to create an [issue](https://
+github.com/Nriver/trilium-py/issues/new). ## (Advanced Usage) ð¨ Beautify
+notes Because of the constraints imposed by the library utilized by Trilium,
+imported notes may experience minor formatting problems. These issues include
+an additional line appearing at the end of code blocks, images becoming
+integrated with the note content, and the absence of line breaks between
+headings, resulting in a cramped appearance of the note content. Here is what
+you can do to beautify your note. ### Beautify a note Specify a note id to
+beautify note content. ``` ea.beautify_note('krm8B9JthNfi') ``` ### Beautify a
+note and its child notes ``` ea.beautify_sub_notes('tlPuzU2szLJh') ``` #
+ð ï¸ Develop Install with pip egg link to make package change without
+reinstall. ```python python -m pip install --user -e . ``` # ð Original
+OpenAPI Documentation The original OpenAPI document is [here](https://
 github.com/zadam/trilium/blob/master/src/etapi/etapi.openapi.yaml). You can
 open it with [swagger editor](https://editor.swagger.io/).
```

