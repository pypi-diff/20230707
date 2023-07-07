# Comparing `tmp/astro-p3-1.0.tar.gz` & `tmp/astro-p3-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-p3-1.0.tar", last modified: Fri Apr  7 10:48:29 2023, max compression
+gzip compressed data, was "astro-p3-1.1.tar", last modified: Fri Jul  7 08:35:26 2023, max compression
```

## Comparing `astro-p3-1.0.tar` & `astro-p3-1.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.675770 astro-p3-1.0/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.635769 astro-p3-1.0/.github/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.635769 astro-p3-1.0/.github/workflows/
--rw-r--r--   0 simon     (1000) simon     (1000)      923 2023-03-28 07:24:14.000000 astro-p3-1.0/.github/workflows/publish.yml
--rw-r--r--   0 simon     (1000) simon     (1000)      372 2023-03-28 07:24:14.000000 astro-p3-1.0/.gitignore
--rw-r--r--   0 simon     (1000) simon     (1000)     1492 2023-04-07 10:38:48.000000 astro-p3-1.0/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)       25 2023-04-06 16:06:53.000000 astro-p3-1.0/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1000)      263 2023-04-07 10:48:29.675770 astro-p3-1.0/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)       12 2023-01-18 12:35:13.000000 astro-p3-1.0/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.635769 astro-p3-1.0/astro_p3.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)      263 2023-04-07 10:48:29.000000 astro-p3-1.0/astro_p3.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     6534 2023-04-07 10:48:29.000000 astro-p3-1.0/astro_p3.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-04-07 10:48:29.000000 astro-p3-1.0/astro_p3.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-07 10:48:29.000000 astro-p3-1.0/astro_p3.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        8 2023-04-07 10:48:29.000000 astro-p3-1.0/astro_p3.egg-info/top_level.txt
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.635769 astro-p3-1.0/p3/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      155 2023-04-07 10:48:29.000000 astro-p3-1.0/p3/_version.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.639102 astro-p3-1.0/p3/aoSystem/
--rw-r--r--   0 simon     (1000) simon     (1000)    38646 2023-03-31 16:18:37.000000 astro-p3-1.0/p3/aoSystem/FourierUtils.py
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/__init__.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.639102 astro-p3-1.0/p3/aoSystem/_txtFile/
--rw-r--r--   0 simon     (1000) simon     (1000)    39085 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/_txtFile/ELT_segmentVertices.txt
--rw-r--r--   0 simon     (1000) simon     (1000)      392 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/_txtFile/Keck_segmentVertices.txt
--rw-r--r--   0 simon     (1000) simon     (1000)     6709 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/anisoplanatismModel.py
--rw-r--r--   0 simon     (1000) simon     (1000)    34248 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/aoSystem.py
--rw-r--r--   0 simon     (1000) simon     (1000)    10300 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/atmosphere.py
--rw-r--r--   0 simon     (1000) simon     (1000)     2530 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/createSegmentedModes.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.635769 astro-p3-1.0/p3/aoSystem/data/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.642436 astro-p3-1.0/p3/aoSystem/data/ELT_CALIBRATION/
--rw-r--r--   0 simon     (1000) simon     (1000)  4331520 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   938880 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.642436 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.642436 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/
--rw-r--r--   0 simon     (1000) simon     (1000)      924 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidActuatorMap.txt
--rw-r--r--   0 simon     (1000) simon     (1000)      840 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidSubapMap.txt
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.659103 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/
--rw-r--r--   0 simon     (1000) simon     (1000) 11522880 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits
--rw-r--r--   0 simon     (1000) simon     (1000)  2882880 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits
--rw-r--r--   0 simon     (1000) simon     (1000) 11522880 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits
--rw-r--r--   0 simon     (1000) simon     (1000) 11845440 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   325440 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.635769 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.659103 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/
--rw-r--r--   0 simon     (1000) simon     (1000)     2200 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat
--rw-r--r--   0 simon     (1000) simon     (1000)      600 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat
--rw-r--r--   0 simon     (1000) simon     (1000)     6828 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.659103 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/
--rw-r--r--   0 simon     (1000) simon     (1000)     9125 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat
--rw-r--r--   0 simon     (1000) simon     (1000)     3175 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    26149 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.659103 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/
--rw-r--r--   0 simon     (1000) simon     (1000)     8350 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat
--rw-r--r--   0 simon     (1000) simon     (1000)     7775 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    25122 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.659103 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/
--rw-r--r--   0 simon     (1000) simon     (1000)     8450 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat
--rw-r--r--   0 simon     (1000) simon     (1000)     7475 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    24174 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.662436 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/
--rw-r--r--   0 simon     (1000) simon     (1000)     9700 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat
--rw-r--r--   0 simon     (1000) simon     (1000)     8650 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    27413 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat
--rw-r--r--   0 simon     (1000) simon     (1000)     8450 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat
--rw-r--r--   0 simon     (1000) simon     (1000)     7475 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    24174 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.662436 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/
--rw-r--r--   0 simon     (1000) simon     (1000)    45636 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    31637 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    51146 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    42642 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    45125 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    60065 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    54054 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    60374 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    58102 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    61576 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat
--rw-r--r--   0 simon     (1000) simon     (1000)    41888 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat
--rw-r--r--   0 simon     (1000) simon     (1000)  2079744 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls
--rw-r--r--   0 simon     (1000) simon     (1000)   128912 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.662436 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/
--rw-r--r--   0 simon     (1000) simon     (1000)    77760 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   463680 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   463680 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.665769 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/
--rw-r--r--   0 simon     (1000) simon     (1000)    17280 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    17280 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    28800 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    28800 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    28800 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    28800 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    28800 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    28800 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    28800 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits
--rw-r--r--   0 simon     (1000) simon     (1000)  1330560 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits
--rw-r--r--   0 simon     (1000) simon     (1000)     5760 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.635769 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.665769 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/
--rw-r--r--   0 simon     (1000) simon     (1000)   152640 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   593280 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   120960 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   429120 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   120960 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   120960 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits
--rw-r--r--   0 simon     (1000) simon     (1000)   429120 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    60480 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits
--rw-r--r--   0 simon     (1000) simon     (1000)  2102400 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.669103 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/
--rw-r--r--   0 simon     (1000) simon     (1000)  9835200 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits
--rw-r--r--   0 simon     (1000) simon     (1000)    26142 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/defineAoSystem.py
--rw-r--r--   0 simon     (1000) simon     (1000)     7487 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/deformableMirror.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1685 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/detector.py
--rw-r--r--   0 simon     (1000) simon     (1000)    53221 2023-03-31 16:18:37.000000 astro-p3-1.0/p3/aoSystem/fourierModel.py
--rw-r--r--   0 simon     (1000) simon     (1000)     9520 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/frequencyDomain.py
--rw-r--r--   0 simon     (1000) simon     (1000)      866 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/optics.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.672436 astro-p3-1.0/p3/aoSystem/parFiles/
--rw-r--r--   0 simon     (1000) simon     (1000)     9341 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/HarmoniLTAO.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     8428 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/HarmoniSCAO.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     1928 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     8839 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/MavisMCAO.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     4609 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/MosaicGLAO.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     8117 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/eris.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     6840 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/irdis.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     8377 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/nirc2.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     8489 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/nirc2_monochromatic.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     8426 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/parFiles/template.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     1265 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/processing.py
--rw-r--r--   0 simon     (1000) simon     (1000)    21580 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/pupil.py
--rw-r--r--   0 simon     (1000) simon     (1000)     2553 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/rtc.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5045 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/segment.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3692 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/sensor.py
--rw-r--r--   0 simon     (1000) simon     (1000)     4445 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/source.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5253 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/spiders.py
--rw-r--r--   0 simon     (1000) simon     (1000)     8094 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/telescope.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.672436 astro-p3-1.0/p3/aoSystem/testing/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/testing/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     4378 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/testing/tests_aoSystem.py
--rw-r--r--   0 simon     (1000) simon     (1000)     2238 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/testing/tests_tiptop_compatibility.py
--rw-r--r--   0 simon     (1000) simon     (1000)    13520 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/aoSystem/zernike.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.672436 astro-p3-1.0/p3/deepLoop/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6028 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/dataBaseVerification.py
--rw-r--r--   0 simon     (1000) simon     (1000)    10414 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/dataGenerator.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3457 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/dataGeneratorBatch.py
--rw-r--r--   0 simon     (1000) simon     (1000)    24969 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/deepLoopPerformance.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3224 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/deepLoopPerformanceBatch.py
--rwxr-xr-x   0 simon     (1000) simon     (1000)      628 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/jobGenerate.sh
--rwxr-xr-x   0 simon     (1000) simon     (1000)      828 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/jobPerformance.sh
--rw-r--r--   0 simon     (1000) simon     (1000)     1706 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/deepLoop/recover_list.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.675770 astro-p3-1.0/p3/psfFitting/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfFitting/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      910 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfFitting/confidenceInterval.py
--rw-r--r--   0 simon     (1000) simon     (1000)    30451 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfFitting/fittingUtils.py
--rw-r--r--   0 simon     (1000) simon     (1000)     2203 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfFitting/imageModel.py
--rw-r--r--   0 simon     (1000) simon     (1000)    10944 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfFitting/psfFitting.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.675770 astro-p3-1.0/p3/psfao21/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfao21/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     8797 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfao21/psfao21.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.675770 astro-p3-1.0/p3/psfr/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfr/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)    14707 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfr/psfR.py
--rw-r--r--   0 simon     (1000) simon     (1000)     7795 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/psfr/psfrUtils.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.675770 astro-p3-1.0/p3/telemetry/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)    10582 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/configFile.py
--rw-r--r--   0 simon     (1000) simon     (1000)     7650 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/keckUtils.py
--rw-r--r--   0 simon     (1000) simon     (1000)    13812 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/massdimm.py
--rw-r--r--   0 simon     (1000) simon     (1000)     8108 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/sphereUtils.py
--rw-r--r--   0 simon     (1000) simon     (1000)    21961 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/systemDiagnosis.py
--rw-r--r--   0 simon     (1000) simon     (1000)    13021 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/telemetryKASP.py
--rw-r--r--   0 simon     (1000) simon     (1000)    19117 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/telemetry/telemetryKeck.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-07 10:48:29.675770 astro-p3-1.0/p3/testing/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/testing/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)    15100 2023-03-28 07:24:14.000000 astro-p3-1.0/p3/testing/tests_p3.py
--rw-r--r--   0 simon     (1000) simon     (1000)      598 2023-04-07 10:38:48.000000 astro-p3-1.0/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-07 10:48:29.675770 astro-p3-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.003033 astro-p3-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.015034 astro-p3-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 08:35:09.000000 astro-p3-1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-07 08:35:09.000000 astro-p3-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-07 08:35:09.000000 astro-p3-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 08:35:09.000000 astro-p3-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 08:35:26.103036 astro-p3-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 08:35:09.000000 astro-p3-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.015034 astro-p3-1.1/astro_p3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.015034 astro-p3-1.1/p3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 08:35:25.000000 astro-p3-1.1/p3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.023034 astro-p3-1.1/p3/aoSystem/
+-rw-r--r--   0 runner    (1001) docker     (123)    38763 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/FourierUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.023034 astro-p3-1.1/p3/aoSystem/_txtFile/
+-rw-r--r--   0 runner    (1001) docker     (123)    39085 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/_txtFile/ELT_segmentVertices.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/_txtFile/Keck_segmentVertices.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/anisoplanatismModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/aoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/createSegmentedModes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.011034 astro-p3-1.1/p3/aoSystem/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.031034 astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/
+-rw-r--r--   0 runner    (1001) docker     (123)  4331520 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   938880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.031034 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.031034 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidActuatorMap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidSubapMap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.071035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/
+-rw-r--r--   0 runner    (1001) docker     (123) 11522880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  2882880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 11522880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 11845440 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   325440 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.007034 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.071035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    26149 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    25122 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.079035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/
+-rw-r--r--   0 runner    (1001) docker     (123)    45636 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    31637 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    51146 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    42642 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    45125 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    60065 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    54054 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    60374 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    58102 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    61576 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    41888 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat
+-rw-r--r--   0 runner    (1001) docker     (123)  2079744 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls
+-rw-r--r--   0 runner    (1001) docker     (123)   128912 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.079035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/
+-rw-r--r--   0 runner    (1001) docker     (123)    77760 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   463680 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   463680 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.083036 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  1330560 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.011034 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.087036 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/
+-rw-r--r--   0 runner    (1001) docker     (123)   152640 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   593280 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   429120 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   429120 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    60480 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  2102400 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.091036 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/
+-rw-r--r--   0 runner    (1001) docker     (123)  9835200 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/defineAoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/deformableMirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56675 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/fourierModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/frequencyDomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/optics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.099036 astro-p3-1.1/p3/aoSystem/parFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/HarmoniLTAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/HarmoniSCAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/MavisMCAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/MosaicGLAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/eris.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/irdis.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/nirc2.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/nirc2_monochromatic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/template.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/pupil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/spiders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.099036 astro-p3-1.1/p3/aoSystem/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/testing/tests_aoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/testing/tests_tiptop_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/deepLoop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/dataBaseVerification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/dataGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/dataGeneratorBatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/deepLoopPerformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/deepLoopPerformanceBatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/jobGenerate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/jobPerformance.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/recover_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/psfFitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/confidenceInterval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30451 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/fittingUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/imageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/psfFitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/psfao21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfao21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfao21/psfao21.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/psfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfr/psfR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfr/psfrUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/configFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/keckUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/massdimm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/sphereUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/systemDiagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/telemetryKASP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/telemetryKeck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/testing/tests_p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-07 08:35:10.000000 astro-p3-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:35:26.103036 astro-p3-1.1/setup.cfg
```

### Comparing `astro-p3-1.0/.github/workflows/publish.yml` & `astro-p3-1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/LICENSE` & `astro-p3-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/astro_p3.egg-info/SOURCES.txt` & `astro-p3-1.1/astro_p3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/FourierUtils.py` & `astro-p3-1.1/p3/aoSystem/FourierUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,20 @@
         F     = np.pi*D*np.hypot(FX,FY)    
     else:
         F     = np.pi*D*f
         
     #out         = np.zeros_like(F)
     #idx         = F!=0
     #out[idx]    = spc.j1(F[idx])/F[idx]
