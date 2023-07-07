# Comparing `tmp/h5coro-0.0.5.tar.gz` & `tmp/h5coro-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5coro-0.0.5.tar", last modified: Thu Jul  6 14:03:10 2023, max compression
+gzip compressed data, was "h5coro-0.0.6.tar", last modified: Fri Jul  7 19:05:50 2023, max compression
```

## Comparing `h5coro-0.0.5.tar` & `h5coro-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3078 2023-06-27 11:55:04.000000 h5coro-0.0.5/.gitignore
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1511 2023-06-27 11:55:04.000000 h5coro-0.0.5/LICENSE
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      150 2023-06-27 11:55:04.000000 h5coro-0.0.5/MANIFEST.in
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-07-06 14:03:10.450705 h5coro-0.0.5/PKG-INFO
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    13802 2023-07-05 20:41:02.000000 h5coro-0.0.5/README.md
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.446705 h5coro-0.0.5/data/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      338 2023-06-27 19:37:14.000000 h5coro-0.0.5/data/grandmesa.geojson
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/h5coro/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      194 2023-06-27 11:55:04.000000 h5coro-0.0.5/h5coro/__init__.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      229 2023-06-27 13:23:23.000000 h5coro-0.0.5/h5coro/filedriver.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    93760 2023-07-05 20:38:28.000000 h5coro-0.0.5/h5coro/h5coro.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     2059 2023-07-05 20:54:12.000000 h5coro-0.0.5/h5coro/s3driver.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      319 2023-06-27 11:55:04.000000 h5coro-0.0.5/h5coro/version.py
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/h5coro.egg-info/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/PKG-INFO
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      437 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/SOURCES.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        1 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/dependency_links.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       12 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/requires.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       13 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/top_level.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      134 2023-06-27 13:30:21.000000 h5coro-0.0.5/pytest.ini
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       11 2023-06-27 13:24:47.000000 h5coro-0.0.5/requirements.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       38 2023-07-06 14:03:10.450705 h5coro-0.0.5/setup.cfg
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1078 2023-07-03 19:56:10.000000 h5coro-0.0.5/setup.py
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/utils/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3380 2023-07-06 12:51:32.000000 h5coro-0.0.5/utils/read_variable.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     7347 2023-06-29 20:21:49.000000 h5coro-0.0.5/utils/subset_atl03.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     5127 2023-06-28 18:01:05.000000 h5coro-0.0.5/utils/subset_atl06.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    10271 2023-07-05 20:48:46.000000 h5coro-0.0.5/utils/utils.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        7 2023-07-06 13:57:02.000000 h5coro-0.0.5/version.txt
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-07 19:05:50.214020 h5coro-0.0.6/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3078 2023-06-27 11:55:04.000000 h5coro-0.0.6/.gitignore
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1511 2023-06-27 11:55:04.000000 h5coro-0.0.6/LICENSE
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      150 2023-06-27 11:55:04.000000 h5coro-0.0.6/MANIFEST.in
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-07-07 19:05:50.214020 h5coro-0.0.6/PKG-INFO
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    13802 2023-07-05 20:41:02.000000 h5coro-0.0.6/README.md
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-07 19:05:50.210020 h5coro-0.0.6/data/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      338 2023-06-27 19:37:14.000000 h5coro-0.0.6/data/grandmesa.geojson
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-07 19:05:50.210020 h5coro-0.0.6/h5coro/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      194 2023-06-27 11:55:04.000000 h5coro-0.0.6/h5coro/__init__.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      229 2023-06-27 13:23:23.000000 h5coro-0.0.6/h5coro/filedriver.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    95053 2023-07-07 18:59:00.000000 h5coro-0.0.6/h5coro/h5coro.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     2059 2023-07-05 20:54:12.000000 h5coro-0.0.6/h5coro/s3driver.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      319 2023-06-27 11:55:04.000000 h5coro-0.0.6/h5coro/version.py
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-07 19:05:50.210020 h5coro-0.0.6/h5coro.egg-info/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-07-07 19:05:50.000000 h5coro-0.0.6/h5coro.egg-info/PKG-INFO
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      437 2023-07-07 19:05:50.000000 h5coro-0.0.6/h5coro.egg-info/SOURCES.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        1 2023-07-07 19:05:50.000000 h5coro-0.0.6/h5coro.egg-info/dependency_links.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       12 2023-07-07 19:05:50.000000 h5coro-0.0.6/h5coro.egg-info/requires.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       13 2023-07-07 19:05:50.000000 h5coro-0.0.6/h5coro.egg-info/top_level.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      134 2023-06-27 13:30:21.000000 h5coro-0.0.6/pytest.ini
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       11 2023-06-27 13:24:47.000000 h5coro-0.0.6/requirements.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       38 2023-07-07 19:05:50.214020 h5coro-0.0.6/setup.cfg
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1078 2023-07-03 19:56:10.000000 h5coro-0.0.6/setup.py
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-07 19:05:50.214020 h5coro-0.0.6/utils/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3380 2023-07-06 12:51:32.000000 h5coro-0.0.6/utils/read_variable.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     7347 2023-06-29 20:21:49.000000 h5coro-0.0.6/utils/subset_atl03.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     5127 2023-06-28 18:01:05.000000 h5coro-0.0.6/utils/subset_atl06.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    10271 2023-07-06 16:55:32.000000 h5coro-0.0.6/utils/utils.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        7 2023-07-07 19:04:15.000000 h5coro-0.0.6/version.txt
```

### Comparing `h5coro-0.0.5/.gitignore` & `h5coro-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/LICENSE` & `h5coro-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/PKG-INFO` & `h5coro-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5coro
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for reading HDF5 data from S3
 Home-page: https://github.com/ICESat2-SlideRule/h5coro/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `h5coro-0.0.5/README.md` & `h5coro-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/h5coro/h5coro.py` & `h5coro-0.0.6/h5coro/h5coro.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,17 +228,17 @@
             }
         }
     }
 
     #######################
     # Constructor
     #######################
