# Comparing `tmp/nifti_mrs-0.1.7.tar.gz` & `tmp/nifti_mrs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti_mrs-0.1.7.tar", last modified: Sun Apr  2 16:05:09 2023, max compression
+gzip compressed data, was "nifti_mrs-1.0.0.tar", last modified: Fri Jul  7 11:01:25 2023, max compression
```

## Comparing `nifti_mrs-0.1.7.tar` & `nifti_mrs-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:05:09.684588 nifti_mrs-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-02 16:05:09.684588 nifti_mrs-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-02 16:05:09.684588 nifti_mrs-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:05:09.668588 nifti_mrs-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:05:09.672587 nifti_mrs-0.1.7/src/mrs_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/mrs_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/mrs_tools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:05:09.684588 nifti_mrs-0.1.7/src/nifti_mrs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-02 16:05:09.684588 nifti_mrs-0.1.7/src/nifti_mrs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/hdr_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/nifti_mrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:05:09.680588 nifti_mrs-0.1.7/src/nifti_mrs/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/tools/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/tools/split_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/src/nifti_mrs/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:05:09.676587 nifti_mrs-0.1.7/src/nifti_mrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-02 16:05:09.000000 nifti_mrs-0.1.7/src/nifti_mrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-02 16:05:09.000000 nifti_mrs-0.1.7/src/nifti_mrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:05:09.000000 nifti_mrs-0.1.7/src/nifti_mrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-02 16:05:09.000000 nifti_mrs-0.1.7/src/nifti_mrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-02 16:05:09.000000 nifti_mrs-0.1.7/src/nifti_mrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-02 16:05:09.000000 nifti_mrs-0.1.7/src/nifti_mrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:05:09.684588 nifti_mrs-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/tests/test_create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/tests/test_nifti_mrs.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/tests/test_nifti_mrs_tools_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/tests/test_nifti_mrs_tools_reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    28525 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/tests/test_nifti_mrs_tools_split_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/tests/test_nifti_mrs_tools_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-02 16:04:56.000000 nifti_mrs-0.1.7/tests/test_script_mrs_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.973532 nifti_mrs-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/src/mrs_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/mrs_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/mrs_tools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/src/nifti_mrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/src/nifti_mrs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/nifti_mrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/src/nifti_mrs/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_script_mrs_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_validator.py
```

### Comparing `nifti_mrs-0.1.7/LICENSE` & `nifti_mrs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti_mrs-0.1.7/PKG-INFO` & `nifti_mrs-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti_mrs
-Version: 0.1.7
+Version: 1.0.0
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nifti_mrs-0.1.7/README.md` & `nifti_mrs-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nifti_mrs-0.1.7/setup.cfg` & `nifti_mrs-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nifti_mrs-0.1.7/src/mrs_tools/__init__.py` & `nifti_mrs-1.0.0/src/mrs_tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
     """
     import nifti_mrs.tools as nmrs_tools
     from nifti_mrs.nifti_mrs import NIFTI_MRS
     # 1. Load the file
     to_reorder = NIFTI_MRS(args.file)
     reorder_name = args.file.with_suffix('').with_suffix('').name
 
-    # 2. Merge the files
+    # 2. Reorder the files
     dim_order = args.dim_order
     while len(dim_order) < 3:
         dim_order.append(None)
     reordered = nmrs_tools.reorder(to_reorder, args.dim_order)
 
     # 3. Save the output file
     if args.filename:
```

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs/create_nmrs.py` & `nifti_mrs-1.0.0/src/nifti_mrs/create_nmrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs/definitions.py` & `nifti_mrs-1.0.0/src/nifti_mrs/definitions.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs/hdr_ext.py` & `nifti_mrs-1.0.0/src/nifti_mrs/hdr_ext.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 class Hdr_Ext:
     """Class to hold meta data stored in a NIfTI MRS header extension.
     Required fields must be passed to initialise,
     Default dimension information automatically generated, but may be modified by set_dim_info method.
     Standard defined meta-data and user-defined data can be added using set_standard_def and
     set_user_def respectively.
     """
-    def __init__(self, spec_frequency, resonant_nucleus, dimensions=7):
+    def __init__(self, spec_frequency, resonant_nucleus, dimensions=None):
         """Initialise NIfTI-MRS header extension object with the two mandatory bits of meta-data.
 
+        Use the dimensions kwarg to initialise with the default dimension tags (DIM_COIL, DIM_DYN,
+        DIM_INDIRECT_0) for values for 5, 6, and 7 respectively.
+
         :param spec_frequency: Spectrometer frequency in MHz
         :type spec_frequency: float
         :param resonant_nucleus: Resonant nucleus e.g. '1H'
         :type resonant_nucleus: str
-        :param dimensions: Number of dimensions in image. Controls number of dim tags in extension. Defaults to 7
+        :param dimensions: Number of dimensions in image. Defaults to None
         :type dimensions: int, optional
         """
         if isinstance(spec_frequency, float):
             self.SpectrometerFrequency = [spec_frequency, ]
         elif isinstance(spec_frequency, (list, tuple))\
                 and isinstance(spec_frequency[0], float):
             self.SpectrometerFrequency = spec_frequency
@@ -31,25 +34,39 @@
             self.ResonantNucleus = [resonant_nucleus, ]
         elif isinstance(resonant_nucleus, (list, tuple))\
                 and isinstance(resonant_nucleus[0], str):
             self.ResonantNucleus = resonant_nucleus
         else:
             raise ValueError('resonant_nucleus must be a string or array of strings.')
 
-        self._dim_info = [{"tag": "DIM_COIL", "info": None, "hdr": None},
-                          {"tag": "DIM_DYN", "info": None, "hdr": None},
-                          {"tag": "DIM_INDIRECT_0", "info": None, "hdr": None}]
+        # Standard tags definition
+        standard_tags = [{"tag": "DIM_COIL", "info": None, "hdr": None},
+                         {"tag": "DIM_DYN", "info": None, "hdr": None},
+                         {"tag": "DIM_INDIRECT_0", "info": None, "hdr": None}]
+        if dimensions is None or dimensions <= 4:
+            self._dim_info = [{"tag": None, "info": None, "hdr": None}, ] * 3
+        elif dimensions > 4 and dimensions <= 7:
+            self._dim_info = [{"tag": None, "info": None, "hdr": None}, ] * 3
+            dim_higher = dimensions - 4
+            self._dim_info[:dim_higher] = standard_tags[:dim_higher]
+        else:
+            raise ValueError('dimensions kwarg must be None or an int from 4 to 7.')
 
         self._standard_data = {}
         self._user_data = {}
-        self.dimensions = dimensions
 
     @classmethod
-    def from_header_ext(cls, hdr_ext_dict, dimensions=7):
+    def from_header_ext(cls, hdr_ext_dict):
+        """Create a Hdr_Ext object from a json string deserialised into a python dict
 
