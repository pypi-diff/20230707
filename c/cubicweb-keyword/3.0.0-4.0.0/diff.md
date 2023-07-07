# Comparing `tmp/cubicweb-keyword-3.0.0.tar.gz` & `tmp/cubicweb-keyword-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-keyword-3.0.0.tar", last modified: Thu Nov 24 03:11:32 2022, max compression
+gzip compressed data, was "cubicweb-keyword-4.0.0.tar", last modified: Fri Jul  7 13:23:40 2023, max compression
```

## Comparing `cubicweb-keyword-3.0.0.tar` & `cubicweb-keyword-4.0.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.586828 cubicweb-keyword-3.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      482 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1347 2022-11-24 03:11:32.586828 cubicweb-keyword-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.574828 cubicweb-keyword-3.0.0/cubicweb_keyword/
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.578828 cubicweb-keyword-3.0.0/cubicweb_keyword/data/
--rw-rw-rw-   0 root         (0) root         (0)     1276 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/data/cubes.keyword.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.578828 cubicweb-keyword-3.0.0/cubicweb_keyword/doc/
--rw-rw-rw-   0 root         (0) root         (0)    47481 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/doc/schema.png
--rw-rw-rw-   0 root         (0) root         (0)     8172 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/doc/screenshot_keyword_tree.png
--rw-rw-rw-   0 root         (0) root         (0)     3974 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.578828 cubicweb-keyword-3.0.0/cubicweb_keyword/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     4562 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     6163 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.582828 cubicweb-keyword-3.0.0/cubicweb_keyword/migration/
--rw-rw-rw-   0 root         (0) root         (0)       55 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/migration/1.0.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/migration/1.4.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     2875 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1915 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/sobjects.py
--rw-rw-rw-   0 root         (0) root         (0)    10612 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/cubicweb_keyword/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.574828 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1347 2022-11-24 03:11:31.000000 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2022-11-24 03:11:32.000000 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 03:11:31.000000 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-24 03:11:32.000000 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 03:11:31.000000 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-24 03:11:32.000000 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-24 03:11:32.000000 cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.582828 cubicweb-keyword-3.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)    47481 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/doc/schema.png
--rw-rw-rw-   0 root         (0) root         (0)     8172 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/doc/screenshot_keyword_tree.png
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 03:11:32.586828 cubicweb-keyword-3.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2628 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.582828 cubicweb-keyword-3.0.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 03:11:32.586828 cubicweb-keyword-3.0.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/test/test_classification.py
--rw-rw-rw-   0 root         (0) root         (0)    12828 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/test/test_descendant_of.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/test/test_keyword.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/test/test_security.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2022-11-24 03:11:00.000000 cubicweb-keyword-3.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.143096 cubicweb-keyword-4.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-07 13:23:40.143096 cubicweb-keyword-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.119095 cubicweb-keyword-4.0.0/cubicweb_keyword/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.123095 cubicweb-keyword-4.0.0/cubicweb_keyword/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1276 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/data/cubes.keyword.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.123095 cubicweb-keyword-4.0.0/cubicweb_keyword/doc/
+-rw-rw-rw-   0 root         (0) root         (0)    47481 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/doc/schema.png
+-rw-rw-rw-   0 root         (0) root         (0)     8172 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/doc/screenshot_keyword_tree.png
+-rw-rw-rw-   0 root         (0) root         (0)     3917 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.123095 cubicweb-keyword-4.0.0/cubicweb_keyword/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     4562 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     6163 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.131095 cubicweb-keyword-4.0.0/cubicweb_keyword/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/migration/1.0.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/migration/1.4.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)    10740 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/cubicweb_keyword/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.123095 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-07 13:23:39.000000 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-07 13:23:40.000000 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 13:23:39.000000 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-07 13:23:39.000000 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 13:23:39.000000 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-07 13:23:39.000000 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-07 13:23:39.000000 cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.135095 cubicweb-keyword-4.0.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)    47481 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/doc/schema.png
+-rw-rw-rw-   0 root         (0) root         (0)     8172 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/doc/screenshot_keyword_tree.png
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 13:23:40.143096 cubicweb-keyword-4.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.139095 cubicweb-keyword-4.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:23:40.139095 cubicweb-keyword-4.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/test/test_classification.py
+-rw-rw-rw-   0 root         (0) root         (0)    15443 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/test/test_descendant_of.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/test/test_keyword.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/test/test_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-07 13:23:08.000000 cubicweb-keyword-4.0.0/tox.ini
```

### Comparing `cubicweb-keyword-3.0.0/PKG-INFO` & `cubicweb-keyword-4.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-keyword
-Version: 3.0.0
+Version: 4.0.0
 Summary: classification schemes system for the Cubicweb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-keyword
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -35,8 +34,7 @@
 
 Some methods are defined in order to get parents and children or get the status
 of a keyword (leaf or root).
 
 See also `cubicweb-tag`_ as another (simpler) way to classify content.
 
 .. _`cubicweb-tag`: http://www.cubicweb.org/project/cubicweb-tag
-
```

### Comparing `cubicweb-keyword-3.0.0/README.rst` & `cubicweb-keyword-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/data/cubes.keyword.js` & `cubicweb-keyword-4.0.0/cubicweb_keyword/data/cubes.keyword.js`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/doc/schema.png` & `cubicweb-keyword-4.0.0/cubicweb_keyword/doc/schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/doc/screenshot_keyword_tree.png` & `cubicweb-keyword-4.0.0/cubicweb_keyword/doc/screenshot_keyword_tree.png`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/entities.py` & `cubicweb-keyword-4.0.0/cubicweb_keyword/entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 from cubicweb.entities import AnyEntity, fetch_config, adapters
 from cubicweb.entity import EntityAdapter
 from cubicweb.predicates import is_instance
 
 
 class Classification(AnyEntity):
-    __regid__ = 'Classification'
-    fetch_attrs, cw_fetch_order = fetch_config(['name'])
+    __regid__ = "Classification"
+    fetch_attrs, cw_fetch_order = fetch_config(["name"])
 
 
 class ClassificationITreeAdapter(EntityAdapter):
-    __regid__ = 'ITree'
-    __select__ = is_instance('Classification')
+    __regid__ = "ITree"
+    __select__ = is_instance("Classification")
 
     def root(self):
         """returns the root object"""
         return None
 
     def parent(self):
         """returns the parent entity"""
@@ -32,61 +32,65 @@
 
     def iterparents(self):
         """returns parent entities"""
         yield self
 
     def children(self, entities=True):
         """returns the item's children"""
-        return self.entity.related('included_in', 'object', entities=entities)
+        return self.entity.related("included_in", "object", entities=entities)
 
     def children_rql(self):
         """XXX returns RQL to get children"""
-        return self.entity.cw_related_rql('included_in', 'object')
+        return self.entity.cw_related_rql("included_in", "object")
 
     def is_leaf(self):
         """returns true if this node as no child"""
         return bool(self.children())
 
     def is_root(self):
         """returns true if this node has no parent"""
         return True
 
-    @callable_deprecated('[3.6] was specific to external project')
+    @callable_deprecated("[3.6] was specific to external project")
     def first_level_keywords(self):
-        return self.req.execute('Any K,N ORDERBY N WHERE K included_in C, '
-                                'NOT K subkeyword_of KK, K name N, '
-                                'C eid %(x)s', {'x': self.eid})
+        return self.req.execute(
+            "Any K,N ORDERBY N WHERE K included_in C, "
+            "NOT K subkeyword_of KK, K name N, "
+            "C eid %(x)s",
+            {"x": self.eid},
+        )
 
 
 class Keyword(AnyEntity):
-    __regid__ = 'Keyword'
-    fetch_attrs, cw_fetch_order = fetch_config(['name'])
+    __regid__ = "Keyword"
+    fetch_attrs, cw_fetch_order = fetch_config(["name"])
 
 
 class KeywordITreeAdapter(adapters.ITreeAdapter):
-    __select__ = is_instance('Keyword', 'CodeKeyword')
-    tree_relation = 'subkeyword_of'
+    __select__ = is_instance("Keyword", "CodeKeyword")
+    tree_relation = "subkeyword_of"
 
     @property
     def classification(self):
         if self.entity.included_in:
             return self.entity.included_in[0]
         return None
 
     def parent(self):
         """ITree + IBreadcrumbs implementation"""
         try:
-            return self.entity.related(self.tree_relation, self.child_role,
-                                       entities=True)[0]
+            return self.entity.related(
+                self.tree_relation, self.child_role, entities=True
+            )[0]
         except (KeyError, IndexError):
             return self.classification
 
     def iterparents(self):
         """returns parent keyword entities,
-           without the root classification
+        without the root classification
         """
         if self.entity.subkeyword_of:
             parent = self.entity.subkeyword_of[0]
             while parent is not None:
                 yield parent
                 if parent.subkeyword_of:
                     parent = parent.subkeyword_of[0]
@@ -110,18 +114,17 @@
             return
         if _done is not None:
             _done.add(self.entity.eid)
             yield self.entity
         else:
             _done = set()
         for child in self.children():
-            for entity in child.cw_adapt_to('ITree').recurse_children(_done):
-                yield entity
+            yield from child.cw_adapt_to("ITree").recurse_children(_done)
 
 
 class CodeKeyword(Keyword):
