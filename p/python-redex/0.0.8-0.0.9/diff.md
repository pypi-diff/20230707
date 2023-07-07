# Comparing `tmp/python_redex-0.0.8.tar.gz` & `tmp/python_redex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_redex-0.0.8.tar", last modified: Sun Jul  2 21:14:42 2023, max compression
+gzip compressed data, was "python_redex-0.0.9.tar", last modified: Fri Jul  7 17:48:24 2023, max compression
```

## Comparing `python_redex-0.0.8.tar` & `python_redex-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 21:14:42.004934 python_redex-0.0.8/
--rw-rw-rw-   0        0        0      596 2023-07-02 21:13:23.000000 python_redex-0.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.8/LICENCE.txt
--rw-rw-rw-   0        0        0       27 2023-07-02 16:36:53.000000 python_redex-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      635 2023-07-02 21:14:42.004934 python_redex-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 21:14:41.955186 python_redex-0.0.8/python_redex.egg-info/
--rw-rw-rw-   0        0        0      635 2023-07-02 21:14:41.000000 python_redex-0.0.8/python_redex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-07-02 21:14:41.000000 python_redex-0.0.8/python_redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 21:14:41.000000 python_redex-0.0.8/python_redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 21:14:41.000000 python_redex-0.0.8/python_redex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 21:14:41.984507 python_redex-0.0.8/redex/
--rw-rw-rw-   0        0        0     1520 2023-07-02 21:05:59.000000 python_redex-0.0.8/redex/__init__.py
--rw-rw-rw-   0        0        0     2452 2023-07-02 21:02:26.000000 python_redex-0.0.8/redex/action.py
--rw-rw-rw-   0        0        0     2207 2023-07-02 21:02:41.000000 python_redex-0.0.8/redex/lexical_analysis.py
--rw-rw-rw-   0        0        0      581 2023-07-02 15:01:38.000000 python_redex-0.0.8/redex/split.py
--rw-rw-rw-   0        0        0      559 2023-07-02 15:02:16.000000 python_redex-0.0.8/redex/wildcards.py
-drwxrwxrwx   0        0        0        0 2023-07-02 21:14:41.998292 python_redex-0.0.8/redex.egg-info/
--rw-rw-rw-   0        0        0      177 2023-07-02 15:53:02.000000 python_redex-0.0.8/redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:53:02.000000 python_redex-0.0.8/redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 15:53:02.000000 python_redex-0.0.8/redex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 21:14:42.004934 python_redex-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-07-02 21:14:19.000000 python_redex-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:48:24.069587 python_redex-0.0.9/
+-rw-rw-rw-   0        0        0      596 2023-07-02 21:13:23.000000 python_redex-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.9/LICENCE.txt
+-rw-rw-rw-   0        0        0       27 2023-07-02 16:36:53.000000 python_redex-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      635 2023-07-07 17:48:24.068201 python_redex-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 17:48:23.995898 python_redex-0.0.9/python_redex.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-07-07 17:48:23.000000 python_redex-0.0.9/python_redex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-07-07 17:48:23.000000 python_redex-0.0.9/python_redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:48:23.000000 python_redex-0.0.9/python_redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 17:48:23.000000 python_redex-0.0.9/python_redex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 17:48:24.047088 python_redex-0.0.9/redex/
+-rw-rw-rw-   0        0        0     1775 2023-07-07 17:47:58.000000 python_redex-0.0.9/redex/__init__.py
+-rw-rw-rw-   0        0        0     2473 2023-07-07 17:46:24.000000 python_redex-0.0.9/redex/action.py
+-rw-rw-rw-   0        0        0     2207 2023-07-07 17:46:49.000000 python_redex-0.0.9/redex/lexical_analysis.py
+-rw-rw-rw-   0        0        0      581 2023-07-02 15:01:38.000000 python_redex-0.0.9/redex/split.py
+-rw-rw-rw-   0        0        0      559 2023-07-02 15:02:16.000000 python_redex-0.0.9/redex/wildcards.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:48:24.065409 python_redex-0.0.9/redex.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-07-02 15:53:02.000000 python_redex-0.0.9/redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:53:02.000000 python_redex-0.0.9/redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 15:53:02.000000 python_redex-0.0.9/redex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:48:24.069587 python_redex-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-07-07 17:42:25.000000 python_redex-0.0.9/setup.py
```

### Comparing `python_redex-0.0.8/CHANGELOG.txt` & `python_redex-0.0.9/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.8/LICENCE.txt` & `python_redex-0.0.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.8/PKG-INFO` & `python_redex-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_redex
-Version: 0.0.8
+Version: 0.0.9
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-0.0.8/python_redex.egg-info/PKG-INFO` & `python_redex-0.0.9/python_redex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redex
-Version: 0.0.8
+Version: 0.0.9
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-0.0.8/redex/__init__.py` & `python_redex-0.0.9/redex/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,43 @@
 # local imports
 
 from redex.lexical_analysis import *
 from redex.split import *
 
 # main functionalities
 
