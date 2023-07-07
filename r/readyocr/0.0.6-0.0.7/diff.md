# Comparing `tmp/readyocr-0.0.6.tar.gz` & `tmp/readyocr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readyocr-0.0.6.tar", last modified: Fri Jul  7 04:31:18 2023, max compression
+gzip compressed data, was "readyocr-0.0.7.tar", last modified: Fri Jul  7 08:54:15 2023, max compression
```

## Comparing `readyocr-0.0.6.tar` & `readyocr-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.540905 readyocr-0.0.6/
--rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.6/LICENSE
--rw-r--r--   0 annguyen   (501) staff       (20)     4110 2023-07-07 04:31:18.540756 readyocr-0.0.6/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)     2354 2023-07-07 04:29:22.000000 readyocr-0.0.6/README.md
--rw-r--r--   0 annguyen   (501) staff       (20)      954 2023-07-07 04:30:46.000000 readyocr-0.0.6/pyproject.toml
--rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-07 04:31:18.540955 readyocr-0.0.6/setup.cfg
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.530127 readyocr-0.0.6/src/
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.531594 readyocr-0.0.6/src/readyocr/
--rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.6/src/readyocr/__init__.py
--rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.6/src/readyocr/__main__.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.538786 readyocr-0.0.6/src/readyocr/entities/
--rw-r--r--   0 annguyen   (501) staff       (20)      627 2023-07-06 09:39:53.000000 readyocr-0.0.6/src/readyocr/entities/__init__.py
--rw-r--r--   0 annguyen   (501) staff       (20)     6096 2023-07-04 09:06:20.000000 readyocr-0.0.6/src/readyocr/entities/bbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.6/src/readyocr/entities/block.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1707 2023-07-04 10:52:14.000000 readyocr-0.0.6/src/readyocr/entities/cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     3092 2023-07-06 09:13:13.000000 readyocr-0.0.6/src/readyocr/entities/document.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2900 2023-07-06 09:24:46.000000 readyocr-0.0.6/src/readyocr/entities/entity_list.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1044 2023-07-06 09:24:44.000000 readyocr-0.0.6/src/readyocr/entities/entity_tag.py
--rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.6/src/readyocr/entities/key.py
--rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.6/src/readyocr/entities/line.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1800 2023-07-04 14:14:05.000000 readyocr-0.0.6/src/readyocr/entities/merged_cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     3184 2023-07-06 09:12:12.000000 readyocr-0.0.6/src/readyocr/entities/page.py
--rw-r--r--   0 annguyen   (501) staff       (20)     4740 2023-07-06 09:12:08.000000 readyocr-0.0.6/src/readyocr/entities/page_entity.py
--rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.6/src/readyocr/entities/paragraph.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1071 2023-07-04 10:51:14.000000 readyocr-0.0.6/src/readyocr/entities/table.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1702 2023-07-04 07:38:31.000000 readyocr-0.0.6/src/readyocr/entities/textbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.6/src/readyocr/entities/value.py
--rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.6/src/readyocr/entities/word.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.6/src/readyocr/exceptions.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.539394 readyocr-0.0.6/src/readyocr/parsers/
--rw-r--r--   0 annguyen   (501) staff       (20)     5782 2023-07-07 04:10:18.000000 readyocr-0.0.6/src/readyocr/parsers/google_document_ai_parser.py
--rw-r--r--   0 annguyen   (501) staff       (20)     7385 2023-07-07 04:02:42.000000 readyocr-0.0.6/src/readyocr/parsers/textract_parser.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.540446 readyocr-0.0.6/src/readyocr/utils/
--rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.6/src/readyocr/utils/geometry_utils.py
--rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.6/src/readyocr/utils/languages.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1819 2023-07-07 03:50:49.000000 readyocr-0.0.6/src/readyocr/utils/visualize.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.532683 readyocr-0.0.6/src/readyocr.egg-info/
--rw-r--r--   0 annguyen   (501) staff       (20)     4110 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)     1034 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/SOURCES.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/dependency_links.txt
--rw-r--r--   0 annguyen   (501) staff       (20)      176 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/requires.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/top_level.txt
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.638320 readyocr-0.0.7/
+-rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.7/LICENSE
+-rw-r--r--   0 annguyen   (501) staff       (20)     4976 2023-07-07 08:54:15.638163 readyocr-0.0.7/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     3220 2023-07-07 08:52:15.000000 readyocr-0.0.7/README.md
+-rw-r--r--   0 annguyen   (501) staff       (20)      954 2023-07-07 08:54:01.000000 readyocr-0.0.7/pyproject.toml
+-rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-07 08:54:15.638372 readyocr-0.0.7/setup.cfg
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.632150 readyocr-0.0.7/src/
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.633249 readyocr-0.0.7/src/readyocr/
+-rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.7/src/readyocr/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.7/src/readyocr/__main__.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.636899 readyocr-0.0.7/src/readyocr/entities/
+-rw-r--r--   0 annguyen   (501) staff       (20)      673 2023-07-07 07:27:48.000000 readyocr-0.0.7/src/readyocr/entities/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     6096 2023-07-04 09:06:20.000000 readyocr-0.0.7/src/readyocr/entities/bbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.7/src/readyocr/entities/block.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1707 2023-07-04 10:52:14.000000 readyocr-0.0.7/src/readyocr/entities/cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3092 2023-07-06 09:13:13.000000 readyocr-0.0.7/src/readyocr/entities/document.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2900 2023-07-06 09:24:46.000000 readyocr-0.0.7/src/readyocr/entities/entity_list.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1044 2023-07-06 09:24:44.000000 readyocr-0.0.7/src/readyocr/entities/entity_tag.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.7/src/readyocr/entities/key.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.7/src/readyocr/entities/line.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1800 2023-07-04 14:14:05.000000 readyocr-0.0.7/src/readyocr/entities/merged_cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3184 2023-07-06 09:12:12.000000 readyocr-0.0.7/src/readyocr/entities/page.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     4740 2023-07-06 09:12:08.000000 readyocr-0.0.7/src/readyocr/entities/page_entity.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.7/src/readyocr/entities/paragraph.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1071 2023-07-04 10:51:14.000000 readyocr-0.0.7/src/readyocr/entities/table.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1702 2023-07-04 07:38:31.000000 readyocr-0.0.7/src/readyocr/entities/textbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.7/src/readyocr/entities/value.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.7/src/readyocr/entities/word.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.7/src/readyocr/exceptions.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.637437 readyocr-0.0.7/src/readyocr/parsers/
+-rw-r--r--   0 annguyen   (501) staff       (20)     5782 2023-07-07 04:10:18.000000 readyocr-0.0.7/src/readyocr/parsers/google_document_ai_parser.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     7385 2023-07-07 07:50:05.000000 readyocr-0.0.7/src/readyocr/parsers/textract_parser.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.637928 readyocr-0.0.7/src/readyocr/utils/
+-rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.7/src/readyocr/utils/geometry_utils.py
+-rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.7/src/readyocr/utils/languages.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     4165 2023-07-07 08:41:10.000000 readyocr-0.0.7/src/readyocr/utils/visualize.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.633987 readyocr-0.0.7/src/readyocr.egg-info/
+-rw-r--r--   0 annguyen   (501) staff       (20)     4976 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     1034 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/SOURCES.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/dependency_links.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)      176 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/requires.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/top_level.txt
```

### Comparing `readyocr-0.0.6/LICENSE` & `readyocr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/PKG-INFO` & `readyocr-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readyocr
-Version: 0.0.6
+Version: 0.0.7
 Summary: A nice package OCR for Amazon Textract and Google Document AI
 Author-email: Sy An <syan.vn@gmail.com>
 License: Copyright 2023 Sy An
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,28 +21,31 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: textract
 Provides-Extra: documentai
 License-File: LICENSE
 
