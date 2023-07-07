# Comparing `tmp/astro-eddy-2.3.7.tar.gz` & `tmp/astro-eddy-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-eddy-2.3.7.tar", last modified: Fri Mar 31 20:03:01 2023, max compression
+gzip compressed data, was "astro-eddy-2.3.9.tar", last modified: Mon May 15 18:14:15 2023, max compression
```

## Comparing `astro-eddy-2.3.7.tar` & `astro-eddy-2.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-03-31 20:03:01.551277 astro-eddy-2.3.7/
--rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/LICENSE.md
--rw-r--r--   0 richardteague   (501) staff       (20)       33 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/MANIFEST.in
--rw-r--r--   0 richardteague   (501) staff       (20)     3300 2023-03-31 20:03:01.551160 astro-eddy-2.3.7/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     2858 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-03-31 20:03:01.547262 astro-eddy-2.3.7/astro_eddy.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)     3300 2023-03-31 20:03:01.000000 astro-eddy-2.3.7/astro_eddy.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      465 2023-03-31 20:03:01.000000 astro-eddy-2.3.7/astro_eddy.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-03-31 20:03:01.000000 astro-eddy-2.3.7/astro_eddy.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       58 2023-03-31 20:03:01.000000 astro-eddy-2.3.7/astro_eddy.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        5 2023-03-31 20:03:01.000000 astro-eddy-2.3.7/astro_eddy.egg-info/top_level.txt
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-03-31 20:03:01.548678 astro-eddy-2.3.7/docs/
--rw-r--r--   0 richardteague   (501) staff       (20)     6148 2023-03-28 14:40:45.000000 astro-eddy-2.3.7/docs/.DS_Store
--rw-r--r--   0 richardteague   (501) staff       (20)      580 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/docs/Makefile
--rw-r--r--   0 richardteague   (501) staff       (20)     1794 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/docs/citations.md
--rw-r--r--   0 richardteague   (501) staff       (20)     2254 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/docs/conf.py
--rw-r--r--   0 richardteague   (501) staff       (20)     1820 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/docs/index.rst
--rw-r--r--   0 richardteague   (501) staff       (20)       68 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/docs/requirements.txt
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-03-31 20:03:01.550927 astro-eddy-2.3.7/eddy/
--rw-r--r--   0 richardteague   (501) staff       (20)      147 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/eddy/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)    64943 2023-03-28 19:14:26.000000 astro-eddy-2.3.7/eddy/annulus.py
--rw-r--r--   0 richardteague   (501) staff       (20)    60651 2023-03-29 18:55:17.000000 astro-eddy-2.3.7/eddy/datacube.py
--rw-r--r--   0 richardteague   (501) staff       (20)     3954 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/eddy/default_parameters.yml
--rw-r--r--   0 richardteague   (501) staff       (20)    16855 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/eddy/helper_functions.py
--rw-r--r--   0 richardteague   (501) staff       (20)    27532 2023-03-29 16:05:04.000000 astro-eddy-2.3.7/eddy/linecube.py
--rw-r--r--   0 richardteague   (501) staff       (20)    10532 2023-03-27 18:31:02.000000 astro-eddy-2.3.7/eddy/modelling.py
--rw-r--r--   0 richardteague   (501) staff       (20)    89534 2023-03-31 19:51:31.000000 astro-eddy-2.3.7/eddy/rotationmap.py
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-03-31 20:03:01.551318 astro-eddy-2.3.7/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)      914 2023-03-31 19:44:34.000000 astro-eddy-2.3.7/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-05-15 18:14:15.009620 astro-eddy-2.3.9/
+-rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/LICENSE.md
+-rw-r--r--   0 richardteague   (501) staff       (20)       33 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/MANIFEST.in
+-rw-r--r--   0 richardteague   (501) staff       (20)     3300 2023-05-15 18:14:15.009504 astro-eddy-2.3.9/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     2858 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-05-15 18:14:15.006835 astro-eddy-2.3.9/astro_eddy.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)     3300 2023-05-15 18:14:14.000000 astro-eddy-2.3.9/astro_eddy.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      465 2023-05-15 18:14:14.000000 astro-eddy-2.3.9/astro_eddy.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-05-15 18:14:14.000000 astro-eddy-2.3.9/astro_eddy.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       72 2023-05-15 18:14:14.000000 astro-eddy-2.3.9/astro_eddy.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        5 2023-05-15 18:14:14.000000 astro-eddy-2.3.9/astro_eddy.egg-info/top_level.txt
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-05-15 18:14:15.007952 astro-eddy-2.3.9/docs/
+-rw-r--r--   0 richardteague   (501) staff       (20)     6148 2023-04-17 18:17:39.000000 astro-eddy-2.3.9/docs/.DS_Store
+-rw-r--r--   0 richardteague   (501) staff       (20)      580 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/docs/Makefile
+-rw-r--r--   0 richardteague   (501) staff       (20)     1794 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/docs/citations.md
+-rw-r--r--   0 richardteague   (501) staff       (20)     2254 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/docs/conf.py
+-rw-r--r--   0 richardteague   (501) staff       (20)     1820 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/docs/index.rst
+-rw-r--r--   0 richardteague   (501) staff       (20)       68 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/docs/requirements.txt
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-05-15 18:14:15.009265 astro-eddy-2.3.9/eddy/
+-rw-r--r--   0 richardteague   (501) staff       (20)      147 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/eddy/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    77572 2023-04-04 19:10:44.000000 astro-eddy-2.3.9/eddy/annulus.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    74008 2023-04-26 15:23:48.000000 astro-eddy-2.3.9/eddy/datacube.py
+-rw-r--r--   0 richardteague   (501) staff       (20)     3954 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/eddy/default_parameters.yml
+-rw-r--r--   0 richardteague   (501) staff       (20)    16855 2023-04-04 14:17:34.000000 astro-eddy-2.3.9/eddy/helper_functions.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    27859 2023-04-17 18:21:13.000000 astro-eddy-2.3.9/eddy/linecube.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    10532 2023-03-27 18:31:02.000000 astro-eddy-2.3.9/eddy/modelling.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    88645 2023-04-17 17:58:28.000000 astro-eddy-2.3.9/eddy/rotationmap.py
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-05-15 18:14:15.009657 astro-eddy-2.3.9/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)      939 2023-04-26 14:25:25.000000 astro-eddy-2.3.9/setup.py
```

### Comparing `astro-eddy-2.3.7/LICENSE.md` & `astro-eddy-2.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/PKG-INFO` & `astro-eddy-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-eddy
-Version: 2.3.7
+Version: 2.3.9
 Summary: Tools to study the dynamics of protoplanetary disks.
 Home-page: https://github.com/richteague/eddy
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-eddy Version: 2.3.7 Summary: Tools to study
+Metadata-Version: 2.1 Name: astro-eddy Version: 2.3.9 Summary: Tools to study
 the dynamics of protoplanetary disks. Home-page: https://github.com/richteague/
 eddy Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE.md # eddy -
 Extracting Disk Dynamics
```

### Comparing `astro-eddy-2.3.7/README.md` & `astro-eddy-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/astro_eddy.egg-info/PKG-INFO` & `astro-eddy-2.3.9/astro_eddy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-eddy
-Version: 2.3.7
+Version: 2.3.9
 Summary: Tools to study the dynamics of protoplanetary disks.
 Home-page: https://github.com/richteague/eddy
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-eddy Version: 2.3.7 Summary: Tools to study
+Metadata-Version: 2.1 Name: astro-eddy Version: 2.3.9 Summary: Tools to study
 the dynamics of protoplanetary disks. Home-page: https://github.com/richteague/
 eddy Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE.md # eddy -
 Extracting Disk Dynamics
```

### Comparing `astro-eddy-2.3.7/docs/.DS_Store` & `astro-eddy-2.3.9/docs/.DS_Store`

 * *Files 21% similar despite different names*

```diff
@@ -28,44 +28,44 @@
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0004 0000 0009  ................
 00000210: 0074 0075 0074 006f 0072 0069 0061 006c  .t.u.t.o.r.i.a.l
-00000220: 0073 6277 7370 626c 6f62 0000 00b8 6270  .sbwspblob....bp
+00000220: 0073 6277 7370 626c 6f62 0000 00b9 6270  .sbwspblob....bp
 00000230: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
 00000240: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 00000250: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 00000260: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 00000270: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 00000280: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00000290: 6f77 5369 6465 6261 7208 0908 095f 1018  owSidebar...._..
