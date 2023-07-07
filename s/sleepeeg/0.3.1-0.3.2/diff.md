# Comparing `tmp/sleepeeg-0.3.1.tar.gz` & `tmp/sleepeeg-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepeeg-0.3.1.tar", last modified: Wed Jun 28 12:55:18 2023, max compression
+gzip compressed data, was "sleepeeg-0.3.2.tar", last modified: Fri Jul  7 12:13:45 2023, max compression
```

## Comparing `sleepeeg-0.3.1.tar` & `sleepeeg-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 12:55:18.991817 sleepeeg-0.3.1/
--rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1728 2023-06-28 12:55:18.990816 sleepeeg-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 12:55:18.955908 sleepeeg-0.3.1/docs/
--rw-rw-rw-   0        0        0     2433 2023-06-24 10:09:30.000000 sleepeeg-0.3.1/docs/conf.py
--rw-rw-rw-   0        0        0      839 2023-06-28 12:52:35.000000 sleepeeg-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 12:55:18.992811 sleepeeg-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 12:55:18.970869 sleepeeg-0.3.1/sleepeeg/
--rw-rw-rw-   0        0        0    48389 2023-06-28 12:51:11.000000 sleepeeg-0.3.1/sleepeeg/base.py
--rw-rw-rw-   0        0        0    12311 2023-06-24 12:39:28.000000 sleepeeg-0.3.1/sleepeeg/dashboard.py
--rw-rw-rw-   0        0        0    28327 2023-06-24 12:51:40.000000 sleepeeg-0.3.1/sleepeeg/pipeline.py
--rw-rw-rw-   0        0        0     2005 2023-06-24 08:52:40.000000 sleepeeg-0.3.1/sleepeeg/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:55:18.988821 sleepeeg-0.3.1/sleepeeg.egg-info/
--rw-rw-rw-   0        0        0     1728 2023-06-28 12:55:18.000000 sleepeeg-0.3.1/sleepeeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-28 12:55:18.000000 sleepeeg-0.3.1/sleepeeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 12:55:18.000000 sleepeeg-0.3.1/sleepeeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-06-28 12:55:18.000000 sleepeeg-0.3.1/sleepeeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-28 12:55:18.000000 sleepeeg-0.3.1/sleepeeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.069857 sleepeeg-0.3.2/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1728 2023-07-07 12:13:45.069857 sleepeeg-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.035898 sleepeeg-0.3.2/docs/
+-rw-rw-rw-   0        0        0     2433 2023-06-24 10:09:30.000000 sleepeeg-0.3.2/docs/conf.py
+-rw-rw-rw-   0        0        0      839 2023-07-07 12:10:05.000000 sleepeeg-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:13:45.070804 sleepeeg-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.049894 sleepeeg-0.3.2/sleepeeg/
+-rw-rw-rw-   0        0        0    48389 2023-06-28 12:51:11.000000 sleepeeg-0.3.2/sleepeeg/base.py
+-rw-rw-rw-   0        0        0    12432 2023-07-07 11:38:44.000000 sleepeeg-0.3.2/sleepeeg/dashboard.py
+-rw-rw-rw-   0        0        0    28533 2023-07-07 12:11:25.000000 sleepeeg-0.3.2/sleepeeg/pipeline.py
+-rw-rw-rw-   0        0        0     2005 2023-06-24 08:52:40.000000 sleepeeg-0.3.2/sleepeeg/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.067844 sleepeeg-0.3.2/sleepeeg.egg-info/
+-rw-rw-rw-   0        0        0     1728 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/top_level.txt
```

### Comparing `sleepeeg-0.3.1/LICENSE` & `sleepeeg-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.1/PKG-INFO` & `sleepeeg-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.3.1
+Version: 0.3.2
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

### Comparing `sleepeeg-0.3.1/README.md` & `sleepeeg-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.1/docs/conf.py` & `sleepeeg-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.1/pyproject.toml` & `sleepeeg-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["notebooks"]  # empty by default
 
 [project]
 name = "sleepeeg"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     {name = "Gennadiy Belonosov", email = "gennadiyb@mail.tau.ac.il"},
 ]
 description = "Sleep EEG preprocessing and analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
```

### Comparing `sleepeeg-0.3.1/sleepeeg/base.py` & `sleepeeg-0.3.2/sleepeeg/base.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.1/sleepeeg/dashboard.py` & `sleepeeg-0.3.2/sleepeeg/dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,30 +69,30 @@
 
     return sfreq, fmin, fmax, notch_freqs
 
 
 def _hypno_psd(
     s_pipe,
     sleep_stages,
-    ref_channels,
     hypno_psd_pick,
     ax_hypno,
     ax_psd,
     min_psd,
     max_psd,
+    rba,
 ):
     s_pipe.compute_psds_per_stage(
         sleep_stages=sleep_stages,
-        reference=ref_channels,
+        reference=None,
         method="welch",
         fmin=0,
         fmax=25,
         save=False,
         picks="eeg",
-        reject_by_annotation=True,
+        reject_by_annotation=rba,
         n_jobs=-1,
         verbose=False,
         n_fft=2048,
         n_per_seg=768,
         n_overlap=512,
         window="hamming",
     )
