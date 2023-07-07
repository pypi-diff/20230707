# Comparing `tmp/planetmapper-1.7.5.tar.gz` & `tmp/planetmapper-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.7.5.tar", last modified: Wed Jun 21 20:40:38 2023, max compression
+gzip compressed data, was "planetmapper-1.7.6.tar", last modified: Fri Jul  7 16:50:54 2023, max compression
```

## Comparing `planetmapper-1.7.5.tar` & `planetmapper-1.7.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 20:40:28.000000 planetmapper-1.7.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-21 20:40:38.400402 planetmapper-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-21 20:40:28.000000 planetmapper-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.396402 planetmapper-1.7.5/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   112285 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/data/ring_aliases.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118682 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-21 20:40:28.000000 planetmapper-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:40:38.400402 planetmapper-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-21 20:40:28.000000 planetmapper-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    28477 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.271321 planetmapper-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 16:50:40.000000 planetmapper-1.7.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-07 16:50:54.271321 planetmapper-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-07 16:50:40.000000 planetmapper-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.267321 planetmapper-1.7.6/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112285 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.267321 planetmapper-1.7.6/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118974 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46648 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.267321 planetmapper-1.7.6/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-07 16:50:40.000000 planetmapper-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:50:54.271321 planetmapper-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-07 16:50:40.000000 planetmapper-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.271321 planetmapper-1.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29465 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_utils.py
```

### Comparing `planetmapper-1.7.5/LICENSE.txt` & `planetmapper-1.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/PKG-INFO` & `planetmapper-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.5
+Version: 1.7.6
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.5/README.md` & `planetmapper-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/__init__.py` & `planetmapper-1.7.6/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/base.py` & `planetmapper-1.7.6/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/basic_body.py` & `planetmapper-1.7.6/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/body.py` & `planetmapper-1.7.6/planetmapper/body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/body_xy.py` & `planetmapper-1.7.6/planetmapper/body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/data/rings.json` & `planetmapper-1.7.6/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/data_loader.py` & `planetmapper-1.7.6/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/gui.py` & `planetmapper-1.7.6/planetmapper/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,30 +224,38 @@
                     lambda: self.get_observation().centre_disc(),
                     'Centre disc in image',
                     'Centre the target\'s planetary disc and make it fill ~90% of the observation',
                 ),
             ],
             'Use WCS data from FITS header': [
                 (
-                    lambda: self.get_observation().disc_from_wcs(True, False),
+                    lambda: self.get_observation().disc_from_wcs(
+                        suppress_warnings=True, validate=False
+                    ),
                     'Use WCS position, rotation & scale',
                     'Set all disc parameters using approximate WCS information in the observation\'s FITS header',
                 ),
                 (
-                    lambda: self.get_observation().position_from_wcs(True, False),
+                    lambda: self.get_observation().position_from_wcs(
+                        suppress_warnings=True, validate=False
+                    ),
                     'Use WCS position',
                     'Set disc position using approximate WCS information in the observation\'s FITS header',
                 ),
                 (
-                    lambda: self.get_observation().rotation_from_wcs(True, False),
+                    lambda: self.get_observation().rotation_from_wcs(
+                        suppress_warnings=True, validate=False
+                    ),
                     'Use WCS rotation',
                     'Set disc rotation using approximate WCS information in the observation\'s FITS header',
                 ),
                 (
-                    lambda: self.get_observation().plate_scale_from_wcs(True, False),
+                    lambda: self.get_observation().plate_scale_from_wcs(
+                        suppress_warnings=True, validate=False
+                    ),
                     'Use WCS plate scale',
                     'Set plate scale using approximate WCS information in the observation\'s FITS header',
                 ),
             ],
             'Fit observation': [
                 (
                     lambda: self.get_observation().fit_disc_position(),
```

### Comparing `planetmapper-1.7.5/planetmapper/kernel_downloader.py` & `planetmapper-1.7.6/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/observation.py` & `planetmapper-1.7.6/planetmapper/observation.py`

 * *Files 5% similar despite different names*

```diff
@@ -318,14 +318,15 @@
                 warnings.simplefilter('ignore', category=AstropyWarning)
             return astropy.wcs.WCS(self.header).celestial
 
     def _get_disc_params_from_wcs(
         self,
         suppress_warnings: bool = False,
         validate: bool = True,
+        use_header_offsets: bool = True,
     ) -> tuple[float, float, float, float]:
         wcs = self._get_wcs_from_header(suppress_warnings=suppress_warnings)
 
         if wcs.naxis == 0:
             raise ValueError('No WCS information found in FITS header')
 
         if validate:
@@ -336,30 +337,41 @@
             if not wcs.world_axis_physical_types == ['pos.eq.ra', 'pos.eq.dec']:
                 raise ValueError(
                     'WCS axes are not RA/Dec coordinates'
                 )  # pragma: no cover
             if wcs.has_distortion:
                 raise ValueError('WCS conversion contains distortion terms')
 
-        x0, y0 = wcs.world_to_pixel_values(self.target_ra, self.target_dec)
+        if use_header_offsets:
+            dra_arcsec = float(self.header.get('HIERARCH NAV RA_OFFSET', 0.0))  # type: ignore
+            ddec_arcsec = float(self.header.get('HIERARCH NAV DEC_OFFSET', 0.0))  # type: ignore
+            dra = dra_arcsec / 3600
+            ddec = ddec_arcsec / 3600
+        else:
+            dra = 0.0
+            ddec = 0.0
+
+        x0, y0 = wcs.world_to_pixel_values(self.target_ra + dra, self.target_dec + ddec)
 
         b1, b2 = wcs.pixel_to_world_values(x0, y0 + 1)
         c1, c2 = wcs.pixel_to_world_values(x0, y0)
 
         rotation = np.rad2deg(np.arctan2(b1 - c1, b2 - c2))
 
         s = self.angular_dist(b1, b2, c1, c2)
         arcsec_per_px = s * 60 * 60  # s = degrees/px
         r0 = self.target_diameter_arcsec / (2 * arcsec_per_px)
-        x0, y0 = wcs.world_to_pixel_values(self.target_ra, self.target_dec)
 
         return x0, y0, r0, rotation
 
     def disc_from_wcs(
-        self, suppress_warnings: bool = False, validate: bool = True
+        self,
+        suppress_warnings: bool = False,
+        validate: bool = True,
+        use_header_offsets: bool = True,
     ) -> None:
         """
         Set disc parameters using WCS information in the observation's FITS header.
 
         See also :func:`rotation_from_wcs` and :func:`plate_scale_from_wcs`.
 
         .. note::
@@ -369,96 +381,80 @@
             PlanetMapper
 
         Args:
             suppress_warnings: Hide warnings produced by astropy when calculating WCS
                 conversions.
             validate: Run checks to ensure the WCS conversion has appropriate RA/Dec
                 coordinate dimensions.
+            use_header_offsets: If present, use the `HIERARCH NAV RA_OFFSET` and
+                `HIERARCH NAV DEC_OFFSET` values from the FITS headerr to adjust the
+                target's disc location by the specified arcsecond offsets. If these
+                keywords are not present or `use_header_offsets` is `False`, no
+                adjustment is made.
         Raises:
             ValueError: if no WCS information is found in the FITS header, or validation
                 fails.
         """
         x0, y0, r0, rotation = self._get_disc_params_from_wcs(
-            suppress_warnings, validate
+            suppress_warnings, validate, use_header_offsets
         )
         self.set_x0(x0)
         self.set_y0(y0)
         self.set_r0(r0)
         self.set_rotation(rotation)
         self.set_disc_method('wcs')
 
-    def position_from_wcs(
-        self, suppress_warnings: bool = False, validate: bool = True
-    ) -> None:
+    def position_from_wcs(self, *args, **kwargs) -> None:
         """
         Set disc position `(x0, y0)` using WCS information in the observation's FITS
         header.
 
         See also :func:`disc_from_wcs`.
 
         Args:
-            suppress_warnings: Hide warnings produced by astropy when calculating WCS
-                conversions.
-            validate: Run checks to ensure the WCS conversion has appropriate RA/Dec
-                coordinate dimensions.
+            *args, **kwargs: See :func:`disc_from_wcs` for additional arguments.
         Raises:
             ValueError: if no WCS information is found in the FITS header, or validation
                 fails.
         """
-        x0, y0, r0, rotation = self._get_disc_params_from_wcs(
-            suppress_warnings, validate
-        )
+        x0, y0, r0, rotation = self._get_disc_params_from_wcs(*args, **kwargs)
         self.set_x0(x0)
         self.set_y0(y0)
         self.set_disc_method('wcs_position')
 
-    def rotation_from_wcs(
-        self, suppress_warnings: bool = False, validate: bool = True
-    ) -> None:
+    def rotation_from_wcs(self, *args, **kwargs) -> None:
         """
         Set disc rotation using WCS information in the observation's FITS header.
 
         See also :func:`disc_from_wcs`.
 
         Args:
-            suppress_warnings: Hide warnings produced by astropy when calculating WCS
-                conversions.
-            validate: Run checks to ensure the WCS conversion has appropriate RA/Dec
-                coordinate dimensions.
+            *args, **kwargs: See :func:`disc_from_wcs` for additional arguments.
         Raises:
             ValueError: if no WCS information is found in the FITS header, or validation
                 fails.
         """
-        x0, y0, r0, rotation = self._get_disc_params_from_wcs(
-            suppress_warnings, validate
-        )
+        x0, y0, r0, rotation = self._get_disc_params_from_wcs(*args, **kwargs)
         self.set_rotation(rotation)
         self.set_disc_method('wcs_rotation')
 
-    def plate_scale_from_wcs(
-        self, suppress_warnings: bool = False, validate: bool = True
-    ) -> None:
+    def plate_scale_from_wcs(self, *args, **kwargs) -> None:
         """
         Set plate scale (i.e. `r0`) using WCS information in the observation's FITS
         header.
 
         See also :func:`disc_from_wcs`.
 
         Args:
-            suppress_warnings: Hide warnings produced by astropy when calculating WCS
-                conversions.
-            validate: Run checks to ensure the WCS conversion has appropriate RA/Dec
-                coordinate dimensions.
+            *args, **kwargs: See :func:`disc_from_wcs` for additional arguments.
         Raises:
             ValueError: if no WCS information is found in the FITS header, or validation
                 fails.
         """
-        x0, y0, r0, rotation = self._get_disc_params_from_wcs(
-            suppress_warnings, validate
-        )
+        x0, y0, r0, rotation = self._get_disc_params_from_wcs(*args, **kwargs)
         self.set_r0(r0)
         self.set_disc_method('wcs_plate_scale')
 
     def _get_img_for_fitting(self) -> np.ndarray:
         img = np.nansum(self.data, axis=0)
         mask_img = np.isnan(img)
         img[mask_img] = np.nanmin(img)  # Mask nan values for com calculation etc.
```

### Comparing `planetmapper-1.7.5/planetmapper/progress.py` & `planetmapper-1.7.6/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper/utils.py` & `planetmapper-1.7.6/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.7.6/planetmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.5
+Version: 1.7.6
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.5/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.7.6/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/pyproject.toml` & `planetmapper-1.7.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     "^if TYPE_CHECKING:$",
     ]
 
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = [
     "C",
-    "fixme",
     "unused-variable",
     "no-else-return",
     "use-dict-literal",
     "duplicate-code",
     "too-many-arguments",
     "too-many-instance-attributes",
     "too-many-locals",
@@ -43,14 +42,17 @@
     "too-many-ancestors",
     "too-many-return-statements",
     ]
 enable = [
     "useless-suppression",
     ]
 
+[tool.pylint.miscellaneous]
+notes=["FIXME", "XXX"] # Allow TODO comments, but not FIXME or XXX
+
 
 [tool.pyright]
 include = ["planetmapper/*.py", "setup.py"]
 reportPropertyTypeMismatch = true
 reportConstantRedefinition = true
 reportIncompatibleMethodOverride = true
 reportIncompatibleVariableOverride = true
```

### Comparing `planetmapper-1.7.5/setup.py` & `planetmapper-1.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_base.py` & `planetmapper-1.7.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_basic_body.py` & `planetmapper-1.7.6/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_body.py` & `planetmapper-1.7.6/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_body_xy.py` & `planetmapper-1.7.6/tests/test_body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_common.py` & `planetmapper-1.7.6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_data_loader.py` & `planetmapper-1.7.6/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_init.py` & `planetmapper-1.7.6/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_kernel_downloader.py` & `planetmapper-1.7.6/tests/test_kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_observation.py` & `planetmapper-1.7.6/tests/test_observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,14 +414,38 @@
                 'CUNIT1': 'deg',
                 'CUNIT2': 'deg',
             }
         )
         obs = Observation(data=data, header=header)
         obs.disc_from_wcs(suppress_warnings=True)
 
