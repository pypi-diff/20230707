# Comparing `tmp/spikeinterface-gui-0.6.0.tar.gz` & `tmp/spikeinterface-gui-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikeinterface-gui-0.6.0.tar", last modified: Fri Feb 10 16:08:21 2023, max compression
+gzip compressed data, was "spikeinterface-gui-0.7.0.tar", last modified: Fri Jul  7 13:57:10 2023, max compression
```

## Comparing `spikeinterface-gui-0.6.0.tar` & `spikeinterface-gui-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:08:21.154644 spikeinterface-gui-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-02-10 16:08:21.154644 spikeinterface-gui-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 16:08:21.154644 spikeinterface-gui-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:08:21.154644 spikeinterface-gui-0.6.0/spikeinterface_gui/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/crosscorrelogramview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/isiview.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/myqt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/ndscatterview.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/pairlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/probeview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/similarityview.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/spikeamplitudeview.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/spikelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/traceview.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/unitlist.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/viewlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/waveformheatmapview.py
--rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-02-10 16:07:34.000000 spikeinterface-gui-0.6.0/spikeinterface_gui/waveformview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:08:21.154644 spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-02-10 16:08:21.000000 spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-10 16:08:21.000000 spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 16:08:21.000000 spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-10 16:08:21.000000 spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-10 16:08:21.000000 spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-10 16:08:21.000000 spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:10.643542 spikeinterface-gui-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-07 13:57:10.643542 spikeinterface-gui-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:57:10.643542 spikeinterface-gui-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:10.643542 spikeinterface-gui-0.7.0/spikeinterface_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/crosscorrelogramview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/isiview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/myqt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/ndscatterview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/pairlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/probeview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/similarityview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/spikeamplitudeview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/spikelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/traceview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/unitlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/viewlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/waveformheatmapview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-07-07 13:56:18.000000 spikeinterface-gui-0.7.0/spikeinterface_gui/waveformview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:10.643542 spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-07 13:57:10.000000 spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-07 13:57:10.000000 spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:57:10.000000 spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 13:57:10.000000 spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-07 13:57:10.000000 spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 13:57:10.000000 spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/top_level.txt
```

### Comparing `spikeinterface-gui-0.6.0/LICENSE` & `spikeinterface-gui-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/PKG-INFO` & `spikeinterface-gui-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface-gui
-Version: 0.6.0
+Version: 0.7.0
 Summary: Qt GUI for spikeinterface
 Author-email: Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: Homepage, https://github.com/SpikeInterface/spikeinterface-gui
 Project-URL: Repository, https://github.com/SpikeInterface/spikeinterface-gui
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,115 +15,126 @@
 
 # spikeinterface-gui
 
 GUI for spikeinterface objects without data copy.
 
 This is a cross platform interactive viewer to inspect the final results
 and quality of any spike sorter supported by spikeinterface 
-(kilosort, spykingcircus, tridesclous, moutainssort, yass, ironclust, herdinspikes, hdsort, klusta...)
+(kilosort, spykingcircus, tridesclous, mountainssort, yass, ironclust, herdingspikes, hdsort, klusta...)
 
 This interactive GUI offer several views that dynamically refresh other views.
-This allow to very quickly check strenght and wikness of a sorter otuput.
+This allows us to very quickly check the strengths and weaknesses of any sorter output.
 
-Contrary to other viewers (like  phy), this viewer skip the tedious and long step of
-copying and reformating the entire dataset (filetred signal + waveform + PCA) to a particular
-format or folder organisation. This gui is built on top of spike interface objects
+Contrary to other viewers (like  phy), this viewer skips the tedious and long step of
+copying and reformating the entire dataset (filtered signal + waveform + PCA) to a particular
+format or folder organisation. This gui is built on top of spikeinterface objects
 (Recording, Sorting, WaveformExtractor)
-Theses objects are "lazy" and retrieve data on the fly (no copy!).
+These objects are "lazy" and retrieve data on the fly (no copy!).
 And contrary to phy, this is a view only tool : no manual curation at the moment (split/merge/trash have to be done outside).
 
 This viewer internally use Qt (with PySide6, PyQT6 or PyQt5) and pyqtgraph.
