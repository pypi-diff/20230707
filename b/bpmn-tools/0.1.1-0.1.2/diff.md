# Comparing `tmp/bpmn-tools-0.1.1.tar.gz` & `tmp/bpmn-tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpmn-tools-0.1.1.tar", last modified: Sun Jun 25 08:14:28 2023, max compression
+gzip compressed data, was "bpmn-tools-0.1.2.tar", last modified: Fri Jul  7 10:06:04 2023, max compression
```

## Comparing `bpmn-tools-0.1.1.tar` & `bpmn-tools-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.510932 bpmn-tools-0.1.1/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.506826 bpmn-tools-0.1.1/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.1/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-06-25 08:14:28.510821 bpmn-tools-0.1.1/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.507771 bpmn-tools-0.1.1/bpmn_tools/
--rw-r--r--   0 xtof       (501) staff       (20)       91 2023-06-25 08:13:25.000000 bpmn-tools-0.1.1/bpmn_tools/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-06-25 07:47:11.000000 bpmn-tools-0.1.1/bpmn_tools/collaboration.py
--rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.1/bpmn_tools/colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     6325 2023-05-31 09:17:36.000000 bpmn-tools-0.1.1/bpmn_tools/diagrams.py
--rw-r--r--   0 xtof       (501) staff       (20)     7094 2023-06-25 08:11:42.000000 bpmn-tools-0.1.1/bpmn_tools/flow.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.508583 bpmn-tools-0.1.1/bpmn_tools/layout/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.1/bpmn_tools/layout/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     4430 2023-05-31 09:03:53.000000 bpmn-tools-0.1.1/bpmn_tools/layout/simple.py
--rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-06-25 08:13:52.000000 bpmn-tools-0.1.1/bpmn_tools/notation.py
--rw-r--r--   0 xtof       (501) staff       (20)      744 2023-05-31 09:05:57.000000 bpmn-tools-0.1.1/bpmn_tools/util.py
--rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.1/bpmn_tools/visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-05-31 07:52:16.000000 bpmn-tools-0.1.1/bpmn_tools/xml.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.508408 bpmn-tools-0.1.1/bpmn_tools.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      703 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       48 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       24 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       22 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/top_level.txt
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.508763 bpmn-tools-0.1.1/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/docs/conf.py
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-25 08:14:28.510970 bpmn-tools-0.1.1/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.1/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.510525 bpmn-tools-0.1.1/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.1/tests/test_colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.1/tests/test_flows.py
--rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.1/tests/test_hello.py
--rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.1/tests/test_lanes.py
--rw-r--r--   0 xtof       (501) staff       (20)     1133 2023-05-31 08:58:08.000000 bpmn-tools-0.1.1/tests/test_roundtrip.py
--rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.1/tests/test_visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.1/tests/test_xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.923704 bpmn-tools-0.1.2/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.920544 bpmn-tools-0.1.2/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.2/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 10:06:04.923597 bpmn-tools-0.1.2/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.921444 bpmn-tools-0.1.2/bpmn_tools/
+-rw-r--r--   0 xtof       (501) staff       (20)       91 2023-07-07 10:05:15.000000 bpmn-tools-0.1.2/bpmn_tools/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-06-25 07:47:11.000000 bpmn-tools-0.1.2/bpmn_tools/collaboration.py
+-rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.2/bpmn_tools/colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     6325 2023-07-07 10:03:27.000000 bpmn-tools-0.1.2/bpmn_tools/diagrams.py
+-rw-r--r--   0 xtof       (501) staff       (20)     7799 2023-07-07 09:17:18.000000 bpmn-tools-0.1.2/bpmn_tools/flow.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.922418 bpmn-tools-0.1.2/bpmn_tools/layout/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.2/bpmn_tools/layout/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4607 2023-07-07 10:00:11.000000 bpmn-tools-0.1.2/bpmn_tools/layout/simple.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-06-25 08:13:52.000000 bpmn-tools-0.1.2/bpmn_tools/notation.py
+-rw-r--r--   0 xtof       (501) staff       (20)      865 2023-07-07 09:23:39.000000 bpmn-tools-0.1.2/bpmn_tools/util.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.2/bpmn_tools/visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-07-07 10:03:09.000000 bpmn-tools-0.1.2/bpmn_tools/xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.922186 bpmn-tools-0.1.2/bpmn_tools.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      703 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       48 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       24 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/top_level.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.922635 bpmn-tools-0.1.2/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/docs/conf.py
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-07-07 10:06:04.923739 bpmn-tools-0.1.2/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.2/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.923432 bpmn-tools-0.1.2/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.2/tests/test_colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.2/tests/test_flows.py
+-rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.2/tests/test_hello.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.2/tests/test_lanes.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1275 2023-07-07 09:43:06.000000 bpmn-tools-0.1.2/tests/test_roundtrip.py
+-rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.2/tests/test_visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.2/tests/test_xml.py
```

### Comparing `bpmn-tools-0.1.1/.github/README.md` & `bpmn-tools-0.1.2/.github/README.md`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/LICENSE.txt` & `bpmn-tools-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/PKG-INFO` & `bpmn-tools-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.1/bpmn_tools/collaboration.py` & `bpmn-tools-0.1.2/bpmn_tools/collaboration.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/bpmn_tools/colors.py` & `bpmn-tools-0.1.2/bpmn_tools/colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/bpmn_tools/diagrams.py` & `bpmn-tools-0.1.2/bpmn_tools/diagrams.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/bpmn_tools/flow.py` & `bpmn-tools-0.1.2/bpmn_tools/flow.py`

 * *Files 11% similar despite different names*