-def has(query, string, split=' ', granularity=1, threads=2):
+def has(query, string, split=' ', granularity=1, threads=2) -> bool:
     search = RedexSearch(query, string, split=split, granularity=granularity, threads=threads)
     search.parse_query()
     if True in search.get_result():
         return True
     else:
         return False
 
-def find(query, string, split=' ', granularity=1, format='string', threads=2):
+def find(query, string, split=' ', granularity=1, format='string', threads=2) -> list:
     search = RedexSearch(query, string, split=split, granularity=granularity, threads=threads)
     search.parse_query()
     locations = []
     for index, location in enumerate(redex_split(string, split, granularity)):
         if search.get_result()[index] and format == 'int':
             locations.append(index)
         elif search.get_result()[index] and format == 'string':
             locations.append(location)
         elif search.get_result()[index] and format == 'tuple':
             locations.append((index, location))
     return locations
 
-def info():
-    print('\n---')
-    print('    ^ ^          Description:        Python library for readable regex.')
-    print('("\(-_-)/")      Version:            0.0.8') 
-    print(' )(  O  )(       Author:             Timo Kats')
-    print('((...)(...))     Last updated:       02/07/2023', end='\n---\n\n')
+def count(query, string, split=' ', granularity=1, threads=2) -> int:
+    search = RedexSearch(query, string, split=split, granularity=granularity, threads=threads)
+    search.parse_query()
+    count = 0
+    for substring in search.get_result():
+        if substring:
+            count += 1
+    return count
 
-if __name__ == '__main__':
-    print(find('endswith:*num', 'testing 4the test sete5'))
+def info():
+    print('\n')
+    print('  ;,//;,    ,;/      Description:        Python library for readable regex.')
+    print(' o:::::::;;///       Version:            0.0.9')
+    print('>::::::::;;\\\\\\       Author:             Timo Kats')
+    print('  "\\\\\\\\\\""  \';\      Last updated:       06/07/2023', end='\n\n\n')
```

### Comparing `python_redex-0.0.8/redex/action.py` & `python_redex-0.0.9/redex/action.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # local imports
 
 from redex.wildcards import *
 
 # helper functions
 
-def is_in(char, string):
+def is_in(char, string) -> bool:
     if char in wildcard.keys():
         for wchar in wildcard[char]:
             if wchar in string:
                 return True
     else:
         return char in string
 
@@ -44,33 +44,34 @@
 
 def proximity(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
     char_set = list(sub_query.split('}')[0][1:].split(','))
     threshold = int(sub_query.split('}')[1])
     max_proximity = -1
     for char in char_set:
-        proximity = abs(string.find(char)-string.find(char_set[0]))
+        proximity = abs(string.find(char) - string.find(char_set[0]))
         if is_in(char, string) and (max_proximity < proximity or max_proximity == -1):
             max_proximity = proximity
-        if char not in string:
+        if not is_in(char, string):
             return False
     return max_proximity <= threshold and max_proximity != -1
 
 def sequence(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
     sequence_list = list(sub_query[1:-1].split(','))
     current_index = 0
     for char in string:
-        if is_in(char, sequence_list[current_index]) and current_index < len(sequence_list) - 1:
+        if is_in(sequence_list[current_index], char) and current_index < len(sequence_list) - 1:
             current_index += 1
-        if sequence_list[current_index] not in string:
+        if not is_in(sequence_list[current_index], string):
             return False
     return current_index == len(sequence_list) - 1
 
 def location(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
     char = list(sub_query[1:-1].split(','))[0]
     location = int(list(sub_query[1:-1].split(','))[1])
     if location < len(string) - 1:
         return is_in(char, string[location])
     else:
         return False
+
```

### Comparing `python_redex-0.0.8/redex/lexical_analysis.py` & `python_redex-0.0.9/redex/lexical_analysis.py`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.8/redex/split.py` & `python_redex-0.0.9/redex/split.py`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.8/redex/wildcards.py` & `python_redex-0.0.9/redex/wildcards.py`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.8/setup.py` & `python_redex-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='python_redex',
-    version='0.0.8',
+    version='0.0.9',
     description='User friendly version of regex. More information available at https://github.com/TimoKats/redex',
     long_description='More information available at https://github.com/TimoKats/redex',
     url='',  
     author='Timo Kats',
     author_email='tpakats@gmail.com',
     license='MIT', 
     classifiers=classifiers,
```