+        :param hdr_ext_dict: header extension as a dict.
+        :type hdr_ext_dict: dict
+        :return: Class object
+        :rtype: Hdr_Ext
+        """
         optional_dict = dict(hdr_ext_dict)
         obj = cls(
             hdr_ext_dict['SpectrometerFrequency'],
             hdr_ext_dict['ResonantNucleus'])
         optional_dict.pop('SpectrometerFrequency')
         optional_dict.pop('ResonantNucleus')
 
@@ -69,20 +86,40 @@
                     hdr = None
                 obj.set_dim_info(idx - 5, tag, info=info, hdr=hdr)
 
         for key in optional_dict:
             if key in standard_defined:
                 obj.set_standard_def(key, hdr_ext_dict[key])
             else:
-                obj.set_user_def(key=key, value=hdr_ext_dict[key])
-
-        obj.dimensions = dimensions
+                if 'Value' in hdr_ext_dict[key]\
+                        and 'Description' in hdr_ext_dict[key]:
+                    obj.set_user_def(
+                        key,
+                        hdr_ext_dict[key]['Value'],
+                        hdr_ext_dict[key]['Description'])
+                elif isinstance(hdr_ext_dict[key], dict)\
+                        and 'Description' in hdr_ext_dict[key]:
+                    obj.set_user_def(
+                        key,
+                        hdr_ext_dict[key],
+                        hdr_ext_dict[key]['Description'])
+                else:
+                    raise ValueError(f'User-defined key {key} must contain a "Description" field"')
 
         return obj
 
+    @property
+    def ndim(self):
+        """Returns the number of dimensions implied by the 'dim_{5,6,7}' tags"""
+        ndim = 4
+        for ddx in range(5, 8):
+            if f'dim_{ddx}' in self.current_keys:
+                ndim += 1
+        return ndim
+
     def set_dim_info(self, dim, tag, info=None, hdr=None):
         """Set information associated with the optional, higher data dimensions.
 
         :param dim:  May be (0,1,2) or ("5th","6th","7th")
         :type dim: str or int
         :param tag: Must be one of the defined dimension tag strings. E.g. DIM_DYN
         :type tag: str
@@ -126,42 +163,37 @@
             elif dim == "7th":
                 dim = 2
         else:
             raise ValueError('dim must be 0,1,2 or "5th","6th","7th".')
 
         self._dim_info.pop(dim)
         self._dim_info.append({"tag": None, "info": None, "hdr": None})
-        self.dimensions -= 1
 
     def set_standard_def(self, key, value):
         """Add a single standard-defined bit of meta-data to the object."""
         if key not in standard_defined:
             raise ValueError("key must be one of the standard-defined keys.")
 
         self._standard_data[key] = value
 
-    def set_user_def(self, all_keys=None, key=None, value=None, doc=None):
-        """Add user defined meta data keys to the header extension.
-        Pass dict as kwarg all_keys to set all key/value pairs, or
+    def set_user_def(self, key, value, doc):
+        """Add user-defined metadata keys to the header extension.
         add keys and values one at a time using key, value and doc.
         """
 
-        if all_keys is not None:
-            self._user_data = all_keys
-        else:
-            if key in standard_defined:
-                raise ValueError("key must not be one of the standard-defined keys.")
+        if key in standard_defined:
+            raise ValueError("key must not be one of the standard-defined keys.")
 
-            if isinstance(value, dict):
-                self._user_data[key] = value
-                self._user_data[key].update({'Description': doc})
-            else:
-                self._user_data[key] = {
-                    'Value': value,
-                    'Description': doc}
+        if isinstance(value, dict):
+            self._user_data[key] = value
+            self._user_data[key].update({'Description': doc})
+        else:
+            self._user_data[key] = {
+                'Value': value,
+                'Description': doc}
 
     def remove_standard_def(self, key):
         """Remove key from list of standard defined key-value pairs
 
         :param key: Key name
         :type key: str
         """
@@ -176,35 +208,30 @@
         :type key: str
         """
         if key not in self.current_keys:
             raise KeyError(f'{key} is not defined in the header extension.')
         self._user_data.pop(key)
 
     def to_dict(self):
-        """Generate dictionay representation from properties."""
+        """Generate dictionary representation from properties."""
 
         # Required meta-data
         out_dict = {'SpectrometerFrequency': self.SpectrometerFrequency,
                     'ResonantNucleus': self.ResonantNucleus}
 
         # Dimension information
-        if self.dimensions < 4:
-            raise ValueError('dimensions must be 4 or greater')
-        elif self.dimensions == 4:
-            pass
-        else:
-            update_dict = {}
-            for idx in range(5, self.dimensions + 1):
+        update_dict = {}
+        for idx in range(5, 8):
+            if self._dim_info[idx - 5]['tag'] is not None:
                 update_dict[f'dim_{idx}'] = self._dim_info[idx - 5]['tag']
-                if self._dim_info[idx - 5]['info'] is not None:
-                    update_dict[f'dim_{idx}_info'] = self._dim_info[idx - 5]['info']
-                if self._dim_info[idx - 5]['hdr'] is not None:
-                    update_dict[f'dim_{idx}_header'] = self._dim_info[idx - 5]['hdr']
-
-            out_dict.update(update_dict)
+            if self._dim_info[idx - 5]['info'] is not None:
+                update_dict[f'dim_{idx}_info'] = self._dim_info[idx - 5]['info']
+            if self._dim_info[idx - 5]['hdr'] is not None:
+                update_dict[f'dim_{idx}_header'] = self._dim_info[idx - 5]['hdr']
+        out_dict.update(update_dict)
 
         # Add standard defined
         out_dict.update(self._standard_data)
 
         # Add user defined
         out_dict.update(self._user_data)
