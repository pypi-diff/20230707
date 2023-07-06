# Comparing `tmp/spectrum_io-0.2.1.tar.gz` & `tmp/spectrum_io-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_io-0.2.1.tar", max compression
+gzip compressed data, was "spectrum_io-0.3.0.tar", max compression
```

## Comparing `spectrum_io-0.2.1.tar` & `spectrum_io-0.3.0.tar`

### file list

```diff
@@ -1,89 +1,28 @@
--rw-r--r--   0        0        0     1072 2023-06-25 12:55:35.701807 spectrum_io-0.2.1/LICENSE
--rw-r--r--   0        0        0     2411 2023-06-25 12:55:35.701807 spectrum_io-0.2.1/README.rst
--rw-r--r--   0        0        0     2338 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1048 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/__init__.py
--rw-r--r--   0        0        0      351 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/__main__.py
--rw-r--r--   0        0        0      103 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/file/__init__.py
--rw-r--r--   0        0        0      556 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/file/csv.py
--rw-r--r--   0        0        0     5912 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/file/hdf5.py
--rw-r--r--   0        0        0        0 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/py.typed
--rw-r--r--   0        0        0      104 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/__init__.py
--rw-r--r--   0        0        0    11999 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/msraw.py
--rw-r--r--   0        0        0     3752 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/thermo_raw.py
--rwxr-xr-x   0        0        0    33200 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll
--rwxr-xr-x   0        0        0     5384 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb
--rwxr-xr-x   0        0        0    17827 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml
--rwxr-xr-x   0        0        0   136192 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll
--rwxr-xr-x   0        0        0    73260 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb
--rwxr-xr-x   0        0        0   607957 2023-06-25 12:55:35.709807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml
--rwxr-xr-x   0        0        0   904704 2023-06-25 12:55:35.713807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll
--rwxr-xr-x   0        0        0   245016 2023-06-25 12:55:35.717807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb
--rwxr-xr-x   0        0        0   726825 2023-06-25 12:55:35.717807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml
--rwxr-xr-x   0        0        0   636928 2023-06-25 12:55:35.721807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll
--rwxr-xr-x   0        0        0   281820 2023-06-25 12:55:35.725807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb
--rwxr-xr-x   0        0        0  1215406 2023-06-25 12:55:35.729807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml
--rwxr-xr-x   0        0        0    15360 2023-06-25 12:55:35.729807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll
--rw-r--r--   0        0        0    11324 2023-06-25 12:55:35.729807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE
--rwxr-xr-x   0        0        0  1689600 2023-06-25 12:55:35.737807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll
--rwxr-xr-x   0        0        0  3688730 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml
--rwxr-xr-x   0        0        0    45168 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll
--rwxr-xr-x   0        0        0   229376 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll
--rwxr-xr-x   0        0        0   181640 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml
--rwxr-xr-x   0        0        0    52224 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll
--rwxr-xr-x   0        0        0    40909 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml
--rwxr-xr-x   0        0        0   701992 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll
--rwxr-xr-x   0        0        0   698888 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml
--rwxr-xr-x   0        0        0    34304 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll
--rwxr-xr-x   0        0        0    61952 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll
--rwxr-xr-x   0        0        0    50343 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml
--rwxr-xr-x   0        0        0   159232 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll
--rwxr-xr-x   0        0        0    91970 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml
--rwxr-xr-x   0        0        0    20856 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll
--rwxr-xr-x   0        0        0     3445 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml
--rwxr-xr-x   0        0        0    28552 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll
--rwxr-xr-x   0        0        0    64416 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml
--rwxr-xr-x   0        0        0   141184 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll
--rwxr-xr-x   0        0        0    13585 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml
--rwxr-xr-x   0        0        0   115856 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll
--rwxr-xr-x   0        0        0   180815 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml
--rwxr-xr-x   0        0        0    16768 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll
--rwxr-xr-x   0        0        0    17733 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml
--rwxr-xr-x   0        0        0    33672 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll
--rwxr-xr-x   0        0        0   218987 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml
--rwxr-xr-x   0        0        0    18312 2023-06-25 12:55:35.765807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll
--rwxr-xr-x   0        0        0    89643 2023-06-25 12:55:35.765807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml
--rwxr-xr-x   0        0        0   758664 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll
--rwxr-xr-x   0        0        0     2048 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml
--rwxr-xr-x   0        0        0    25232 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll
--rwxr-xr-x   0        0        0      134 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.xml
--rw-r--r--   0        0        0     6509 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE
--rw-r--r--   0        0        0   404480 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll
--rw-r--r--   0        0        0  1433139 2023-06-25 12:55:35.781808 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml
--rw-r--r--   0        0        0   639488 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll
--rw-r--r--   0        0        0  1547413 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml
--rw-r--r--   0        0        0   174592 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe
--rw-r--r--   0        0        0     3096 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config
--rw-r--r--   0        0        0    56512 2023-06-25 12:55:35.789807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb
--rw-r--r--   0        0        0  4630427 2023-06-25 12:55:35.805807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip
--rw-r--r--   0        0        0      920 2023-06-25 12:55:35.805807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config
--rwxr-xr-x   0        0        0   270336 2023-06-25 12:55:35.805807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll
--rwxr-xr-x   0        0        0  1513051 2023-06-25 12:55:35.809807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml
--rwxr-xr-x   0        0        0   480768 2023-06-25 12:55:35.813807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll
--rwxr-xr-x   0        0        0  1086558 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml
--rwxr-xr-x   0        0        0    69632 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll
--rw-r--r--   0        0        0      122 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/__init__.py
--rw-r--r--   0        0        0     4410 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/mascot.py
--rw-r--r--   0        0        0     4507 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/maxquant.py
--rw-r--r--   0        0        0     4143 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/msamanda.py
--rw-r--r--   0        0        0     3634 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/msfragger.py
--rw-r--r--   0        0        0     2685 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/search_results.py
--rw-r--r--   0        0        0      191 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/__init__.py
--rw-r--r--   0        0        0    22118 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/digest.py
--rw-r--r--   0        0        0    45056 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/dlib/myPrositLib.dlib
--rw-r--r--   0        0        0     7918 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/dlib.py
--rw-r--r--   0        0        0    98385 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/msp/myPrositLib.msp
--rw-r--r--   0        0        0     3997 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/msp.py
--rw-r--r--   0        0        0     1148 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/spectral_library.py
--rw-r--r--   0        0        0   565091 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
--rw-r--r--   0        0        0     4999 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut.py
--rw-r--r--   0        0        0     3618 1970-01-01 00:00:00.000000 spectrum_io-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2409 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/README.rst
+-rw-r--r--   0        0        0     2338 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1048 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/__init__.py
+-rw-r--r--   0        0        0      351 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/__main__.py
+-rw-r--r--   0        0        0      103 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/file/__init__.py
+-rw-r--r--   0        0        0      556 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/file/csv.py
+-rw-r--r--   0        0        0     5912 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/file/hdf5.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/py.typed
+-rw-r--r--   0        0        0      104 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/raw/__init__.py
+-rw-r--r--   0        0        0    11999 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/raw/msraw.py
+-rw-r--r--   0        0        0     3897 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/raw/thermo_raw.py
+-rw-r--r--   0        0        0      122 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/search_result/__init__.py
+-rw-r--r--   0        0        0     4410 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/search_result/mascot.py
+-rw-r--r--   0        0        0     4507 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/search_result/maxquant.py
+-rw-r--r--   0        0        0     4143 2023-07-06 22:36:36.836306 spectrum_io-0.3.0/spectrum_io/search_result/msamanda.py
+-rw-r--r--   0        0        0     3634 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/search_result/msfragger.py
+-rw-r--r--   0        0        0     2685 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/search_result/search_results.py
+-rw-r--r--   0        0        0      191 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/__init__.py
+-rw-r--r--   0        0        0    22168 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/digest.py
+-rw-r--r--   0        0        0    45056 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib
+-rw-r--r--   0        0        0     7918 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/dlib.py
+-rw-r--r--   0        0        0    98385 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/msp/myPrositLib.msp
+-rw-r--r--   0        0        0     3997 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/msp.py
+-rw-r--r--   0        0        0     1148 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/spectral_library.py
+-rw-r--r--   0        0        0   565091 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
+-rw-r--r--   0        0        0     4999 2023-07-06 22:36:36.840306 spectrum_io-0.3.0/spectrum_io/spectral_library/spectronaut.py
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 spectrum_io-0.3.0/PKG-INFO
```

### Comparing `spectrum_io-0.2.1/LICENSE` & `spectrum_io-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/README.rst` & `spectrum_io-0.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -75,77 +75,77 @@
 000004a0: 6f6e 733f 776f 726b 666c 6f77 3d54 6573  ons?workflow=Tes
 000004b0: 7473 0a20 2020 3a61 6c74 3a20 5275 6e20  ts.   :alt: Run 
 000004c0: 5465 7374 7320 5374 6174 7573 0a2e 2e20  Tests Status... 
 000004d0: 7c43 6f64 6563 6f76 7c20 696d 6167 653a  |Codecov| image:
 000004e0: 3a20 6874 7470 733a 2f2f 636f 6465 636f  : https://codeco
 000004f0: 762e 696f 2f67 682f 7769 6c68 656c 6d2d  v.io/gh/wilhelm-
 00000500: 6c61 622f 7370 6563 7472 756d 5f69 6f2f  lab/spectrum_io/
