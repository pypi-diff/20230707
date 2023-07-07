# Comparing `tmp/Perdy-1.8.tar.gz` & `tmp/Perdy-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Perdy-1.8.tar", last modified: Mon Oct 19 10:02:10 2020, max compression
+gzip compressed data, was "dist/Perdy-1.9.tar", last modified: Tue Nov 17 05:29:51 2020, max compression
```

## Comparing `Perdy-1.8.tar` & `Perdy-1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-10-19 10:02:10.552619 Perdy-1.8/
--rw-r--r--   0 dave       (501) staff       (20)      334 2020-10-19 10:02:10.552749 Perdy-1.8/PKG-INFO
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-10-19 10:02:10.549009 Perdy-1.8/Perdy/
--rwxr-xr-x   0 dave       (501) staff       (20)     1270 2020-04-16 02:11:31.000000 Perdy-1.8/Perdy/PrettyYAML.py
--rwxr-xr-x   0 dave       (501) staff       (20)        0 2020-04-16 02:11:31.000000 Perdy-1.8/Perdy/__init__.py
--rwxr-xr-x   0 dave       (501) staff       (20)     2372 2020-04-16 02:11:31.000000 Perdy-1.8/Perdy/diff.py
--rwxr-xr-x   0 dave       (501) staff       (20)      512 2020-03-26 03:35:55.000000 Perdy-1.8/Perdy/eddo.py
--rwxr-xr-x   0 dave       (501) staff       (20)    11898 2020-04-16 02:11:31.000000 Perdy-1.8/Perdy/parser.py
--rwxr-xr-x   0 dave       (501) staff       (20)    12861 2020-10-19 10:01:24.000000 Perdy-1.8/Perdy/pretty.py
--rwxr-xr-x   0 dave       (501) staff       (20)     4749 2020-03-26 03:35:55.000000 Perdy-1.8/Perdy/pyson.py
--rwxr-xr-x   0 dave       (501) staff       (20)      931 2020-03-26 03:35:55.000000 Perdy-1.8/Perdy/pyxbext.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-10-19 10:02:10.550916 Perdy-1.8/Perdy.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      334 2020-10-19 10:02:10.000000 Perdy-1.8/Perdy.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      346 2020-10-19 10:02:10.000000 Perdy-1.8/Perdy.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2020-10-19 10:02:10.000000 Perdy-1.8/Perdy.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       64 2020-10-19 10:02:10.000000 Perdy-1.8/Perdy.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)        6 2020-10-19 10:02:10.000000 Perdy-1.8/Perdy.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       22 2020-02-14 10:30:04.000000 Perdy-1.8/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-10-19 10:02:10.552131 Perdy-1.8/bin/
--rwxr-xr-x   0 dave       (501) staff       (20)     3323 2020-03-26 03:35:55.000000 Perdy-1.8/bin/colourize.py
--rwxr-xr-x   0 dave       (501) staff       (20)     4208 2020-03-26 03:35:55.000000 Perdy-1.8/bin/parser.py
--rwxr-xr-x   0 dave       (501) staff       (20)     4748 2020-03-26 03:35:55.000000 Perdy-1.8/bin/pyson.py
--rw-r--r--   0 dave       (501) staff       (20)       79 2020-10-19 10:02:10.553233 Perdy-1.8/setup.cfg
--rwxr-xr-x   0 dave       (501) staff       (20)      818 2020-10-19 09:53:05.000000 Perdy-1.8/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-11-17 05:29:51.285420 Perdy-1.9/
+-rw-r--r--   0 dave       (501) staff       (20)      334 2020-11-17 05:29:51.285520 Perdy-1.9/PKG-INFO
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-11-17 05:29:51.282987 Perdy-1.9/Perdy/
+-rwxr-xr-x   0 dave       (501) staff       (20)     1270 2020-04-16 02:11:31.000000 Perdy-1.9/Perdy/PrettyYAML.py
+-rwxr-xr-x   0 dave       (501) staff       (20)        0 2020-04-16 02:11:31.000000 Perdy-1.9/Perdy/__init__.py
+-rwxr-xr-x   0 dave       (501) staff       (20)     2372 2020-04-16 02:11:31.000000 Perdy-1.9/Perdy/diff.py
+-rwxr-xr-x   0 dave       (501) staff       (20)      512 2020-03-26 03:35:55.000000 Perdy-1.9/Perdy/eddo.py
+-rwxr-xr-x   0 dave       (501) staff       (20)    11898 2020-04-16 02:11:31.000000 Perdy-1.9/Perdy/parser.py
+-rwxr-xr-x   0 dave       (501) staff       (20)    13022 2020-11-17 05:24:05.000000 Perdy-1.9/Perdy/pretty.py
+-rwxr-xr-x   0 dave       (501) staff       (20)     4749 2020-03-26 03:35:55.000000 Perdy-1.9/Perdy/pyson.py
+-rwxr-xr-x   0 dave       (501) staff       (20)      931 2020-03-26 03:35:55.000000 Perdy-1.9/Perdy/pyxbext.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-11-17 05:29:51.284203 Perdy-1.9/Perdy.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      334 2020-11-17 05:29:51.000000 Perdy-1.9/Perdy.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      346 2020-11-17 05:29:51.000000 Perdy-1.9/Perdy.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2020-11-17 05:29:51.000000 Perdy-1.9/Perdy.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       64 2020-11-17 05:29:51.000000 Perdy-1.9/Perdy.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)        6 2020-11-17 05:29:51.000000 Perdy-1.9/Perdy.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       22 2020-02-14 10:30:04.000000 Perdy-1.9/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2020-11-17 05:29:51.285216 Perdy-1.9/bin/
+-rwxr-xr-x   0 dave       (501) staff       (20)     3323 2020-03-26 03:35:55.000000 Perdy-1.9/bin/colourize.py
+-rwxr-xr-x   0 dave       (501) staff       (20)     4208 2020-03-26 03:35:55.000000 Perdy-1.9/bin/parser.py
+-rwxr-xr-x   0 dave       (501) staff       (20)     4748 2020-03-26 03:35:55.000000 Perdy-1.9/bin/pyson.py
+-rw-r--r--   0 dave       (501) staff       (20)       79 2020-11-17 05:29:51.285883 Perdy-1.9/setup.cfg
+-rwxr-xr-x   0 dave       (501) staff       (20)      818 2020-11-17 05:20:59.000000 Perdy-1.9/setup.py
```

### Comparing `Perdy-1.8/Perdy/PrettyYAML.py` & `Perdy-1.9/Perdy/PrettyYAML.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/Perdy/diff.py` & `Perdy-1.9/Perdy/diff.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/Perdy/eddo.py` & `Perdy-1.9/Perdy/eddo.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/Perdy/parser.py` & `Perdy-1.9/Perdy/parser.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/Perdy/pretty.py` & `Perdy-1.9/Perdy/pretty.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,24 +163,26 @@
 				self.prettify(d[key], indent='%s  '%indent, parent=d)
 								
 				if self.style == Style.YAML:
 					if i < (len(keys)-1):
 						self.output.write('\n')
 						if type(parent) == list:
 							self.output.write(indent[:-2])