-000002a0: 7b7b 3136 382c 2033 3331 7d2c 207b 3932  {{168, 331}, {92
-000002b0: 302c 2034 3336 7d7d 0908 1523 2f3b 525f  0, 436}}...#/;R_
-000002c0: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
-000002d0: 0000 0000 000d 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 008b 0000 0009 0074 0075 0074  ...........t.u.t
-000002f0: 006f 0072 0069 0061 006c 0073 7653 726e  .o.r.i.a.l.svSrn
-00000300: 6c6f 6e67 0000 0001 0000 0004 0075 0073  long.........u.s
-00000310: 0065 0072 6277 7370 626c 6f62 0000 00b8  .e.rbwspblob....
-00000320: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
-00000330: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00000340: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
-00000350: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00000360: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00000370: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00000380: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-00000390: 1018 7b7b 3239 362c 2033 3831 7d2c 207b  ..{{296, 381}, {
-000003a0: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
-000003b0: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
-000003c0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
-000003d0: 0000 0000 0000 008b 0000 0004 0075 0073  .............u.s
-000003e0: 0065 0072 7653 726e 6c6f 6e67 0000 0001  .e.rvSrnlong....
-000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 6f77 5369 6465 6261 7208 0908 095f 1019  owSidebar...._..
+000002a0: 7b7b 3239 362c 2032 3832 7d2c 207b 3131  {{296, 282}, {11
+000002b0: 3738 2c20 3533 357d 7d09 0815 232f 3b52  78, 535}}...#/;R
+000002c0: 5f6b 6c6d 6e6f 8b00 0000 0000 0001 0100  _klmno..........
+000002d0: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 8c00 0000 0900 7400 7500  ............t.u.
+000002f0: 7400 6f00 7200 6900 6100 6c00 7376 5372  t.o.r.i.a.l.svSr
+00000300: 6e6c 6f6e 6700 0000 0100 0000 0400 7500  nlong.........u.
+00000310: 7300 6500 7262 7773 7062 6c6f 6200 0000  s.e.rbwspblob...
+00000320: b962 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00000330: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
+00000340: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
+00000350: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00000360: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00000370: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00000380: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
+00000390: 5f10 197b 7b32 3936 2c20 3238 327d 2c20  _..{{296, 282}, 
+000003a0: 7b31 3137 382c 2035 3335 7d7d 0908 1523  {1178, 535}}...#
+000003b0: 2f3b 525f 6b6c 6d6e 6f8b 0000 0000 0000  /;R_klmno.......
+000003c0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
+000003d0: 0000 0000 0000 0000 008c 0000 0004 0075  ...............u
+000003e0: 0073 0065 0072 7653 726e 6c6f 6e67 0000  .s.e.rvSrnlong..
+000003f0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `astro-eddy-2.3.7/docs/Makefile` & `astro-eddy-2.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/docs/citations.md` & `astro-eddy-2.3.9/docs/citations.md`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/docs/conf.py` & `astro-eddy-2.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/docs/index.rst` & `astro-eddy-2.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/eddy/annulus.py` & `astro-eddy-2.3.9/eddy/annulus.py`

 * *Files 15% similar despite different names*

```diff
@@ -113,17 +113,18 @@
         else:
             return [self.velax_grid[0], self.velax_grid[-1],
                     self.theta_grid[0], self.theta_grid[-1]]
 
     # -- Measure the Velocity -- #
 
     def get_vlos(self, p0=None, fit_method='SHO', fit_vrad=False, fix_vlsr=None,
-                 resample=None, optimize=True, nwalkers=32, nburnin=500,
-                 nsteps=500, scatter=1e-3, signal='int', optimize_kwargs=None,
-                 mcmc='emcee', mcmc_kwargs=None, centroid_method='quadratic'):
+            vrot_mask=None, vlsr_mask=None, vrad_mask=None, dv_mask=None,
+            resample=None, optimize=True, nwalkers=32, nburnin=500, nsteps=500,
+            scatter=1e-3, signal='int', optimize_kwargs=None, mcmc='emcee',
+            mcmc_kwargs=None, centroid_method='quadratic', repeat_with_mask=0):
         """
         Infer the requested velocities by shifting lines back to a common
         center and stacking. The quality of fit is given by the selected
         method which must be ``'dv'``, ``'GP'``, ``'SNR'`` or ``'SHO'``. The
         former, described in `Teague et al. (2018a)`_, minimizes the line width
         of the resulting spectrum via :func:`deprojected_width`. Similarly,
         ``fit_method='SNR'`` aims to maximize the signal to noise of the
@@ -135,34 +136,47 @@
         oscillator, as in `Casassus & Perez (2019)`_.
 
         Different types of resampling can be applied to the spectrum. In
         general it is recommended that ``resample=False`` for the Gaussian
         Process approach, while ``resample=True`` for the other two.
 
         Args:
-            fit_method (optional[str]): Method used to define the quality of
-                fit. Must be one of ``'GP'``, ``'dV'``, ``'SNR'`` or ``'SHO'``.
             p0 (optional[list]): Starting positions for the minimization. If
                 nothing is provided these will be guessed but this may not
                 result in very good starting positions.
+            fit_method (optional[str]): Method used to define the quality of
+                fit. Must be one of ``'GP'``, ``'dV'``, ``'SNR'`` or ``'SHO'``.
             fit_vrad (bool): Include radial motion in the fit.
             fix_vlsr (optional[bool]): Fix the systemic velocity to calculate
                 the deprojected vertical velocities. Only available for
                 `fit_method='SHO'`.
+            vrot_mask (optional[float]):
+            vlsr_mask (optional[float]):
+            vrad_mask (optional[float]):
+            dv_mask (optional[float]):
             resample (optional[bool]): Resampling method to apply. See
                 :func:`deprojected_spectrum` for more details.
             optimize (optional[bool]): Optimize the starting positions before
                 the MCMC runs. If an integer, the number of iterations to use
                 of optimization.
             nwalkers (optional[int]): Number of walkers used for the MCMC runs.
             nburnin (optional[int]): Number of steps used to burn in walkers.
             nsteps (optional[int]): Number of steps taken to sample posteriors.
             scatter (optional[float]): Scatter applied to the starting
                 positions before running the MCMC.
+            signal (optional[str]):
+            optimize_kwargs (optional[dict]):
+            mcmc (optional[str]):
+            mcmc_kwargs (optional[dict]):
+            centroid_method (optional[str]): Method used to determine the line
+                centroids, and must be one of ``'quadratic'``, ``'max'``,
+                ``'gaussian'``, ``'doublegauss'`` or ``'doublegauss_fixeddv'``.
             plots (optional[list]):
+            repeat_with_mask (optional[int]): Number of iterations to use.
+                Currently only works with `fit_method='SHO'`.
 
         Returns:
             Either the samples of the posterior for each free parameter, or the
             16th, 50th and 84th pecentiles of the distributions depending on
             what ``returns`` was set to.
 
         .. _Teague et al. (2018a): https://ui.adsabs.harvard.edu/abs/2018ApJ...860L..12T/abstract
@@ -181,60 +195,121 @@
         if fix_vlsr is not None and fit_method != 'sho':
             print("WARNING: fix_vlsr only available for fit_method='SHO'.")
 
         # Run the appropriate methods.
 
         if fit_method == 'gp':
             resample = False if resample is None else resample
-            popt = self.get_vlos_GP(p0=p0, fit_vrad=fit_vrad,
-                                    nwalkers=nwalkers, nsteps=nsteps,
-                                    nburnin=nburnin, scatter=scatter,
-                                    plots='none', returns='percentiles',
-                                    resample=resample, mcmc=mcmc,
+            popt = self.get_vlos_GP(p0=p0,
+                                    fit_vrad=fit_vrad,
+                                    vlsr_mask=vlsr_mask,
+                                    dv_mask=dv_mask,
+                                    nwalkers=nwalkers,
+                                    nsteps=nsteps,
+                                    nburnin=nburnin,
+                                    scatter=scatter,
+                                    plots='none',
+                                    returns='percentiles',
+                                    resample=resample,
+                                    mcmc=mcmc,
                                     optimize_kwargs=optimize_kwargs,
                                     mcmc_kwargs=mcmc_kwargs)
             cvar = 0.5 * (popt[:, 2] - popt[:, 0])
-            popt = popt[:, 1]
-            return (popt[:2], cvar[:2]) if fit_vrad else (popt[0], cvar[0])
+            popt = popt[:2, 1] if fit_vrad else popt[:1, 1]
+            cvar = cvar[:2] if fit_vrad else cvar[:1]
 
         elif fit_method == 'dv':
             resample = True if resample is None else resample
-            popt = self.get_vlos_dV(p0=p0, fit_vrad=fit_vrad,
+            popt = self.get_vlos_dV(p0=p0,
+                                    fit_vrad=fit_vrad,
                                     resample=resample,
+                                    vlsr_mask=vlsr_mask,
+                                    dv_mask=dv_mask,
                                     optimize_kwargs=optimize_kwargs)
-            return popt[:2] if fit_vrad else popt[0]
+            popt = popt[:2] if fit_vrad else popt[:1]
+            cvar = np.ones(popt.size) * np.nan
 
         elif fit_method == 'snr':
             resample = True if resample is None else resample
-            popt = self.get_vlos_SNR(p0=p0, fit_vrad=fit_vrad,
-                                     resample=resample, signal=signal,
+            popt = self.get_vlos_SNR(p0=p0,
+                                     fit_vrad=fit_vrad,
+                                     resample=resample,
+                                     signal=signal,
+                                     vlsr_mask=vlsr_mask,
+                                     dv_mask=dv_mask,
                                      optimize_kwargs=optimize_kwargs)
-            return popt[:2] if fit_vrad else popt[0]
+            popt = popt[:2] if fit_vrad else popt[:1]
+            cvar = np.ones(popt.size) * np.nan
 
         elif fit_method == 'sho':
             popt, cvar = self.get_vlos_SHO(p0=p0, 
                                            fit_vrad=fit_vrad,
                                            fix_vlsr=fix_vlsr,
+                                           vrot_mask=vrot_mask,
+                                           vlsr_mask=vlsr_mask,
+                                           vrad_mask=vrad_mask,
+                                           dv_mask=dv_mask,
                                            centroid_method=centroid_method,
                                            optimize_kwargs=optimize_kwargs)
-            return popt, cvar
+            
+        # If required, iterate using these results as a mask. This is only
+        # available with SHO given that a systemic velocity is required.
+
+        if repeat_with_mask and fit_method == 'sho':
+
+            vrot_mask = popt[0]
+            vrad_mask = popt[1] if fit_vrad else 0.0
+            vlsr_mask = popt[2] if fit_vrad else popt[1]
+
+            # Here somtimes the guess is sufficiently bad that it'll mask out
+            # all the points. If this is the case, we just skip this and move
+            # on.
+
+            try:
+                return self.get_vlos(p0=p0,
+                                    fit_method=fit_method,
+                                    fit_vrad=fit_vrad,
+                                    fix_vlsr=fix_vlsr,
+                                    vrot_mask=vrot_mask,
+                                    vlsr_mask=vlsr_mask,
+                                    vrad_mask=vrad_mask,
+                                    dv_mask=dv_mask,
+                                    resample=resample,
+                                    optimize=optimize,
+                                    nwalkers=nwalkers,
+                                    nburnin=nburnin,
+                                    nsteps=nsteps,
+                                    scatter=scatter,
+                                    signal=signal,
+                                    optimize_kwargs=optimize_kwargs,
+                                    mcmc=mcmc,
+                                    mcmc_kwargs=mcmc_kwargs,
+                                    centroid_method=centroid_method,
+                                    repeat_with_mask=repeat_with_mask-1)
+            except:
+                return popt, cvar
+        
+        return popt, cvar
 
     # -- Gaussian Processes Approach -- #
 
-    def get_vlos_GP(self, p0=None, fit_vrad=False, optimize=False, nwalkers=64,
-        nburnin=50, nsteps=100, scatter=1e-3, niter=1, plots=None, returns=None,
-        resample=False, mcmc='emcee', optimize_kwargs=None, mcmc_kwargs=None):
+    def get_vlos_GP(self, p0=None, fit_vrad=False, vlsr_mask=None, dv_mask=None,
+        optimize=False, nwalkers=64,nburnin=50, nsteps=100, scatter=1e-3,
+        niter=1, plots=None, returns=None, resample=False, mcmc='emcee',
+        optimize_kwargs=None, mcmc_kwargs=None):
         """
         Determine the azimuthally averaged rotational (and optionally radial)
         velocity by finding the greatest overlap between 
 
         Args:
             p0 (optional[list]): Starting positions.
             fit_vrad (optional[bool]): Whether to also fit for radial
                 velocities. Default is ``False``.
+            vlsr_mask (optional[float]):
+            dv_mask (optional[float]):
             optimize (optional[bool]): Run an optimization step prior to the
                 MCMC.
             nwalkers (optional[int]): Number of walkers for the MCMC.
             nburnin (optional[int]): Number of steps to discard for burn-in.
             nsteps (optional[int]): Number of steps used to sample the
                 posterior distributions.
             scatter (optional[float]): Scatter of walkers around ``p0``.
@@ -278,15 +353,19 @@
             raise ValueError("WARNING: NaNs in the p0 array.")
 
         # Optimize the starting positions.
 
         if optimize:
             if optimize_kwargs is None:
                 optimize_kwargs = {}
-            p0 = self._optimize_p0_GP(p0, N=int(optimize), **optimize_kwargs)
+            p0 = self._optimize_p0_GP(p0,
+                                      N=int(optimize),
+                                      vlsr_mask=vlsr_mask,
+                                      dv_mask=dv_mask,
+                                      **optimize_kwargs)
 
         # Run the sampler.
 
         nsteps = np.atleast_1d(nsteps)
         nburnin = np.atleast_1d(nburnin)
         nwalkers = np.atleast_1d(nwalkers)
         mcmc_kwargs = {} if mcmc_kwargs is None else mcmc_kwargs
@@ -302,15 +381,18 @@
                 EnsembleSampler = emcee.EnsembleSampler
 
             p0 = random_p0(p0, scatter, nwalkers[n % nwalkers.size])
 
             sampler = EnsembleSampler(nwalkers[n % nwalkers.size],
                                       p0.shape[1],
                                       self._lnprobability,
-                                      args=(p0[:, 0].mean(), resample),
+                                      args=(p0[:, 0].mean(),
+                                            vlsr_mask,
+                                            dv_mask,
+                                            resample),
                                       moves=moves,
                                       pool=pool)
 
             total_steps = nburnin[n % nburnin.size] + nsteps[n % nsteps.size]
             sampler.run_mcmc(p0, total_steps, progress=progress, **mcmc_kwargs)
 
             # Split off the burnt in samples.
@@ -345,15 +427,16 @@
             idx = returns.index('percentiles')
             returns[idx] = np.percentile(samples, [16, 50, 84], axis=0).T
         if 'samples' in returns:
             idx = returns.index('samples')
             returns[idx] = samples
         return returns[0] if len(returns) == 1 else returns
 
-    def _optimize_p0_GP(self, p0, N=1, resample=True, verbose=False, **kwargs):
+    def _optimize_p0_GP(self, p0, N=1, vlsr_mask=None, dv_mask=None,
+                        resample=True, verbose=False, **kwargs):
         """
         Optimize the starting positions, p0. We do this in a slightly hacky way
         because the minimum is not easily found. We first optimize the hyper
         parameters of the GP model, holding the rotation velocity constant,
         then, holding the GP hyperparameters constant, optimizing the rotation
         velocity, before optimizing everything together. This can be run
         multiple times to iteratie to a global optimum. We only update p0 if
@@ -363,14 +446,16 @@
         One can also pass all the options to optimize.minimize to try different
         minimization techniques. The default values here were based on trial
         and error.
 
         Args:
             p0 (ndarray): Initial guess of the starting positions.
             N (Optional[int]): Interations of the optimization to run.
+            vlsr_mask (Optional[float]):
+            dv_mask (Optional[float]):
             resample (Optional[bool/int]): If true, resample the deprojected
                 spectra donw to the original velocity resolution. If an integer
                 is given, use this as the bew sampling rate relative to the
                 original data.
 
         Returns:
             p0 (ndarray): Optimized array. If scipy.minimize does not converge
@@ -387,82 +472,107 @@
                              'ftol': options.pop('ftol', 1e-4)}
         for key in options.keys():
             kwargs['options'][key] = options[key]
 
         # Starting negative log likelihood to test against.
 
         fit_vrad = len(p0) == 5
-        nlnL = self._nlnL(p0, resample=resample)
+        nlnL = self._nlnL(p0=p0,
+                          vlsr_mask=vlsr_mask,
+                          dv_mask=dv_mask,
+                          resample=resample)
 
         # Cycle through the required number of iterations.
 
         for _ in range(int(N)):
 
             # Define the bounds.
             bounds = [(0.8 * p0[0], 1.2 * p0[0])]
             if fit_vrad:
                 bounds.append((-0.3 * p0[0], 0.3 * p0[0]))
             bounds += [(0.0, None), (-15.0, 10.0), (0.0, 10.0)]
 
             # Optimize hyper-parameters, holding vrot and vrad constant.
 
             res = minimize(self._nlnL_hyper, x0=p0[-3:],
-                           args=(p0[0], p0[1] if fit_vrad else 0., resample),
+                           args=(p0[0],
+                                 p0[1] if fit_vrad else 0.,
+                                 vlsr_mask,
+                                 dv_mask,
+                                 resample),
                            bounds=bounds[-3:], **kwargs)
             if res.success:
                 p0_temp = p0
                 p0_temp[-3:] = res.x
-                nlnL_temp = self._nlnL(p0_temp, resample)
+                nlnL_temp = self._nlnL(p0_temp, vlsr_mask, dv_mask, resample)
                 if nlnL_temp < nlnL:
                     p0 = p0_temp
                     nlnL = nlnL_temp
             else:
                 if verbose:
                     print('Failed hyper-params mimization: %s' % res.message)
 
             # Optimize vrot holding the hyper-parameters and vrad constant.
 
             res = minimize(self._nlnL_vrot, x0=p0[0],
-                           args=(p0[-3:], p0[1] if fit_vrad else 0., resample),
+                           args=(p0[-3:],
+                                 p0[1] if fit_vrad else 0.,
+                                 vlsr_mask,
+                                 dv_mask,
+                                 resample),
                            bounds=[bounds[0]], **kwargs)
             if res.success:
                 p0_temp = p0
                 p0_temp[0] = res.x
-                nlnL_temp = self._nlnL(p0_temp, resample)
+                nlnL_temp = self._nlnL(p0_temp,
+                                       vlsr_mask,
+                                       dv_mask,
+                                       resample)
                 if nlnL_temp < nlnL:
                     p0 = p0_temp
                     nlnL = nlnL_temp
                 else:
                     if verbose:
                         print('Failed vrot mimization: %s' % res.message)
 
             # Optimize vrad holding the hyper-parameters and vrot constant.
 
             if fit_vrad:
                 res = minimize(self._nlnL_vrad, x0=p0[1],
-                               args=(p0[0], p0[-3:], resample),
+                               args=(p0[0],
+                                     p0[-3:],
+                                     vlsr_mask,
+                                     dv_mask,
+                                     resample),
                                bounds=[bounds[1]], **kwargs)
                 if res.success:
                     p0_temp = p0
                     p0_temp[1] = res.x
-                    nlnL_temp = self._nlnL(p0_temp, resample)
+                    nlnL_temp = self._nlnL(p0_temp,
+                                           vlsr_mask,
+                                           dv_mask,
+                                           resample)
                     if nlnL_temp < nlnL:
                         p0 = p0_temp
                         nlnL = nlnL_temp
                     else:
                         if verbose:
                             print('Failed vrad mimization: %s' % res.message)
 
             # Final minimization with everything.
 
-            res = minimize(self._nlnL, x0=p0, args=(resample),
-                           bounds=bounds, **kwargs)
+            res = minimize(self._nlnL,
+                           x0=p0,
+                           args=(vlsr_mask, dv_mask, resample),
+                           bounds=bounds,
+                           **kwargs)
+
             if res.success:
                 p0_temp = res.x
-                nlnL_temp = self._nlnL(p0_temp, resample)
+                nlnL_temp = self._nlnL(p0_temp, vlsr_mask, dv_mask, resample)
                 if nlnL_temp < nlnL:
                     p0 = p0_temp
                     nlnL = nlnL_temp
             else:
                 if verbose:
                     print('Failed total mimization: %s' % res.message)
 
@@ -480,35 +590,50 @@
     @staticmethod
     def _randomize_p0(p0, nwalkers, scatter):
         """Estimate (vrot, noise, lnp, lns) for the spectrum."""
         dp0 = np.random.randn(nwalkers * len(p0)).reshape(nwalkers, len(p0))
         dp0 = np.where(p0 == 0.0, 1.0, p0)[None, :] * (1.0 + scatter * dp0)
         return np.where(p0[None, :] == 0.0, dp0 - 1.0, dp0)
 
-    def _nlnL_vrot(self, vrot, hyperparams, vrad, resample=False):
+    def _nlnL_vrot(self, vrot, hyperparams, vrad, vlsr_mask=None, dv_mask=None,
+                   resample=False):
         """Negative lnlikelihood function with vrot as only argument."""
         theta = np.insert(hyperparams, 0, [vrot, vrad])
-        nll = -self._lnlikelihood(theta, resample=resample)
+        nll = -self._lnlikelihood(theta=theta,
+                                  vlsr_mask=vlsr_mask,
+                                  dv_mask=dv_mask,
+                                  resample=resample)
         return nll if np.isfinite(nll) else 1e15
 
-    def _nlnL_hyper(self, hyperparams, vrot, vrad, resample=False):
+    def _nlnL_hyper(self, hyperparams, vrot, vrad, vlsr_mask=None, dv_mask=None,
+                    resample=False):
         """Negative lnlikelihood function with hyperparams as only argument."""
         theta = np.insert(hyperparams, 0, [vrot, vrad])
-        nll = -self._lnlikelihood(theta, resample=resample)
+        nll = -self._lnlikelihood(theta=theta,
+                                  vlsr_mask=vlsr_mask,
+                                  dv_mask=dv_mask,
+                                  resample=resample)
         return nll if np.isfinite(nll) else 1e15
 
-    def _nlnL_vrad(self, vrad, vrot, hyperparams, resample=False):
+    def _nlnL_vrad(self, vrad, vrot, hyperparams, vlsr_mask=None, dv_mask=None,
+                   resample=False):
         """Negative lnlikelihood function with vrad as only argument."""
         theta = np.insert(hyperparams, 0, [vrot, vrad])
-        nll = -self._lnlikelihood(theta, resample=resample)
+        nll = -self._lnlikelihood(theta=theta,
+                                  vlsr_mask=vlsr_mask,
+                                  dv_mask=dv_mask,
+                                  resample=resample)
         return nll if np.isfinite(nll) else 1e15
 
-    def _nlnL(self, theta, resample=False):
+    def _nlnL(self, theta, vlsr_mask=None, dv_mask=None, resample=False):
         """Negative log-likelihood function for optimization."""
-        nll = -self._lnlikelihood(theta, resample=resample)
+        nll = -self._lnlikelihood(theta=theta,
+                                  vlsr_mask=vlsr_mask,
+                                  dv_mask=dv_mask,
+                                  resample=resample)
         return nll if np.isfinite(nll) else 1e15
 
     @staticmethod
     def _build_kernel(x, y, hyperparams):
         """Build the GP kernel. Returns None if gp.compute(x) fails."""
         noise, lnsigma, lnrho = hyperparams
         k_noise = celerite.terms.JitterTerm(log_sigma=np.log(noise))
@@ -538,61 +663,71 @@
             return -np.inf
         if not -15.0 < lnsigma < 10.:
             return -np.inf
         if not 0.0 <= lnrho <= 10.:
             return -np.inf
         return 0.0
 
-    def _lnlikelihood(self, theta, resample=False):
+    def _lnlikelihood(self, theta, vlsr_mask=None, dv_mask=None,
+                      resample=False):
         """Log-likelihood function for the MCMC."""
 
         # Unpack the free parameters.
 
         try:
             vrot, vrad = theta[:-3]
         except ValueError:
             vrot, vrad = theta[0], 0.0
         hyperparams = theta[-3:]
 
         # Deproject the data and resample if requested.
 
-        x, y = self.deprojected_spectrum(vrot=vrot, vrad=vrad,
+        x, y = self.deprojected_spectrum(vrot=vrot,
+                                         vrad=vrad,
                                          resample=resample,
-                                         scatter=False)
+                                         scatter=False,
+                                         vlsr_mask=vlsr_mask,
+                                         dv_mask=dv_mask)
         x, y = self._get_masked_spectrum(x, y)
 
         # Build the GP model and calculate the log-likelihood.
 
         gp = annulus._build_kernel(x, y, hyperparams)
         if gp is None:
             return -np.inf
         ll = gp.log_likelihood(y, quiet=True)
         return ll if np.isfinite(ll) else -np.inf
 
-    def _lnprobability(self, theta, vref, resample=False):
+    def _lnprobability(self, theta, vref, vlsr_mask=None, dv_mask=None,
+                       resample=False):
         """Log-probability function for the MCMC."""
         if ~np.isfinite(annulus._lnprior(theta, vref)):
             return -np.inf
-        return self._lnlikelihood(theta, resample)
+        return self._lnlikelihood(theta=theta,
+                                  vlsr_mask=vlsr_mask,
+                                  dv_mask=dv_mask,
+                                  resample=resample)
 
     # -- Minimizing Line Width Approach -- #
 
     def get_vlos_dV(self, p0=None, fit_vrad=False, resample=False,
-                    optimize_kwargs=None):
+                    vlsr_mask=None, dv_mask=None, optimize_kwargs=None):
         """
         Infer the rotational (and optically radial) velocity by minimizing the
         width of the shifted-and-stacked azimuthally averaged spectrum.
 
         Args:
             p0 (optional[list]): Starting positions for the optimization.
             fit_vrad (optional[bool]): Whether to include the radial velocity
                 in the fit. Default is ``False``.
             resample (optional[bool]): Resample the shifted spectra by this
                 factor. For example, resample = 2 will shift and bin the
                 spectrum down to sampling rate twice that of the original data.
+            vlsr_mask (optional[float]):
+            dv_mask (optional[float]):
             optimize_kwargs (optional[dict]): Kwargs to pass to ``minimize``.
 
         Returns:
             Velocities which minimize the line width of the shifted and stacked
             spectrum.
         """
 
@@ -614,68 +749,83 @@
         options['ftol'] = options.pop('ftol', 1e-4)
         optimize_kwargs['options'] = options
 
         # Run the minimization.
 
         res = minimize(self.deprojected_width,
                        x0=p0,
-                       args=(fit_vrad, resample),
+                       args=(fit_vrad, resample, vlsr_mask, dv_mask),
                        **optimize_kwargs)
         if not res.success:
             print("WARNING: minimize did not converge.")
         return res.x if res.success else np.nan
 
-    def deprojected_width(self, theta, fit_vrad=False, resample=True):
+    def deprojected_width(self, theta, fit_vrad=False, resample=True,
+                          vlsr_mask=None, dv_mask=None):
         """
         Return the Gaussian width of the deprojected and stacked spectra.
 
         Args:
             theta (list): Deprojection velocities, ``(vrot[, vrad])``.
             fit_vrad (optional[bool]): Whether ``vrad`` in is ``theta``.
             resample (optional): How to resample the data.  See
                 :func:`deprojected_spectrum` for more details.
+            vlsr_mask (optional[float]):
+            dv_mask (optional[float]):
 
         Returns:
             The Doppler width of the average stacked spectrum using the
             velocities to align the individual spectra.
         """
         from .helper_functions import get_gaussian_width
         vrot, vrad = theta if fit_vrad else (theta, 0.0)
         x, y = self.deprojected_spectrum(vrot=vrot,
                                          vrad=vrad,
                                          resample=resample,
-                                         scatter=False)
+                                         scatter=False,
+                                         vlsr_mask=vlsr_mask,
+                                         dv_mask=dv_mask)
         return get_gaussian_width(*self._get_masked_spectrum(x, y))
 
     # -- Rotation Velocity by Fitting a SHO -- #
 
     def get_vlos_SHO(self, p0=None, fit_vrad=False, fix_vlsr=None,
-                     centroid_method='quadratic', optimize_kwargs=None):
+                     vrot_mask=None, vlsr_mask=None, vrad_mask=None,
+                     dv_mask=None, centroid_method='quadratic',
+                     optimize_kwargs=None):
         """
         Infer the disk-frame rotational (and, optionally, radial) velocity by
         finding velocity which best describes the azimuthal dependence of the
         line centroid modelled as a simple harmonic oscillator.
 
         Args:
             p0 (optional[list]): Starting positions for the optimization.
             fit_vrad (optional[bool]): Whether to include the radial velocity
                 in the fit. Default is ``False``.
             fix_vlsr (optional[float]): If provided, use this value to deproject
                 the vertical velocity component.
+            vrot_mask
+            vlsr_mask
+            vrad_mask
+            dv_mask
             centroid_method (optional[str]): Method used to determine the line
-                centroids, and must be one of ``'quadratic'``, ``'max'`` or
-                ``'gaussian'``.
+                centroids, and must be one of ``'quadratic'``, ``'max'``,
+                ``'gaussian'``, ``'doublegauss'`` or ``'doublegauss_fixeddv'``.
             optimize_kwargs (optional[dict]): Kwargs to pass to ``curve_fit``.
 
         Returns:
             pop, cvar (array, array): Arrays of the best-fit parameter values
             and their uncertainties returned from ``curve_fit``.
         """
         from .helper_functions import SHO, SHO_double
-        v0, dv0 = self.line_centroids(method=centroid_method)
+        v0, dv0 = self.line_centroids(method=centroid_method,
+                                      vrot_mask=vrot_mask,
+                                      vlsr_mask=vlsr_mask,
+                                      vrad_mask=vrad_mask,
+                                      dv_mask=dv_mask)
         assert v0.size == self.theta.size
 
         # Starting positions. Here we're using projected velocities such that
         # A = vrot * sin(|i|), B = -vrad * sin(i) and C = vlsr - vz * cos(i).
 
         if p0 is None:
             A, B, C = 0.5 * (v0.max() - v0.min()), 0.0, v0.mean()
@@ -716,15 +866,16 @@
         # Return the optimized values.
 
         return popt, cvar
 
     # -- Rotation Velocity by Maximizing SNR -- #
 
     def get_vlos_SNR(self, p0=None, fit_vrad=False, resample=False,
-                     signal='int', optimize_kwargs=None):
+                     signal='int', vlsr_mask=None, dv_mask=None,
+                     optimize_kwargs=None):
         """
         Infer the rotation (and, optically, the radial) velocity by finding the
         rotation velocity (and radial velocities) which, after shifting all
         spectra to a common velocity, results in the maximum signal-to=noise
         ratio of the stacked profile. This is an implementation of the method
         described in Yen et al. (2016, 2018).
 
@@ -733,14 +884,16 @@
             fit_vrad (optional[bool]): Whether to include the radial velocity
                 in the fit. Default is ``False``.
             resample (optional[bool]): Resample the shifted spectra by this
                 factor. For example, resample = 2 will shift and bin the
                 spectrum down to sampling rate twice that of the original data.
             signal (Optional[str]): Method used to calculate the signal, either
                 'max' for the line peak or 'int' for the integrated intensity.
+            vlsr_mask (Optional[float]):
+            dv_mask (Optional[float]):
             optimize_kwargs (optional[dict]): Kwargs to pass to ``minimize``.
 
         Returns:
             Velocities which maximizese signal to noise of the shifted and
             stacked spectrum.
 
         .. _Yen et al. (2016): https://ui.adsabs.harvard.edu/abs/2016ApJ...832..204Y/abstract
@@ -771,22 +924,22 @@
         options['ftol'] = options.pop('ftol', 1e-4)
         optimize_kwargs['options'] = options
 
         # Run the minimization.
 
         res = minimize(self.deprojected_nSNR,
                        x0=p0,
-                       args=(fit_vrad, resample, signal),
+                       args=(fit_vrad, resample, signal, vlsr_mask, dv_mask),
                        **optimize_kwargs)
         if not res.success:
             print("WARNING: minimize did not converge.")
         return res.x if res.success else np.nan
 
     def deprojected_nSNR(self, theta, fit_vrad=False, resample=False,
-                         signal='int'):
+                         signal='int', vlsr_mask=None, dv_mask=None):
         """
         Return the negative SNR of the deprojected spectrum. There are three
         ways to calculate the signal of the data. ``signal='max'`` will use the
         Gaussian peak relative to the noise, ``signal='int'`` will use the
         integrated spectrum as the signal, while ``signal='weighted'`` will
         additionally use a Gaussian shape weighting so that noise in the line
         wings are minimized, as in `Yen et al. (2016)`_.
@@ -800,24 +953,29 @@
 
         Args:
             theta (list): Disk-frame velocities, ``(vrot[, vrad])``.
             fit_vrad (optional[bool]): Whether ``vrad`` in is ``theta``.
             resample (optional): How to resample the data. See
                 :func:`deprojected_spectrum` for more details.
             signal (optional[str]): Definition of SNR to use.
+            vlsr_mask (optional[float]):
+            dv_mask (optional[float]):
 
         Returns:
             Negative of the signal-to-noise ratio.
         """
         from .helper_functions import gaussian, fit_gaussian
         vrot, vrad = theta if fit_vrad else (theta, 0.0)
         x, y = self.deprojected_spectrum(vrot=vrot,
                                          vrad=vrad,
                                          resample=resample,
-                                         scatter=False)
+                                         scatter=False,
+                                         vlsr_mask=vlsr_mask,
+                                         dv_mask=dv_mask)
+
         x0, dx, A = fit_gaussian(x, y)
         noise = np.std(x[(x - x0) / dx > 3.0])  # Check: noise will vary.
         if signal == 'max':
             SNR = A / noise
         else:
             if signal == 'weighted':
                 w = gaussian(x, x0, dx, (np.sqrt(np.pi) * dx)**-1)
