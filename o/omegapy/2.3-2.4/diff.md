# Comparing `tmp/omegapy-2.3.tar.gz` & `tmp/omegapy-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegapy-2.3.tar", last modified: Mon Jan 30 19:00:48 2023, max compression
+gzip compressed data, was "omegapy-2.4.tar", last modified: Fri Jul  7 18:36:15 2023, max compression
```

## Comparing `omegapy-2.3.tar` & `omegapy-2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:00:48.198042 omegapy-2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-30 19:00:40.000000 omegapy-2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-01-30 19:00:48.198042 omegapy-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-01-30 19:00:40.000000 omegapy-2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:00:48.186041 omegapy-2.3/omegapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:00:48.194041 omegapy-2.3/omegapy/OMEGA_dataref/
--rw-r--r--   0 runner    (1001) docker     (123)   143760 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/boundcur.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/corrupted_obs.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1495234 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/cubindex.ref
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/flatVIS050701.bin
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/fond2.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/lambda_0403.dat
--rw-r--r--   0 runner    (1001) docker     (123)    48007 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/linearC.dat
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/mtf120315_25.dat
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/mtf120315_50.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/omega_wvl_CL.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/rapcur_25.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/rapcur_50.dat
--rw-r--r--   0 runner    (1001) docker     (123)  6723584 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/rapmtflcur.bin
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/OMEGA_dataref/specsol_0403.dat
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119762 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/omega_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    79105 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/omega_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:00:48.194041 omegapy-2.3/omegapy/res_findcube/
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/res_findcube/cubelist
--rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-01-30 19:00:40.000000 omegapy-2.3/omegapy/useful_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 19:00:48.186041 omegapy-2.3/omegapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-01-30 19:00:48.000000 omegapy-2.3/omegapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-30 19:00:48.000000 omegapy-2.3/omegapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 19:00:48.000000 omegapy-2.3/omegapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-30 19:00:48.000000 omegapy-2.3/omegapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-30 19:00:48.000000 omegapy-2.3/omegapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 19:00:48.198042 omegapy-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-01-30 19:00:40.000000 omegapy-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:36:15.869549 omegapy-2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 18:36:04.000000 omegapy-2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-07 18:36:15.869549 omegapy-2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-07 18:36:04.000000 omegapy-2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:36:15.861549 omegapy-2.4/omegapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:36:15.869549 omegapy-2.4/omegapy/OMEGA_dataref/
+-rw-r--r--   0 runner    (1001) docker     (123)   143760 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/boundcur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/corrupted_obs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1495234 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/cubindex.ref
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/flatVIS050701.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/fond2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/lambda_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    48007 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/linearC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/mtf120315_25.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/mtf120315_50.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/omega_wvl_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/rapcur_25.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/rapcur_50.dat
+-rw-r--r--   0 runner    (1001) docker     (123)  6723584 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/rapmtflcur.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/OMEGA_dataref/specsol_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124930 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/omega_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72803 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/omega_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:36:15.869549 omegapy-2.4/omegapy/res_findcube/
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/res_findcube/cubelist
+-rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-07-07 18:36:04.000000 omegapy-2.4/omegapy/useful_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:36:15.861549 omegapy-2.4/omegapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-07 18:36:15.000000 omegapy-2.4/omegapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-07 18:36:15.000000 omegapy-2.4/omegapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:36:15.000000 omegapy-2.4/omegapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 18:36:15.000000 omegapy-2.4/omegapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 18:36:15.000000 omegapy-2.4/omegapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:36:15.869549 omegapy-2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-07 18:36:04.000000 omegapy-2.4/setup.py
```

### Comparing `omegapy-2.3/LICENSE` & `omegapy-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/PKG-INFO` & `omegapy-2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: omegapy
-Version: 2.3
+Version: 2.4
 Summary: Python tools for OMEGA/MEx observations analysis
 Home-page: https://astcherbinine.github.io/omegapy
 Author: Aurélien Stcherbinine
 Author-email: aurelien@stcherbinine.net
 Project-URL: Source, https://github.com/AStcherbinine/omegapy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![version](https://img.shields.io/badge/version-2.3-blue)