```diff
@@ -105,24 +105,51 @@
     children = []
     if self.incoming:
       children.extend([ flow for flow in self.incoming ])
     if self.outgoing:
       children.extend([ flow for flow in self.outgoing ])
     return children
 
+class MessageEventDefinition(IdentifiedElement):
+  __tag__ = "bpmn:messageEventDefinition"
+
 class Event(Element):
   __labeled__ = False
-  def __init__(self, **kwargs):
+
+  def __init__(self, name=None, message=False, **kwargs):
     super().__init__(**kwargs)
-    self.width  = 36
-    self.height = 36
+    self.width   = 36
+    self.height  = 36
+    if name:
+      self["name"] = name
+    self.message = message
+
+  def append(self, child):
+    if type(child) == MessageEventDefinition:
+      self.message = True
+    else:
+      super().append(child) # something else
+    return self
+
+  @property
+  def children(self):
+    children = super().children
+    if self.message:
+      children.append(MessageEventDefinition(id=f"MessageEventDefinition_{self['id']}"))
+    return children
 
 class Start(Event):
   __tag__    = "bpmn:startEvent"
 
+class IntermediateThrow(Event):
+  __tag__ = "bpmn:intermediateThrowEvent"
+
+class IntermediateCatch(Event):
+  __tag__ = "bpmn:intermediateCatchEvent"
+
 class End(Event):
   __tag__ = "bpmn:endEvent"
 
 class Task(Element):
   __tag__     = "bpmn:task"
 
   def __init__(self, name="", **kwargs):
```

### Comparing `bpmn-tools-0.1.1/bpmn_tools/layout/simple.py` & `bpmn-tools-0.1.2/bpmn_tools/layout/simple.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 import json
 
 from bpmn_tools.flow          import Process, Start, End
+from bpmn_tools.flow          import IntermediateCatch, IntermediateThrow
 from bpmn_tools.flow          import Task, UserTask, ServiceTask, ScriptTask
 from bpmn_tools.collaboration import Participant
 from bpmn_tools.visitor       import Visitor, visiting
 
 class LayoutVisitor(Visitor):
   def __init__(self):
     super().__init__()
@@ -36,14 +37,18 @@
     self.process_participant[participant.process.id] = participant
   
   @visiting(Start)
   def visit(self, event):
     self.current_process["start"] = event
     self._analyse_element(event)
 
