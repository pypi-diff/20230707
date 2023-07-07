# Comparing `tmp/pyciactions-1.0.8a8.tar.gz` & `tmp/pyciactions-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyciactions-1.0.8a8.tar", last modified: Fri Jul  7 05:51:30 2023, max compression
+gzip compressed data, was "pyciactions-1.0.9.tar", last modified: Fri Jul  7 05:53:13 2023, max compression
```

## Comparing `pyciactions-1.0.8a8.tar` & `pyciactions-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:51:30.262663 pyciactions-1.0.8a8/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.8a8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:51:30.259209 pyciactions-1.0.8a8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.8a8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:51:30.088282 pyciactions-1.0.8a8/pyciactions/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.8a8/pyciactions/IWorkflow.py
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-07 05:49:29.000000 pyciactions-1.0.8a8/pyciactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.8a8/pyciactions/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:51:30.242843 pyciactions-1.0.8a8/pyciactions/github/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-07 05:42:49.000000 pyciactions-1.0.8a8/pyciactions/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-06-07 06:28:53.000000 pyciactions-1.0.8a8/pyciactions/github/job.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-06-07 06:25:57.000000 pyciactions-1.0.8a8/pyciactions/github/on.py
--rw-r--r--   0 root         (0) root         (0)      759 2023-06-07 06:26:04.000000 pyciactions-1.0.8a8/pyciactions/github/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:51:30.161144 pyciactions-1.0.8a8/pyciactions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:51:29.000000 pyciactions-1.0.8a8/pyciactions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-07 05:51:29.000000 pyciactions-1.0.8a8/pyciactions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 05:51:29.000000 pyciactions-1.0.8a8/pyciactions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 05:51:29.000000 pyciactions-1.0.8a8/pyciactions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 05:51:29.000000 pyciactions-1.0.8a8/pyciactions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 05:51:30.263742 pyciactions-1.0.8a8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-07 05:51:25.000000 pyciactions-1.0.8a8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:53:13.678633 pyciactions-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 05:53:13.675171 pyciactions-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:53:13.498137 pyciactions-1.0.9/pyciactions/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-07 05:52:57.000000 pyciactions-1.0.9/pyciactions/IWorkflow.py
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-07 05:49:29.000000 pyciactions-1.0.9/pyciactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.9/pyciactions/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:53:13.656565 pyciactions-1.0.9/pyciactions/github/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-07 05:42:49.000000 pyciactions-1.0.9/pyciactions/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-06-07 06:28:53.000000 pyciactions-1.0.9/pyciactions/github/job.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-07 06:25:57.000000 pyciactions-1.0.9/pyciactions/github/on.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-07 05:52:48.000000 pyciactions-1.0.9/pyciactions/github/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:53:13.571446 pyciactions-1.0.9/pyciactions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 05:53:13.000000 pyciactions-1.0.9/pyciactions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-07 05:53:13.000000 pyciactions-1.0.9/pyciactions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 05:53:13.000000 pyciactions-1.0.9/pyciactions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 05:53:13.000000 pyciactions-1.0.9/pyciactions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 05:53:13.000000 pyciactions-1.0.9/pyciactions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 05:53:13.679759 pyciactions-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      498 2023-07-07 05:53:09.000000 pyciactions-1.0.9/setup.py
```

### Comparing `pyciactions-1.0.8a8/LICENSE` & `pyciactions-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a8/PKG-INFO` & `pyciactions-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.8a8
+Version: 1.0.9
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```

### Comparing `pyciactions-1.0.8a8/README.md` & `pyciactions-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a8/pyciactions/github/job.py` & `pyciactions-1.0.9/pyciactions/github/job.py`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a8/pyciactions/github/on.py` & `pyciactions-1.0.9/pyciactions/github/on.py`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a8/pyciactions/github/workflow.py` & `pyciactions-1.0.9/pyciactions/github/workflow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from dataclasses import dataclass
 from typing import Optional, List, Dict
 
-from pyactions import IWorkflow
+from pyciactions import IWorkflow
 from .on import On
 from .job import Job
 
+
 @dataclass
 class Workflow(IWorkflow):
     name: str
     on: List[On]
     jobs: List[Job]
     permissions: Optional[Dict[str, str]] = None
     env: Optional[Dict[str, str]] = None
 
     def to_dict(self):
         result = {
             "name": self.name,
             "on": [on.to_dict() for on in self.on],
             "jobs": {job.id: job.to_dict() for job in self.jobs},
         }
-        additional_attrs = {k: v for k, v in vars(self).items() if v is not None and k not in result}
+        additional_attrs = {
+            k: v for k, v in vars(self).items() if v is not None and k not in result
+        }
         result.update(additional_attrs)
         return result
-        
+
     def __getstate__(self):
-        return self.to_dict()
+        return self.to_dict()
```

### Comparing `pyciactions-1.0.8a8/pyciactions.egg-info/PKG-INFO` & `pyciactions-1.0.9/pyciactions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.8a8
+Version: 1.0.9
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```