+[![License: MIT](https://img.shields.io/github/license/syanng/readyocr)](https://opensource.org/licenses/MIT) [![PyPI Version](https://img.shields.io/pypi/v/readyocr)](https://pypi.org/project/readyocr/) [![Downloads](https://img.shields.io/pypi/dm/readyocr)](https://pypi.org/project/readyocr/)
+
+
 # ReadyOCR
 
 ReadyOCR is a Python library that allows you to quickly and easily parse data from various OCR API services, including AWS Textract and Google Document AI. The package also comes with nice features for searching and visualizing.
 
-![Textract Output Visualize](images/visualize.png)
+![Textract Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize.png)
 
 ## Installation
 
 You can install ReadyOCR using pip. Depending on the OCR API service you want to use, you can install the corresponding version of ReadyOCR:
 
 * For minimal usage, if you only want to create ReadyOCR document object format:
 
     ```
-    pip install "readyocr[all]"
+    pip install readyocr
     ```
 
 * Or you can choose a specific version to support a specific API response:
 
     ```
     # support AWS Textract response
     pip install "readyocr[textract]"
@@ -52,59 +55,72 @@
 
     # support all available
     pip install "readyocr[all]"
     ```
 
 ## Basic Usage
 
-ReadyOCR allows you to create a Document object, which represents the OCR results. A Document can contain one or many pages, and each page can have multiple page entity objects, such as line, word, or table.
+* ReadyOCR allows you to create a Document object, which represents the OCR results. A Document can contain one or many pages, and each page can have multiple page entity objects, such as line, word, or table.
 
-```
-from readyocr.entities import Document, Page, Block, Paragraph, Line, Word, Table, Cell, Key, Value
+    ```
+    from readyocr.entities import Document, Page, Block, Paragraph, Line, Word, Table, Cell, Key, Value
 
-document = Document(...)
-page = Page(...)
-word = Word(...)
+    document = Document(...)
+    page = Page(...)
+    word = Word(...)
+
+    # linking all object
+    page.children.add(word)
+    document.pages.append(page)
+    ```
 
-# linking all object
-page.children.add(word)
-document.pages.append(page)
-```
+* You can define any document structure you want by using the `.children` property for page entities. For example, a line object can have many word objects as children.
 
-You can define any document structure you want by using the `.children` property for page entities. For example, a line object can have many word objects as children.
+    ```
+    page = Page(...)
+    line = Line(...)
+    word1 = Word(...)
+    word2 = Word(...)
 
-```
-page = Page(...)
-line = Line(...)
-word1 = Word(...)
-word2 = Word(...)
+    line.children = [word1, word2]
 
-line.children = [word1, word2]
+    # add line object to page children
+    page.children.add(line)
 
-# add line object to page children
-page.children.add(line)
+    # you can get descendant of a object
+    all_page_entity = page.descendant
 
-# you can get descendant of a object
-all_page_entity = page.descendant
+    # you can also filter all object by class, tag or attribute
+    all_word = page.descendant.filter_by_class(Word)
+    ```
 
-# you can also filter all object by class, tag or attribute
-all_word = page.descendant.filter_by_class(Word)
-```
+* You can also use tags attribute to identify some specific attribute:
 
-You can also use tags attribute to identify some specific attribute:
+    ```
+    table = Table(...)
+    cell = Cell(...)
+    cell.tags.add('COLUMN_HEADER')
+    table.children.add(cell)
+
+    # Get all table cell which is column header
+    table.children.filter_by_tags('COLUMN_HEADER') 
+    ```
 
-```
-table = Table(...)
-cell = Cell(...)
-cell.tags.add('COLUMN_HEADER')
-table.children.add(cell)
+* ReadyOCR support visualize for bounding box and textbox
+
+    ```
+    for item in page.descendants.filter_by_class(Line):
+        visualize_image = draw_textbox(
+            image=visualize_image, 
+            textbox=item,
+            padding=1,
+        )
+    ```
 
-# Get all table cell which is column header
-table.children.filter_by_tags('COLUMN_HEADER') 
-```
+    ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
```

### Comparing `readyocr-0.0.6/pyproject.toml` & `readyocr-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "readyocr"
-version = "0.0.6"
+version = "0.0.7"
 description = "A nice package OCR for Amazon Textract and Google Document AI"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
   { name="Sy An", email="syan.vn@gmail.com" },
 ]
 classifiers = [
```

### Comparing `readyocr-0.0.6/src/readyocr/entities/__init__.py` & `readyocr-0.0.7/src/readyocr/entities/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from readyocr.entities.bbox import BoundingBox
+from readyocr.entities.textbox import TextBox
 from readyocr.entities.word import Word
 from readyocr.entities.line import Line
 from readyocr.entities.block import Block
 from readyocr.entities.paragraph import Paragraph
 from readyocr.entities.table import Table
 from readyocr.entities.cell import Cell
 from readyocr.entities.merged_cell import MergedCell
```

### Comparing `readyocr-0.0.6/src/readyocr/entities/bbox.py` & `readyocr-0.0.7/src/readyocr/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/block.py` & `readyocr-0.0.7/src/readyocr/entities/block.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/cell.py` & `readyocr-0.0.7/src/readyocr/entities/cell.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/document.py` & `readyocr-0.0.7/src/readyocr/entities/document.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/entity_list.py` & `readyocr-0.0.7/src/readyocr/entities/entity_list.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/entity_tag.py` & `readyocr-0.0.7/src/readyocr/entities/entity_tag.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/key.py` & `readyocr-0.0.7/src/readyocr/entities/key.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/line.py` & `readyocr-0.0.7/src/readyocr/entities/line.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/merged_cell.py` & `readyocr-0.0.7/src/readyocr/entities/merged_cell.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/page.py` & `readyocr-0.0.7/src/readyocr/entities/page.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/page_entity.py` & `readyocr-0.0.7/src/readyocr/entities/page_entity.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/paragraph.py` & `readyocr-0.0.7/src/readyocr/entities/paragraph.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/table.py` & `readyocr-0.0.7/src/readyocr/entities/table.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/textbox.py` & `readyocr-0.0.7/src/readyocr/entities/textbox.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/value.py` & `readyocr-0.0.7/src/readyocr/entities/value.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/entities/word.py` & `readyocr-0.0.7/src/readyocr/entities/word.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/exceptions.py` & `readyocr-0.0.7/src/readyocr/exceptions.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/parsers/google_document_ai_parser.py` & `readyocr-0.0.7/src/readyocr/parsers/google_document_ai_parser.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr/parsers/textract_parser.py` & `readyocr-0.0.7/src/readyocr/parsers/textract_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         # Extract t_line t_word from textract and add to readyocr page
         for t_line in t_page.lines:
             line = Line(
                 id=t_line.id,
                 bbox=BoundingBox(
                     x=t_line.x,
-                    y=t_line.x,
+                    y=t_line.y,
                     width=t_line.width,
                     height=t_line.height,
                 ),
                 text=t_line.text,
                 confidence=t_line.confidence
             )
             page.children.add(line)
```

### Comparing `readyocr-0.0.6/src/readyocr/utils/languages.py` & `readyocr-0.0.7/src/readyocr/utils/languages.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.6/src/readyocr.egg-info/PKG-INFO` & `readyocr-0.0.7/src/readyocr.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readyocr
-Version: 0.0.6
+Version: 0.0.7
 Summary: A nice package OCR for Amazon Textract and Google Document AI
 Author-email: Sy An <syan.vn@gmail.com>
 License: Copyright 2023 Sy An
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,28 +21,31 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: textract
 Provides-Extra: documentai
 License-File: LICENSE
 
+[![License: MIT](https://img.shields.io/github/license/syanng/readyocr)](https://opensource.org/licenses/MIT) [![PyPI Version](https://img.shields.io/pypi/v/readyocr)](https://pypi.org/project/readyocr/) [![Downloads](https://img.shields.io/pypi/dm/readyocr)](https://pypi.org/project/readyocr/)
+
+
 # ReadyOCR
 
 ReadyOCR is a Python library that allows you to quickly and easily parse data from various OCR API services, including AWS Textract and Google Document AI. The package also comes with nice features for searching and visualizing.
 
-![Textract Output Visualize](images/visualize.png)
+![Textract Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize.png)
 
 ## Installation
 
 You can install ReadyOCR using pip. Depending on the OCR API service you want to use, you can install the corresponding version of ReadyOCR:
 
 * For minimal usage, if you only want to create ReadyOCR document object format:
 
     ```
-    pip install "readyocr[all]"
+    pip install readyocr
     ```
 
 * Or you can choose a specific version to support a specific API response:
 
     ```
     # support AWS Textract response
     pip install "readyocr[textract]"
@@ -52,59 +55,72 @@
 
     # support all available
     pip install "readyocr[all]"
     ```
 
 ## Basic Usage
 
-ReadyOCR allows you to create a Document object, which represents the OCR results. A Document can contain one or many pages, and each page can have multiple page entity objects, such as line, word, or table.
+* ReadyOCR allows you to create a Document object, which represents the OCR results. A Document can contain one or many pages, and each page can have multiple page entity objects, such as line, word, or table.
 
-```
-from readyocr.entities import Document, Page, Block, Paragraph, Line, Word, Table, Cell, Key, Value
+    ```
+    from readyocr.entities import Document, Page, Block, Paragraph, Line, Word, Table, Cell, Key, Value
 
-document = Document(...)
-page = Page(...)
-word = Word(...)
+    document = Document(...)
+    page = Page(...)
+    word = Word(...)
+
+    # linking all object
+    page.children.add(word)
+    document.pages.append(page)
+    ```
 
-# linking all object
-page.children.add(word)
-document.pages.append(page)
-```
+* You can define any document structure you want by using the `.children` property for page entities. For example, a line object can have many word objects as children.
 
-You can define any document structure you want by using the `.children` property for page entities. For example, a line object can have many word objects as children.
+    ```
+    page = Page(...)
+    line = Line(...)
+    word1 = Word(...)
+    word2 = Word(...)
 
-```
-page = Page(...)
-line = Line(...)
-word1 = Word(...)
-word2 = Word(...)
+    line.children = [word1, word2]
 
-line.children = [word1, word2]
+    # add line object to page children
+    page.children.add(line)
 
-# add line object to page children
-page.children.add(line)
+    # you can get descendant of a object
+    all_page_entity = page.descendant
 
-# you can get descendant of a object
-all_page_entity = page.descendant
+    # you can also filter all object by class, tag or attribute
+    all_word = page.descendant.filter_by_class(Word)
+    ```
 
-# you can also filter all object by class, tag or attribute
-all_word = page.descendant.filter_by_class(Word)
-```
+* You can also use tags attribute to identify some specific attribute:
 
-You can also use tags attribute to identify some specific attribute:
+    ```
+    table = Table(...)
+    cell = Cell(...)
+    cell.tags.add('COLUMN_HEADER')
+    table.children.add(cell)
+
+    # Get all table cell which is column header
+    table.children.filter_by_tags('COLUMN_HEADER') 
+    ```
 
-```
-table = Table(...)
-cell = Cell(...)
-cell.tags.add('COLUMN_HEADER')
-table.children.add(cell)
+* ReadyOCR support visualize for bounding box and textbox
+
+    ```
+    for item in page.descendants.filter_by_class(Line):
+        visualize_image = draw_textbox(
+            image=visualize_image, 
+            textbox=item,
+            padding=1,
+        )
+    ```
 
-# Get all table cell which is column header
-table.children.filter_by_tags('COLUMN_HEADER') 
-```
+    ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
```

### Comparing `readyocr-0.0.6/src/readyocr.egg-info/SOURCES.txt` & `readyocr-0.0.7/src/readyocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