+  @visiting(IntermediateThrow, IntermediateCatch)
+  def visit(self, event):
+    self._analyse_element(event)
+
   @visiting(End)
   def visit(self, event):
     self.current_process["end"] = event
     self._analyse_element (event)
 
   @visiting(Task, UserTask, ServiceTask, ScriptTask)
   def visit(self, task):
@@ -112,22 +117,24 @@
       width = left - START
       self.process_participant[process].width = width
       for lane in analysis["process"].laneset.lanes:
         lane.width  = width - HEADER
       top += self.process_participant[process].height
 
   def _order(self, analysis):
-    if analysis["start"] and analysis["end"]:
-      # follow from start to end
+    if analysis["start"]:
+      # follow from start to ...
       step = analysis["start"]
-      end  = analysis["end"]
       yield step
-      while step != end:
-        step = analysis["elements"][analysis["steps"][step.id][0]]
-        yield step
+      while True:
+        try:
+          step = analysis["elements"][analysis["steps"][step.id][0]]
+          yield step
+        except:
+          break
     else:
       # just return the elements
       if analysis["start"]:
         yield analysis["start"]
       for element in analysis["elements"].values():
         yield element
       if analysis["end"]:
```

### Comparing `bpmn-tools-0.1.1/bpmn_tools/notation.py` & `bpmn-tools-0.1.2/bpmn_tools/notation.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/bpmn_tools/util.py` & `bpmn-tools-0.1.2/bpmn_tools/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,11 +14,14 @@
   expected = json.dumps(expected, indent=2, sort_keys=True, default=as_dict)
   diff = unified_diff(expected.splitlines(keepends=True),
                       result.splitlines(keepends=True),
                       fromfile="expected", tofile="result")
   print("".join(diff), end="")
 
 def compare(result, expected):
+  print("=" * 20, "result dict", "=" * 20)
   print(json.dumps(result, indent=2))
+  print("=" * 20, "result XML", "=" * 20)
   print(xmltodict.unparse(result, pretty=True))
+  print("=" * 20, "diff", "=" * 20)
   show_diff(result, expected)
   assert result == expected
```

### Comparing `bpmn-tools-0.1.1/bpmn_tools/visitor.py` & `bpmn-tools-0.1.2/bpmn_tools/visitor.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/bpmn_tools/xml.py` & `bpmn-tools-0.1.2/bpmn_tools/xml.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/bpmn_tools.egg-info/PKG-INFO` & `bpmn-tools-0.1.2/bpmn_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.1/bpmn_tools.egg-info/SOURCES.txt` & `bpmn-tools-0.1.2/bpmn_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/docs/conf.py` & `bpmn-tools-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/setup.py` & `bpmn-tools-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/tests/test_colors.py` & `bpmn-tools-0.1.2/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/tests/test_flows.py` & `bpmn-tools-0.1.2/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/tests/test_hello.py` & `bpmn-tools-0.1.2/tests/test_hello.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/tests/test_lanes.py` & `bpmn-tools-0.1.2/tests/test_lanes.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.1/tests/test_roundtrip.py` & `bpmn-tools-0.1.2/tests/test_roundtrip.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,7 +38,11 @@
 def test_hello_lanes_with_message():
   with open(Path(__file__).resolve().parent / "hello-lanes-with-message.bpmn") as fp:
     compare_with_roundtrip(fp.read())
 
 def test_hello_colors():
   with open(Path(__file__).resolve().parent / "hello-colors.bpmn") as fp:
     compare_with_roundtrip(fp.read())
+
+def test_message_events():
+  with open(Path(__file__).resolve().parent / "message-events.bpmn") as fp:
+    compare_with_roundtrip(fp.read())
```

### Comparing `bpmn-tools-0.1.1/tests/test_visitor.py` & `bpmn-tools-0.1.2/tests/test_visitor.py`

 * *Files identical despite different names*

