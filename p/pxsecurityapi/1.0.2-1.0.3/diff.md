# Comparing `tmp/pxsecurityapi-1.0.2.tar.gz` & `tmp/pxsecurityapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxsecurityapi-1.0.2.tar", last modified: Thu Jul  6 23:49:57 2023, max compression
+gzip compressed data, was "pxsecurityapi-1.0.3.tar", last modified: Thu Jul  6 23:51:58 2023, max compression
```

## Comparing `pxsecurityapi-1.0.2.tar` & `pxsecurityapi-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/
--rw-rw-rw-   0        0        0      357 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxsecurityapi-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      528 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/src/pxsecurityapi/
--rw-rw-rw-   0        0        0     1870 2023-07-06 22:49:22.000000 pxsecurityapi-1.0.2/src/pxsecurityapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 23:49:57.545585 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/
--rw-rw-rw-   0        0        0      357 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-06 23:49:57.000000 pxsecurityapi-1.0.2/src/pxsecurityapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/
+-rw-rw-rw-   0        0        0      333 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxsecurityapi-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      523 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.066502 pxsecurityapi-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.066502 pxsecurityapi-1.0.3/src/pxsecurityapi/
+-rw-rw-rw-   0        0        0     1870 2023-07-06 22:49:22.000000 pxsecurityapi-1.0.3/src/pxsecurityapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/
+-rw-rw-rw-   0        0        0      333 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/top_level.txt
```

### Comparing `pxsecurityapi-1.0.2/setup.cfg` & `pxsecurityapi-1.0.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7873 6563 7572 6974 7961 7069   = pxsecurityapi
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 320d 0a61 7574 686f 7220 3d20 506f 756e  2..author = Poun
+00000030: 330d 0a61 7574 686f 7220 3d20 506f 756e  3..author = Poun
 00000040: 6465 7820 4173 736f 6369 6174 6573 2043  dex Associates C
 00000050: 6f72 706f 7261 7469 6f6e 0d0a 6175 7468  orporation..auth
 00000060: 6f72 5f65 6d61 696c 203d 2069 7440 706f  or_email = it@po
 00000070: 756e 6465 782e 636f 6d0d 0a64 6573 6372  undex.com..descr
 00000080: 6970 7469 6f6e 203d 200d 0a6c 6f6e 675f  iption = ..long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 0d0a  description = ..
 000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
@@ -21,13 +21,13 @@
 00000140: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
 00000150: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 00000160: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
 00000170: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
 00000180: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
 00000190: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
 000001a0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-000001b0: 6573 203d 203e 3d33 2e39 0d0a 0d0a 5b6f  es = >=3.9....[o
-000001c0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-000001d0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-000001e0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
-000001f0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000200: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000001b0: 6573 203d 200d 0a0d 0a5b 6f70 7469 6f6e  es = ....[option
+000001c0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000001d0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+000001e0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000001f0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000200: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `pxsecurityapi-1.0.2/src/pxsecurityapi/__init__.py` & `pxsecurityapi-1.0.3/src/pxsecurityapi/__init__.py`

 * *Files identical despite different names*

