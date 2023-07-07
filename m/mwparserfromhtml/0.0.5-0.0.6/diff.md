# Comparing `tmp/mwparserfromhtml-0.0.5.tar.gz` & `tmp/mwparserfromhtml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwparserfromhtml-0.0.5.tar", last modified: Tue Sep 27 16:49:56 2022, max compression
+gzip compressed data, was "mwparserfromhtml-0.0.6.tar", last modified: Fri Jul  7 14:47:07 2023, max compression
```

## Comparing `mwparserfromhtml-0.0.5.tar` & `mwparserfromhtml-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxr-x   0 appledora  (1000) appledora  (1000)        0 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     1073 2022-08-18 11:16:14.000000 mwparserfromhtml-0.0.5/LICENSE
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     6660 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/PKG-INFO
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     5679 2022-09-27 16:31:41.000000 mwparserfromhtml-0.0.5/README.md
--rw-rw-r--   0 appledora  (1000) appledora  (1000)       38 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/setup.cfg
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     1839 2022-09-24 20:00:00.000000 mwparserfromhtml-0.0.5/setup.py
-drwxrwxr-x   0 appledora  (1000) appledora  (1000)        0 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/src/
-drwxrwxr-x   0 appledora  (1000) appledora  (1000)        0 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/src/mwparserfromhtml/
--rw-rw-r--   0 appledora  (1000) appledora  (1000)      375 2022-09-24 19:59:43.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/__init__.py
-drwxrwxr-x   0 appledora  (1000) appledora  (1000)        0 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/src/mwparserfromhtml/dump/
--rw-rw-r--   0 appledora  (1000) appledora  (1000)        0 2022-08-07 18:15:03.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/dump/__init__.py
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     2183 2022-09-24 17:45:57.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/dump/dump.py
-drwxrwxr-x   0 appledora  (1000) appledora  (1000)        0 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/
--rw-rw-r--   0 appledora  (1000) appledora  (1000)        0 2022-08-07 18:15:03.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/__init__.py
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     9296 2022-09-24 18:44:57.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/article.py
--rw-rw-r--   0 appledora  (1000) appledora  (1000)   272741 2022-08-23 14:31:40.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/const.py
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     5973 2022-09-24 18:35:08.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/elements.py
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     8039 2022-09-23 13:43:47.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/utils.py
-drwxrwxr-x   0 appledora  (1000) appledora  (1000)        0 2022-09-27 16:49:56.701097 mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/
--rw-rw-r--   0 appledora  (1000) appledora  (1000)     6660 2022-09-27 16:49:56.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/PKG-INFO
--rw-rw-r--   0 appledora  (1000) appledora  (1000)      581 2022-09-27 16:49:56.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/SOURCES.txt
--rw-rw-r--   0 appledora  (1000) appledora  (1000)        1 2022-09-27 16:49:56.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/dependency_links.txt
--rw-rw-r--   0 appledora  (1000) appledora  (1000)        1 2022-08-24 20:24:34.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/not-zip-safe
--rw-rw-r--   0 appledora  (1000) appledora  (1000)      138 2022-09-27 16:49:56.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/requires.txt
--rw-rw-r--   0 appledora  (1000) appledora  (1000)       17 2022-09-27 16:49:56.000000 mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:47:07.134956 mwparserfromhtml-0.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6660 2023-07-07 14:47:07.134956 mwparserfromhtml-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5679 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 14:47:07.134956 mwparserfromhtml-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:47:07.130956 mwparserfromhtml-0.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:47:07.130956 mwparserfromhtml-0.0.6/src/mwparserfromhtml/
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:47:07.134956 mwparserfromhtml-0.0.6/src/mwparserfromhtml/dump/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/dump/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/dump/dump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:47:07.134956 mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9295 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/article.py
+-rw-rw-rw-   0 root         (0) root         (0)   272741 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     5973 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/elements.py
+-rw-rw-rw-   0 root         (0) root         (0)     8031 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:47:07.134956 mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6660 2023-07-07 14:47:07.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-07-07 14:47:07.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:47:07.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:47:06.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-07 14:47:07.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-07 14:47:07.000000 mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:47:07.134956 mwparserfromhtml-0.0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/tests/test_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     7532 2023-07-07 14:46:49.000000 mwparserfromhtml-0.0.6/tests/test_parse.py
```

### Comparing `mwparserfromhtml-0.0.5/LICENSE` & `mwparserfromhtml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mwparserfromhtml-0.0.5/PKG-INFO` & `mwparserfromhtml-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwparserfromhtml
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wikipedia HTML Dump Parsing
 Home-page: https://gitlab.wikimedia.org/repos/research/html-dumps
 Author: Appledora & Isaac Johnson & Martin Gerlach
 Author-email: <isaac@wikimedia.org>
 License: MIT License
 Keywords: python,wikipedia,html
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mwparserfromhtml-0.0.5/README.md` & `mwparserfromhtml-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mwparserfromhtml-0.0.5/setup.py` & `mwparserfromhtml-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "Wikipedia HTML Dump Parsing"
 LONG_DESCRIPTION = (
     "A package that supports plaintext and object extraction from Wikipedia HTML dumps."
 )
 
 # Dev dependencies
 EXTRAS_REQUIRE = {
```

### Comparing `mwparserfromhtml-0.0.5/src/mwparserfromhtml/dump/dump.py` & `mwparserfromhtml-0.0.6/src/mwparserfromhtml/dump/dump.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,8 +64,12 @@
                 with tar_file_.extractfile(html_fn) as file_input:
                     for line in file_input:
                         if count == max_article:
                             tar_file_.close()
                             return
                         article = json.loads(line)
                         count += 1
-                        yield Article(article)
+                        try:
+                            yield Article(article)
+                        except Exception:
+                            print(f"Article parsing failed for: {article}")
+                            continue
```

### Comparing `mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/article.py` & `mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/article.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
             tag, attrs={"class": "mw-reference-text"}
         )
         return [Reference(r) for r in references]
 
     def get_media(
         self, skip_images=False, skip_audio=False, skip_video=False
     ) -> typing.List[Media]:
-
         """
         extract image, video and audio information from a Beautifulsoup object.
         Media not appearing inside `img`, `video` or `audio` html  tag won't be
         captured by this method.
         Args:
             skip_images: boolean. If true doesn't include Image data.
             skip_audio: boolean. If true, doesn't include audio data.
```

### Comparing `mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/const.py` & `mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/const.py`

 * *Files identical despite different names*

### Comparing `mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/elements.py` & `mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/elements.py`

 * *Files identical despite different names*

### Comparing `mwparserfromhtml-0.0.5/src/mwparserfromhtml/parse/utils.py` & `mwparserfromhtml-0.0.6/src/mwparserfromhtml/parse/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,13 +241,13 @@
             yield cnode.text
 
 
 def get_metadata(body):
     # the NON_KEYS array contains the keys which has already been defined
     # within the article class by extracting directly from the HTML.
     # That's why we don't redundantly include them in the metadata.
-    NON_KEYS = ["article_body", "url", "namespace", "name", "in_language"]
+    NON_KEYS = ["article_body", "url", "namespace", "in_language"]
     metadata = {}
     for k in body.keys():
         if k not in NON_KEYS:
             metadata[k] = body.get(k)
     return metadata
```

### Comparing `mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/PKG-INFO` & `mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwparserfromhtml
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wikipedia HTML Dump Parsing
 Home-page: https://gitlab.wikimedia.org/repos/research/html-dumps
 Author: Appledora & Isaac Johnson & Martin Gerlach
 Author-email: <isaac@wikimedia.org>
 License: MIT License
 Keywords: python,wikipedia,html
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mwparserfromhtml-0.0.5/src/mwparserfromhtml.egg-info/SOURCES.txt` & `mwparserfromhtml-0.0.6/src/mwparserfromhtml.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 src/mwparserfromhtml.egg-info/top_level.txt
 src/mwparserfromhtml/dump/__init__.py
 src/mwparserfromhtml/dump/dump.py
 src/mwparserfromhtml/parse/__init__.py
 src/mwparserfromhtml/parse/article.py
 src/mwparserfromhtml/parse/const.py
 src/mwparserfromhtml/parse/elements.py
-src/mwparserfromhtml/parse/utils.py
+src/mwparserfromhtml/parse/utils.py
+tests/test_dump.py
+tests/test_parse.py
```