@@ -839,34 +997,35 @@
                 std = std_new
         else:
             std = np.nanstd([self.spectra[:, :N], self.spectra[:, -N:]])
         return std
 
     # -- Deprojection Functions -- #
 
-    def calc_vlos(self, vrot, vrad=0.0):
+    def calc_vlos(self, vrot, vrad=0.0, vlsr=0.0):
         """
         Calculate the line of sight velocity for each spectrum given the
         rotational and radial velocities at the attached polar angles.
 
         Note that the rotational and radial velocities are specified in the disk
         frame and do not take into account the projection along the line of
         sight. Remember that a positive radial velocity is moving away from the
         star.
 
         Args:
             vrot (float): Disk-frame rotation velocity in [m/s].
             vrad (optional[float]): Disk-frame radial velocity in [m/s].
+            vlsr (optional[float]): Systemtic velocity in [m/s].
 
         Returns
             Array of projected line of sight velocities at each polar angle.
         """
         vrot_proj = vrot * np.cos(self.theta) * np.sin(abs(self.inc_rad))
         vrad_proj = -vrad * np.sin(self.theta) * np.sin(self.inc_rad)
-        return vrot_proj + vrad_proj
+        return vrot_proj + vrad_proj + vlsr
 
     def deprojected_spectra(self, vrot, vrad=0.0, kind='linear', weights=None):
         """
         Returns all deprojected points as an ensemble.
 
         Args:
             vrot (float): Disk-frame rotation velocity in [m/s].
@@ -921,15 +1080,16 @@
         Returns:
             The polar angle grid, the velocity grid and the river.
         """
         river = self.deprojected_spectra(vrot, vrad, kind, weights)
         river = self._grid_river(river, method)
         return self.theta_grid, self.velax_grid, river
 
