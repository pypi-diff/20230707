# Comparing `tmp/KeSi-1.4.3.tar.gz` & `tmp/KeSi-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KeSi-1.4.3.tar", last modified: Tue Jan  3 01:47:57 2023, max compression
+gzip compressed data, was "dist/KeSi-1.5.0.tar", last modified: Fri Jul  7 05:59:42 2023, max compression
```

## Comparing `KeSi-1.4.3.tar` & `KeSi-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-03 01:47:57.000000 KeSi-1.4.3/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-03 01:47:57.000000 KeSi-1.4.3/KeSi.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2023-01-03 01:47:57.000000 KeSi-1.4.3/KeSi.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2023-01-03 01:47:57.000000 KeSi-1.4.3/KeSi.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-01-03 01:47:57.000000 KeSi-1.4.3/KeSi.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-01-03 01:47:57.000000 KeSi-1.4.3/KeSi.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2023-01-03 01:47:41.000000 KeSi-1.4.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2023-01-03 01:47:41.000000 KeSi-1.4.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2023-01-03 01:47:57.000000 KeSi-1.4.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1036 2023-01-03 01:47:41.000000 KeSi-1.4.3/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-03 01:47:57.000000 KeSi-1.4.3/kesi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      433 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-03 01:47:57.000000 KeSi-1.4.3/kesi/butkian/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/butkian/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1461 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/butkian/ji.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2696 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/butkian/kongiong.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17988 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/butkian/ku.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3090 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/butkian/su.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-03 01:47:57.000000 KeSi-1.4.3/kesi/susia/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3407 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/susia/POJ.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1739 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/susia/TL.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/susia/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/susia/kongke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2023-01-03 01:47:41.000000 KeSi-1.4.3/kesi/susia/pio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2023-01-03 01:47:41.000000 KeSi-1.4.3/panpun.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-01-03 01:47:57.000000 KeSi-1.4.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      808 2023-01-03 01:47:41.000000 KeSi-1.4.3/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 05:59:42.699490 KeSi-1.5.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 05:59:42.695489 KeSi-1.5.0/KeSi.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      615 2023-07-07 05:59:42.000000 KeSi-1.5.0/KeSi.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      381 2023-07-07 05:59:42.000000 KeSi-1.5.0/KeSi.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-07 05:59:42.000000 KeSi-1.5.0/KeSi.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-07-07 05:59:42.000000 KeSi-1.5.0/KeSi.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2023-07-07 05:59:25.000000 KeSi-1.5.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       52 2023-07-07 05:59:25.000000 KeSi-1.5.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      615 2023-07-07 05:59:42.699490 KeSi-1.5.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4454 2023-07-07 05:59:25.000000 KeSi-1.5.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 05:59:42.695489 KeSi-1.5.0/kesi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      433 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 05:59:42.695489 KeSi-1.5.0/kesi/butkian/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/butkian/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1670 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/butkian/ji.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2696 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/butkian/kongiong.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18069 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/butkian/ku.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3171 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/butkian/su.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 05:59:42.699490 KeSi-1.5.0/kesi/susia/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3407 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/susia/POJ.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1739 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/susia/TL.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/susia/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/susia/kongke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2023-07-07 05:59:25.000000 KeSi-1.5.0/kesi/susia/pio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       17 2023-07-07 05:59:25.000000 KeSi-1.5.0/panpun.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-07 05:59:42.699490 KeSi-1.5.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      808 2023-07-07 05:59:25.000000 KeSi-1.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `KeSi-1.4.3/KeSi.egg-info/PKG-INFO` & `KeSi-1.5.0/KeSi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeSi
-Version: 1.4.3
+Version: 1.5.0
 Summary: 台語文NLP家私
 Home-page: https://ithuan.tw/
 Download-URL: https://github.com/i3thuan5/KeSi
 Author: Tshuà Bûn-lī
 Author-email: ithuan@ithuan.tw
 Keywords: Parser,Alignment,Taigi,Hanji,Lomaji
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `KeSi-1.4.3/LICENSE` & `KeSi-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `KeSi-1.4.3/PKG-INFO` & `KeSi-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeSi
-Version: 1.4.3
+Version: 1.5.0
 Summary: 台語文NLP家私
 Home-page: https://ithuan.tw/
 Download-URL: https://github.com/i3thuan5/KeSi
 Author: Tshuà Bûn-lī
 Author-email: ithuan@ithuan.tw
 Keywords: Parser,Alignment,Taigi,Hanji,Lomaji
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `KeSi-1.4.3/kesi/butkian/ji.py` & `KeSi-1.5.0/kesi/butkian/ji.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,21 @@
         if lomaji and si_khinsiann:
             self.lomaji = '--{}'.format(lomaji)
         elif lomaji:
             self.lomaji = lomaji
         else:
             self.lomaji = self.hanlo
 