-    __regid__ = 'CodeKeyword'
-    rest_attr = 'code'
-    fetch_attrs, cw_fetch_order = fetch_config(['code', 'name'])
+    __regid__ = "CodeKeyword"
+    rest_attr = "code"
+    fetch_attrs, cw_fetch_order = fetch_config(["code", "name"])
 
     def dc_title(self):
-        return u'%s - %s' % (self.code, self.name)
+        return f"{self.code} - {self.name}"
```

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/hooks.py` & `cubicweb-keyword-4.0.0/cubicweb_keyword/hooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,73 +10,88 @@
 from cubicweb import ValidationError
 from cubicweb.server.hook import Hook, Operation, match_rtype
 from yams.schema import role_name
 from cubicweb import _
 
 
 class BeforeAddDescendantOf(Hook):
-    """check indirect cycle for ``descendant_of`` relation
-    """
-    __regid__ = 'beforeadddescendant'
-    events = ('before_add_relation', )
-    __select__ = Hook.__select__ & match_rtype('descendant_of')
+    """check indirect cycle for ``descendant_of`` relation"""
+
+    __regid__ = "beforeadddescendant"
+    events = ("before_add_relation",)
+    __select__ = Hook.__select__ & match_rtype("descendant_of")
 
     def __call__(self):
         entity = self._cw.entity_from_eid(self.eidfrom)
         parent = self._cw.entity_from_eid(self.eidto)
-        parents = set([x.eid for x in chain([parent, ], parent.cw_adapt_to('ITree').iterparents())])
-        children = set([x.eid for x in chain([entity], entity.cw_adapt_to('ITree').recurse_children())])
+        parents = {
+            x.eid
+            for x in chain(
+                [
+                    parent,
+                ],
+                parent.cw_adapt_to("ITree").iterparents(),
+            )
+        }
+        children = {
+            x.eid
+            for x in chain([entity], entity.cw_adapt_to("ITree").recurse_children())
+        }
         if children & parents:
-            msg = _('detected descendant_of cycle')
-            raise ValidationError(self.eidfrom, {role_name(self.rtype, 'subject'): msg})
+            msg = _("detected descendant_of cycle")
+            raise ValidationError(self.eidfrom, {role_name(self.rtype, "subject"): msg})
 
 
 class AfterAddSubKeywordOf(Hook):
-    """sets ``descendant_of`` relation
-    """
-    __regid__ = 'afteradddescendant'
-    events = ('after_add_relation', )
-    __select__ = Hook.__select__ & match_rtype('subkeyword_of')
+    """sets ``descendant_of`` relation"""
+
+    __regid__ = "afteradddescendant"
+    events = ("after_add_relation",)
+    __select__ = Hook.__select__ & match_rtype("subkeyword_of")
 
     def __call__(self):
         entity = self._cw.entity_from_eid(self.eidfrom)
         parent = self._cw.entity_from_eid(self.eidto)
         SetDescendantOfKeywordOp(self._cw, parent=parent, entity=entity)
 
 
 class SetIncludedInRelationHook(Hook):
-    """sets the included_in relation on a subkeyword if not already set
-    """
-    __regid__ = 'setincludedinrelationhook'
-    events = ('before_add_relation',)
-    __select__ = Hook.__select__ & match_rtype('subkeyword_of')
+    """sets the included_in relation on a subkeyword if not already set"""
+
+    __regid__ = "setincludedinrelationhook"
+    events = ("before_add_relation",)
+    __select__ = Hook.__select__ & match_rtype("subkeyword_of")
 
     def __call__(self):
         # immediate test direct cycles
         if self.eidfrom == self.eidto:
-            msg = self._cw._('keyword cannot be subkeyword of himself')
-            raise ValidationError(self.eidfrom, {role_name(self.rtype, 'subject'): msg})
-        SetIncludedInRelationOp(self._cw, vreg=self._cw.vreg,
-                                eidfrom=self.eidfrom, eidto=self.eidto)
+            msg = self._cw._("keyword cannot be subkeyword of himself")
+            raise ValidationError(self.eidfrom, {role_name(self.rtype, "subject"): msg})
+        SetIncludedInRelationOp(
+            self._cw, vreg=self._cw.vreg, eidfrom=self.eidfrom, eidto=self.eidto
+        )
 
 
 class RemoveDescendantOfRelation(Hook):
     """removes ``descendant_of`` relation
 
     we delete the relation for entity's parents recursively
     """
-    __regid__ = 'removedescendantofrelation'
-    events = ('after_delete_relation',)
-    __select__ = Hook.__select__ & match_rtype('subkeyword_of')
+
+    __regid__ = "removedescendantofrelation"
+    events = ("after_delete_relation",)
+    __select__ = Hook.__select__ & match_rtype("subkeyword_of")
 
     def __call__(self):
         parent = self._cw.entity_from_eid(self.eidto)
-        for parent in chain([parent], parent.cw_adapt_to('ITree').iterparents()):
-            self._cw.execute('DELETE K descendant_of P WHERE K eid %(k)s, '
-                             'P eid %(p)s', {'p': parent.eid, 'k': self.eidfrom})
+        for parent in chain([parent], parent.cw_adapt_to("ITree").iterparents()):
+            self._cw.execute(
+                "DELETE K descendant_of P WHERE K eid %(k)s, " "P eid %(p)s",
+                {"p": parent.eid, "k": self.eidfrom},
+            )
 
 
 # operations #################################################################
 class SetIncludedInRelationOp(Operation):
     """delay this operation to commit to avoid conflict with a late rql query
     already setting the relation
     """
@@ -85,40 +100,55 @@
         cnx = self.cnx
         # test for indirect cycles
         self.check_cycle()
         subkw = cnx.entity_from_eid(self.eidfrom)
         if subkw.included_in:
             kw = cnx.entity_from_eid(self.eidto)
             if subkw.included_in[0].eid != kw.included_in[0].eid:
-                msgid = "keywords %(subkw)s and %(kw)s belong to different classifications"
-                raise ValidationError(subkw.eid, {role_name('subkeyword_of', 'subject'): cnx._(msgid) %
-                                                  {'subkw': subkw.eid, 'kw': kw.eid}})
+                msgid = (
+                    "keywords %(subkw)s and %(kw)s belong to different classifications"
+                )
+                raise ValidationError(
+                    subkw.eid,
+                    {
+                        role_name("subkeyword_of", "subject"): cnx._(msgid)
+                        % {"subkw": subkw.eid, "kw": kw.eid}
+                    },
+                )
         else:
-            cnx.execute('SET SK included_in C WHERE SK eid %(x)s, '
-                        'SK subkeyword_of K, K included_in C',
-                        {'x': subkw.eid})
+            cnx.execute(
+                "SET SK included_in C WHERE SK eid %(x)s, "
+                "SK subkeyword_of K, K included_in C",
+                {"x": subkw.eid},
+            )
 
     def check_cycle(self):
-        parents = set([self.eidto])
+        parents = {self.eidto}
         parent = self.cnx.entity_from_eid(self.eidto)
         while parent.subkeyword_of:
             parent = parent.subkeyword_of[0]
             if parent.eid in parents:
-                msg = self.cnx._('detected subkeyword cycle')
-                raise ValidationError(self.eidfrom, {role_name('subkeyword_of', 'subject'): msg})
+                msg = self.cnx._("detected subkeyword cycle")
+                raise ValidationError(
+                    self.eidfrom, {role_name("subkeyword_of", "subject"): msg}
+                )
             parents.add(parent.eid)
 
 
 class SetDescendantOfKeywordOp(Operation):
     def precommit_event(self):
         """transitive closure of ``descendant_of`` relations to current entity"""
         closure = set()
         entity = self.entity
         parent = self.parent
-        for parent in chain([parent, entity], parent.cw_adapt_to('ITree').iterparents()):
-            for child in chain([entity], entity.cw_adapt_to('ITree').recurse_children()):
+        for parent in chain(
+            [parent, entity], parent.cw_adapt_to("ITree").iterparents()
+        ):
+            for child in chain(
+                [entity], entity.cw_adapt_to("ITree").recurse_children()
+            ):
                 if child.eid != parent.eid:
                     closure.add((child, parent))
         for child, parent in closure:
             descendants = [p.eid for p in child.descendant_of]
             if parent.eid not in descendants:
                 child.cw_set(descendant_of=parent)
```

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/i18n/en.po` & `cubicweb-keyword-4.0.0/cubicweb_keyword/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/i18n/fr.po` & `cubicweb-keyword-4.0.0/cubicweb_keyword/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/schema.py` & `cubicweb-keyword-4.0.0/cubicweb_keyword/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,83 +7,89 @@
 from yams.buildobjs import EntityType, RelationType, SubjectRelation, String
 
 from cubicweb import _
 from cubicweb.schema import RQLConstraint
 
 
 class Classification(EntityType):