-    def deprojected_spectrum(self, vrot, vrad=0.0, resample=True, scatter=True):
+    def deprojected_spectrum(self, vrot, vrad=0.0, resample=True, scatter=True,
+                             vlsr_mask=None, dv_mask=None):
         """
         Returns ``(x, y[, dy])`` of the collapsed and deprojected spectrum
         using the provided velocities to deproject the data.
         
         Note that the rotational and radial velocities are specified in the disk
         frame and do not take into account the projection along the line of
         sight. Remember that a positive radial velocity is moving away from the
@@ -955,78 +1115,144 @@
 
         Args:
             vrot (float): Disk-frame rotational velocity in [m/s].
             vrad (optional[float]): Disk-frame radial velocity in [m/s].
             resample (optional): Type of resampling to be applied.
             scatter (optional[bool]): If the spectrum is resampled, whether to
                 return the scatter in each velocity bin.
+            vlsr_mask (optional[float]):
+            dv_mask (optional[float]):
 
         Returns:
             A deprojected spectrum, resampled using the provided method.
         """
         vlos = self.calc_vlos(vrot=vrot, vrad=vrad)
         vpnts = self.velax[None, :] - vlos[:, None]
         vpnts, spnts = self._order_spectra(vpnts=vpnts.flatten())
-        return self._resample_spectra(vpnts, spnts, resample=resample,
-                                      scatter=scatter)
+        x, y, dy = self._resample_spectra(vpnts=vpnts,
+                                          spnts=spnts,
+                                          resample=resample,
+                                          scatter=True)
+        if vlsr_mask is not None:
+            if dv_mask is None:
+                dv_mask = 2.0 * self.chan
+            mask = abs(x - vlsr_mask) <= dv_mask
+        else:
+            mask = np.isfinite(y)
+        if scatter:
+            return x[mask], y[mask], dy[mask]
+        return x[mask], y[mask]
 
