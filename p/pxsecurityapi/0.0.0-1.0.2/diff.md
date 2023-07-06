# Comparing `tmp/pxsecurityapi-0.0.0.tar.gz` & `tmp/pxsecurityapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxsecurityapi-0.0.0.tar", last modified: Thu Jul  6 23:41:15 2023, max compression
+gzip compressed data, was "pxsecurityapi-1.0.2.tar", last modified: Thu Jul  6 23:49:57 2023, max compression
```

## Comparing `pxsecurityapi-0.0.0.tar` & `pxsecurityapi-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 23:41:15.880107 pxsecurityapi-0.0.0/
--rw-rw-rw-   0        0        0      360 2023-07-06 23:41:15.880107 pxsecurityapi-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxsecurityapi-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      526 2023-07-06 23:41:15.880107 pxsecurityapi-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 23:41:15.880107 pxsecurityapi-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 23:41:15.880107 pxsecurityapi-0.0.0/src/pxsecurityapi/
--rw-rw-rw-   0        0        0     1870 2023-07-06 22:49:22.000000 pxsecurityapi-0.0.0/src/pxsecurityapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 23:41:15.880107 pxsecurityapi-0.0.0/src/pxsecurityapi.egg-info/
--rw-rw-rw-   0        0        0      360 2023-07-06 23:41:15.000000 pxsecurityapi-0.0.0/src/pxsecurityapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-06 23:41:15.000000 pxsecurityapi-0.0.0/src/pxsecurityapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 23:41:15.000000 pxsecurityapi-0.0.0/src/pxsecurityapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-06 23:41:15.000000 pxsecurityapi-0.0.0/src/pxsecurityapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/
+-rw-rw-rw-   0        0        0      357 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxsecurityapi-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      528 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/src/pxsecurityapi/
+-rw-rw-rw-   0        0        0     1870 2023-07-06 22:49:22.000000 pxsecurityapi-1.0.2/src/pxsecurityapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/top_level.txt
```

### Comparing `pxsecurityapi-0.0.0/setup.cfg` & `pxsecurityapi-1.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7873 6563 7572 6974 7961 7069   = pxsecurityapi
-00000020: 0d0a 7665 7273 696f 6e20 3d20 0d0a 6175  ..version = ..au
-00000030: 7468 6f72 203d 2050 6f75 6e64 6578 2041  thor = Poundex A
-00000040: 7373 6f63 6961 7465 7320 436f 7270 6f72  ssociates Corpor
-00000050: 6174 696f 6e0d 0a61 7574 686f 725f 656d  ation..author_em
-00000060: 6169 6c20 3d20 6974 4070 6f75 6e64 6578  ail = it@poundex
-00000070: 2e63 6f6d 0d0a 6465 7363 7269 7074 696f  .com..descriptio
-00000080: 6e20 3d20 0d0a 6c6f 6e67 5f64 6573 6372  n = ..long_descr
-00000090: 6970 7469 6f6e 203d 200d 0a6c 6f6e 675f  iption = ..long_
-000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000b0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000c0: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-000000d0: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
-000000e0: 200d 0a63 6c61 7373 6966 6965 7273 203d   ..classifiers =
-000000f0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-00000100: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000110: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-00000120: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000130: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000140: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000150: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-00000160: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-00000170: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000180: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000190: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-000001a0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000001b0: 3e3d 332e 392e 3132 0d0a 0d0a 5b6f 7074  >=3.9.12....[opt
-000001c0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000001d0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-000001e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000001f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000200: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
+00000030: 320d 0a61 7574 686f 7220 3d20 506f 756e  2..author = Poun
+00000040: 6465 7820 4173 736f 6369 6174 6573 2043  dex Associates C
+00000050: 6f72 706f 7261 7469 6f6e 0d0a 6175 7468  orporation..auth
+00000060: 6f72 5f65 6d61 696c 203d 2069 7440 706f  or_email = it@po
+00000070: 756e 6465 782e 636f 6d0d 0a64 6573 6372  undex.com..descr
+00000080: 6970 7469 6f6e 203d 200d 0a6c 6f6e 675f  iption = ..long_
+00000090: 6465 7363 7269 7074 696f 6e20 3d20 0d0a  description = ..
+000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000b0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000c0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
+000000d0: 726c 203d 200d 0a70 726f 6a65 6374 5f75  rl = ..project_u
+000000e0: 726c 7320 3d20 0d0a 636c 6173 7369 6669  rls = ..classifi
+000000f0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+00000100: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000110: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
+00000120: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000130: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000140: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+00000150: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000160: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
+00000170: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+00000180: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
+00000190: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000001a0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+000001b0: 6573 203d 203e 3d33 2e39 0d0a 0d0a 5b6f  es = >=3.9....[o
+000001c0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000001d0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+000001e0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
+000001f0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000200: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `pxsecurityapi-0.0.0/src/pxsecurityapi/__init__.py` & `pxsecurityapi-1.0.2/src/pxsecurityapi/__init__.py`

 * *Files identical despite different names*