-    def __init__(self, resourceObject, dataset, startRow=0, numRows=ALL_ROWS):
+    def __init__(self, resourceObject, dataset, startRow=0, numRows=ALL_ROWS, metaOnly=False):
         self.resourceObject         = resourceObject
-        self.metaOnly               = False
+        self.metaOnly               = metaOnly
         self.pos                    = self.resourceObject.rootAddress
         self.dataset                = dataset
         self.datasetStartRow        = startRow
         self.datasetNumRows         = numRows
         self.datasetPath            = list(filter(('').__ne__, self.dataset.split('/')))
         self.datasetPathLevels      = len(self.datasetPath)
         self.datasetFound           = False
@@ -478,14 +478,18 @@
     #######################
     def readObjHdrV0(self, dlvl):
         FILE_STATS_BIT          = 0x20
         STORE_CHANGE_PHASE_BIT  = 0x10
         SIZE_OF_CHUNK_0_MASK    = 0x3
         starting_position       = self.pos
 
+        # display
+        if verboseOption:
+            logger.info(f'<<Object Information V0 - {self.dataset}[{dlvl}] @0x{starting_position:x}>>')
+
         # check signature and version
         if errorCheckingOption:
             signature = self.readField(4)
             version = self.readField(1)
             if signature != self.H5_OHDR_SIGNATURE_LE:
                 raise FatalError(f'invalid version 0 object header signature: 0x{signature:x}')
             if version != 2:
@@ -497,15 +501,14 @@
         obj_hdr_flags = self.readField(1)
         if obj_hdr_flags & FILE_STATS_BIT:
             if verboseOption:
                 access_time = self.readField(4)
                 modification_time = self.readField(4)
                 change_time = self.readField(4)
                 birth_time = self.readField(4)