-    def line_centroids(self, method='quadratic'):
+    def get_masked_spectra(self, vrot_mask, vlsr_mask, vrad_mask=None, dv_mask=None):
+        """
+        Returns spectra masked only around the line peaks based on the provided
+        velocity profile.
+
+        Args:
+            vrot_mask (float): TBD
+            vlsr_mask (float): TBD
+            vrad_mask (float): TBD
+            dv_mask (float): TBD
+
+        Returns:
+            velax, spectra (array, array): TBD
+        """
+        if vrot_mask is None:
+            return [self.velax for _ in self.spectra], self.spectra
+        if vlsr_mask is None:
+            raise ValueError("Must specify 'vlsr' explicity.")
+        if vrad_mask is None:
+            vrad_mask = 0.0
+        if dv_mask is None:
+            dv_mask = 2.0 * self.chan
+        if dv_mask < self.chan:
+            raise ValueError("`dv` must be at least twice the channel spacing.")
+        mask = self.calc_vlos(vrot=vrot_mask,
+                              vrad=vrad_mask,
+                              vlsr=vlsr_mask)
+        mask = abs(mask[:, None] - self.velax[None, :]) <= dv_mask
+        velax = [self.velax[m] for m in mask]
+        spectra = [s[m] for s, m in zip(self.spectra, mask)]
+        return velax, spectra
+
+    def line_centroids(self, method='quadratic', vrot_mask=None, vlsr_mask=None,
+                       vrad_mask=None, dv_mask=None):
         """
         Returns the line centroid for each of the spectra in the annulus.
         Various methods of determining the centroid are possible accessible
         through the ``method`` argument.
 
         Args:
             method (str): Method used to determine the line centroid. Must be
-                in ['max', 'quadratic', 'gaussian', 'gaussthick']. The former
-                returns the pixel of maximum value, 'quadratic' fits a
-                quadratic function to the pixel of maximum value and its two
-                neighbouring pixels (see Teague & Foreman-Mackey 2018 for
-                details) and 'gaussian' and 'gaussthick' fits an analytical
-                Gaussian profile to the line.
+                in ['max', 'quadratic', 'gaussian', 'gaussthick', 'doublegauss', 
+                'doublegauss_fixeddv]. The former returns the pixel of maximum
+                value, 'quadratic' fits a quadratic function to the pixel of
+                maximum value and its two neighbouring pixels (see Teague &
+                Foreman-Mackey 2018 for details) and 'gaussian', 'gaussthick'
+                'doublegauss' and 'doublegauss_fixeddv' fit (an) analytical
+                Gaussian profile(s) to the line.
+            vrot_mask (Optional[float]): TBD
+            vrad_mask (Optional[float]): TBD
+            vlsr_mask (Optional[float]): TBD
+            dv_mask (Optional[float]): TBD
 
         Returns:
             vmax, dvmax (array, array): Line centroids and associated
                 uncertainties.
         """
+
+        # Get the spectra to fit, using the mask if appropriate.
+
+        velax, spectra = self.get_masked_spectra(vrot_mask=vrot_mask,
+                                                 vlsr_mask=vlsr_mask,
+                                                 vrad_mask=vrad_mask,
+                                                 dv_mask=dv_mask)
+
+        # Cycle through the methods and apply.
+
         method = method.lower()
+       
         if method == 'max':
-            vmax = np.take(self.velax, np.argmax(self.spectra, axis=1))
+            vmax = np.array([v[np.argmax(s)] for v, s in zip(velax, spectra)])
             dvmax = np.ones(vmax.size) * self.chan
+       
         elif method == 'quadratic':
-            try:
-                from bettermoments.quadratic import quadratic
-            except ImportError:
-                raise ImportError("Please install 'bettermoments'.")
+            from bettermoments.quadratic import quadratic
             vmax = [quadratic(s, uncertainty=self.rms,
-                              x0=self.velax[0], dx=self.chan)
-                    for s in self.spectra]
+                              x0=v[0], dx=self.chan)
+                    for v, s in zip(velax, spectra)]
             vmax, dvmax = np.array(vmax).T[:2]
+       
         elif method == 'gaussian':
             from .helper_functions import get_gaussian_center
-            vmax = [get_gaussian_center(self.velax, s, self.rms)
-                    for s in self.spectra]
+            vmax = [get_gaussian_center(v, s, self.rms)
+                    for v, s in zip(velax, spectra)]
             vmax, dvmax = np.array(vmax).T
+       
         elif method == 'gaussthick':
             from .helper_functions import get_gaussthick_center
-            vmax = [get_gaussthick_center(self.velax, s, self.rms)
-                    for s in self.spectra]
+            vmax = [get_gaussthick_center(v, s, self.rms)
+                    for v, s in zip(velax, spectra)]
             vmax, dvmax = np.array(vmax).T
+        
         elif method == 'doublegauss':
             from .helper_functions import get_doublegauss_center
-            vmax = [get_doublegauss_center(self.velax, s, self.rms)
-                    for s in self.spectra]
+            vmax = [get_doublegauss_center(v, s, self.rms)
+                    for v, s in zip(velax, spectra)]
             vmax, dvmax = np.array(vmax).T
+        
         elif method == 'doublegauss_fixeddv':
             from .helper_functions import get_doublegauss_fixeddV_center
-            vmax = [get_doublegauss_fixeddV_center(self.velax, s, self.rms)
-                    for s in self.spectra]
+            vmax = [get_doublegauss_fixeddV_center(v, s, self.rms)
+                    for v, s in zip(velax, spectra)]
             vmax, dvmax = np.array(vmax).T
+        
         else:
             raise ValueError(f"Unknown method, {method}.")
+        
         return vmax, dvmax
 
     def _order_spectra(self, vpnts, spnts=None):
         """Return velocity order spectra."""
         spnts = self.spectra_flat if spnts is None else spnts
         if len(spnts) != len(vpnts):
             raise ValueError("Wrong size in 'vpnts' and 'spnts'.")
@@ -1162,17 +1388,20 @@
                          method=method)
         sgrid = np.where(self.theta_grid[:, None] > tpnts.max(), np.nan, sgrid)
         sgrid = np.where(self.theta_grid[:, None] < tpnts.min(), np.nan, sgrid)
         return sgrid
 
     # -- Plotting Functions -- #
 
-    def plot_spectra(self, ax=None, return_fig=False, step_kwargs=None):
+    def plot_spectra(self, ax=None, return_fig=False, step_kwargs=None,
+                     vrot_mask=None, vlsr_mask=None, vrad_mask=0.0,
+                     dv_mask=200.0):
         """
-        Plot the attached spectra on the same velocity axis.
+        Plot the attached spectra on the same velocity axis. You can include the
+        velocity mask to see how that affects the spectra.
 
         Args:
             ax (Optional): Matplotlib axis onto which the data will be plotted.
             return_fig (Optional[bool]): Return the figure.
             step_kwargs (Optional[dict])
 
         Returns
@@ -1182,16 +1411,21 @@
             fig, ax = plt.subplots(figsize=(5.0, 3.1), constrained_layout=True)
         else:
             return_fig = False
         step_kwargs = {} if step_kwargs is None else step_kwargs
         step_kwargs['where'] = step_kwargs.pop('where', 'mid')
         step_kwargs['lw'] = step_kwargs.pop('lw', 1.0)
         step_kwargs['c'] = step_kwargs.pop('c', 'k')
-        for spectrum in self.spectra:
-            ax.step(self.velax, spectrum, **step_kwargs)
+
+        velax, spectra = self.get_masked_spectra(vrot_mask=vrot_mask,
+                                                 vlsr_mask=vlsr_mask,
+                                                 vrad_mask=vrad_mask,
+                                                 dv_mask=dv_mask)
+        for v, s in zip(velax, spectra):
+            ax.step(v, s, **step_kwargs)
         ax.set_xlabel('Velocity (m/s)')
         ax.set_ylabel('Intensity (Jy/beam)')
         ax.set_xlim(self.velax[0], self.velax[-1])
         if return_fig:
             return fig
 
     def plot_spectrum(self, vrot=0.0, vrad=0.0, resample=True, plot_fit=False,
@@ -1287,32 +1521,32 @@
                         transform=ax.transAxes)
 
         # Return fig.
         if return_fig:
             return fig
 
     def plot_river(self, vrot=None, vrad=0.0, residual=False, method='nearest',
-                   plot_kwargs=None, profile_kwargs=None, return_fig=False):
+                   vrot_mask=None, vlsr_mask=None, vrad_mask=None, dv_mask=None,
+                   plot_kwargs=None, return_fig=False):
         """
         Make a river plot, showing how the spectra change around the azimuth.
         This is a nice way to search for structure within the data.
 
         Args:
             vrot (Optional[float]): Rotational velocity used to deprojected the
                 spectra. If none is provided, no deprojection is used.
             vrad (Optional[float]): Radial velocity used to deproject the
                 spectra.
             residual (Optional[bool]): If true, subtract the azimuthally
                 averaged line profile.