```

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs/nifti_mrs.py` & `nifti_mrs-1.0.0/src/nifti_mrs/nifti_mrs.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 
 from fsl.data.image import Image
 
 from . import validator
 from .hdr_ext import Hdr_Ext
 from .definitions import dimension_tags, standard_defined
+import nifti_mrs.utils as utils
 
 
 class NIFTIMRS_DimDoesntExist(Exception):
     pass
 
 
 class NotNIFTI_MRS(Exception):
@@ -31,15 +32,15 @@
 
     Access the underlying fslpy Image object for useful attributes using obj.image.
     """
 
     def __init__(self, *args, **kwargs):
         """Create a NIFTI_MRS object with the given image data or file name.
 
-        Aguments mirror those of the leveraged fsl.data.image.IMage class.
+        Arguments mirror those of the leveraged fsl.data.image.IMage class.
 
         :arg image:      A string containing the name of an image file to load,
                          or a Path object pointing to an image file, or a
                          :mod:`numpy` array, or a :mod:`nibabel` image object,
                          or an ``Image`` object.
 
         :arg name:       A name for the image.
@@ -115,16 +116,21 @@
         else:
             hdr_ext_codes = self.header.extensions.get_codes()
             if 44 not in hdr_ext_codes:
                 raise NotNIFTI_MRS('NIFTI-MRS must have a header extension.')
 
             self._hdr_ext = Hdr_Ext.from_header_ext(
                 json.loads(
-                    self.header.extensions[hdr_ext_codes.index(44)].get_content()),
-                dimensions=self.ndim)
+                    self.header.extensions[hdr_ext_codes.index(44)].get_content()))
+
+        # Some validation upon creation
+        validator.validate_hdr_ext(
+            self._hdr_ext.to_json(),
+            self.image.shape,
+            np.max((self._hdr_ext.ndim, self.image.ndim)))
 
         try:
             self.nucleus
             self.spectrometer_frequency
         except KeyError:
             raise NotNIFTI_MRS('NIFTI-MRS header extension must have nucleus and spectrometerFrequency keys.')
 
@@ -147,22 +153,26 @@
     # Implement useful calls to attributes of the image class object. Should I just be using inheretence here? Not sure.
     @property
     def header(self):
         """Returns NIfTI-MRS header object"""
         return self.image.header
 
     @property
-    def shape(self):
-        """Returns data shape"""
-        return self.image.shape
+    def ndim(self):
+        """Returns number of dimensions in the NIfTI-MRS object"""
+        return self.hdr_ext.ndim
 
     @property
-    def ndim(self):
-        """Returns number of data dimensions"""
-        return self.image.ndim
+    def shape(self):
+        """Returns the data shape. Singleton dimensions implied by header extension keys are included.
+        Use obj.image.shape to get the shape of the stored data"""
+        base_shape = self.image.shape
+        for _ in range(self.image.ndim, self.hdr_ext.ndim):
+            base_shape += (1, )
+        return base_shape
 
     @property
     def dtype(self):
         """Returns data type"""
         return self.image.dtype
 
     @property
@@ -250,18 +260,18 @@
         self.header.extensions.clear()
         self.header.extensions.append(extension)
 
     @hdr_ext.setter
     def hdr_ext(self, new_hdr):
         '''Update MRS JSON header extension from python dict or Hdr_Ext object'''
         if isinstance(new_hdr, dict):
-            validator.validate_hdr_ext(json.dumps(new_hdr), self.ndim)
-            self._hdr_ext = Hdr_Ext.from_header_ext(new_hdr, dimensions=self.ndim)
+            validator.validate_hdr_ext(json.dumps(new_hdr), self.shape)
+            self._hdr_ext = Hdr_Ext.from_header_ext(new_hdr)
         elif isinstance(new_hdr, Hdr_Ext):
-            validator.validate_hdr_ext(new_hdr.to_json(), self.ndim)
+            validator.validate_hdr_ext(new_hdr.to_json(), self.shape)
             self._hdr_ext = new_hdr
         else:
             raise TypeError('Passed header extension must be a dict or Hdr_Ext object')
 
         # Update the underlying Image object headers with new hdr extension
         self._save_hdr_ext()
 
@@ -393,29 +403,30 @@
         current_hdr_ext = self.hdr_ext
         current_hdr_ext.set_dim_info(dim - 4, tag, info=info, hdr=header)
         self.hdr_ext = current_hdr_ext
 
     def copy(self, remove_dim=None):
         """Return a copy of this image, optionally with a dimension removed.
 
-        :param remove_dim: dimension index (4, 5, 6) or tag. None iterates over all indices., defaults to None
+        :param remove_dim: dimension index (4, 5, 6) or tag to remove. Takes first index. Defaults to None/no removal
         :type remove_dim: str or int, optional
         :return: Copy of object
         :rtype: NIFTI_MRS
         """
         if remove_dim:
             dim = self._dim_tag_to_index(remove_dim)
             reduced_data = self[:].take(0, axis=dim)
-            new_obj = NIFTI_MRS(reduced_data, header=self.header)
-            new_obj._filename = self.filename
+            new_hdr_ext = self.hdr_ext.copy()
+            new_hdr_ext.remove_dim_info(dim - 4)
+            new_hd = utils.modify_hdr_ext(
+                new_hdr_ext,
+                self.header)
 
-            # Modify the dim information in
-            hdr_ext = self.hdr_ext.copy()
-            hdr_ext.remove_dim_info(dim - 4)
-            new_obj.hdr_ext = hdr_ext.to_dict()
+            new_obj = NIFTI_MRS(reduced_data, header=new_hd)
+            new_obj._filename = self.filename
 
             return new_obj
         else:
             return NIFTI_MRS(self[:], header=self.header)
 
     def save(self, filepath):
         """Save NIfTI-MRS to file
@@ -529,31 +540,36 @@
 
         for idx in np.ndindex(data.shape[:3]):
             yield self[idx], calc_slice_idx(idx)
 
     def dynamic_hdr_vals(self):
         """Return representations of the dynamic header values
 
-        :return: List of dicts containing labeled header parameters
+        :return: List of dicts containing labelled header parameters
         :return: List of tuples containing header values
         :return: Flattened numpy array for each generated spectrum containing header values
         """
         def list_of_dict_from_dim(dim_hdr, size):
             """Form a list of dicts where each index of the list corresponds to one element"""
             out = []
             for idx in range(size):
                 tmp_dict = {}
                 for key in dim_hdr:
+                    # Handle the non-standard case with an extra level
+                    if 'Value' in dim_hdr[key]:
+                        curr_val = dim_hdr[key]['Value']
+                    else:
+                        curr_val = dim_hdr[key]
                     # Handle the short form!
-                    if 'increment' in dim_hdr[key]:
-                        start = dim_hdr[key]['start']
-                        inc = dim_hdr[key]['increment']
+                    if 'increment' in curr_val:
+                        start = curr_val['start']
+                        inc = curr_val['increment']
                         tmp_dict.update({key: start + inc * idx})
                     else:
-                        tmp_dict.update({key: dim_hdr[key][idx]})
+                        tmp_dict.update({key: curr_val[idx]})
                 out.append(tmp_dict)
             return out
 
         def sort_output(hdr_list):
             if len(hdr_list) == 1:
                 X = np.meshgrid(hdr_list[0])
                 tvar = [x for x in X[0]]
```

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs/tools/reshape.py` & `nifti_mrs-1.0.0/src/nifti_mrs/tools/reshape.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tools for reshaping the higher dimensions of NIfTI-MRS
 
     Author: Will Clarke <william.clarke@ndcn.ox.ac.uk>
     Copyright (C) 2021 University of Oxford
 """
 from nifti_mrs.nifti_mrs import NIFTI_MRS
+from nifti_mrs import utils
 
 import numpy as np
 
 # TO DO:
 # def _reshape_hdr(dynamic_hdr, target):
 
 #     return reshaped_hdr
@@ -31,29 +32,34 @@
     :type d6: str, optional
     :param d7: Dimension tag to set dim_7, defaults to None
     :type d7: str, optional
     """
 
     shape = nmrs[:].shape[0:4]
     shape += reshape
-    nmrs_reshaped = NIFTI_MRS(np.reshape(nmrs[:], shape), header=nmrs.header)
-
-    # reshpaed_hrd = _reshape_hdr(nmrs_reshaped.dynamic_hdr_vals[2],)
+    reshaped_data = np.reshape(nmrs[:], shape)
+    new_hdr_ext = nmrs.hdr_ext.copy()
 
     # Note numerical index is N-1
     if d5:
-        nmrs_reshaped.set_dim_tag(4, d5)
-    elif nmrs_reshaped.ndim > 4\
+        new_hdr_ext.set_dim_info('5th', d5)
+    elif reshaped_data.ndim > 4\
             and nmrs.dim_tags[0] is None:
-        raise TypeError(f'An appropriate d5 dim tag must be given as ndim = {nmrs_reshaped.ndim}.')
+        raise TypeError(f'An appropriate d5 dim tag must be given as ndim = {reshaped_data.ndim}.')
     if d6:
-        nmrs_reshaped.set_dim_tag(5, d6)
-    elif nmrs_reshaped.ndim > 5\
+        new_hdr_ext.set_dim_info('6th', d6)
+    elif reshaped_data.ndim > 5\
             and nmrs.dim_tags[1] is None:
-        raise TypeError(f'An appropriate d6 dim tag must be given as ndim = {nmrs_reshaped.ndim}.')
+        raise TypeError(f'An appropriate d6 dim tag must be given as ndim = {reshaped_data.ndim}.')
     if d7:
-        nmrs_reshaped.set_dim_tag(6, d7)
-    elif nmrs_reshaped.ndim > 6\
+        new_hdr_ext.set_dim_info('7th', d7)
+    elif reshaped_data.ndim > 6\
             and nmrs.dim_tags[2] is None:
-        raise TypeError(f'An appropriate d7 dim tag must be given as ndim = {nmrs_reshaped.ndim}.')
+        raise TypeError(f'An appropriate d7 dim tag must be given as ndim = {reshaped_data.ndim}.')
+
+    new_header = utils.modify_hdr_ext(new_hdr_ext, nmrs.header)
+
+    nmrs_reshaped = NIFTI_MRS(reshaped_data, header=new_header)
+
+    # reshpaed_hrd = _reshape_hdr(nmrs_reshaped.dynamic_hdr_vals[2],)
 
     return nmrs_reshaped
```

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs/tools/split_merge.py` & `nifti_mrs-1.0.0/src/nifti_mrs/tools/split_merge.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-"""Tools for merging, splitting and reordering the dimensions of NIfTI-MRS
+"""Tools for merging and splitting the dimensions of NIfTI-MRS
 
     Author: Will Clarke <william.clarke@ndcn.ox.ac.uk>
     Copyright (C) 2021 University of Oxford
 """
 import re
 
 import numpy as np
 
 from nifti_mrs.nifti_mrs import NIFTI_MRS, NIFTIMRS_DimDoesntExist
-from nifti_mrs.tools import utils
-
-
-class NIfTI_MRSIncompatible(Exception):
-    pass
+from nifti_mrs import utils
 
 
 def split(nmrs, dimension, index_or_indicies):
     """Splits, or extracts indices from, a specified dimension of a
     NIFTI_MRS object. Output is two NIFTI_MRS objects. Header information preserved.
 
     :param nmrs: Input nifti_mrs object to split
@@ -190,24 +186,26 @@
                 return False
         return True
 
     to_concat = []
     for idx, nmrs in enumerate(array_of_nmrs):
         # Check shape
         if not check_shape(nmrs):
-            raise NIfTI_MRSIncompatible('The shape of all concatentated objects must match.'
-                                        f' The shape ({nmrs.shape}) of the {idx} object does'
-                                        f' not match that of the first ({array_of_nmrs[0].shape}).')
+            raise utils.NIfTI_MRSIncompatible(
+                'The shape of all concatenated objects must match.'
+                f' The shape ({nmrs.shape}) of the {idx} object does'
+                f' not match that of the first ({array_of_nmrs[0].shape}).')
         # Check dim tags for compatibility
         if not check_tag(nmrs):
-            raise NIfTI_MRSIncompatible('The tags of all concatentated objects must match.'
-                                        f' The tags ({nmrs.dim_tags}) of the {idx} object does'
-                                        f' not match that of the first ({array_of_nmrs[0].dim_tags}).')
+            raise utils.NIfTI_MRSIncompatible(
+                'The tags of all concatenated objects must match.'
+                f' The tags ({nmrs.dim_tags}) of the {idx} object does'
+                f' not match that of the first ({array_of_nmrs[0].dim_tags}).')
 
-        if nmrs.ndim == dim_index:
+        if nmrs.shape[-1] == 1:
             # If a squeezed singleton on the end.
             to_concat.append(np.expand_dims(nmrs[:], -1))
         else:
             to_concat.append(nmrs[:])
 
         # Merge header extension
         if idx == 0:
@@ -274,103 +272,37 @@
 
     def run_check():
         # Check all other dimension fields are consistent
         dim_n = re.compile(r'dim_[567].*')
         for key in hdr1:
             if dim_n.match(key) and key != key_str:
                 if hdr1[key] != hdr2[key]:
-                    raise NIfTI_MRSIncompatible(f'Both files must have matching dimension headers apart from the '
-                                                f'one being merged. {key} does not match.')
+                    raise utils.NIfTI_MRSIncompatible(
+                        f'Both files must have matching dimension headers apart from the '
+                        f'one being merged. {key} does not match.')
 
     if key_str in hdr1 and key_str in hdr2:
         run_check()
         # Check the subfields of the header to merge are consistent
         if not hdr1[key_str].keys() == hdr2[key_str].keys():
-            raise NIfTI_MRSIncompatible(f'Both NIfTI-MRS files must have matching dim {dimension} header fields.'
-                                        f'The first header contains {hdr1[key_str].keys()}. '
-                                        f'The second header contains {hdr2[key_str].keys()}.')
+            raise utils.NIfTI_MRSIncompatible(
+                f'Both NIfTI-MRS files must have matching dim {dimension} header fields.'
+                f'The first header contains {hdr1[key_str].keys()}. '
+                f'The second header contains {hdr2[key_str].keys()}.')
         new_h = {}
         for sub_key in hdr1[key_str]:
             new_h[sub_key] = merge_single(hdr1[key_str][sub_key], hdr2[key_str][sub_key])
 
         curr_tag = hdr1[key_str_tag]
         if key_str_info in hdr1:
             curr_info = hdr1[key_str_info]
         else:
             curr_info = None
         out_hdr.set_dim_info(dimension - 5, curr_tag, info=curr_info, hdr=new_h)
     elif key_str in hdr1 and key_str not in hdr2\
             or key_str not in hdr1 and key_str in hdr2:
         # Incompatible headers
-        raise NIfTI_MRSIncompatible(f'Both NIfTI-MRS files must have matching dim {dimension} header fields')
+        raise utils.NIfTI_MRSIncompatible(f'Both NIfTI-MRS files must have matching dim {dimension} header fields')
     elif key_str not in hdr1 and key_str not in hdr2:
         # Nothing to merge - still run check
         run_check()
     return out_hdr
-
-
-def reorder(nmrs, dim_tag_list):
-    """Reorder the higher dimensions of a NIfTI-MRS object.
-    Can force a singleton dimension with new tag.
-
-    :param nmrs: NIFTI-MRS object to reorder.
-    :type nmrs: fsl_mrs.core.nifti_mrs.NIFTI_MRS
-    :param dim_tag_list: List of dimension tags in desired order
-    :type dim_tag_list: List of str
-    :return: Reordered NIfTI-MRS object.
-    :rtype: fsl_mrs.core.nifti_mrs.NIFTI_MRS
-    """
-
-    # Check existing tags are in the list of desired tags
-    for idx, tag in enumerate(nmrs.dim_tags):
-        if tag not in dim_tag_list\
-                and tag is not None:
-            raise NIfTI_MRSIncompatible(
-                f'The existing tag ({tag}) does not appear '
-                f'in the requested tag order ({dim_tag_list}).')
-
-    # Create singleton dimensions if required
-    original_dims = nmrs.ndim
-    new_dim = sum(x is not None for x in nmrs.dim_tags) + 4
-    dims_to_add = tuple(range(original_dims, new_dim + 1))
-    data_with_singleton = np.expand_dims(nmrs[:], dims_to_add)
-
-    # Create list of source indicies
-    # Create list of destination indicies
-    # Keep track of singleton tags
-    source_indicies = []
-    dest_indicies = []
-    singleton_tags = {}
-    counter = 0
-    for idx, tag in enumerate(dim_tag_list):
-        if tag is not None:
-            if tag in nmrs.dim_tags:
-                source_indicies.append(nmrs.dim_tags.index(tag) + 4)
-            else:
-                source_indicies.append(nmrs.ndim + counter)
-                counter += 1
-                singleton_tags.update({(idx + 5): tag})
-
-            dest_indicies.append(idx + 4)
-
-    # Sort header extension dim_tags
-    dim_n = re.compile(r'dim_[567].*')
-    new_hdr_ext = nmrs.hdr_ext.copy()
-    new_hdr_ext.dimensions = data_with_singleton.ndim
-    for key in nmrs.hdr_ext:
-        if dim_n.match(key):
-            new_index = dest_indicies[source_indicies.index(int(key[4]) - 1)] + 1
-            new_ind_str = f'{new_index}th'
-            new_hdr_ext.set_dim_info(new_ind_str, nmrs.hdr_ext[key])
-
-    # For any singleton dimensions we've added
-    for dim in singleton_tags:
-        new_hdr_ext.set_dim_info(f'{dim}th', singleton_tags[dim])
-
-    new_header = nmrs.header.copy()
-    new_nmrs = NIFTI_MRS(
-        np.moveaxis(data_with_singleton, source_indicies, dest_indicies),
-        header=new_header)
-
-    # Finaly insert new header extension
-    new_nmrs.hdr_ext = new_hdr_ext
-    return new_nmrs
```

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs/tools/utils.py` & `nifti_mrs-1.0.0/src/nifti_mrs/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,37 @@
     Copyright (C) 2021 University of Oxford
 """
 
 import numpy as np
 from nibabel.nifti1 import Nifti1Extension
 
 
-def modify_hdr_ext(new_hdr_ext, hdr):
+class NIfTI_MRSIncompatible(Exception):
+    pass
+
+
+def modify_hdr_ext(new_hdr_ext, nifti_header):
     """Generate a new NIfTI header with a modified header extension.
     New header is a copy of the one passed
 
     :param new_hdr_ext: Modified header extension