+    def __eq__(self, other):
+        return (
+            self.hanlo == other.hanlo
+            and self.lomaji == other.lomaji
+            and self.si_khinsiann == other.si_khinsiann
+        )
+
     @property
     def kiphanlo(self):
         if self.si_khinsiann and not si_lomaji(self.hanlo[2]):
             return self.hanlo[2:]
         return self.hanlo
 
     def POJ(self):
@@ -46,10 +53,12 @@
             hanlo = self.hanlo
             lomaji = self.lomaji
         return Ji(
             tsuanTL(hanlo), tsuanTL(lomaji),
             si_khinsiann=self.si_khinsiann
         )
 
+    KIP = TL
+
     @property
     def si_khinsiann(self):
         return self.hanlo.startswith(KHIN_SIANN_HU)
```

### Comparing `KeSi-1.4.3/kesi/butkian/kongiong.py` & `KeSi-1.5.0/kesi/butkian/kongiong.py`

 * *Files identical despite different names*

### Comparing `KeSi-1.4.3/kesi/butkian/ku.py` & `KeSi-1.5.0/kesi/butkian/ku.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
     def __getitem__(self, kui):
         return self._su[kui]
 
     def __len__(self):
         return len(self._su)
 
+    def __eq__(self, other):
+        return self._su == other._su
+
     def _bun_tsuan_sutin(self, bun_tin, khinsiann_tin):
         sutin = []
         for tsitsu, khinsiann in zip(bun_tin, khinsiann_tin):
             su = Su()
             for ji, si_khinsiann in zip(tsitsu, khinsiann):
                 su.thiam(
                     Ji(ji, si_khinsiann=si_khinsiann)
@@ -183,14 +186,16 @@
 
     def TL(self):
         sin_ku = Ku()
         for su in self:
             sin_ku.thiam(su.TL())
         return sin_ku
 
+    KIP = TL
+
     def _tngsu(self, 字陣列, 輕聲陣列, 佮後一个字無仝一个詞):
         巢狀詞陣列 = []
         巢狀輕聲陣列 = []
         位置 = 0
         while 位置 < len(字陣列):
             範圍 = 位置
             while 範圍 < len(佮後一个字無仝一个詞) and not 佮後一个字無仝一个詞[範圍]:
```

### Comparing `KeSi-1.4.3/kesi/butkian/su.py` & `KeSi-1.5.0/kesi/butkian/su.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
     def __iter__(self):
         yield from self._ji
 
     def __len__(self):
         return len(self._ji)
 
+    def __eq__(self, other):
+        return self._ji == other._ji
+
     @property
     def hanlo(self):
         """
         會 kā 文本標準化：
         判斷愛先添連字符無
           H, H -> 'HH'
           H, L -> 'HL'
@@ -110,7 +113,9 @@
         return sin_su
 
     def TL(self):
         sin_su = Su()
         for ji in self:
             sin_su.thiam(ji.TL())
         return sin_su
+
+    KIP = TL
```

### Comparing `KeSi-1.4.3/kesi/susia/POJ.py` & `KeSi-1.5.0/kesi/susia/POJ.py`

 * *Files identical despite different names*

### Comparing `KeSi-1.4.3/kesi/susia/TL.py` & `KeSi-1.5.0/kesi/susia/TL.py`

 * *Files identical despite different names*

### Comparing `KeSi-1.4.3/kesi/susia/kongke.py` & `KeSi-1.5.0/kesi/susia/kongke.py`

 * *Files identical despite different names*

### Comparing `KeSi-1.4.3/kesi/susia/pio.py` & `KeSi-1.5.0/kesi/susia/pio.py`

 * *Files identical despite different names*

### Comparing `KeSi-1.4.3/setup.py` & `KeSi-1.5.0/setup.py`

 * *Files identical despite different names*

