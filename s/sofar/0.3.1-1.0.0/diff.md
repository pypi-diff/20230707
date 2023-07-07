# Comparing `tmp/sofar-0.3.1.tar.gz` & `tmp/sofar-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sofar-0.3.1.tar", last modified: Tue Mar 22 07:38:45 2022, max compression
+gzip compressed data, was "sofar-1.0.0.tar", last modified: Fri Dec 16 14:22:47 2022, max compression
```

## Comparing `sofar-0.3.1.tar` & `sofar-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,91 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-22 07:38:45.000000 sofar-0.3.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2022-03-22 07:38:36.000000 sofar-0.3.1/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     7163 2022-03-22 07:38:36.000000 sofar-0.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2211 2022-03-22 07:38:36.000000 sofar-0.3.1/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2022-03-22 07:38:36.000000 sofar-0.3.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      186 2022-03-22 07:38:36.000000 sofar-0.3.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2022-03-22 07:38:45.000000 sofar-0.3.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2022-03-22 07:38:36.000000 sofar-0.3.1/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      453 2022-03-22 07:38:45.000000 sofar-0.3.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1527 2022-03-22 07:38:36.000000 sofar-0.3.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar/
--rw-rw-r--   0 travis    (2000) travis    (2000)      431 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar/conventions/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12627 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/FreeFieldDirectivityTF_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8098 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/FreeFieldHRIR_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7978 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/FreeFieldHRTF_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6614 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/GeneralFIR-E_2.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6603 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/GeneralFIRE_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7048 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/GeneralFIR_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7054 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/GeneralFIR_2.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6738 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/GeneralTF-E_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6677 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/GeneralTF_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6680 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/GeneralTF_2.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8884 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/MultiSpeakerBRIR_0.3.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8446 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SimpleFreeFieldHRIR_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8254 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SimpleFreeFieldHRSOS_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7773 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SimpleFreeFieldHRTF_2.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8249 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SimpleFreeFieldSOS_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9873 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SimpleHeadphoneIR_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8097 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SingleRoomDRIR_0.3.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    12311 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SingleRoomMIMOSRIR_1.0.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    12573 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/SingleRoomSRIR_1.0.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar/conventions/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5125 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/FreeFieldDirectivityTF_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/FreeFieldHRIR_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2201 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/FreeFieldHRTF_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1999 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/GeneralFIR-E_2.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/GeneralFIRE_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/GeneralFIR_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2011 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/GeneralFIR_2.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1995 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/GeneralTF-E_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1936 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/GeneralTF_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1939 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/GeneralTF_2.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2521 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/MultiSpeakerBRIR_0.3.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldHRIR_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2303 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldHRSOS_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1994 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldHRTF_2.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2298 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldSOS_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     3125 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SimpleHeadphoneIR_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1999 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SingleRoomDRIR_0.3.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     3320 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SingleRoomMIMOSRIR_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     3577 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/conventions/source/SingleRoomSRIR_1.0.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    93224 2022-03-22 07:38:36.000000 sofar-0.3.1/sofar/sofar.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2023 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-03-22 07:38:42.000000 sofar-0.3.1/sofar.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2022-03-22 07:38:45.000000 sofar-0.3.1/sofar.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2022-12-16 14:22:34.000000 sofar-1.0.0/AUTHORS.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7512 2022-12-16 14:22:34.000000 sofar-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3149 2022-12-16 14:22:34.000000 sofar-1.0.0/HISTORY.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2022-12-16 14:22:34.000000 sofar-1.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2022-12-16 14:22:34.000000 sofar-1.0.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3032 2022-12-16 14:22:47.342573 sofar-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2022-12-16 14:22:34.000000 sofar-1.0.0/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2022-12-16 14:22:47.342573 sofar-1.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1773 2022-12-16 14:22:34.000000 sofar-1.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.334573 sofar-1.0.0/sofar/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13867 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    67185 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/sofa.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.334573 sofar-1.0.0/sofar/sofa_conventions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/VERSION
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.338573 sofar-1.0.0/sofar/sofa_conventions/conventions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5125 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12627 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5510 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13138 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2479 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8127 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1998 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6615 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2130 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7357 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6757 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6696 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1957 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6699 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2239 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8446 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2303 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8254 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7791 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8249 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9863 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4053 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14346 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4199 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14491 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6603 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2560 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8884 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2093 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7704 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldHRIR_0.4.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1989 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7770 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_0.4.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2028 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7770 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3153 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9870 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3153 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9870 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2045 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8097 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1999 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8097 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/sofar/sofa_conventions/rules/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/deprecations.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22501 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/rules.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/unit_aliases.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4054 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar/sofa_conventions/rules/upgrade.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16193 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/update_conventions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11527 2022-12-16 14:22:34.000000 sofar-1.0.0/sofar/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.334573 sofar-1.0.0/sofar.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3032 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4003 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2022-12-16 14:22:47.000000 sofar-1.0.0/sofar.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:47.342573 sofar-1.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11682 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11415 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_sofa.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3038 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_sofa_upgrade_conventions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15641 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_sofa_verify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7930 2022-12-16 14:22:34.000000 sofar-1.0.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sofar-0.3.1/CONTRIBUTING.rst` & `sofar-1.0.0/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -48,46 +48,50 @@
 ------------
 
 Ready to contribute? Here's how to set up `sofar` for local development.
 
 1. Fork the `sofar` repo on GitHub.
 2. Clone your fork locally and cd into the sofar directory::
 
-    $ git clone https://github.com/pyfar/sofar.git
+    $ git clone --recursive https://github.com/pyfar/sofar.git
     $ cd sofar/
 
-3. Install your local copy into a virtualenv. Assuming you have Anaconda or Miniconda installed, this is how you set up your fork for local development::
+3. Note that some graphical Git interfaces can not do the recursive clone. If the folder sofar/sofa_conventions is empty try
+
+    $ git submodule update --init
+
+4. Install your local copy into a virtualenv. Assuming you have Anaconda or Miniconda installed, this is how you set up your fork for local development::
 
     $ conda create --name sofar python
     $ conda activate sofar
     $ conda install pip
     $ pip install -e .
     $ pip install -r requirements_dev.txt
 
-4. Create a branch for local development. Indicate the intention of your branch in its respective name (i.e. `feature/branch-name` or `bugfix/branch-name`)::
+5. Create a branch for local development. Indicate the intention of your branch in its respective name (i.e. `feature/branch-name` or `bugfix/branch-name`)::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-5. When you're done making changes, check that your changes pass flake8 and the
+6. When you're done making changes, check that your changes pass flake8 and the
    tests::
 
     $ flake8 sofar tests
     $ pytest
 
    flake8 test must pass without any warnings for `./sofar` and `./tests` using the default or a stricter configuration. Flake8 ignores `E123/E133, E226` and `E241/E242` by default. If necessary adjust the your flake8 and linting configuration in your IDE accordingly.
 
-6. Commit your changes and push your branch to GitHub::
+7. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
-7. Submit a pull request through the GitHub website.
+8. Submit a pull request through the GitHub website.
 
 Pull Request Guidelines
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
@@ -167,29 +171,37 @@
 .. code-block:: console
 
     $ make clean
 
 before building the documentation.
 
 
+Submodules
+~~~~~~~~~~
+
+To update the submodules containing the conventions and verification rules run
+
+$ git submodule update --remote sofar/sofa_conventions
+
+
 Deploying
 ~~~~~~~~~
 
 A reminder for the maintainers on how to deploy.
 
 - Commit all changes to develop
 - Update HISTORY.rst in develop
 - Check if new contributors should be added to AUTHORS.rst
 - Merge develop into main
 
 Switch to main and run::
 
 $ bumpversion patch --verbose # possible: major / minor / patch
 
-Bumpversion will update all version strings, create and comitt tags by default
+Bumpversion will update all version strings, create and commit tags by default
 
 $ git push --follow-tags
 
-Travis will then deploy to PyPI if tests pass.
+Continuous integration will then deploy to PyPI if tests pass.
 
 - Merge main back into develop
```

### Comparing `sofar-0.3.1/HISTORY.rst` & `sofar-1.0.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 History
 =======
 
+1.0.0 (2022-12-16)
+------------------
+* Use SOFA conventions of version 2.1 from https://github.com/pyfar/sofa_conventions
+* Verify SOFA data against all rules defined in the SOFA standard AES69-2022
+* Add `Sofa.upgrade_convention` for upgrading outdated conventions. This now uses explicit upgrade rules from https://github.com/pyfar/sofa_conventions
+* Remove upgrade functionality from `Sofa.verify`, `sofar.write_sofa`, and `sofar.read_sofa` for a more clear separation of functionality
+* Add `Sofa.add_missing` to add missing default data to a SOFA object using the default values specified by the SOFA convention
+* Add default parameter value to `Sofa.info`
+* Make `sofar.update_conventions` a public function again
+* Improve documentation and verbosity of command line output
+* Add private function to check congruency of conventions stored as part of SOFAtoolbox and on sofaconventions.org
+* Move to Circle CI and improve testing
+
 0.3.1 (2022-03-21)
 ------------------
 * Improvement `sofar.read`: Files with unknown Convention versions can now be read by updating to the latest or a specific version.
 * Improvement `sofar.read`: Reporting custom variables when reading SOFA files from disk is now optional and no longer a warning.
 * Improvement `Sofa.inspect`: SOFA objects that violate the SOFA convention can now be inspected. In this case, the violations are printed as message instead of raising an Error.
 * Improvement `Sofa.verify`: SOFA objects can now be verified without any output in case the output is not desired when calling `Sofa.inspect`.
```

### Comparing `sofar-0.3.1/LICENSE` & `sofar-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sofar-0.3.1/setup.py` & `sofar-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,27 +38,33 @@
     author_email='info@pyfar.org',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10'
     ],
     description="Maybe the most complete python package for SOFA files so far",
     install_requires=requirements,
     license="MIT license",
     long_description=readme,
     include_package_data=True,
     keywords='sofar',
     name='sofar',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/pyfar/sofar',
-    version='0.3.1',
+    url="https://pyfar.org/",
+    download_url="https://pypi.org/project/sofar/",
+    project_urls={
+        "Bug Tracker": "https://github.com/pyfar/sofar/issues",
+        "Documentation": "https://sofar.readthedocs.io/",
+        "Source Code": "https://github.com/pyfar/sofar",
+    },
+    version='1.0.0',
     zip_safe=False,
-    python_requires='>=3.7'
+    python_requires='>=3.8'
 )
```

### Comparing `sofar-0.3.1/sofar/conventions/FreeFieldDirectivityTF_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982456140350878%*

 * *Differences: {"'GLOBAL:Version'": "{'default': '2.1'}",*

 * * "'SourceTuningFrequency'": "{'comment': 'Frequency (in hertz) to which a musical instrument is "*

 * *                            'tuned to corresponding to the note A4 (MIDINote=69). Recommended for '*

 * *                            "tonal instruments.'}"}*

```diff
@@ -222,15 +222,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "Position of the microphone array during the measurements.",
         "default": [
@@ -374,15 +374,15 @@
         "comment": "",
         "default": "metre",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "SourceTuningFrequency": {
-        "comment": "Frequency (in Hertz) to which a musical instrument is tuned to corresponding to the note A4 (MIDINote=69). Recommended for tonal instruments.",
+        "comment": "Frequency (in hertz) to which a musical instrument is tuned to corresponding to the note A4 (MIDINote=69). Recommended for tonal instruments.",
         "default": 440,
         "dimensions": "I, M",
         "flags": null,
         "type": "double"
     },
     "SourceUp": {
         "comment": "Up vector of the acoustic source (instrument)",
```

