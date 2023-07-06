# Comparing `tmp/capparser-1.0.0.tar.gz` & `tmp/capparser-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capparser-1.0.0.tar", last modified: Fri Dec 23 19:52:02 2022, max compression
+gzip compressed data, was "capparser-2.0.4.tar", last modified: Thu Jul  6 22:31:10 2023, max compression
```

## Comparing `capparser-1.0.0.tar` & `capparser-2.0.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)        0 2022-12-23 19:52:02.090787 capparser-1.0.0/
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)     1108 2022-12-21 00:16:55.000000 capparser-1.0.0/LICENSE
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)      433 2022-12-23 19:52:02.084788 capparser-1.0.0/PKG-INFO
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)       43 2022-12-23 19:28:02.000000 capparser-1.0.0/README.md
-drwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)        0 2022-12-23 19:52:01.764104 capparser-1.0.0/capparser/
-drwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)        0 2022-12-23 19:52:01.856756 capparser-1.0.0/capparser/src/
-drwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)        0 2022-12-23 19:52:02.036923 capparser-1.0.0/capparser/src/capparser.egg-info/
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)      433 2022-12-23 19:52:01.000000 capparser-1.0.0/capparser/src/capparser.egg-info/PKG-INFO
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)      241 2022-12-23 19:52:01.000000 capparser-1.0.0/capparser/src/capparser.egg-info/SOURCES.txt
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)        1 2022-12-23 19:52:01.000000 capparser-1.0.0/capparser/src/capparser.egg-info/dependency_links.txt
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)       10 2022-12-23 19:52:01.000000 capparser-1.0.0/capparser/src/capparser.egg-info/top_level.txt
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)     3430 2022-12-23 15:53:22.000000 capparser-1.0.0/capparser/src/capparser.py
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)       38 2022-12-23 19:52:02.091785 capparser-1.0.0/setup.cfg
--rwxrwxrwx   0 wsl-david  (1000) wsl-david  (1000)      700 2022-12-23 19:26:54.000000 capparser-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:31:10.312757 capparser-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 22:30:57.000000 capparser-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-06 22:31:10.312757 capparser-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-06 22:30:57.000000 capparser-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:31:10.312757 capparser-2.0.4/capparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 22:30:57.000000 capparser-2.0.4/capparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-06 22:30:57.000000 capparser-2.0.4/capparser/capparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31736 2023-07-06 22:30:57.000000 capparser-2.0.4/capparser/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 22:30:57.000000 capparser-2.0.4/capparser/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:31:10.312757 capparser-2.0.4/capparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-06 22:31:10.000000 capparser-2.0.4/capparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-06 22:31:10.000000 capparser-2.0.4/capparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:31:10.000000 capparser-2.0.4/capparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 22:31:10.000000 capparser-2.0.4/capparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:31:10.312757 capparser-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 22:30:57.000000 capparser-2.0.4/setup.py
```

### Comparing `capparser-1.0.0/capparser/src/capparser.py` & `capparser-2.0.4/capparser/capparser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,88 @@
-import element
-import enums
-import xml.etree.ElementTree as ET
-import inspect
-
-def parse(filePath=None, stringXML=None):
-    if filePath != None:
-        file = open(filePath, "r")
-        stringXML = file.read()
-        file.close()
-    root = ET.fromstring(stringXML)
-    return _recursiveParser(root)
-
-
-def _recursiveParser(parent):
-    _, _, tagName = parent.tag.rpartition('}')
-    obj = None
-    if(tagName == str(element.Alert())):
-        obj = element.Alert()
-    elif(tagName == str(element.Info())):
-        obj = element.Info()
-    elif(tagName == str(element.EventCode())):
-        obj = element.EventCode()
-    elif(tagName == str(element.Parameter())):
-        obj = element.Parameter()
-    elif(tagName == str(element.Resource())):
-        obj = element.Resource()
-    elif(tagName == str(element.Area())):
-        obj = element.Area()
-    elif(tagName == str(element.Geocode())):
-        obj = element.Geocode()
-    else:
-        return None
-
-    for child in parent:
-        _, _, childTagName = child.tag.rpartition('}')
-        if len(child) == 0:
-            for attr in inspect.getmembers(obj):
-                if attr[0] == childTagName:
-                    if len(parent.findall(child.tag)) == 1:
-                        setattr(obj, childTagName, (child.text, attr[1][1]))
-                    else:
-                        getattr(obj, childTagName)[0].append(child.text)
-        else:
-            getattr(obj, childTagName)[0].append(_recursiveParser(child))
-
-    return obj
-
-def deparse(alert):
-    return ET.tostring(_recursiveDeparser(alert), encoding='utf8')
-
-def writeAlertToFile(alert, filePath):
-    root = _recursiveDeparser(alert)
-    tree = ET.ElementTree(root)
-    with open(filePath, "wb") as files:
-        tree.write(files)
-
-def _recursiveDeparser(obj, outputFilePath=None):
-    root = ET.Element(str(obj))
-    attrs = _filterOrderAttributes(inspect.getmembers(obj))
-    for attr in attrs:
-        if attr[0] == "xmlns":
-            root.set(attr[0], attr[1][0])
-        elif isinstance(attr[1][0], list):
-            for item in attr[1][0]:
-                if isinstance(item, element.Alert) or isinstance(item, element.Info) or isinstance(item, element.EventCode) or isinstance(item, element.Parameter) or isinstance(item, element.Resource) or isinstance(item, element.Area) or isinstance(item, element.Geocode):
-                    root.append(_recursiveDeparser(item))
-                else:
-                    child = ET.SubElement(root, attr[0])
-                    child.text = item
-        else:
-            if isinstance(attr[1][0], element.Alert) or isinstance(attr[1][0], element.Info) or isinstance(attr[1][0], element.EventCode) or isinstance(attr[1][0], element.Parameter) or isinstance(attr[1][0], element.Resource) or isinstance(attr[1][0], element.Area) or isinstance(attr[1][0], element.Geocode):
-                root.append(_recursiveDeparser(attr[1][0]))
-            else:
-                child = ET.SubElement(root, attr[0])
-                child.text = attr[1][0]
-    return root
-
-
-def _filterOrderAttributes(attrs):
-    result = []
-    for attr in attrs:
-        if not attr[0].startswith('_') and not inspect.ismethod(attr[1]) and len(attr[1]) == 2 and attr[1][0] != None and attr[0] != []:
-            result.append(attr)
-    result.sort(key=lambda x: x[1][1])
-    return result
+from . import element
+from . import enums
+import xml.etree.ElementTree as ET
+import inspect
+
+def parse(filePath=None, stringXML=None):
+    if filePath != None:
+        file = open(filePath, "r")
+        stringXML = file.read()
+        file.close()
+    root = ET.fromstring(stringXML)
+    return _recursiveParser(root)
+
+
+def _recursiveParser(parent):
+    _, _, tagName = parent.tag.rpartition('}')
+    obj = None
+    if(tagName == str(element.Alert())):
+        obj = element.Alert()
+    elif(tagName == str(element.Info())):
+        obj = element.Info()
+    elif(tagName == str(element.EventCode())):
+        obj = element.EventCode()
+    elif(tagName == str(element.Parameter())):
+        obj = element.Parameter()
+    elif(tagName == str(element.Resource())):
+        obj = element.Resource()
+    elif(tagName == str(element.Area())):
+        obj = element.Area()
+    elif(tagName == str(element.Geocode())):
+        obj = element.Geocode()
+    else:
+        return None
+
+    for child in parent:
+        _, _, childTagName = child.tag.rpartition('}')
+        if len(child) == 0:
+            for attr in inspect.getmembers(obj):
+                if attr[0] == childTagName:
+                    if len(parent.findall(child.tag)) == 1:
+                        setattr(obj, childTagName, (child.text, attr[1][1]))
+                    else:
+                        getattr(obj, childTagName)[0].append(child.text)
+        else:
+            getattr(obj, childTagName)[0].append(_recursiveParser(child))
+
+    return obj
+
+def deparse(alert):
+    return ET.tostring(_recursiveDeparser(alert), encoding='utf8')
+
+def writeAlertToFile(alert, filePath):
+    root = _recursiveDeparser(alert)
+    tree = ET.ElementTree(root)
+    with open(filePath, "wb") as files:
+        tree.write(files)
+
+def _recursiveDeparser(obj):
+    root = ET.Element(str(obj))
+    attrs = _filterOrderAttributes(inspect.getmembers(obj))
+    
+    for attr in attrs:
+        if attr[0] == "xmlns":
+            root.set(attr[0], attr[1][0])
+        elif isinstance(attr[1][0], list):
+            for item in attr[1][0]:
+                if isinstance(item, element.Alert) or isinstance(item, element.Info) or isinstance(item, element.EventCode) or isinstance(item, element.Parameter) or isinstance(item, element.Resource) or isinstance(item, element.Area) or isinstance(item, element.Geocode):
+                    root.append(_recursiveDeparser(item))
+                else:
+                    child = ET.SubElement(root, attr[0])
+                    child.text = str(item)
+        else:
+            if isinstance(attr[1][0], element.Alert) or isinstance(attr[1][0], element.Info) or isinstance(attr[1][0], element.EventCode) or isinstance(attr[1][0], element.Parameter) or isinstance(attr[1][0], element.Resource) or isinstance(attr[1][0], element.Area) or isinstance(attr[1][0], element.Geocode):
+                root.append(_recursiveDeparser(attr[1][0]))
+            else:
+                child = ET.SubElement(root, attr[0])
+                child.text = str(attr[1][0])
+                
+    return root
+
+
+def _filterOrderAttributes(attrs):
+    result = []
+    for attr in attrs:
+        if not attr[0].startswith('_') and not inspect.ismethod(attr[1]) and len(attr[1]) == 2 and attr[1][0] != None and attr[0] != []:
+            result.append(attr)
+    result.sort(key=lambda x: x[1][1])
+    return result
```

