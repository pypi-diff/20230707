# Comparing `tmp/scientific_plots-1.5.7.tar.gz` & `tmp/scientific_plots-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.5.7.tar", last modified: Fri Jun 30 22:24:28 2023, max compression
+gzip compressed data, was "scientific_plots-1.6.0.tar", last modified: Fri Jul  7 14:48:26 2023, max compression
```

## Comparing `scientific_plots-1.5.7.tar` & `scientific_plots-1.6.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.689537 scientific_plots-1.5.7/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.5.7/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)    11607 2023-06-30 22:24:28.689537 scientific_plots-1.5.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.5.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.7/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 22:24:28.689537 scientific_plots-1.5.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.677538 scientific_plots-1.5.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.681537 scientific_plots-1.5.7/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.681537 scientific_plots-1.5.7/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.681537 scientific_plots-1.5.7/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.5.7/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.7/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-06-30 21:18:04.000000 scientific_plots-1.5.7/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.681537 scientific_plots-1.5.7/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     7299 2023-06-30 21:18:04.000000 scientific_plots-1.5.7/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.5.7/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.681537 scientific_plots-1.5.7/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.7/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.7/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.681537 scientific_plots-1.5.7/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.681537 scientific_plots-1.5.7/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.685537 scientific_plots-1.5.7/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-30 21:18:04.000000 scientific_plots-1.5.7/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.5.7/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    17756 2023-06-25 08:00:18.000000 scientific_plots-1.5.7/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-30 22:24:02.000000 scientific_plots-1.5.7/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.5.7/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.685537 scientific_plots-1.5.7/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11607 2023-06-30 22:24:28.000000 scientific_plots-1.5.7/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1363 2023-06-30 22:24:28.000000 scientific_plots-1.5.7/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 22:24:28.000000 scientific_plots-1.5.7/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-30 22:24:28.000000 scientific_plots-1.5.7/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-30 22:24:28.000000 scientific_plots-1.5.7/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.685537 scientific_plots-1.5.7/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.685537 scientific_plots-1.5.7/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 22:24:28.685537 scientific_plots-1.5.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.7/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3672 2023-06-25 09:13:03.000000 scientific_plots-1.5.7/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.7/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.6.0/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.6.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.6.0/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.6.0/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.6.0/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     8959 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.6.0/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.6.0/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.6.0/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.6.0/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    17756 2023-06-25 08:00:18.000000 scientific_plots-1.6.0/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 14:48:00.000000 scientific_plots-1.6.0/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.6.0/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.6.0/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3672 2023-06-25 09:13:03.000000 scientific_plots-1.6.0/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/tests/test_utilties.py
```

### Comparing `scientific_plots-1.5.7/COPYING.LESSER` & `scientific_plots-1.6.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/PKG-INFO` & `scientific_plots-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific_plots
-Version: 1.5.7
+Version: 1.6.0
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.5.7/pyproject.toml` & `scientific_plots-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/readme.md` & `scientific_plots-1.6.0/readme.md`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.6.0/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.6.0/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.6.0/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.6.0/src/matplotlib-stubs/figure.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 """This is the stub for the figure-type in matplot-lib."""
 from __future__ import annotations
 
-from typing import Optional, Tuple, Iterable, Any
+from typing import Optional, Tuple, Iterable, Any, Union
 
 from .pyplot import Axes
 
 
 class Canvas:
     """Canvas, which contains the figure."""
 
@@ -38,7 +38,13 @@
                     projection: str = "2d") -> Axes: ...
 
     def set_label(self, label: str) -> None: ...
 
     def text(self, x: float, y: float, s: str) -> None: ...
 
     def legend(self, *args: Any, **kwargs: Any) -> None: ...
+
+    def savefig(
+        self, fname: str, *, dpi: Union[str, float] = "figure",
+        bbox_inches: Optional[tuple[float, float]] = None,
+        pad_inches: float = 0.1, backend: Optional[str] = None
+        ) -> None: ...
```

