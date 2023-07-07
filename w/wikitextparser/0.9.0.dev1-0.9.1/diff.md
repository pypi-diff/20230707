# Comparing `tmp/wikitextparser-0.9.0.dev1.tar.gz` & `tmp/wikitextparser-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wikitextparser-0.9.0.dev1.tar", last modified: Wed Oct 26 14:52:39 2016, max compression
+gzip compressed data, was "dist\wikitextparser-0.9.1.tar", last modified: Wed Nov  2 13:13:38 2016, max compression
```

## Comparing `wikitextparser-0.9.0.dev1.tar` & `wikitextparser-0.9.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/
--rw-rw-rw-   0        0        0    35795 2015-03-24 09:52:20.000000 wikitextparser-0.9.0.dev1/LICENSE.md
--rw-rw-rw-   0        0        0       14 2016-10-24 02:10:33.000000 wikitextparser-0.9.0.dev1/MANIFEST.in
--rw-rw-rw-   0        0        0     8538 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     6268 2016-10-25 02:22:59.000000 wikitextparser-0.9.0.dev1/README.rst
--rw-rw-rw-   0        0        0       64 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0     1161 2016-10-26 14:50:31.000000 wikitextparser-0.9.0.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/wikitextparser/
--rw-rw-rw-   0        0        0     4778 2016-10-25 05:44:46.000000 wikitextparser-0.9.0.dev1/wikitextparser/argument.py
--rw-rw-rw-   0        0        0     3050 2016-10-25 00:10:38.000000 wikitextparser-0.9.0.dev1/wikitextparser/argument_test.py
--rw-rw-rw-   0        0        0      950 2016-10-13 01:13:10.000000 wikitextparser-0.9.0.dev1/wikitextparser/comment.py
--rw-rw-rw-   0        0        0      342 2016-10-17 08:07:18.000000 wikitextparser-0.9.0.dev1/wikitextparser/comment_test.py
--rw-rw-rw-   0        0        0     2485 2016-10-26 13:24:44.000000 wikitextparser-0.9.0.dev1/wikitextparser/externallink.py
--rw-rw-rw-   0        0        0     2166 2016-10-17 08:09:25.000000 wikitextparser-0.9.0.dev1/wikitextparser/externallink_test.py
--rw-rw-rw-   0        0        0    18058 2016-10-24 12:26:18.000000 wikitextparser-0.9.0.dev1/wikitextparser/list_parser.py
--rw-rw-rw-   0        0        0     1695 2016-07-20 09:21:21.000000 wikitextparser-0.9.0.dev1/wikitextparser/list_parser_test_ignore.py
--rw-rw-rw-   0        0        0     3533 2016-10-26 13:27:12.000000 wikitextparser-0.9.0.dev1/wikitextparser/parameter.py
--rw-rw-rw-   0        0        0     2945 2016-10-17 08:12:29.000000 wikitextparser-0.9.0.dev1/wikitextparser/parameter_test.py
--rw-rw-rw-   0        0        0     2546 2016-10-25 04:35:30.000000 wikitextparser-0.9.0.dev1/wikitextparser/parser_function.py
--rw-rw-rw-   0        0        0     1826 2016-10-17 08:15:59.000000 wikitextparser-0.9.0.dev1/wikitextparser/parser_function_test.py
--rw-rw-rw-   0        0        0     2932 2016-10-25 04:37:22.000000 wikitextparser-0.9.0.dev1/wikitextparser/section.py
--rw-rw-rw-   0        0        0     2065 2016-09-16 03:07:22.000000 wikitextparser-0.9.0.dev1/wikitextparser/section_test.py
--rw-rw-rw-   0        0        0    13158 2016-10-25 02:21:26.000000 wikitextparser-0.9.0.dev1/wikitextparser/spans.py
--rw-rw-rw-   0        0        0    13257 2016-10-11 17:04:38.000000 wikitextparser-0.9.0.dev1/wikitextparser/spans_test.py
--rw-rw-rw-   0        0        0    16525 2016-10-26 13:27:38.000000 wikitextparser-0.9.0.dev1/wikitextparser/table.py
--rw-rw-rw-   0        0        0    10900 2016-10-25 14:37:48.000000 wikitextparser-0.9.0.dev1/wikitextparser/table_test.py
--rw-rw-rw-   0        0        0     8564 2016-10-26 13:28:04.000000 wikitextparser-0.9.0.dev1/wikitextparser/tag.py
--rw-rw-rw-   0        0        0     4643 2016-10-26 03:09:05.000000 wikitextparser-0.9.0.dev1/wikitextparser/tag_test.py
--rw-rw-rw-   0        0        0    13603 2016-10-26 13:51:46.000000 wikitextparser-0.9.0.dev1/wikitextparser/template.py
--rw-rw-rw-   0        0        0     9707 2016-10-17 08:31:11.000000 wikitextparser-0.9.0.dev1/wikitextparser/template_test.py
--rw-rw-rw-   0        0        0     2075 2016-10-26 13:29:07.000000 wikitextparser-0.9.0.dev1/wikitextparser/wikilink.py
--rw-rw-rw-   0        0        0     1674 2016-10-17 08:33:17.000000 wikitextparser-0.9.0.dev1/wikitextparser/wikilink_test.py
--rw-rw-rw-   0        0        0    37214 2016-10-26 14:42:50.000000 wikitextparser-0.9.0.dev1/wikitextparser/wikitext.py
--rw-rw-rw-   0        0        0      230 2016-10-12 08:07:10.000000 wikitextparser-0.9.0.dev1/wikitextparser/wikitextparser_test.py
--rw-rw-rw-   0        0        0    24873 2016-10-26 14:47:21.000000 wikitextparser-0.9.0.dev1/wikitextparser/wikitext_test.py
--rw-rw-rw-   0        0        0      717 2016-10-26 03:19:31.000000 wikitextparser-0.9.0.dev1/wikitextparser/__init__.py
-drwxrwxrwx   0        0        0        0 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/wikitextparser.egg-info/
--rw-rw-rw-   0        0        0        1 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/wikitextparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     8538 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/wikitextparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/wikitextparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1074 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/wikitextparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2016-10-26 14:52:39.000000 wikitextparser-0.9.0.dev1/wikitextparser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/
+-rw-rw-rw-   0        0        0    35795 2015-03-24 09:52:20.000000 wikitextparser-0.9.1/LICENSE.md
+-rw-rw-rw-   0        0        0       14 2016-10-24 02:10:33.000000 wikitextparser-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8533 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6268 2016-10-25 02:22:59.000000 wikitextparser-0.9.1/README.rst
+-rw-rw-rw-   0        0        0       64 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2016-11-02 13:06:12.000000 wikitextparser-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/wikitextparser/
+-rw-rw-rw-   0        0        0     4778 2016-10-25 05:44:46.000000 wikitextparser-0.9.1/wikitextparser/argument.py
+-rw-rw-rw-   0        0        0     3050 2016-10-25 00:10:38.000000 wikitextparser-0.9.1/wikitextparser/argument_test.py
+-rw-rw-rw-   0        0        0      950 2016-10-13 01:13:10.000000 wikitextparser-0.9.1/wikitextparser/comment.py
+-rw-rw-rw-   0        0        0      342 2016-10-17 08:07:18.000000 wikitextparser-0.9.1/wikitextparser/comment_test.py
+-rw-rw-rw-   0        0        0     2485 2016-10-26 13:24:44.000000 wikitextparser-0.9.1/wikitextparser/externallink.py
+-rw-rw-rw-   0        0        0     2166 2016-10-17 08:09:25.000000 wikitextparser-0.9.1/wikitextparser/externallink_test.py
+-rw-rw-rw-   0        0        0    18058 2016-10-24 12:26:18.000000 wikitextparser-0.9.1/wikitextparser/list_parser.py
+-rw-rw-rw-   0        0        0     1695 2016-07-20 09:21:21.000000 wikitextparser-0.9.1/wikitextparser/list_parser_test_ignore.py
+-rw-rw-rw-   0        0        0     3533 2016-10-26 13:27:12.000000 wikitextparser-0.9.1/wikitextparser/parameter.py
+-rw-rw-rw-   0        0        0     2945 2016-10-17 08:12:29.000000 wikitextparser-0.9.1/wikitextparser/parameter_test.py
+-rw-rw-rw-   0        0        0     2546 2016-10-25 04:35:30.000000 wikitextparser-0.9.1/wikitextparser/parser_function.py
+-rw-rw-rw-   0        0        0     1826 2016-10-17 08:15:59.000000 wikitextparser-0.9.1/wikitextparser/parser_function_test.py
+-rw-rw-rw-   0        0        0     2932 2016-10-25 04:37:22.000000 wikitextparser-0.9.1/wikitextparser/section.py
+-rw-rw-rw-   0        0        0     2065 2016-09-16 03:07:22.000000 wikitextparser-0.9.1/wikitextparser/section_test.py
+-rw-rw-rw-   0        0        0    13219 2016-10-30 14:27:24.000000 wikitextparser-0.9.1/wikitextparser/spans.py
+-rw-rw-rw-   0        0        0    13457 2016-10-30 14:24:26.000000 wikitextparser-0.9.1/wikitextparser/spans_test.py
+-rw-rw-rw-   0        0        0    17003 2016-11-02 12:55:41.000000 wikitextparser-0.9.1/wikitextparser/table.py
+-rw-rw-rw-   0        0        0    12116 2016-11-02 12:56:55.000000 wikitextparser-0.9.1/wikitextparser/table_test.py
+-rw-rw-rw-   0        0        0     8564 2016-10-30 01:17:18.000000 wikitextparser-0.9.1/wikitextparser/tag.py
+-rw-rw-rw-   0        0        0     4643 2016-10-26 03:09:05.000000 wikitextparser-0.9.1/wikitextparser/tag_test.py
+-rw-rw-rw-   0        0        0    14026 2016-10-27 16:53:08.000000 wikitextparser-0.9.1/wikitextparser/template.py
+-rw-rw-rw-   0        0        0    10499 2016-10-27 16:45:29.000000 wikitextparser-0.9.1/wikitextparser/template_test.py
+-rw-rw-rw-   0        0        0     2075 2016-10-26 13:29:07.000000 wikitextparser-0.9.1/wikitextparser/wikilink.py
+-rw-rw-rw-   0        0        0     1674 2016-10-17 08:33:17.000000 wikitextparser-0.9.1/wikitextparser/wikilink_test.py
+-rw-rw-rw-   0        0        0    37281 2016-10-31 10:24:45.000000 wikitextparser-0.9.1/wikitextparser/wikitext.py
+-rw-rw-rw-   0        0        0      230 2016-10-12 08:07:10.000000 wikitextparser-0.9.1/wikitextparser/wikitextparser_test.py
+-rw-rw-rw-   0        0        0    25575 2016-10-31 10:24:08.000000 wikitextparser-0.9.1/wikitextparser/wikitext_test.py
+-rw-rw-rw-   0        0        0      717 2016-10-26 03:19:31.000000 wikitextparser-0.9.1/wikitextparser/__init__.py
+drwxrwxrwx   0        0        0        0 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/wikitextparser.egg-info/
+-rw-rw-rw-   0        0        0        1 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/wikitextparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     8533 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/wikitextparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/wikitextparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1074 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/wikitextparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2016-11-02 13:13:38.000000 wikitextparser-0.9.1/wikitextparser.egg-info/top_level.txt
```

### Comparing `wikitextparser-0.9.0.dev1/LICENSE.md` & `wikitextparser-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/PKG-INFO` & `wikitextparser-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wikitextparser
-Version: 0.9.0.dev1
+Version: 0.9.1
 Summary: A simple, purely python, WikiText parsing tool.
 Home-page: https://github.com/5j9/wikitextparser
 Author: 5j9
 Author-email: 5j9@users.noreply.github.com
 License: GNU General Public License v3 (GPLv3)
 Description: .. image:: https://travis-ci.org/5j9/wikitextparser.svg?branch=master
             :target: https://travis-ci.org/5j9/wikitextparser
