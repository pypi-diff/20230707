# Comparing `tmp/banf-0.0.4-py3-none-any.whl.zip` & `tmp/banf-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 15547 bytes, number of entries: 18
+Zip file size: 15527 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-03 02:05 banf/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-09 00:00 banf/communicate/__init__.py
 -rw-rw-rw-  2.0 fat     3025 b- defN 23-Feb-22 05:10 banf/communicate/db_inserter.py
 -rw-rw-rw-  2.0 fat     1694 b- defN 23-Mar-02 00:17 banf/communicate/kafka_consumer.py
 -rw-rw-rw-  2.0 fat     1750 b- defN 23-Mar-06 00:26 banf/communicate/mqtt_receiver.py
 -rw-rw-rw-  2.0 fat     3967 b- defN 23-May-26 03:55 banf/communicate/mqtt_sender.py
 -rw-rw-rw-  2.0 fat     2560 b- defN 23-May-26 03:56 banf/communicate/prometheus_sender.py
 -rw-rw-rw-  2.0 fat     2386 b- defN 23-Jul-03 09:20 banf/communicate/s3_sender.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-03 02:17 banf/data_processing/__init__.py
 -rw-rw-rw-  2.0 fat    18505 b- defN 23-Jul-03 10:12 banf/data_processing/preprocessing.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-09 00:00 banf/etc/__init__.py
 -rw-rw-rw-  2.0 fat      538 b- defN 23-May-25 05:45 banf/etc/bench.py
 -rw-rw-rw-  2.0 fat     2488 b- defN 23-May-30 22:47 banf/etc/observe.py
 -rw-rw-rw-  2.0 fat      240 b- defN 22-Dec-13 04:20 banf/etc/pattern.py
--rw-rw-rw-  2.0 fat     2899 b- defN 23-Jul-07 00:45 banf-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 00:45 banf-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-07 00:45 banf-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1453 b- defN 23-Jul-07 00:45 banf-0.0.4.dist-info/RECORD
-18 files, 41602 bytes uncompressed, 13159 bytes compressed:  68.4%
+-rw-rw-rw-  2.0 fat     2824 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1453 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/RECORD
+18 files, 41527 bytes uncompressed, 13139 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: banf/etc/observe.py
 Comment: 
 
 Filename: banf/etc/pattern.py
 Comment: 
 
-Filename: banf-0.0.4.dist-info/METADATA
+Filename: banf-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: banf-0.0.4.dist-info/WHEEL
+Filename: banf-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: banf-0.0.4.dist-info/top_level.txt
+Filename: banf-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: banf-0.0.4.dist-info/RECORD
+Filename: banf-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `banf-0.0.4.dist-info/METADATA` & `banf-0.0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banf
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for BANF Co., Ltd.
 Author: BANF Co., Ltd.
 Author-email: gwjeon@banf.co.kr
 Keywords: tire sensor,mqtt,aws,BANF Co., Ltd.
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: bleach (>=6.0.0)
@@ -55,16 +55,14 @@
 Requires-Dist: Pillow (>=9.5.0)
 Requires-Dist: pkginfo (>=1.9.6)
 Requires-Dist: pyarrow (>=12.0.1)
 Requires-Dist: pyct (>=0.5.0)
 Requires-Dist: pyparsing (>=3.0.9)
 Requires-Dist: pytz (>=2023.3)
 Requires-Dist: pyviz-comms (>=2.3.2)
-Requires-Dist: pywin32 (>=305.1)
-Requires-Dist: pywin32-ctypes (>=0.2.2)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: readme-renderer (>=40.0)
 Requires-Dist: requests (>=2.31.0)
 Requires-Dist: requests-toolbelt (>=1.0.0)
 Requires-Dist: rfc3986 (>=2.0.0)
 Requires-Dist: rich (>=13.4.2)
 Requires-Dist: s3transfer (>=0.6.1)
```

## Comparing `banf-0.0.4.dist-info/RECORD` & `banf-0.0.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 banf/communicate/s3_sender.py,sha256=iZ-I98BhIuL0t2Vje6B4Jvpfsw8AaW_5dWz6XC0mBZU,2386
 banf/data_processing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 banf/data_processing/preprocessing.py,sha256=qkvtXnMhMdM16jUv0UfNS-wpwb9ZkDK_rmH8jJ8K8lY,18505
 banf/etc/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 banf/etc/bench.py,sha256=2Cl_DZrIPLWZWOMRk7vJ37R5tgft04Vu0rPZUAKsg5Q,538
 banf/etc/observe.py,sha256=hsBzz3YEJdEBWCrFDAqz3_orQzVNuhc4IGFq8j_LweM,2488
 banf/etc/pattern.py,sha256=n_j7-mN-QvHRkTP0Tpk8XKfKxXGkZdJfT7eBa_nPQV4,240
-banf-0.0.4.dist-info/METADATA,sha256=qcojeJoMn_Vh9YMIZvlIToqQ0i37m_KroCsqgPWspF0,2899
-banf-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-banf-0.0.4.dist-info/top_level.txt,sha256=6ofKzRyfdu0ATVSHwt9hzGECFmXRGpQ9Fs0igCzbNgM,5
-banf-0.0.4.dist-info/RECORD,,
+banf-0.0.5.dist-info/METADATA,sha256=qhnEKcsPkGZ-lHp68bz94RsMyB9LhABVZSANU3DXKYU,2824
+banf-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+banf-0.0.5.dist-info/top_level.txt,sha256=6ofKzRyfdu0ATVSHwt9hzGECFmXRGpQ9Fs0igCzbNgM,5
+banf-0.0.5.dist-info/RECORD,,
```

