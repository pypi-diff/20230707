# Comparing `tmp/cirq-1.2.0.dev20230706165102-py3-none-any.whl.zip` & `tmp/cirq-1.2.0.dev20230706194816-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8392 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 23-Jul-06 16:51 cirq-1.2.0.dev20230706165102.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 16:51 cirq-1.2.0.dev20230706165102.dist-info/LICENSE
--rw-r--r--  2.0 unx     7850 b- defN 23-Jul-06 16:51 cirq-1.2.0.dev20230706165102.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 16:51 cirq-1.2.0.dev20230706165102.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 16:51 cirq-1.2.0.dev20230706165102.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Jul-06 16:51 cirq-1.2.0.dev20230706165102.dist-info/RECORD
-6 files, 20155 bytes uncompressed, 7354 bytes compressed:  63.5%
+Zip file size: 8393 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-06 19:48 cirq-1.2.0.dev20230706194816.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 19:48 cirq-1.2.0.dev20230706194816.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7850 b- defN 23-Jul-06 19:48 cirq-1.2.0.dev20230706194816.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 19:48 cirq-1.2.0.dev20230706194816.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 19:48 cirq-1.2.0.dev20230706194816.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Jul-06 19:48 cirq-1.2.0.dev20230706194816.dist-info/RECORD
+6 files, 20155 bytes uncompressed, 7355 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.2.0.dev20230706165102.dist-info/AUTHORS
+Filename: cirq-1.2.0.dev20230706194816.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.2.0.dev20230706165102.dist-info/LICENSE
+Filename: cirq-1.2.0.dev20230706194816.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.2.0.dev20230706165102.dist-info/METADATA
+Filename: cirq-1.2.0.dev20230706194816.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.2.0.dev20230706165102.dist-info/WHEEL
+Filename: cirq-1.2.0.dev20230706194816.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.2.0.dev20230706165102.dist-info/top_level.txt
+Filename: cirq-1.2.0.dev20230706194816.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.2.0.dev20230706165102.dist-info/RECORD
+Filename: cirq-1.2.0.dev20230706194816.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.2.0.dev20230706165102.dist-info/LICENSE` & `cirq-1.2.0.dev20230706194816.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.2.0.dev20230706165102.dist-info/METADATA` & `cirq-1.2.0.dev20230706194816.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.2.0.dev20230706165102
+Version: 1.2.0.dev20230706194816
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.9.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt (==1.2.0.dev20230706165102)
-Requires-Dist: cirq-core (==1.2.0.dev20230706165102)
-Requires-Dist: cirq-ft (==1.2.0.dev20230706165102)
-Requires-Dist: cirq-google (==1.2.0.dev20230706165102)
-Requires-Dist: cirq-ionq (==1.2.0.dev20230706165102)
-Requires-Dist: cirq-pasqal (==1.2.0.dev20230706165102)
-Requires-Dist: cirq-rigetti (==1.2.0.dev20230706165102)
-Requires-Dist: cirq-web (==1.2.0.dev20230706165102)
+Requires-Dist: cirq-aqt (==1.2.0.dev20230706194816)
+Requires-Dist: cirq-core (==1.2.0.dev20230706194816)
+Requires-Dist: cirq-ft (==1.2.0.dev20230706194816)
+Requires-Dist: cirq-google (==1.2.0.dev20230706194816)
+Requires-Dist: cirq-ionq (==1.2.0.dev20230706194816)
+Requires-Dist: cirq-pasqal (==1.2.0.dev20230706194816)
+Requires-Dist: cirq-rigetti (==1.2.0.dev20230706194816)
+Requires-Dist: cirq-web (==1.2.0.dev20230706194816)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
```

## Comparing `cirq-1.2.0.dev20230706165102.dist-info/RECORD` & `cirq-1.2.0.dev20230706194816.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-cirq-1.2.0.dev20230706165102.dist-info/AUTHORS,sha256=FyiF0gaNIILE_9q7HDCtKOsTlwNwu0qsTbOAXF67F9A,292
-cirq-1.2.0.dev20230706165102.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-cirq-1.2.0.dev20230706165102.dist-info/METADATA,sha256=SQlP5fxm04X5kFsEauRq539zK9NzJQe_nSMObUY4CGY,7850
-cirq-1.2.0.dev20230706165102.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cirq-1.2.0.dev20230706165102.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-cirq-1.2.0.dev20230706165102.dist-info/RECORD,,
+cirq-1.2.0.dev20230706194816.dist-info/AUTHORS,sha256=FyiF0gaNIILE_9q7HDCtKOsTlwNwu0qsTbOAXF67F9A,292
+cirq-1.2.0.dev20230706194816.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+cirq-1.2.0.dev20230706194816.dist-info/METADATA,sha256=SwqTN_M6fCbbelBQPa-zY4TmzYPJbQQ1grzT57LlS0w,7850
+cirq-1.2.0.dev20230706194816.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cirq-1.2.0.dev20230706194816.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+cirq-1.2.0.dev20230706194816.dist-info/RECORD,,
```