-            resample (Optional[int/float]): Resample the velocity axis by this
-                factor if a ``int``, else set the channel spacing to this value
-                if a ``float``. Note that this is not the same resampling
-                method as used for the spectra and should only be used for
-                qualitative analysis.
             method (Optional[str]): Interpolation method for ``griddata``.
+            vrot_mask (Optional[float]):
+            vlsr_mask (Optional[float]):
+            vrad_mask (Optional[float]):
+            dv_mask (Optional[float]):
             xlims (Optional[list]): Minimum and maximum x-range for the figure.
             ylims (Optional[list]): Minimum and maximum y-range for the figure.
             tgrid (Optional[ndarray]): Theta grid in [rad] used for gridding
                 the data. By default this spans ``-pi`` to ``pi``.
             return_fig (Optional[bool]): Whether to return the figure axes.
 
         Returns:
@@ -1324,14 +1558,15 @@
         from matplotlib.ticker import MultipleLocator
         from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
 
         # Deproject and grid the spectra.
 
         if vrot is None:
             spectra = self.spectra
+            vrot = 0.0
         else:
             spectra = self.deprojected_spectra(vrot=vrot, vrad=vrad)
         spectra = self._grid_river(spectra, method=method)
 
         # Get the residual if necessary.
 
         mean_spectrum = np.nanmean(spectra, axis=0)
@@ -1356,22 +1591,55 @@
         kw['vmin'] = kw.pop('vmin', -kw['vmax'] if residual else -rms)
         kw['cmap'] = kw.pop('cmap', 'RdBu_r' if residual else 'turbo')
 
         # Plot the data.
 
         fig, ax = plt.subplots(figsize=(6.0, 2.25), constrained_layout=True)
         ax_divider = make_axes_locatable(ax)
-        im = ax.pcolormesh(self.velax_grid, np.degrees(self.theta_grid),
+        im = ax.pcolormesh(self.velax_grid,
+                           np.degrees(self.theta_grid),
                            spectra, **kw)
         ax.set_ylim(-180, 180)
         ax.yaxis.set_major_locator(MultipleLocator(60.0))
         ax.set_xlim(xlim)
         ax.set_xlabel('Velocity (m/s)')
         ax.set_ylabel(r'$\phi$' + ' (deg)')
 
+        # Include the proposed mask.
+
+        if vrot_mask is not None:
+            if vlsr_mask is None:
+                raise ValueError("Must specify `vlsr_mask`.")
+            if vrad_mask is None:
+                vrad_mask = 0.0
+            if dv_mask is None:
+                dv_mask = 2.0 * self.chan
+
+            # Note here that we allow for the mask to be deprojected in case
+            # the the shifting isn't the same as the mask...
+
+            mask = (vrot_mask - vrot) * np.cos(self.theta_grid) * abs(self.sini)
+            mask += (vrad - vrad_mask) * np.sin(self.theta_grid) * self.sini
+            mask += vlsr_mask
+
+            ax.fill_betweenx(np.degrees(self.theta_grid),
+                             self.velax_grid[0] - np.diff(self.velax_grid)[0],
+                             mask - dv_mask,
+                             color='k' if residual else 'w', lw=0.0,
+                             alpha=0.3 if residual else 0.7)
+            ax.fill_betweenx(np.degrees(self.theta_grid),
+                             mask + dv_mask,
+                             self.velax_grid[-1] + np.diff(self.velax_grid)[0],
+                             color='k' if residual else 'w', lw=0.0,
+                             alpha=0.3 if residual else 0.7)
+            ax.plot(mask - dv_mask, np.degrees(self.theta_grid),
+                    color='k' if residual else 'w')
+            ax.plot(mask + dv_mask, np.degrees(self.theta_grid),
+                    color='k' if residual else 'w')
+
         # Add the mean spectrum panel.
 
         if not residual:
             fig.set_size_inches(6.0, 2.5, forward=True)
             ax1 = ax_divider.append_axes('top', size='25%', pad='2%')
             ax1.step(self.velax_grid, mean_spectrum,
                      where='mid', lw=1., c='k')
@@ -1394,28 +1662,33 @@
         else:
             cb.set_label('Intensity (Jy/beam)', rotation=270, labelpad=13)
 
         if return_fig:
             return fig
 
     def plot_centroids(self, centroid_method='quadratic', plot_fit=None,
-                       fit_vrad=False, fix_vlsr=None, ax=None, return_fig=False,
-                       plot_kwargs=None):
+                       fit_vrad=False, fix_vlsr=None, vrot_mask=None,
+                       vlsr_mask=None, vrad_mask=None, dv_mask=None, ax=None,
+                       return_fig=False, plot_kwargs=None):
         """
         Plot the measured line centroids as a function of polar angle.
 
         Args:
             centroid_method (Optional[str]): Method used to determine the line
                 centroid. Default is `'quadratic'`.
             plot_fit (Optional[bool]): Whether to overplot a SHO fit to the
                 data.
             fit_vrad (Optional[bool]): Whether to include a radial velocity
                 component to the fit.
             fix_vlsr (Optional[bool]): Fix the systemic velocity to calculate
                 the deprojected vertical velocities.
+            vrot_mask (Optional[float]):
+            vlsr_mask (Optional[float]):
+            vrad_mask (Optional[float]):
+            dv_mask (Optional[float]):
             ax (Optional[matploib axis]): Axis to plot the data (and fit) onto,
                 otherwise a new figure will be created.
             return_fig (Optional[bool]): Whether to return the figure for
                 subsequent plotting.
             plot_kwargs (Optional[dict]):
 
         Returns:
@@ -1425,17 +1698,21 @@
 
         from .helper_functions import SHO_double
         if ax is None:
             fig, ax = plt.subplots()
         else:
             return_fig = False
 
-        # Calculate the line centroids.
+        # Calculate the line centroids, including any masking necessary.
 
-        v0, dv0 = self.line_centroids(method=centroid_method)
+        v0, dv0 = self.line_centroids(method=centroid_method,
+                                      vrot_mask=vrot_mask,
+                                      vlsr_mask=vlsr_mask,
+                                      vrad_mask=vrad_mask,
+                                      dv_mask=dv_mask)
         dv0 = abs(dv0)
 
         # Set the defaults for plotting.
 
         plot_kwargs = {} if plot_kwargs is None else plot_kwargs
         plot_kwargs['fmt'] = plot_kwargs.pop('fmt', 'o')
         plot_kwargs['c'] = plot_kwargs.pop('c', 'k')
@@ -1455,14 +1732,17 @@
 
         if plot_fit:
 
             # Fit the data.
 
             popt, cvar = self.get_vlos_SHO(fit_vrad=fit_vrad,
                                            fix_vlsr=fix_vlsr,
+                                           vrot_mask=vrot_mask,
+                                           vlsr_mask=vlsr_mask,
+                                           vrad_mask=vrad_mask,
                                            centroid_method=centroid_method)
 
             v_p, dv_p = popt[0] * abs(self.sini), cvar[0] * abs(self.sini)
             if fit_vrad:
                 v_r, dv_r = popt[1] * self.sini, cvar[1] * abs(self.sini)
             else:
                 v_r, dv_r = 0.0, 0.0
```

### Comparing `astro-eddy-2.3.7/eddy/datacube.py` & `astro-eddy-2.3.9/eddy/datacube.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,14 +49,18 @@
         # Clip down the cube spatially and spectrally.
 
         if FOV is not None:
             self._clip_cube_spatial(FOV / 2.0, initial_load=True)
         if velocity_range is not None:
             self._clip_cube_velocity(*velocity_range)
 
+    @property
+    def rms(self):
+        return self.estimate_cube_RMS()
+
     # -- PIXEL DEPROJECTION -- #
 
     def disk_coords(self, x0=0.0, y0=0.0, inc=0.0, PA=0.0, z0=None, psi=None,
                     r_cavity=0.0, r_taper=None, q_taper=1.0, z_func=None,
                     shadowed=False, outframe='cylindrical', flatten=False, **_):
         r"""
         Get the disk coordinates given certain geometrical parameters and an
@@ -528,15 +532,15 @@
         return grid, gridded
 
     def polar_deprojection(self, data, x0=0.0, y0=0.0, inc=0.0, PA=0.0,
                            z0=None, psi=None, r_taper=None, q_taper=1.0,
                            r_cavity=0.0, z_func=None, shadowed=False,
                            rgrid=None, tgrid=None, griddata_kwargs=None):
         """
-        Deproject the data onto 
+        Deproject the provided data onto a polar grid.
 
         Args:
             data (array): Data to be deprojected. Must be the same shape as a
                 channel of the attached data.
             x0 (Optional[float]): Source right ascension offset [arcsec].
             y0 (Optional[float]): Source declination offset [arcsec].
             inc (Optional[float]): Source inclination [degrees]. A positive
@@ -566,39 +570,38 @@
             array, array, array: The radial and azimuthal grids onto which the
                 data is interpolated, and the interpolated data.
         """
 
         # Set the default grids.
 
         if rgrid is None:
-            rgrid = np.linspace(0, self.xaxis.max(), 100)
+            rgrid = np.arange(0, self.xaxis.max(), self.dpix)
         if tgrid is None:
-            tgrid = np.linspace(-180.0, 180.0, 180)
+            tgrid = np.linspace(-np.pi, np.pi, self.xaxis.size)
 
         # Get the pixel coordinates.
 
         r, t, _ = self.disk_coords(x0=x0,
                                    y0=y0,
                                    inc=inc,
                                    PA=PA,
                                    z0=z0,
                                    psi=psi,
                                    r_taper=r_taper,
                                    q_taper=q_taper,
                                    r_cavity=r_cavity,
                                    z_func=z_func,
                                    shadowed=shadowed,
-                                   outframe='cylindrical',
-                                   flatten=True)
+                                   outframe='cylindrical')
         
         # Deproject onto a polar grid.
         
