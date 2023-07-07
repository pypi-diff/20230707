# Comparing `tmp/pyclpu-1.1.0.tar.gz` & `tmp/pyclpu-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclpu-1.1.0.tar", last modified: Fri Jul  7 15:01:59 2023, max compression
+gzip compressed data, was "pyclpu-1.1.1.tar", last modified: Fri Jul  7 18:05:07 2023, max compression
```

## Comparing `pyclpu-1.1.0.tar` & `pyclpu-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:01:59.429757 pyclpu-1.1.0/
--rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    10334 2023-07-07 15:01:59.429757 pyclpu-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9926 2023-07-07 14:57:42.000000 pyclpu-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 15:01:59.423050 pyclpu-1.1.0/pyclpu/
--rw-rw-rw-   0        0        0      629 2023-07-07 15:00:40.000000 pyclpu-1.1.0/pyclpu/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.1.0/pyclpu/constants.py
--rw-rw-rw-   0        0        0      981 2023-07-05 07:06:32.000000 pyclpu-1.1.0/pyclpu/formats.py
--rw-rw-rw-   0        0        0    21605 2023-07-05 10:21:29.000000 pyclpu-1.1.0/pyclpu/image.py
--rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.1.0/pyclpu/main.py
--rw-rw-rw-   0        0        0    21183 2023-07-07 14:32:42.000000 pyclpu-1.1.0/pyclpu/manager.py
--rw-rw-rw-   0        0        0    28837 2023-07-07 14:47:26.000000 pyclpu-1.1.0/pyclpu/metrology.py
--rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.1.0/pyclpu/s33293804.py
--rw-rw-rw-   0        0        0    14839 2023-07-07 12:39:09.000000 pyclpu-1.1.0/pyclpu/waveform.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:01:59.428642 pyclpu-1.1.0/pyclpu.egg-info/
--rw-rw-rw-   0        0        0    10334 2023-07-07 15:01:59.000000 pyclpu-1.1.0/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-07-07 15:01:59.000000 pyclpu-1.1.0/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:01:59.000000 pyclpu-1.1.0/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-07 15:01:59.000000 pyclpu-1.1.0/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 15:01:59.000000 pyclpu-1.1.0/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-07-07 15:01:59.429757 pyclpu-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-07-05 11:27:02.000000 pyclpu-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:05:07.201583 pyclpu-1.1.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0    10583 2023-07-07 18:05:07.201583 pyclpu-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10175 2023-07-07 18:00:36.000000 pyclpu-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 18:05:07.178987 pyclpu-1.1.1/pyclpu/
+-rw-rw-rw-   0        0        0      629 2023-07-07 18:04:22.000000 pyclpu-1.1.1/pyclpu/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.1.1/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      981 2023-07-05 07:06:32.000000 pyclpu-1.1.1/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    21605 2023-07-05 10:21:29.000000 pyclpu-1.1.1/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.1.1/pyclpu/main.py
+-rw-rw-rw-   0        0        0    25307 2023-07-07 17:59:55.000000 pyclpu-1.1.1/pyclpu/manager.py
+-rw-rw-rw-   0        0        0    28837 2023-07-07 14:47:26.000000 pyclpu-1.1.1/pyclpu/metrology.py
+-rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.1.1/pyclpu/s33293804.py
+-rw-rw-rw-   0        0        0    14839 2023-07-07 12:39:09.000000 pyclpu-1.1.1/pyclpu/waveform.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:05:07.201583 pyclpu-1.1.1/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0    10583 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-07-07 18:05:07.201583 pyclpu-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-07-05 11:27:02.000000 pyclpu-1.1.1/setup.py
```

### Comparing `pyclpu-1.1.0/LICENSE` & `pyclpu-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/PKG-INFO` & `pyclpu-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -107,14 +107,25 @@
 chase.loop = True
 
 chase.ignored = []
 
 chase.loop = False
 ```
 
+#### ... changing only their location
+
+```
+from pyclpu import manager
+        
+detector_to_server = manager.Pipeline()
+detector_to_server.source = "C:\\bin"
+detector_to_server.destination = "C:\\bin\\pipe"
+detector_to_server.start()
+```
+
 ### Time-of-Flight Analysis
 
 Data of Time-of-Flight detectors comprises a timeline and an amplitude for every recorded temporal bin. The `ToF` class is ment to make data analysis easier. After input of the data and the geometrical situation (location of the detector with respect to the source), it is possible to obtain a spectrum. The x-axis of the output is normalized to be in units of `gamma -1`, where `gamma` is the Lorenz factor. This way the result of the analysis is kept universal without further interpretation regarding the type of particles. If the type of projectiles is known: To obtain the kinetic energy of projectiles it is sufficient to multiply the values with the rest mass energy of the projectiles, e.g. in units of MeV.
 
 ```
 from pyclpu import metrology