+							
 				if self.style == Style.XML:
 					self.output.write(''.join([
 						self.colours.Off,
-						'%s  '%indent,
+						#'%s  '%indent,
 						'</',
 						self.colours.Teal,
 						'%s'%key,
 						self.colours.Off,
 						'>\n',
 					]))
+					
 				if self.style == Style.JSON:
 					if i < (len(keys) - 1):
 						self.output.write(',')
 					self.output.write('\n')
 					
 			if self.style == Style.JSON:
 				self.output.write('%s'%indent)
@@ -234,15 +236,20 @@
 				if self.style == Style.JSON:
 					self.output.write('"')
 				self.output.write(self.colours.Red)
 				_new = '%s'%d.replace('\r','\\r').replace('\n','\\n')
 				
 				if self.style == Style.JSON:
 					_new = _new.replace('"','\\"')
-				
+
+				if self.style == Style.XML:
+					_new = _new.replace('&','&amp;')
+					_new = _new.replace('>','&gt;')
+					_new = _new.replace('<','&lt;')
+					
 				self.output.write(_new)
 				self.output.write(self.colours.Off)
 				if self.style == Style.JSON and len(self.walked) == 0:
 						self.output.write('"')
 
 		#........................................................
 		elif \
```

### Comparing `Perdy-1.8/Perdy/pyson.py` & `Perdy-1.9/Perdy/pyson.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/Perdy/pyxbext.py` & `Perdy-1.9/Perdy/pyxbext.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/bin/colourize.py` & `Perdy-1.9/bin/colourize.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/bin/parser.py` & `Perdy-1.9/bin/parser.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/bin/pyson.py` & `Perdy-1.9/bin/pyson.py`

 * *Files identical despite different names*

### Comparing `Perdy-1.8/setup.py` & `Perdy-1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 from setuptools import setup
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
     long_description = input.read()
 
-version='1.8'
+version='1.9'
 	
 setup(
 	name='Perdy',
 	version=version,
 	license='MIT',
     long_description=long_description,
 	long_description_content_type="text/markdown",
```