-    """classification schemes are used by users to classify entities.
-    """
+    """classification schemes are used by users to classify entities."""
+
     __permissions__ = {
-        'read': ('managers', 'users', 'guests'),
-        'add': ('managers', ),
-        'delete': ('managers', ),
-        'update': ('managers', ),
+        "read": ("managers", "users", "guests"),
+        "add": ("managers",),
+        "delete": ("managers",),
+        "update": ("managers",),
     }
     name = String(required=True, fulltextindexed=True, unique=True, maxsize=128)
     classifies = SubjectRelation(
-        'CWEType',
+        "CWEType",
         # see relation type docstring
         constraints=[
             RQLConstraint(
-                'RDEF to_entity O,'
-                'RDEF relation_type R,'
-                'R name "applied_to"',
+                "RDEF to_entity O," "RDEF relation_type R," 'R name "applied_to"',
                 msg="Classification is trying to classifies an EntityType "
-                "without applied_to relation"
+                "without applied_to relation",
             )
-        ]
+        ],
     )
 
 
 class classifies(RelationType):
     """entity types classified by the classification. Only entity type
     supporting the applied_to relation can be selectioned
     """
 
 
 class Keyword(EntityType):
     """A keyword is like a tag but is application specific
     and used to define a classification scheme
     """
+
     __permissions__ = {
-        'read': ('managers', 'users', 'guests'),
-        'add': ('managers', 'users'),
-        'delete': ('managers', ),
-        'update': ('managers', ),
+        "read": ("managers", "users", "guests"),
+        "add": ("managers", "users"),
+        "delete": ("managers",),
+        "update": ("managers",),
     }
     name = String(required=True, fulltextindexed=True, indexed=True, maxsize=128)
 
     subkeyword_of = SubjectRelation(
-        'Keyword', cardinality='?*',
-        description=_('which keyword (if any) this keyword specializes'),
+        "Keyword",
+        cardinality="?*",
+        description=_("which keyword (if any) this keyword specializes"),
         # if no included_in set, it'll be automatically added by a hook
-        constraints=[RQLConstraint(
-            'NOT S included_in CS1 OR EXISTS(S included_in CS2, O included_in CS2)'
-        )])
-    descendant_of = SubjectRelation('Keyword')
-    included_in = SubjectRelation('Classification', cardinality='1*')
+        constraints=[
+            RQLConstraint(
+                "NOT S included_in CS1 OR EXISTS(S included_in CS2, O included_in CS2)"
+            )
+        ],
+    )
+    descendant_of = SubjectRelation("Keyword")
+    included_in = SubjectRelation("Classification", cardinality="1*")
 
 
 class CodeKeyword(Keyword):
-    """A CodeKeyword is a keyword with a code and a name
-    """
+    """A CodeKeyword is a keyword with a code and a name"""
+
     __specializes_schema__ = True
     code = String(required=True, fulltextindexed=True, indexed=True, maxsize=128)
 
 
 class subkeyword_of(RelationType):
     """a keyword can specialize another keyword"""
 
 
 class included_in(RelationType):
     """a keyword is included in a classification scheme"""
+
     inlined = True
 
 
 # define in parent application which entity types may be linked to a keyword
 # by the applied_to relation
 
+
 class applied_to(RelationType):
     """tagged objects"""
-    fulltext_container = 'object'
-    constraints = [RQLConstraint('S included_in CS, O is ET, CS classifies ET')]
+
+    fulltext_container = "object"
+    constraints = [RQLConstraint("S included_in CS, O is ET, CS classifies ET")]
```

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/sobjects.py` & `cubicweb-keyword-4.0.0/cubicweb_keyword/sobjects.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,48 +10,51 @@
 
 from cubicweb.predicates import is_instance
 from cubicweb.sobjects.notification import NotificationView
 from cubicweb import _
 
 
 class KeywordNotificationView(NotificationView):
-    __select__ = is_instance('Keyword')
+    __select__ = is_instance("Keyword")
     msgid_timestamp = True
 
     def recipients(self):
         """Returns the project's interested people (entities)"""
         creator = self.cw_rset.get_entity(0, 0).created_by[0]
-        if not creator.is_in_group('managers') and creator.primary_email:
-            return [(creator.primary_email[0].address, 'fr')]
+        if not creator.is_in_group("managers") and creator.primary_email:
+            return [(creator.primary_email[0].address, "fr")]
         return []
 
     def context(self, **kwargs):
         context = NotificationView.context(self, **kwargs)
         entity = self.cw_rset.get_entity(0, 0)
-        context['kw'] = entity.name
+        context["kw"] = entity.name
         return context
 
 
 class KeywordNameChanged(KeywordNotificationView):
-    __regid__ = 'notif_after_update_entity'
+    __regid__ = "notif_after_update_entity"
 
     content = _("keyword name changed from %(oldname)s to %(kw)s")
 
     @cached
     def get_oldname(self, entity):
         session = self.req
         try:
-            return session.execute('Any N WHERE X eid %(x)s, X name N',
-                                   {'x': entity.eid}, 'x')[0][0]
+            return session.execute(
+                "Any N WHERE X eid %(x)s, X name N", {"x": entity.eid}, "x"
+            )[0][0]
         except IndexError:
-            return u'?'
+            return "?"
 
     def context(self, **kwargs):
         entity = self.cw_rset.get_entity(0, 0)
         context = KeywordNotificationView.context(self, **kwargs)
-        context['oldname'] = self.get_oldname(entity)
+        context["oldname"] = self.get_oldname(entity)
         return context
 
     def subject(self):
         entity = self.cw_rset.get_entity(0, 0)
-        return self.req._('keyword name changed from %s to %s') % (
-            self.get_oldname(entity), entity.name)
+        return self.req._("keyword name changed from %s to %s") % (
+            self.get_oldname(entity),
+            entity.name,
+        )
```

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword/views.py` & `cubicweb-keyword-4.0.0/cubicweb_keyword/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,266 +14,307 @@
 from cubicweb_web import stdmsgs, component, facet
 from cubicweb_web.views import primary, treeview
 from cubicweb_web.views.ajaxcontroller import ajaxfunc
 
 from cubicweb_web.views import uicfg
 
 _pvs = uicfg.primaryview_section
-_pvs.tag_object_of(('*', 'applied_to', '*'), 'hidden')
-_pvs.tag_subject_of(('*', 'applied_to', '*'), 'hidden')
-_pvs.tag_object_of(('*', 'included_in', 'Classification'), 'hidden')
+_pvs.tag_object_of(("*", "applied_to", "*"), "hidden")
+_pvs.tag_subject_of(("*", "applied_to", "*"), "hidden")
+_pvs.tag_object_of(("*", "included_in", "Classification"), "hidden")
 
 _abaa = uicfg.actionbox_appearsin_addmenu
-_abaa.tag_object_of(('CodeKeyword', 'included_in', 'Classification'), True)
-_abaa.tag_object_of(('Keyword', 'included_in', 'Classification'), True)
-_abaa.tag_object_of(('CodeKeyword', 'subkeyword_of', 'CodeKeyword'), True)
-_abaa.tag_object_of(('Keyword', 'subkeyword_of', 'Keyword'), True)
+_abaa.tag_object_of(("CodeKeyword", "included_in", "Classification"), True)
+_abaa.tag_object_of(("Keyword", "included_in", "Classification"), True)
+_abaa.tag_object_of(("CodeKeyword", "subkeyword_of", "CodeKeyword"), True)
+_abaa.tag_object_of(("Keyword", "subkeyword_of", "Keyword"), True)
 
 
 # classification views ########################################################
 
+
 class ClassificationPrimaryView(primary.PrimaryView):
-    __select__ = is_instance('Classification')
+    __select__ = is_instance("Classification")
 
     def render_entity_attributes(self, entity):
         pass
 
     def render_entity_relations(self, entity):
-        rset = self._cw.execute('Any K ORDERBY N WHERE K included_in C, '
-                                'NOT K subkeyword_of KK, K name N, '
-                                'C eid %(x)s', {'x': entity.eid})
-        self.wview('treeview', rset, 'null')
+        rset = self._cw.execute(
+            "Any K ORDERBY N WHERE K included_in C, "
+            "NOT K subkeyword_of KK, K name N, "
+            "C eid %(x)s",
+            {"x": entity.eid},
+        )
+        self.wview("treeview", rset, "null")
 
 
 # keyword views ###############################################################
 
+
 class KeywordPrimaryView(primary.PrimaryView):
-    __select__ = is_instance('Keyword')
+    __select__ = is_instance("Keyword")
 
     def cell_call(self, row, col, **kwargs):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(u'<h1 class="titleUnderline">%s</h1>'
-               % xml_escape(entity.dc_long_title()))
-        rset = entity.related('subkeyword_of', 'object')
-        self.wview('treeview', rset, 'null')
+        self.w(f'<h1 class="titleUnderline">{xml_escape(entity.dc_long_title())}</h1>')
+        rset = entity.related("subkeyword_of", "object")
+        self.wview("treeview", rset, "null")
 
 
 class KeywordComboBoxView(treeview.TreePathView):
     """display keyword in edition's combobox"""
-    __regid__ = 'combobox'
-    __select__ = is_instance('Keyword', 'Classification')
 
-    item_vid = 'text'
-    separator = u' > '
+    __regid__ = "combobox"
+    __select__ = is_instance("Keyword", "Classification")
+
+    item_vid = "text"
+    separator = " > "
+
 
 # skos views ############################################################
 
 
