# Comparing `tmp/pyMapVBVD-0.5.2.tar.gz` & `tmp/pyMapVBVD-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMapVBVD-0.5.2.tar", last modified: Tue Jan 10 11:31:51 2023, max compression
+gzip compressed data, was "pyMapVBVD-0.5.3.tar", last modified: Fri Jul  7 12:53:52 2023, max compression
```

## Comparing `pyMapVBVD-0.5.2.tar` & `pyMapVBVD-0.5.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:31:51.250309 pyMapVBVD-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-01-10 11:31:51.250309 pyMapVBVD-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:31:51.250309 pyMapVBVD-0.5.2/mapvbvd/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/mapvbvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/mapvbvd/_attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-10 11:31:51.250309 pyMapVBVD-0.5.2/mapvbvd/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/mapvbvd/mapVBVD.py
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/mapvbvd/read_twix_hdr.py
--rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/mapvbvd/twix_map_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:31:51.246309 pyMapVBVD-0.5.2/pyMapVBVD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-01-10 11:31:51.000000 pyMapVBVD-0.5.2/pyMapVBVD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-10 11:31:51.000000 pyMapVBVD-0.5.2/pyMapVBVD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 11:31:51.000000 pyMapVBVD-0.5.2/pyMapVBVD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-10 11:31:51.000000 pyMapVBVD-0.5.2/pyMapVBVD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-10 11:31:51.000000 pyMapVBVD-0.5.2/pyMapVBVD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-10 11:31:51.250309 pyMapVBVD-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:31:51.250309 pyMapVBVD-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/tests/test_slicing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/tests/test_svs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-01-10 11:31:41.000000 pyMapVBVD-0.5.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/mapvbvd/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/_attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/mapvbvd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23055 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/mapVBVD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/read_twix_hdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/twix_map_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.877327 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/versioneer.py
```

### Comparing `pyMapVBVD-0.5.2/LICENSE` & `pyMapVBVD-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.2/PKG-INFO` & `pyMapVBVD-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyMapVBVD
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python twix file reader
 Home-page: https://github.com/wtclarke/pymapvbvd
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 # pyMapVBVD
 
 ![PyPI](https://img.shields.io/pypi/v/pyMapVBVD)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyMapVBVD)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5909806.svg)](https://doi.org/10.5281/zenodo.5909806)
@@ -88,10 +89,10 @@
 ```
 
 Some of the auxiliary parts of mapVBVD remain unimplemented. Please feel free to contribute these parts! As this is a port the code is intended to resemble the original matlab code, it is not "good" python code.
 
 ## Credit where credit is due
 This code is a port of Philipp Ehses' original Matlab code. I am incredibly grateful to him for releasing this code to the MR community. There are a number of other names in the original code comments and log, these are: Felix Breuer, Wolf Blecher, Stephen Yutzy, Zhitao Li, Michael VÃlker, Jonas Bause and Chris Mirke.
 
-More recent thanks to Mo Shahdloo and Aaron Hess for edits.
+More recent thanks to Mo Shahdloo and Aaron Hess for edits, and Alex Craven for performance enhancements.
 
 This port is released under the MIT licence and no credit is sought for its use.
```

### Comparing `pyMapVBVD-0.5.2/README.md` & `pyMapVBVD-0.5.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -69,10 +69,10 @@
 ```
 
 Some of the auxiliary parts of mapVBVD remain unimplemented. Please feel free to contribute these parts! As this is a port the code is intended to resemble the original matlab code, it is not "good" python code.
 
 ## Credit where credit is due
 This code is a port of Philipp Ehses' original Matlab code. I am incredibly grateful to him for releasing this code to the MR community. There are a number of other names in the original code comments and log, these are: Felix Breuer, Wolf Blecher, Stephen Yutzy, Zhitao Li, Michael VÃlker, Jonas Bause and Chris Mirke.
 
-More recent thanks to Mo Shahdloo and Aaron Hess for edits.
+More recent thanks to Mo Shahdloo and Aaron Hess for edits, and Alex Craven for performance enhancements.
 
 This port is released under the MIT licence and no credit is sought for its use.
```

### Comparing `pyMapVBVD-0.5.2/mapvbvd/_attrdict.py` & `pyMapVBVD-0.5.3/mapvbvd/_attrdict.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.2/mapvbvd/mapVBVD.py` & `pyMapVBVD-0.5.3/mapvbvd/mapVBVD.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,26 +69,29 @@
         dmaSkip = byteMDH
 
     if print_prog:
         last_progress = 0
         t = tqdm(total=measLength, unit='B', unit_scale=True, unit_divisor=1024,
                  desc='Scan %d/%d, read all mdhs' % (scan + 1, Nscans), leave=False,
                  file=stdout)
+
     while True:
         #         Read mdh as binary (uint8) and evaluate as little as possible to know...
         #           ... where the next mdh is (ulDMALength / ushSamplesInScan & ushUsedChannels)
         #           ... whether it is only for sync (MDH_SYNCDATA)
         #           ... whether it is the last one (MDH_ACQEND)
         #         evalMDH() contains the correct and readable code for all mdh entries.
         try:
-            # read everything and cut out the mdh
-            data_u8 = np.fromfile(fid, dtype=np.uint8, count=int(ulDMALength))
-            if data_u8.size < int(ulDMALength):
+            # read only the MDH part
+            # Note, mhdStart is NEGATIVE offset relative to end of this block
+            fid.seek(int(ulDMALength) + mdhStart, 1)
+            # fid.read might be faster...
+            data_u8 = np.fromfile(fid, dtype=np.uint8, count=-mdhStart)
+            if data_u8.size < -mdhStart:
                 raise EOFError
-            data_u8 = data_u8[mdhStart:]
 
         except EOFError:
             import warnings
             warningString =\
                 '\nAn unexpected read error occurred at this byte offset:'\
                 f' {cPos} ({cPos / 1024 ** 3} GiB)\n'
             warningString += 'Will stop reading now.\n'
@@ -307,15 +310,16 @@
     # bReadImaScan = kwargs.get('bReadImaScan', True)
     # bReadNoiseScan = kwargs.get('bReadNoiseScan', True)
     # bReadPCScan = kwargs.get('bReadPCScan', True)
     # bReadRefScan = kwargs.get('bReadRefScan', True)
     # bReadRefPCScan = kwargs.get('bReadRefPCScan', True)
     # bReadRTfeedback = kwargs.get('bReadRTfeedback', True)
     # bReadPhaseStab = kwargs.get('bReadPhaseStab', True)
-    # bReadHeader = kwargs.get('bReadHeader', True)
+    bReadHeader = kwargs.get('bReadHeader', True)
+    bReadMDH = kwargs.get('bReadMDH', True)
 
     # ignoreROoffcenter = kwargs.get('ignoreROoffcenter', False)
 
     # TODO: handle filename input variations
     fid = open(filename, 'rb')
 
     fid.seek(0, 2)
@@ -364,182 +368,187 @@
     for s in range(NScans):
         cPos = measOffset[s]
         fid.seek(cPos, 0)
         hdr_len = np.fromfile(fid, dtype=np.uint32, count=1, offset=0)
 
         currTwixObj = AttrDict()
         currTwixObjHdr = twix_hdr()
-        # rstraj = 0
-        # read header
-        currTwixObjHdr, rstraj = read_twix_hdr(fid, currTwixObjHdr)
-        currTwixObj.update({'hdr': currTwixObjHdr})
-
-        # declare data objects:
-        def mytmo(dtype):
-            return twix_map_obj(dtype, filename, version, rstraj, **kwargs)
-        currTwixObj.update({'image': mytmo('image')})
-        currTwixObj.update({'noise': mytmo('noise')})
-        currTwixObj.update({'phasecor': mytmo('phasecor')})
-        currTwixObj.update({'phasestab': mytmo('phasestab')})
-        currTwixObj.update({'phasestab_ref0': mytmo('phasestab_ref0')})
-        currTwixObj.update({'phasestab_ref1': mytmo('phasestab_ref1')})
-        currTwixObj.update({'refscan': mytmo('refscan')})
-        currTwixObj.update({'refscanPC': mytmo('refscanPC')})
-        currTwixObj.update({'refscan_phasestab': mytmo('refscan_phasestab')})
-        currTwixObj.update({'refscan_phasestab_ref0': mytmo('refscan_phasestab_ref0')})
-        currTwixObj.update({'refscan_phasestab_ref1': mytmo('refscan_phasestab_ref1')})
-        currTwixObj.update({'rtfeedback': mytmo('rtfeedback')})
-        currTwixObj.update({'vop': mytmo('vop')})
-
-        # TODO: print reader version information
-        # if s == 0:
-        #     # print(f'Reader version: {currTwixObj['image'].readerVersion})
-        #     print('UTC: TODO')
-
-        # jump to first mdh
-        cPos += hdr_len
-        # print(cPos[0])
-        fid.seek(cPos[0], 0)
-
-        # print(f'Scan {s + 1}/{NScans}, read all mdhs:')
-
-        mdh_blob, filePos, isEOF = loop_mdh_read(fid, version, NScans, s, measOffset[s],
-                                                 measLength[s], print_prog=not quiet)  # uint8; size: [ byteMDH  Nmeas ]
-
-        cPos = filePos[-1]
-        # filePos = filePos[:-1]
-
-        # get mdhs and masks for each scan, no matter if noise, image, RTfeedback etc:
-        [mdh, mask] = evalMDH(mdh_blob, version)
-
-        # Assign mdhs to their respective scans and parse it in the correct twix objects.
-
-        # MDH_IMASCAN
-        isCurrScan = mask.MDH_IMASCAN.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.image.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('image', None)
-
-        # MDH_NOISEADJSCAN
-        isCurrScan = mask.MDH_NOISEADJSCAN.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.noise.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('noise', None)
-
-        # MDH_PATREFSCAN refscan
-        isCurrScan = \
-            (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)\
-            & ~(mask.MDH_PHASCOR
-                | mask.MDH_PHASESTABSCAN
-                | mask.MDH_REFPHASESTABSCAN
-                | mask.MDH_RTFEEDBACK
-                | mask.MDH_HPFEEDBACK)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.refscan.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('refscan', None)
-
-        # MDH_RTFEEDBACK
-        isCurrScan = (mask.MDH_RTFEEDBACK | mask.MDH_HPFEEDBACK) & ~mask.MDH_VOP
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.rtfeedback.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('rtfeedback', None)
-
-        # VOP
-        isCurrScan = (mask.MDH_RTFEEDBACK & mask.MDH_VOP)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.vop.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('vop', None)
-
-        # MDH_PHASCOR
-        isCurrScan = mask.MDH_PHASCOR & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.phasecor.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('phasecor', None)
-
-        # refscanPC
-        isCurrScan = mask.MDH_PHASCOR & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.refscanPC.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('refscanPC', None)
 
-        # phasestab MDH_PHASESTABSCAN
-        isCurrScan = (mask.MDH_PHASESTABSCAN & ~mask.MDH_REFPHASESTABSCAN)\
-            & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.phasestab.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('phasestab', None)
-
-        # refscanPS MDH_PHASESTABSCAN
-        isCurrScan = (mask.MDH_PHASESTABSCAN & ~mask.MDH_REFPHASESTABSCAN)\
-            & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.refscan_phasestab.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('refscan_phasestab', None)
-
-        # phasestabRef0 MDH_PHASESTABSCAN
-        isCurrScan = (mask.MDH_REFPHASESTABSCAN & ~mask.MDH_PHASESTABSCAN)\
-            & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.phasestab_ref0.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('phasestab_ref0', None)
-
-        # refscanPSRef0 MDH_PHASESTABSCAN
-        isCurrScan = (mask.MDH_REFPHASESTABSCAN & ~mask.MDH_PHASESTABSCAN)\
-            & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.refscan_phasestab_ref0.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('refscan_phasestab_ref0', None)
-
-        # phasestabRef1 MDH_PHASESTABSCAN
-        isCurrScan = (mask.MDH_REFPHASESTABSCAN & mask.MDH_PHASESTABSCAN)\
-            & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.phasestab_ref1.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('phasestab_ref1', None)
-
-        # refscanPSRef1 MDH_PHASESTABSCAN
-        isCurrScan = (mask.MDH_REFPHASESTABSCAN & mask.MDH_PHASESTABSCAN)\
-            & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
-        isCurrScan = isCurrScan.astype(bool)
-        if isCurrScan.any():
-            currTwixObj.refscan_phasestab_ref1.readMDH(mdh, filePos, isCurrScan)
-        else:
-            currTwixObj.pop('refscan_phasestab_ref1', None)
-
-        if isEOF:
-            # recover from read error
-            for keys in currTwixObj:
-                if keys != 'hdr':
-                    currTwixObj[keys].tryAndFixLastMdh()
-        else:
-            for keys in currTwixObj:
-                if keys != 'hdr':
-                    currTwixObj[keys].clean()
+        if bReadHeader:
+            currTwixObjHdr, rstraj = read_twix_hdr(fid, currTwixObjHdr)
+            currTwixObj.update({'hdr': currTwixObjHdr})
+        else:
+            rstraj = 0
+
+        if bReadMDH:
+
+            # declare data objects:
+            def mytmo(dtype):
+                return twix_map_obj(dtype, filename, version, rstraj, **kwargs)
+            currTwixObj.update({'image': mytmo('image')})
+            currTwixObj.update({'noise': mytmo('noise')})
+            currTwixObj.update({'phasecor': mytmo('phasecor')})
+            currTwixObj.update({'phasestab': mytmo('phasestab')})
+            currTwixObj.update({'phasestab_ref0': mytmo('phasestab_ref0')})
+            currTwixObj.update({'phasestab_ref1': mytmo('phasestab_ref1')})
+            currTwixObj.update({'refscan': mytmo('refscan')})
+            currTwixObj.update({'refscanPC': mytmo('refscanPC')})
+            currTwixObj.update({'refscan_phasestab': mytmo('refscan_phasestab')})
+            currTwixObj.update({'refscan_phasestab_ref0': mytmo('refscan_phasestab_ref0')})
+            currTwixObj.update({'refscan_phasestab_ref1': mytmo('refscan_phasestab_ref1')})
+            currTwixObj.update({'rtfeedback': mytmo('rtfeedback')})
+            currTwixObj.update({'vop': mytmo('vop')})
+
+            # TODO: print reader version information
+            # if s == 0:
+            #     # print(f'Reader version: {currTwixObj['image'].readerVersion})
+            #     print('UTC: TODO')
+
+            # jump to first mdh
+            cPos += hdr_len
+            # print(cPos[0])
+            fid.seek(cPos[0], 0)
+
+            # print(f'Scan {s + 1}/{NScans}, read all mdhs:')
+
+            mdh_blob, filePos, isEOF = loop_mdh_read(fid, version, NScans, s, measOffset[s],
+                                                     measLength[s], print_prog=not quiet)
+            # uint8; size: [ byteMDH  Nmeas ]
+
+            cPos = filePos[-1]
+            # filePos = filePos[:-1]
+
+            # get mdhs and masks for each scan, no matter if noise, image, RTfeedback etc:
+            [mdh, mask] = evalMDH(mdh_blob, version)
+
+            # Assign mdhs to their respective scans and parse it in the correct twix objects.
+
+            # MDH_IMASCAN
+            isCurrScan = mask.MDH_IMASCAN.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.image.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('image', None)
+
+            # MDH_NOISEADJSCAN
+            isCurrScan = mask.MDH_NOISEADJSCAN.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.noise.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('noise', None)
+
+            # MDH_PATREFSCAN refscan
+            isCurrScan = \
+                (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)\
+                & ~(mask.MDH_PHASCOR
+                    | mask.MDH_PHASESTABSCAN
+                    | mask.MDH_REFPHASESTABSCAN
+                    | mask.MDH_RTFEEDBACK
+                    | mask.MDH_HPFEEDBACK)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.refscan.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('refscan', None)
+
+            # MDH_RTFEEDBACK
+            isCurrScan = (mask.MDH_RTFEEDBACK | mask.MDH_HPFEEDBACK) & ~mask.MDH_VOP
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.rtfeedback.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('rtfeedback', None)
+
+            # VOP
+            isCurrScan = (mask.MDH_RTFEEDBACK & mask.MDH_VOP)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.vop.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('vop', None)
+
+            # MDH_PHASCOR
+            isCurrScan = mask.MDH_PHASCOR & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.phasecor.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('phasecor', None)
+
+            # refscanPC
+            isCurrScan = mask.MDH_PHASCOR & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.refscanPC.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('refscanPC', None)
+
+            # phasestab MDH_PHASESTABSCAN
+            isCurrScan = (mask.MDH_PHASESTABSCAN & ~mask.MDH_REFPHASESTABSCAN)\
+                & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.phasestab.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('phasestab', None)
+
+            # refscanPS MDH_PHASESTABSCAN
+            isCurrScan = (mask.MDH_PHASESTABSCAN & ~mask.MDH_REFPHASESTABSCAN)\
+                & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.refscan_phasestab.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('refscan_phasestab', None)
+
+            # phasestabRef0 MDH_PHASESTABSCAN
+            isCurrScan = (mask.MDH_REFPHASESTABSCAN & ~mask.MDH_PHASESTABSCAN)\
+                & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.phasestab_ref0.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('phasestab_ref0', None)
+
+            # refscanPSRef0 MDH_PHASESTABSCAN
+            isCurrScan = (mask.MDH_REFPHASESTABSCAN & ~mask.MDH_PHASESTABSCAN)\
+                & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.refscan_phasestab_ref0.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('refscan_phasestab_ref0', None)
+
+            # phasestabRef1 MDH_PHASESTABSCAN
+            isCurrScan = (mask.MDH_REFPHASESTABSCAN & mask.MDH_PHASESTABSCAN)\
+                & (~mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.phasestab_ref1.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('phasestab_ref1', None)
+
+            # refscanPSRef1 MDH_PHASESTABSCAN
+            isCurrScan = (mask.MDH_REFPHASESTABSCAN & mask.MDH_PHASESTABSCAN)\
+                & (mask.MDH_PATREFSCAN | mask.MDH_PATREFANDIMASCAN)
+            isCurrScan = isCurrScan.astype(bool)
+            if isCurrScan.any():
+                currTwixObj.refscan_phasestab_ref1.readMDH(mdh, filePos, isCurrScan)
+            else:
+                currTwixObj.pop('refscan_phasestab_ref1', None)
+
+            if isEOF:
+                # recover from read error
+                for keys in currTwixObj:
+                    if keys != 'hdr':
+                        currTwixObj[keys].tryAndFixLastMdh()
+            else:
+                for keys in currTwixObj:
+                    if keys != 'hdr':
+                        currTwixObj[keys].clean()
 
         twix_obj.append(myAttrDict(currTwixObj))
 
     fid.close()
 
     if len(twix_obj) == 1:
         twix_obj = twix_obj[0]
```

### Comparing `pyMapVBVD-0.5.2/mapvbvd/read_twix_hdr.py` & `pyMapVBVD-0.5.3/mapvbvd/read_twix_hdr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 import numpy as np
 from scipy.integrate import cumtrapz
-from itertools import chain
 
 from mapvbvd._attrdict import AttrDict
 
 
 class twix_hdr(AttrDict):
     def __init__(self, *args):
         super().__init__(*args)
@@ -73,64 +72,70 @@
 
         return out
 
 
 def parse_ascconv(buffer):
     # print(buffer)
     vararray = re.finditer(r'(?P<name>\S*)\s*=\s*(?P<value>\S*)\n', buffer)
+
+    # for splitting array name and index (if present)
+    re_array_name_index = re.compile(r'(?P<name>\w+)(?:\[(?P<ix>[0-9]+)\])?')
+
     # print(vararray)
     mrprot = AttrDict()
     for v in vararray:
         try:
             value = float(v.group('value'))
         except ValueError:
             value = v.group('value')
 
         # now split array name and index (if present)
-        vvarray = re.finditer(r'(?P<name>\w+)(\[(?P<ix>[0-9]+)\])?', v.group('name'))
-
-        currKey = []
-        for vv in vvarray:
-            # print(vv.group('name'))
-            currKey.append(vv.group('name'))
-            if vv.group('ix') is not None:
-                # print(vv.group('ix'))
-                currKey.append(vv.group('ix'))
+        vvarray = re_array_name_index.findall(v.group('name'))
+        # for each match, take all non-empty components to form the final key
+        currKey = (x for y in vvarray for x in y if x)
 
         mrprot.update({tuple(currKey): value})
 
     return mrprot
 
 
 def parse_xprot(buffer):
     xprot = {}
-    tokens = re.finditer(r'<Param(?:Bool|Long|String)\."(\w+)">\s*{([^}]*)', buffer)
-    tokensDouble = re.finditer(r'<ParamDouble\."(\w+)">\s*{\s*(<Precision>\s*[0-9]*)?\s*([^}]*)', buffer)
-    alltokens = chain(tokens, tokensDouble)
+
+    # captured groups are 1: name, 2: value.
+    # param type isn't that useful, since integer values are often stored in string types
+    alltokens = re.finditer(
+        r'<Param(?:Bool|Long|String|Double)\."(\w+)">\s*{\s*(?:<Precision>\s*[0-9]*)?\s*([^}]*)',
+        buffer
+    )
 
     for t in alltokens:
-        # print(t.group(1))
-        # print(t.group(2))
         name = t.group(1)
+        value = t.group(2).strip()
 
-        value = re.sub(r'("*)|( *<\w*> *[^\n]*)', '', t.groups()[-1])
-        # value = re.sub(r'\s*',' ',value)
-        # for some bonkers reason this inserts whitespace between all the letters!
-        # Just look for other whitespace that \s usually does.
-        value = re.sub(r'[\t\n\r\f\v]*', '', value.strip())
-        try:
-            value = float(value)
-        except ValueError:
-            pass
+        # clean up the obtained values, removing quotes, nested tags and repeated whitespace.
+        # Skipped for really lengthy values: most likely nested ASCCONV blocks which aren't handled meaningfully anyway
+        if len(value) < 5000:
+            value = parse_xprot.re_quotes_and_nested_tags.sub('', value).strip()
+            value = parse_xprot.re_repeated_whitespace.sub(' ', value)
+
+            try:
+                value = float(value)
+            except ValueError:
+                pass
 
         xprot.update({name: value})
 
     return xprot
 
 
+parse_xprot.re_repeated_whitespace = re.compile(r'\s+')
+parse_xprot.re_quotes_and_nested_tags = re.compile(r'("+)|( *<\w*> *[^\n]*)')
+
+
 def parse_buffer(buffer):
     reASCCONV = re.compile(r'### ASCCONV BEGIN[^\n]*\n(.*)\s### ASCCONV END ###', re.DOTALL)
     # print(f'buffer = {buffer[0:10]}')
     # import pdb; pdb.set_trace()
 
     ascconv = reASCCONV.search(buffer)
     # print(f'ascconv = {ascconv}')
@@ -159,22 +164,50 @@
     for _ in range(nbuffers[0]):
         tmpBuff = np.fromfile(fid, dtype=np.uint8, count=10)
         bufname = ''.join([chr(item) for item in tmpBuff])
         bufname = re.match(r'^\w*', bufname).group(0)
 
         fid.seek(len(bufname) - 9, 1)
         buflen = np.fromfile(fid, dtype=np.uint32, count=1)
-        tmpBuff = np.fromfile(fid, dtype=np.uint8, count=buflen[0])
-        buffer = ''.join([chr(item) for item in tmpBuff])
-        buffer = re.sub(r'\n\s*\n', '', buffer)
+
+        # read entire buffer, as series of bytes
+        buffer = fid.read(buflen[0])
+
+        if len(bufname) == 0:
+            warningString =\
+                '\nEmpty buffer name at file offset %d: file may be corrupt or unsupported\n' % (
+                    fid.tell(),
+                )
+        elif len(buffer) < buflen[0]:
+            warningString =\
+                '\nRead only %d of expected %d bytes (offset %d); file may be corrupt or unsupported\n' % (
+                    len(buffer),
+                    buflen[0],
+                    fid.tell()
+                )
+        else:
+            warningString = None
+
+        if warningString:
+            # warning only, in keeping with mapVBVD behaviour; could alternatively raise EOFError
+            import warnings
+            warningString += 'Header read stopped prematurely.\n'
+            warnings.warn(warningString)
+            break
+
+        buffer = buffer.decode('latin-1', errors='ignore')
+
+        # trim whitespace and drop blank lines
+        buffer = '\n'.join([l2 for l2 in [line.strip() for line in buffer.split('\n')] if l2])
+
         prot.update({bufname: parse_buffer(buffer)})
 
     rstraj = None
     # read gridding info
-    if 'alRegridMode' in prot.Meas:
+    if hasattr(prot, 'Meas') and 'alRegridMode' in prot.Meas:
         regrid_mode = int(prot.Meas.alRegridMode.split(' ')[0])
         if regrid_mode > 1:
             ncol = int(prot.Meas.alRegridDestSamples.split(' ')[0])
             dwelltime = float(prot.Meas.aflRegridADCDuration.split(' ')[0]) / ncol
             gr_adc = np.zeros(ncol, dtype=np.single)
             start = float(prot.Meas.alRegridDelaySamplesTime.split(' ')[0])
             time_adc = start + dwelltime * (np.array(range(ncol)) + 0.5)
```

### Comparing `pyMapVBVD-0.5.2/mapvbvd/twix_map_obj.py` & `pyMapVBVD-0.5.3/mapvbvd/twix_map_obj.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.2/pyMapVBVD.egg-info/PKG-INFO` & `pyMapVBVD-0.5.3/pyMapVBVD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyMapVBVD
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python twix file reader
 Home-page: https://github.com/wtclarke/pymapvbvd
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 # pyMapVBVD
 
 ![PyPI](https://img.shields.io/pypi/v/pyMapVBVD)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyMapVBVD)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5909806.svg)](https://doi.org/10.5281/zenodo.5909806)
@@ -88,10 +89,10 @@
 ```
 
 Some of the auxiliary parts of mapVBVD remain unimplemented. Please feel free to contribute these parts! As this is a port the code is intended to resemble the original matlab code, it is not "good" python code.
 
 ## Credit where credit is due
 This code is a port of Philipp Ehses' original Matlab code. I am incredibly grateful to him for releasing this code to the MR community. There are a number of other names in the original code comments and log, these are: Felix Breuer, Wolf Blecher, Stephen Yutzy, Zhitao Li, Michael VÃlker, Jonas Bause and Chris Mirke.
 
-More recent thanks to Mo Shahdloo and Aaron Hess for edits.
+More recent thanks to Mo Shahdloo and Aaron Hess for edits, and Alex Craven for performance enhancements.
 
 This port is released under the MIT licence and no credit is sought for its use.
```

### Comparing `pyMapVBVD-0.5.2/setup.py` & `pyMapVBVD-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     author='Will Clarke',
     author_email='william.clarke@ndcn.ox.ac.uk',
     url='https://github.com/wtclarke/pymapvbvd',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=install_requires,
+    extras_require={"tests": ['pytest', ]},
     license_file='LICENSE',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `pyMapVBVD-0.5.2/tests/test_flags.py` & `pyMapVBVD-0.5.3/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.2/tests/test_read.py` & `pyMapVBVD-0.5.3/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.2/tests/test_slicing.py` & `pyMapVBVD-0.5.3/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.2/tests/test_svs.py` & `pyMapVBVD-0.5.3/tests/test_svs.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.2/versioneer.py` & `pyMapVBVD-0.5.3/versioneer.py`

 * *Files identical despite different names*