@@ -104,25 +104,27 @@
     s_pipe.plot_hypnospectrogram(
         picks=hypno_psd_pick,
         win_sec=win_sec,
         freq_range=(0, 25),
         cmap="Spectral_r",
         overlap=True,
         axis=ax_hypno,
+        reject_by_annotation="NaN" if rba else None,
     )
     r = max_psd - min_psd
     s_pipe.plot_psds(
         picks=hypno_psd_pick,
         psd_range=(min_psd - 0.1 * r, max_psd + 0.1 * r),
         freq_range=(0, 25),
         dB=True,
         xscale="linear",
         axis=ax_psd,
         legend_args=dict(loc="upper right", fontsize="medium"),
     )
+    ax_psd.axvspan(0, s_pipe.mne_raw.info["highpass"], alpha=0.3, color="gray")
     return min_psd, max_psd
 
 
 def _topo(s_pipe, ref_channels, sleep_stages, topo_axes, topo_lims):
     if len(sleep_stages) == 1:
         stages = ["All"] * 4
         topo_axes[0, 0].set_title(f"Alpha (8-12 Hz)")
@@ -192,16 +194,16 @@
 
 
 def create_dashboard(
     subject_code: str | os.PathLike,
     path_to_eeg: str | os.PathLike,
     path_to_hypnogram: str | os.PathLike | None,
     hypno_freq: float | None,
-    path_to_bad_channels: str | os.PathLike,
-    path_to_annotations: str | os.PathLike,
+    path_to_bad_channels: str | os.PathLike | None,
+    path_to_annotations: str | os.PathLike | None,
     output_dir: str | os.PathLike,
     reference: str,
     resampling_freq: float | None = None,
     bandpass_filter_freqs: Iterable[float | None] = None,
     hypno_psd_pick: Iterable[str] | str = ["E101"],
     path_to_ica_fif: str | os.PathLike = None,
     save_fif: bool = False,
@@ -268,44 +270,51 @@
 
     fig.suptitle(f"Dashboard <{subject_code}>")
     pick = (
         hypno_psd_pick
         if isinstance(hypno_psd_pick, str)
         else ", ".join(str(x) for x in hypno_psd_pick)
     )
-    spectrum_before.suptitle(f"Spectra after filtering ({pick})")
-    spectrum_after.suptitle(f"Spectra after removing bad channels & epochs ({pick})")
+    spectrum_before.suptitle(f"Spectra after interpolating bad channels ({pick})")
+    spectrum_after.suptitle(f"Spectra after rejecting bad data spans ({pick})")
 
     pipe = CleaningPipe(path_to_eeg=path_to_eeg, output_dir=output_dir)
 
     sfreq, fmin, fmax, notch_freqs = _filter(
         pipe,
         resampling_freq,
         bandpass_filter_freqs[0],
         bandpass_filter_freqs[1],
     )
 
     pipe.set_eeg_reference(ref_channels=ref_channels)
 
+    if path_to_bad_channels is not None:
+        pipe.read_bad_channels(path=path_to_bad_channels)
+        bads = pipe.mne_raw.info["bads"]
+        pipe.interpolate_bads(reset_bads=True)
+    else:
+        from ast import literal_eval
+
+        bads = literal_eval(pipe.mne_raw.info["description"])
+
     s_pipe, sleep_stages = _init_s_pipe(pipe, path_to_hypnogram, hypno_freq)
     min_psd, max_psd = _hypno_psd(
         s_pipe,
         sleep_stages,
-        ref_channels,
         hypno_psd_pick,
         hypno_before,
         psd_before,
         min_psd=None,
         max_psd=None,
+        rba=False,
     )
 
-    pipe.read_bad_channels(path=path_to_bad_channels)
-    bads = pipe.mne_raw.info["bads"]
-    pipe.interpolate_bads(reset_bads=True)
-    pipe.read_annotations(path=path_to_annotations)
+    if path_to_annotations is not None:
+        pipe.read_annotations(path=path_to_annotations)
 
     is_ica = False
     if path_to_ica_fif:
         from sleepeeg.pipeline import ICAPipe
 
         is_ica = True
         pipe = ICAPipe(prec_pipe=pipe, path_to_ica=path_to_ica_fif)
@@ -323,30 +332,24 @@
         pointsize=20,
         linewidth=1.5,
     )
 
     recording_time = time.strftime(
         "%H:%M:%S", time.gmtime(pipe.mne_raw.n_times / pipe.sf)
     )