-    :type new_hdr_ext: dict
-    :param hdr: NIfTI header
-    :type hdr: nibabel.nifti2.Nifti2Header
+    :type new_hdr_ext: Hdr_Ext object
+    :param nifti_header: NIfTI header
+    :type nifti_header: nibabel.nifti2.Nifti2Header
     :return: Copied header with modified hdr extension
     :rtype: nibabel.nifti2.Nifti2Header
     """
-    modded_hdr = hdr.copy()
-    json_s = new_hdr_ext.to_json()
-    extension = Nifti1Extension(44, json_s.encode('UTF-8'))
-    modded_hdr.extensions.clear()
+    modded_hdr = nifti_header.copy()
+    extension = Nifti1Extension(
+        44,
+        new_hdr_ext.to_json().encode('UTF-8'))
+
+    hdr_ext_codes = modded_hdr.extensions.get_codes()
+    if 44 in hdr_ext_codes:
+        modded_hdr.extensions.pop(hdr_ext_codes.index(44))
     modded_hdr.extensions.append(extension)
 
     return modded_hdr
 
 
 def check_type(in_format):
     """Return type of header: long (list) or short (dict)
```

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs.egg-info/PKG-INFO` & `nifti_mrs-1.0.0/src/nifti_mrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti-mrs
-Version: 0.1.7
+Version: 1.0.0
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nifti_mrs-0.1.7/src/nifti_mrs.egg-info/SOURCES.txt` & `nifti_mrs-1.0.0/src/nifti_mrs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 src/mrs_tools/constants.py
 src/nifti_mrs/__init__.py
 src/nifti_mrs/_version.py
 src/nifti_mrs/create_nmrs.py
 src/nifti_mrs/definitions.py
 src/nifti_mrs/hdr_ext.py
 src/nifti_mrs/nifti_mrs.py
+src/nifti_mrs/utils.py
 src/nifti_mrs/validator.py
 src/nifti_mrs.egg-info/PKG-INFO
 src/nifti_mrs.egg-info/SOURCES.txt
 src/nifti_mrs.egg-info/dependency_links.txt
 src/nifti_mrs.egg-info/entry_points.txt
 src/nifti_mrs.egg-info/requires.txt
 src/nifti_mrs.egg-info/top_level.txt
 src/nifti_mrs/tools/__init__.py
 src/nifti_mrs/tools/misc.py
+src/nifti_mrs/tools/reorder.py
 src/nifti_mrs/tools/reshape.py
 src/nifti_mrs/tools/split_merge.py
-src/nifti_mrs/tools/utils.py
 tests/test_create_nmrs.py
+tests/test_hdr_ext.py
 tests/test_nifti_mrs.py
 tests/test_nifti_mrs_tools_misc.py
+tests/test_nifti_mrs_tools_reorder.py
 tests/test_nifti_mrs_tools_reshape.py
 tests/test_nifti_mrs_tools_split_merge.py
 tests/test_nifti_mrs_tools_utils.py
-tests/test_script_mrs_tools.py
+tests/test_script_mrs_tools.py
+tests/test_validator.py
```

### Comparing `nifti_mrs-0.1.7/tests/test_create_nmrs.py` & `nifti_mrs-1.0.0/tests/test_create_nmrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-0.1.7/tests/test_nifti_mrs.py` & `nifti_mrs-1.0.0/tests/test_nifti_mrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from nifti_mrs.create_nmrs import gen_nifti_mrs, gen_nifti_mrs_hdr_ext
 
 # Files
 testsPath = Path(__file__).parent
 data = {'unprocessed': testsPath / 'test_data' / 'metab_raw.nii.gz'}
 
 
-def test_nifti_mrs():
+def test_nifti_mrs_class():
     obj = NIFTI_MRS(data['unprocessed'])
 
     assert obj.nifti_mrs_version == '0.2'
     assert obj.shape == (1, 1, 1, 4096, 4, 16)
     assert obj.ndim == 6
     assert obj.dwelltime == 8.33e-05
     assert obj.nucleus == ['1H']
@@ -30,15 +30,16 @@
     assert obj.bandwidth == 1 / obj.dwelltime
     assert obj.dim_tags == ['DIM_COIL', 'DIM_DYN', None]
     assert obj.dim_position('DIM_DYN') == 5
 
     copy_obj = obj.copy(remove_dim='DIM_DYN')
     assert copy_obj.shape == (1, 1, 1, 4096, 4)
     assert copy_obj.dim_tags == ['DIM_COIL', None, None]
-    assert copy_obj.hdr_ext.dimensions == 5
+    assert copy_obj.hdr_ext.ndim == 5
+    assert copy_obj.ndim == 5
 
 
 def test_copy():
     obj1 = NIFTI_MRS(data['unprocessed'])
     obj2 = obj1.copy()
     obj3 = NIFTI_MRS(obj1)
 
@@ -61,17 +62,15 @@
     obj = NIFTI_MRS(data['unprocessed'])
 
     # Test dictionay like access of keys
     assert 'EchoTime' in obj.hdr_ext
     assert obj.hdr_ext['EchoTime'] == 0.011
 
     # Test direct manipulation of hdr_ext
-    obj.hdr_ext.set_user_def(
-        key='bogus',
-        value='test')
+    obj.hdr_ext.set_user_def('bogus', 'test', 'Description')
     assert 'bogus' in obj.hdr_ext
 
     # Test external manipulation
     newhdr = obj.hdr_ext
     newhdr.SpectrometerFrequency = [10.0, ]
     obj.hdr_ext = newhdr
     assert obj.spectrometer_frequency == [10.0]
