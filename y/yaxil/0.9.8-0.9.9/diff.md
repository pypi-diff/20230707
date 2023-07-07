# Comparing `tmp/yaxil-0.9.8-py2.py3-none-any.whl.zip` & `tmp/yaxil-0.9.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 30656 bytes, number of entries: 19
+Zip file size: 30797 bytes, number of entries: 19
 -rw-r--r--  2.0 unx    46800 b- defN 23-Jul-06 18:06 yaxil/__init__.py
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-06 19:03 yaxil/__version__.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-07 17:18 yaxil/__version__.py
 -rw-r--r--  2.0 unx       84 b- defN 23-Jul-06 18:06 yaxil/assessments/__init__.py
--rw-r--r--  2.0 unx    25510 b- defN 23-Jul-06 19:02 yaxil/assessments/neuroinfo/__init__.py
+-rw-r--r--  2.0 unx    24717 b- defN 23-Jul-07 17:09 yaxil/assessments/neuroinfo/__init__.py
 -rw-r--r--  2.0 unx     7117 b- defN 23-Jul-06 18:06 yaxil/assessments/neuroinfo/legacy/__init__.py
--rw-r--r--  2.0 unx      699 b- defN 23-Jul-06 18:06 yaxil/assessments/neuroinfo/session/__init__.py
+-rw-r--r--  2.0 unx      798 b- defN 23-Jul-07 17:08 yaxil/assessments/neuroinfo/session/__init__.py
 -rw-r--r--  2.0 unx    16280 b- defN 23-Jul-06 18:06 yaxil/bids/__init__.py
 -rw-r--r--  2.0 unx     2805 b- defN 23-Jul-06 18:06 yaxil/commons/__init__.py
 -rw-r--r--  2.0 unx     1656 b- defN 23-Jul-06 18:06 yaxil/dicom/__init__.py
 -rw-r--r--  2.0 unx      625 b- defN 23-Jul-06 18:06 yaxil/exceptions/__init__.py
 -rw-r--r--  2.0 unx      783 b- defN 23-Jul-06 18:06 yaxil/functools/__init__.py
 -rw-r--r--  2.0 unx     1477 b- defN 23-Jul-06 18:06 yaxil/session/__init__.py
--rwxr-xr-x  2.0 unx     9426 b- defN 23-Jul-06 19:03 yaxil-0.9.8.data/scripts/ArcGet.py
--rwxr-xr-x  2.0 unx     4114 b- defN 23-Jul-06 19:03 yaxil-0.9.8.data/scripts/xnat_auth
--rw-r--r--  2.0 unx     1541 b- defN 23-Jul-06 19:03 yaxil-0.9.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 23-Jul-06 19:03 yaxil-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-06 19:03 yaxil-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-06 19:03 yaxil-0.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1586 b- defN 23-Jul-06 19:03 yaxil-0.9.8.dist-info/RECORD
-19 files, 121238 bytes uncompressed, 28060 bytes compressed:  76.9%
+-rwxr-xr-x  2.0 unx     9426 b- defN 23-Jul-07 17:20 yaxil-0.9.9.data/scripts/ArcGet.py
+-rwxr-xr-x  2.0 unx     4114 b- defN 23-Jul-07 17:20 yaxil-0.9.9.data/scripts/xnat_auth
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jul-07 17:20 yaxil-0.9.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      414 b- defN 23-Jul-07 17:20 yaxil-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-07 17:20 yaxil-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-07 17:20 yaxil-0.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1586 b- defN 23-Jul-07 17:20 yaxil-0.9.9.dist-info/RECORD
+19 files, 120571 bytes uncompressed, 28201 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -30,29 +30,29 @@
 
 Filename: yaxil/functools/__init__.py
 Comment: 
 
 Filename: yaxil/session/__init__.py
 Comment: 
 
-Filename: yaxil-0.9.8.data/scripts/ArcGet.py
+Filename: yaxil-0.9.9.data/scripts/ArcGet.py
 Comment: 
 
-Filename: yaxil-0.9.8.data/scripts/xnat_auth
+Filename: yaxil-0.9.9.data/scripts/xnat_auth
 Comment: 
 
-Filename: yaxil-0.9.8.dist-info/LICENSE
+Filename: yaxil-0.9.9.dist-info/LICENSE
 Comment: 
 