+![version](https://img.shields.io/badge/version-2.4-blue)
 ![pythonversion](https://img.shields.io/badge/Python-3.7+-blue)
+[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/badge/latestdoi/349763849)
+
 
 <p align="center">
 <img width="250" height="250" src="https://github.com/AStcherbinine/omegapy/blob/master/docs/logo_omegapy_small2.png">
 </p>
 
 # OMEGA-Py : Python tools for OMEGA data
 
@@ -102,22 +104,27 @@
 # Simultaneous Atmospheric & Thermal corrections (for the use of the L-channel)
 # > Use the `npool` argument to control the number of simultaneous processes used to compute the thermal correction 
 # > (e.g., npool=15 is usually a nice choice if your system can handle it)
 # > Note: multiprocessing is currently not available for Windows
 omega_corr_therm_atm = od.corr_therm_atm(omega_corr, npool=1)
 # Thermal correction only
 omega_corr_therm = od.corr_therm(omega, npool=1)
+# OMEGA mask to hide bad pixels / calibration lines
+mask = od.omega_mask(omega, hide_128=True, emer_lim=10, inci_lim=70, temc_lim=-194, limsat_c=500)
 # Interactive display of the observation (@ λ = 1.085 µm)
 op.show_omega_interactif_v2(omega_corr_therm_atm, lam=1.085, cmap='Greys_r', vmin=0, vmax=0.5, polar=True)
 # Search for the index of λ = 1.085 µm in the wavelength array
 i_lam = uf.where_closer(1.085, omega.lam)
 ~~~
 
+## Documentation
 See [`docs/*.md`](https://github.com/AStcherbinine/omegapy/blob/master/docs/) or the interactive IPython help for more details.
 
+Planetary Data Workshop 2023: [abstract](https://github.com/AStcherbinine/omegapy/blob/master/docs/Stcherbinine_PDW2023_7007_omegapy.pdf) & [slides](https://github.com/AStcherbinine/omegapy/blob/master/docs/PDW_Flagstaff_Stcherbinine_omegapy_upload.pdf)
+
 ## Credits
 
 © Aurélien Stcherbinine (2020–2023)
 
 Institut d'Astrophysique Spatiale (IAS), Université Paris-Saclay, CNRS, Orsay, France
 
 LATMOS/IPSL, UVSQ Université Paris-Saclay, Sorbonne Université, CNRS, Guyancourt, France
```

### Comparing `omegapy-2.3/README.md` & `omegapy-2.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-![version](https://img.shields.io/badge/version-2.3-blue)
+![version](https://img.shields.io/badge/version-2.4-blue)
 ![pythonversion](https://img.shields.io/badge/Python-3.7+-blue)
+[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/badge/latestdoi/349763849)
+
 
 <p align="center">
 <img width="250" height="250" src="https://github.com/AStcherbinine/omegapy/blob/master/docs/logo_omegapy_small2.png">
 </p>
 
 # OMEGA-Py : Python tools for OMEGA data
 
@@ -85,22 +87,27 @@
 # Simultaneous Atmospheric & Thermal corrections (for the use of the L-channel)
 # > Use the `npool` argument to control the number of simultaneous processes used to compute the thermal correction 
 # > (e.g., npool=15 is usually a nice choice if your system can handle it)
 # > Note: multiprocessing is currently not available for Windows
 omega_corr_therm_atm = od.corr_therm_atm(omega_corr, npool=1)
 # Thermal correction only
 omega_corr_therm = od.corr_therm(omega, npool=1)
+# OMEGA mask to hide bad pixels / calibration lines
+mask = od.omega_mask(omega, hide_128=True, emer_lim=10, inci_lim=70, temc_lim=-194, limsat_c=500)
 # Interactive display of the observation (@ λ = 1.085 µm)
 op.show_omega_interactif_v2(omega_corr_therm_atm, lam=1.085, cmap='Greys_r', vmin=0, vmax=0.5, polar=True)
 # Search for the index of λ = 1.085 µm in the wavelength array
 i_lam = uf.where_closer(1.085, omega.lam)
 ~~~
 
+## Documentation
 See [`docs/*.md`](https://github.com/AStcherbinine/omegapy/blob/master/docs/) or the interactive IPython help for more details.
 
+Planetary Data Workshop 2023: [abstract](https://github.com/AStcherbinine/omegapy/blob/master/docs/Stcherbinine_PDW2023_7007_omegapy.pdf) & [slides](https://github.com/AStcherbinine/omegapy/blob/master/docs/PDW_Flagstaff_Stcherbinine_omegapy_upload.pdf)
+
 ## Credits
 
 © Aurélien Stcherbinine (2020–2023)
 
 Institut d'Astrophysique Spatiale (IAS), Université Paris-Saclay, CNRS, Orsay, France
 
 LATMOS/IPSL, UVSQ Université Paris-Saclay, Sorbonne Université, CNRS, Guyancourt, France
```

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav` & `omegapy-2.4/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/boundcur.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/boundcur.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/corrupted_obs.csv` & `omegapy-2.4/omegapy/OMEGA_dataref/corrupted_obs.csv`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/cubindex.ref` & `omegapy-2.4/omegapy/OMEGA_dataref/cubindex.ref`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/flatVIS050701.bin` & `omegapy-2.4/omegapy/OMEGA_dataref/flatVIS050701.bin`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/fond2.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/fond2.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/lambda_0403.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/lambda_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/linearC.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/linearC.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/mtf120315_25.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/mtf120315_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/mtf120315_50.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/mtf120315_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/omega_atmorap_CL.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/omega_atmorap_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/omega_wvl_CL.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/omega_wvl_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/rapcur_25.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/rapcur_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/rapcur_50.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/rapcur_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/rapmtflcur.bin` & `omegapy-2.4/omegapy/OMEGA_dataref/rapmtflcur.bin`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/OMEGA_dataref/specsol_0403.dat` & `omegapy-2.4/omegapy/OMEGA_dataref/specsol_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/omega_data.py` & `omegapy-2.4/omegapy/omega_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ## omega_data.py
 ## Created by Aurélien STCHERBININE
-## Last modified by Aurélien STCHERBININE : 25/01/2023
+## Last modified by Aurélien STCHERBININE : 16/06/2023
 
 ##----------------------------------------------------------------------------------------
 """Importation and correction of OMEGA/MEx observations from binaries files.
 """
 ##----------------------------------------------------------------------------------------
 ##----------------------------------------------------------------------------------------
 ## Packages
@@ -31,15 +31,15 @@
 import ctypes
 import platform
 # Local
 from . import useful_functions as uf
 
 # Name of the current file
 _py_file = 'omega_data.py'
-_Version = 2.2
+_Version = 2.3
 
 # Path of the package files
 package_path = os.path.abspath(os.path.dirname(__file__))
 # Path of the directory containing the OMEGA binary files (.QUB and .NAV)
 _omega_bin_path = os.getenv('OMEGA_BIN_PATH', default='/data2/opt/geomeg/data/product/')
 # Path of the directory containing the OMEGA python-made files
 _omega_py_path = os.getenv('OMEGA_PY_PATH', default='/data/mex-omegj/data1/omega_python/omegapy/')
@@ -2284,14 +2284,25 @@
     # print('Duration : {0:.0f} min {1:.2f} sec'.format((tfin-tini)//60, (tfin-tini)%60))
     return omega_corr
     
 ##-----------------------------------------------------------------------------------
 ## Correction mode 128
 def corr_mode_128(omega):
     """Correction corrupted pixels mode 128.
+
+    Parameters
+    ==========
+    omega : OMEGAdata
+        The OMEGA observation data.
+
+    Returns
+    =======
+    omega_corr : OMEGAdata
+        The input OMEGA observation, where data from the corrupted columns of 128-pixels wide
+        observations have been corrected if possible.
     """
     omega_corr = deepcopy(omega)
     ic128 = deepcopy(omega.ic)
     npixel = omega.npixel
     nscan = omega.nscan
     if npixel != 128:
         print('\033[1mNot a 128 pixel cube\033[0m')
@@ -2529,15 +2540,15 @@
     if base_folder == "_omega_py_path":
         base_folder = _omega_py_path
     N = len(liste_obs)
     if folder == 'auto':
         folder = 'v' + str(int(_Version))
     for i, obsname in enumerate(liste_obs):
         print('\n\033[01mComputing observation {0} / {1} : {2}\033[0m\n'.format(i+1, N, obsname))
-        corr_save_omega(obsname, folder, base_folder, security, overwrite, compress, npool)
+        corr_save_omega2(obsname, folder, base_folder, security, overwrite, compress, npool)
     print("\n\033[01;32m Done\033[0m\n")
 
 ##-----------------------------------------------------------------------------------
 ## Liste observations depuis fichier CSV
 def import_list_obs_csv(filename):
     """Import a list of observations ID from a csv file generated by JMars.
 
@@ -2986,10 +2997,129 @@
                 test = False
                 break
         if test:
             lam2.append(lami)
     lam2 = np.array(lam2)
     return lam2
 
+##----------------------------------------------------------------------------------------
+## Mask OMEGA observation
+def omega_mask(omega, emer_lim=None, inci_lim=None, tempc_lim=None, limsat_c=None,
+               hide_128=True, reject_low_quality=False):
+    """Return a mask to remove the bad, corrupted or undesired pixels of an observation.
+
+    Parameters
+    ==========
+    omega : OMEGAdata
+        The OMEGA observation data.
+    emer_lim : float or None, optional (default None)
+        The maximum emergence angle.
+    inci_lim : float or None, optional (default None)
+        The maximum incidence angle.
+    tempc_lim : float or None, optional (default None)
+        The maximum temperature for the C-channel.
+    limsat_c : float or None, optional (default None)
+        The maximum value of the C-channel saturation [DN].
+        The maximum value in DN for the spectel #40 (i.e., λ=1.486μm).
+        > See Vincendon et al. (2015) or Stcherbinine et al. (2021).
+    hide_128 : bool, optional (default True)
+        If True, hide the corrupted columns for 128-px wide cubes affected.
+    reject_low_quality : bool, optional (default False)
+        Reject observations flagged as low quality, as defined in Stcherbinine et al. (2021).
+        I.e., if: 
+         >  (omega.data_quality == 0)   # Low quality
+         >  or (not omega.orbit in good_orbits_OBC) # Not in "good orbits" file
+         >  or (omega.quality == 0)
+         >  or ((numCube == 0) and (npixel == 64) and (omega.bits_per_data == 1)) 
+         >  or (omega.target != 'MARS') # Mars pointing only
+         >  or (omega.mode_channel != 1)    # All 3 channels required
+         >  or (omega.point_mode == 'N/A')  # Unknown pointing informations
+
+    Returns
+    =======
+    mask : 2D array 
+        The array that identify the bad/corrupted pixels to remove.
+        | 1 -> Good pixel
+        | NaN -> Bad pixel
+    """
+    # Initialisation
+    mask = np.ones((omega.nscan, omega.npixel))
+    numCube = int(omega.name[-1], 16)
+    npixel = omega.npixel
+    summation = omega.summation
+    OBC = readsav(os.path.join(package_path, 'OMEGA_dataref', 'OBC_OMEGA_OCT2017.sav'))
+    good_orbits_OBC = np.array(OBC['good_orbits'][0], dtype=int)
+    # Rejected cubes : NaN everywhere
+    if reject_low_quality:
+        test_rej = ( 
+            (omega.data_quality == 0)   # Low quality
+            or (not omega.orbit in good_orbits_OBC) # Not in "good orbits" file
+            or (omega.quality == 0)
+            or ((numCube == 0) and (npixel == 64) and (omega.bits_per_data == 1)) 
+            or (omega.target != 'MARS') # Mars pointing only
+            or (omega.mode_channel != 1)    # All 3 channels required
+            or (omega.point_mode == 'N/A')  # Unknown pointing informations
+            # or (omega.npixel == 16)
+                    )
+        if test_rej:
+            mask.fill(np.nan)
+            print('\033[1mObservation {0} rejected because of low data quality.\033[0m'.format(omega.name))
+            return mask
+    # Create mask
+    # Modes 128
+    if (npixel == 128) and hide_128:
+        if omega.orbit >= 511:
+            # print("Mode 128 pixels observation")
+            mask[:, 80:96] = np.nan
+        if (omega.orbit >= 2124) and (omega.orbit <= 3283):
+            mask[:, 64:] = np.nan
+    # Calibration lines C-channel for cubes 0
+    if numCube == 0:
+        if npixel == 16:
+            mask[:192] = np.nan
+        elif npixel == 32:
+            mask[:96] = np.nan
+        elif npixel == 64:
+            mask[:48] = np.nan
+        elif npixel == 128:
+            if summation == 1:
+                mask[:24] = np.nan
+            elif summation == 2:
+                mask[:12] = np.nan
+            elif summation == 4:
+                mask[:6] = np.nan
+    # Calib lines VIS-channel for all cubes
+    else:   # Already included in C-channel calib lines for cubes 0
+        if npixel == 16:
+            mask[:56] = np.nan
+        elif npixel == 32:
+            mask[:28] = np.nan
+        elif npixel == 64:
+            mask[:14] = np.nan
+        elif npixel == 128:
+            if summation == 1:
+                mask[:7] = np.nan
+            elif summation == 2:
+                mask[:3] = np.nan
+            elif summation == 4:
+                mask[0] = np.nan
+    # Remove 4 last lines
+    mask[-4:] = np.nan
+    # Incidence angle limit
+    if not (inci_lim is None):
+        mask[omega.inci > inci_lim] = np.nan
+    # Emergence angle limit
+    if not (emer_lim is None):
+        mask[omega.emer > emer_lim] = np.nan
+    # C-channel temperature limit
+    if not (tempc_lim is None):
+        mask[omega.sensor_temp_c > tempc_lim] = np.nan
+    # C-channel saturation criterion limit
+    # (cf Vincendon et al. (2015) or Stcherbinine et al. (2021))
+    if not (limsat_c is None):
+        mask[omega.saturation_c < limsat_c] = np.nan
+    # Output
+    return mask
+
 ##-----------------------------------------------------------------------------------
 ## End of code
 ##-----------------------------------------------------------------------------------
```

### Comparing `omegapy-2.3/omegapy/omega_plots.py` & `omegapy-2.4/omegapy/omega_plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ## omega_plots.py
 ## Created by Aurélien STCHERBININE
-## Last modified by Aurélien STCHERBININE : 20/04/2022
+## Last modified by Aurélien STCHERBININE : 07/07/2023
 
 ##----------------------------------------------------------------------------------------
 """Display of OMEGAdata cubes.
 """
 ##----------------------------------------------------------------------------------------
 ##----------------------------------------------------------------------------------------
 ## Packages
@@ -243,25 +243,26 @@
         plt.ylim(latlim)
         plt.gca().set_adjustable('box')
         plt.xlabel('Longitude [°]')
         plt.ylabel('Latitude [°]')
     if cbar:
         cb = plt.colorbar()
         cb.set_label(cb_title)
+    plt.grid(visible=False)
     if grid:
         ax = plt.figure(Nfig).get_axes()[0]
         lonlim = ax.get_xlim()
         latlim = ax.get_ylim()
         lon_sgn = np.sign(lonlim[1] - lonlim[0])
         lat_sgn = np.sign(latlim[1] - latlim[0])
         lon_grid = np.arange(np.round(lonlim[0]/10)*10, np.round(lonlim[1]/10)*10+lon_sgn, 
                     10 * lon_sgn)   # 10° grid in longitude
         lat_grid = np.arange(np.round(latlim[0]/10)*10, np.round(latlim[1]/10)*10+lat_sgn, 
                     10 * lat_sgn)   # 10° grid in latitude
-        plt.grid()
+        plt.grid(visible=True)
         if polar:
             ax.set_rticks(lat_grid)
         else:
             ax.set_xticks(lon_grid)
             ax.set_yticks(lat_grid)
     plt.title(title)
     plt.tight_layout()
@@ -849,25 +850,26 @@
         plt.ylim(latlim)
         plt.gca().set_adjustable('box')
         plt.xlabel('Longitude [°]')
         plt.ylabel('Latitude [°]')
     if cbar:
         cb = plt.colorbar()
         cb.set_label(cb_title)
+    plt.grid(visible=False)
     if grid:
         ax = plt.figure(Nfig).get_axes()[0]
         lonlim = ax.get_xlim()
         latlim = ax.get_ylim()
         lon_sgn = np.sign(lonlim[1] - lonlim[0])
         lat_sgn = np.sign(latlim[1] - latlim[0])
         lon_grid = np.arange(np.round(lonlim[0]/10)*10, np.round(lonlim[1]/10)*10+lon_sgn, 
                     10 * lon_sgn)   # 10° grid in longitude
         lat_grid = np.arange(np.round(latlim[0]/10)*10, np.round(latlim[1]/10)*10+lat_sgn, 
                     10 * lat_sgn)   # 10° grid in latitude
-        plt.grid()
+        plt.grid(visible=True)
         if polar:
             ax.set_rticks(lat_grid)
         else:
             ax.set_xticks(lon_grid)
             ax.set_yticks(lat_grid)
     plt.title(title)
     plt.tight_layout()
@@ -902,17 +904,17 @@
 
     Returns
     =======
     grid_data : 2D array (dim : Nlon x Nlat)
         The data values, sampled on the new lat/lon grid.
     mask : 2D array
         The array indicating where the new grid has been filled by the OMEGA data.
-    grid lat : 2D array
+    grid_lat : 2D array
         The new latitude grid.
-    grid lon : 2D array
+    grid_lon : 2D array
         The new longitude grid.
     """
     # Initialisation
     lat_array = np.arange(lat_min, lat_max+pas_lat, pas_lat)
     lon_array = np.arange(lon_min, lon_max+pas_lon, pas_lon)
     Nlon, Nlat = len(lon_array)-1, len(lat_array)-1
     grid_lat, grid_lon = np.meshgrid(lat_array, lon_array)
@@ -938,14 +940,231 @@
                     grid_data[i_lon,j_lat] += data_tmp
                     mask[i_lon,j_lat] += 1
     grid_data[grid_data==0] = np.nan
     grid_data2 = grid_data / mask       # Normalisation
     mask2 = np.clip(mask, 0, 1)
     return grid_data2, mask2, grid_lat, grid_lon
 
+def reorder_pts(X4, Y4):
+    Xa, Xb, Xc, Xd = deepcopy(X4)
+    Ya, Yb, Yc, Yd = deepcopy(Y4)
+    while ((Xa > Xb) or (Xd > Xc) or (Ya > Yd) or (Yb > Yc)):
+        if Xa > Xb:
+            Xa, Xb = Xb, Xa
+            Ya, Yb = Yb, Ya
+        if Xd > Xc:
+            Xd, Xc = Xc, Xd
+            Yd, Yc = Yc, Yd
+        if Ya > Yd:
+            Ya, Yd = Yd, Ya
+            Xa, Xd = Xd, Xa
+        if Yb > Yc:
+            Yb, Yc = Yc, Yb
+            Xb, Xc = Xc, Xb
+    X4_new = (Xa, Xb, Xc, Xd)
+    Y4_new = (Ya, Yb, Yc, Yd)
+    return X4_new, Y4_new
+
+def point_in_poly4(x0, y0, X4, Y4):
+    """Test if a point of coordinates (x0, y0) is within a polygon with 4 sides.
+
+    Parameters
+    ==========
+    x0 : float or array-like
+        The x-coordinate of the point to test.
+    y0 : float or array-like
+        The y-coordinate of the point to test.
+    X4 : 4-tuple of floats
+        The x-coordinates of the polygon corners.
+    Y4 : 4-tuple of floats
+        The y-coordinates of the polygon corners.
+
+    Returns
+    =======
+    testin : bool or array-like of bool
+        True if (x0, y0) is within the polygon.
+    """
+    # Extraction
+    Xa, Xb, Xc, Xd = deepcopy(X4)
+    Ya, Yb, Yc, Yd = deepcopy(Y4)
+    # re-order to have
+    #  D--C
+    #  |  |
+    #  A--B
+    while ((Xa > Xb) or (Xd > Xc) or (Ya > Yd) or (Yb > Yc)):
+        if Xa > Xb:
+            Xa, Xb = Xb, Xa
+            Ya, Yb = Yb, Ya
+        if Xd > Xc:
+            Xd, Xc = Xc, Xd
+            Yd, Yc = Yc, Yd
+        if Ya > Yd:
+            Ya, Yd = Yd, Ya
+            Xa, Xd = Xd, Xa
+        if Yb > Yc:
+            Yb, Yc = Yc, Yb
+            Xb, Xc = Xc, Xb
+    # Internal test functions
+    def f_xmin(y):
+        return Xa + ((Xd - Xa) / (Yd - Ya)) * (y - Ya)
+    def f_xmax(y):
+        return Xb + ((Xc - Xb) / (Yc - Yb)) * (y - Yb)
+    def f_ymin(x):
+        return Ya + ((Yb - Ya) / (Xb - Xa)) * (x - Xa)
+    def f_ymax(x):
+        return Yd + ((Yc - Yd) / (Xc - Xd)) * (x - Xd)
+    # Test if point in poly
+    testin = (
+        ( x0 >= f_xmin(y0) ) &
+        ( x0 <= f_xmax(y0) ) &
+        ( y0 >= f_ymin(x0) ) &
+        ( y0 <= f_ymax(x0) )
+        )
+    return testin
+
+def proj_grid2(omega, data, lat_min=-90, lat_max=90, lon_min=0, lon_max=360,
+              pas_lat=0.1, pas_lon=0.1, negative_values=False):
+    """Sample the data from the input OMEGA/MEx observation on a given lat/lon grid.
+
+    Parameters
+    ==========
+    omega : OMEGAdata
+        The OMEGA/MEx observation
+    data : 2D array
+        The initial array of values associated to the OMEGAdata observation.
+        e.g.: Refelectance at selected wvl, spectra, or derived data such as IBD map.
+    lat_min : float, optional (default -90)
+        The minimal latitude of the grid.
+    lat_max : float, optional (default 90)
+        The maximum latitude of the grid.
+    lon_min : float, optional (default 0)
+        The minimal longitude of the grid.
+    lon_max : float, optional (default 360)
+        The maximal longitude of the grid.
+    pas_lat : float, optional (default 0.1)
+        The latitude intervals of the grid.
+    pas_lon : float, optional (default 0.1)
+        The longitude intervals of the grid.
+    negative_values : bool, optional (default False)
+        Set if the negative values are considered as relevant data or not.
+
+    Returns
+    =======
+    grid_data : 2D array (dim : Nlon x Nlat)
+        The data values, sampled on the new lat/lon grid.
+    mask : 2D array
+        The array indicating where the new grid has been filled by the OMEGA data.
+    grid_lat : 2D array
+        The new latitude grid.
+    grid_lon : 2D array
+        The new longitude grid.
+    """
+    # Initialisation
+    #-- OMEGA grids
+    Ωlat = deepcopy(omega.lat)
+    Ωlon = deepcopy(omega.lon)
+    Ωgrid_lat = deepcopy(omega.lat_grid)
+    Ωgrid_lon = deepcopy(omega.lon_grid)
+    #-- Test negative longitudes if close to 0°/360°
+    mask_lat = (np.abs(omega.lat) < 85)
+    if (omega.lon[mask_lat] < 10).any() and (omega.lon[mask_lat] > 350).any() and (lon_min >= 0) and (lon_max > 180):
+        negatives_longitudes = True
+    else:
+        negatives_longitudes = False
+    #-- Test polar case
+    if (omega.lat > 85).any():
+        polarN = True
+        polarS = False
+    elif (omega.lat < -85).any():
+        polarN = False
+        polarS = True
+    else:
+        polarN = False
+        polarS = False
+    #-- Lon/Lat grids
+    lat_array = np.arange(lat_min, lat_max+pas_lat, pas_lat)
+    lon_array = np.arange(lon_min, lon_max+pas_lon, pas_lon)
+    if negatives_longitudes:
+        n_neg_lon = np.sum(lon_array > 180) # nb of negative longitudes (>180°)
+        i_lon180 = np.where(lon_array > 180)[0][0] # 1st index of lon > 180°
+        lon_array_nl = deepcopy(lon_array)        # new longitude grid [-180°, 180°]
+        lon_array_nl[:n_neg_lon] = lon_array[i_lon180-1:-1] - 360
+        lon_array_nl[n_neg_lon:] = lon_array[:i_lon180]
+        lon_array = deepcopy(lon_array_nl)
+        Ωgrid_lon[Ωgrid_lon > 180] -= 360
+        Ωlon[Ωlon > 180] -= 360
+    Nlon, Nlat = len(lon_array)-1, len(lat_array)-1
+    grid_lat, grid_lon = np.meshgrid(lat_array, lon_array)
+    grid_data = np.zeros((Nlon, Nlat))
+    mask = np.zeros((Nlon, Nlat))
+    #-- Center grids for projection
+    if np.min(lat_array) < np.min(Ωgrid_lat):
+        i_lat_min = np.where(lat_array < np.min(Ωgrid_lat))[0][-1]
+    else:
+        i_lat_min = 0
+    if np.max(lat_array) > np.max(Ωgrid_lat):
+        i_lat_max = np.where(lat_array > np.max(Ωgrid_lat))[0][0]
+    else:
+        i_lat_max = Nlat
+    if np.min(lon_array) < np.min(Ωgrid_lon):
+        i_lon_min = np.where(lon_array < np.min(Ωgrid_lon))[0][-1]
+    else:
+        i_lon_min = 0
+    if np.max(lon_array) > np.max(Ωgrid_lon):
+        i_lon_max = np.where(lon_array > np.max(Ωgrid_lon))[0][0]
+    else:
+        i_lon_max = Nlon
+    if polarN or polarS:
+        i_lon_min, i_lon_max = 0, Nlon
+    grid_latC = deepcopy(grid_lat)[i_lon_min:i_lon_max, i_lat_min:i_lat_max] + pas_lat/2
+    grid_lonC = deepcopy(grid_lon)[i_lon_min:i_lon_max, i_lat_min:i_lat_max] + pas_lon/2
+    # Sampling on the new grid
+    nx, ny = data.shape
+    for j in tqdm(range(ny)):
+        for i in tqdm(range(nx), leave=False):
+            data_tmp = data[i,j]
+            lat4 = Ωgrid_lat[i:i+2, j:j+2].reshape(-1)
+            lon4 = Ωgrid_lon[i:i+2, j:j+2].reshape(-1)
+            # Filtrage régions sans données
+            if negative_values:
+                data_ok = (not np.isnan(data_tmp)) & (not np.isinf(data_tmp))
+            else:   # negative values = No data
+                data_ok = (not np.isnan(data_tmp)) & (data_tmp > 0) & (not np.isinf(data_tmp))
+            # Filling grids with data
+            if data_ok:
+                testin = point_in_poly4(grid_lonC, grid_latC, lon4, lat4)   # Test if in Ω pixel
+                grid_data[i_lon_min:i_lon_max, i_lat_min:i_lat_max] += (data_tmp * testin)
+                mask[i_lon_min:i_lon_max, i_lat_min:i_lat_max] += testin
+                # if testin.any():
+                    # print(i,j, np.sum(testin))
+    grid_data[grid_data==0] = np.nan
+    grid_data2 = grid_data / mask       # Normalisation
+    mask2 = np.clip(mask, 0, 1)
+    # Re-ordering if negatives longitudes
+    if negatives_longitudes:
+        n_pos_lon = np.sum(grid_lon[:,0] >= 0) # nb of positives longitudes (>= 0°)
+        i_lon0 = np.where(grid_lon[:,0] >= 0)[0][0] # 1st index of lon >= 0°
+        # lon
+        grid_lon_pl = deepcopy(grid_lon)        # new longitude grid [0°, 360°]
+        grid_lon_pl[:n_pos_lon] = grid_lon[i_lon0:]
+        grid_lon_pl[n_pos_lon:] = grid_lon[1:i_lon0+1] + 360
+        grid_lon = deepcopy(grid_lon_pl)
+        # data
+        grid_data2_pl = deepcopy(grid_data2)      # new data array
+        grid_data2_pl[:n_pos_lon-1] = grid_data2[i_lon0:]
+        grid_data2_pl[n_pos_lon-1:] = grid_data2[:i_lon0]
+        grid_data2 = deepcopy(grid_data2_pl)
+        # mask
+        mask2_pl = deepcopy(mask2)      # new mask array
+        mask2_pl[:n_pos_lon-1] = mask2[i_lon0:]
+        mask2_pl[n_pos_lon-1:] = mask2[:i_lon0]
+        mask2 = deepcopy(mask2_pl)
+    # Output
+    return grid_data2, mask2, grid_lat, grid_lon
+
 def check_list_data_omega(omega_list, data_list, disp=True):
     """Check the compatibility between data_list and the list of OMEGA/MEx observations.
     Raise ValueError if uncompatibility.
 
     Parameters
     ==========
     omega_list : array of OMEGAdata
@@ -986,15 +1205,15 @@
     if disp:
         print("\033[01;32mCompatibility between omega_list and mask_list OK\033[0m")
 
 def show_omega_list_v2(omega_list, lam=1.085, lat_min=-90, lat_max=90, lon_min=0, lon_max=360,
                        pas_lat=0.1, pas_lon=0.1, cmap='Greys_r', vmin=None, vmax=None, 
                        title='auto', Nfig=None, polar=False, cbar=True, cb_title='auto',
                        data_list=None, mask_list=None, negative_values=False, plot=True, 
-                       grid=True, out=False, negatives_longitudes=False, 
+                       grid=True, out=False, negatives_longitudes=False, proj_method=1,
                        edgecolor='face', lw=0.1, **kwargs):
     """Display an composite map from a list OMEGA/MEx observations, sampled on a new lat/lon grid.
 
     Parameters
     ==========
     omega_list : array of OMEGAdata
         The list of OMEGA/MEx observations.
@@ -1044,14 +1263,20 @@
         Enable the display of the lat/lon grid.
     out : bool, optional (default False)
         If True -> Return output.
     negatives_longitudes : bool, optional (default False)
         Argument for non-polar plots.
         | True -> longitudes between 0° and 360°.
         | False -> longitudus between -180° and 180°.
+    proj_method : int, optional (default 1)
+        Select the projection method used (1 or 2).
+        | 1 -> Consider only the center point of each pixel.
+               Faster but not adapted if the grid resolution is lower than the OMEGA pixels size.
+        | 2 -> Consider the entire spatial extent of each pixel.
+               More accurate, but take more time.
     edgecolor : {'none', None, 'face', color', color sequence}, optional (default 'face')
         The color of the edges, see documentation of plt.pcolormesh for more details.
         > Added in version 2.2.8 to fix display due for new version of matplotlib.
     lw : float, optional (default 0.1)
         The line width of the edges (if diplayed).
     **kwargs:
         Optional arguments for the plt.pcolormesh() function.
@@ -1065,14 +1290,16 @@
     grid lat : 2D array
         The new latitude grid.
     grid lon : 2D array
         The new longitude grid.
     mask_obs : 2D array of str
         The array indicating which observations have been used to fill each grid position.
     """
+    if proj_method not in [1, 2]:
+        raise ValueError("`proj_method` must be 1 (pixel centers) or 2 (polygons).")
     # Sampling on same grid
     lat_array = np.arange(lat_min, lat_max+pas_lat, pas_lat)
     lon_array = np.arange(lon_min, lon_max+pas_lon, pas_lon)
     Nlon, Nlat = len(lon_array)-1, len(lat_array)-1
     grid_lat, grid_lon = np.meshgrid(lat_array, lon_array)
     data, mask = np.zeros((Nlon, Nlat)), np.zeros((Nlon, Nlat))
     mask_obs = np.ndarray((Nlon, Nlat), dtype=object)
@@ -1082,28 +1309,36 @@
     if data_list is None:
         for i, omega in enumerate(tqdm(omega_list)):
             i_lam = uf.where_closer(lam, omega.lam)
             if mask_list is None:
                 data_tmp = omega.cube_rf[:,:,i_lam]     # Reflectance without mask
             else:
                 data_tmp = omega.cube_rf[:,:,i_lam] * mask_list[i]  # Reflectance with mask
-            data0, mask0 = proj_grid(omega, data_tmp, lat_min, lat_max,
-                                     lon_min, lon_max, pas_lat, pas_lon, negative_values)[:2]
+            if proj_method == 1:
+                data0, mask0 = proj_grid(omega, data_tmp, lat_min, lat_max,
+                                        lon_min, lon_max, pas_lat, pas_lon, negative_values)[:2]
+            else:
+                data0, mask0 = proj_grid2(omega, data_tmp, lat_min, lat_max,
+                                         lon_min, lon_max, pas_lat, pas_lon, negative_values)[:2]
             data += np.nan_to_num(data0)    # Conversion NaN -> 0 pour somme des images
             mask += mask0
             mask_obs[mask0 == 1] += (omega.name + ',')
     else:
         check_list_data_omega(omega_list, data_list, disp=True)
         for i, omega in enumerate(tqdm(omega_list)):
             if mask_list is None:
                 data_tmp = data_list[i]     # Data without mask
             else:
                 data_tmp = data_list[i] * mask_list[i]  # Data with mask
-            data0, mask0 = proj_grid(omega, data_tmp, lat_min, lat_max,
-                                     lon_min, lon_max, pas_lat, pas_lon, negative_values)[:2]
+            if proj_method == 1:
+                data0, mask0 = proj_grid(omega, data_tmp, lat_min, lat_max,
+                                        lon_min, lon_max, pas_lat, pas_lon, negative_values)[:2]
+            else:
+                data0, mask0 = proj_grid2(omega, data_tmp, lat_min, lat_max,
+                                         lon_min, lon_max, pas_lat, pas_lon, negative_values)[:2]
             data += np.nan_to_num(data0)    # Conversion NaN -> 0 pour somme des images
             mask += mask0
             mask_obs[mask0 == 1] += (omega.name + ',')
     data[mask == 0] = np.nan
     data2 = data/mask   # Normalisation
     # Affichage figure
     if plot:
@@ -1150,25 +1385,26 @@
             plt.xlim(lon_min, lon_max)
             plt.ylim(lat_min, lat_max)
         if cbar:
             if cb_title == 'auto':
                 cb_title = r'Reflectance @ $\lambda$' + ' = {0:.2f} µm'.format(lam)
             cb = plt.colorbar()
             cb.set_label(cb_title)
+        plt.grid(visible=False)
         if grid:
             ax = plt.figure(Nfig).get_axes()[0]
             lonlim = ax.get_xlim()
             latlim = ax.get_ylim()
             lon_sgn = np.sign(lonlim[1] - lonlim[0])
             lat_sgn = np.sign(latlim[1] - latlim[0])
             lon_grid = np.arange(np.round(lonlim[0]/10)*10, np.round(lonlim[1]/10)*10+lon_sgn, 
                         10 * lon_sgn)   # 10° grid in longitude
             lat_grid = np.arange(np.round(latlim[0]/10)*10, np.round(latlim[1]/10)*10+lat_sgn, 
                         10 * lat_sgn)   # 10° grid in latitude
-            plt.grid()
+            plt.grid(visible=True)
             if polar:
                 ax.set_rticks(lat_grid)
             else:
                 ax.set_xticks(lon_grid)
                 ax.set_yticks(lat_grid)
         plt.title(title)
         plt.tight_layout()
@@ -1177,15 +1413,16 @@
         mask2 = np.clip(mask, 0, 1)
         return data2, mask2, grid_lat, grid_lon, mask_obs
 
 ##----------------------------------------------------------------------------------------
 ## Sauvegarde résultats
 def save_map_omega_list(omega_list, lat_min=-90, lat_max=90, lon_min=0, lon_max=360,
                         pas_lat=0.1, pas_lon=0.1, lam=1.085, data_list=None, data_desc='', 
-                        mask_list=None, negative_values=False, sav_filename='auto', ext='',
+                        mask_list=None, negative_values=False, proj_method=1, 
+                        sav_filename='auto', ext='',
                         base_folder='../data/OMEGA/sav_map_list_v2/', sub_folder=''):
     """Save the output of the omega_plots.show_omega_list_v2() function with the requested
     parameters as a dictionary.
 
     Parameters
     ==========
     omega_list : array of OMEGAdata
@@ -1212,14 +1449,20 @@
     mask_list : 3D array
         1D array of the same dimension of `omega_list` containing the masks to remove the
         corrupted pixels of each observaiton, in the **same order** than the observations of 
         `omega_list`.
         Each mask is a 2D array, filled with 1 for good pixels and NaN for bad ones.
     negative_values : bool, optional (default False)
         Set if the negative values are considered as relevant data or not.
+    proj_method : int, optional (default 1)
+        Select the projection method used (1 or 2).
+        | 1 -> Consider only the center point of each pixel.
+               Faster but not adapted if the grid resolution is lower than the OMEGA pixels size.
+        | 2 -> Consider the entire spatial extent of each pixel.
+               More accurate, but take more time.
     sav_filename : str, optional (default 'auto')
         The saving file name.
         | If 'auto' -> Automatically generated.
     ext : str, optional (default '')
         Extension to add at the end of the filename (useful in case of automatic generation).
     base_folder : str, optional (default '../data/OMEGA/sav_map_list_v2/')
         The base folder to save the data.
@@ -1237,27 +1480,29 @@
         data_desc = 'Reflectance @ λ = {0:0} µm'.format(lam)
     elif data_desc == '':
         data_desc = 'unknown input data'
     # Compute the data sampling
     data, mask, grid_lat, grid_lon, mask_obs = show_omega_list_v2(omega_list,
                 lam, lat_min, lat_max, lon_min, lon_max, pas_lat, pas_lon,
                 data_list=data_list, mask_list=mask_list, negative_values=negative_values,
-                plot=False, out=True)
+                proj_method=proj_method, plot=False, out=True)
     # Sav file
     input_params = {
         'omega_list' : od.get_names(omega_list),
         'lat_min' : lat_min,
         'lat_max' : lat_max,
         'lon_min' : lon_min,
         'lon_max' : lon_max,
         'pas_lat' : pas_lat,
         'pas_lon' : pas_lon,
         'data'    : data_desc,
         'filename': sav_filename,
-        'datetime': datetime.datetime.now().strftime('%d/%m/%Y %H:%M')}
+        'datetime': datetime.datetime.now().strftime('%d/%m/%Y %H:%M'),
+        'proj_method' : proj_method,
+            }
     save_file = {
         'data' : data,
         'mask' : mask,
         'grid_lat' : grid_lat,
         'grid_lon' : grid_lon,
         'mask_obs' : mask_obs,
         'infos' : input_params
@@ -1384,25 +1629,26 @@
         plt.xlim(lon_min, lon_max)
         plt.ylim(lat_min, lat_max)
     if cbar:
         if cb_title == 'auto':
             cb_title = infos['data']
         cb = plt.colorbar()
         cb.set_label(cb_title)
+    plt.grid(visible=False)
     if grid:
         ax = plt.figure(Nfig).get_axes()[0]
         lonlim = ax.get_xlim()
         latlim = ax.get_ylim()
         lon_sgn = np.sign(lonlim[1] - lonlim[0])
         lat_sgn = np.sign(latlim[1] - latlim[0])
         lon_grid = np.arange(np.round(lonlim[0]/10)*10, np.round(lonlim[1]/10)*10+lon_sgn, 
                     10 * lon_sgn)   # 10° grid in longitude
         lat_grid = np.arange(np.round(latlim[0]/10)*10, np.round(latlim[1]/10)*10+lat_sgn, 
                     10 * lat_sgn)   # 10° grid in latitude
-        plt.grid()
+        plt.grid(visible=True)
         if polar:
             ax.set_rticks(lat_grid)
         else:
             ax.set_xticks(lon_grid)
             ax.set_yticks(lat_grid)
     plt.title(title)
     plt.tight_layout()
@@ -1447,345 +1693,10 @@
         ylabel = 'Ratioed reflectance'
     plt.figure(Nfig)
     plt.plot(lam, sp, *args, **kwargs)
     plt.xlabel('λ [µm]')
     plt.ylabel(ylabel)
     plt.tight_layout()
 
-# ##----------------------------------------------------------------------------------------
-# ## Affichage cartes composites - sauvegardées high-level
-# def proj_grid_v3(Lat, Lon, data, lat_min=-90, lat_max=90, lon_min=0, lon_max=360,
-                 # pas_lat=0.1, pas_lon=0.1):
-    # """Sample the data from the input OMEGA/MEx observation on a given lat/lon grid.
-
-    # Parameters
-    # ==========
-    # Lat : 2D array
-        # The array of latitudes for each pixel of data.
-    # Lon : 2D array
-        # The array of longitudes for each pixel of data.
-    # data : 2D array
-        # The initial array of values from an OMEGA/MEx observation.
-        # e.g.: Refelectance at selected wvl, spectra, or derived data such as IBD map.
-    # lat_min : float, optional (default -90)
-        # The minimal latitude of the grid.
-    # lat_max : float, optional (default 90)
-        # The maximum latitude of the grid.
-    # lon_min : float, optional (default 0)
-        # The minimal longitude of the grid.
-    # lon_max : float, optional (default 360)
-        # The maximal longitude of the grid.
-    # pas_lat : float, optional (default 0.1)
-        # The latitude intervals of the grid.
-    # pas_lon : float, optional (default 0.1)
-        # The longitude intervals of the grid.
-
-    # Returns
-    # =======
-    # grid_data : 2D array (dim : Nlon x Nlat)
-        # The data values, sampled on the new lat/lon grid.
-    # mask : 2D array
-        # The array indicating where the new grid has been filled by the OMEGA data.
-    # grid lat : 2D array
-        # The new latitude grid.
-    # grid lon : 2D array
-        # The new longitude grid.
-    # """
-    # # Initialisation
-    # lat_array = np.arange(lat_min, lat_max+pas_lat, pas_lat)
-    # lon_array = np.arange(lon_min, lon_max+pas_lon, pas_lon)
-    # Nlon, Nlat = len(lon_array)-1, len(lat_array)-1
-    # grid_lat, grid_lon = np.meshgrid(lat_array, lon_array)
-    # grid_data = np.zeros((Nlon, Nlat))
-    # mask = np.zeros((Nlon, Nlat))
-    # lat2 = np.floor(np.clip(Lat, lat_min, lat_max-0.1*pas_lat) /pas_lat) * pas_lat
-    # lon2 = np.floor(np.clip(Lon, lon_min, lon_max-0.1*pas_lon) /pas_lon) * pas_lon
-    # nx, ny = lat2.shape
-    # # Sampling on the new grid
-    # for j in range(ny):
-        # for i in range(nx):
-            # longi, lati = lon2[i,j], lat2[i,j]
-            # i_lon = int(longi/pas_lon - lon_min/pas_lon)
-            # j_lat = int(lati/pas_lat - lat_min/pas_lat)
-            # data_tmp = data[i,j]
-            # if (not np.isnan(data_tmp)) & (data_tmp > 0):   # Filtrage régions sans données
-                # grid_data[i_lon,j_lat] += data_tmp
-                # mask[i_lon,j_lat] += 1
-    # grid_data[grid_data==0] = np.nan
-    # grid_data2 = grid_data / mask       # Normalisation
-    # mask2 = np.clip(mask, 0, 1)
-    # return grid_data2, mask2, grid_lat, grid_lon
-
-# def check_list_data_mask(data_list, mask_list, disp=True):
-    # """Check the compatibility between data_list and mask_list.
-    # Raise ValueError if uncompatibility.
-
-    # Parameters
-    # ==========
-    # data_list : 3D array
-        # List of high-level map associated to a sample of OMEGA/MEx observations.
-    # mask_list : 3D array
-        # List of masks to remove the corrupted pixels of each OMEGA/MEx observation.
-    # disp : bool, optional (default True)
-        # Enable the display of the result of the test.
-    # """
-    # if len(mask_list) != len(data_list):
-        # raise ValueError("data_list and mask_list must have the same size")
-    # else:
-        # for i in range(len(data_list)):
-            # if mask_list[i].shape != data_list[i].shape:
-                # raise ValueError("The shapes of items {0} of data_list and mask_list does not match.".format(i))
-    # if disp:
-        # print("\033[01;32mCompatibility between data_list and mask_list OK\033[0m")
-
-# def show_omega_list_v3(data_list, geom_list, lat_min=-90, lat_max=90, lon_min=0, lon_max=360,
-                       # pas_lat=0.1, pas_lon=0.1, cmap='Greys_r', vmin=None, vmax=None, 
-                       # title='auto', Nfig=None, polar=False, cbar=True, cb_title='auto',
-                       # mask_list=None, plot=True, grid=True, out=False, 
-                       # negatives_longitudes=False, **kwargs):
-    # """Display an composite map from a list OMEGA/MEx observations, sampled on a new lat/lon grid.
-    
-    # Specificities of v3 : use previously saved high-level data from OMEGA/MEx observations.
-
-    # Parameters
-    # ==========
-    # data_list : 3D array
-        # List of 2D array maps corresponding to severals OMEGA/MEx observations.
-    # geom_list : 1D array of dict
-        # List of dictionaries containing geometric informations corresponding to the 
-        # OMEGA/MEx observations that are in `data_list` in the **same order**.
-    # lat_min : float, optional (default -90)
-        # The minimal latitude of the grid.
-    # lat_max : float, optional (default 90)
-        # The maximum latitude of the grid.
-    # lon_min : float, optional (default 0)
-        # The minimal longitude of the grid.
-    # lon_max : float, optional (default 360)
-        # The maximal longitude of the grid.
-    # pas_lat : float, optional (default 0.1)
-        # The latitude intervals of the grid.
-    # pas_lon : float, optional (default 0.1)
-        # The longitude intervals of the grid.
-    # cmap : str, optional (default 'Greys_r')
-        # The matplotlib colormap.
-    # vmin : float or None, optional (default None)
-        # The lower bound of the coloscale.
-    # vmax : float or None, optional (default None)
-        # The upper bound of the colorscale.
-    # title : str, optional (default 'auto')
-        # The title of the figure.
-    # Nfig : int or str or None, optional (default None)
-        # The target figure ID.
-    # polar : bool, optional (default False)
-        # If True -> Use a polar projection for the plot.
-    # cbar : bool, optional (default True)
-        # If True -> Diplay the colorbar.
-    # cb_title : str, optional (default 'auto')
-        # The title of the colorbar.
-    # mask_list : 3D array
-        # 1D array of the same dimension of `omega_list` containing the masks to remove the
-        # corrupted pixels of each observaiton, in the **same order** that the observations of 
-        # `data_list`.
-        # Each mask is a 2D array, filled with 1 for good pixels and NaN for bad ones.
-    # plot : bool, optional (default True)
-        # If True -> Diplay the final figure.
-    # grid : bool, optional (default True)
-        # Enable the display of the lat/lon grid.
-    # out : bool, optional (default False)
-        # If True -> Return output.
-    # negatives_longitudes : bool, optional (default False)
-        # Argument for non-polar plots.
-        # | True -> longitudes between 0° and 360°.
-        # | False -> longitudus between -180° and 180°.
-    # **kwargs:
-        # Optional arguments for the plt.pcolormesh() function.
-
-    # Returns (if out=True)
-    # =======
-    # data : 2D array (dim : Nlon x Nlat)
-        # The omega reflectance at lam, sampled on the new lat/lon grid.
-    # mask : 2D array
-        # The array indicating where the new grid has been filled by the OMEGA data.
-    # grid lat : 2D array
-        # The new latitude grid.
-    # grid lon : 2D array
-        # The new longitude grid.
-    # mask_obs : 2D array of str
-        # The array indicating which observations have been used to fill each grid position.
-    # """
-    # # Init grids
-    # lat_array = np.arange(lat_min, lat_max+pas_lat, pas_lat)
-    # lon_array = np.arange(lon_min, lon_max+pas_lon, pas_lon)
-    # Nlon, Nlat = len(lon_array)-1, len(lat_array)-1
-    # grid_lat, grid_lon = np.meshgrid(lat_array, lon_array)
-    # data, mask = np.zeros((Nlon, Nlat)), np.zeros((Nlon, Nlat))
-    # mask_obs = np.ndarray((Nlon, Nlat), dtype=object)
-    # mask_obs.fill('')
-    # # Test compatibility
-    # # > add test avec geom
-    # if not (mask_list is None):
-        # check_list_data_mask(data_list, mask_list, disp=True)
-    # # Loop on observations -> sampling and projection on the same grid
-    # for i in tqdm(range(len(data_list))):
-        # if mask_list is None:
-            # data_tmp = data_list[i]     # Data without mask
-        # else:
-            # data_tmp = data_list[i] * mask_list[i]  # Data with mask
-        # data0, mask0 = proj_grid_v3(geom_list[i]['lat'], geom_list[i]['lon'], data_tmp, 
-                                    # lat_min, lat_max, lon_min, lon_max, pas_lat, pas_lon)[:2]
-        # data += np.nan_to_num(data0)    # Conversion NaN -> 0 pour somme des images
-        # mask += mask0
-        # mask_obs[mask0 == 1] += (geom_list[i]['obsname'] + ',')
-    # data[mask == 0] = np.nan
-    # data2 = data/mask   # Normalisation
-    # # Affichage figure
-    # if plot:
-        # if title == 'auto':
-            # title = 'Composite map from OMEGA/MEx observations' 
-        # fig = plt.figure(Nfig)
-        # Nfig = fig.number   # get the actual figure number if Nfig=None
-        # if polar:
-            # ax = plt.axes(polar=True)
-            # plt.pcolormesh(grid_lon*np.pi/180, grid_lat, data2, cmap=cmap, 
-                        # vmin=vmin, vmax=vmax, **kwargs)
-            # ax.set_yticklabels([])  # remove the latitude values in the plot
-            # plt.xlim(0, 2*np.pi)
-            # if np.abs(lat_max) >= np.abs(lat_min):
-                # latlim = (lat_max, lat_min)
-            # else:
-                # latlim = (lat_min, lat_max)
-            # if latlim[0] > 0:   # Northern hemisphere
-                # ax.set_theta_offset(-np.pi/2)   # longitude origin at the bottom
-            # else:               # Southern hemisphere
-                # ax.set_theta_offset(np.pi/2)    # longitude origin at the top
-                # ax.set_theta_direction(-1)      # clockwise theta
-            # plt.ylim(latlim)
-        # else:
-            # if negatives_longitudes and (lon_max > 180):
-                # n_neg_lon = np.sum(grid_lon[:,0] > 180) # nb of negative longitudes (>180°)
-                # i_lon180 = np.where(grid_lon[:,0] > 180)[0][0] # 1st index of lon > 180°
-                # grid_lon_nl = deepcopy(grid_lon)        # new longitude grid [-180°, 180°]
-                # grid_lon_nl[:n_neg_lon] = grid_lon[i_lon180-1:-1] - 360
-                # grid_lon_nl[n_neg_lon:] = grid_lon[:i_lon180]
-                # data2_nl = deepcopy(data2)      # new data array
-                # data2_nl[:n_neg_lon] = data2[i_lon180-1:]
-                # data2_nl[n_neg_lon:] = data2[:i_lon180-1]
-                # plt.pcolormesh(grid_lon_nl, grid_lat, data2_nl, cmap=cmap, vmin=vmin, 
-                               # vmax=vmax, **kwargs)
-                # lon_min, lon_max = grid_lon_nl[[0,-1], 0]   # new longitude bounds
-            # else:
-                # plt.pcolormesh(grid_lon, grid_lat, data2, cmap=cmap, vmin=vmin, 
-                               # vmax=vmax, **kwargs)
-            # plt.gca().axis('equal')
-            # plt.gca().set_adjustable('box')
-            # plt.xlabel('Longitude [°]')
-            # plt.ylabel('Latitude [°]')
-            # plt.xlim(lon_min, lon_max)
-            # plt.ylim(lat_min, lat_max)
-        # if cbar:
-            # if cb_title == 'auto':
-                # cb_title = r'Reflectance @ $\lambda$' + ' = {0:.2f} µm'.format(lam)
-            # cb = plt.colorbar()
-            # cb.set_label(cb_title)
-        # if grid:
-            # ax = plt.figure(Nfig).get_axes()[0]
-            # lonlim = ax.get_xlim()
-            # latlim = ax.get_ylim()
-            # lon_sgn = np.sign(lonlim[1] - lonlim[0])
-            # lat_sgn = np.sign(latlim[1] - latlim[0])
-            # lon_grid = np.arange(np.round(lonlim[0]/10)*10, np.round(lonlim[1]/10)*10+lon_sgn, 
-                        # 10 * lon_sgn)   # 10° grid in longitude
-            # lat_grid = np.arange(np.round(latlim[0]/10)*10, np.round(latlim[1]/10)*10+lat_sgn, 
-                        # 10 * lat_sgn)   # 10° grid in latitude
-            # plt.grid()
-            # if polar:
-                # ax.set_rticks(lat_grid)
-            # else:
-                # ax.set_xticks(lon_grid)
-                # ax.set_yticks(lat_grid)
-        # plt.title(title)
-        # plt.tight_layout()
-    # # Output
-    # if out:
-        # mask2 = np.clip(mask, 0, 1)
-        # return data2, mask2, grid_lat, grid_lon, mask_obs
-
-# def save_map_omega_list_v3(data_list, geom_list, lat_min=-90, lat_max=90, lon_min=0, lon_max=360,
-                           # pas_lat=0.1, pas_lon=0.1, data_desc='', mask_list=None, sav_filename='auto', ext='',
-                           # base_folder='../data/OMEGA/sav_map_list_v2/', sub_folder=''):
-    # """Save the output of the omega_plots.show_omega_list_v2() function with the requested
-    # parameters as a dictionary.
-
-    # Parameters
-    # ==========
-    # data_list : 3D array
-        # List of 2D array maps corresponding to severals OMEGA/MEx observations.
-    # geom_list : 1D array of dict
-        # List of dictionaries containing geometric informations corresponding to the 
-        # OMEGA/MEx observations that are in `data_list` in the **same order**.
-    # lat_min : float, optional (default -90)
-        # The minimal latitude of the grid.
-    # lat_max : float, optional (default 90)
-        # The maximum latitude of the grid.
-    # lon_min : float, optional (default 0)
-        # The minimal longitude of the grid.
-    # lon_max : float, optional (default 360)
-        # The maximal longitude of the grid.
-    # pas_lat : float, optional (default 0.1)
-        # The latitude intervals of the grid.
-    # pas_lon : float, optional (default 0.1)
-        # The longitude intervals of the grid.
-    # data_desc : str, optional (default '')
-        # Description of the data contained in data_list (if used).
-    # mask_list : 3D array
-        # 1D array of the same dimension of `omega_list` containing the masks to remove the
-        # corrupted pixels of each observaiton, in the **same order** than the observations of 
-        # `omega_list`.
-        # Each mask is a 2D array, filled with 1 for good pixels and NaN for bad ones.
-    # sav_filename : str, optional (default 'auto')
-        # The saving file name.
-        # | If 'auto' -> Automatically generated.
-    # ext : str, optional (default '')
-        # Extension to add at the end of the filename (useful in case of automatic generation).
-    # base_folder : str, optional (default '../data/OMEGA/sav_map_list_v2/')
-        # The base folder to save the data.
-    # sub_folder : str, optional (default '')
-        # The subfolder to save the data.
-        # Final path = "base_folder / sub_folder / sav_filename"
-    # """
-    # # Initialization filename
-    # if sav_filename == 'auto':
-        # sav_filename = ('res_show_omega_list_v3__lat{0:0>2d}-{1:0>2d}_pas{2:0}_'
-                        # + 'lon{3:0>3d}-{4:0>3d}_pas{5:0}__{6:s}.pkl').format(
-                            # lat_min, lat_max, pas_lat, lon_min, lon_max, pas_lon, ext)
-    # sav_filename2 = os.path.join(base_folder, sub_folder, sav_filename)
-    # if data_desc == '':
-        # data_desc = 'unknown data'
-    # # Compute the data sampling
-    # data, mask, grid_lat, grid_lon, mask_obs = show_omega_list_v3(data_list,
-                # geom_list, lat_min, lat_max, lon_min, lon_max, pas_lat, pas_lon,
-                # mask_list=mask_list, plot=False, out=True)
-    # # Sav file
-    # input_params = {
-        # 'omega_list' : np.array([geom_obs['obsname'] for geom_obs in geom_list]),
-        # 'lat_min' : lat_min,
-        # 'lat_max' : lat_max,
-        # 'lon_min' : lon_min,
-        # 'lon_max' : lon_max,
-        # 'pas_lat' : pas_lat,
-        # 'pas_lon' : pas_lon,
-        # 'data'    : data_desc,
-        # 'filename': sav_filename,
-        # 'datetime': datetime.datetime.now().strftime('%d/%m/%Y %H:%M')}
-    # save_file = {
-        # 'data' : data,
-        # 'mask' : mask,
-        # 'grid_lat' : grid_lat,
-        # 'grid_lon' : grid_lon,
-        # 'mask_obs' : mask_obs,
-        # 'infos' : input_params
-                # }
-    # uf.save_pickle(save_file, sav_filename2, True)
-    
 ##----------------------------------------------------------------------------------------
 ## End of code
 ##----------------------------------------------------------------------------------------
```

### Comparing `omegapy-2.3/omegapy/res_findcube/cubelist` & `omegapy-2.4/omegapy/res_findcube/cubelist`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy/useful_functions.py` & `omegapy-2.4/omegapy/useful_functions.py`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/omegapy.egg-info/PKG-INFO` & `omegapy-2.4/omegapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: omegapy
-Version: 2.3
+Version: 2.4
 Summary: Python tools for OMEGA/MEx observations analysis
 Home-page: https://astcherbinine.github.io/omegapy
 Author: Aurélien Stcherbinine
 Author-email: aurelien@stcherbinine.net
 Project-URL: Source, https://github.com/AStcherbinine/omegapy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![version](https://img.shields.io/badge/version-2.3-blue)
+![version](https://img.shields.io/badge/version-2.4-blue)
 ![pythonversion](https://img.shields.io/badge/Python-3.7+-blue)
+[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/badge/latestdoi/349763849)
+
 
 <p align="center">
 <img width="250" height="250" src="https://github.com/AStcherbinine/omegapy/blob/master/docs/logo_omegapy_small2.png">
 </p>
 
 # OMEGA-Py : Python tools for OMEGA data
 
@@ -102,22 +104,27 @@
 # Simultaneous Atmospheric & Thermal corrections (for the use of the L-channel)
 # > Use the `npool` argument to control the number of simultaneous processes used to compute the thermal correction 
 # > (e.g., npool=15 is usually a nice choice if your system can handle it)
 # > Note: multiprocessing is currently not available for Windows
 omega_corr_therm_atm = od.corr_therm_atm(omega_corr, npool=1)
 # Thermal correction only
 omega_corr_therm = od.corr_therm(omega, npool=1)
+# OMEGA mask to hide bad pixels / calibration lines
+mask = od.omega_mask(omega, hide_128=True, emer_lim=10, inci_lim=70, temc_lim=-194, limsat_c=500)
 # Interactive display of the observation (@ λ = 1.085 µm)
 op.show_omega_interactif_v2(omega_corr_therm_atm, lam=1.085, cmap='Greys_r', vmin=0, vmax=0.5, polar=True)
 # Search for the index of λ = 1.085 µm in the wavelength array
 i_lam = uf.where_closer(1.085, omega.lam)
 ~~~
 
+## Documentation
 See [`docs/*.md`](https://github.com/AStcherbinine/omegapy/blob/master/docs/) or the interactive IPython help for more details.
 
+Planetary Data Workshop 2023: [abstract](https://github.com/AStcherbinine/omegapy/blob/master/docs/Stcherbinine_PDW2023_7007_omegapy.pdf) & [slides](https://github.com/AStcherbinine/omegapy/blob/master/docs/PDW_Flagstaff_Stcherbinine_omegapy_upload.pdf)
+
 ## Credits
 
 © Aurélien Stcherbinine (2020–2023)
 
 Institut d'Astrophysique Spatiale (IAS), Université Paris-Saclay, CNRS, Orsay, France
 
 LATMOS/IPSL, UVSQ Université Paris-Saclay, Sorbonne Université, CNRS, Guyancourt, France
```

### Comparing `omegapy-2.3/omegapy.egg-info/SOURCES.txt` & `omegapy-2.4/omegapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegapy-2.3/setup.py` & `omegapy-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 package_data = {
     '': ['OMEGA_dataref/*', 'res_findcube/*'],
     }
 
 setuptools.setup(
     name='omegapy',
-    version='2.3',
+    version='2.4',
     author='Aurélien Stcherbinine',
     author_email='aurelien@stcherbinine.net',
     description='Python tools for OMEGA/MEx observations analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://astcherbinine.github.io/omegapy',
     project_urls={
```