-                logger.info(f'<<Object Information V0 - {self.dataset}[{dlvl}] @0x{starting_position:x}>>')
                 logger.info(f'Access Time:          {datetime.fromtimestamp(access_time)}')
                 logger.info(f'Modification Time:    {datetime.fromtimestamp(modification_time)}')
                 logger.info(f'Change Time:          {datetime.fromtimestamp(change_time)}')
                 logger.info(f'Birth Time:           {datetime.fromtimestamp(birth_time)}')
             else:
                 self.pos += 16
 
@@ -549,21 +552,21 @@
 
             # read message
             bytes_read = self.readMessage(msg_type, msg_size, obj_hdr_flags, dlvl)
             if errorCheckingOption and (bytes_read != msg_size):
                 raise FatalError(f'header v0 message different size than specified: {bytes_read} != {msg_size}')
 
             # check if dataset found
-            if self.datasetFound:
+            if not self.metaOnly and self.datasetFound:
                 self.pos = end_of_hdr # go directory to end of header
                 break # exit loop because dataset is found
 
         # check bytes read
-        if errorCheckingOption and (self.pos != end_of_hdr):
-            raise FatalError(f'did not read correct number of v0 bytes: 0x{self.pos:x} != 0x{end_of_hdr:x}')
+        if errorCheckingOption and (self.pos < end_of_hdr):
+            raise FatalError(f'did not read enough v0 bytes: 0x{self.pos:x} < 0x{end_of_hdr:x}')
 
         # return bytes read
         return self.pos - starting_position
 
     #######################
     # readObjHdrV1
     #######################
@@ -620,25 +623,25 @@
             alignment_padding = ((8 - (bytes_read % 8)) % 8) # align to 8-byte boundary
             self.pos += alignment_padding
             bytes_read += alignment_padding
             if errorCheckingOption and (bytes_read != msg_size):
                 raise FatalError(f'header v1 message different size than specified: {bytes_read} != {msg_size}')
 
             # check if dataset found
-            if self.datasetFound:
+            if not self.metaOnly and self.datasetFound:
                 self.pos = end_of_hdr # go directory to end of header
                 break # exit loop because dataset is found
 
         # move past gap
         if self.pos < end_of_hdr:
             self.pos = end_of_hdr
 
         # check bytes read
-        if errorCheckingOption and (self.pos != end_of_hdr):
-            raise FatalError(f'did not read correct number of v1 bytes: 0x{self.pos:x} != 0x{end_of_hdr:x}')
+        if errorCheckingOption and (self.pos < end_of_hdr):
+            raise FatalError(f'did not read enough v1 bytes: 0x{self.pos:x} < 0x{end_of_hdr:x}')
 
         # return bytes read
         return self.pos - starting_position
 
     #######################
     # readMessage
     #######################
@@ -993,15 +996,15 @@
             logger.info(f'Link Type:            {link_type}')
             logger.info(f'Creation Order:       {create_order}')
             logger.info(f'Character Set:        {char_set}')
             logger.info(f'Link Name:            {link_name}')
 
         # check if follow link
         follow_link = False
-        if link_name == self.datasetPath[dlvl]:
+        if dlvl < len(self.datasetPath) and link_name == self.datasetPath[dlvl]:
             follow_link = True
 
         # process link
         if link_type == HARD_LINK:
             obj_hdr_addr = self.readField(self.resourceObject.offsetSize)
             if verboseOption:
                 logger.info(f'Hard Link:            0x{obj_hdr_addr:x}')
@@ -1347,19 +1350,19 @@
             for _ in range(entries_used):
                 symbol_table_addr = self.readField(self.resourceObject.offsetSize)
                 current_node_pos = self.pos
                 self.pos = symbol_table_addr
                 self.readSymbolTable(head_data_addr, dlvl)
                 self.pos = current_node_pos
                 self.pos += self.resourceObject.lengthSize # skip next key
-                if self.datasetFound:
+                if not self.metaOnly and self.datasetFound:
                     break
 
             # exit loop or go to next node