-Filename: yaxil-0.9.8.dist-info/METADATA
+Filename: yaxil-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: yaxil-0.9.8.dist-info/WHEEL
+Filename: yaxil-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: yaxil-0.9.8.dist-info/top_level.txt
+Filename: yaxil-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: yaxil-0.9.8.dist-info/RECORD
+Filename: yaxil-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yaxil/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'yaxil'
 __description__ = 'Yet another XNAT interface libary'
 __url__ = 'https://github.com/harvard-nrg/yaxil'
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## yaxil/assessments/neuroinfo/__init__.py

```diff
@@ -1,11 +1,74 @@
 import yaxil
+from jsonpath_ng import jsonpath
+from jsonpath_ng.ext import parse
 from contextlib import contextmanager
 from yaxil.assessments.neuroinfo.session import Session
 
+def dwiqc(auth, label=None, scan_ids=None, project=None, aid=None):
+    '''
+    Get DwiQC data as a sequence of dictionaries.
+
+    Example:
+        >>> import json
+        >>> import yaxil.assessments.neuroinfo as neuroinfo
+        >>> auth = yaxil.auth('doctest')
+        >>> for qc in neuroinfo.dwiqc(auth, 'TestSession01'):
+        ...   print(json.dumps(qc, indent=2))
+        {
+          "id": "TestSession01_DWI_30_DWIQC",
+          ...
+        }
+
+    :param auth: XNAT authentication object
+    :type auth: :mod:`yaxil.XnatAuth`
+    :param label: XNAT MR Session label
+    :type label: str
+    :param scan_ids: Scan numbers to include
+    :type scan_ids: list
+    :param project: XNAT MR Session project
+    :type project: str
+    :param aid: XNAT MR Session Accession ID
+    :type aid: str
+    :returns: Generator of DwiQC data dictionaries
+    :rtype: :mod:`dict`
+    '''
+    scan_ids = map(str, scan_ids)
+    if not aid:
+        aid = yaxil.accession(auth, label, project)
+    experiment_details = yaxil.__experiment_details(auth, aid)
+    path = f'/data/experiments/{aid}/assessors'
+    params = {
+        'xsiType': 'neuroinfo:dwiqc',
+        'columns': 'label'
+    }
+    if project:
+        params['project'] = project
+    _,result = yaxil._get(auth, path, 'json', autobox=True, params=params)
+    dwiqc_ids = [ x['label'] for x in result['ResultSet']['Result'] ]
+    for dwiqc_id in dwiqc_ids:
+        path = f'/data/experiments/{dwiqc_id}'
+        params = dict()
+        if project:
+            params['project'] = project
+        _,result = yaxil._get(auth, path, 'json', autobox=True, params=params)
+        expr = parse('items[0].data_fields')
+        data = expr.find(result)[0].value
+        if scan_ids and data['dwi_scan_id'] not in scan_ids:
+            continue
+        expr = parse("$.items[0].children[?(@.field == 'eddy_quad/shell_cnr/cnr')].items[*].data_fields")
+        shell_cnr = [ x.value for x in expr.find(result) ]
+        for x in shell_cnr:
+            del x['neuroinfo_dwiqc_cnr_id'] # internal XNAT bookkeeping material?
+        data['shell_cnr'] = shell_cnr
+        data.update(experiment_details)
+        files = __files(auth, dwiqc_id)
+        data['files'] = files
+        yield data
+
 @contextmanager
 def session(auth):
     '''
     Create a session context to avoid explicitly passing authentication to
     every function.
 
     Example:
@@ -457,91 +520,14 @@
     'neuroinfo:anatqc/manual/spike': 'manual_spike',
     'neuroinfo:anatqc/manual/art_brain': 'manual_art_brain',
     'neuroinfo:anatqc/manual/art_out': 'manual_art_out',
     'neuroinfo:anatqc/manual/inhom': 'manual_inhom',
     'neuroinfo:anatqc/manual/overall': 'manual_overall'
 }
 
-def dwiqc(auth, label=None, scan_ids=None, project=None, aid=None):
-    '''
-    Get DwiQC data as a sequence of dictionaries.
-
-    Example:
-        >>> import json
-        >>> import yaxil.assessments.neuroinfo as neuroinfo
-        >>> auth = yaxil.auth('doctest')
-        >>> for qc in neuroinfo.dwiqc(auth, 'TestSession01'):
-        ...   print(json.dumps(qc, indent=2))
-        {
-          "id": "TestSession01_DWI_30_DWIQC",
-          ...
-        }
-
-    :param auth: XNAT authentication object
-    :type auth: :mod:`yaxil.XnatAuth`
-    :param label: XNAT MR Session label
-    :type label: str
-    :param scan_ids: Scan numbers to include
-    :type scan_ids: list
-    :param project: XNAT MR Session project
-    :type project: str
-    :param aid: XNAT MR Session Accession ID
-    :type aid: str
-    :returns: Generator of DwiQC data dictionaries
-    :rtype: :mod:`dict`
-    '''
-
-    if not aid:
-        aid = yaxil.accession(auth, label, project)
-    experiment_details = yaxil.__experiment_details(auth, aid)
-    path = '/data/experiments'
-    params = {
-        'xsiType': 'neuroinfo:dwiqc',
-        'columns': ','.join(dwiqc.columns.keys())
-    }
-    if project:
-        params['project'] = project
-    params['xnat:mrSessionData/ID'] = aid
-    _,result = yaxil._get(auth, path, 'json', autobox=True, params=params)
-    for result in result['ResultSet']['Result']:
-        if scan_ids == None or result['neuroinfo:dwiqc/dwi_scan_id'] in scan_ids:
-            data = dict()
-            for k,v in iter(dwiqc.columns.items()):
-                data[v] = result[k]
-            files = __files(auth, result['neuroinfo:dwiqc/id'])
-            data.update(experiment_details)
-            data['files'] = files
-            yield data
-dwiqc.columns = {
-    'neuroinfo:dwiqc/id': 'ID',
-    'neuroinfo:dwiqc/id': 'id',
-    'neuroinfo:dwiqc/date': 'date',
-    'neuroinfo:dwiqc/time': 'time',
-    'neuroinfo:dwiqc/imagesession_id': 'session_id',
-    'neuroinfo:dwiqc/dwi_scan_id': 'dwi_scan_id',
-    'neuroinfo:dwiqc/ap_fmap_scan_id': 'ap_fmap_scan_id',
-    'neuroinfo:dwiqc/pa_fmap_scan_id': 'pa_fmap_scan_id',    
-    'neuroinfo:dwiqc/session_label': 'session_label',
-    'neuroinfo:dwiqc/eddy_quad/average_abs_motion_mm': 'average_abs_motion_mm',
-    'neuroinfo:dwiqc/eddy_quad/average_rel_motion_mm': 'average_rel_motion_mm',
-    'neuroinfo:dwiqc/eddy_quad/average_x_translation_mm': 'average_x_translation_mm',
-    'neuroinfo:dwiqc/eddy_quad/average_y_translation_mm': 'average_y_translation_mm',
-    'neuroinfo:dwiqc/eddy_quad/average_z_translation_mm': 'average_z_translation_mm',
-    'neuroinfo:dwiqc/eddy_quad/average_snr_b0': 'average_snr_b0',
-    'neuroinfo:dwiqc/manual/wrap': 'manual_wrap',
-    'neuroinfo:dwiqc/manual/motion': 'manual_motion',
-    'neuroinfo:dwiqc/manual/cover': 'manual_cover',
-    'neuroinfo:dwiqc/manual/ghost_brain': 'manual_ghost_brain',
-    'neuroinfo:dwiqc/manual/ghost_out': 'manual_ghost_out',
-    'neuroinfo:dwiqc/manual/spike': 'manual_spike',
-    'neuroinfo:dwiqc/manual/inhom': 'manual_inhom',
-    'neuroinfo:dwiqc/manual/overall': 'manual_overall'
-
-}
-
 def __files(auth, aid):
     path = f'/data/experiments/{aid}/files'
     _,result = yaxil._get(auth, path, 'json', autobox=True)
     files = dict()
     for result in result['ResultSet']['Result']:
         name = result['URI'].split('/')[-2]
         files[name] = result
```