```

### Comparing `wikitextparser-0.9.0.dev1/README.rst` & `wikitextparser-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/setup.py` & `wikitextparser-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import path
 
 
 here = path.abspath(path.dirname(__file__))
 setup(
     name='wikitextparser',
     # Scheme: [N!]N(.N)*[{a|b|rc}N][.postN][.devN]
-    version='0.9.0.dev1',
+    version='0.9.1',
     description='A simple, purely python, WikiText parsing tool.',
     long_description=open(path.join(here, 'README.rst')).read(),
     url='https://github.com/5j9/wikitextparser',
     author='5j9',
     author_email='5j9@users.noreply.github.com',
     license='GNU General Public License v3 (GPLv3)',
     packages=find_packages(),
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/argument.py` & `wikitextparser-0.9.1/wikitextparser/argument.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/argument_test.py` & `wikitextparser-0.9.1/wikitextparser/argument_test.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/comment.py` & `wikitextparser-0.9.1/wikitextparser/comment.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/externallink.py` & `wikitextparser-0.9.1/wikitextparser/externallink.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/externallink_test.py` & `wikitextparser-0.9.1/wikitextparser/externallink_test.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/list_parser.py` & `wikitextparser-0.9.1/wikitextparser/list_parser.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/list_parser_test_ignore.py` & `wikitextparser-0.9.1/wikitextparser/list_parser_test_ignore.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/parameter.py` & `wikitextparser-0.9.1/wikitextparser/parameter.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/parameter_test.py` & `wikitextparser-0.9.1/wikitextparser/parameter_test.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/parser_function.py` & `wikitextparser-0.9.1/wikitextparser/parser_function.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/parser_function_test.py` & `wikitextparser-0.9.1/wikitextparser/parser_function_test.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/section.py` & `wikitextparser-0.9.1/wikitextparser/section.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/section_test.py` & `wikitextparser-0.9.1/wikitextparser/section_test.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/spans.py` & `wikitextparser-0.9.1/wikitextparser/spans.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     TEMPLATE_PATTERN + r'(?!\})'
     r'|(?<!{)' + TEMPLATE_PATTERN
 )
 # Parameters
 TEMPLATE_PARAMETER_REGEX = re.compile(r'\{\{\{[^{}]*?\}\}\}')
 # Parser functions
 # According to https://www.mediawiki.org/wiki/Help:Magic_words
