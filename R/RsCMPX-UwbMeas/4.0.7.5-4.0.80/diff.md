# Comparing `tmp/RsCMPX_UwbMeas-4.0.7.5.tar.gz` & `tmp/RsCMPX_UwbMeas-4.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_UwbMeas-4.0.7.5.tar", last modified: Sun May 16 18:24:58 2021, max compression
+gzip compressed data, was "dist\RsCMPX_UwbMeas-4.0.80.tar", last modified: Tue Dec 20 09:29:19 2022, max compression
```

## Comparing `RsCMPX_UwbMeas-4.0.7.5.tar` & `RsCMPX_UwbMeas-4.0.80.tar`

### file list

```diff
@@ -1,331 +1,472 @@
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.373171 RsCMPX_UwbMeas-4.0.7.5/
--rw-rw-rw-   0        0        0     2516 2021-05-16 18:24:58.372174 RsCMPX_UwbMeas-4.0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     1662 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/README.md
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.026764 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.068652 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/CustomFiles/
--rw-rw-rw-   0        0        0        0 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3304 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4517 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    18659 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.093586 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/
--rw-rw-rw-   0        0        0     1020 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.102562 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/
--rw-rw-rw-   0        0        0     1293 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.117522 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/
--rw-rw-rw-   0        0        0    15446 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.147442 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/
--rw-rw-rw-   0        0        0     1015 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.159410 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation_/
--rw-rw-rw-   0        0        0     8133 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation_/Limit.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation_/__init__.py
--rw-rw-rw-   0        0        0     3514 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Result.py
--rw-rw-rw-   0        0        0     1646 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Spectrum.py
--rw-rw-rw-   0        0        0     1257 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/StsGap.py
--rw-rw-rw-   0        0        0      991 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.168386 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/
--rw-rw-rw-   0        0        0      979 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.183347 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit_/
--rw-rw-rw-   0        0        0     3646 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit_/Area.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/__init__.py
--rw-rw-rw-   0        0        0     5970 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/RfSettings.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/__init__.py
--rw-rw-rw-   0        0        0      995 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.194317 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/
--rw-rw-rw-   0        0        0     1033 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/UwbMeas.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.204294 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/UwbMeas_/
--rw-rw-rw-   0        0        0     1381 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/UwbMeas_/RfSettings.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/UwbMeas_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/__init__.py
--rw-rw-rw-   0        0        0     1007 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.217256 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/
--rw-rw-rw-   0        0        0     1025 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.228227 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/
--rw-rw-rw-   0        0        0     7611 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.237203 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval_/
--rw-rw-rw-   0        0        0     1018 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval_/Catalog.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/__init__.py
--rw-rw-rw-   0        0        0     1025 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.248173 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/
--rw-rw-rw-   0        0        0     7348 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.286072 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/
--rw-rw-rw-   0        0        0     4944 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.380820 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/
--rw-rw-rw-   0        0        0     3893 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Average.py
--rw-rw-rw-   0        0        0     1772 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.405753 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/
--rw-rw-rw-   0        0        0     2596 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Average.py
--rw-rw-rw-   0        0        0     2596 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Current.py
--rw-rw-rw-   0        0        0     2596 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Extreme.py
--rw-rw-rw-   0        0        0     2638 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/__init__.py
--rw-rw-rw-   0        0        0     1744 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.429689 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/
--rw-rw-rw-   0        0        0     1829 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Average.py
--rw-rw-rw-   0        0        0     1829 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Current.py
--rw-rw-rw-   0        0        0     1829 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Extreme.py
--rw-rw-rw-   0        0        0     1861 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/__init__.py
--rw-rw-rw-   0        0        0     1780 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.455620 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/
--rw-rw-rw-   0        0        0     1925 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Average.py
--rw-rw-rw-   0        0        0     1925 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Current.py
--rw-rw-rw-   0        0        0     1925 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Extreme.py
--rw-rw-rw-   0        0        0     1957 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/__init__.py
--rw-rw-rw-   0        0        0     1780 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.480553 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/
--rw-rw-rw-   0        0        0     1925 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Average.py
--rw-rw-rw-   0        0        0     1925 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Current.py
--rw-rw-rw-   0        0        0     1925 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Extreme.py
--rw-rw-rw-   0        0        0     1957 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/__init__.py
--rw-rw-rw-   0        0        0     3893 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Current.py
--rw-rw-rw-   0        0        0     3893 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Extreme.py
--rw-rw-rw-   0        0        0     1772 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.507482 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/
--rw-rw-rw-   0        0        0     2683 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Average.py
--rw-rw-rw-   0        0        0     2683 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Current.py
--rw-rw-rw-   0        0        0     2683 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Extreme.py
--rw-rw-rw-   0        0        0     2725 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/__init__.py
--rw-rw-rw-   0        0        0     1744 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.531417 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/
--rw-rw-rw-   0        0        0     1863 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Average.py
--rw-rw-rw-   0        0        0     1863 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Current.py
--rw-rw-rw-   0        0        0     1863 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Extreme.py
--rw-rw-rw-   0        0        0     1895 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/__init__.py
--rw-rw-rw-   0        0        0     1744 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.559343 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/
--rw-rw-rw-   0        0        0     1919 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Average.py
--rw-rw-rw-   0        0        0     1919 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Current.py
--rw-rw-rw-   0        0        0     1919 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Extreme.py
--rw-rw-rw-   0        0        0     1951 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/__init__.py
--rw-rw-rw-   0        0        0     1781 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.586271 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/
--rw-rw-rw-   0        0        0     2686 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Average.py
--rw-rw-rw-   0        0        0     2686 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Current.py
--rw-rw-rw-   0        0        0     2686 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Extreme.py
--rw-rw-rw-   0        0        0     2728 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/__init__.py
--rw-rw-rw-   0        0        0     1744 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.610208 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/
--rw-rw-rw-   0        0        0     1843 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Average.py
--rw-rw-rw-   0        0        0     1843 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Current.py
--rw-rw-rw-   0        0        0     1843 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Extreme.py
--rw-rw-rw-   0        0        0     1875 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/__init__.py
--rw-rw-rw-   0        0        0     1763 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.632148 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/
--rw-rw-rw-   0        0        0     2854 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Average.py
--rw-rw-rw-   0        0        0     2854 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Current.py
--rw-rw-rw-   0        0        0     2854 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Extreme.py
--rw-rw-rw-   0        0        0     2896 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/__init__.py
--rw-rw-rw-   0        0        0     1799 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.656086 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/
--rw-rw-rw-   0        0        0     2821 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Average.py
--rw-rw-rw-   0        0        0     2821 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Current.py
--rw-rw-rw-   0        0        0     2821 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Extreme.py
--rw-rw-rw-   0        0        0     2863 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/__init__.py
--rw-rw-rw-   0        0        0     1780 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.680021 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/
--rw-rw-rw-   0        0        0     1907 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Average.py
--rw-rw-rw-   0        0        0     1907 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Current.py
--rw-rw-rw-   0        0        0     1907 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Extreme.py
--rw-rw-rw-   0        0        0     1939 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/__init__.py
--rw-rw-rw-   0        0        0     1780 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.702960 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/
--rw-rw-rw-   0        0        0     1903 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Average.py
--rw-rw-rw-   0        0        0     1903 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Current.py
--rw-rw-rw-   0        0        0     1903 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Extreme.py
--rw-rw-rw-   0        0        0     1935 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/__init__.py
--rw-rw-rw-   0        0        0     3925 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/__init__.py
--rw-rw-rw-   0        0        0     3177 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.760806 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/
--rw-rw-rw-   0        0        0     2680 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Average.py
--rw-rw-rw-   0        0        0     2680 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Current.py
--rw-rw-rw-   0        0        0     2014 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.798704 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/
--rw-rw-rw-   0        0        0     1777 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Average.py
--rw-rw-rw-   0        0        0     1777 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Current.py
--rw-rw-rw-   0        0        0     1777 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Maximum.py
--rw-rw-rw-   0        0        0     1777 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Minimum.py
--rw-rw-rw-   0        0        0     1809 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/__init__.py
--rw-rw-rw-   0        0        0     2004 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.830620 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/
--rw-rw-rw-   0        0        0     1751 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Average.py
--rw-rw-rw-   0        0        0     1751 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Current.py
--rw-rw-rw-   0        0        0     1751 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Maximum.py
--rw-rw-rw-   0        0        0     1751 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Minimum.py
--rw-rw-rw-   0        0        0     1783 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/__init__.py
--rw-rw-rw-   0        0        0     2680 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Maximum.py
--rw-rw-rw-   0        0        0     2680 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Minimum.py
--rw-rw-rw-   0        0        0     2014 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.860540 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/
--rw-rw-rw-   0        0        0     1921 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Average.py
--rw-rw-rw-   0        0        0     1921 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Current.py
--rw-rw-rw-   0        0        0     1921 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Maximum.py
--rw-rw-rw-   0        0        0     1921 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Minimum.py
--rw-rw-rw-   0        0        0     1953 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/__init__.py
--rw-rw-rw-   0        0        0     2014 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.890460 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/
--rw-rw-rw-   0        0        0     1793 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Average.py
--rw-rw-rw-   0        0        0     1793 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Current.py
--rw-rw-rw-   0        0        0     1793 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Maximum.py
--rw-rw-rw-   0        0        0     1793 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Minimum.py
--rw-rw-rw-   0        0        0     1825 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/__init__.py
--rw-rw-rw-   0        0        0     2004 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.920380 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/
--rw-rw-rw-   0        0        0     1767 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Average.py
--rw-rw-rw-   0        0        0     1767 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Current.py
--rw-rw-rw-   0        0        0     1767 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Maximum.py
--rw-rw-rw-   0        0        0     1767 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Minimum.py
--rw-rw-rw-   0        0        0     1799 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/__init__.py
--rw-rw-rw-   0        0        0     2712 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/__init__.py
--rw-rw-rw-   0        0        0     4779 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.963265 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/
--rw-rw-rw-   0        0        0     1838 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/AsSymbols.py
--rw-rw-rw-   0        0        0     1671 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Cindex.py
--rw-rw-rw-   0        0        0     1759 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/CsLength.py
--rw-rw-rw-   0        0        0     1832 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Dlength.py
--rw-rw-rw-   0        0        0     1736 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Drate.py
--rw-rw-rw-   0        0        0      957 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.974236 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr_/
--rw-rw-rw-   0        0        0     1838 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr_/Crc.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr_/__init__.py
--rw-rw-rw-   0        0        0     1194 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.988200 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/
--rw-rw-rw-   0        0        0     1609 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/Crc.py
--rw-rw-rw-   0        0        0     1724 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/Length.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/__init__.py
--rw-rw-rw-   0        0        0     1834 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.998172 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/State_/
--rw-rw-rw-   0        0        0     1189 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/State_/__init__.py
--rw-rw-rw-   0        0        0     2488 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.035074 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/
--rw-rw-rw-   0        0        0     1505 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.052029 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/
--rw-rw-rw-   0        0        0     1943 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Average.py
--rw-rw-rw-   0        0        0     1943 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Current.py
--rw-rw-rw-   0        0        0     1771 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Xvalues.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/__init__.py
--rw-rw-rw-   0        0        0     1505 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.069981 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/
--rw-rw-rw-   0        0        0     1943 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/Average.py
--rw-rw-rw-   0        0        0     1943 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/Current.py
--rw-rw-rw-   0        0        0     1769 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/Xvalues.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/__init__.py
--rw-rw-rw-   0        0        0     1489 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.089928 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/
--rw-rw-rw-   0        0        0     2011 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/Average.py
--rw-rw-rw-   0        0        0     2011 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/Current.py
--rw-rw-rw-   0        0        0     1781 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/Xvalues.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/__init__.py
--rw-rw-rw-   0        0        0     1529 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.108877 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/
--rw-rw-rw-   0        0        0     1947 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/Maximum.py
--rw-rw-rw-   0        0        0     1947 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/Minimum.py
--rw-rw-rw-   0        0        0     1745 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/Xvalues.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/__init__.py
--rw-rw-rw-   0        0        0     1505 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.126829 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/
--rw-rw-rw-   0        0        0     1957 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/Average.py
--rw-rw-rw-   0        0        0     1957 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/Current.py
--rw-rw-rw-   0        0        0     1777 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/Xvalues.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/__init__.py
--rw-rw-rw-   0        0        0     1505 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.146776 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/
--rw-rw-rw-   0        0        0     1955 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/Average.py
--rw-rw-rw-   0        0        0     1955 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/Current.py
--rw-rw-rw-   0        0        0     1773 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/Xvalues.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/__init__.py
--rw-rw-rw-   0        0        0     1489 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.165726 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/
--rw-rw-rw-   0        0        0     1965 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Average.py
--rw-rw-rw-   0        0        0     1965 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Current.py
--rw-rw-rw-   0        0        0     1769 2021-05-16 18:24:55.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Xvalues.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/__init__.py
--rw-rw-rw-   0        0        0      997 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.176696 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/
--rw-rw-rw-   0        0        0      983 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.184676 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/
--rw-rw-rw-   0        0        0     2039 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.198637 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/
--rw-rw-rw-   0        0        0     1259 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.212601 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/
--rw-rw-rw-   0        0        0     3274 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/Average.py
--rw-rw-rw-   0        0        0     3251 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/Current.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/__init__.py
--rw-rw-rw-   0        0        0     1259 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.225566 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/
--rw-rw-rw-   0        0        0     3266 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/Average.py
--rw-rw-rw-   0        0        0     3243 2021-05-16 18:24:54.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/Current.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:58.365194 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/
--rw-rw-rw-   0        0        0      541 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4003 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1061 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1000 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9026 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5624 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3354 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2446 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5176 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    20227 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3618 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4409 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    10299 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Core.py
--rw-rw-rw-   0        0        0    38340 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Instrument.py
--rw-rw-rw-   0        0        0     3918 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2081 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0     5101 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3380 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4331 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     3841 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4719 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     4938 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1040 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/StructBase.py
--rw-rw-rw-   0        0        0     2893 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Types.py
--rw-rw-rw-   0        0        0     4530 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Utilities.py
--rw-rw-rw-   0        0        0     4850 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    44232 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     6999 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/__init__.py
--rw-rw-rw-   0        0        0     8568 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/RsCMPX_UwbMeas.py
--rw-rw-rw-   0        0        0      853 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/__init__.py
--rw-rw-rw-   0        0        0     3012 2021-05-16 18:24:52.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/enums.py
--rw-rw-rw-   0        0        0      675 2021-05-16 18:24:52.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/repcap.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:24:57.049703 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas.egg-info/
--rw-rw-rw-   0        0        0     2516 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19074 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-16 18:24:58.376187 RsCMPX_UwbMeas-4.0.7.5/setup.cfg
--rw-rw-rw-   0        0        0      880 2021-05-16 18:24:56.000000 RsCMPX_UwbMeas-4.0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.706301 RsCMPX_UwbMeas-4.0.80/
+-rw-rw-rw-   0        0        0     3136 2022-12-20 09:29:19.704349 RsCMPX_UwbMeas-4.0.80/PKG-INFO
+-rw-rw-rw-   0        0        0     1718 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/README.rst
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.728048 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.752449 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/
+-rw-rw-rw-   0        0        0       90 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3727 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4916 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    21638 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.754401 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.759280 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/
+-rw-rw-rw-   0        0        0      875 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/UwbMeas.py
+-rw-rw-rw-   0        0        0     1033 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.761233 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.763185 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.777824 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.780753 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.797344 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/
+-rw-rw-rw-   0        0        0     2225 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/CcError.py
+-rw-rw-rw-   0        0        0     2241 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Foffset.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.802225 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/
+-rw-rw-rw-   0        0        0     2232 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/Nrmse.py
+-rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/__init__.py
+-rw-rw-rw-   0        0        0     2313 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Plevel.py
+-rw-rw-rw-   0        0        0     2251 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/PmlWidth.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.807108 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/
+-rw-rw-rw-   0        0        0     2240 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/Nrmse.py
+-rw-rw-rw-   0        0        0     1012 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.812961 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/
+-rw-rw-rw-   0        0        0     2232 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/Nrmse.py
+-rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/__init__.py
+-rw-rw-rw-   0        0        0     2223 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SlPeak.py
+-rw-rw-rw-   0        0        0     2289 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SmAccuracy.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.816864 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/
+-rw-rw-rw-   0        0        0     2232 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/Nrmse.py
+-rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/__init__.py
+-rw-rw-rw-   0        0        0     3125 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/__init__.py
+-rw-rw-rw-   0        0        0     1040 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py
+-rw-rw-rw-   0        0        0      850 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.818817 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.823698 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/
+-rw-rw-rw-   0        0        0     2261 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Area.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.828578 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/
+-rw-rw-rw-   0        0        0     3111 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/Area.py
+-rw-rw-rw-   0        0        0     1009 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.832480 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/
+-rw-rw-rw-   0        0        0     3153 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/Area.py
+-rw-rw-rw-   0        0        0     1009 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py
+-rw-rw-rw-   0        0        0     1463 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/__init__.py
+-rw-rw-rw-   0        0        0     1013 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/__init__.py
+-rw-rw-rw-   0        0        0     1267 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Ppdu.py
+-rw-rw-rw-   0        0        0      850 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu.py
+-rw-rw-rw-   0        0        0     4401 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py
+-rw-rw-rw-   0        0        0     2896 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Spectrum.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.834433 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.840289 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/
+-rw-rw-rw-   0        0        0     3972 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py
+-rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py
+-rw-rw-rw-   0        0        0    21130 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.842241 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.847120 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/
+-rw-rw-rw-   0        0        0     2068 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/Range.py
+-rw-rw-rw-   0        0        0     2104 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/__init__.py
+-rw-rw-rw-   0        0        0     5615 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py
+-rw-rw-rw-   0        0        0     1321 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     1044 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.850048 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.854930 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/
+-rw-rw-rw-   0        0        0     1388 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py
+-rw-rw-rw-   0        0        0     2015 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     1023 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.857857 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.859809 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.864689 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/
+-rw-rw-rw-   0        0        0     1025 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     7676 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1051 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     1033 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.866640 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.868592 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.879329 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/
+-rw-rw-rw-   0        0        0     2280 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Clength.py
+-rw-rw-rw-   0        0        0     2562 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Content.py
+-rw-rw-rw-   0        0        0     2506 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/RsParity.py
+-rw-rw-rw-   0        0        0     1543 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.893969 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/
+-rw-rw-rw-   0        0        0     5265 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Average.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.906659 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/
+-rw-rw-rw-   0        0        0     3148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Average.py
+-rw-rw-rw-   0        0        0     4468 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Current.py
+-rw-rw-rw-   0        0        0     3148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Extreme.py
+-rw-rw-rw-   0        0        0     3190 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/StandardDev.py
+-rw-rw-rw-   0        0        0     1804 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.919346 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/
+-rw-rw-rw-   0        0        0     2148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Average.py
+-rw-rw-rw-   0        0        0     3422 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Current.py
+-rw-rw-rw-   0        0        0     2148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Extreme.py
+-rw-rw-rw-   0        0        0     2180 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.931057 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/
+-rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Average.py
+-rw-rw-rw-   0        0        0     3574 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Current.py
+-rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2332 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.945697 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/
+-rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Average.py
+-rw-rw-rw-   0        0        0     3472 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Current.py
+-rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2230 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/__init__.py
+-rw-rw-rw-   0        0        0     6538 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Current.py
+-rw-rw-rw-   0        0        0     5265 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Extreme.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.958385 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/
+-rw-rw-rw-   0        0        0     3235 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Average.py
+-rw-rw-rw-   0        0        0     4555 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Current.py
+-rw-rw-rw-   0        0        0     3235 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Extreme.py
+-rw-rw-rw-   0        0        0     3277 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/StandardDev.py
+-rw-rw-rw-   0        0        0     1804 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.970097 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/
+-rw-rw-rw-   0        0        0     2242 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Average.py
+-rw-rw-rw-   0        0        0     3516 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Current.py
+-rw-rw-rw-   0        0        0     2242 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Extreme.py
+-rw-rw-rw-   0        0        0     2274 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.984737 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/
+-rw-rw-rw-   0        0        0     2156 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Average.py
+-rw-rw-rw-   0        0        0     3430 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Current.py
+-rw-rw-rw-   0        0        0     2156 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Extreme.py
+-rw-rw-rw-   0        0        0     2188 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.997424 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/
+-rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Average.py
+-rw-rw-rw-   0        0        0     3574 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Current.py
+-rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Extreme.py
+-rw-rw-rw-   0        0        0     2332 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/__init__.py
+-rw-rw-rw-   0        0        0     2130 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Otolerance.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.000352 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.011089 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/
+-rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4527 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3248 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.026704 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/
+-rw-rw-rw-   0        0        0     2318 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Average.py
+-rw-rw-rw-   0        0        0     4638 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Current.py
+-rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     3359 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2045 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/__init__.py
+-rw-rw-rw-   0        0        0     1240 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.042324 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/
+-rw-rw-rw-   0        0        0     4288 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Average.py
+-rw-rw-rw-   0        0        0     5608 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Current.py
+-rw-rw-rw-   0        0        0     4288 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     4288 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     4330 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.055009 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/
+-rw-rw-rw-   0        0        0     3115 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Average.py
+-rw-rw-rw-   0        0        0     4435 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Current.py
+-rw-rw-rw-   0        0        0     3115 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Extreme.py
+-rw-rw-rw-   0        0        0     3157 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/StandardDev.py
+-rw-rw-rw-   0        0        0     1809 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.057938 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.068673 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/
+-rw-rw-rw-   0        0        0     3218 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4539 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3218 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3260 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.083313 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/
+-rw-rw-rw-   0        0        0     2326 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Average.py
+-rw-rw-rw-   0        0        0     4650 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Current.py
+-rw-rw-rw-   0        0        0     3329 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     3329 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     3371 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2045 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/__init__.py
+-rw-rw-rw-   0        0        0     1245 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.095025 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/
+-rw-rw-rw-   0        0        0     2162 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Average.py
+-rw-rw-rw-   0        0        0     3436 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Current.py
+-rw-rw-rw-   0        0        0     2162 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Extreme.py
+-rw-rw-rw-   0        0        0     2194 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/StandardDev.py
+-rw-rw-rw-   0        0        0     1803 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.108690 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/
+-rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Average.py
+-rw-rw-rw-   0        0        0     3432 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Current.py
+-rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Extreme.py
+-rw-rw-rw-   0        0        0     2190 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.110641 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.118449 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/
+-rw-rw-rw-   0        0        0     3761 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Current.py
+-rw-rw-rw-   0        0        0     2486 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Extreme.py
+-rw-rw-rw-   0        0        0     1300 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/__init__.py
+-rw-rw-rw-   0        0        0     1043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.120402 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.136017 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/
+-rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4527 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3248 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/__init__.py
+-rw-rw-rw-   0        0        0     1004 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.149681 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/
+-rw-rw-rw-   0        0        0     3460 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Average.py
+-rw-rw-rw-   0        0        0     4780 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Current.py
+-rw-rw-rw-   0        0        0     3460 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Extreme.py
+-rw-rw-rw-   0        0        0     3502 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/StandardDev.py
+-rw-rw-rw-   0        0        0     1799 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.165297 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/
+-rw-rw-rw-   0        0        0     3463 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Average.py
+-rw-rw-rw-   0        0        0     4783 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Current.py
+-rw-rw-rw-   0        0        0     3463 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Extreme.py
+-rw-rw-rw-   0        0        0     3505 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/StandardDev.py
+-rw-rw-rw-   0        0        0     1819 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.180445 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/
+-rw-rw-rw-   0        0        0     2274 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Average.py
+-rw-rw-rw-   0        0        0     3548 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Current.py
+-rw-rw-rw-   0        0        0     2274 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2306 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.194109 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/
+-rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Average.py
+-rw-rw-rw-   0        0        0     3472 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Current.py
+-rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2230 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/__init__.py
+-rw-rw-rw-   0        0        0     5297 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StandardDev.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.196060 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.207774 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/
+-rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4527 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3248 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.214604 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/
+-rw-rw-rw-   0        0        0     3761 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Current.py
+-rw-rw-rw-   0        0        0     2486 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Extreme.py
+-rw-rw-rw-   0        0        0     1300 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.229245 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/
+-rw-rw-rw-   0        0        0     2318 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Average.py
+-rw-rw-rw-   0        0        0     4638 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Current.py
+-rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     3359 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2045 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/__init__.py
+-rw-rw-rw-   0        0        0     1508 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.232173 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.239981 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/
+-rw-rw-rw-   0        0        0     4182 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Current.py
+-rw-rw-rw-   0        0        0     2907 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Extreme.py
+-rw-rw-rw-   0        0        0     1300 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/__init__.py
+-rw-rw-rw-   0        0        0     1048 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/__init__.py
+-rw-rw-rw-   0        0        0     7239 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.244861 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.246812 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.251694 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/
+-rw-rw-rw-   0        0        0     3443 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/Margin.py
+-rw-rw-rw-   0        0        0     1831 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/__init__.py
+-rw-rw-rw-   0        0        0     1005 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.254621 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.261453 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/
+-rw-rw-rw-   0        0        0     3568 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/Current.py
+-rw-rw-rw-   0        0        0     1839 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.268544 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/
+-rw-rw-rw-   0        0        0     3721 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Current.py
+-rw-rw-rw-   0        0        0     2446 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Extreme.py
+-rw-rw-rw-   0        0        0     1305 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/__init__.py
+-rw-rw-rw-   0        0        0     1286 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/__init__.py
+-rw-rw-rw-   0        0        0     1676 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Otolerance.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.270498 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.275376 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/
+-rw-rw-rw-   0        0        0     3443 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/Margin.py
+-rw-rw-rw-   0        0        0     1831 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/__init__.py
+-rw-rw-rw-   0        0        0     1005 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/__init__.py
+-rw-rw-rw-   0        0        0     1744 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.289041 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/
+-rw-rw-rw-   0        0        0     3077 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Average.py
+-rw-rw-rw-   0        0        0     4350 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Current.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.304658 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/
+-rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Average.py
+-rw-rw-rw-   0        0        0     3432 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Current.py
+-rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Maximum.py
+-rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Minimum.py
+-rw-rw-rw-   0        0        0     2190 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.320274 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/
+-rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Average.py
+-rw-rw-rw-   0        0        0     3426 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Current.py
+-rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Maximum.py
+-rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Minimum.py
+-rw-rw-rw-   0        0        0     2184 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/StandardDev.py
+-rw-rw-rw-   0        0        0     2043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/__init__.py
+-rw-rw-rw-   0        0        0     3077 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Maximum.py
+-rw-rw-rw-   0        0        0     3077 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Minimum.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.335888 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/
+-rw-rw-rw-   0        0        0     2206 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Average.py
+-rw-rw-rw-   0        0        0     3480 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Current.py
+-rw-rw-rw-   0        0        0     2206 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Maximum.py
+-rw-rw-rw-   0        0        0     2206 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Minimum.py
+-rw-rw-rw-   0        0        0     2238 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.350528 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/
+-rw-rw-rw-   0        0        0     2214 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Average.py
+-rw-rw-rw-   0        0        0     3488 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Current.py
+-rw-rw-rw-   0        0        0     2214 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Maximum.py
+-rw-rw-rw-   0        0        0     2214 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Minimum.py
+-rw-rw-rw-   0        0        0     2246 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2053 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.369581 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/
+-rw-rw-rw-   0        0        0     2166 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Average.py
+-rw-rw-rw-   0        0        0     3440 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Current.py
+-rw-rw-rw-   0        0        0     2166 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Maximum.py
+-rw-rw-rw-   0        0        0     2166 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Minimum.py
+-rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.391058 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/
+-rw-rw-rw-   0        0        0     2160 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Average.py
+-rw-rw-rw-   0        0        0     3434 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Current.py
+-rw-rw-rw-   0        0        0     2160 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py
+-rw-rw-rw-   0        0        0     2160 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py
+-rw-rw-rw-   0        0        0     2192 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/StandardDev.py
+-rw-rw-rw-   0        0        0     2043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py
+-rw-rw-rw-   0        0        0     3109 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/StandardDev.py
+-rw-rw-rw-   0        0        0     3493 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.426189 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/
+-rw-rw-rw-   0        0        0     2170 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py
+-rw-rw-rw-   0        0        0     2049 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Cindex.py
+-rw-rw-rw-   0        0        0     2109 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/CsLength.py
+-rw-rw-rw-   0        0        0     2150 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dlength.py
+-rw-rw-rw-   0        0        0     1681 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dppdu.py
+-rw-rw-rw-   0        0        0     2102 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Drate.py
+-rw-rw-rw-   0        0        0     2305 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/FcsCheck.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.436925 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/
+-rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/AsSymbols.py
+-rw-rw-rw-   0        0        0     2989 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Bitrate.py
+-rw-rw-rw-   0        0        0     2289 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py
+-rw-rw-rw-   0        0        0     1491 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.446686 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/
+-rw-rw-rw-   0        0        0     2064 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py
+-rw-rw-rw-   0        0        0     2103 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py
+-rw-rw-rw-   0        0        0     1228 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py
+-rw-rw-rw-   0        0        0     3056 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/PstGap.py
+-rw-rw-rw-   0        0        0     2092 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/RaBit.py
+-rw-rw-rw-   0        0        0     2096 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/ReBit.py
+-rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Sfd.py
+-rw-rw-rw-   0        0        0     2118 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/SfdLength.py
+-rw-rw-rw-   0        0        0     8135 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.451564 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/
+-rw-rw-rw-   0        0        0     2110 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/All.py
+-rw-rw-rw-   0        0        0     2751 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.454492 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.466205 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/
+-rw-rw-rw-   0        0        0     1870 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py
+-rw-rw-rw-   0        0        0     3592 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Current.py
+-rw-rw-rw-   0        0        0     1780 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.475965 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/
+-rw-rw-rw-   0        0        0     1868 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py
+-rw-rw-rw-   0        0        0     3590 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Current.py
+-rw-rw-rw-   0        0        0     1776 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.486701 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/
+-rw-rw-rw-   0        0        0     1936 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Average.py
+-rw-rw-rw-   0        0        0     3658 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Current.py
+-rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Xvalues.py
+-rw-rw-rw-   0        0        0     1522 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.497436 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/
+-rw-rw-rw-   0        0        0     3560 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Current.py
+-rw-rw-rw-   0        0        0     1768 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Xvalues.py
+-rw-rw-rw-   0        0        0     1273 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.509148 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/
+-rw-rw-rw-   0        0        0     2384 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Maximum.py
+-rw-rw-rw-   0        0        0     2384 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Minimum.py
+-rw-rw-rw-   0        0        0     1768 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Xvalues.py
+-rw-rw-rw-   0        0        0     1547 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.520860 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/
+-rw-rw-rw-   0        0        0     1848 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Average.py
+-rw-rw-rw-   0        0        0     3570 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Current.py
+-rw-rw-rw-   0        0        0     1760 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Xvalues.py
+-rw-rw-rw-   0        0        0     1512 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.531596 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/
+-rw-rw-rw-   0        0        0     1846 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Average.py
+-rw-rw-rw-   0        0        0     3568 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Current.py
+-rw-rw-rw-   0        0        0     1758 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Xvalues.py
+-rw-rw-rw-   0        0        0     1512 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.542334 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/
+-rw-rw-rw-   0        0        0     1882 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Average.py
+-rw-rw-rw-   0        0        0     3604 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Current.py
+-rw-rw-rw-   0        0        0     1784 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.552093 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/
+-rw-rw-rw-   0        0        0     1880 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Average.py
+-rw-rw-rw-   0        0        0     3602 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Current.py
+-rw-rw-rw-   0        0        0     1780 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.565757 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/
+-rw-rw-rw-   0        0        0     1866 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Average.py
+-rw-rw-rw-   0        0        0     3588 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Current.py
+-rw-rw-rw-   0        0        0     1776 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Xvalues.py
+-rw-rw-rw-   0        0        0     1522 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/__init__.py
+-rw-rw-rw-   0        0        0     3209 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.573565 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.576493 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.588205 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/
+-rw-rw-rw-   0        0        0     2432 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Average.py
+-rw-rw-rw-   0        0        0     3667 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Current.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.598940 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/
+-rw-rw-rw-   0        0        0     3701 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py
+-rw-rw-rw-   0        0        0     4954 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Current.py
+-rw-rw-rw-   0        0        0     1287 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.607726 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/
+-rw-rw-rw-   0        0        0     3701 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py
+-rw-rw-rw-   0        0        0     4954 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Current.py
+-rw-rw-rw-   0        0        0     1287 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py
+-rw-rw-rw-   0        0        0     2572 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/__init__.py
+-rw-rw-rw-   0        0        0     1011 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/__init__.py
+-rw-rw-rw-   0        0        0     2102 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Otolerance.py
+-rw-rw-rw-   0        0        0     1293 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/__init__.py
+-rw-rw-rw-   0        0        0     5413 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1051 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.701421 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/
+-rw-rw-rw-   0        0        0      586 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4165 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1116 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1145 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9097 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5751 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3439 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2546 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5238 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    25292 2022-12-19 08:08:03.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3781 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4812 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    12772 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Core.py
+-rw-rw-rw-   0        0        0     1386 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/GlobalData.py
+-rw-rw-rw-   0        0        0    59235 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4785 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2225 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0    12709 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3518 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4390 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0     4289 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4745 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ScpiEnums.py
+-rw-rw-rw-   0        0        0    34488 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ScpiLogger.py
+-rw-rw-rw-   0        0        0     5098 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5856 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1114 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3608 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Types.py
+-rw-rw-rw-   0        0        0     5498 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5632 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    49606 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7361 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0       29 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/__init__.py
+-rw-rw-rw-   0        0        0    12875 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/RsCMPX_UwbMeas.py
+-rw-rw-rw-   0        0        0      932 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     3542 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/enums.py
+-rw-rw-rw-   0        0        0     3166 2022-12-20 09:29:10.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/repcap.py
+drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.742689 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/
+-rw-rw-rw-   0        0        0     3136 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    26592 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-20 09:29:19.706301 RsCMPX_UwbMeas-4.0.80/setup.cfg
+-rw-rw-rw-   0        0        0     1435 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/setup.py
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/CustomFiles/events.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,89 @@
-from typing import Callable
-
-from ..Internal import Core
-
-
-class Events:
-	"""Common Events class.
-	Event-related methods common for all types of drivers."""
-	def __init__(self, core: Core):
-		self._core = core
-
-	@property
-	def io_events_include_data(self) -> bool:
-		"""Returns the current state of the io_events_include_data See the setter for more details."""
-		return self._core.io.io_events_include_data
-
-	@io_events_include_data.setter
-	def io_events_include_data(self, value: bool) -> None:
-		"""If True, the on_write and on_read events include also the sent/received data.
-		Default value is False, to avoid handling potentially big data."""
-		self._core.io.io_events_include_data = value
-
-	@property
-	def before_write_handler(self) -> Callable:
-		"""Returns the handler of before_write events. \n
-		:return: current before_write_handler"""
-		return self._core.io.before_write_handler
-
-	@before_write_handler.setter
-	def before_write_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_write events.
-		The before_write event is invoked before each write operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, cmd: str)
-		:param handler: new handler"""
-		self._core.io.before_write_handler = handler
-
-	@property
-	def on_write_handler(self) -> Callable:
-		"""Returns the handler of on_write events. \n
-		:return: current on_write_handler"""
-		return self._core.io.on_write_handler
-
-	@on_write_handler.setter
-	def on_write_handler(self, handler: Callable) -> None:
-		"""Sets handler for on_write events.
-		The on_write event is invoked every time the driver performs a write operation to the instrument (for each write chunk)
-		Event arguments type: IoTransferEventArgs
-		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
-		:param handler: new handler for all write operations"""
-		self._core.io.on_write_handler = handler
-
-	@property
-	def on_read_handler(self) -> Callable:
-		"""Returns the handler of on_read events. \n
-		:return: current on_read_handler"""
-		return self._core.io.on_read_handler
-
-	@on_read_handler.setter
-	def on_read_handler(self, handler: Callable) -> None:
-		"""Sets handler for on_read events.
-		The on_read event is invoked every time the driver performs a read operation to the instrument.
-		Event arguments type: IoTransferEventArgs
-		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
-		:param handler: new handler for all read operations"""
-		self._core.io.on_read_handler = handler
-
-	@property
-	def before_query_handler(self) -> Callable:
-		"""Returns the handler of before_query events. \n
-		:return: current before_query_handler"""
-		return self._core.io.before_query_handler
-
-	@before_query_handler.setter
-	def before_query_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_query events.
-		The before_query event is invoked before each query operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, query: str)
-		:param handler: new handler"""
-		self._core.io.before_query_handler = handler
+"""Event-related methods and properties. Here you can set all the event handlers."""
+
+from typing import Callable
+
+from ..Internal import Core
+
+
+class Events:
+	"""Common Events class.
+	Event-related methods and properties. Here you can set all the event handlers."""
+	def __init__(self, core: Core):
+		self._core = core
+
+	@property
+	def io_events_include_data(self) -> bool:
+		"""Returns the current state of the io_events_include_data See the setter for more details."""
+		return self._core.io.io_events_include_data
+
+	@io_events_include_data.setter
+	def io_events_include_data(self, value: bool) -> None:
+		"""If True, the on_write and on_read events include also the sent/received data.
+		Default value is False, to avoid handling potentially big data."""
+		self._core.io.io_events_include_data = value
+
+	@property
+	def before_write_handler(self) -> Callable:
+		"""Returns the handler of before_write events. \n
+		:return: current ``before_write_handler``"""
+		return self._core.io.before_write_handler
+
+	@before_write_handler.setter
+	def before_write_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_write events.
+		The before_write event is invoked before each write operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, cmd: str)
+		:param handler: new handler"""
+		self._core.io.before_write_handler = handler
+
+	@property
+	def on_write_handler(self) -> Callable:
+		"""Returns the handler of on_write events. \n
+		:return: current ``on_write_handler``"""
+		return self._core.io.on_write_handler
+
+	@on_write_handler.setter
+	def on_write_handler(self, handler: Callable) -> None:
+		"""Sets handler for on_write events.
+		The on_write event is invoked every time the driver performs a write operation to the instrument (for each write chunk)
+		Event arguments type: IoTransferEventArgs
+		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
+		:param handler: new handler for all write operations"""
+		self._core.io.on_write_handler = handler
+
+	@property
+	def on_read_handler(self) -> Callable:
+		"""Returns the handler of on_read events. \n
+		:return: current ``on_read_handler``"""
+		return self._core.io.on_read_handler
+
+	@on_read_handler.setter
+	def on_read_handler(self, handler: Callable) -> None:
+		"""Sets handler for on_read events.
+		The on_read event is invoked every time the driver performs a read operation to the instrument.
+		Event arguments type: IoTransferEventArgs
+		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
+		:param handler: new handler for all read operations"""
+		self._core.io.on_read_handler = handler
+
+	@property
+	def before_query_handler(self) -> Callable:
+		"""Returns the handler of before_query events. \n
+		:return: current ``before_query_handler``"""
+		return self._core.io.before_query_handler
+
+	@before_query_handler.setter
+	def before_query_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_query events.
+		The before_query event is invoked before each query operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, query: str)
+		:param handler: new handler"""
+		self._core.io.before_query_handler = handler
+
+	def sync_from(self, source: 'Events') -> None:
+		"""Synchronises these Events with the source."""
+		self.before_query_handler = source.before_query_handler
+		self.before_write_handler = source.before_write_handler
+		self.io_events_include_data = source.io_events_include_data
+		self.on_read_handler = source.on_read_handler
+		self.on_write_handler = source.on_write_handler
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/CustomFiles/reliability.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/reliability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Class for R&S Mobile Radio Test instruments that use reliability indicators."""
+
+
 import time
 from typing import Callable
 
 from ..Internal import ArgLinkedEventArgs
 from ..Internal import Core
 
 codes_table = {
@@ -60,25 +63,25 @@
 		self.context = context
 
 
 class Reliability:
 	"""Reliability class that handles all the necessary tasks related to reliability indicator."""
 
 	def __init__(self, core: Core):
-		self._core = core
-		self._last_value = 0
-		self._last_context = ''
+		self._core: Core = core
+		self._last_value: int = 0
+		self._last_context: str = ''
 		self._last_timestamp = None
 		self._exception_on_error = False
 		# noinspection PyTypeChecker
 		self._on_update_handler: Callable = None
 		self._core.set_link_handler('Reliability', self._permanent_on_update_handler)
 
 	@property
-	def last_value(self):
+	def last_value(self) -> int:
 		"""Returns the last updated Reliability code."""
 		return self._last_value
 
 	@property
 	def last_context(self) -> str:
 		"""Returns the last updated Context of the reliability code - usually the SCPI query on which the instrument responded with the Reliability code."""
 		return self._last_context
@@ -94,36 +97,39 @@
 		if self._last_value in codes_table:
 			return codes_table[self._last_value]
 		else:
 			return f'Undefined reliability code {self._last_value}.'
 
 	@property
 	def exception_on_error(self) -> bool:
-		"""see the exception_on_error.setter."""
+		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
 		return self._exception_on_error
 
 	@exception_on_error.setter
 	def exception_on_error(self, value) -> None:
 		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
 		self._exception_on_error = value
 
 	def on_update_handler(self, handler: Callable) -> None:
 		"""Register the handler for on_update event.
 		This handler is invoked with each update of the reliability indicator.
 		Handler API: handler(event_args: ReliabilityEventArgs)"""
 		self._on_update_handler = handler
 
-	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs):
+	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs) -> None:
 		"""Permanent on_update handler. Takes care of updating all the 'last_xxx' values and calling a user-defined updated_handler."""
 		self._last_value = int(str(event_args.value))
 		self._last_context = event_args.context
 		self._last_timestamp = event_args.timestamp
-
 		if self._on_update_handler:
 			# Call the additional handler if registered
 			rel_events_args = ReliabilityEventArgs(self._last_timestamp, self._last_value, self.last_message, self._last_context)
 			self._on_update_handler(rel_events_args)
-
 		if self._exception_on_error and self._last_value != 0:
 			raise Exception(
 				f'Reliability indicator error. Time: {time.strftime("%H:%M:%S", time.localtime(self._last_timestamp))}, '
 				f'Context: {self._last_context}, Value {self._last_value}: {self.last_message}')
+
+	def sync_from(self, source: 'Reliability') -> None:
+		"""Synchronises this Reliability with the source."""
+		self.exception_on_error = source.exception_on_error
+		self.on_update_handler(source._on_update_handler)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Configure:
-	"""Configure commands group definition. 26 total commands, 1 Sub-groups, 0 group commands"""
+class CatalogCls:
+	"""Catalog commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("configure", core, parent)
+		self._cmd_group = CommandsGroup("catalog", core, parent)
 
 	@property
 	def uwbMeas(self):
-		"""uwbMeas commands group. 2 Sub-classes, 0 commands."""
+		"""uwbMeas commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_uwbMeas'):
-			from .Configure_.UwbMeas import UwbMeas
-			self._uwbMeas = UwbMeas(self._core, self._base)
+			from .UwbMeas import UwbMeasCls
+			self._uwbMeas = UwbMeasCls(self._core, self._cmd_group)
 		return self._uwbMeas
 
-	def clone(self) -> 'Configure':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'CatalogCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Configure(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CatalogCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UwbMeas:
-	"""UwbMeas commands group definition. 26 total commands, 2 Sub-groups, 0 group commands"""
+class UpperCls:
+	"""Upper commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uwbMeas", core, parent)
+		self._cmd_group = CommandsGroup("upper", core, parent)
 
 	@property
-	def multiEval(self):
-		"""multiEval commands group. 5 Sub-classes, 10 commands."""
-		if not hasattr(self, '_multiEval'):
-			from .UwbMeas_.MultiEval import MultiEval
-			self._multiEval = MultiEval(self._core, self._base)
-		return self._multiEval
+	def area(self):
+		"""area commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_area'):
+			from .Area import AreaCls
+			self._area = AreaCls(self._core, self._cmd_group)
+		return self._area
 
-	@property
-	def rfSettings(self):
-		"""rfSettings commands group. 0 Sub-classes, 5 commands."""
-		if not hasattr(self, '_rfSettings'):
-			from .UwbMeas_.RfSettings import RfSettings
-			self._rfSettings = RfSettings(self._core, self._base)
-		return self._rfSettings
-
-	def clone(self) -> 'UwbMeas':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'UpperCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UwbMeas(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UpperCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,123 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.Utilities import trim_str_response
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MultiEval:
-	"""MultiEval commands group definition. 21 total commands, 5 Sub-groups, 10 group commands"""
+class MultiEvalCls:
+	"""MultiEval commands group definition. 39 total commands, 8 Subgroups, 16 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("multiEval", core, parent)
+		self._cmd_group = CommandsGroup("multiEval", core, parent)
 
 	@property
-	def stsGap(self):
-		"""stsGap commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_stsGap'):
-			from .MultiEval_.StsGap import StsGap
-			self._stsGap = StsGap(self._core, self._base)
-		return self._stsGap
+	def phr(self):
+		"""phr commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_phr'):
+			from .Phr import PhrCls
+			self._phr = PhrCls(self._core, self._cmd_group)
+		return self._phr
+
+	@property
+	def psdu(self):
+		"""psdu commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_psdu'):
+			from .Psdu import PsduCls
+			self._psdu = PsduCls(self._core, self._cmd_group)
+		return self._psdu
 
 	@property
 	def spectrum(self):
-		"""spectrum commands group. 0 Sub-classes, 1 commands."""
+		"""spectrum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_spectrum'):
-			from .MultiEval_.Spectrum import Spectrum
-			self._spectrum = Spectrum(self._core, self._base)
+			from .Spectrum import SpectrumCls
+			self._spectrum = SpectrumCls(self._core, self._cmd_group)
 		return self._spectrum
 
 	@property
+	def ppdu(self):
+		"""ppdu commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ppdu'):
+			from .Ppdu import PpduCls
+			self._ppdu = PpduCls(self._core, self._cmd_group)
+		return self._ppdu
+
+	@property
 	def result(self):
-		"""result commands group. 0 Sub-classes, 3 commands."""
+		"""result commands group. 0 Sub-classes, 4 commands."""
 		if not hasattr(self, '_result'):
-			from .MultiEval_.Result import Result
-			self._result = Result(self._core, self._base)
+			from .Result import ResultCls
+			self._result = ResultCls(self._core, self._cmd_group)
 		return self._result
 
 	@property
 	def modulation(self):
 		"""modulation commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_modulation'):
-			from .MultiEval_.Modulation import Modulation
-			self._modulation = Modulation(self._core, self._base)
+			from .Modulation import ModulationCls
+			self._modulation = ModulationCls(self._core, self._cmd_group)
 		return self._modulation
 
 	@property
 	def tsMask(self):
 		"""tsMask commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_tsMask'):
-			from .MultiEval_.TsMask import TsMask
-			self._tsMask = TsMask(self._core, self._base)
+			from .TsMask import TsMaskCls
+			self._tsMask = TsMaskCls(self._core, self._cmd_group)
 		return self._tsMask
 
+	@property
+	def pmask(self):
+		"""pmask commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_pmask'):
+			from .Pmask import PmaskCls
+			self._pmask = PmaskCls(self._core, self._cmd_group)
+		return self._pmask
+
+	def get_mpr_frequency(self) -> str:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:MPRFrequency \n
+		Snippet: value: str = driver.configure.uwbMeas.multiEval.get_mpr_frequency() \n
+		Queries the mean pulse repetition frequency. \n
+			:return: mpr_frequency: No help available
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:MPRFrequency?')
+		return trim_str_response(response)
+
+	def get_prf_mode(self) -> str:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PRFMode \n
+		Snippet: value: str = driver.configure.uwbMeas.multiEval.get_prf_mode() \n
+		Queries the pulse repetition frequency mode. \n
+			:return: prf_mode: BPRF HPRF ---
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PRFMode?')
+		return trim_str_response(response)
+
+	# noinspection PyTypeChecker
+	def get_pmode(self) -> enums.PpduMode:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PMODe \n
+		Snippet: value: enums.PpduMode = driver.configure.uwbMeas.multiEval.get_pmode() \n
+		Selects the measurement mode. \n
+			:return: ppdu_mode: SPPDu: single PPDU packet analysis MPPDu: multi PPDU packet analysis
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PMODe?')
+		return Conversions.str_to_scalar_enum(response, enums.PpduMode)
+
+	def set_pmode(self, ppdu_mode: enums.PpduMode) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PMODe \n
+		Snippet: driver.configure.uwbMeas.multiEval.set_pmode(ppdu_mode = enums.PpduMode.MPPDu) \n
+		Selects the measurement mode. \n
+			:param ppdu_mode: SPPDu: single PPDU packet analysis MPPDu: multi PPDU packet analysis
+		"""
+		param = Conversions.enum_scalar_to_str(ppdu_mode, enums.PpduMode)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PMODe {param}')
+
 	# noinspection PyTypeChecker
 	def get_scondition(self) -> enums.StopCondition:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:SCONdition \n
 		Snippet: value: enums.StopCondition = driver.configure.uwbMeas.multiEval.get_scondition() \n
 		Qualifies whether the measurement is stopped after a failed limit check or continued. SLFail means that the measurement
 		is stopped and reaches the RDY state when one of the results exceeds the limits. \n
 			:return: stop_condition: NONE: Continue measurement irrespective of the limit check SLFail: Stop measurement on limit failure
@@ -73,37 +135,35 @@
 		param = Conversions.enum_scalar_to_str(stop_condition, enums.StopCondition)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:SCONdition {param}')
 
 	def get_timeout(self) -> float:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:TOUT \n
 		Snippet: value: float = driver.configure.uwbMeas.multiEval.get_timeout() \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
-		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
-		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
-		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
-		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
-		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
-		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
-		measurement timeout. \n
+		It is not started if the measurement is initiated manually. When the measurement has completed the first measurement
+		cycle (first single shot) , the statistical depth is reached and the timer is reset. If the first measurement cycle has
+		not been completed when the timer expires, the measurement is stopped. The measurement state changes to RDY.
+		The reliability indicator is set to 1, indicating that a measurement timeout occurred. Still running READ, FETCh or
+		CALCulate commands are completed, returning the available results. At least for some results, there are no values at all
+		or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite measurement timeout. \n
 			:return: tcd_timeout: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:TOUT?')
 		return Conversions.str_to_float(response)
 
 	def set_timeout(self, tcd_timeout: float) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:TOUT \n
 		Snippet: driver.configure.uwbMeas.multiEval.set_timeout(tcd_timeout = 1.0) \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
-		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
-		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
-		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
-		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
-		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
-		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
-		measurement timeout. \n
+		It is not started if the measurement is initiated manually. When the measurement has completed the first measurement
+		cycle (first single shot) , the statistical depth is reached and the timer is reset. If the first measurement cycle has
+		not been completed when the timer expires, the measurement is stopped. The measurement state changes to RDY.
+		The reliability indicator is set to 1, indicating that a measurement timeout occurred. Still running READ, FETCh or
+		CALCulate commands are completed, returning the available results. At least for some results, there are no values at all
+		or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite measurement timeout. \n
 			:param tcd_timeout: No help available
 		"""
 		param = Conversions.decimal_value_to_str(tcd_timeout)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:TOUT {param}')
 
 	def get_scount(self) -> int:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:SCOunt \n
@@ -184,25 +244,25 @@
 		param = Conversions.decimal_value_to_str(ppdu_sts_format)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PSFormat {param}')
 
 	def get_pp_length(self) -> int:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength \n
 		Snippet: value: int = driver.configure.uwbMeas.multiEval.get_pp_length() \n
 		Specifies the bit length of the PHR payload length field. This setting is only relevant in HPRF mode (RHML or RHMH set
-		viamethod RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.phrRate ) . \n
+		via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.phrRate ) . \n
 			:return: phr_payload_len: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength?')
 		return Conversions.str_to_int(response)
 
 	def set_pp_length(self, phr_payload_len: int) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength \n
 		Snippet: driver.configure.uwbMeas.multiEval.set_pp_length(phr_payload_len = 1) \n
 		Specifies the bit length of the PHR payload length field. This setting is only relevant in HPRF mode (RHML or RHMH set
-		viamethod RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.phrRate ) . \n
+		via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.phrRate ) . \n
 			:param phr_payload_len: No help available
 		"""
 		param = Conversions.decimal_value_to_str(phr_payload_len)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength {param}')
 
 	def get_st_segments(self) -> int:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSegments \n
@@ -237,33 +297,89 @@
 		Snippet: driver.configure.uwbMeas.multiEval.set_sts_length(sts_segment_len = enums.StsSegmentLen.L128) \n
 		Specifies the length of the STS segment in units of 512 chips. \n
 			:param sts_segment_len: No help available
 		"""
 		param = Conversions.enum_scalar_to_str(sts_segment_len, enums.StsSegmentLen)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:STSLength {param}')
 
+	def get_sts_gap(self) -> int:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap \n
+		Snippet: value: int = driver.configure.uwbMeas.multiEval.get_sts_gap() \n
+		Specifies additional gaps between the payload and the STS in unit of 4 chips. This setting is only relevant for PPDU STS
+		packet structure configuration two set via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.psFormat) . \n
+			:return: sts_gap: No help available
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap?')
+		return Conversions.str_to_int(response)
+
+	def set_sts_gap(self, sts_gap: int) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap \n
+		Snippet: driver.configure.uwbMeas.multiEval.set_sts_gap(sts_gap = 1) \n
+		Specifies additional gaps between the payload and the STS in unit of 4 chips. This setting is only relevant for PPDU STS
+		packet structure configuration two set via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.psFormat) . \n
+			:param sts_gap: No help available
+		"""
+		param = Conversions.decimal_value_to_str(sts_gap)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap {param}')
+
 	# noinspection PyTypeChecker
 	def get_phr_rate(self) -> enums.PhrDataRate:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate \n
 		Snippet: value: enums.PhrDataRate = driver.configure.uwbMeas.multiEval.get_phr_rate() \n
 		Specifies the data rate of the PHY header (PHR) . \n
-			:return: phr_data_rate: DRMD: 110 kb/s or 850 kb/s (DRMDR) DRLP: 850 kb/s (DRBM_LP) DRHP: 6.8 Mb/s (DRBM_HP) RHML: 3.9 Mb/s or 7.8 Mb/s (DRHM_LR) RHMH: 15.6 Mb/s or 31.2 Mb/s (DRHM_HR)
+			:return: phr_data_rate: DRMD: 110 kb/s or 850 kb/s (DRMDR) DRLP: 850 kb/s (DRBM_LP) DRHP: 6.8 Mb/s (DRBM_HP) RHML: 3.9 Mb/s or 7.8 Mb/s (DRHM_LR) RHMH: 15.6 Mb/s or 31.2 Mb/s (DRHM_HR) SYNC: PPDU contains only SYNC field (SYNC_ONLY)
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate?')
 		return Conversions.str_to_scalar_enum(response, enums.PhrDataRate)
 
 	def set_phr_rate(self, phr_data_rate: enums.PhrDataRate) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate \n
 		Snippet: driver.configure.uwbMeas.multiEval.set_phr_rate(phr_data_rate = enums.PhrDataRate.DRHP) \n
 		Specifies the data rate of the PHY header (PHR) . \n
-			:param phr_data_rate: DRMD: 110 kb/s or 850 kb/s (DRMDR) DRLP: 850 kb/s (DRBM_LP) DRHP: 6.8 Mb/s (DRBM_HP) RHML: 3.9 Mb/s or 7.8 Mb/s (DRHM_LR) RHMH: 15.6 Mb/s or 31.2 Mb/s (DRHM_HR)
+			:param phr_data_rate: DRMD: 110 kb/s or 850 kb/s (DRMDR) DRLP: 850 kb/s (DRBM_LP) DRHP: 6.8 Mb/s (DRBM_HP) RHML: 3.9 Mb/s or 7.8 Mb/s (DRHM_LR) RHMH: 15.6 Mb/s or 31.2 Mb/s (DRHM_HR) SYNC: PPDU contains only SYNC field (SYNC_ONLY)
 		"""
 		param = Conversions.enum_scalar_to_str(phr_data_rate, enums.PhrDataRate)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate {param}')
 
-	def clone(self) -> 'MultiEval':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def get_cap_length(self) -> float:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:CAPLength \n
+		Snippet: value: float = driver.configure.uwbMeas.multiEval.get_cap_length() \n
+		Defines the length to capture the signal. \n
+			:return: capture_length: No help available
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:CAPLength?')
+		return Conversions.str_to_float(response)
+
+	def set_cap_length(self, capture_length: float) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:CAPLength \n
+		Snippet: driver.configure.uwbMeas.multiEval.set_cap_length(capture_length = 1.0) \n
+		Defines the length to capture the signal. \n
+			:param capture_length: No help available
+		"""
+		param = Conversions.decimal_value_to_str(capture_length)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:CAPLength {param}')
+
+	def get_eoffset(self) -> float:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:EOFFset \n
+		Snippet: value: float = driver.configure.uwbMeas.multiEval.get_eoffset() \n
+		Specifies which time period is excluded from the measurement at the beginning of the capture length. \n
+			:return: eval_offset: No help available
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:EOFFset?')
+		return Conversions.str_to_float(response)
+
+	def set_eoffset(self, eval_offset: float) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:EOFFset \n
+		Snippet: driver.configure.uwbMeas.multiEval.set_eoffset(eval_offset = 1.0) \n
+		Specifies which time period is excluded from the measurement at the beginning of the capture length. \n
+			:param eval_offset: No help available
+		"""
+		param = Conversions.decimal_value_to_str(eval_offset)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:EOFFset {param}')
+
+	def clone(self) -> 'MultiEvalCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = MultiEval(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MultiEvalCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Modulation:
-	"""Modulation commands group definition. 5 total commands, 1 Sub-groups, 0 group commands"""
+class ModulationCls:
+	"""Modulation commands group definition. 10 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("modulation", core, parent)
+		self._cmd_group = CommandsGroup("modulation", core, parent)
 
 	@property
 	def limit(self):
-		"""limit commands group. 0 Sub-classes, 5 commands."""
+		"""limit commands group. 10 Sub-classes, 0 commands."""
 		if not hasattr(self, '_limit'):
-			from .Modulation_.Limit import Limit
-			self._limit = Limit(self._core, self._base)
+			from .Limit import LimitCls
+			self._limit = LimitCls(self._core, self._cmd_group)
 		return self._limit
 
-	def clone(self) -> 'Modulation':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'ModulationCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Modulation(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ModulationCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Result.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,84 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Result:
-	"""Result commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ResultCls:
+	"""Result commands group definition. 4 total commands, 0 Subgroups, 4 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("result", core, parent)
+		self._cmd_group = CommandsGroup("result", core, parent)
 
 	def get_ts_mask(self) -> bool:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask \n
 		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_ts_mask() \n
-		Enables or disables the evaluation of results in the multi-evaluation measurement. \n
+		Enables or disables the evaluation of spectrum emission mask results. \n
 			:return: enable: OFF: Do not evaluate results ON: Evaluate results
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask?')
 		return Conversions.str_to_bool(response)
 
 	def set_ts_mask(self, enable: bool) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask \n
 		Snippet: driver.configure.uwbMeas.multiEval.result.set_ts_mask(enable = False) \n
-		Enables or disables the evaluation of results in the multi-evaluation measurement. \n
+		Enables or disables the evaluation of spectrum emission mask results. \n
 			:param enable: OFF: Do not evaluate results ON: Evaluate results
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask {param}')
 
 	def get_power_vs_time(self) -> bool:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime \n
 		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_power_vs_time() \n
-		Enables or disables the evaluation of results in the multi-evaluation measurement. \n
+		Enables or disables the evaluation of power results. \n
 			:return: enable: OFF: Do not evaluate results ON: Evaluate results
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime?')
 		return Conversions.str_to_bool(response)
 
 	def set_power_vs_time(self, enable: bool) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime \n
 		Snippet: driver.configure.uwbMeas.multiEval.result.set_power_vs_time(enable = False) \n
-		Enables or disables the evaluation of results in the multi-evaluation measurement. \n
+		Enables or disables the evaluation of power results. \n
 			:param enable: OFF: Do not evaluate results ON: Evaluate results
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime {param}')
 
 	def get_emodulation(self) -> bool:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation \n
 		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_emodulation() \n
-		Enables or disables the evaluation of results in the multi-evaluation measurement. \n
+		Enables or disables the evaluation of modulation and jitter results. \n
 			:return: enable: OFF: Do not evaluate results ON: Evaluate results
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation?')
 		return Conversions.str_to_bool(response)
 
 	def set_emodulation(self, enable: bool) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation \n
 		Snippet: driver.configure.uwbMeas.multiEval.result.set_emodulation(enable = False) \n
-		Enables or disables the evaluation of results in the multi-evaluation measurement. \n
+		Enables or disables the evaluation of modulation and jitter results. \n
 			:param enable: OFF: Do not evaluate results ON: Evaluate results
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation {param}')
+
+	def get_ddecoding(self) -> bool:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding \n
+		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_ddecoding() \n
+		Enables or disables the evaluation of the PPDU payload contents. \n
+			:return: enable: OFF: Do not evaluate results ON: Evaluate results
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding?')
+		return Conversions.str_to_bool(response)
+
+	def set_ddecoding(self, enable: bool) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding \n
+		Snippet: driver.configure.uwbMeas.multiEval.result.set_ddecoding(enable = False) \n
+		Enables or disables the evaluation of the PPDU payload contents. \n
+			:param enable: OFF: Do not evaluate results ON: Evaluate results
+		"""
+		param = Conversions.bool_to_str(enable)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding {param}')
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/StsGap.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Ppdu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StsGap:
-	"""StsGap commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class PpduCls:
+	"""Ppdu commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("stsGap", core, parent)
+		self._cmd_group = CommandsGroup("ppdu", core, parent)
 
-	def get_enable(self) -> bool:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap:ENABle \n
-		Snippet: value: bool = driver.configure.uwbMeas.multiEval.stsGap.get_enable() \n
+	def get_number(self) -> int:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PPDU:NUMBer \n
+		Snippet: value: int = driver.configure.uwbMeas.multiEval.ppdu.get_number() \n
 		No command help available \n
-			:return: sts_gap: No help available
+			:return: ppdu_number: No help available
 		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap:ENABle?')
-		return Conversions.str_to_bool(response)
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PPDU:NUMBer?')
+		return Conversions.str_to_int(response)
 
-	def set_enable(self, sts_gap: bool) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap:ENABle \n
-		Snippet: driver.configure.uwbMeas.multiEval.stsGap.set_enable(sts_gap = False) \n
+	def set_number(self, ppdu_number: int) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PPDU:NUMBer \n
+		Snippet: driver.configure.uwbMeas.multiEval.ppdu.set_number(ppdu_number = 1) \n
 		No command help available \n
-			:param sts_gap: No help available
+			:param ppdu_number: No help available
 		"""
-		param = Conversions.bool_to_str(sts_gap)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap:ENABle {param}')
+		param = Conversions.decimal_value_to_str(ppdu_number)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PPDU:NUMBer {param}')
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class TsMask:
-	"""TsMask commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class MarginCls:
+	"""Margin commands group definition. 5 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("tsMask", core, parent)
+		self._cmd_group = CommandsGroup("margin", core, parent)
 
 	@property
-	def limit(self):
-		"""limit commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_limit'):
-			from .TsMask_.Limit import Limit
-			self._limit = Limit(self._core, self._base)
-		return self._limit
+	def prMonotonic(self):
+		"""prMonotonic commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_prMonotonic'):
+			from .PrMonotonic import PrMonotonicCls
+			self._prMonotonic = PrMonotonicCls(self._core, self._cmd_group)
+		return self._prMonotonic
 
-	def clone(self) -> 'TsMask':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def area(self):
+		"""area commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_area'):
+			from .Area import AreaCls
+			self._area = AreaCls(self._core, self._cmd_group)
+		return self._area
+
+	def clone(self) -> 'MarginCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = TsMask(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MarginCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Limit:
-	"""Limit commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class PsduCls:
+	"""Psdu commands group definition. 4 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("limit", core, parent)
+		self._cmd_group = CommandsGroup("psdu", core, parent)
 
 	@property
-	def area(self):
-		"""area commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_area'):
-			from .Limit_.Area import Area
-			self._area = Area(self._core, self._base)
-		return self._area
+	def length(self):
+		"""length commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_length'):
+			from .Length import LengthCls
+			self._length = LengthCls(self._core, self._cmd_group)
+		return self._length
 
-	def clone(self) -> 'Limit':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def crc(self):
+		"""crc commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_crc'):
+			from .Crc import CrcCls
+			self._crc = CrcCls(self._core, self._cmd_group)
+		return self._crc
+
+	def clone(self) -> 'PsduCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Limit(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PsduCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit_/Area.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 from .......Internal.Core import Core
 from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal.Types import DataType
 from .......Internal.StructBase import StructBase
 from .......Internal.ArgStruct import ArgStruct
+from .......Internal.ArgSingleList import ArgSingleList
+from .......Internal.ArgSingle import ArgSingle
 from .......Internal.RepeatedCapability import RepeatedCapability
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Area:
-	"""Area commands group definition. 1 total commands, 0 Sub-groups, 1 group commands
+class AreaCls:
+	"""Area commands group definition. 1 total commands, 0 Subgroups, 1 group commands
 	Repeated Capability: Area, default value after init: Area.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("area", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_area_get', 'repcap_area_set', repcap.Area.Nr1)
+		self._cmd_group = CommandsGroup("area", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_area_get', 'repcap_area_set', repcap.Area.Nr1)
 
-	def repcap_area_set(self, enum_value: repcap.Area) -> None:
+	def repcap_area_set(self, area: repcap.Area) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Area.Default
 		Default value after init: Area.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(area)
 
 	def repcap_area_get(self) -> repcap.Area:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
+
+	def set(self, enable: bool, area_limit: float = None, area=repcap.Area.Default) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:TSMask:LIMit:AREA<nr> \n
+		Snippet: driver.configure.uwbMeas.multiEval.tsMask.limit.area.set(enable = False, area_limit = 1.0, area = repcap.Area.Default) \n
+		Activates and defines an upper limit for the two areas of the spectral mask. \n
+			:param enable: No help available
+			:param area_limit: No help available
+			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('area_limit', area_limit, DataType.Float, None, is_optional=True))
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:TSMask:LIMit:AREA{area_cmd_val} {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class AreaStruct(StructBase):
-		"""Structure for setting input parameters. Contains optional setting parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- Enable: bool: No parameter help available
-			- Area: float: No parameter help available"""
+			- Area_Limit: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
-			ArgStruct.scalar_float('Area')]
+			ArgStruct.scalar_float('Area_Limit')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Enable: bool = None
-			self.Area: float = None
-
-	def set(self, structure: AreaStruct, area=repcap.Area.Default) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:TSMask:LIMit:AREA<nr> \n
-		Snippet: driver.configure.uwbMeas.multiEval.tsMask.limit.area.set(value = [PROPERTY_STRUCT_NAME](), area = repcap.Area.Default) \n
-		Activates and defines an upper limit for the two areas of the spectral mask. \n
-			:param structure: for set value, see the help for AreaStruct structure arguments.
-			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')"""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		self._core.io.write_struct(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:TSMask:LIMit:AREA{area_cmd_val}', structure)
+			self.Area_Limit: float = None
 
 	def get(self, area=repcap.Area.Default) -> AreaStruct:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:TSMask:LIMit:AREA<nr> \n
 		Snippet: value: AreaStruct = driver.configure.uwbMeas.multiEval.tsMask.limit.area.get(area = repcap.Area.Default) \n
 		Activates and defines an upper limit for the two areas of the spectral mask. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:return: structure: for return value, see the help for AreaStruct structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		return self._core.io.query_struct(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:TSMask:LIMit:AREA{area_cmd_val}?', self.__class__.AreaStruct())
 
-	def clone(self) -> 'Area':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'AreaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Area(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = AreaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/RfSettings.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RfSettings:
-	"""RfSettings commands group definition. 5 total commands, 0 Sub-groups, 5 group commands"""
+class RfSettingsCls:
+	"""RfSettings commands group definition. 6 total commands, 1 Subgroups, 4 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rfSettings", core, parent)
+		self._cmd_group = CommandsGroup("rfSettings", core, parent)
 
-	def get_frequency(self) -> float:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency \n
-		Snippet: value: float = driver.configure.uwbMeas.rfSettings.get_frequency() \n
-		Selects the center frequency of the measured carrier. For the supported frequency range, see 'Frequency Ranges'. \n
-			:return: analyzer_freq: No help available
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency?')
-		return Conversions.str_to_float(response)
-
-	def set_frequency(self, analyzer_freq: float) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency \n
-		Snippet: driver.configure.uwbMeas.rfSettings.set_frequency(analyzer_freq = 1.0) \n
-		Selects the center frequency of the measured carrier. For the supported frequency range, see 'Frequency Ranges'. \n
-			:param analyzer_freq: No help available
-		"""
-		param = Conversions.decimal_value_to_str(analyzer_freq)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency {param}')
+	@property
+	def frequency(self):
+		"""frequency commands group. 1 Sub-classes, 1 commands."""
+		if not hasattr(self, '_frequency'):
+			from .Frequency import FrequencyCls
+			self._frequency = FrequencyCls(self._core, self._cmd_group)
+		return self._frequency
 
 	def get_channel(self) -> int:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:CHANnel \n
 		Snippet: value: int = driver.configure.uwbMeas.rfSettings.get_channel() \n
 		Selects the channel number. \n
 			:return: analyzer_chan: No help available
 		"""
@@ -100,7 +90,15 @@
 		Sets the margin that the measurement adds to the expected nominal power to determine the reference power. The reference
 		power minus the external input attenuation must be within the power range of the selected input connector. Refer to the
 		data sheet. \n
 			:param user_margin: No help available
 		"""
 		param = Conversions.decimal_value_to_str(user_margin)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:RFSettings:UMARgin {param}')
+
+	def clone(self) -> 'RfSettingsCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
+		Also copies all the existing default Repeated Capabilities setting,
+		which you can change independently without affecting the original group"""
+		new_group = RfSettingsCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
+		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Route:
-	"""Route commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class TriggerCls:
+	"""Trigger commands group definition. 7 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("route", core, parent)
+		self._cmd_group = CommandsGroup("trigger", core, parent)
 
 	@property
 	def uwbMeas(self):
 		"""uwbMeas commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_uwbMeas'):
-			from .Route_.UwbMeas import UwbMeas
-			self._uwbMeas = UwbMeas(self._core, self._base)
+			from .UwbMeas import UwbMeasCls
+			self._uwbMeas = UwbMeasCls(self._core, self._cmd_group)
 		return self._uwbMeas
 
-	def clone(self) -> 'Route':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'TriggerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Route(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = TriggerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/UwbMeas.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UwbMeas:
-	"""UwbMeas commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class UwbMeasCls:
+	"""UwbMeas commands group definition. 465 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uwbMeas", core, parent)
+		self._cmd_group = CommandsGroup("uwbMeas", core, parent)
 
 	@property
-	def rfSettings(self):
-		"""rfSettings commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_rfSettings'):
-			from .UwbMeas_.RfSettings import RfSettings
-			self._rfSettings = RfSettings(self._core, self._base)
-		return self._rfSettings
+	def multiEval(self):
+		"""multiEval commands group. 8 Sub-classes, 3 commands."""
+		if not hasattr(self, '_multiEval'):
+			from .MultiEval import MultiEvalCls
+			self._multiEval = MultiEvalCls(self._core, self._cmd_group)
+		return self._multiEval
 
-	def clone(self) -> 'UwbMeas':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'UwbMeasCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UwbMeas(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UwbMeasCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Route_/UwbMeas_/RfSettings.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RfSettings:
-	"""RfSettings commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class RfSettingsCls:
+	"""RfSettings commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rfSettings", core, parent)
+		self._cmd_group = CommandsGroup("rfSettings", core, parent)
 
 	# noinspection PyTypeChecker
 	def get_connector(self) -> enums.Connector:
 		"""SCPI: ROUTe:UWB:MEASurement<Instance>:RFSettings:CONNector \n
 		Snippet: value: enums.Connector = driver.route.uwbMeas.rfSettings.get_connector() \n
 		No command help available \n
 			:return: connector: No help available
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Trigger:
-	"""Trigger commands group definition. 7 total commands, 1 Sub-groups, 0 group commands"""
+class RouteCls:
+	"""Route commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("trigger", core, parent)
+		self._cmd_group = CommandsGroup("route", core, parent)
 
 	@property
 	def uwbMeas(self):
-		"""uwbMeas commands group. 1 Sub-classes, 0 commands."""
+		"""uwbMeas commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_uwbMeas'):
-			from .Trigger_.UwbMeas import UwbMeas
-			self._uwbMeas = UwbMeas(self._core, self._base)
+			from .UwbMeas import UwbMeasCls
+			self._uwbMeas = UwbMeasCls(self._core, self._cmd_group)
 		return self._uwbMeas
 
-	def clone(self) -> 'Trigger':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'RouteCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Trigger(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = RouteCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UwbMeas:
-	"""UwbMeas commands group definition. 7 total commands, 1 Sub-groups, 0 group commands"""
+class UwbMeasCls:
+	"""UwbMeas commands group definition. 45 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uwbMeas", core, parent)
+		self._cmd_group = CommandsGroup("uwbMeas", core, parent)
 
 	@property
 	def multiEval(self):
-		"""multiEval commands group. 1 Sub-classes, 6 commands."""
+		"""multiEval commands group. 8 Sub-classes, 16 commands."""
 		if not hasattr(self, '_multiEval'):
-			from .UwbMeas_.MultiEval import MultiEval
-			self._multiEval = MultiEval(self._core, self._base)
+			from .MultiEval import MultiEvalCls
+			self._multiEval = MultiEvalCls(self._core, self._cmd_group)
 		return self._multiEval
 
-	def clone(self) -> 'UwbMeas':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def rfSettings(self):
+		"""rfSettings commands group. 1 Sub-classes, 4 commands."""
+		if not hasattr(self, '_rfSettings'):
+			from .RfSettings import RfSettingsCls
+			self._rfSettings = RfSettingsCls(self._core, self._cmd_group)
+		return self._rfSettings
+
+	def clone(self) -> 'UwbMeasCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UwbMeas(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UwbMeasCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from ....Internal.Utilities import trim_str_response
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.Utilities import trim_str_response
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MultiEval:
-	"""MultiEval commands group definition. 7 total commands, 1 Sub-groups, 6 group commands"""
+class MultiEvalCls:
+	"""MultiEval commands group definition. 7 total commands, 1 Subgroups, 6 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("multiEval", core, parent)
+		self._cmd_group = CommandsGroup("multiEval", core, parent)
 
 	@property
 	def catalog(self):
 		"""catalog commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_catalog'):
-			from .MultiEval_.Catalog import Catalog
-			self._catalog = Catalog(self._core, self._base)
+			from .Catalog import CatalogCls
+			self._catalog = CatalogCls(self._core, self._cmd_group)
 		return self._catalog
 
 	def get_source(self) -> str:
 		"""SCPI: TRIGger:UWB:MEASurement<Instance>:MEValuation:SOURce \n
 		Snippet: value: str = driver.trigger.uwbMeas.multiEval.get_source() \n
 		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
 		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
@@ -64,25 +64,25 @@
 		self._core.io.write(f'TRIGger:UWB:MEASurement<Instance>:MEValuation:THReshold {param}')
 
 	def get_timeout(self) -> float or bool:
 		"""SCPI: TRIGger:UWB:MEASurement<Instance>:MEValuation:TOUT \n
 		Snippet: value: float or bool = driver.trigger.uwbMeas.multiEval.get_timeout() \n
 		Selects the maximum time that the measurement waits for a trigger event before it stops in remote control mode or
 		indicates a trigger timeout in manual operation mode. This setting has no influence on Free Run measurements. \n
-			:return: timeout: No help available
+			:return: timeout: (float or boolean) No help available
 		"""
 		response = self._core.io.query_str('TRIGger:UWB:MEASurement<Instance>:MEValuation:TOUT?')
 		return Conversions.str_to_float_or_bool(response)
 
 	def set_timeout(self, timeout: float or bool) -> None:
 		"""SCPI: TRIGger:UWB:MEASurement<Instance>:MEValuation:TOUT \n
 		Snippet: driver.trigger.uwbMeas.multiEval.set_timeout(timeout = 1.0) \n
 		Selects the maximum time that the measurement waits for a trigger event before it stops in remote control mode or
 		indicates a trigger timeout in manual operation mode. This setting has no influence on Free Run measurements. \n
-			:param timeout: No help available
+			:param timeout: (float or boolean) No help available
 		"""
 		param = Conversions.decimal_or_bool_value_to_str(timeout)
 		self._core.io.write(f'TRIGger:UWB:MEASurement<Instance>:MEValuation:TOUT {param}')
 
 	def get_mgap(self) -> float:
 		"""SCPI: TRIGger:UWB:MEASurement<Instance>:MEValuation:MGAP \n
 		Snippet: value: float = driver.trigger.uwbMeas.multiEval.get_mgap() \n
@@ -138,14 +138,14 @@
 		Defines a time delaying the start of the measurement relative to the trigger event. This setting has no influence on free
 		run measurements. \n
 			:param delay: No help available
 		"""
 		param = Conversions.decimal_value_to_str(delay)
 		self._core.io.write(f'TRIGger:UWB:MEASurement<Instance>:MEValuation:DELay {param}')
 
-	def clone(self) -> 'MultiEval':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MultiEvalCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = MultiEval(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MultiEvalCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval_/Catalog.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/Catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Catalog:
-	"""Catalog commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class CatalogCls:
+	"""Catalog commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("catalog", core, parent)
+		self._cmd_group = CommandsGroup("catalog", core, parent)
 
 	def get_source(self) -> List[str]:
 		"""SCPI: TRIGger:UWB:MEASurement<Instance>:MEValuation:CATalog:SOURce \n
 		Snippet: value: List[str] = driver.trigger.uwbMeas.multiEval.catalog.get_source() \n
 		Lists all trigger source values that can be set using method RsCMPX_UwbMeas.Trigger.UwbMeas.MultiEval.source. \n
 			:return: trigger_sources: Comma-separated list of all supported values, one string per value.
 		"""
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UwbMeas:
-	"""UwbMeas commands group definition. 265 total commands, 1 Sub-groups, 0 group commands"""
+class UwbMeasCls:
+	"""UwbMeas commands group definition. 7 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uwbMeas", core, parent)
+		self._cmd_group = CommandsGroup("uwbMeas", core, parent)
 
 	@property
 	def multiEval(self):
-		"""multiEval commands group. 6 Sub-classes, 3 commands."""
+		"""multiEval commands group. 1 Sub-classes, 6 commands."""
 		if not hasattr(self, '_multiEval'):
-			from .UwbMeas_.MultiEval import MultiEval
-			self._multiEval = MultiEval(self._core, self._base)
+			from .MultiEval import MultiEvalCls
+			self._multiEval = MultiEvalCls(self._core, self._cmd_group)
 		return self._multiEval
 
-	def clone(self) -> 'UwbMeas':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'UwbMeasCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UwbMeas(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UwbMeasCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,116 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MultiEval:
-	"""MultiEval commands group definition. 265 total commands, 6 Sub-groups, 3 group commands"""
+class MultiEvalCls:
+	"""MultiEval commands group definition. 465 total commands, 8 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("multiEval", core, parent)
+		self._cmd_group = CommandsGroup("multiEval", core, parent)
 
 	@property
 	def state(self):
 		"""state commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_state'):
-			from .MultiEval_.State import State
-			self._state = State(self._core, self._base)
+			from .State import StateCls
+			self._state = StateCls(self._core, self._cmd_group)
 		return self._state
 
 	@property
+	def ddecoding(self):
+		"""ddecoding commands group. 3 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ddecoding'):
+			from .Ddecoding import DdecodingCls
+			self._ddecoding = DdecodingCls(self._core, self._cmd_group)
+		return self._ddecoding
+
+	@property
 	def tsMask(self):
-		"""tsMask commands group. 1 Sub-classes, 0 commands."""
+		"""tsMask commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_tsMask'):
-			from .MultiEval_.TsMask import TsMask
-			self._tsMask = TsMask(self._core, self._base)
+			from .TsMask import TsMaskCls
+			self._tsMask = TsMaskCls(self._core, self._cmd_group)
 		return self._tsMask
 
 	@property
 	def modulation(self):
-		"""modulation commands group. 17 Sub-classes, 0 commands."""
+		"""modulation commands group. 27 Sub-classes, 0 commands."""
 		if not hasattr(self, '_modulation'):
-			from .MultiEval_.Modulation import Modulation
-			self._modulation = Modulation(self._core, self._base)
+			from .Modulation import ModulationCls
+			self._modulation = ModulationCls(self._core, self._cmd_group)
 		return self._modulation
 
 	@property
 	def power(self):
-		"""power commands group. 10 Sub-classes, 0 commands."""
+		"""power commands group. 11 Sub-classes, 0 commands."""
 		if not hasattr(self, '_power'):
-			from .MultiEval_.Power import Power
-			self._power = Power(self._core, self._base)
+			from .Power import PowerCls
+			self._power = PowerCls(self._core, self._cmd_group)
 		return self._power
 
 	@property
 	def sinfo(self):
-		"""sinfo commands group. 7 Sub-classes, 2 commands."""
+		"""sinfo commands group. 14 Sub-classes, 2 commands."""
 		if not hasattr(self, '_sinfo'):
-			from .MultiEval_.Sinfo import Sinfo
-			self._sinfo = Sinfo(self._core, self._base)
+			from .Sinfo import SinfoCls
+			self._sinfo = SinfoCls(self._core, self._cmd_group)
 		return self._sinfo
 
 	@property
+	def pmask(self):
+		"""pmask commands group. 4 Sub-classes, 0 commands."""
+		if not hasattr(self, '_pmask'):
+			from .Pmask import PmaskCls
+			self._pmask = PmaskCls(self._core, self._cmd_group)
+		return self._pmask
+
+	@property
 	def trace(self):
-		"""trace commands group. 7 Sub-classes, 0 commands."""
+		"""trace commands group. 10 Sub-classes, 0 commands."""
 		if not hasattr(self, '_trace'):
-			from .MultiEval_.Trace import Trace
-			self._trace = Trace(self._core, self._base)
+			from .Trace import TraceCls
+			self._trace = TraceCls(self._core, self._cmd_group)
 		return self._trace
 
-	def initiate(self) -> None:
+	def initiate(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:UWB:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.uwbMeas.multiEval.initiate() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
-		"""
-		self._core.io.write(f'INITiate:UWB:MEASurement<Instance>:MEValuation')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'INITiate:UWB:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
-	def initiate_with_opc(self) -> None:
-		"""SCPI: INITiate:UWB:MEASurement<Instance>:MEValuation \n
-		Snippet: driver.uwbMeas.multiEval.initiate_with_opc() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
-			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
-			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
-			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
-		Use FETCh...STATe? to query the current measurement state. \n
-		Same as initiate, but waits for the operation to complete before continuing further. Use the RsCMPX_UwbMeas.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'INITiate:UWB:MEASurement<Instance>:MEValuation')
-
-	def stop(self) -> None:
+	def stop(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:UWB:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.uwbMeas.multiEval.stop() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
-		"""
-		self._core.io.write(f'STOP:UWB:MEASurement<Instance>:MEValuation')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'STOP:UWB:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
-	def stop_with_opc(self) -> None:
-		"""SCPI: STOP:UWB:MEASurement<Instance>:MEValuation \n
-		Snippet: driver.uwbMeas.multiEval.stop_with_opc() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
-			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
-			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
-			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
-		Use FETCh...STATe? to query the current measurement state. \n
-		Same as stop, but waits for the operation to complete before continuing further. Use the RsCMPX_UwbMeas.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'STOP:UWB:MEASurement<Instance>:MEValuation')
-
-	def abort(self) -> None:
+	def abort(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:UWB:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.uwbMeas.multiEval.abort() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
-		"""
-		self._core.io.write(f'ABORt:UWB:MEASurement<Instance>:MEValuation')
-
-	def abort_with_opc(self) -> None:
-		"""SCPI: ABORt:UWB:MEASurement<Instance>:MEValuation \n
-		Snippet: driver.uwbMeas.multiEval.abort_with_opc() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
-			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
-			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
-			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
-		Use FETCh...STATe? to query the current measurement state. \n
-		Same as abort, but waits for the operation to complete before continuing further. Use the RsCMPX_UwbMeas.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'ABORt:UWB:MEASurement<Instance>:MEValuation')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'ABORt:UWB:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
-	def clone(self) -> 'MultiEval':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MultiEvalCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = MultiEval(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MultiEvalCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Average.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,73 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from ..... import enums
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
+			- Reliability: int: 'Reliability indicator'
 			- Freq_Offset_Hz: float: No parameter help available
 			- Freq_Offset: float: No parameter help available
 			- Chip_Clock_Error: float: No parameter help available
 			- Pulse_Nsme: float: No parameter help available
 			- Sym_Mod_Accuracy: float: No parameter help available
 			- Side_Lobe_Peak: float: No parameter help available
 			- Pulse_Ml_Width: float: No parameter help available
-			- Sym_Time_Jitter: float: RMS time jitter value averaged over all the detected preamble symbols
-			- Sym_Phase_Jitter: float: RMS phase jitter value averaged over all the detected preamble symbols
+			- Sym_Time_Jitter: float: No parameter help available
+			- Sym_Phase_Jitter: float: No parameter help available
 			- Chip_Time_Jitter: float: No parameter help available
 			- Chip_Phase_Jitter: float: No parameter help available
 			- Symbol_Evm: float: No parameter help available
-			- Chip_Evm: float: No parameter help available"""
+			- Chip_Evm: float: No parameter help available
+			- Rmarker: float: RMARKER time
+			- Shr_Nrmse: float: NRMSE for SHR
+			- Phr_Nrmse: float: NRMSE for PHR
+			- Psdu_Nrmse: float: NRMSE for PSDU
+			- Sts_Nrmse: float: NRMSE for STS
+			- Sync_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Sfd_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Sts_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Iq_Offset: float: I/Q offset"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Freq_Offset_Hz'),
 			ArgStruct.scalar_float('Freq_Offset'),
 			ArgStruct.scalar_float('Chip_Clock_Error'),
 			ArgStruct.scalar_float('Pulse_Nsme'),
 			ArgStruct.scalar_float('Sym_Mod_Accuracy'),
 			ArgStruct.scalar_float('Side_Lobe_Peak'),
 			ArgStruct.scalar_float('Pulse_Ml_Width'),
 			ArgStruct.scalar_float('Sym_Time_Jitter'),
 			ArgStruct.scalar_float('Sym_Phase_Jitter'),
 			ArgStruct.scalar_float('Chip_Time_Jitter'),
 			ArgStruct.scalar_float('Chip_Phase_Jitter'),
 			ArgStruct.scalar_float('Symbol_Evm'),
-			ArgStruct.scalar_float('Chip_Evm')]
+			ArgStruct.scalar_float('Chip_Evm'),
+			ArgStruct.scalar_float('Rmarker'),
+			ArgStruct.scalar_float('Shr_Nrmse'),
+			ArgStruct.scalar_float('Phr_Nrmse'),
+			ArgStruct.scalar_float('Psdu_Nrmse'),
+			ArgStruct.scalar_float('Sts_Nrmse'),
+			ArgStruct.scalar_enum('Sync_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_enum('Sfd_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_enum('Sts_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_float('Iq_Offset')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Freq_Offset_Hz: float = None
 			self.Freq_Offset: float = None
 			self.Chip_Clock_Error: float = None
@@ -57,23 +77,34 @@
 			self.Pulse_Ml_Width: float = None
 			self.Sym_Time_Jitter: float = None
 			self.Sym_Phase_Jitter: float = None
 			self.Chip_Time_Jitter: float = None
 			self.Chip_Phase_Jitter: float = None
 			self.Symbol_Evm: float = None
 			self.Chip_Evm: float = None
-
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.average.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+			self.Rmarker: float = None
+			self.Shr_Nrmse: float = None
+			self.Phr_Nrmse: float = None
+			self.Psdu_Nrmse: float = None
+			self.Sts_Nrmse: float = None
+			self.Sync_Pulse_Loc_Pol: enums.Result = None
+			self.Sfd_Pulse_Loc_Pol: enums.Result = None
+			self.Sts_Pulse_Loc_Pol: enums.Result = None
+			self.Iq_Offset: float = None
+
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value modulation results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.average.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value modulation results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CcError:
-	"""CcError commands group definition. 12 total commands, 4 Sub-groups, 0 group commands"""
+class MsfPowerCls:
+	"""MsfPower commands group definition. 10 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ccError", core, parent)
+		self._cmd_group = CommandsGroup("msfPower", core, parent)
 
 	@property
 	def current(self):
-		"""current commands group. 0 Sub-classes, 3 commands."""
+		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .CcError_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
-		"""average commands group. 0 Sub-classes, 3 commands."""
+		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .CcError_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
-	def extreme(self):
-		"""extreme commands group. 0 Sub-classes, 3 commands."""
-		if not hasattr(self, '_extreme'):
-			from .CcError_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
-		return self._extreme
+	def maximum(self):
+		"""maximum commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_maximum'):
+			from .Maximum import MaximumCls
+			self._maximum = MaximumCls(self._core, self._cmd_group)
+		return self._maximum
+
+	@property
+	def minimum(self):
+		"""minimum commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_minimum'):
+			from .Minimum import MinimumCls
+			self._minimum = MinimumCls(self._core, self._cmd_group)
+		return self._minimum
 
 	@property
 	def standardDev(self):
-		"""standardDev commands group. 0 Sub-classes, 3 commands."""
+		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .CcError_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'CcError':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MsfPowerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = CcError(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MsfPowerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Average.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class AverageCls:
+	"""Average commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.average.fetch() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.average.read() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:AVERage \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.ccError.average.calculate() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.average.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Otolerance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ...... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class OtoleranceCls:
+	"""Otolerance commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
-
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.current.fetch() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		self._cmd_group = CommandsGroup("otolerance", core, parent)
 
 	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.current.read() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:OTOLerance \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.otolerance.read() \n
+		Returns the out of tolerance result for modulation measurements. It indicates the percentage of measurement intervals of
+		the statistic count for modulation measurements exceeding the specified TX Modulation limits or Pulse Mask limits. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:return: out_of_tolerance: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:OTOLerance?', suppressed)
 		return Conversions.str_to_float(response)
 
-	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:CURRent \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.ccError.current.calculate() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+	def fetch(self) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:OTOLerance \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.otolerance.fetch() \n
+		Returns the out of tolerance result for modulation measurements. It indicates the percentage of measurement intervals of
+		the statistic count for modulation measurements exceeding the specified TX Modulation limits or Pulse Mask limits. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:return: out_of_tolerance: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:CURRent?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:OTOLerance?', suppressed)
+		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Otolerance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ...... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class OtoleranceCls:
+	"""Otolerance commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("otolerance", core, parent)
 
 	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.extreme.fetch() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:OTOLerance \n
+		Snippet: value: float = driver.uwbMeas.multiEval.tsMask.otolerance.fetch() \n
+		Returns the out of tolerance result for transmit spectrum mask measurements. It indicates the percentage of measurement
+		intervals of the statistic count for spectrum measurements exceeding the specified Transmit Spectrum Mask limits. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:return: out_of_tolerance: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:OTOLerance?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.extreme.read() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:OTOLerance \n
+		Snippet: value: float = driver.uwbMeas.multiEval.tsMask.otolerance.read() \n
+		Returns the out of tolerance result for transmit spectrum mask measurements. It indicates the percentage of measurement
+		intervals of the statistic count for spectrum measurements exceeding the specified Transmit Spectrum Mask limits. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:return: out_of_tolerance: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:OTOLerance?', suppressed)
 		return Conversions.str_to_float(response)
-
-	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.ccError.extreme.calculate() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/StandardDev.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
-from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.standardDev.fetch() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: evm: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.standardDev.read() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: evm: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
-
-	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:SDEViation \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.ccError.standardDev.calculate() \n
-		Returns the positive or negative chip clock error for the selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: error: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:SDEViation?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Cevm:
-	"""Cevm commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class PmlWidthCls:
+	"""PmlWidth commands group definition. 12 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("cevm", core, parent)
+		self._cmd_group = CommandsGroup("pmlWidth", core, parent)
 
 	@property
 	def current(self):
-		"""current commands group. 0 Sub-classes, 2 commands."""
+		"""current commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_current'):
-			from .Cevm_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
-		"""average commands group. 0 Sub-classes, 2 commands."""
+		"""average commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_average'):
-			from .Cevm_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
-		"""extreme commands group. 0 Sub-classes, 2 commands."""
+		"""extreme commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_extreme'):
-			from .Cevm_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
-		"""standardDev commands group. 0 Sub-classes, 2 commands."""
+		"""standardDev commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Cevm_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'Cevm':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PmlWidthCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Cevm(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PmlWidthCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Average.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.average.fetch() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: evm: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.average.read() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: evm: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Xvalues.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.current.fetch() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.xvalues.fetch() \n
+		Returns the x-values of the transmit spectrum trace. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:return: values: Comma-separated list of frequency values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.current.read() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.xvalues.read() \n
+		Returns the x-values of the transmit spectrum trace. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:return: values: Comma-separated list of frequency values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Extreme.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.extreme.fetch() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.rmarker.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMARKER time. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: rmarker: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.extreme.read() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.rmarker.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMARKER time. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: rmarker: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/StandardDev.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.standardDev.fetch() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbol: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.standardDev.read() \n
-		Returns the RMS of the chip error vector magnitude for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: evm: Chip error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbol: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CpJitter:
-	"""CpJitter commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class CpJitterCls:
+	"""CpJitter commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("cpJitter", core, parent)
+		self._cmd_group = CommandsGroup("cpJitter", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .CpJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .CpJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_extreme'):
-			from .CpJitter_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .CpJitter_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'CpJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'CpJitterCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = CpJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CpJitterCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Xvalues.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.average.fetch() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.xvalues.fetch() \n
+		Returns the x-values of the normalized cross correlation trace. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.average.read() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.xvalues.read() \n
+		Returns the x-values of the normalized cross correlation trace. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Xvalues.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.current.fetch() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.powerVsTime.xvalues.fetch() \n
+		Returns the x-values of the power vs time trace. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.current.read() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.powerVsTime.xvalues.read() \n
+		Returns the x-values of the power vs time trace. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Extreme.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.extreme.fetch() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.extreme.read() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
+
+	# noinspection PyTypeChecker
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
+		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/StandardDev.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.standardDev.fetch() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.standardDev.read() \n
-		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols for the selected packet
-		number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip phase jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CtJitter:
-	"""CtJitter commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class CtJitterCls:
+	"""CtJitter commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ctJitter", core, parent)
+		self._cmd_group = CommandsGroup("ctJitter", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .CtJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .CtJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_extreme'):
-			from .CtJitter_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .CtJitter_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'CtJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'CtJitterCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = CtJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CtJitterCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.average.fetch() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ctJitter.average.fetch() \n
+		Returns the y-values of the average chip time jitter trace. See also 'Chip Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:return: jitter: Comma-separated list of chip jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.average.read() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ctJitter.average.read() \n
+		Returns the y-values of the average chip time jitter trace. See also 'Chip Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:return: jitter: Comma-separated list of chip jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Average.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.current.fetch() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbws.average.fetch() \n
+		Returns the y-values of the average 1-MHz spectrum trace. See also '1MHz / 50MHz Spectrum square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:return: power: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:AVERage?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.current.read() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbws.average.read() \n
+		Returns the y-values of the average 1-MHz spectrum trace. See also '1MHz / 50MHz Spectrum square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:return: power: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:AVERage?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Extreme.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.extreme.fetch() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip time jitter RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.extreme.read() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip time jitter RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Extreme.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.standardDev.fetch() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.standardDev.read() \n
-		Returns the RMS time jitter value averaged over all chips of the detected preamble symbols for the selected packet number
-		<PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cpJitter.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over all chips of the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Chip time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CPJitter:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Extreme.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,73 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from ..... import enums
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
+			- Reliability: int: 'Reliability indicator'
 			- Freq_Offset_Hz: float: No parameter help available
 			- Freq_Offset: float: No parameter help available
 			- Chip_Clock_Error: float: No parameter help available
 			- Pulse_Nsme: float: No parameter help available
 			- Sym_Mod_Accuracy: float: No parameter help available
 			- Side_Lobe_Peak: float: No parameter help available
 			- Pulse_Ml_Width: float: No parameter help available
-			- Sym_Time_Jitter: float: RMS time jitter value averaged over all the detected preamble symbols
-			- Sym_Phase_Jitter: float: RMS phase jitter value averaged over all the detected preamble symbols
+			- Sym_Time_Jitter: float: No parameter help available
+			- Sym_Phase_Jitter: float: No parameter help available
 			- Chip_Time_Jitter: float: No parameter help available
 			- Chip_Phase_Jitter: float: No parameter help available
 			- Symbol_Evm: float: No parameter help available
-			- Chip_Evm: float: No parameter help available"""
+			- Chip_Evm: float: No parameter help available
+			- Rmarker: float: RMARKER time
+			- Shr_Nrmse: float: NRMSE for SHR
+			- Phr_Nrmse: float: NRMSE for PHR
+			- Psdu_Nrmse: float: NRMSE for PSDU
+			- Sts_Nrmse: float: NRMSE for STS
+			- Sync_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Sfd_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Sts_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Iq_Offset: float: I/Q offset"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Freq_Offset_Hz'),
 			ArgStruct.scalar_float('Freq_Offset'),
 			ArgStruct.scalar_float('Chip_Clock_Error'),
 			ArgStruct.scalar_float('Pulse_Nsme'),
 			ArgStruct.scalar_float('Sym_Mod_Accuracy'),
 			ArgStruct.scalar_float('Side_Lobe_Peak'),
 			ArgStruct.scalar_float('Pulse_Ml_Width'),
 			ArgStruct.scalar_float('Sym_Time_Jitter'),
 			ArgStruct.scalar_float('Sym_Phase_Jitter'),
 			ArgStruct.scalar_float('Chip_Time_Jitter'),
 			ArgStruct.scalar_float('Chip_Phase_Jitter'),
 			ArgStruct.scalar_float('Symbol_Evm'),
-			ArgStruct.scalar_float('Chip_Evm')]
+			ArgStruct.scalar_float('Chip_Evm'),
+			ArgStruct.scalar_float('Rmarker'),
+			ArgStruct.scalar_float('Shr_Nrmse'),
+			ArgStruct.scalar_float('Phr_Nrmse'),
+			ArgStruct.scalar_float('Psdu_Nrmse'),
+			ArgStruct.scalar_float('Sts_Nrmse'),
+			ArgStruct.scalar_enum('Sync_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_enum('Sfd_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_enum('Sts_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_float('Iq_Offset')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Freq_Offset_Hz: float = None
 			self.Freq_Offset: float = None
 			self.Chip_Clock_Error: float = None
@@ -57,23 +77,34 @@
 			self.Pulse_Ml_Width: float = None
 			self.Sym_Time_Jitter: float = None
 			self.Sym_Phase_Jitter: float = None
 			self.Chip_Time_Jitter: float = None
 			self.Chip_Phase_Jitter: float = None
 			self.Symbol_Evm: float = None
 			self.Chip_Evm: float = None
-
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.current.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+			self.Rmarker: float = None
+			self.Shr_Nrmse: float = None
+			self.Phr_Nrmse: float = None
+			self.Psdu_Nrmse: float = None
+			self.Sts_Nrmse: float = None
+			self.Sync_Pulse_Loc_Pol: enums.Result = None
+			self.Sfd_Pulse_Loc_Pol: enums.Result = None
+			self.Sts_Pulse_Loc_Pol: enums.Result = None
+			self.Iq_Offset: float = None
+
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value modulation results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CURRent?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.current.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value modulation results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CURRent?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Current.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from .....Internal.RepeatedCapability import RepeatedCapability
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class CurrentCls:
+	"""Current commands group definition. 2 total commands, 0 Subgroups, 2 group commands
+	Repeated Capability: Ppdu, default value after init: Ppdu.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("current", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_ppdu_get', 'repcap_ppdu_set', repcap.Ppdu.Nr1)
+
+	def repcap_ppdu_set(self, ppdu: repcap.Ppdu) -> None:
+		"""Repeated Capability default value numeric suffix.
+		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Ppdu.Default
+		Default value after init: Ppdu.Nr1"""
+		self._cmd_group.set_repcap_enum_value(ppdu)
+
+	def repcap_ppdu_get(self) -> repcap.Ppdu:
+		"""Returns the current default repeated capability for the child set/get methods"""
+		# noinspection PyTypeChecker
+		return self._cmd_group.get_repcap_enum_value()
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
-			- Freq_Offset_Hz: float: No parameter help available
-			- Freq_Offset: float: No parameter help available
-			- Chip_Clock_Error: float: No parameter help available
-			- Pulse_Nsme: float: No parameter help available
-			- Sym_Mod_Accuracy: float: No parameter help available
-			- Side_Lobe_Peak: float: No parameter help available
-			- Pulse_Ml_Width: float: No parameter help available
-			- Sym_Time_Jitter: float: RMS time jitter value averaged over all the detected preamble symbols
-			- Sym_Phase_Jitter: float: RMS phase jitter value averaged over all the detected preamble symbols
-			- Chip_Time_Jitter: float: No parameter help available
-			- Chip_Phase_Jitter: float: No parameter help available
-			- Symbol_Evm: float: No parameter help available
-			- Chip_Evm: float: No parameter help available"""
+			- Reliability: int: 'Reliability indicator'
+			- Preamble_Power: float: No parameter help available
+			- Pre_Peak_Power: float: No parameter help available
+			- Data_Power: float: No parameter help available
+			- Data_Peak_Power: float: No parameter help available
+			- Max_Spec_Power: float: No parameter help available
+			- Max_Spec_50_Power: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
-			ArgStruct.scalar_float('Freq_Offset_Hz'),
-			ArgStruct.scalar_float('Freq_Offset'),
-			ArgStruct.scalar_float('Chip_Clock_Error'),
-			ArgStruct.scalar_float('Pulse_Nsme'),
-			ArgStruct.scalar_float('Sym_Mod_Accuracy'),
-			ArgStruct.scalar_float('Side_Lobe_Peak'),
-			ArgStruct.scalar_float('Pulse_Ml_Width'),
-			ArgStruct.scalar_float('Sym_Time_Jitter'),
-			ArgStruct.scalar_float('Sym_Phase_Jitter'),
-			ArgStruct.scalar_float('Chip_Time_Jitter'),
-			ArgStruct.scalar_float('Chip_Phase_Jitter'),
-			ArgStruct.scalar_float('Symbol_Evm'),
-			ArgStruct.scalar_float('Chip_Evm')]
+			ArgStruct.scalar_float('Preamble_Power'),
+			ArgStruct.scalar_float('Pre_Peak_Power'),
+			ArgStruct.scalar_float('Data_Power'),
+			ArgStruct.scalar_float('Data_Peak_Power'),
+			ArgStruct.scalar_float('Max_Spec_Power'),
+			ArgStruct.scalar_float('Max_Spec_50_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
-			self.Freq_Offset_Hz: float = None
-			self.Freq_Offset: float = None
-			self.Chip_Clock_Error: float = None
-			self.Pulse_Nsme: float = None
-			self.Sym_Mod_Accuracy: float = None
-			self.Side_Lobe_Peak: float = None
-			self.Pulse_Ml_Width: float = None
-			self.Sym_Time_Jitter: float = None
-			self.Sym_Phase_Jitter: float = None
-			self.Chip_Time_Jitter: float = None
-			self.Chip_Phase_Jitter: float = None
-			self.Symbol_Evm: float = None
-			self.Chip_Evm: float = None
-
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.extreme.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+			self.Preamble_Power: float = None
+			self.Pre_Peak_Power: float = None
+			self.Data_Power: float = None
+			self.Data_Peak_Power: float = None
+			self.Max_Spec_Power: float = None
+			self.Max_Spec_50_Power: float = None
+
+	def fetch(self, ppdu=repcap.Ppdu.Default) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.current.fetch(ppdu = repcap.Ppdu.Default) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.extreme.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Default) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.current.read(ppdu = repcap.Ppdu.Default) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:EXTReme?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
+
+	def clone(self) -> 'CurrentCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
+		Also copies all the existing default Repeated Capabilities setting,
+		which you can change independently without affecting the original group"""
+		new_group = CurrentCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
+		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Foffset:
-	"""Foffset commands group definition. 12 total commands, 4 Sub-groups, 0 group commands"""
+class FoffsetCls:
+	"""Foffset commands group definition. 12 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("foffset", core, parent)
+		self._cmd_group = CommandsGroup("foffset", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_current'):
-			from .Foffset_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_average'):
-			from .Foffset_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_extreme'):
-			from .Foffset_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Foffset_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'Foffset':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'FoffsetCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Foffset(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = FoffsetCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/StandardDev.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,53 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ...... import enums
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .......Internal.Types import DataType
+from ....... import enums
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.average.fetch() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: level: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.average.read() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: level: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:AVERage \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.foffset.average.calculate() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.phr.plevel.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: level: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Extreme.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.current.fetch() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the frequency error relative to the channel center frequency in ppm. \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.current.read() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the frequency error relative to the channel center frequency in ppm. \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:CURRent \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.foffset.current.calculate() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.foffset.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the frequency error relative to the channel center frequency in ppm. \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Extreme.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
-from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.extreme.fetch() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.extreme.read() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
-
-	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.foffset.extreme.calculate() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:EXTReme?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/StandardDev.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.standardDev.fetch() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.foffset.standardDev.read() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:SDEViation \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.foffset.standardDev.calculate() \n
-		Returns the frequency error relative to the channel center frequency in ppm for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse main lobe width. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: width: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFFset:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Fofh:
-	"""Fofh commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class StJitterCls:
+	"""StJitter commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("fofh", core, parent)
+		self._cmd_group = CommandsGroup("stJitter", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .Fofh_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .Fofh_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_extreme'):
-			from .Fofh_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Fofh_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'Fofh':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'StJitterCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Fofh(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = StJitterCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Average.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.average.fetch() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the frequency error relative to the channel center frequency in Hz. \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.average.read() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the frequency error relative to the channel center frequency in Hz. \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/StandardDev.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.current.fetch() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.current.read() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/StandardDev.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.extreme.fetch() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:SDEViation<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.modulation.iqOffset.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the I/Q offset. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: iq_offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:EXTReme?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:SDEViation{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.extreme.read() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:SDEViation<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.modulation.iqOffset.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the I/Q offset. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: iq_offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:EXTReme?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:SDEViation{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Xvalues.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.standardDev.fetch() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.spJitter.xvalues.fetch() \n
+		Returns the x-values of the symbol phase jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:return: values: Comma-separated list of phase values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.fofh.standardDev.read() \n
-		Returns the frequency error relative to the channel center frequency in Hz for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.spJitter.xvalues.read() \n
+		Returns the x-values of the symbol phase jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: offset: No help available"""
+			:return: values: Comma-separated list of phase values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:FOFH:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Nmse:
-	"""Nmse commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class SpJitterCls:
+	"""SpJitter commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("nmse", core, parent)
+		self._cmd_group = CommandsGroup("spJitter", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .Nmse_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .Nmse_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_extreme'):
-			from .Nmse_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Nmse_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'Nmse':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SpJitterCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Nmse(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SpJitterCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Extreme.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.average.fetch() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse NMSE (normalized mean square error between the measured pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: nmse: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.average.read() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse NMSE (normalized mean square error between the measured pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: nmse: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Average.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.current.fetch() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse NMSE (normalized mean square error between the measured pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: nmse: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.current.read() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse NMSE (normalized mean square error between the measured pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: nmse: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Extreme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.extreme.fetch() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: evm: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.extreme.read() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.cevm.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: evm: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CEVM:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/StandardDev.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.standardDev.fetch() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse NMSE (normalized mean square error between the measured pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: nmse: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.standardDev.read() \n
-		Returns the normalized mean square error between the measured pulse and the reference pulse for the selected packet
-		number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.nmse.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the pulse NMSE (normalized mean square error between the measured pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: nmse: Normalized mean square error"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: nmse: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:NMSE:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class PmlWidth:
-	"""PmlWidth commands group definition. 12 total commands, 4 Sub-groups, 0 group commands"""
+class SbwlCls:
+	"""Sbwl commands group definition. 6 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("pmlWidth", core, parent)
+		self._cmd_group = CommandsGroup("sbwl", core, parent)
 
 	@property
 	def current(self):
-		"""current commands group. 0 Sub-classes, 3 commands."""
+		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .PmlWidth_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
-		"""average commands group. 0 Sub-classes, 3 commands."""
+		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .PmlWidth_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
-	def extreme(self):
-		"""extreme commands group. 0 Sub-classes, 3 commands."""
-		if not hasattr(self, '_extreme'):
-			from .PmlWidth_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
-		return self._extreme
+	def xvalues(self):
+		"""xvalues commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_xvalues'):
+			from .Xvalues import XvaluesCls
+			self._xvalues = XvaluesCls(self._core, self._cmd_group)
+		return self._xvalues
 
-	@property
-	def standardDev(self):
-		"""standardDev commands group. 0 Sub-classes, 3 commands."""
-		if not hasattr(self, '_standardDev'):
-			from .PmlWidth_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
-		return self._standardDev
-
-	def clone(self) -> 'PmlWidth':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SbwlCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = PmlWidth(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SbwlCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Extreme.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,53 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ...... import enums
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .......Internal.Types import DataType
+from ....... import enums
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.average.fetch() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.nrmse.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the NRMSE for STS, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.average.read() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.nrmse.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the NRMSE for STS, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.average.calculate() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:EXTReme<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.sts.nrmse.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the NRMSE for STS, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Extreme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.current.fetch() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.current.read() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.current.calculate() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Extreme.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
-from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.fetch() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:EXTReme<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.modulation.iqOffset.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the I/Q offset. \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: iq_offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:EXTReme{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.read() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:EXTReme<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.modulation.iqOffset.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the I/Q offset. \n
 		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: iq_offset: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme?', suppressed)
-		return Conversions.str_to_float(response)
-
-	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.calculate() \n
-		Returns the width of the main lobe at a cross correlation magnitude of 0.8 for the selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: width: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:IQOFfset:EXTReme{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sevm:
-	"""Sevm commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class SevmCls:
+	"""Sevm commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sevm", core, parent)
+		self._cmd_group = CommandsGroup("sevm", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .Sevm_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .Sevm_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_extreme'):
-			from .Sevm_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Sevm_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'Sevm':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SevmCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Sevm(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SevmCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Average.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.average.fetch() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the peak power of the data part. \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.average.read() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the peak power of the data part. \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Otolerance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class OtoleranceCls:
+	"""Otolerance commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("otolerance", core, parent)
 
 	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.current.fetch() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:OTOLerance \n
+		Snippet: value: float = driver.uwbMeas.multiEval.pmask.otolerance.fetch() \n
+		No command help available \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:return: out_of_tolerance: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:OTOLerance?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.current.read() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:PMASk:OTOLerance \n
+		Snippet: value: float = driver.uwbMeas.multiEval.pmask.otolerance.read() \n
+		No command help available \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:return: out_of_tolerance: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:PMASk:OTOLerance?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Extreme.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.extreme.fetch() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbol: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.extreme.read() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbol: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/StandardDev.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.standardDev.fetch() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.rmarker.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMARKER time. \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: rmarker: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.standardDev.read() \n
-		Returns the RMS of the symbol error vector magnitude for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.rmarker.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMARKER time. \n
 		Suppressed linked return values: reliability \n
-			:return: symbol: Symbol error vector magnitude"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: rmarker: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:RMARker:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SlPeak:
-	"""SlPeak commands group definition. 12 total commands, 4 Sub-groups, 0 group commands"""
+class SlPeakCls:
+	"""SlPeak commands group definition. 12 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("slPeak", core, parent)
+		self._cmd_group = CommandsGroup("slPeak", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_current'):
-			from .SlPeak_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_average'):
-			from .SlPeak_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_extreme'):
-			from .SlPeak_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .SlPeak_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'SlPeak':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SlPeakCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = SlPeak(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SlPeakCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Extreme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.average.fetch() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the positive or negative chip clock error. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.average.read() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ccError.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the positive or negative chip clock error. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.average.calculate() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.ccError.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the positive or negative chip clock error. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:CCERor:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Extreme.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.current.fetch() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.current.read() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.current.calculate() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/StandardDev.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
-from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.extreme.fetch() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip time jitter RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.extreme.read() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.ctJitter.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the chip time jitter RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:CTJittter:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
-
-	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.extreme.calculate() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Average.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,53 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ...... import enums
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .......Internal.Types import DataType
+from ....... import enums
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class AverageCls:
+	"""Average commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.standardDev.fetch() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SHR:NRMSe:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.shr.nrmse.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the NRMSE for SHR, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SHR:NRMSe:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.standardDev.read() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SHR:NRMSe:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.shr.nrmse.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the NRMSE for SHR, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SHR:NRMSe:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.standardDev.calculate() \n
-		Returns the largest magnitude of side lobe peaks of the normalized cross correlation between the measured pulse and the
-		reference pulse for the selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SHR:NRMSe:AVERage<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.shr.nrmse.average.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the NRMSE for SHR, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
-			:return: peak: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: error: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SHR:NRMSe:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SmAccuracy:
-	"""SmAccuracy commands group definition. 12 total commands, 4 Sub-groups, 0 group commands"""
+class CcErrorCls:
+	"""CcError commands group definition. 12 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("smAccuracy", core, parent)
+		self._cmd_group = CommandsGroup("ccError", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_current'):
-			from .SmAccuracy_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_average'):
-			from .SmAccuracy_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_extreme'):
-			from .SmAccuracy_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .SmAccuracy_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'SmAccuracy':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'CcErrorCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = SmAccuracy(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CcErrorCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Average.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class AverageCls:
+	"""Average commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.average.fetch() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.average.read() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.average.calculate() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.average.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ...... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class AsSymbolsCls:
+	"""AsSymbols commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("asSymbols", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.current.fetch() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.asSymbols.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the number of symbols detected in the SYNC field of the SHR. \n
 		Suppressed linked return values: reliability \n
-			:return: accuracy: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbols: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.current.read() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.asSymbols.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the number of symbols detected in the SYNC field of the SHR. \n
 		Suppressed linked return values: reliability \n
-			:return: accuracy: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbols: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
-
-	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.current.calculate() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: accuracy: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Extreme.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,42 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ...... import enums
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .......Internal.Types import DataType
+from ....... import enums
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.fetch() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
-		Suppressed linked return values: reliability \n
-			:return: accuracy: No help available"""
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme?', suppressed)
-		return Conversions.str_to_float(response)
-
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.read() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	# noinspection PyTypeChecker
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> enums.Result:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLPolarity:EXTReme<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.modulation.sts.plPolarity.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the result of the check for correct pulse location and polarity, for STS. \n
 		Suppressed linked return values: reliability \n
-			:return: accuracy: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: sts_polarity: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLPolarity:EXTReme{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.calculate() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> enums.Result:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLPolarity:EXTReme<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.modulation.sts.plPolarity.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the result of the check for correct pulse location and polarity, for STS. \n
 		Suppressed linked return values: reliability \n
-			:return: accuracy: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: sts_polarity: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLPolarity:EXTReme{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/StandardDev.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.fetch() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.read() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
-	def calculate(self) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.calculate() \n
-		Returns the magnitude of the normalized cross correlation between the measured pulse and the reference pulse for the
-		selected packet number <PPDU>. \n
+	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SpJitter:
-	"""SpJitter commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class FofhCls:
+	"""Fofh commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("spJitter", core, parent)
+		self._cmd_group = CommandsGroup("fofh", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .SpJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .SpJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_extreme'):
-			from .SpJitter_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .SpJitter_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'SpJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'FofhCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = SpJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = FofhCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.average.fetch() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.average.fetch() \n
+		Returns the y-values of the average chip phase jitter trace. See also 'Chip Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:return: jitter: Comma-separated list of chip jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.average.read() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.average.read() \n
+		Returns the y-values of the average chip phase jitter trace. See also 'Chip Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:return: jitter: Comma-separated list of chip jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dppdu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class DppduCls:
+	"""Dppdu commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("dppdu", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.current.fetch() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def fetch(self) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DPPDu \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.dppdu.fetch() \n
+		Returns the number of detected PPDUs in the capture length. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:return: detected_ppdu: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DPPDu?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.current.read() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def read(self) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DPPDu \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.dppdu.read() \n
+		Returns the number of detected PPDUs in the capture length. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:return: detected_ppdu: No help available"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DPPDu?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Average.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.extreme.fetch() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbol: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.extreme.read() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sevm.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the symbol EVM RMS value. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbol: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SEVM:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Xvalues.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.standardDev.fetch() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbwl.xvalues.fetch() \n
+		Returns the x-values of the 50-MHz spectrum trace. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:return: values: Comma-separated list of frequency values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.standardDev.read() \n
-		Returns the RMS phase jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbwl.xvalues.read() \n
+		Returns the x-values of the 50-MHz spectrum trace. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol phase jitter"""
+			:return: values: Comma-separated list of frequency values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StJitter:
-	"""StJitter commands group definition. 8 total commands, 4 Sub-groups, 0 group commands"""
+class IqOffsetCls:
+	"""IqOffset commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("stJitter", core, parent)
+		self._cmd_group = CommandsGroup("iqOffset", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .StJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .StJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def extreme(self):
 		"""extreme commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_extreme'):
-			from .StJitter_.Extreme import Extreme
-			self._extreme = Extreme(self._core, self._base)
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
 		return self._extreme
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .StJitter_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'StJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'IqOffsetCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = StJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = IqOffsetCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Average.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.average.fetch() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.stJitter.average.fetch() \n
+		Returns the y-values of the average symbol time jitter trace. See also 'Symbol Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:return: jitter: Comma-separated list of symbol jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:AVERage?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.average.read() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.stJitter.average.read() \n
+		Returns the y-values of the average symbol time jitter trace. See also 'Symbol Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:return: jitter: Comma-separated list of symbol jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:AVERage?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Extreme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .......Internal.Types import DataType
+from ....... import enums
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ExtremeCls:
+	"""Extreme commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("extreme", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.current.fetch() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	# noinspection PyTypeChecker
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> enums.Result:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SFD:PLPolarity:EXTReme<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.modulation.sfd.plPolarity.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the result of the check for correct pulse location and polarity, for SFD. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: sfd_polarity: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SFD:PLPolarity:EXTReme{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.current.read() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	# noinspection PyTypeChecker
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> enums.Result:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SFD:PLPolarity:EXTReme<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.modulation.sfd.plPolarity.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the result of the check for correct pulse location and polarity, for SFD. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: sfd_polarity: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SFD:PLPolarity:EXTReme{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Extreme.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Average.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .......Internal.Types import DataType
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Extreme:
-	"""Extreme commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("extreme", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.extreme.fetch() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: level: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:EXTReme \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.extreme.read() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: level: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:EXTReme?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Average.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.standardDev.fetch() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbwl.average.fetch() \n
+		Returns the y-values of the average 50-MHz spectrum trace. See also '1MHz / 50MHz Spectrum square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:return: power: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:AVERage?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.stJitter.standardDev.read() \n
-		Returns the RMS time jitter value averaged over all the detected preamble symbols for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbwl.average.read() \n
+		Returns the y-values of the average 50-MHz spectrum trace. See also '1MHz / 50MHz Spectrum square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Symbol time jitter"""
+			:return: power: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STJitter:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWL:AVERage?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StandardDev.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,73 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from ..... import enums
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
+			- Reliability: int: 'Reliability indicator'
 			- Freq_Offset_Hz: float: No parameter help available
 			- Freq_Offset: float: No parameter help available
 			- Chip_Clock_Error: float: No parameter help available
 			- Pulse_Nsme: float: No parameter help available
 			- Sym_Mod_Accuracy: float: No parameter help available
 			- Side_Lobe_Peak: float: No parameter help available
 			- Pulse_Ml_Width: float: No parameter help available
-			- Sym_Time_Jitter: float: RMS time jitter value averaged over all the detected preamble symbols
-			- Sym_Phase_Jitter: float: RMS phase jitter value averaged over all the detected preamble symbols
+			- Sym_Time_Jitter: float: No parameter help available
+			- Sym_Phase_Jitter: float: No parameter help available
 			- Chip_Time_Jitter: float: No parameter help available
 			- Chip_Phase_Jitter: float: No parameter help available
 			- Symbol_Evm: float: No parameter help available
-			- Chip_Evm: float: No parameter help available"""
+			- Chip_Evm: float: No parameter help available
+			- Rmarker: float: RMARKER time
+			- Shr_Nrmse: float: NRMSE for SHR
+			- Phr_Nrmse: float: NRMSE for PHR
+			- Psdu_Nrmse: float: NRMSE for PSDU
+			- Sts_Nrmse: float: NRMSE for STS
+			- Sync_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Sfd_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Sts_Pulse_Loc_Pol: enums.Result: No parameter help available
+			- Iq_Offset: float: I/Q offset"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Freq_Offset_Hz'),
 			ArgStruct.scalar_float('Freq_Offset'),
 			ArgStruct.scalar_float('Chip_Clock_Error'),
 			ArgStruct.scalar_float('Pulse_Nsme'),
 			ArgStruct.scalar_float('Sym_Mod_Accuracy'),
 			ArgStruct.scalar_float('Side_Lobe_Peak'),
 			ArgStruct.scalar_float('Pulse_Ml_Width'),
 			ArgStruct.scalar_float('Sym_Time_Jitter'),
 			ArgStruct.scalar_float('Sym_Phase_Jitter'),
 			ArgStruct.scalar_float('Chip_Time_Jitter'),
 			ArgStruct.scalar_float('Chip_Phase_Jitter'),
 			ArgStruct.scalar_float('Symbol_Evm'),
-			ArgStruct.scalar_float('Chip_Evm')]
+			ArgStruct.scalar_float('Chip_Evm'),
+			ArgStruct.scalar_float('Rmarker'),
+			ArgStruct.scalar_float('Shr_Nrmse'),
+			ArgStruct.scalar_float('Phr_Nrmse'),
+			ArgStruct.scalar_float('Psdu_Nrmse'),
+			ArgStruct.scalar_float('Sts_Nrmse'),
+			ArgStruct.scalar_enum('Sync_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_enum('Sfd_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_enum('Sts_Pulse_Loc_Pol', enums.Result),
+			ArgStruct.scalar_float('Iq_Offset')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Freq_Offset_Hz: float = None
 			self.Freq_Offset: float = None
 			self.Chip_Clock_Error: float = None
@@ -57,23 +77,34 @@
 			self.Pulse_Ml_Width: float = None
 			self.Sym_Time_Jitter: float = None
 			self.Sym_Phase_Jitter: float = None
 			self.Chip_Time_Jitter: float = None
 			self.Chip_Phase_Jitter: float = None
 			self.Symbol_Evm: float = None
 			self.Chip_Evm: float = None
-
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.standardDev.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+			self.Rmarker: float = None
+			self.Shr_Nrmse: float = None
+			self.Phr_Nrmse: float = None
+			self.Psdu_Nrmse: float = None
+			self.Sts_Nrmse: float = None
+			self.Sync_Pulse_Loc_Pol: enums.Result = None
+			self.Sfd_Pulse_Loc_Pol: enums.Result = None
+			self.Sts_Pulse_Loc_Pol: enums.Result = None
+			self.Iq_Offset: float = None
+
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value modulation results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.standardDev.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value modulation results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SDEViation{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,59 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Power:
-	"""Power commands group definition. 60 total commands, 10 Sub-groups, 0 group commands"""
+class PlevelCls:
+	"""Plevel commands group definition. 14 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("power", core, parent)
+		self._cmd_group = CommandsGroup("plevel", core, parent)
 
 	@property
 	def current(self):
-		"""current commands group. 0 Sub-classes, 2 commands."""
+		"""current commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_current'):
-			from .Power_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .Power_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def maximum(self):
-		"""maximum commands group. 0 Sub-classes, 2 commands."""
+		"""maximum commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_maximum'):
-			from .Power_.Maximum import Maximum
-			self._maximum = Maximum(self._core, self._base)
+			from .Maximum import MaximumCls
+			self._maximum = MaximumCls(self._core, self._cmd_group)
 		return self._maximum
 
 	@property
 	def minimum(self):
-		"""minimum commands group. 0 Sub-classes, 2 commands."""
+		"""minimum commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_minimum'):
-			from .Power_.Minimum import Minimum
-			self._minimum = Minimum(self._core, self._base)
+			from .Minimum import MinimumCls
+			self._minimum = MinimumCls(self._core, self._cmd_group)
 		return self._minimum
 
 	@property
 	def standardDev(self):
-		"""standardDev commands group. 0 Sub-classes, 2 commands."""
+		"""standardDev commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Power_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	@property
-	def ppower(self):
-		"""ppower commands group. 5 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ppower'):
-			from .Power_.Ppower import Ppower
-			self._ppower = Ppower(self._core, self._base)
-		return self._ppower
-
-	@property
-	def ppPower(self):
-		"""ppPower commands group. 5 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ppPower'):
-			from .Power_.PpPower import PpPower
-			self._ppPower = PpPower(self._core, self._base)
-		return self._ppPower
-
-	@property
-	def dpower(self):
-		"""dpower commands group. 5 Sub-classes, 0 commands."""
-		if not hasattr(self, '_dpower'):
-			from .Power_.Dpower import Dpower
-			self._dpower = Dpower(self._core, self._base)
-		return self._dpower
-
-	@property
-	def dpPower(self):
-		"""dpPower commands group. 5 Sub-classes, 0 commands."""
-		if not hasattr(self, '_dpPower'):
-			from .Power_.DpPower import DpPower
-			self._dpPower = DpPower(self._core, self._base)
-		return self._dpPower
-
-	@property
-	def msPower(self):
-		"""msPower commands group. 5 Sub-classes, 0 commands."""
-		if not hasattr(self, '_msPower'):
-			from .Power_.MsPower import MsPower
-			self._msPower = MsPower(self._core, self._base)
-		return self._msPower
-
-	def clone(self) -> 'Power':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PlevelCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Power(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PlevelCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Average.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
+			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
-			- Max_Spec_Power: float: No parameter help available"""
+			- Max_Spec_Power: float: No parameter help available
+			- Max_Spec_50_Power: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
-			ArgStruct.scalar_float('Max_Spec_Power')]
+			ArgStruct.scalar_float('Max_Spec_Power'),
+			ArgStruct.scalar_float('Max_Spec_50_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
+			self.Max_Spec_50_Power: float = None
 
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.average.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.average.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/StandardDev.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
+			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
-			- Max_Spec_Power: float: No parameter help available"""
+			- Max_Spec_Power: float: No parameter help available
+			- Max_Spec_50_Power: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
-			ArgStruct.scalar_float('Max_Spec_Power')]
+			ArgStruct.scalar_float('Max_Spec_Power'),
+			ArgStruct.scalar_float('Max_Spec_50_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
+			self.Max_Spec_50_Power: float = None
 
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.current.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:SDEViation<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:SDEViation{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.current.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:SDEViation<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:SDEViation{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,43 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class DpPower:
-	"""DpPower commands group definition. 10 total commands, 5 Sub-groups, 0 group commands"""
+class TsMaskCls:
+	"""TsMask commands group definition. 6 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dpPower", core, parent)
+		self._cmd_group = CommandsGroup("tsMask", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .DpPower_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .DpPower_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
-	def maximum(self):
-		"""maximum commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_maximum'):
-			from .DpPower_.Maximum import Maximum
-			self._maximum = Maximum(self._core, self._base)
-		return self._maximum
+	def xvalues(self):
+		"""xvalues commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_xvalues'):
+			from .Xvalues import XvaluesCls
+			self._xvalues = XvaluesCls(self._core, self._cmd_group)
+		return self._xvalues
 
-	@property
-	def minimum(self):
-		"""minimum commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_minimum'):
-			from .DpPower_.Minimum import Minimum
-			self._minimum = Minimum(self._core, self._base)
-		return self._minimum
-
-	@property
-	def standardDev(self):
-		"""standardDev commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_standardDev'):
-			from .DpPower_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
-		return self._standardDev
-
-	def clone(self) -> 'DpPower':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'TsMaskCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = DpPower(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = TsMaskCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.average.fetch() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.xvalues.fetch() \n
+		Returns the x-values of the chip phase jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of phase values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.average.read() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.xvalues.read() \n
+		Returns the x-values of the chip phase jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of phase values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:AVERage?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Xvalues.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.current.fetch() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbws.xvalues.fetch() \n
+		Returns the x-values of the 1-MHz spectrum trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of frequency values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.current.read() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.sbws.xvalues.read() \n
+		Returns the x-values of the 1-MHz spectrum trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of frequency values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:CURRent?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SBWS:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Maximum.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Xvalues.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Maximum:
-	"""Maximum commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("maximum", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MAXimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.maximum.fetch() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:PMASk:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.pmask.xvalues.fetch() \n
+		Returns the x-values of the pulse mask trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of normalized time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MAXimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:PMASk:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MAXimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.maximum.read() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:PMASk:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.pmask.xvalues.read() \n
+		Returns the x-values of the pulse mask trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of normalized time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MAXimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:PMASk:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Minimum.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/RaBit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Minimum:
-	"""Minimum commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class RaBitCls:
+	"""RaBit commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("minimum", core, parent)
+		self._cmd_group = CommandsGroup("raBit", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MINimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.minimum.fetch() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:RABit<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.raBit.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the decoded ranging bit of the PHR. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: ranging_bit: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MINimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:RABit{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MINimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.minimum.read() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:RABit<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.raBit.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the decoded ranging bit of the PHR. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: ranging_bit: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:MINimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:RABit{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Xvalues.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.standardDev.fetch() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.stJitter.xvalues.fetch() \n
+		Returns the x-values of the symbol time jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpPower.standardDev.read() \n
-		Returns the value of the data peak power for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.stJitter.xvalues.read() \n
+		Returns the x-values of the symbol time jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data peak power"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPPower:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dpower:
-	"""Dpower commands group definition. 10 total commands, 5 Sub-groups, 0 group commands"""
+class PpowerCls:
+	"""Ppower commands group definition. 10 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dpower", core, parent)
+		self._cmd_group = CommandsGroup("ppower", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .Dpower_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .Dpower_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def maximum(self):
 		"""maximum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_maximum'):
-			from .Dpower_.Maximum import Maximum
-			self._maximum = Maximum(self._core, self._base)
+			from .Maximum import MaximumCls
+			self._maximum = MaximumCls(self._core, self._cmd_group)
 		return self._maximum
 
 	@property
 	def minimum(self):
 		"""minimum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_minimum'):
-			from .Dpower_.Minimum import Minimum
-			self._minimum = Minimum(self._core, self._base)
+			from .Minimum import MinimumCls
+			self._minimum = MinimumCls(self._core, self._cmd_group)
 		return self._minimum
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Dpower_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'Dpower':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PpowerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Dpower(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PpowerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class MinimumCls:
+	"""Minimum commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("minimum", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.current.fetch() \n
-		Returns the value of the data power for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MINimum<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppower.minimum.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the mean power of the preamble part. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:CURRent \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.current.read() \n
-		Returns the value of the data power for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MINimum<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppower.minimum.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the mean power of the preamble part. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:CURRent?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Minimum.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/AsSymbols.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Minimum:
-	"""Minimum commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AsSymbolsCls:
+	"""AsSymbols commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("minimum", core, parent)
+		self._cmd_group = CommandsGroup("asSymbols", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:MINimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.minimum.fetch() \n
-		Returns the value of the data power for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:ASSYmbols<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.phr.asSymbols.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the number of symbols in the SYNC field, read from the PHR. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbols: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:MINimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:ASSYmbols{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:MINimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.minimum.read() \n
-		Returns the value of the data power for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:ASSYmbols<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.phr.asSymbols.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the number of symbols in the SYNC field, read from the PHR. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: symbols: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:MINimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:ASSYmbols{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Average.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.standardDev.fetch() \n
-		Returns the value of the data power for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.spJitter.average.fetch() \n
+		Returns the y-values of the average symbol phase jitter trace. See also 'Symbol Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data power"""
+			:return: jitter: Comma-separated list of symbol jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:AVERage?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.standardDev.read() \n
-		Returns the value of the data power for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.spJitter.average.read() \n
+		Returns the y-values of the average symbol phase jitter trace. See also 'Symbol Jitter square'. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Data power"""
+			:return: jitter: Comma-separated list of symbol jitter values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:SPJitter:AVERage?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Maximum.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Minimum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Maximum:
-	"""Maximum commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class MinimumCls:
+	"""Minimum commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("maximum", core, parent)
+		self._cmd_group = CommandsGroup("minimum", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
+			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
-			- Max_Spec_Power: float: No parameter help available"""
+			- Max_Spec_Power: float: No parameter help available
+			- Max_Spec_50_Power: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
-			ArgStruct.scalar_float('Max_Spec_Power')]
+			ArgStruct.scalar_float('Max_Spec_Power'),
+			ArgStruct.scalar_float('Max_Spec_50_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
+			self.Max_Spec_50_Power: float = None
 
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.maximum.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.minimum.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.maximum.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.minimum.read(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Minimum.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Maximum.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Minimum:
-	"""Minimum commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class MaximumCls:
+	"""Maximum commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("minimum", core, parent)
+		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
+			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
-			- Max_Spec_Power: float: No parameter help available"""
+			- Max_Spec_Power: float: No parameter help available
+			- Max_Spec_50_Power: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
-			ArgStruct.scalar_float('Max_Spec_Power')]
+			ArgStruct.scalar_float('Max_Spec_Power'),
+			ArgStruct.scalar_float('Max_Spec_50_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
+			self.Max_Spec_50_Power: float = None
 
-	def fetch(self) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.minimum.fetch() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum{ppdu_cmd_val}?', self.__class__.ResultData())
 
-	def read(self) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.minimum.read() \n
-		Return the current, average, extreme and standard deviation single value results for the selected packet number <PPDU>.
-		The values described below are returned by FETCh and READ commands. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.maximum.read(ppdu = repcap.Ppdu.Nr1) \n
+		Return the current, average, extreme and standard deviation single value power results. \n
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum?', self.__class__.ResultData())
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MsPower:
-	"""MsPower commands group definition. 10 total commands, 5 Sub-groups, 0 group commands"""
+class DpPowerCls:
+	"""DpPower commands group definition. 10 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("msPower", core, parent)
+		self._cmd_group = CommandsGroup("dpPower", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .MsPower_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .MsPower_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def maximum(self):
 		"""maximum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_maximum'):
-			from .MsPower_.Maximum import Maximum
-			self._maximum = Maximum(self._core, self._base)
+			from .Maximum import MaximumCls
+			self._maximum = MaximumCls(self._core, self._cmd_group)
 		return self._maximum
 
 	@property
 	def minimum(self):
 		"""minimum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_minimum'):
-			from .MsPower_.Minimum import Minimum
-			self._minimum = Minimum(self._core, self._base)
+			from .Minimum import MinimumCls
+			self._minimum = MinimumCls(self._core, self._cmd_group)
 		return self._minimum
 
 	@property
 	def standardDev(self):
 		"""standardDev commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .MsPower_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'MsPower':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'DpPowerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = MsPower(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = DpPowerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Average.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.msPower.average.fetch() \n
-		Returns the value of the maximum spectral density at the 0-dB reference of the transmit spectrum mask for the selected
-		packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the mean power of the data part. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Maximum spectral density"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:AVERage \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.msPower.average.read() \n
-		Returns the value of the maximum spectral density at the 0-dB reference of the transmit spectrum mask for the selected
-		packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.dpower.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the mean power of the data part. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Maximum spectral density"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:AVERage?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:DPOWer:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Average.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.msPower.standardDev.fetch() \n
-		Returns the value of the maximum spectral density at the 0-dB reference of the transmit spectrum mask for the selected
-		packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.average.fetch() \n
+		Returns the y-values of the average transmit spectrum trace. See also 'Transmit Spectrum Mask square'. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Maximum spectral density"""
+			:return: ratio: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.msPower.standardDev.read() \n
-		Returns the value of the maximum spectral density at the 0-dB reference of the transmit spectrum mask for the selected
-		packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.average.read() \n
+		Returns the y-values of the average transmit spectrum trace. See also 'Transmit Spectrum Mask square'. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Maximum spectral density"""
+			:return: ratio: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:MSPower:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class PpPower:
-	"""PpPower commands group definition. 10 total commands, 5 Sub-groups, 0 group commands"""
+class PlevelCls:
+	"""Plevel commands group definition. 14 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ppPower", core, parent)
+		self._cmd_group = CommandsGroup("plevel", core, parent)
 
 	@property
 	def current(self):
-		"""current commands group. 0 Sub-classes, 2 commands."""
+		"""current commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_current'):
-			from .PpPower_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .PpPower_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def maximum(self):
-		"""maximum commands group. 0 Sub-classes, 2 commands."""
+		"""maximum commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_maximum'):
-			from .PpPower_.Maximum import Maximum
-			self._maximum = Maximum(self._core, self._base)
+			from .Maximum import MaximumCls
+			self._maximum = MaximumCls(self._core, self._cmd_group)
 		return self._maximum
 
 	@property
 	def minimum(self):
-		"""minimum commands group. 0 Sub-classes, 2 commands."""
+		"""minimum commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_minimum'):
-			from .PpPower_.Minimum import Minimum
-			self._minimum = Minimum(self._core, self._base)
+			from .Minimum import MinimumCls
+			self._minimum = MinimumCls(self._core, self._cmd_group)
 		return self._minimum
 
 	@property
 	def standardDev(self):
-		"""standardDev commands group. 0 Sub-classes, 2 commands."""
+		"""standardDev commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .PpPower_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'PpPower':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PlevelCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = PpPower(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PlevelCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Minimum.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Xvalues.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from typing import List
+
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Minimum:
-	"""Minimum commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class XvaluesCls:
+	"""Xvalues commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("minimum", core, parent)
+		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:MINimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.ppPower.minimum.fetch() \n
-		Returns the value of the preamble peak power for the selected packet number <PPDU>. \n
+	def fetch(self) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ctJitter.xvalues.fetch() \n
+		Returns the x-values of the chip time jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Preamble peak power"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:MINimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:XVALues?', suppressed)
+		return response
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:MINimum \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.ppPower.minimum.read() \n
-		Returns the value of the preamble peak power for the selected packet number <PPDU>. \n
+	def read(self) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:XVALues \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ctJitter.xvalues.read() \n
+		Returns the x-values of the chip time jitter trace. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Preamble peak power"""
+			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:MINimum?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:XVALues?', suppressed)
+		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/StandardDev.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDev:
-	"""StandardDev commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class LengthCls:
+	"""Length commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("length", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.ppPower.standardDev.fetch() \n
-		Returns the value of the preamble peak power for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.psdu.length.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the length of the PSDU. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Preamble peak power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation \n
-		Snippet: value: float = driver.uwbMeas.multiEval.power.ppPower.standardDev.read() \n
-		Returns the value of the preamble peak power for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.psdu.length.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the length of the PSDU. \n
 		Suppressed linked return values: reliability \n
-			:return: power: Preamble peak power"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation?', suppressed)
-		return Conversions.str_to_float(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ppower:
-	"""Ppower commands group definition. 10 total commands, 5 Sub-groups, 0 group commands"""
+class NrmseCls:
+	"""Nrmse commands group definition. 12 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ppower", core, parent)
+		self._cmd_group = CommandsGroup("nrmse", core, parent)
 
 	@property
 	def current(self):
-		"""current commands group. 0 Sub-classes, 2 commands."""
+		"""current commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_current'):
-			from .Ppower_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
-		"""average commands group. 0 Sub-classes, 2 commands."""
+		"""average commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_average'):
-			from .Ppower_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
-	def maximum(self):
-		"""maximum commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_maximum'):
-			from .Ppower_.Maximum import Maximum
-			self._maximum = Maximum(self._core, self._base)
-		return self._maximum
-
-	@property
-	def minimum(self):
-		"""minimum commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_minimum'):
-			from .Ppower_.Minimum import Minimum
-			self._minimum = Minimum(self._core, self._base)
-		return self._minimum
+	def extreme(self):
+		"""extreme commands group. 0 Sub-classes, 3 commands."""
+		if not hasattr(self, '_extreme'):
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
+		return self._extreme
 
 	@property
 	def standardDev(self):
-		"""standardDev commands group. 0 Sub-classes, 2 commands."""
+		"""standardDev commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_standardDev'):
-			from .Ppower_.StandardDev import StandardDev
-			self._standardDev = StandardDev(self._core, self._base)
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
 		return self._standardDev
 
-	def clone(self) -> 'Ppower':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'NrmseCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Ppower(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = NrmseCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/AsSymbols.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
-from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from .....Internal.Types import DataType
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class AsSymbols:
-	"""AsSymbols commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class CrcCls:
+	"""Crc commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("asSymbols", core, parent)
+		self._cmd_group = CommandsGroup("crc", core, parent)
 
-	def fetch(self) -> int:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.asSymbols.fetch() \n
-		Returns the number of analyzed preamble symbols that comprises the SYNC field of the SHR for the selected packet number
-		<PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> bool:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC<PPDU> \n
+		Snippet: value: bool = driver.uwbMeas.multiEval.sinfo.psdu.crc.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		No command help available \n
 		Suppressed linked return values: reliability \n
-			:return: symbols: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: crc: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols?', suppressed)
-		return Conversions.str_to_int(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_bool(response)
 
-	def read(self) -> int:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.asSymbols.read() \n
-		Returns the number of analyzed preamble symbols that comprises the SYNC field of the SHR for the selected packet number
-		<PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> bool:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC<PPDU> \n
+		Snippet: value: bool = driver.uwbMeas.multiEval.sinfo.psdu.crc.read(ppdu = repcap.Ppdu.Nr1) \n
+		No command help available \n
 		Suppressed linked return values: reliability \n
-			:return: symbols: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: crc: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:ASSYmbols?', suppressed)
-		return Conversions.str_to_int(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_bool(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Cindex.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
-from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from .....Internal.Types import DataType
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from ......Internal.Types import DataType
+from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Cindex:
-	"""Cindex commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class CrcCls:
+	"""Crc commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("cindex", core, parent)
+		self._cmd_group = CommandsGroup("crc", core, parent)
 
-	def fetch(self) -> int:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.cindex.fetch() \n
-		Returns the code index for the selected packet number <PPDU>. \n
+	# noinspection PyTypeChecker
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> enums.Result:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:CRC<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.sinfo.phr.crc.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the result of the PHR checksum (SECDED) verification. \n
 		Suppressed linked return values: reliability \n
-			:return: index: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: crc: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex?', suppressed)
-		return Conversions.str_to_int(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:CRC{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
 
-	def read(self) -> int:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.cindex.read() \n
-		Returns the code index for the selected packet number <PPDU>. \n
+	# noinspection PyTypeChecker
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> enums.Result:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:CRC<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.sinfo.phr.crc.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the result of the PHR checksum (SECDED) verification. \n
 		Suppressed linked return values: reliability \n
-			:return: index: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: crc: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex?', suppressed)
-		return Conversions.str_to_int(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:CRC{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/CsLength.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dlength.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CsLength:
-	"""CsLength commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class DlengthCls:
+	"""Dlength commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("csLength", core, parent)
+		self._cmd_group = CommandsGroup("dlength", core, parent)
 
-	def fetch(self) -> int:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.csLength.fetch() \n
-		Returns the length 31, 91 or 127 of the code sequence for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.dlength.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the oversampling factor (delta length) of the code sequence. \n
 		Suppressed linked return values: reliability \n
-			:return: cs_length: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_int(response)
 
-	def read(self) -> int:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.csLength.read() \n
-		Returns the length 31, 91 or 127 of the code sequence for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.dlength.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the oversampling factor (delta length) of the code sequence. \n
 		Suppressed linked return values: reliability \n
-			:return: cs_length: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Dlength.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/SfdLength.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dlength:
-	"""Dlength commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class SfdLengthCls:
+	"""SfdLength commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dlength", core, parent)
+		self._cmd_group = CommandsGroup("sfdLength", core, parent)
 
-	def fetch(self) -> int:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.dlength.fetch() \n
-		Returns the oversampling factor (delta length) of the code sequence to create a preamble symbol for the selected packet
-		number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:SFDLength<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.sfdLength.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the length of the SFD sequence. \n
 		Suppressed linked return values: reliability \n
-			:return: length: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: sfd_length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:SFDLength{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_int(response)
 
-	def read(self) -> int:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.dlength.read() \n
-		Returns the oversampling factor (delta length) of the code sequence to create a preamble symbol for the selected packet
-		number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:SFDLength<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.sfdLength.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the length of the SFD sequence. \n
 		Suppressed linked return values: reliability \n
-			:return: length: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: sfd_length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DLENgth?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:SFDLength{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Drate.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Drate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Drate:
-	"""Drate commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class DrateCls:
+	"""Drate commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("drate", core, parent)
+		self._cmd_group = CommandsGroup("drate", core, parent)
 
-	def fetch(self) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe \n
-		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.drate.fetch() \n
-		Returns the data rate of the received PHY payload for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.drate.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the data rate of the PHY payload. \n
 		Suppressed linked return values: reliability \n
-			:return: data_rate: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: psdu_bitrate: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
-	def read(self) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe \n
-		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.drate.read() \n
-		Returns the data rate of the received PHY payload for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.drate.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the data rate of the PHY payload. \n
 		Suppressed linked return values: reliability \n
-			:return: data_rate: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: psdu_bitrate: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:DRATe{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Phr:
-	"""Phr commands group definition. 2 total commands, 1 Sub-groups, 0 group commands"""
+class TsMaskCls:
+	"""TsMask commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("phr", core, parent)
+		self._cmd_group = CommandsGroup("tsMask", core, parent)
 
 	@property
-	def crc(self):
-		"""crc commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_crc'):
-			from .Phr_.Crc import Crc
-			self._crc = Crc(self._core, self._base)
-		return self._crc
+	def limit(self):
+		"""limit commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_limit'):
+			from .Limit import LimitCls
+			self._limit = LimitCls(self._core, self._cmd_group)
+		return self._limit
 
-	def clone(self) -> 'Phr':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'TsMaskCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Phr(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = TsMaskCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Psdu:
-	"""Psdu commands group definition. 4 total commands, 2 Sub-groups, 0 group commands"""
+class PhrCls:
+	"""Phr commands group definition. 6 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("psdu", core, parent)
-
-	@property
-	def length(self):
-		"""length commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_length'):
-			from .Psdu_.Length import Length
-			self._length = Length(self._core, self._base)
-		return self._length
+		self._cmd_group = CommandsGroup("phr", core, parent)
 
 	@property
 	def crc(self):
 		"""crc commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_crc'):
-			from .Psdu_.Crc import Crc
-			self._crc = Crc(self._core, self._base)
+			from .Crc import CrcCls
+			self._crc = CrcCls(self._core, self._cmd_group)
 		return self._crc
 
-	def clone(self) -> 'Psdu':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def asSymbols(self):
+		"""asSymbols commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_asSymbols'):
+			from .AsSymbols import AsSymbolsCls
+			self._asSymbols = AsSymbolsCls(self._core, self._cmd_group)
+		return self._asSymbols
+
+	@property
+	def bitrate(self):
+		"""bitrate commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_bitrate'):
+			from .Bitrate import BitrateCls
+			self._bitrate = BitrateCls(self._core, self._cmd_group)
+		return self._bitrate
+
+	def clone(self) -> 'PhrCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Psdu(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PhrCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/Crc.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Cindex.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Crc:
-	"""Crc commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class CindexCls:
+	"""Cindex commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("crc", core, parent)
+		self._cmd_group = CommandsGroup("cindex", core, parent)
 
-	def fetch(self) -> bool:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC \n
-		Snippet: value: bool = driver.uwbMeas.multiEval.sinfo.psdu.crc.fetch() \n
-		No command help available \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.cindex.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the code index. \n
 		Suppressed linked return values: reliability \n
-			:return: crc: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: index: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC?', suppressed)
-		return Conversions.str_to_bool(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> bool:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC \n
-		Snippet: value: bool = driver.uwbMeas.multiEval.sinfo.psdu.crc.read() \n
-		No command help available \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.cindex.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the code index. \n
 		Suppressed linked return values: reliability \n
-			:return: crc: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: index: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:CRC?', suppressed)
-		return Conversions.str_to_bool(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CINDex{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/Length.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Length:
-	"""Length commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class MaximumCls:
+	"""Maximum commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("length", core, parent)
+		self._cmd_group = CommandsGroup("maximum", core, parent)
 
-	def fetch(self) -> int:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.psdu.length.fetch() \n
-		Returns the length of the PSDU for the selected packet number <PPDU>. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MAXimum<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppower.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the mean power of the preamble part. \n
 		Suppressed linked return values: reliability \n
-			:return: length: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth?', suppressed)
-		return Conversions.str_to_int(response)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MAXimum{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
 
-	def read(self) -> int:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth \n
-		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.psdu.length.read() \n
-		Returns the length of the PSDU for the selected packet number <PPDU>. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MAXimum<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppower.maximum.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the mean power of the preamble part. \n
 		Suppressed linked return values: reliability \n
-			:return: length: No help available"""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PSDU:LENGth?', suppressed)
-		return Conversions.str_to_int(response)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPOWer:MAXimum{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,99 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Trace:
-	"""Trace commands group definition. 42 total commands, 7 Sub-groups, 0 group commands"""
+class LimitCls:
+	"""Limit commands group definition. 10 total commands, 10 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("trace", core, parent)
+		self._cmd_group = CommandsGroup("limit", core, parent)
 
 	@property
-	def ncCorr(self):
-		"""ncCorr commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ncCorr'):
-			from .Trace_.NcCorr import NcCorr
-			self._ncCorr = NcCorr(self._core, self._base)
-		return self._ncCorr
-
-	@property
-	def tsMask(self):
-		"""tsMask commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_tsMask'):
-			from .Trace_.TsMask import TsMask
-			self._tsMask = TsMask(self._core, self._base)
-		return self._tsMask
-
-	@property
-	def stJitter(self):
-		"""stJitter commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_stJitter'):
-			from .Trace_.StJitter import StJitter
-			self._stJitter = StJitter(self._core, self._base)
-		return self._stJitter
-
-	@property
-	def spJitter(self):
-		"""spJitter commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_spJitter'):
-			from .Trace_.SpJitter import SpJitter
-			self._spJitter = SpJitter(self._core, self._base)
-		return self._spJitter
-
-	@property
-	def ctJitter(self):
-		"""ctJitter commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ctJitter'):
-			from .Trace_.CtJitter import CtJitter
-			self._ctJitter = CtJitter(self._core, self._base)
-		return self._ctJitter
-
-	@property
-	def cpJitter(self):
-		"""cpJitter commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_cpJitter'):
-			from .Trace_.CpJitter import CpJitter
-			self._cpJitter = CpJitter(self._core, self._base)
-		return self._cpJitter
-
-	@property
-	def powerVsTime(self):
-		"""powerVsTime commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_powerVsTime'):
-			from .Trace_.PowerVsTime import PowerVsTime
-			self._powerVsTime = PowerVsTime(self._core, self._base)
-		return self._powerVsTime
+	def foffset(self):
+		"""foffset commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_foffset'):
+			from .Foffset import FoffsetCls
+			self._foffset = FoffsetCls(self._core, self._cmd_group)
+		return self._foffset
+
+	@property
+	def ccError(self):
+		"""ccError commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ccError'):
+			from .CcError import CcErrorCls
+			self._ccError = CcErrorCls(self._core, self._cmd_group)
+		return self._ccError
+
+	@property
+	def smAccuracy(self):
+		"""smAccuracy commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_smAccuracy'):
+			from .SmAccuracy import SmAccuracyCls
+			self._smAccuracy = SmAccuracyCls(self._core, self._cmd_group)
+		return self._smAccuracy
+
+	@property
+	def slPeak(self):
+		"""slPeak commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_slPeak'):
+			from .SlPeak import SlPeakCls
+			self._slPeak = SlPeakCls(self._core, self._cmd_group)
+		return self._slPeak
+
+	@property
+	def pmlWidth(self):
+		"""pmlWidth commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_pmlWidth'):
+			from .PmlWidth import PmlWidthCls
+			self._pmlWidth = PmlWidthCls(self._core, self._cmd_group)
+		return self._pmlWidth
+
+	@property
+	def shr(self):
+		"""shr commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_shr'):
+			from .Shr import ShrCls
+			self._shr = ShrCls(self._core, self._cmd_group)
+		return self._shr
+
+	@property
+	def phr(self):
+		"""phr commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_phr'):
+			from .Phr import PhrCls
+			self._phr = PhrCls(self._core, self._cmd_group)
+		return self._phr
+
+	@property
+	def psdu(self):
+		"""psdu commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_psdu'):
+			from .Psdu import PsduCls
+			self._psdu = PsduCls(self._core, self._cmd_group)
+		return self._psdu
+
+	@property
+	def sts(self):
+		"""sts commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_sts'):
+			from .Sts import StsCls
+			self._sts = StsCls(self._core, self._cmd_group)
+		return self._sts
+
+	@property
+	def plevel(self):
+		"""plevel commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_plevel'):
+			from .Plevel import PlevelCls
+			self._plevel = PlevelCls(self._core, self._cmd_group)
+		return self._plevel
 
-	def clone(self) -> 'Trace':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'LimitCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Trace(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = LimitCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CpJitter:
-	"""CpJitter commands group definition. 6 total commands, 3 Sub-groups, 0 group commands"""
+class SbwsCls:
+	"""Sbws commands group definition. 6 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("cpJitter", core, parent)
+		self._cmd_group = CommandsGroup("sbws", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .CpJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .CpJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def xvalues(self):
 		"""xvalues commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_xvalues'):
-			from .CpJitter_.Xvalues import Xvalues
-			self._xvalues = Xvalues(self._core, self._base)
+			from .Xvalues import XvaluesCls
+			self._xvalues = XvaluesCls(self._core, self._cmd_group)
 		return self._xvalues
 
-	def clone(self) -> 'CpJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SbwsCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = CpJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SbwsCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Average.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self) -> List[float]:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.average.fetch() \n
-		Returns the values of the chip time jitter trace. The current and average values can be retrieved. See also 'Square Chip
-		Jitter'. \n
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.average.fetch() \n
+		Returns the y-values of the average normalized cross correlation trace. See also 'Normalized Cross Correlation square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Comma-separated list of chip jitter values."""
+			:return: correlation: Comma-separated list of cross correlation values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage?', suppressed)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage?', suppressed)
 		return response
 
 	def read(self) -> List[float]:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.average.read() \n
-		Returns the values of the chip time jitter trace. The current and average values can be retrieved. See also 'Square Chip
-		Jitter'. \n
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.average.read() \n
+		Returns the y-values of the average normalized cross correlation trace. See also 'Normalized Cross Correlation square'. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Comma-separated list of chip jitter values."""
+			:return: correlation: Comma-separated list of cross correlation values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:AVERage?', suppressed)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Xvalues.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Maximum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from typing import List
 
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Xvalues:
-	"""Xvalues commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class MaximumCls:
+	"""Maximum commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("xvalues", core, parent)
+		self._cmd_group = CommandsGroup("maximum", core, parent)
 
-	def fetch(self) -> List[float]:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.xvalues.fetch() \n
-		Returns the x-values of the chip time jitter trace. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> List[float]:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:MAXimum<PPDU> \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.powerVsTime.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the y-values of the power vs time trace. The minimum and maximum values can be retrieved. See also 'Power vs Time
+		square'. \n
 		Suppressed linked return values: reliability \n
-			:return: values: Comma-separated list of phase values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: Comma-separated list of power values."""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues?', suppressed)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:MAXimum{ppdu_cmd_val}?', suppressed)
 		return response
 
-	def read(self) -> List[float]:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.cpJitter.xvalues.read() \n
-		Returns the x-values of the chip time jitter trace. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> List[float]:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:MAXimum<PPDU> \n
+		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.powerVsTime.maximum.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the y-values of the power vs time trace. The minimum and maximum values can be retrieved. See also 'Power vs Time
+		square'. \n
 		Suppressed linked return values: reliability \n
-			:return: values: Comma-separated list of phase values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: Comma-separated list of power values."""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CPJitter:XVALues?', suppressed)
+		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:PVTime:MAXimum{ppdu_cmd_val}?', suppressed)
 		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CtJitter:
-	"""CtJitter commands group definition. 6 total commands, 3 Sub-groups, 0 group commands"""
+class SpJitterCls:
+	"""SpJitter commands group definition. 6 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ctJitter", core, parent)
+		self._cmd_group = CommandsGroup("spJitter", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .CtJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .CtJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
 	def xvalues(self):
 		"""xvalues commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_xvalues'):
-			from .CtJitter_.Xvalues import Xvalues
-			self._xvalues = Xvalues(self._core, self._base)
+			from .Xvalues import XvaluesCls
+			self._xvalues = XvaluesCls(self._core, self._cmd_group)
 		return self._xvalues
 
-	def clone(self) -> 'CtJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SpJitterCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = CtJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SpJitterCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Average.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from typing import List
-
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
-	def fetch(self) -> List[float]:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ctJitter.average.fetch() \n
-		Returns the values of the chip time jitter trace. The current and average values can be retrieved. See also 'Square Chip
-		Jitter'. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Comma-separated list of chip jitter values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
 
-	def read(self) -> List[float]:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ctJitter.average.read() \n
-		Returns the values of the chip time jitter trace. The current and average values can be retrieved. See also 'Square Chip
-		Jitter'. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.spJitter.average.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the RMS phase jitter value averaged over the detected preamble symbols. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Comma-separated list of chip jitter values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: jitter: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:CTJitter:AVERage?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SPJitter:AVERage{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ........Internal.Core import Core
+from ........Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class NcCorr:
-	"""NcCorr commands group definition. 6 total commands, 3 Sub-groups, 0 group commands"""
+class PositivCls:
+	"""Positiv commands group definition. 4 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ncCorr", core, parent)
+		self._cmd_group = CommandsGroup("positiv", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .NcCorr_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .NcCorr_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
-	@property
-	def xvalues(self):
-		"""xvalues commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_xvalues'):
-			from .NcCorr_.Xvalues import Xvalues
-			self._xvalues = Xvalues(self._core, self._base)
-		return self._xvalues
-
-	def clone(self) -> 'NcCorr':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PositivCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = NcCorr(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PositivCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class PowerVsTime:
-	"""PowerVsTime commands group definition. 6 total commands, 3 Sub-groups, 0 group commands"""
+class PowerVsTimeCls:
+	"""PowerVsTime commands group definition. 6 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("powerVsTime", core, parent)
+		self._cmd_group = CommandsGroup("powerVsTime", core, parent)
 
 	@property
 	def minimum(self):
 		"""minimum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_minimum'):
-			from .PowerVsTime_.Minimum import Minimum
-			self._minimum = Minimum(self._core, self._base)
+			from .Minimum import MinimumCls
+			self._minimum = MinimumCls(self._core, self._cmd_group)
 		return self._minimum
 
 	@property
 	def maximum(self):
 		"""maximum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_maximum'):
-			from .PowerVsTime_.Maximum import Maximum
-			self._maximum = Maximum(self._core, self._base)
+			from .Maximum import MaximumCls
+			self._maximum = MaximumCls(self._core, self._cmd_group)
 		return self._maximum
 
 	@property
 	def xvalues(self):
 		"""xvalues commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_xvalues'):
-			from .PowerVsTime_.Xvalues import Xvalues
-			self._xvalues = Xvalues(self._core, self._base)
+			from .Xvalues import XvaluesCls
+			self._xvalues = XvaluesCls(self._core, self._cmd_group)
 		return self._xvalues
 
-	def clone(self) -> 'PowerVsTime':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PowerVsTimeCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = PowerVsTime(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PowerVsTimeCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ........Internal.Core import Core
+from ........Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SpJitter:
-	"""SpJitter commands group definition. 6 total commands, 3 Sub-groups, 0 group commands"""
+class NegativCls:
+	"""Negativ commands group definition. 4 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("spJitter", core, parent)
+		self._cmd_group = CommandsGroup("negativ", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .SpJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .SpJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
-	@property
-	def xvalues(self):
-		"""xvalues commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_xvalues'):
-			from .SpJitter_.Xvalues import Xvalues
-			self._xvalues = Xvalues(self._core, self._base)
-		return self._xvalues
-
-	def clone(self) -> 'SpJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'NegativCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = SpJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = NegativCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,51 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StJitter:
-	"""StJitter commands group definition. 6 total commands, 3 Sub-groups, 0 group commands"""
+class RmarkerCls:
+	"""Rmarker commands group definition. 8 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("stJitter", core, parent)
+		self._cmd_group = CommandsGroup("rmarker", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .StJitter_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .StJitter_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
 	@property
-	def xvalues(self):
-		"""xvalues commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_xvalues'):
-			from .StJitter_.Xvalues import Xvalues
-			self._xvalues = Xvalues(self._core, self._base)
-		return self._xvalues
+	def extreme(self):
+		"""extreme commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_extreme'):
+			from .Extreme import ExtremeCls
+			self._extreme = ExtremeCls(self._core, self._cmd_group)
+		return self._extreme
 
-	def clone(self) -> 'StJitter':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def standardDev(self):
+		"""standardDev commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_standardDev'):
+			from .StandardDev import StandardDevCls
+			self._standardDev = StandardDevCls(self._core, self._cmd_group)
+		return self._standardDev
+
+	def clone(self) -> 'RmarkerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = StJitter(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = RmarkerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/CsLength.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from typing import List
-
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class CsLengthCls:
+	"""CsLength commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("csLength", core, parent)
 
-	def fetch(self) -> List[float]:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:CURRent \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.stJitter.current.fetch() \n
-		Returns the values of the symbol time jitter trace. The current and average values can be retrieved. See also 'Square
-		Symbol Jitter'. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.csLength.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the length of the code sequence. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Comma-separated list of symbol jitter values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: cs_length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:CURRent?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> List[float]:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:CURRent \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.stJitter.current.read() \n
-		Returns the values of the symbol time jitter trace. The current and average values can be retrieved. See also 'Square
-		Symbol Jitter'. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.csLength.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the length of the code sequence. \n
 		Suppressed linked return values: reliability \n
-			:return: jitter: Comma-separated list of symbol jitter values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: cs_length: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:STJitter:CURRent?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:CSLength{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class TsMask:
-	"""TsMask commands group definition. 6 total commands, 3 Sub-groups, 0 group commands"""
+class PmaskCls:
+	"""Pmask commands group definition. 4 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("tsMask", core, parent)
+		self._cmd_group = CommandsGroup("pmask", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .TsMask_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
-	def average(self):
-		"""average commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_average'):
-			from .TsMask_.Average import Average
-			self._average = Average(self._core, self._base)
-		return self._average
-
-	@property
 	def xvalues(self):
 		"""xvalues commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_xvalues'):
-			from .TsMask_.Xvalues import Xvalues
-			self._xvalues = Xvalues(self._core, self._base)
+			from .Xvalues import XvaluesCls
+			self._xvalues = XvaluesCls(self._core, self._cmd_group)
 		return self._xvalues
 
-	def clone(self) -> 'TsMask':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PmaskCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = TsMask(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PmaskCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/ReBit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from typing import List
-
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .....Internal.Types import DataType
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ReBitCls:
+	"""ReBit commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("reBit", core, parent)
 
-	def fetch(self) -> List[float]:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.average.fetch() \n
-		Returns the values of the transmit spectrum trace. The current and average values can be retrieved. See also 'Square
-		Transmit Spectrum Mask'. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:REBit<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.reBit.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the decoded reserved bit of the PHR. \n
 		Suppressed linked return values: reliability \n
-			:return: ratio: Comma-separated list of transmit spectrum values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: reserved_bit: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:REBit{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
 
-	def read(self) -> List[float]:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.average.read() \n
-		Returns the values of the transmit spectrum trace. The current and average values can be retrieved. See also 'Square
-		Transmit Spectrum Mask'. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> int:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:REBit<PPDU> \n
+		Snippet: value: int = driver.uwbMeas.multiEval.sinfo.reBit.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the decoded reserved bit of the PHR. \n
 		Suppressed linked return values: reliability \n
-			:return: ratio: Comma-separated list of transmit spectrum values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: reserved_bit: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:REBit{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from typing import List
-
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
 from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ......Internal.Types import DataType
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
-	def fetch(self) -> List[float]:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.current.fetch() \n
-		Returns the values of the transmit spectrum trace. The current and average values can be retrieved. See also 'Square
-		Transmit Spectrum Mask'. \n
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppPower.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the peak power of the preamble part. \n
 		Suppressed linked return values: reliability \n
-			:return: ratio: Comma-separated list of transmit spectrum values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
 
-	def read(self) -> List[float]:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent \n
-		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.current.read() \n
-		Returns the values of the transmit spectrum trace. The current and average values can be retrieved. See also 'Square
-		Transmit Spectrum Mask'. \n
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppPower.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
+		Returns the peak power of the preamble part. \n
 		Suppressed linked return values: reliability \n
-			:return: ratio: Comma-separated list of transmit spectrum values."""
+			:param ppdu: optional repeated capability selector. Default value: Nr1
+			:return: power: No help available"""
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent?', suppressed)
-		return response
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPPower:SDEViation{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ........Internal.Core import Core
+from ........Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class TsMask:
-	"""TsMask commands group definition. 8 total commands, 1 Sub-groups, 0 group commands"""
+class UpperCls:
+	"""Upper commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("tsMask", core, parent)
+		self._cmd_group = CommandsGroup("upper", core, parent)
 
 	@property
-	def margin(self):
-		"""margin commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_margin'):
-			from .TsMask_.Margin import Margin
-			self._margin = Margin(self._core, self._base)
-		return self._margin
+	def area(self):
+		"""area commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_area'):
+			from .Area import AreaCls
+			self._area = AreaCls(self._core, self._cmd_group)
+		return self._area
 
-	def clone(self) -> 'TsMask':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'UpperCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = TsMask(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UpperCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Margin:
-	"""Margin commands group definition. 8 total commands, 1 Sub-groups, 0 group commands"""
+class MarginCls:
+	"""Margin commands group definition. 10 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("margin", core, parent)
+		self._cmd_group = CommandsGroup("margin", core, parent)
 
 	@property
 	def area(self):
-		"""area commands group. 2 Sub-classes, 0 commands."""
+		"""area commands group. 4 Sub-classes, 0 commands."""
 		if not hasattr(self, '_area'):
-			from .Margin_.Area import Area
-			self._area = Area(self._core, self._base)
+			from .Area import AreaCls
+			self._area = AreaCls(self._core, self._cmd_group)
 		return self._area
 
-	def clone(self) -> 'Margin':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MarginCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Margin(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MarginCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,42 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.RepeatedCapability import RepeatedCapability
-from ...... import repcap
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal.RepeatedCapability import RepeatedCapability
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Area:
-	"""Area commands group definition. 8 total commands, 2 Sub-groups, 0 group commands
+class AreaCls:
+	"""Area commands group definition. 2 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: Area, default value after init: Area.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("area", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_area_get', 'repcap_area_set', repcap.Area.Nr1)
+		self._cmd_group = CommandsGroup("area", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_area_get', 'repcap_area_set', repcap.Area.Nr1)
 
-	def repcap_area_set(self, enum_value: repcap.Area) -> None:
+	def repcap_area_set(self, area: repcap.Area) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Area.Default
 		Default value after init: Area.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(area)
 
 	def repcap_area_get(self) -> repcap.Area:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
-	def negativ(self):
-		"""negativ commands group. 2 Sub-classes, 0 commands."""
-		if not hasattr(self, '_negativ'):
-			from .Area_.Negativ import Negativ
-			self._negativ = Negativ(self._core, self._base)
-		return self._negativ
+	def margin(self):
+		"""margin commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_margin'):
+			from .Margin import MarginCls
+			self._margin = MarginCls(self._core, self._cmd_group)
+		return self._margin
 
-	@property
-	def positiv(self):
-		"""positiv commands group. 2 Sub-classes, 0 commands."""
-		if not hasattr(self, '_positiv'):
-			from .Area_.Positiv import Positiv
-			self._positiv = Positiv(self._core, self._base)
-		return self._positiv
-
-	def clone(self) -> 'Area':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'AreaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Area(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = AreaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from .......Internal.Core import Core
-from .......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Negativ:
-	"""Negativ commands group definition. 4 total commands, 2 Sub-groups, 0 group commands"""
+class PsduCls:
+	"""Psdu commands group definition. 26 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("negativ", core, parent)
+		self._cmd_group = CommandsGroup("psdu", core, parent)
 
 	@property
-	def current(self):
-		"""current commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_current'):
-			from .Negativ_.Current import Current
-			self._current = Current(self._core, self._base)
-		return self._current
+	def nrmse(self):
+		"""nrmse commands group. 4 Sub-classes, 0 commands."""
+		if not hasattr(self, '_nrmse'):
+			from .Nrmse import NrmseCls
+			self._nrmse = NrmseCls(self._core, self._cmd_group)
+		return self._nrmse
 
 	@property
-	def average(self):
-		"""average commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_average'):
-			from .Negativ_.Average import Average
-			self._average = Average(self._core, self._base)
-		return self._average
+	def plevel(self):
+		"""plevel commands group. 5 Sub-classes, 0 commands."""
+		if not hasattr(self, '_plevel'):
+			from .Plevel import PlevelCls
+			self._plevel = PlevelCls(self._core, self._cmd_group)
+		return self._plevel
 
-	def clone(self) -> 'Negativ':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PsduCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Negativ(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PsduCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,52 +2,56 @@
 from ........Internal.CommandsGroup import CommandsGroup
 from ........Internal.StructBase import StructBase
 from ........Internal.ArgStruct import ArgStruct
 from ........ import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
-			- Margin_Aver_Neg_X: float: X-position of the margin for the area no
-			- Margin_Aver_Neg_Y: float: Y-value of the margin for the area no"""
+			- Reliability: int: 'Reliability indicator'
+			- Margin_Aver_Pos_X: float: X-position of the margin for the area no
+			- Margin_Aver_Pos_Y: float: Y-value of the margin for the area no"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
-			ArgStruct.scalar_float('Margin_Aver_Neg_X'),
-			ArgStruct.scalar_float('Margin_Aver_Neg_Y')]
+			ArgStruct.scalar_float('Margin_Aver_Pos_X'),
+			ArgStruct.scalar_float('Margin_Aver_Pos_Y')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
-			self.Margin_Aver_Neg_X: float = None
-			self.Margin_Aver_Neg_Y: float = None
+			self.Margin_Aver_Pos_X: float = None
+			self.Margin_Aver_Pos_Y: float = None
 
-	def fetch(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.average.fetch(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with the negative
+	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.average.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with positive
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:AVERage?', self.__class__.ResultData())
-
-	def read(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.average.read(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with the negative
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
+
+	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.average.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with positive
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:AVERage?', self.__class__.ResultData())
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/Margin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-from ........Internal.Core import Core
-from ........Internal.CommandsGroup import CommandsGroup
-from ........Internal.StructBase import StructBase
-from ........Internal.ArgStruct import ArgStruct
-from ........ import repcap
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal.StructBase import StructBase
+from .......Internal.ArgStruct import ArgStruct
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class MarginCls:
+	"""Margin commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("margin", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
-			- Margin_Curr_Neg_X: float: No parameter help available
-			- Margin_Curr_Neg_Y: float: No parameter help available"""
+			- Reliability: int: 'Reliability indicator'
+			- Margin_Lower_X: float: X-position of the margin for the lower area no
+			- Margin_Lower_Y: float: Y-value of the margin for the lower area no"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
-			ArgStruct.scalar_float('Margin_Curr_Neg_X'),
-			ArgStruct.scalar_float('Margin_Curr_Neg_Y')]
+			ArgStruct.scalar_float('Margin_Lower_X'),
+			ArgStruct.scalar_float('Margin_Lower_Y')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
-			self.Margin_Curr_Neg_X: float = None
-			self.Margin_Curr_Neg_Y: float = None
+			self.Margin_Lower_X: float = None
+			self.Margin_Lower_Y: float = None
 
-	def fetch(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.current.fetch(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with the negative
-		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:LOWer:AREA<nr>:MARGin<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.pmask.lower.area.margin.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the transmitted pulse trace and the pulse mask for the lower area <no>. A negative
+		margin indicates that the trace is located below the limit line, i.e. the limit is exceeded. See also 'Pulse Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:CURRent?', self.__class__.ResultData())
-
-	def read(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.current.read(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with the negative
-		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:LOWer:AREA{area_cmd_val}:MARGin{ppdu_cmd_val}?', self.__class__.ResultData())
+
+	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:PMASk:LOWer:AREA<nr>:MARGin<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.pmask.lower.area.margin.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the transmitted pulse trace and the pulse mask for the lower area <no>. A negative
+		margin indicates that the trace is located below the limit line, i.e. the limit is exceeded. See also 'Pulse Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:CURRent?', self.__class__.ResultData())
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:PMASk:LOWer:AREA{area_cmd_val}:MARGin{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-from .......Internal.Core import Core
-from .......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Positiv:
-	"""Positiv commands group definition. 4 total commands, 2 Sub-groups, 0 group commands"""
+class CpJitterCls:
+	"""CpJitter commands group definition. 6 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("positiv", core, parent)
+		self._cmd_group = CommandsGroup("cpJitter", core, parent)
 
 	@property
 	def current(self):
 		"""current commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_current'):
-			from .Positiv_.Current import Current
-			self._current = Current(self._core, self._base)
+			from .Current import CurrentCls
+			self._current = CurrentCls(self._core, self._cmd_group)
 		return self._current
 
 	@property
 	def average(self):
 		"""average commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_average'):
-			from .Positiv_.Average import Average
-			self._average = Average(self._core, self._base)
+			from .Average import AverageCls
+			self._average = AverageCls(self._core, self._cmd_group)
 		return self._average
 
-	def clone(self) -> 'Positiv':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def xvalues(self):
+		"""xvalues commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_xvalues'):
+			from .Xvalues import XvaluesCls
+			self._xvalues = XvaluesCls(self._core, self._cmd_group)
+		return self._xvalues
+
+	def clone(self) -> 'CpJitterCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Positiv(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CpJitterCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/Average.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,52 +2,56 @@
 from ........Internal.CommandsGroup import CommandsGroup
 from ........Internal.StructBase import StructBase
 from ........Internal.ArgStruct import ArgStruct
 from ........ import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Average:
-	"""Average commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class AverageCls:
+	"""Average commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
-			- Margin_Aver_Pos_X: float: X-position of the margin for the area no
-			- Margin_Aver_Pos_Y: float: Y-value of the margin for the area no"""
+			- Reliability: int: 'Reliability indicator'
+			- Margin_Aver_Neg_X: float: X-position of the margin for the area no
+			- Margin_Aver_Neg_Y: float: Y-value of the margin for the area no"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
-			ArgStruct.scalar_float('Margin_Aver_Pos_X'),
-			ArgStruct.scalar_float('Margin_Aver_Pos_Y')]
+			ArgStruct.scalar_float('Margin_Aver_Neg_X'),
+			ArgStruct.scalar_float('Margin_Aver_Neg_Y')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
-			self.Margin_Aver_Pos_X: float = None
-			self.Margin_Aver_Pos_Y: float = None
+			self.Margin_Aver_Neg_X: float = None
+			self.Margin_Aver_Neg_Y: float = None
 
-	def fetch(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.average.fetch(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with positive
+	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.average.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with negative
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:AVERage?', self.__class__.ResultData())
-
-	def read(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:AVERage \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.average.read(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with positive
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
+
+	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:AVERage<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.average.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with negative
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:AVERage?', self.__class__.ResultData())
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/Current.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/Margin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-from ........Internal.Core import Core
-from ........Internal.CommandsGroup import CommandsGroup
-from ........Internal.StructBase import StructBase
-from ........Internal.ArgStruct import ArgStruct
-from ........ import repcap
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal.StructBase import StructBase
+from .......Internal.ArgStruct import ArgStruct
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class MarginCls:
+	"""Margin commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("margin", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
-			- Reliability: int: 'Reliability Indicator'
-			- Margin_Curr_Pos_X: float: No parameter help available
-			- Margin_Curr_Pos_Y: float: No parameter help available"""
+			- Reliability: int: 'Reliability indicator'
+			- Margin_Lower_X: float: X-position of the margin for the upper area no
+			- Margin_Lower_Y: float: Y-value of the margin for the upper area no"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
-			ArgStruct.scalar_float('Margin_Curr_Pos_X'),
-			ArgStruct.scalar_float('Margin_Curr_Pos_Y')]
+			ArgStruct.scalar_float('Margin_Lower_X'),
+			ArgStruct.scalar_float('Margin_Lower_Y')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
-			self.Margin_Curr_Pos_X: float = None
-			self.Margin_Curr_Pos_Y: float = None
+			self.Margin_Lower_X: float = None
+			self.Margin_Lower_Y: float = None
 
-	def fetch(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.current.fetch(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with positive
-		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:UPPer:AREA<nr>:MARGin<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.pmask.upper.area.margin.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the transmitted pulse trace and the pulse mask for the upper area <no>. A negative
+		margin indicates that the trace is located above the limit line, i.e. the limit is exceeded. See also 'Pulse Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:CURRent?', self.__class__.ResultData())
-
-	def read(self, area=repcap.Area.Default) -> ResultData:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:CURRent \n
-		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.current.read(area = repcap.Area.Default) \n
-		Returns the margin values between the result trace and the transmission spectrum mask for the area <no> with positive
-		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Square Transmit Spectrum Mask'. \n
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:UPPer:AREA{area_cmd_val}:MARGin{ppdu_cmd_val}?', self.__class__.ResultData())
+
+	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:PMASk:UPPer:AREA<nr>:MARGin<PPDU> \n
+		Snippet: value: ResultData = driver.uwbMeas.multiEval.pmask.upper.area.margin.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
+		Returns the margin values between the transmitted pulse trace and the pulse mask for the upper area <no>. A negative
+		margin indicates that the trace is located above the limit line, i.e. the limit is exceeded. See also 'Pulse Mask square'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
-		area_cmd_val = self._base.get_repcap_cmd_value(area, repcap.Area)
-		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:CURRent?', self.__class__.ResultData())
+		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:PMASk:UPPer:AREA{area_cmd_val}:MARGin{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Class defining Linked argument Event."""
+
 import time
 
 
 class ArgLinkedEventArgs(object):
 	"""Contains event data for suppressed argument."""
 
 	def __init__(self, link_name: str, arg_name: str, value: object = None, context: str = '', timestamp: time = None):
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgSingle.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,57 @@
+"""Single argument definition for a scalar argument."""
+
 from .ConverterFromScpiString import ConverterFromScpiString
 from .ConverterToScpiString import ConverterToScpiString
+from .InstrumentErrors import RsInstrException
+
 from .Types import DataType
 
 
 class ArgSingle(object):
 	"""Single Argument outside a structure - used for composing query arguments.
 	Contains the argument value as well (self.value)."""
 
-	def __init__(self, name: str, value, data_type: DataType, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
+	def __init__(self, name: str, value, data_type: DataType, enum_type=None, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
 		self.name = name if name else ''
 		self.argument_ix = None
 		self.value = value
 		self.data_type = data_type
+		self.enum_type = enum_type
 		self.is_optional = is_optional
 		self.is_open_list = is_open_list
 		self.repetition = repetition
 		self.intern_link = intern_link
 		self.conv_from_scpi_string = None
 		self.conv_to_scpi_string = None
 
-		if self.data_type == DataType.Enum:
-			self.assert_mandatory_has_value(self)
-			if self.value is not None:
-				self.enum_type = type(self.value)
-				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-		elif self.data_type == DataType.EnumList:
-			self.assert_mandatory_has_value(self)
+		if self.data_type.is_scalar_enum:
+			# self.assert_mandatory_has_value(self)
+			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+			self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+		elif self.data_type.is_list_enum:
+			# self.assert_mandatory_has_value(self)
 			if self.value is not None:
-				self.enum_type = type(self.value[0])
 				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
 				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
 		else:
 			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type)
 			self.conv_to_scpi_string = ConverterToScpiString(self.data_type)
 
 		self.check_consistency()
 
 	@classmethod
-	def as_open_list(cls, name: str, value: object, data_type: DataType) -> 'ArgSingle':
+	def as_open_list(cls, name: str, value: object, data_type: DataType, enum_type=None) -> 'ArgSingle':
 		"""Creates new ArgSingle of open list type.Use this method for all non-interleaved list types. \n
-		:param name: name of the argument.
-		:param value: value of the argument.
-		:param data_type: data type of the argument.
-		:return: ArgSingle object of an open list type."""
-		return cls(name, value, data_type, False, True, 1, None)
+		:param name: name of the argument
+		:param value: value of the argument
+		:param data_type: data type of the argument
+		:param enum_type: enum type if the data_type is Enum or EnumExt (or list of those)
+		:return: ArgSingle object of an open list type"""
+		return cls(name, value, data_type, enum_type, False, True, 1, None)
 
 	def __str__(self):
 		opt = '~' if self.is_optional else ''
 		name = f" '{self.name}'" if self.name != '' else ''
 		out = f"SingleArg {opt}{self.data_type.name}{name}"
 
 		if self.is_open_list is False and self.repetition > 1:
@@ -72,15 +75,15 @@
 
 	# noinspection PyUnusedLocal
 	def assert_is_optional(self, obj=None) -> None:
 		"""Asserts that the parameter is optional.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
-		raise Exception(f'Single argument is not optional: {self}')
+		raise RsInstrException(f'Single argument is not optional: {self}')
 
 	# noinspection PyUnusedLocal
 	def assert_mandatory_has_value(self, value_obj=None) -> None:
 		"""Asserts that if the parameter is mandatory, it must have value assigned.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
@@ -93,11 +96,11 @@
 
 	def check_consistency(self) -> None:
 		"""Checks the consistency of the object"""
 		if self.value is None:
 			return
 		if isinstance(self.value, list):
 			if self.data_type.is_scalar:
-				raise Exception(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
+				raise RsInstrException(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
 		else:
 			if self.data_type.is_list:
-				raise Exception(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
+				raise RsInstrException(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgSingleList.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleList.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Single argument definition for a list argument."""
+
 from .ArgSingle import ArgSingle
 from .ArgStringComposer import compose_cmd_string_from_single_args
 
 
 class ArgSingleList(object):
 	"""Contains methods for composing cmd string for the list of single arguments.
 	Used in methods with 1+ set or query arguments.
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Contains definition for an argument that is suppressed and not exposed to the user.
+Usually such arguments are also linked to a callback."""
+
 from .Types import DataType
 
 
 class ArgSingleSuppressed(object):
 	"""Single suppressed Argument - used in Query_XxXx_Suppressed() to remove it from the returned value.
 	It does not contain:
 	- 'value' attribute, since this is discarded or linked internally directly  in the Query_XxXx_Suppressed().
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStringComposer.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStringComposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 The composing of the SCPI parameter string is similar for the ArgStruct and ArgSingle[] objects, therefore they share the same module."""
 
 from typing import Dict
 
 from .ArgSingle import ArgSingle
 from .ArgStruct import ArgStruct
 from .Utilities import get_plural_string
+from .InstrumentErrors import RsInstrException
 
 
 class SingleComposer:
 	"""Composes strings for single argument.
 	Provides Composer interface with 3 functions:
 	- from_scalar_arg
 	- from_list_arg
@@ -135,15 +136,15 @@
 					# The last argument, ignore the repetitions and convert the whole list to string
 					string_arg.append(composer.from_list_arg(arg))
 				else:
 					# The optional argument, which has no value. End the entire string_arg composition
 					arg.assert_is_optional(values_obj)
 					opt_null_ix = arg_ix
 			else:
-				# More than one arguments remaining. Loop through them interleaving the result strings
+				# More than one argument remaining. Loop through them interleaving the result strings
 				# Interleaving arguments must all have values
 
 				# Check if each list has at least Repetition number of elements
 				cycles_error = False
 				alignments_error = False
 				cycle = -1
 				data = {}
@@ -151,19 +152,18 @@
 					arg = args[x]
 					curr_size: int = composer.get_arg_list_size(arg)
 					curr_cycle: int = curr_size // arg.repetition
 					curr_align: int = curr_size % arg.repetition
 					data[x] = (curr_size, curr_cycle, curr_align)
 
 					if curr_size < 0:
-						raise Exception(
-							f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
+						raise RsInstrException(f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
 
 					if arg.repetition > curr_size:
-						raise Exception(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
+						raise RsInstrException(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
 
 					# noinspection PyChainedComparisons
 					if cycle >= 0 and curr_cycle != cycle:
 						cycles_error = True
 
 					cycle = curr_cycle
 
@@ -171,23 +171,21 @@
 						alignments_error = True
 
 				if cycles_error:
 					message = 'Arguments interleaving is not aligned - all the cycles must be the same. Actual cycles:\n'
 					for x in range(arg_ix, arg_count):
 						message += f'{args[x].name}[{data[x][0]}] sliced by {get_plural_string("element", args[x].repetition)} ' \
 							f'results in {data[x][0] / args[x].repetition} cycles\n'
-
-					raise Exception(message)
+					raise RsInstrException(message)
 
 				if alignments_error:
 					message = 'At least one argument has a list size not dividable by the defined repetitions:\n'
 					for x in range(arg_ix, arg_count):
 						message += f'{args[x].name}[{data[x][0]}] modulo {args[x].repetition}x results in {data[x][0] % args[x].repetition}\n'
-
-					raise Exception(message)
+					raise RsInstrException(message)
 
 				for x in range(cycle):
 					for y in range(arg_ix, arg_count):
 						arg = args[y]
 						string_arg.append(composer.from_list_arg(arg, arg.repetition * x, arg.repetition))
 
 	if opt_null_ix >= 0:
@@ -198,15 +196,15 @@
 			if arg.has_value(values_obj):
 				rest.append(arg.name)
 
 		if len(rest):
 			msg = f"Optional Argument '{args[opt_null_ix].name}' has no value, but the further ones do. " \
 				f"If you skip an optional argument, you have to skip all the ones following it. " \
 				f"Clear the values for the rest of the argument(s):\n{', '.join(rest)}"
-			raise Exception(msg)
+			raise RsInstrException(msg)
 
 	return ','.join(string_arg)
 
 
 def compose_cmd_string_from_single_args(args: Dict[int, ArgSingle]) -> str:
 	"""Returns SCPI-composed string based on the single args specification.
 	We can use the same function as for the struct arguments, with the difference of providing a SingleComposer.
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStruct.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+"""Definition for an argument which is a part of a structure."""
+
 from .ConverterFromScpiString import ConverterFromScpiString
 from .ConverterToScpiString import ConverterToScpiString
 from .Types import DataType
+from .InstrumentErrors import RsInstrException
 
 
 class ArgStruct(object):
 	"""Describes an argument in data structures.
 	This info is used to parse a string query response to the output structure,
 	or to parse the output structure to the string parameter for writing.
 	Contains reference to the value in the owning structure."""
@@ -121,17 +124,17 @@
 	def assert_is_optional(self, obj) -> None:
 		"""Asserts that the parameter is optional.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
 		value = getattr(obj, self.name)
 		if value is None:
-			raise Exception(f"Structure '{obj}', argument without value is not optional: {self}")
+			raise RsInstrException(f"Structure '{obj}', argument without value is not optional: {self}")
 		else:
-			raise Exception(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
+			raise RsInstrException(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
 
 	def assert_mandatory_has_value(self, obj) -> None:
 		"""Asserts that if the parameter is mandatory, it must have value assigned.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
 		if getattr(obj, self.name) is None:
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStructList.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+"""See the class docstring."""
+
 from .ArgStringComposer import StructComposer, compose_cmd_string_from_struct_args
 from .ArgStructStringParser import ArgStructStringParser
 from .StructBase import StructBase
+from .InstrumentErrors import RsInstrException
 
 
 class ArgStructList(object):
 	"""Contains methods for composing cmd string and parsing cmd response to the provided structure instance."""
 
 	RAW_DATA_PROP_NAME = 'RawReturnData'
 
@@ -53,22 +56,22 @@
 			# Still some args to go
 			if arg.is_open_list is True:
 				# The previous loop ended because the next argument had is_open_list True
 				if arg_ix == (arg_count - 1):
 					# This is the last argument, ignore the repetitions and take the whole rest of the elements
 					parser.to_list_value(arg, True, 0, parser.remaining, parser.remaining, 1)
 				else:
-					# More than one arguments remaining. Loop through them interleaving the result strings
+					# More than one argument remaining. Loop through them interleaving the result strings
 					open_list_args = {key: value for key, value in self.args.items() if key >= arg_ix}
 
 					# Accumulate the number of repetitions from all the open_list_args
 					period: int = sum(open_list_args[ix].repetition for ix in open_list_args)
 					reminder: int = parser.remaining % period
 					if reminder != 0:
-						raise Exception(
+						raise RsInstrException(
 							f'Arguments parsing is not aligned - source string elements remaining to parse {parser.remaining}'
 							f'is not dividable by the summary Period {period} of all the open list arguments:\n' + '\n'.join(['{}'.format(x) for x in open_list_args]))
 					# Go through the arguments and accumulate the list content
 					offset = 0
 					for x in open_list_args:
 						arg = open_list_args[x]
 						parser.to_list_value(arg, False, offset, arg.repetition, period, -1)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+"""See the class docstring."""
+
 from . import Utilities
 from .ArgStruct import ArgStruct
+from .InstrumentErrors import RsInstrException
 
 
 class ArgStructStringParser:
 	"""Class for parsing a response from the instrument to an output structure of arguments.
 	It is used by the ArgStructList class for filling structures with return values."""
 
 	def __init__(self, struct, value: str):
@@ -17,34 +20,34 @@
 		"""Remaining items to parse."""
 		return self.count - self.position
 
 	def to_scalar_value(self, arg: ArgStruct):
 		"""Parses the current element to a scalar argument."""
 		assert arg.data_type.is_scalar, f'to_scalar_value() method only works with scalar values. Data type: {arg.data_type}'
 		if self.position >= self.count:
-			raise Exception(
+			raise RsInstrException(
 				f"Cannot parse a scalar value to structure argument. Response contains only {self.count} elements, "
 				f"argument '{arg.name}' has position {self.position + 1}.\n"
 				f"Response (commas replaced by new lines):\n" + Utilities.truncate_string_from_end('\n'.join(self.elements), 1000))
 		string = self.elements[self.position]
 		value = arg.conv_from_scpi_string.get_one_element_value(string)
 		setattr(self.struct, arg.name, value)
 		self.position += 1
 
 	def to_list_value(self, arg: ArgStruct, increase_pos: bool, offset: int, count: int, period: int, cycles: int) -> None:
 		"""Parses more elements to the list argument - slicing."""
 		assert arg.data_type.is_list, f'to_list_value method only works with list values. Data type: {arg.data_type}'
 		if cycles < 0:
 			cycles = self.remaining // period
 		if self.position >= self.count:
-			raise Exception(
+			raise RsInstrException(
 				f"Cannot parse an list value to the argument '{arg.name}', "
 				f"because the element position {self.position} is over the parsed list length {self.count}")
 		if (self.position + offset + count) > self.count:
-			raise Exception(
+			raise RsInstrException(
 				f"Cannot parse the whole list value to the argument '{arg.name}', because the element position {self.position} "
 				f"plus the argument offset {offset} and argument length {count} would be over the parsed list length {self.count}")
 
 		result = []
 		for cycle in range(cycles):
 			start_ix = self.position + (cycle * period) + offset
 			for i in range(count):
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/CommandsGroup.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/CommandsGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the class docstring."""
+
 from enum import Enum
 from typing import List
 from .Core import Core
 from .RepeatedCapability import RepeatedCapability as RepCap
 from .InstrumentErrors import DriverValueError
 
 
@@ -38,27 +40,27 @@
 		return self.multi_repcap_types != ''
 
 	def add_existing_child(self, child: 'CommandsGroup') -> None:
 		"""Adds the child to the parent's list of created children.
 		This is used when the group is cloned, where the whole existing tree of groups have to be recreated"""
 		self.existing_children.append(child)
 
-	def set_repcap_enum_value(self, enum_value: Enum) -> None:
-		"""Sets RepCap value as enum
-		Default is not allowed."""
+	def set_repcap_enum_value(self, enum_value: Enum or int) -> None:
+		"""Sets RepCap value as enum or integer
+		Default is not allowed here."""
 		try:
 			self.rep_cap.set_enum_value(enum_value)
 		except ValueError:
 			raise DriverValueError(self.io.resource_name, f"Commands group RepCap value '{self.rep_cap.name}.Default' cannot be set. Please select a concrete value.")
 
 	def get_repcap_enum_value(self) -> Enum:
 		"""Returns RepCap value as enum"""
 		return self.rep_cap.get_enum_value()
 
-	def get_repcap_cmd_value(self, enum_value: Enum, enum_type) -> str:
+	def get_repcap_cmd_value(self, enum_value: Enum or int, enum_type) -> str:
 		"""Returns the current string of RepCapCmdValue for the entered RepCapEnumName
 		The enum_value can be a repcap of the current CommandsGroup or any of their parents"""
 		# Use the static functions of the RepeatedCapability to get the non-default value
 		# It is faster, since there is no need to use the RepCap instance
 		if not RepCap.clsm_is_default_value(enum_value, enum_type):
 			return RepCap.clsm_get_cmd_string_value(enum_value, enum_type)
 		# Default value - get it from the group or the parent groups
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Conversions.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Conversions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+"""Contains conversion functions for SCPI string -> parameter and vice versa."""
+
 import math
 import struct
 import sys
 from enum import Enum
-from typing import List
+from typing import List, Tuple
+from .ScpiEnums import ScpiEnum, enum_spec_prefixes, enum_spec_strings
+from datetime import datetime
 
 from . import Utilities
+from .InstrumentErrors import RsInstrException
 
 
 class BinFloatFormat(Enum):
 	"""Binary format of a float number."""
 	Single_4bytes = 1
 	Single_4bytes_swapped = 2
 	Double_8bytes = 3
@@ -24,15 +29,15 @@
 
 
 def assert_string_data(value: str) -> None:
 	"""Asserts value is string type."""
 	assert isinstance(value, str), f"Input value type must be string. Actual type: {type(value)}, value: {value}"
 
 
-def assert_list_data(value: list) -> None:
+def assert_list_data(value: List) -> None:
 	"""Asserts value is list type."""
 	assert isinstance(value, list), f"Input value type must be a list. Actual type: {type(value)}, value: {value}"
 
 
 def _get_endianness_symbol(swap_endianness: bool) -> str:
 	"""Based on the current endianness returns the symbol used in the 'struct' module."""
 	if swap_endianness is False:
@@ -143,15 +148,15 @@
 bool_true_lookup = frozenset(['1', 'on', 'On', 'ON', 'true', 'True', 'TRUE'])
 bool_false_lookup = frozenset(['0', 'off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
 pure_bool_false_lookup = frozenset(['off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
 
 
 def str_to_bool(string: str) -> bool:
 	"""Converts string to boolean value.
-	The function robust, and case insensitive.
+	The function is robust, and case-insensitive.
 	If the string can not be converted to a boolean, the function returns False."""
 	assert_string_data(string)
 	if string in bool_true_lookup:
 		return True
 	if string in bool_false_lookup:
 		return False
 	# If leading/trailing spaces
@@ -193,24 +198,33 @@
 
 
 number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
 number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
 number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
 number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
 number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
+number_si_suffix = {'pHz': 1E-12, 'MHz': 1E+6, 'kHz': 1E+3, 'GHz': 1E+9, 'mHz': 1E-3, 'uHz': 1E-6, 'µHz': 1E-6, 'THz': 1E+12, 'nHz': 1E-9, 'ns': 1E-9, 'fW': 1E-15, 'pW': 1E-12, 'nW': 1E-9, 'uW': 1E-6, 'µW': 1E-6, 'mW': 1E-3, 'kW': 1E3, 'MW': 1E6, 'GW': 1E9, 'MV': 1E+6, 'MA': 1E+6, 'ps': 1E-12, 'fs':1E-15, 'km': 1E+3, 'kV': 1E+3, 'kA': 1E+3, 'pF': 1E-2, 'Hz': 1.0, 'mm': 1E-3, 'mA': 1E-3, 'mF': 1E-3, 'mV': 1E-3, 'pV': 1E-12, 'nF': 1E-9, 'nA': 1E-9, 'nV': 1E-9, 'nm': 1E-9, 'pm': 1E-12, 'us': 1E-6, 'µs': 1E-6, 'uF': 1E-6, 'µF': 1E-6, 'ms': 1E-3, 'uA': 1E-6, 'µA': 1E-6, 'uV': 1E-6, 'µV': 1E-6, 'um': 1E-6, 'µm': 1E-6, 'pA': 1E-12, 'V': 1, 'W': 1, 'A': 1, 'F': 1, 's': 1, 'm': 1}
 int_neg_inf = -(sys.maxsize - 1)
-enum_spec_prefixes = {'_minus': '-', '_plus': '+', '_': ''}
-enum_spec_strings = {'_dash_': '-', '_dot_': '.'}
+
+
+def strip_si_suffix(string: str) -> Tuple[bool, str, float]:
+	"""Tries to find defined suffixes in the text and returns the stripped text and the multiplier as double number.
+	If no known suffix is detected, the method returns false, strippedText=text, multiplier=1.0
+	Example: text='123 MHz' strippedText='123' multiplier=1E6"""
+	for suffix in number_si_suffix.keys():
+		if string.endswith(suffix):
+			return True, string[:-len(suffix)].rstrip(), number_si_suffix[suffix]
+	return False, string, 1.0
 
 
 def str_to_int(string: str) -> int:
 	"""Converts string to integer value. Float values are coerced to integer.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	Also recognizes case-insensitive special values like NaN, INV, NCAP..."""
 	assert_string_data(string)
-	string = string.strip()
+	string = string.strip(" \t\r\n'\"")
 	if string == '':
 		return 0
 	value = str_special_values_to_int(string)
 	if value:
 		return value
 
 	# Hexadecimal numbers
@@ -232,15 +246,24 @@
 		if ',' in string:
 			return int(string[2:string.find(',')], 8)
 		else:
 			return int(string[2:], 8)
 	# Simulation
 	if string == 'Simulating':
 		return 0
-	return int(round(float(string)))
+	try:
+		return int(round(float(string)))
+	except ValueError:
+		result = strip_si_suffix(string)
+		if result[0] is False:
+			raise
+		try:
+			return int(round(float(result[1]) * result[2]))
+		except ValueError:
+			raise ValueError(f"could not convert string to integer: '{string}'")
 
 
 def str_special_values_to_int(string: str) -> int:
 	"""Converts special string values to integer. Returns None if no special value was found."""
 	assert_string_data(string)
 	if string in number_plus_inf_lookup or string in number_max_lookup:
 		return sys.maxsize
@@ -270,17 +293,17 @@
 	if result is not None:
 		return result
 	return str_to_int(string)
 
 
 def str_to_float(string: str) -> float:
 	"""Converts string to float value.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	Also recognizes case-insensitive special values like NaN, INV, NCAP..."""
 	assert_string_data(string)
-	string = string.strip()
+	string = string.strip(" \t\r\n'\"")
 	if string == '':
 		return 0.0
 	if string in number_plus_inf_lookup:
 		return math.inf
 	if string in number_minus_inf_lookup:
 		return -math.inf
 	if string in number_nan_lookup:
@@ -299,15 +322,24 @@
 		return -sys.float_info.max / 100
 	if string == 'ULEU':
 		return sys.float_info.max / 10
 	if string == 'ULEL':
 		return -sys.float_info.max / 10
 	if string == 'Simulating':
 		return 0.0
-	return float(string)
+	try:
+		return float(string)
+	except ValueError:
+		result = strip_si_suffix(string)
+		if result[0] is False:
+			raise
+		try:
+			return float(result[1]) * result[2]
+		except ValueError:
+			raise ValueError(f"could not convert string to float: '{string}'")
 
 
 def str_to_float_or_bool(string: str) -> float or bool:
 	"""Similar to str_to_float, but for special values "ON/OFF" the function returns boolean"""
 	result = string_to_pure_bool(string)
 	if result is not None:
 		return result
@@ -320,24 +352,24 @@
 
 
 def bool_to_str(value: bool) -> str:
 	"""Converts boolean to 'ON' or 'OFF' string."""
 	if type(value) is bool:
 		return 'ON' if value is True else 'OFF'
 	else:
-		raise Exception(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
+		raise RsInstrException(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
 
 
 def str_enclose_by_quotes(string: str) -> str:
 	"""Returns string enclosed by single quotes."""
 	assert_string_data(string)
 	return "'" + string + "'"
 
 
-def list_to_csv_str(value: list) -> str:
+def list_to_csv_str(value: List, delimiter: str = ',') -> str:
 	"""Converts list of elements to strings separated by commas.
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string -> string no quotes
@@ -345,18 +377,18 @@
 	assert_list_data(value)
 	result = []
 	for x in value:
 		el = value_to_str(x)
 		if not el:
 			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_str: '{x}'")
 		result.append(el)
-	return ','.join(result)
+	return delimiter.join(result)
 
 
-def list_to_csv_quoted_str(value: list) -> str:
+def list_to_csv_quoted_str(value: List) -> str:
 	"""Converts list of elements to quoted strings separated by commas.
 	Only string elements are enclosed by single quotes
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
 	- bool
 	- float
@@ -368,29 +400,28 @@
 		if isinstance(x, str):
 			el = str_enclose_by_quotes(x)
 		else:
 			el = value_to_str(x)
 		if not el:
 			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_quoted_str: '{x}'")
 		result.append(el)
-
 	return ','.join(result)
 
 
 def decimal_value_to_str(x: int or float) -> str:
 	"""Converts scalar decimal value to string.
 	Supported element types:
 	- int
 	- float"""
 	if isinstance(x, int) and type(x) is not bool:
 		return str(x)
 	elif isinstance(x, float):
 		return float_to_str(x)
 	else:
-		raise Exception(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
+		raise RsInstrException(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
 
 
 def decimal_or_bool_value_to_str(x: int or float or bool) -> str:
 	"""Converts scalar decimal value to string.
 	Supported element types:
 	- int
 	- float
@@ -398,15 +429,15 @@
 	if type(x) is bool:
 		return bool_to_str(x)
 	if isinstance(x, int):
 		return str(x)
 	elif isinstance(x, float):
 		return float_to_str(x)
 	else:
-		raise Exception(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
+		raise RsInstrException(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
 
 
 def value_to_str(x: int or bool or float or str or Enum) -> str:
 	"""Converts scalar value to string.
 	Supported element types:
 	- int
 	- bool
@@ -418,17 +449,19 @@
 	elif isinstance(x, int):
 		return str(x)
 	elif isinstance(x, float):
 		return float_to_str(x)
 	elif isinstance(x, str):
 		return x
 	elif isinstance(x, Enum):
+		if isinstance(x.value, str):
+			return enum_value_to_scpi_string(x.value)
 		return enum_value_to_scpi_string(x.name)
 	else:
-		raise Exception(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
+		raise RsInstrException(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
 
 
 def enum_value_to_scpi_string(enum_value: str) -> str:
 	"""Conversion EnumValue -> SCPI_String
 	Unescapes all the special characters that can not be contained in the enum member definition, but can be sent to the instrument as enum string.
 	Use this to send the scpi enum value to the instrument."""
 	for key in enum_spec_prefixes:
@@ -504,103 +537,158 @@
 		return []
 	result = [*map(Utilities.trim_str_response, string.split(','))]
 	if clear_one_empty_item and len(result) == 1 and result[0] == '':
 		return []
 	return result
 
 
-def _find_in_enum_members(item: str, enum_members: List[str]) -> int:
-	"""Matches a string in the provided list of member strings.
-	The item must be not fully matched.
-	The item is matched if a member string starts with the item (the item is a prefix of the member).
-	Example: item='CONN' will match the enum_member 'CONNected'
-	If the item contains a comma, only the value before comma is considered
-	Returns found index in the enum_members list"""
-	if ',' in item:
-		item = item[:item.index(',')].strip()
-	i = 0
-	for x in enum_members:
-		if x.startswith(item):
-			return i
-		i += 1
-
-	# smart matching:
-	# item = 'MAX' matches enum 'MAXpeak'
-	# item = 'SPECtrum1' matches enum 'SPEC1'
-	# item = 'SPEC' matches enum 'SPECtrum1'
-
-	item = ''.join([c for c in item if not c.islower()])
-	# item must be longer than 1 character
-	if len(item) < 2:
-		return -1
-	i = 0
-	for x in enum_members:
-		x_uc = ''.join([c for c in x if not c.islower()])
-		if x_uc == item:
-			return i
-		i += 1
-	return -1
-
-
-def str_to_scalar_enum_helper(string: str, enum_type: Enum, enum_members=None) -> Enum:
+def str_to_scalar_enum_helper(string: str, scpi_enum: ScpiEnum, array_search: bool, exc_if_not_found) -> Enum:
 	"""Converts string to one enum element.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	value = Utilities.trim_str_response(string)
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
-
-	# Search in the enum member and return the index of the matched item
-	ix = _find_in_enum_members(value, enum_members)
-	if ix >= 0:
-		# noinspection PyUnresolvedReferences
-		return enum_type[enum_members[ix]]
-
-	# If the result is -1 (not found), try to replace the special values and search again
-	# This is done to improve the performance, since most of the enums have no special values
-	enum_members_conv = [enum_value_to_scpi_string(x) for x in enum_members]
-	ix = _find_in_enum_members(value, enum_members_conv)
-	if ix >= 0:
-		# noinspection PyUnresolvedReferences
-		return enum_type[enum_members[ix]]
-
+	array_search signal no need to force the comma removing,
+	because the elements definitely do not have any commas - commas have been used to split string to the list of strings
+	The function can also return:
+	- integer special value, if the string was not found in the enum, and it is a special value.
+	- input string, if the string was not found and raise_if_not_found is set to False - used for the EnumExt types."""
+	if scpi_enum.has_quotes:
+		value = Utilities.trim_str_response(string, mode=Utilities.TrimStringMode.white_chars_double_quotes)
+	else:
+		value = Utilities.trim_str_response(string)
+	enum_value = scpi_enum.find_in_enum_members(value, False)
+	if enum_value is not None:
+		return enum_value
+	if array_search is False:
+		# If the result is still -1 (not found), try to force removing the comma in the string.
+		enum_value = scpi_enum.find_in_enum_members(value, True)
+		if enum_value is not None:
+			return enum_value
 	# If not found, search in the special integer numbers:
 	spec_value = str_special_values_to_int(value)
-	if not spec_value:
-		raise Exception(f"String '{value}' can not be found in the enum type '{enum_type}'")
+	if spec_value:
+		# noinspection PyTypeChecker
+		return spec_value
+	if exc_if_not_found:
+		raise RsInstrException(f"String '{value}' can not be found in the enum type '{scpi_enum.enum_type}'")
 	# noinspection PyTypeChecker
-	return spec_value
+	return Utilities.trim_str_response(string)
 
 
-def str_to_list_enum_helper(string: str, enum_type: Enum, enum_members=None) -> List[Enum]:
-	"""Converts string to list of enum elements.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
+def str_to_simple_scalar_enum(string: str, enum_type, case_sensitive: bool = True, ignore_underscores: bool = False) -> Enum or None:
+	"""Converts string to one enum element.
+	Does not handle special value or non-mandatory parts.
+	Function is used in core only for standard enum conversions, not for SCPI enum conversions."""
+	value = Utilities.trim_str_response(string)
+	enum_members = [x.name for x in enum_type]
+	enum_members_mod = [x.name for x in enum_type]
+	if not case_sensitive:
+		enum_members_mod = [x.upper() for x in enum_members]
+		value = value.upper()
+	if ignore_underscores:
+		enum_members_mod = [x.replace('_', '') for x in enum_members_mod]
+		value = value.replace('_', '')
+	if value in enum_members_mod:
+		return enum_type[enum_members[enum_members_mod.index(value)]]
+	return None
+
+
+def str_to_list_enum_helper(string: str, scpi_enum: ScpiEnum, exc_if_not_found: bool = True) -> List[Enum]:
+	"""Converts string to list of enum elements. separated by comma"""
 	elements = string.split(',')
-	return [str_to_scalar_enum_helper(x, enum_type, enum_members) for x in elements]
+	return [str_to_scalar_enum_helper(x, scpi_enum, True, exc_if_not_found) for x in elements]
 
 
 def enum_scalar_to_str(data, enum_type) -> str:
 	"""Converts enum scalar value to string."""
 	assert isinstance(data, enum_type), f"Expected command parameter {enum_type}, actual data type: {type(data)}. Value: {data}"
 	return value_to_str(data)
 
 
+def enum_ext_scalar_to_str(data, enum_type) -> str:
+	"""Converts enum scalar value to string.
+	If the input value is string, the function returns the string with single quotes."""
+	if isinstance(data, str):
+		# Return string with quotes
+		return value_to_quoted_str(Utilities.trim_str_response(data))
+	assert isinstance(data, enum_type), f"Expected command parameter string or {enum_type}, actual data type: {type(data)}. Value: {data}"
+	return value_to_str(data)
+
+
 def enum_list_to_str(data: List, enum_type) -> str:
 	"""Converts enum list to csv-string."""
 	# For enums, check that each element is an enum
 	assert all(isinstance(x, enum_type) for x in data), f"Expected command parameter list of {enum_type}, detected one or more elements of non-enum type. Value: {data}"
 	return list_to_csv_str(data)
 
 
+def enum_ext_list_to_str(data: List, enum_type) -> str:
+	"""Converts enum list to csv-string. Allows the elements to be either enum or string."""
+	assert all((isinstance(x, enum_type or str) or isinstance(x, str)) for x in data), f"Expected command parameter list of strings or {enum_type}, detected one or more elements of non-enum/non-string type. Value: {data}"
+	return list_to_csv_quoted_str(data)
+
+
 def str_to_scalar_enum(string: str, enum_type) -> Enum:
-	"""Converts string to one enum element."""
-	return str_to_scalar_enum_helper(string, enum_type)
+	"""Converts string to one enum element.
+	Throws exception if the string can not be converted to an enum element or a special value."""
+	return str_to_scalar_enum_helper(string, ScpiEnum(enum_type), False, exc_if_not_found=True)
+
+
+def str_to_scalar_enum_ext(string: str, enum_type) -> Enum:
+	"""Converts string to one enum element.
+	Compared to str_to_scalar_enum, in case the string can not be converted, it is returned trimmed for quotes and ."""
+	return str_to_scalar_enum_helper(string, ScpiEnum(enum_type), False, exc_if_not_found=False)
 
 
 def str_to_list_enum(string: str, enum_type) -> List[Enum]:
 	"""Converts string to list of enum elements."""
-	return str_to_list_enum_helper(string, enum_type)
+	return str_to_list_enum_helper(string, ScpiEnum(enum_type))
+
+
+def str_to_list_enum_ext(string: str, enum_type) -> List[Enum]:
+	"""Converts string to list of enum or string elements."""
+	return str_to_list_enum_helper(string, ScpiEnum(enum_type), exc_if_not_found=False)
+
+
+def convert_ts_to_datetime(timestamp: datetime or float) -> datetime:
+	"""Converts timestamp as float to datetime. For datetime tuple it just passes the value."""
+	if isinstance(timestamp, float) or isinstance(timestamp, int):
+		return datetime.fromtimestamp(timestamp)
+	return timestamp
+
+
+def get_timestamp_string(timestamp: datetime or float) -> str:
+	"""Returns the timestamp as string. The timestamp can be a datetime tuple or float seconds coming from the time.time()."""
+	timestamp = convert_ts_to_datetime(timestamp)
+	cur_time = timestamp.strftime('%H:%M:%S.%f')[:-3]
+	return cur_time
+
+
+def get_timedelta_fixed_string(time_start: datetime or float, time_end: datetime or float) -> str:
+	"""Returns the time span as string - fixed in the format of '%H:%M:%S.%f'."""
+	time_a = convert_ts_to_datetime(time_start)
+	time_b = convert_ts_to_datetime(time_end)
+	frac = (time_b - time_a).total_seconds()
+	wh = math.floor(frac)
+	d = int(wh / 86400)
+	h = int((wh - (d * 86400)) / 3600)
+	m = int((wh - (d * 86400 + h * 3600)) / 60)
+	s = int((wh - (d * 86400 + h * 3600 + m * 60)))
+	ms = int((frac - wh) * 1000)
+	res = f'{h:02d}:{m:02d}:{s:02d}.{ms:03d}'
+	if d > 0:
+		res = f'{d}d ' + res
+	return res
+
+
+def get_timedelta_string(time_a: datetime or float, time_b: datetime or float) -> str:
+	"""Returns the time span as string - dynamic based on the difference."""
+	time_a = convert_ts_to_datetime(time_a)
+	time_b = convert_ts_to_datetime(time_b)
+	if time_b < time_a:
+		return '0.000 ms'
+	diff = time_b - time_a
+	if diff.seconds < 10:
+		return f'{diff.total_seconds() * 1000:0.3f} ms'
+	elif diff.seconds < 1000:
+		a = diff.total_seconds()
+		return f'{a:0.3f} secs'
+	hours, remainder = divmod(diff.seconds, 3600)
+	minutes, seconds = divmod(remainder, 60)
+	return f'{hours:02d}:{minutes:02d}:{seconds:02d}'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+"""See the class docstring."""
+
 from enum import Enum
 
 from .Conversions import str_to_bool, str_to_int, str_to_int_or_bool, str_to_float, str_to_float_or_bool, str_to_scalar_enum_helper
 from .Conversions import str_to_str_list, str_to_bool_list, str_to_int_list, str_to_int_or_bool_list, str_to_float_list, str_to_float_or_bool_list, str_to_list_enum_helper
 from .Types import DataType
 from .Utilities import trim_str_response
+from .InstrumentErrors import RsInstrException
+from .ScpiEnums import ScpiEnum
 
 
 class ConverterFromScpiString:
 	"""Converter from SCPI response string to argument value
 	For list argument types, you must use the method get_one_element_value in a loop for each element.
 	Provides methods:
 	- get_one_element_value(str): returns one scalar value converted from the SCPI string.
 	- get_list_value(str): return complete list value converted from the SCPI string.
 	- get_value(str): calls either get_one_element_value or get_list_value() depending on the data type. \n
 	The reason for the different methods is, that sometimes the list data are interleaved with other arguments.
 	In order to parse them properly, the ArgStructStringParser module must be able to set the argument value element-by-element.
 	On the other side, the driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
 
 	def __init__(self, data_type: DataType, enum_type: Enum = None):
-		self.enum_type = enum_type
+		self.scpi_enum = None
 		self.data_type = data_type
 		self.element_type = self.data_type.element_type
 
 		if self.element_type == DataType.RawString:
 			self.converter = trim_str_response
 			self.list_converter = str_to_str_list
 
@@ -46,30 +50,30 @@
 			self.converter = str_to_float
 			self.list_converter = str_to_float_list
 
 		elif self.element_type == DataType.FloatExt:
 			self.converter = str_to_float_or_bool
 			self.list_converter = str_to_float_or_bool_list
 
-		elif self.element_type == DataType.Enum:
-			assert self.enum_type, f"For data type enum, you have to define the enum_type variable."
+		elif self.element_type.is_scalar_enum:
+			assert enum_type, f"For data type enum, you have to define the enum_type variable."
 			# noinspection PyTypeChecker
-			self.enum_members = [x.name for x in self.enum_type]
+			self.scpi_enum = ScpiEnum(enum_type)
 		else:
-			raise Exception(f"Unsupported data type '{data_type}'")
+			raise RsInstrException(f"Unsupported data type '{data_type}'")
 
 	def get_one_element_value(self, scpi_string: str):
 		"""Returns single element !!! of the argument value converted from the SCPI string (single element)"""
 		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
-		if self.element_type is DataType.Enum:
-			return str_to_scalar_enum_helper(scpi_string, self.enum_type, self.enum_members)
+		if self.element_type.is_scalar_enum:
+			return str_to_scalar_enum_helper(scpi_string, self.scpi_enum, False, exc_if_not_found=self.element_type == DataType.Enum)
 		return self.converter(scpi_string)
 
 	def get_value(self, scpi_string: str):
 		"""Returns complete value of the argument converted from the SCPI string (list or scalar)"""
 		if not self.data_type.is_list:
 			return self.get_one_element_value(scpi_string)
 
 		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
 		if self.element_type is DataType.Enum:
-			return str_to_list_enum_helper(scpi_string, self.enum_type, self.enum_members)
+			return str_to_list_enum_helper(scpi_string, self.scpi_enum, exc_if_not_found=self.element_type == DataType.Enum)
 		return self.list_converter(scpi_string)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+"""See the class docstring."""
+
 from enum import Enum
 
-from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str
+from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str, enum_ext_scalar_to_str, enum_ext_list_to_str
 from .Types import DataType
+from .InstrumentErrors import RsInstrException
 
 
 def value_to_scpi_string(data, data_type: DataType):
 	"""Method to be used in the driver implementation.
-	Convert data to SCPI string parameter: data -> str"""
+	Convert data to SCPI string parameter: data -> str.
+	Does not work with enum data types."""
 	if data_type.is_list:
 		assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
 	else:
 		assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
 	# Strings are enclosed by single quotes
 	if data_type == DataType.StringList:
 		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
@@ -46,35 +50,39 @@
 	elif data_type == DataType.IntegerExtList or data_type == DataType.FloatExtList:
 		assert all((isinstance(x, int) or isinstance(x, float) or isinstance(x, bool)) for x in data), f"Expected command parameter list of numbers or booleans, detected one or more elements of non-number type. Value: {data}"
 		return list_to_csv_str(data)
 	elif data_type == DataType.IntegerExt or data_type == DataType.FloatExt:
 		assert (isinstance(data, int) or isinstance(data, float) or isinstance(data, bool)), f"Expected command parameter number or boolean, actual data type: {type(data)}. Value: {data}"
 		return value_to_str(data)
 	else:
-		raise Exception(f"Unsupported data type: '{type(data_type)}'.")
+		raise RsInstrException(f"Unsupported data type: '{type(data_type)}'.")
 
 
 class ConverterToScpiString:
 	"""Converter from argument value to SCPI string.
 	Provides method get_value(arg_value) -> str
 	"""
 
 	def __init__(self, data_type: DataType, enum_type: Enum = None):
 		self.enum_type = enum_type
 		self.data_type = data_type
 		self.element_type = self.data_type.element_type
-		if self.element_type == DataType.Enum:
+		if self.element_type == DataType.Enum or self.element_type == DataType.EnumExt:
 			assert self.enum_type, f"For data_type {data_type.name}, you have to define the enum_type variable."
 
 	def get_value(self, data) -> str:
 		"""Returns SCPI string converted from the argument data."""
 		if self.data_type.is_list:
 			assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
 		else:
 			assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
 
 		if self.data_type == DataType.Enum:
 			return enum_scalar_to_str(data, self.enum_type)
-		elif self.data_type == DataType.EnumList:
+		if self.data_type == DataType.EnumExt:
+			return enum_ext_scalar_to_str(data, self.enum_type)
+		if self.data_type == DataType.EnumList:
 			return enum_list_to_str(data, self.enum_type)
+		if self.data_type == DataType.EnumExtList:
+			return enum_ext_list_to_str(data, self.enum_type)
 
 		return value_to_scpi_string(data, self.data_type)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Core.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,110 @@
-import re
+"""See the class docstring."""
+
 from typing import Callable
 
-from . import InstrumentOptions as Options, Conversions as Conv
+from . import InstrumentOptions as Options
 from .ArgSingle import ArgSingle
 from .ArgSingleList import ArgSingleList
 from .Conversions import BinFloatFormat, BinIntFormat
 from .Instrument import Instrument
 from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
-from .Utilities import parse_token_to_key_and_value, trim_str_response
+from .ScpiLogger import LoggingMode
+from .InstrumentErrors import RsInstrException
 
 
 class Core(object):
 	"""Main driver component. Provides: \n
 		- Main core constructor
 		- 'io' interface for all the write / query operations
 		- Command parameters string composer for single arguments...
 		- Link handlers adding / changing / deleting
 
 		Version history:
 
+		1.53.0 (18.10.2022)
+			- Improved mode where the instrument works with a session from another object.
+			- Silently ignoring invalid *IDN? string.
+			- Added new options profile 'Minimal' for non-SCPI-99 instruments.
+
+		1.52.0 (28.09.2022)
+			- Fixed DisableOpcQuery=True settings effect.
+			- Improved robustness of the TerminationCharacter option value entry.
+			- Added new options profile for CMQ500.
+
+		1.51.0 (08.09.2022)
+			- Changed the accepted IDN? response to more permissive.
+			- added methods go_to_remote() and go_to_local()
+			- added methods file_exists() and get_file_size()
+
+		1.50.0 (23.06.2022)
+			- Added relative timestamp to the logger.
+			- ScpiLogger can read GlobalData class variables making it possible to define common target and reference timestamp for all instances.
+			- Logger stream entries are by default immediately flushed, making sure that the log is complete.
+			- Added time statistic methods get_total_execution_time(), get_total_time(), reset_time_statistics().
+
+		1.24.0 (03.06.2022)
+			- Changed parsing of SYST:ERR? response to tolerate +0,"No Error" response.
+			- Added settings integer token OpenTimeout. Example: OpenTimeout=5000. Default: 0
+			- Added settings boolean token ExclusiveLock. Example: ExclusiveLock=True. Default: False
+
+		1.23.0 (24.05.2022)
+			- Added stripping of trailing commas when parsing the *IDN? response.
+			- If the Resource Manager does not find any default VISA implementation, it falls back to R&S VISA - relevant for LINUX or macOS
+			- Other typos and formatting corrections.
+
+		1.22.0 (20.04.2022)
+			- Added optional parameter timeout to reset()
+			- Added query list methods:  query_bool_list, query_bool_list_with_opc
+
+		1.21.0 (07.01.2022)
+			- Added logging to UDP port (49200) to integrate with new R&S Instrument Control plugin for Pycharm
+
+		1.20.0 (19.11.2021)
+			- Fixed logging strings when device name was a substring of the resource name
+
+		1.18.0 (build 64) 05.11.2021
+			- Added setting profile for non-standard instruments. Example of the options string: options='Profile=hm8123'
+
+		1.17.0 (build 63) 15.10.2021
+			- Added correct conversion of strings with SI suffixes (e.g.: MHz, KHz, THz, GHz, ms, us) to float and integer
+
+		1.16.0 (build 62) 31.08.2021
+			- Changed default encoding of string<=>bin from utf-8 to charmap.
+			- Added settable encoding for the session. Property: RsInstrument.encoding
+
+		1.15.0 (build 61) 17.08.2021
+			- Added support for EnumExt and EnumExtList
+			- Added support for custom scpi enums
+			- Improved exception handling in cases where the instrument session is closed.
+			- Fixed warning in Instrument.py
+			- Fixed Instrument.query_bin_block() for timeout errors
+			- Repeated capabilities are now allowed to be integer numbers as well
+
+		1.14.0 (build 53) 12.07.2021
+			- Scpi logger time entries now support not only datetime tuples, but also float timestamps
+			- changed handling of the syst:err? responses - now they are always Tuple (code, message)
+			- StatusException has new field errors_list: List[ Tuple[code, message] ]
+			- Added logger.log_status_check_ok property. This allows for skipping lines with 'Status check: OK'
+
+		1.12.0 (build 50) 26.06.2021
+			- Added SCPI Logger
+			- Simplified constructor's options string format - removed DriverSetup=() syntax:
+			Instead of "DriverSetup=(TerminationCharacter='\n')", you use "TerminationCharacter='\n'"
+			The original format is still supported.
+
+			- Fixed calling SYST:ERR? even if *STB? returned 0
+			- Replaced @ni backend with @ivi for resource manager - this is necessary for the future pyvisa version 1.12+
+
+		1.11.0 (build 49) 09.06.2021
+			- Added is_connection_active() + reconnect()
+
+		1.10.1 (build 47) 01.06.2021
+			- Fixed bug with error checking when events are defined
+
 		1.10.0 (build 46) 03.05.2021
 			- Added methods to Instrument: query_struct_with_opc(), query_str_suppressed_with_opc()
 
 		1.9.0 (build 45) 13.04.2021
 			- Added option to set callbacks before_write and before_query
 			- When a RepCap has a member with integer number 0 defined, the command string interpretation of such member is '0', not empty string
 
@@ -32,15 +114,15 @@
 		1.7.7 (build 42) 26.11.2020
 			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
 
 		1.7.6 (build 41) 23.11.2020
 			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
 
 		1.7.5 (build 40) 12.11.2020
-			- Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
+			- Extended 'Conversions' method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
 
 		1.7.4 (build 39) 11.09.2020
 			- Fixed parsing of the instrument errors when an error message contains two double quotes
 
 		1.7.3 (build 38) 21.10.2020
 			- Added 'UND' to the list of float numbers that are represented as NaN
 
@@ -60,15 +142,15 @@
 
 		1.4.0 (build 32) 17.09.2020
 			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'
 			- Fixed bug in reading binary data 16 bit
 
 		1.3.0 (build 31) 04.09.2020
 			- added DRIVERSETUP_QUERYOPT to the driver's option string
-			- *OPT? is no longer performed at the init, but only at the first access to options string.
+			- *OPT? is no longer performed at the init, but only at the first access to the options string.
 				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed
 
 		1.2.0 (build 30), 03.08.2020
 			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000
 
 		1.1.0 (build 29), 20.06.2020
 			- Added RepeatedCapability and base class CommandsGroup
@@ -89,85 +171,91 @@
 			reset: bool = False,
 			driver_options: str = None,
 			user_options: str = None,
 			direct_session: object = None):
 		"""Initializes new driver session. For cleaner code, use the class methods: \n
 		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
 
-		self.core_version = '1.9.0'
-		self.simulating = False
-		self.supported_idn_patterns = []
-		self.supported_instr_models = []
-
-		self._args_single_list = ArgSingleList()
-		sett_dr = self._parse_init_settings_string(driver_options)
-		self._apply_settings_to_core(sett_dr)
-		sett_user = self._parse_init_settings_string(user_options)
-		self._apply_settings_to_core(sett_user)
+		self.core_version = '1.53.0'
+		self.resource_name = resource_name
 
 		# Typical settings for the Core
 		self._instrumentSettings = InstrumentSettings(
 			InstrViClearMode.execute_on_all,  # Instrument viClear mode
 			False,  # Full model name. True: SMW200A, False: SMW
 			0,  # Delay by each write
 			0,  # Delay by each read
-			100000,  # Max chunk read / write size in bytes
+			1000000,  # Max chunk read / write size in bytes
 			WaitForOpcMode.stb_poll,  # Waiting for OPC Mode: Status byte polling
 			30000,  # OPC timeout
 			10000,  # VISA timeout
 			60000,  # Self-test timeout
 			Options.ParseMode.Auto,  # *OPT? response parsing mode
 			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
 			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
-			False  # OPC query after each setting
+			False,  # OPC query after each setting
+			LoggingMode.Off  # Logging mode
 		)
 
-		self._instrumentSettings.apply_option_settings(sett_dr)
-		self._instrumentSettings.apply_option_settings(sett_user)
+		self._instrumentSettings.apply_option_settings(driver_options)
+		self._instrumentSettings.apply_option_settings(user_options)
 
-		# Resolve the direct_session to handle. Options for direct_session type:
-		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
-		# - string in case of a simulation session
-		handle = direct_session
-		if handle:
-			# Check if the entered 'direct_session' is either the driver object or the Visa session
-			if hasattr(direct_session, 'get_session_handle'):
-				assert hasattr(direct_session, '_core'), f"Direct session is a class type. It must be an instance of the top-level driver class."
-				handle = direct_session.get_session_handle()
-			# Check if the handle is not a simulation mode string
-			if isinstance(handle, str):
-				if "Simulating session, resource name " in handle:
-					self.simulating = True
-					handle = None
+		self.simulating = self._instrumentSettings.simulating
+		self.supported_idn_patterns = self._instrumentSettings.supported_idn_patterns
+		self.supported_instr_models = self._instrumentSettings.supported_instr_models
 
-		self.io = Instrument(resource_name, self.simulating, self._instrumentSettings, handle)
+		self._args_single_list = ArgSingleList()
+		handle = self._resolve_direct_session(direct_session)
+		self.io = Instrument(self.resource_name, self.simulating, self._instrumentSettings, handle)
 		self.io.query_instr_status = True
+		# Update the resource name if it changed, for example because of the direct session
+		self.resource_name = self.io.resource_name
+		self.allow_reconnect = self.io.allow_reconnect
 
-		self._apply_settings_to_instrument(sett_dr)
-		self._apply_settings_to_instrument(sett_user)
-
+		self._apply_settings_to_instrument(self._instrumentSettings)
 		self.io.set_simulating_cmds()
 
 		if id_query:
 			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
 
 		if reset:
 			self.io.reset()
 		else:
 			self.io.check_status()
 
 	@classmethod
 	def from_existing_session(cls, session: object, driver_options: str = None) -> 'Core':
 		"""Creates a new Core object with the entered 'session' reused."""
 		# noinspection PyTypeChecker
-		return cls(None, False, False, driver_options, None, session)
+		return cls(resource_name=None, id_query=False, reset=False, driver_options=driver_options, user_options=None, direct_session=session)
 
 	def __str__(self):
 		return f"Core session '{self.io.resource_name}'"
 
+	def _resolve_direct_session(self, direct_session):
+		# Resolve the direct_session to handle. Options for direct_session type:
+		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
+		# - string in case of a simulation session
+		handle = direct_session
+		if not direct_session:
+			return None
+		# Check if the entered 'direct_session' is either the driver object or the Visa session
+		if hasattr(direct_session, 'get_session_handle'):
+			if not hasattr(direct_session, '_core'):
+				raise RsInstrException('Direct session is a class type. It must be an instance of the top-level driver class.')
+			handle = direct_session.get_session_handle()
+		# If the handle is a simulating session, change the session to simulating and set disable the 'from existing session' feature
+		if isinstance(handle, str):
+			mand_string = 'Simulating session, resource name '
+			if mand_string in handle:
+				self.resource_name = handle[len(mand_string):].strip().strip("'").strip()
+				self.simulating = True
+				handle = None
+		return handle
+
 	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
 		"""Adds / Updates link handler for the entered link_name.
 		Handler API: handler(event_args: ArgLinkedEventArgs)
 		Returns the previous registered handler, or None if no handler was registered before."""
 		return self.io.set_link_handler(link_name, handler)
 
 	def del_link_handler(self, link_name: str) -> Callable:
@@ -176,82 +264,24 @@
 		return self.io.del_link_handler(link_name)
 
 	def del_all_link_handlers(self) -> int:
 		"""Deletes all the link handlers.
 		Returns number of deleted links."""
 		return self.io.del_all_link_handlers()
 
-	# noinspection PyMethodMayBeStatic
-	def _parse_init_settings_string(self, text: str) -> dict:
-		"""Parses init string to a dictionary of settings: name -> value."""
-		tokens = {}
-		if not text:
-			return tokens
-
-		# Text enclosed in single brackets '' must have the commas escaped
-		literal_pattern = r"'([^']+)'"
-		while True:
-			# literal loop
-			m = re.search(literal_pattern, text)
-			if not m:
-				break
-			lit_part = '"' + m.group(1).replace(',', '<COMMA_ESC>') + '"'
-			text = text.replace(m.group(0), lit_part)
-
-		# Remove all the class-options enclosed by round brackets e.g. "<groupName>=(<groupTokens>)"
-		group_pattern = r'(\w+)\s*=\s*\(([^\)]*)\)'
-		# Match class-settings, add them as separate keys with groupName_Key
-		while True:
-			# Group loop
-			m = re.search(group_pattern, text)
-			if not m:
-				break
-			text = text.replace(m.group(0), '')
-			group_name = m.group(1).upper()
-			group_tokens = m.group(2).strip().split(',')
-			for token in group_tokens:
-				key, value = parse_token_to_key_and_value(token)
-				if value:
-					tokens[f'{group_name}_{key.upper()}'] = value
-
-		# All groups are removed from the text, now we can use splitting on commas and remove white-space-only elements
-		for token in text.split(','):
-			key, value = parse_token_to_key_and_value(token.replace('<COMMA_ESC>', ','))
-			if value:
-				tokens[key.upper()] = value
-		return tokens
-
-	def _apply_settings_to_core(self, settings: dict) -> None:
-		"""Applies settings relevant for the Core from the dictionary."""
-		value = settings.get('SIMULATE')
-		if value:
-			self.simulating = Conv.str_to_bool(value)
-
-		value = settings.get('SUPPORTEDINSTRMODELS')
-		if value:
-			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
-
-		value = settings.get('SUPPORTEDIDNPATTERNS')
-		if value:
-			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
-
-	def _apply_settings_to_instrument(self, settings: dict) -> None:
-		"""Applies settings relevant for the Instrument from the dictionary."""
-		value = settings.get('QUERYINSTRUMENTSTATUS')
-		if value:
-			self.io.query_instr_status = Conv.str_to_bool(value)
-
-		value = settings.get('SIMULATIONIDNSTRING')
-		if value and self.simulating:
-			# Use the '*' instead of the ',' in the value to avoid comma as token delimiter
-			self.io.idn_string = value.replace('*', ',')
+	def _apply_settings_to_instrument(self, settings: InstrumentSettings) -> None:
+		"""Applies settings relevant for the Instrument from the InstrumentSettings structure."""
+		if settings.instrument_status_check is not None:
+			self.io.query_instr_status = settings.instrument_status_check
+		if self.simulating and settings.instrument_simulation_idn_string is not None:
+			self.io.idn_string = settings.instrument_simulation_idn_string
 
 	def compose_cmd_arg_param(
 			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
-		"""Composes command parameter string based on the single arguments definition."""
+		"""Composes command parameter string based on the single argument definition."""
 		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
 
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
 		return self.io.get_last_sent_cmd()
 
 	def get_session_handle(self):
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Instrument.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSession.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,854 +1,1265 @@
+"""Visa Session is an extension of the pure VISA providing higher level of methods regardless of the session kind."""
+
+import time
+from enum import Enum, Flag
+from typing import List, Tuple, Callable, AnyStr
+import os.path
 import re
 import threading
-from enum import Enum
-from typing import List, Callable, Tuple, Dict
 
-from . import Utilities, InstrumentSettings, InstrumentOptions, InstrumentErrors, Conversions as Conv
-from .ArgSingleSuppressed import ArgSingleSuppressed
-from .ArgStructList import ArgStructList
-from .InternalLinker import InternalLinker
-from .IoTransferEventArgs import IoTransferEventArgs
+# noinspection PyPackageRequirements
+import pyvisa
+
+from .VisaPluginSocketIo import ResourceManager, SocketIo
+from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
+from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
-from .Utilities import trim_str_response
-from .VisaSession import VisaSession, EventArgsChunk
-from .VisaSessionSim import VisaSessionSim
-from .RepeatedCapability import RepeatedCapability
-
-
-class Instrument(object):
-	"""Model of an Instrument with VISA interface."""
-
-	def __init__(self, resource_name: str, simulate: bool, settings: InstrumentSettings, direct_session=None):
-		"""Opening an instrument session.
-		If simulate is true, it cannot be later switched to false anymore."""
-		self._simulating: bool = simulate
-		self._session = None
-		self._global_repcaps: Dict[str, RepeatedCapability] = {}
-		self._linker = InternalLinker()
-		# noinspection PyTypeChecker
-		self.on_write_handler: Callable = None
+from .Utilities import size_to_kb_mb_string, calculate_chunks_count
+import platform
+import struct
+
+
+class SessionKind(Enum):
+	"""Visa instrument session type."""
+	unsupported = 0
+	gpib = 1
+	serial = 2
+	vxi11 = 3
+	socket = 5
+	usb = 6
+	rs_nrp = 7
+
+
+class ReadDataType(Enum):
+	"""Data type returned by the instrument."""
+	unknown = 0
+	ascii = 1
+	null = 2
+	bin_known_len = 3
+	bin_unknown_len = 4
+
+
+class StatusByte(Flag):
+	"""Status Byte flags."""
+	NONE = 0x00
+	error_queue_not_empty = 0x04
+	questionable_status_reg = 0x08
+	message_available = 0x10
+	event_status_byte = 0x20
+	request_service = 0x40
+	operation_status_reg = 0x80
+
+
+class EventStatusRegister(Flag):
+	"""Event Status Register flags."""
+	null = 0x00
+	operation_complete = 0x01
+
+
+# noinspection PyUnresolvedReferences
+class VisaSession(object):
+	"""Extended VISA class."""
+
+	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
+		self.reusing_session = direct_session is not None
 		# noinspection PyTypeChecker
-		self.on_read_handler: Callable = None
-		self._io_events_include_data: bool = False
+		self._data_chunk_size: int = None
+		self._std_bin_block_header_max_len: int = 999999999
 		self._lock = None
-		self._before_query_handler = None
-		self._before_write_handler = None
+		self.disable_opc_query: bool = settings.disable_opc_query
+		self.last_status = None
+		self.visa_library_name = None
+		self.resource_name = resource_name  # might be changed later if direct_session is used
+		self.encoding = settings.encoding  # default encoder between bytes and string
+		self.cmd_idn = settings.cmd_idn
+		self.skip_status_system_setting = settings.skip_status_system_setting
+		self.skip_clear_status = settings.skip_clear_status
+		self.stb_in_error_check = settings.stb_in_error_check
 
-		# Fixed settings
-		self.selftest_timeout = 100000 if settings.selftest_timeout == 0 else settings.selftest_timeout
-		self.idn_model_full_name = settings.idn_model_full_name
-		self.instr_options_parse_mode = settings.instr_options_parse_mode
+		# Implemented for interface compatibility with VisaSessionSim
+		self.cached_to_stream = False
+
+		# Event handlers
+		# noinspection PyTypeChecker
+		self.on_read_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
+		# noinspection PyTypeChecker
+		self.on_write_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
+		self.io_events_include_data: bool = False
+		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
+
+		if self.reusing_session:
+			# Reuse the session
+			self._session = VisaSession.get_and_check_direct_session(direct_session)
+			self.resource_name = self._session.resource_name
+		else:
+			# Create new session
+			# Check resource_name for the trailing (SelectVisa=..)
+			pure_resource_name, visa_select = self._get_pure_resource_name(resource_name)
+			if settings.visa_select is not None:
+				visa_select = settings.visa_select
+			self._rm = VisaSession.get_resource_manager(visa_select)
+			self.manufacturer = self._get_visa_manufacturer()
+
+			# Resource manager opening
+			try:
+				acc_mode = pyvisa.constants.AccessModes.no_lock if settings.exclusive_lock is False else pyvisa.constants.AccessModes.exclusive_lock
+				self._session = self._rm.open_resource(resource_name=pure_resource_name, open_timeout=settings.open_timeout, access_mode=acc_mode)
+			except pyvisa.VisaIOError as e:
+				if e.error_code != pyvisa.constants.StatusCode.error_resource_not_found:
+					raise e
+				message = e.description
+				message += f"\nLibrary: {self._rm.visalib}\nManufacturer: {self.manufacturer}\nResource Name: '{resource_name}'"
+				raise InstrumentErrors.ResourceError(resource_name, message)
+			self.resource_name = resource_name
+
+		# Decide, whether to create a new thread lock or the existing one from the session
+		if hasattr(self._session, 'session_thread_rlock'):
+			rlock = self._session.session_thread_rlock
+			if isinstance(rlock, type(threading.RLock())):
+				self.assign_lock(rlock)
+		if self.get_lock() is None:
+			# The existing session did not have a thread lock, assign a new one
+			self.assign_lock(threading.RLock())
+
+		self._interface_type = SessionKind.unsupported
+		if self._session.interface_type == pyvisa.constants.InterfaceType.gpib or self._session.interface_type == pyvisa.constants.InterfaceType.gpib:
+			self._interface_type = SessionKind.gpib
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.rsnrp:
+			self._interface_type = SessionKind.rs_nrp
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.asrl:
+			self._interface_type = SessionKind.serial
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.usb:
+			# Check whether it is not the NRP-Z
+			intf_type = self._session.get_visa_attribute(pyvisa.constants.VI_ATTR_INTF_TYPE)
+			if intf_type == pyvisa.constants.InterfaceType.rsnrp:
+				self._interface_type = SessionKind.rs_nrp
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.tcpip:
+			self._interface_type = SessionKind.vxi11
+			if self._session.resource_class == 'SOCKET':
+				self._interface_type = SessionKind.socket
+
+		# Specifics for different interfaces
+		self._assure_write_with_tc = settings.assure_write_with_tc
+		self._term_char = settings.term_char
+		self._term_char_bin = self._term_char.encode(self.encoding)
+		self._session.write_termination = ''
+		self.vxi_capable = settings.vxi_capable
+
+		if self._interface_type == SessionKind.serial:
+			self.vxi_capable = False
+		elif self._interface_type == SessionKind.socket:
+			self.vxi_capable = False
+
+		# NRP-Z specific settings
+		if self.is_rsnrp_session():
+			self.disable_opc_query = True
+			# NRP-Z does not support chunk reading, therefore the segment must be in one piece
+			settings.io_segment_size = 1000000
+			self.vxi_capable = False
+
+		self.write_delay = settings.write_delay
+		self.read_delay = settings.read_delay
+		self._viclear_exe_mode = settings.viclear_exe_mode
+		self._opc_wait_mode = settings.opc_wait_mode
+
+		# Parameters that need to be coerced based on Vxi-capability
+		if self.vxi_capable:
+			self._add_term_char_to_write_bin_block = settings.add_term_char_to_write_bin_block
+			self._session.read_termination = ''
+		else:
+			self._add_term_char_to_write_bin_block = True
+			self._session.read_termination = self._term_char
+			self._assure_write_with_tc = True
 
 		# Changeable settings
-		self.resource_name: str = resource_name
-		self._instr_options: InstrumentOptions = None  # Internal private property for the lazy property self.instr_options - see the getter for self.instr_options. Initialized by the first access
-		self.query_instr_status: bool = True
-		self.opc_query_after_write: bool = False
-		self.bin_float_numbers_format = settings.bin_float_numbers_format
-		self.bin_int_numbers_format = settings.bin_int_numbers_format
-		self.opc_query_after_write: bool = settings.opc_query_after_write
-		self.stb_in_error_check: bool = settings.stb_in_error_check
-
-		self.manufacturer: str = 'Rohde&Schwarz'
-		self.model: str = 'R&S Instrument'
-		self.serial_number: str = '100001'
-		self.firmware_version: str = '1.00'
-
-		if self._simulating:
-			self._session = VisaSessionSim(resource_name, settings, direct_session)
-			self._lock = self._session.get_lock()
-			self._instr_options = InstrumentOptions.Options('K0', InstrumentOptions.ParseMode.KeepOriginal)
-			self._session.write('*OPT K0')
+		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
+		self.visa_timeout = settings.visa_timeout
+		self._session.chunk_size = settings.io_segment_size
+		self._data_chunk_size = settings.io_segment_size
+
+		# Must call the VISA viClear() before any communication with the instrument
+		self.clear()
+
+		# Further steps are for NRP-Z session not valid
+		if self.is_rsnrp_session():
 			return
 
-		self._session = VisaSession(resource_name, settings, direct_session)
-		self._lock = self._session.get_lock()
-		with self._lock:
-			self._session.clear_before_read()
-			self.idn_string = Utilities.trim_str_response(self._session.query_str('*IDN?')).strip()
-
-			# NRP-Z session coercing
-			if self._session.is_rsnrp_session():
-				settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
-				self.stb_in_error_check = False
-			self.instr_options_parse_mode = settings.instr_options_parse_mode
+		# Clear instrument status
+		if self.skip_clear_status is False:
+			self.write('*CLS')
+			if self.vxi_capable:
+				stb = self._read_stb()
+				if stb & StatusByte.message_available:
+					self._flush_junk_data()
 
-	def __str__(self):
-		if self._simulating:
-			return f"Simulated, Model: '{self.model}', ResourceName: '{self.resource_name}'"
-		else:
-			return f"Instrument Model: '{self.model}', ResourceName: '{self.resource_name}'"
+		# Apply settings for ESE and SRE, plus coerce the _opcWaitMode if necessary
+		self._opc_wait_mode = self._set_regs_ese_sre(self._opc_wait_mode)
+
+	@staticmethod
+	def get_and_check_direct_session(direct_session):
+		"""Returns direct session if it's a proper type.
+		If the direct_session is None, the function returns None.
+		If the direct_session is of an unsupported type, the function raises RsInstrException."""
+		if direct_session is None:
+			return None
+		# Reuse the session
+		if not isinstance(direct_session, pyvisa.Resource) and not isinstance(direct_session, SocketIo):
+			raise InstrumentErrors.RsInstrException(f"Direct_session must be a VISA resource object. Actual type: '{type(direct_session)}', value: '{direct_session}'")
+		return direct_session
 
-	def set_simulating_cmds(self) -> None:
-		"""Updated cached values in the simulating VISA session to properly respond to *IDN? or *OPT?"""
-		if self._simulating:
-			self.write(f'*idn {self.idn_string}')
-			self.write(f'*opt {Conv.list_to_csv_str(self.instr_options.get_all())}')
-			self.write(f'*opc 1')
-			self.write(f'*stb 0')
-			self.write(f'*tst 0,"Passed"')
-			self.write(f'syst:err 0,"No Error"')
-			self.write(f'system:error 0,"No Error"')
-
-	def get_last_sent_cmd(self) -> str:
-		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
-		if self._simulating:
-			# noinspection PyUnresolvedReferences
-			return self._session.get_last_sent_cmd()
-		raise Exception('get_last_sent_cmd() can only be used in simulation mode')
+	@staticmethod
+	def _get_pure_resource_name(resource_name: str):
+		"""Returns pure resource name stripped of the (SelectVisa) part and the visa_select string"""
+		m = re.search(r'(.+)\(SelectVisa=([^),]+)\)', resource_name)
+		if not m:
+			return resource_name, None
+		resource_name = m.group(1).strip()
+		visa_select = m.group(2).strip()
+		return resource_name, visa_select
+
+	@classmethod
+	def get_resource_manager(cls, visa_select: str) -> pyvisa.ResourceManager:
+		"""Returns resource manager for the desired VISA implementation"""
+		operating_system = platform.system().lower()
+		vsl = None if visa_select is None else visa_select.lower()
+		bittness = struct.calcsize('P') * 8
+		# Try if you find the default VISA dll
+		try:
+			if visa_select is None or visa_select in ['@default', '@standard', 'default', 'standard', 'defaultvisa', 'standardvisa', '@defaultvisa', '@standardvisa']:
+				return pyvisa.ResourceManager()
+
+			if vsl in ['@ni', 'ni', 'ivi', '@ivi', 'visa-ni', 'nivisa', 'ni-visa', 'nationalinstruments', 'nationalinstrumentsvisa']:
+				return pyvisa.ResourceManager()
+
+			if vsl in ['@py', 'pyvisa', 'visa-py', 'pyvisa-py']:
+				return pyvisa.ResourceManager('@py')
+		except ValueError:
+			# None of the required implementations found, fall back to the R&S VISA
+			visa_select = 'rsvisa'
+			vsl = visa_select.lower()
+
+		# from here, RsVisa implementation is considered
+		if 'rohde&schwarz' in vsl or 'rohdeschwarz' in vsl or vsl == 'rsvisa' or vsl == 'rs' or vsl == 'r&s':
+			if operating_system == 'windows':
+				if bittness == 32:
+					visa_select = r'c:\Windows\SysWOW64\RsVisa32.dll'
+				else:
+					visa_select = r'c:\Windows\system32\RsVisa32.dll'
+				return pyvisa.ResourceManager(visa_select)
+			elif operating_system == 'linux':
+				# The default install location may be different
+				# for debian/red hat/opensuse derived distributions
+				check_visa = [f'/usr/lib{bittness}/librsvisa.so', r'/usr/lib/librsvisa.so']
+				for check in check_visa:
+					if os.path.isfile(check):
+						return pyvisa.ResourceManager(check)
+			elif operating_system == 'darwin':
+				# MacOS
+				check_visa = [f'/Library/Frameworks/RsVisa.framework/Versions/Current/RsVisa/librsvisa.dylib']
+				for check in check_visa:
+					if os.path.isfile(check):
+						return pyvisa.ResourceManager(check)
+
+		if vsl in ['socketio', 'socket', 'none']:
+			return ResourceManager()
+
+		return pyvisa.ResourceManager(visa_select)
+
+	def _get_visa_manufacturer(self) -> str:
+		"""Returns manufacturer of the current VISA"""
+		if hasattr(self._rm, 'VisaManufacturerName'):
+			return self._rm.VisaManufacturerName
+		try:
+			return self._rm.visalib.get_attribute(self._rm.session, pyvisa.constants.VI_ATTR_RSRC_MANF_NAME)[0]
+		except TypeError:
+			return self._rm.visalib.__class__.__name__
+
+	def is_rsnrp_session(self) -> bool:
+		"""Returns True, if the current session is a NRP-Z session"""
+		return self._interface_type == SessionKind.rs_nrp
 
 	def assign_lock(self, lock: threading.RLock) -> None:
-		"""Assigns the thread lock provided from by the user. Trickles down to the VisaSession."""
+		"""Assigns the provided thread lock by setting the pyvisa runtime session attribute 'session_thread_rlock'
+		This is done, because if the session is to be entered as an existing session to another RsInstrument object,
+		the lock must be shared as well. The lock is only used by the parent class Instrument."""
+		setattr(self._session, 'session_thread_rlock', lock)
 		self._lock = lock
-		self._session.assign_lock(lock)
 
 	def get_lock(self) -> threading.RLock:
 		"""Returns the current RLock object."""
 		return self._lock
 
-	def clear_lock(self):
-		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
-		self.assign_lock(threading.RLock())
-
-	@property
-	def visa_manufacturer(self) -> str:
-		"""Returns the visa manufacturer of the current session."""
-		return self._session.manufacturer
-
-	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
-		"""Adds / Updates link handler for the entered link_name.
-		Handler API: handler(event_args: ArgLinkedEventArgs)
-		Returns the previous registered handler, or None if no handler was registered before."""
-		return self._linker.set_handler(link_name, handler)
-
-	def del_link_handler(self, link_name: str) -> Callable:
-		"""Deletes link handler for the link_name.
-		Returns the deleted handler, or None if none existed."""
-		return self._linker.del_handler(link_name)
-
-	def del_all_link_handlers(self) -> int:
-		"""Deletes all the link handlers.
-		Returns number of deleted links."""
-		return self._linker.del_all_handlers()
-
-	@property
-	def idn_string(self) -> str:
-		return self._idn_string
-
-	@idn_string.setter
-	def idn_string(self, value: str) -> None:
-		"""IDN string. Set it to force a different IDN string than the default *IDN? response."""
-		self._idn_string = value
-		self._parse_idn_string(self._idn_string)
-
-	@property
-	def instr_options(self) -> InstrumentOptions:
-		"""Public getter for the lazy property instr_options"""
-		if self._instr_options is None:
-			self._query_options_and_parse(self.instr_options_parse_mode)
-		return self._instr_options
-
-	@property
-	def opc_timeout(self) -> int:
-		"""See the opc_timeout.setter."""
-		return self._session.opc_timeout
-
-	@opc_timeout.setter
-	def opc_timeout(self, value: int) -> None:
-		"""Sets / Gets timeout in milliseconds for all the operations that use OPC synchronization."""
-		self._session.opc_timeout = value
-
 	@property
 	def visa_timeout(self) -> int:
 		"""See the visa_timeout.setter."""
-		return self._session.visa_timeout
+		return int(self._session.timeout)
 
 	@visa_timeout.setter
 	def visa_timeout(self, value: int) -> None:
 		"""Sets / Gets visa IO timeout in milliseconds."""
-		self._session.visa_timeout = value
+		self._session.timeout = int(value)
 
 	@property
 	def data_chunk_size(self) -> int:
 		"""Returns max chunk size of one data block."""
-		return self._session.data_chunk_size
+		return self._data_chunk_size
 
 	@data_chunk_size.setter
 	def data_chunk_size(self, chunk_size: int) -> None:
 		"""Sets the maximum size of one block transferred during write/read operations."""
-		self._session.data_chunk_size = int(chunk_size)
+		self._data_chunk_size = int(chunk_size)
+		self._session.chunk_size = int(chunk_size)
 
-	# noinspection PyMethodMayBeStatic
-	def _sim_cached_value_found(self, value) -> bool:
-		return value != 'Simulating'
-
-	# noinspection PyMethodMayBeStatic
-	def _sim_cached_value_not_found(self, value) -> bool:
-		return value == 'Simulating'
-
-	def _parse_idn_string(self, idn_string: str) -> None:
-		"""Parse the *IDN? response to:
-		- Manufacturer
-		- Model
-		- SerialNumber
-		- FirmwareRevision"""
-		idn_string = idn_string.strip()
-		m = re.search(r'([\w& ]+),([a-zA-Z ]+)([\-0-9a-zA-Z ]*),([^,]+),([\w .\-/]+)', idn_string)
-		if not m:
-			raise Exception(f"The instrument *IDN? string parsing failed. Parsed *IDN? response: '{idn_string}'")
-		self.manufacturer = m.group(1).strip()
-		self.model = m.group(2).strip()
-		self.full_model_name = self.model + m.group(3).strip()
-		self.serial_number = m.group(4).strip()
-		self.firmware_version = m.group(5).strip()
-		if self.idn_model_full_name:
-			self.model = self.full_model_name
-
-	def fits_idn_pattern(self, patterns: List[str], supported_models: List[str]) -> None:
-		"""Throws exception if the current instrument model does not fit  any of the patterns.
-		The supported_models argument is only used for exception messages"""
-		matches = False
-		assert self._idn_string, f'*IDN? was not assigned yet.'
-		for x in patterns:
-			matches = re.search(x, self.idn_string, re.IGNORECASE)
-			if matches:
+	def _resolve_opc_timeout(self, timeout: int) -> int:
+		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
+		if timeout is None or timeout < 1:
+			return self.opc_timeout
+		else:
+			return timeout
+
+	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
+		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
+		Returns coerced WaitForOpcMode."""
+		# Set the SRE and ESE registers accordingly
+		# No SRE is supported
+		if self.skip_status_system_setting:
+			return mode
+		self._set_ese_mask(EventStatusRegister.operation_complete)
+		self._set_sre_mask(StatusByte.NONE)
+		return mode
+
+	# noinspection PyTypeChecker
+	def _set_ese_mask(self, mask: EventStatusRegister, reset: bool = True) -> None:
+		"""Sends *ESE command with mask parameter."""
+		if reset is False:
+			current_value = int(self._query_str_no_events('*ESE?'))
+			mask = current_value | mask.value
+		self.write("*ESE %d" % mask.value)
+
+	# noinspection PyTypeChecker
+	def _set_sre_mask(self, mask: StatusByte, reset: bool = True) -> None:
+		"""Sends *SRE command with StatusByte mask parameter."""
+		if reset is False:
+			current_value = int(self._query_str_no_events('*SRE?'))
+			mask = current_value | mask.value
+		# Also affect the _opc_wait_mode:
+		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
+		# If the mask has event_status_byte == true, do not change anything
+		self.write(f'*SRE {mask.value}')
+
+	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
+		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
+		Also works with the SOCKET and SERIAL interface by sending *STB? query.
+		In that case however, command cannot be a query.
+		Returns the last read Status Byte value."""
+		timeout_secs = timeout / 1000
+		self.clear_before_read()
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		self.write(command + ';*OPC')
+		# Use catch to return the VISA Timeout back
+		start = time.time()
+		# STB polling loop
+		while True:
+			stb = self._read_stb()
+			elapsed = self._polling_delay(start)
+			if elapsed > timeout_secs:
+				self._narrow_down_opc_tout_error(command, is_query, timeout)
+			if end_mask & stb:
 				break
-		if not matches:
-			message = f"Instrument is not supported.\n*IDN? string: '{self.idn_string}'"
-			if len(supported_models) > 0:
-				message += f"\nSupported models: '{', '.join(supported_models)}'"
-			if len(patterns) == 1:
-				message += f"\nSupported IDN pattern: '{patterns[0]}'"
-			if len(patterns) > 1:
-				message += "\nSupported IDN patterns:\n" + '\n'.join(patterns)
-			raise InstrumentErrors.UnexpectedResponseException(self.resource_name, message)
-
-	def _query_options_and_parse(self, mode: InstrumentOptions.ParseMode) -> None:
-		"""Queries *OPT? and parses it based on the ParseMode."""
-		if mode == InstrumentOptions.ParseMode.Skip:
-			self._instr_options = InstrumentOptions.Options('', mode)
-			return
-		if self._simulating is False:
-			with self._lock:
-				opts = self._session.query_str_no_tout_err('*OPT?', 1000)
-				if opts is None:
-					opts = 'Cannot read the instrument options - *OPT? query is not supported'
-				self._instr_options = InstrumentOptions.Options(opts, mode)
+		return stb
+
+	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
+		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
+			The command must not be a query. Also works with the SOCKET and SERIAL interface.
+			Returns the last read Status Byte value."""
+		timeout_secs = timeout / 1000
+		self.clear_before_read()
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		self.write(command + ';*OPC')
+		start = time.time()
+		# STB polling loop
+		while True:
+			stb = self._query_stb()
+			elapsed = self._polling_delay(start)
+			if elapsed > timeout_secs:
+				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout)
+			if stb & end_mask:
+				break
+		return stb
+
+	def _narrow_down_opc_tout_error(self, command: str, is_query: bool, timeout: int) -> None:
+		"""Called by the _write_and_poll_stb_vxi when the timeout expires.
+		The method tries to closer identify the cause of the timeout."""
+		stb = self._read_stb()
+		timeout = self._resolve_opc_timeout(timeout)
+		if is_query:
+			if stb & StatusByte.error_queue_not_empty:
+				self.clear()
+				context = f"Query '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context, first_exc=InstrumentErrors.TimeoutException)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Query '{command.strip()}'.")
+		else:
+			if stb & StatusByte.error_queue_not_empty:
+				self.clear()
+				context = f"Command '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context, first_exc=InstrumentErrors.TimeoutException)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Command '{command.strip()}'.")
+
+	def _narrow_down_io_tout_error(self, context: str, visa_timeout: int = 0) -> None:
+		"""Called internally after IOTimeoutException can narrow down the error to more specific exception.
+		You can define the visa_timeout value for the error message. Otherwise, the current visa_timeout is reported."""
+		context_stripped = context.strip().rstrip("- ")
+		if self.stb_in_error_check is False:
+			raise InstrumentErrors.TimeoutException(context_stripped)
+		if self.vxi_capable:
+			stb = self._read_stb()
+		else:
+			# Non-Vxi session
+			old_tout = self.visa_timeout
+			try:
+				self.visa_timeout = 500
+				stb = self._query_stb(False)
+			finally:
+				self.visa_timeout = old_tout
+		if visa_timeout <= 0:
+			visa_timeout = self.visa_timeout
+
+		context = context + f'VISA Timeout error occurred ({visa_timeout} milliseconds)'
+		if stb & StatusByte.error_queue_not_empty:
+			InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context + ' and ...', first_exc=InstrumentErrors.TimeoutException)
+		# In case none of the previous exceptions is thrown
+		raise InstrumentErrors.TimeoutException(context)
+
+	def _polling_delay(self, start):
+		"""Generates progressive polling delay."""
+
+		elapsed = time.time() - start
+		if self._opc_wait_mode == WaitForOpcMode.stb_poll:
+			if elapsed < 0.01:
+				return elapsed
+			if elapsed < 0.1:
+				time.sleep(0.005)
+				return elapsed
+			if elapsed < 1:
+				time.sleep(0.02)
+				return elapsed
+			if elapsed < 5:
+				time.sleep(0.05)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 50:
+				time.sleep(0.5)
+				return elapsed
+			time.sleep(1)
+		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_slow:
+			if elapsed < 0.01:
+				time.sleep(0.001)
+				return elapsed
+			if elapsed < 1:
+				time.sleep(0.02)
+				return elapsed
+			if elapsed < 5:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.2)
+				return elapsed
+			if elapsed < 20:
+				time.sleep(0.5)
+				return elapsed
+			time.sleep(1)
+		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_superslow:
+			if elapsed < 1:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.5)
+				return elapsed
+			if elapsed < 20:
+				time.sleep(1)
+				return elapsed
+			time.sleep(2)
+
+		return elapsed
 
 	@staticmethod
-	def _parse_err_query_response(response: str) -> str:
-		"""Parses entered response string to string error message without the error code.
-		E.g.: response = '-110,"Command error"' returns: 'Command error'."""
-		m = re.match(r'(-?[\d]+).*?"(.*)"', response)
+	def _parse_err_query_response(response: str) -> Tuple[int, str]:
+		"""
+		Parses entered response string to Tuple(code, message).
+		E.g.: response = '-110,"Command error"' returns: (-110,'Command error')
+		"""
+		m = re.match(r'([-+]?\d+).*?[\'"](.*)[\'"]', response)
+		code = 0
 		if m:
-			return m.group(2)
+			try:
+				code = int(m.group(1))
+			except ValueError:
+				pass
+			return code, m.group(2)
 		else:
-			return response
+			return code, response
 
-	def add_global_repcap(self, name: str, rep_cap: RepeatedCapability) -> None:
-		"""Adds the global repcap name to the list of global repcaps
-		and sets its value to the provided default value."""
-		if name in self._global_repcaps:
-			raise Exception(f"Error adding new global repcap: '{name}' already exists in the list.")
-		self._global_repcaps[name] = rep_cap
-
-	def set_global_repcap_value(self, name: str, enum_value: Enum) -> None:
-		"""Updates the existing global repcap value as enum"""
-		if name not in self._global_repcaps:
-			raise Exception(f"Error updating global repcap: '{name}' does not exist in the list.")
-		self._global_repcaps[name].set_enum_value(enum_value)
-
-	def get_global_repcap_value(self, name: str) -> Enum:
-		"""Returns the current global repcap value as enum"""
-		if name not in self._global_repcaps:
-			raise Exception(f"Error retrieving global repcap: '{name}' does not exist in the list.")
-		return self._global_repcaps[name].get_enum_value()
-
-	def _replace_global_repcaps(self, cmd: str) -> str:
-		"""Replaces all the global repcaps in the command: e.g. '<instance>' => '1'.
-		Returns the replaced command."""
-		for name, value in self._global_repcaps.items():
-			cmd_value = value.get_cmd_string_value()
-			cmd = cmd.replace(name, cmd_value)
-		return cmd
+	def query_syst_error(self) -> Tuple[int, str] or None:
+		"""Returns one response to the SYSTEM:ERROR? query.
+		The response is a Tuple of (code: int, message: str)"""
+		error = self._query_str_no_events('SYST:ERR?')
+		if error.startswith('0,') or error.startswith('+0,'):
+			return None
+		return self._parse_err_query_response(error.strip())
 
-	def query_opc(self, timeout: int = 0) -> bool:
-		"""Sends *OPC? query and returns the result.
-		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
-		with self._lock:
-			self.start_send_read_event('*OPC?', False)
-			opc: bool = self._session.query_opc(timeout)
-			self.end_send_read_event()
-			return opc
-
-	def query_all_syst_errors(self, include_codes=True) -> List[str]:
+	def query_all_syst_errors(self) -> List[Tuple[int, str]] or None:
 		"""Returns all errors in the instrument's error queue.
-		If include_codes is False, you only get the error messages without the error codes."""
-		with self._lock:
-			self.start_send_read_event('SYST:ERROR?', False)
-			errors = self._session.query_all_syst_errors()
-			if include_codes is False and errors is not None:
-				errors = [self._parse_err_query_response(x) for x in errors]
-			self.end_send_read_event()
+		If no error is detected, the return value is None."""
+		errors = []
+		while True:
+			entry = self.query_syst_error()
+			if entry is None:
+				break
+			errors.append(entry)
+			if len(errors) > 50:
+				# Safety stop
+				errors.append('query_all_syst_errors - max limit 50 of SYST:ERR? sent.')
+				break
+		if len(errors) == 0:
+			return None
+		else:
 			return errors
 
-	def check_status(self) -> None:
-		"""Throws InstrumentStatusException in case of an error in the instrument's error queue.
-		The procedure is skipped, if the QueryInstrumentStatus is set to false."""
-		with self._lock:
-			if not self.query_instr_status:
-				return
-			call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
-			if call_syst_error:
-				errors = self.query_all_syst_errors(False)
-				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, errors)
-
-	def clear_status(self) -> None:
-		"""Clears instrument's status subsystem."""
-		with self._lock:
+	def _query_stb(self, allow_tout_error_narrow_down: bool = True) -> StatusByte:
+		"""Sends *STB? query and reads the result."""
+		return StatusByte(int(self._query_str_no_events('*STB?', allow_tout_error_narrow_down)))
+
+	def _read_stb(self) -> StatusByte:
+		"""Calls viReadStb and returns the result."""
+		return StatusByte(self._session.read_stb())
+
+	def clear_before_read(self) -> None:
+		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
+
+		# For NRP-Z sessions, skip this completely
+		if self.is_rsnrp_session() or self.skip_clear_status:
+			return
+
+		if not self.vxi_capable:
+			# Non-Vxi session must use *CLS in any case
+			self.write('*CLS')
+			correct = False
+			if self.disable_opc_query:
+				opc = '1'
+			else:
+				opc = self._query_str_no_events('*OPC?')
+			repeat = 0
+			while not correct:
+				if len(opc) <= 2:
+					opc = opc.strip()
+					correct = opc == '0' or opc == '1'
+				if not correct:
+					# Read again with a small VISA timeout
+					opc = self._read_str_timed(5, True)
+				repeat += 1
+				if repeat > 10:
+					break
+
+		stb = self._query_stb()
+		condition = StatusByte.error_queue_not_empty | StatusByte.message_available | StatusByte.event_status_byte
+		if not stb & condition:
+			return
+		repeat = 0
+		# Loop more times to clear the status subsystem
+		while stb & condition:
+			if stb & StatusByte.error_queue_not_empty:
+				self.write('*CLS')
+				_ = self.query_all_syst_errors()
+			if stb & StatusByte.message_available:
+				# Clear output buffer
+				self._flush_junk_data()
+			if stb & StatusByte.event_status_byte:
+				# OPC or error bits in the ESR
+				self.write('*CLS')
+				self.query_and_clear_esr()
+			# Check if the status byte value changed
+			previous_stb = stb
+			stb = self._query_stb()
+			if stb == previous_stb:
+				repeat += 1
+				if repeat > 10:
+					raise RsInstrException(f"Cannot clear the instrument's status subsystem. Status Byte: '{stb}'")
+
+	def _flush_junk_data(self) -> None:
+		"""Reads junk bytes to clear the instrument's output buffer."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		self._read_unknown_len(StreamWriter.as_bin_var(), False)
+
+	def clear(self) -> None:
+		"""Perform VISA viClear conditionally based on the instrument settings."""
+		perform_all = ViClearMode.execute_on_all in self._viclear_exe_mode
+		perform = False
+		if perform_all:
+			perform = True
+		else:
+			# Perform on all is blocked, use the SessionKind to decide
+			if self._interface_type == SessionKind.gpib:
+				perform = ViClearMode.execute_on_gpib in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.serial:
+				perform = ViClearMode.execute_on_serial in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.socket:
+				perform = ViClearMode.execute_on_socket in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.usb:
+				perform = ViClearMode.execute_on_usb in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.vxi11:
+				perform = ViClearMode.execute_on_tcpvxi in self._viclear_exe_mode
+
+		if not perform:
+			return
+
+		if ViClearMode.ignore_error in self._viclear_exe_mode:
+			# noinspection PyBroadException
+			try:
+				self._session.clear()
+			except Exception:
+				pass
+		else:
 			self._session.clear()
-			self._session.clear_before_read()
 
-	def reset(self) -> None:
-		"""Resets the instrument and clears its status."""
-		with self._lock:
-			self.write('*RST', True)
-			self.query_opc()
-			self.clear_status()
-			self.check_status()
+	def is_connection_active(self) -> bool:
+		"""Returns true, if the VISA connection is active and the communication with the instrument still works.
+		This is achieved by:
+		- checking the session property timeout
+		- sending the *IDN? query"""
+		if self._session is None:
+			return False
+		# noinspection PyBroadException
+		try:
+			old_tout = self.visa_timeout
+			self.visa_timeout = 2000
+			self.write(self.cmd_idn)
+			_ = self._read_str_no_events()
+			self.visa_timeout = old_tout
+			return True
+		except Exception:
+			return False
+
+	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
+		"""Internal method to synchronise a command with OPC timeout.
+		Timeout value 0 means the OPC timeout is used."""
+		timeout = self._resolve_opc_timeout(timeout)
+
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		if is_query:
+			InstrumentErrors.assert_query_has_qmark(command, 'Query with OPC')
+		else:
+			InstrumentErrors.assert_cmd_has_no_qmark(command, 'Write with OPC')
 
-	def write(self, cmd: str, block_callback: bool = False) -> None:
-		"""Writes string command to the instrument."""
-		with self._lock:
-			cmd = self._replace_global_repcaps(cmd)
-			self._call_before_write_handler(cmd, block_callback)
-			self._session.write(cmd)
-			if self.opc_query_after_write:
-				self._session.query_opc()
-			if self.on_write_handler:
-				self.send_write_str_event(cmd, False)
-			self.check_status()
-
-	def write_with_opc(self, cmd: str, timeout: int = None, block_callback: bool = False) -> None:
-		"""Writes a OPC-synced command.
-		Also performs error checking if the property self.query_instr_status is set to True.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			cmd = self._replace_global_repcaps(cmd)
-			self._call_before_write_handler(cmd, block_callback)
-			self._session.write_with_opc(cmd, timeout)
-			self._session.query_and_clear_esr()
-			if self.on_write_handler:
-				self.send_write_str_event(cmd, True)
-			self.check_status()
-
-	def write_struct(self, cmd: str, struct: object) -> None:
-		"""Writes command to the instrument with the parameter composed from the entered structure."""
-		with self._lock:
-			worker = ArgStructList(struct)
-			param = worker.compose_cmd_string()
-			cmd += f' {param}'.rstrip()
+		if self._opc_wait_mode == WaitForOpcMode.opc_query:
+			if is_query:
+				raise RsInstrException('Sending a query with OpcQuery synchronization is not possible')
+			stb = self._write_and_query_opc(command, timeout)
+		else:
+			# STB polling
+			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
+			if is_query:
+				end_stb_mask |= StatusByte.message_available
+			if self.vxi_capable:
+				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
+			else:
+				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
+
+		return stb
+
+	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
+		"""Internal method to write a command followed by query_opc().
+		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
+		Timeout value 0 means the OPC timeout is used."""
+		old_tout = self.visa_timeout
+
+		# Change VISA Timeout if necessary
+		if old_tout != timeout:
+			self.visa_timeout = timeout
+		try:
+			# try-catch to set the VISA timeout back
 			self.write(cmd)
+			self.query_opc()
+		finally:
+			if old_tout != timeout:
+				self.visa_timeout = old_tout
+		return self._query_stb()
+
+	def write(self, cmd: str) -> None:
+		"""Writes command to the instrument."""
+		if self.write_delay > 0:
+			time.sleep(self.write_delay / 1000)
+		add_tc = False
+		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
+			add_tc = True
+		cmd_bytes = cmd.encode(self.encoding)
+		if add_tc:
+			cmd_bytes += self._term_char.encode(self.encoding)
+		self._session.write_raw(cmd_bytes)
+
+	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
+		"""Reads data of unknown length to the provided WriteStream.
+		The read is performed in an incremental chunk steps to optimize memory use (for NRP-Z session it is set to fixed self._data_chunk_size):
+			- The first read is performed with the fixed size of 1024 bytes
+			- The 2nd one reads 64 kBytes
+			- The 3rd one reads 128 kBytes
+			- The 4th one reads 256 kBytes and so on, with the max cap of self._data_chunk_size
+		:param stream: [StreamWriter] target for the read data
+		:param allow_chunk_events: [bool] if True, the method can send the chunk_events. If False, sending events is blocked.
+		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first chunk read
+		:return: read data [bytes or string], depending on the parameter binary."""
+		with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
+			if prepend_data and isinstance(prepend_data, str):
+				prepend_data = prepend_data.encode(self.encoding)
+			chunk_ix = 0
+			eot = False
+			while not eot:
+				if self.is_rsnrp_session():
+					chunk_size = self._data_chunk_size
+				else:
+					if chunk_ix == 0:
+						# First read, set 1024 bytes read size
+						chunk_size = 1024
+					elif chunk_ix == 1:
+						chunk_size = 65536
+					else:
+						chunk_size *= 2
+				if chunk_size > self._data_chunk_size:
+					chunk_size = self._data_chunk_size
+				chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
+				if chunk_ix == 0 and prepend_data:
+					chunk = prepend_data + chunk
+				eot = not self._last_status_more_data_available()
+				if not stream.binary:
+					chunk = chunk.decode(self.encoding)
+					if eot:
+						chunk = chunk.rstrip(self._term_char)
+				stream.write(chunk)
+				if self.on_read_chunk_handler and allow_chunk_events:
+					total_size = len(stream) if eot is True else None
+					event_args = EventArgsChunk(stream.binary, chunk_ix, len(chunk), total_size, len(stream), eot, None, chunk if self.io_events_include_data else None)
+					self.on_read_chunk_handler(event_args)
+				chunk_ix += 1
+
+	def _last_status_more_data_available(self):
+		"""Returns True, if the last status signalled that more data is available"""
+		return self.last_status == pyvisa.constants.StatusCode.success_max_count_read
+
+	def _read_str_no_events(self) -> str:
+		"""Reads response from the instrument. The response is then trimmed for trailing LF. \n
+		Sending of any read events is blocked."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		stream = StreamWriter.as_string_var()
+		self._read_unknown_len(stream, False)
+		return stream.content
+
+	def _query_str_no_events(self, query: str, allow_tout_error_narrow_down: bool = True) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF.
+		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str_no_events()
+		except pyvisa.VisaIOError:
+			context = f"Query '{query.rstrip(self._term_char)}'"
+			if allow_tout_error_narrow_down:
+				self._narrow_down_io_tout_error(context + ' - ')
+			else:
+				raise InstrumentErrors.TimeoutException(context)
+		return response
 
-	def write_struct_with_opc(self, cmd: str, struct: object, timeout: int = None) -> None:
-		"""Writes OPC-synced command to the instrument with the parameter composed from the entered structure.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			worker = ArgStructList(struct)
-			param = worker.compose_cmd_string()
-			cmd += f' {param}'.rstrip()
-			self.write_with_opc(cmd, timeout)
-
-	def query_str(self, query: str, block_callback: bool = False) -> str:
-		"""Sends a query and reads response from the instrument.
-		The response is trimmed of any trailing LF characters and has no length limit."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			self._call_pre_query_handler(query, block_callback)
-			response = self._session.query_str(query)
-			self.end_send_read_event()
-			self.check_status()
-			return response
-
-	def query_str_with_opc(self, query: str, timeout: int = None, block_callback: bool = False) -> str:
-		"""Sends a OPC-synced query.
-		Also performs error checking if the self.query_instr_status is true.
-		The response is trimmed of any trailing LF characters and has no length limit.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			self._call_pre_query_handler(query, block_callback)
-			response = self._session.query_str_with_opc(query, timeout)
-			self.end_send_read_event()
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return response
-
-	def query_bin_block_to_stream(self, query: str, stream: StreamWriter) -> None:
-		"""Queries binary data block to the provided stream.
-		Use it for querying data from instrument to a variable or a file.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block(query, stream, True)
-			self.end_send_read_event()
-			self.check_status()
-
-	def query_bin_block(self, query: str) -> bytes:
-		"""Queries binary data block to bytes and returns data as bytes.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			writer = StreamWriter.as_bin_var()
-			self.query_bin_block_to_stream(query, writer)
-			return writer.content
-
-	def query_bin_block_to_file(self, cmd: str, file_path: str, append: bool = False) -> None:
-		"""Queries binary data block to the provided file.
-		If append is False, any existing file content is discarded.
-		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			with StreamWriter.as_bin_file(file_path, append) as writer:
-				self.query_bin_block_to_stream(cmd, writer)
-
-	def query_bin_block_to_stream_with_opc(self, query: str, stream: StreamWriter, timeout: int = None) -> None:
-		"""Sends a OPC-synced query and returns data the provided stream.
-		Use it for querying data from instrument to a variable or a file.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block_with_opc(query, stream, True, timeout)
-			self.end_send_read_event()
-			self._session.query_and_clear_esr()
-			self.check_status()
+	def _query_str_no_events_timed(self, query: str, timeout: int, suppress_read_tout: bool = False) -> str:
+		"""Queries the instrument and reads the response as string.
+		The entered timeout sets the VISA timeout just for this call. You can suppress the timeout error.
+		The length of the string is not limited. The response is then trimmed for trailing LF.
+		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str_timed(timeout, suppress_read_tout)
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error(f"Query with timeout {timeout} ms '{query.rstrip(self._term_char)}' - ", timeout)
+		return response
+
+	def _read_str_timed(self, timeout: int, suppress_read_tout: bool = False) -> str:
+		"""Reads response from the instrument with a VISA timeout temporarily set for the read.
+		The VISA timeout is set back to the previous value before the method finishes even if an exception occurs.
+		Sending of any read events is blocked."""
+		old_visa_tout = self.visa_timeout
+		if suppress_read_tout:
+			try:
+				if timeout != old_visa_tout:
+					self.visa_timeout = timeout
+				data = self._read_str_no_events()
+				return data
+			except TimeoutError:
+				pass
+			finally:
+				self.visa_timeout = old_visa_tout
+		else:
+			try:
+				if timeout != old_visa_tout:
+					self.visa_timeout = timeout
+				data = self._read_str_no_events()
+				return data
+			finally:
+				self.visa_timeout = old_visa_tout
+
+	def _read_str(self) -> str:
+		"""Reads response from the instrument. The response is then trimmed for trailing LF."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		stream = StreamWriter.as_string_var()
+		self._read_unknown_len(stream, True)
+		return stream.content
+
+	def query_str(self, query: str) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str()
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error(f"Query '{query.rstrip(self._term_char)}' - ")
+		return response
+
+	def query_str_no_tout_err(self, query: str, tout: int) -> str:
+		"""Same as query_str, but you can set the timeout just for this one call.
+		If the timeout exception occurs, it is suppressed and the method returns Null"""
+		response = None
+		old_tout = self.visa_timeout
+		try:
+			self.visa_timeout = tout
+			response = self.query_str(query)
+		except (pyvisa.VisaIOError, InstrumentErrors.StatusException):
+			pass
+		finally:
+			self.visa_timeout = old_tout
+		return response
 
-	def query_bin_block_with_opc(self, query: str, timeout: int = None) -> bytes:
-		"""Sends a OPC-synced query and returns data as bytes.
+	def write_with_opc(self, command: str, timeout: int = None) -> None:
+		"""Sends command with OPC-sync.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			with StreamWriter.as_bin_var() as stream:
-				self.query_bin_block_to_stream_with_opc(query, stream, timeout)
-				return stream.content
-
-	def query_bin_block_to_file_with_opc(self, cmd: str, file_path: str, append: bool = False, timeout: int = None) -> None:
-		"""Sends a OPC-synced query and writes the returned data to the provided file.
-		If append is False, any existing file content is discarded.
-		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			with StreamWriter.as_bin_file(file_path, append) as writer:
-				self.query_bin_block_to_stream_with_opc(cmd, writer, timeout)
-
-	def query_int(self, query: str) -> int:
-		"""Sends a query and reads response from the instrument as integer."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0
-			return Conv.str_to_int(string)
+		self._write_and_wait_for_opc(command, False, timeout)
 
-	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
-		"""Sends a OPC-synced query and reads response from the instrument as integer number.
+	def query_str_with_opc(self, query: str, timeout: int = None, context: str = 'Query string with OPC') -> str:
+		"""Query string with OPC synchronization.
+		The response is trimmed for any trailing LF.
 		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0
-			return Conv.str_to_int(string)
-
-	def query_float(self, query: str) -> float:
-		"""Sends a query and reads response from the instrument as float number."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0.0
-			return Conv.str_to_float(string)
+		timeout = self._resolve_opc_timeout(timeout)
+		if self.vxi_capable and self._opc_wait_mode is not WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll or SRQ wait and then read the response
+			stb = self._write_and_wait_for_opc(query, True, timeout)
+			self._check_msg_available_after_opc_wait(stb, query, timeout, context)
+			response = self._read_str()
+		else:
+			# For non-Vxi sessions, use the longer VISA Timeout without the *OPC?
+			# Same is valid for WaitForOpcMode.OpcQuery
+			InstrumentErrors.assert_query_has_qmark(query, 'Query with VISA timeout')
+			self.write(query)
+			old_tout = self.visa_timeout
+			# Change VISA Timeout if necessary
+			if old_tout != timeout:
+				self.visa_timeout = timeout
+			try:
+				# try-catch to set the VISA timeout back
+				response = self._read_str()
+				if self._opc_wait_mode is WaitForOpcMode.opc_query:
+					self.query_opc()
+			finally:
+				if old_tout != timeout:
+					self.visa_timeout = old_tout
 
-	def query_float_with_opc(self, query: str, timeout: int = None) -> float:
-		"""Sends a OPC-synced query and reads response from the instrument as float number.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0.0
-			return Conv.str_to_float(string)
-
-	def query_bool(self, query: str) -> bool:
-		"""Sends a query and reads response from the instrument as boolean value."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return False
-			return Conv.str_to_bool(string)
+		return response
 
-	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
-		"""Sends a OPC-synced query and reads response from the instrument as boolean value.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return False
-			return Conv.str_to_bool(string)
-
-	def query_str_list(self, query: str) -> List[str]:
-		"""Sends a query and reads response from the instrument as csv-list."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
-			return response
+	def query_opc(self, timeout: int = 0) -> bool:
+		"""Sends *OPC? query and reads the result.
+		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
+		if self.disable_opc_query:
+			return True
+		if timeout > 0:
+			response = self._query_str_no_events_timed('*OPC?', timeout)
+		else:
+			response = self._query_str_no_events('*OPC?')
+		return Conv.str_to_bool(response)
 
-	def query_str_list_with_opc(self, query: str, timeout: int = None) -> List[str]:
-		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
-			return response
-
-	def write_bin_block_from_stream(self, cmd: str, stream: StreamReader) -> None:
-		"""Writes all the stream content as binary data block to the instrument.
-		Use it for writing data to instrument from a variable or a file.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
-		with self._lock:
-			if self.on_write_handler:
-				self.start_send_write_bin_event(cmd)
-			self._call_pre_query_handler(cmd, False)
-			self._session.write_bin_block(cmd, stream)
-			self.end_send_write_bin_event()
-			self.check_status()
+	def query_and_clear_esr(self) -> int:
+		"""Sends *ESR? query and reads the result."""
+		response = self._query_str_no_events('*ESR?')
+		return int(response)
+
+	def _check_msg_available_after_opc_wait(self, stb: StatusByte, query: str, timeout: int, context: str) -> None:
+		"""Used internally after _StbPolling() to check if the message is available.
+		Throws an exception in case of MAV not available."""
+		if not self.vxi_capable:
+			return
+		if stb & StatusByte.message_available:
+			return
+		# Message not available
+		context = context + f" Query '{query.rstrip(self._term_char)}'"
+		if stb & StatusByte.error_queue_not_empty:
+			# Instrument reports an error
+			InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context)
+		else:
+			# Sometimes even if the StatusByte.MessageAvailable is false, the message is available.
+			# Try to read the STB again
+			stb = self._read_stb()
+			if not stb & StatusByte.event_status_byte:
+				# Instrument did not respond within the defined time
+				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f'{context} No response from the instrument.')
+
+	def error_in_error_queue(self) -> bool:
+		"""Returns true, if error queue contains at least one error."""
+		stb = self._query_stb()
+		if stb & StatusByte.error_queue_not_empty:
+			return True
+		return False
+
+	def reset_ese_sre(self) -> None:
+		"""Resets the status of ESE and SRE registers to default values."""
+		self._set_regs_ese_sre(self._opc_wait_mode)
 
-	def write_bin_block(self, cmd: str, payload: bytes) -> None:
+	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
 		"""Writes all the payload as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
-		self.write_bin_block_from_stream(cmd, StreamReader.as_bin_var(payload))
+		The binary data header is added at the beginning of the transmission automatically.
+		:param cmd: [str] SCPI command with which to send the data
+		:param data_stream: [StreamReader] data provider for the payload"""
+		data_size = len(data_stream)
+		len_str = f'{data_size}'
+		cmd = cmd.rstrip(self._term_char)
+		if '#' in cmd:
+			raise RsInstrException(
+				f"Command '{cmd}' must be provided without the binary data header. "
+				f"The method 'write_bin_block' composes and prepends the binary data header automatically.")
+		if data_size <= self._std_bin_block_header_max_len:
+			# Standard bin data header for sizes below 1E9 bytes, e.g.: '#512345'
+			cmd_plus_header = f'{cmd}#{len(len_str)}{len_str}'.encode(self.encoding)
+		else:
+			# Big sizes bin data header: e.g.: '#(3000000000)'
+			cmd_plus_header = f'{cmd}#({len_str})'.encode(self.encoding)
 
-	def write_bin_block_from_file(self, cmd: str, file_path: str) -> None:
-		"""Writes all the file content as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the file content!!!"""
-		with StreamReader.as_bin_file(file_path) as reader:
-			self.write_bin_block_from_stream(cmd, reader)
-
-	def query_bin_or_ascii_float_list(self, query: str) -> List[float]:
-		"""Queries a list of floating-point numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32)."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block(query, stream, False)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-			else:
-				result = Conv.str_to_float_list(stream.content)
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None) -> List[float]:
-		"""Sends a OPC-synced query and reads a list of floating-point numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32).
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block_with_opc(query, stream, False, timeout)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-			else:
-				result = Conv.str_to_float_list(stream.content)
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_float_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[float]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return Conv.str_to_float_list(response)
-
-	def query_bin_or_ascii_float_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[float]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
-		If you do not provide timeout, the method uses current opc_timeout.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return Conv.str_to_float_list(response)
-
-	def query_bin_or_ascii_int_list(self, query: str) -> List[int]:
-		"""Queries a list of integer numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32)."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block(query, stream, False)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-			else:
-				result = Conv.str_to_int_list(stream.content)
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_int_list_with_opc(self, query: str, timeout: int = None) -> List[int]:
-		"""Sends a OPC-synced query and reads a list of integer numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32).
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block_with_opc(query, stream, False, timeout)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-			else:
-				result = Conv.str_to_int_list(stream.content)
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_int_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[int]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			response = self.query_str(query)
-			if self._simulating:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			response = self._linker.cut_from_response_string(suppressed, response, query)
-			return Conv.str_to_int_list(response)
-
-	def query_bin_or_ascii_int_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[int]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
-		If you do not provide timeout, the method uses current opc_timeout.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			response = self.query_str_with_opc(query, timeout)
-			if self._simulating:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			response = self._linker.cut_from_response_string(suppressed, response, query)
-			return Conv.str_to_int_list(response)
-
-	def query_struct(self, query: str, struct: object) -> object:
-		"""Queries string of from instrument, and parses it based on the provided structure object.
-		THe method returns the copy of the entered object that it had modified."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return struct
-			struct_list = ArgStructList(struct)
-			struct_list.parse_from_cmd_response(string)
-			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
-			return struct
-
-	def query_struct_with_opc(self, query: str, struct: object, timeout: int = None) -> object:
-		"""Queries string of from instrument, and parses it based on the provided structure object.
-		THe method returns the copy of the entered object that it had modified."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return struct
-			struct_list = ArgStructList(struct)
-			struct_list.parse_from_cmd_response(string)
-			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
-			return struct
-
-	def query_str_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> str:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return string
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return response
-
-	def query_str_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> str:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return string
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return response
-
-	def self_test(self, timeout: int = None) -> Tuple[int, str]:
-		"""Performs instrument's selftest (*TST?).
-		Returns tuple (code:int, message: str). . Code 0 means the self-test passed.
-		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
-		with self._lock:
-			if timeout is None or timeout == 0:
-				timeout = self.selftest_timeout
-			response = self.query_str_with_opc('*TST?', timeout)
-			m = re.search(r'^(-?[\d]+)(,(.*))?', response)
-			if not m:
-				raise InstrumentErrors.UnexpectedResponseException(self.resource_name, f"Unexpected response to a '*TST?' self-test query: '{response}'")
-			code = Conv.str_to_int(m.group(1))
-			msg = Utilities.trim_str_response(m.group(3))
-			self.check_status()
-			return code, msg
+		if data_size <= self._data_chunk_size:
+			# Write all in one step
+			full_chunk = data_stream.read_as_binary(self.encoding)
+			write_buf = cmd_plus_header + full_chunk
+			if self._add_term_char_to_write_bin_block:
+				write_buf += self._term_char_bin
+			self._session.write_raw(write_buf)
+			# Event sending
+			if self.on_write_chunk_handler:
+				event_args = EventArgsChunk(True, 0, data_size, data_size, data_size, True, 1, full_chunk if self.io_events_include_data else None)
+				self.on_write_chunk_handler(event_args)
+		else:
+			# Write in chunks
+			try:
+				# Use finally to set the session send_end back to True
+				self._session.send_end = False
+				total_chunks = calculate_chunks_count(data_size, self._data_chunk_size)
+				chunk_ix = 0
+				if self.write_delay > 0:
+					time.sleep(self.write_delay / 1000)
+				# Write bin header
+				self._session.write_raw(cmd_plus_header)
+				# Write chunks
+				while True:
+					if len(data_stream) > self._data_chunk_size:
+						#  Not the last segment
+						chunk = data_stream.read_as_binary(self.encoding, self._data_chunk_size)
+						self._session.write_raw(chunk)
+						# Event sending
+						if self.on_write_chunk_handler:
+							event_args = EventArgsChunk(
+								True, chunk_ix, self._data_chunk_size, data_size, data_size - len(data_stream), False, total_chunks, chunk if self.io_events_include_data else None)
+							self.on_write_chunk_handler(event_args)
+					else:
+						# Last segment, indicate end of message again
+						chunk = data_stream.read_as_binary(self.encoding)
+						if self._add_term_char_to_write_bin_block:
+							# Append LF
+							self._session.write_raw(chunk)
+							self._session.send_end = True
+							self._session.write_raw(self._term_char_bin)
+						else:
+							self._session.send_end = True
+							self._session.write_raw(chunk)
+
+						# Event sending
+						if self.on_write_chunk_handler:
+							event_args = EventArgsChunk(True, chunk_ix, len(chunk), data_size, data_size, True, total_chunks, chunk if self.io_events_include_data else None)
+							self.on_write_chunk_handler(event_args)
+						break
+					chunk_ix += 1
+			finally:
+				self._session.send_end = True
+
+	def _parse_bin_data_header(self, exc_if_not_bin: bool) -> Tuple[ReadDataType, str, int]:
+		"""Parses the binary data block and returns the expected length of the following data block. \n
+		:param exc_if_not_bin: [bool] if True, the method throws exception in case the data is not binary.
+		:return: read_data_type: [ReadDataType], parsed_header: [string], bin_data_len: [integer]"""
+		length = -1
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+
+		char: AnyStr = self._session.read_bytes(1, break_on_termchar=True)
+		if char == b'#':
+			# binary transfer
+			char = self._session.read_bytes(1, break_on_termchar=True)
+			if char == b'0':
+				data_type = ReadDataType.bin_unknown_len
+				return data_type, '#0', -1
+			if char == b'(':
+				# format for big lengths i.e. > 1E9 bytes: '#(1234567890123)...'
+				data_type = ReadDataType.bin_known_len
+				len_str = (self.read_up_to_char(b')', 100)[:-1]).decode(self.encoding)
+				whole_hdr = '#(' + len_str + ')'
+				length = int(len_str)
+				return data_type, whole_hdr, length
+
+			# classic format for < 1E9 bytes: '#9123456789...'
+			data_type = ReadDataType.bin_known_len
+			len_of_len = int(char)
+			len_str = self._session.read_bytes(len_of_len).decode(self.encoding)
+			length = int(len_str)
+			whole_hdr = '#' + char.decode(self.encoding) + len_str
+			return data_type, whole_hdr, length
+
+		data_type = ReadDataType.ascii
+		if char == self._term_char_bin:
+			data_type = ReadDataType.null
+		if self.vxi_capable:
+			# For Vxi session, to be sure, check whether there are more chars in the read buffer
+			stb = self._read_stb()
+			if stb & StatusByte.message_available:
+				data_type = ReadDataType.ascii
+		whole_hdr = char.decode(self.encoding)
+		if exc_if_not_bin:
+			if data_type == ReadDataType.null:
+				InstrumentErrors.throw_bin_block_unexp_resp_exception(self.resource_name, self._term_char)
+			# Read 20 more characters to compose a better exception message
+			whole_hdr += self.read_up_to_char(self._term_char_bin, 20).decode(self.encoding)
+			if self.last_status == pyvisa.constants.StatusCode.success_max_count_read:
+				self._flush_junk_data()
+			InstrumentErrors.throw_bin_block_unexp_resp_exception(self.resource_name, whole_hdr)
+		return data_type, whole_hdr, length
+
+	def get_bin_data_length(self, query: str) -> int or None:
+		"""Returns only the length binary data header, and discards the actual data.
+		Any timeout error is suppressed, and the method returns None instead.
+		Warning!!! - for non-VXI sessions (SOCKET, ASRL) this method transfers the entire file to the control PC, which might take a long time."""
+		if self.vxi_capable and self._opc_wait_mode != WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll and read the header
+			stb = self._write_and_wait_for_opc(query, True, 0)
+			try:
+				self._check_msg_available_after_opc_wait(stb, query, 0, 'get_bin_data_length')
+			except InstrumentErrors.StatusException:
+				return None
+			data_type, header, length = self._parse_bin_data_header(True)
+			self.clear()
+			self.clear_before_read()
+			return length
+		else:
+			with StreamWriter.as_forget() as stream:
+				old_timeout = self.visa_timeout
+				try:
+					self.visa_timeout = 2000
+					self.query_bin_block(query, stream, True)
+				except InstrumentErrors.StatusException:
+					return None
+				finally:
+					self.visa_timeout = old_timeout
+				length = stream.written_len
+		return length
+
+	def read_bin_block(self, stream: StreamWriter, exc_if_not_bin: bool) -> None:
+		"""Reads binary data block to the provided stream. \n
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: if True, the method throws exception if the received data is not binary"""
+		data_type, header, length = self._parse_bin_data_header(exc_if_not_bin)
+		if data_type == ReadDataType.ascii:
+			stream.switch_to_string_data(self.encoding)
+			self._read_unknown_len(stream, True, header)
+		elif data_type == ReadDataType.null:
+			# No data, consider it ASCII. Change the stream type to ASCII and return empty string
+			stream.switch_to_string_data(self.encoding)
+		elif data_type == ReadDataType.bin_unknown_len:
+			if not self.vxi_capable:
+				raise RsInstrException(f'Non-Vxi11 sessions can not read binary data block of unknown length.')
+			self._read_unknown_len(stream, True)
+		elif length == 0:
+			self._flush_junk_data()
+		else:
+			self._read_bin_block_known_len(stream, length)
+
+	def _read_bin_block_known_len(self, stream: StreamWriter, length: int) -> None:
+		"""Reads binary data of defined length. All remaining data above the length are disposed of. \n
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param length: [int] expected length of the data"""
+		# Use try-catch to switch the termination character back ON in case of an exception (for non-Vxi sessions)
+		try:
+			# Binary transmission, for non-Vxi session, set the termination character to OFF
+			if not self.vxi_capable:
+				self._session.read_termination = False
+			# Binary data of known length
+			left_to_read = length
+			self.last_status = pyvisa.constants.StatusCode.success
+			with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
+				chunk_ix = 0
+				total_chunks = calculate_chunks_count(length, self._data_chunk_size)
+				while len(stream) < length:
+					chunk_size = min(self._data_chunk_size, left_to_read)
+					chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
+					left_to_read -= len(chunk)
+					stream.write(chunk)
+					if self.on_read_chunk_handler:
+						event_args = EventArgsChunk(True, chunk_ix, chunk_size, length, len(stream), left_to_read == 0, total_chunks, chunk if self.io_events_include_data else None)
+						self.on_read_chunk_handler(event_args)
+					chunk_ix += 1
+			if self._last_status_more_data_available():
+				if not self.vxi_capable:
+					self._session.read_termination = self._term_char
+				self._flush_junk_data()
+		finally:
+			# Make sure that in any case the self._session.read_termination is ON again for non-Vxi sessions
+			if not self.vxi_capable:
+				self._session.read_termination = self._term_char
+
+	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
+		"""Query binary data block and returns it as byte data. \n
+		:param query: [str] query to send to the instrument
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary"""
+		self.write(query)
+		try:
+			self.read_bin_block(stream, exc_if_not_bin)
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error(f"Query bin block '{query.rstrip(self._term_char)}' - ")
+		return
+
+	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
+		"""Query binary data block with OPC and returns it as byte data.
+		:param query: [str] query to send to the instrument
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary
+		:param timeout: Optional[Integer] timeout for the operation. If you skip it, the method uses the current opc timeout."""
+		timeout = self._resolve_opc_timeout(timeout)
+		if self.vxi_capable and self._opc_wait_mode != WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll and read the response
+			stb = self._write_and_wait_for_opc(query, True, timeout)
+			self._check_msg_available_after_opc_wait(stb, query, timeout, 'query_bin_block_with_opc')
+			self.read_bin_block(stream, exc_if_not_bin)
+		else:
+			# For non-Vxi session, use the longer VISA Timeout without the *OPC
+			InstrumentErrors.assert_query_has_qmark(query, 'query_bin_block_with_opc')
+			self.write(query)
+			old_visa_timeout = self.visa_timeout
+			# Change VISA Timeout if necessary
+			if old_visa_timeout != timeout:
+				self.visa_timeout = timeout
+			try:
+				# try-catch to set the VISA timeout back
+				self.read_bin_block(stream, exc_if_not_bin)
+				if self._opc_wait_mode == WaitForOpcMode.opc_query:
+					self.query_opc()
+			finally:
+				# Change VISA Timeout back if necessary
+				if old_visa_timeout != timeout:
+					self.visa_timeout = old_visa_timeout
+
+	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
+		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
+		Returns the read data including the stop character."""
+		response = b''
+		for i in range(max_cnt):
+			char, self.last_status = self._session.visalib.read(self._session.session, 1)
+			response += char
+			if char in stop_chars:
+				break
+			if self.last_status != pyvisa.constants.StatusCode.success_max_count_read:
+				break
+		return response
+
+	def go_to_local(self) -> None:
+		"""Puts the instrument into local state."""
+		if self.vxi_capable:
+			self._session.control_ren(pyvisa.constants.RENLineOperation.deassert_gtl)
+		else:
+			self.write("&GTL")
+
+	def go_to_remote(self) -> None:
+		"""Puts the instrument into remote state."""
+		if self.vxi_capable:
+			self._session.control_ren(pyvisa.constants.RENLineOperation.asrt_address)
+		else:
+			self.write("&GTR")
 
 	def get_session_handle(self) -> object:
 		"""Returns the underlying pyvisa session."""
-		return self._session.get_session_handle()
+		return self._session
 
 	def close(self) -> None:
-		"""Closes the Instrument session."""
-		with self._lock:
+		"""Closes the Visa session.
+		If the object was created with the direct session input, the session is not closed."""
+		if not self.reusing_session:
 			self._session.close()
-			self._session = None
 
-	# Events part
+	# Events
 
-	@property
-	def io_events_include_data(self) -> bool:
-		"""If true, the read and write handlers also include read and written data."""
-		return self._io_events_include_data
-
-	@io_events_include_data.setter
-	def io_events_include_data(self, value: bool) -> None:
-		"""If true, the read and write handlers also include read and written data."""
-		self._io_events_include_data = value
-		self._session.io_events_include_data = value
-
-	def event_args_append_instr_info(self, args: IoTransferEventArgs) -> IoTransferEventArgs:
-		"""Appends instrument-related information to the read/write event argument"""
-		args.chunk_size = self.data_chunk_size
-		args.resource_name = self.resource_name
-		return args
-
-	def send_write_str_event(self, cmd: str, opc_sync: bool) -> None:
-		"""Creates and sends write string event. The transfer is marked as done (end_of_transfer = True)."""
-		args = IoTransferEventArgs.write_str(opc_sync, len(cmd), cmd)
-		args.transferred_size = args.total_size
-		args.chunk_ix = 0
-		args.end_of_transfer = True
-		args = self.event_args_append_instr_info(args)
-		if self._io_events_include_data:
-			args.data = cmd
-		self.on_write_handler(args)
-
-	def start_send_read_event(self, query: str, opc_sync: bool) -> None:
-		"""Registers VisaSession.on_read_chunk_handler() which then generates events with each chunk transfer.
-		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_read_handler()"""
-		if not self.on_read_handler:
-			return
 
-		def _read_chunk_handler(visa_args: EventArgsChunk) -> None:
-			"""Receives events from VisaSession on read chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_read_handler()"""
-			args.end_of_transfer = visa_args.end_of_transfer
-			args.chunk_ix = visa_args.chunk_ix
-			args.total_chunks = visa_args.total_chunks
-			args.chunk_size = visa_args.chunk_size
-			args.transferred_size = visa_args.transferred_size
-			args.total_size = visa_args.total_size
-			args.data = visa_args.data
-			args.binary = visa_args.binary
-			self.on_read_handler(args)
-
-		args = IoTransferEventArgs.read_chunk(opc_sync, query)
-		args = self.event_args_append_instr_info(args)
-		self._session.on_read_chunk_handler = _read_chunk_handler
-
-	def end_send_read_event(self):
-		"""Unregisters VisaSession.on_read_chunk_handler()"""
-		self._session.on_read_chunk_handler = None
-
-	def start_send_write_bin_event(self, cmd: str) -> None:
-		"""Registers VisaSession.on_write_chunk_handler() which then generates events with each chunk transfer.
-		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_write_handler()"""
-		if not self.on_write_handler:
-			return
+class EventArgsChunk:
+	"""Event arguments for chunk io event."""
 
-		def _write_chunk_handler(visa_args: EventArgsChunk) -> None:
-			"""Receives events from VisaSession on write chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_write_handler()"""
-			args.end_of_transfer = visa_args.end_of_transfer
-			args.chunk_ix = visa_args.chunk_ix
-			args.total_chunks = visa_args.total_chunks
-			args.chunk_size = visa_args.chunk_size
-			args.transferred_size = visa_args.transferred_size
-			args.total_size = visa_args.total_size
-			args.data = visa_args.data
-			args.binary = visa_args.binary
-			self.on_write_handler(args)
-
-		args = IoTransferEventArgs.write_bin(cmd)
-		args = self.event_args_append_instr_info(args)
-		self._session.on_write_chunk_handler = _write_chunk_handler
-
-	def end_send_write_bin_event(self):
-		"""Unregisters VisaSession.on_write_chunk_handler()"""
-		self._session.on_write_chunk_handler = None
-
-	def _call_before_write_handler(self, cmd: str, block_callback: bool) -> None:
-		"""Calls the _pre_write_handler if defined. Used in all the base write methods."""
-		if block_callback is False and self._before_write_handler:
-			self._before_write_handler(self, cmd)
-
-	def _call_pre_query_handler(self, query: str, block_callback: bool) -> None:
-		"""Calls the _pre_query_handler if defined. Used in all the base query methods."""
-		if block_callback is False and self._before_query_handler:
-			self._before_query_handler(self, query)
+	def __init__(
+			self,
+			binary: bool,
+			chunk_ix: int,
+			chunk_size: int,
+			total_size: int,
+			transferred_size: int,
+			end_of_transfer: bool,
+			total_chunks: int or None,
+			data: AnyStr = None):
+
+		self.binary = binary
+		self.chunk_ix = chunk_ix
+		self.total_chunks = total_chunks
+		self.chunk_size = chunk_size
+		self.transferred_size = transferred_size
+		self.total_size = total_size
+		self.end_of_transfer = end_of_transfer
+		self.data = data
 
-	@property
-	def before_write_handler(self) -> Callable:
-		"""Returns the handler of before_write events. \n
-		:return: current before_write_handler"""
-		return self._before_write_handler
-
-	@before_write_handler.setter
-	def before_write_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_write events.
-		The before_write event is invoked before each write operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, cmd: str)
-		:param handler: new handler"""
-		self._before_write_handler = handler
-
-	@property
-	def before_query_handler(self) -> Callable:
-		"""Returns the handler of before_query events. \n
-		:return: current before_query_handler"""
-		return self._before_query_handler
-
-	@before_query_handler.setter
-	def before_query_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_query events.
-		The before_query event is invoked before each query operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, query: str)
-		:param handler: new handler"""
-		self._before_query_handler = handler
+	def __str__(self):
+		if self.binary:
+			type_info = 'binary'
+		else:
+			type_info = 'ascii'
+		if not self.total_chunks:
+			chunk_info = f' chunk nr. {self.chunk_ix + 1}'
+		elif self.total_chunks > 1:
+			chunk_info = f' chunk nr. {self.chunk_ix + 1}/{self.total_chunks}'
+		else:
+			chunk_info = ' chunk nr. 1/1'
+		eot = ' (EOT)' if self.end_of_transfer else ''
+		result = \
+			f'EventArgsChunk {type_info},{chunk_info}, {size_to_kb_mb_string(self.chunk_size, True)}, ' \
+			f'sum {size_to_kb_mb_string(self.transferred_size, True)} / {size_to_kb_mb_string(self.total_size, True) if self.total_size else "<N.A.>"}{eot}.'
+		return result
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/InstrumentErrors.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentErrors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,79 @@
+"""Definition of RsInstrument exceptions, assert functions, and other error-related functions."""
+
+from typing import List, Tuple
+
+
 class RsInstrException(Exception):
 	"""Exception base class for all the RsInstrument exceptions."""
 	def __init__(self, message: str):
 		super(RsInstrException, self).__init__(message)
+		self.message = message
 
 
 class TimeoutException(RsInstrException):
 	"""Exception for timeout errors."""
 	def __init__(self, message: str):
 		super(TimeoutException, self).__init__(message)
 
 
 class StatusException(RsInstrException):
-	"""Exception for instrument status errors."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+	"""Exception for instrument status errors.
+	Tje field  errors_list contains the complete list of all the errors with messages and codes."""
+	def __init__(self, rsrc_name: str, message: str, errors_list: List[Tuple[int, str]], first_exc: Exception = None):
+		self.rsrc_name: str = rsrc_name
+		self.first_exc: Exception = first_exc
+		self.errors_list: List[Tuple[int, str]] = errors_list
 		super(StatusException, self).__init__(message)
 
 
 class UnexpectedResponseException(RsInstrException):
 	"""Exception for instrument unexpected responses."""
 	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+		self.rsrc_name: str = rsrc_name
 		super(UnexpectedResponseException, self).__init__(message)
 
 
 class ResourceError(RsInstrException):
 	"""Exception for resource name - e.g. resource not found."""
 	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+		self.rsrc_name: str = rsrc_name
 		super(ResourceError, self).__init__(message)
 
 
 class DriverValueError(RsInstrException):
 	"""Exception for different driver value settings e.g. RepCap values or Enum values."""
 	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+		self.rsrc_name: str = rsrc_name
 		super(DriverValueError, self).__init__(message)
 
 
-def assert_no_instrument_status_errors(rsrc_name: str, errors: list, context: str = '') -> None:
-	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
-	if errors is None:
-		return
-	if len(errors) == 0:
+def get_instrument_status_errors(rsrc_name: str, errors: List[Tuple[int, str]], context: str = '') -> str or None:
+	"""Checks the errors list and of it contains at least one element, it returns the error message.
+	Otherwise, it returns None."""
+	if errors is None or len(errors) == 0:
 		return
 	if context:
 		message = f"'{rsrc_name}': {context} "
 	else:
 		message = f"'{rsrc_name}': "
+	errors_msg = '\n'.join([f'{x[0]},"{x[1]}"' for x in errors])
 	if len(errors) == 1:
-		message += f'Instrument error detected: {errors[0]}'
-		raise StatusException(rsrc_name, message)
+		message += f'Instrument error detected: {errors_msg}'
+		return message
 	if len(errors) > 1:
-		message += '{} Instrument errors detected:\n{}'.format(len(errors), '\n'.join(errors))
-		raise StatusException(rsrc_name, message)
+		message += f'{len(errors)} Instrument errors detected:\n{errors_msg}'
+		return message
+
+
+def assert_no_instrument_status_errors(rsrc_name: str, errors: List[Tuple[int, str]], context: str = '', first_exc=None) -> None:
+	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
+	msg = get_instrument_status_errors(rsrc_name, errors, context)
+	if msg:
+		raise StatusException(rsrc_name, msg, errors, first_exc=first_exc)
 
 
 def throw_opc_tout_exception(opc_tout: int, used_tout: int, context: str = '') -> None:
 	"""Throws TimeoutException - use it for any timeout error."""
 	if not context:
 		message = ''
 	else:
@@ -83,21 +99,21 @@
 
 def assert_query_has_qmark(query: str, context: str = '') -> None:
 	"""Throws Exception if the query does not contain any question marks."""
 	if '?' in query:
 		return
 	message = ''
 	if context:
-		message = ' ' + context
+		message = context.strip() + ': '
 	message = message + "Query commands must contain question-marks. Sent query: '{0}'".format(query.strip('\n'))
-	raise Exception(message)
+	raise RsInstrException(message)
 
 
 def assert_cmd_has_no_qmark(command: str, context: str = '') -> None:
 	"""Throws Exception if the query contains a question marks."""
 	if '?' not in command:
 		return
 	message = ''
 	if context:
-		message = ' ' + context
+		message = context.strip() + ': '
 	message = message + "Set commands must not contain question-marks. Sent command: '{0}'".format(command.strip('\n'))
-	raise Exception(message)
+	raise RsInstrException(message)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/InstrumentOptions.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentOptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the class docstring."""
+
 import re
 from enum import Enum
 
 from .Utilities import trim_str_response
 
 
 class ParseMode(Enum):
@@ -10,14 +12,15 @@
 	KeepOriginal = 1
 	KeepBeforeDash = 2
 	KeepAfterDash = 3
 	Auto = 4
 
 
 class Options(object):
+	"""Class for handling the instrument options - parsing from the *OPT? string and providing method get_all()"""
 	_optionsList = []
 
 	def __init__(self, options_str: str, mode=ParseMode.Auto):
 		"""Initializes the options with the *OPT? return string."""
 		self._initialize_from_string(options_str, mode)
 
 	def __str__(self):
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/InternalLinker.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InternalLinker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Links a variable from a structure to a callback in the driver."""
+
 from time import time
 from typing import Dict, Callable
 
 from . import ArgSingle, ArgSingleSuppressed
 from .ArgLinkedEventArgs import ArgLinkedEventArgs
 from .Utilities import get_plural_string
+from .InstrumentErrors import RsInstrException
 
 
 class InternalLinker(object):
 	"""Class for:
 		- cutting out suppressed arguments from a device response.
 		- invoking a handler if the argument has InternalLinking defined.
 		- holds dictionary of handlers where the dict_key is the InternalLinking string.
@@ -44,22 +47,22 @@
 		Returns number of deleted links."""
 		count = len(self._handlers)
 		self._handlers = {}
 		return count
 
 	def cut_from_response_string(self, arg: ArgSingleSuppressed, response: str, context: str) -> str:
 		"""Takes the string 'response', removes the suppressed argument value from it and returns the rest.
-		The cut out part is sent via handler if the internal linking exists for that argument exists."""
+		The cut-out part is sent via handler if the internal linking exists for that argument exists."""
 		result = ''
 		if arg.argument_ix is None:
-			raise Exception(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
+			raise RsInstrException(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
 		if arg.argument_ix != 0:
-			raise Exception(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
+			raise RsInstrException(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
 		if arg.is_open_list:
-			raise Exception(f'Open List arguments can not be suppressed. Argument: {arg}')
+			raise RsInstrException(f'Open List arguments can not be suppressed. Argument: {arg}')
 		repetition = 0
 		i = 0
 		for c in response:
 			if c == ',':
 				repetition += 1
 			if repetition == arg.repetition:
 				break
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the docstring for the IoTransferEventArgs class."""
+
 import itertools
 from typing import AnyStr
 
 from .Utilities import size_to_kb_mb_string
 
 
 class IoTransferEventArgs(object):
@@ -48,25 +50,25 @@
 		return cls(True, opc_sync, None, context)
 
 	@classmethod
 	def write_str(cls, opc_sync: bool, total_size: int, context: str) -> 'IoTransferEventArgs':
 		"""Creates new IoTransferEventArgs of write string \n
 		:param opc_sync: defines if the command is OPC-synchronised
 		:param total_size: size of the data to write
-		:param context: SCPI command write. It is truncated to maximum of 100 characters.
-		:return: IoTransferEventArgs object of a write string operation."""
+		:param context: SCPI command write. It is truncated to maximum of 100 characters
+		:return: IoTransferEventArgs object of a write-string operation."""
 		obj = cls(False, opc_sync, total_size, context)
 		obj.binary = False
 		return obj
 
 	@classmethod
 	def write_bin(cls, context: str) -> 'IoTransferEventArgs':
 		"""Creates new IoTransferEventArgs of read binary data \n
 		:param context: SCPI command. It is truncated to maximum of 100 characters.
-		:return: IoTransferEventArgs object of a write binary data operation."""
+		:return: IoTransferEventArgs object of a write-binary-data operation."""
 		# noinspection PyTypeChecker
 		obj = cls(False, False, None, context.rstrip())
 		obj.binary = True
 		return obj
 
 	def __str__(self):
 		if self.binary:
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/RepeatedCapability.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/RepeatedCapability.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the docstring for the RepeatedCapability class."""
+
 from enum import Enum
 
 
 # Command integer value that signals Default value "DEFAULT"
 VALUE_DEFAULT = -1
 
 # Command integer value that signals "EMPTY"
@@ -26,39 +28,47 @@
 	def __str__(self) -> str:
 		out = f'RepCap {self.name}'
 		if self._enum_value is not None:
 			out += f" = {self._enum_value}"
 		return out
 
 	@classmethod
-	def clsm_assert_type(cls, enum_value: Enum, enum_type) -> None:
-		"""Static assertion function to check if the entered value is a member of the defined repcap enum"""
+	def clsm_assert_type(cls, enum_value: Enum or int, enum_type) -> None:
+		"""Static assertion function to check if the entered value is a member of the defined repcap enum.
+		In addition, the integer value is also supported."""
+		if isinstance(enum_value, int):
+			return
 		if not isinstance(enum_value, enum_type):
 			raise TypeError(f"RepCap value must be of type '{enum_type}'. Entered value type: {type(enum_value)}, value '{enum_value}'")
 
 	@classmethod
-	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum, enum_type) -> int:
+	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum or int, enum_type) -> int:
 		"""Static function to get an integer interpretation of a direct enum value
 		Does not work with Empty or Default"""
 		RepeatedCapability.clsm_assert_type(enum_value, enum_type)
+		if isinstance(enum_value, int):
+			return enum_value
 		return enum_value.value
 
 	@classmethod
-	def clsm_is_default_value(cls, enum_value: Enum, enum_type) -> bool:
+	def clsm_is_default_value(cls, enum_value: Enum or int, enum_type) -> bool:
 		"""Returns True, if the entered value is enum.Default"""
 		return cls.clsm_get_direct_cmd_value_int(enum_value, enum_type) == VALUE_DEFAULT
 
 	def is_default_value(self) -> bool:
 		"""Returns True, if the repcap value is enum.Default"""
 		return RepeatedCapability.clsm_is_default_value(self._enum_value, self.enum_type)
 
-	def set_enum_value(self, enum_value: Enum) -> None:
+	def set_enum_value(self, enum_value: Enum or int) -> None:
 		"""Sets new enum value. Can not be Default"""
 		if RepeatedCapability.clsm_is_default_value(enum_value, self.enum_type):
 			raise ValueError(f"Setting RepCap enum value '{enum_value}' is not allowed. Please select a concrete value")
+		if isinstance(enum_value, int):
+			# Find the enum value that corresponds to the entered integer value
+			enum_value = self.enum_type(enum_value)
 		self._enum_value = enum_value
 
 	def get_enum_value(self) -> Enum:
 		"""Returns the actual enum value"""
 		return self._enum_value
 
 	def set_to_start_value(self) -> None:
@@ -66,16 +76,17 @@
 		self.set_enum_value(self._start_value)
 
 	def matches_type(self, enum_type) -> bool:
 		"""Returns true, if the entered type matches the EnumType"""
 		return self.enum_type == enum_type
 
 	@classmethod
-	def clsm_get_cmd_string_value(cls, enum_value: Enum, enum_type) -> str:
-		"""Converts RepCap integer value to string
+	def clsm_get_cmd_string_value(cls, enum_value: Enum or int, enum_type) -> str:
+		"""Class method version of the get_cmd_string_value().
+		Converts RepCap integer value to string
 		ValueEmpty is converted to "" (Not valid, but tolerated)
 		ValueDefault throws an exception
 		0 is converted to "" (Not valid, but tolerated)
 		Positive numbers are converted to integer strings e.g. 1 => '1' """
 		number = cls.clsm_get_direct_cmd_value_int(enum_value, enum_type)
 		if number == VALUE_EMPTY:
 			return ''
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/StreamReader.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamReader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+"""See the docstring for the StreamReader class."""
+
 from enum import Enum
 from os import path
 from typing import AnyStr
 
 from .Utilities import size_to_kb_mb_string
+from .InstrumentErrors import RsInstrException
 
 
 class Type(Enum):
+	"""Defines type of the stream - variable or file."""
 	Variable = 1
 	File = 2
 
 
 class StreamReader:
 	"""Lightweight stream reader implementation. Data source can be: \n
 	- variable
@@ -21,31 +25,32 @@
 		:param source: Source type for the stream. Variable / File
 		:param data: Depending on the 'binary' and 'source':
 		For source type Variable the data must be either bytes() or str
 		For source type File data must be string with existing file path."""
 		self._source = source
 		self._binary = binary
 		self._start_ptr = 0
+		self._read_len = 0
 
 		if self._source == Type.Variable:
 			if self._binary:
 				assert isinstance(data, bytes), f'Data must be of bytes type. Actual type: {type(data)}'
 			else:
 				assert isinstance(data, str), f'Data must be of string type. Actual type: {type(data)}'
 			self._data = data
 			self._full_len = len(self._data)
 		elif self._source == Type.File:
 			assert isinstance(data, str), f'Data must be of string type (file path). Actual type: {type(data)}'
 			if not path.isfile(data):
-				raise Exception(f'File does not exist. File path: {data}')
+				raise RsInstrException(f'File does not exist. File path: {data}')
 			self.file_path = data
 			self._data = open(self.file_path, 'rb' if self._binary else 'r')
 			self._full_len = path.getsize(self.file_path)
 		else:
-			raise Exception(f'StreamReader unknown type {source}')
+			raise RsInstrException(f'StreamReader unknown type {source}')
 
 	@classmethod
 	def as_bin_var(cls, data: bytes) -> 'StreamReader':
 		"""Creates new StreamReader from bytes.
 		:param data: [bytes] data for the stream."""
 		return cls(True, Type.Variable, data)
 
@@ -100,29 +105,34 @@
 		If the remaining length is smaller than the chunk_size, the method returns the remaining length only.
 		:param chunk_size: chunk to read. If not set, the method reads the entire data."""
 		assert self._data is not None, 'StreamReader buffer is invalid. You have probably closed it already.'
 		chunk_size = len(self) if chunk_size is None else chunk_size
 		chunk_size = min(chunk_size, len(self))
 		if chunk_size < 0:
 			raise ValueError(f'Chunk size can not be negative number: {chunk_size}')
-
+		self._read_len += chunk_size
 		if self._source == Type.Variable:
 			self._start_ptr += chunk_size
 			return self._data[self._start_ptr - chunk_size: self._start_ptr]
 		elif self._source == Type.File:
 			self._start_ptr += chunk_size
 			return self._data.read(chunk_size)
 
-	def read_as_binary(self, chunk_size: int = None) -> bytes:
+	@property
+	def read_len(self) -> int:
+		"""Returns number of bytes read from the stream since its creation."""
+		return self._read_len
+
+	def read_as_binary(self, encoding: str, chunk_size: int = None) -> bytes:
 		"""Same as read(), but always returns the data in binary format.
 		Practically works exactly as read() for binary streams.
-		For string streams, the method converts the returned data using utf-8 encoding to bytes()."""
+		For string streams, the method converts the returned data using the provided encoding to bytes()."""
 		if self._binary:
 			return self.read(chunk_size)
 		else:
-			return self.read(chunk_size).encode('utf-8')
+			return self.read(chunk_size).encode(encoding)
 
 	def close(self):
 		"""Closes the StreamReader. You can not use its instance afterwards."""
 		if self._source == Type.File and self._data:
 			self._data.close()
 		self._data = None
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/StreamWriter.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamWriter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+"""See the docstring for the StreamWriter class."""
+
 from enum import Flag
 from typing import AnyStr
+from io import BytesIO, StringIO
 
 from .Utilities import size_to_kb_mb_string
+from .InstrumentErrors import RsInstrException
 
 
 class Type(Flag):
+	"""Defines type of the stream - variable or file."""
 	Variable = 1
-	File = 2
-	FileAppend = 6
+	Forget = 2
+	File = 4
+	FileAppend = 12
 
 
 class StreamWriter:
 	"""Lightweight stream writer implementation. Data target can be: \n
 	- bytes
 	- string
 	- file"""
@@ -19,41 +25,48 @@
 	def __init__(self, binary: bool, target: Type, meta_data=None):
 		"""Initializes StreamWriter instance.\n
 		:param binary: True: Binary data, False: ASCII data
 		:param target: Target for the stream. Variable / File (FileAppend)
 		:param meta_data: Only valid for File and FileAppend - define file path as string:
 		For Type.File, data must be string with file path. If the file exists, it will be overwritten.
 		For Type.FileAppend, data must be string with file path. If the file exists, it will be appended."""
-		self._binary = binary
-		self._written_len = 0
+		self._binary: bool = binary
+		self._written_len: int = 0
 		self._target = target
 
 		if Type.Variable in self._target:
 			assert meta_data is None, f'You can not define input meta_data for a Variable StreamWriter.'
-			self._data: AnyStr = bytes() if binary else ''
+			self._data = BytesIO() if binary else StringIO()
+		elif Type.Forget in self._target:
+			self._data: AnyStr = ''
 		elif Type.File in self._target:
 			assert isinstance(meta_data, str), f'Additional data must be of string type (file path). Actual type: {type(meta_data)}'
 			self._file_path = meta_data
 			mode = 'w' if self._target == Type.File else 'a'
 			mode += 'b' if self._binary else ''
 			self._data = open(self._file_path, mode)
 		else:
-			raise Exception(f'StreamWriter unknown target {target}')
+			raise RsInstrException(f'StreamWriter unknown target {target}')
 
 	@classmethod
 	def as_bin_var(cls) -> 'StreamWriter':
 		"""Creates new StreamWriter with bytes variable."""
 		return cls(True, Type.Variable)
 
 	@classmethod
 	def as_string_var(cls) -> 'StreamWriter':
 		"""Creates new StreamWriter with string variable."""
 		return cls(False, Type.Variable)
 
 	@classmethod
+	def as_forget(cls) -> 'StreamWriter':
+		"""Creates new StreamWriter which writes to nowhere - forgets the data."""
+		return cls(False, Type.Forget)
+
+	@classmethod
 	def as_bin_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
 		"""Creates new StreamWriter to binary file.
 		:param file_path: [str] Path to the file.
 		:param append: Optional [bool] If True, the content is appended to the existing content."""
 		return cls(True, Type.FileAppend if append else Type.File, file_path)
 
 	@classmethod
@@ -67,14 +80,16 @@
 		if Type.Variable in self._target:
 			mode = 'binary' if self._binary else 'string'
 			return f'StreamWriter {mode} variable, current size {size_to_kb_mb_string(len(self), True)}'
 		if Type.File in self._target:
 			mode = 'binary' if self._binary else 'text'
 			append = ' appended' if Type.FileAppend in self._target else ''
 			return f'StreamWriter {mode} file{append}, current{append} size {size_to_kb_mb_string(len(self), True)}, file: {self._file_path}'
+		if Type.Forget in self._target:
+			return 'StreamWriter to nowhere.'
 
 	def __len__(self):
 		"""Returns remaining length."""
 		return self._written_len
 
 	def __enter__(self):
 		return self
@@ -88,49 +103,62 @@
 		File streams are always binary."""
 		return self._binary
 
 	def write(self, data: AnyStr) -> None:
 		"""Writes chunk to the stream.
 			- For Type.Bytes data must be bytes.
 			- For Type.String, data must be string.
-			- For Type.File and Type.FileAppend, data must be bytes"""
+			- For Type.File and Type.FileAppend, data must be bytes."""
+		if Type.Forget in self._target:
+			self._written_len += len(data)
+			return
+
 		assert self._data is not None, 'StreamWriter buffer is invalid. You have probably closed it already.'
 		if self._binary:
 			assert isinstance(data, bytes), f'Bytes data is required. Actual type: {type(data)}. {self}'
 		else:
 			assert isinstance(data, str), f'String data is required. Actual type: {type(data)}. {self}'
-
 		if Type.Variable in self._target:
-			self._data += data
+			self._data.write(data)
 		elif Type.File in self._target:
 			self._data.write(data)
 		self._written_len += len(data)
 
-	def switch_to_string_data(self) -> None:
+	def switch_to_string_data(self, encoding: str) -> None:
 		"""Switches from binary to string data.
-		For variables, the current content is converted.
+		For variables, the current content is converted to string using the provided encoding.
 		For files, they are closed and reopened as for appended text writing."""
 		if self._binary is False:
 			return
 		self._binary = False
 		if Type.Variable in self._target:
-			if len(self) == 0:
-				self._data = ''
-			else:
-				# noinspection PyUnresolvedReferences
-				self._data = self._data.decode('utf-8')
+			self._data = StringIO(self.content.decode(encoding))
 		elif Type.File in self._target:
 			self._data.close()
 			self._data = open(self._file_path, 'a')
 
+	# noinspection PyTypeChecker
 	@property
 	def content(self) -> AnyStr:
-		"""Returns content of the writer. Does only work with variable types."""
-		assert Type.Variable in self._target, f'Can not return content for the current {self}'
+		"""Returns content of the writer. Only works with variable types."""
+		if self._target == Type.Forget:
+			return ''
+		if self._target != Type.Variable:
+			raise RsInstrException(f'Can not return content for the current {self}')
 		# noinspection PyTypeChecker
-		return self._data
+		if not self._data:
+			return None
+		self._data.seek(0)
+		ret_val = self._data.read()
+		self._data.close()
+		return ret_val
+
+	@property
+	def written_len(self) -> int:
+		"""Returns number of bytes written to the stream since its creation."""
+		return self._written_len
 
 	def close(self) -> None:
 		"""Closes the StreamWriter. You can not use its instance afterwards."""
 		if Type.File in self._target and self._data:
 			self._data.close()
 		self._data = None
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/StructBase.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StructBase.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+"""See the docstring for the StructBase class."""
+
 from .Types import DataType
 
 
 class StructBase:
 	"""Base class for all the driver's argument structures."""
 	def __init__(self, owner):
 		self.__meta_args_link = dict()
 		ix = 0
 		for arg in self.__get_meta_args_list(owner):
 			arg.argument_ix = ix
 			ix += 1
 
-			if arg.data_type == DataType.Enum or arg.data_type == DataType.EnumList:
+			if arg.data_type in [DataType.Enum, DataType.EnumExt, DataType.EnumList, DataType.EnumExtList]:
 				assert arg.enum_type, f"Struct Argument '{arg.name}' is of enum type, you must define the parameter 'enum_type'"
 			else:
 				assert not arg.enum_type, f"Struct Argument '{arg.name}' data type is '{arg.data_type.name}'. You must set the parameter 'enum_type' to None"
 
 			if arg.is_optional:
 				# set all optional values to None
 				setattr(self, arg.name, None)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Types.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,70 @@
+"""Data type class for the variables containing all the methods related to data types."""
+
 from enum import Enum, auto
 from typing import Any
 
 
+# noinspection PyArgumentList
 class DataType(Enum):
-	"""Data type of a variable in the driver."""
+	"""Data type of variable in the driver."""
 	String = auto()
 	RawString = auto()
 	Integer = auto()
 	IntegerExt = auto()
 	Boolean = auto()
 	Float = auto()
 	FloatExt = auto()
 	Enum = auto()
+	EnumExt = auto()
 	StringList = auto()
 	RawStringList = auto()
 	IntegerList = auto()
 	IntegerExtList = auto()
 	BooleanList = auto()
 	FloatList = auto()
 	FloatExtList = auto()
 	EnumList = auto()
+	EnumExtList = auto()
 
 	@property
 	def is_list(self) -> bool:
 		"""Returns True, if the data type is a list."""
 		return self in frozenset(
 			{
 				DataType.StringList,
 				DataType.RawStringList,
 				DataType.IntegerList,
 				DataType.IntegerExtList,
 				DataType.BooleanList,
 				DataType.FloatList,
 				DataType.FloatExtList,
-				DataType.EnumList
+				DataType.EnumList,
+				DataType.EnumExtList
 			})
 
 	@property
 	def is_scalar(self) -> bool:
 		"""Returns True, if the data type is a scalar."""
 		return not self.is_list
 
 	@property
+	def is_scalar_enum(self) -> bool:
+		"""Returns True, if the data type is a scalar enum or enum_ext."""
+		return self == DataType.Enum or self == DataType.EnumExt
+
+	@property
+	def is_list_enum(self) -> bool:
+		"""Returns True, if the data type is a list enum or list enum_ext."""
+		return self == DataType.EnumList or self == DataType.EnumExtList
+
+	@property
 	def is_enum(self) -> bool:
-		"""Returns True, if the data type is enum or enum array."""
-		return self == DataType.Enum or self == DataType.EnumList
+		"""Returns True, if the data type is enum or enum array - including the extended."""
+		return self in [DataType.Enum, DataType.EnumExt, DataType.EnumList, DataType.EnumExtList]
 
 	@property
 	def is_raw_string(self) -> bool:
 		"""Returns True for raw string and raw string list."""
 		return self == DataType.RawString or self == DataType.RawStringList
 
 	@property
@@ -81,14 +97,16 @@
 			return DataType.IntegerExt
 		elif self == DataType.FloatList:
 			return DataType.Float
 		elif self == DataType.FloatExtList:
 			return DataType.FloatExt
 		elif self == DataType.EnumList:
 			return DataType.Enum
+		elif self == DataType.EnumExtList:
+			return DataType.EnumExt
 
 	def get_default_value(self, enm: Enum = None) -> Any:
 		"""Returns default value for the current type.
 		If the data type is Enum or EnumString, you have to provide the enum class."""
 		if self.is_list:
 			return []
 		if self == DataType.RawString:
@@ -103,7 +121,9 @@
 			return 0
 		elif self == DataType.Float:
 			return 0.0
 		elif self == DataType.FloatExt:
 			return 0.0
 		elif self == DataType.Enum:
 			return enm(0)
+		elif self == DataType.EnumExt:
+			return enm(0)
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/Utilities.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Utilities for string manipulation and string formatting for the user."""
+
 from enum import Flag
 from typing import Tuple
 
 
 class TrimStringMode(Flag):
 	"""Trimming mode for strings."""
 	white_chars_only = 1
@@ -133,7 +135,41 @@
 
 
 def calculate_chunks_count(data_size: int, chunk_size: int) -> int:
 	"""Returns number of chunks needed to transfer the data_size split to maximum of chunk_size blocks. \n
 	:param data_size: total data size
 	:param chunk_size: maximum size of one block"""
 	return (data_size // chunk_size) + (1 if (data_size % chunk_size) > 0 else 0)
+
+
+def escape_nonprintable_chars(string: str, encoding: str = 'charmap') -> str:
+	"""
+	Replace nonprintable characters in string s by its hex representation.
+	"""
+	if string.isprintable():
+		return string
+	new_string = ''
+	for char in string:
+		if char.isprintable():
+			new_string += char
+		elif char == '\n':
+			new_string += r'\n'
+		elif char == '\r':
+			new_string += r'\r'
+		elif char == '\t':
+			new_string += r'\t'
+		else:
+			byte = bytes(char, encoding)
+			char = byte.hex()
+			new_string += r'\x' + char
+	return new_string
+
+
+def shorten_string_middle(string: str, max_len: int) -> str:
+	"""If the length of the string is bigger than the max_len,
+	the middle of the string is abbreviated with ' .... ' """
+	count = len(string)
+	if count <= max_len:
+		return string
+	half = int((max_len - 6) / 2)
+	md = (max_len - 6) % 2
+	return string[:half + md] + ' .... ' + string[(count - half):]
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+"""See the docstring for the SocketIo class."""
+
 import socket
 import re
 from contextlib import contextmanager
+from typing import Any
+
+from .InstrumentErrors import RsInstrException
 
 # noinspection PyPackageRequirements
 import pyvisa
 
 
 class SocketIo:
-
+	"""Socket IO plugin providing implementations for all the necessary VISA functions. This class does not need the underlying VISA installation."""
 	def __init__(self, resource_name: str):
 		self.session = socket.socket()
 		self.resource_name = resource_name
 		m = re.search(r'TCPIP::([^:]+)::([^:]+)::SOCKET', self.resource_name)
 		if not m:
-			raise Exception(f"SocketIO instrument unsupported resource name. '{self.resource_name}' Supported resource name example: 'TCPIP::192.168.1.100::5025::SOCKET'")
+			raise RsInstrException(f"SocketIO instrument unsupported resource name. '{self.resource_name}' Supported resource name example: 'TCPIP::192.168.1.100::5025::SOCKET'")
 		self.host = m.group(1).strip()
 		self.port = int(m.group(2).strip())
 		self._read_termination = None
 		self._chunk_size = 1024
 		self._timeout = 5000
 		self.visalib = VisaLib(self)
 
@@ -90,14 +95,22 @@
 
 	# noinspection PyUnusedLocal
 	def read_bytes(self, count: int, **kwargs) -> bytes:
 		"""Reads count bytes"""
 		data, status = self.visalib.read(self.session, count)
 		return data
 
+	def go_to_local(self) -> None:
+		"""Puts the instrument into local state."""
+		self.write("&GTL")
+
+	def go_to_remote(self) -> None:
+		"""Puts the instrument into remote state."""
+		self.write("&GTR")
+
 	# noinspection PyUnusedLocal
 	@contextmanager
 	def ignore_warning(self, filter_value: int) -> None:
 		"""Context property with no effect for the socket connection"""
 		try:
 			yield None
 		finally:
@@ -106,15 +119,15 @@
 
 	def close(self) -> None:
 		"""Closes the socket connection"""
 		self.session.close()
 
 
 class VisaLib:
-
+	"""Implementation of the pyvisa's VisaLib providing the method read()"""
 	def __init__(self, socket_io: SocketIo):
 		self._socket_io = socket_io
 
 	def __str__(self):
 		return "SocketIO"
 
 	# noinspection PyUnresolvedReferences
@@ -159,17 +172,18 @@
 				more_data_available = True
 
 		return_code = pyvisa.constants.StatusCode.success_max_count_read if more_data_available else pyvisa.constants.StatusCode.success
 		return chunk, return_code
 
 
 class ResourceManager:
-
+	"""Implementation of the VISA's Resource Manager."""
 	def __init__(self):
 		self.VisaManufacturerName = "SocketIO"
 		self.connection = None
 
-	def open_resource(self, resource_name: str) -> SocketIo:
-		"""Creates new Socket connection"""
+	# noinspection PyUnusedLocal
+	def open_resource(self, resource_name: str, access_mode: Any = None, open_timeout: Any = None) -> SocketIo:
+		"""Creates new Socket connection. access_mode and open_timeout are here for compatibility reasons with the pyvisa rm.open_resource()"""
 		self.connection = SocketIo(resource_name)
 		self.connection.connect()
 		return self.connection
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/Internal/VisaSessionSim.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSessionSim.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""VisaSession for simulated sessions."""
+
 import threading
 from typing import Callable, Dict, AnyStr
 
 from . import InstrumentSettings
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
 
@@ -9,14 +11,15 @@
 # noinspection PyMethodMayBeStatic,PyUnusedLocal
 class VisaSessionSim(object):
 	"""Visa session in simulation mode.
 	Provides the properties for the simulation mode.
 	Also serves as a cache for the SCPI command values: If you query a SCPI command value, it returns the last set value by that SCPI command."""
 
 	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
+		self.reusing_session = direct_session is not None
 		# noinspection PyTypeChecker
 		self._data_chunk_size: int = None
 		# noinspection PyTypeChecker
 		self._lock: threading.RLock = None
 
 		# Event handlers
 		# noinspection PyTypeChecker
@@ -25,16 +28,17 @@
 		# noinspection PyTypeChecker
 		self.on_write_chunk_handler: Callable = None
 		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
 		self.io_events_include_data: bool = False
 		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
 
 		self.manufacturer: str = 'Rohde&Schwarz'
-		self._resource_name = resource_name
+		self.resource_name = resource_name
 		self.vxi_capable = True
+		self.encoding = settings.encoding  # default encoder between bytes and string
 
 		# Changeable settings
 		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
 		self.visa_timeout = settings.visa_timeout
 		self.data_chunk_size = settings.io_segment_size
 
 		self._last_cmd = None
@@ -50,14 +54,17 @@
 			rlock = direct_session.session_thread_rlock
 			if isinstance(rlock, type(threading.RLock())):
 				self.assign_lock(rlock)
 		if self.get_lock() is None:
 			# The existing session did not have a thread lock, assign a new one
 			self.assign_lock(threading.RLock())
 
+		if self.reusing_session:
+			self.resource_name = direct_session.resource_name
+
 	def assign_lock(self, lock: threading.RLock) -> None:
 		"""Assigns the provided thread lock. The lock is only used by the parent class Instrument."""
 		self._lock = lock
 
 	def get_lock(self) -> threading.RLock:
 		"""Returns the current RLock object."""
 		return self._lock
@@ -92,16 +99,17 @@
 		return False
 
 	def query_syst_error(self) -> str or None:
 		"""Returns one response to the SYSTEM:ERROR? query."""
 		return None
 
 	def query_all_syst_errors(self) -> list or None:
-		"""Returns all errors in the instrument's error queue."""
-		return []
+		"""Returns all errors in the instrument's error queue.
+		If no error is detected, the return value is None."""
+		return None
 
 	def clear_before_read(self) -> None:
 		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
 		return
 
 	def clear(self) -> None:
 		"""Perform VISA viClear conditionally based on the instrument settings."""
@@ -121,15 +129,15 @@
 		return 'Simulating' if cached is None else cached
 
 	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
 		"""Sends command with OPC-sync.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		self.write(cmd)
 
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+	def query_str_with_opc(self, query: str, timeout: int = None, context: str = 'Query string with OPC') -> str:
 		"""Query string with OPC synchronization.
 		The response is trimmed for any trailing LF.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		return self.query_str(query)
 
 	def query_opc(self, timeout: int = 0) -> bool:
 		"""Sends *OPC? query and reads the result."""
@@ -160,28 +168,28 @@
 		cached = self._get_cmd_cached_value(query)
 
 		if cached is None:
 			stream.write(bytes([0, 1, 2, 3, 4, 5, 6, 7, 8, 65, 66]))
 			self.cached_to_stream = False
 		else:
 			if isinstance(cached, str):
-				stream.switch_to_string_data()
+				stream.switch_to_string_data(self.encoding)
 			stream.write(cached)
 			self.cached_to_stream = True
 
 	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
 		"""Query binary data block with OPC and returns it as byte data."""
 		self.query_bin_block(query, stream)
 
 	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
 		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
 		Returns the read data including the stop character."""
 		return b'Simulating'
 
 	def get_session_handle(self) -> object:
 		"""Returns the underlying pyvisa session."""
-		return f"Simulating session, resource name '{self._resource_name}'"
+		return f"Simulating session, resource name '{self.resource_name}'"
 
 	def close(self) -> None:
 		"""Closes the Visa session.
 		If the object was created with the direct session input, the session is not closed."""
 		return
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/__init__.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """RsCMPX_UwbMeas instrument driver
-	:version: 4.0.7.5
+	:version: 4.0.80.16
 	:copyright: 2021 by Rohde & Schwarz GMBH & Co. KG
 	:license: MIT, see LICENSE for more details.
 """
 
-__version__ = '4.0.7.5'
+__version__ = '4.0.80.16'
 
 # Main class
 from RsCMPX_UwbMeas.RsCMPX_UwbMeas import RsCMPX_UwbMeas
 
 # Bin data format
 from RsCMPX_UwbMeas.Internal.Conversions import BinIntFormat, BinFloatFormat
 
 # Exceptions
 from RsCMPX_UwbMeas.Internal.InstrumentErrors import RsInstrException, TimeoutException, StatusException, UnexpectedResponseException, ResourceError, DriverValueError
 
 # Callback Event Argument prototypes
 from RsCMPX_UwbMeas.Internal.IoTransferEventArgs import IoTransferEventArgs
 
+# Logging Mode
+from RsCMPX_UwbMeas.Internal.ScpiLogger import LoggingMode
+
 # enums
 from RsCMPX_UwbMeas import enums
 
 # repcaps
 from RsCMPX_UwbMeas import repcap
 
 # Reliability interface
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas/enums.py` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -166,19 +166,36 @@
 	RH5 = 159
 	RH6 = 160
 	RH7 = 161
 	RH8 = 162
 
 
 # noinspection SpellCheckingInspection
+class MaxSpecPowLen(Enum):
+	"""2 Members, MS1 ... PPDU"""
+	MS1 = 0
+	PPDU = 1
+
+
+# noinspection SpellCheckingInspection
 class PhrDataRate(Enum):
-	"""3 Members, DRHP ... DRMD"""
+	"""6 Members, DRHP ... SYNC"""
 	DRHP = 0
 	DRLP = 1
 	DRMD = 2
+	RHMH = 3
+	RHML = 4
+	SYNC = 5
+
+
+# noinspection SpellCheckingInspection
+class PpduMode(Enum):
+	"""2 Members, MPPDu ... SPPDu"""
+	MPPDu = 0
+	SPPDu = 1
 
 
 # noinspection SpellCheckingInspection
 class Repeat(Enum):
 	"""2 Members, CONTinuous ... SINGleshot"""
 	CONTinuous = 0
 	SINGleshot = 1
@@ -236,7 +253,22 @@
 # noinspection SpellCheckingInspection
 class StsSegmentLen(Enum):
 	"""4 Members, L128 ... L64"""
 	L128 = 0
 	L256 = 1
 	L32 = 2
 	L64 = 3
+
+
+# noinspection SpellCheckingInspection
+class TargetMainState(Enum):
+	"""3 Members, OFF ... RUN"""
+	OFF = 0
+	RDY = 1
+	RUN = 2
+
+
+# noinspection SpellCheckingInspection
+class TargetSyncState(Enum):
+	"""2 Members, ADJusted ... PENDing"""
+	ADJusted = 0
+	PENDing = 1
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/RsCMPX_UwbMeas.egg-info/SOURCES.txt` & `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,271 +1,368 @@
-README.md
+README.rst
 setup.py
 RsCMPX_UwbMeas/RsCMPX_UwbMeas.py
 RsCMPX_UwbMeas/__init__.py
 RsCMPX_UwbMeas/enums.py
 RsCMPX_UwbMeas/repcap.py
 RsCMPX_UwbMeas.egg-info/PKG-INFO
 RsCMPX_UwbMeas.egg-info/SOURCES.txt
 RsCMPX_UwbMeas.egg-info/dependency_links.txt
 RsCMPX_UwbMeas.egg-info/requires.txt
 RsCMPX_UwbMeas.egg-info/top_level.txt
 RsCMPX_UwbMeas/CustomFiles/__init__.py
 RsCMPX_UwbMeas/CustomFiles/events.py
 RsCMPX_UwbMeas/CustomFiles/reliability.py
 RsCMPX_UwbMeas/CustomFiles/utilities.py
-RsCMPX_UwbMeas/Implementations/Configure.py
-RsCMPX_UwbMeas/Implementations/Route.py
-RsCMPX_UwbMeas/Implementations/Trigger.py
-RsCMPX_UwbMeas/Implementations/UwbMeas.py
 RsCMPX_UwbMeas/Implementations/__init__.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas.py
-RsCMPX_UwbMeas/Implementations/Configure_/__init__.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/RfSettings.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/__init__.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Result.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Spectrum.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/StsGap.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/__init__.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation_/Limit.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/Modulation_/__init__.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/__init__.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit_/Area.py
-RsCMPX_UwbMeas/Implementations/Configure_/UwbMeas_/MultiEval_/TsMask_/Limit_/__init__.py
-RsCMPX_UwbMeas/Implementations/Route_/UwbMeas.py
-RsCMPX_UwbMeas/Implementations/Route_/__init__.py
-RsCMPX_UwbMeas/Implementations/Route_/UwbMeas_/RfSettings.py
-RsCMPX_UwbMeas/Implementations/Route_/UwbMeas_/__init__.py
-RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas.py
-RsCMPX_UwbMeas/Implementations/Trigger_/__init__.py
-RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval.py
-RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/__init__.py
-RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval_/Catalog.py
-RsCMPX_UwbMeas/Implementations/Trigger_/UwbMeas_/MultiEval_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/State.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CcError_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Cevm_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CpJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/CtJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Foffset_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Fofh_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Nmse_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/PmlWidth_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/Sevm_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SlPeak_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SmAccuracy_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/SpJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/Extreme.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Modulation_/StJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Maximum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Minimum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Maximum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/Minimum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/DpPower_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Maximum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/Minimum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Dpower_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Maximum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/Minimum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/MsPower_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Maximum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/Minimum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/PpPower_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Maximum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/Minimum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/StandardDev.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Power_/Ppower_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/AsSymbols.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Cindex.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/CsLength.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Dlength.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Drate.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr_/Crc.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Phr_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/Crc.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/Length.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Sinfo_/Psdu_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/State_/All.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/State_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/Xvalues.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CpJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/Xvalues.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/CtJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/Xvalues.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/NcCorr_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/Maximum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/Minimum.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/Xvalues.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/PowerVsTime_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/Xvalues.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/SpJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/Xvalues.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/StJitter_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/Xvalues.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/Trace_/TsMask_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Negativ_/__init__.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/Average.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/Current.py
-RsCMPX_UwbMeas/Implementations/UwbMeas_/MultiEval_/TsMask_/Margin_/Area_/Positiv_/__init__.py
+RsCMPX_UwbMeas/Implementations/Catalog/UwbMeas.py
+RsCMPX_UwbMeas/Implementations/Catalog/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Ppdu.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Spectrum.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/CcError.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Foffset.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Plevel.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/PmlWidth.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SlPeak.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SmAccuracy.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/Nrmse.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/Nrmse.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/Nrmse.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/Nrmse.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Area.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/Area.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/Area.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/Range.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/__init__.py
+RsCMPX_UwbMeas/Implementations/Route/__init__.py
+RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py
+RsCMPX_UwbMeas/Implementations/Route/UwbMeas/__init__.py
+RsCMPX_UwbMeas/Implementations/Trigger/__init__.py
+RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/__init__.py
+RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/Catalog.py
+RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Clength.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Content.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/RsParity.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Otolerance.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Otolerance.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/Margin.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Extreme.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/Margin.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Cindex.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/CsLength.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dlength.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dppdu.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Drate.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/FcsCheck.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/PstGap.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/RaBit.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/ReBit.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Sfd.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/SfdLength.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/AsSymbols.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Bitrate.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/All.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Xvalues.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Otolerance.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py
 RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py
 RsCMPX_UwbMeas/Internal/ArgSingle.py
 RsCMPX_UwbMeas/Internal/ArgSingleList.py
 RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py
 RsCMPX_UwbMeas/Internal/ArgStringComposer.py
 RsCMPX_UwbMeas/Internal/ArgStruct.py
 RsCMPX_UwbMeas/Internal/ArgStructList.py
 RsCMPX_UwbMeas/Internal/ArgStructStringParser.py
 RsCMPX_UwbMeas/Internal/CommandsGroup.py
 RsCMPX_UwbMeas/Internal/Conversions.py
 RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py
 RsCMPX_UwbMeas/Internal/ConverterToScpiString.py
 RsCMPX_UwbMeas/Internal/Core.py
+RsCMPX_UwbMeas/Internal/GlobalData.py
 RsCMPX_UwbMeas/Internal/Instrument.py
 RsCMPX_UwbMeas/Internal/InstrumentErrors.py
 RsCMPX_UwbMeas/Internal/InstrumentOptions.py
 RsCMPX_UwbMeas/Internal/InstrumentSettings.py
 RsCMPX_UwbMeas/Internal/InternalLinker.py
 RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py
 RsCMPX_UwbMeas/Internal/RepeatedCapability.py
+RsCMPX_UwbMeas/Internal/ScpiEnums.py
+RsCMPX_UwbMeas/Internal/ScpiLogger.py
 RsCMPX_UwbMeas/Internal/StreamReader.py
 RsCMPX_UwbMeas/Internal/StreamWriter.py
 RsCMPX_UwbMeas/Internal/StructBase.py
 RsCMPX_UwbMeas/Internal/Types.py
 RsCMPX_UwbMeas/Internal/Utilities.py
 RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py
 RsCMPX_UwbMeas/Internal/VisaSession.py
```

### Comparing `RsCMPX_UwbMeas-4.0.7.5/setup.py` & `RsCMPX_UwbMeas-4.0.80/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import pathlib
 from setuptools import setup, find_packages
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
-README = (HERE / "README.md").read_text()
+README = (HERE / "README.rst").read_text()
 
 # This call to setup() does all the work
 setup(
     name="RsCMPX_UwbMeas",
-    version="4.0.7.5",
-    description="CMP/CMX Ultra Wideband Measurement Remote-control Module",
+    version="4.0.80",
+    description="CMP/CMX Ultra Wideband Measurement Remote-control module",
     long_description=README,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     author="Rohde & Schwarz GmbH & Co. KG",
-    copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2021",
-    author_email="Customer.Support@rohde-schwarz.com",
+    copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2022",
     license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
-    ],
+    classifiers=['License :: OSI Approved :: MIT License',
+                 'Intended Audience :: Developers',
+                 'Operating System :: Microsoft :: Windows',
+                 'Operating System :: POSIX :: Linux',
+                 'Operating System :: MacOS :: MacOS X',
+                 'Programming Language :: Python',
+                 'Programming Language :: Python :: 3',
+                 'Programming Language :: Python :: 3.6',
+                 'Programming Language :: Python :: 3.7',
+                 'Programming Language :: Python :: 3.8',
+                 'Programming Language :: Python :: 3.9',
+                 'Programming Language :: Python :: 3.10'
+                ],
     packages=(find_packages(include=['RsCMPX_UwbMeas', 'RsCMPX_UwbMeas.*'])),
-    install_requires=['PyVisa']
+    install_requires=['PyVisa>=1.11.3'],
+    python_requires='>=3.6'
 )
```

