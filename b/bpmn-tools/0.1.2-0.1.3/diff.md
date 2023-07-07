# Comparing `tmp/bpmn-tools-0.1.2.tar.gz` & `tmp/bpmn-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpmn-tools-0.1.2.tar", last modified: Fri Jul  7 10:06:04 2023, max compression
+gzip compressed data, was "bpmn-tools-0.1.3.tar", last modified: Fri Jul  7 14:37:15 2023, max compression
```

## Comparing `bpmn-tools-0.1.2.tar` & `bpmn-tools-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.923704 bpmn-tools-0.1.2/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.920544 bpmn-tools-0.1.2/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.2/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 10:06:04.923597 bpmn-tools-0.1.2/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.921444 bpmn-tools-0.1.2/bpmn_tools/
--rw-r--r--   0 xtof       (501) staff       (20)       91 2023-07-07 10:05:15.000000 bpmn-tools-0.1.2/bpmn_tools/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-06-25 07:47:11.000000 bpmn-tools-0.1.2/bpmn_tools/collaboration.py
--rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.2/bpmn_tools/colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     6325 2023-07-07 10:03:27.000000 bpmn-tools-0.1.2/bpmn_tools/diagrams.py
--rw-r--r--   0 xtof       (501) staff       (20)     7799 2023-07-07 09:17:18.000000 bpmn-tools-0.1.2/bpmn_tools/flow.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.922418 bpmn-tools-0.1.2/bpmn_tools/layout/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.2/bpmn_tools/layout/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     4607 2023-07-07 10:00:11.000000 bpmn-tools-0.1.2/bpmn_tools/layout/simple.py
--rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-06-25 08:13:52.000000 bpmn-tools-0.1.2/bpmn_tools/notation.py
--rw-r--r--   0 xtof       (501) staff       (20)      865 2023-07-07 09:23:39.000000 bpmn-tools-0.1.2/bpmn_tools/util.py
--rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.2/bpmn_tools/visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-07-07 10:03:09.000000 bpmn-tools-0.1.2/bpmn_tools/xml.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.922186 bpmn-tools-0.1.2/bpmn_tools.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      703 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       48 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       24 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       22 2023-07-07 10:06:04.000000 bpmn-tools-0.1.2/bpmn_tools.egg-info/top_level.txt
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.922635 bpmn-tools-0.1.2/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/docs/conf.py
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-07-07 10:06:04.923739 bpmn-tools-0.1.2/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.2/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 10:06:04.923432 bpmn-tools-0.1.2/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.2/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.2/tests/test_colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.2/tests/test_flows.py
--rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.2/tests/test_hello.py
--rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.2/tests/test_lanes.py
--rw-r--r--   0 xtof       (501) staff       (20)     1275 2023-07-07 09:43:06.000000 bpmn-tools-0.1.2/tests/test_roundtrip.py
--rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.2/tests/test_visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.2/tests/test_xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.124358 bpmn-tools-0.1.3/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.121156 bpmn-tools-0.1.3/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.3/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 14:37:15.124243 bpmn-tools-0.1.3/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.122069 bpmn-tools-0.1.3/bpmn_tools/
+-rw-r--r--   0 xtof       (501) staff       (20)       91 2023-07-07 14:16:02.000000 bpmn-tools-0.1.3/bpmn_tools/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-06-25 07:47:11.000000 bpmn-tools-0.1.3/bpmn_tools/collaboration.py
+-rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.3/bpmn_tools/colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     6375 2023-07-07 14:28:39.000000 bpmn-tools-0.1.3/bpmn_tools/diagrams.py
+-rw-r--r--   0 xtof       (501) staff       (20)     8045 2023-07-07 14:09:04.000000 bpmn-tools-0.1.3/bpmn_tools/flow.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.123112 bpmn-tools-0.1.3/bpmn_tools/layout/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.3/bpmn_tools/layout/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4984 2023-07-07 14:04:06.000000 bpmn-tools-0.1.3/bpmn_tools/layout/simple.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-06-25 08:13:52.000000 bpmn-tools-0.1.3/bpmn_tools/notation.py
+-rw-r--r--   0 xtof       (501) staff       (20)      865 2023-07-07 09:23:39.000000 bpmn-tools-0.1.3/bpmn_tools/util.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.3/bpmn_tools/visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-07-07 10:03:09.000000 bpmn-tools-0.1.3/bpmn_tools/xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.122915 bpmn-tools-0.1.3/bpmn_tools.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      703 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       48 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       24 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/top_level.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.123314 bpmn-tools-0.1.3/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/docs/conf.py
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-07-07 14:37:15.124399 bpmn-tools-0.1.3/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.3/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.124066 bpmn-tools-0.1.3/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.3/tests/test_colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.3/tests/test_flows.py
+-rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.3/tests/test_hello.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.3/tests/test_lanes.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1275 2023-07-07 09:43:06.000000 bpmn-tools-0.1.3/tests/test_roundtrip.py
+-rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.3/tests/test_visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.3/tests/test_xml.py
```

### Comparing `bpmn-tools-0.1.2/.github/README.md` & `bpmn-tools-0.1.3/.github/README.md`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/LICENSE.txt` & `bpmn-tools-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/PKG-INFO` & `bpmn-tools-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.2/bpmn_tools/collaboration.py` & `bpmn-tools-0.1.3/bpmn_tools/collaboration.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/bpmn_tools/colors.py` & `bpmn-tools-0.1.3/bpmn_tools/colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/bpmn_tools/diagrams.py` & `bpmn-tools-0.1.3/bpmn_tools/diagrams.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,26 +123,28 @@
       })
     return attributes
 
   @property
   def children(self):
     children = super().children.copy()
     if self.flow:
-      if type(self.flow) == Flow:
+      below = self.flow.target.y > (self.flow.source.y + self.flow.source.height)
+      above = (self.flow.target.y + self.flow.target.height) < self.flow.source.y
+      if not (above or below): 
         children = [
           WayPoint(
             x=self.flow.source.x + self.flow.source.width,
             y=self.flow.source.y + int(self.flow.source.height/2)
           ),
           WayPoint(
             x=self.flow.target.x,
             y=self.flow.target.y + int(self.flow.target.height/2)
           )
         ]
-      elif type(self.flow) == MessageFlow:
+      else:
         if self.flow.source.y < self.flow.target.y:
           top     = self.flow.source
           bottom  = self.flow.target
           reverse = False
         else:
           top     = self.flow.target
           bottom  = self.flow.source
@@ -164,16 +166,14 @@
           WayPoint(
             x=bottom.x + int(bottom.width/2),
             y=bottom.y
           )
         ]
         if reverse:
           children.reverse()
-      else:
-        raise ValueError("unsupported flow type: {type(self.flow)}")
     return children
 
 class Plane(xml.Element):
   __tag__ = "bpmndi:BPMNPlane"
 
   def __init__(self, id="plane", element=None):
     super().__init__()
```