@@ -159,21 +158,21 @@
 
     with pytest.raises(
             ValueError,
             match='New dim header length must be 16'):
         nmrs.set_dim_tag(
             'DIM_DYN',
             'DIM_DYN',
-            header={'my_hdr': np.arange(10).tolist()})
+            header={'EchoTime': np.arange(10).tolist()})
 
     nmrs.set_dim_tag(
         'DIM_DYN',
         'DIM_DYN',
-        header={'my_hdr': np.arange(16).tolist()})
-    assert nmrs.hdr_ext['dim_6_header'] == {'my_hdr': np.arange(16).tolist()}
+        header={'EchoTime': np.arange(16).tolist()})
+    assert nmrs.hdr_ext['dim_6_header'] == {'EchoTime': np.arange(16).tolist()}
 
 
 def test_nifti_mrs_filename():
     obj = NIFTI_MRS(data['unprocessed'])
     assert obj.filename == 'metab_raw.nii.gz'
 
     obj = gen_nifti_mrs(np.zeros((1, 1, 1, 2), dtype=complex), 0.0005, 120.0)
@@ -283,15 +282,17 @@
     hdr_ext = Hdr_Ext(128.0, '1H', dimensions=5)
     hdr_ext.set_dim_info(
         0,
         'DIM_INDIRECT_0',
         info="Incremented echo time for j-evolution",
         hdr={
             "EchoTime": np.linspace(0.03, 0.12, 10).tolist(),
-            "EchoTime2": {"start": 0.03, "increment": 0.01},
+            "EchoTime2": {
+                'Value': {"start": 0.03, "increment": 0.01},
+                'Description': "second echo time"},
             "RepetitionTime": np.linspace(1.0, 1.9, 10).tolist()})
 
     nmrs = gen_nifti_mrs_hdr_ext(
         data,
         1 / 2000.0,
         hdr_ext,
         affine=affine)
```

### Comparing `nifti_mrs-0.1.7/tests/test_nifti_mrs_tools_reshape.py` & `nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_reshape.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-0.1.7/tests/test_nifti_mrs_tools_split_merge.py` & `nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_split_merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Test the split, merge and reorder tools for NIFTI-MRS
+"""Test the split and merge tools for NIFTI-MRS
 
 Author: Will Clarke <william.clarke@ndcn.ox.ac.uk>
 Copyright (C) 2021 University of Oxford
 """
 
 from pathlib import Path
 import pytest
@@ -10,15 +10,15 @@
 import numpy as np
 
 
 from nifti_mrs.nifti_mrs import NIFTI_MRS
 from nifti_mrs.hdr_ext import Hdr_Ext
 from nifti_mrs import tools as nmrs_tools
 from nifti_mrs.create_nmrs import gen_nifti_mrs
-from nifti_mrs.tools.split_merge import NIfTI_MRSIncompatible
+from nifti_mrs.utils import NIfTI_MRSIncompatible
 
 testsPath = Path(__file__).parent
 test_data_split = testsPath / 'test_data' / 'metab_raw.nii.gz'
 test_data_merge_1 = testsPath / 'test_data' / 'wref_raw.nii.gz'
 test_data_merge_2 = testsPath / 'test_data' / 'quant_raw.nii.gz'
 test_data_other = testsPath / 'test_data' / 'ecc.nii.gz'
 
@@ -34,15 +34,15 @@
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_6': 'DIM_EDIT',
          'dim_6_info': 'edit',
          'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_7': 'DIM_USER_0',
          'dim_7_info': 'other',
-         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                           'p2': [0.1, 0.2, 0.3, 0.4]}})
 
     # Headers occuring as a list.
     hdr1, hdr2 = nmrs_tools.split_merge._split_dim_header(hdr_in, 5, 4, 1)
     assert hdr1 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
