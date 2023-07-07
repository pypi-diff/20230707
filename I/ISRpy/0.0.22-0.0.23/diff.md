# Comparing `tmp/ISRpy-0.0.22.tar.gz` & `tmp/ISRpy-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ISRpy-0.0.22.tar", last modified: Wed Jan  5 02:33:06 2022, max compression
+gzip compressed data, was "ISRpy-0.0.23.tar", last modified: Fri Jul  7 08:43:24 2023, max compression
```

## Comparing `ISRpy-0.0.22.tar` & `ISRpy-0.0.23.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2022-01-05 02:33:06.939745 ISRpy-0.0.22/
-drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2022-01-05 02:33:06.921148 ISRpy-0.0.22/ISRpy/
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1220 2022-01-05 02:32:36.000000 ISRpy-0.0.22/ISRpy/__init__.py
-drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2022-01-05 02:33:06.934051 ISRpy-0.0.22/ISRpy/beampack/
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1148 2022-01-05 02:26:58.000000 ISRpy-0.0.22/ISRpy/beampack/ALTAIRbeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1108 2022-01-05 02:31:02.000000 ISRpy-0.0.22/ISRpy/beampack/AObeam.py
--rw-rw-r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1091 2022-01-05 02:24:54.000000 ISRpy-0.0.22/ISRpy/beampack/PFISRbeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1008 2022-01-05 02:24:00.000000 ISRpy-0.0.22/ISRpy/beampack/__init__.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1241 2022-01-05 02:30:45.000000 ISRpy-0.0.22/ISRpy/beampack/bahirdarbeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    10428 2022-01-05 02:24:18.000000 ISRpy-0.0.22/ISRpy/beampack/beamtools.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1125 2022-01-05 02:30:22.000000 ISRpy-0.0.22/ISRpy/beampack/esrbeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1225 2022-01-05 02:30:05.000000 ISRpy-0.0.22/ISRpy/beampack/irisbeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     2154 2022-01-05 02:29:44.000000 ISRpy-0.0.22/ISRpy/beampack/jrobeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     7175 2021-12-21 01:15:06.000000 ISRpy-0.0.22/ISRpy/beampack/jrobeam0.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1145 2022-01-05 02:28:57.000000 ISRpy-0.0.22/ISRpy/beampack/kairabeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1443 2022-01-05 02:28:34.000000 ISRpy-0.0.22/ISRpy/beampack/kwajbeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1148 2022-01-05 02:27:57.000000 ISRpy-0.0.22/ISRpy/beampack/laplatabeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1136 2022-01-05 02:27:40.000000 ISRpy-0.0.22/ISRpy/beampack/sanyabeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1163 2022-01-05 02:27:27.000000 ISRpy-0.0.22/ISRpy/beampack/tromsobeam.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1204 2021-12-20 21:36:44.000000 ISRpy-0.0.22/ISRpy/enoise.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    28635 2021-12-20 21:36:44.000000 ISRpy-0.0.22/ISRpy/kmltools.py
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    10310 2021-12-21 07:02:00.000000 ISRpy-0.0.22/ISRpy/pyigrf.py
-drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2022-01-05 02:33:06.938590 ISRpy-0.0.22/ISRpy/readpack/
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     2743 2021-12-20 21:36:44.000000 ISRpy-0.0.22/ISRpy/readpack/JROfileread.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)      425 2021-12-20 21:36:44.000000 ISRpy-0.0.22/ISRpy/readpack/__init__.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)   109079 2021-12-20 21:36:44.000000 ISRpy-0.0.22/ISRpy/readpack/digital_rf_hdf5.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     5651 2022-01-01 07:47:51.000000 ISRpy-0.0.22/ISRpy/readpack/irisread.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    20122 2021-12-20 21:36:44.000000 ISRpy-0.0.22/ISRpy/readpack/jroread.py
--rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    18889 2021-12-20 21:36:44.000000 ISRpy-0.0.22/ISRpy/readpack/rdvme.py
-drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2022-01-05 02:33:06.923606 ISRpy-0.0.22/ISRpy.egg-info/
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1643 2022-01-05 02:33:06.000000 ISRpy-0.0.22/ISRpy.egg-info/PKG-INFO
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)      822 2022-01-05 02:33:06.000000 ISRpy-0.0.22/ISRpy.egg-info/SOURCES.txt
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)        1 2022-01-05 02:33:06.000000 ISRpy-0.0.22/ISRpy.egg-info/dependency_links.txt
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)       12 2022-01-05 02:33:06.000000 ISRpy-0.0.22/ISRpy.egg-info/requires.txt
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)        6 2022-01-05 02:33:06.000000 ISRpy-0.0.22/ISRpy.egg-info/top_level.txt
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1074 2021-12-20 21:36:44.000000 ISRpy-0.0.22/LICENSE
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1643 2022-01-05 02:33:06.939401 ISRpy-0.0.22/PKG-INFO
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1029 2021-12-21 16:31:12.000000 ISRpy-0.0.22/README.md
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)       38 2022-01-05 02:33:06.939861 ISRpy-0.0.22/setup.cfg
--rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1232 2022-01-01 07:47:51.000000 ISRpy-0.0.22/setup.py
+drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2023-07-07 08:43:24.915615 ISRpy-0.0.23/
+drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2023-07-07 08:43:24.909743 ISRpy-0.0.23/ISRpy/
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1220 2023-07-07 08:40:58.000000 ISRpy-0.0.23/ISRpy/__init__.py
+drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2023-07-07 08:43:24.912721 ISRpy-0.0.23/ISRpy/beampack/
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1148 2022-01-05 02:26:58.000000 ISRpy-0.0.23/ISRpy/beampack/ALTAIRbeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1108 2022-01-05 02:31:02.000000 ISRpy-0.0.23/ISRpy/beampack/AObeam.py
+-rw-rw-r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1091 2022-01-05 02:24:54.000000 ISRpy-0.0.23/ISRpy/beampack/PFISRbeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1008 2022-01-05 02:24:00.000000 ISRpy-0.0.23/ISRpy/beampack/__init__.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1241 2022-01-05 02:30:45.000000 ISRpy-0.0.23/ISRpy/beampack/bahirdarbeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    10428 2022-01-05 02:24:18.000000 ISRpy-0.0.23/ISRpy/beampack/beamtools.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1125 2022-01-05 02:30:22.000000 ISRpy-0.0.23/ISRpy/beampack/esrbeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1225 2022-01-05 02:30:05.000000 ISRpy-0.0.23/ISRpy/beampack/irisbeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     2154 2022-01-05 02:29:44.000000 ISRpy-0.0.23/ISRpy/beampack/jrobeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     7175 2021-12-21 01:15:06.000000 ISRpy-0.0.23/ISRpy/beampack/jrobeam0.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1145 2022-01-05 02:28:57.000000 ISRpy-0.0.23/ISRpy/beampack/kairabeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1443 2022-01-05 02:28:34.000000 ISRpy-0.0.23/ISRpy/beampack/kwajbeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1148 2022-01-05 02:27:57.000000 ISRpy-0.0.23/ISRpy/beampack/laplatabeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1136 2022-01-05 02:27:40.000000 ISRpy-0.0.23/ISRpy/beampack/sanyabeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1163 2022-01-05 02:27:27.000000 ISRpy-0.0.23/ISRpy/beampack/tromsobeam.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     1204 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/enoise.py
+drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2023-07-07 08:43:24.914145 ISRpy-0.0.23/ISRpy/igrfdata/
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    21618 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/igrfdata/IGRFGEN7.DAT
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    21825 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/igrfdata/IGRFGEN8.DAT
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    41496 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/igrfdata/igrf10coeffs.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    36306 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/igrfdata/igrf11coeffs.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    38673 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/igrfdata/igrf12coeffs.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    40639 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/igrfdata/igrf13coeffs.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    12300 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/igrfdata/igrf9coeffs.txt
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    28698 2023-07-07 06:52:49.000000 ISRpy-0.0.23/ISRpy/kmltools.py
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)    10310 2021-12-21 07:02:00.000000 ISRpy-0.0.23/ISRpy/pyigrf.py
+drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2023-07-07 08:43:24.915262 ISRpy-0.0.23/ISRpy/readpack/
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     2743 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/readpack/JROfileread.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)      425 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/readpack/__init__.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)   109079 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/readpack/digital_rf_hdf5.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)     5651 2022-01-01 07:47:51.000000 ISRpy-0.0.23/ISRpy/readpack/irisread.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    20122 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/readpack/jroread.py
+-rwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)    18889 2021-12-20 21:36:44.000000 ISRpy-0.0.23/ISRpy/readpack/rdvme.py
+drwxr-xr-x   0 e30824   (618061100) SRI\Domain Users (12104065)        0 2023-07-07 08:43:24.910429 ISRpy-0.0.23/ISRpy.egg-info/
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1441 2023-07-07 08:43:24.000000 ISRpy-0.0.23/ISRpy.egg-info/PKG-INFO
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1037 2023-07-07 08:43:24.000000 ISRpy-0.0.23/ISRpy.egg-info/SOURCES.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)        1 2023-07-07 08:43:24.000000 ISRpy-0.0.23/ISRpy.egg-info/dependency_links.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)       12 2023-07-07 08:43:24.000000 ISRpy-0.0.23/ISRpy.egg-info/requires.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)        6 2023-07-07 08:43:24.000000 ISRpy-0.0.23/ISRpy.egg-info/top_level.txt
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1074 2021-12-20 21:36:44.000000 ISRpy-0.0.23/LICENSE
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1441 2023-07-07 08:43:24.915492 ISRpy-0.0.23/PKG-INFO
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1029 2021-12-21 16:31:12.000000 ISRpy-0.0.23/README.md
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)       38 2023-07-07 08:43:24.915652 ISRpy-0.0.23/setup.cfg
+-rw-r--r--   0 e30824   (618061100) SRI\Domain Users (12104065)     1232 2022-01-01 07:47:51.000000 ISRpy-0.0.23/setup.py
```

### Comparing `ISRpy-0.0.22/ISRpy/__init__.py` & `ISRpy-0.0.23/ISRpy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,12 @@
 """
 from . import readpack
 from . import beampack
 from . import enoise
 from .pyigrf import pyigrf
 
 # from . import kmltools # needs to be fixed
-__version__ = '0.0.22'
+__version__ = '0.0.23'
 
 igrf = pyigrf() # instantiating with the latest IGRF coefficients
 
 __all__=['readpack','beampack','kmltools','enoise', 'igrf']
```

### Comparing `ISRpy-0.0.22/ISRpy/beampack/ALTAIRbeam.py` & `ISRpy-0.0.23/ISRpy/beampack/ALTAIRbeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/AObeam.py` & `ISRpy-0.0.23/ISRpy/beampack/AObeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/PFISRbeam.py` & `ISRpy-0.0.23/ISRpy/beampack/PFISRbeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/__init__.py` & `ISRpy-0.0.23/ISRpy/beampack/__init__.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/bahirdarbeam.py` & `ISRpy-0.0.23/ISRpy/beampack/bahirdarbeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/beamtools.py` & `ISRpy-0.0.23/ISRpy/beampack/beamtools.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/esrbeam.py` & `ISRpy-0.0.23/ISRpy/beampack/esrbeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/irisbeam.py` & `ISRpy-0.0.23/ISRpy/beampack/irisbeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/jrobeam.py` & `ISRpy-0.0.23/ISRpy/beampack/jrobeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/jrobeam0.py` & `ISRpy-0.0.23/ISRpy/beampack/jrobeam0.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/kairabeam.py` & `ISRpy-0.0.23/ISRpy/beampack/kairabeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/kwajbeam.py` & `ISRpy-0.0.23/ISRpy/beampack/kwajbeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/laplatabeam.py` & `ISRpy-0.0.23/ISRpy/beampack/laplatabeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/sanyabeam.py` & `ISRpy-0.0.23/ISRpy/beampack/sanyabeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/beampack/tromsobeam.py` & `ISRpy-0.0.23/ISRpy/beampack/tromsobeam.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/enoise.py` & `ISRpy-0.0.23/ISRpy/enoise.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/kmltools.py` & `ISRpy-0.0.23/ISRpy/kmltools.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 #  - June 5, 2016 by E. Kudeki
 #    -importing radarbeam from beampack rather than radarpack
 #    -beampack is now a sub package of ISRpy.
 
 
 # ------------ radar specifications -------------------------
 import numpy as np
-import StringIO as __StringIO__
+try:
+    import StringIO as __StringIO__
+except:
+    from io import StringIO as __StringIO__
 
 class kmzfile:
     """Will contain functions to create a kmz file"""
     def __init__(self, fname=None, title = None):
         import zipfile as __zipfile__
         self.fname = fname
         self.title = title
@@ -137,20 +140,20 @@
             self.fname = basen+str(i)+'.kml'
         if type(self.fname) == str:
             try:
                 fp = open(self.fname,'w')
                 fp.write(self.outstr)
                 fp.close()
             except:
-                print "Error writing  ", self.fname
+                print("Error writing  ", self.fname)
         else:
             try:
                 self.fname.write(self.outstr)
             except:
-                print "Error writing in ", self.fname
+                print("Error writing in ", self.fname)
 
     def startfolder(self,foldertitle=None):
         self.outstr += "<Folder>\n"
         if foldertitle!=None:
             self.outstr += "<name>"+foldertitle+"</name>\n"
 
     def addtime(self,yyyy,mm,dd,HH=0,MM=0,SS=0):
```

### Comparing `ISRpy-0.0.22/ISRpy/pyigrf.py` & `ISRpy-0.0.23/ISRpy/pyigrf.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/readpack/JROfileread.py` & `ISRpy-0.0.23/ISRpy/readpack/JROfileread.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/readpack/digital_rf_hdf5.py` & `ISRpy-0.0.23/ISRpy/readpack/digital_rf_hdf5.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/readpack/irisread.py` & `ISRpy-0.0.23/ISRpy/readpack/irisread.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/readpack/jroread.py` & `ISRpy-0.0.23/ISRpy/readpack/jroread.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/ISRpy/readpack/rdvme.py` & `ISRpy-0.0.23/ISRpy/readpack/rdvme.py`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/LICENSE` & `ISRpy-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/README.md` & `ISRpy-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `ISRpy-0.0.22/setup.py` & `ISRpy-0.0.23/setup.py`

 * *Files identical despite different names*