-        gridded = datacube._griddata(points=(np.degrees(t), r),
+        gridded = datacube._griddata(points=(r.flatten(), t.flatten()),
                                      values=data.flatten(),
-                                     xi=(tgrid[:, None], rgrid[None, :]),
+                                     xi=(rgrid[None, :], tgrid[:, None]),
                                      griddata_kwargs=griddata_kwargs)
 
         return rgrid, tgrid, gridded
 
     @staticmethod
     def _griddata(points, values, xi, griddata_kwargs=None):
         """Wrapper for ``scipy.interpolate.griddata``."""
@@ -1126,14 +1129,296 @@
             pvals = pvals[::sampling]
             dvals = dvals[::sampling]
         else:
             print("Pixels appear to be close to spatially independent.")
 
         return rvals, pvals, dvals
     
+    def velocity_to_restframe_frequency(self, velax=None, vlsr=0.0):
+        """Return restframe frequency [Hz] of the given velocity [m/s]."""
+        velax = self.velax if velax is None else np.squeeze(velax)
+        return self.nu0 * (1. - (velax - vlsr) / 2.998e8)
+
+    def restframe_frequency_to_velocity(self, nu, vlsr=0.0):
+        """Return velocity [m/s] of the given restframe frequency [Hz]."""
+        return 2.998e8 * (1. - nu / self.nu0) + vlsr
+    
+    def spectral_resolution(self, dV=None):
+        """Convert velocity resolution in [m/s] to [Hz]."""
+        dV = dV if dV is not None else self.chan
+        nu = self.velocity_to_restframe_frequency(velax=[-dV, 0.0, dV])
+        return np.mean([abs(nu[1] - nu[0]), abs(nu[2] - nu[1])])
+    
+    # -- GENERAL ANALYSIS FUNCTIONS -- #
+
+    def _beam_mask(self, x, y, threshold=0.5, stretch=1.0, response=False):
+        """
+        Returns a 2D Gaussian mask based on the attached beam centered at
+        (x, y) on the sky.
+
+        Args:
+            x (flaot): RA offset of the center of the beam.
+            y (float): Dec offset of the center of the beam.
+            threshold (Optional[float]): Threshold beam power to consider a
+                pixel within the beam. Default is 0.5.
+            stretch (Optional[float]): Stretch the beam by this factor. A
+                `stretch=2` will result in a beam mask that is twice as large
+                as the attached beam.
+            response (Optional[bool]): If ``True``, return the beam response
+                function rather than a boolean mask.
+
+        Returns:
+            beammask (arr): 2D boolean array of pixels covered by the beam if
+            ``response=False``, the default, otherwise a 2D array of the beam
+            response function centered at that location.
+        """
+        xx, yy = np.meshgrid(self.xaxis - x, self.yaxis - y)
+        theta = -np.radians(self.bpa)
+        std_x = 0.5 * stretch * self.bmin / np.sqrt(np.log(2.0))
+        std_y = 0.5 * stretch * self.bmaj / np.sqrt(np.log(2.0))
+        a = np.cos(theta)**2 / std_x**2 + np.sin(theta)**2 / std_y**2
+        b = np.sin(2*theta) / std_x**2 - np.sin(2*theta) / std_y**2
+        c = np.sin(theta)**2 / std_x**2 + np.cos(theta)**2 / std_y**2
+        f = np.exp(-(a*xx**2 + b*xx*yy + c*yy**2))
+        return f if response else f >= threshold
+
+    def radial_sampling(self, rbins=None, rvals=None, dr=None):
+        """
+        Return bins and bin center values. If the desired bin edges are known,
+        will return the bin edges and vice versa. If neither are known will
+        return default binning with the desired spacing.
+
+        Args:
+            rbins (Optional[list]): List of bin edges.
+            rvals (Optional[list]): List of bin centers.
+            dr (Optional[float]): Spacing of bin centers in [arcsec]. Defaults
+                to a quarter of the beam major axis.
+
+        Returns:
+            rbins (list): List of bin edges.
+            rpnts (list): List of bin centres.
+        """
+        if rbins is not None and rvals is not None:
+            raise ValueError("Specify only 'rbins' or 'rvals', not both.")
+        if rvals is not None:
+            try:
+                dr = np.diff(rvals)[0] * 0.5
+            except IndexError:
+                if self.dpix == self.bmaj:
+                    dr = 2.0 * self.dpix
+                else:
+                    dr = self.bmaj / 4.0
+            rbins = np.linspace(rvals[0] - dr, rvals[-1] + dr, len(rvals) + 1)
+        if rbins is not None:
+            rvals = np.average([rbins[1:], rbins[:-1]], axis=0)
+        else:
+            if dr is None:
+                if self.dpix == self.bmaj:
+                    dr = 2.0 * self.dpix
+                else:
+                    dr = self.bmaj / 4.0
+            rbins = np.arange(0, self.xaxis.max(), dr)
+            rvals = np.average([rbins[1:], rbins[:-1]], axis=0)
+        return rbins, rvals
+
+    def radial_profile(self, rbins=None, rvals=None, dr=None, x0=0.0, y0=0.0,
+            inc=0.0, PA=0.0, z0=None, psi=None, r_cavity=0.0, r_taper=None,
+            q_taper=1.0, z_func=None, shadowed=False, data=None,
+            assume_correlated=True, percentiles=False):
+        """
+        Make an azimuthally averaged radial profile from the data.
+
+        Args:
+            rbins (Optional[list]): List of bin edges.
+            rvals (Optional[list]): List of bin centers.
+            dr (Optional[float]): Spacing of bin centers in [arcsec]. Defaults
+                to a quarter of the beam major axis.
+            x0 (Optional[float]): Source right ascension offset [arcsec].
+            y0 (Optional[float]): Source declination offset [arcsec].
+            inc (Optional[float]): Source inclination [degrees]. A positive
+                inclination denotes a disk rotating clockwise on the sky, while
+                a negative inclination represents a counter-clockwise rotation.
+            PA (Optional[float]): Source position angle [degrees]. Measured
+                between north and the red-shifted semi-major axis in an
+                easterly direction.
+            z0 (Optional[float]): Aspect ratio at 1" for the emission surface.
+                To get the far side of the disk, make this number negative.
+            psi (Optional[float]): Flaring angle for the emission surface.
+            r_taper (Optional[float]): Radius for tapered emission surface.
+            q_taper (Optional[float]): Exponent for tapered emission surface.
+            r_cavity (Optional[float]): Outer radius of a cavity. Within this
+                region the emission surface is taken to be zero.
+            z_func (Optional[callable]): A user-defined emission surface
+                function that will return ``z`` in [arcsec] for a given ``r``
+                in [arcsec]. This will override the analytical form.
+            shadowed (Optional[bool]): Whether to use the slower, but more
+                robust method for deprojecting pixel values.
+            data (Optional[array]): Data to calculate a radial profile of. If
+                not provided, will use the attached dataset.
+            assumed_correlated (Optional[bool]): If ``True``, take into account
+                the beam size in calculating the uncertainty on the radial
+                profile.
+            percentiles (Optional[bool]): If ``True``, use the 16th, 50th and
+                84th percentiles to define the profile and uncertainties.
+                Otherwise use the mean and standard deviation.
+
+        Returns:
+            Three 1D arrays with ``x``, ``y`` and ``dy`` for plotting.
+        """
+
+        # Select the data to use. Defaults to attached data if not provided.
+
+        data = self.data if data is None else data
+        assert data.ndim == 2, "Can only provide radial profiles for 2D data."
+
+        # Get the radial sampling.
+
+        rbins, rvals = self.radial_sampling(rbins=rbins,
+                                            rvals=rvals,
+                                            dr=dr)
+
+        # Calculate the deprojected pixel values.
+
+        rpnts, _, _ = self.disk_coords(x0=x0, 
+                                       y0=y0,
+                                       inc=inc,
+                                       PA=PA,
+                                       z0=z0,
+                                       psi=psi,
+                                       r_cavity=r_cavity,
+                                       r_taper=r_taper,
+                                       q_taper=q_taper,
+                                       z_func=z_func,
+                                       shadowed=shadowed,
+                                       flatten=True)
+        
+        # Calculate the radial profile.
+
+        if assume_correlated:
+            nbeams = 2.0 * np.pi * rvals / self.bmaj
+        else:
+            nbeams = 1.0
+
+        # Radial binning.
+
+        toavg = data.flatten()
+        assert toavg.size == rpnts.size
+        ridxs = np.digitize(rpnts, rbins)
+
+        # Averaging.
+
+        if percentiles:
+            rstat = np.array([np.nabpercentile(toavg[ridxs == r], [16, 50, 84])
+                              for r in range(1, rbins.size)]).T
+            ravgs = rstat[1]
+            rstds = np.array([rstat[1] - rstat[0], rstat[2] - rstat[1]])
+            rstds /= np.sqrt(nbeams)[None, :]
+        else:
+            ravgs = np.array([np.nanmean(toavg[ridxs == r])
+                              for r in range(1, rbins.size)])
+            rstds = np.array([np.nanstd(toavg[ridxs == r])
+                              for r in range(1, rbins.size)])
+            rstds /= np.sqrt(nbeams)
+
+        # Return.
+
+        return rvals, ravgs, rstds
+
+    def background_residual(self, rbins=None, rvals=None, dr=None, x0=0.0,
+            y0=0.0, inc=0.0, PA=0.0, z0=None, psi=None, r_cavity=0.0,
+            r_taper=None, q_taper=1.0, z_func=None, shadowed=False, data=None,
+            return_background=False):
+        """
+        Subtract an azimuthally averaged residual from the data to highlight
+        residuals.
+
+        Args:
+            rbins (Optional[list]): List of bin edges.
+            rvals (Optional[list]): List of bin centers.
+            dr (Optional[float]): Spacing of bin centers in [arcsec]. Defaults
+                to a quarter of the beam major axis.
+            x0 (Optional[float]): Source right ascension offset [arcsec].
+            y0 (Optional[float]): Source declination offset [arcsec].
+            inc (Optional[float]): Source inclination [degrees]. A positive
+                inclination denotes a disk rotating clockwise on the sky, while
+                a negative inclination represents a counter-clockwise rotation.
+            PA (Optional[float]): Source position angle [degrees]. Measured
+                between north and the red-shifted semi-major axis in an
+                easterly direction.
+            z0 (Optional[float]): Aspect ratio at 1" for the emission surface.
+                To get the far side of the disk, make this number negative.
+            psi (Optional[float]): Flaring angle for the emission surface.
+            r_taper (Optional[float]): Radius for tapered emission surface.
+            q_taper (Optional[float]): Exponent for tapered emission surface.
+            r_cavity (Optional[float]): Outer radius of a cavity. Within this
+                region the emission surface is taken to be zero.
+            z_func (Optional[callable]): A user-defined emission surface
+                function that will return ``z`` in [arcsec] for a given ``r``
+                in [arcsec]. This will override the analytical form.
+            shadowed (Optional[bool]): Whether to use the slower, but more
+                robust method for deprojecting pixel values.
+            data (Optional[array]): Data to calculate a radial profile of. If
+                not provided, will use the attached dataset.
+            return_background (Optional[bool]): If ``True``, return the modeled
+                background rather than the residual.
+                
+        Returns:
+            background (array): The residuals after subtracted an azimuthally
+                symmetric background, or the modeled background if
+                ``return_background=True``.
+
+        """
+        from scipy.interpolate import interp1d
+
+        # Calculate the deprojected pixel values.
+
+        rpnts, _, _ = self.disk_coords(x0=x0, 
+                                       y0=y0,
+                                       inc=inc,
+                                       PA=PA,
+                                       z0=z0,
+                                       psi=psi,
+                                       r_cavity=r_cavity,
+                                       r_taper=r_taper,
+                                       q_taper=q_taper,
+                                       z_func=z_func,
+                                       shadowed=shadowed,
+                                       flatten=False)
+        
+        # Calculate the radial profile. Note here we already define what the
+        # data array is such that we can subtract the model from it later.
+
+        data = self.data if data is None else data
+        x, y, _ = self.radial_profile(rbins=rbins,
+                                      rvals=rvals,
+                                      dr=dr,
+                                      x0=x0, 
+                                      y0=y0,
+                                      inc=inc,
+                                      PA=PA,
+                                      z0=z0,
+                                      psi=psi,
+                                      r_cavity=r_cavity,
+                                      r_taper=r_taper,
+                                      q_taper=q_taper,
+                                      z_func=z_func,
+                                      shadowed=shadowed,
+                                      data=data)
+        
+        # Calculate the background model and return if necessary.
+
+        background = interp1d(x, y, bounds_error=False)(rpnts)
+        if return_background:
+            return background
+        
+        # Calculate the residual and return.
+
+        residual = data - background
+        return residual
+
     # -- PLOTTING FUNCTIONS -- #
 
     @staticmethod
     def cmap():
         import matplotlib.colors as mcolors
         c2 = plt.cm.Reds(np.linspace(0, 1, 16))
         c1 = plt.cm.Blues_r(np.linspace(0, 1, 16))
```

### Comparing `astro-eddy-2.3.7/eddy/default_parameters.yml` & `astro-eddy-2.3.9/eddy/default_parameters.yml`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/eddy/helper_functions.py` & `astro-eddy-2.3.9/eddy/helper_functions.py`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/eddy/linecube.py` & `astro-eddy-2.3.9/eddy/linecube.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def get_velocity_profile(self, rbins=None, fit_method='GP', fit_vrad=False,
             fix_vlsr=None, x0=0.0, y0=0.0, inc=0.0, PA=0.0, z0=0.0, psi=1.0,
             r_cavity=0.0, r_taper=np.inf, q_taper=1.0, w_i=None, w_r=None,
             w_t=None, z_func=None, shadowed=False, phi_min=None, phi_max=None,
             exclude_phi=False, abs_phi=False, mask_frame='disk', user_mask=None,
             beam_spacing=True, niter=1, get_vlos_kwargs=None,
-            weighted_average=True, return_samples=False):
+            weighted_average=True, return_samples=False, repeat_with_mask=0):
         """
         Returns the rotational and, optionally, radial velocity profiles under
         the assumption that the disk is azimuthally symmetric (at least across
         the regions extracted).
 
         Several different inference methods can be used through the
         ``fit_method`` argument:
@@ -112,14 +112,15 @@
             get_vlos_kwargs=None,
             weighted_average (Optional[bool]): Whether to combine multiple
                 iterations with a weighted average and standard deviation,
                 ``weighted_average=True``, or the traditional mean and standard
                 deviation, ``weighted_average=False``.
             return_samples (Optional[bool]): Whether to return the samples
                 instead of combining them.
+            repeat_with_mask (Optional[int]):
 
         Returns:
             samples (array): If ``return_samples=True``. The array of ``niter``
                 samples of the velocity profiles.
             rvals, profile, uncertainty (array, array, array): If
                 ``return_samples=False``. The arrays of radial locations and
                 combined velocity and uncertainties.
@@ -152,15 +153,16 @@
                                           phi_min=phi_min,
                                           phi_max=phi_max,
                                           exclude_phi=exclude_phi,
                                           abs_phi=abs_phi,
                                           mask_frame=mask_frame,
                                           user_mask=user_mask,
                                           beam_spacing=beam_spacing,
-                                          get_vlos_kwargs=get_vlos_kwargs)
+                                          get_vlos_kwargs=get_vlos_kwargs,
+                                          repeat_with_mask=repeat_with_mask)
 
         # Multiple iterations.
 
         if beam_spacing is False:
             raise ValueError("niter must equal 1 when beam_spacing=False.")
 
         samples = [self._velocity_profile(rbins=rbins,
@@ -184,15 +186,16 @@
                                           phi_min=phi_min,
                                           phi_max=phi_max,
                                           exclude_phi=exclude_phi,
                                           abs_phi=abs_phi,
                                           mask_frame=mask_frame,
                                           user_mask=user_mask,
                                           beam_spacing=beam_spacing,
-                                          get_vlos_kwargs=get_vlos_kwargs)
+                                          get_vlos_kwargs=get_vlos_kwargs,
+                                          repeat_with_mask=repeat_with_mask)
                    for _ in range(niter)]
 
         # Just return the samples if requested.
 
         if return_samples:
             return samples
         
@@ -230,15 +233,16 @@
         return rpnts, profile, uncertainty
 
     def _velocity_profile(self, rbins=None, fit_method='GP', fit_vrad=False,
             fix_vlsr=None, x0=0.0, y0=0.0, inc=0.0, PA=0.0, z0=0.0, psi=1.0,
             r_cavity=0.0,  r_taper=np.inf, q_taper=1.0, w_i=None, w_r=None,
             w_t=None, z_func=None, shadowed=False, phi_min=None, phi_max=None,
             exclude_phi=False, abs_phi=False, mask_frame='disk',
-            user_mask=None, beam_spacing=True, get_vlos_kwargs=None):
+            user_mask=None, beam_spacing=True, get_vlos_kwargs=None,
+            repeat_with_mask=0):
         """
         Returns the velocity (rotational and radial) profiles.
 
         Args:
             TBD
 
         Returns:
@@ -253,14 +257,15 @@
 
         # Set up the kwargs for the fitting.
 
         kw = {} if get_vlos_kwargs is None else get_vlos_kwargs
         kw['fit_vrad'] = fit_vrad
         kw['fix_vlsr'] = fix_vlsr
         kw['fit_method'] = fit_method
+        kw['repeat_with_mask'] = repeat_with_mask
 
         # Cycle through the annuli.
 
         profiles = []
         uncertainties = []
         for r_min, r_max in zip(rbins[:-1], rbins[1:]):
             annulus = self.get_annulus(r_min=r_min,
@@ -462,14 +467,16 @@
         contourf_kwargs['colors'] = contourf_kwargs.pop('colors', mask_color)
 
         # Plot the contour and return the figure.
 
         ax.contourf(self.xaxis, self.yaxis, mask, [-.5, .5], **contourf_kwargs)
         ax.contour(self.xaxis, self.yaxis, mask, 1, **contour_kwargs)
 
+    # -- UTILITIES -- #
+
     def get_spectrum(self, coords, x0=0.0, y0=0.0, inc=0.0, PA=0.0,
                      z0=0.0, psi=1.0, z_func=None, frame='sky',
                      coord_type='cartesian', area=0.0, beam_weighting=False,
                      return_mask=False):
         """
         Return a spectrum at a position defined by a coordinates given either
         in sky-frame position (``frame='sky'``) or a disk-frame location
```

### Comparing `astro-eddy-2.3.7/eddy/modelling.py` & `astro-eddy-2.3.9/eddy/modelling.py`

 * *Files identical despite different names*

### Comparing `astro-eddy-2.3.7/eddy/rotationmap.py` & `astro-eddy-2.3.9/eddy/rotationmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -811,20 +811,27 @@
 
         Returns:
             fig (Matplotlib figure): If ``return_fig`` is ``True``. Can access
                 the axes through ``fig.axes`` for additional plotting.
         """
         import matplotlib.pyplot as plt
         fig, ax = plt.subplots()
+    
+        if vmin is None or vmax is None:
+            vmin_tmp, vmax_tmp = np.nanpercentile(self.data, [2, 98])
+            vmax_tmp = max(abs(vmin_tmp - self.vlsr), abs(vmax_tmp - self.vlsr))
+            vmin_tmp = (self.vlsr - vmax_tmp) / 1e3
+            vmax_tmp = (self.vlsr + vmax_tmp) / 1e3
+            if vmin is None:
+                vmin = vmin_tmp
+            if vmax is None:
+                vmax = vmax_tmp
 
-        vmin = np.nanpercentile(self.data, [2]) if vmin is None else vmin
-        vmax = np.nanpercentile(self.data, [98]) if vmax is None else vmax
-        vmax = max(abs(vmin - self.vlsr), abs(vmax - self.vlsr))
         im = ax.imshow(self.data / 1e3, origin='lower', extent=self.extent,
-                       vmin=(self.vlsr-vmax)/1e3, vmax=(self.vlsr+vmax)/1e3,
+                       vmin=vmin, vmax=vmax,
                        cmap=rotationmap.cmap(), zorder=-9)
         cb = plt.colorbar(im, pad=0.03, extend='both', format='%.2f')
         cb.minorticks_on()
         cb.set_label(r'${\rm v_{0} \quad (km\,s^{-1})}$',
                      rotation=270, labelpad=15)
         if ivar is not None:
             ax.contour(self.xaxis, self.yaxis, ivar,
@@ -1051,40 +1058,16 @@
         else:
             params['vfunc'] = self._vkep
 
         # Deprojection properties.
 
         params['z_func'] = params.pop('z_func', None)
         params['shadowed'] = params.pop('shadowed', False)
-
-        # Masking parameters.
-
-        # params['r_min'] = params.pop('r_min', 0.0)
-        # params['r_max'] = params.pop('r_max', 1e10)
-        # params['exclude_r'] = params.pop('exclude_r', False)
-        # params['phi_min'] = params.pop('phi_min', -180.0)
-        # params['phi_max'] = params.pop('phi_max', 180.0)
-        # params['exclude_phi'] = params.pop('exclude_phi', False)
-        # params['abs_phi'] = params.pop('abs_phi', False)
-        # params['v_min'] = params.pop('v_min', np.nanmin(self.data))
-        # params['v_max'] = params.pop('v_max', np.nanmax(self.data))
-        # params['exclude_v'] = params.pop('exclude_v', False)
         params['user_mask'] = params.pop('user_mask', np.ones(self.data.shape))
 
-        # if params['r_min'] >= params['r_max']:
-        #     raise ValueError("`r_max` must be greater than `r_min`.")
-        # if params['phi_min'] >= params['phi_max']:
-        #     raise ValueError("`phi_max` must be great than `phi_min`.")
-        # if params['v_min'] >= params['v_max']:
-        #     raise ValueError("`v_max` must be greater than `v_min`.")
-
-        # Beam convolution.
-
-        # params['beam'] = bool(params.pop('beam', False))
-
         return params
 
     def evaluate_models(self, samples=None, params=None, draws=50,
                         collapse_func=np.mean, coords_only=False,
                         profile_only=False):
         """
         Evaluate models based on the samples provided and the parameter
@@ -1425,14 +1408,15 @@
             data_tmp = np.where(hotpix, coldpix, data_tmp)
         
         # Either replace the attached data or return as an array.
 
         if not replace:
             return data_tmp
         self.data = data_tmp
+        self.mask = np.isfinite(self.data)
 
     # -- Functions to help determine the emission height. -- #
 
     def find_maxima(self, x0=0.0, y0=0.0, PA=0.0, vlsr=None, r_max=None,
                     r_min=None, smooth=False, through_center=True):
         """
         Find the node of velocity maxima along the major axis of the disk.
```

### Comparing `astro-eddy-2.3.7/setup.py` & `astro-eddy-2.3.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="astro-eddy",
-    version="2.3.7",
+    version="2.3.9",
     author="Richard Teague",
     author_email="rteague@mit.edu",
     description=("Tools to study the dynamics of protoplanetary disks."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/richteague/eddy",
     packages=["eddy"],
@@ -20,14 +20,15 @@
     install_requires=[
         "scipy>=1",
         "numpy",
         "matplotlib>=3",
         "emcee>=3",
         "corner>=2",
         "zeus-mcmc",
+        "bettermoments",
         ],
     package_data={'eddy': ['*.yml']},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

