# Comparing `tmp/pygrb_lc-0.0.9.tar.gz` & `tmp/pygrb_lc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.0.9.tar", last modified: Thu Jun 22 21:24:55 2023, max compression
+gzip compressed data, was "pygrb_lc-0.1.0.tar", last modified: Fri Jul  7 09:48:37 2023, max compression
```

## Comparing `pygrb_lc-0.0.9.tar` & `pygrb_lc-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.527002 pygrb_lc-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    32983 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.359226 pygrb_lc-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.359226 pygrb_lc-0.1.0/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 09:48:37.000000 pygrb_lc-0.1.0/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:37.363226 pygrb_lc-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 09:48:26.000000 pygrb_lc-0.1.0/tests/test_utils.py
```

### Comparing `pygrb_lc-0.0.9/LICENSE` & `pygrb_lc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.9/PKG-INFO` & `pygrb_lc-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb_lc
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.0.9/README.md` & `pygrb_lc-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.9/setup.cfg` & `pygrb_lc-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.0.9
+version = 0.1.0
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.1.0/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc/config.py` & `pygrb_lc-0.1.0/src/pygrb_lc/config.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.1.0/src/pygrb_lc/crossmatching.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from .config import DATA_PATH, logging
-
 def find_closest_event(time,list_of_events):
     '''
     Return index of closest event to time by value
     Args:
         time ([float, datetime.datetime, datetime.date]): time to compare
         list_of_events (list): list of events to search in the same time format as 'time'
     '''
```

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc/furie.py` & `pygrb_lc-0.1.0/src/pygrb_lc/furie.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 from .light_curves import LightCurve
 from scipy.stats import chi2
-from typing import Callable, Iterable
+from collections.abc import Callable, Iterable
 
 
 def make_pds(signal, time_step, total_counts = None, pad_size = None):
     '''
     Get Power Density Spectrum from signal
     Args:
         signal (np.array): input signal
@@ -54,19 +54,20 @@
         flux.append(np.mean(ps[mask1]) if len(ps[mask1])!=0 else 0)
         flux_err.append(chi2.ppf(0.67, 2*len(ps[mask1]))/len(ps[mask1]) if len(ps[mask1]) != 0 else 1)
     
     return np.array(time), np.array(time_err), np.array(flux), np.array(flux_err)
 
 class FurieLightCurve():
     def __init__(self, light_curve: LightCurve, 
-                       interval_t90: Iterable = None,
+                       interval_t90: Iterable | None = None,
                        bkg_substraction_resolution: float = 10,
                        bkg_polynom_degree: int = 3,
-                       pad_size: int = None,
-                       window: Callable = None
+                       bkg_intervals: Iterable | None = None,
+                       pad_size: int | None  = None,
+                       window: Callable | None = None
                        ):
 
         '''
         Args:
             light_curve (LightCurve): light curve object
             interval_t90 (tuple, optional): time interval for t90. If None, uses 2 and 3 quartile of time
             bkg_substraction_resolution (float, optional): background substraction resolution, defaults to 10
@@ -75,16 +76,19 @@
             window (function, optional): window function, that applies to signal, defaults to None
         '''
         self.light_curve = light_curve
 
         if interval_t90 is None:
             interval_t90 = (self.light_curve.times[0]/2,self.light_curve.times[-1]/2)
         
-        bkg_intervals = [(self.light_curve.times[0]-self.light_curve.resolution,interval_t90[0]),
+        if bkg_intervals is None:
+            bkg_intervals = [(self.light_curve.times[0]-self.light_curve.resolution,interval_t90[0]),
                          (interval_t90[1],self.light_curve.times[-1]+self.light_curve.resolution)]
+        else:
+            bkg_intervals = bkg_intervals
         
         self.bkg_intervals = bkg_intervals
         self.interval_t90 = interval_t90
 
         rebined_param = np.polyfit(self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).times,self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).signal,bkg_polynom_degree)
         rebined_param = rebined_param * (self.light_curve.original_resolution/self.light_curve.resolution)
         self.rebined_param = rebined_param
```

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.1.0/src/pygrb_lc/light_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,16 +103,16 @@
         Auxiliary method for rebining the light curve
 
         '''
         if binning is None:
             # binning = np.linspace(times[0]+bin_duration,
             #                       times[-1]-bin_duration,
             #                       num=int(((times[-1]-resolution) - (times[0]+resolution))/bin_duration))
-            N_new_bins = int(np.floor((times[-1] - times[0] + 2*resolution)/bin_duration)+1)
-            binning = times[0] - resolution + np.linspace(0, N_new_bins*bin_duration, num = N_new_bins+1)
+            N_new_bins = int(np.floor((times[-1] - times[0] + resolution)/bin_duration)+1)
+            binning = times[0] - resolution/2 + np.linspace(0, N_new_bins*bin_duration, num = N_new_bins+1)
             
         new_times = binning[:-1] + bin_duration/2
         # fill the time error array
         new_times_err = np.ones_like(new_times)*bin_duration/2
         # determine the number of counts in each bin
         new_counts = np.histogram(times, bins=binning)[0]
         # determine the signal in each bin
@@ -230,22 +230,22 @@
         Args:
             data (np.array): data array with shape (n_samples,n_channels), where n_channels is 2 or 4
         '''
         if data.shape[1] == 2:
             self.original_times = data[:,0]
             self.original_signal = data[:,1]
             