@@ -51,29 +51,29 @@
                                      'p2': [0.1, 0.2]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
     assert hdr2 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
                     'dim_5_info': 'averages',
                     'dim_5_header': {'p1': [3, 4],
                                      'p2': [0.3, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
 
     hdr1, hdr2 = nmrs_tools.split_merge._split_dim_header(hdr_in, 5, 4, [1, 3])
     assert hdr1 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
                     'dim_5_info': 'averages',
@@ -81,29 +81,29 @@
                                      'p2': [0.1, 0.3]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
     assert hdr2 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
                     'dim_5_info': 'averages',
                     'dim_5_header': {'p1': [2, 4],
                                      'p2': [0.2, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
 
     # Headers as a dict
     hdr1, hdr2 = nmrs_tools.split_merge._split_dim_header(hdr_in, 6, 4, 1)
     assert hdr1 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
@@ -112,29 +112,29 @@
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                      'p2': [0.1, 0.2]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
     assert hdr2 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
                     'dim_5_info': 'averages',
                     'dim_5_header': {'p1': [1, 2, 3, 4],
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 3, 'increment': 1},
                                      'p2': [0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
 
     hdr1, hdr2 = nmrs_tools.split_merge._split_dim_header(hdr_in, 6, 4, [1, ])
     assert hdr1 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
                     'dim_5_info': 'averages',
@@ -142,29 +142,29 @@
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': [1, 3, 4],
                                      'p2': [0.1, 0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
     assert hdr2 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
                     'dim_5_info': 'averages',
                     'dim_5_header': {'p1': [1, 2, 3, 4],
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': [2, ],
                                      'p2': [0.2, ]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2, 0.3, 0.4]}}
 
     # User defined structures
     hdr1, hdr2 = nmrs_tools.split_merge._split_dim_header(hdr_in, 7, 4, 1)
     assert hdr1 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
@@ -173,29 +173,29 @@
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.1, 0.2]}}
     assert hdr2 == {'SpectrometerFrequency': [100.0, ],
                     'ResonantNucleus': ['1H', ],
                     'dim_5': 'DIM_DYN',
                     'dim_5_info': 'averages',
                     'dim_5_header': {'p1': [1, 2, 3, 4],
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_6': 'DIM_EDIT',
                     'dim_6_info': 'edit',
                     'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                      'p2': [0.1, 0.2, 0.3, 0.4]},
                     'dim_7': 'DIM_USER_0',
                     'dim_7_info': 'other',
-                    'dim_7_header': {'p1': {'Value': {'start': 3, 'increment': 1}, 'description': 'user'},
+                    'dim_7_header': {'p1': {'Value': {'start': 3, 'increment': 1}, 'Description': 'user'},
                                      'p2': [0.3, 0.4]}}
 
 
 def test_merge_dim_header():
     """Test the ability to merge the dim_N_header fields"""
     hdr_in_1 = Hdr_Ext.from_header_ext(
         {'SpectrometerFrequency': [100.0, ],
@@ -206,30 +206,30 @@
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_6': 'DIM_EDIT',
          'dim_6_info': 'edit',
          'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_7': 'DIM_USER_0',
          'dim_7_info': 'other',
-         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                           'p2': [0.1, 0.2, 0.3, 0.4]}})
     hdr_in_2 = Hdr_Ext.from_header_ext(
         {'SpectrometerFrequency': [100.0, ],
          'ResonantNucleus': ['1H', ],
          'dim_5': 'DIM_DYN',
          'dim_5_info': 'averages',
          'dim_5_header': {'p1': [1, 2, 3],
                           'p2': [0.1, 0.2, 0.3]},
          'dim_6': 'DIM_EDIT',
          'dim_6_info': 'edit',
          'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_7': 'DIM_USER_0',
          'dim_7_info': 'other',
-         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                           'p2': [0.1, 0.2, 0.3, 0.4]}})
 
     hdr_out = nmrs_tools.split_merge._merge_dim_header(hdr_in_1, hdr_in_2, 5, 4, 3)
     assert hdr_out == {'SpectrometerFrequency': [100.0, ],
                        'ResonantNucleus': ['1H', ],
                        'dim_5': 'DIM_DYN',
                        'dim_5_info': 'averages',
@@ -237,15 +237,15 @@
                                         'p2': [0.1, 0.2, 0.3, 0.4, 0.1, 0.2, 0.3]},
                        'dim_6': 'DIM_EDIT',
                        'dim_6_info': 'edit',
                        'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                         'p2': [0.1, 0.2, 0.3, 0.4]},
                        'dim_7': 'DIM_USER_0',
                        'dim_7_info': 'other',
-                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                         'p2': [0.1, 0.2, 0.3, 0.4]}}
 
     hdr_in_2 = Hdr_Ext.from_header_ext(
         {'SpectrometerFrequency': [100.0, ],
          'ResonantNucleus': ['1H', ],
          'dim_5': 'DIM_DYN',
          'dim_5_info': 'averages',
@@ -253,30 +253,30 @@
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_6': 'DIM_EDIT',
          'dim_6_info': 'edit',
          'dim_6_header': {'p1': {'start': 5, 'increment': 1},
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_7': 'DIM_USER_0',
          'dim_7_info': 'other',
-         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+         'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                           'p2': [0.1, 0.2, 0.3, 0.4]}})
     hdr_out = nmrs_tools.split_merge._merge_dim_header(hdr_in_1, hdr_in_2, 6, 4, 4)
     assert hdr_out == {'SpectrometerFrequency': [100.0, ],
                        'ResonantNucleus': ['1H', ],
                        'dim_5': 'DIM_DYN',
                        'dim_5_info': 'averages',
                        'dim_5_header': {'p1': [1, 2, 3, 4],
                                         'p2': [0.1, 0.2, 0.3, 0.4]},
                        'dim_6': 'DIM_EDIT',
                        'dim_6_info': 'edit',
                        'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                         'p2': [0.1, 0.2, 0.3, 0.4, 0.1, 0.2, 0.3, 0.4]},
                        'dim_7': 'DIM_USER_0',
                        'dim_7_info': 'other',
-                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                         'p2': [0.1, 0.2, 0.3, 0.4]}}
 
     hdr_out = nmrs_tools.split_merge._merge_dim_header(hdr_in_2, hdr_in_1, 6, 4, 4)
     assert hdr_out == {'SpectrometerFrequency': [100.0, ],
                        'ResonantNucleus': ['1H', ],
                        'dim_5': 'DIM_DYN',
                        'dim_5_info': 'averages',
@@ -284,15 +284,15 @@
                                         'p2': [0.1, 0.2, 0.3, 0.4]},
                        'dim_6': 'DIM_EDIT',
                        'dim_6_info': 'edit',
                        'dim_6_header': {'p1': [5, 6, 7, 8, 1, 2, 3, 4],
                                         'p2': [0.1, 0.2, 0.3, 0.4, 0.1, 0.2, 0.3, 0.4]},
                        'dim_7': 'DIM_USER_0',
                        'dim_7_info': 'other',
-                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                         'p2': [0.1, 0.2, 0.3, 0.4]}}
 
     hdr_in_2 = Hdr_Ext.from_header_ext(
         {'SpectrometerFrequency': [100.0, ],
          'ResonantNucleus': ['1H', ],
          'dim_5': 'DIM_DYN',
          'dim_5_info': 'averages',
@@ -300,30 +300,30 @@
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_6': 'DIM_EDIT',
          'dim_6_info': 'edit',
          'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                           'p2': [0.1, 0.2, 0.3, 0.4]},
          'dim_7': 'DIM_USER_0',
          'dim_7_info': 'other',
-         'dim_7_header': {'p1': {'Value': {'start': 5, 'increment': 1}, 'description': 'user'},
+         'dim_7_header': {'p1': {'Value': {'start': 5, 'increment': 1}, 'Description': 'user'},
                           'p2': [0.1, 0.2, 0.3, 0.4]}})
     hdr_out = nmrs_tools.split_merge._merge_dim_header(hdr_in_1, hdr_in_2, 7, 4, 4)
     assert hdr_out == {'SpectrometerFrequency': [100.0, ],
                        'ResonantNucleus': ['1H', ],
                        'dim_5': 'DIM_DYN',
                        'dim_5_info': 'averages',
                        'dim_5_header': {'p1': [1, 2, 3, 4],
                                         'p2': [0.1, 0.2, 0.3, 0.4]},
                        'dim_6': 'DIM_EDIT',
                        'dim_6_info': 'edit',
                        'dim_6_header': {'p1': {'start': 1, 'increment': 1},
                                         'p2': [0.1, 0.2, 0.3, 0.4]},
                        'dim_7': 'DIM_USER_0',
                        'dim_7_info': 'other',
-                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'description': 'user'},
+                       'dim_7_header': {'p1': {'Value': {'start': 1, 'increment': 1}, 'Description': 'user'},
                                         'p2': [0.1, 0.2, 0.3, 0.4, 0.1, 0.2, 0.3, 0.4]}}
 
     with pytest.raises(NIfTI_MRSIncompatible) as exc_info:
         hdr_out = nmrs_tools.split_merge._merge_dim_header(hdr_in_1, hdr_in_2, 5, 4, 4)
     assert exc_info.type is NIfTI_MRSIncompatible
     assert exc_info.value.args[0] == "Both files must have matching dimension headers apart from the one being merged."\
                                      " dim_7_header does not match."
@@ -491,24 +491,24 @@
     assert exc_info.value.args[0] == "Dimension must be an int (4, 5, or 6) or string (DIM_TAG string)."
 
     # Incompatible shapes
     with pytest.raises(NIfTI_MRSIncompatible) as exc_info:
         nmrs_tools.merge((nmrs_1, nmrs_bad_shape), 'DIM_DYN')
 
     assert exc_info.type is NIfTI_MRSIncompatible
-    assert exc_info.value.args[0] == "The shape of all concatentated objects must match. "\
+    assert exc_info.value.args[0] == "The shape of all concatenated objects must match. "\
                                      "The shape ((1, 1, 1, 4096, 2, 2)) of the 1 object does "\
                                      "not match that of the first ((1, 1, 1, 4096, 4, 2))."
 
     # Incompatible tags
     with pytest.raises(NIfTI_MRSIncompatible) as exc_info:
         nmrs_tools.merge((nmrs_1, nmrs_no_tag), 'DIM_DYN')
 
     assert exc_info.type is NIfTI_MRSIncompatible
-    assert exc_info.value.args[0] == "The tags of all concatentated objects must match. "\
+    assert exc_info.value.args[0] == "The tags of all concatenated objects must match. "\
                                      "The tags (['DIM_COIL', None, None]) of the 1 object does "\
                                      "not match that of the first (['DIM_COIL', 'DIM_DYN', None])."
 
     # Functionality testing
     out = nmrs_tools.merge((nmrs_1, nmrs_2), 'DIM_DYN')
     assert out[:].shape == (1, 1, 1, 4096, 4, 4)
     assert np.allclose(out[:][:, :, :, :, :, 0:2], nmrs_1[:])
