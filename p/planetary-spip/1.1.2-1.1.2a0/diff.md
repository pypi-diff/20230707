# Comparing `tmp/planetary-spip-1.1.2.tar.gz` & `tmp/planetary-spip-1.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetary-spip-1.1.2.tar", last modified: Thu Jul  6 22:36:24 2023, max compression
+gzip compressed data, was "planetary-spip-1.1.2a0.tar", last modified: Thu Jul  6 22:53:11 2023, max compression
```

## Comparing `planetary-spip-1.1.2.tar` & `planetary-spip-1.1.2a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:36:24.407833 planetary-spip-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-06 22:36:24.407833 planetary-spip-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:36:24.407833 planetary-spip-1.1.2/planetary_spip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-06 22:36:24.000000 planetary-spip-1.1.2/planetary_spip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-06 22:36:24.000000 planetary-spip-1.1.2/planetary_spip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:36:24.000000 planetary-spip-1.1.2/planetary_spip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 22:36:24.000000 planetary-spip-1.1.2/planetary_spip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 22:36:24.000000 planetary-spip-1.1.2/planetary_spip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:36:24.407833 planetary-spip-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:36:24.407833 planetary-spip-1.1.2/spip/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/spip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/spip/circular_pixels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:36:24.407833 planetary-spip-1.1.2/spip/data/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/spip/data/celestial_objects.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/spip/data/instruments.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-06 22:36:13.000000 planetary-spip-1.1.2/spip/emm_emirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:53:11.580212 planetary-spip-1.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-06 22:53:11.580212 planetary-spip-1.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:53:11.580212 planetary-spip-1.1.2a0/planetary_spip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-06 22:53:11.000000 planetary-spip-1.1.2a0/planetary_spip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-06 22:53:11.000000 planetary-spip-1.1.2a0/planetary_spip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:53:11.000000 planetary-spip-1.1.2a0/planetary_spip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 22:53:11.000000 planetary-spip-1.1.2a0/planetary_spip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 22:53:11.000000 planetary-spip-1.1.2a0/planetary_spip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:53:11.580212 planetary-spip-1.1.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:53:11.580212 planetary-spip-1.1.2a0/spip/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/spip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/spip/circular_pixels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:53:11.580212 planetary-spip-1.1.2a0/spip/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/spip/data/celestial_objects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/spip/data/instruments.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-06 22:52:58.000000 planetary-spip-1.1.2a0/spip/emm_emirs.py
```

### Comparing `planetary-spip-1.1.2/LICENSE` & `planetary-spip-1.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `planetary-spip-1.1.2/PKG-INFO` & `planetary-spip-1.1.2a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetary-spip
-Version: 1.1.2
+Version: 1.1.2a0
 Summary: Spacecraft Pixel footprint Projection
 Author: Aurélien Stcherbinine
 Author-email: aurelien.stcherbinine@nau.edu
 Project-URL: Source, https://github.com/NAU-PIXEL/spip
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,21 @@
 [![DOI](https://zenodo.org/badge/490546598.svg)](https://zenodo.org/badge/latestdoi/490546598)
 
 # SPiP : Spacecraft Pixel footprint Projection
 
 Projection of the pixel footprint from an instrument onboard an orbital spacecraft on a planetary surface.
 
 ## Installation & Update
+### Method 1: from PyPI (recommended)
+**Installation:** `pip3 install planetary-spip`
+
+**Update:** `pip3 install planetary-spip --upgrade` 
+
+
+### Method 2: from the GitHub repository (development version)
 **Installation:** Clone the repository and install with pip:
 
 ~~~bash
 git clone https://github.com/NAU-PIXEL/spip.git
 cd spip
 pip3 install .
 ~~~
```

### Comparing `planetary-spip-1.1.2/README.md` & `planetary-spip-1.1.2a0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 [![DOI](https://zenodo.org/badge/490546598.svg)](https://zenodo.org/badge/latestdoi/490546598)
 
 # SPiP : Spacecraft Pixel footprint Projection
 
 Projection of the pixel footprint from an instrument onboard an orbital spacecraft on a planetary surface.
 
 ## Installation & Update
+### Method 1: from PyPI (recommended)
+**Installation:** `pip3 install planetary-spip`
+
+**Update:** `pip3 install planetary-spip --upgrade` 
+
+
+### Method 2: from the GitHub repository (development version)
 **Installation:** Clone the repository and install with pip:
 
 ~~~bash
 git clone https://github.com/NAU-PIXEL/spip.git
 cd spip
 pip3 install .
 ~~~
```

### Comparing `planetary-spip-1.1.2/planetary_spip.egg-info/PKG-INFO` & `planetary-spip-1.1.2a0/planetary_spip.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetary-spip
-Version: 1.1.2
+Version: 1.1.2a0
 Summary: Spacecraft Pixel footprint Projection
 Author: Aurélien Stcherbinine
 Author-email: aurelien.stcherbinine@nau.edu
 Project-URL: Source, https://github.com/NAU-PIXEL/spip
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,21 @@
 [![DOI](https://zenodo.org/badge/490546598.svg)](https://zenodo.org/badge/latestdoi/490546598)
 
 # SPiP : Spacecraft Pixel footprint Projection
 
 Projection of the pixel footprint from an instrument onboard an orbital spacecraft on a planetary surface.
 
 ## Installation & Update
+### Method 1: from PyPI (recommended)
+**Installation:** `pip3 install planetary-spip`
+
+**Update:** `pip3 install planetary-spip --upgrade` 
+
+
+### Method 2: from the GitHub repository (development version)
 **Installation:** Clone the repository and install with pip:
 
 ~~~bash
 git clone https://github.com/NAU-PIXEL/spip.git
 cd spip
 pip3 install .
 ~~~
```

### Comparing `planetary-spip-1.1.2/setup.py` & `planetary-spip-1.1.2a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 package_data = {
     '': ['data/*'],
     }
 
 setuptools.setup(
     name='planetary-spip',
-    version='1.1.2',
+    version='1.1.2-a',
     author='Aurélien Stcherbinine',
     author_email='aurelien.stcherbinine@nau.edu',
     description='Spacecraft Pixel footprint Projection',
     long_description=long_description,
     long_description_content_type='text/markdown',
     project_urls={
         'Source' : 'https://github.com/NAU-PIXEL/spip',
```

### Comparing `planetary-spip-1.1.2/spip/circular_pixels.py` & `planetary-spip-1.1.2a0/spip/circular_pixels.py`

 * *Files identical despite different names*

### Comparing `planetary-spip-1.1.2/spip/emm_emirs.py` & `planetary-spip-1.1.2a0/spip/emm_emirs.py`

 * *Files identical despite different names*

