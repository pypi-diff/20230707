# Comparing `tmp/readyocr-0.0.5.tar.gz` & `tmp/readyocr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readyocr-0.0.5.tar", last modified: Thu Jul  6 06:14:59 2023, max compression
+gzip compressed data, was "readyocr-0.0.6.tar", last modified: Fri Jul  7 04:31:18 2023, max compression
```

## Comparing `readyocr-0.0.5.tar` & `readyocr-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-06 06:14:59.493054 readyocr-0.0.5/
--rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.5/LICENSE
--rw-r--r--   0 annguyen   (501) staff       (20)     1828 2023-07-06 06:14:59.492889 readyocr-0.0.5/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)       72 2023-07-06 03:07:19.000000 readyocr-0.0.5/README.md
--rw-r--r--   0 annguyen   (501) staff       (20)      908 2023-07-06 06:14:46.000000 readyocr-0.0.5/pyproject.toml
--rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-06 06:14:59.493116 readyocr-0.0.5/setup.cfg
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-06 06:14:59.486941 readyocr-0.0.5/src/
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-06 06:14:59.488422 readyocr-0.0.5/src/readyocr/
--rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.5/src/readyocr/__init__.py
--rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.5/src/readyocr/__main__.py
--rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-06-29 03:55:22.000000 readyocr-0.0.5/src/readyocr/bbox.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-06 06:14:59.492124 readyocr-0.0.5/src/readyocr/entities/
--rw-r--r--   0 annguyen   (501) staff       (20)     6096 2023-07-04 09:06:20.000000 readyocr-0.0.5/src/readyocr/entities/bbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.5/src/readyocr/entities/block.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1707 2023-07-04 10:52:14.000000 readyocr-0.0.5/src/readyocr/entities/cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2888 2023-07-05 07:48:21.000000 readyocr-0.0.5/src/readyocr/entities/document.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2819 2023-07-05 10:33:59.000000 readyocr-0.0.5/src/readyocr/entities/entity_list.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1043 2023-07-04 13:32:26.000000 readyocr-0.0.5/src/readyocr/entities/entity_tag.py
--rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.5/src/readyocr/entities/key.py
--rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.5/src/readyocr/entities/line.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1800 2023-07-04 14:14:05.000000 readyocr-0.0.5/src/readyocr/entities/merged_cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2996 2023-07-05 07:47:28.000000 readyocr-0.0.5/src/readyocr/entities/page.py
--rw-r--r--   0 annguyen   (501) staff       (20)     5117 2023-07-04 14:14:02.000000 readyocr-0.0.5/src/readyocr/entities/page_entity.py
--rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.5/src/readyocr/entities/paragraph.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1071 2023-07-04 10:51:14.000000 readyocr-0.0.5/src/readyocr/entities/table.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1702 2023-07-04 07:38:31.000000 readyocr-0.0.5/src/readyocr/entities/textbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.5/src/readyocr/entities/value.py
--rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.5/src/readyocr/entities/word.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.5/src/readyocr/exceptions.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-06 06:14:59.492414 readyocr-0.0.5/src/readyocr/parsers/
--rw-r--r--   0 annguyen   (501) staff       (20)     6168 2023-07-05 10:23:46.000000 readyocr-0.0.5/src/readyocr/parsers/google_document_ai_parser.py
--rw-r--r--   0 annguyen   (501) staff       (20)     7629 2023-07-04 14:16:46.000000 readyocr-0.0.5/src/readyocr/parsers/textract_parser.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-06 06:14:59.492672 readyocr-0.0.5/src/readyocr/utils/
--rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.5/src/readyocr/utils/geometry_utils.py
--rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.5/src/readyocr/utils/languages.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-06 06:14:59.489135 readyocr-0.0.5/src/readyocr.egg-info/
--rw-r--r--   0 annguyen   (501) staff       (20)     1828 2023-07-06 06:14:59.000000 readyocr-0.0.5/src/readyocr.egg-info/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)      989 2023-07-06 06:14:59.000000 readyocr-0.0.5/src/readyocr.egg-info/SOURCES.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-06 06:14:59.000000 readyocr-0.0.5/src/readyocr.egg-info/dependency_links.txt
--rw-r--r--   0 annguyen   (501) staff       (20)      151 2023-07-06 06:14:59.000000 readyocr-0.0.5/src/readyocr.egg-info/requires.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-06 06:14:59.000000 readyocr-0.0.5/src/readyocr.egg-info/top_level.txt
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.540905 readyocr-0.0.6/
+-rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.6/LICENSE
+-rw-r--r--   0 annguyen   (501) staff       (20)     4110 2023-07-07 04:31:18.540756 readyocr-0.0.6/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     2354 2023-07-07 04:29:22.000000 readyocr-0.0.6/README.md
+-rw-r--r--   0 annguyen   (501) staff       (20)      954 2023-07-07 04:30:46.000000 readyocr-0.0.6/pyproject.toml
+-rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-07 04:31:18.540955 readyocr-0.0.6/setup.cfg
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.530127 readyocr-0.0.6/src/
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.531594 readyocr-0.0.6/src/readyocr/
+-rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.6/src/readyocr/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.6/src/readyocr/__main__.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.538786 readyocr-0.0.6/src/readyocr/entities/
+-rw-r--r--   0 annguyen   (501) staff       (20)      627 2023-07-06 09:39:53.000000 readyocr-0.0.6/src/readyocr/entities/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     6096 2023-07-04 09:06:20.000000 readyocr-0.0.6/src/readyocr/entities/bbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.6/src/readyocr/entities/block.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1707 2023-07-04 10:52:14.000000 readyocr-0.0.6/src/readyocr/entities/cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3092 2023-07-06 09:13:13.000000 readyocr-0.0.6/src/readyocr/entities/document.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2900 2023-07-06 09:24:46.000000 readyocr-0.0.6/src/readyocr/entities/entity_list.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1044 2023-07-06 09:24:44.000000 readyocr-0.0.6/src/readyocr/entities/entity_tag.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.6/src/readyocr/entities/key.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.6/src/readyocr/entities/line.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1800 2023-07-04 14:14:05.000000 readyocr-0.0.6/src/readyocr/entities/merged_cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3184 2023-07-06 09:12:12.000000 readyocr-0.0.6/src/readyocr/entities/page.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     4740 2023-07-06 09:12:08.000000 readyocr-0.0.6/src/readyocr/entities/page_entity.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.6/src/readyocr/entities/paragraph.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1071 2023-07-04 10:51:14.000000 readyocr-0.0.6/src/readyocr/entities/table.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1702 2023-07-04 07:38:31.000000 readyocr-0.0.6/src/readyocr/entities/textbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.6/src/readyocr/entities/value.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.6/src/readyocr/entities/word.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.6/src/readyocr/exceptions.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.539394 readyocr-0.0.6/src/readyocr/parsers/
+-rw-r--r--   0 annguyen   (501) staff       (20)     5782 2023-07-07 04:10:18.000000 readyocr-0.0.6/src/readyocr/parsers/google_document_ai_parser.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     7385 2023-07-07 04:02:42.000000 readyocr-0.0.6/src/readyocr/parsers/textract_parser.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.540446 readyocr-0.0.6/src/readyocr/utils/
+-rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.6/src/readyocr/utils/geometry_utils.py
+-rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.6/src/readyocr/utils/languages.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1819 2023-07-07 03:50:49.000000 readyocr-0.0.6/src/readyocr/utils/visualize.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 04:31:18.532683 readyocr-0.0.6/src/readyocr.egg-info/
+-rw-r--r--   0 annguyen   (501) staff       (20)     4110 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     1034 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/SOURCES.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/dependency_links.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)      176 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/requires.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-07 04:31:18.000000 readyocr-0.0.6/src/readyocr.egg-info/top_level.txt
```

### Comparing `readyocr-0.0.5/LICENSE` & `readyocr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/pyproject.toml` & `readyocr-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "readyocr"
-version = "0.0.5"
+version = "0.0.6"
 description = "A nice package OCR for Amazon Textract and Google Document AI"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
   { name="Sy An", email="syan.vn@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["ocr", "textract", "documentai"]
 dependencies = [
-    "numpy"
+    "numpy",
+    "typing-extensions",
+    "Pillow",
+    "pdf2image"
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
-all = ["amazon-textract-response-parser", "google-cloud-documentai"]
-textract = ["amazon-textract-response-parser"]
+all = ["amazon-textract-textractor", "google-cloud-documentai"]
+textract = ["amazon-textract-textractor"]
 documentai = ["google-cloud-documentai"]
 
 [project.urls]
 "Homepage" = "https://github.com/syanng/readyocr"
 "Bug Tracker" = "https://github.com/syanng/readyocr/issues"
```

### Comparing `readyocr-0.0.5/src/readyocr/entities/bbox.py` & `readyocr-0.0.6/src/readyocr/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/block.py` & `readyocr-0.0.6/src/readyocr/entities/block.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/cell.py` & `readyocr-0.0.6/src/readyocr/entities/cell.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/document.py` & `readyocr-0.0.6/src/readyocr/entities/document.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import List
 
-from readyocr.entities.bbox import SpatialObject, BoundingBox
+from readyocr.entities.bbox import SpatialObject
 from readyocr.entities.page import Page
 from readyocr.entities.entity_list import EntityList
 from readyocr.exceptions import InputError
 
 
 class Document(SpatialObject):
     """ 
@@ -42,14 +42,23 @@
         Add Page objects to the Document.
 
         :param pages: List of Page objects, each representing a Page within the Document. No specific ordering is assumed with input.
         :type pages: List[Page]
         """
         self._pages = sorted(pages, key=lambda x: x.page_num)
 
+    def add(self, page: Page):
+        """
+        Add Page object to the Document.
+
+        :param page: Page object to be added to the Document.
+        :type page: Page
+        """
+        self.pages.append(page)
+
     def page(self, page_no: int = 0):
         """
         Returns :class:`Page` object/s depending on the input page_no. Follows zero-indexing.
 
         :param page_no: if int, returns single Page Object, else if list, it return a list of Page objects.
         :type page_no: int if single page, list of int if multiple pages
```

### Comparing `readyocr-0.0.5/src/readyocr/entities/entity_list.py` & `readyocr-0.0.6/src/readyocr/entities/entity_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 
     :param obj: Custom list of objects.
     :type objs: list
     """
 
     def __init__(self, objs=None):
         super().__init__()
-
+        
         if objs is None:
-            objs = []
-        elif not isinstance(objs, list):
-            objs = [objs]
+            objs = set()
+        elif isinstance(objs, list):
+            objs = set(objs)
+        elif not isinstance(objs, set):
+            objs = set([objs])
 
         self.update(objs)
 
     def filter_by_class(self, type) -> Self:
         """
         Filters the list of entities by class type.
```

### Comparing `readyocr-0.0.5/src/readyocr/entities/entity_tag.py` & `readyocr-0.0.6/src/readyocr/entities/entity_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-import os
-from typing import TypeVar, Generic
 
 
-T = TypeVar('T')
-
-
-class EntityTag(set, Generic[T]):
+class EntityTag(set):
     """
     Creates a set tag object, initially empty but extended with the set passed in objs.
 
     :param tags: Custom set of tags.
     :type tags: set
     """
 
-    def __init__(self, tags=None):
+    def __init__(self, objs=None):
         super().__init__()
 
-        if tags is None:
-            tags = []
-        elif isinstance(tags, str):
-            tags = [tags]
+        if objs is None:
+            objs = set()
+        elif isinstance(objs, list):
+            objs = set(objs)
+        elif not isinstance(objs, set):
+            objs = set([objs])
         
-        self.update(tags)
+        self.update(objs)
 
     def has(self, tags) -> bool:
         """
         Checks if the tag object has the input tag/s.
 
         :param tags: Tag/s to check for.
         :type tags: str or list
```

### Comparing `readyocr-0.0.5/src/readyocr/entities/key.py` & `readyocr-0.0.6/src/readyocr/entities/key.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/line.py` & `readyocr-0.0.6/src/readyocr/entities/line.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/merged_cell.py` & `readyocr-0.0.6/src/readyocr/entities/merged_cell.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/page.py` & `readyocr-0.0.6/src/readyocr/entities/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,34 +36,43 @@
         image=None
     ):
         super().__init__(width=width, height=height)
         self.id = id
         self.metadata = {}
         self.page_num = page_num
         self.image = image
-        self._children = EntityList([])
+        self._children = EntityList()
 
     @property
     def children(self) -> EntityList:
         """
         :return: Returns all the objects present in the Page.
         :rtype: EntityList
         """
         return self._children
     
-    @children.setter
-    def children(self, children):
+    # @children.setter
+    # def children(self, children):
+    #     """
+    #     :param children: List of children entities.
+    #     :type children: list
+    #     """
+    #     self._children = EntityList(children)
+    #     for desc in self.descendants:
+    #         desc.page_num = self.page_num
+    #         desc.page_id = self.id
+
+    def add(self, child: PageEntity):
         """
-        :param children: List of children entities.
-        :type children: list
+        _summary_
+
+        :return: _description_
+        :rtype: _type_
         """
-        self._children = EntityList(children)
-        for desc in self.descendants:
-            desc.page_num = self.page_num
-            desc.page_id = self.id
+        self._children.add(child)
 
     @property
     def descendants(self):
         """
         :return: Returns all the children of the entity.
         :rtype: list
         """
```

### Comparing `readyocr-0.0.5/src/readyocr/entities/page_entity.py` & `readyocr-0.0.6/src/readyocr/entities/page_entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,17 +26,17 @@
         :param entity_id: Unique identifier for the document entity.
         :param bbox: Bounding box of the entity
         """
 
         self.id = entity_id
         self._bbox: BoundingBox = bbox
         self.metadata = dict() # Holds optional information about the entity
-        self._children = EntityList([])
+        self._children = EntityList()
         self._raw_object = None
-        self._tags = EntityTag([])
+        self._tags = EntityTag()
 
     @property
     def raw_object(self) -> Dict:
         """
         :return: Returns the raw dictionary object that was used to create this Python object
         :rtype: Dict
         """
@@ -135,43 +135,27 @@
     def children(self) -> EntityList[Self]:
         """
         :return: Returns all the objects present in the Page.
         :rtype: EntityList
         """
         return self._children
     
-    @children.setter
-    def children(self, children: EntityList[Self]):
-        """
-        :param children: List of children entities.
-        :type children: list
-        """ 
-        self._children = EntityList(children)
-    
     @property
     def tags(self) -> EntityTag:
         """
         :return: Returns all the tags of this entity.
         :rtype: EntityTag
         """
         return self._tags
-    
-    @tags.setter
-    def tags(self, tags):
-        """
-        :param tags: List of tags.
-        :type tags: list
-        """
-        self._tags = EntityTag(tags)
 
     @property
-    def descendants(self):
+    def descendants(self) -> EntityList[Self]:
         """
         :return: Returns all the children of the entity.
-        :rtype: list
+        :rtype: EntityList
         """
         descendants = set()
         for child in self.children:
             descendants.add(child)
             for desc in child.descendants:
                 if desc not in descendants:
                     descendants.add(desc)
```

### Comparing `readyocr-0.0.5/src/readyocr/entities/paragraph.py` & `readyocr-0.0.6/src/readyocr/entities/paragraph.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/table.py` & `readyocr-0.0.6/src/readyocr/entities/table.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/textbox.py` & `readyocr-0.0.6/src/readyocr/entities/textbox.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/value.py` & `readyocr-0.0.6/src/readyocr/entities/value.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/entities/word.py` & `readyocr-0.0.6/src/readyocr/entities/word.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/exceptions.py` & `readyocr-0.0.6/src/readyocr/exceptions.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr/parsers/google_document_ai_parser.py` & `readyocr-0.0.6/src/readyocr/parsers/google_document_ai_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 from uuid import uuid4
 import json
 from google.cloud import documentai_v1 as documentai
 
-from readyocr.entities.bbox import BoundingBox
-from readyocr.entities.word import Word
-from readyocr.entities.line import Line
-from readyocr.entities.block import Block
-from readyocr.entities.paragraph import Paragraph
-from readyocr.entities.table import Table
-from readyocr.entities.cell import Cell
-from readyocr.entities.merged_cell import MergedCell
-from readyocr.entities.key import Key
-from readyocr.entities.value import Value
-from readyocr.entities.page import Page
-from readyocr.entities.document import Document
+from readyocr.entities import BoundingBox, Word, Line, Block, Paragraph, Table, Cell, Key, Value, Page, Document
 
 
 def _parse_text(text: str, text_anchor: dict):
     return ' '.join([text[text_segment.start_index:text_segment.end_index] for text_segment in text_anchor.text_segments])
 
 
 def _parse_bbox(bounding_poly: dict):
     xmin = min([vertex.x for vertex in bounding_poly.normalized_vertices])
-    ymin = min([vertex.x for vertex in bounding_poly.normalized_vertices])
+    ymin = min([vertex.y for vertex in bounding_poly.normalized_vertices])
     xmax = max([vertex.x for vertex in bounding_poly.normalized_vertices])
-    ymax = max([vertex.x for vertex in bounding_poly.normalized_vertices])
+    ymax = max([vertex.y for vertex in bounding_poly.normalized_vertices])
     width = xmax - xmin
     height = ymax - ymin
 
     bbox=BoundingBox(
         x=xmin,
         y=ymin,
         width=width,
@@ -55,116 +44,116 @@
     for idx, g_page in enumerate(g_document.pages):
         page = Page(
             id=str(uuid4()),
             width=g_page.dimension.width,
             height=g_page.dimension.height,
             page_num=(idx+1)
         )
-        page.metadata = g_page
+        page.raw_object = g_page
 
         # Add block to page
         for g_block in g_page.blocks:
             block = Block(
                 id=str(uuid4()),
                 bbox=_parse_bbox(g_block.layout.bounding_poly),
                 text=_parse_text(g_text, g_block.layout.text_anchor),
                 confidence=g_block.layout.confidence
             )
-            block.metadata = g_block
+            block.raw_object = g_block
             page.children.add(block)
 
         # Add paragraph to page
         for g_paragraph in g_page.paragraphs:
             paragraph = Paragraph(
                 id=str(uuid4()),
                 bbox=_parse_bbox(g_paragraph.layout.bounding_poly),
                 text=_parse_text(g_text, g_paragraph.layout.text_anchor),
                 confidence=g_paragraph.layout.confidence
             )
-            paragraph.metadata = g_paragraph
+            paragraph.raw_object = g_paragraph
             page.children.add(paragraph)
         
         # Add line to page
         for g_line in g_page.lines:
             line = Line(
                 id=str(uuid4()),
                 bbox=_parse_bbox(g_line.layout.bounding_poly),
                 text=_parse_text(g_text, g_line.layout.text_anchor),
                 confidence=g_line.layout.confidence
             )
-            line.metadata = g_line
+            line.raw_object = g_line
             page.children.add(line)
 
         # Add word to page
         for g_token in g_page.tokens:
             word = Word(
                 id=str(uuid4()),
                 bbox=_parse_bbox(g_token.layout.bounding_poly),
                 text=_parse_text(g_text, g_token.layout.text_anchor),
                 confidence=g_token.layout.confidence
             )
-            word.metadata = g_token
+            word.raw_object = g_token
             page.children.add(word)
 
         # Add table and cell to page
         for g_table in g_page.tables:
             table = Table(
                 id=str(uuid4()),
                 bbox=_parse_bbox(g_table.layout.bounding_poly),
                 confidence=g_table.layout.confidence
             )
-            table.metadata = g_table
+            table.raw_object = g_table
             page.children.add(table)
 
             row_index = 0
             for g_header_row in g_table.header_rows:
                 for col_index, g_cell in enumerate(g_header_row.cells):
                     cell = Cell(
                         id=str(uuid4()),
                         bbox=_parse_bbox(g_cell.layout.bounding_poly),
                         row_index=row_index,
                         col_index=col_index,
                         text=_parse_text(g_text, g_cell.layout.text_anchor),
                         confidence=g_cell.layout.confidence
                     )
-                    cell.metadata = g_cell
-                    cell.tags = 'COLUMN_HEADER'
+                    cell.raw_object = g_cell
+                    cell.tags.add('COLUMN_HEADER')
                     table.children.add(cell)
                 row_index += 1
 
             for g_body_row in g_table.body_rows:
                 for col_index, g_cell in enumerate(g_body_row.cells):
                     cell = Cell(
                         id=str(uuid4()),
                         bbox=_parse_bbox(g_cell.layout.bounding_poly),
                         row_index=row_index,
                         col_index=col_index,
                         text=_parse_text(g_text, g_cell.layout.text_anchor),
                         confidence=g_cell.layout.confidence
                     )
-                    cell.metadata = g_cell
+                    cell.raw_object = g_cell
                     table.children.add(cell)
                 row_index += 1
 
         # Add key and value to page
         for g_form_field in g_page.form_fields: 
             key = Key(
                 id=str(uuid4()),
                 bbox=_parse_bbox(g_form_field.field_name.bounding_poly),
                 text=g_form_field.field_name.text_anchor.content,
                 confidence=g_form_field.field_name.confidence
             )
-            key.metadata = g_form_field.field_name
+            key.raw_object = g_form_field.field_name
             page.children.add(key)
 
             value = Value(
                 id=str(uuid4()),
                 bbox=_parse_bbox(g_form_field.field_value.bounding_poly),
                 text=g_form_field.field_value.text_anchor.content,
                 confidence=g_form_field.field_value.confidence
             )
-            value.metadata = g_form_field.field_value
+            value.raw_object = g_form_field.field_value
             page.children.add(value)
 
         document.pages.append(page)
 
     return document
```

### Comparing `readyocr-0.0.5/src/readyocr/parsers/textract_parser.py` & `readyocr-0.0.6/src/readyocr/parsers/textract_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,10 @@
 from textractor.parsers.response_parser import parse
 
-from readyocr.entities.bbox import BoundingBox
-from readyocr.entities.word import Word
-from readyocr.entities.line import Line
-from readyocr.entities.table import Table
-from readyocr.entities.cell import Cell
-from readyocr.entities.merged_cell import MergedCell
-from readyocr.entities.key import Key
-from readyocr.entities.value import Value
-from readyocr.entities.page import Page
-from readyocr.entities.document import Document
-
+from readyocr.entities import BoundingBox, Word, Line, Table, Cell, MergedCell, Key, Value, Page, Document
 
 def load(textract_json: dict) -> Document:
     """
     Convert textract json to readyocr document
 
     :param textract_json: json response from textract
     :type textract_json: dict
@@ -149,15 +139,15 @@
                     row_index=t_cell.row_index,
                     col_index=t_cell.col_index,
                     text=t_cell.text,
                     confidence=t_cell.confidence
                 )
                 
                 if t_cell.is_column_header:
-                    cell.tags = 'COLUMN_HEADER'
+                    cell.tags.add('COLUMN_HEADER')
                 if t_cell.is_title:
                     cell.tags.add('TITLE')
                 if t_cell.is_footer:
                     cell.tags.add('FOOTER')
                 if t_cell.is_summary:
                     cell.tags.add('SUMMARY')
                 if t_cell.is_section_title:
@@ -205,13 +195,17 @@
                         row_index=row_index,
                         col_index=col_index,
                         row_span=row_span,
                         col_span=col_span,
                         text='',
                         confidence=1
                     )
-                    merged_cell.children = [x for x in table.children if x.id in [x.id for x in t_cell.siblings]]
+                    
+                    for x in table.children:
+                        if x.id in [x.id for x in t_cell.siblings]:
+                            merged_cell.children.add(x)
+
                     table.children.add(merged_cell)
 
         document.pages.append(page)
 
     return document
```

### Comparing `readyocr-0.0.5/src/readyocr/utils/languages.py` & `readyocr-0.0.6/src/readyocr/utils/languages.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.5/src/readyocr.egg-info/SOURCES.txt` & `readyocr-0.0.6/src/readyocr.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 src/readyocr/__init__.py
 src/readyocr/__main__.py
-src/readyocr/bbox.py
 src/readyocr/exceptions.py
 src/readyocr.egg-info/PKG-INFO
 src/readyocr.egg-info/SOURCES.txt
 src/readyocr.egg-info/dependency_links.txt
 src/readyocr.egg-info/requires.txt
 src/readyocr.egg-info/top_level.txt
+src/readyocr/entities/__init__.py
 src/readyocr/entities/bbox.py
 src/readyocr/entities/block.py
 src/readyocr/entities/cell.py
 src/readyocr/entities/document.py
 src/readyocr/entities/entity_list.py
 src/readyocr/entities/entity_tag.py
 src/readyocr/entities/key.py
@@ -25,8 +25,9 @@
 src/readyocr/entities/table.py
 src/readyocr/entities/textbox.py
 src/readyocr/entities/value.py
 src/readyocr/entities/word.py
 src/readyocr/parsers/google_document_ai_parser.py
 src/readyocr/parsers/textract_parser.py
 src/readyocr/utils/geometry_utils.py
-src/readyocr/utils/languages.py
+src/readyocr/utils/languages.py
+src/readyocr/utils/visualize.py
```