-And so, this viewer is local desktop app (old school!!).
-There is a web based viewer work-in-progres [here](https://github.com/magland/sortingview).
+And so, this viewer is a local desktop app (old school!!).
+There is a web based viewer work-in-progress [here](https://github.com/magland/sortingview).
 
 ![screenshot](screenshot.png)
 
 ## Launch
 
-You will need this viewer only and only if you known a bit of [spikeinterface](https://spikeinterface.readthedocs.io/)
+In order to use this viewer you will need to know a bit of [spikeinterface](https://spikeinterface.readthedocs.io/)
 
 ### Step 1 : extract waveforms
 
 You first need to "extract waveform" with spikeinterface
 See help [here](https://spikeinterface.readthedocs.io/en/latest/modules/core/plot_4_waveform_extractor.html#sphx-glr-modules-core-plot-4-waveform-extractor-py)
 
 Note that:
-  * not all waveforms snipet are extracted (See `max_spikes_per_unit`) only some of then
+  * not all waveform snippets are extracted (See `max_spikes_per_unit`) only some of them
   * this step is cached to a folder (and can be reloaded)
-  * this step can be run in parralel (and so quite fast)
-  * optionaly PCa can be compute and displayed
+  * this step can be run in parallel (and so is quite fast)
+  * optionally PCA can be computed and displayed
 
   
 Example:
 
 ```python
 import spikeinterface.full as si
 recording = si.read_XXXX('/path/to/my/recording')
 recording_filtered = si.bandpass_filter(recording)
 sorting = si.run_sorter('YYYYY', recording_filtered)
+
+# extract waveforms 
+# sparse is important because make everything faster!!!
 waveform_folder = '/path/for/my/waveforms'
+job_kwargs = dict(n_jobs=10, chunk_duration='1s', progress_bar=True,)
 we = si.extract_waveforms(
     recording_filtered, sorting, waveform_folder,
     max_spikes_per_unit=500,
     ms_before=1.5, ms_after=2.5,
-    n_jobs=10, total_memory='500M',
-    progress_bar=True,
+    sparse=True,
+    **job_kwargs
 )
-# and optionally compute principal component
-pc = si.compute_principal_components(we,
-    n_components=5,
+# compute the noise level a faster opening in sigui
+si.compute_noise_levels(we)
+
+# optionally compute more stuff using the spikeinterface.postprocessing module
+# principal components, template similarity, spike amplitudes
+# This will enable to display more views
+si.compute_principal_components(we,
+    n_components=3,
     mode='by_channel_local',
     whiten=True)
+si.compute_template_similarity(we,  method='cosine_similarity',
+si.compute_spike_amplitudes(we, **job_kwargs)
 ```
 
 ### Step 2 : open the GUI
 
 With python:
 
 ```python
 import spikeinterface_gui
-# This cerate a Qt app
+# This creates a Qt app
 app = spikeinterface_gui.mkQApp() 
 # reload the waveform folder
 we = si.WaveformExtractor.load_from_folder(waveform_folder)
 # create the mainwindow and show
 win = spikeinterface_gui.MainWindow(we)
 win.show()
 # run the main Qt6 loop
 app.exec_()
 ```
 
-With the commend line
+With the command line
 
-```
+```bash
 sigui /path/for/my/waveforms
 ```
 
 
 ## Install
 
-You need first to install one of this 3 packages (by order of preference):
+You need first to install one of these 3 packages (by order of preference):
   * `pip install PySide6`
   * `pip install PyQt6`
   * `pip install PyQt5`
 
 
 From pypi:
 
 ```bash
 pip install spikeinterface-gui
 ```
 
-From sources:
+From source:
 
 ```bash
 git clone https://github.com/SpikeInterface/spikeinterface-gui.git
 cd spikeinterface-gui
 pip install .
 ```
 
 ## Author
 
 Samuel Garcia, CNRS, Lyon, France
 
-This work is a port of the old `tridesclous.gui` submodule of top of
+This work is a port of the old `tridesclous.gui` submodule on top of
 [spikeinterface](https://github.com/SpikeInterface/spikeinterface).
```

### Comparing `spikeinterface-gui-0.6.0/README.md` & `spikeinterface-gui-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,125 @@
 # spikeinterface-gui
 
 GUI for spikeinterface objects without data copy.
 
 This is a cross platform interactive viewer to inspect the final results
 and quality of any spike sorter supported by spikeinterface 
-(kilosort, spykingcircus, tridesclous, moutainssort, yass, ironclust, herdinspikes, hdsort, klusta...)
+(kilosort, spykingcircus, tridesclous, mountainssort, yass, ironclust, herdingspikes, hdsort, klusta...)
 
 This interactive GUI offer several views that dynamically refresh other views.
-This allow to very quickly check strenght and wikness of a sorter otuput.
+This allows us to very quickly check the strengths and weaknesses of any sorter output.
 
-Contrary to other viewers (like  phy), this viewer skip the tedious and long step of
-copying and reformating the entire dataset (filetred signal + waveform + PCA) to a particular
-format or folder organisation. This gui is built on top of spike interface objects
+Contrary to other viewers (like  phy), this viewer skips the tedious and long step of
+copying and reformating the entire dataset (filtered signal + waveform + PCA) to a particular
+format or folder organisation. This gui is built on top of spikeinterface objects
 (Recording, Sorting, WaveformExtractor)
-Theses objects are "lazy" and retrieve data on the fly (no copy!).
+These objects are "lazy" and retrieve data on the fly (no copy!).
 And contrary to phy, this is a view only tool : no manual curation at the moment (split/merge/trash have to be done outside).
 
 This viewer internally use Qt (with PySide6, PyQT6 or PyQt5) and pyqtgraph.
-And so, this viewer is local desktop app (old school!!).
-There is a web based viewer work-in-progres [here](https://github.com/magland/sortingview).
+And so, this viewer is a local desktop app (old school!!).
+There is a web based viewer work-in-progress [here](https://github.com/magland/sortingview).
 
 ![screenshot](screenshot.png)
 
 ## Launch
 
-You will need this viewer only and only if you known a bit of [spikeinterface](https://spikeinterface.readthedocs.io/)
+In order to use this viewer you will need to know a bit of [spikeinterface](https://spikeinterface.readthedocs.io/)
 
 ### Step 1 : extract waveforms
 
 You first need to "extract waveform" with spikeinterface
 See help [here](https://spikeinterface.readthedocs.io/en/latest/modules/core/plot_4_waveform_extractor.html#sphx-glr-modules-core-plot-4-waveform-extractor-py)
 
 Note that:
-  * not all waveforms snipet are extracted (See `max_spikes_per_unit`) only some of then
+  * not all waveform snippets are extracted (See `max_spikes_per_unit`) only some of them
   * this step is cached to a folder (and can be reloaded)
-  * this step can be run in parralel (and so quite fast)
-  * optionaly PCa can be compute and displayed
+  * this step can be run in parallel (and so is quite fast)
+  * optionally PCA can be computed and displayed
 
   
 Example:
 
 ```python
 import spikeinterface.full as si
 recording = si.read_XXXX('/path/to/my/recording')
 recording_filtered = si.bandpass_filter(recording)
 sorting = si.run_sorter('YYYYY', recording_filtered)
+
+# extract waveforms 
+# sparse is important because make everything faster!!!
 waveform_folder = '/path/for/my/waveforms'
+job_kwargs = dict(n_jobs=10, chunk_duration='1s', progress_bar=True,)
 we = si.extract_waveforms(
     recording_filtered, sorting, waveform_folder,
     max_spikes_per_unit=500,
     ms_before=1.5, ms_after=2.5,
-    n_jobs=10, total_memory='500M',
-    progress_bar=True,
+    sparse=True,
+    **job_kwargs
 )
-# and optionally compute principal component
-pc = si.compute_principal_components(we,
-    n_components=5,
+# compute the noise level a faster opening in sigui
+si.compute_noise_levels(we)
+
+# optionally compute more stuff using the spikeinterface.postprocessing module
+# principal components, template similarity, spike amplitudes
+# This will enable to display more views
+si.compute_principal_components(we,
+    n_components=3,
     mode='by_channel_local',
     whiten=True)
+si.compute_template_similarity(we,  method='cosine_similarity',
+si.compute_spike_amplitudes(we, **job_kwargs)
 ```
 
 ### Step 2 : open the GUI
 
 With python:
 
 ```python
 import spikeinterface_gui
-# This cerate a Qt app
+# This creates a Qt app
 app = spikeinterface_gui.mkQApp() 
 # reload the waveform folder
 we = si.WaveformExtractor.load_from_folder(waveform_folder)
 # create the mainwindow and show
 win = spikeinterface_gui.MainWindow(we)
 win.show()
 # run the main Qt6 loop
 app.exec_()
 ```
 
-With the commend line
+With the command line
 
-```
+```bash
 sigui /path/for/my/waveforms
 ```
 
 
 ## Install
 
-You need first to install one of this 3 packages (by order of preference):
+You need first to install one of these 3 packages (by order of preference):
   * `pip install PySide6`
   * `pip install PyQt6`
   * `pip install PyQt5`
 
 
 From pypi:
 
 ```bash
 pip install spikeinterface-gui
 ```
 
-From sources:
+From source:
 
 ```bash
 git clone https://github.com/SpikeInterface/spikeinterface-gui.git
 cd spikeinterface-gui
 pip install .
 ```
 
 ## Author
 
 Samuel Garcia, CNRS, Lyon, France
 
-This work is a port of the old `tridesclous.gui` submodule of top of
+This work is a port of the old `tridesclous.gui` submodule on top of
 [spikeinterface](https://github.com/SpikeInterface/spikeinterface).
```

### Comparing `spikeinterface-gui-0.6.0/pyproject.toml` & `spikeinterface-gui-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "spikeinterface-gui"
-version = '0.6.0'
+version = '0.7.0'
 authors = [
   { name="Samuel Garcia", email="sam.garcia.die@gmail.com" },
 ]
 
 description = "Qt GUI for spikeinterface"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "spikeinterface[full]>=0.97.0",
+    "spikeinterface[full]>=0.98.0",
     "pyqtgraph",
 ]
 
 [project.urls]
 Homepage = "https://github.com/SpikeInterface/spikeinterface-gui"
 Repository = "https://github.com/SpikeInterface/spikeinterface-gui"
```

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/base.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/base.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/controller.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,17 +108,17 @@
         
         num_spikes = np.sum([e[0].size for e in all_spikes])
         
         # make internal spike vector
         self.spikes = np.zeros(num_spikes, dtype=spike_dtype)
         # TODO : align fields with spikeinterface !!!!!!
         spikes_ = self.we.sorting.to_spike_vector()
-        self.spikes['sample_index'] = spikes_['sample_ind']
-        self.spikes['unit_index'] = spikes_['unit_ind']
-        self.spikes['segment_index'] = spikes_['segment_ind']
+        self.spikes['sample_index'] = spikes_['sample_index']
+        self.spikes['unit_index'] = spikes_['unit_index']
+        self.spikes['segment_index'] = spikes_['segment_index']
         
         self.num_spikes = {unit_id: 0 for unit_id in self.unit_ids}
         self._spike_index_by_units = {unit_id: [] for unit_id in self.unit_ids}
         for segment_index in range(self.num_segments):
             i0 = np.searchsorted(self.spikes['segment_index'], segment_index)
             i1 = np.searchsorted(self.spikes['segment_index'], segment_index + 1)
             for unit_index, unit_id in enumerate(self.unit_ids):
@@ -235,28 +235,14 @@
             raise NotImplemented
             # TODO get with parent recording the non process recording
             pass
         kargs['return_scaled'] = self.we.return_scaled
         traces = rec.get_traces(**kargs)
         return traces
     
-    #~ def estimate_noise(self):
-        #~ duration_s = 1
-        #~ seg_num = 0
-        #~ end_frame = min(int(duration_s * self.sampling_frequency), self.get_num_samples(seg_num))
-        #~ sigs = self.get_traces(segment_index=seg_num, start_frame=0, end_frame=end_frame)
-
-        #~ self.med = np.median(sigs, axis=0).astype('float32')
-        #~ self.mad = np.median(np.abs(sigs - self.med),axis=0).astype('float32') * 1.4826
-        
-        #~ return self.med, self.mad
-        
-        
-
-
     def get_contact_location(self):
         location = self.we.recording.get_channel_locations()
         return location
     
     def get_waveform_sweep(self):
         return self.we.nbefore, self.we.nafter
```

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/crosscorrelogramview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/crosscorrelogramview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/isiview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/isiview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/main.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/main.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/mainwindow.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/myqt.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/myqt.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/ndscatterview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/ndscatterview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/pairlist.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/pairlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/probeview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/probeview.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class ProbeView(WidgetBase):
     _params = [
             #~ {'name': 'colormap', 'type': 'list', 'value': 'inferno', 'values': ['inferno', 'summer', 'viridis', 'jet'] },
             {'name': 'show_channel_id', 'type': 'bool', 'value': False},
             {'name': 'radius', 'type': 'float', 'value': 40.},
             {'name': 'roi_change_channel_visibility', 'type': 'bool', 'value': True},
-            {'name': 'roi_change_unit_visibility', 'type': 'bool', 'value': True},
+            {'name': 'roi_change_unit_visibility', 'type': 'bool', 'value': False},
             {'name': 'auto_zoom_on_unit_selection', 'type': 'bool', 'value': True},
             {'name': 'method_localize_unit', 'type': 'list', 'limits': possible_localization_methods},
             
             
         ]
     
     _need_compute = True
@@ -156,38 +156,44 @@
         if self.params['show_channel_id']:
             for label in self.channel_labels:
                 label.show()
         else:
             for label in self.channel_labels:
                 label.hide()
             
-        
+    
+    def update_channel_visibility_from_roi(self, emit_signals=False):
+            r = self.roi.state['size'][0] / 2
+            x = self.roi.state['pos'].x() + r
+            y = self.roi.state['pos'].y() + r
+        
+            dist = np.sqrt(np.sum((self.contact_positions - np.array([[x, y]]))**2, axis=1))
+            visible_channel_inds,  = np.nonzero(dist < r)
+            pos = self.contact_positions[visible_channel_inds, :]
+            order = np.lexsort((-pos[:, 0], pos[:, 1], ))[::-1]
+            visible_channel_inds = visible_channel_inds[order]
+            self.controller.set_channel_visibility(visible_channel_inds)
+            if emit_signals:
+                self.channel_visibility_changed.emit()
+
     
     def on_roi_change(self, emit_signals=True):
         
         r = self.roi.state['size'][0] / 2
         x = self.roi.state['pos'].x() + r
         y = self.roi.state['pos'].y() + r
         
         self.params.blockSignals(True)
         self.params['radius'] = r
         self.params.blockSignals(False)
         
         if emit_signals:
             self.roi.blockSignals(True)
             if self.params['roi_change_channel_visibility']:
-                #~ t0 = time.perf_counter()
-                dist = np.sqrt(np.sum((self.contact_positions - np.array([[x, y]]))**2, axis=1))
-                visible_channel_inds,  = np.nonzero(dist < r)
-                order = np.argsort(dist[visible_channel_inds])
-                visible_channel_inds = visible_channel_inds[order]
-                self.controller.set_channel_visibility(visible_channel_inds)
-                self.channel_visibility_changed.emit()
-                #~ t1 = time.perf_counter()
-                #~ print(' probe view change_channel_visibility', t1-t0)
+                self.update_channel_visibility_from_roi(emit_signals=True)
 
             if self.params['roi_change_unit_visibility']:
                 #~ t0 = time.perf_counter()
                 dist = np.sqrt(np.sum((self.controller.unit_positions - np.array([[x, y]]))**2, axis=1))
                 for unit_index, unit_id in enumerate(self.controller.unit_ids):
                     self.controller.unit_visible_dict[unit_id] = (dist[unit_index] < r)
                 #~ t1 = time.perf_counter()
@@ -208,14 +214,15 @@
             unit_index  = np.nonzero(visible_mask)[0][0]
             x, y = self.controller.unit_positions[unit_index, :]
             radius = self.params['radius']
             self.roi.blockSignals(True)
             self.roi.setPos(x - radius, y - radius)
             self.roi.blockSignals(False)
             self.on_roi_change(emit_signals=False)
+            self.update_channel_visibility_from_roi(emit_signals=True)
         
         # change scatter pen for selection
         pen = [pg.mkPen('magenta', width=4)
                     if self.controller.unit_visible_dict[u] else pg.mkPen('black', width=4)
                     for u in self.controller.unit_ids]
         self.scatter.setPen(pen)
```

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/similarityview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/similarityview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/spikeamplitudeview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/spikeamplitudeview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/spikelist.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/spikelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .base import WidgetBase
 
 
 _columns = ['num', 'unit_id', 'segment', 'sample_index', 'channel_index', 'included_in_pc']
 
 class SpikeModel(QT.QAbstractItemModel):
+
     def __init__(self, parent =None, controller=None):
         QT.QAbstractItemModel.__init__(self,parent)
         self.controller = controller
         self.refresh_colors()
         
         self.visible_ind = self.controller.get_indices_spike_visible()
     
@@ -94,14 +95,19 @@
     
     def refresh(self):
         self.visible_ind = self.controller.get_indices_spike_visible()
         self.layoutChanged.emit()
 
 
 class SpikeListView(WidgetBase):
+    _params = [
+            {'name': 'select_change_channel_visibility', 'type': 'bool', 'value': False},
+        ]    
+    
+    
     def __init__(self,controller=None, parent=None):
         WidgetBase.__init__(self, parent=parent, controller=controller)
         self.controller = controller
         
         self.layout = QT.QVBoxLayout()
         self.setLayout(self.layout)
         
@@ -149,15 +155,15 @@
         inds = []
         for index in self.tree.selectedIndexes():
             if index.column() == 0:
                 ind = self.model.visible_ind[index.row()]
                 inds.append(ind)
         self.controller.set_indices_spike_selected(inds)
         self.spike_selection_changed.emit()
-        if len(inds) == 1:
+        if len(inds) == 1 and self.params['select_change_channel_visibility']:
             # also change channel for centering trace view.
             sparsity_mask = self.controller.get_sparsity_mask()
             unit_index = self.controller.spikes[inds[0]]['unit_index']
             visible_channel_inds, = np.nonzero(sparsity_mask[unit_index, :])
 
             # check ifchannel visibility must be changed
             if not np.all(np.in1d(visible_channel_inds, self.controller.visible_channel_inds)):
```

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/tools.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/traceview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/traceview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/unitlist.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/unitlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/viewlist.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/viewlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/waveformheatmapview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/waveformheatmapview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui/waveformview.py` & `spikeinterface-gui-0.7.0/spikeinterface_gui/waveformview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/PKG-INFO` & `spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface-gui
-Version: 0.6.0
+Version: 0.7.0
 Summary: Qt GUI for spikeinterface
 Author-email: Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: Homepage, https://github.com/SpikeInterface/spikeinterface-gui
 Project-URL: Repository, https://github.com/SpikeInterface/spikeinterface-gui
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,115 +15,126 @@
 
 # spikeinterface-gui
 
 GUI for spikeinterface objects without data copy.
 
 This is a cross platform interactive viewer to inspect the final results
 and quality of any spike sorter supported by spikeinterface 
-(kilosort, spykingcircus, tridesclous, moutainssort, yass, ironclust, herdinspikes, hdsort, klusta...)
+(kilosort, spykingcircus, tridesclous, mountainssort, yass, ironclust, herdingspikes, hdsort, klusta...)
 
 This interactive GUI offer several views that dynamically refresh other views.
-This allow to very quickly check strenght and wikness of a sorter otuput.
+This allows us to very quickly check the strengths and weaknesses of any sorter output.
 
-Contrary to other viewers (like  phy), this viewer skip the tedious and long step of
-copying and reformating the entire dataset (filetred signal + waveform + PCA) to a particular
-format or folder organisation. This gui is built on top of spike interface objects
+Contrary to other viewers (like  phy), this viewer skips the tedious and long step of
+copying and reformating the entire dataset (filtered signal + waveform + PCA) to a particular
+format or folder organisation. This gui is built on top of spikeinterface objects
 (Recording, Sorting, WaveformExtractor)
-Theses objects are "lazy" and retrieve data on the fly (no copy!).
+These objects are "lazy" and retrieve data on the fly (no copy!).
 And contrary to phy, this is a view only tool : no manual curation at the moment (split/merge/trash have to be done outside).
 
 This viewer internally use Qt (with PySide6, PyQT6 or PyQt5) and pyqtgraph.
-And so, this viewer is local desktop app (old school!!).
-There is a web based viewer work-in-progres [here](https://github.com/magland/sortingview).
+And so, this viewer is a local desktop app (old school!!).
+There is a web based viewer work-in-progress [here](https://github.com/magland/sortingview).
 
 ![screenshot](screenshot.png)
 
 ## Launch
 
-You will need this viewer only and only if you known a bit of [spikeinterface](https://spikeinterface.readthedocs.io/)
+In order to use this viewer you will need to know a bit of [spikeinterface](https://spikeinterface.readthedocs.io/)
 
 ### Step 1 : extract waveforms
 
 You first need to "extract waveform" with spikeinterface
 See help [here](https://spikeinterface.readthedocs.io/en/latest/modules/core/plot_4_waveform_extractor.html#sphx-glr-modules-core-plot-4-waveform-extractor-py)
 
 Note that:
-  * not all waveforms snipet are extracted (See `max_spikes_per_unit`) only some of then
+  * not all waveform snippets are extracted (See `max_spikes_per_unit`) only some of them
   * this step is cached to a folder (and can be reloaded)
-  * this step can be run in parralel (and so quite fast)
-  * optionaly PCa can be compute and displayed
+  * this step can be run in parallel (and so is quite fast)
+  * optionally PCA can be computed and displayed
 
   
 Example:
 
 ```python
 import spikeinterface.full as si
 recording = si.read_XXXX('/path/to/my/recording')
 recording_filtered = si.bandpass_filter(recording)
 sorting = si.run_sorter('YYYYY', recording_filtered)
+
+# extract waveforms 
+# sparse is important because make everything faster!!!
 waveform_folder = '/path/for/my/waveforms'
+job_kwargs = dict(n_jobs=10, chunk_duration='1s', progress_bar=True,)
 we = si.extract_waveforms(
     recording_filtered, sorting, waveform_folder,
     max_spikes_per_unit=500,
     ms_before=1.5, ms_after=2.5,
-    n_jobs=10, total_memory='500M',
-    progress_bar=True,
+    sparse=True,
+    **job_kwargs
 )
-# and optionally compute principal component
-pc = si.compute_principal_components(we,
-    n_components=5,
+# compute the noise level a faster opening in sigui
+si.compute_noise_levels(we)
+
+# optionally compute more stuff using the spikeinterface.postprocessing module
+# principal components, template similarity, spike amplitudes
+# This will enable to display more views
+si.compute_principal_components(we,
+    n_components=3,
     mode='by_channel_local',
     whiten=True)
+si.compute_template_similarity(we,  method='cosine_similarity',
+si.compute_spike_amplitudes(we, **job_kwargs)
 ```
 
 ### Step 2 : open the GUI
 
 With python:
 
 ```python
 import spikeinterface_gui
-# This cerate a Qt app
+# This creates a Qt app
 app = spikeinterface_gui.mkQApp() 
 # reload the waveform folder
 we = si.WaveformExtractor.load_from_folder(waveform_folder)
 # create the mainwindow and show
 win = spikeinterface_gui.MainWindow(we)
 win.show()
 # run the main Qt6 loop
 app.exec_()
 ```
 
-With the commend line
+With the command line
 
-```
+```bash
 sigui /path/for/my/waveforms
 ```
 
 
 ## Install
 
-You need first to install one of this 3 packages (by order of preference):
+You need first to install one of these 3 packages (by order of preference):
   * `pip install PySide6`
   * `pip install PyQt6`
   * `pip install PyQt5`
 
 
 From pypi:
 
 ```bash
 pip install spikeinterface-gui
 ```
 
-From sources:
+From source:
 
 ```bash
 git clone https://github.com/SpikeInterface/spikeinterface-gui.git
 cd spikeinterface-gui
 pip install .
 ```
 
 ## Author
 
 Samuel Garcia, CNRS, Lyon, France
 
-This work is a port of the old `tridesclous.gui` submodule of top of
+This work is a port of the old `tridesclous.gui` submodule on top of
 [spikeinterface](https://github.com/SpikeInterface/spikeinterface).
```

### Comparing `spikeinterface-gui-0.6.0/spikeinterface_gui.egg-info/SOURCES.txt` & `spikeinterface-gui-0.7.0/spikeinterface_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