-            self.original_resolution = round(np.mean(self.original_times[1:] - self.original_times[:-1]),3) # determine size of time window
+            self.original_resolution = round(np.median(self.original_times[1:] - self.original_times[:-1]),3) # determine size of time window
             self._reset_light_curve()
         elif data.shape[1] == 4:
             self.original_times = data[:,0]
             self.original_signal = data[:,2]
             
             self.times = self.original_times
-            self.original_resolution = round(np.mean(self.times[1:] - self.times[:-1]),3) # determine size of time window
+            self.original_resolution = round(np.median(self.times[1:] - self.times[:-1]),3) # determine size of time window
             self.times_err = data[:,1]
             self.signal = self.original_signal
             self.signal_err = data[:,3]
             self.resolution = self.original_resolution
 
     @classmethod
     def load(cls,filename: str):
@@ -711,15 +711,15 @@
 
 def plot_gbm_all_detectors(center_time: str, duration: float, binning: float = 0.5, **kwargs):
     detector_list = [x for x in GBM_DETECTORS if x[0] == 'n']
     data = {}
 
     fig, ax = plt.subplots(4,3,figsize=(30,30))
     ax = ax.reshape(-1,)
-    for i, detector in enumerate(detector_list[:-2]):
+    for i, detector in enumerate(detector_list):
         lc = GBM_LightCurve(center_time, [detector], duration = duration, **kwargs)
         lc.rebin(binning).plot(ax=ax[i], label = detector)
         signal = lc.signal
         ax[i].axhline(np.mean(signal),color = 'blue')
         ax[i].axhline(np.mean(signal)+3*np.std(signal),color = 'green')
         ax[i].axhline(np.mean(signal)-3*np.std(signal),color = 'green')
         ax[i].legend()
```

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc/time.py` & `pygrb_lc-0.1.0/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc/utils.py` & `pygrb_lc-0.1.0/src/pygrb_lc/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,18 @@
         all_heads = [th.get_text() for th in all_th]
         for tr in table.find_all('tr'):
             all_th = tr.find_all('th')
             if all_th:
                 continue
             all_td = tr.find_all('td')
             data.append([extract_number(td.get_text().strip()) for td in all_td])
-    return pd.DataFrame(data, columns = all_heads)
+    if len(all_heads) > 1:
+        return pd.DataFrame(data, columns = all_heads)
+    else:
+        return pd.DataFrame(data[1:], columns = data[0])
 
 def retry(expr, tries = 5):
     '''
     Function to retry expression if it fails
     Args:
         expr: expression to retry
         tries: number of tries
```

### Comparing `pygrb_lc-0.0.9/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.1.0/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb-lc
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.0.9/tests/test_utils.py` & `pygrb_lc-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