### Comparing `scientific_plots-1.5.7/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 """
 This are the typing-stubs for "matplotlib.pyplot".
 They are needed for a testing using mypy.
 """
 from __future__ import annotations
 from typing import (
-    Optional, Tuple, Iterable, Union, TypeVar, List, TypedDict, Any)
+    Optional, Tuple, Iterable, Union, TypeVar, List, TypedDict, Any,
+    overload)
 from pathlib import Path
 from contextlib import contextmanager
 from collections.abc import Generator
 
 from ..ticker import Locator
 from ..figure import Figure
 from .. import colors, RCParams
@@ -141,52 +142,64 @@
     def get_lines(self) -> Iterable[Line]: ...
 
     def get_legend(self) -> Legend: ...
 
     def set_xlabel(self, label: str,
                    linespacing: Optional[float] = None,
                    rotation: Optional[float] = None,
-                   labelpad: Optional[float] = None) -> None: ...
+                   labelpad: Optional[float] = None,
+                   color: Optional[str] = None) -> None: ...
 
     def set_ylabel(self, label: str,
                    linespacing: Optional[float] = None,
                    rotation: Optional[float] = None,
-                   labelpad: Optional[float] = None) -> None: ...
+                   labelpad: Optional[float] = None,
+                   color: Optional[str] = None) -> None: ...
 
     def set_zlabel(self, label: str,
                    linespacing: Optional[float] = None,
                    rotation: Optional[float] = None,
-                   labelpad: Optional[float] = None) -> None: ...
-
-    def set_title(self, label: str) -> None: ...
+                   labelpad: Optional[float] = None,
+                   color: Optional[str] = None) -> None: ...
 
     def set_xlim(self, min_: float, max_: float) -> None: ...
 
     def set_ylim(self, min_: float, max_: float) -> None: ...
 
     def set_zlim(self, min_: float, max_: float) -> None: ...
 
     def set_xscale(self, scale: str) -> None: ...
 
     def set_yscale(self, scale: str) -> None: ...
 
     def set_zscale(self, scale: str) -> None: ...
 
-    def plot_surface(self, X: In2D, Y: In2D, Z: In2D,
-                     cmap: str = "") -> None: ...
+    def plot_surface(self, X: In2D, Y: In2D, Z: In2D, *,
+                     cmap: str = "", alpha: Optional[float] = None) -> None: ...
 
     def scatter(self, X: In, Y: In, Z: In,
                 cmap: Union[str, colors.ColorMap] = "jet") -> None: ...
 
     def plot_trisurf(self, X: In, Y: In, Z: In,
                      cmap: Union[str, colors.ColorMap] = "jet")\
         -> None: ...
 
-    def plot(self, X: In, Y: In, label: Optional[str] = None,
-             color: Optional[str] = None, linestyle: Optional[str] = None)\
+    @overload
+    def plot(self, X: In2D, Y: In2D, Z: In2D,
+             fmt: Optional[str] = None, *,
+             label: Optional[str] = None,
+             color: Optional[str] = None, linestyle: Optional[str] = None,
+             alpha: Optional[float] = None)\
+        -> list[Line]: ...
+
+    @overload
+    def plot(self, X: In, Y: In, fmt: Optional[str] = None, *,
+             label: Optional[str] = None,
+             color: Optional[str] = None, linestyle: Optional[str] = None,
+             alpha: Optional[float] = None)\
         -> list[Line]: ...
 
     def twinx(self) -> Axes: ...
 
     def get_ylabel(self) -> str: ...
 
     def get_xlabel(self) -> str: ...
@@ -197,24 +210,41 @@
                     colors: str = "") -> None: ...
 
     def ticklabel_format(
         self,
         useLocale: bool = False, useMathText: bool = False) -> None: ...
 
     def set_box_aspect(
-        cself,
+        self,
         aspect: Optional[str] = None, zoom: float = 1.)\
         -> None: ...
 
     def legend(
         self,
         handles: Optional[Union[list[Line], list[str]]] = None,
         labels: Optional[list[str]] = None) -> None: ...
 
-    def set(**kwargs: Any) -> None: ...
+    def set(
+        self, **kwargs: Any) -> None: ...
+
+    def set_title(self, label: str, loc: Optional[str] = None) -> None: ...
+
+    def grid(self, visible: Optional[bool] = None, which: str = "major")\
+        -> None: ...
+
+    def hist(
+        self, x: Union[Vector, Matrix],
+        bins: Optional[Union[int, Vector, str]] = None,
+        range: Optional[tuple[float, float]] = None,
+        density: bool = False, weights: Optional[Vector] = None,
+        cumulative: bool = False, bottom: Optional[float] = None,
+        histtype: str = "bar", align: str = "mid",
+        orientation: str = "vertical", log: bool = False,
+        color: Optional[str] = None, label: Optional[str] = None,
+        stacked: bool = False) -> None: ...
 
 
 def figure(figsize: Optional[Tuple[float, float]] = None) -> Figure: ...
 
 
 def close(fig: Union[Figure, str, None] = None) -> None: ...
 
@@ -314,7 +344,19 @@
     s: str = "",
     xy: Optional[tuple[float, float]] = None,
     xytext: Optional[tuple[float, float]] = None,
     arrowprops: Optional[_ArrowProps] = None) -> None: ...
 
 
 def text(x: float, y: float, text: str) -> None: ...
+
+def axes(arg: Optional[tuple[str, str, str, str]] = None,
+         label: str = "", projection: Optional[str] = None,
+         polar: bool = False, sharex: Optional[Axes] = None,
+         sharey: Optional[Axes] = None) -> Axes: ...
+
+
+def subplot(
+    *args: Any,
+    label: str = "", projection: Optional[str] = None,
+    polar: bool = False, sharex: Optional[Axes] = None,
+    sharey: Optional[Axes] = None) -> Axes: ...
```

### Comparing `scientific_plots-1.5.7/src/matplotlib-stubs/ticker.pyi` & `scientific_plots-1.6.0/src/matplotlib-stubs/ticker.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/numba-stubs/__init__.pyi` & `scientific_plots-1.6.0/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scientific_plots/data_analysis.py` & `scientific_plots-1.6.0/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scientific_plots/default_plots.py` & `scientific_plots-1.6.0/src/scientific_plots/default_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scientific_plots/plot_settings.py` & `scientific_plots-1.6.0/src/scientific_plots/plot_settings.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.6.0/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scientific_plots/types_.py` & `scientific_plots-1.6.0/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scientific_plots/utilities.py` & `scientific_plots-1.6.0/src/scientific_plots/utilities.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.6.0/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-plots
-Version: 1.5.7
+Version: 1.6.0
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.5.7/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.6.0/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scipy-stubs/fft.pyi` & `scientific_plots-1.6.0/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.6.0/src/scipy-stubs/integrate.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 def romberg(func: Callable[[Input], Input], x_min: float, x_max: float,
             tol: float = 1e-30,
             rtol: float = 1e-30,
             divmax: int = 15) -> float: ...
 
 
-def quad(func: Callable[[Input], Input], xmin: float, xmax: float,
-         limit: int = 50, epsabs: float = 1.49e-8, epsrel: float = 1.49e-8)\
+def quad(func: Callable[..., Input], xmin: float, xmax: float,
+         limit: int = 50, epsabs: float = 1.49e-8, epsrel: float = 1.49e-8,
+         args: Optional[tuple[float, ...]] = None)\
     -> Tuple[float, Any]: ...
 
 
 def dblquad(func: Callable[[Input, Input], Input], a: float, b: float,
             gfun: Callable[[Input], Input],
             hfun: Callable[[Input], Input]) -> Tuple[float, Any]: ...
```

### Comparing `scientific_plots-1.5.7/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.6.0/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.6.0/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/tests/test_plot_manual.py` & `scientific_plots-1.6.0/tests/test_plot_manual.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/tests/test_plots.py` & `scientific_plots-1.6.0/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/tests/test_types.py` & `scientific_plots-1.6.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.5.7/tests/test_utilties.py` & `scientific_plots-1.6.0/tests/test_utilties.py`

 * *Files identical despite different names*