-SKOS_OPENING_ROOT = u'''<?xml version="1.0" encoding="UTF-8"?>
+SKOS_OPENING_ROOT = """<?xml version="1.0" encoding="UTF-8"?>
 <!DOCTYPE rdfs [
     <!ENTITY rdf "http://www.w3.org/1999/02/22-rdf-syntax-ns#">
     <!ENTITY rdfs "http://www.w3.org/2000/01/rdf-schema#">
     <!ENTITY dc "http://purl.org/dc/elements/1.1/">
     <!ENTITY dct "http://purl.org/dc/terms/">
 ]>
 <rdf:RDF  xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
           xmlns:skos="http://www.w3.org/2004/02/skos/core#">
-'''
-SKOS_CLOSING_ROOT = u'</rdf:RDF>'
+"""
+SKOS_CLOSING_ROOT = "</rdf:RDF>"
 
 
 class SkosView(EntityView):
-    __regid__ = 'skos'
-    content_type = 'application/xml'
+    __regid__ = "skos"
+    content_type = "application/xml"
     templatable = False
-    __select__ = is_instance('Keyword', 'Classification')
+    __select__ = is_instance("Keyword", "Classification")
 
     def call(self, **kwargs):
         self.w(SKOS_OPENING_ROOT)
         for i in range(self.rset.rowcount):
             self.cell_call(i, 0)
         self.w(SKOS_CLOSING_ROOT)
 
     def cell_call(self, row, col):
-        self.wview('skositemview', self.rset, row=row, col=col)
+        self.wview("skositemview", self.rset, row=row, col=col)
 
 
 class SkosItemView(EntityView):
-    __regid__ = 'skositemview'
-    content_type = 'application/xml'
-    __select__ = is_instance('Keyword', 'Classification')
+    __regid__ = "skositemview"
+    content_type = "application/xml"
+    __select__ = is_instance("Keyword", "Classification")
 
     def cell_call(self, row, col, show_parent=True, stop=False):
         w = self.w
         entity = self.complete_entity(row, col)
         eschema = entity.e_schema
-        w(u'<skos:%s>' % eschema)
-        w(u'<skos:prefLabel>%s</skos:prefLabel>' % xml_escape(entity.name))
+        w(f"<skos:{eschema}>")
+        w(f"<skos:prefLabel>{xml_escape(entity.name)}</skos:prefLabel>")
         if not stop:
             if show_parent and not entity.is_root():
                 par = entity.parent()
-                w(u'<skos:broader>')
-                par.view('skositemview', show_parent=False, stop=True, w=self.w)
-                w(u'</skos:broader>')
+                w("<skos:broader>")
+                par.view("skositemview", show_parent=False, stop=True, w=self.w)
+                w("</skos:broader>")
             for child in entity.children(entities=True):
-                w(u'<skos:narrower>')
-                self.wview('skositemview', child.as_rset(), show_parent=False)
-                w(u'</skos:narrower>')
-        w(u'</skos:%s>' % eschema)
+                w("<skos:narrower>")
+                self.wview("skositemview", child.as_rset(), show_parent=False)
+                w("</skos:narrower>")
+        w(f"</skos:{eschema}>")
 
 
 # keyword component ###########################################################
 
+
 class KeywordBarVComponent(component.EntityCtxComponent):
     """the keywords path bar: display keywords of a tagged entity"""
-    __regid__ = 'keywordsbar'
-    __select__ = (component.EntityCtxComponent.__select__ &
-                  relation_possible('applied_to', 'object', 'Keyword'))
-    context = 'header'
+
+    __regid__ = "keywordsbar"
+    __select__ = component.EntityCtxComponent.__select__ & relation_possible(
+        "applied_to", "object", "Keyword"
+    )
+    context = "header"
     order = 152
-    htmlclass = 'navigation'
+    htmlclass = "navigation"
 
     def get_keywords(self):
         """helper method for subclasses redefinition"""
-        return self.entity.related('applied_to', 'object')
+        return self.entity.related("applied_to", "object")
 
     def render_body(self, w):
         rset = self.get_keywords()
         if rset:
-            w(u'<div class="%s" id="%s">\n' % (self.cssclass, self.domid))
-            w(u'<span>%s</span>&nbsp;' % self._cw._('keywords:'))
-            self._cw.view('csv', rset, 'null', w=w)
-            w(u'</div>\n')
+            w(f'<div class="{self.cssclass}" id="{self.domid}">\n')
+            w(f"<span>{self._cw._('keywords:')}</span>&nbsp;")
+            self._cw.view("csv", rset, "null", w=w)
+            w("</div>\n")
         else:
-            w(u'<div class="%s hidden" id="%s"></div>\n' % (
-                self.cssclass, self.domid))
+            w(f'<div class="{self.cssclass} hidden" id="{self.domid}"></div>\n')
 
 
 class AddKeywordVComponent(component.EntityCtxComponent):
     """the 'add keyword' component"""
-    __regid__ = 'addkeywords'
-    __select__ = component.EntityCtxComponent.__select__ & \
-        relation_possible('applied_to', 'object', 'Keyword', action='add') & \
-        rql_condition('X is ET, CL classifies ET')
 
-    context = 'header'
+    __regid__ = "addkeywords"
+    __select__ = (
+        component.EntityCtxComponent.__select__
+        & relation_possible("applied_to", "object", "Keyword", action="add")
+        & rql_condition("X is ET, CL classifies ET")
+    )
+
+    context = "header"
     order = 153
-    htmlclass = 'navigation'
+    htmlclass = "navigation"
 
     def render_body(self, w):
         entity = self.entity
-        self._cw.add_js(['cubicweb.widgets.js', 'cubes.keyword.js'])
-        self._cw.add_css('cubicweb.suggest.css')
-        w(u'<table><tr><td>')
-        w(u'<a class="button sglink" href="javascript: showKeywordSelector(%s, \'%s\', \'%s\');">%s</a></td>' % (
-            entity.eid, self._cw._(stdmsgs.BUTTON_OK[0]),
-            self._cw._(stdmsgs.BUTTON_CANCEL[0]), self._cw._('add keywords')))
-        w(u'<td><div id="kwformholder"></div>')
-        w(u'</td></tr></table>')
+        self._cw.add_js(["cubicweb.widgets.js", "cubes.keyword.js"])
+        self._cw.add_css("cubicweb.suggest.css")
+        w("<table><tr><td>")
+        w(
+            "<a class=\"button sglink\" href=\"javascript: showKeywordSelector({}, '{}', '{}');\">{}</a></td>".format(
+                entity.eid,
+                self._cw._(stdmsgs.BUTTON_OK[0]),
+                self._cw._(stdmsgs.BUTTON_CANCEL[0]),
+                self._cw._("add keywords"),
+            )
+        )
+        w('<td><div id="kwformholder"></div>')
+        w("</td></tr></table>")
 
 
 # applied_to relation facet ####################################################
 
+
 class AppliedToFacet(facet.RelationFacet):
-    __regid__ = 'applied-to-facet'
-    rtype = 'applied_to'
-    role = 'object'
-    target_attr = 'name'
+    __regid__ = "applied-to-facet"
+    rtype = "applied_to"
+    role = "object"
+    target_attr = "name"
 
     def rset_vocabulary(self, rset):
         _ = self._cw._
         vocab = []
         scheme = None
-        for e in sorted(rset.entities(),
-                        key=lambda e: (e.cw_adapt_to('ITree').classification.name,
-                                       e.view('combobox'))):
-            classification_name = e.cw_adapt_to('ITree').classification.name
+        for e in sorted(
+            rset.entities(),
+            key=lambda e: (
+                e.cw_adapt_to("ITree").classification.name,
+                e.view("combobox"),
+            ),
+        ):
+            classification_name = e.cw_adapt_to("ITree").classification.name
             if scheme != classification_name:
                 vocab.append((_(classification_name), None))
-            vocab.append((e.view('combobox'), e.eid))
+            vocab.append((e.view("combobox"), e.eid))
         return vocab
 
 
 class ClassificationFacet(facet.RelationFacet):
     """abstract per-classification facet
 
     subclasses must define their own id the classification name, e.g :
 
     class Classifaction1Facet(ClassificationFacet):
         __regid__ = 'classif1'
         classification = u'classification1'
 
     """
+
     __abstract__ = True
     classification = None
-    rtype = 'applied_to'
-    role = 'object'
+    rtype = "applied_to"
+    role = "object"
 
     def vocabulary(self):
-        """return vocabulary for this facet, eg a list of 2-uple (label, value)
-        """
+        """return vocabulary for this facet, eg a list of 2-uple (label, value)"""
         rqlst = self.rqlst
         rqlst.save_state()
         try:
             mainvar = self.filtered_variable  # X
             keyword_var = rqlst.make_variable()  # K
             keyword_name_var = rqlst.make_variable()  # KN
             classif_var = rqlst.make_variable()  # C
             rqlst.make_variable()  # CN
-            rqlst.add_relation(keyword_var, 'applied_to', mainvar)  # K applied_to X
-            rqlst.add_relation(keyword_var, 'name', keyword_name_var)  # K name KN
-            rqlst.add_relation(keyword_var, 'included_in', classif_var)  # K included_in C
+            rqlst.add_relation(keyword_var, "applied_to", mainvar)  # K applied_to X
+            rqlst.add_relation(keyword_var, "name", keyword_name_var)  # K name KN
+            rqlst.add_relation(
+                keyword_var, "included_in", classif_var
+            )  # K included_in C
             # C name "classification-name"
-            rqlst.add_constant_restriction(classif_var, 'name', self.classification, 'String')
+            rqlst.add_constant_restriction(
+                classif_var, "name", self.classification, "String"
+            )
             rqlst.add_selected(keyword_var)
             rqlst.add_selected(keyword_name_var)
             # ORDERBY KN
             rqlst.add_sort_var(keyword_name_var, True)
             try:
-                rset = self._cw.execute(rqlst.as_string(), self.rset.args,
-                                        self.rset.cachekey)
+                rset = self._cw.execute(
+                    rqlst.as_string(), self.rset.args, self.rset.cachekey
+                )
             except Unauthorized:
                 return []
         finally:
             rqlst.recover()
         return self.rset_vocabulary(rset)
 
     @property
     def title(self):
         return self._cw._(self.classification)
 
     def support_and(self):
         return False
 
+
 # add some classification schema related methods to the Jsoncontroller ########
 
 
-@ajaxfunc(output_type='json')
+@ajaxfunc(output_type="json")
 def js_possible_keywords(self, eid):
-    rql = ('DISTINCT Any N WHERE K is Keyword, K name N, NOT K applied_to X, '
-           'X eid %(x)s, K included_in C, C classifies ET, X is ET')
-    rset = self.cursor.execute(rql, {'x': eid, 'u': self._cw.user.eid}, 'x')
+    rql = (
+        "DISTINCT Any N WHERE K is Keyword, K name N, NOT K applied_to X, "
+        "X eid %(x)s, K included_in C, C classifies ET, X is ET"
+    )
+    rset = self.cursor.execute(rql, {"x": eid, "u": self._cw.user.eid}, "x")
     return [name for (name,) in rset]
 
 
-@ajaxfunc(output_type='json')
+@ajaxfunc(output_type="json")
 def js_add_keywords(self, eid, kwlist):
-    msg = self._cw._('keywords applied')
-    kwrset = self.cursor.execute('Any K,N,C WHERE K is Keyword, K name N, K included_in C, '
-                                 'C classifies ET, X eid %(x)s, X is ET',
-                                 {'x': eid}, 'x')
+    msg = self._cw._("keywords applied")
+    kwrset = self.cursor.execute(
+        "Any K,N,C WHERE K is Keyword, K name N, K included_in C, "
+        "C classifies ET, X eid %(x)s, X is ET",
+        {"x": eid},
+        "x",
+    )
     if not kwrset:
-        return self._cw._('No suitable classification scheme found')
+        return self._cw._("No suitable classification scheme found")
     classification = kwrset[0][2]  # XXX what if we have several classifications ?
-    valid_keywords = set(kwname for _, kwname, _ in kwrset)
+    valid_keywords = {kwname for _, kwname, _ in kwrset}
     user_keywords = set(kwlist)
     invalid_keywords = sorted(user_keywords - valid_keywords)
-    kweids = dict((kwname, str(kweid)) for kweid, kwname, _ in kwrset if kwname in user_keywords)
+    kweids = {
+        kwname: str(kweid) for kweid, kwname, _ in kwrset if kwname in user_keywords
+    }
     if invalid_keywords:
         for keyword in invalid_keywords:
-            neweid = self.cursor.execute('INSERT Keyword K: K name %(name)s, K included_in C WHERE C eid %(c)s',
-                                         {'name': keyword, 'c': classification}, 'c')[0][0]
+            neweid = self.cursor.execute(
+                "INSERT Keyword K: K name %(name)s, K included_in C WHERE C eid %(c)s",
+                {"name": keyword, "c": classification},
+                "c",
+            )[0][0]
             kweids[keyword] = str(neweid)
     if kweids:
-        self.cursor.execute('SET KW applied_to X WHERE X eid %%(x)s, KW eid IN (%s)'
-                            % ','.join(kweids.values()), {'x': eid}, 'x')
+        self.cursor.execute(
+            "SET KW applied_to X WHERE X eid %%(x)s, KW eid IN (%s)"
+            % ",".join(kweids.values()),
+            {"x": eid},
+            "x",
+        )
     return msg
```

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/PKG-INFO` & `cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-keyword
-Version: 3.0.0
+Version: 4.0.0
 Summary: classification schemes system for the Cubicweb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-keyword
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -35,8 +34,7 @@
 
 Some methods are defined in order to get parents and children or get the status
 of a keyword (leaf or root).
 
 See also `cubicweb-tag`_ as another (simpler) way to classify content.
 
 .. _`cubicweb-tag`: http://www.cubicweb.org/project/cubicweb-tag
-
```

### Comparing `cubicweb-keyword-3.0.0/cubicweb_keyword.egg-info/SOURCES.txt` & `cubicweb-keyword-4.0.0/cubicweb_keyword.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/doc/schema.png` & `cubicweb-keyword-4.0.0/doc/schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/doc/screenshot_keyword_tree.png` & `cubicweb-keyword-4.0.0/doc/screenshot_keyword_tree.png`

 * *Files identical despite different names*

### Comparing `cubicweb-keyword-3.0.0/setup.py` & `cubicweb-keyword-4.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,56 +27,55 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_keyword', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_keyword", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README.rst')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'keyword=cubicweb_keyword',
+        "cubicweb.cubes": [
+            "keyword=cubicweb_keyword",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-keyword-3.0.0/test/test_classification.py` & `cubicweb-keyword-4.0.0/test/test_classification.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,81 @@
 from cubicweb.devtools.testlib import CubicWebTC
 
 from cubicweb import ValidationError
 
 
 class ClassificationHooksTC(CubicWebTC):
-
     def setup_database(self):
         with self.admin_access.cnx() as cnx:
             # classification for CWGroup
             cwgroup = cnx.execute('Any U WHERE U is ET, U name "CWGroup"').one()
-            self.classif1_eid = cnx.create_entity('Classification', name=u"classif1", classifies=cwgroup).eid
-            self.kwgroup_eid = cnx.create_entity('Keyword', name=u'kwgroup', included_in=self.classif1_eid).eid
+            self.classif1_eid = cnx.create_entity(
+                "Classification", name="classif1", classifies=cwgroup
+            ).eid
+            self.kwgroup_eid = cnx.create_entity(
+                "Keyword", name="kwgroup", included_in=self.classif1_eid
+            ).eid
             # classification for CWUser
             cwuser = cnx.execute('Any U WHERE U is ET, U name "CWUser"').one()
-            self.classif2_eid = cnx.create_entity('Classification', name=u"classif2", classifies=cwuser).eid
-            self.kwuser_eid = cnx.create_entity('Keyword', name=u'kwuser', included_in=self.classif2_eid).eid
+            self.classif2_eid = cnx.create_entity(
+                "Classification", name="classif2", classifies=cwuser
+            ).eid
+            self.kwuser_eid = cnx.create_entity(
+                "Keyword", name="kwuser", included_in=self.classif2_eid
+            ).eid
             cnx.commit()
 
     def test_application_of_bad_keyword_fails(self):
         with self.admin_access.cnx() as cnx:
-            cnx.execute('SET K applied_to G WHERE G is CWGroup, K eid %(k)s',
-                        {'k': self.kwuser_eid})
+            cnx.execute(
+                "SET K applied_to G WHERE G is CWGroup, K eid %(k)s",
+                {"k": self.kwuser_eid},
+            )
             self.assertRaises(ValidationError, cnx.commit)
 
     def test_creating_a_new_subkeyword_sets_included_in(self):
         with self.admin_access.cnx() as cnx:
-            kwgroup2_eid = cnx.create_entity('Keyword', name=u'kwgroup2', subkeyword_of=self.kwgroup_eid).eid
+            kwgroup2_eid = cnx.create_entity(
+                "Keyword", name="kwgroup2", subkeyword_of=self.kwgroup_eid
+            ).eid
             cnx.commit()
-            rset = cnx.execute('Any N WHERE C name N, K included_in C, K eid %(k)s', {'k': kwgroup2_eid})
+            rset = cnx.execute(
+                "Any N WHERE C name N, K included_in C, K eid %(k)s",
+                {"k": kwgroup2_eid},
+            )
             self.assertEqual(len(rset), 1)
-            self.assertEqual(rset[0][0], 'classif1')
+            self.assertEqual(rset[0][0], "classif1")
 
     def test_cannot_create_subkeyword_from_other_classification(self):
         with self.admin_access.cnx() as cnx:
-            cnx.execute('SET K1 subkeyword_of K2 WHERE K1 eid %(k1)s, K2 eid %(k2)s',
-                        {'k1': self.kwgroup_eid, 'k2': self.kwuser_eid})
+            cnx.execute(
+                "SET K1 subkeyword_of K2 WHERE K1 eid %(k1)s, K2 eid %(k2)s",
+                {"k1": self.kwgroup_eid, "k2": self.kwuser_eid},
+            )
             self.assertRaises(ValidationError, cnx.commit)
 
     def test_cannot_create_cycles(self):
         with self.admin_access.cnx() as cnx:
             # direct obvious cycle
-            cnx.execute('SET K1 subkeyword_of K2 WHERE K1 eid %(k1)s, K2 eid %(k2)s',
-                        {'k1': self.kwgroup_eid, 'k2': self.kwuser_eid})
+            cnx.execute(
+                "SET K1 subkeyword_of K2 WHERE K1 eid %(k1)s, K2 eid %(k2)s",
+                {"k1": self.kwgroup_eid, "k2": self.kwuser_eid},
+            )
             self.assertRaises(ValidationError, cnx.commit)
             # testing indirect cycles
-            kwgroup2_eid = cnx.create_entity('Keyword', name=u'kwgroup2',
-                                             included_in=self.classif1_eid,
-                                             subkeyword_of=self.kwgroup_eid).eid
-            cnx.execute('SET K subkeyword_of K2 WHERE K eid %(k)s, K2 eid %(k2)s',
-                        {'k': self.kwgroup_eid, 'k2': kwgroup2_eid})
+            kwgroup2_eid = cnx.create_entity(
+                "Keyword",
+                name="kwgroup2",
+                included_in=self.classif1_eid,
+                subkeyword_of=self.kwgroup_eid,
+            ).eid
+            cnx.execute(
+                "SET K subkeyword_of K2 WHERE K eid %(k)s, K2 eid %(k2)s",
+                {"k": self.kwgroup_eid, "k2": kwgroup2_eid},
+            )
             self.assertRaises(ValidationError, cnx.commit)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from logilab.common.testlib import unittest_main
+
     unittest_main()
```

### Comparing `cubicweb-keyword-3.0.0/test/test_descendant_of.py` & `cubicweb-keyword-4.0.0/test/test_descendant_of.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,205 +1,392 @@
-from __future__ import with_statement
 from cubicweb.devtools.testlib import CubicWebTC
 
 from cubicweb import ValidationError
 
 
 class KeywordHooksTC(CubicWebTC):
-
     def setup_database(self):
         with self.admin_access.cnx() as cnx:
             cwgroup = cnx.execute('Any U WHERE U is ET, U name "CWGroup"').one()
-            self.classif1_eid = cnx.create_entity('Classification', name=u"classif1", classifies=cwgroup).eid
+            self.classif1_eid = cnx.create_entity(
+                "Classification", name="classif1", classifies=cwgroup
+            ).eid
             cnx.commit()
 
     def test_keyword_add1(self):
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw1_eid = ce('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
-            kw2_eid = ce('Keyword', name=u'kw2', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            kw3_eid = ce('Keyword', name=u'kw3', subkeyword_of=kw2_eid, included_in=self.classif1_eid).eid
-            kw4_eid = ce('Keyword', name=u'kw4', subkeyword_of=kw3_eid, included_in=self.classif1_eid).eid
-            kw5_eid = ce('Keyword', name=u'kw5', subkeyword_of=kw4_eid, included_in=self.classif1_eid).eid
-            cnx.commit()
-            parent = cnx.find('Keyword', eid=kw1_eid).one()
-            child = cnx.find('Keyword', eid=kw5_eid).one()
-            self.assertCountEqual([kw.name for kw in child.cw_adapt_to('ITree').iterparents()],
-                                  ['kw4', 'kw3', 'kw2', 'kw1'])
-            self.assertCountEqual([kw.name for kw in child.descendant_of], ['kw4', 'kw3', 'kw2', 'kw1'])
-            self.assertCountEqual([kw.name for kw in parent.reverse_descendant_of], ['kw5', 'kw4', 'kw3', 'kw2'])
-            self.assertCountEqual([kw.name for kw in parent.cw_adapt_to('ITree').recurse_children()],
-                                  ['kw5', 'kw4', 'kw3', 'kw2'])
+            kw1_eid = ce("Keyword", name="kw1", included_in=self.classif1_eid).eid
+            kw2_eid = ce(
+                "Keyword",
+                name="kw2",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw3_eid = ce(
+                "Keyword",
+                name="kw3",
+                subkeyword_of=kw2_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw4_eid = ce(
+                "Keyword",
+                name="kw4",
+                subkeyword_of=kw3_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw5_eid = ce(
+                "Keyword",
+                name="kw5",
+                subkeyword_of=kw4_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            cnx.commit()
+            parent = cnx.find("Keyword", eid=kw1_eid).one()
+            child = cnx.find("Keyword", eid=kw5_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in child.cw_adapt_to("ITree").iterparents()],
+                ["kw4", "kw3", "kw2", "kw1"],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in child.descendant_of], ["kw4", "kw3", "kw2", "kw1"]
+            )
+            self.assertCountEqual(
+                [kw.name for kw in parent.reverse_descendant_of],
+                ["kw5", "kw4", "kw3", "kw2"],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in parent.cw_adapt_to("ITree").recurse_children()],
+                ["kw5", "kw4", "kw3", "kw2"],
+            )
 
     def test_keyword_add2(self):
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw1_eid = ce('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
-            kw2_eid = ce('Keyword', name=u'kw2', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            kw3_eid = ce('Keyword', name=u'kw3', included_in=self.classif1_eid).eid
-            kw4_eid = ce('Keyword', name=u'kw4', subkeyword_of=kw3_eid, included_in=self.classif1_eid).eid
-            kw5_eid = ce('Keyword', name=u'kw5',  subkeyword_of=kw4_eid, included_in=self.classif1_eid).eid
-            cnx.commit()
-            cnx.execute('SET K3 subkeyword_of K2 WHERE K3 eid %(kw3)s, K2 eid %(kw2)s',
-                        {'kw3': kw3_eid, 'kw2': kw2_eid})
-            cnx.commit()
-            parent = cnx.find('Keyword', eid=kw1_eid).one()
-            child = cnx.find('Keyword', eid=kw5_eid).one()
-            self.assertCountEqual([kw.name for kw in child.cw_adapt_to('ITree').iterparents()],
-                                  ['kw4', 'kw3', 'kw2', 'kw1'])
-            self.assertCountEqual([kw.name for kw in child.descendant_of], ['kw4', 'kw3', 'kw2', 'kw1'])
-            self.assertCountEqual([kw.name for kw in parent.reverse_descendant_of], ['kw5', 'kw4', 'kw3', 'kw2'])
-            self.assertCountEqual([kw.name for kw in parent.cw_adapt_to('ITree').recurse_children()],
-                                  ['kw5', 'kw4', 'kw3', 'kw2'])
+            kw1_eid = ce("Keyword", name="kw1", included_in=self.classif1_eid).eid
+            kw2_eid = ce(
+                "Keyword",
+                name="kw2",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw3_eid = ce("Keyword", name="kw3", included_in=self.classif1_eid).eid
+            kw4_eid = ce(
+                "Keyword",
+                name="kw4",
+                subkeyword_of=kw3_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw5_eid = ce(
+                "Keyword",
+                name="kw5",
+                subkeyword_of=kw4_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            cnx.commit()
+            cnx.execute(
+                "SET K3 subkeyword_of K2 WHERE K3 eid %(kw3)s, K2 eid %(kw2)s",
+                {"kw3": kw3_eid, "kw2": kw2_eid},
+            )
+            cnx.commit()
+            parent = cnx.find("Keyword", eid=kw1_eid).one()
+            child = cnx.find("Keyword", eid=kw5_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in child.cw_adapt_to("ITree").iterparents()],
+                ["kw4", "kw3", "kw2", "kw1"],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in child.descendant_of], ["kw4", "kw3", "kw2", "kw1"]
+            )
+            self.assertCountEqual(
+                [kw.name for kw in parent.reverse_descendant_of],
+                ["kw5", "kw4", "kw3", "kw2"],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in parent.cw_adapt_to("ITree").recurse_children()],
+                ["kw5", "kw4", "kw3", "kw2"],
+            )
 
     def test_keyword_add3(self):
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw1_eid = ce('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
-            kw2_eid = ce('Keyword', name=u'kw2', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            kw3_eid = ce('Keyword', name=u'kw3', included_in=self.classif1_eid).eid
-            kw4_eid = ce('Keyword', name=u'kw4', included_in=self.classif1_eid).eid
-            kw5_eid = ce('Keyword', name=u'kw5', subkeyword_of=kw4_eid, included_in=self.classif1_eid).eid
-            cnx.commit()
-            cnx.execute('SET K2 subkeyword_of K3 WHERE K2 eid %(k2)s, K3 eid %(k3)s',
-                        {'k2': kw4_eid, 'k3': kw3_eid})
-            cnx.execute('SET K3 subkeyword_of K4 WHERE K3 eid %(k3)s, K4 eid %(k4)s',
-                        {'k3': kw3_eid, 'k4': kw2_eid})
-            cnx.commit()
-            child = cnx.find('Keyword', eid=kw5_eid).one()
-            parent = cnx.find('Keyword', eid=kw1_eid).one()
-            self.assertCountEqual([kw.name for kw in child.descendant_of], ['kw4', 'kw3', 'kw2', 'kw1'])
+            kw1_eid = ce("Keyword", name="kw1", included_in=self.classif1_eid).eid
+            kw2_eid = ce(
+                "Keyword",
+                name="kw2",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw3_eid = ce("Keyword", name="kw3", included_in=self.classif1_eid).eid
+            kw4_eid = ce("Keyword", name="kw4", included_in=self.classif1_eid).eid
+            kw5_eid = ce(
+                "Keyword",
+                name="kw5",
+                subkeyword_of=kw4_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            cnx.commit()
+            cnx.execute(
+                "SET K2 subkeyword_of K3 WHERE K2 eid %(k2)s, K3 eid %(k3)s",
+                {"k2": kw4_eid, "k3": kw3_eid},
+            )
+            cnx.execute(
+                "SET K3 subkeyword_of K4 WHERE K3 eid %(k3)s, K4 eid %(k4)s",
+                {"k3": kw3_eid, "k4": kw2_eid},
+            )
+            cnx.commit()
+            child = cnx.find("Keyword", eid=kw5_eid).one()
+            parent = cnx.find("Keyword", eid=kw1_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in child.descendant_of], ["kw4", "kw3", "kw2", "kw1"]
+            )
             # XXX check the order of iterparents
-            self.assertCountEqual([kw.name for kw in child.cw_adapt_to('ITree').iterparents()],
-                                  ['kw4', 'kw3', 'kw2', 'kw1'])
-            self.assertCountEqual([kw.name for kw in parent.cw_adapt_to('ITree').recurse_children()],
-                                  ['kw2', 'kw3', 'kw4', 'kw5'])
-            self.assertCountEqual([kw.name for kw in parent.reverse_descendant_of], ['kw2', 'kw3', 'kw4', 'kw5'])
+            self.assertCountEqual(
+                [kw.name for kw in child.cw_adapt_to("ITree").iterparents()],
+                ["kw4", "kw3", "kw2", "kw1"],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in parent.cw_adapt_to("ITree").recurse_children()],
+                ["kw2", "kw3", "kw4", "kw5"],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in parent.reverse_descendant_of],
+                ["kw2", "kw3", "kw4", "kw5"],
+            )
 
     def test_keyword_add4(self):
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw0_eid = ce('Keyword', name=u'kw0', included_in=self.classif1_eid).eid
-            kw1_eid = ce('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
-            kw2_eid = ce('Keyword', name=u'kw2', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            kw3_eid = ce('Keyword', name=u'kw3', included_in=self.classif1_eid).eid
-            kw4_eid = ce('Keyword', name=u'kw4', included_in=self.classif1_eid).eid
-            kw5_eid = ce('Keyword', name=u'kw5',  subkeyword_of=kw4_eid, included_in=self.classif1_eid).eid
-            cnx.execute('SET K3 subkeyword_of K2 WHERE K3 eid %(kw3)s, K2 eid %(kw2)s',
-                        {'kw2': kw2_eid, 'kw3': kw3_eid})
-            cnx.commit()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw1', 'kw2'])
-            cnx.execute('SET K3 descendant_of K0 WHERE K3 eid %(kw3)s, K0 eid %(kw0)s',
-                        {'kw3': kw3_eid, 'kw0': kw0_eid})
-            cnx.commit()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw0', 'kw1', 'kw2'])
-            cnx.execute('SET K3 descendant_of K4 WHERE K3 eid %(kw3)s, K4 eid %(kw4)s',
-                        {'kw3': kw3_eid, 'kw4': kw4_eid})
-            cnx.commit()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw0', 'kw1', 'kw2', 'kw4'])
-            cnx.execute('SET K3 descendant_of K5 WHERE K3 eid %(kw3)s, K5 eid %(kw5)s',
-                        {'kw3': kw3_eid, 'kw5': kw5_eid})
+            kw0_eid = ce("Keyword", name="kw0", included_in=self.classif1_eid).eid
+            kw1_eid = ce("Keyword", name="kw1", included_in=self.classif1_eid).eid
+            kw2_eid = ce(
+                "Keyword",
+                name="kw2",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw3_eid = ce("Keyword", name="kw3", included_in=self.classif1_eid).eid
+            kw4_eid = ce("Keyword", name="kw4", included_in=self.classif1_eid).eid
+            kw5_eid = ce(
+                "Keyword",
+                name="kw5",
+                subkeyword_of=kw4_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            cnx.execute(
+                "SET K3 subkeyword_of K2 WHERE K3 eid %(kw3)s, K2 eid %(kw2)s",
+                {"kw2": kw2_eid, "kw3": kw3_eid},
+            )
+            cnx.commit()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ["kw1", "kw2"])
+            cnx.execute(
+                "SET K3 descendant_of K0 WHERE K3 eid %(kw3)s, K0 eid %(kw0)s",
+                {"kw3": kw3_eid, "kw0": kw0_eid},
+            )
+            cnx.commit()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in kw3.descendant_of], ["kw0", "kw1", "kw2"]
+            )
+            cnx.execute(
+                "SET K3 descendant_of K4 WHERE K3 eid %(kw3)s, K4 eid %(kw4)s",
+                {"kw3": kw3_eid, "kw4": kw4_eid},
+            )
+            cnx.commit()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in kw3.descendant_of], ["kw0", "kw1", "kw2", "kw4"]
+            )
+            cnx.execute(
+                "SET K3 descendant_of K5 WHERE K3 eid %(kw3)s, K5 eid %(kw5)s",
+                {"kw3": kw3_eid, "kw5": kw5_eid},
+            )
             cnx.commit()
             kw3.cw_clear_all_caches()
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw0', 'kw1', 'kw2', 'kw4', 'kw5'])
+            self.assertCountEqual(
+                [kw.name for kw in kw3.descendant_of],
+                ["kw0", "kw1", "kw2", "kw4", "kw5"],
+            )
 
     def test_keyword_update1(self):
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw1_eid = ce('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
-            kw2_eid = ce('Keyword', name=u'kw2', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            kw3_eid = ce('Keyword', name=u'kw3', included_in=self.classif1_eid).eid
-            kw4_eid = ce('Keyword', name=u'kw4', included_in=self.classif1_eid).eid
-            kw5_eid = ce('Keyword', name=u'kw5',  subkeyword_of=kw4_eid, included_in=self.classif1_eid).eid
-            cnx.execute('SET K3 subkeyword_of K2 WHERE K3 eid %(kw3)s, K2 eid %(kw2)s',
-                        {'kw3': kw3_eid, 'kw2': kw2_eid})
-            cnx.commit()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw1', 'kw2'])
-            cnx.execute('SET K3 subkeyword_of K4 WHERE K3 eid %(kw3)s, K4 eid %(kw4)s',
-                        {'kw3': kw3_eid, 'kw4': kw4_eid})
-            cnx.commit()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw4'])
-            cnx.execute('SET K3 subkeyword_of K5 WHERE K3 eid %(kw3)s, K5 eid %(kw5)s',
-                        {'kw3': kw3_eid, 'kw5': kw5_eid})
+            kw1_eid = ce("Keyword", name="kw1", included_in=self.classif1_eid).eid
+            kw2_eid = ce(
+                "Keyword",
+                name="kw2",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw3_eid = ce("Keyword", name="kw3", included_in=self.classif1_eid).eid
+            kw4_eid = ce("Keyword", name="kw4", included_in=self.classif1_eid).eid
+            kw5_eid = ce(
+                "Keyword",
+                name="kw5",
+                subkeyword_of=kw4_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            cnx.execute(
+                "SET K3 subkeyword_of K2 WHERE K3 eid %(kw3)s, K2 eid %(kw2)s",
+                {"kw3": kw3_eid, "kw2": kw2_eid},
+            )
+            cnx.commit()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ["kw1", "kw2"])
+            cnx.execute(
+                "SET K3 subkeyword_of K4 WHERE K3 eid %(kw3)s, K4 eid %(kw4)s",
+                {"kw3": kw3_eid, "kw4": kw4_eid},
+            )
+            cnx.commit()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ["kw4"])
+            cnx.execute(
+                "SET K3 subkeyword_of K5 WHERE K3 eid %(kw3)s, K5 eid %(kw5)s",
+                {"kw3": kw3_eid, "kw5": kw5_eid},
+            )
             cnx.commit()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw4', 'kw5'])
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ["kw4", "kw5"])
 
     def test_keyword_descendant_of(self):
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw1_eid = ce('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
-            kw2_eid = ce('Keyword', name=u'kw2', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            kw3_eid = ce('Keyword', name=u'kw3', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            cnx.commit()
-
-            kw1 = cnx.find('Keyword', eid=kw1_eid).one()
-            kw2 = cnx.find('Keyword', eid=kw2_eid).one()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw2.descendant_of], ['kw1', ])
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw1', ])
-            self.assertCountEqual([kw.name for kw in kw1.reverse_descendant_of], ['kw3', 'kw2'])
-            self.assertCountEqual([kw.name for kw in kw1.cw_adapt_to('ITree').recurse_children()], ['kw2', 'kw3'])
-            kw0_eid = ce('Keyword', name=u'kw0', included_in=self.classif1_eid).eid
-
-            cnx.execute('SET K1 subkeyword_of K0 WHERE K1 eid %(kw1)s, K0 eid %(kw0)s',
-                        {'kw1': kw1_eid, 'kw0': kw0_eid})
-            cnx.commit()
-
-            kw0 = cnx.find('Keyword', eid=kw0_eid).one()
-            kw1 = cnx.find('Keyword', eid=kw1_eid).one()
-            kw2 = cnx.find('Keyword', eid=kw2_eid).one()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw0.cw_adapt_to('ITree').recurse_children()],
-                                  ['kw1', 'kw2', 'kw3'])
-            self.assertCountEqual([kw.name for kw in kw0.reverse_descendant_of], ['kw3', 'kw2', 'kw1'])
-            self.assertCountEqual([kw.name for kw in kw1.descendant_of], ['kw0'])
-            self.assertCountEqual([kw.name for kw in kw2.descendant_of], ['kw1', 'kw0'])
-            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ['kw1', 'kw0'])
+            kw1_eid = ce("Keyword", name="kw1", included_in=self.classif1_eid).eid
+            kw2_eid = ce(
+                "Keyword",
+                name="kw2",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw3_eid = ce(
+                "Keyword",
+                name="kw3",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            cnx.commit()
+
+            kw1 = cnx.find("Keyword", eid=kw1_eid).one()
+            kw2 = cnx.find("Keyword", eid=kw2_eid).one()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in kw2.descendant_of],
+                [
+                    "kw1",
+                ],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in kw3.descendant_of],
+                [
+                    "kw1",
+                ],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in kw1.reverse_descendant_of], ["kw3", "kw2"]
+            )
+            self.assertCountEqual(
+                [kw.name for kw in kw1.cw_adapt_to("ITree").recurse_children()],
+                ["kw2", "kw3"],
+            )
+            kw0_eid = ce("Keyword", name="kw0", included_in=self.classif1_eid).eid
+
+            cnx.execute(
+                "SET K1 subkeyword_of K0 WHERE K1 eid %(kw1)s, K0 eid %(kw0)s",
+                {"kw1": kw1_eid, "kw0": kw0_eid},
+            )
+            cnx.commit()
+
+            kw0 = cnx.find("Keyword", eid=kw0_eid).one()
+            kw1 = cnx.find("Keyword", eid=kw1_eid).one()
+            kw2 = cnx.find("Keyword", eid=kw2_eid).one()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in kw0.cw_adapt_to("ITree").recurse_children()],
+                ["kw1", "kw2", "kw3"],
+            )
+            self.assertCountEqual(
+                [kw.name for kw in kw0.reverse_descendant_of], ["kw3", "kw2", "kw1"]
+            )
+            self.assertCountEqual([kw.name for kw in kw1.descendant_of], ["kw0"])
+            self.assertCountEqual([kw.name for kw in kw2.descendant_of], ["kw1", "kw0"])
+            self.assertCountEqual([kw.name for kw in kw3.descendant_of], ["kw1", "kw0"])
 
     def test_keyword_delete(self):
-        """*after_delete_relation* of ``subkeyword_of``
-        """
+        """*after_delete_relation* of ``subkeyword_of``"""
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw1_eid = ce('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
-            kw2_eid = ce('Keyword', name=u'kw2', subkeyword_of=kw1_eid, included_in=self.classif1_eid).eid
-            kw3_eid = ce('Keyword', name=u'kw3', subkeyword_of=kw2_eid, included_in=self.classif1_eid).eid
-            kw4_eid = ce('Keyword', name=u'kw4', subkeyword_of=kw3_eid, included_in=self.classif1_eid).eid
-            ce('Keyword', name=u'kw5',  subkeyword_of=kw4_eid, included_in=self.classif1_eid).eid
-            cnx.commit()
-            cnx.execute('DELETE K subkeyword_of K3 WHERE K is Keyword, K eid %(kw3)s',
-                        {'kw3': kw3_eid})
-            cnx.commit()
-            kw3 = cnx.find('Keyword', eid=kw3_eid).one()
-            self.assertCountEqual([kw.name for kw in kw3.cw_adapt_to('ITree').iterparents()], [])
+            kw1_eid = ce("Keyword", name="kw1", included_in=self.classif1_eid).eid
+            kw2_eid = ce(
+                "Keyword",
+                name="kw2",
+                subkeyword_of=kw1_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw3_eid = ce(
+                "Keyword",
+                name="kw3",
+                subkeyword_of=kw2_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            kw4_eid = ce(
+                "Keyword",
+                name="kw4",
+                subkeyword_of=kw3_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            ce(
+                "Keyword",
+                name="kw5",
+                subkeyword_of=kw4_eid,
+                included_in=self.classif1_eid,
+            ).eid
+            cnx.commit()
+            cnx.execute(
+                "DELETE K subkeyword_of K3 WHERE K is Keyword, K eid %(kw3)s",
+                {"kw3": kw3_eid},
+            )
+            cnx.commit()
+            kw3 = cnx.find("Keyword", eid=kw3_eid).one()
+            self.assertCountEqual(
+                [kw.name for kw in kw3.cw_adapt_to("ITree").iterparents()], []
+            )
             self.assertCountEqual([kw.name for kw in kw3.descendant_of], [])
-            self.assertCountEqual([kw.name for kw in kw3.reverse_descendant_of], ['kw5', 'kw4'])
-            self.assertCountEqual([kw.name for kw in kw3.cw_adapt_to('ITree').recurse_children()], ['kw5', 'kw4'])
+            self.assertCountEqual(
+                [kw.name for kw in kw3.reverse_descendant_of], ["kw5", "kw4"]
+            )
+            self.assertCountEqual(
+                [kw.name for kw in kw3.cw_adapt_to("ITree").recurse_children()],
+                ["kw5", "kw4"],
+            )
 
     def test_no_add_descendant_cycle(self):
         """no ``descendant_of`` cycle"""
         with self.admin_access.cnx() as cnx:
             ce = cnx.create_entity
-            kw1 = ce('Keyword', name=u'kw1', included_in=self.classif1_eid)
-            kw2 = ce('Keyword', name=u'kw2', subkeyword_of=kw1, included_in=self.classif1_eid)
-            kw3 = ce('Keyword', name=u'kw3', subkeyword_of=kw2, included_in=self.classif1_eid)
+            kw1 = ce("Keyword", name="kw1", included_in=self.classif1_eid)
+            kw2 = ce(
+                "Keyword", name="kw2", subkeyword_of=kw1, included_in=self.classif1_eid
+            )
+            kw3 = ce(
+                "Keyword", name="kw3", subkeyword_of=kw2, included_in=self.classif1_eid
+            )
             cnx.commit()
-            rql = 'SET K1 descendant_of K3 WHERE K1 eid %(kw1)s, K3 eid %(kw3)s' % {'kw1': kw1.eid,  'kw3': kw3.eid}
+            rql = f"SET K1 descendant_of K3 WHERE K1 eid {kw1.eid}, K3 eid {kw3.eid}"
             self.assertRaises(ValidationError, cnx.execute, rql)
             cnx.rollback()
-            kw4 = ce('Keyword', name=u'kw4', included_in=self.classif1_eid)
-            kw5 = ce('Keyword', name=u'kw4', subkeyword_of=kw4, included_in=self.classif1_eid)
+            kw4 = ce("Keyword", name="kw4", included_in=self.classif1_eid)
+            kw5 = ce(
+                "Keyword", name="kw4", subkeyword_of=kw4, included_in=self.classif1_eid
+            )
             cnx.commit()
             with self.assertRaises(ValidationError):
-                cnx.execute('SET K4 descendant_of K5 WHERE K4 eid %(kw4)s, K5 eid %(kw5)s',
-                            {'kw4': kw4.eid,  'kw5': kw5.eid})
+                cnx.execute(
+                    "SET K4 descendant_of K5 WHERE K4 eid %(kw4)s, K5 eid %(kw5)s",
+                    {"kw4": kw4.eid, "kw5": kw5.eid},
+                )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from logilab.common.testlib import unittest_main
+
     unittest_main()
```

### Comparing `cubicweb-keyword-3.0.0/test/test_security.py` & `cubicweb-keyword-4.0.0/test/test_security.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from cubicweb.devtools.testlib import CubicWebTC
 
 
 class SecurityTC(CubicWebTC):
     def setup_database(self):
         with self.admin_access.cnx() as cnx:
             cwgroup = cnx.execute('Any U WHERE U is ET, U name "CWGroup"').one()
-            self.classif1_eid = cnx.create_entity('Classification', name=u"classif1", classifies=cwgroup).eid
-            self.kw1_eid = cnx.create_entity('Keyword', name=u'kw1', included_in=self.classif1_eid).eid
+            self.classif1_eid = cnx.create_entity(
+                "Classification", name="classif1", classifies=cwgroup
+            ).eid
+            self.kw1_eid = cnx.create_entity(
+                "Keyword", name="kw1", included_in=self.classif1_eid
+            ).eid
             cnx.commit()
 
     def test_nonregr_keyword_selection_as_guest(self):
         with self.new_access("anon").cnx() as cnx:
-            cnx.execute('Any X ORDERBY Z WHERE X modification_date Z, K eid %(k)s, K applied_to X', {'k': self.kw1_eid})
+            cnx.execute(
+                "Any X ORDERBY Z WHERE X modification_date Z, K eid %(k)s, K applied_to X",
+                {"k": self.kw1_eid},
+            )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from logilab.common.testlib import unittest_main
+
     unittest_main()
```

### Comparing `cubicweb-keyword-3.0.0/tox.ini` & `cubicweb-keyword-4.0.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
-envlist = py3,flake8,safety,yamllint
+envlist = py3,flake8,safety,yamllint,black
 
 [testenv]
 deps =
   pytest
+  webtest
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs}
 
 [pytest]
 python_files = *test_*.py
 testpaths = test
@@ -36,15 +37,15 @@
 deps = safety
 commands =
   {envpython} -msafety check --full-report
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -54,7 +55,21 @@
 
 [testenv:yamllint]
 skip_install = true
 deps = yamllint
 commands =
   yamllint .
 
+
+[testenv:black]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black --check .
+
+[testenv:black-run]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black .
```