+        x0_before = obs.get_x0()
+        y0_before = obs.get_y0()
+
+        data = np.ones((5, 6, 7))
+        h2 = header.copy()
+        h2['HIERARCH NAV RA_OFFSET'] = 1
+        h2['HIERARCH NAV DEC_OFFSET'] = -2.5
+        obs = Observation(data=data, header=h2)
+        obs.disc_from_wcs(suppress_warnings=True)
+        self.assertNotEqual(obs.get_x0(), x0_before)
+        self.assertNotEqual(obs.get_y0(), y0_before)
+
+        obs.add_arcsec_offset(-1, 2.5)  # undo the header offsets
+        self.assertAlmostEqual(obs.get_x0(), x0_before, delta=0.2)
+        self.assertAlmostEqual(obs.get_y0(), y0_before, delta=0.2)
+
+        obs.disc_from_wcs(suppress_warnings=True)
+        self.assertNotEqual(obs.get_x0(), x0_before)
+        self.assertNotEqual(obs.get_y0(), y0_before)
+
+        obs.disc_from_wcs(suppress_warnings=True, use_header_offsets=False)
+        self.assertAlmostEqual(obs.get_x0(), x0_before, delta=0.2)
+        self.assertAlmostEqual(obs.get_y0(), y0_before, delta=0.2)
+
         h2 = header.copy()
         h2['CTYPE1'] = 'DEC--TAN'
         obs = Observation(data=data, header=h2)
         with self.assertRaises(ValueError):
             obs.disc_from_wcs(suppress_warnings=True)
 
         h2 = header.copy()
```

### Comparing `planetmapper-1.7.5/tests/test_progress.py` & `planetmapper-1.7.6/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.5/tests/test_utils.py` & `planetmapper-1.7.6/tests/test_utils.py`

 * *Files identical despite different names*