-00000510: 6272 616e 6368 2f6d 6173 7465 722f 6772  branch/master/gr
-00000520: 6170 682f 6261 6467 652e 7376 670a 2020  aph/badge.svg.  
-00000530: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000540: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-00000550: 7769 6c68 656c 6d2d 6c61 622f 7370 6563  wilhelm-lab/spec
-00000560: 7472 756d 5f69 6f0a 2020 203a 616c 743a  trum_io.   :alt:
-00000570: 2043 6f64 6563 6f76 0a2e 2e20 7c70 7265   Codecov... |pre
-00000580: 2d63 6f6d 6d69 747c 2069 6d61 6765 3a3a  -commit| image::
-00000590: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
-000005a0: 656c 6473 2e69 6f2f 6261 6467 652f 7072  elds.io/badge/pr
-000005b0: 652d 2d63 6f6d 6d69 742d 656e 6162 6c65  e--commit-enable
-000005c0: 642d 6272 6967 6874 6772 6565 6e3f 6c6f  d-brightgreen?lo
-000005d0: 676f 3d70 7265 2d63 6f6d 6d69 7426 6c6f  go=pre-commit&lo
-000005e0: 676f 436f 6c6f 723d 7768 6974 650a 2020  goColor=white.  
-000005f0: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000600: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7265  //github.com/pre
-00000610: 2d63 6f6d 6d69 742f 7072 652d 636f 6d6d  -commit/pre-comm
-00000620: 6974 0a20 2020 3a61 6c74 3a20 7072 652d  it.   :alt: pre-
-00000630: 636f 6d6d 6974 0a2e 2e20 7c42 6c61 636b  commit... |Black
-00000640: 7c20 696d 6167 653a 3a20 6874 7470 733a  | image:: https:
-00000650: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000660: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000670: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
-00000680: 2e73 7667 0a20 2020 3a74 6172 6765 743a  .svg.   :target:
-00000690: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000006a0: 636f 6d2f 7073 662f 626c 6163 6b0a 2020  com/psf/black.  
-000006b0: 203a 616c 743a 2042 6c61 636b 0a0a 0a46   :alt: Black...F
-000006c0: 6561 7475 7265 730a 2d2d 2d2d 2d2d 2d2d  eatures.--------
-000006d0: 0a0a 2a20 544f 444f 0a0a 0a49 6e73 7461  ..* TODO...Insta
-000006e0: 6c6c 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d  llation.--------
-000006f0: 2d2d 2d2d 0a0a 596f 7520 6361 6e20 696e  ----..You can in
-00000700: 7374 616c 6c20 2a73 7065 6374 7275 6d5f  stall *spectrum_
-00000710: 696f 2a20 7669 6120 7069 705f 2066 726f  io* via pip_ fro
-00000720: 6d20 5079 5049 5f3a 0a0a 2e2e 2063 6f64  m PyPI_:.... cod
-00000730: 653a 3a20 636f 6e73 6f6c 650a 0a20 2020  e:: console..   
-00000740: 2420 7069 7020 696e 7374 616c 6c20 7370  $ pip install sp
-00000750: 6563 7472 756d 5f69 6f0a 0a0a 5573 6167  ectrum_io...Usag
-00000760: 650a 2d2d 2d2d 2d0a 0a50 6c65 6173 6520  e.-----..Please 
-00000770: 7365 6520 7468 6520 6043 6f6d 6d61 6e64  see the `Command
-00000780: 2d6c 696e 6520 5265 6665 7265 6e63 6520  -line Reference 
-00000790: 3c55 7361 6765 5f3e 605f 2066 6f72 2064  <Usage_>`_ for d
-000007a0: 6574 6169 6c73 2e0a 0a0a 4372 6564 6974  etails....Credit
-000007b0: 730a 2d2d 2d2d 2d2d 2d0a 0a54 6869 7320  s.-------..This 
-000007c0: 7061 636b 6167 6520 7761 7320 6372 6561  package was crea
-000007d0: 7465 6420 7769 7468 2063 6f6f 6b69 6574  ted with cookiet
-000007e0: 656d 706c 655f 2075 7369 6e67 2043 6f6f  emple_ using Coo
-000007f0: 6b69 6563 7574 7465 725f 2062 6173 6564  kiecutter_ based
-00000800: 206f 6e20 4879 7065 726d 6f64 6572 6e5f   on Hypermodern_
-00000810: 5079 7468 6f6e 5f43 6f6f 6b69 6563 7574  Python_Cookiecut
-00000820: 7465 725f 2e0a 0a2e 2e20 5f63 6f6f 6b69  ter_..... _cooki
-00000830: 6574 656d 706c 653a 2068 7474 7073 3a2f  etemple: https:/
-00000840: 2f63 6f6f 6b69 6574 656d 706c 652e 636f  /cookietemple.co
-00000850: 6d0a 2e2e 205f 436f 6f6b 6965 6375 7474  m... _Cookiecutt
-00000860: 6572 3a20 6874 7470 733a 2f2f 6769 7468  er: https://gith
-00000870: 7562 2e63 6f6d 2f61 7564 7265 7972 2f63  ub.com/audreyr/c
-00000880: 6f6f 6b69 6563 7574 7465 720a 2e2e 205f  ookiecutter... _
-00000890: 5079 5049 3a20 6874 7470 733a 2f2f 7079  PyPI: https://py
-000008a0: 7069 2e6f 7267 2f0a 2e2e 205f 4879 7065  pi.org/... _Hype
-000008b0: 726d 6f64 6572 6e5f 5079 7468 6f6e 5f43  rmodern_Python_C
-000008c0: 6f6f 6b69 6563 7574 7465 723a 2068 7474  ookiecutter: htt
-000008d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000008e0: 636a 6f6c 6f77 6963 7a2f 636f 6f6b 6965  cjolowicz/cookie
-000008f0: 6375 7474 6572 2d68 7970 6572 6d6f 6465  cutter-hypermode
-00000900: 726e 2d70 7974 686f 6e0a 2e2e 205f 7069  rn-python... _pi
-00000910: 703a 2068 7474 7073 3a2f 2f70 6970 2e70  p: https://pip.p
-00000920: 7970 612e 696f 2f0a 2e2e 205f 5573 6167  ypa.io/... _Usag
-00000930: 653a 2068 7474 7073 3a2f 2f73 7065 6374  e: https://spect
-00000940: 7275 6d5f 696f 2e72 6561 6474 6865 646f  rum_io.readthedo
-00000950: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00000960: 7573 6167 652e 6874 6d6c 0a              usage.html.
+00000510: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
+00000520: 682f 6261 6467 652e 7376 670a 2020 203a  h/badge.svg.   :
+00000530: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
+00000540: 636f 6465 636f 762e 696f 2f67 682f 7769  codecov.io/gh/wi
+00000550: 6c68 656c 6d2d 6c61 622f 7370 6563 7472  lhelm-lab/spectr
+00000560: 756d 5f69 6f0a 2020 203a 616c 743a 2043  um_io.   :alt: C
+00000570: 6f64 6563 6f76 0a2e 2e20 7c70 7265 2d63  odecov... |pre-c
+00000580: 6f6d 6d69 747c 2069 6d61 6765 3a3a 2068  ommit| image:: h
+00000590: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000005a0: 6473 2e69 6f2f 6261 6467 652f 7072 652d  ds.io/badge/pre-
+000005b0: 2d63 6f6d 6d69 742d 656e 6162 6c65 642d  -commit-enabled-
+000005c0: 6272 6967 6874 6772 6565 6e3f 6c6f 676f  brightgreen?logo
+000005d0: 3d70 7265 2d63 6f6d 6d69 7426 6c6f 676f  =pre-commit&logo
+000005e0: 436f 6c6f 723d 7768 6974 650a 2020 203a  Color=white.   :
+000005f0: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
+00000600: 6769 7468 7562 2e63 6f6d 2f70 7265 2d63  github.com/pre-c
+00000610: 6f6d 6d69 742f 7072 652d 636f 6d6d 6974  ommit/pre-commit
+00000620: 0a20 2020 3a61 6c74 3a20 7072 652d 636f  .   :alt: pre-co
+00000630: 6d6d 6974 0a2e 2e20 7c42 6c61 636b 7c20  mmit... |Black| 
+00000640: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
+00000650: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000660: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
+00000670: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
+00000680: 7667 0a20 2020 3a74 6172 6765 743a 2068  vg.   :target: h
+00000690: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006a0: 6d2f 7073 662f 626c 6163 6b0a 2020 203a  m/psf/black.   :
+000006b0: 616c 743a 2042 6c61 636b 0a0a 0a46 6561  alt: Black...Fea
+000006c0: 7475 7265 730a 2d2d 2d2d 2d2d 2d2d 0a0a  tures.--------..
+000006d0: 2a20 544f 444f 0a0a 0a49 6e73 7461 6c6c  * TODO...Install
+000006e0: 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d  ation.----------
+000006f0: 2d2d 0a0a 596f 7520 6361 6e20 696e 7374  --..You can inst
+00000700: 616c 6c20 2a73 7065 6374 7275 6d5f 696f  all *spectrum_io
+00000710: 2a20 7669 6120 7069 705f 2066 726f 6d20  * via pip_ from 
+00000720: 5079 5049 5f3a 0a0a 2e2e 2063 6f64 653a  PyPI_:.... code:
+00000730: 3a20 636f 6e73 6f6c 650a 0a20 2020 2420  : console..   $ 
+00000740: 7069 7020 696e 7374 616c 6c20 7370 6563  pip install spec
+00000750: 7472 756d 5f69 6f0a 0a0a 5573 6167 650a  trum_io...Usage.
+00000760: 2d2d 2d2d 2d0a 0a50 6c65 6173 6520 7365  -----..Please se
+00000770: 6520 7468 6520 6043 6f6d 6d61 6e64 2d6c  e the `Command-l
+00000780: 696e 6520 5265 6665 7265 6e63 6520 3c55  ine Reference <U
+00000790: 7361 6765 5f3e 605f 2066 6f72 2064 6574  sage_>`_ for det
+000007a0: 6169 6c73 2e0a 0a0a 4372 6564 6974 730a  ails....Credits.
+000007b0: 2d2d 2d2d 2d2d 2d0a 0a54 6869 7320 7061  -------..This pa
+000007c0: 636b 6167 6520 7761 7320 6372 6561 7465  ckage was create
+000007d0: 6420 7769 7468 2063 6f6f 6b69 6574 656d  d with cookietem
+000007e0: 706c 655f 2075 7369 6e67 2043 6f6f 6b69  ple_ using Cooki
+000007f0: 6563 7574 7465 725f 2062 6173 6564 206f  ecutter_ based o
+00000800: 6e20 4879 7065 726d 6f64 6572 6e5f 5079  n Hypermodern_Py
+00000810: 7468 6f6e 5f43 6f6f 6b69 6563 7574 7465  thon_Cookiecutte
+00000820: 725f 2e0a 0a2e 2e20 5f63 6f6f 6b69 6574  r_..... _cookiet
+00000830: 656d 706c 653a 2068 7474 7073 3a2f 2f63  emple: https://c
+00000840: 6f6f 6b69 6574 656d 706c 652e 636f 6d0a  ookietemple.com.
+00000850: 2e2e 205f 436f 6f6b 6965 6375 7474 6572  .. _Cookiecutter
+00000860: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000870: 2e63 6f6d 2f61 7564 7265 7972 2f63 6f6f  .com/audreyr/coo
+00000880: 6b69 6563 7574 7465 720a 2e2e 205f 5079  kiecutter... _Py
+00000890: 5049 3a20 6874 7470 733a 2f2f 7079 7069  PI: https://pypi
+000008a0: 2e6f 7267 2f0a 2e2e 205f 4879 7065 726d  .org/... _Hyperm
+000008b0: 6f64 6572 6e5f 5079 7468 6f6e 5f43 6f6f  odern_Python_Coo
+000008c0: 6b69 6563 7574 7465 723a 2068 7474 7073  kiecutter: https
+000008d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 636a  ://github.com/cj
+000008e0: 6f6c 6f77 6963 7a2f 636f 6f6b 6965 6375  olowicz/cookiecu
+000008f0: 7474 6572 2d68 7970 6572 6d6f 6465 726e  tter-hypermodern
+00000900: 2d70 7974 686f 6e0a 2e2e 205f 7069 703a  -python... _pip:
+00000910: 2068 7474 7073 3a2f 2f70 6970 2e70 7970   https://pip.pyp
+00000920: 612e 696f 2f0a 2e2e 205f 5573 6167 653a  a.io/... _Usage:
+00000930: 2068 7474 7073 3a2f 2f73 7065 6374 7275   https://spectru
+00000940: 6d5f 696f 2e72 6561 6474 6865 646f 6373  m_io.readthedocs
+00000950: 2e69 6f2f 656e 2f6c 6174 6573 742f 7573  .io/en/latest/us
+00000960: 6167 652e 6874 6d6c 0a                   age.html.
```

### Comparing `spectrum_io-0.2.1/pyproject.toml` & `spectrum_io-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_io"
-version = "0.2.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.3.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "IO related functionalities for oktoberfest."
 authors = ["Mario Picciani <mario.picciani@tum.de>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_io"
 repository = "https://github.com/wilhelm-lab/spectrum_io"
 documentation = "https://spectrum_io.readthedocs.io"
```

### Comparing `spectrum_io-0.2.1/spectrum_io/__init__.py` & `spectrum_io-0.3.0/spectrum_io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for spectrum_io."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 from . import file, raw
```

### Comparing `spectrum_io-0.2.1/spectrum_io/file/csv.py` & `spectrum_io-0.3.0/spectrum_io/file/csv.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/file/hdf5.py` & `spectrum_io-0.3.0/spectrum_io/file/hdf5.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/raw/msraw.py` & `spectrum_io-0.3.0/spectrum_io/raw/msraw.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/raw/thermo_raw.py` & `spectrum_io-0.3.0/spectrum_io/raw/thermo_raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,19 @@
         possible_types_str = types.__name__
     else:
         type_names = [t.__name__ for t in types]
         possible_types_str = "{} or {}".format(", ".join(type_names[:-1]), type_names[-1])
     raise TypeError(f"{varname} must be of type {possible_types_str}")
 
 
-def _assemble_arg_list(input_path: Path, output_path: Path, ms_level: List[int], gzip: bool) -> List[Union[str, Path]]:
-    exec_path = Path(__file__).parent.absolute()  # get path of parent directory of this file
-    exec_path /= "utils/ThermoRawFileParser/ThermoRawFileParser.exe"
+def _assemble_arg_list(
+    input_path: Path, output_path: Path, ms_level: List[int], gzip: bool, thermo_exe: Path
+) -> List[Union[str, Path]]:
     exec_arg_list: List[Union[str, Path]] = [
-        exec_path,
+        thermo_exe,
         f"--msLevel={','.join([str(l) for l in ms_level])}",
         "-i",
         input_path.resolve(),
         "-b",
         output_path,
     ]
     if gzip:
@@ -44,47 +44,52 @@
 
     @staticmethod
     def convert_raw_mzml(
         input_path: Union[Path, str],
         gzip: bool = False,
         ms_level: Union[int, List[int]] = 2,
         output_path: Optional[Union[Path, str]] = None,
+        thermo_exe: Union[Path, str] = "ThermoRawFileParser.exe",
     ) -> Path:
         """Converts a ThermoRaw file to mzML.
 
         Use https://github.com/compomics/ThermoRawFileParser for conversion.
 
         :param input_path: file path of the Thermo Rawfile
         :param gzip: whether to gzip the file
         :param ms_level: level of MS, can be a single integer (1, 2, 3) or any combination of that provided as a list
         :param output_path: file path of the mzML path
+        :param thermo_exe: path to the executable of ThermoRawFileParser. Default: ThermoRawFileParser.exe
         :raises subprocess.CalledProcessError: if the subprocess for conversion failed
         :raises ValueError: if ms_level(s) provided are other than 1, 2 or 3.
         :return: path to converted file as string
         """
         _type_check(input_path, "input_path", (Path, str))
         input_path = Path(input_path)
         if output_path is None:
             output_path = input_path.with_suffix(".mzML")
         _type_check(output_path, "output_path", (Path, str))
         output_path = Path(output_path)
 
+        _type_check(thermo_exe, "thermo_exe", (Path, str))
+        thermo_exe = Path(thermo_exe)
+
         _type_check(ms_level, "ms_level", (int, list))
         if isinstance(ms_level, int):
             ms_level = [ms_level]
         for level in ms_level:
             _type_check(level, "all ms_levels in list", int)
             if not 1 <= level <= 3:
                 raise ValueError(f"Value of all ms_levels must be within [1,3]. Got {level}")
 
         if output_path.is_file():
             logger.info(f"Found converted file at {output_path}, skipping conversion")
             return output_path
 
-        exec_arg_list = _assemble_arg_list(input_path, output_path, ms_level, gzip)
+        exec_arg_list = _assemble_arg_list(input_path, output_path, ms_level, gzip, thermo_exe)
 
         logger.info(
             f"Converting thermo rawfile to mzml with the command: {' '.join([str(arg) for arg in exec_arg_list])}"
         )
 
         try:
             subprocess.run(exec_arg_list, shell=False, check=True)
```

### Comparing `spectrum_io-0.2.1/spectrum_io/search_result/mascot.py` & `spectrum_io-0.3.0/spectrum_io/search_result/mascot.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/search_result/maxquant.py` & `spectrum_io-0.3.0/spectrum_io/search_result/maxquant.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/search_result/msamanda.py` & `spectrum_io-0.3.0/spectrum_io/search_result/msamanda.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/search_result/msfragger.py` & `spectrum_io-0.3.0/spectrum_io/search_result/msfragger.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/search_result/search_results.py` & `spectrum_io-0.3.0/spectrum_io/search_result/search_results.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/digest.py` & `spectrum_io-0.3.0/spectrum_io/spectral_library/digest.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     # 10090_UP000000589_UniProtKB_Mouse_CanIso_2018_03_27.fasta
     # --peptide_protein_map ../data/fasta/10090_UP000000589_UniProtKB_Mouse_CanIso_2018_03_27.peptide_to_protein_map.txt
     if args.peptide_protein_map:
         with open(args.peptide_protein_map + ".params.txt", "w") as f:
             f.write(" ".join(sys.argv))
         writer = get_tsv_writer(args.peptide_protein_map, delimiter="\t")
 
-        pre, not_post = cleavage_sites(args.enzyme)
+        pre, not_post = cleavage_sites[args.enzyme]
         for peptide, proteins in get_peptide_to_protein_map(
             args.fasta,
             db="concat",
             digestion=args.digestion,
             min_len=args.min_length,
             max_len=args.max_length,
             pre=pre,
@@ -279,35 +279,33 @@
     """Read fasta maxquant."""
     if special_aas is None:
         special_aas = ["K", "R"]
     if db not in ["target", "decoy", "concat"]:
         sys.exit("unknown db mode: %s" % db)
 
     hasspecial_aas = len(special_aas) > 0
-    name = None
-    seq: List[str] = []
     with open(file_path) as fp:
+        line = next(fp).rstrip()
+        name = parse_id(line[1:])
+        sequence_lines: List[str] = []
         for line in itertools.chain(fp, [">"]):
             line = line.rstrip()
             if line.startswith(">"):
-                if name:
-                    seq = ["".join(seq)]
-                    if db in ["target", "concat"]:
-                        yield (name, seq)
-
-                    if db in ["decoy", "concat"]:
-                        rev_seq = seq[::-1]
-                        if hasspecial_aas:
-                            rev_seq = swap_special_aas(rev_seq, special_aas)
-                        yield (decoy_prefix + name, rev_seq)
-
-                if len(line) > 1:
-                    name, seq = parse_id(line[1:]), []
-            else:
-                seq.append(line)
+                sequence = "".join(sequence_lines)
+                if db in ["target", "concat"]:
+                    yield name, sequence
+                if db in ["decoy", "concat"]:
+                    rev_sequence = sequence[::-1]
+                    if hasspecial_aas:
+                        rev_sequence = swap_special_aas(rev_sequence, special_aas)
+                    yield decoy_prefix + name, rev_sequence
+                name = parse_id(line[1:])
+                sequence_lines = []
+                continue
+            sequence_lines.append(line)
 
 
 read_fasta = read_fasta_maxquant
 
 
 # e.g. special_aas = ['R', 'K'] transforms ABCKDEFRK into ABKCDERKF
 def swap_special_aas(seq, special_aas):
```

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/dlib/myPrositLib.dlib` & `spectrum_io-0.3.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/dlib.py` & `spectrum_io-0.3.0/spectrum_io/spectral_library/dlib.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/msp/myPrositLib.msp` & `spectrum_io-0.3.0/spectrum_io/spectral_library/msp/myPrositLib.msp`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/msp.py` & `spectrum_io-0.3.0/spectrum_io/spectral_library/msp.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/spectral_library.py` & `spectrum_io-0.3.0/spectrum_io/spectral_library/spectral_library.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut/myPrositLib.csv` & `spectrum_io-0.3.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut.py` & `spectrum_io-0.3.0/spectrum_io/spectral_library/spectronaut.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.1/PKG-INFO` & `spectrum_io-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-io
-Version: 0.2.1
+Version: 0.3.0
 Summary: IO related functionalities for oktoberfest.
 Home-page: https://github.com/wilhelm-lab/spectrum_io
 License: MIT
 Author: Mario Picciani
 Author-email: mario.picciani@tum.de
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -48,15 +48,15 @@
    :alt: Read the documentation at https://spectrum_io.readthedocs.io/
 .. |Build| image:: https://github.com/wilhelm-lab/spectrum_io/workflows/Build%20spectrum_io%20Package/badge.svg
    :target: https://github.com/wilhelm-lab/spectrum_io/actions?workflow=Package
    :alt: Build Package Status
 .. |Tests| image:: https://github.com/wilhelm-lab/spectrum_io/workflows/Run%20spectrum_io%20Tests/badge.svg
    :target: https://github.com/wilhelm-lab/spectrum_io/actions?workflow=Tests
    :alt: Run Tests Status
-.. |Codecov| image:: https://codecov.io/gh/wilhelm-lab/spectrum_io/branch/master/graph/badge.svg
+.. |Codecov| image:: https://codecov.io/gh/wilhelm-lab/spectrum_io/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/wilhelm-lab/spectrum_io
    :alt: Codecov
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