-            if (right_sibling == INVALID_VALUE[self.resourceObject.offsetSize]) or self.datasetFound:
+            if (right_sibling == INVALID_VALUE[self.resourceObject.offsetSize]) or (not self.metaOnly and self.datasetFound):
                 break
             else:
                 self.pos = right_sibling
 
             # read header info
             if errorCheckingOption:
                 signature = self.readField(4)
@@ -1479,15 +1482,15 @@
 
             # update meta data table
             group_path = '/'.join(self.datasetPath[:dlvl] + [link_name])
             self.resourceObject.metaDataTable[group_path] = obj_hdr_addr
 
             # process link
             return_position = self.pos
-            if link_name == self.datasetPath[dlvl]:
+            if dlvl < len(self.datasetPath) and link_name == self.datasetPath[dlvl]:
                 if cache_type == 2:
                     raise FatalError(f'symbolic links are unsupported: {link_name}')
                 self.readObjHdr(obj_hdr_addr, dlvl + 1)
                 self.pos = return_position
                 if not self.metaOnly:
                     break # datasetFound
 
@@ -1667,15 +1670,15 @@
             heap_info['cur_objects'] += 1
 
             # check reading past block
             if errorCheckingOption and data_left < 0:
                 raise FatalError(f'reading message exceeded end of direct block: {starting_position}')
 
             # check if dataset found
-            if self.datasetFound:
+            if not self.metaOnly and self.datasetFound:
                 break
 
         # skip to end of block (useful only if exited loop above early)
         self.pos += data_left
 
         # return bytes read
         return self.pos - starting_position
@@ -2030,15 +2033,15 @@
         self.conditions = {}
 
         self.readDatasets(datasets, block)
 
     #######################
     # readDatasets
     #######################
-    def readDatasets(self, datasets, block):
+    def readDatasets(self, datasets, block=True):
 
         # check if datasets supplied
         if len(datasets) <= 0:
             return
 
         # make into dictionary
         dataset_table = {}
@@ -2061,14 +2064,41 @@
         # wait for results to be populated OR populate results in the background
         if block:
             resultThread(self)
         else:
             threading.Thread(target=resultThread, args=(self,), daemon=True).start()
 
     #######################
+    # listDirectory
+    #######################
+    def listDirectory(self, directory):
+        try:
+            dataset_worker = H5Dataset(self, directory, metaOnly=True)
+            dataset_worker.readDataset()
+        except FatalError as e:
+            logger.debug(f'H5Coro exited listing the directory {directory}: {e}')
+        if len(directory) > 0 and directory[0] == '/':
+            directory = directory[1:]
+        if len(directory) > 0 and directory[-1] == '/':
+            directory = directory[:-1]
+        elements = {}
+        for entry in self.metaDataTable:
+            if entry.startswith(directory):
+                if len(directory) > 0:
+                    element = entry.split(directory)[1]
+                else:
+                    element = entry
+                if len(element) > 0 and element[0] == '/':
+                    element = element[1:]
+                if len(element) > 0:
+                    element = element.split('/')[0]
+                    elements[element] = True
+        return list(elements.keys())
+
+    #######################
     # operator: []
     #######################
     def __getitem__(self, key):
         self.waitOnResult(key)
         return self.results[key]
 
     #######################
```

### Comparing `h5coro-0.0.5/h5coro/s3driver.py` & `h5coro-0.0.6/h5coro/s3driver.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/h5coro.egg-info/PKG-INFO` & `h5coro-0.0.6/h5coro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5coro
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for reading HDF5 data from S3
 Home-page: https://github.com/ICESat2-SlideRule/h5coro/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `h5coro-0.0.5/setup.py` & `h5coro-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/utils/read_variable.py` & `h5coro-0.0.6/utils/read_variable.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/utils/subset_atl03.py` & `h5coro-0.0.6/utils/subset_atl03.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/utils/subset_atl06.py` & `h5coro-0.0.6/utils/subset_atl06.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.5/utils/utils.py` & `h5coro-0.0.6/utils/utils.py`

 * *Files identical despite different names*