-# See also :
+# See also:
 # https://translatewiki.net/wiki/MediaWiki:Sp-translate-data-MagicWords/fa
 PARSER_FUNCTION_REGEX = re.compile(
     r"""
     \{\{\s*
     (?:
       \#[^{}\s]*?|
       # Variables acting like parser functions
@@ -328,19 +328,18 @@
     parameter_spans: list,
     parser_function_spans: list,
     template_spans: list,
 ) -> None:
     """Parse the substring to spans.
 
     This function is basically the same as `parse_to_spans`, but accepts an
-    index that indicates the start of the substring. `substrings` are the
+    index that indicates the start of the substring. `substring`s are the
     contents of PARSABLE_TAG_EXTENSIONS.
 
     """
-    # Todo: Do we need to parse for nested tag extensions?
     # Remove the braces inside WikiLinks.
     # WikiLinks may contain braces that interfere with
     # detection of templates. For example when parsing `{{text |[[A|}}]] }}`,
     # the span of the template should be the whole string.
     loop = True
     while loop:
         loop = False
@@ -372,22 +371,23 @@
 def parse_to_spans_innerloop(
     string: str,
     index: int,
     parameter_spans: list,
     parser_function_spans: list,
     template_spans: list,
 ) -> None:
-    """Run the main loop for _get_spans.
+    """Find the spans of parameters, parser functions, and templates.
 
     :string: The string or part of string that is being parsed.
     :index: Add to every returned index.
 
-    This function was created because the _get_spans function needs to
-    call it n + 1 time. One time for the whole string and n times for
-    each of the n WikiLinks.
+    This is the innermost loop of the parse_to_spans function.
+    If the string passed to parse_to_spans contains n WikiLinks, then
+    this function will be called n + 1 times. One time for the whole string
+    and n times for each of the n WikiLinks.
 
     """
     while True:
         # Single braces will interfere with detection of other elements and
         # should be removed beforehand.
         string = SINGLE_BRACES_REGEX.sub('_', string)
         # Also remove empty double braces
@@ -398,15 +398,15 @@
                 loop = True
                 group = match.group()
                 string = string.replace(group, len(group) * '_')
         # The following was much more faster than
         # string = re.sub(r'{(?=[^}]*$)', '_', string)
         head, sep, tail = string.rpartition('}')
         string = ''.join((head, sep, tail.replace('{', '_')))
-        # Also Python does not support non-fixed-length lookbehinds
+        # Also the re module does not support non-fixed-length lookbehinds.
         head, sep, tail = string.partition('{')
         string = ''.join((head.replace('}', '_'), sep, tail))
         match = None
         # Template parameters
         loop = True
         while loop:
             loop = False
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/spans_test.py` & `wikitextparser-0.9.1/wikitextparser/spans_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,10 +302,16 @@
         # May change in the future.
         self.assertNotRegex('{{msg:xyz}}', regex)
         self.assertNotRegex('{{raw:xyz}}', regex)
         self.assertNotRegex('{{raw:xyz}}', regex)
         # Miscellaneous
         self. assertRegex('{{#language:language code}}', regex)
 
+    def test_wikilinks_inside_exttags(self):
+        wt = wtp.WikiText("<ref>[[w]]</ref>")
+        self.assertEqual(
+            [(5, 10)],
+            wt._type_to_spans['wikilinks'],
+        )
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/table.py` & `wikitextparser-0.9.1/wikitextparser/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,21 +159,21 @@
         return 'Table(' + repr(self.string) + ')'
 
     def _get_span(self) -> tuple:
         """Return the self-span."""
         return self._type_to_spans['tables'][self._index]
 
     def getdata(self, span: bool=True) -> list:
-        """Return a list containing list of values of all rows.
+        """Return a list containing lists of row values.
 
-        :span: indicates if rowspans and colspans attributes should be
-            expanded or not.
+        :span: If true, calculate rows according to rowspans and colspans
+            attributes. Otherwise ignore them.
 
-        Due to the lots of complications that it will cause, this function
-        won't look inside templates, parserfunctions, etc.
+        Due to the lots of complications that it may cause, this function
+        won't look inside templates, parser functions, etc.
 
         See https://www.mediawiki.org/wiki/Extension:Pipe_Escape for how
         wikitables can be inserted within templates.
 
         """
         string = self.string
         length = len(string)
@@ -370,38 +370,39 @@
         self.feed('<a ' + attrs + '>')
         return dict(self.parsed)
 
 
 def _apply_attr_spans(
     attr_spans: list, data: list, string: str
 ) -> list:
-    """Apply colspans to data and return data."""
+    """Apply row and column spans and return data."""
     # Todo: maybe it's better to do this parsing in self.getdata?
     attrs = []
     for r in attr_spans:
         attrs.append([])
         for ss, se in r:
             if se is not None:
                 attrs[-1].append(attrs_parser(string[ss:se]))
             else:
                 attrs[-1].append(None)
     # The following code is based on the table forming algorithm described
     # at http://www.w3.org/TR/html5/tabular-data.html#processing-model-1
-    # Some comments indicate the step in that algorithm.
+    # Numbered comments indicate the step in that algorithm.
     # 1
     xwidth = 0
     # 2
     yheight = 0
     # 4
     # The xwidth and yheight variables give the table's dimensions.
     # The table is initially empty.
     table = []
+    # getdata won't call this function if data is empty.
     # 5
-    if not data:
-        return data
+    # if not data:
+    #     return data
     # 10
     ycurrent = 0
     # 11
     downward_growing_cells = []
     # 13, 18
     # Algorithm for processing rows
     for i, row in enumerate(data):
@@ -418,39 +419,45 @@
             for x in range(cellx, cellx + width):
                 r[x] = cell
         # 13.4 will be handled by the following for-loop.
         # 13.5, 13.16
         for j, current_cell in enumerate(row):
             # 13.6
             while (
-                        xcurrent < xwidth and
-                        table[ycurrent][xcurrent] is not None
+                xcurrent < xwidth and
+                table[ycurrent][xcurrent] is not None
             ):
                 xcurrent += 1
             # 13.7
             if xcurrent == xwidth:
                 # xcurrent is never greater than xwidth
                 xwidth += 1
                 for r in table:
                     if xwidth > len(r):
                         r.extend([None] * (xwidth - len(r)))
             # 13.8
             try:
                 colspan = int(attrs[i][j]['colspan'])
                 if colspan == 0:
+                    # Note: colspan="0" tells the browser to span the cell to
+                    # the last column of the column group (colgroup)
+                    # http://www.w3schools.com/TAGS/att_td_colspan.asp
                     colspan = 1
             except Exception:
                 colspan = 1
             # 13.9
             try:
                 rowspan = int(attrs[i][j]['rowspan'])
             except Exception:
                 rowspan = 1
             # 13.10
             if rowspan == 0:
+                # Note: rowspan="0" tells the browser to span the cell to the
+                # last row of the table.
+                # http://www.w3schools.com/tags/att_td_rowspan.asp
                 cell_grows_downward = True
                 rowspan = 1
             else:
                 cell_grows_downward = False
             # 13.11
             if xwidth < xcurrent + colspan:
                 xwidth = xcurrent + colspan
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/table_test.py` & `wikitextparser-0.9.1/wikitextparser/table_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -209,27 +209,78 @@
             ['11', '11', '11', '11', '11', '11'],
             ['21', '22', '23', '24', '25', '25'],
             ['21', '31', '32', '32', '33', '34'],
         ])
 
     def test_inline_colspan_and_rowspan(self):
         table = wtp.Table(
-            '{| class=wikitable\n !a !! b !!  c !! colspan = 2 | d \n '
-            '|- \n | e || colspan = "2"| f   || g || h\n |}'
+            '{| class=wikitable\n'
+            ' !a !! b !!  c !! rowspan = 2 | d \n'
+            ' |- \n'
+            ' | e || colspan = "2"| f\n'
+            '|}'
         )
         self.assertEqual(table.getdata(span=True), [
-            ['a', 'b', 'c', 'd', 'd'],
-            ['e', 'f', 'f', 'g', 'h']
+            ['a', 'b', 'c', 'd'],
+            ['e', 'f', 'f', 'd']
         ])
 
-    def test_template_inside_table(self):
-        # This tests self._shadow function.
-        s = '{{t|1}}\n{|class=wikitable\n|a\n|}\n{{t|1}}'
-        p = wtp.parse(s)
-        self.assertEqual([['a']], p.tables[0].getdata())
+    def test_growing_downward_growing_cells(self):
+        table = wtp.Table(
+            '{|class=wikitable\n'
+            '| a || rowspan=0 | b\n'
+            '|-\n'
+            '| c\n'
+            '|}'
+        )
+        self.assertEqual(table.getdata(span=True), [
+            ['a', 'b'],
+            ['c', 'b'],
+        ])
+
+    def test_colspan_0(self):
+        table = wtp.Table(
+            '{|class=wikitable\n'
+            '| colspan=0 | a || b\n'
+            '|-\n'
+            '| c || d\n'
+            '|}'
+        )
+        self.assertEqual(table.getdata(span=True), [
+            ['a', 'b'],
+            ['c', 'd'],
+        ])
+
+    def test_ending_row_group(self):
+        table = wtp.Table(
+            '{|class=wikitable\n'
+            '| rowspan = 3 | a || b\n'
+            '|-\n'
+            '| c\n'
+            '|}'
+        )
+        self.assertEqual(table.getdata(span=True), [
+            ['a', 'b'],
+            ['a', 'c'],
+            ['a', None],
+        ])
+
+    def test_ending_row_group_and_rowspan_0(self):
+        table = wtp.Table(
+            '{|class=wikitable\n'
+            '| rowspan = 3 | a || rowspan = 0 | b || c\n'
+            '|-\n'
+            '| d\n'
+            '|}'
+        )
+        self.assertEqual(table.getdata(span=True), [
+            ['a', 'b', 'c'],
+            ['a', 'b', 'd'],
+            ['a', 'b', None],
+        ])
 
 
 class GetRowData(unittest.TestCase):
 
     """Test the getrdata method of the Table class."""
 
     def test_second_of_three(self):
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/tag.py` & `wikitextparser-0.9.1/wikitextparser/tag.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/tag_test.py` & `wikitextparser-0.9.1/wikitextparser/tag_test.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/template.py` & `wikitextparser-0.9.1/wikitextparser/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,19 +65,19 @@
                     )
                 )
         return arguments
 
     @property
     def name(self) -> str:
         """Return template's name (includes whitespace)."""
-        p0 = self._not_in_atomic_subspans_partition('|')[0]
-        if len(p0) == len(self.string):
-            return p0[2:-2]
+        h = self._not_in_atomic_subspans_partition('|')[0]
+        if len(h) == len(self.string):
+            return h[2:-2]
         else:
-            return p0[2:]
+            return h[2:]
 
     @name.setter
     def name(self, newname: str) -> None:
         """Set the new name for the template."""
         name = self.name
         self[2:2 + len(name)] = newname
 
@@ -156,69 +156,71 @@
                 del a[0:len(a.string)]
             else:
                 names.append(name)
 
     def rm_dup_args_safe(self, tag: str or None=None) -> None:
         """Remove duplicate arguments in a safe manner.
 
-        Remove the duplicate arguments only if:
-        1. Both arguments have the same name AND value.
-        2. Arguments have the same name and one of them is empty. (Remove the
-            empty one.)
-
-        Warning: Although this is considered to be safe as no meaningful data
-            is removed but the result of the renedered wikitext may actually
-            change if the second arg is empty and removed but the first has a
-            value.
+        Remove the duplicate arguments only in the following situations:
+            1. Both arguments have the same name AND value. (Remove one of
+                them.)
+            2. Arguments have the same name and one of them is empty. (Remove
+                the empty one.)
+
+        Warning: Although this is considered to be safe and no meaningful data
+            is removed from wikitext, but the result of the rendered wikitext
+            may actually change if the second arg is empty and removed but
+            the first had had a value.
 
-        If `tag` is defined, it should be a string, tag the remaining
-        arguments by appending the provided tag to their value.
+        If `tag` is defined, it should be a string that will be appended to
+        the value of the remaining duplicate arguments.
 
         Also see `rm_first_of_dup_args` function.
 
         """
-        name_args_vals = {}
+        name_to_lastarg_vals = {}
         # Removing positional args affects their name. By reversing the list
         # we avoid encountering those kind of args.
         for arg in reversed(self.arguments):
             name = arg.name.strip()
             if arg.positional:
                 # Value of keyword arguments is automatically stripped by MW.
                 val = arg.value
             else:
                 # But it's not OK to strip whitespace in positional arguments.
                 val = arg.value.strip()
-            if name in name_args_vals:
+            if name in name_to_lastarg_vals:
                 # This is a duplicate argument.
                 if not val:
                     # This duplicate argument is empty. It's safe to remove it.
                     del arg[0:len(arg.string)]
                 else:
                     # Try to remove any of the detected duplicates of this
                     # that are empty or their value equals to this one.
-                    name_args = name_args_vals[name][0]
-                    name_vals = name_args_vals[name][1]
-                    if val in name_vals:
+                    lastarg, dup_vals = name_to_lastarg_vals[name]
+                    if val in dup_vals:
                         del arg[0:len(arg.string)]
-                    elif '' in name_vals:
-                        i = name_vals.index('')
-                        a = name_args.pop(i)
-                        del a[0:len(a.string)]
-                        name_vals.pop(i)
+                    elif '' in dup_vals:
+                        # This happens only if the last occurrence of name has
+                        # been an empty string; other empty values will
+                        # be removed as they are seen.
+                        # In other words index of the empty argument in
+                        # dup_vals is always 0.
+                        del lastarg[0:len(lastarg.string)]
+                        dup_vals.pop(0)
                     else:
                         # It was not possible to remove any of the duplicates.
-                        name_vals.append(arg)
-                        name_vals.append(val)
+                        dup_vals.append(val)
                         if tag:
                             arg.value += tag
             else:
-                name_args_vals[name] = ([arg], [val])
+                name_to_lastarg_vals[name] = (arg, [val])
 
     def set_arg(
-        self, name: str,
+        self, name: str or None,
         value: str,
         positional: bool or None=None,
         before: str or None=None,
         after: str or None=None,
         preserve_spacing: bool=True
     ) -> None:
         """Set the value for `name` argument. Add it if it doesn't exist.
@@ -242,15 +244,15 @@
             if preserve_spacing:
                 val = arg.value
                 arg.value = val.replace(val.strip(), value)
             else:
                 arg.value = value
             return
         # Adding a new argument
-        if positional is None and not name:
+        if not name and positional is None:
             positional = True
         # Calculate the whitespace needed before arg-name and after arg-value.
         if not positional and preserve_spacing and args:
             before_names = []
             name_lengths = []
             before_values = []
             after_values = []
@@ -287,32 +289,35 @@
             arg = get_arg(before, args)
             arg.insert(0, addstring)
         elif after:
             arg = get_arg(after, args)
             arg.insert(len(arg.string), addstring)
         else:
             if args and not positional:
-                # Insert after the last argument.
-                # The addstring needs to be recalculated because we don't
-                # want to change the the whitespace before the final braces.
                 arg = args[0]
                 arg_string = arg.string
-                arg[0:len(arg_string)] = (
-                    arg.string.rstrip() + after_value + addstring.rstrip() +
-                    after_values[0]
-                )
+                if preserve_spacing:
+                    # Insert after the last argument.
+                    # The addstring needs to be recalculated because we don't
+                    # want to change the the whitespace before the final braces.
+                    arg[0:len(arg_string)] = (
+                        arg.string.rstrip() + after_value + addstring.rstrip() +
+                        after_values[0]
+                    )
+                else:
+                    arg.insert(len(arg_string), addstring)
             else:
                 # The template has no arguments or the new arg is
                 # positional AND is to be added at the end of the template.
                 self.insert(-2, addstring)
 
     def get_arg(self, name: str) -> Argument or None:
         """Return the last argument with the given name.
 
-        Return None if no such argument is found.
+        Return None if no argument with that name is found.
 
         """
         return get_arg(name, reversed(self.arguments))
 
     def has_arg(self, name: str, value: str or None=None) -> bool:
         """Return true if the is an arg named `name`.
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/template_test.py` & `wikitextparser-0.9.1/wikitextparser/template_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,18 @@
         t = Template('{{t|1=v|v|1=v}}')
         t.rm_dup_args_safe(tag='<!-- dup -->')
         self.assertEqual('{{t|1=v}}', t.string)
         # Tag even if one of the duplicate values is different.
         t = Template('{{t|1=v|v|1=u}}')
         t.rm_dup_args_safe(tag='<!-- dup -->')
         self.assertEqual('{{t|v<!-- dup -->|1=u}}', t.string)
+        # Duplicate argument's value is empty
+        t = Template('{{t|b|1=c|1=}}')
+        t.rm_dup_args_safe()
+        self.assertEqual('{{t|b|1=c}}', t.string)
 
     def test_has_arg(self):
         t = Template('{{t|a|b=c}}')
         self.assertEqual(True, t.has_arg('1'))
         self.assertEqual(True, t.has_arg('1', 'a'))
         self.assertEqual(True, t.has_arg('b'))
         self.assertEqual(True, t.has_arg('b', 'c'))
@@ -183,17 +187,17 @@
         self.assertEqual('', p.string)
 
     def test_no_param_template_name(self):
         t = Template("{{صعود}}")
         self.assertEqual('صعود', t.name)
 
 
-class TemplateSetArg(unittest.TestCase):
+class SetArg(unittest.TestCase):
 
-    """Test set_arg function of Template class."""
+    """Test set_arg method of Template class."""
 
     def test_set_arg(self):
         # Template with no args, keyword
         t = Template('{{t}}')
         t.set_arg('a', 'b')
         self.assertEqual('{{t|a=b}}', t.string)
         # Template with no args, auto positional
@@ -221,14 +225,28 @@
         # Preserve spacing, only one argument
         t = Template('{{t\n  |  afadfaf =   value \n}}')
         t.set_arg('z', 'z')
         self.assertEqual(
             '{{t\n  |  afadfaf =   value\n  |  z       =   z\n}}', t.string
         )
 
+    def test_existing_dont_preserve_space(self):
+        t = Template('{{t\n  |  a =   v \n}}')
+        t.set_arg('a', 'w', preserve_spacing=False)
+        self.assertEqual(
+            '{{t\n  |  a =w}}', t.string
+        )
+
+    def test_new_dont_preserve_space(self):
+        t = Template('{{t\n  |  a =   v \n}}')
+        t.set_arg('b', 'w', preserve_spacing=False)
+        self.assertEqual(
+            '{{t\n  |  a =   v \n|b=w}}', t.string
+        )
+
     def test_before(self):
         t = Template('{{t|a|b|c=c|d}}')
         t.set_arg('e', 'e', before='c')
         self.assertEqual('{{t|a|b|e=e|c=c|d}}', t.string)
 
     def test_after(self):
         t = Template('{{t|a|b|c=c|d}}')
@@ -254,9 +272,14 @@
 
     def test_nowiki_makes_equal_ineffective(self):
         t = Template('{{text|1<nowiki>=</nowiki>g}}')
         a = t.arguments[0]
         self.assertEqual(a.value, '1<nowiki>=</nowiki>g')
         self.assertEqual(a.name, '1')
 
+    def test_not_name_and_positional_is_none(self):
+        t = Template('{{t}}')
+        t.set_arg(None, 'v')
+        self.assertEqual('{{t|v}}', t.string)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/wikilink.py` & `wikitextparser-0.9.1/wikitextparser/wikilink.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/wikilink_test.py` & `wikitextparser-0.9.1/wikitextparser/wikilink_test.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/wikitext.py` & `wikitextparser-0.9.1/wikitextparser/wikitext.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,14 +100,17 @@
             return False
         ps, pe = value._get_span()
         ss, se = self._get_span()
         if ss <= ps and se >= pe:
             return True
         return False
 
+    def __len__(self):
+        return len(self.string)
+
     def __getitem__(self, key: slice or int) -> str:
         """Return self.string[item]."""
         return self.string[key]
 
     def _check_index(self, key: slice or int) -> (int, int):
         """Return adjusted start and stop index as tuple.
 
@@ -329,16 +332,17 @@
             'wikilinks', 'comments', 'exttags'
         ):
             for span in types_to_spans[key]:
                 if ss < span[0] and span[1] <= se:
                     subspans.append(span)
 
         # Define the function to be returned.
+        # Todo: index_in_spans can be cached.
         def index_in_spans(index: int) -> bool:
-            """Return True if the given index is found within a subspans."""
+            """Return True if the given index belongs to a sub-span."""
             for ss, se in subspans:
                 if ss <= index < se:
                     return True
             return False
 
         return index_in_spans
 
@@ -351,55 +355,55 @@
                 yield i
 
     def _close_subspans(self, start: int, stop: int) -> None:
         """Close all subspans of (start, stop)."""
         ss, se = self._get_span()
         for type_spans in self._type_to_spans.values():
             for i, (s, e) in enumerate(type_spans):
-                if (
-                    (start <= s and e < stop) or
-                    (start < s and e <= stop) or
-                    (start == s and e == stop and (ss != s or se != e))
-                ):
+                if (start <= s and e <= stop) and (ss != s or se != e):
                     type_spans[i] = (start, start)
 
     def _shrink_span_update(self, rmstart: int, rmstop: int) -> None:
         """Update self._type_to_spans according to the removed span.
 
         Warning: If an operation involves both _shrink_span_update and
         _extend_span_update, you might wanna consider doing the
         _extend_span_update before the _shrink_span_update as this function
         can cause data loss in self._type_to_spans.
 
         """
         # Note: No span should be removed from _type_to_spans.
         rmlength = rmstop - rmstart
         for t, spans in self._type_to_spans.items():
-            for i, (spanstart, spanend) in enumerate(spans):
-                if spanend <= rmstart:
+            for i, (s, e) in enumerate(spans):
+                if e <= rmstart:
+                    # s <= e <= rmstart <= rmstop
                     continue
-                elif rmstop <= spanstart:
-                    # removed part is before the span
-                    spans[i] = (spanstart - rmlength, spanend - rmlength)
-                elif rmstart < spanstart:
-                    # spanstart needs to be changed
-                    # we already know that rmstop is after the spanstart
-                    # so the new spanstart should be located at rmstart
-                    if rmstop <= spanend:
-                        spans[i] = (rmstart, spanend - rmlength)
-                    else:
-                        # Shrink to an empty string.
+                elif rmstop <= s:
+                    # rmstart <= rmstop <= s <= e
+                    spans[i] = (s - rmlength, e - rmlength)
+                elif rmstart <= s:
+                    # s needs to be changed.
+                    # We already know that rmstop is after the s,
+                    # therefore the new s should be located at rmstart.
+                    if rmstop >= e:
+                        # rmstart <= s <= e < rmstop
                         spans[i] = (rmstart, rmstart)
+                    else:
+                        # rmstart < s <= rmstop <= e
+                        spans[i] = (rmstart, e - rmlength)
                 else:
-                    # we already know that spanstart is before the rmstart
-                    # so the spanstart needs no change.
-                    if rmstop <= spanend:
-                        spans[i] = (spanstart, spanend - rmlength)
+                    # From the previous comparison we know that s is before
+                    # the rmstart; so s needs no change.
+                    if rmstop < e:
+                        # s <= rmstart <= rmstop <= e
+                        spans[i] = (s, e - rmlength)
                     else:
-                        spans[i] = (spanstart, rmstart)
+                        # s <= rmstart <= e < rmstop
+                        spans[i] = (s, rmstart)
 
     def _extend_span_update(self, estart: int, elength: int) -> None:
         """Update self._type_to_spans according to the added span."""
         # Note: No span should be removed from _type_to_spans.
         ss, se = self._get_span()
         for spans in self._type_to_spans.values():
             for i, (spanstart, spanend) in enumerate(spans):
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/wikitext_test.py` & `wikitextparser-0.9.1/wikitextparser/wikitext_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 import wikitextparser as wtp
 
 
 class WikiText(unittest.TestCase):
 
     """Test basic functionalities of the WikiText class."""
 
+    def test_len(self):
+        t2, t1 = wtp.WikiText('{{t1|{{t2}}}}').templates
+        self.assertEqual(len(t2), 6)
+        self.assertEqual(len(t1), 13)
+
     def test_repr(self):
         self.assertEqual(repr(wtp.parse('')), "WikiText('')")
 
     def test_getitem(self):
         s = '{{t1|{{t2}}}}'
         t2, t1 = wtp.WikiText(s).templates
         self.assertEqual(t2[2], 't')
@@ -136,58 +141,43 @@
     def test_opcodes_in_spans_should_be_referenced_based_on_self_lststr0(self):
         wt = wtp.WikiText('{{a}}{{ b\n|d=}}')
         template = wt.templates[1]
         arg = template.arguments[0]
         template.name = template.name.strip()
         self.assertEqual('|d=', arg.string)
 
+    def test_rmstart_s__rmstop__e(self):
+        wt = wtp.WikiText('{{t|<!--c-->}}')
+        c = wt.comments[0]
+        t = wt.templates[0]
+        t[3:8] = ''
+        self.assertEqual(c.string, 'c-->')
+
 
 class ExpandSpanUpdate(unittest.TestCase):
 
     """Test the _expand_span_update method."""
 
     def test_extending_template_name_should_not_effect_arg_string(self):
         t = wtp.Template('{{t|1=2}}')
         a = t.arguments[0]
         t.name = 't\n    '
         self.assertEqual('|1=2', a.string)
 
-    def test_extend_selfspan_when_inserting_at_the_end_of_selfspan(self):
-        wt = wtp.WikiText('{{ t|a={{#if:c|a}}|b=}}\n')
+    def test_overwriting_or_extending_selfspan_will_cause_data_loss(self):
+        wt = wtp.WikiText('{{t|{{#if:a|b|c}}}}')
         a = wt.templates[0].arguments[0]
         pf = wt.parser_functions[0]
-        a.value += '    \n'
-        self.assertEqual('|a={{#if:c|a}}    \n', a.string)
-        # Note that the parser function is overwritten
+        a.value += ''
+        self.assertEqual('|{{#if:a|b|c}}', a.string)
+        # Note that the old parser function is overwritten
+        self.assertEqual('', pf.string)
+        pf = a.parser_functions[1]
+        a.value = 'a'
         self.assertEqual('', pf.string)
-
-
-class IndentLevel(unittest.TestCase):
-
-    """Test the _get_indent_level method of the WikiText class."""
-
-    def test_a_in_b(self):
-        s = '{{b|{{a}}}}'
-        a, b = wtp.WikiText(s).templates
-        self.assertEqual(1, b._get_indent_level())
-        self.assertEqual(2, a._get_indent_level())
-
-    def test_repprint(self):
-        """Make sure that pprint won't mutate self."""
-        s = '{{a|{{b|{{c}}}}}}'
-        c, b, a = wtp.WikiText(s).templates
-        self.assertEqual(
-            '{{a\n    | 1 = {{b\n        | 1 = {{c}}\n    }}\n}}',
-            a.pprint(),
-        )
-        # Again:
-        self.assertEqual(
-            '{{a\n    | 1 = {{b\n        | 1 = {{c}}\n    }}\n}}',
-            a.pprint(),
-        )
 
 
 class ExternalLinks(unittest.TestCase):
 
     """Test the WikiText class."""
 
     def test_bare_link(self):
@@ -409,14 +399,31 @@
         other extension tags.
 
         """
         s = '<nowiki>:</nowiki>{|class=wikitable\n|a\n|}'
         wt = wtp.parse(s)
         self.assertEqual(len(wt.tables), 0)
 
+    def test_template_before_or_after_table(self):
+        # This tests self._shadow function.
+        s = '{{t|1}}\n{|class=wikitable\n|a\n|}\n{{t|1}}'
+        p = wtp.parse(s)
+        self.assertEqual([['a']], p.tables[0].getdata())
+
+
+class IndentLevel(unittest.TestCase):
+
+    """Test the _get_indent_level method of the WikiText class."""
+
+    def test_a_in_b(self):
+        s = '{{b|{{a}}}}'
+        a, b = wtp.WikiText(s).templates
+        self.assertEqual(1, b._get_indent_level())
+        self.assertEqual(2, a._get_indent_level())
+
 
 class PrettyPrint(unittest.TestCase):
 
     """Test the pprint method of the WikiText class."""
 
     def test_template_with_multi_args(self):
         s = "{{a|b=b|c=c|d=d|e=e}}"
@@ -705,14 +712,28 @@
         self.assertEqual(
             '{{b\n'
             '    | 1 = {{c}}\n'
             '}}',
             b.pprint(),
         )
 
+    def test_repprint(self):
+        """Make sure that pprint won't mutate self."""
+        s = '{{a|{{b|{{c}}}}}}'
+        c, b, a = wtp.WikiText(s).templates
+        self.assertEqual(
+            '{{a\n    | 1 = {{b\n        | 1 = {{c}}\n    }}\n}}',
+            a.pprint(),
+        )
+        # Again:
+        self.assertEqual(
+            '{{a\n    | 1 = {{b\n        | 1 = {{c}}\n    }}\n}}',
+            a.pprint(),
+        )
+
 
 class Sections(unittest.TestCase):
 
     """Test the sections method of the WikiText class."""
 
     def test_grab_the_final_newline_for_the_last_section(self):
         wt = wtp.WikiText('== s ==\nc\n')
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser/__init__.py` & `wikitextparser-0.9.1/wikitextparser/__init__.py`

 * *Files identical despite different names*

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser.egg-info/PKG-INFO` & `wikitextparser-0.9.1/wikitextparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wikitextparser
-Version: 0.9.0.dev1
+Version: 0.9.1
 Summary: A simple, purely python, WikiText parsing tool.
 Home-page: https://github.com/5j9/wikitextparser
 Author: 5j9
 Author-email: 5j9@users.noreply.github.com
 License: GNU General Public License v3 (GPLv3)
 Description: .. image:: https://travis-ci.org/5j9/wikitextparser.svg?branch=master
             :target: https://travis-ci.org/5j9/wikitextparser
```

### Comparing `wikitextparser-0.9.0.dev1/wikitextparser.egg-info/SOURCES.txt` & `wikitextparser-0.9.1/wikitextparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