-    R         = sombrero(1,F)        
-    return 1 - 4 * R**2
+    R         = sombrero(1,F)      
+    pFilter   =  1 - 4 * R**2
+    if np.min(pFilter)<0:
+        pFilter[np.where(pFilter<0)] = 0
+
+    return pFilter
              
 def psd2cov(psd,pixelScale):
     nPts = np.array(psd.shape)
     psd  = fft.fftshift(psd)
     if len(nPts) ==1:
         out = fft.fft(psd)*pixelScale**2
     elif len(nPts) ==2:
@@ -712,17 +716,17 @@
     nEE   = min([nY-y0,nX-x0])
     
     EE = np.zeros(nEE+1)
     for n in range(nEE+1):
         EE[n] = psf[y0 - n:y0+n+1,x0-n:x0+n+1].sum()
     return EE/S
 
-def getEncircledEnergy(psf,pixelscale=1,nargout=1):            
+def getEncircledEnergy(psf,pixelscale=1, center=None,nargout=1):            
     
-    rr, radialprofile2, ee = radial_profile(psf,ee=True,pixelscale=pixelscale)
+    rr, radialprofile2, ee = radial_profile(psf,ee=True, center=None,pixelscale=pixelscale)
     if nargout==1:
         return ee
     elif nargout == 2:
         return ee,rr
 
 
 def radial_profile(image, ext=0, pixelscale=1,ee=False, center=None, stddev=False, binsize=None, maxradius=None,
```

### Comparing `astro-p3-1.0/p3/aoSystem/_txtFile/ELT_segmentVertices.txt` & `astro-p3-1.1/p3/aoSystem/_txtFile/ELT_segmentVertices.txt`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/anisoplanatismModel.py` & `astro-p3-1.1/p3/aoSystem/anisoplanatismModel.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/aoSystem.py` & `astro-p3-1.1/p3/aoSystem/aoSystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,25 +140,44 @@
                 
         #----- TELESCOPE ABERRATIONS
         if self.check_config_key('telescope', 'PathStatModes'):
             path_statModes = path_root + self.get_config_value('telescope','PathStatModes')
         else:
             path_statModes = ''
             
+        #----- EXTRA ERROR
+        if self.check_config_key('telescope', 'extraErrorNm'):       
+            extraErrorNm = self.get_config_value('telescope','extraErrorNm')
+        else:
+            extraErrorNm = 0
+            
+        if self.check_config_key('telescope', 'extraErrorExp'):
+            extraErrorExp = self.get_config_value('telescope','extraErrorExp')
+        else:
+            extraErrorExp = -2
+            
+        if self.check_config_key('telescope', 'extraErrorMin'):
+            extraErrorMin = self.get_config_value('telescope','extraErrorMin')
+        else:
+            extraErrorMin = 0
+            
         # ----- class definition     
         self.tel = telescope(D, nPup,
                              zenith_angle=zenithAngle,
                              obsRatio=obsRatio,
                              pupilAngle=pupilAngle,
                              path_pupil=path_pupil,
                              path_static_on=path_static_on,
                              path_static_off=path_static_off,
                              path_static_pos=path_static_pos,
                              path_apodizer=path_apodizer,
-                             path_statModes=path_statModes)                     
+                             path_statModes=path_statModes,
+                             extraErrorNm=extraErrorNm,
+                             extraErrorExp=extraErrorExp,
+                             extraErrorMin=extraErrorMin)                     
 
         #%% ATMOSPHERE
         
         if self.check_config_key('atmosphere','Wavelength'):
             wvlAtm = self.get_config_value('atmosphere','Wavelength') 
         else:
             wvlAtm = 500e-9
@@ -567,15 +586,19 @@
             
         if self.check_config_key('RTC','LoopDelaySteps_HO'):
             delay_HO = self.get_config_value('RTC','LoopDelaySteps_HO')
         else:
             delay_HO = 2
                      
         if self.check_config_key('RTC','LoopGain_LO'):
-            LoopGain_LO = self.get_config_value('RTC','LoopGain_LO')
+            temp = self.get_config_value('RTC','LoopGain_LO')
+            if temp != 'optimize':
+                LoopGain_LO = temp
+            else:
+                LoopGain_LO = None
         else:
             LoopGain_LO = None
             
         if self.check_config_key('RTC','SensorFrameRate_LO'):
             frameRate_LO = self.get_config_value('RTC','SensorFrameRate_LO')
         else:
             frameRate_LO = None
```

### Comparing `astro-p3-1.0/p3/aoSystem/atmosphere.py` & `astro-p3-1.1/p3/aoSystem/atmosphere.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/createSegmentedModes.py` & `astro-p3-1.1/p3/aoSystem/createSegmentedModes.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits` & `astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits` & `astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits` & `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits` & `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/defineAoSystem.py` & `astro-p3-1.1/p3/aoSystem/defineAoSystem.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/deformableMirror.py` & `astro-p3-1.1/p3/aoSystem/deformableMirror.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/detector.py` & `astro-p3-1.1/p3/aoSystem/detector.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/fourierModel.py` & `astro-p3-1.1/p3/aoSystem/fourierModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,28 +52,28 @@
     """
     
     # CONTRUCTOR
     def __init__(self, path_ini, calcPSF=True, verbose=False, display=True, path_root='',
                  normalizePSD=False, displayContour=False, getPSDatNGSpositions=False,
                  getErrorBreakDown=False, getFWHM=False, getEnsquaredEnergy=False,
                  getEncircledEnergy=False, fftphasor=False, MV=0, nyquistSampling=False,
-                 addOtfPixel=False, computeFocalAnisoCov=True):
+                 addOtfPixel=False, computeFocalAnisoCov=True, TiltFilter=False):
         
         tstart = time.time()
         
         # PARSING INPUTS
         self.verbose = verbose
         self.path_ini = path_ini  
         self.display = display
         self.getErrorBreakDown = getErrorBreakDown
         self.getPSFmetrics = getFWHM or getEnsquaredEnergy or getEncircledEnergy
         self.calcPSF = calcPSF
         self.tag = 'TIPTOP'
         self.addOtfPixel = addOtfPixel
-
+        
         # GRAB PARAMETERS
         self.ao = aoSystem(path_ini,path_root=path_root,getPSDatNGSpositions=getPSDatNGSpositions)
         self.t_initAO = 1000*(time.time() - tstart)
         
         if self.ao.error==False:
             
             # DEFINING THE FREQUENCY DOMAIN
@@ -123,15 +123,18 @@
             self.Wphi = self.ao.atm.spectrum(np.sqrt(self.freq.k2AO_))
             
             # DEFINE THE RECONSTRUCTOR
             self.spatialReconstructor(MV=MV)
                 
             # DEFINE THE CONTROLLER
             self.controller(display=self.display)
-                
+                            
+            #set tilt filter key before computing the PSD
+            self.applyTiltFilter = TiltFilter
+            
             # COMPUTE THE PSD
             if normalizePSD == True:
                 wfe = self.ao.rtc.holoop['wfe']
             else:
                 wfe = None
             self.PSD = self.powerSpectrumDensity(wfe=wfe)
             
@@ -381,15 +384,15 @@
             nPts        = self.freq.resAO
             thetaWind   = np.linspace(0, 2*np.pi-2*np.pi/nTh,nTh)
             costh       = np.cos(thetaWind)
             weights     = self.ao.atm.weights
             Ts          = 1.0/self.ao.rtc.holoop['rate']#samplingTime
             delay       = self.ao.rtc.holoop['delay']#latency        
             loopGain    = self.ao.rtc.holoop['gain']
-            #delay       = np.floor(td/Ts)
+            #delay       = np.floor(delay/Ts)
                        
             # Instantiation
             h1          = np.zeros((nPts,nPts),dtype=complex)
             h2          = np.zeros((nPts,nPts))
             hn          = np.zeros((nPts,nPts))
             
             # Get the noise propagation factor
@@ -504,14 +507,29 @@
                 psd *= (dk * rad2nm)**2
                 psd *= wfe**2/psd.sum()
                 
             # Fitting
             self.psdFit = np.real(self.fittingPSD())
             psd += np.repeat(self.psdFit[:, :, np.newaxis], self.ao.src.nSrc, axis=2)
             
+            # Tilt filter
+            if self.applyTiltFilter == True:
+                tiltFilter = self.TiltFilter()                      
+                for i in range(self.ao.src.nSrc):
+                    psd[:,:,i] *= tiltFilter
+            
+            # Extra error
+            if self.verbose:
+                print('extra error in nm RMS: ',self.ao.tel.extraErrorNm)
+                print('extra error spatial frequency exponent: ',self.ao.tel.extraErrorExp)
+            if self.ao.tel.extraErrorNm > 0:
+                self.psdExtra = np.real(self.extraErrorPSD())
+                for i in range(self.ao.src.nSrc):
+                    psd[:,:,i] += self.psdExtra
+            
         self.t_powerSpectrumDensity = 1000*(time.time() - tstart)
             
         # Return the 3D PSD array in nm^2
         return psd * (dk * rad2nm)**2
     
     def fittingPSD(self):
         """ Fitting error power spectrum density """                 
@@ -630,15 +648,15 @@
         tstart  = time.time()   
         nK  = self.freq.resAO
         psd = np.zeros((nK,nK,self.ao.src.nSrc),dtype=complex)        
         i   = complex(0,1)
         nH  = self.ao.atm.nL
         Hs  = self.ao.atm.heights * self.strechFactor
         Ws  = self.ao.atm.weights
-        deltaT  = (1 + self.ao.rtc.holoop['delay'])/self.ao.rtc.holoop['rate']
+        deltaT  = self.ao.rtc.holoop['delay']/self.ao.rtc.holoop['rate']
         wDir_x  = np.cos(self.ao.atm.wDir*np.pi/180)
         wDir_y  = np.sin(self.ao.atm.wDir*np.pi/180)
         Watm    = self.Wphi * self.freq.pistonFilterAO_      
         F       = self.Rx*self.SxAv + self.Ry*self.SyAv
         
         for s in range(self.ao.src.nSrc):
             if self.nGs < 2:  
@@ -725,21 +743,21 @@
         tstart  = time.time()
         
         psd= np.zeros((self.freq.resAO,self.freq.resAO,self.ao.src.nSrc))
         if self.ao.tel.zenith_angle != 0:
             Hs   = self.ao.atm.heights * self.strechFactor
             Ws   = self.ao.atm.weights
             Watm = self.Wphi * self.freq.pistonFilterAO_     
-            A    = 0
             k    = np.sqrt(self.freq.k2AO_)
             arg_k= np.arctan2(self.freq.kyAO_,self.freq.kxAO_)
             azimuth = self.ao.src.azimuth
         
             theta = differentialRefractiveAnisoplanatism(self.ao.tel.zenith_angle*np.pi/180,self.gs.wvl[0], self.freq.wvlRef)
             for s in range(self.ao.src.nSrc):
+                A    = 0
                 for l in range(self.ao.atm.nL):
                     A   = A + 2*Ws[l]*(1 - np.cos(2*np.pi*Hs[l]*k*np.tan(theta)*np.cos(arg_k-azimuth[s])))            
                 psd[:,:,s] = self.freq.mskInAO_ *A*Watm
          
         self.t_differentialRefractionPSD = 1000*(time.time() - tstart)
         return  psd
       
@@ -770,14 +788,15 @@
         
         #Instantiate the function output
         psd      = np.zeros((self.freq.nOtf,self.freq.nOtf))
         # atmo PSD 
         psd_atmo = self.ao.atm.spectrum(np.sqrt(self.freq.k2_))    
         
         nPoints = 1001
+        nPhase = 5 # number of phase shift cases
         x = self.ao.tel.D*np.linspace(-0.5, 0.5, nPoints, endpoint=1)
         h = self.ao.atm.heights
         h_laser = self.gs.height[0]
         ratio = (h_laser-h)/h_laser
         nCn2 = len(h)
         freqs = self.freq.kx_[int(np.ceil(self.freq.nOtf/2)-1):,0]
         if freqs[0] < 0:
@@ -792,33 +811,96 @@
             print('ratio',ratio)
         
         for j in range(nCn2):
             for i in range(nf0):
                 if freqs[i]*ratio[j] > self.freq.kc_:
                     coeff[i,j] = 0.0
                 else:
-                    sin_ref = np.sin(2*np.pi*freqs[i]*x)
-                    sin_temp = np.sin(2*np.pi*freqs[i]*ratio[j]*x)
-                    sin_res = sin_ref - sin_temp
                     if freqs[i] < 1e-5:
-                        coeff[i,j] = 1-ratio[j]
+                        coeff[i,j] = 0
                     else:
-                        coeff[i,j] = np.sqrt(np.mean(abs(sin_res)**2.)) / np.sqrt(np.mean(abs(sin_ref)**2.))
+                        for k in range(nPhase):
+                            sin_ref = np.sin(2*np.pi*freqs[i]*x+2*np.pi*k/nPhase)
+                            sin_temp = np.sin(2*np.pi*freqs[i]*ratio[j]*x+2*np.pi*k/nPhase)
+                            sin_res = sin_ref - np.std(sin_ref)/np.std(sin_temp)*sin_temp
+                            coeff[i,j] += np.std(sin_res) / np.std(sin_ref) * 1/nPhase
                          
             coeff_tot = np.interp(np.sqrt(self.freq.k2_), freqs, coeff[:,j])**2
             
             #fig, ax1 = plt.subplots(1,1)
-            #im = ax1.imshow(coeff_tot, cmap='hot')
-            #ax1.set_title('cone effect filter coefficients', color='black')
+            #im = ax1.plot(coeff)
+            #fig, ax2 = plt.subplots(1,1)
+            #im = ax2.imshow(coeff_tot, cmap='hot')
+            #ax2.set_title('cone effect filter coefficients', color='black')
             
             psd += coeff_tot*psd_atmo*self.ao.atm.weights[j]
         
         self.t_focalAnisoplanatism = 1000*(time.time() - tstart)
         
         return np.real(psd)
+    
+    def extraErrorPSD(self):
+    
+        k   = np.sqrt(self.freq.k2_)
+        psd = k**self.ao.tel.extraErrorExp
+        pf  = FourierUtils.pistonFilter(self.ao.tel.D,k)
+        psd = psd * pf
+        if self.ao.tel.extraErrorMin>0:
+            psd[np.where(k<self.ao.tel.extraErrorMin)] = 0
+        
+        psd = psd * self.ao.tel.extraErrorNm**2/np.sum(psd)
+        
+        #fig, ax1 = plt.subplots(1,1)
+        #im = ax1.imshow(np.log(np.abs(psd)), cmap='hot')
+        #ax1.set_title('extra error PSD', color='black') 
+        
+        # Derives wavefront error
+        rad2nm = (2*self.freq.kcMax_/self.freq.resAO) * self.freq.wvlRef*1e9/2/np.pi 
+        
+        psd = psd * 1/rad2nm**2
+    
+        return np.real(psd)
+    
+    def TiltFilter(self):
+        """%% Spatial filter to remove tilt related errors
+        """
+        
+        nPoints = 1001
+        nPhase = 10 # number of phase shift cases
+        x = self.ao.tel.D*np.linspace(-0.5, 0.5, nPoints, endpoint=1)
+        freqs = self.freq.kx_[int(np.ceil(self.freq.nOtf/2)-1):,0]
+        if freqs[0] < 0:
+            freqs = freqs[1:]
+        nf0 = len(freqs)
+        coeff = np.zeros(nf0)
+               
+        for i in range(nf0):
+            if freqs[i] == 0:
+                coeff[i] = 0
+            elif 1/freqs[i] < 0.1*self.ao.tel.D:
+                coeff[i] = 1
+            else:
+                for k in range(nPhase):
+                    sin_ref = np.sin(2*np.pi*freqs[i]*x+2*np.pi*k/nPhase)
+                    coeff_lin = np.polyfit(x,sin_ref,1)
+                    sin_temp = coeff_lin[0]*x+coeff_lin[1]
+                    sin_res = sin_ref - sin_temp
+                    coeff[i] += np.std(sin_res) / np.std(sin_ref) * 1/nPhase
+               
+        coeff_tot = np.interp(np.sqrt(self.freq.k2_), freqs, coeff)**2
+        
+        #fig, ax1 = plt.subplots(1,1)
+        #im = ax1.plot(coeff)      
+        #plt.xlim([0, 20])
+        #fig, ax2 = plt.subplots(1,1)
+        #from matplotlib import colors
+        #im = ax2.imshow(coeff_tot, cmap='hot', norm=colors.LogNorm())
+        #ax2.set_title('tilt filter coefficients', color='black')
+            
+        return np.real(coeff_tot)
        
 #%% AO ERROR BREAKDOWN
     def errorBreakDown(self,verbose=True):
         """ AO error breakdown from the PSD integrals
         """        
         tstart  = time.time()
         
@@ -834,19 +916,20 @@
             self.wfeFit    = np.sqrt(self.psdFit.sum()) * rad2nm
             self.wfeAl     = np.sqrt(self.psdAlias.sum()) * rad2nm
             self.wfeN      = np.sqrt(self.psdNoise.sum(axis=(0,1)))* rad2nm
             self.wfeST     = np.sqrt(self.psdSpatioTemporal.sum(axis=(0,1)))* rad2nm
             self.wfeDiffRef= np.sqrt(self.psdDiffRef.sum(axis=(0,1)))* rad2nm
             self.wfeChrom  = np.sqrt(self.psdChromatism.sum(axis=(0,1)))* rad2nm
             self.wfeJitter = 1e9*self.ao.tel.D*np.mean(self.ao.cam.spotFWHM[0][0:2])/rad2mas/4
+            self.wfeExtra  = self.ao.tel.extraErrorNm
             
             # Total wavefront error
             self.wfeTot = np.sqrt(self.wfeNCPA**2 + self.wfeFit**2 + self.wfeAl**2\
                                   + self.wfeST**2 + self.wfeN**2 + self.wfeDiffRef**2\
-                                  + self.wfeChrom**2 + self.wfeJitter**2)
+                                  + self.wfeChrom**2 + self.wfeJitter**2 + self.wfeExtra**2)
             
             # Maréchal appoximation to get the Strehl-ratio
             self.SRmar  = 100*np.exp(-(self.wfeTot*2*np.pi*1e-9/self.freq.wvlRef)**2)
             
             # bonus
             self.psdS = self.servoLagPSD()
             self.wfeS = np.sqrt(self.psdS.sum()) * rad2nm
@@ -873,14 +956,15 @@
                 print('.Aliasing error:\t\t%4.2fnm'%self.wfeAl)
                 if self.nGs == 1:
                     print('.Noise error:\t\t\t%4.2fnm'%self.wfeN)
                 else:
                     print('.Noise error:\t\t\t%4.2fnm'%self.wfeN[idCenter])
                 print('.Spatio-temporal error:\t\t%4.2fnm'%self.wfeST[idCenter])
                 print('.Additionnal jitter:\t\t%4.2fmas / %4.2fnm'%(np.mean(self.ao.cam.spotFWHM[0][0:2]),self.wfeJitter))
+                print('.Extra error:\t\t\t%4.2fnm'%self.wfeExtra)
                 print('-------------------------------------------')
                 print('.Sole servoLag error:\t\t%4.2fnm'%self.wfeS)
                 print('.Sole reconstruction error:\t%4.2fnm'%self.wfeR)
                 print('-------------------------------------------')            
                 if self.nGs == 1:
                     print('.Sole anisoplanatism error:\t%4.2fnm'%self.wfeAni[idCenter])
                 else:
@@ -1133,15 +1217,16 @@
                 # Controller
                 print("Required time for controller instantiation (ms)\t : {:f}".format(self.t_controller))
                 # PSD
                 print("Required time for fitting PSD calculation (ms)\t : {:f}".format(self.t_fittingPSD))
                 print("Required time for aliasing PSD calculation (ms)\t : {:f}".format(self.t_aliasingPSD))
                 print("Required time for noise PSD calculation (ms)\t : {:f}".format(self.t_noisePSD))
                 print("Required time for ST PSD calculation (ms)\t : {:f}".format(self.t_spatioTemporalPSD))
-                print("Required time for focal Aniso PSD calculation (ms)\t : {:f}".format(self.t_focalAnisoplanatism))
+                if hasattr(self,"t_focalAnisoplanatism"):
+                    print("Required time for focal Aniso PSD calculation (ms)\t : {:f}".format(self.t_focalAnisoplanatism))
                 
                 # Error breakdown
                 if hasattr(self,'t_errorBreakDown'):
                     print("Required time for error calculation (ms)\t : {:f}".format(self.t_errorBreakDown))
                     
                 # PSF metrics
                 if hasattr(self,'t_getPsfMetrics'):
```

### Comparing `astro-p3-1.0/p3/aoSystem/frequencyDomain.py` & `astro-p3-1.1/p3/aoSystem/frequencyDomain.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/optics.py` & `astro-p3-1.1/p3/aoSystem/optics.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/HarmoniLTAO.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/HarmoniLTAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/HarmoniSCAO.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/HarmoniSCAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/MavisMCAO.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/MavisMCAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/MosaicGLAO.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/MosaicGLAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/eris.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/eris.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/irdis.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/irdis.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/nirc2.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/nirc2.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/nirc2_monochromatic.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/nirc2_monochromatic.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/parFiles/template.ini` & `astro-p3-1.1/p3/aoSystem/parFiles/template.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/processing.py` & `astro-p3-1.1/p3/aoSystem/processing.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/pupil.py` & `astro-p3-1.1/p3/aoSystem/pupil.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/rtc.py` & `astro-p3-1.1/p3/aoSystem/rtc.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/segment.py` & `astro-p3-1.1/p3/aoSystem/segment.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/sensor.py` & `astro-p3-1.1/p3/aoSystem/sensor.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/source.py` & `astro-p3-1.1/p3/aoSystem/source.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/spiders.py` & `astro-p3-1.1/p3/aoSystem/spiders.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/telescope.py` & `astro-p3-1.1/p3/aoSystem/telescope.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,28 +49,32 @@
     @property
     def airmass(self):
         return 1/np.cos(self.zenith_angle*np.pi/180)
     
     # CONSTRUCTOR
     def __init__(self,D,resolution, zenith_angle=0.0,obsRatio=0.0,pupilAngle = 0.0,\
                  path_pupil='', path_static_on='', path_static_off='', path_static_pos='',\
-                 path_apodizer='', path_statModes='', verbose=True):
+                 path_apodizer='', path_statModes='', extraErrorNm=0.0, extraErrorExp=-2, \
+                 extraErrorMin=0.0, verbose=True):
         
         # PARSING INPUTS
         self.D               = D            # primary mirror diameter in meters
         self.zenith_angle    = zenith_angle # telescope zenith angle in degrees
         self.obsRatio        = obsRatio     # secondary mirror diameter in D units
         self.resolution      = resolution   # pupil resolution in pixels
         self.verbose         = verbose
         self.pupilAngle      = pupilAngle
         self.path_pupil      = path_pupil
         self.path_static_on  = path_static_on
         self.path_static_pos = path_static_off
         self.path_apodizer   = path_apodizer
         self.path_statModes  = path_statModes
+        self.extraErrorNm    = extraErrorNm
+        self.extraErrorExp   = extraErrorExp
+        self.extraErrorMin   = extraErrorMin
         
         #----- PUPIL DEFINITION        
         
         pupil = [] 
         if path_pupil!= '' and ospath.isfile(path_pupil) == True and re.search(".fits",path_pupil)!=None:
             self.verb = True
             pupil = fits.getdata(path_pupil)
```

### Comparing `astro-p3-1.0/p3/aoSystem/testing/tests_aoSystem.py` & `astro-p3-1.1/p3/aoSystem/testing/tests_aoSystem.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/testing/tests_tiptop_compatibility.py` & `astro-p3-1.1/p3/aoSystem/testing/tests_tiptop_compatibility.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/aoSystem/zernike.py` & `astro-p3-1.1/p3/aoSystem/zernike.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/dataBaseVerification.py` & `astro-p3-1.1/p3/deepLoop/dataBaseVerification.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/dataGenerator.py` & `astro-p3-1.1/p3/deepLoop/dataGenerator.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/dataGeneratorBatch.py` & `astro-p3-1.1/p3/deepLoop/dataGeneratorBatch.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/deepLoopPerformance.py` & `astro-p3-1.1/p3/deepLoop/deepLoopPerformance.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/deepLoopPerformanceBatch.py` & `astro-p3-1.1/p3/deepLoop/deepLoopPerformanceBatch.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/jobGenerate.sh` & `astro-p3-1.1/p3/deepLoop/jobGenerate.sh`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/jobPerformance.sh` & `astro-p3-1.1/p3/deepLoop/jobPerformance.sh`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/deepLoop/recover_list.py` & `astro-p3-1.1/p3/deepLoop/recover_list.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/psfFitting/confidenceInterval.py` & `astro-p3-1.1/p3/psfFitting/confidenceInterval.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/psfFitting/fittingUtils.py` & `astro-p3-1.1/p3/psfFitting/fittingUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/psfFitting/imageModel.py` & `astro-p3-1.1/p3/psfFitting/imageModel.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/psfFitting/psfFitting.py` & `astro-p3-1.1/p3/psfFitting/psfFitting.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/psfao21/psfao21.py` & `astro-p3-1.1/p3/psfao21/psfao21.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/psfr/psfR.py` & `astro-p3-1.1/p3/psfr/psfR.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/psfr/psfrUtils.py` & `astro-p3-1.1/p3/psfr/psfrUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/telemetry/configFile.py` & `astro-p3-1.1/p3/telemetry/configFile.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/telemetry/keckUtils.py` & `astro-p3-1.1/p3/telemetry/keckUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/telemetry/massdimm.py` & `astro-p3-1.1/p3/telemetry/massdimm.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/telemetry/sphereUtils.py` & `astro-p3-1.1/p3/telemetry/sphereUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/telemetry/systemDiagnosis.py` & `astro-p3-1.1/p3/telemetry/systemDiagnosis.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/telemetry/telemetryKASP.py` & `astro-p3-1.1/p3/telemetry/telemetryKASP.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/telemetry/telemetryKeck.py` & `astro-p3-1.1/p3/telemetry/telemetryKeck.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.0/p3/testing/tests_p3.py` & `astro-p3-1.1/p3/testing/tests_p3.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 rad2mas = 3600 * 180 * 1e3/np.pi
 
 #%% MANAGING PATHS
 path_root = str(pathlib.Path(psfao21Main.__file__).parent.parent.parent.absolute()) +"/"
 path_p3 = str(pathlib.Path(psfao21Main.__file__).parent.parent.absolute())
 path_ini = path_p3 + '/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini'
-path_img = path_p3 + '/data/20130801_n0004.fits'
+path_img = path_p3 + '/../data/20130801_n0004.fits'
 path_calib = path_p3 + '/aoSystem/data/KECK_CALIBRATION/'
 
 im_nirc2 = fits.getdata(path_img, ignore_missing_simple=True)
 filename   = 'n0004_fullNGS_trs.sav'
 
 #%% TEST THE SPATIAL FREQUENCY ADAPTIVE OPTICS MODEL
```

### Comparing `astro-p3-1.0/pyproject.toml` & `astro-p3-1.1/pyproject.toml`

 * *Files identical despite different names*

