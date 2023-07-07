# Comparing `tmp/tja2fumen-0.4.0.tar.gz` & `tmp/tja2fumen-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.4.0.tar", last modified: Thu Jul  6 03:55:54 2023, max compression
+gzip compressed data, was "tja2fumen-0.4.1.tar", last modified: Fri Jul  7 03:41:38 2023, max compression
```

## Comparing `tja2fumen-0.4.0.tar` & `tja2fumen-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/
--rw-rw-rw-   0        0        0     1083 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4388 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/README.md
--rw-rw-rw-   0        0        0      897 2023-07-06 03:55:38.000000 tja2fumen-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.312815 tja2fumen-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.328426 tja2fumen-0.4.0/src/tja2fumen/
--rw-rw-rw-   0        0        0     1825 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    15705 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    19907 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.344051 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
--rw-rw-rw-   0        0        0     3308 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2905 2023-07-06 03:54:36.000000 tja2fumen-0.4.0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:55:54.328426 tja2fumen-0.4.0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4388 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 03:55:54.000000 tja2fumen-0.4.0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4388 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-07 03:41:26.000000 tja2fumen-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 03:41:38.678982 tja2fumen-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.647740 tja2fumen-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1825 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     3856 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    15506 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    19907 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/
+-rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
+-rw-rw-rw-   0        0        0    23890 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
+-rw-rw-rw-   0        0        0    23883 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
+-rw-rw-rw-   0        0        0    23887 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
+-rw-rw-rw-   0        0        0    23880 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
+-rw-rw-rw-   0        0        0    23872 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
+-rw-rw-rw-   0        0        0    23869 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
+-rw-rw-rw-   0        0        0     3308 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2905 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4388 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.4.0/LICENSE.txt` & `tja2fumen-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/PKG-INFO` & `tja2fumen-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.4.0
+Version: 0.4.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.4.0/README.md` & `tja2fumen-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/pyproject.toml` & `tja2fumen-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.4.0"
+version = "0.4.1"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.4.0/src/tja2fumen/__init__.py` & `tja2fumen-0.4.1/src/tja2fumen/__init__.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/constants.py` & `tja2fumen-0.4.1/src/tja2fumen/constants.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/converters.py` & `tja2fumen-0.4.1/src/tja2fumen/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,29 +155,27 @@
 
             # Compute the duration of the measure
             measureSize = measureTJA['time_sig'][0] / measureTJA['time_sig'][1]
             measureLength = measureTJA['pos_end'] - measureTJA['pos_start']
             measureRatio = 1.0 if measureTJA['subdivisions'] == 0.0 else (measureLength / measureTJA['subdivisions'])
             # - measureDurationBase: The "base" measure duration, computed using a single BPM value.
             # - measureDuration: The actual measure duration, which may be adjusted if there is a mid-measure BPM change.
-            measureDurationBase = measureDuration = (4 * 60_000 * measureSize * measureRatio / measureTJA['bpm'])
+            measureDurationFullMeasure = 4 * 60_000 / measureTJA['bpm']
+            measureDurationBase = measureDuration = (measureDurationFullMeasure * measureSize * measureRatio)
             # The following adjustment accounts for BPM changes. (!!! Discovered by tana :3 !!!)
             if idx_m != len(branch)-1:
                 measureTJANext = branch[idx_m + 1]
                 if measureTJA['bpm'] != measureTJANext['bpm']:
                     measureDuration -= (4 * 60_000 * ((1 / measureTJANext['bpm']) - (1 / measureTJA['bpm'])))
 
             # Compute the millisecond offset for each measure
             if idx_m == 0:
-                pass  # NB: Pass for now, since we need the 2nd measure's duration to compute the 1st measure's offset
+                tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
+                tjaConverted['measures'][idx_m]['fumenOffset'] = tjaOffset - measureDurationFullMeasure
             else:
-                # Compute the 1st measure's offset by subtracting the 2nd measure's duration from the tjaOffset
-                if idx_m == 1:
-                    tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
-                    tjaConverted['measures'][idx_m-1]['fumenOffset'] = tjaOffset - measureDurationPrev
                 # Use the previous measure's offset plus the previous duration to compute the current measure's offset
                 measureOffsetPrev = tjaConverted['measures'][idx_m-1]['fumenOffset']
                 measureFumen['fumenOffset'] = measureOffsetPrev + measureDurationPrev + measureTJA['delay']
             measureDurationPrev = measureDuration
 
             # Best guess at what 'barline' status means for each measure:
             # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
```

### Comparing `tja2fumen-0.4.0/src/tja2fumen/parsers.py` & `tja2fumen-0.4.1/src/tja2fumen/parsers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv` & `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/utils.py` & `tja2fumen-0.4.1/src/tja2fumen/utils.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen/writers.py` & `tja2fumen-0.4.1/src/tja2fumen/writers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.0/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.4.1/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.4.0
+Version: 0.4.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.4.0/src/tja2fumen.egg-info/SOURCES.txt` & `tja2fumen-0.4.1/src/tja2fumen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