### Comparing `sofar-0.3.1/sofar/conventions/FreeFieldHRIR_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285714%*

 * *Differences: {"'Data.Delay'": "{'dimensions': 'IRI, MRI, MRE'}",*

 * * "'GLOBAL:ListenerShortName'": "{'comment': 'Short name of the listener (as for example the "*

 * *                               "subject ID).'}",*

 * * "'GLOBAL:Version'": "{'default': '2.1'}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "Data.Delay": {
         "comment": "Additional delay of each IR (in samples)",
         "default": [
             0,
             0
         ],
-        "dimensions": "IRE, MRE",
+        "dimensions": "IRI, MRI, MRE",
         "flags": "m",
         "type": "double"
     },
     "Data.IR": {
         "comment": "",
         "default": [
             0,
@@ -146,15 +146,15 @@
         "comment": "",
         "default": "No license provided, ask the author for permission",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:ListenerShortName": {
-        "comment": "ID of the subject from the database",
+        "comment": "Short name of the listener (as for example the subject ID).",
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Organization": {
         "comment": "",
@@ -203,15 +203,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
```

### Comparing `sofar-0.3.1/sofar/conventions/FreeFieldHRTF_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965116279069768%*

 * *Differences: {"'GLOBAL:Version'": "{'default': '2.1'}",*

 * * "'N:LongName'": "{'flags': 'm', 'comment': 'narrative name of N'}"}*

```diff
@@ -189,15 +189,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
@@ -263,18 +263,18 @@
         "comment": "",
         "default": 0,
         "dimensions": "N",
         "flags": "m",
         "type": "double"
     },
     "N:LongName": {
-        "comment": "",
+        "comment": "narrative name of N",
         "default": "frequency",
         "dimensions": null,
-        "flags": null,
+        "flags": "m",
         "type": "attribute"
     },
     "N:Units": {
         "comment": "",
         "default": "hertz",
         "dimensions": null,
         "flags": "m",
```

### Comparing `sofar-0.3.1/sofar/conventions/GeneralFIR-E_2.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972222222222222%*

 * *Differences: {"'GLOBAL:Comment'": "{'flags': None}", "'GLOBAL:Version'": "{'default': '2.1'}"}*

```diff
@@ -87,15 +87,15 @@
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Comment": {
         "comment": "",
         "default": "",
         "dimensions": null,
-        "flags": "m",
+        "flags": null,
         "type": "attribute"
     },
     "GLOBAL:Conventions": {
         "comment": "",
         "default": "SOFA",
         "dimensions": null,
         "flags": "rm",
@@ -183,15 +183,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
```

### Comparing `sofar-0.3.1/sofar/conventions/GeneralFIRE_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-0.3.1/sofar/conventions/GeneralFIR_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994871794871795%*

 * *Differences: {"'Data.IR'": "{'dimensions': 'mrn'}",*

 * * "'Data.SamplingRate'": "{'dimensions': 'I, M'}",*

 * * "'GLOBAL:Version'": "{'default': '2.1'}",*

 * * "'ReceiverPosition'": "{'dimensions': 'IC, RC, RCM'}"}*

```diff
@@ -5,22 +5,22 @@
         "dimensions": "IR, MR",
         "flags": "m",
         "type": "double"
     },
     "Data.IR": {
         "comment": "Impulse responses",
         "default": 0,
-        "dimensions": "mRn",
+        "dimensions": "mrn",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate": {
         "comment": "Sampling rate of the samples in Data.IR and Data.Delay",
         "default": 48000,
-        "dimensions": "I",
+        "dimensions": "I, M",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate:Units": {
         "comment": "Unit of the sampling rate",
         "default": "hertz",
         "dimensions": null,
@@ -183,15 +183,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "1.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
@@ -245,15 +245,15 @@
     "ReceiverPosition": {
         "comment": "",
         "default": [
             0,
             0,
             0
         ],
-        "dimensions": "rCI, rCM",
+        "dimensions": "IC, RC, RCM",
         "flags": "m",
         "type": "double"
     },
     "ReceiverPosition:Type": {
         "comment": "",
         "default": "cartesian",
         "dimensions": null,
```

### Comparing `sofar-0.3.1/sofar/conventions/GeneralFIR_2.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9387500000000001%*

 * *Differences: {"'Data.Delay'": "{'comment': 'Broadband delay (in samples resulting from SamplingRate)'}",*

 * * "'Data.SOS'": "OrderedDict([('default', [[[0, 0, 0, 1, 0, 0]]]), ('flags', 'm'), ('dimensions', "*

 * *               "'mrn'), ('type', 'double'), ('comment', 'Filter coefficients as SOS "*

 * *               "coefficients.')])",*

 * * "'Data.SamplingRate'": "{'comment': 'Sampling rate of the coefficients in Data.SOS and the delay "*

 * *                        "in Data.Delay'}",*

 * * "'GLOBAL:Comment'": "{'flags': None}",*

 * * "'GLOBAL:DataTy […]*

```diff
@@ -1,24 +1,35 @@
 {
     "Data.Delay": {
-        "comment": "Additional delay of each IR (in samples)",
+        "comment": "Broadband delay (in samples resulting from SamplingRate)",
         "default": 0,
         "dimensions": "IR, MR",
         "flags": "m",
         "type": "double"
     },
-    "Data.IR": {
-        "comment": "Impulse responses",
-        "default": 0,
+    "Data.SOS": {
+        "comment": "Filter coefficients as SOS coefficients.",
+        "default": [
+            [
+                [
+                    0,
+                    0,
+                    0,
+                    1,
+                    0,
+                    0
+                ]
+            ]
+        ],
         "dimensions": "mrn",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate": {
-        "comment": "Sampling rate of the samples in Data.IR and Data.Delay",
+        "comment": "Sampling rate of the coefficients in Data.SOS and the delay in Data.Delay",
         "default": 48000,
         "dimensions": "I, M",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate:Units": {
         "comment": "Unit of the sampling rate",
@@ -87,27 +98,27 @@
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Comment": {
         "comment": "",
         "default": "",
         "dimensions": null,
-        "flags": "m",
+        "flags": null,
         "type": "attribute"
     },
     "GLOBAL:Conventions": {
         "comment": "",
         "default": "SOFA",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:DataType": {
-        "comment": "We store IRs here",
-        "default": "FIR",
+        "comment": "Filters described as second-order section (SOS) coefficients",
+        "default": "SOS",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:DateCreated": {
         "comment": "",
         "default": "",
@@ -161,37 +172,37 @@
         "comment": "The room information can be arbitrary",
         "default": "free field",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventions": {
-        "comment": "This conventions stores IRs for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined",
-        "default": "GeneralFIR",
+        "comment": "This conventions follows GeneralFIR but the data is stored as second-order section (SOS) coefficients.",
+        "default": "GeneralSOS",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventionsVersion": {
         "comment": "",
-        "default": "2.0",
+        "default": "1.0",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:Title": {
         "comment": "",
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
```

### Comparing `sofar-0.3.1/sofar/conventions/GeneralTF-E_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945945945945945%*

 * *Differences: {"'GLOBAL:Comment'": "{'flags': None}",*

 * * "'GLOBAL:Version'": "{'default': '2.1'}",*

 * * "'N:LongName'": "{'flags': 'm', 'comment': 'narrative name of N'}"}*

```diff
@@ -73,15 +73,15 @@
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Comment": {
         "comment": "",
         "default": "",
         "dimensions": null,
-        "flags": "m",
+        "flags": null,
         "type": "attribute"
     },
     "GLOBAL:Conventions": {
         "comment": "",
         "default": "SOFA",
         "dimensions": null,
         "flags": "rm",
@@ -169,15 +169,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
@@ -207,18 +207,18 @@
         "comment": "Frequency values",
         "default": 0,
         "dimensions": "N",
         "flags": "m",
         "type": "double"
     },
     "N:LongName": {
-        "comment": "",
+        "comment": "narrative name of N",
         "default": "frequency",
         "dimensions": null,
-        "flags": null,
+        "flags": "m",
         "type": "attribute"
     },
     "N:Units": {
         "comment": "Unit of the values given in N",
         "default": "hertz",
         "dimensions": null,
         "flags": "m",
```

### Comparing `sofar-0.3.1/sofar/conventions/GeneralTF_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986486486486488%*

 * *Differences: {"'N:LongName'": "{'comment': 'narrative name of N'}"}*

```diff
@@ -207,15 +207,15 @@
         "comment": "Frequency values",
         "default": 0,
         "dimensions": "N",
         "flags": "m",
         "type": "double"
     },
     "N:LongName": {
-        "comment": "",
+        "comment": "narrative name of N",
         "default": "frequency",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "N:Units": {
         "comment": "Unit of the values given in N",
```

### Comparing `sofar-0.3.1/sofar/conventions/GeneralTF_2.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945945945945945%*

 * *Differences: {"'EmitterPosition'": "{'dimensions': 'eC, eCM'}",*

 * * "'GLOBAL:Comment'": "{'flags': None}",*

 * * "'GLOBAL:Version'": "{'default': '2.1'}",*

 * * "'N:LongName'": "{'comment': 'narrative name of N'}"}*

```diff
@@ -16,15 +16,15 @@
     "EmitterPosition": {
         "comment": "",
         "default": [
             0,
             0,
             0
         ],
-        "dimensions": "eCI, eCM",
+        "dimensions": "eC, eCM",
         "flags": "m",
         "type": "double"
     },
     "EmitterPosition:Type": {
         "comment": "",
         "default": "cartesian",
         "dimensions": null,
@@ -73,15 +73,15 @@
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Comment": {
         "comment": "",
         "default": "",
         "dimensions": null,
-        "flags": "m",
+        "flags": null,
         "type": "attribute"
     },
     "GLOBAL:Conventions": {
         "comment": "",
         "default": "SOFA",
         "dimensions": null,
         "flags": "rm",
@@ -169,15 +169,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "1.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
@@ -207,15 +207,15 @@
         "comment": "Frequency values",
         "default": 0,
         "dimensions": "N",
         "flags": "m",
         "type": "double"
     },
     "N:LongName": {
-        "comment": "",
+        "comment": "narrative name of N",
         "default": "frequency",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "N:Units": {
         "comment": "Unit of the values given in N",
```

### Comparing `sofar-0.3.1/sofar/conventions/MultiSpeakerBRIR_0.3.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/MultiSpeakerBRIR_0.3.json`

 * *Files identical despite different names*

### Comparing `sofar-0.3.1/sofar/conventions/SimpleFreeFieldHRIR_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRIR_1.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989130434782609%*

 * *Differences: {"'GLOBAL:Version'": "{'default': '2.1'}"}*

```diff
@@ -203,15 +203,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
```

### Comparing `sofar-0.3.1/sofar/conventions/SimpleFreeFieldHRSOS_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988095238095239%*

 * *Differences: {"'GLOBAL:Version'": "{'default': '2.1'}"}*

```diff
@@ -219,15 +219,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
```

### Comparing `sofar-0.3.1/sofar/conventions/SimpleFreeFieldHRTF_2.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleFreeFieldTF_1.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9066666666666666%*

 * *Differences: {"'GLOBAL:SOFAConventions'": "{'default': 'SimpleFreeFieldTF', 'comment': 'This conventions is for "*

 * *                             "TFs created under conditions where room information is irrelevant'}",*

 * * "'GLOBAL:SOFAConventionsVersion'": "{'default': '1.0'}",*

 * * "'GLOBAL:Version'": "{'default': '1.0'}",*

 * * "'N_LongName'": "OrderedDict([('default', 'frequency'), ('flags', None), ('dimensions', None), "*

 * *                 "('type', 'attribute'), ('comment', '')])",*

 * * "'N_Units'": "OrderedDict([('default', 'hertz'), ( […]*

```diff
@@ -167,37 +167,37 @@
         "comment": "",
         "default": "free field",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventions": {
-        "comment": "This conventions is for HRTFs created under conditions where room information is irrelevant",
-        "default": "SimpleFreeFieldHRTF",
+        "comment": "This conventions is for TFs created under conditions where room information is irrelevant",
+        "default": "SimpleFreeFieldTF",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventionsVersion": {
         "comment": "",
-        "default": "2.0",
+        "default": "1.0",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:Title": {
         "comment": "",
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "1.0",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
@@ -262,26 +262,26 @@
     "N": {
         "comment": "",
         "default": 0,
         "dimensions": "N",
         "flags": "m",
         "type": "double"
     },
-    "N:LongName": {
+    "N_LongName": {
         "comment": "",
         "default": "frequency",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
-    "N:Units": {
+    "N_Units": {
         "comment": "",
         "default": "hertz",
         "dimensions": null,
-        "flags": "m",
+        "flags": null,
         "type": "attribute"
     },
     "ReceiverPosition": {
         "comment": "",
         "default": [
             [
                 0,
```

### Comparing `sofar-0.3.1/sofar/conventions/SimpleFreeFieldSOS_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.json`

 * *Files identical despite different names*

### Comparing `sofar-0.3.1/sofar/conventions/SimpleHeadphoneIR_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997%*

 * *Differences: {"'Data.SamplingRate'": "{'dimensions': 'I'}",*

 * * "'GLOBAL:SOFAConventionsVersion'": "{'default': '0.2'}",*

 * * "'GLOBAL:Version'": "{'default': '1.0'}"}*

```diff
@@ -18,15 +18,15 @@
         "dimensions": "mRn",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate": {
         "comment": "",
         "default": 48000,
-        "dimensions": "I, M",
+        "dimensions": "I",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate:Units": {
         "comment": "",
         "default": "hertz",
         "dimensions": null,
@@ -226,15 +226,15 @@
         "default": "SimpleHeadphoneIR",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventionsVersion": {
         "comment": "",
-        "default": "1.0",
+        "default": "0.2",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:SourceDescription": {
         "comment": "Narrative description of the headphones",
         "default": "",
@@ -268,15 +268,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "1.0",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
```

### Comparing `sofar-0.3.1/sofar/conventions/SingleRoomDRIR_0.3.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.json`

 * *Files identical despite different names*

### Comparing `sofar-0.3.1/sofar/conventions/SingleRoomMIMOSRIR_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8597402597402601%*

 * *Differences: {"'Data.Delay'": "{'dimensions': 'IR, MR'}",*

 * * "'Data.IR'": "{'dimensions': 'mrn'}",*

 * * "'EmitterDescriptions'": "OrderedDict([('default', ['']), ('flags', None), ('dimensions', 'ES, "*

 * *                          "ESM'), ('type', 'string'), ('comment', 'E-dependent version of the "*

 * *                          "attribute EmitterDescription')])",*

 * * "'EmitterPosition'": "{'dimensions': 'eCI, eCM', 'comment': ''}",*

 * * "'EmitterPosition:Type'": '{\'comment\': "Shall be \'cartesian\' or \'spherical\', restricting to '*

 * *     […]*

```diff
@@ -1,19 +1,19 @@
 {
     "Data.Delay": {
         "comment": "Additional delay of each IR (in samples)",
         "default": 0,
-        "dimensions": "IRI, MRI, MRE",
+        "dimensions": "IR, MR",
         "flags": "m",
         "type": "double"
     },
     "Data.IR": {
         "comment": "Impulse responses",
         "default": 0,
-        "dimensions": "mrne",
+        "dimensions": "mrn",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate": {
         "comment": "Sampling rate of the samples in Data.IR and Data.Delay",
         "default": 48000,
         "dimensions": "I, M",
@@ -23,27 +23,36 @@
     "Data.SamplingRate:Units": {
         "comment": "Unit of the sampling rate",
         "default": "hertz",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
+    "EmitterDescriptions": {
+        "comment": "E-dependent version of the attribute EmitterDescription",
+        "default": [
+            ""
+        ],
+        "dimensions": "ES, ESM",
+        "flags": null,
+        "type": "string"
+    },
     "EmitterPosition": {
-        "comment": "Can be of any type enabling both spatially discrete and spatially continuous representations.",
+        "comment": "",
         "default": [
             0,
             0,
             0
         ],
-        "dimensions": "IC, ECI, ECM",
+        "dimensions": "eCI, eCM",
         "flags": "m",
         "type": "double"
     },
     "EmitterPosition:Type": {
-        "comment": "",
+        "comment": "Shall be 'cartesian' or 'spherical', restricting to spatially discrete emitters.",
         "default": "spherical",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "EmitterPosition:Units": {
         "comment": "",
@@ -71,15 +80,15 @@
             0
         ],
         "dimensions": "ECI, ECM",
         "flags": null,
         "type": "double"
     },
     "EmitterView:Type": {
-        "comment": "",
+        "comment": "Shall be 'cartesian' or 'spherical', restricting to spatially discrete emitters.",
         "default": "cartesian",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
     "EmitterView:Units": {
         "comment": "",
@@ -134,16 +143,16 @@
         "comment": "",
         "default": "SOFA",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:DataType": {
-        "comment": "Shall be FIR-E",
-        "default": "FIR-E",
+        "comment": "Shall be FIR",
+        "default": "FIR",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:DatabaseName": {
         "comment": "Name of the database. Used for classification of the data.",
         "default": "",
@@ -239,30 +248,51 @@
         "comment": "",
         "default": "",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
     "GLOBAL:RoomDescription": {
-        "comment": "narrative description of the room",
+        "comment": "Informal verbal description of the room",
+        "default": "",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "GLOBAL:RoomGeometry": {
+        "comment": "URI to a file describing the room geometry.",
+        "default": "",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "GLOBAL:RoomLocation": {
+        "comment": "Location of the room",
+        "default": "",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "GLOBAL:RoomShortName": {
+        "comment": "Short name of the Room",
         "default": "",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
     "GLOBAL:RoomType": {
         "comment": "Shall be 'shoebox' or 'dae'",
         "default": "shoebox",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventions": {
-        "comment": "Single-room multiple-input multiple-output spatial room impulse responses, depending on Emitters",
-        "default": "SingleRoomMIMOSRIR",
+        "comment": "For measuring SRIRs in a single room with a single excitation source (e.g., a loudspeaker) and a listener containing an arbitrary number of omnidirectional receivers (e.g., a microphone array).",
+        "default": "SingleRoomSRIR",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventionsVersion": {
         "comment": "",
         "default": "1.0",
@@ -289,15 +319,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
@@ -355,14 +385,30 @@
     "ListenerView:Units": {
         "comment": "",
         "default": "metre",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
+    "MeasurementDate": {
+        "comment": "Optional M-dependent date and time of the measurement",
+        "default": 0,
+        "dimensions": "M",
+        "flags": null,
+        "type": "double"
+    },
+    "ReceiverDescriptions": {
+        "comment": "R-dependent version of the attribute ReceiverDescription",
+        "default": [
+            ""
+        ],
+        "dimensions": "RS, RSM",
+        "flags": null,
+        "type": "string"
+    },
     "ReceiverPosition": {
         "comment": "",
         "default": [
             0,
             0,
             0
         ],
@@ -424,47 +470,75 @@
         "comment": "",
         "default": [
             0,
             0,
             0
         ],
         "dimensions": "IC, MC",
-        "flags": "m",
+        "flags": null,
         "type": "double"
     },
     "RoomCornerB": {
         "comment": "",
         "default": [
             1,
             2,
             3
         ],
         "dimensions": "IC, MC",
-        "flags": "m",
+        "flags": null,
         "type": "double"
     },
     "RoomCorners": {
         "comment": "The value of this attribute is to be ignored. It only exist to for RoomCorners:Type and RoomCorners:Units",
         "default": 0,
         "dimensions": "II",
         "flags": null,
         "type": "double"
     },
     "RoomCorners:Type": {
         "comment": "",
         "default": "cartesian",
         "dimensions": null,
-        "flags": "m",
+        "flags": null,
         "type": "attribute"
     },
     "RoomCorners:Units": {
         "comment": "",
         "default": "metre",
         "dimensions": null,
-        "flags": "m",
+        "flags": null,
+        "type": "attribute"
+    },
+    "RoomTemperature": {
+        "comment": "Temperature during measurements, given in Kelvin.",
+        "default": 0,
+        "dimensions": "I, M",
+        "flags": null,
+        "type": "double"
+    },
+    "RoomTemperature:Units": {
+        "comment": "Units of the room temperature.",
+        "default": "kelvin",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "RoomVolume": {
+        "comment": "Volume of the room.",
+        "default": 0,
+        "dimensions": "I, M",
+        "flags": null,
+        "type": "double"
+    },
+    "RoomVolume:Units": {
+        "comment": "Units of the room volume.",
+        "default": "cubic metre",
+        "dimensions": null,
+        "flags": null,
         "type": "attribute"
     },
     "SourcePosition": {
         "comment": "",
         "default": [
             0,
             0,
```

### Comparing `sofar-0.3.1/sofar/conventions/SingleRoomSRIR_1.0.json` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8610389610389614%*

 * *Differences: {"'Data.Delay'": "{'dimensions': 'IRI, MRI, MRE'}",*

 * * "'Data.IR'": "{'dimensions': 'mrne'}",*

 * * "'EmitterDescriptions'": "OrderedDict([('default', ['']), ('flags', None), ('dimensions', 'ES, "*

 * *                          "ESM'), ('type', 'string'), ('comment', 'E-dependent version of the "*

 * *                          "attribute EmitterDescription')])",*

 * * "'EmitterPosition'": "{'dimensions': 'IC, ECI, ECM', 'comment': 'Can be of any type enabling both "*

 * *                      "spatially discrete and spatially continu […]*

```diff
@@ -1,19 +1,19 @@
 {
     "Data.Delay": {
         "comment": "Additional delay of each IR (in samples)",
         "default": 0,
-        "dimensions": "IR, MR",
+        "dimensions": "IRI, MRI, MRE",
         "flags": "m",
         "type": "double"
     },
     "Data.IR": {
         "comment": "Impulse responses",
         "default": 0,
-        "dimensions": "mrn",
+        "dimensions": "mrne",
         "flags": "m",
         "type": "double"
     },
     "Data.SamplingRate": {
         "comment": "Sampling rate of the samples in Data.IR and Data.Delay",
         "default": 48000,
         "dimensions": "I, M",
@@ -23,27 +23,36 @@
     "Data.SamplingRate:Units": {
         "comment": "Unit of the sampling rate",
         "default": "hertz",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
+    "EmitterDescriptions": {
+        "comment": "E-dependent version of the attribute EmitterDescription",
+        "default": [
+            ""
+        ],
+        "dimensions": "ES, ESM",
+        "flags": null,
+        "type": "string"
+    },
     "EmitterPosition": {
-        "comment": "",
+        "comment": "Can be of any type enabling both spatially discrete and spatially continuous representations.",
         "default": [
             0,
             0,
             0
         ],
-        "dimensions": "eCI, eCM",
+        "dimensions": "IC, ECI, ECM",
         "flags": "m",
         "type": "double"
     },
     "EmitterPosition:Type": {
-        "comment": "Shall be 'cartesian' or 'spherical', restricting to spatially discrete emitters.",
+        "comment": "",
         "default": "spherical",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "EmitterPosition:Units": {
         "comment": "",
@@ -71,15 +80,15 @@
             0
         ],
         "dimensions": "ECI, ECM",
         "flags": null,
         "type": "double"
     },
     "EmitterView:Type": {
-        "comment": "Shall be 'cartesian' or 'spherical', restricting to spatially discrete emitters.",
+        "comment": "",
         "default": "cartesian",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
     "EmitterView:Units": {
         "comment": "",
@@ -134,16 +143,16 @@
         "comment": "",
         "default": "SOFA",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:DataType": {
-        "comment": "Shall be FIR",
-        "default": "FIR",
+        "comment": "Shall be FIR-E",
+        "default": "FIR-E",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:DatabaseName": {
         "comment": "Name of the database. Used for classification of the data.",
         "default": "",
@@ -239,30 +248,51 @@
         "comment": "",
         "default": "",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
     "GLOBAL:RoomDescription": {
-        "comment": "narrative description of the room",
+        "comment": "Informal verbal description of the room",
+        "default": "",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "GLOBAL:RoomGeometry": {
+        "comment": "URI to a file describing the room geometry.",
+        "default": "",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "GLOBAL:RoomLocation": {
+        "comment": "Location of the room",
+        "default": "",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "GLOBAL:RoomShortName": {
+        "comment": "Short name of the Room",
         "default": "",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
     "GLOBAL:RoomType": {
         "comment": "Shall be 'shoebox' or 'dae'",
         "default": "shoebox",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventions": {
-        "comment": "For measuring SRIRs in a single room with a single excitation source (e.g., a loudspeaker) and a listener containing an arbitrary number of omnidirectional receivers (e.g., a microphone array).",
-        "default": "SingleRoomSRIR",
+        "comment": "Single-room multiple-input multiple-output spatial room impulse responses, depending on Emitters",
+        "default": "SingleRoomMIMOSRIR",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "GLOBAL:SOFAConventionsVersion": {
         "comment": "",
         "default": "1.0",
@@ -289,15 +319,15 @@
         "default": "",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
     "GLOBAL:Version": {
         "comment": "",
-        "default": "2.0",
+        "default": "2.1",
         "dimensions": null,
         "flags": "rm",
         "type": "attribute"
     },
     "ListenerPosition": {
         "comment": "",
         "default": [
@@ -355,14 +385,30 @@
     "ListenerView:Units": {
         "comment": "",
         "default": "metre",
         "dimensions": null,
         "flags": "m",
         "type": "attribute"
     },
+    "MeasurementDate": {
+        "comment": "Optional M-dependent date and time of the measurement.",
+        "default": 0,
+        "dimensions": "M",
+        "flags": null,
+        "type": "double"
+    },
+    "ReceiverDescriptions": {
+        "comment": "R-dependent version of the attribute ReceiverDescription",
+        "default": [
+            ""
+        ],
+        "dimensions": "RS, RSM",
+        "flags": null,
+        "type": "string"
+    },
     "ReceiverPosition": {
         "comment": "",
         "default": [
             0,
             0,
             0
         ],
@@ -446,27 +492,55 @@
         "comment": "The value of this attribute is to be ignored. It only exist to for RoomCorners:Type and RoomCorners:Units",
         "default": 0,
         "dimensions": "II",
         "flags": null,
         "type": "double"
     },
     "RoomCorners:Type": {
-        "comment": "Type of coordinate system for RoomCornerA and RoomCornerB",
+        "comment": "",
         "default": "cartesian",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
     "RoomCorners:Units": {
-        "comment": "Unit of coordinate system for RoomCornerA and RoomCornerB",
+        "comment": "",
         "default": "metre",
         "dimensions": null,
         "flags": null,
         "type": "attribute"
     },
+    "RoomTemperature": {
+        "comment": "Temperature during measurements, given in Kelvin.",
+        "default": 0,
+        "dimensions": "I, M",
+        "flags": null,
+        "type": "double"
+    },
+    "RoomTemperature:Units": {
+        "comment": "Units of the room temperature",
+        "default": "kelvin",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
+    "RoomVolume": {
+        "comment": "Volume of the room",
+        "default": 0,
+        "dimensions": "I, MI",
+        "flags": null,
+        "type": "double"
+    },
+    "RoomVolume:Units": {
+        "comment": "Units of the room volume",
+        "default": "cubic metre",
+        "dimensions": null,
+        "flags": null,
+        "type": "attribute"
+    },
     "SourcePosition": {
         "comment": "",
         "default": [
             0,
             0,
             1
         ],
```

### Comparing `sofar-0.3.1/sofar/conventions/source/FreeFieldDirectivityTF_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldDirectivityTF_1.0.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm		attribute
-GLOBAL:Version	2.0	rm		attribute
+GLOBAL:Version	2.1	rm		attribute
 GLOBAL:SOFAConventions	FreeFieldDirectivityTF	rm		attribute	This conventions stores directivities of acoustic sources (instruments, loudspeakers, singers, talkers, etc) in the frequency domain for multiple musical notes in free field.
 GLOBAL:SOFAConventionsVersion	1.0	rm		attribute
 GLOBAL:DataType	TF	rm		attribute	We store frequency-dependent data here
 GLOBAL:RoomType	free field	m		attribute	The room information can be arbitrary, but the spatial setup assumes free field.
 GLOBAL:Title		m		attribute
 GLOBAL:DateCreated		m		attribute
 GLOBAL:DateModified		m		attribute
@@ -46,13 +46,13 @@
 SourceUp:Reference		m		attribute	Narrative description of the spatial reference of the source up, e.g., for the trumpet, 'Along the keys, keys up'. Mandatory in order to provide a reference across different instruments
 EmitterPosition	[0 0 0]	m	IC, MC	double	A more detailed structure of the Source. In a simple settings, a single Emitter is considered that is collocated with the source.
 EmitterPosition:Type	cartesian	m		attribute
 EmitterPosition:Units	metre	m		attribute
 EmitterDescription	{''}		IS, MS	string	A more detailed structure of the source. In a simple setting, a single Emitter is considered that is collocated with the source. In a more complicated setting, this may be the strings of a violin or the units of a loudspeaker.
 MIDINote	0		I, M	double	Defines the note played by the source during the measurement. The note is specified a MIDI note by the [https://www.midi.org/specifications-old/item/the-midi-1-0-specification MIDI specifications, version 1.0]. Not mandatory, but recommended for tonal instruments.
 Description	{''}		MS	string	This variable is used when the description varies with M.
-SourceTuningFrequency	440		I, M	double	Frequency (in Hertz) to which a musical instrument is tuned to corresponding to the note A4 (MIDINote=69). Recommended for tonal instruments.
+SourceTuningFrequency	440		I, M	double	Frequency (in hertz) to which a musical instrument is tuned to corresponding to the note A4 (MIDINote=69). Recommended for tonal instruments.
 Data.Real	0	m	mrn	double	Real part of the complex spectrum. The default value 0 indicates that all data fields are initialized with zero values.
 Data.Imag	0	m	MRN	double	Imaginary part of the complex spectrum
 N	0	m	N	double	Frequency values
 N:LongName	frequency	m		attribute
 N:Units	hertz	m		attribute	Units used for N
```

### Comparing `sofar-0.3.1/sofar/conventions/source/FreeFieldHRIR_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRIR_1.0.csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	FreeFieldHRIR	rm	  	attribute	An extension of SimpleFreeFieldHRIR in order to consider more complex data sets described in spatially continuous representation. Each HRTF direction corresponds to an emitter, and a consistent measurement for a single listener and all directions is described by a set of the emitter positions surrounding the listener.
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Comment			 	attribute
 GLOBAL:DataType	FIR-E	rm	  	attribute
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
-GLOBAL:ListenerShortName		m		attribute	ID of the subject from the database
+GLOBAL:ListenerShortName		m		attribute	Short name of the listener (as for example the subject ID).
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
 GLOBAL:RoomType	free field	m	  	attribute
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
 GLOBAL:Title		m		attribute
@@ -36,8 +36,8 @@
 ListenerUp	[0 0 1]	m	IC, MC	double
 ListenerView	[1 0 0]	m	IC, MC	double
 ListenerView:Type	cartesian	m		attribute
 ListenerView:Units	metre	m		attribute
 Data.IR	[0 0]	m	mrne	double
 Data.SamplingRate	48000	m	I, M	double
 Data.SamplingRate:Units	hertz	m		attribute
-Data.Delay	[0 0]	m	IRE, MRE	double	Additional delay of each IR (in samples)
+Data.Delay	[0 0]	m	IRI, MRI, MRE	double	Additional delay of each IR (in samples)
```

### Comparing `sofar-0.3.1/sofar/conventions/source/FreeFieldHRTF_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/FreeFieldHRTF_1.0.csv`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	FreeFieldHRTF	rm	  	attribute	This conventions is for HRTFs created under conditions where room information is irrelevant and stored as SH coefficients
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
@@ -36,9 +36,9 @@
 ListenerUp	[0 0 1]	m	IC, MC	double
 ListenerView	[1 0 0]	m	IC, MC	double
 ListenerView:Type	cartesian	m		attribute
 ListenerView:Units	metre	m		attribute
 Data.Real	[0 0]	m	mrne	double
 Data.Imag	[0 0]	m	MRNE	double
 N	0	m	N	double
-N:LongName	frequency			attribute
+N:LongName	frequency	m		attribute	narrative name of N
 N:Units	hertz	m		attribute
```

### Comparing `sofar-0.3.1/sofar/conventions/source/GeneralFIR-E_2.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR-E_2.0.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	GeneralFIR-E	rm	  	attribute	This conventions stores IRs for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined
 GLOBAL:SOFAConventionsVersion	2.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
-GLOBAL:Comment		m	 	attribute
+GLOBAL:Comment			 	attribute
 GLOBAL:DataType	FIR-E	rm	  	attribute	We use FIR datatype which in addition depends on Emitters (E)
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
 GLOBAL:RoomType	free field	m	  	attribute	The room information can be arbitrary
 GLOBAL:Origin				attribute
```

### Comparing `sofar-0.3.1/sofar/conventions/source/GeneralFIRE_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/GeneralFIRE_1.0.csv`

 * *Files identical despite different names*

### Comparing `sofar-0.3.1/sofar/conventions/source/GeneralFIR_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralFIR_1.0.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	1.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	GeneralFIR	rm	  	attribute	This conventions stores IRs for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
@@ -18,23 +18,23 @@
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
 GLOBAL:Title		m		attribute
 ListenerPosition	[0 0 0] 	m	IC, MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
-ReceiverPosition	[0 0 0]	m	rCI, rCM	double
+ReceiverPosition	[0 0 0]	m	IC, RC, RCM	double
 ReceiverPosition:Type	cartesian	m	  	attribute
 ReceiverPosition:Units	metre	m	  	attribute
 SourcePosition	[0 0 1]	m	IC, MC	double	In order to store different directions/positions around the listener, SourcePosition is assumed to vary
 SourcePosition:Type	spherical	m	  	attribute
 SourcePosition:Units	degree, degree, metre	m	  	attribute
 EmitterPosition	[0 0 0]	m	eCI, eCM	double
 EmitterPosition:Type	cartesian	m	  	attribute
 EmitterPosition:Units	metre	m	  	attribute
-Data.IR	0	m	mRn	double	Impulse responses
-Data.SamplingRate	48000	m	I	double	Sampling rate of the samples in Data.IR and Data.Delay
+Data.IR	0	m	mrn	double	Impulse responses
+Data.SamplingRate	48000	m	I, M	double	Sampling rate of the samples in Data.IR and Data.Delay
 Data.SamplingRate:Units	hertz	m		attribute	Unit of the sampling rate
 Data.Delay	0	m	IR, MR	double	Additional delay of each IR (in samples)
 ListenerView	[1 0 0]		IC, MC	double
 ListenerView:Type	cartesian			attribute
 ListenerView:Units	metre			attribute
```

### Comparing `sofar-0.3.1/sofar/conventions/source/GeneralFIR_2.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_1.0.csv`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
-GLOBAL:SOFAConventions	GeneralFIR	rm	  	attribute	This conventions stores IRs for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined
-GLOBAL:SOFAConventionsVersion	2.0	rm	  	attribute
+GLOBAL:Version	1.0	rm	 	attribute
+GLOBAL:SOFAConventions	GeneralTF	rm	  	attribute	This conventions stores TFs for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined. This convention is based on GeneralFIR.
+GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Comment		m	 	attribute
-GLOBAL:DataType	FIR	rm	  	attribute	We store IRs here
+GLOBAL:DataType	TF	rm	  	attribute	We store frequency-dependent data here
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
 GLOBAL:RoomType	free field	m	  	attribute	The room information can be arbitrary
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
 GLOBAL:Title		m		attribute
 ListenerPosition	[0 0 0] 	m	IC, MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
-ReceiverPosition	[0 0 0]	m	IC, RC, RCM	double
+ReceiverPosition	[0 0 0]	m	rCI, rCM	double
 ReceiverPosition:Type	cartesian	m	  	attribute
 ReceiverPosition:Units	metre	m	  	attribute
 SourcePosition	[0 0 1]	m	IC, MC	double	In order to store different directions/positions around the listener, SourcePosition is assumed to vary
 SourcePosition:Type	spherical	m	  	attribute
 SourcePosition:Units	degree, degree, metre	m	  	attribute
 EmitterPosition	[0 0 0]	m	eCI, eCM	double
 EmitterPosition:Type	cartesian	m	  	attribute
 EmitterPosition:Units	metre	m	  	attribute
-Data.IR	0	m	mrn	double	Impulse responses
-Data.SamplingRate	48000	m	I, M	double	Sampling rate of the samples in Data.IR and Data.Delay
-Data.SamplingRate:Units	hertz	m		attribute	Unit of the sampling rate
-Data.Delay	0	m	IR, MR	double	Additional delay of each IR (in samples)
-ListenerView	[1 0 0]		IC, MC	double
-ListenerView:Type	cartesian			attribute
-ListenerView:Units	metre			attribute
+Data.Real	0	m	mRn	double	The real part of the complex spectrum
+Data.Imag	0	m	MRN	double	The imaginary part of the complex spectrum
+N	0	m	N	double	Frequency values
+N:LongName	frequency	m		attribute	narrative name of N
+N:Units	hertz	m		attribute	Unit of the values given in N
```

### Comparing `sofar-0.3.1/sofar/conventions/source/GeneralTF-E_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF-E_1.0.csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	GeneralTF-E	rm	  	attribute	This conventions stores TFs depending in the Emiiter for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined. This convention is based on GeneralTF
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
-GLOBAL:Comment		m	 	attribute
+GLOBAL:Comment			 	attribute
 GLOBAL:DataType	TF-E	rm	  	attribute	We store frequency-dependent data depending on the emitter here
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
 GLOBAL:RoomType	free field	m	  	attribute	The room information can be arbitrary
 GLOBAL:Origin				attribute
@@ -30,9 +30,9 @@
 SourcePosition:Units	degree, degree, metre	m	  	attribute
 EmitterPosition	[0 0 0]	m	IC, EC, ECM	double
 EmitterPosition:Type	cartesian	m	  	attribute
 EmitterPosition:Units	metre	m	  	attribute
 Data.Real	0	m	mrne	double	The real part of the complex spectrum
 Data.Imag	0	m	MRNE	double	The imaginary part of the complex spectrum
 N	0	m	N	double	Frequency values
-N:LongName	frequency			attribute
+N:LongName	frequency	m		attribute	narrative name of N
 N:Units	hertz	m		attribute	Unit of the values given in N
```

### Comparing `sofar-0.3.1/sofar/conventions/source/GeneralTF_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralTF_2.0.csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	1.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	GeneralTF	rm	  	attribute	This conventions stores TFs for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined. This convention is based on GeneralFIR.
-GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
+GLOBAL:SOFAConventionsVersion	2.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
-GLOBAL:Comment		m	 	attribute
+GLOBAL:Comment			 	attribute
 GLOBAL:DataType	TF	rm	  	attribute	We store frequency-dependent data here
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
 GLOBAL:RoomType	free field	m	  	attribute	The room information can be arbitrary
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
 GLOBAL:Title		m		attribute
 ListenerPosition	[0 0 0] 	m	IC, MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
-ReceiverPosition	[0 0 0]	m	rCI, rCM	double
+ReceiverPosition	[0 0 0]	m	IC, RC, RCM	double
 ReceiverPosition:Type	cartesian	m	  	attribute
 ReceiverPosition:Units	metre	m	  	attribute
 SourcePosition	[0 0 1]	m	IC, MC	double	In order to store different directions/positions around the listener, SourcePosition is assumed to vary
 SourcePosition:Type	spherical	m	  	attribute
 SourcePosition:Units	degree, degree, metre	m	  	attribute
-EmitterPosition	[0 0 0]	m	eCI, eCM	double
+EmitterPosition	[0 0 0]	m	eC, eCM	double
 EmitterPosition:Type	cartesian	m	  	attribute
 EmitterPosition:Units	metre	m	  	attribute
-Data.Real	0	m	mRn	double	The real part of the complex spectrum
+Data.Real	0	m	mrn	double	The real part of the complex spectrum
 Data.Imag	0	m	MRN	double	The imaginary part of the complex spectrum
 N	0	m	N	double	Frequency values
-N:LongName	frequency	m		attribute
+N:LongName	frequency	m		attribute	narrative name of N
 N:Units	hertz	m		attribute	Unit of the values given in N
```

### Comparing `sofar-0.3.1/sofar/conventions/source/GeneralTF_2.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.3.csv`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
 GLOBAL:Version	1.0	rm	 	attribute
-GLOBAL:SOFAConventions	GeneralTF	rm	  	attribute	This conventions stores TFs for general purposes, i.e., only the mandatory, SOFA general metadata are pre-defined. This convention is based on GeneralFIR.
-GLOBAL:SOFAConventionsVersion	2.0	rm	  	attribute
+GLOBAL:SOFAConventions	SingleRoomDRIR	rm	  	attribute	This convention stores arbitrary number of receivers while providing an information about the room. The main application is to store DRIRs for a single room.
+GLOBAL:SOFAConventionsVersion	0.3	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Comment		m	 	attribute
-GLOBAL:DataType	TF	rm	  	attribute	We store frequency-dependent data here
+GLOBAL:DataType	FIR	rm	  	attribute
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
-GLOBAL:RoomType	free field	m	  	attribute	The room information can be arbitrary
+GLOBAL:RoomType	reverberant	m	  	attribute
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
 GLOBAL:Title		m		attribute
 ListenerPosition	[0 0 0] 	m	IC, MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
-ReceiverPosition	[0 0 0]	m	IC, RC, RCM	double
+ReceiverPosition	[0 0 0]	m	RCI, RCM	double
 ReceiverPosition:Type	cartesian	m	  	attribute
 ReceiverPosition:Units	metre	m	  	attribute
-SourcePosition	[0 0 1]	m	IC, MC	double	In order to store different directions/positions around the listener, SourcePosition is assumed to vary
-SourcePosition:Type	spherical	m	  	attribute
-SourcePosition:Units	degree, degree, metre	m	  	attribute
+SourcePosition	[0 0 0]	m	IC, MC	double
+SourcePosition:Type	cartesian	m	  	attribute
+SourcePosition:Units	metre	m	  	attribute
 EmitterPosition	[0 0 0]	m	eCI, eCM	double
 EmitterPosition:Type	cartesian	m	  	attribute
 EmitterPosition:Units	metre	m	  	attribute
-Data.Real	0	m	mrn	double	The real part of the complex spectrum
-Data.Imag	0	m	MRN	double	The imaginary part of the complex spectrum
-N	0	m	N	double	Frequency values
-N:LongName	frequency	m		attribute
-N:Units	hertz	m		attribute	Unit of the values given in N
+GLOBAL:DatabaseName		m	  	attribute
+GLOBAL:RoomDescription		m	  	attribute
+ListenerUp	[0 0 1]	m	IC, MC	double
+ListenerView	[1 0 0]	m	IC, MC	double
+ListenerView:Type	cartesian	m		attribute
+ListenerView:Units	metre	m		attribute
+SourceUp	[0 0 1]	m	IC, MC	double
+SourceView	[-1 0 0]	m	IC, MC	double
+SourceView:Type	cartesian	m		attribute
+SourceView:Units	metre	m		attribute
+Data.IR	[0]	m	mrn	double
+Data.SamplingRate	48000	m	I	double
+Data.SamplingRate:Units	hertz	m		attribute
+Data.Delay	[0]	m	IR, MR	double
```

### Comparing `sofar-0.3.1/sofar/conventions/source/MultiSpeakerBRIR_0.3.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRSOS_1.0.csv`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	1.0	rm	 	attribute
-GLOBAL:SOFAConventions	MultiSpeakerBRIR	rm	  	attribute	This convention is for BRIRs recorded in reverberant conditions from multiple loudspeaker sources at a number of listener orientations.
-GLOBAL:SOFAConventionsVersion	0.3	rm	  	attribute
+GLOBAL:Version	2.1	rm	 	attribute
+GLOBAL:SOFAConventions	SimpleFreeFieldHRSOS	rm	  	attribute	This convention set follows SimpleFreeFieldHRIR but the data is stored as second-order section (SOS) coefficients.
+GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
-GLOBAL:Comment		m	 	attribute
-GLOBAL:DataType	FIRE	rm	  	attribute	We use FIR datatype which in addition depends on Emitters (E)
+GLOBAL:Comment			 	attribute
+GLOBAL:DataType	SOS	rm	  	attribute	Filters described as second-order section (SOS) coefficients
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
-GLOBAL:RoomType	reverberant	m	  	attribute
+GLOBAL:RoomType	free field	m	  	attribute
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
 GLOBAL:Title		m		attribute
 ListenerPosition	[0 0 0] 	m	IC, MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
 ReceiverPosition	[0 0.09 0; 0 -0.09 0]	m	rCI, rCM	double
 ReceiverPosition:Type	cartesian	m	  	attribute
 ReceiverPosition:Units	metre	m	  	attribute
-SourcePosition	[0 0 1]	m	IC, MC	double
+SourcePosition	[0 0 1]	m	IC, MC	double	Source position is assumed to vary for different directions/positions around the listener
 SourcePosition:Type	spherical	m	  	attribute
 SourcePosition:Units	degree, degree, metre	m	  	attribute
-EmitterPosition	[0 0 0]	m	eCI, eCM	double	Each speaker is represented as an emitter. Use EmitterPosition to represent the position of a particular speaker. Size of EmitterPosition determines E
+EmitterPosition	[0 0 0]	m	eCI, eCM	double
 EmitterPosition:Type	cartesian	m	  	attribute
 EmitterPosition:Units	metre	m	  	attribute
 GLOBAL:DatabaseName		m	  	attribute	name of the database to which these data belong
 GLOBAL:ListenerShortName		m	  	attribute	ID of the subject from the database
-GLOBAL:RoomDescription				attribute	narrative description of the room
 ListenerUp	[0 0 1]	m	IC, MC	double
 ListenerView	[1 0 0]	m	IC, MC	double
-ListenerView:Type	cartesian	m	  	attribute
-ListenerView:Units	metre	m	  	attribute
-EmitterUp	[0 0 1]		ECI, ECM	double	When EmitterUp provided, EmitterView must be provided as well
-EmitterView	[1 0 0]		ECI, ECM	double	When EmitterView provided, EmitterUp must be provided as well
-EmitterView:Type	cartesian		  	attribute
-EmitterView:Units	metre		  	attribute
-Data.IR	[1 1]	m	mREn	double
-Data.SamplingRate	48000	m	I	double
+ListenerView:Type	cartesian	m		attribute
+ListenerView:Units	metre	m		attribute
+Data.SOS	permute([0 0 0 1 0 0; 0 0 0 1 0 0], [3 1 2]);	m	mRn	double	Filter coefficients as SOS coefficients.
+Data.SamplingRate	48000	m	I, M	double	Sampling rate of the coefficients in Data.SOS and the delay in Data.Delay
 Data.SamplingRate:Units	hertz	m		attribute
-Data.Delay	[0 0]	m	IRE, MRE	double
+Data.Delay	[0 0]	m	IR, MR	double	Broadband delay (in samples resulting from SamplingRate)
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldHRIR_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldSOS_1.0.csv`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
-GLOBAL:SOFAConventions	SimpleFreeFieldHRIR	rm	  	attribute	This convention set is for HRIRs recorded under free-field conditions or other IRs created under conditions where room information is irrelevant
+GLOBAL:Version	1.0	rm	 	attribute
+GLOBAL:SOFAConventions	SimpleFreeFieldSOS	rm	  	attribute	This convention set follows SimpleFreeFieldHRIR but the data is stored as second-order section (SOS) coefficients.
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Comment			 	attribute
-GLOBAL:DataType	FIR	rm	  	attribute
+GLOBAL:DataType	SOS	rm	  	attribute	Filters described as second-order section (SOS) coefficients
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
 GLOBAL:RoomType	free field	m	  	attribute
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
@@ -33,15 +33,11 @@
 EmitterPosition:Units	metre	m	  	attribute
 GLOBAL:DatabaseName		m	  	attribute	name of the database to which these data belong
 GLOBAL:ListenerShortName		m	  	attribute	ID of the subject from the database
 ListenerUp	[0 0 1]	m	IC, MC	double
 ListenerView	[1 0 0]	m	IC, MC	double
 ListenerView:Type	cartesian	m		attribute
 ListenerView:Units	metre	m		attribute
-Data.IR	[0 0]	m	mRn	double
-Data.SamplingRate	48000	m	I, M	double
+Data.SOS	permute([0 0 0 1 0 0; 0 0 0 1 0 0], [3 1 2]);	m	mRn	double	Filter coefficients as SOS coefficients.
+Data.SamplingRate	48000	m	I	double	Sampling rate of the coefficients in Data.SOS and the delay in Data.Delay
 Data.SamplingRate:Units	hertz	m		attribute
-Data.Delay	[0 0]	m	IR, MR	double
-SourceUp	[0 0 1]		IC, MC	double
-SourceView	[1 0 0]		IC, MC	double
-SourceView:Type	cartesian			attribute
-SourceView:Units	metre			attribute
+Data.Delay	[0 0]	m	IR, MR	double	Broadband delay (in samples resulting from SamplingRate)
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldHRSOS_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/GeneralSOS_1.0.csv`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
-GLOBAL:SOFAConventions	SimpleFreeFieldHRSOS	rm	  	attribute	This convention set follows SimpleFreeFieldHRIR but the data is stored as second-order section (SOS) coefficients.
+GLOBAL:Version	2.1	rm	 	attribute
+GLOBAL:SOFAConventions	GeneralSOS	rm	  	attribute	This conventions follows GeneralFIR but the data is stored as second-order section (SOS) coefficients.
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Comment			 	attribute
-GLOBAL:DataType	SOS	rm	  	attribute	Filters described as second-order section (SOS) coefficients
+GLOBAL:DataType	SOS	rm		attribute	Filters described as second-order section (SOS) coefficients
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
-GLOBAL:RoomType	free field	m	  	attribute
+GLOBAL:RoomType	free field	m	  	attribute	The room information can be arbitrary
 GLOBAL:Origin				attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
 GLOBAL:Title		m		attribute
 ListenerPosition	[0 0 0] 	m	IC, MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
-ReceiverPosition	[0 0.09 0; 0 -0.09 0]	m	rCI, rCM	double
+ListenerView	[1 0 0]		IC, MC	double
+ListenerView:Type	cartesian			attribute
+ListenerView:Units	metre			attribute
+ReceiverPosition	[0 0 0]	m	IC, RC, RCM	double
 ReceiverPosition:Type	cartesian	m	  	attribute
 ReceiverPosition:Units	metre	m	  	attribute
-SourcePosition	[0 0 1]	m	IC, MC	double	Source position is assumed to vary for different directions/positions around the listener
+SourcePosition	[0 0 1]	m	IC, MC	double	In order to store different directions/positions around the listener, SourcePosition is assumed to vary
 SourcePosition:Type	spherical	m	  	attribute
 SourcePosition:Units	degree, degree, metre	m	  	attribute
 EmitterPosition	[0 0 0]	m	eCI, eCM	double
 EmitterPosition:Type	cartesian	m	  	attribute
 EmitterPosition:Units	metre	m	  	attribute
-GLOBAL:DatabaseName		m	  	attribute	name of the database to which these data belong
-GLOBAL:ListenerShortName		m	  	attribute	ID of the subject from the database
-ListenerUp	[0 0 1]	m	IC, MC	double
-ListenerView	[1 0 0]	m	IC, MC	double
-ListenerView:Type	cartesian	m		attribute
-ListenerView:Units	metre	m		attribute
-Data.SOS	permute([0 0 0 1 0 0; 0 0 0 1 0 0], [3 1 2]);	m	mRn	double	Filter coefficients as SOS coefficients.
+Data.SOS	permute([0 0 0 1 0 0], [3 1 2]);	m	mrn	double	Filter coefficients as SOS coefficients.
 Data.SamplingRate	48000	m	I, M	double	Sampling rate of the coefficients in Data.SOS and the delay in Data.Delay
-Data.SamplingRate:Units	hertz	m		attribute
-Data.Delay	[0 0]	m	IR, MR	double	Broadband delay (in samples resulting from SamplingRate)
+Data.SamplingRate:Units	hertz	m		attribute	Unit of the sampling rate
+Data.Delay	0	m	IR, MR	double	Broadband delay (in samples resulting from SamplingRate)
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldHRTF_2.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleFreeFieldHRTF_1.0.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	SimpleFreeFieldHRTF	rm	  	attribute	This conventions is for HRTFs created under conditions where room information is irrelevant
-GLOBAL:SOFAConventionsVersion	2.0	rm	  	attribute
+GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Comment			 	attribute
 GLOBAL:DataType	TF	rm	  	attribute
@@ -36,9 +36,9 @@
 ListenerUp	[0 0 1]	m	IC, MC	double
 ListenerView	[1 0 0]	m	IC, MC	double
 ListenerView:Type	cartesian	m		attribute
 ListenerView:Units	metre	m		attribute
 Data.Real	[0 0]	m	mRn	double
 Data.Imag	[0 0]	m	MRN	double
 N	0	m	N	double
-N:LongName	frequency			attribute
+N:LongName	frequency	m		attribute	narrative name of N
 N:Units	hertz	m		attribute
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SimpleFreeFieldSOS_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SimpleHeadphoneIR_0.2.csv`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 Name	Default	Flags	Dimensions	Type	Comment
-GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	1.0	rm	 	attribute
-GLOBAL:SOFAConventions	SimpleFreeFieldSOS	rm	  	attribute	This convention set follows SimpleFreeFieldHRIR but the data is stored as second-order section (SOS) coefficients.
-GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
-GLOBAL:APIName		rm	  	attribute
-GLOBAL:APIVersion		rm	  	attribute
-GLOBAL:ApplicationName			  	attribute
-GLOBAL:ApplicationVersion			  	attribute
-GLOBAL:AuthorContact		m	  	attribute
-GLOBAL:Comment			 	attribute
-GLOBAL:DataType	SOS	rm	  	attribute	Filters described as second-order section (SOS) coefficients
-GLOBAL:History			 	attribute
-GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
-GLOBAL:Organization		m	  	attribute
-GLOBAL:References				attribute
-GLOBAL:RoomType	free field	m	  	attribute
-GLOBAL:Origin				attribute
-GLOBAL:DateCreated		m	 	attribute
-GLOBAL:DateModified		m	 	attribute
-GLOBAL:Title		m		attribute
-ListenerPosition	[0 0 0] 	m	IC, MC	double
-ListenerPosition:Type	cartesian	m	  	attribute
-ListenerPosition:Units	metre	m	  	attribute
-ReceiverPosition	[0 0.09 0; 0 -0.09 0]	m	rCI, rCM	double
-ReceiverPosition:Type	cartesian	m	  	attribute
-ReceiverPosition:Units	metre	m	  	attribute
-SourcePosition	[0 0 1]	m	IC, MC	double	Source position is assumed to vary for different directions/positions around the listener
-SourcePosition:Type	spherical	m	  	attribute
-SourcePosition:Units	degree, degree, metre	m	  	attribute
-EmitterPosition	[0 0 0]	m	eCI, eCM	double
-EmitterPosition:Type	cartesian	m	  	attribute
-EmitterPosition:Units	metre	m	  	attribute
-GLOBAL:DatabaseName		m	  	attribute	name of the database to which these data belong
-GLOBAL:ListenerShortName		m	  	attribute	ID of the subject from the database
-ListenerUp	[0 0 1]	m	IC, MC	double
-ListenerView	[1 0 0]	m	IC, MC	double
-ListenerView:Type	cartesian	m		attribute
-ListenerView:Units	metre	m		attribute
-Data.SOS	permute([0 0 0 1 0 0; 0 0 0 1 0 0], [3 1 2]);	m	mRn	double	Filter coefficients as SOS coefficients.
-Data.SamplingRate	48000	m	I	double	Sampling rate of the coefficients in Data.SOS and the delay in Data.Delay
-Data.SamplingRate:Units	hertz	m		attribute
-Data.Delay	[0 0]	m	IR, MR	double	Broadband delay (in samples resulting from SamplingRate)
+GLOBAL:Conventions	SOFA	rm	  	attribute	
+GLOBAL:Version	1.0	rm	 	attribute	
+GLOBAL:SOFAConventions	SimpleHeadphoneIR	rm	  	attribute	Conventions for IRs with a 1-to-1 correspondence between emitter and receiver. The main application for this convention is to store headphone IRs recorded for each emitter and each ear.
+GLOBAL:SOFAConventionsVersion	0.2	rm	  	attribute	
+GLOBAL:APIName		rm	  	attribute	
+GLOBAL:APIVersion		rm	  	attribute	
+GLOBAL:ApplicationName			  	attribute	
+GLOBAL:ApplicationVersion			  	attribute	
+GLOBAL:AuthorContact		m	  	attribute	
+GLOBAL:Comment		m	 	attribute	
+GLOBAL:DataType	FIR	rm	  	attribute	We will store IRs here
+GLOBAL:History			 	attribute	
+GLOBAL:License	No license provided, ask the author for permission	m	  	attribute	
+GLOBAL:Organization		m	  	attribute	
+GLOBAL:References				attribute	
+GLOBAL:RoomType	free field	m	  	attribute	Room type is not relevant here
+GLOBAL:Origin				attribute	
+GLOBAL:DateCreated		m	 	attribute	
+GLOBAL:DateModified		m	 	attribute	
+GLOBAL:Title		m		attribute	
+ListenerPosition	[0 0 0] 	m	IC, MC	double	
+ListenerPosition:Type	cartesian	m	  	attribute	
+ListenerPosition:Units	metre	m	  	attribute	
+ReceiverPosition	[0 0.09 0; 0 -0.09 0]	m	rCI, rCM	double	
+ReceiverPosition:Type	cartesian	m	  	attribute	
+ReceiverPosition:Units	metre	m	  	attribute	
+SourcePosition	[0 0 0]	m	IC, MC	double	Default: Headphones are located at the position of the listener
+SourcePosition:Type	spherical	m	  	attribute	
+SourcePosition:Units	degree, degree, metre	m	  	attribute	
+EmitterPosition	[0 0.09 0; 0 -0.09 0]	m	eCI, eCM	double	Default: Reflects the correspondence of each emitter to each receiver
+EmitterPosition:Type	cartesian	m	  	attribute	
+EmitterPosition:Units	metre	m	  	attribute	
+Data.IR	[0 0]	m	mRn	double	
+Data.SamplingRate	48000	m	I	double	
+Data.SamplingRate:Units	hertz	m		attribute	
+Data.Delay	[0 0]	m	IR, MR	double	
+GLOBAL:DatabaseName		m	  	attribute	Correspondence to a database
+GLOBAL:ListenerShortName		m	  	attribute	Correspondence to a subject from the database
+GLOBAL:ListenerDescription		m		attribute	Narrative description of the listener (or mannequin)
+GLOBAL:SourceDescription		m		attribute	Narrative description of the headphones
+GLOBAL:SourceManufacturer		m		attribute	Name of the headphones manufacturer
+SourceManufacturer	{''}		MS	string	Optional M-dependent version of the attribute SourceManufucturer
+GLOBAL:SourceModel		m		attribute	Name of the headphone model. Must uniquely describe the headphones of the manufacturer
+SourceModel	{''}		MS	string	Optional M-dependent version of the attribute SourceModel
+GLOBAL:SourceURI		m		attribute	URI of the headphone specifications
+GLOBAL:ReceiverDescription		m		attribute	Narrative description of the microphones
+ReceiverDescription	{''}		MS	string	Optional M-dependent version of the attribute ReceiverDescription
+GLOBAL:EmitterDescription		m		attribute	Narrative description of the headphone drivers
+EmitterDescription	{''}		MS	string	Optional M-dependent version of the attribute EmitterDescription
+MeasurementDate	0		M	double	Optional M-dependent date and time of the measurement
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SimpleHeadphoneIR_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SimpleHeadphoneIR_1.0.csv`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	SimpleHeadphoneIR	rm	  	attribute	Conventions for IRs with a 1-to-1 correspondence between emitter and receiver. The main application for this convention is to store headphone IRs recorded for each emitter and each ear.
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:APIName		rm	  	attribute
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:AuthorContact		m	  	attribute
-GLOBAL:Comment		m	 	attribute
+GLOBAL:Comment			 	attribute
 GLOBAL:DataType	FIR	rm	  	attribute	We will store IRs here
 GLOBAL:History			 	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:References				attribute
 GLOBAL:RoomType	free field	m	  	attribute	Room type is not relevant here
 GLOBAL:Origin				attribute
@@ -33,19 +33,19 @@
 EmitterPosition:Units	metre	m	  	attribute
 Data.IR	[0 0]	m	mRn	double
 Data.SamplingRate	48000	m	I, M	double
 Data.SamplingRate:Units	hertz	m		attribute
 Data.Delay	[0 0]	m	IR, MR	double
 GLOBAL:DatabaseName		m	  	attribute	Correspondence to a database
 GLOBAL:ListenerShortName		m	  	attribute	Correspondence to a subject from the database
-GLOBAL:ListenerDescription		m		attribute	Narrative description of the listener (or mannequin)
-GLOBAL:SourceDescription		m		attribute	Narrative description of the headphones
-GLOBAL:SourceManufacturer		m		attribute	Name of the headphones manufacturer
+GLOBAL:ListenerDescription				attribute	Narrative description of the listener (or mannequin)
+GLOBAL:SourceDescription				attribute	Narrative description of the headphones
+GLOBAL:SourceManufacturer				attribute	Name of the headphones manufacturer
 SourceManufacturer	{''}		MS	string	Optional M-dependent version of the attribute SourceManufucturer
-GLOBAL:SourceModel		m		attribute	Name of the headphone model. Must uniquely describe the headphones of the manufacturer
+GLOBAL:SourceModel				attribute	Name of the headphone model. Must uniquely describe the headphones of the manufacturer
 SourceModel	{''}		MS	string	Optional M-dependent version of the attribute SourceModel
-GLOBAL:SourceURI		m		attribute	URI of the headphone specifications
+GLOBAL:SourceURI				attribute	URI of the headphone specifications
 GLOBAL:ReceiverDescription		m		attribute	Narrative description of the microphones
-ReceiverDescription	{''}		MS	string	Optional M-dependent version of the attribute ReceiverDescription
+ReceiverDescriptions	{''}		MS	string	R-dependent version of the attribute ReceiverDescription
 GLOBAL:EmitterDescription		m		attribute	Narrative description of the headphone drivers
-EmitterDescription	{''}		MS	string	Optional M-dependent version of the attribute EmitterDescription
+EmitterDescriptions	{''}		MS	string	E-dependent version of the attribute EmitterDescription
 MeasurementDate	0		M	double	Optional M-dependent date and time of the measurement
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SingleRoomDRIR_0.3.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/deprecated/SingleRoomDRIR_0.2.csv`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Name	Default	Flags	Dimensions	Type	Comment
-GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	1.0	rm	 	attribute
+GLOBAL:Conventions	SOFA	rm	  	attribute	
+GLOBAL:Version	1.0	rm	 	attribute	
 GLOBAL:SOFAConventions	SingleRoomDRIR	rm	  	attribute	This convention stores arbitrary number of receivers while providing an information about the room. The main application is to store DRIRs for a single room.
-GLOBAL:SOFAConventionsVersion	0.3	rm	  	attribute
-GLOBAL:APIName		rm	  	attribute
-GLOBAL:APIVersion		rm	  	attribute
-GLOBAL:ApplicationName			  	attribute
-GLOBAL:ApplicationVersion			  	attribute
-GLOBAL:AuthorContact		m	  	attribute
-GLOBAL:Comment		m	 	attribute
-GLOBAL:DataType	FIR	rm	  	attribute
-GLOBAL:History			 	attribute
-GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
-GLOBAL:Organization		m	  	attribute
-GLOBAL:References				attribute
-GLOBAL:RoomType	reverberant	m	  	attribute
-GLOBAL:Origin				attribute
-GLOBAL:DateCreated		m	 	attribute
-GLOBAL:DateModified		m	 	attribute
-GLOBAL:Title		m		attribute
-ListenerPosition	[0 0 0] 	m	IC, MC	double
-ListenerPosition:Type	cartesian	m	  	attribute
-ListenerPosition:Units	metre	m	  	attribute
-ReceiverPosition	[0 0 0]	m	RCI, RCM	double
-ReceiverPosition:Type	cartesian	m	  	attribute
-ReceiverPosition:Units	metre	m	  	attribute
-SourcePosition	[0 0 0]	m	IC, MC	double
-SourcePosition:Type	cartesian	m	  	attribute
-SourcePosition:Units	metre	m	  	attribute
-EmitterPosition	[0 0 0]	m	eCI, eCM	double
-EmitterPosition:Type	cartesian	m	  	attribute
-EmitterPosition:Units	metre	m	  	attribute
-GLOBAL:DatabaseName		m	  	attribute
-GLOBAL:RoomDescription		m	  	attribute
-ListenerUp	[0 0 1]	m	IC, MC	double
-ListenerView	[1 0 0]	m	IC, MC	double
+GLOBAL:SOFAConventionsVersion	0.2	rm	  	attribute	
+GLOBAL:APIName		rm	  	attribute	
+GLOBAL:APIVersion		rm	  	attribute	
+GLOBAL:ApplicationName			  	attribute	
+GLOBAL:ApplicationVersion			  	attribute	
+GLOBAL:AuthorContact		m	  	attribute	
+GLOBAL:Comment		m	 	attribute	
+GLOBAL:DataType	FIR	rm	  	attribute	
+GLOBAL:History			 	attribute	
+GLOBAL:License	No license provided, ask the author for permission	m	  	attribute	
+GLOBAL:Organization		m	  	attribute	
+GLOBAL:References				attribute	
+GLOBAL:RoomType	reverberant	m	  	attribute	
+GLOBAL:Origin				attribute	
+GLOBAL:DateCreated		m	 	attribute	
+GLOBAL:DateModified		m	 	attribute	
+GLOBAL:Title		m		attribute	
+ListenerPosition	[0 0 0] 	m	IC, MC	double	
+ListenerPosition:Type	cartesian	m	  	attribute	
+ListenerPosition:Units	meter	m	  	attribute	
+ReceiverPosition	[0 0 0]	m	rCI, rCM	double	
+ReceiverPosition:Type	cartesian	m	  	attribute	
+ReceiverPosition:Units	meter	m	  	attribute	
+SourcePosition	[0 0 0]	m	IC, MC	double	
+SourcePosition:Type	cartesian	m	  	attribute	
+SourcePosition:Units	meter	m	  	attribute	
+EmitterPosition	[0 0 0]	m	eCI, eCM	double	
+EmitterPosition:Type	cartesian	m	  	attribute	
+EmitterPosition:Units	meter	m	  	attribute	
+GLOBAL:DatabaseName		m	  	attribute	
+GLOBAL:RoomDescription		m	  	attribute	
+ListenerUp	[0 0 1]	m	IC, MC	double	
+ListenerView	[1 0 0]	m	IC, MC	double	
 ListenerView:Type	cartesian	m		attribute
-ListenerView:Units	metre	m		attribute
-SourceUp	[0 0 1]	m	IC, MC	double
-SourceView	[-1 0 0]	m	IC, MC	double
-SourceView:Type	cartesian	m		attribute
-SourceView:Units	metre	m		attribute
-Data.IR	[0]	m	mrn	double
-Data.SamplingRate	48000	m	I	double
-Data.SamplingRate:Units	hertz	m		attribute
-Data.Delay	[0]	m	IR, MR	double
+ListenerView:Units	metre	m		attribute	
+SourceUp	[0 0 1]	m	IC, MC	double	
+SourceView	[-1 0 0]	m	IC, MC	double	
+SourceView:Type	cartesian	m		attribute	
+SourceView:Units	metre	m		attribute   
+Data.IR	[1]	m	mRn	double	
+Data.SamplingRate	48000	m	I	double	
+Data.SamplingRate:Units	hertz	m		attribute	
+Data.Delay	[0]	m	IR, MR	double
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SingleRoomMIMOSRIR_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomMIMOSRIR_1.0.csv`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	SingleRoomMIMOSRIR	rm	  	attribute	Single-room multiple-input multiple-output spatial room impulse responses, depending on Emitters
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:DataType	FIR-E	rm	  	attribute	Shall be FIR-E
 GLOBAL:RoomType	shoebox	m	  	attribute	Shall be 'shoebox' or 'dae'
 GLOBAL:Title		m		attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
@@ -12,29 +12,43 @@
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:Comment			 	attribute
-GLOBAL:RoomDescription				attribute	narrative description of the room
 GLOBAL:History			 	attribute
 GLOBAL:References				attribute
 GLOBAL:Origin				attribute
+GLOBAL:DatabaseName		m		attribute	Name of the database. Used for classification of the data.
+GLOBAL:RoomShortName				attribute	Short name of the Room
+GLOBAL:RoomDescription				attribute	Informal verbal description of the room
+GLOBAL:RoomLocation				attribute	Location of the room
+GLOBAL:RoomGeometry				attribute	URI to a file describing the room geometry.
+RoomTemperature	0		I, M	double	Temperature during measurements, given in Kelvin.
+RoomTemperature:Units	kelvin			attribute	Units of the room temperature
+RoomVolume	0		I, MI	double	Volume of the room
+RoomVolume:Units	cubic metre			attribute	Units of the room volume
+RoomCornerA	[0 0 0]		IC, MC	double
+RoomCornerB	[1 2 3]		IC, MC	double
+RoomCorners	0		II	double	The value of this attribute is to be ignored. It only exist to for RoomCorners:Type and RoomCorners:Units
+RoomCorners:Type	cartesian			attribute
+RoomCorners:Units	metre			attribute
 GLOBAL:ListenerShortName				attribute
 GLOBAL:ListenerDescription				attribute
 ListenerPosition	[0 0 0] 	m	MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
 ListenerView	[1 0 0]	m	IC, MC	double
 ListenerUp	[0 0 1]	m	IC, MC	double
 ListenerView:Type	cartesian	m		attribute
 ListenerView:Units	metre	m		attribute
 GLOBAL:ReceiverShortName				attribute
 GLOBAL:ReceiverDescription				attribute
+ReceiverDescriptions	{''}		RS, RSM	string	R-dependent version of the attribute ReceiverDescription
 ReceiverPosition	[0 0 0]	m	IC, RCI, RCM	double
 ReceiverPosition:Type	spherical	m	  	attribute	Can be of any type enabling both spatially discrete and spatially continuous representations.
 ReceiverPosition:Units	degree, degree, metre	m	  	attribute
 ReceiverView	[1 0 0]		RCI, RCM	double
 ReceiverUp	[0 0 1]		RCI, RCM	double
 ReceiverView:Type	cartesian			attribute
 ReceiverView:Units	metre			attribute
@@ -45,24 +59,20 @@
 SourcePosition:Units	metre	m	  	attribute
 SourceView	[1 0 0]	m	IC, MC	double
 SourceUp	[0 0 1]	m	IC, MC	double
 SourceView:Type	cartesian	m		attribute
 SourceView:Units	metre	m		attribute
 GLOBAL:EmitterShortName				attribute
 GLOBAL:EmitterDescription				attribute
+EmitterDescriptions	{''}		ES, ESM	string	E-dependent version of the attribute EmitterDescription
 EmitterPosition	[0 0 0]	m	IC, ECI, ECM	double	Can be of any type enabling both spatially discrete and spatially continuous representations.
 EmitterPosition:Type	spherical	m	  	attribute
 EmitterPosition:Units	degree, degree, metre	m	  	attribute
 EmitterView	[1 0 0]		ECI, ECM	double
 EmitterUp	[0 0 1]		ECI, ECM	double
 EmitterView:Type	cartesian			attribute
 EmitterView:Units	metre			attribute
 Data.IR	0	m	mrne	double	Impulse responses
 Data.SamplingRate	48000	m	I, M	double	Sampling rate of the samples in Data.IR and Data.Delay
 Data.SamplingRate:Units	hertz	m		attribute	Unit of the sampling rate
 Data.Delay	0	m	IRI, MRI, MRE	double	Additional delay of each IR (in samples)
-RoomCornerA	[0 0 0]	m	IC, MC	double
-RoomCornerB	[1 2 3]	m	IC, MC	double
-RoomCorners	0		II	double	The value of this attribute is to be ignored. It only exist to for RoomCorners:Type and RoomCorners:Units
-RoomCorners:Type	cartesian	m		attribute
-RoomCorners:Units	metre	m		attribute
-GLOBAL:DatabaseName		m		attribute	Name of the database. Used for classification of the data.
+MeasurementDate	0		M	double	Optional M-dependent date and time of the measurement.
```

### Comparing `sofar-0.3.1/sofar/conventions/source/SingleRoomSRIR_1.0.csv` & `sofar-1.0.0/sofar/sofa_conventions/conventions/SingleRoomSRIR_1.0.csv`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Name	Default	Flags	Dimensions	Type	Comment
 GLOBAL:Conventions	SOFA	rm	  	attribute
-GLOBAL:Version	2.0	rm	 	attribute
+GLOBAL:Version	2.1	rm	 	attribute
 GLOBAL:SOFAConventions	SingleRoomSRIR	rm	  	attribute	For measuring SRIRs in a single room with a single excitation source (e.g., a loudspeaker) and a listener containing an arbitrary number of omnidirectional receivers (e.g., a microphone array).
 GLOBAL:SOFAConventionsVersion	1.0	rm	  	attribute
 GLOBAL:DataType	FIR	rm	  	attribute	Shall be FIR
 GLOBAL:RoomType	shoebox	m	  	attribute	Shall be 'shoebox' or 'dae'
 GLOBAL:Title		m		attribute
 GLOBAL:DateCreated		m	 	attribute
 GLOBAL:DateModified		m	 	attribute
@@ -12,29 +12,43 @@
 GLOBAL:APIVersion		rm	  	attribute
 GLOBAL:AuthorContact		m	  	attribute
 GLOBAL:Organization		m	  	attribute
 GLOBAL:License	No license provided, ask the author for permission	m	  	attribute
 GLOBAL:ApplicationName			  	attribute
 GLOBAL:ApplicationVersion			  	attribute
 GLOBAL:Comment			 	attribute
-GLOBAL:RoomDescription				attribute	narrative description of the room
 GLOBAL:History			 	attribute
 GLOBAL:References				attribute
 GLOBAL:Origin				attribute
+GLOBAL:DatabaseName		m		attribute	Name of the database. Used for classification of the data.
+GLOBAL:RoomShortName				attribute	Short name of the Room
+GLOBAL:RoomDescription				attribute	Informal verbal description of the room
+GLOBAL:RoomLocation				attribute	Location of the room
+GLOBAL:RoomGeometry				attribute	URI to a file describing the room geometry.
+RoomTemperature	0		I, M	double	Temperature during measurements, given in Kelvin.
+RoomTemperature:Units	kelvin			attribute	Units of the room temperature.
+RoomVolume	0		I, M	double	Volume of the room.
+RoomVolume:Units	cubic metre			attribute	Units of the room volume.
+RoomCornerA	[0 0 0]		IC, MC	double
+RoomCornerB	[1 2 3]		IC, MC	double
+RoomCorners	0		II	double	The value of this attribute is to be ignored. It only exist to for RoomCorners:Type and RoomCorners:Units
+RoomCorners:Type	cartesian			attribute
+RoomCorners:Units	metre			attribute
 GLOBAL:ListenerShortName				attribute
 GLOBAL:ListenerDescription				attribute
 ListenerPosition	[0 0 0] 	m	MC	double
 ListenerPosition:Type	cartesian	m	  	attribute
 ListenerPosition:Units	metre	m	  	attribute
 ListenerView	[1 0 0]	m	IC, MC	double
 ListenerUp	[0 0 1]	m	IC, MC	double
 ListenerView:Type	cartesian	m		attribute
 ListenerView:Units	metre	m		attribute
 GLOBAL:ReceiverShortName				attribute
 GLOBAL:ReceiverDescription				attribute
+ReceiverDescriptions	{''}		RS, RSM	string	R-dependent version of the attribute ReceiverDescription
 ReceiverPosition	[0 0 0]	m	IC, RCI, RCM	double
 ReceiverPosition:Type	spherical	m	  	attribute	Can be of any type enabling both spatially discrete and spatially continuous representations.
 ReceiverPosition:Units	degree, degree, metre	m	  	attribute
 ReceiverView	[1 0 0]		RCI, RCM	double
 ReceiverUp	[0 0 1]		RCI, RCM	double
 ReceiverView:Type	cartesian			attribute
 ReceiverView:Units	metre			attribute
@@ -45,24 +59,20 @@
 SourcePosition:Units	metre	m	  	attribute
 SourceView	[1 0 0]	m	IC, MC	double
 SourceUp	[0 0 1]	m	IC, MC	double
 SourceView:Type	cartesian	m		attribute
 SourceView:Units	metre	m		attribute
 GLOBAL:EmitterShortName				attribute
 GLOBAL:EmitterDescription				attribute
+EmitterDescriptions	{''}		ES, ESM	string	E-dependent version of the attribute EmitterDescription
 EmitterPosition	[0 0 0]	m	eCI, eCM	double
 EmitterPosition:Type	spherical	m	  	attribute	Shall be 'cartesian' or 'spherical', restricting to spatially discrete emitters.
 EmitterPosition:Units	degree, degree, metre	m	  	attribute
 EmitterView	[1 0 0]		ECI, ECM	double
 EmitterUp	[0 0 1]		ECI, ECM	double
 EmitterView:Type	cartesian			attribute	Shall be 'cartesian' or 'spherical', restricting to spatially discrete emitters.
 EmitterView:Units	metre			attribute
 Data.IR	0	m	mrn	double	Impulse responses
 Data.SamplingRate	48000	m	I, M	double	Sampling rate of the samples in Data.IR and Data.Delay
 Data.SamplingRate:Units	hertz	m		attribute	Unit of the sampling rate
 Data.Delay	0	m	IR, MR	double	Additional delay of each IR (in samples)
-RoomCornerA	[0 0 0]		IC, MC	double
-RoomCornerB	[1 2 3]		IC, MC	double
-RoomCorners	0		II	double	The value of this attribute is to be ignored. It only exist to for RoomCorners:Type and RoomCorners:Units
-RoomCorners:Type	cartesian			attribute	Type of coordinate system for RoomCornerA and RoomCornerB
-RoomCorners:Units	metre			attribute	Unit of coordinate system for RoomCornerA and RoomCornerB
-GLOBAL:DatabaseName		m		attribute	Name of the database. Used for classification of the data.
+MeasurementDate	0		M	double	Optional M-dependent date and time of the measurement
```

### Comparing `sofar-0.3.1/sofar/sofar.py` & `sofar-1.0.0/sofar/sofa.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import os
 import re
-import glob
 import json
-import requests
 from datetime import datetime
 import platform
 import numpy as np
-import numpy.testing as npt
-from packaging.version import parse as version_parse
 import warnings
-from bs4 import BeautifulSoup
-from netCDF4 import Dataset, stringtochar, chartostring
 from copy import deepcopy
 import sofar as sf
+from .utils import (_nd_newaxis, _atleast_nd, _get_conventions,
+                    _verify_convention_and_version)
 
 
 class Sofa():
     """Create a new SOFA object.
 
     Parameters
     ----------
@@ -100,16 +96,18 @@
             key for key in self._convention.keys()
             if self._read_only(self._convention[key]["flags"])]
 
         # add attributes with default values
         self._convention_to_sofa(mandatory)
 
         # add and update the API
-        if verify:
-            self.verify(version)
+        # (mandatory=False can not be verified because some conventions have
+        # default values that have optional variables as dependencies)
+        if verify and not mandatory:
+            self.verify(mode="read")
 
         self._protected = True
 
     def __setattr__(self, name: str, value):
         # don't allow new attributes to be added outside the class
         if self._protected and not hasattr(self, name):
             raise TypeError(f"{name} is an invalid attribute")
@@ -148,15 +146,20 @@
                 f"{self.GLOBAL_SOFAConventionsVersion}")
 
     @property
     def list_dimensions(self):
         """
         Print the dimensions of the SOFA object
 
-        The SOFA file standard defines the following dimensions:
+        See :py:func:`~Sofa.inspect` to see the shapes of the data inside the
+        SOFA object and :py:func:`~Sofa.get_dimension` to get the size/value
+        of a specific dimensions as integer number.
+
+        The SOFA file standard defines the following dimensions that are used
+        to define the shape of the data entries:
 
         M
             number of measurements
         N
             number of samles, frequencies, SOS coefficients
             (depending on self.GLOBAL_DataType)
         R
@@ -168,35 +171,26 @@
         S
             Maximum length of a string in a string array
         C
             Size of the coordinate dimension. This is always three.
         I
             Single dimension. This is always one.
 
-        see :py:func:`~Sofa.info` to see the shapes of the data inside the SOFA
-        object.
         """
 
         # Check if the dimensions can be updated
         self._update_dimensions()
 
         # get verbose description for dimesion N
         if self.GLOBAL_DataType.startswith("FIR"):
             N_verbose = "samples"
         elif self.GLOBAL_DataType.startswith("TF"):
             N_verbose = "frequencies"
         elif self.GLOBAL_DataType.startswith("SOS"):
             N_verbose = "SOS coefficients"
-        else:
-            # This line can not be tested. An invalid DataType would be cached
-            # in self.verify above. This to make sure we don't miss something
-            # in case new DataTypes are added to SOFA in the future.
-            raise ValueError((
-                "GLOBAL_DataType start with 'FIR', 'TF', "
-                f"or 'SOS' but not with {self.GLOBAL_DataType}"))
 
         # get verbose description for dimensions R and E
         R_verbose = "receiver spherical harmonics coefficients" if \
             'harmonic' in self.ReceiverPosition_Type else "receiver"
         E_verbose = "emitter spherical harmonics coefficients" if \
             'harmonic' in self.EmitterPosition_Type else "emitter"
 
@@ -259,23 +253,23 @@
     def _update_dimensions(self):
         """
         Call verify and raise an error if the dimensions could not be updated.
 
         used in Sofa.list_dimensions and Sofa.get_dimension
         """
 
-        issues = self.verify(version="match", issue_handling="return")
+        issues = self.verify(issue_handling="return")
         if issues is not None and ("data of wrong type" in issues or
                                    "variables of wrong shape" in issues or
                                    not hasattr(self, "_api")):
             raise ValueError(("Dimensions can not be shown because variables "
                               "of wrong type or shape were detected. "
                               "Call Sofa.verify() for more information."))
 
-    def info(self, info):
+    def info(self, info="all"):
         """
         Print information about the convention of a SOFA object.
 
         Prints the variable type (attribute, double, string), shape, flags
         (mandatory, read only) and comment (if any) for each or selected
         entries.
 
@@ -374,15 +368,16 @@
         easy of display, i.e., an array of shape (1, 3, 2) will be displayed as
         an array of shape (3, 2).
 
         Parameters
         ----------
         file : str
             Full path of a file under which the information is to be stored in
-            plain text. The default ``None`` does only print the information.
+            plain text. The default ``None`` only print the information to the
+            console.
         issue_handling : str, optional
             Defines how issues detected during verification of the SOFA object
             are handeled (see :py:func:`~sofar.sofar.Sofa.verify`)
 
             ``'raise'``
                 Warnings and errors are raised if issues are detected
             ``'print'``
@@ -393,15 +388,15 @@
                 Issues are ignored, i.e., not raised, printed, or returned.
 
             The default is ``print'``.
         """
 
         # update the private attribute `_convention` to make sure the required
         # meta data is in place
-        self.verify(version="match", issue_handling=issue_handling)
+        self.verify(issue_handling=issue_handling)
 
         # list of all attributes
         keys = [k for k in self.__dict__.keys() if not k.startswith("_")]
 
         # start printing the information
         info_str = (
             f"{self.GLOBAL_SOFAConventions} "
@@ -444,14 +439,59 @@
         if file is not None:
             with open(file, 'w') as f_id:
                 f_id.write(info_str + "\n")
 
         # output to console
         print(info_str)
 
+    def add_missing(self, mandatory=True, optional=True, verbose=True):
+        """
+        Add missing data with default values.
+
+        Data might be missing in SOFA objects if the creator did not include it
+        or if a new data was suggested for a newer version of a SOFA
+        convention. Use this function to add the data with its default values.
+
+        mandatory : Bool
+            Add missing mandatory data. The default is ``True``.
+        optional : Bool
+            Add missing optional data. The default is ``True``.
+        verbose : Bool
+            Print the information about added data to the console. The default
+            is ``True``.
+        """
+
+        # initialize
+        self._update_convention(version="match")
+        added = "Added the following missing data with their default values:\n"
+
+        # current data
+        keys = [key for key in self.__dict__.keys() if not key.startswith("_")]
+
+        self._protected = False
+
+        # loop data in convention
+        for key in self._convention.keys():
+            is_mandatory = self._mandatory(self._convention[key]["flags"])
+            add_data = (is_mandatory and mandatory) or \
+                (not is_mandatory and optional)
+            # add with default
+            if key not in keys and add_data:
+                setattr(self, key, self._convention[key]["default"])
+                added += f"- {key} "
+                added += f"({'mandatory' if is_mandatory else 'optional'})\n"
+
+        self._protected = True
+
+        if verbose:
+            if "-" in added:
+                print(added)
+            else:
+                print("All mandatory data contained.")
+
     def add_variable(self, name, value, dtype, dimensions):
         """
         Add custom variable to the SOFA object, i.e., numeric or string arrays.
 
         Parameters
         ----------
         name : str
@@ -568,33 +608,244 @@
             dimensions = dimensions.upper()
             for dimension in dimensions:
                 if dimension not in "ERMNCIS":
                     warnings.warn(
                         f"Added custom dimension {dimensions} to SOFA object")
 
         # add attribute to class
-        _add_custom_api_entry(
-            self, name, value, None, dimensions, dtype)
+        self._add_custom_api_entry(name, value, None, dimensions, dtype)
 
-    def verify(self, version="latest", issue_handling="raise"):
+    def _add_custom_api_entry(self, key, value, flags, dimensions, dtype):
+        """
+        Add custom entry to the sofa._convention and permanently save it in
+        sofa._custom
+
+        Parameters
+        ----------
+        key : str
+            name of the entry
+        value: any
+            Value of the entry
+        flags, dimensions, dtype : any
+            as in sofa._convention
+        dimensions : string
+            Dimensions in case of numeric or string array
+        dtype : string
+            double, string, or attribute
+        """
+        # create custom API if it not exists
+        self._protected = False
+
+        # lower case letters to indicate custom dimensions
+        if dimensions is not None:
+            dimensions = [d.upper() if d.upper() in "ERMNCIS" else d.lower()
+                          for d in dimensions]
+            dimensions = "".join(dimensions)
+
+        # add user entry to custom API, if not contained in the convention
+        if not hasattr(self, "_convention") or key not in self._convention:
+            if not hasattr(self, "_custom"):
+                self._custom = {}
+
+            self._custom[key] = {
+                "flags": flags,
+                "dimensions": dimensions,
+                "type": dtype,
+                "default": None,
+                "comment": ""}
+        self._update_convention(version="match")
+
+        # add attribute to object
+        setattr(self, key, value)
+        self._protected = True
+
+    def upgrade_convention(self, target=None, verify=True):
+        """
+        Upgrade Sofa data to newer conventions.
+
+        Calling this with the default arguments returns a list of possible
+        conventions to which the data will be upgraded. If the data is up to
+        date the list will be empty.
+
+        Parameters
+        ----------
+        target : str, optional
+            The convention and version to which the data should be upgraded as
+            a string. For example ``'SimpleFreeFieldHRIR_1.0'`` would upgrade
+            the data to the SOFA-Convention `SimpleFreeFieldHRIR` version 1.0.
+            The default is ``None`` which returns a list of possible
+            conventions to which the data can be updated.
+        verify : bool, optional
+            Flag to specify if the data should be verified after the upgrade
+            using :py:func:`~Sofa.verify`. The default is ``True``.
+
+        Returns
+        -------
+        target : list of strings
+            List with available conventions to which the data can be updated.
+            If the data is up to data, the list will be empty. `target` is only
+            returned if `target` is ``None``.
+        """
+
+        # check input ---------------------------------------------------------
+        self._update_convention(version="match")
+
+        # get deprecations and information about Sofa object
+        _, _, deprecations, upgrade = self._verification_rules()
+        convention_current = self.GLOBAL_SOFAConventions
+        version_current = self.GLOBAL_SOFAConventionsVersion
+        sofa_version_current = self.GLOBAL_Version
+
+        # check if convention is deprecated -----------------------------------
+        is_deprecated = False
+
+        if convention_current in deprecations["GLOBAL:SOFAConventions"]:
+            is_deprecated = True
+        elif convention_current in upgrade:
+            for from_to in upgrade[convention_current]["from_to"]:
+                if version_current in from_to[0]:
+                    is_deprecated = True
+                    break
+
+        # check for upgrades --------------------------------------------------
+        if is_deprecated:
+            version_matched = False
+            # check if upgrade is available for this convention
+            if convention_current not in upgrade:
+                print((f"Convention {convention_current} v{version_current} is"
+                       " outdated but is missing upgrade rules"))
+                return
+
+            # check if upgrade is available for this version
+            for from_to in upgrade[convention_current]["from_to"]:
+                if version_current in from_to[0]:
+                    version_matched = True
+                    targets = from_to[1]
+
+                    if target in targets:
+                        target_id = from_to[2]
+                    else:
+                        if target is not None:
+                            print(f"{target} is invalid.")
+
+                        upgrades = (
+                            f"{convention_current} v{version_current} "
+                            "can be upgraded to:\n")
+                        for t in targets:
+                            t = t.split("_")
+                            upgrades += f"- {t[0]} v{t[1]}\n"
+                        print(upgrades)
+                        return targets
+                    break
+            if not version_matched:
+                print((f"Convention {convention_current} v{version_current} is"
+                       " outdated but is missing upgrade rules"))
+        else:
+            print((f"Convention {convention_current} v{version_current} "
+                   "is up to date"))
+            return
+
+        # get information to upgrade ------------------------------------------
+        upgrade = upgrade[self.GLOBAL_SOFAConventions][target_id]
+        convention_target, version_target = target.split("_")
+
+        # upgrade -------------------------------------------------------------
+        self._convention = self._load_convention(
+            convention_target, version_target)
+        sofa_version_target = self._convention["GLOBAL_Version"]["default"]
+
+        print((f"Upgrading {convention_current} v{version_current} to "
+               f"{convention_target} v{version_target} (SOFA version "
+               f"{sofa_version_current} to {sofa_version_target})"))
+
+        # upgrade convention
+        keys = ["GLOBAL_SOFAConventions",
+                "GLOBAL_SOFAConventionsVersion",
+                "GLOBAL_Version",
+                "GLOBAL_DataType"]
+
+        self._protected = False
+        for key in keys:
+            setattr(self, key, self._convention[key]["default"])
+
+        # move data
+        for source, move in upgrade["move"].items():
+            # get info
+            source_sofar = source.replace(".", '_').replace(":", "_")
+            target_sofar = move["target"].replace(".", '_').replace(":", "_")
+            move_info = f"- Moving {source_sofar} to {target_sofar}."
+            # get data
+            data = getattr(self, source_sofar)
+            # delete from Sofa object
+            delattr(self, source_sofar)
+            # Check move axis
+            moveaxis = upgrade["move"][source]["moveaxis"]
+            if moveaxis is not None:
+                # add dimensions if required
+                # (sofar discards trailing singular dimensions)
+                while data.ndim < np.max(moveaxis) + 1:
+                    data = data[..., None]
+                # move the axis
+                data = np.moveaxis(data, moveaxis[0], moveaxis[1])
+                move_info += f" Moving axis {moveaxis[0]} to {moveaxis[1]}."
+            # Check deprecated dimensions
+            deprecated_dimensions = \
+                upgrade["move"][source]["deprecated_dimensions"]
+            if deprecated_dimensions is not None:
+                move_info += (
+                    f" WARNING: Dimensions {', '.join(deprecated_dimensions)} "
+                    "are now deprecated.")
+            # add data
+            setattr(self, target_sofar, data)
+            # print info
+            print(move_info)
+
+        if not upgrade["move"]:
+            print("- No data to move")
+
+        # remove data
+        for target in upgrade["remove"]:
+            target_sofar = target.replace(".", '_').replace(":", "_")
+            delattr(self, target_sofar)
+            print(f"- Deleting {target_sofar}.")
+
+        if not upgrade["remove"]:
+            print("- No data to remove")
+
+        # check for missing mandatory data
+        self.add_missing(True, False)
+        self._protected = True
+
+        # display general message
+        if upgrade["message"] is not None:
+            print(upgrade["message"])
+
+        if verify:
+            self.verify()
+
+    def verify(self, issue_handling="raise", mode="write"):
         """
         Verify a SOFA object against the SOFA standard.
 
         This function updates the API, and checks the following
 
-        - Are all mandatory fields contained? If not mandatory fields are added
-          with their default value and a warning is raised.
+        - Are all mandatory data contained? If `issue_handling` is ``"raise"``
+          missing mandatory data raises an error. Otherwise mandatory data are
+          added with their default value and a warning is given.
         - Are the names of variables and attributes in accordance to the SOFA
-          standard? If not a warning is raised.
+          standard?
         - Are the data types in accordance with the SOFA standard?
         - Are the dimensions of the variables consistent and in accordance
           to the SOFA standard?
         - Are the values of attributes consistent and in accordance to the
           SOFA standard?
 
+        A detailed set of validation rules can be found at
+        https://github.com/pyfar/sofar/tree/main/sofar/verification_rules
+
         .. note::
             :py:func:`~verify` is automatically called when you create a new
             SOFA object, read a SOFA file from disk, and write a SOFA file to
             disk (using the default parameters).
 
         The API of a SOFA object consists of four parts, that are stored
         dictionaries in private attributes. This is required for writing data
@@ -612,39 +863,35 @@
             specifies the dimensions of the data inside the SOFA object.
         self._custom
             Stores information of custom variables that are not defined by the
             convention. The format is the same as in `self._convention`.
 
         Parameters
         ----------
-        version : str, optional
-            The version to which the API is updated.
-
-            ``'latest'``
-                Use the latest API and upgrade the SOFA file if required.
-            ``'match'``
-                Match the version of the sofa file.
-            str
-                Version string, e.g., ``'1.0'``. Note that this might downgrade
-                the SOFA object
-
-            The default is ``'latest'``
         issue_handling : str, optional
             Defines how detected issues are handeled
 
             ``'raise'``
                 Warnings and errors are raised if issues are detected
             ``'print'``
                 Issues are printed without raising warnings and errors
             ``'return'``
                 Issues are returned as string but neither raised nor printed
-            ``'ignore'``
-                Issues are ignored, i.e., not raised, printed, or returned.
 
             The default is ``'raise'``.
+        mode : str, optional
+            The SOFA standard is more strict for writing data than for reading
+            data.
+
+            ``'write'``
+                All units (e.g. 'meter') must be written be lower case.
+            ``'read'``
+                Units can contain upper case letters (e.g. 'Meter')
+
+            The default is ``'write'``
 
         Returns
         -------
         issues : str, None
             Detected issues as a string. None if no issues were detected. Note
             that this is only returned if ``issue_handling='return'`` (see
             above)
@@ -657,35 +904,42 @@
 
         # initialize warning and error messages
         error_msg = "\nERRORS\n------\n"
         warning_msg = "\nWARNINGS\n--------\n"
 
         # ---------------------------------------------------------------------
         # 0. update the convention
-        self._update_convention(version)
+        self._update_convention("match")
 
         # ---------------------------------------------------------------------
         # 1. check if the mandatory attributes are contained
-        current_warning = ""
+        missing = ""
         keys = [key for key in self.__dict__.keys() if not key.startswith("_")]
 
         for key in self._convention.keys():
             if self._mandatory(self._convention[key]["flags"]) \
                     and key not in keys:
-                # add missing data with default value
-                self._protected = False
-                setattr(self, key, self._convention[key]["default"])
-                self._protected = True
+
+                if issue_handling != "raise":
+                    # add missing data with default value
+                    self._protected = False
+                    setattr(self, key, self._convention[key]["default"])
+                    self._protected = True
 
                 # prepare to raise warning
-                current_warning += "- " + key + "\n"
+                missing += "- " + key + "\n"
 
-        if current_warning:
-            warning_msg += "Added mandatory data with default values:\n"
-            warning_msg += current_warning
+        if missing:
+            if issue_handling == "raise":
+                error_msg += ("Detected missing mandatory data "
+                              "call sofa.add_missing() to fix this):\n")
+                error_msg += missing
+            else:
+                warning_msg += "Added mandatory data with default values:\n"
+                warning_msg += missing
 
         # ---------------------------------------------------------------------
         # 2. verify data type
         current_error = ""
         for key in keys:
 
             # handle dimensions
@@ -801,14 +1055,55 @@
 
         if current_error:
             error_msg += (
                 "Detected variable names with too many underscores."
                 "Underscores are only allowed for the variable Data:\n")
             error_msg += current_error
 
+        # check reserved names
+        current_error = ""
+        for key in keys:
+
+            # AES69-2020 Sec. 4.7.1
+            if key.startswith("PRIVATE") or key.startswith("API"):
+                current_error += "- " + key + "\n"
+            if (key.startswith("GLOBAL") and not key.startswith("GLOBAL_")) or\
+                    (key.startswith("GLOBAL") and
+                     self._convention[key]["type"] != "attribute"):
+                current_error += "- " + key + "\n"
+
+        if current_error:
+            error_msg += (
+                "Detected variable or attribute with reserved key words "
+                "PRIVATE, API, or GLOBAL:\n")
+            error_msg += current_error
+
+        # check names of custom data (shall not have the same name as
+        # normative data contained in the convention AES69-2022 Sec. 5.3)
+        current_error = ""
+        if hasattr(self, "_custom"):
+
+            # get normative variables and attributes
+            normative = sf.Sofa(
+                self.GLOBAL_SOFAConventions,
+                version=self.GLOBAL_SOFAConventionsVersion)._convention.keys()
+            normative = [n.replace("GLOBAL_", "") for n in normative]
+
+            # compare against custom
+            for key in self._custom.keys():
+                if key.replace("GLOBAL_", "") in normative:
+                    current_error += "- " + key + "\n"
+
+        if current_error:
+            error_msg += (
+                "Detected custom variable or attribute with reserved names. "
+                "Custom data shall not have the same name as data contained in"
+                " the convention itself:\n")
+            error_msg += current_error
+
         # ---------------------------------------------------------------------
         # 4. Get dimensions (E, R, M, N, S, c, I, and custom)
 
         # initialize required API fields
         self._protected = False
         self._dimensions = {}
         self._api = {}
@@ -907,179 +1202,292 @@
 
         if current_error:
             error_msg += "Detected variables of wrong shape:\n"
             error_msg += current_error
 
         # ---------------------------------------------------------------------
         # 6. check restrictions on the content of SOFA files
-        data, data_type, api, convention, unit_aliases = _sofa_restrictions()
+        rules, unit_aliases, deprecations, _ = self._verification_rules()
 
-        # general restrictions on data
         current_error = ""
-        for key in data.keys():
+        for key in rules.keys():
 
-            ref = data[key]["value"]
-            if hasattr(self, key):
+            # convert to sofar format
+            key_sofar = key.replace(".", "_").replace(":", "_")
 
-                # test if the value is valid
-                test = getattr(self, key)
-                if not self._verify_value(test, ref, unit_aliases):
-                    current_error += \
-                        f"- {key} is {test} but must be {', '.join(ref)}\n"
+            if not hasattr(self, key_sofar):
+                continue
 
-                # check dependencies
-                if "dependency" not in data[key]:
+            # actual and possible values for the current key
+            test = getattr(self, key_sofar)
+            ref = rules[key]["value"]
+
+            # test if the value is valid
+            if not self._verify_value(test, ref, unit_aliases, key_sofar):
+                current_error += (f"- {key_sofar} is {test} "
+                                  f"but must be {', '.join(ref)}\n")
+
+            # get lower case value for of test for verifying specific
+            # dependencies
+            if isinstance(test, str) and test.lower() in \
+                    ["cartesian", "spherical", "spherical harmonics"]:
+                test = test.lower()
+
+            # check general dependencies
+            items = rules[key]["general"] if "general" in rules[key] else []
+
+            for key_dep in items:
+
+                # convert key to sofar format
+                key_dep = key_dep.replace(".", "_").replace(":", "_")
+
+                # check if dependency is contained in SOFA object hard to test,
+                # for mandatory fields (added by sofar by default).
+                if not hasattr(self, key_dep):
+                    current_error += (f"- {key_dep} must be given if "
+                                      f"{key_sofar} is in SOFA object\n")
                     continue
 
-                for key_dep, ref_dep in data[key]["dependency"].items():
+            # check specific dependencies
+            if "specific" in rules[key] \
+                    and test in rules[key]["specific"]:
+                items = rules[key]["specific"][test].items()
+            else:
+                items = {}.items()
+
+            for key_dep, ref_dep in items:
+
+                if key_dep == "_dimensions":
+                    # requires specific dimension(s) to have a vertain size
+                    for dim in rules[key]["specific"][test]["_dimensions"]:
+                        # possible sizes
+                        dim_ref = \
+                            rules[key]["specific"][test]["_dimensions"][dim]["value"]  # noqa
+                        # current size
+                        dim_act = self._api[dim]
+                        # verbose error string for possible sizes
+                        dim_str = \
+                            rules[key]["specific"][test]["_dimensions"][dim]["value_str"]  # noqa
+                        # perform the check
+                        if dim_act not in dim_ref:
+                            current_error += \
+                                (f"- Dimension {dim} is of size {dim_act} "
+                                 f"but must be {dim_str} if {key_sofar} "
+                                 f"is {test}\n")
+                else:
+
+                    # convert name from NetCDF format to sofar format
+                    key_dep_sofar = key_dep.replace(".", "_").replace(":", "_")
 
                     # check if dependency is contained in SOFA object
-                    # hard to test, because mandatory fields are added by sofar
-                    # this is more to be future proof
-                    if not hasattr(self, key_dep):
-                        current_error += (f"- {key_dep} must be given if "
-                                          f"{key} is in SOFA object\n")
+                    if not hasattr(self, key_dep_sofar):
+                        current_error += (f"- {key_dep_sofar} must be given if"
+                                          f" {key_sofar} is {test}\n")
                         continue
 
                     # check if dependency has the correct value
-                    test_dep = getattr(self, key_dep)
-                    if not (isinstance(ref, list) and
-                            isinstance(ref_dep, list)):
+                    if ref_dep is None:
                         continue
 
-                    idx = ref.index(test)
-                    if not self._verify_value(test_dep, ref_dep[idx],
-                                              unit_aliases):
+                    # convert name from NetCDF format to sofar format
+                    test_dep = getattr(self, key_dep_sofar)
+
+                    if not self._verify_value(
+                            test_dep, ref_dep, unit_aliases, key_dep_sofar):
                         current_error += (
-                            f"- {key_dep} is {test_dep} but must be "
-                            f"{ref_dep[idx]} if {key} is {test}\n")
+                            f"- {key_dep_sofar} is {test_dep} but must be "
+                            f"{', '.join(ref_dep)} if {key_sofar} is {test}\n")
 
-        # restriction posed by GLOBAL_DataType
-        if self.GLOBAL_DataType.startswith("FIR"):
-            data_str = "FIR"
-        elif self.GLOBAL_DataType.startswith("TF"):
-            data_str = "TF"
-        elif self.GLOBAL_DataType.startswith("SOS"):
-            data_str = "SOS"
-        else:
-            # the data type was tested before. This is to prevent redundant
-            # errors in the next for loop
-            data_str = False
-
-        if data_str:
-            for key, value in data_type[data_str].items():
-
-                # hard to test. included to detect problems with future
-                # conventions
-                if not hasattr(self, key):
-                    current_error += (
-                        f"- {key} must be contained if"
-                        f" GLOBAL_DataType={self.GLOBAL_DataType}\n")
-
-                if value is not None and getattr(self, key) not in value[0]:
-                    current_error += (f"{key} is {getattr(self, key)} but "
-                                      f"must be {value[1]}\n")
-
-        # restrictions on the API
-        for key, value in api.items():
-            if hasattr(self, key) and getattr(self, key) == value["value"]:
-                size = getattr(self, "_api")[value["API"][0]]
-                if size not in value["API"][1]:
-                    current_error += \
-                        (f"- Dimension {value['API'][0]} is of size {size} "
-                         f"but must be {value['API'][2]} if "
-                         f"{key} is {getattr(self, key)}\n")
-
-        # restrictions from the SOFA convention (on the data and API)
-        if self.GLOBAL_SOFAConventions in convention:
-            for key, ref in convention[self.GLOBAL_SOFAConventions].items():
-
-                if key == "API":
-                    for dimension, size in ref.items():
-                        if self._api[dimension] != size:
-                            current_error += \
-                    (f"- Dimension {dimension} is of size "  # noqa
-                     f"{self._api[dimension]} but must be {size} if "
-                     f"GLOBAL_SOFAConventions is {key}\n")
-                else:
-                    value = getattr(self, key)
-                    if value not in ref:
-                        current_error += \
-                            f"{key} is {value} but must be {ref}\n"
+        # ---------------------------------------------------------------------
+        # 7. check write only restrictions: units shall be in lower-case
+        # (could be tested in _verify_unit but this way a more verbose error
+        # message can be generated)
+
+        if mode == "write":
+            keys = [k for k in self.__dict__.keys() if k.endswith("Units")]
+            for key in keys:
+                unit = getattr(self, key)
+                if unit.lower() != unit:
+                    current_error += (f"- {key} is {unit} but must contain "
+                                      "only lower case letters when writing "
+                                      "SOFA files to disk.\n")
 
         if current_error:
             error_msg += "Detected violations of the SOFA convention:\n"
             error_msg += current_error
 
-        # handle warnings and errors
+        # ---------------------------------------------------------------------
+        # 8. check deprecations
+        # (so far there are only deprecations for the convention)
+        if self.GLOBAL_SOFAConventions in \
+                deprecations["GLOBAL:SOFAConventions"]:
+            msg = ("Detected deprecations:\n"
+                   f"- GLOBAL_SOFAConventions is "
+                   f"{self.GLOBAL_SOFAConventions}, which is deprecated. Use "
+                   "Sofa.upgrade_convention() to upgrade to "
+                   f"{deprecations['GLOBAL:SOFAConventions'][self.GLOBAL_SOFAConventions]}")  # noqa
+            if mode == "write":
+                error_msg += msg
+            else:
+                warning_msg += msg
+
+        # warn if preliminary conventions versions are used
+        if float(self.GLOBAL_SOFAConventionsVersion) < 1.0:
+            warning_msg += (
+                "\n\nDetected preliminary conventions version "
+                f"{self.GLOBAL_SOFAConventionsVersion}:\n - Upgrade data to "
+                "version >= 1.0 if possible. Preliminary conventions might "
+                "change in the future, which could invalidate data that was "
+                "written before the changes.")
+
+        # ---------------------------------------------------------------------
+        # 9. handle warnings and errors
         if issue_handling != "ignore":
             error_occurred, issues = self._verify_handle_issues(
                     warning_msg, error_msg, issue_handling)
 
             if error_occurred:
                 if issue_handling == "print":
                     return
                 elif issue_handling == "return":
                     return issues
 
     @staticmethod
-    def _verify_value(test, ref, unit_aliases):
+    def _verify_value(test, ref, unit_aliases, key):
         """
         Check a value agains the SOFA standard for Sofa.verify()
 
         Parameters
         ----------
         test :
             the value under test
         ref :
             the value enforced by the SOFA standard
         unit_aliases :
-            dict of aliases for units from _sofa_restrictions()
+            dict of aliases for units from _verification_rules()
+        key :
+            The name of the current attribute, e.g., "GLOBAL_DataType"
 
         Returns
         -------
         ``True`` if `test` and `ref` agree, ``False`` otherwise
         """
 
-        value_valid = True
+        # General case of valid value
+        if ref is None or test in ref:
+            return True
+
+        # only string data should remain for verification
+        if not isinstance(test, str):
+            raise TypeError((
+                "At this point, only string data should remain. Please report "
+                "the issue: github.com/pyfar/sofar/issues"))
+
+        # case sensitive check for DataType and SOFAConventions
+        if key in ["GLOBAL_DataType", "GLOBAL_SOFAConventions"]:
+            if test in ref:
+                return True
+            else:
+                return False
 
-        # Don't check the value if ref is None or test in ref
-        if ref is not None and test not in ref:
+        # general case insensitive test
+        test = test.lower()
+        if test in ref:
+            return True
+
+        # if we are not checking a unit, the test value is invalid
+        if key.endswith("Units"):
+            return sf.Sofa._verify_unit(test, ref, unit_aliases)
+        else:
+            return False
 
-            # in case test is a string it might be a unit and unit aliases
-            # according to the SOFA standard must be checked
+    @staticmethod
+    def _verify_unit(test, ref, unit_aliases):
+        """
+        Verify if a unit string agrees with AES69
 
-            # Following the SOFA standard AES69-2020, units may be separated by
-            # `, ` (comma and space), `,` (comma only), and ` ` (space only).
-            # (regexp ', ?' matches ', ' and ',')
-            ref = re.split(', ?| ', ref) if isinstance(ref, str) else ref
-            units = re.split(', ?| ', test) if isinstance(test, str) else []
-
-            # check if number of units agree
-            if not units or len(ref) != len(units):
-                value_valid = False
-                return value_valid
-
-            # check if units are valid
-            for unit, unit_ref in zip(units, ref):
-                if unit != unit_ref and (unit not in unit_aliases
-                                         or unit_aliases[unit] != unit_ref):
-                    value_valid = False
-                    break
+        Parameters:
+        -----------
+        test : string
+            Current unit string (single units or multiple units separated by
+            commas, commas plus spaces, or spaces).
+        ref : list
+            List of length one containing the LOWER reference case unit string,
+            i.e., only the keys from unit_aliases are allowed words.
+        unit_aliases : dict
+            dict of aliases for units from _verification_rules()
+
+        Returns
+        -------
+        verified : bool
+        """
+        # check format of reference units
+        if not isinstance(ref, list) \
+                or len(ref) != 1 \
+                or not isinstance(ref[0], str):
+            raise TypeError("ref must be a list of length 1 containing a str")
+
+        # Following the SOFA standard AES69-2020, units may be separated by
+        # `, ` (comma and space), `,` (comma only), and ` ` (space only).
+        # (regexp ', ?' matches ', ' and ',')
+        units_ref = re.split(', ?', ref[0])
+        units_test = re.split(', ?', test)
+
+        # check if number of units agree
+        if len(units_ref) != len(units_test):
+            return False
+
+        # check if units are valid
+        for unit_test, unit_ref in zip(units_test, units_ref):
+            if unit_test not in unit_aliases \
+                    or unit_aliases[unit_test] != unit_ref:
+                return False
+
+        return True
 
-        return value_valid
+    @staticmethod
+    def _get_reference_unit(test, unit_aliases):
+        """
+        Return units in reference for, .e.g.,
+        "meter" is converted to "metre" and
+        "degrees degrees,meter" is converted to "degree, degree, metre"
+
+        Parameters:
+        -----------
+        test : string
+            Current unit string MUST be valid, i.e., tested with
+            Sofa._verify_unit (single units or multiple units separated by
+            commas, commas plus spaces, or spaces).
+        unit_aliases : dict
+            dict of aliases for units from _verification_rules()
+
+        Returns
+        -------
+        reference_units : str
+        """
+        # Following the SOFA standard AES69-2020, units may be separated by
+        # `, ` (comma and space), `,` (comma only), and ` ` (space only).
+        # (regexp ', ?' matches ', ' and ',')
+        units_test = re.split(', ?| ', test.lower())
+
+        # get list of reference units
+        units = [unit_aliases[u] for u in units_test]
+        # get reference unit string
+        units = ", ".join(units) if units[0] != "cubic" else " ".join(units)
+
+        return units
 
     @staticmethod
     def _verify_handle_issues(warning_msg, error_msg, issue_handling):
         """Handle warnings and errors from Sofa.verify"""
 
         # handle warnings
         if warning_msg != "\nWARNINGS\n--------\n":
             if issue_handling == "raise":
-                warnings.warn(warning_msg)
+                warnings.warn(UserWarning(warning_msg))
             elif issue_handling == "print":
                 print(warning_msg)
         else:
             warning_msg = None
 
         # handle errors
         if error_msg != "\nERRORS\n------\n":
@@ -1101,14 +1509,45 @@
         elif error_msg:
             issues = error_msg
         else:
             issues = None
 
         return error_occurred, issues
 
+    @staticmethod
+    def _verification_rules():
+        """
+        Return dictionaries to verify SOFA objects in Sofa.verify(). For
+        detailed information see folder 'sofa_conventions'.
+
+        Returns:
+        rules : dict
+            All general and specific verification rules
+        unit_aliases : dict
+            Aliases for specific units allowed in SOFA
+        deprecations : dict
+            Deprecated conventions and their substitute
+        upgrade : dict
+            Rules for upgrading deprecated conventions
+        """
+
+        base = os.path.join(
+            os.path.dirname(__file__), "sofa_conventions", "rules")
+
+        with open(os.path.join(base, "rules.json"), "r") as file:
+            rules = json.load(file)
+        with open(os.path.join(base, "unit_aliases.json"), "r") as file:
+            unit_aliases = json.load(file)
+        with open(os.path.join(base, "deprecations.json"), "r") as file:
+            deprecations = json.load(file)
+        with open(os.path.join(base, "upgrade.json"), "r") as file:
+            upgrade = json.load(file)
+
+        return rules, unit_aliases, deprecations, upgrade
+
     def copy(self):
         """Return a copy of the SOFA object."""
         return deepcopy(self)
 
     def _update_convention(self, version):
         """
         Add SOFA convention to SOFA object in private attribute `_convention`.
@@ -1245,15 +1684,15 @@
 
         # write API and date specific fields (some read only)
         now = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self._protected = False
         self.GLOBAL_DateCreated = now
         self.GLOBAL_DateModified = now
         self.GLOBAL_APIName = "sofar SOFA API for Python (pyfar.org)"
-        self.GLOBAL_APIVersion = sf.__version__
+        self.GLOBAL_APIVersion = sf.version()
         self.GLOBAL_ApplicationName = "Python"
         self.GLOBAL_ApplicationVersion = (
             f"{platform.python_version()} "
             f"[{platform.python_implementation()} - "
             f"{platform.python_compiler()}]")
         self._protected = True
 
@@ -1326,1206 +1765,7 @@
             is_read_only = False
         elif "r" not in flags:
             is_read_only = False
         else:
             is_read_only = True
 
         return is_read_only
-
-
-def _update_conventions(conventions_path=None):
-    """
-    Update SOFA conventions.
-
-    A SOFA convention defines the kind of data and the data format that is
-    stored in a SOFA file. Updating the conventions is done in two steps:
-
-    1.
-        Download official SOFA conventions as csv files from
-        https://github.com/sofacoustics/API_MO/tree/master/API_MO/conventions.
-    2.
-        Convert csv files to json files for easier handling
-
-    The csv and json files are stored at sofar/conventions. Sofar works only on
-    the json files. To get a list of all currently available SOFA conventions
-    and their paths see :py:func:`~sofar.list_conventions`.
-
-    .. note::
-        If the official convention contain errors, calling this function might
-        break sofar. Be sure that you want to do this.
-
-    Parameters
-    ----------
-    conventions_path : str, optional
-        Path to the folder where the conventions are saved. The default is
-        ``None``, which saves the conventions inside the sofar package.
-        Conventions saved under a different path can not be used by sofar.
-    """
-
-    # url for parsing and downloading the convention files
-    url = ("https://github.com/sofacoustics/API_MO/tree/"
-           "master/API_MO/conventions")
-    url_raw = ("https://raw.githubusercontent.com/sofacoustics/API_MO/"
-               "master/API_MO/conventions")
-    ext = 'csv'
-
-    print(f"Reading SOFA conventions from {url} ...")
-
-    # get file names of conventions from the SOFA Matlab/Octave API
-    page = requests.get(url).text
-    soup = BeautifulSoup(page, 'html.parser')
-    conventions = [os.path.split(node.get('href'))[1]
-                   for node in soup.find_all('a')
-                   if node.get('href').endswith(ext)]
-
-    # directory handling
-    if conventions_path is None:
-        conventions_path = os.path.join(os.path.dirname(__file__),
-                                        "conventions")
-    if not os.path.isdir(os.path.join(conventions_path, "source")):
-        os.mkdir(os.path.join(conventions_path, "source"))
-
-    # Loop and download conventions if they changed
-    updated = False
-    for convention in conventions:
-
-        # exclude these conventions
-        if convention.startswith(("General_", "GeneralString_")):
-            continue
-
-        filename_csv = os.path.join(conventions_path, "source", convention)
-
-        # download SOFA convention definitions to package diretory
-        data = requests.get(url_raw + "/" + convention)
-        # remove trailing tabs
-        data = data.content.replace(b"\t\n", b"\n").replace(b"\r\n", b"\n")
-
-        # check if convention needs to be added or updated
-        update = False
-        if not os.path.isfile(filename_csv):
-            update = True
-            updated = f"- added new convention: {convention}"
-        else:
-            with open(filename_csv, "rb") as file:
-                data_current = b"".join(file.readlines())
-                data_current = data_current.replace(b"\r\n", b"\n")
-            if data_current != data:
-                update = True
-                updated = f"- updated existing convention: {convention}"
-
-        # update convention
-        if update:
-            with open(filename_csv, "wb") as file:
-                file.write(data)
-            print(updated)
-
-    # compile json files from csv file
-    # (this is also done if nothing changed. It won't affect the content of
-    #  the json files but the time-stamp will be updated)
-    _compile_conventions()
-
-    if updated:
-        print("... done.")
-    else:
-        print("... conventions already up to date.")
-
-
-def _compile_conventions(conventions_path=None):
-    """
-    Compile SOFA conventions (json files) from source conventions (csv files
-    from SOFA API_MO), i.e., only do step 2 from `_update_conventions`. This is
-    a helper function for debugging and developing and might break sofar.
-
-    Parameters
-    ----------
-    conventions_path : str
-        Path to the folder containing the conventions as json files (might be
-        empty) and the source convention as csv files in the subfolder `source`
-        (must not be empty). The default is ``None``, which uses the
-        default location inside the sofar package.
-    """
-    # directory handling
-    if conventions_path is None:
-        conventions_path = os.path.join(os.path.dirname(__file__),
-                                        "conventions")
-    if not os.path.isdir(os.path.join(conventions_path, "source")):
-        raise ValueError("conventions_path must contain the folder 'source'")
-
-    # get list of source conventions
-    csv_files = glob.glob(os.path.join(
-        conventions_path, "source", "*.csv"))
-    csv_files = [os.path.split(csv_file)[1] for csv_file in csv_files]
-
-    for csv_file in csv_files:
-
-        # directories for reading and writing
-        json_file = os.path.join(conventions_path, csv_file[:-3] + "json")
-        csv_file = os.path.join(conventions_path, "source", csv_file)
-
-        # convert SOFA conventions from csv to json
-        convention_dict = sf.sofar._convention_csv2dict(csv_file)
-        with open(json_file, 'w') as file:
-            json.dump(convention_dict, file, indent=4)
-
-
-def list_conventions():
-    """
-    List available SOFA conventions by printing to the console.
-    """
-    print(_get_conventions("string"))
-
-
-def _get_conventions(return_type):
-    """
-    Get available SOFA conventions.
-
-    Parameters
-    ----------
-    return_type : string, optional
-        ``'path'``
-            Return a list with the full paths and filenames of the convention
-            files (json files)
-        ``'path_source'``
-            Return a list with the full paths and filenames of the source
-            convention files from API_MO (csv files)
-        ``'name'``
-            Return a list of the convention names without version
-        ``'name_version'``
-            Return a list of tuples containing the convention name and version.
-        ``'string'``
-            Returns a string that lists the names and versions of all
-            conventions.
-
-    Returns
-    -------
-    See parameter `return_type`.
-    """
-    # directory containing the SOFA conventions
-    if return_type == "path_source":
-        directory = os.path.join(
-            os.path.dirname(__file__), "conventions", "source")
-        reg_str = "*.csv"
-    else:
-        directory = os.path.join(os.path.dirname(__file__), "conventions")
-        reg_str = "*.json"
-
-    # SOFA convention files
-    paths = [file for file in glob.glob(os.path.join(directory, reg_str))]
-
-    conventions_str = "Available SOFA conventions:\n"
-
-    conventions = []
-    versions = []
-    for path in paths:
-        fileparts = os.path.basename(path).split(sep="_")
-        conventions += [fileparts[0]]
-        versions += [fileparts[1][:-5]]
-        conventions_str += f"{conventions[-1]} (Version {versions[-1]})\n"
-
-    if return_type is None:
-        return
-    elif return_type.startswith("path"):
-        return paths
-    elif return_type == "name":
-        return conventions
-    elif return_type == "name_version":
-        return [(n, v) for n, v in zip(conventions, versions)]
-    elif return_type == "string":
-        return conventions_str
-    else:
-        raise ValueError(f"return_type {return_type} is invalid")
-
-
-def read_sofa(filename, verify=True, version="latest", verbose=True):
-    """
-    Read SOFA file from disk and convert it to SOFA object.
-
-    Numeric data is returned as floats or numpy float arrays unless they have
-    missing data, in which case they are returned as numpy masked arrays.
-
-    Parameters
-    ----------
-    filename : str
-        The filename. '.sofa' is appended to the filename, if it is not
-        explicitly given.
-    verify : bool, optional
-        Verify and update the SOFA object by calling :py:func:`~Sofa.verify`.
-        This helps to find potential errors in the default values and is thus
-        recommended. If reading a file does not work, try to call `Sofa` with
-        ``verify=False``. The default is ``True``.
-    version : str, optional
-        Control if the SOFA file convention is changed.
-
-        ``'latest'``
-            Update the conventions to the latest version
-        ``'match'``
-            Do not change the conventions version, i.e. match the version
-            of the SOFA file that is being read.
-        str
-            Force specific version, e.g., ``'1.0'``. Note that this might
-            downgrade the SOFA object.
-
-        The default is ``'latest'``
-    verbose : bool, optional
-        Print the names of detected custom variables and attributes. The
-        default is ``True``
-
-    Returns
-    -------
-    sofa : Sofa
-        The SOFA object filled with the default values of the convention.
-
-    Notes
-    -----
-
-    1. Missing dimensions are appended when writing the SOFA object to disk.
-       E.g., if ``sofa.Data_IR`` is of shape (1, 2) it is written as an array
-       of shape (1, 2, 1) because the SOFA standard AES69-2020 defines it as a
-       three dimensional array with the dimensions (`M: measurements`,
-       `R: receivers`, `N: samples`)
-    2. When reading data from a SOFA file, array data is always returned as
-       numpy arrays and singleton trailing dimensions are discarded (numpy
-       default). I.e., ``sofa.Data_IR`` will again be an array of shape (1, 2)
-       after writing and reading to and from disk.
-    3. One dimensional arrays with only one element will be converted to scalar
-       values. E.g. ``sofa.Data_SamplingRate`` is stored as an array of shape
-       (1, ) inside SOFA files (according to the SOFA standard AES69-2020) but
-       will be a scalar inside SOFA objects after reading from disk.
-    """
-
-    # check the filename
-    if not filename.endswith('.sofa'):
-        raise ValueError("Filename must end with .sofa")
-    if not os.path.isfile(filename):
-        raise ValueError(f"{filename} does not exist")
-
-    # attributes that are skipped
-    skip = ["_Encoding"]
-
-    # init list of all and custom attributes
-    all_attr = []
-    custom = []
-
-    # open new NETCDF4 file for reading
-    with Dataset(filename, "r", format="NETCDF4") as file:
-
-        # get convention name and version
-        convention = getattr(file, "SOFAConventions")
-        all_attr.append("GLOBAL_SOFAConventions")
-        version_in = getattr(file, "SOFAConventionsVersion")
-        all_attr.append("GLOBAL_SOFAConventionsVersion")
-
-        # check if convention and version exist
-        version_out = _verify_convention_and_version(
-            version, version_in, convention)
-
-        # get SOFA object with default values
-        sofa = sf.Sofa(convention, version=version_out, verify=verify)
-
-        # allow writing read only attributes
-        sofa._protected = False
-
-        # load global attributes
-        for attr in file.ncattrs():
-
-            if attr in ["SOFAConventionsVersion", "SOFAConventions"]:
-                # convention and version were already set above
-                continue
-
-            value = getattr(file, attr)
-            all_attr.append("GLOBAL_" + attr)
-
-            if not hasattr(sofa, "GLOBAL_" + attr):
-                _add_custom_api_entry(sofa, "GLOBAL_" + attr, value, None,
-                                      None, "attribute")
-                custom.append("GLOBAL_" + attr)
-                sofa._protected = False
-            else:
-                setattr(sofa, "GLOBAL_" + attr, value)
-
-        # load data
-        for var in file.variables.keys():
-
-            value = _format_value_from_netcdf(file[var][:], var)
-            all_attr.append(var.replace(".", "_"))
-
-            if hasattr(sofa, var.replace(".", "_")):
-                setattr(sofa, var.replace(".", "_"), value)
-            else:
-                dimensions = "".join([d for d in file[var].dimensions])
-                # SOFA only uses dtypes 'double' and 'S1' but netCDF has more
-                dtype = "string" if file[var].datatype == "S1" else "double"
-                _add_custom_api_entry(sofa, var.replace(".", "_"), value, None,
-                                      dimensions, dtype)
-                custom.append(var.replace(".", "_"))
-                sofa._protected = False
-
-            # load variable attributes
-            for attr in [a for a in file[var].ncattrs() if a not in skip]:
-
-                value = getattr(file[var], attr)
-                all_attr.append(var.replace(".", "_") + "_" + attr)
-
-                if not hasattr(sofa, var.replace(".", "_") + "_" + attr):
-                    _add_custom_api_entry(
-                        sofa, var.replace(".", "_") + "_" + attr, value, None,
-                        None, "attribute")
-                    custom.append(var.replace(".", "_") + "_" + attr)
-                    sofa._protected = False
-                else:
-                    setattr(sofa, var.replace(".", "_") + "_" + attr, value)
-
-    # remove fields from initial Sofa object that were not contained in NetCDF
-    # file (initial Sofa object contained mandatory and optional fields)
-    attrs = [attr for attr in sofa.__dict__.keys() if not attr.startswith("_")]
-    for attr in attrs:
-        if attr not in all_attr:
-            delattr(sofa, attr)
-
-    # do not allow writing read only attributes any more
-    sofa._protected = True
-
-    # notice about custom entries
-    if custom and verbose:
-        print(("SOFA file contained custom entries\n"
-               "----------------------------------\n"
-               f"{', '.join(custom)}"))
-
-    # update api
-    if verify:
-        try:
-            sofa.verify(version)
-        except: # noqa (No error handling - just improved verbosity)
-            raise ValueError((
-                "The SOFA object could not be verified, maybe due to errornous"
-                " data. Call sofa=sofar.read_sofa(filename, verify=False) and "
-                "than sofa.verify() to get more information"))
-
-    return sofa
-
-
-def write_sofa(filename: str, sofa: Sofa, version="latest", compression=4):
-    """
-    Write a SOFA object to disk as a SOFA file.
-
-    Parameters
-    ----------
-    filename : str
-        The filename. '.sofa' is appended to the filename, if it is not
-        explicitly given.
-    sofa : object
-        The SOFA object that is written to disk
-    version : str
-        The SOFA object is verified and updated with :py:func:`~Sofa.verify`
-        before writing to disk. Version specifies, which version of the
-        convention is used:
-
-        ``'latest'``
-            Use the latest version upgrade the SOFA file if required.
-        ``'match'``
-            Match the version of the SOFA object.
-        str
-            Version string, e.g., ``'1.0'``.
-
-        The default is ``'latest'``.
-    compression : int
-        The level of compression with ``0`` being no compression and ``9``
-        being the best compression. The default of ``9`` optimizes the file
-        size but increases the time for writing files to disk.
-
-    Notes
-    -----
-
-    1. Missing dimensions are appended when writing the SOFA object to disk.
-       E.g., if ``sofa.Data_IR`` is of shape (1, 2) it is written as an array
-       of shape (1, 2, 1) because the SOFA standard AES69-2020 defines it as a
-       three dimensional array with the dimensions (`M: measurements`,
-       `R: receivers`, `N: samples`)
-    2. When reading data from a SOFA file, array data is always returned as
-       numpy arrays and singleton trailing dimensions are discarded (numpy
-       default). I.e., ``sofa.Data_IR`` will again be an array of shape (1, 2)
-       after writing and reading to and from disk.
-    3. One dimensional arrays with only one element will be converted to scalar
-       values. E.g. ``sofa.Data_SamplingRate`` is stored as an array of shape
-       (1, ) inside SOFA files (according to the SOFA standard AES69-2020) but
-       will be a scalar inside SOFA objects after reading from disk.
-    """
-
-    # check the filename
-    if not filename.endswith('.sofa'):
-        raise ValueError("Filename must end with .sofa")
-
-    # setting the netCDF compression parameter
-    zlib = False if compression == 0 else True
-
-    # update the dimensions
-    sofa.verify(version)
-
-    # list of all attribute names
-    all_keys = [key for key in sofa.__dict__.keys() if not key.startswith("_")]
-
-    # open new NETCDF4 file for writing
-    with Dataset(filename, "w", format="NETCDF4") as file:
-
-        # write dimensions
-        for dim in sofa._api:
-            file.createDimension(dim, sofa._api[dim])
-
-        # write global attributes
-        keys = [key for key in all_keys if key.startswith("GLOBAL_")]
-        for key in keys:
-            setattr(file, key[7:], str(getattr(sofa, key)))
-
-        # write data
-        for key in all_keys:
-
-            # skip attributes
-            # Note: This definition of attribute is blurry:
-            # lax definition:
-            #   sofa._convention[key]["type"] == "attribute":
-            # strict definition:
-            #   ("_" in key and not key.startswith("Data_")) or \
-            #       key.count("_") > 1
-            #
-            # The strict definition is implicitly included in the SOFA standard
-            # since underscores only occur for variables starting with Data_
-            if sofa._convention[key]["type"] == "attribute":
-                continue
-
-            # get the data and type and shape
-            value, dtype = _format_value_for_netcdf(
-                getattr(sofa, key), key, sofa._convention[key]["type"],
-                sofa._dimensions[key], sofa._api["S"])
-
-            # create variable and write data
-            shape = tuple([dim for dim in sofa._dimensions[key]])
-            tmp_var = file.createVariable(
-                key.replace("Data_", "Data."), dtype, shape,
-                zlib=zlib, complevel=compression)
-            if dtype == "f8":
-                tmp_var[:] = value
-            else:
-                tmp_var[:] = stringtochar(value)
-                tmp_var._Encoding = "ascii"
-
-            # write variable attributes
-            sub_keys = [k for k in all_keys if k.startswith(key + "_")]
-            for sub_key in sub_keys:
-                setattr(tmp_var, sub_key[len(key)+1:],
-                        str(getattr(sofa, sub_key)))
-
-
-def equals(sofa_a, sofa_b, verbose=True, exclude=None):
-    """
-    Compare two SOFA objects against each other.
-
-    Parameters
-    ----------
-    sofa_a : Sofa
-        SOFA object
-    sofa_b : Sofa
-        SOFA object
-    verbose : bool, optional
-        Print differences to the console. The default is True.
-    exclude : str, optional
-        Specify what fields should be excluded from the comparison
-
-        ``'GLOBAL'``
-            Exclude all global attributes, i.e., fields starting with 'GLOBAL:'
-        ``'DATE'``
-            Exclude date attributs, i.e., fields that contain 'Date'
-        ``'ATTR'``
-            Exclude all attributes, i.e., fields that contain ':'
-
-        The default is None, which does not exclude anything.
-
-    Returns
-    -------
-    is_identical : bool
-        ``True`` if sofa_a and sofa_b are identical, ``False`` otherwise.
-    """
-
-    is_identical = True
-
-    # get and filter keys
-    # ('_*' are SOFA object private variables, '__' are netCDF attributes)
-    keys_a = [k for k in sofa_a.__dict__.keys() if not k.startswith("_")]
-    keys_b = [k for k in sofa_b.__dict__.keys() if not k.startswith("_")]
-
-    if exclude is not None:
-        if exclude.upper() == "GLOBAL":
-            keys_a = [k for k in keys_a if not k.startswith("GLOBAL_")]
-            keys_b = [k for k in keys_b if not k.startswith("GLOBAL_")]
-        elif exclude.upper() == "ATTR":
-            keys_a = [k for k in keys_a if
-                      sofa_a._convention[k]["type"] != "attribute"]
-            keys_b = [k for k in keys_b if
-                      sofa_b._convention[k]["type"] != "attribute"]
-        elif exclude.upper() == "DATE":
-            keys_a = [k for k in keys_a if "Date" not in k]
-            keys_b = [k for k in keys_b if "Date" not in k]
-        else:
-            raise ValueError(
-                f"exclude is {exclude} but must be GLOBAL, DATE, or ATTR")
-
-    # check for equal length
-    if len(keys_a) != len(keys_b):
-        is_identical = _equals_raise_warning((
-            f"not identical: sofa_a has {len(keys_a)} attributes for "
-            f"comparison and sofa_b has {len(keys_b)}."), verbose)
-
-        return is_identical
-
-    # check if the keys match
-    if set(keys_a) != set(keys_b):
-        is_identical = _equals_raise_warning(
-            "not identical: sofa_a and sofa_b do not have the ame attributes",
-            verbose)
-
-        return is_identical
-
-    # compare the data inside the SOFA object
-    for key in keys_a:
-
-        # get data and types
-        a = getattr(sofa_a, key)
-        b = getattr(sofa_b, key)
-        type_a = sofa_a._convention[key]["type"]
-        type_b = sofa_b._convention[key]["type"]
-
-        # compare attributes
-        if type_a == "attribute" and type_b == "attribute":
-
-            # handling versions (might be integer, float, or string)
-            if not isinstance(a, str) or not isinstance(a, str):
-                a = str(float(a))
-                b = str(float(b))
-
-            # compare
-            if a != b:
-                is_identical = _equals_raise_warning(
-                    f"not identical: different values for {key}", verbose)
-
-        # compare double variables
-        elif type_a == "double" and type_b == "double":
-
-            try:
-                npt.assert_allclose(np.squeeze(a), np.squeeze(b))
-            except AssertionError:
-                is_identical = _equals_raise_warning(
-                    "not identical: different values for {key}", verbose)
-
-        # compare string variables
-        elif type_a == "string" and type_b == "string":
-            try:
-                assert np.all(
-                    np.squeeze(a).astype("S") == np.squeeze(b).astype("S"))
-            except AssertionError:
-                is_identical = _equals_raise_warning(
-                    "not identical: different values for {key}", verbose)
-        else:
-            is_identical = _equals_raise_warning(
-                (f"not identical: {key} has different data types "
-                 f"({type_a}, {type_b})"), verbose)
-
-    return is_identical
-
-
-def _equals_raise_warning(message, verbose):
-    if verbose:
-        warnings.warn(message)
-    return False
-
-
-def _convention_csv2dict(file: str):
-    """
-    Read SOFA convention from csv file and convert to json file. The csv files
-    are taken from the official Matlab/Octave SOFA API.
-
-    Parameters
-    ----------
-    file : str
-        filename of the SOFA convention
-
-    Returns
-    -------
-    convention : dict
-        SOFA convention as nested dictionary. Each attribute is a sub
-        dictionary with the keys `default`, `flags`, `dimensions`, `type`, and
-        `comment`.
-    """
-
-    # read the file
-    # (encoding should be changed to utf-8 after the SOFA conventions repo is
-    # clean.)
-    # TODO: add explicit test for this function that checks the output
-    with open(file, 'r', encoding="windows-1252") as fid:
-        lines = fid.readlines()
-
-    # write into dict
-    convention = {}
-    for idl, line in enumerate(lines):
-
-        try:
-            # separate by tabs
-            line = line.strip().split("\t")
-            # parse the line entry by entry
-            for idc, cell in enumerate(line):
-                # detect empty cells and leading trailing white spaces
-                cell = None if cell.replace(' ', '') == '' else cell.strip()
-                # nothing to do for empty cells
-                if cell is None:
-                    line[idc] = cell
-                    continue
-                # parse text cells that do not contain arrays
-                if cell[0] != '[':
-                    # check for numbers
-                    try:
-                        cell = float(cell) if '.' in cell else int(cell)
-                    except ValueError:
-                        pass
-
-                    line[idc] = cell
-                    continue
-
-                # parse array cell
-                # remove brackets
-                cell = cell[1:-1]
-
-                if ';' not in cell:
-                    # get rid of white spaces
-                    cell = cell.strip()
-                    cell = cell.replace(' ', ',')
-                    cell = cell.replace(' ', '')
-                    # create flat list of integers and floats
-                    numbers = cell.split(',')
-                    cell = [float(n) if '.' in n else int(n) for n in numbers]
-                else:
-                    # create a nested list of integers and floats
-                    # separate multidimensional arrays
-                    cell = cell.split(';')
-                    cell_nd = [None] * len(cell)
-                    for idx, cc in enumerate(cell):
-                        # get rid of white spaces
-                        cc = cc.strip()
-                        cc = cc.replace(' ', ',')
-                        cc = cc.replace(' ', '')
-                        numbers = cc.split(',')
-                        cell_nd[idx] = [float(n) if '.' in n else int(n)
-                                        for n in numbers]
-
-                    cell = cell_nd
-
-                # write parsed cell to line
-                line[idc] = cell
-
-            # first line contains field names
-            if idl == 0:
-                fields = line[1:]
-                continue
-
-            # add blank comment if it does not exist
-            if len(line) == 5:
-                line.append("")
-            # convert empty defaults from None to ""
-            if line[1] is None:
-                line[1] = ""
-
-            # make sure some unusual default values are converted for json
-            if line[1] == "permute([0 0 0 1 0 0; 0 0 0 1 0 0], [3 1 2]);":
-                # Field Data.SOS in SimpleFreeFieldHRSOS and SimpleFreeFieldSOS
-                line[1] = [[[0, 0, 0, 1, 0, 0], [0, 0, 0, 1, 0, 0]]]
-            if line[1] == "{''}":
-                line[1] = ['']
-            # convert versions to strings
-            if "Version" in line[0] and not isinstance(line[1], str):
-                line[1] = str(float(line[1]))
-
-            # write second to last line
-            convention[line[0]] = {}
-            for ff, field in enumerate(fields):
-                convention[line[0]][field.lower()] = line[ff + 1]
-
-        except: # noqa
-            raise ValueError((f"Failed to parse line {idl}, entry {idc} in: "
-                              f"{file}: \n{line}\n"))
-
-    # reorder the fields to be nicer to read and understand
-    # 1. Move everything to the end that is not GLOBAL
-    keys = [key for key in convention.keys()]
-    for key in keys:
-        if "GLOBAL" not in key:
-            convention[key] = convention.pop(key)
-    # 1. Move Data entries to the end
-    for key in keys:
-        if key.startswith("Data"):
-            convention[key] = convention.pop(key)
-
-    return convention
-
-
-def _format_value_for_netcdf(value, key, dtype, dimensions, S):
-    """
-    Format value from SOFA object for saving in a NETCDF4 file.
-
-    Parameters
-    ----------
-    value : str, array like
-        The value to be formatted
-    key : str
-        The name of the current attribute. Needed for verbose errors.
-    dtype : str
-        The the data type of value
-    dimensions : str
-        The intended dimensions from ``sofa.dimensions``
-    S : int
-        Length of the string array.
-
-    Returns
-    -------
-    value : str, numpy array
-        The formatted value.
-    netcdf_dtype : str
-        The data type as a string for writing to a NETCDF4 file ('attribute',
-        'f8', or 'S1').
-    """
-    # copy value
-    try:
-        value = value.copy()
-    except AttributeError:
-        pass
-
-    # parse data
-    if dtype == "attribute":
-        value = str(value)
-        netcdf_dtype = "attribute"
-    elif dtype == "double":
-        value = _atleast_nd(value, len(dimensions))
-        netcdf_dtype = "f8"
-    elif dtype == "string":
-        value = np.array(value, dtype="S" + str(S))
-        value = _atleast_nd(value, len(dimensions))
-        netcdf_dtype = 'S1'
-    else:
-        raise ValueError(f"Unknown type {dtype} for {key}")
-
-    return value, netcdf_dtype
-
-
-def _format_value_from_netcdf(value, key):
-    """
-    Format value from NETCDF4 file for saving in a SOFA object
-
-    Parameters
-    ----------
-    value : np.array of dtype float or S
-        The value to be formatted
-    key : str
-        The variable name of the current value. Needed for verbose errors.
-
-    Returns
-    -------
-    value : str, number, numpy array
-        The formatted value.
-    """
-
-    if "float" in str(value.dtype) or "int" in str(value.dtype):
-        if np.ma.is_masked(value):
-            warnings.warn(f"Entry {key} contains missing data")
-        else:
-            # Convert to numpy array or scalar
-            value = np.asarray(value)
-    elif str(value.dtype)[1] in ["S", "U"]:
-        # string arrays are stored in masked arrays with empty strings '' being
-        # masked. Convert to regular arrays with unmasked empty strings
-        if str(value.dtype)[1] == "S":
-            value = chartostring(value, encoding="ascii")
-        value = np.atleast_1d(value).astype("U")
-    else:
-        raise TypeError(
-            f"{key}: value.dtype is {value.dtype} but must be float, S or, U")
-
-    # convert arrays to scalars if they do not store data that is usually used
-    # as scalar metadata, e.g., the SamplingRate
-    data_keys = ["Data_IR", "Data_Real", "Data_Imag", "Data_SOS" "Data_Delay"]
-    if value.size == 1 and key not in data_keys:
-        value = value[0]
-
-    return value
-
-
-def _add_custom_api_entry(sofa, key, value, flags, dimensions, dtype):
-    """
-    Add custom entry to the sofa._convention and permanently save it in
-    sofa._custom
-
-    Parameters
-    ----------
-    sofa : Sofa
-    key : str
-        name of the entry
-    flags, dimensions, dtype : any
-        as in sofa._convention
-    """
-    # create custom API if it not exists
-    sofa._protected = False
-    if not hasattr(sofa, "_custom"):
-        sofa._custom = {}
-
-    # lower case letters to indicate custom dimensions
-    if dimensions is not None:
-        dimensions = [d.upper() if d.upper() in "ERMNCIS" else d.lower()
-                      for d in dimensions]
-        dimensions = "".join(dimensions)
-
-    # add user entry to custom API
-    sofa._custom[key] = {
-        "flags": flags,
-        "dimensions": dimensions,
-        "type": dtype,
-        "default": None,
-        "comment": ""}
-    sofa._update_convention(version="match")
-
-    # add attribute to object
-    setattr(sofa, key, value)
-    sofa._protected = True
-
-
-def _verify_convention_and_version(version, version_in, convention):
-    """
-    Verify if convention and version exist and return version
-
-    Parameters
-    ----------
-    version : str
-        'latest', 'match', version string (e.g., '1.0')
-    version_in : str
-        The version to be checked against
-    convention : str
-        The name of the convention to be checked
-
-    Returns
-    -------
-    version_out : str
-        The version to be used depending on `version`, and `version_in`
-    """
-
-    # check if the convention exists in sofar
-    if convention not in _get_conventions("name"):
-        raise ValueError(
-            f"Convention '{convention}' does not exist")
-
-    name_version = _get_conventions("name_version")
-
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
-        if version == "match":
-            match = version_in
-        else:
-            match = version
-
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
-
-
-def _atleast_nd(array, ndim):
-    """
-    Get numpy array with specified number of dimensions. Dimensions are
-    appended at the end if ndim > 3.
-    """
-    try:
-        array = array.copy()
-    except AttributeError:
-        array = array
-
-    if ndim == 1:
-        array = np.atleast_1d(array)
-    if ndim == 2:
-        array = np.atleast_2d(array)
-    if ndim >= 3:
-        array = np.atleast_3d(array)
-    for _ in range(ndim - array.ndim):
-        array = array[..., np.newaxis]
-    return array
-
-
-def _nd_newaxis(array, ndim):
-    """Append dimensions to the end of an array until array.ndim == ndim"""
-    array = np.array(array)
-
-    for _ in range(ndim - array.ndim):
-        array = array[..., np.newaxis]
-    return array
-
-
-def _sofa_restrictions():
-    """
-    Return dictionaries to check restrictions on the data posed by SOFA.
-
-    The check is done in SOFA.verify(). This is not a private class method,
-    to save additional indention that would make the code harder to read and
-    write.
-
-    Returns:
-    data : dict
-        General restrictions on the data of any SOFA convention
-    data_type : dict
-        Restriction depending on GLOBAL_DataType
-    api : dict
-        Restrictions on the API depending on specific fields of a SOFA file
-    """
-
-    # definition of valid coordinate systems and units
-    coords_min = ["cartesian", "spherical"]
-    coords_full = coords_min + ["spherical harmonics"]
-    units_min = ["metre", "degree, degree, metre"]
-    units_full = units_min + [units_min[1]]
-    unit_aliases = {
-        "metres": "metre",
-        "meter": "metre",
-        "meters": "metre",
-        "cubic metres": "cubic metre",
-        "cubic meter": "cubic metre",
-        "cubic meters": "cubic metre",
-        "degrees": "degree",
-        "seconds": "second"
-    }
-    # possible values for restricted dimensions in the API
-    sh_dimension = ([(N+1)**2 for N in range(200)],
-                    "(N+1)**2 where N is the spherical harmonics order")
-    sos_dimension = ([6 * (N + 1) for N in range(1000)],
-                     "an integer multiple of 6 greater 0")
-
-    # restrictions on the data
-    # - if `value` is None it in only checked if the SOFA object has the attr
-    # - if `value` is a list, it is also checked if the actual value is in
-    #   `value`
-    # - if there is a list of values for a dependency the value of the SOFA
-    #   object has to match the value of the list at a certain index. The index
-    #   is determined by the value of the parent.
-    data = {
-        # Global --------------------------------------------------------------
-        # GLOBAL_SOFAConventions?
-        # Check value of GLOBAL_DataType
-        # (FIRE and TFE are legacy data types from SOFA version 1.0)
-        "GLOBAL_DataType": {
-            "value": ["FIR", "FIR-E", "FIRE", "TF", "TF-E", "TFE", "SOS"]},
-        "GLOBAL_RoomType": {
-            "value": ["free field", "reverberant", "shoebox", "dae"]},
-        "GLOBAL_SOFAConventions": {
-            "value": _get_conventions(return_type="name")},
-        # check NLongName
-        "N_LongName": {
-            "value": ["frequency"]},
-        # Listener ------------------------------------------------------------
-        # Check values and consistency of if ListenerPosition Type and Unit
-        "ListenerPosition_Type": {
-            "value": coords_min,
-            "dependency": {
-                "ListenerPosition_Units": units_min}},
-        # Check if dependencies of ListenerView are contained
-        "ListenerView": {
-            "value": None,
-            "dependency": {
-                "ListenerView_Type": None,
-                "ListenerView_Units": None}},
-        # Check values and consistency of if ListenerView Type and Unit
-        "ListenerView_Type": {
-            "value": coords_min,
-            "dependency": {
-                "ListenerView_Units": units_min}},
-        # Check if dependencies of ListenerUp are contained
-        "ListenerUp": {
-            "value": None,
-            "dependency": {
-                "ListenerView": None}},
-        # Receiver ------------------------------------------------------------
-        # Check values and consistency of if ReceiverPosition Type and Unit
-        "ReceiverPosition_Type": {
-            "value": coords_full,
-            "dependency": {
-                "ReceiverPosition_Units": units_full}},
-        # Check if dependencies of ReceiverView are contained
-        "ReceiverView": {
-            "value": None,
-            "dependency": {
-                "ReceiverView_Type": None,
-                "ReceiverView_Units": None}},
-        # Check values and consistency of if ReceiverView Type and Unit
-        "ReceiverView_Type": {
-            "value": coords_min,
-            "dependency": {
-                "ReceiverView_Units": units_min}},
-        # Check if dependencies of ReceiverUp are contained
-        "ReceiverUp": {
-            "value": None,
-            "dependency": {
-                "ReceiverView": None}},
-        # Source --------------------------------------------------------------
-        # Check values and consistency of if SourcePosition Type and Unit
-        "SourcePosition_Type": {
-            "value": coords_min,
-            "dependency": {
-                "SourcePosition_Units": units_min}},
-        # Check if dependencies of SourceView are contained
-        "SourceView": {
-            "value": None,
-            "dependency": {
-                "SourceView_Type": None,
-                "SourceView_Units": None}},
-        # Check values and consistency of if SourceView Type and Unit
-        "SourceView_Type": {
-            "value": coords_min,
-            "dependency": {
-                "SourceView_Units": units_min}},
-        # Check if dependencies of SourceUp are contained
-        "SourceUp": {
-            "value": None,
-            "dependency": {
-                "SourceView": None}},
-        # Emitter -------------------------------------------------------------
-        # Check values and consistency of if EmitterPosition Type and Unit
-        "EmitterPosition_Type": {
-            "value": coords_full,
-            "dependency": {
-                "EmitterPosition_Units": units_full}},
-        # Check if dependencies of EmitterView are contained
-        "EmitterView": {
-            "value": None,
-            "dependency": {
-                "EmitterView_Type": None,
-                "EmitterView_Units": None}},
-        # Check values and consistency of if EmitterView Type and Unit
-        "EmitterView_Type": {
-            "value": coords_min,
-            "dependency": {
-                "EmitterView_Units": units_min}},
-        # Check if dependencies of EmitterUp are contained
-        "EmitterUp": {
-            "value": None,
-            "dependency": {
-                "EmitterView": None}},
-        # Room ----------------------------------------------------------------
-        "RoomVolume": {
-            "value": None,
-            "dependency": {
-                "RoomVolume_Units": None}},
-        "RoomTemperature": {
-            "value": None,
-            "dependency": {
-                "RoomTemperature_Units": None}},
-        "RoomVolume_Units": {
-            "value": ["cubic metre"]},
-        "RoomTemperature_Units": {
-            "value": ["Kelvin"]}
-    }
-
-    # restrictions arising from GLOBAL_DataType
-    # - if `value` is None it is only checked if the SOFA object has the attr
-    # - if `value` is a list, it is also checked if the actual value is in
-    #   `value`
-    data_type = {
-        "FIR": {
-            "Data_IR": None,
-            "Data_Delay": None,
-            "Data_SamplingRate": None,
-            "Data_SamplingRate_Units": (["hertz"], "hertz")},
-        "TF": {
-            "Data_Real": None,
-            "Data_Imag": None,
-            "N": None,
-            # "N_LongName": (["frequency"], "frequency"),  # optional parameter
-            "N_Units": (["hertz"], "hertz")},
-        "SOS": {
-            "Data_SOS": None,
-            "Data_Delay": None,
-            "Data_SamplingRate": None,
-            "Data_SamplingRate_Units": (["hertz"], "hertz")}
-    }
-
-    # restrictions on the API
-    api = {
-        # Check dimension R if using spherical harmonics for the Receiver
-        # (assuming SH orders < 200)
-        "ReceiverPosition_Type": {
-            "value": "spherical harmonics",
-            "API": ("R", ) + sh_dimension},
-        # Check dimension E if using spherical harmonics for the Emitter
-        # (assuming SH orders < 200)
-        "EmitterPosition_Type": {
-            "value": "spherical harmonics",
-            "API": ("E", ) + sh_dimension},
-        # Checking the dimension of N if having SOS data
-        # (assuming up to 1000 second order sections)
-        "GLOBAL_DataType": {
-            "value": "SOS",
-            "API": ("N", ) + sos_dimension}
-    }
-
-    # restrictions from the convention. Values of fields will be checked.
-    # Must contain testing the API. If this would be tested under api={}, the
-    # entry GLOBAL_SOFAConventions would be repeated.
-    convention = {
-        "GeneralFIR": {
-            "GLOBAL_DataType": ["FIR"]},
-        "GeneralFIR-E": {
-            "GLOBAL_DataType": ["FIR-E"]},
-        "GeneralFIRE": {  # SOFA version 1.0 legacy
-            "GLOBAL_DataType": ["FIRE"]},
-        "GeneralTF": {
-            "GLOBAL_DataType": ["TF"]},
-        "GeneralTF-E": {
-            "GLOBAL_DataType": ["TF-E"]},
-        "SimpleFreeFieldHRIR": {
-            "GLOBAL_DataType": ["FIR"],
-            "GLOBAL_RoomType": ["free field"],
-            "EmitterPosition_Type": coords_min,
-            "API": {"E": 1}},
-        "SimpleFreeFieldHRTF": {
-            "GLOBAL_DataType": ["TF"],
-            "GLOBAL_RoomType": ["free field"],
-            "EmitterPosition_Type": coords_min,
-            "API": {"E": 1}},
-        "SimpleFreeFieldHRSOS": {
-            "GLOBAL_DataType": ["SOS"],
-            "GLOBAL_RoomType": ["free field"],
-            "EmitterPosition_Type": coords_min,
-            "API": {"E": 1}},
-        "FreeFieldHRIR": {
-            "GLOBAL_DataType": ["FIR-E"],
-            "GLOBAL_RoomType": ["free field"]},
-        "FreeFieldHRTF": {
-            "GLOBAL_DataType": ["TF-E"],
-            "GLOBAL_RoomType": ["free field"]},
-        "SimpleHeadphoneIR": {
-            "GLOBAL_DataType": ["FIR"]},
-        "SingleRoomSRIR": {
-            "GLOBAL_DataType": ["FIR"]},
-        "SingleRoomMIMOSRIR": {
-            "GLOBAL_DataType": ["FIR-E"]},
-        "FreeFieldDirectivityTF": {
-            "GLOBAL_DataType": ["TF"]}
-    }
-
-    return data, data_type, api, convention, unit_aliases
```