### Comparing `bpmn-tools-0.1.2/bpmn_tools/flow.py` & `bpmn-tools-0.1.3/bpmn_tools/flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -243,14 +243,20 @@
       super().append(child) # something else
     return self
 
   @property
   def children(self):
     return super().children + self.refs
 
+  def has_child(self, child):
+    for ref in self.refs:
+      if ref.ref == child:
+        return True
+    return False
+
 class LaneSet(IdentifiedElement):
   __tag__ = "bpmn:laneSet"
 
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     self.lanes = []
   
@@ -269,14 +275,20 @@
   def __len__(self):
     return len(self.lanes)
 
   @property
   def children(self):
     return super().children + self.lanes
 
+  def lane_of(self, child):
+    for lane in self.lanes:
+      if lane.has_child(child):
+        return lane
+    return None
+
 class Process(IdentifiedElement):
   __tag__ = "bpmn:process"
   
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     self.laneset = LaneSet(id=f"LaneSet_{self['id']}")
     self._elements = []
```

### Comparing `bpmn-tools-0.1.2/bpmn_tools/layout/simple.py` & `bpmn-tools-0.1.3/bpmn_tools/layout/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,24 +100,37 @@
     SPACING = 30
 
     top = 80
     for process, analysis in self.processes.items():
       left = START
       self.process_participant[process].x = left
       self.process_participant[process].y = top
-      for lane in analysis["process"].laneset.lanes:
-        lane.x = left + HEADER
-        lane.y = top
-        
+
+      if analysis["process"].laneset.lanes:
+        lanes_height = 0
+        for lane in analysis["process"].laneset.lanes:
+          lane.x = left + HEADER
+          lane.y = top + lanes_height
+          lanes_height += lane.height
+        self.process_participant[process].height = lanes_height
+      else:
+        pass
+
       left += HEADER + PADDING
       top += PADDING
+
       for step in self._order(analysis):
         step.x = left
-        step.y = top + (analysis["height"]-step.height) / 2
+        lane = analysis["process"].laneset.lane_of(step)
+        if lane:
+          step.y = PADDING + lane.y + (analysis["height"]-step.height) / 2
+        else:
+          step.y = top + (analysis["height"]-step.height) / 2
         left += step.width + SPACING
+
       width = left - START
       self.process_participant[process].width = width
       for lane in analysis["process"].laneset.lanes:
         lane.width  = width - HEADER
       top += self.process_participant[process].height
 
   def _order(self, analysis):
```

### Comparing `bpmn-tools-0.1.2/bpmn_tools/notation.py` & `bpmn-tools-0.1.3/bpmn_tools/notation.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/bpmn_tools/util.py` & `bpmn-tools-0.1.3/bpmn_tools/util.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/bpmn_tools/visitor.py` & `bpmn-tools-0.1.3/bpmn_tools/visitor.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/bpmn_tools/xml.py` & `bpmn-tools-0.1.3/bpmn_tools/xml.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/bpmn_tools.egg-info/PKG-INFO` & `bpmn-tools-0.1.3/bpmn_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.2/bpmn_tools.egg-info/SOURCES.txt` & `bpmn-tools-0.1.3/bpmn_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/docs/conf.py` & `bpmn-tools-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/setup.py` & `bpmn-tools-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/tests/test_colors.py` & `bpmn-tools-0.1.3/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/tests/test_flows.py` & `bpmn-tools-0.1.3/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/tests/test_hello.py` & `bpmn-tools-0.1.3/tests/test_hello.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/tests/test_lanes.py` & `bpmn-tools-0.1.3/tests/test_lanes.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/tests/test_roundtrip.py` & `bpmn-tools-0.1.3/tests/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.2/tests/test_visitor.py` & `bpmn-tools-0.1.3/tests/test_visitor.py`

 * *Files identical despite different names*