```

### Comparing `pyclpu-1.1.0/README.md` & `pyclpu-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,25 @@
 chase.loop = True
 
 chase.ignored = []
 
 chase.loop = False
 ```
 
+#### ... changing only their location
+
+```
+from pyclpu import manager
+        
+detector_to_server = manager.Pipeline()
+detector_to_server.source = "C:\\bin"
+detector_to_server.destination = "C:\\bin\\pipe"
+detector_to_server.start()
+```
+
 ### Time-of-Flight Analysis
 
 Data of Time-of-Flight detectors comprises a timeline and an amplitude for every recorded temporal bin. The `ToF` class is ment to make data analysis easier. After input of the data and the geometrical situation (location of the detector with respect to the source), it is possible to obtain a spectrum. The x-axis of the output is normalized to be in units of `gamma -1`, where `gamma` is the Lorenz factor. This way the result of the analysis is kept universal without further interpretation regarding the type of particles. If the type of projectiles is known: To obtain the kinetic energy of projectiles it is sufficient to multiply the values with the rest mass energy of the projectiles, e.g. in units of MeV.
 
 ```
 from pyclpu import metrology
```

### Comparing `pyclpu-1.1.0/pyclpu/__init__.py` & `pyclpu-1.1.1/pyclpu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-1.1.0/pyclpu/constants.py` & `pyclpu-1.1.1/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/pyclpu/formats.py` & `pyclpu-1.1.1/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/pyclpu/image.py` & `pyclpu-1.1.1/pyclpu/image.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/pyclpu/main.py` & `pyclpu-1.1.1/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/pyclpu/manager.py` & `pyclpu-1.1.1/pyclpu/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 # =============================================================================
 # PYTHON HEADER
 # =============================================================================
 # EXTERNAL
 import os
 import sys
+import shutil
 import threading
 import time
 
 from inspect import getsourcefile
 from importlib import reload
 
 import math
@@ -306,14 +307,114 @@
     def next(self):
         # get file from list `new` by order of arrival, remove it and add it to list `processed`, returns filename
         if len(self.new) > 0:
             file = self.new.pop(0)
             self.processed.append(file)
         return file
         
