# Comparing `tmp/pygrb_lc-0.1.0.tar.gz` & `tmp/pygrb_lc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.1.0.tar", last modified: Fri Jul  7 09:48:37 2023, max compression
+gzip compressed data, was "pygrb_lc-0.1.1.tar", last modified: Fri Jul  7 16:48:05 2023, max compression
```

## Comparing `pygrb_lc-0.1.0.tar` & `pygrb_lc-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.359226 pygrb_lc-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.359226 pygrb_lc-0.1.0/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.461765 pygrb_lc-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/tests/test_utils.py
```

### Comparing `pygrb_lc-0.1.0/LICENSE` & `pygrb_lc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/PKG-INFO` & `pygrb_lc-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pygrb_lc
-Version: 0.1.0
-Summary: Python package for GRB analysis
-Home-page: https://github.com/Jorezzz/pygrb_lc
-Author: Mozgunov Georgiy
-Author-email: georgiy99@bk.ru
-Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pygrb_lc
 Package to load and handle GRB (Gamma-ray bursts) light curves, their furie transformations and various other functions.
 
 To install run the following command
 
 ```bash
 pip install --upgrade pygrb_lc
@@ -68,13 +53,29 @@
 All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
 ```python
 fig,(ax1,ax2) = plt.subplots(2,1)
 lc.plot(ax = ax1)
 flc.plot(ax = ax2)
 ```
 
+# Catalog
+
+```Catalog```  class is an extension of pandas.DataFrame. It provides simplicity of manipulations and visualization and extend it with crossmatching functionality. Easiest way to start using it is to create it from existing tabular data. It is important to provide `event_column` argument, it is the name of column that will be used for crossmatching and comparison
+
+```python
+from pygrb_lc.catalogs import Catalog
+import pandas as pd
+import numpy as np
+
+data = np.loadtxt('test.txt')
+cat = Catalog(data, columns = ['datetime','duration'], event_column = 'datetime')
+cat.find_event(pd.Timestamp('2023-01-01 00:00:00'), precision = 10)
+```
+
+`precision` (in seconds) controls uncertainity that is allowed for the event. If there is no such event method will return `None`.
+There is a method of crossmatching two catalogs `crossmatch`, it works like inner join for SQL tables, but compares only corresponding `event_column` columns and allows uncertainity via `precision`. `precision = 0` equals to exact match.
+
 
 # Roadmap
-Add support of main GRB catalogues and their connection with light curves. 
-Create Catalogue class that can be compared and intersected to other. 
-Add support of spectra (based on current ```photon_data``` in GBM_LightCurve class)
-Add typical functions for approximation: Band function, power law, etc. and their interaction with ```LightCurve``` and ```FurieLightCurve``` classes.
+Add support of `LightCurve` class in `Catalog`
+Add support of spectra (based on current `photon_data` in `GBM_LightCurve` class)
+Add typical functions for approximation: Band function, power law, etc. and their interaction with `LightCurve` and `FurieLightCurve` classes.
```

### Comparing `pygrb_lc-0.1.0/setup.cfg` & `pygrb_lc-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.1.0
+version = 0.1.1
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.1.1/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/catalogs.py` & `pygrb_lc-0.1.1/src/pygrb_lc/catalogs.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/config.py` & `pygrb_lc-0.1.1/src/pygrb_lc/config.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.1.1/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/furie.py` & `pygrb_lc-0.1.1/src/pygrb_lc/furie.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.1.1/src/pygrb_lc/light_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,25 +705,29 @@
         plt.axvline(t_5_low)
         plt.axvline(t_5_high)
         plt.axvline(t_95_low)
         plt.axvline(t_95_high)
 
     return t_90, (-negative_err, positive_err)
 
-def plot_gbm_all_detectors(center_time: str, duration: float, binning: float = 0.5, **kwargs):
+def plot_gbm_all_detectors(center_time: str, duration: float, binning: float = 0.5, axs = None, **kwargs):
     detector_list = [x for x in GBM_DETECTORS if x[0] == 'n']
     data = {}
 
-    fig, ax = plt.subplots(4,3,figsize=(30,30))
-    ax = ax.reshape(-1,)
+    if axs is None:
+        fig, ax = plt.subplots(4,3,figsize=(30,30))
+        ax = ax.reshape(-1,)
+    else:
+        ax = axs
+        
     for i, detector in enumerate(detector_list):
         lc = GBM_LightCurve(center_time, [detector], duration = duration, **kwargs)
         lc.rebin(binning).plot(ax=ax[i], label = detector)
         signal = lc.signal
         ax[i].axhline(np.mean(signal),color = 'blue')
         ax[i].axhline(np.mean(signal)+3*np.std(signal),color = 'green')
         ax[i].axhline(np.mean(signal)-3*np.std(signal),color = 'green')
         ax[i].legend()
         data[detector] = lc
-    fig.suptitle(center_time)
-    return fig, ax, data
+    plt.suptitle(center_time)
+    return ax, data
     # plt.savefig(IMAGE_PATH + center_time.replace(':','_') + '.png',bbox_inches='tight')
```

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/time.py` & `pygrb_lc-0.1.1/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc/utils.py` & `pygrb_lc-0.1.1/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.0/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.1.1/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb-lc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -68,13 +68,29 @@
 All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
 ```python
 fig,(ax1,ax2) = plt.subplots(2,1)
 lc.plot(ax = ax1)
 flc.plot(ax = ax2)
 ```
 
+# Catalog
+
+```Catalog```  class is an extension of pandas.DataFrame. It provides simplicity of manipulations and visualization and extend it with crossmatching functionality. Easiest way to start using it is to create it from existing tabular data. It is important to provide `event_column` argument, it is the name of column that will be used for crossmatching and comparison
+
+```python
+from pygrb_lc.catalogs import Catalog
+import pandas as pd
+import numpy as np
+
+data = np.loadtxt('test.txt')
+cat = Catalog(data, columns = ['datetime','duration'], event_column = 'datetime')
+cat.find_event(pd.Timestamp('2023-01-01 00:00:00'), precision = 10)
+```
+
+`precision` (in seconds) controls uncertainity that is allowed for the event. If there is no such event method will return `None`.
+There is a method of crossmatching two catalogs `crossmatch`, it works like inner join for SQL tables, but compares only corresponding `event_column` columns and allows uncertainity via `precision`. `precision = 0` equals to exact match.
+
 
 # Roadmap
-Add support of main GRB catalogues and their connection with light curves. 
-Create Catalogue class that can be compared and intersected to other. 
-Add support of spectra (based on current ```photon_data``` in GBM_LightCurve class)
-Add typical functions for approximation: Band function, power law, etc. and their interaction with ```LightCurve``` and ```FurieLightCurve``` classes.
+Add support of `LightCurve` class in `Catalog`
+Add support of spectra (based on current `photon_data` in `GBM_LightCurve` class)
+Add typical functions for approximation: Band function, power law, etc. and their interaction with `LightCurve` and `FurieLightCurve` classes.
```

### Comparing `pygrb_lc-0.1.0/tests/test_utils.py` & `pygrb_lc-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