## yaxil/assessments/neuroinfo/session/__init__.py

```diff
@@ -12,14 +12,17 @@
 
     def anatqc(self, *args, **kwargs):
         return neuroinfo.anatqc(self._auth, *args, **kwargs)
 
     def t2qc(self, *args, **kwargs):
         return neuroinfo.t2qc(self._auth, *args, **kwargs)
 
+    def dwiqc(self, *args, **kwargs):
+        return neuroinfo.dwiqc(self._auth, *args, **kwargs)
+
     def __enter__(self):
         self._auth = yaxil.start_session(self._auth)
         return self
 
     def __exit__(self, type, value, traceback):
         yaxil.end_session(self._auth)
         return
```

## Comparing `yaxil-0.9.8.data/scripts/ArcGet.py` & `yaxil-0.9.9.data/scripts/ArcGet.py`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.8.data/scripts/xnat_auth` & `yaxil-0.9.9.data/scripts/xnat_auth`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.8.dist-info/LICENSE` & `yaxil-0.9.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.8.dist-info/RECORD` & `yaxil-0.9.9.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 yaxil/__init__.py,sha256=ORVt8FrzAKC-vkG6-Nmne_ydZUgjnojDPgoAN3iXHsE,46800
-yaxil/__version__.py,sha256=PovqQipXzNJhYkh9ZvIcUUsWchfj18O2twDFVSjAjlo,232
+yaxil/__version__.py,sha256=-84epgn-OfC0jwUrKYUcW_5f2V5e6HWbNSd7pl5vUk0,232
 yaxil/assessments/__init__.py,sha256=TpcTgZ9L8FnHvBOwkeK07BDBnoqqHLV1hVaVG9-yXg8,84
