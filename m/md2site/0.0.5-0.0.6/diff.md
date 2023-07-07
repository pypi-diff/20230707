# Comparing `tmp/md2site-0.0.5.tar.gz` & `tmp/md2site-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2site-0.0.5.tar", max compression
+gzip compressed data, was "md2site-0.0.6.tar", max compression
```

## Comparing `md2site-0.0.5.tar` & `md2site-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.5/LICENSE.md
--rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.5/md2site/__init__.py
--rw-r--r--   0        0        0     4048 2023-07-04 11:00:46.653809 md2site-0.0.5/md2site/generator.py
--rw-r--r--   0        0        0     2464 2023-07-04 10:39:56.386981 md2site-0.0.5/md2site/post.py
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.5/md2site/py.typed
--rw-r--r--   0        0        0     2169 2023-07-01 05:43:16.526132 md2site-0.0.5/md2site/renderer.py
--rw-r--r--   0        0        0      419 2023-07-01 10:42:34.126426 md2site-0.0.5/md2site/site.py
--rw-r--r--   0        0        0     1015 2023-07-04 11:01:05.027423 md2site-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.6/md2site/__init__.py
+-rw-r--r--   0        0        0     4048 2023-07-04 11:00:46.653809 md2site-0.0.6/md2site/generator.py
+-rw-r--r--   0        0        0     2464 2023-07-04 10:39:56.386981 md2site-0.0.6/md2site/post.py
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.6/md2site/py.typed
+-rw-r--r--   0        0        0     3002 2023-07-07 10:48:01.140471 md2site-0.0.6/md2site/renderer.py
+-rw-r--r--   0        0        0      419 2023-07-01 10:42:34.126426 md2site-0.0.6/md2site/site.py
+-rw-r--r--   0        0        0     1015 2023-07-07 10:49:55.950570 md2site-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.6/PKG-INFO
```

### Comparing `md2site-0.0.5/LICENSE.md` & `md2site-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `md2site-0.0.5/md2site/generator.py` & `md2site-0.0.6/md2site/generator.py`

 * *Files identical despite different names*

### Comparing `md2site-0.0.5/md2site/post.py` & `md2site-0.0.6/md2site/post.py`

 * *Files identical despite different names*

### Comparing `md2site-0.0.5/md2site/renderer.py` & `md2site-0.0.6/md2site/renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,53 @@
         self.target = splits[0].strip()
         if len(splits) == 1:
             self.children = (RawText(self.target),)
         else:
             self.children = (RawText(splits[1].strip()),)
 
 
+class AutoUrlLink(SpanToken):
+    """
+    AutoURLLink token. ("http://www.example.com")
+
+    This is an inline token with a single child of type RawText.
+
+    Attributes:
+        children (list): a single RawText node for the link target.
+        target (str): link target.
+    """
+
+    repr_attributes = "target"
+    pattern = re.compile(
+        r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)"
+    )
+    parse_inner = False
+
+    def __init__(self, match: re.Match):
+        content = match.group(0)
+        self.children = (RawText(content),)
+        self.target = content
+
+
 class Renderer(HTMLRenderer):
     def __init__(self, config: Site):
-        super().__init__(WikiLink)
+        super().__init__(WikiLink, AutoUrlLink)
         self.site = config
 
     def render_wiki_link(self, token: WikiLink):
         template = '<a href="{base_url}/{target}.html">{inner}</a>'
         target = self.site.link_map.get(token.target, "#")
         inner = self.render_inner(token)
         return template.format(base_url=self.site.base_url, target=target, inner=inner)
 
+    def render_auto_url_link(self, token: AutoUrlLink):
+        template = '<a href="{target}">{target}</a>'
+        target = token.target
+        return template.format(target=target)
+
 
 class Parser:
     def __init__(self):
         span_token.add_token(WikiLink)
 
     def __enter__(self):
         return self
```

### Comparing `md2site-0.0.5/pyproject.toml` & `md2site-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md2site"
-version = "0.0.5"
+version = "0.0.6"
 description = "A static site generator with bare-minimum functionality."
 license = "GPL-3.0-or-later"
 authors = ["Yoonseop Kang <e0engoon@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/e0en/md2site"
 repository = "https://github.com/e0en/md2site"
 classifiers = [
```

### Comparing `md2site-0.0.5/PKG-INFO` & `md2site-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2site
-Version: 0.0.5
+Version: 0.0.6
 Summary: A static site generator with bare-minimum functionality.
 Home-page: https://github.com/e0en/md2site
 License: GPL-3.0-or-later
 Author: Yoonseop Kang
 Author-email: e0engoon@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 1 - Planning
```

