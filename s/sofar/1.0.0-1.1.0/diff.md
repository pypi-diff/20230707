# Comparing `tmp/sofar-1.0.0.tar.gz` & `tmp/sofar-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sofar-1.0.0.tar", last modified: Fri Dec 16 14:22:47 2022, max compression
+gzip compressed data, was "sofar-1.1.0.tar", last modified: Fri Jul  7 09:12:11 2023, max compression
```

## Comparing `sofar-1.0.0.tar` & `sofar-1.1.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2022-12-16 14:22:34.000000 sofar-1.0.0/AUTHORS.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7512 2022-12-16 14:22:34.000000 sofar-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3149 2022-12-16 14:22:34.000000 sofar-1.0.0/HISTORY.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2022-12-16 14:22:34.000000 sofar-1.0.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2022-12-16 14:22:34.000000 sofar-1.0.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3032 2022-12-16 14:22:47.342573 sofar-1.0.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2022-12-16 14:22:34.000000 sofar-1.0.0/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2022-12-16 14:22:47.342573 sofar-1.0.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1773 2022-12-16 14:22:34.000000 sofar-1.0.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.334573 sofar-1.0.0/sofar/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13867 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    67185 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/sofa.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.334573 sofar-1.0.0/sofar/sofa_conventions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/VERSION
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.338573 sofar-1.0.0/sofar/sofa_conventions/conventions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5125 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12627 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5510 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13138 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2479 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8127 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1998 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6615 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2130 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7357 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6757 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6696 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1957 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6699 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2239 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8446 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2303 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8254 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7791 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8249 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9863 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4053 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14346 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4199 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14491 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6603 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2560 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8884 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2093 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7704 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1989 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7770 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2028 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7770 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3153 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9870 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3153 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9870 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2045 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8097 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1999 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8097 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/sofar/sofa_conventions/rules/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/deprecations.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22501 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/rules.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/unit_aliases.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4054 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/upgrade.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16193 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/update_conventions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11527 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.334573 sofar-1.0.0/sofar.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3032 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4003 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11682 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11415 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_sofa.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3038 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_sofa_upgrade_conventions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15641 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_sofa_verify.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7930 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.039065 sofar-1.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-07-07 09:11:51.000000 sofar-1.1.0/AUTHORS.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7571 2023-07-07 09:11:51.000000 sofar-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3652 2023-07-07 09:11:51.000000 sofar-1.1.0/HISTORY.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-07-07 09:11:51.000000 sofar-1.1.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-07-07 09:11:51.000000 sofar-1.1.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-07 09:12:11.039065 sofar-1.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2084 2023-07-07 09:11:51.000000 sofar-1.1.0/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2023-07-07 09:12:11.039065 sofar-1.1.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1823 2023-07-07 09:11:51.000000 sofar-1.1.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.011064 sofar-1.1.0/sofar/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      595 2023-07-07 09:11:51.000000 sofar-1.1.0/sofar/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15761 2023-07-07 09:11:51.000000 sofar-1.1.0/sofar/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    68255 2023-07-07 09:11:51.000000 sofar-1.1.0/sofar/sofa.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.011064 sofar-1.1.0/sofar/sofa_conventions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/VERSION
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.015064 sofar-1.1.0/sofar/sofa_conventions/conventions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5510 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13138 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8127 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1998 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6615 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2130 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7357 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6757 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6696 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1957 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6699 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2239 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8446 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2303 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8254 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7791 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8249 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9863 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4053 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14346 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4199 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14491 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.035065 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5125 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/FreeFieldDirectivityTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12627 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/FreeFieldDirectivityTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6603 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2560 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8884 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2093 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7704 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1989 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7770 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2028 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7770 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3153 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9870 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3153 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9870 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2045 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8097 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1999 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8097 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.035065 sofar-1.1.0/sofar/sofa_conventions/rules/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/rules/deprecations.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22501 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/rules/rules.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/rules/unit_aliases.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar/sofa_conventions/rules/upgrade.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16753 2023-07-07 09:11:51.000000 sofar-1.1.0/sofar/update_conventions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10754 2023-07-07 09:11:51.000000 sofar-1.1.0/sofar/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.011064 sofar-1.1.0/sofar.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4052 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-07-07 09:12:10.000000 sofar-1.1.0/sofar.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:12:11.039065 sofar-1.1.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-07 09:11:51.000000 sofar-1.1.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-07-07 09:11:51.000000 sofar-1.1.0/tests/test_deprecations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11808 2023-07-07 09:11:51.000000 sofar-1.1.0/tests/test_io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11314 2023-07-07 09:11:51.000000 sofar-1.1.0/tests/test_sofa.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3377 2023-07-07 09:11:51.000000 sofar-1.1.0/tests/test_sofa_upgrade_conventions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15631 2023-07-07 09:11:51.000000 sofar-1.1.0/tests/test_sofa_verify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8307 2023-07-07 09:11:51.000000 sofar-1.1.0/tests/test_utils.py
```

### Comparing `sofar-1.0.0/CONTRIBUTING.rst` & `sofar-1.1.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -174,17 +174,20 @@
 
 before building the documentation.
 
 
 Submodules
 ~~~~~~~~~~
 
-To update the submodules containing the conventions and verification rules run
+To update the submodule containing the conventions and verification rules run
 
-$ git submodule update --remote sofar/sofa_conventions
+$ git submodule update --init --recursive
+$ git submodule update --recursive --remote
+
+and then commit the changes
 
 
 Deploying
 ~~~~~~~~~
 
 A reminder for the maintainers on how to deploy.
```

### Comparing `sofar-1.0.0/HISTORY.rst` & `sofar-1.1.0/HISTORY.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 History
 =======
 
+1.1.0 (2023-7-7)
+----------------
+* Deprecate FreeFieldDirectivityTV 1.0 in favor of FreeFieldDirectivityTV 1.1 (according to sofaconventoins.org and AES69-2022)
+* Add `sofar.read_sofa_as_netcdf` for reading SOFA files with erroneous data
+* Document SOFA conventions on https://sofar.readthedocs.io/en/stable/resources/conventions.html. `Sofa.info()` will this be deprecated in sofar v1.3.0
+* `sofar.read_sofa` and `sofar.write_sofa` now accept filenames and path objects
+* Add testing for Python 3.11
+
 1.0.0 (2022-12-16)
 ------------------
 * Use SOFA conventions of version 2.1 from https://github.com/pyfar/sofa_conventions
 * Verify SOFA data against all rules defined in the SOFA standard AES69-2022
 * Add `Sofa.upgrade_convention` for upgrading outdated conventions. This now uses explicit upgrade rules from https://github.com/pyfar/sofa_conventions
 * Remove upgrade functionality from `Sofa.verify`, `sofar.write_sofa`, and `sofar.read_sofa` for a more clear separation of functionality
 * Add `Sofa.add_missing` to add missing default data to a SOFA object using the default values specified by the SOFA convention
```

### Comparing `sofar-1.0.0/LICENSE` & `sofar-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/PKG-INFO` & `sofar-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sofar
-Version: 1.0.0
+Version: 1.1.0
 Summary: Maybe the most complete python package for SOFA files so far
 Home-page: https://pyfar.org/
+Download-URL: https://pypi.org/project/sofar/
 Author: The pyfar developers
 Author-email: info@pyfar.org
 License: MIT license
-Download-URL: https://pypi.org/project/sofar/
 Project-URL: Bug Tracker, https://github.com/pyfar/sofar/issues
 Project-URL: Documentation, https://sofar.readthedocs.io/
 Project-URL: Source Code, https://github.com/pyfar/sofar
 Keywords: sofar
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======
 Readme
 ======