+class Pipeline():
+    """ Responsive file pipeline
+    This class looks up files in a directory and moves them to a destination. Existing files are moved to begin with, new files are moved after they are written into the source directory. Files are not moved if a file with the same name is already in the destination.
+    
+    Args:
+        source (str) : Path to directory where new files are expected.
+        destination (str) : Path to directory where new files are moved.
+        
+    Attributes:
+        status (bool) : True if the pipeline is open, else False.
+            Initializes to False.
+    
+    Examples:
+        A object oriented use case is described below. The chase for new files is activated by setting the input parameter `loop = True` and paused by setting `loop = False`.
+        ```
+        from pyclpu import manager
+        
+        detector_to_server = manager.Pipeline()
+        detector_to_server.lsource = "C:\\bin"
+        detector_to_server.destination = "C:\\bin\\pipe"
+        detector_to_server.start()
+        ```
+    """
+    # INI
+    def __new__(cls, *args, **kwargs):
+        return super().__new__(cls)
+    def __init__(self, *args, **kwargs):
+        # INPUT
+        self.__dict__.update(kwargs)
+        # VARIABLES
+        self.status = False
+        # INTEGRITY
+        if not hasattr(self, 'source'):
+            warning(self.__class__.__name__,"Find no source directory, expect key `source` as string.")
+        if not hasattr(self, 'destination'):
+            warning(self.__class__.__name__,"Find no destination directory, expect key `destination` as string.")
+        return None
+    def __setattr__(self, name, value):
+        super().__setattr__(name, value)
+        if name == "status" and value == True:
+            self.start()
+        if name == "status" and value == False:
+            self.stop()
+        return None
+    def __run__(self):
+        # INTEGRITY
+        if not hasattr(self, 'source'):
+            warning(self.__class__.__name__,"No source directory defined, expect key `source` as `source=path/to/directorty`.")
+            return None
+        if not hasattr(self, 'destination'):
+            warning(self.__class__.__name__,"No destination directory defined, expect key `destination` as `destination=path/to/directorty`.")
+            return None
+        # METHODS
+        #@classmethod
+        def _worker(event):
+            self.ident = threading.get_ident()
+            while not self._event.is_set():
+                if len(self.chase.new) > 0:
+                    new_file = self.chase.next()
+                    origin = os.path.join(self.chase.directory,new_file)
+                    moveto = os.path.join(self.destination,new_file)
+                    if os.path.isfile(origin) and not os.path.isfile(moveto):
+                        shutil.move(origin, moveto)
+                    del new_file, origin, moveto
+        # MAIN
+        self.chase = Catch()
+        self.chase.directory = self.source
+        self.chase.leap = False
+        self.chase.loop = True
+        if not os.path.isdir(self.destination):
+            os.makedirs(self.destination)
+        if not hasattr(self,"_event"):
+            self._event = threading.Event()
+            self._process = threading.Thread(target=_worker, args=(self._event,))
+        if hasattr(self,"_process"):
+            self._process.start()
+        else:
+            warning(self.__class__.__name__,"THREAD ALREADY STARTED: DO NOTHING")                  
+        
+    def start(self):
+        # START
+        self.__run__()
+    
+    def stop(self):
+        try:
+            self._event.set()
+            self._process.join()
+        except:
+            warning(self.__class__.__name__,"THREAD ALREADY STOPPED: DO NOTHING")  
+        # integrity of results
+        # ..
+        # housekeeping
+        try:
+            del self.ident, self._event, self._process
+            self.chase.stop()
+            del self.chase
+        except:
+            pass
+        return None
+        
 class CatchAndRename():
     """ Responsive file catcher
     This class waits for new files in a directory and renames them upon arrival.
     
     Args:
         directory (str) : Path to directory where new files are expected.
         prefix (str, optional) : Prefix of renamed filename. Defaults to `""`.
```

### Comparing `pyclpu-1.1.0/pyclpu/metrology.py` & `pyclpu-1.1.1/pyclpu/metrology.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/pyclpu/s33293804.py` & `pyclpu-1.1.1/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/pyclpu/waveform.py` & `pyclpu-1.1.1/pyclpu/waveform.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.0/pyclpu.egg-info/PKG-INFO` & `pyclpu-1.1.1/pyclpu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -107,14 +107,25 @@
 chase.loop = True
 
 chase.ignored = []
 
 chase.loop = False
 ```
 
+#### ... changing only their location
+
+```
+from pyclpu import manager
+        
+detector_to_server = manager.Pipeline()
+detector_to_server.source = "C:\\bin"
+detector_to_server.destination = "C:\\bin\\pipe"
+detector_to_server.start()
+```
+
 ### Time-of-Flight Analysis
 
 Data of Time-of-Flight detectors comprises a timeline and an amplitude for every recorded temporal bin. The `ToF` class is ment to make data analysis easier. After input of the data and the geometrical situation (location of the detector with respect to the source), it is possible to obtain a spectrum. The x-axis of the output is normalized to be in units of `gamma -1`, where `gamma` is the Lorenz factor. This way the result of the analysis is kept universal without further interpretation regarding the type of particles. If the type of projectiles is known: To obtain the kinetic energy of projectiles it is sufficient to multiply the values with the rest mass energy of the projectiles, e.g. in units of MeV.
 
 ```
 from pyclpu import metrology
```

### Comparing `pyclpu-1.1.0/setup.py` & `pyclpu-1.1.1/setup.py`

 * *Files identical despite different names*