@@ -557,51 +557,14 @@
         dim_tags=['DIM_DYN', None, None])
     nhdr_2 = nhdr_1.copy()
     nhdr_1_e = nmrs_tools.reorder(nhdr_1, ['DIM_DYN', 'DIM_EDIT', None])
     nhdr_2_e = nmrs_tools.reorder(nhdr_2, ['DIM_DYN', 'DIM_EDIT', None])
 
     nhdr_1_e.set_dim_tag('DIM_DYN', 'DIM_DYN', header={'RepetitionTime': {'start': 1, 'increment': 1}})
     nhdr_2_e.set_dim_tag('DIM_DYN', 'DIM_DYN', header={'RepetitionTime': {'start': 1, 'increment': 1}})
-    nhdr_1_e.set_dim_tag('DIM_EDIT', 'DIM_EDIT', header={'OtherTime': [0.1, ]})
-    nhdr_2_e.set_dim_tag('DIM_EDIT', 'DIM_EDIT', header={'OtherTime': [0.2, ]})
+    nhdr_1_e.set_dim_tag('DIM_EDIT', 'DIM_EDIT', header={'OtherTime': {'Value': [0.1, ], 'Description': 'N/A'}})
+    nhdr_2_e.set_dim_tag('DIM_EDIT', 'DIM_EDIT', header={'OtherTime': {'Value': [0.2, ], 'Description': 'N/A'}})
 
     out = nmrs_tools.merge((nhdr_1_e, nhdr_2_e), 'DIM_EDIT')
     assert out[:].shape == (1, 1, 1, 10, 4, 2)
     assert out.hdr_ext['dim_6'] == 'DIM_EDIT'
-    assert out.hdr_ext['dim_6_header'] == {'OtherTime': [0.1, 0.2, ]}
-
-
-def test_reorder():
-    """Test the reorder functionality
-    """
-    nmrs = NIFTI_MRS(test_data_split)
-
-    # Error testing
-    # Miss existing tag
-    with pytest.raises(NIfTI_MRSIncompatible) as exc_info:
-        nmrs_tools.reorder(nmrs, ['DIM_COIL', 'DIM_EDIT'])
-
-    assert exc_info.type is NIfTI_MRSIncompatible
-    assert exc_info.value.args[0] == "The existing tag (DIM_DYN) does not appear"\
-                                     " in the requested tag order (['DIM_COIL', 'DIM_EDIT'])."
-
-    # Functionality testing
-    # Swap order of dimensions
-    out = nmrs_tools.reorder(nmrs, ['DIM_DYN', 'DIM_COIL'])
-    assert out[:].shape == (1, 1, 1, 4096, 16, 4)
-    assert np.allclose(np.swapaxes(nmrs[:], 4, 5), out[:])
-    assert out.hdr_ext['dim_5'] == 'DIM_DYN'
-    assert out.hdr_ext['dim_6'] == 'DIM_COIL'
-
-    # # Add an additional singleton at end (not reported in shape)
-    out = nmrs_tools.reorder(nmrs, ['DIM_COIL', 'DIM_DYN', 'DIM_EDIT'])
-    assert out[:].shape == (1, 1, 1, 4096, 4, 16)
-    assert out.hdr_ext['dim_5'] == 'DIM_COIL'
-    assert out.hdr_ext['dim_6'] == 'DIM_DYN'
-    assert out.hdr_ext['dim_7'] == 'DIM_EDIT'
-
-    # Add an additional singleton at 5 (not reported in shape)
-    out = nmrs_tools.reorder(nmrs, ['DIM_EDIT', 'DIM_COIL', 'DIM_DYN'])
-    assert out[:].shape == (1, 1, 1, 4096, 1, 4, 16)
-    assert out.hdr_ext['dim_5'] == 'DIM_EDIT'
-    assert out.hdr_ext['dim_6'] == 'DIM_COIL'
-    assert out.hdr_ext['dim_7'] == 'DIM_DYN'
+    assert out.hdr_ext['dim_6_header'] == {'OtherTime': {'Description': 'N/A', 'Value': [0.1, 0.2]}}
```

### Comparing `nifti_mrs-0.1.7/tests/test_nifti_mrs_tools_utils.py` & `nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """Test the miscellaneous functions for NIFTI-MRS tools
 
 Author: Will Clarke <william.clarke@ndcn.ox.ac.uk>
 Copyright (C) 2021 University of Oxford
 """
 
-import nifti_mrs.tools.utils as utils
+import nifti_mrs.utils as utils
 
 
 def test_short_to_long():
     dict_repr = utils.dim_n_header_short_to_long({'start': 0.0, 'increment': 0.1}, 3)
     assert dict_repr == [0.0, 0.1, 0.2]
 
     dict_repr = utils.dim_n_header_short_to_long([0.0, 0.1, 0.2], 3)
     assert dict_repr == [0.0, 0.1, 0.2]
 
-    dict_repr = utils.dim_n_header_short_to_long({'Value': [0.0, 0.1, 0.2], 'description': 'test'}, 3)
-    assert dict_repr == {'Value': [0.0, 0.1, 0.2], 'description': 'test'}
+    dict_repr = utils.dim_n_header_short_to_long({'Value': [0.0, 0.1, 0.2], 'Description': 'test'}, 3)
+    assert dict_repr == {'Value': [0.0, 0.1, 0.2], 'Description': 'test'}
 
-    dict_repr = utils.dim_n_header_short_to_long({'Value': {'start': 0.0, 'increment': 0.1}, 'description': 'test'}, 3)
-    assert dict_repr == {'Value': [0.0, 0.1, 0.2], 'description': 'test'}
+    dict_repr = utils.dim_n_header_short_to_long({'Value': {'start': 0.0, 'increment': 0.1}, 'Description': 'test'}, 3)
+    assert dict_repr == {'Value': [0.0, 0.1, 0.2], 'Description': 'test'}
 
 
 def test_long_to_short():
     dict_repr = utils.dim_n_header_long_to_short([0.0, 0.1, 0.2])
     assert dict_repr == {'start': 0.0, 'increment': 0.1}
 
     dict_repr = utils.dim_n_header_long_to_short({'start': 0.0, 'increment': 0.1})
     assert dict_repr == {'start': 0.0, 'increment': 0.1}
 
-    dict_repr = utils.dim_n_header_long_to_short({'Value': [0.0, 0.1, 0.2], 'description': 'test'})
-    assert dict_repr == {'Value': {'start': 0.0, 'increment': 0.1}, 'description': 'test'}
+    dict_repr = utils.dim_n_header_long_to_short({'Value': [0.0, 0.1, 0.2], 'Description': 'test'})
+    assert dict_repr == {'Value': {'start': 0.0, 'increment': 0.1}, 'Description': 'test'}
 
-    dict_repr = utils.dim_n_header_long_to_short({'Value': {'start': 0.0, 'increment': 0.1}, 'description': 'test'})
-    assert dict_repr == {'Value': {'start': 0.0, 'increment': 0.1}, 'description': 'test'}
+    dict_repr = utils.dim_n_header_long_to_short({'Value': {'start': 0.0, 'increment': 0.1}, 'Description': 'test'})
+    assert dict_repr == {'Value': {'start': 0.0, 'increment': 0.1}, 'Description': 'test'}
 
 
 def test_dict_to_list():
     list_repr = utils._dict_to_list({'start': 0.0, 'increment': 0.1}, 3)
     assert list_repr == [0.0, 0.1, 0.2]
 
     list_repr = utils._dict_to_list({'start': 0.0, 'increment': 0.1}, 1)
```

### Comparing `nifti_mrs-0.1.7/tests/test_script_mrs_tools.py` & `nifti_mrs-1.0.0/tests/test_script_mrs_tools.py`

 * *Files identical despite different names*