-    df = pipe.mne_raw.annotations.to_data_frame()
-    bad_epochs_percent = round(
-        100
-        * (df[df.description.str.contains("bad", case=False)].duration.sum() * pipe.sf)
-        / pipe.mne_raw.n_times,
-        2,
-    )
+
     interpolated_channels_percent = round(
         100 * len(interpolated) / len(pick_types(pipe.mne_raw.info, eeg=True)), 2
     )
 
     textstr = "\n\n".join(
         (
             f"Recording duration: {recording_time}",
             f"Sampling frequency: {sfreq} Hz",
-            f"Bad epochs: {bad_epochs_percent}%",
+            f"Bad data spans: {pipe.bad_data_percent}%",
             f"Interpolated channels: {interpolated_channels_percent}%",
             f"EEG reference: {reference}",
             f"Band-pass filter: [{round(fmin, 2)}, {round(fmax, 2)}] Hz",
             f"Notch filter: {set(notch_freqs)} Hz",
             f"ICA performed: {'Yes' if is_ica else 'No'}",
             f"Adaptive topomaps: {'Yes' if is_adaptive_topo else 'No'}",
         )
@@ -363,18 +366,18 @@
     )
 
     s_pipe, sleep_stages = _init_s_pipe(pipe, path_to_hypnogram, hypno_freq)
 
     _hypno_psd(
         s_pipe,
         sleep_stages,
-        ref_channels,
         hypno_psd_pick,
         hypno_after,
         psd_after,
         min_psd,
         max_psd,
+        rba=True,
     )
 
     _topo(s_pipe, ref_channels, sleep_stages, topo_axes, topomap_cbar_limits)
 
     fig.savefig(f"{output_dir}/dashboard_{subject_code}.png")
```

### Comparing `sleepeeg-0.3.1/sleepeeg/pipeline.py` & `sleepeeg-0.3.2/sleepeeg/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,14 +352,15 @@
         self,
         picks: str | Iterable[str] = ("E101",),
         win_sec: float = 10,
         trimperc: float = 2.5,
         freq_range: tuple = (0, 40),
         cmap: str = "Spectral_r",
         overlap: bool = False,
+        reject_by_annotation: None | str = "NaN",
         save: bool = False,
         axis: plt.Axes = None,
     ):
         """Plots hypnogram and spectrogram.
 
         Adapted from YASA.
 
@@ -370,20 +371,24 @@
             trimperc: The amount of data to trim on both ends of the distribution
                 when normalizing the colormap. Defaults to 2.5.
             freq_range: Range of x axis on spectrogram plot. Defaults to (0, 40).
             cmap: Matplotlib colormap. :std:doc:`mpl:tutorials/colors/colormaps`.
                 Defaults to "Spectral_r".
             overlap: Whether to plot hypnogram over the spectrogram or on top of it.
                 Defaults to False.
+            reject_by_annotation: Whether to reject the annotations for the spectrogram computation.
+                Can be 'NaN', 'omit' or None. Defaults to 'NaN'.
             save: Whether to save the figure. Defaults to False.
             axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
         """
         # Import data from the raw mne file.
-        data = self.mne_raw.get_data(picks, units="uV", reject_by_annotation="NaN")[0]
+        data = self.mne_raw.get_data(
+            picks, units="uV", reject_by_annotation=reject_by_annotation
+        )[0]
         # Create a plot figure
         if overlap or self.hypno_up is None:
             if axis is None:
                 fig, axis = plt.subplots(nrows=1, figsize=(12, 4))
 
             im = self.__plot_spectrogram(
                 data,
@@ -397,15 +402,15 @@
             )
             if self.hypno_up is not None:
                 ax_hypno = axis.twinx()
                 self.__plot_hypnogram(self.sf, self.hypno_up, ax_hypno)
             # Add colorbar
             cbar = plt.colorbar(im, ax=axis, shrink=0.95, fraction=0.1, aspect=25)
             cbar.ax.set_ylabel(r"$\mu V^{2}/Hz$ (dB)", rotation=90)
-            return None if axis is not None else fig
+
         else:
             if axis is None:
                 fig, (ax0, ax1) = plt.subplots(
                     nrows=2, figsize=(12, 6), gridspec_kw={"height_ratios": [1, 2]}
                 )
                 plt.subplots_adjust(hspace=0.1)
             else:
```

### Comparing `sleepeeg-0.3.1/sleepeeg/utils.py` & `sleepeeg-0.3.2/sleepeeg/utils.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.1/sleepeeg.egg-info/PKG-INFO` & `sleepeeg-0.3.2/sleepeeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.3.1
+Version: 0.3.2
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