-yaxil/assessments/neuroinfo/__init__.py,sha256=w9jMK30L3BO6QdMrP5hiP4ziai0zngVNd98IO3H_UG8,25510
+yaxil/assessments/neuroinfo/__init__.py,sha256=ddY6J74kTRIFEHq7DLAS_rE-zZ2_Z_kzhXo9WqIEfdo,24717
 yaxil/assessments/neuroinfo/legacy/__init__.py,sha256=k7kzdPUCcFDE7CWYzLQj6KkgokcZPiAwa0Pp62-V2fY,7117
-yaxil/assessments/neuroinfo/session/__init__.py,sha256=W3COlgCEoyO0hth3idT1JP7IRhaFmT0CC7lNxVG0uRs,699
+yaxil/assessments/neuroinfo/session/__init__.py,sha256=1m9NH4EyfFl1-2Koc0IbgnQ2bnbItCeG5qNPV55bd6U,798
 yaxil/bids/__init__.py,sha256=I4VUikLW9gLwfPmEpw4SXJDSa_riBX7IOPryykxOFF8,16280
 yaxil/commons/__init__.py,sha256=lCdwSNdIavfJi5Wux0mZ5Ay_HgKU-FnG-X6vZclDq24,2805
 yaxil/dicom/__init__.py,sha256=hsrcXBZDMBJDrDtaGuVG-T8Btb-EDBSAf5PJbs-qht0,1656
 yaxil/exceptions/__init__.py,sha256=1xNTBxyCkWGevMNBe1kbESSMD5gH06bOG_3XUMYcUHQ,625
 yaxil/functools/__init__.py,sha256=P5yiAU1yotWAFPTi0_rs9SpKTxj1EH9NeBjVMHG3lGs,783
 yaxil/session/__init__.py,sha256=Tr9ALXprn6Xnx6smZHJgOcSBESMkgjB3dSnW_RnrZh8,1477
-yaxil-0.9.8.data/scripts/ArcGet.py,sha256=eNhHHTVeBgkkaZVu1fdLgiJv0ZHSGqNQU9aTRU-hIrU,9426
-yaxil-0.9.8.data/scripts/xnat_auth,sha256=wQ1aNeFxLjtarDu7LqdG-zEepMUShVjw0av_sT8uv3w,4114
-yaxil-0.9.8.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
-yaxil-0.9.8.dist-info/METADATA,sha256=XMo_dOYM1h3UiN0na-MZ-7SlSCaVqJtl5s929fGhfs0,387
-yaxil-0.9.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-yaxil-0.9.8.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
-yaxil-0.9.8.dist-info/RECORD,,
+yaxil-0.9.9.data/scripts/ArcGet.py,sha256=eNhHHTVeBgkkaZVu1fdLgiJv0ZHSGqNQU9aTRU-hIrU,9426
+yaxil-0.9.9.data/scripts/xnat_auth,sha256=wQ1aNeFxLjtarDu7LqdG-zEepMUShVjw0av_sT8uv3w,4114
+yaxil-0.9.9.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
+yaxil-0.9.9.dist-info/METADATA,sha256=H2vMPtcYjWm-Vzk05DHB1pfbM9pLBXez98JcIDijGmM,414
+yaxil-0.9.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+yaxil-0.9.9.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
+yaxil-0.9.9.dist-info/RECORD,,
```