@@ -77,11 +77,9 @@
 
 AES69-2022: *AES standard for file exchange - Spatial acoustic data file
 format*, Audio Engineering Society, Inc., New York, NY, USA.
 (https://www.aes.org/publications/standards/search.cfm?docID=99)
 
 P. Majdak, F. Zotter, F. Brinkmann, J. De Muynke, M. Mihocic, and M.
 Noisternig, "Spatially Oriented Format for Acoustics 2.1: Introduction and
-Recent Advances,” *J. Audio Eng. Soc.*, vol. 70, no. 7/8, pp. 565–584,
+Recent Advances", *J. Audio Eng. Soc.*, vol. 70, no. 7/8, pp. 565-584,
 Jul. 2022. DOI: https://doi.org/10.17743/jaes.2022.0026
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sofar-1.0.0/README.rst` & `sofar-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 
 AES69-2022: *AES standard for file exchange - Spatial acoustic data file
 format*, Audio Engineering Society, Inc., New York, NY, USA.
 (https://www.aes.org/publications/standards/search.cfm?docID=99)
 
 P. Majdak, F. Zotter, F. Brinkmann, J. De Muynke, M. Mihocic, and M.
 Noisternig, "Spatially Oriented Format for Acoustics 2.1: Introduction and
-Recent Advances,” *J. Audio Eng. Soc.*, vol. 70, no. 7/8, pp. 565–584,
+Recent Advances", *J. Audio Eng. Soc.*, vol. 70, no. 7/8, pp. 565-584,
 Jul. 2022. DOI: https://doi.org/10.17743/jaes.2022.0026
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sofar-1.0.0/setup.py` & `sofar-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     description="Maybe the most complete python package for SOFA files so far",
     install_requires=requirements,
     license="MIT license",
     long_description=readme,
     include_package_data=True,
     keywords='sofar',
@@ -60,11 +61,11 @@
     url="https://pyfar.org/",
     download_url="https://pypi.org/project/sofar/",
     project_urls={
         "Bug Tracker": "https://github.com/pyfar/sofar/issues",
         "Documentation": "https://sofar.readthedocs.io/",
         "Source Code": "https://github.com/pyfar/sofar",
     },
-    version='1.0.0',
+    version='1.1.0',
     zip_safe=False,
     python_requires='>=3.8'
 )
```

### Comparing `sofar-1.0.0/sofar/io.py` & `sofar-1.1.0/sofar/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import contextlib
 import os
 import numpy as np
 from netCDF4 import Dataset, chartostring, stringtochar
 import warnings
-import packaging
+import pathlib
+from packaging.version import parse
 import sofar as sf
 from .utils import _verify_convention_and_version, _atleast_nd
 
 
 def read_sofa(filename, verify=True, verbose=True):
     """
     Read SOFA file from disk and convert it to SOFA object.
 
     Numeric data is returned as floats or numpy float arrays unless they have
     missing data, in which case they are returned as numpy masked arrays.
 
     Parameters
     ----------
     filename : str
-        The filename. '.sofa' is appended to the filename, if it is not
-        explicitly given.
+        The full path to the sofa data.
     verify : bool, optional
         Verify and update the SOFA object by calling :py:func:`~Sofa.verify`.
         This helps to find potential errors in the default values and is thus
         recommended. If reading a file does not work, try to call `Sofa` with
         ``verify=False``. The default is ``True``.
     verbose : bool, optional
         Print the names of detected custom variables and attributes. The
         default is ``True``
 
     Returns
     -------
     sofa : Sofa
-        The SOFA object filled with the default values of the convention.
+        Object containing the data from `filename`.
 
     Notes
     -----
 
     1. Missing dimensions are appended when writing the SOFA object to disk.
        E.g., if ``sofa.Data_IR`` is of shape (1, 2) it is written as an array
        of shape (1, 2, 1) because the SOFA standard AES69-2020 defines it as a
@@ -48,61 +48,111 @@
        after writing and reading to and from disk.
     3. One dimensional arrays with only one element will be converted to scalar
        values. E.g. ``sofa.Data_SamplingRate`` is stored as an array of shape
        (1, ) inside SOFA files (according to the SOFA standard AES69-2020) but
        will be a scalar inside SOFA objects after reading from disk.
     """
 
+    return _read_netcdf(filename, verify, verbose, mode="sofa")
+
+
+def read_sofa_as_netcdf(filename):
+    """
+    Read corrupted SOFA data from disk.
+
+    .. note::
+        `read_sofa_as_netcdf` is intended to read and fix corrupted SOFA data
+        that could not be read by :py:func:`~read_sofa`. The recommend workflow
+        is
+
+        - Try to read the data with `read_sofa` and ``verify=True``
+        - If this fails, try the above with ``verify=False``
+        - If this fails, use `read_sofa_as_netcdf`
+
+        The SOFA object  returned by `read_sofa_as_netcdf` may not work
+        correctly before the issues with the data were fixed, i.e., before the
+        data are in agreement with the SOFA standard AES-69.
+
+    Numeric data is returned as floats or numpy float arrays unless they have
+    missing data, in which case they are returned as numpy masked arrays.
+
+    Parameters
+    ----------
+    filename : str
+        The full path to the NetCDF data.
+
+    Returns
+    -------
+    sofa : Sofa
+        Object containing the data from `filename`.
+
+    Notes
+    -----
+
+    1. Missing dimensions are appended when writing the SOFA object to disk.
+       E.g., if ``sofa.Data_IR`` is of shape (1, 2) it is written as an array
+       of shape (1, 2, 1) because the SOFA standard AES69-2020 defines it as a
+       three dimensional array with the dimensions (`M: measurements`,
+       `R: receivers`, `N: samples`)
+    2. When reading data from a SOFA file, array data is always returned as
+       numpy arrays and singleton trailing dimensions are discarded (numpy
+       default). I.e., ``sofa.Data_IR`` will again be an array of shape (1, 2)
+       after writing and reading to and from disk.
+    3. One dimensional arrays with only one element will be converted to scalar
+       values. E.g. ``sofa.Data_SamplingRate`` is stored as an array of shape
+       (1, ) inside SOFA files (according to the SOFA standard AES69-2020) but
+       will be a scalar inside SOFA objects after reading from disk.
+    """
+    return _read_netcdf(filename, False, False, mode="netcdf")
+
+
+def _read_netcdf(filename, verify, verbose, mode):
+
     # check the filename
-    if not filename.endswith('.sofa'):
-        raise ValueError("Filename must end with .sofa")
+    filename = pathlib.Path(filename).with_suffix('.sofa')
     if not os.path.isfile(filename):
         raise ValueError(f"{filename} does not exist")
 
     # attributes that are skipped
     skip = ["_Encoding"]
 
     # init list of all and custom attributes
     all_attr = []
     custom = []
 
     # open new NETCDF4 file for reading
     with Dataset(filename, "r", format="NETCDF4") as file:
 
-        # get convention name and version
-        convention = getattr(file, "SOFAConventions")
-        all_attr.append("GLOBAL_SOFAConventions")
-        version_in = getattr(file, "SOFAConventionsVersion")
-        all_attr.append("GLOBAL_SOFAConventionsVersion")
-
-        # check if convention and version exist
-        version_out = _verify_convention_and_version(
-            version_in, version_in, convention)
-
-        # get SOFA object with default values
-        sofa = sf.Sofa(convention, version=version_out, verify=verify)
+        if mode == "sofa":
+            # get convention name and version
+            convention = getattr(file, "SOFAConventions")
+            version = getattr(file, "SOFAConventionsVersion")
+
+            # check if convention and version exist
+            _verify_convention_and_version(version, convention)
+
+            # get SOFA object with default values
+            sofa = sf.Sofa(convention, version=version, verify=verify)
+        else:
+            sofa = sf.Sofa(None)
 
         # allow writing read only attributes
-        sofa._protected = False
+        sofa.protected = False
 
         # load global attributes
         for attr in file.ncattrs():
 
-            if attr in ["SOFAConventionsVersion", "SOFAConventions"]:
-                # convention and version were already set above
-                continue
-
             value = getattr(file, attr)
             all_attr.append(f"GLOBAL_{attr}")
 
             if not hasattr(sofa, f"GLOBAL_{attr}"):
                 sofa._add_custom_api_entry(
                     f"GLOBAL_{attr}", value, None, None, "attribute")
                 custom.append(f"GLOBAL_{attr}")
-                sofa._protected = False
+                sofa.protected = False
             else:
                 setattr(sofa, f"GLOBAL_{attr}", value)
 
         # load data
         for var in file.variables.keys():
 
             value = _format_value_from_netcdf(file[var][:], var)
@@ -113,40 +163,40 @@
             else:
                 dimensions = "".join(list(file[var].dimensions))
                 # SOFA only uses dtypes 'double' and 'S1' but netCDF has more
                 dtype = "string" if file[var].datatype == "S1" else "double"
                 sofa._add_custom_api_entry(var.replace(".", "_"), value, None,
                                            dimensions, dtype)
                 custom.append(var.replace(".", "_"))
-                sofa._protected = False
+                sofa.protected = False
 
             # load variable attributes
             for attr in [a for a in file[var].ncattrs() if a not in skip]:
 
                 value = getattr(file[var], attr)
                 all_attr.append(var.replace(".", "_") + "_" + attr)
 
                 if not hasattr(sofa, var.replace(".", "_") + "_" + attr):
                     sofa._add_custom_api_entry(
                         var.replace(".", "_") + "_" + attr, value, None,
                         None, "attribute")
                     custom.append(var.replace(".", "_") + "_" + attr)
-                    sofa._protected = False
+                    sofa.protected = False
                 else:
                     setattr(sofa, var.replace(".", "_") + "_" + attr, value)
 
     # remove fields from initial Sofa object that were not contained in NetCDF
     # file (initial Sofa object contained mandatory and optional fields)
     attrs = [attr for attr in sofa.__dict__.keys() if not attr.startswith("_")]
     for attr in attrs:
         if attr not in all_attr:
             delattr(sofa, attr)
 
     # do not allow writing read only attributes any more
-    sofa._protected = True
+    sofa.protected = True
 
     # notice about custom entries
     if custom and verbose:
         print(("SOFA file contained custom entries\n"
                "----------------------------------\n"
                f"{', '.join(custom)}"))
 
@@ -202,28 +252,31 @@
 def _write_sofa(filename: str, sofa: sf.Sofa, compression=4, verify=True):
     """
     Private write function for writing invalid SOFA files for testing. See
     write_sofa for documentation.
     """
 
     # check the filename
-    if not filename.endswith('.sofa'):
-        raise ValueError("Filename must end with .sofa")
+    filename = pathlib.Path(filename).with_suffix('.sofa')
 
-    # check if the latest version is used for writing and warn otherwise
-    # if case required for writing SOFA test data that violates the conventions
-    if sofa.GLOBAL_SOFAConventions != "invalid-value":
-        latest = sf.Sofa(sofa.GLOBAL_SOFAConventions)
-        latest = latest.GLOBAL_SOFAConventionsVersion
-        current = sofa.GLOBAL_SOFAConventionsVersion
-
-        if packaging.version.parse(current) < packaging.version.parse(latest):
-            warnings.warn(("Writing SOFA object with outdated Convention "
-                           f"version {current}. Use version='latest' to write "
-                           f"data with version {latest}."))
+    if verify:
+        # check if the latest version is used for writing and warn otherwise
+        # if case required for writing SOFA test data that violates the
+        # conventions
+        if sofa.GLOBAL_SOFAConventions != "invalid-value":
+            latest = sf.Sofa(sofa.GLOBAL_SOFAConventions)
+            latest = latest.GLOBAL_SOFAConventionsVersion
+            current = sofa.GLOBAL_SOFAConventionsVersion
+
+            if parse(current) < parse(latest):
+                warnings.warn((
+                    "Writing SOFA object with outdated Convention "
+                    f"version {current}. It is recommend to upgrade "
+                    " data with Sofa.upgrade_convention() before "
+                    "writing to disk if possible."))
 
     # setting the netCDF compression parameter
     use_zlib = compression != 0
 
     # update the dimensions
     if verify:
         sofa.verify(mode="write")
```

### Comparing `sofar-1.0.0/sofar/sofa.py` & `sofar-1.1.0/sofar/sofa.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,55 +85,63 @@
     _read_only_attr = []
 
     def __init__(self, convention, mandatory=False, version="latest",
                  verify=True):
         """See class docstring"""
 
         # get convention
-        self._convention = self._load_convention(convention, version)
+        if convention is not None:
+            self._convention = self._load_convention(convention, version)
 
-        # update read only attributes
-        self._read_only_attr = [
-            key for key in self._convention.keys()
-            if self._read_only(self._convention[key]["flags"])]
-
-        # add attributes with default values
-        self._convention_to_sofa(mandatory)
-
-        # add and update the API
-        # (mandatory=False can not be verified because some conventions have
-        # default values that have optional variables as dependencies)
-        if verify and not mandatory:
-            self.verify(mode="read")
+            # update read only attributes
+            self._read_only_attr = [
+                key for key in self._convention.keys()
+                if self._read_only(self._convention[key]["flags"])]
+
+            # add attributes with default values
+            self._convention_to_sofa(mandatory)
+
+            # add and update the API
+            # (mandatory=False can not be verified because some conventions
+            # have default values that have optional variables as dependencies)
+            if verify and not mandatory:
+                self.verify(mode="read")
 
-        self._protected = True
+            self.protected = True
+        else:
+            verify = False
+            self._convention = {}
 
     def __setattr__(self, name: str, value):
         # don't allow new attributes to be added outside the class
-        if self._protected and not hasattr(self, name):
+        if self.protected and not hasattr(self, name):
             raise TypeError(f"{name} is an invalid attribute")
 
         # don't allow setting read only attributes
-        if name in self._read_only_attr and self._protected:
-            raise TypeError(f"{name} is a read only attribute")
+        if name in self._read_only_attr and self.protected:
+            raise TypeError((
+                f"{name} is a read only attribute. Iy you know what you are "
+                "doing, you can set Sofa.protected = False to write read "
+                "only data (e.g., to repair corrupted SOFA data)."))
 
         # convert to numpy array or scalar
-        if not isinstance(value, (str, dict, np.ndarray)):
+        if not isinstance(value, (str, dict, np.ndarray)) \
+                and name != "protected":
             value = np.atleast_2d(value)
             if value.size == 1:
                 value = value.flatten()[0]
 
         super.__setattr__(self, name, value)
 
     def __delattr__(self, name: str):
         # can't delete non existing attributes
         if not hasattr(self, name):
             raise TypeError(f"{name} is not an attribute")
         # delete anything if not frozen, delete non mandatory
-        if not self._protected or \
+        if not self.protected or \
                 not self._mandatory(self._convention[name]["flags"]):
             super().__delattr__(name)
 
             # check if custom field as to be deleted
             if hasattr(self, "_custom"):
                 if name in self._custom:
                     self._custom.pop(name)
@@ -283,17 +291,25 @@
                 selected entries of the SOFA object. ``'data'`` does not show
                 entries of type attribute.
             key
                 If key is the name of an object attribute, all information for
                 attribute will be printed.
         """
 
+        # warn for upcoming deprecation
+        warnings.warn((
+            'Sofa.info() will be deprecated in sofar 1.3.0 The conventions are'
+            ' now documented at '
+            'https://sofar.readthedocs.io/en/stable/resources/conventions.html'),  # noqa
+            UserWarning)
+
         # update the private attribute `_convention` to make sure the required
         # meta data is in place
-        self._update_convention(version="match")
+        if not hasattr(self, "_convention"):
+            self._reset_convention()
 
         # list of all attributes
         keys = [k for k in self.__dict__.keys() if not k.startswith("_")]
 
         # start printing the information
         info_str = (
             f"{self.GLOBAL_SOFAConventions} "
@@ -457,34 +473,34 @@
             Add missing optional data. The default is ``True``.
         verbose : Bool
             Print the information about added data to the console. The default
             is ``True``.
         """
 
         # initialize
-        self._update_convention(version="match")
+        self._reset_convention()
         added = "Added the following missing data with their default values:\n"
 
         # current data
         keys = [key for key in self.__dict__.keys() if not key.startswith("_")]
 
-        self._protected = False
+        self.protected = False
 
         # loop data in convention
         for key in self._convention.keys():
             is_mandatory = self._mandatory(self._convention[key]["flags"])
             add_data = (is_mandatory and mandatory) or \
                 (not is_mandatory and optional)
             # add with default
             if key not in keys and add_data:
                 setattr(self, key, self._convention[key]["default"])
                 added += f"- {key} "
                 added += f"({'mandatory' if is_mandatory else 'optional'})\n"
 
-        self._protected = True
+        self.protected = True
 
         if verbose:
             if "-" in added:
                 print(added)
             else:
                 print("All mandatory data contained.")
 
@@ -506,15 +522,15 @@
                 list or numpy array.
             ``'string'``
                 Use this to store string variables as numpy string arrays of
                 type ``'U'`` or ``'S'``.
 
         dimensions : str
             The shape of the new entry as a string. See
-            ``self.info('dimensions')``.
+            :py:func:`~Sofa.list_dimensions`.
 
         Examples
         --------
         .. code-block:: python
 
             import sofar as sf
             sofa = sf.Sofa("GeneralTF")
@@ -561,25 +577,46 @@
 
         self._add_entry(name, value, 'attribute', None)
 
     def delete(self, name):
         """
         Delete variable or attribute from SOFA object.
 
-        Note that mandatory data can not be deleted. Call
-        :py:func:`Sofa.info("optional") <sofar.sofar.Sofa.info>` to list all
-        optional variables and attributes.
+        Note that mandatory data can not be deleted. Check the
+        `sofar documentation
+        <https://sofar.readthedocs.io/en/stable/resources/conventions.html>`_
+        for a complete list of optional variables and attributes.
 
         Parameters
         ----------
         name : str
             Name of the variable or attribute to be deleted
         """
         delattr(self, name)
 
+    @property
+    def protected(self):
+        """
+        If Sofa.protected is ``True``, read only data can not be changed. Only
+        change this to ``False`` if you know what you are doing, e.g., if you
+        need to repair corrupted SOFA data.
+        """
+        return self._protected
+
+    @protected.setter
+    def protected(self, value: bool):
+        """
+        If Sofa.protected is ``True``, read only data can not be changed. Only
+        change this to ``False`` if you know what you are doing, e.g., if you
+        need to repair corrupted SOFA data.
+        """
+        if not isinstance(value, bool):
+            raise ValueError("Sofa.protected can only be True or False")
+        self._protected = value
+
     def _add_entry(self, name, value, dtype, dimensions):
         """
         Add custom data to a SOFA object. See add_variable and add_attribute
         for more information.
         """
 
         # check input
@@ -629,15 +666,15 @@
             as in sofa._convention
         dimensions : string
             Dimensions in case of numeric or string array
         dtype : string
             double, string, or attribute
         """
         # create custom API if it not exists
-        self._protected = False
+        self.protected = False
 
         # lower case letters to indicate custom dimensions
         if dimensions is not None:
             dimensions = [d.upper() if d.upper() in "ERMNCIS" else d.lower()
                           for d in dimensions]
             dimensions = "".join(dimensions)
 
@@ -648,19 +685,19 @@
 
             self._custom[key] = {
                 "flags": flags,
                 "dimensions": dimensions,
                 "type": dtype,
                 "default": None,
                 "comment": ""}
-        self._update_convention(version="match")
+            self._convention[key] = self._custom[key]
 
         # add attribute to object
         setattr(self, key, value)
-        self._protected = True
+        self.protected = True
 
     def upgrade_convention(self, target=None, verify=True):
         """
         Upgrade Sofa data to newer conventions.
 
         Calling this with the default arguments returns a list of possible
         conventions to which the data will be upgraded. If the data is up to
@@ -683,15 +720,15 @@
         target : list of strings
             List with available conventions to which the data can be updated.
             If the data is up to data, the list will be empty. `target` is only
             returned if `target` is ``None``.
         """
 
         # check input ---------------------------------------------------------
-        self._update_convention(version="match")
+        self._reset_convention()
 
         # get deprecations and information about Sofa object
         _, _, deprecations, upgrade = self._verification_rules()
         convention_current = self.GLOBAL_SOFAConventions
         version_current = self.GLOBAL_SOFAConventionsVersion
         sofa_version_current = self.GLOBAL_Version
 
@@ -759,15 +796,15 @@
 
         # upgrade convention
         keys = ["GLOBAL_SOFAConventions",
                 "GLOBAL_SOFAConventionsVersion",
                 "GLOBAL_Version",
                 "GLOBAL_DataType"]
 
-        self._protected = False
+        self.protected = False
         for key in keys:
             setattr(self, key, self._convention[key]["default"])
 
         # move data
         for source, move in upgrade["move"].items():
             # get info
             source_sofar = source.replace(".", '_').replace(":", "_")
@@ -809,15 +846,15 @@
             print(f"- Deleting {target_sofar}.")
 
         if not upgrade["remove"]:
             print("- No data to remove")
 
         # check for missing mandatory data
         self.add_missing(True, False)
-        self._protected = True
+        self.protected = True
 
         # display general message
         if upgrade["message"] is not None:
             print(upgrade["message"])
 
         if verify:
             self.verify()
@@ -904,30 +941,30 @@
 
         # initialize warning and error messages
         error_msg = "\nERRORS\n------\n"
         warning_msg = "\nWARNINGS\n--------\n"
 
         # ---------------------------------------------------------------------
         # 0. update the convention
-        self._update_convention("match")
+        self._reset_convention()
 
         # ---------------------------------------------------------------------
         # 1. check if the mandatory attributes are contained
         missing = ""
         keys = [key for key in self.__dict__.keys() if not key.startswith("_")]
 
         for key in self._convention.keys():
             if self._mandatory(self._convention[key]["flags"]) \
                     and key not in keys:
 
                 if issue_handling != "raise":
                     # add missing data with default value
-                    self._protected = False
+                    self.protected = False
                     setattr(self, key, self._convention[key]["default"])
-                    self._protected = True
+                    self.protected = True
 
                 # prepare to raise warning
                 missing += "- " + key + "\n"
 
         if missing:
             if issue_handling == "raise":
                 error_msg += ("Detected missing mandatory data "
@@ -1100,18 +1137,18 @@
                 " the convention itself:\n")
             error_msg += current_error
 
         # ---------------------------------------------------------------------
         # 4. Get dimensions (E, R, M, N, S, c, I, and custom)
 
         # initialize required API fields
-        self._protected = False
+        self.protected = False
         self._dimensions = {}
         self._api = {}
-        self._protected = True
+        self.protected = True
 
         # get keys for checking the dimensions (all SOFA variables)
         keys = [key for key in self.__dict__.keys()
                 if key in self._convention
                 and self._convention[key]["dimensions"] is not None]
         if hasattr(self, "_custom"):
             keys_custom = [key for key in self._custom.keys()
@@ -1544,57 +1581,44 @@
 
         return rules, unit_aliases, deprecations, upgrade
 
     def copy(self):
         """Return a copy of the SOFA object."""
         return deepcopy(self)
 
-    def _update_convention(self, version):
+    def _reset_convention(self):
         """
-        Add SOFA convention to SOFA object in private attribute `_convention`.
-        If The object already contains a convention, it will be overwritten.
-
-        Parameters
-        ----------
-        version : str
-            ``'latest'``
-                Use the latest API and upgrade the SOFA file if required.
-            ``'match'``
-                Match the version of the sofa file.
-            str
-                Version string, e.g., ``'1.0'``.
+        - Add SOFA convention to SOFA object in private attribute
+          `_convention`. If The object already contains a convention, it will
+          be overwritten.
+        - If the SOFA object contains custom entries, check if any of the
+          custom entries part of the convention. If yes, delete the entry from
+          self._custom
+        - If the SOFA objects contains custom entries, add entries from
+          self._custom to self._convention
         """
 
         # verify convention and version
         c_current = self.GLOBAL_SOFAConventions
         v_current = str(self.GLOBAL_SOFAConventionsVersion)
 
-        v_new = _verify_convention_and_version(
-                version, v_current, c_current)
+        _verify_convention_and_version(v_current, c_current)
 
         # load and add convention and version
         convention = self._load_convention(
-            c_current, v_new)
+            c_current, v_current)
         self._convention = convention
 
-        if v_current != v_new:
-            self._protected = False
-            self.GLOBAL_SOFAConventionsVersion = v_new
-            self._protected = True
-
-        # feedback in case of up/downgrade
-        if float(v_current) < float(v_new):
-            warnings.warn(("Upgraded SOFA object from "
-                           f"version {v_current} to {v_new}"))
-        elif float(v_current) > float(v_new):
-            warnings.warn(("Downgraded SOFA object from "
-                           f"version {v_current} to {v_new}"))
-
-        # check if custom fields can be added
         if hasattr(self, "_custom"):
+            # check of custom fields can be removed
+            for key in self._convention:
+                if key in self._custom:
+                    del self._custom[key]
+
+            # check if custom fields can be added
             for key in self._custom:
                 self._convention[key] = self._custom[key]
 
     def _load_convention(self, convention, version):
         """
         Load SOFA convention from json file.
 
@@ -1680,25 +1704,25 @@
                 default = _atleast_nd(default, ndim)
 
             # create attribute with default value
             setattr(self, key, default)
 
         # write API and date specific fields (some read only)
         now = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-        self._protected = False
+        self.protected = False
         self.GLOBAL_DateCreated = now
         self.GLOBAL_DateModified = now
         self.GLOBAL_APIName = "sofar SOFA API for Python (pyfar.org)"
         self.GLOBAL_APIVersion = sf.version()
         self.GLOBAL_ApplicationName = "Python"
         self.GLOBAL_ApplicationVersion = (
             f"{platform.python_version()} "
             f"[{platform.python_implementation()} - "
             f"{platform.python_compiler()}]")
-        self._protected = True
+        self.protected = True
 
     @staticmethod
     def _get_size_and_shape_of_string_var(value, key):
         """
         String variables can be strings, list of strings, or numpy arrays of
         strings. This functions returns the length of the longest string S
         inside the string variable and the shape of the string variable as
```

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/FreeFieldDirectivityTF_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/FreeFieldDirectivityTF_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.csv` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.csv`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.json` & `sofar-1.1.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/rules/rules.json` & `sofar-1.1.0/sofar/sofa_conventions/rules/rules.json`

 * *Files identical despite different names*

### Comparing `sofar-1.0.0/sofar/sofa_conventions/rules/upgrade.json` & `sofar-1.1.0/sofar/sofa_conventions/rules/upgrade.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'FreeFieldDirectivityTF'": "OrderedDict([('from_to', [[['1.0'], ['FreeFieldDirectivityTF_1.1'], "*

 * *                             "'1']]), ('1', OrderedDict([('move', OrderedDict([('EmitterPosition', "*

 * *                             "OrderedDict([('target', 'EmitterPosition'), ('moveaxis', None), "*

 * *                             "('deprecated_dimensions', ['IC', 'MC'])])), ('EmitterDescription', "*

 * *                             "OrderedDict([('target', 'EmitterDescriptions'), ('moveaxis', None), "*

 * *                 […]*

```diff
@@ -1,8 +1,42 @@
 {
+    "FreeFieldDirectivityTF": {
+        "1": {
+            "message": "Consider to add the optional data 'GLOBAL_EmitterDescription'introduced in convention version 1.1.\nWARNING: Adding 'GLOBAL_EmitterDescription' is required if 'EmitterDescriptions' is contained in the SOFA object.",
+            "move": {
+                "EmitterDescription": {
+                    "deprecated_dimensions": [
+                        "IS"
+                    ],
+                    "moveaxis": null,
+                    "target": "EmitterDescriptions"
+                },
+                "EmitterPosition": {
+                    "deprecated_dimensions": [
+                        "IC",
+                        "MC"
+                    ],
+                    "moveaxis": null,
+                    "target": "EmitterPosition"
+                }
+            },
+            "remove": []
+        },
+        "from_to": [
+            [
+                [
+                    "1.0"
+                ],
+                [
+                    "FreeFieldDirectivityTF_1.1"
+                ],
+                "1"
+            ]
+        ]
+    },
     "GeneralFIRE": {
         "1": {
             "message": "Consider providing optional data that was introduced in SingleRoomSRIR version 1.0",
             "move": {
                 "Data.IR": {
                     "deprecated_dimensions": null,
                     "moveaxis": [
```

### Comparing `sofar-1.0.0/sofar/update_conventions.py` & `sofar-1.1.0/sofar/update_conventions.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,55 +329,68 @@
     for key in keys:
         if key.startswith("Data"):
             convention[key] = convention.pop(key)
 
     return convention
 
 
-def _check_congruency(save_dir=None):
+def _check_congruency(save_dir=None, branch="master"):
     """
     SOFA conventions are stored in two different places - is this a good idea?
     They should be identical, but let's find out.
 
     Prints warnings about incongruent conventions
 
     Parameters
     ----------
     save : str
         directory to save diverging conventions for further inspections
     """
 
-    urls = ["https://www.sofaconventions.org/conventions/",
-            ("https://raw.githubusercontent.com/sofacoustics/SOFAtoolbox/"
-             "master/SOFAtoolbox/conventions/")]
+    # urls for checking which conventions exist
+    urls_check = ["https://www.sofaconventions.org/conventions/",
+                  ("https://github.com/sofacoustics/SOFAtoolbox/tree/"
+                   f"{branch}/SOFAtoolbox/conventions/")]
+    # urls for loading the convention files
+    urls_load = ["https://www.sofaconventions.org/conventions/",
+                 ("https://raw.githubusercontent.com/sofacoustics/SOFAtoolbox/"
+                  f"{branch}/SOFAtoolbox/conventions/")]
     subdirs = ["sofaconventions", "sofatoolbox"]
 
     # check save_dir
     if save_dir is not None:
         if not os.path.isdir(save_dir):
             raise ValueError(f"{save_dir} does not exist")
         for subdir in subdirs:
             if not os.path.isdir(os.path.join(save_dir, subdir)):
                 os.makedirs(os.path.join(save_dir, subdir))
 
-    # get file names of conventions from sofaconventions.org and SOFAtoolbox
-    url = urls[0]
+    # get file names of conventions from sofaconventions.org
+    url = urls_check[0]
     page = requests.get(url).text
     soup = BeautifulSoup(page, 'html.parser')
     sofaconventions = [os.path.split(node.get('href'))[1]
                        for node in soup.find_all('a')
                        if node.get('href').endswith(".csv")]
 
-    url = ("https://github.com/sofacoustics/SOFAtoolbox/tree/"
-           "master/SOFAtoolbox/conventions/")
-    page = requests.get(url).text
-    soup = BeautifulSoup(page, 'html.parser')
-    sofatoolbox = [os.path.split(node.get('href'))[1]
-                   for node in soup.find_all('a')
-                   if node.get('href').endswith(".csv")]
+    if not sofaconventions:
+        raise ValueError(f"Did not find any conventions at {url}")
+
+    # get file names of conventions from github
+    url = urls_check[1]
+    page = requests.get(url).json()
+    sofatoolbox = []
+    for content in page["payload"]["tree"]["items"]:
+        if content["contentType"] == "file" and \
+                content["path"].startswith("SOFAtoolbox/conventions") and \
+                content["name"].endswith("csv"):
+            sofatoolbox.append(content["name"])
+
+    if not sofatoolbox:
+        raise ValueError(f"Did not find any conventions at {url}")
 
     # check if lists are identical. Remove items not contained in both lists
     report = ""
     for convention in sofaconventions:
         if convention.startswith(("General_", "GeneralString_")):
             sofaconventions.remove(convention)
         elif convention not in sofatoolbox:
@@ -390,15 +403,15 @@
             sofatoolbox.remove(convention)
             report += (f"- {convention} is missing on sofaconventions.org\n")
 
     # Loop and download conventions to check if they are identical
     for convention in sofaconventions:
 
         # download SOFA convention definitions to package directory
-        data = [requests.get(url + convention) for url in urls]
+        data = [requests.get(url + convention) for url in urls_load]
         # remove trailing tabs and windows style line breaks
         data = [d.content.replace(b"\r\n", b"\n").replace(b"\t\n", b"\n")
                 for d in data]
 
         # check for equality
         if data[0] != data[1]:
             report += f"- {convention} differs across platforms\n"
```

### Comparing `sofar-1.0.0/sofar/utils.py` & `sofar-1.1.0/sofar/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import glob
 import numpy as np
 import numpy.testing as npt
-from packaging.version import parse as version_parse
 import warnings
 import sofar as sf
 
 
 def version():
     """Return version of sofar and SOFA conventions"""
 
@@ -15,66 +14,47 @@
     with open(sofa_conventions) as file:
         sofa_conventions = file.readline().strip()
 
     return (f"sofar v{sf.__version__} implementing "
             f"SOFA standard {sofa_conventions}")
 
 
-def _verify_convention_and_version(version, version_in, convention):
+def _verify_convention_and_version(version, convention):
     """
-    Verify if convention and version exist and return version
+    Verify if convention and version exist. Raise a Value error if it does not.
 
     Parameters
     ----------
     version : str
-        'latest', 'match', version string (e.g., '1.0')
-    version_in : str
-        The version to be checked against
+        The version to be checked
     convention : str
         The name of the convention to be checked
-
-    Returns
-    -------
-    version_out : str
-        The version to be used depending on `version`, and `version_in`
     """
 
-    # check if the convention exists in sofar
+    # check if the convention exists
     if convention not in _get_conventions("name"):
         raise ValueError(
             f"Convention '{convention}' does not exist")
 
     name_version = _get_conventions("name_version")
 
-    if version == "latest":
-        # get list of versions as floats
-        version_out = [float(versions[1]) for versions in name_version
-                       if versions[0] == convention]
-        # get latest version as string
-        version_out = str(version_out[np.argmax(version_out)])
-
-        if version_parse(version_out) > version_parse(version_in):
-            print(("Updated conventions version from "
-                   f"{version_in} to {version_out}"))
-    else:
-        # check which version is wanted
-        match = version_in if version == "match" else version
-        version_out = None
-        for versions in name_version:
-            # check if convention and version match
-            if versions[0] == convention \
-                    and str(float(versions[1])) == match:
-                version_out = str(float(versions[1]))
-
-        if version_out is None:
-            raise ValueError((
-                f"Version {match} does not exist for convention {convention}. "
-                "Try to access the data with version='latest'"))
-
-    return version_out
+    # check which version is wanted
+    version_exists = False
+    for versions in name_version:
+        # check if convention and version match
+        if versions[0] == convention \
+                and str(float(versions[1])) == version:
+            version_exists = True
+
+    if not version_exists:
+        raise ValueError((
+            f"{convention} v{version} is not a valid SOFA Convention."
+            "If you are trying to read the data use "
+            "sofar.read_sofa_as_netcdf(). Call sofar.list_conventions() for a "
+            "list of valid Conventions"))
 
 
 def list_conventions():
     """
     List available SOFA conventions by printing to the console.
     """
     print(_get_conventions("string"))
```

### Comparing `sofar-1.0.0/sofar.egg-info/PKG-INFO` & `sofar-1.1.0/sofar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sofar
-Version: 1.0.0
+Version: 1.1.0
 Summary: Maybe the most complete python package for SOFA files so far
 Home-page: https://pyfar.org/
+Download-URL: https://pypi.org/project/sofar/
 Author: The pyfar developers
 Author-email: info@pyfar.org
 License: MIT license
-Download-URL: https://pypi.org/project/sofar/
 Project-URL: Bug Tracker, https://github.com/pyfar/sofar/issues
 Project-URL: Documentation, https://sofar.readthedocs.io/
 Project-URL: Source Code, https://github.com/pyfar/sofar
 Keywords: sofar
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======
 Readme
 ======
@@ -77,11 +77,9 @@
 
 AES69-2022: *AES standard for file exchange - Spatial acoustic data file
 format*, Audio Engineering Society, Inc., New York, NY, USA.
 (https://www.aes.org/publications/standards/search.cfm?docID=99)
 
 P. Majdak, F. Zotter, F. Brinkmann, J. De Muynke, M. Mihocic, and M.
 Noisternig, "Spatially Oriented Format for Acoustics 2.1: Introduction and
-Recent Advances,” *J. Audio Eng. Soc.*, vol. 70, no. 7/8, pp. 565–584,
+Recent Advances", *J. Audio Eng. Soc.*, vol. 70, no. 7/8, pp. 565-584,
 Jul. 2022. DOI: https://doi.org/10.17743/jaes.2022.0026
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sofar-1.0.0/sofar.egg-info/SOURCES.txt` & `sofar-1.1.0/sofar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 sofar.egg-info/PKG-INFO
 sofar.egg-info/SOURCES.txt
 sofar.egg-info/dependency_links.txt
 sofar.egg-info/not-zip-safe
 sofar.egg-info/requires.txt
 sofar.egg-info/top_level.txt
 sofar/sofa_conventions/VERSION
-sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.csv
-sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.json
 sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.csv
 sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.json
 sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.csv
 sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.json
 sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.csv
 sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.json
 sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.csv
@@ -48,14 +46,16 @@
 sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.json
 sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.csv
 sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.json
 sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.csv
 sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.json
 sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.csv
 sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.json
+sofar/sofa_conventions/conventions/deprecated/FreeFieldDirectivityTF_1.0.csv
+sofar/sofa_conventions/conventions/deprecated/FreeFieldDirectivityTF_1.0.json
 sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.csv
 sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.json
 sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.csv
 sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.json
 sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.csv
 sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.json
 sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.csv
@@ -71,12 +71,13 @@
 sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.csv
 sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.json
 sofar/sofa_conventions/rules/deprecations.json
 sofar/sofa_conventions/rules/rules.json
 sofar/sofa_conventions/rules/unit_aliases.json
 sofar/sofa_conventions/rules/upgrade.json
 tests/__init__.py
+tests/test_deprecations.py
 tests/test_io.py
 tests/test_sofa.py
 tests/test_sofa_upgrade_conventions.py
 tests/test_sofa_verify.py
 tests/test_utils.py
```

### Comparing `sofar-1.0.0/tests/test_io.py` & `sofar-1.1.0/tests/test_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,39 @@
 from sofar.utils import (_get_conventions,
                          _verify_convention_and_version,
                          _atleast_nd,
                          _nd_newaxis)
 from sofar.io import (_format_value_for_netcdf,
                       _format_value_from_netcdf)
 import os
+import pathlib
 from tempfile import TemporaryDirectory
 import pytest
 from pytest import raises
 import numpy as np
 import numpy.testing as npt
 from netCDF4 import Dataset
 
 
-def test_read_sofa(capfd):
+def test_read_write_sofa(capfd):
 
     temp_dir = TemporaryDirectory()
     filename = os.path.join(temp_dir.name, "test.sofa")
     sofa = sf.Sofa("SimpleFreeFieldHRIR")
 
     # test defaults
     sf.write_sofa(filename, sofa)
     sofa = sf.read_sofa(filename)
     assert hasattr(sofa, "_api")
 
+    # test with path object
+    sf.write_sofa(pathlib.Path(filename), sofa)
+    sofa = sf.read_sofa(pathlib.Path(filename))
+    assert hasattr(sofa, "_api")
+
     # reading without updating API
     sofa = sf.read_sofa(filename, verify=False)
     assert not hasattr(sofa, "_api")
 
     # read non-existing file
     with raises(ValueError, match="test.sofa does not exist"):
         sf.read_sofa("test.sofa")
@@ -43,15 +49,15 @@
 
     # read file of unknown version (stored in file)
     sofa = sf.Sofa("SimpleFreeFieldHRIR")
     sf.write_sofa(filename, sofa)
     with Dataset(filename, "r+", format="NETCDF4") as file:
         setattr(file, "SOFAConventionsVersion", "0.1")
     # ValueError when version should be matched
-    with raises(ValueError, match="Version 0.1 does not exist for"):
+    with raises(ValueError, match="v0.1 is not a valid SOFA Convention"):
         sf.read_sofa(filename)
 
     # read file containing a variable with wrong shape
     sofa = sf.Sofa("SimpleFreeFieldHRIR")
     sf.write_sofa(filename, sofa)
     # create variable with wrong shape
     with Dataset(filename, "r+", format="NETCDF4") as file:
@@ -60,18 +66,14 @@
         var[:] = np.zeros((1, 10)).astype("double")
     # reading data with update API generates an error
     with raises(ValueError, match="The SOFA object could not be"):
         sf.read_sofa(filename)
     # data can be read without updating API
     sf.read_sofa(filename, verify=False)
 
-    # test assertion for wrong filename
-    with raises(ValueError, match="Filename must end with .sofa"):
-        sf.read_sofa('sofa.exe')
-
 
 def test_read_sofa_custom_data():
     """Test if sofa files with custom data are loaded correctly"""
 
     temp_dir = TemporaryDirectory()
     filename = os.path.join(temp_dir.name, "test.sofa")
     sofa = sf.Sofa("SimpleFreeFieldHRIR")
@@ -79,20 +81,34 @@
     # GLOBAL attribute
     sofa.add_attribute('GLOBAL_Warming', 'critical')
     sf.write_sofa(filename, sofa)
     sofa = sf.read_sofa(filename)
     assert sofa.GLOBAL_Warming == 'critical'
 
 
-def test_write_sofa_assertion():
-    """Test assertion for wrong filename ending"""
+def test_read_netcdf():
+    tmp = TemporaryDirectory()
+    files = [os.path.join(tmp.name, "invalid.sofa"),
+             os.path.join(tmp.name, "invalid.netcdf")]
 
-    sofa = sf.Sofa("SimpleFreeFieldHRIR")
-    with raises(ValueError, match="Filename must end with .sofa"):
-        sf.write_sofa("sofa.exe", sofa)
+    # create data with invalid SOFA convention and version
+    sofa = sf.Sofa("GeneralTF")
+    sofa.protected = False
+    sofa.GLOBAL_SOFAConventions = "MadeUp"
+    sofa.protected = True
+
+    # test reading
+    for file in files:
+        # write data
+        sf.io._write_sofa(file, sofa, verify=False)
+        # can not be read with read_sofa
+        with raises(ValueError):
+            sf.read_sofa(file)
+        sofa_read = sf.read_sofa_as_netcdf(file)
+        sf.equals(sofa, sofa_read)
 
 
 def test_write_sofa_outdated_version():
     """Test the warning for writing SOFA files with outdated versions"""
 
     # generate test data and directory
     tmp = TemporaryDirectory()
@@ -295,31 +311,23 @@
     with raises(TypeError, match="Data_IR: value.dtype is complex"):
         _format_value_from_netcdf(
             np.array([44100], dtype="complex"), "Data_IR")
 
 
 def test_verify_convention_and_version():
 
-    # test different possibilities for version
-    version = _verify_convention_and_version("latest", "1.0", "GeneralTF")
-    assert version == "2.0"
-
-    version = _verify_convention_and_version("2.0", "1.0", "GeneralTF")
-    assert version == "2.0"
-
-    version = _verify_convention_and_version("match", "1.0", "GeneralTF")
-    assert version == "1.0"
+    # test with existing convention and version (no error returns None)
+    out = _verify_convention_and_version("1.0", "GeneralTF")
+    assert out is None
 
     # test assertions
     with raises(ValueError, match="Convention 'Funky' does not exist"):
-        _verify_convention_and_version("latest", "1.0", "Funky")
-    with raises(ValueError, match="Version 1.1 does not exist"):
-        _verify_convention_and_version("match", "1.1", "GeneralTF")
-    with raises(ValueError, match="Version 1.2 does not exist"):
-        _verify_convention_and_version("1.2", "1.0", "GeneralTF")
+        _verify_convention_and_version("1.0", "Funky")
+    with raises(ValueError, match="v1.1 is not a valid SOFA Convention"):
+        _verify_convention_and_version("1.1", "GeneralTF")
 
 
 def test_atleast_nd():
     # test with single dimension array
     for ndim in range(1, 6):
         array = _atleast_nd(1, ndim)
         assert array.ndim == ndim
```

### Comparing `sofar-1.0.0/tests/test_sofa.py` & `sofar-1.1.0/tests/test_sofa.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,17 +227,17 @@
 
     # test deleting an entry
     delattr(sofa, "Temperature_Units")
     assert not hasattr(sofa, "Temperature_Units")
     assert "Temperature_Units" not in sofa._custom
 
     # test adding missing entry defined in convention
-    sofa._protected = False
+    sofa.protected = False
     delattr(sofa, "ListenerPosition")
-    sofa._protected = True
+    sofa.protected = True
     sofa.add_variable("ListenerPosition", [0, 0, 0], "double", "IC")
     assert "ListenerPosition" not in sofa._custom
 
     # test assertions
     # add existing entry
     with raises(ValueError, match="Entry Temperature already exists"):
         sofa.add_variable("Temperature", 25.1, "double", "MI")
@@ -269,18 +269,18 @@
     sofa = sf.Sofa("GeneralTF")
 
     # attributes for testing
     man = "GLOBAL_AuthorContact"
     opt = "GLOBAL_History"
 
     # remove data before adding it again
-    sofa._protected = False
+    sofa.protected = False
     sofa.delete(man)
     sofa.delete(opt)
-    sofa._protected = False
+    sofa.protected = False
 
     # add missing data
     sofa.add_missing(mandatory, optional, verbose)
     out, _ = capfd.readouterr()
 
     if mandatory and optional:
         assert hasattr(sofa, man) and hasattr(sofa, opt)
@@ -309,19 +309,14 @@
     sofa.delete("GLOBAL_History")
     sofa.delete("SourceManufacturer")
     # check if data were removed
     assert not hasattr(sofa, "GLOBAL_History")
     assert not hasattr(sofa, "SourceManufacturer")
 
 
-def test__update_conventions():
-    """Tested in test_sofa_verify.pi::test_version"""
-    pass
-
-
 def test__get_size_and_shape_of_string_var():
 
     # test with string
     S, shape = sf.Sofa._get_size_and_shape_of_string_var("four", "key")
     assert S == 4
     assert shape == (1, 1)
```

### Comparing `sofar-1.0.0/tests/test_sofa_upgrade_conventions.py` & `sofar-1.1.0/tests/test_sofa_upgrade_conventions.py`

 * *Files 15% similar despite different names*

```diff
@@ -80,14 +80,23 @@
 
     # get SOFA object and targets for upgrading
     sofa = sf.Sofa(convention, version=version, verify=False)
     out, _ = capfd.readouterr()
     targets = sofa.upgrade_convention()
     out, _ = capfd.readouterr()
 
+    # don't verify conventions that might require user action after
+    if os.path.basename(path) in ["FreeFieldDirectivityTF_1.0.json"]:
+        # FreeFieldDirectivityTF_1.0
+        # - optional dependency GLOBAL_EmitterDescription
+        #   might need to be added
+        verify = False
+    else:
+        verify = True
+
     if targets:
         for target in targets:
-            sofa.upgrade_convention(target)
+            sofa.upgrade_convention(target, verify=verify)
             out, _ = capfd.readouterr()
             assert "Upgrading" in out
     else:
         assert not deprecated
```

### Comparing `sofar-1.0.0/tests/test_sofa_verify.py` & `sofar-1.1.0/tests/test_sofa_verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,17 @@
     Reading applications shall ignore the case of
     - units and
     - types of coordinate systems
     """
 
     # data type (must be case sensitive) --------------------------------------
     sofa = sf.Sofa("SimpleFreeFieldHRIR")
-    sofa._protected = False
+    sofa.protected = False
     sofa.GLOBAL_DataType = "fir"
-    sofa._protected = True
+    sofa.protected = True
     with raises(ValueError, match="GLOBAL_DataType is fir"):
         sofa.verify()
 
     # room type ---------------------------------------------------------------
     sofa = sf.Sofa("FreeFieldHRIR")
     sofa.GLOBAL_RoomType = "Free field"
     assert sofa.verify() is None
@@ -149,17 +149,17 @@
 
 
 # 1. check if the mandatory attributes are contained --------------------------
 def test_missing_default_attributes(capfd):
 
     # test missing default attribute
     sofa = sf.Sofa("GeneralTF")
-    sofa._protected = False
+    sofa.protected = False
     delattr(sofa, "GLOBAL_Conventions")
-    sofa._protected = True
+    sofa.protected = True
 
     # raises error
     with raises(ValueError, match="Detected missing mandatory data"):
         sofa.verify(issue_handling="raise")
 
     # prints warning and adds data
     sofa.verify(issue_handling="print")
@@ -238,50 +238,50 @@
 
 
 # 3. Verify names of entries --------------------------------------------------
 def test_wrong_name():
 
     # attribute with missing variable
     sofa = sf.Sofa("GeneralTF")
-    sofa._protected = False
+    sofa.protected = False
     sofa.IR_Type = "pressure"
     sofa._custom = {"IR_Type": {"default": None,
                                 "flags": None,
                                 "dimensions": None,
                                 "type": "attribute",
                                 "comment": ""}}
-    sofa._protected = True
+    sofa.protected = True
 
     with raises(ValueError, match="Detected attributes with missing"):
         sofa.verify()
 
     # attribute with no underscore
     sofa = sf.Sofa("GeneralTF")
-    sofa._protected = False
+    sofa.protected = False
     sofa.IRType = "pressure"
     sofa._custom = {"IRType": {"default": None,
                                "flags": None,
                                "dimensions": None,
                                "type": "attribute",
                                "comment": ""}}
-    sofa._protected = True
+    sofa.protected = True
 
     with raises(ValueError, match="Detected attribute names with too many"):
         sofa.verify()
 
     # variable with underscore
     sofa = sf.Sofa("GeneralTF")
-    sofa._protected = False
+    sofa.protected = False
     sofa.IR_Data = 1
     sofa._custom = {"IR_Data": {"default": None,
                                 "flags": None,
                                 "dimensions": "IM",
                                 "type": "double",
                                 "comment": ""}}
-    sofa._protected = True
+    sofa.protected = True
 
     with raises(ValueError, match="Detected variable names with too many"):
         sofa.verify()
 
     # variables with reserved names
     sofa = sf.Sofa("GeneralTF")
     sofa.add_variable("APIfunk", 1, "double", "I")
```

### Comparing `sofar-1.0.0/tests/test_utils.py` & `sofar-1.1.0/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import shutil
 import sofar as sf
 from sofar.utils import _get_conventions
-from sofar.update_conventions import _compile_conventions
+from sofar.update_conventions import _compile_conventions, _check_congruency
 import os
 import json
 from tempfile import TemporaryDirectory
 import pytest
 from pytest import raises
 import numpy as np
 from copy import deepcopy
+import warnings
 
 
 def test_list_conventions(capfd):
 
     # check output to console using pytest default fixture capfd
     sf.list_conventions()
     out, _ = capfd.readouterr()
@@ -44,14 +45,27 @@
     assert isinstance(names_versions, list)
     assert isinstance(names_versions[0], tuple)
 
     with raises(ValueError, match="return_type None is invalid"):
         _get_conventions(return_type="None")
 
 
+@pytest.mark.parametrize('branch', ['master', 'development'])
+def test__congruency(capfd, branch):
+    """
+    Check if conventions from SOFAToolbox and sofaconventions.org are
+    identical.
+    """
+    out, _ = capfd.readouterr()
+    _check_congruency(branch=branch)
+    out, _ = capfd.readouterr()
+    if out != "":
+        warnings.warn(out, Warning)
+
+
 def test_update_conventions(capfd):
 
     # create temporary directory and copy existing conventions
     temp_dir = TemporaryDirectory()
     work_dir = os.path.join(temp_dir.name, "sofa_conventions", "conventions")
     shutil.copytree(
         os.path.join(
@@ -142,61 +156,61 @@
         sf.equals(sofa_a, sofa_a, exclude="wrong")
 
     # check identical objects
     assert sf.equals(sofa_a, sofa_a)
 
     # check different number of keys
     sofa_b = deepcopy(sofa_a)
-    sofa_b._protected = False
+    sofa_b.protected = False
     delattr(sofa_b, "ReceiverPosition")
-    sofa_b._protected = True
+    sofa_b.protected = True
     with pytest.warns(UserWarning, match="not identical: sofa_a has"):
         is_identical = sf.equals(sofa_a, sofa_b)
         assert not is_identical
 
     # check different keys
     sofa_b = deepcopy(sofa_a)
-    sofa_b._protected = False
+    sofa_b.protected = False
     sofa_b.PositionReceiver = sofa_b.ReceiverPosition
     delattr(sofa_b, "ReceiverPosition")
-    sofa_b._protected = True
+    sofa_b.protected = True
     with pytest.warns(UserWarning, match="not identical: sofa_a and sofa_b"):
         is_identical = sf.equals(sofa_a, sofa_b)
         assert not is_identical
 
     # check mismatching data types
     sofa_b = deepcopy(sofa_a)
-    sofa_b._protected = False
+    sofa_b.protected = False
     sofa_b._convention["ReceiverPosition"]["type"] = "int"
-    sofa_b._protected = True
+    sofa_b.protected = True
     with pytest.warns(UserWarning, match="not identical: ReceiverPosition"):
         is_identical = sf.equals(sofa_a, sofa_b)
         assert not is_identical
 
     # check exclude GLOBAL attributes
     sofa_b = deepcopy(sofa_a)
-    sofa_b._protected = False
+    sofa_b.protected = False
     delattr(sofa_b, "GLOBAL_Version")
-    sofa_b._protected = True
+    sofa_b.protected = True
     is_identical = sf.equals(sofa_a, sofa_b, exclude="GLOBAL")
     assert is_identical
 
     # check exclude Date attributes
     sofa_b = deepcopy(sofa_a)
-    sofa_b._protected = False
+    sofa_b.protected = False
     delattr(sofa_b, "GLOBAL_DateModified")
-    sofa_b._protected = True
+    sofa_b.protected = True
     is_identical = sf.equals(sofa_a, sofa_b, exclude="DATE")
     assert is_identical
 
     # check exclude Date attributes
     sofa_b = deepcopy(sofa_a)
-    sofa_b._protected = False
+    sofa_b.protected = False
     delattr(sofa_b, "GLOBAL_DateModified")
-    sofa_b._protected = True
+    sofa_b.protected = True
     is_identical = sf.equals(sofa_a, sofa_b, exclude="ATTR")
     assert is_identical
 
 
 @pytest.mark.parametrize("value_a, value_b, attribute, fails", [
     ("1", "2", "GLOBAL_SOFAConventionsVersion", True),
     ([[1, 2]], [1, 2], "Data_IR", False),
@@ -206,22 +220,22 @@
     ("HD 650", np.array(["HD 650"], dtype="S"), "SourceModel", False),
     ("HD 650", "HD-650", "SourceModel", True)
 ])
 def test_equals_attribute_values(value_a, value_b, attribute, fails):
 
     # generate SOFA objects (SimpleHeadphoneIR has string variables)
     sofa_a = sf.Sofa("SimpleHeadphoneIR")
-    sofa_a._protected = False
+    sofa_a.protected = False
     sofa_b = deepcopy(sofa_a)
 
     # set parameters
     setattr(sofa_a, attribute, value_a)
-    sofa_a._protected = True
+    sofa_a.protected = True
     setattr(sofa_b, attribute, value_b)
-    sofa_b._protected = True
+    sofa_b.protected = True
 
     # compare
     if fails:
         with pytest.warns(UserWarning):
             assert not sf.equals(sofa_a, sofa_b)
     else:
         assert sf.equals(sofa_a, sofa_b)
```

