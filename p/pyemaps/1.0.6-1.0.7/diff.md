# Comparing `tmp/pyemaps-1.0.6.tar.gz` & `tmp/pyemaps-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\.tmp-psmco31c\pyemaps-1.0.6.tar", last modified: Sat May 27 18:57:36 2023, max compression
+gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\.tmp-09mz0306\pyemaps-1.0.7.tar", last modified: Fri Jul  7 18:10:28 2023, max compression
```

## Comparing `pyemaps-1.0.6.tar` & `pyemaps-1.0.7.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/
--rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.6/COPYING
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/CifFile/
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/CifFile/src/
--rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.6/CifFile/src/CifFile_module.py
--rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.6/CifFile/src/StarFile.py
--rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/TypeContentsParser.py
--rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_1_0.py
--rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_1_1.py
--rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_2_0.py
--rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_STAR2.py
--rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/CifFile/src/drel/
--rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/__init__.py
--rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/drel_ast_yacc.py
--rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/drel_lex.py
--rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/drel_runtime.py
--rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/parsetab.py
--rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/py_from_ast.py
--rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/parsetab.py
--rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/yapps3_compiled_rt.py
--rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      885 2023-05-27 18:57:36.000000 pyemaps-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.6/README.md
--rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.6/__config__.py
--rw-rw-rw-   0        0        0     6050 2023-05-27 18:00:42.000000 pyemaps-1.0.6/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.6/__main__.py
--rw-rw-rw-   0        0        0       21 2023-05-27 18:57:19.000000 pyemaps-1.0.6/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/cdata/
--rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Aluminium.xtl
--rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/AluminiumOxide.xtl
--rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Aluminium_FCC.xtl
--rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BariumTitanate_180k.xtl
--rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BariumTitanate_270k.xtl
--rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BariumTitanate_Tetra.xtl
--rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BiMnO3.xtl
--rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Boron_Tetra.xtl
--rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CadmiumSelenide_Hex.xtl
--rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CadmiumSulfide_Cubic.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CadmiumSulfide_Hex.xtl
--rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Chromium_BCC.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CoSb3_Skutterudite.xtl
--rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CopperOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Copper_FCC.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Cu2O_Cuprite.xtl
--rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Diamond.xtl
--rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/ErbiumPyrogermanate.xtl
--rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/FePd_Tetra.xtl
--rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/FeS2_Pyrite.xtl
--rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/GalliumAntimonide.xtl
--rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/GalliumArsenide.xtl
--rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/GalliumNitride.xtl
--rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Germanium.xtl
--rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Gold_FCC.xtl
--rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/IndiumArsenide.xtl
--rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/LaMnO3.xtl
--rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/LeadZirconateTitanate.xtl
--rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Li2MnO3.xtl
--rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/NaFeO2.xtl
--rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Nb3Sn.xtl
--rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Pentacene.xtl
--rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.6/cdata/SiAlONa.xtl
--rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Silicon.xtl
--rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/StrontiumTitanate.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TelluriumDioxide.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TinDioxide_RT.xtl
--rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TitaniumDioxide_Anatase.xtl
--rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TitaniumDioxide_Rutile.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TungstenDiselenide.xtl
--rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/VanadiumDioxide_RT.xtl
--rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/ZincOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Zinc_HCP.xtl
--rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/ZirconiumNitride.xtl
--rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/limno2.xtl
--rw-rw-rw-   0        0        0    41593 2023-05-27 18:00:42.000000 pyemaps-1.0.6/crystals.py
--rw-rw-rw-   0        0        0     2582 2023-04-23 21:55:13.000000 pyemaps-1.0.6/ddiffs.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/diffract/
--rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.6/diffract/__init__.py
--rw-rw-rw-   0        0        0    28522 2023-05-12 19:12:49.000000 pyemaps-1.0.6/diffract/bloch_dec.py
--rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/csf_dec.py
--rw-rw-rw-   0        0        0    15552 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/dif_dec.py
--rw-rw-rw-   0        0        0     5020 2023-05-12 19:12:49.000000 pyemaps-1.0.6/diffract/dpgen_dec.py
--rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/mxtal_dec.py
--rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/powder_dec.py
--rw-rw-rw-   0        0        0     2350 2023-04-03 21:05:15.000000 pyemaps-1.0.6/diffract/stereo_dec.py
--rw-rw-rw-   0        0        0    20247 2023-05-27 18:00:42.000000 pyemaps-1.0.6/display.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/ediom/
--rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.6/ediom/ediom.py
--rw-rw-rw-   0        0        0    35563 2023-05-27 18:19:14.000000 pyemaps-1.0.6/ediom/ediom_dec.py
--rw-rw-rw-   0        0        0    27128 2023-04-23 21:55:13.000000 pyemaps-1.0.6/emcontrols.py
--rw-rw-rw-   0        0        0     7175 2023-05-26 02:13:51.000000 pyemaps-1.0.6/errors.py
--rw-rw-rw-   0        0        0    33216 2023-04-23 21:55:13.000000 pyemaps-1.0.6/fileutils.py
--rw-rw-rw-   0        0        0    30922 2023-04-23 21:55:13.000000 pyemaps-1.0.6/kdiffs.py
--rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.6/license.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/
--rw-rw-rw-   0        0        0      885 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5789 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/samples/
--rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/al.img
--rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.6/samples/al_db.bin
--rw-rw-rw-   0        0        0      797 2023-05-27 18:28:39.000000 pyemaps-1.0.6/samples/al_dpgen.py
--rw-rw-rw-   0        0        0     3899 2023-05-27 18:00:42.000000 pyemaps-1.0.6/samples/al_ediom.py
--rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/powder.py
--rw-rw-rw-   0        0        0     3610 2023-05-27 18:00:42.000000 pyemaps-1.0.6/samples/si_bloch.py
--rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.6/samples/si_constructor.py
--rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.6/samples/si_csf.py
--rw-rw-rw-   0        0        0     3953 2023-04-18 21:27:47.000000 pyemaps-1.0.6/samples/si_dif.py
--rw-rw-rw-   0        0        0     1698 2023-05-27 18:00:42.000000 pyemaps-1.0.6/samples/si_lacbed.py
--rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/si_pyemaps.py
--rw-rw-rw-   0        0        0     1707 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/si_rawblochimgs.py
--rw-rw-rw-   0        0        0     3884 2023-05-12 19:12:49.000000 pyemaps-1.0.6/samples/si_scm.py
--rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.6/samples/si_stereo.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/scattering/
--rw-rw-rw-   0        0        0      892 2023-04-03 21:05:15.000000 pyemaps-1.0.6/scattering/__init__.py
--rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.6/scattering/sct_dec.py
--rw-rw-rw-   0        0        0      734 2023-05-27 18:57:36.000000 pyemaps-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0    21587 2023-05-27 18:00:42.000000 pyemaps-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/spg/
--rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.6/spg/__init__.py
--rw-rw-rw-   0        0        0      793 2023-04-03 21:05:15.000000 pyemaps-1.0.6/spg/spg_dec.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/
+-rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.7/COPYING
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/CifFile/
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/CifFile/src/
+-rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.7/CifFile/src/CifFile_module.py
+-rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.7/CifFile/src/StarFile.py
+-rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/TypeContentsParser.py
+-rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/YappsStarParser_1_0.py
+-rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/YappsStarParser_1_1.py
+-rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/YappsStarParser_2_0.py
+-rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/YappsStarParser_STAR2.py
+-rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/CifFile/src/drel/
+-rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/drel/__init__.py
+-rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/drel/drel_ast_yacc.py
+-rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/drel/drel_lex.py
+-rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/drel/drel_runtime.py
+-rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/drel/parsetab.py
+-rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/drel/py_from_ast.py
+-rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/parsetab.py
+-rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.7/CifFile/src/yapps3_compiled_rt.py
+-rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      885 2023-07-07 18:10:28.000000 pyemaps-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.7/README.md
+-rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.7/__config__.py
+-rw-rw-rw-   0        0        0     6928 2023-07-07 18:08:24.000000 pyemaps-1.0.7/__init__.py
+-rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.7/__main__.py
+-rw-rw-rw-   0        0        0       21 2023-07-07 18:10:08.000000 pyemaps-1.0.7/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/cdata/
+-rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Aluminium.xtl
+-rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/AluminiumOxide.xtl
+-rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Aluminium_FCC.xtl
+-rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/BariumTitanate_180k.xtl
+-rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/BariumTitanate_270k.xtl
+-rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/BariumTitanate_Tetra.xtl
+-rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/BiMnO3.xtl
+-rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Boron_Tetra.xtl
+-rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/CadmiumSelenide_Hex.xtl
+-rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/CadmiumSulfide_Cubic.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/CadmiumSulfide_Hex.xtl
+-rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Chromium_BCC.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/CoSb3_Skutterudite.xtl
+-rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/CopperOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Copper_FCC.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Cu2O_Cuprite.xtl
+-rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Diamond.xtl
+-rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/ErbiumPyrogermanate.xtl
+-rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/FePd_Tetra.xtl
+-rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/FeS2_Pyrite.xtl
+-rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/GalliumAntimonide.xtl
+-rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/GalliumArsenide.xtl
+-rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/GalliumNitride.xtl
+-rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Germanium.xtl
+-rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Gold_FCC.xtl
+-rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/IndiumArsenide.xtl
+-rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/LaMnO3.xtl
+-rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/LeadZirconateTitanate.xtl
+-rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Li2MnO3.xtl
+-rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/NaFeO2.xtl
+-rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Nb3Sn.xtl
+-rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Pentacene.xtl
+-rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.7/cdata/SiAlONa.xtl
+-rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Silicon.xtl
+-rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/StrontiumTitanate.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/TelluriumDioxide.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/TinDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/TitaniumDioxide_Anatase.xtl
+-rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/TitaniumDioxide_Rutile.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/TungstenDiselenide.xtl
+-rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/VanadiumDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/ZincOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/Zinc_HCP.xtl
+-rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/ZirconiumNitride.xtl
+-rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.7/cdata/limno2.xtl
+-rw-rw-rw-   0        0        0    42129 2023-07-07 18:08:24.000000 pyemaps-1.0.7/crystals.py
+-rw-rw-rw-   0        0        0     2618 2023-07-07 18:08:24.000000 pyemaps-1.0.7/ddiffs.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/diffract/
+-rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.7/diffract/__init__.py
+-rw-rw-rw-   0        0        0    28900 2023-07-07 18:08:24.000000 pyemaps-1.0.7/diffract/bloch_dec.py
+-rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.7/diffract/csf_dec.py
+-rw-rw-rw-   0        0        0    15879 2023-07-07 18:08:24.000000 pyemaps-1.0.7/diffract/dif_dec.py
+-rw-rw-rw-   0        0        0     5020 2023-05-12 19:12:49.000000 pyemaps-1.0.7/diffract/dpgen_dec.py
+-rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.7/diffract/mxtal_dec.py
+-rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.7/diffract/powder_dec.py
+-rw-rw-rw-   0        0        0     2436 2023-07-07 18:08:24.000000 pyemaps-1.0.7/diffract/stereo_dec.py
+-rw-rw-rw-   0        0        0    23201 2023-07-07 18:08:24.000000 pyemaps-1.0.7/display.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/ediom/
+-rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.7/ediom/ediom.py
+-rw-rw-rw-   0        0        0    37563 2023-07-07 18:09:41.000000 pyemaps-1.0.7/ediom/ediom_dec.py
+-rw-rw-rw-   0        0        0    27443 2023-07-07 18:08:24.000000 pyemaps-1.0.7/emcontrols.py
+-rw-rw-rw-   0        0        0     7412 2023-07-07 18:08:24.000000 pyemaps-1.0.7/errors.py
+-rw-rw-rw-   0        0        0    33222 2023-07-07 18:08:24.000000 pyemaps-1.0.7/fileutils.py
+-rw-rw-rw-   0        0        0    31629 2023-07-07 18:08:24.000000 pyemaps-1.0.7/kdiffs.py
+-rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.7/license.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/pyemaps.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-07 18:10:27.000000 pyemaps-1.0.7/pyemaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5789 2023-07-07 18:10:28.000000 pyemaps-1.0.7/pyemaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:10:27.000000 pyemaps-1.0.7/pyemaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-07-07 18:10:27.000000 pyemaps-1.0.7/pyemaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 18:10:27.000000 pyemaps-1.0.7/pyemaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/samples/
+-rw-rw-rw-   0        0        0     2148 2023-07-07 18:08:24.000000 pyemaps-1.0.7/samples/adf.py
+-rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.7/samples/al.img
+-rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.7/samples/al_db.bin
+-rw-rw-rw-   0        0        0     2131 2023-07-07 18:08:24.000000 pyemaps-1.0.7/samples/al_dpgen.py
+-rw-rw-rw-   0        0        0     4119 2023-07-07 18:08:24.000000 pyemaps-1.0.7/samples/al_ediom.py
+-rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.7/samples/powder.py
+-rw-rw-rw-   0        0        0     3610 2023-05-27 23:58:52.000000 pyemaps-1.0.7/samples/si_bloch.py
+-rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.7/samples/si_constructor.py
+-rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.7/samples/si_csf.py
+-rw-rw-rw-   0        0        0     3953 2023-07-06 02:03:34.000000 pyemaps-1.0.7/samples/si_dif.py
+-rw-rw-rw-   0        0        0     1698 2023-05-27 23:58:52.000000 pyemaps-1.0.7/samples/si_lacbed.py
+-rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.7/samples/si_pyemaps.py
+-rw-rw-rw-   0        0        0     3884 2023-05-12 19:12:49.000000 pyemaps-1.0.7/samples/si_scm.py
+-rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.7/samples/si_stereo.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/scattering/
+-rw-rw-rw-   0        0        0      890 2023-07-07 18:08:24.000000 pyemaps-1.0.7/scattering/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.7/scattering/sct_dec.py
+-rw-rw-rw-   0        0        0      734 2023-07-07 18:10:28.000000 pyemaps-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0    21667 2023-07-07 18:08:24.000000 pyemaps-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:10:28.000000 pyemaps-1.0.7/spg/
+-rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.7/spg/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-07-07 18:08:24.000000 pyemaps-1.0.7/spg/spg_dec.py
+-rw-rw-rw-   0        0        0    29831 2023-07-07 18:08:24.000000 pyemaps-1.0.7/stackimg.py
```

### Comparing `pyemaps-1.0.6/COPYING` & `pyemaps-1.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/CifFile_module.py` & `pyemaps-1.0.7/CifFile/src/CifFile_module.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/StarFile.py` & `pyemaps-1.0.7/CifFile/src/StarFile.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/TypeContentsParser.py` & `pyemaps-1.0.7/CifFile/src/TypeContentsParser.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/YappsStarParser_1_0.py` & `pyemaps-1.0.7/CifFile/src/YappsStarParser_1_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/YappsStarParser_1_1.py` & `pyemaps-1.0.7/CifFile/src/YappsStarParser_1_1.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/YappsStarParser_2_0.py` & `pyemaps-1.0.7/CifFile/src/YappsStarParser_2_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/YappsStarParser_STAR2.py` & `pyemaps-1.0.7/CifFile/src/YappsStarParser_STAR2.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/drel/drel_ast_yacc.py` & `pyemaps-1.0.7/CifFile/src/drel/drel_ast_yacc.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/drel/drel_lex.py` & `pyemaps-1.0.7/CifFile/src/drel/drel_lex.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/drel/drel_runtime.py` & `pyemaps-1.0.7/CifFile/src/drel/drel_runtime.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/drel/parsetab.py` & `pyemaps-1.0.7/CifFile/src/drel/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/drel/py_from_ast.py` & `pyemaps-1.0.7/CifFile/src/drel/py_from_ast.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/parsetab.py` & `pyemaps-1.0.7/CifFile/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/CifFile/src/yapps3_compiled_rt.py` & `pyemaps-1.0.7/CifFile/src/yapps3_compiled_rt.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/PKG-INFO` & `pyemaps-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.6
+Version: 1.0.7
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyemaps-1.0.6/__config__.py` & `pyemaps-1.0.7/__config__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/__init__.py` & `pyemaps-1.0.7/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 """
 This file is part of pyemaps
-___________________________
 
 pyemaps is free software for non-comercial use: you can 
 redistribute it and/or modify it under the terms of the GNU General 
 Public License as published by the Free Software Foundation, either 
 version 3 of the License, or (at your option) any later version.
 
 pyemaps is distributed in the hope that it will be useful,
@@ -13,15 +12,14 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with pyemaps.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact supprort@emlabsoftware.com for any questions and comments.
-___________________________
 
 ```
 
 Author:     EMLab Solutions, Inc.
 Date:       May 07, 2022    
 """
 
@@ -164,20 +162,52 @@
     
 except ImportError as e:
     # skip this in free package
     pass
 
 
 # #------------------Diffraction Pattern Indexing - paid package only---------------------------
-#  used only with dpgen module ablove
+#  used only with dpgen module above
 
 try:
     from .ediom import ediom
 except ImportError:
     pass
+else:
+    E_INT = ediom.E_INT 
+    EM_INT = ediom.EM_INT
+
+    E_FLOAT = ediom.E_FLOAT
+    EM_FLOAT = ediom.EM_FLOAT
+
+    E_DOUBLE = ediom.E_DOUBLE
+    EM_DOUBLE = ediom.EM_DOUBLE
+
+    MAX_IMAGESIZE = ediom.MAX_IMAGESIZE
+    MIN_IMAGESIZE = ediom.MIN_IMAGESIZE
+    MAX_IMAGESTACK = ediom.MAX_IMAGESTACK
+    MIN_IMAGESTACK = 1
+    DEF_FILTER_THRESHOLD = 0.2                       
+    DEF_SEARCH_THRESHOLD = 0.825
+    DEF_RMIN = 7
+    DEF_BOXSIZE = 10
+    DEF_CC = ediom.cvar.edc.cc      #default value from backend
+    DEF_SIGMA = ediom.cvar.edc.sigma
+    DEF_ICENTER = ediom.cvar.edc.get_center()
+    DEF_XSCALE = 1
+    DEF_TSCALE = 2
+
+    E_SH = 0
+    E_RAW = 1
+    E_NPY = 2
+
+    # imageloading mode
+    EL_ONE = 1  #EDIOM image loading one stack at one time
+    EL_MORE = 2 #EDIOM image loading all stacks
+
 
 #--------------Wrapper classes around diffraction extensions---------------
 from .errors import *
 
 #---------Microscope control data classes handling data properties----------
 from .emcontrols import EMControl as EMC
 from .emcontrols import SIMControl as SIMC
@@ -189,10 +219,13 @@
 
 #--------------Crystal Classes and subclasses-------------------------------
 from .crystals import Cell, Atom, SPG, Crystal
 try:
     from .kdiffs import XMAX, YMAX
 except ImportError as e:
     print(f'Error importing kinematic constants: {e}')
-    
+
+#--------------ediom features -------------------------------
+from .stackimg import StackImage
+
 #--------------Pyemaps Display Functions-------------------------------------
 from .display import showDif, showBloch, showStereo
```

### Comparing `pyemaps-1.0.6/__main__.py` & `pyemaps-1.0.7/__main__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/BiMnO3.xtl` & `pyemaps-1.0.7/cdata/BiMnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/Boron_Tetra.xtl` & `pyemaps-1.0.7/cdata/Boron_Tetra.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/ErbiumPyrogermanate.xtl` & `pyemaps-1.0.7/cdata/ErbiumPyrogermanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/FeS2_Pyrite.xtl` & `pyemaps-1.0.7/cdata/FeS2_Pyrite.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/LeadZirconateTitanate.xtl` & `pyemaps-1.0.7/cdata/LeadZirconateTitanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/Li2MnO3.xtl` & `pyemaps-1.0.7/cdata/Li2MnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/Pentacene.xtl` & `pyemaps-1.0.7/cdata/Pentacene.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/cdata/SiAlONa.xtl` & `pyemaps-1.0.7/cdata/SiAlONa.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/crystals.py` & `pyemaps-1.0.7/crystals.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,16 @@
         return self._gamma
 
     @a.setter
     def a(self, v=None): 
         '''
         Sets b cell length.
 
-        :param v: required, must be a numeral or numberal string
+        :param v: must be a numeral or numberal string
+        :type v: number or string, required
         
         ''' 
         av = 0.0 if v is None else v
 
         try:
             self._a = float(av)
 
@@ -210,15 +211,16 @@
             raise CellValueError(1, "b")
 
     @b.setter
     def b(self, v=None):
         '''
         Sets b cell length.
 
-        :param v: required, must be a numeral or numberal string
+        :param v: must be a numeral or numberal string
+        :type v: number or string, required
         
         ''' 
         bv = 0.0 if v is None else v
 
         try:
             self._b = float(bv)
 
@@ -226,15 +228,16 @@
             raise CellValueError(1, "b")
 
     @c.setter
     def c(self, v=None):
         '''
         Sets c cell length.
 
-        :param v: required, must be a numeral or numberal string
+        :param v: must be a numeral or numberal string
+        :type v: number or string, required
         
         ''' 
         cv = 0.0 if v is None else v
         try:
             self._c = float(cv)
 
         except ValueError as e:
@@ -242,45 +245,48 @@
 
 
     @alpha.setter
     def alpha(self, v=None):
         '''
         Sets cell alpha angle.
 
-        :param v: required, must be a numeral or numberal string
+        :param v: must be a numeral or numberal string
+        :type v: number or string, required
         
         ''' 
         av = 0.0 if v is None else v
         try:
             self._alpha = float(av)
 
         except ValueError as e:
             raise CellValueError("alpha")
 
     @beta.setter
     def beta(self, v=0.0):
         '''
         Sets cell beta angle.
 
-        :param v: required, must be a numeral or numberal string
+        :param v: must be a numeral or numberal string
+        :type v: number or string, required
         
         ''' 
         bv = 0.0 if v is None else v
         try:
             self._beta = float(bv)
 
         except ValueError as e:
             raise CellValueError("beta")
 
     @gamma.setter
     def gamma(self, v=0.0):
         '''
         Sets cell gamma angle.
 
-        :param v: required, must be a numeral or numberal string
+        :param v: must be a numeral or numberal string
+        :type v: number or string, required
         
         ''' 
         gv = 0.0 if v is None else v
         try:
             self._gamma = float(gv)
 
         except ValueError as e:
@@ -406,14 +412,15 @@
     """
     def __init__(self, a_type=iso.value, sym = '', data=None):
         """
         Internal representation of single atom in a crystal object.
 
         :param a_type: Atom thermal factor type.
         :type a_type: int, optional
+
         :param data: Atoms positional and other data input. 
         :type data: dict or list, optional
         :raise UCError: if data validation fails.
 
         """
         setattr(self, 'atype', a_type)
         setattr(self, 'symb', sym)
@@ -685,14 +692,15 @@
         except ValueError as e:
             raise SPGInvalidDataInputError()
         
     @setting.setter
     def setting(self, s=None):
         """
         Symmetry setting data.
+
         :param s: Symmetry setting number
         :type s: int or string, optional
         :raise SPGInvalidDataInputError: if s is not an integer or integer string
 
         """
         if s is None:
             sn = 0
@@ -754,27 +762,27 @@
 #---Powder diffraction Calculation and rendering---
 from .diffract.powder_dec import add_powder
 
 #---Kinematic diffraction patterns database generation (upcoming) 
 from .diffract.dpgen_dec import add_dpgen
 
 #---diffraction pattern indexing----
-from .ediom.ediom_dec import add_ediom
+# from .ediom.ediom_dec import add_ediom
 
 #---Stereodiagram---
 from .diffract.stereo_dec import add_stereo
 #   generates and plots stereographic projections
 
 #---Kinematic Diffraction Simulations---
 from .diffract.dif_dec import add_dif
 
 #---Dynamic Diffraction Simulations---
 from .diffract.bloch_dec import add_bloch
 
-@add_ediom
+# @add_ediom
 @add_dpgen    
 @add_mxtal              
 @add_stereo              
 @add_bloch              
 @add_powder
 @add_csf     
 @add_dif   
@@ -868,20 +876,22 @@
         si.name = 'Silicon' 
         
     .. note::
 
         All atoms in a crystal must have the same thermal type.
 
     """
+    
     def __init__(self, name="Diamond", data=None):
         """
         Default constructor for crystal object    
         
         :param name: Name of the crystal or default to 'Diamond'
         :type name: string, optional
+
         :param data: Other data of the crystal. 
         :type data: dict, optional
         :raise CrystalClassError: If data validations fail.
 
         
         The dictionary object example for Silicon:
 
@@ -953,35 +963,55 @@
 
         # initially nothing is loaded, no rvec and no load type
         self._loaded = False
         self._ltype = -1
 
     @property
     def cell(self):
-        ''' Cell constants '''
+        ''' 
+        
+        Cell constants 
+        
+        '''
         return self._cell
 
     @property
     def dw(self):
-        ''' Debye-Waller factor or thermal factor'''
+        ''' 
+        
+        Debye-Waller factor or thermal factor
+        
+        '''
         return self._dw
 
     @property
     def spg(self):
-        ''' Space group '''
+        ''' 
+        
+        Space group 
+        
+        '''
         return self._spg
 
     @property
     def atoms(self):
-        ''' atom list '''
+        ''' 
+        
+        atom list 
+        
+        '''
         return self._atoms
 
     @property
     def name(self):
-        ''' crystal name '''
+        ''' 
+        
+        crystal name 
+        
+        '''
         return self._name
 
     @cell.setter
     def cell(self, c):
         
         if c is None or not isinstance(c, Cell):
             raise CrystalClassError("Error: cell constant invalid")
@@ -1040,14 +1070,15 @@
         if vspg is None or not isinstance(vspg, SPG):
             raise CrystalClassError('Invalid space group data')
 
         self._spg = vspg
 
     def isISO(self):
         '''
+        
         Check if crystal thermal type is Isotropic or not 
 
         '''
         return self._dw == iso.value
 
     def __del__(self):
         
@@ -1110,27 +1141,31 @@
                  yield('cell', dict(self._cell))
             if k == "_spg":
                  yield('spg', dict(self._spg))
             if k == "_atoms":
                  yield('atoms', [dict(a) for a in self._atoms])
 
     def loaded(self):
+        
         '''
+        
         Check to see if crystal data is loaded into simulation module
         or not.
         
         :return: `True` - loaded; otherwise `False`
         :rtype: bool
 
         '''
         return self._loaded
 
     @classmethod
     def from_builtin(cls, cn='Diamond'):
+        
         """        
+        
         Create a crystal by importing data from pyemaps build-in 
         crystal database
         
         :param cn: Name of the crystal in pyemaps's builtin database.
         :type cn: string, optional
         :raise CrystalClassError: If reading database fails or any of its components 
                                   fail to validate.
@@ -1156,14 +1191,15 @@
         except (FileNotFoundError, IOError) as e:
             raise CrystalClassError('Error creating crystal: ' + str(e))
         else:
             return xtl
 
     @classmethod
     def from_xtl(cls, fn):
+        
         """
         To create a crystal object by importing data from xtl formtted file.
 
         :param fn: Crystal data file name in pyemaps propietory format.
         :type fn: string, required
         :raise CrystalClassError: file reading fails or any of its components fail to validate.
 
@@ -1222,14 +1258,15 @@
         except (FileNotFoundError, AttributeError) as e:
             raise CrystalClassError(e.message)
         else:
             return xtl
     
     @classmethod
     def from_cif(cls, fn):
+        
         """
         import crystal data from a cif (Crystallographic Information File).
 
         :param fn: Crystal data file name in JSON format.
         :type fn: string, required
         :raise CrystalClassError: If file reading fails or any of its components 
                                   (cell, atoms, spg) fail to validate.
@@ -1253,14 +1290,15 @@
         except (CIFError, AttributeError, CellError, UCError, SPGError) as e:
             raise CrystalClassError(e.message) from None
         else:
             return cif
 
     @classmethod 
     def from_json(cls, jfn):
+        
         """
         Import crystal data from a .json file.
 
         :param jfn: Crystal data file name in JSON format.
         :type jfn: string, required
         :raise CrystalClassError: If file reading fails or any of its components fail to validate.
 
@@ -1315,14 +1353,15 @@
             if 'name' not in data:
                 raise CrystalClassError('Json data must have name field')
 
             return cls(name = data['name'], data = data)
 
     @classmethod
     def from_dict(cls, cdict):
+        
         """
         Import crystal data from a python dictionary object.
         
         :param cdict: Crystal data file name in as a python dictionary object.
         :type cdict: dict, required
         :raise CrystalClassError: If any of its components import fails.
 
@@ -1363,15 +1402,17 @@
             raise CrystalClassError('Failed to create crystal object with input dictionary')
         
         name = cdict["name"]
         return cls(name=name, data = cdict)           
 
     @staticmethod
     def list_all_builtin_crystals():
+        
         """
+        
         To list all builtin crystals available in pyemaps built-in crystal database,
         use this routine to determine the name of the crystal to load using 
         `from_builtin <pyemaps.crystals.html#pyemaps.crystals.Crystal.from_builtin>`_.
 
         """
         import glob
         base_dir = os.path.realpath(__file__)
```

### Comparing `pyemaps-1.0.6/ddiffs.py` & `pyemaps-1.0.7/ddiffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,25 @@
 
 
 
 # Author:     EMLab Solutions, Inc.
 # Date:       July 17, 2022    
 # '''
 """
+
 Simple wrapper for dynamic simulation images.
 
 """
 from . import EMC
 from . import BlochListError
 class BlochImgs:
+
     '''
     list of Bloch image objects and its associated controls 
+
     '''
     def __init__(self, name):
         
         setattr(self, 'name', name)
         setattr(self, 'blochList', [])
 
     @property
@@ -72,16 +75,23 @@
            not hasattr(b, "__len__") or \
            b.ndim != 2:
             raise BlochListError('failed to add Bloch image object')
 
         self._blochList.append((emc, b))
     
     def sort(self):
-        '''Sort the bloch simulation results by controls'''
+
+        '''
+
+        Sort the bloch simulation results by controls
+
+        '''
         self._blochList.sort(key=lambda x: x[0])
                 
     def __getitem__(self, key):
+
         '''
         Array like method for retrieving DP
+
         '''
         
         return self._blochList[key]
```

### Comparing `pyemaps-1.0.6/diffract/__init__.py` & `pyemaps-1.0.7/diffract/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/diffract/bloch_dec.py` & `pyemaps-1.0.7/diffract/bloch_dec.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,51 +80,68 @@
                          em_controls = EMC(cl=200, # set smaller that 1000 default value
                                            simc = SIMC(gmax=1.0, 
                                                        excitation=(0.3,1.0)
                                                        )
                                             )
                     ):
         """
+
         Begins a dynamic diffraction (Bloch) simulation session. 
         The simulation results are retained in the session between this and 
         `endBloch call <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_. 
+        
         :param aperture: Optional. Objective aperture
         :type aperture: float
+        
         :param omega: Optional. Diagnization cutoff value
         :type omega: float
+        
         :param sampling: Optional. Number of sampling points
         :type sampling: int
+        
         :param dbsize: Diffracted beams size.
         :type dbsize: float, optional
+        
         :param em_controls: Optional. electron `microscope control <pyemaps.emcontrols.html#module-pyemaps.emcontrols>`_ object. 
         :type em_controls: pyemaps.EMC
+        
         :return: a tuple (n, ns) where ns is a list of sampling points; n is the number of sampling points
         :rtype: tuple 
+
         Default values:
+
         ::
+
             DEF_APERTURE = 1.0
             DEF_OMEGA = 10
             DEF_SAMPLING = 8
             DEF_CBED_DSIZE - 0.16
             DEF_DSIZE_LIMITS =(0.01, 0.5)
+
         .. note:: 
+
             During the simulation session, results are retained in pyemaps 
             bloch module. The following methods are used to retrieve the
             result before the end of session:
+
             1. `getBlochimages <pyemaps.crystals.html#pyemaps.crystals.Crystal.getBlochImages>`_. 
                Retrieve a list of bloch images
+
             2. `getSCMatrix <pyemaps.crystals.html#pyemaps.crystals.Crystal.getSCMatrix>`_. 
                Retrieve a scattering matrix at a sampling point
         
         .. note:: 
+
             Other information available during the session:
             
             a. List of sampling points, diffraction beams tilts etc 
                with `printIBDetails <pyemaps.crystals.html#pyemaps.crystals.Crystal.printIBDetails>`_;
+            
             b. getEigen function is folded into getSCMatrix call starting from Stable verion 1.0.3
+            
             c. Diagnization Miller indexes at each sampling point: 
                `getBeams <pyemaps.crystals.html#pyemaps.crystals.Crystal.getBeams>`_;
         
         """
         if aperture is None or not isinstance(aperture, (int, float)):
             raise BlochError('Objective aperture must be valid numberal')
 
@@ -194,14 +211,23 @@
         em_controls(mode = 2, 
                     dsize = dbsize,
                     aperture = aperture)                      
         
         em_controls.simc(omega = omega, 
                          sampling = sampling
                         )
+        # update x-axis if it was set to (0,0,0)
+        # and new xaxis is calculated by the backend
+
+        if em_controls.xaxis == DEF_XAXIS:
+            xa1 = 0
+            xa2 = 2
+            xa3 = 0
+            xa1, xa2, xa3 = dif.get_xaxis()
+            em_controls(xaxis = (xa1,xa2,xa3))
 
         self.session_controls=em_controls
         return nsampling, sp
 
     def getBlochImages(self, 
                   sample_thickness = DEF_THICKNESS,
                   pix_size = DEF_PIXSIZE,
@@ -416,15 +442,15 @@
 
         '''    
         ncalcbeams = bloch.getncalcbeams()
         if ncalcbeams <= 0:
             raise BlochError("failed to retrieve diffracted beams info")
 
         cb = farray(np.zeros((3, ncalcbeams), dtype=int))
-        # cb, ret = bloch.GETCALCBEAMS(cb)
+        
         cb, ret = bloch.getcalcbeams(cb)
 
         if ret != 0:
             raise BlochError("failed to retrieve incidental beams info")
 
         cbms = np.transpose(cb)
```

### Comparing `pyemaps-1.0.6/diffract/csf_dec.py` & `pyemaps-1.0.7/diffract/csf_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/diffract/dif_dec.py` & `pyemaps-1.0.7/diffract/dif_dec.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,26 @@
             raise DPError('failed to generate diffraction patterns')
 
         # update the controls
         
         em_controls(mode=mode)
         if mode == 2:
             em_controls(dsize=dsize)
-            
+        
+        # @70323 merge
+        # update x-axis if it was set to (0,0,0)
+        # and new xaxis is calculated by the backend
+
+        if em_controls.xaxis == DEF_XAXIS:
+            xa1 = 0
+            xa2 = 2
+            xa3 = 0
+            xa1, xa2, xa3 = dif.get_xaxis()
+            em_controls(xaxis = (xa1,xa2,xa3))
+
         return em_controls, DP(diffp)
 
     def _get_diffraction(self, zone = None, 
                               mode = None, 
                               tx0 = None, 
                               ty0 = None, 
                               dx0 = None,
@@ -278,15 +289,15 @@
          stabel production soon. Its replacement is:
          `generateDP <pyemaps.crystals.html#pyemaps.crystals.Crystal.generateDP>`_.
 
         :param mode: mode of kinemetic diffraction - normal(1) or CBED(2).
         :type mode: int
 
         :param dsize: diffractted beam size, only applied to CBED mode.
-        :param dsize: float
+        :type dsize: float
 
         :param em_controls: electron microscope controls object.
         :type em_controls: pyemaps.EMC
 
         :return: myDif.
         :rtype: pyemaps.DPList.
```

### Comparing `pyemaps-1.0.6/diffract/dpgen_dec.py` & `pyemaps-1.0.7/diffract/dpgen_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/diffract/mxtal_dec.py` & `pyemaps-1.0.7/diffract/mxtal_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/diffract/powder_dec.py` & `pyemaps-1.0.7/diffract/powder_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/diffract/stereo_dec.py` & `pyemaps-1.0.7/diffract/stereo_dec.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,22 @@
         
         """
         from . import dif, stereo
         
         import numpy as np
         from numpy import asfortranarray as farray
 
-        from ..errors import StereodiagramError
+        from ..errors import StereodiagramError 
+        from .. import DEF_XAXIS
 
         dif.initcontrols()
-        dif.setzone(zone[0], zone[1], zone[2])
-        dif.set_xaxis(1, xa[0], xa[1], xa[2])
+        dif.setzone(zone[0], zone[1], zone[2])        
+        
+        if xa != DEF_XAXIS:
+            dif.set_xaxis(1, xa[0], xa[1], xa[2])
         dif.setsamplecontrols(tilt[0], tilt[1], 0.0, 0.0)
 
         # load the crystal
         
         self.load()
 
         ret = dif.diffract(3)
```

### Comparing `pyemaps-1.0.6/display.py` & `pyemaps-1.0.7/display.py`

 * *Files 10% similar despite different names*

```diff
@@ -469,24 +469,30 @@
             bClose = False):
    
     """
     Render kinematic diffraction pattern generated by pyemaps.
 
     :param dpl: Kinematic difraction pattern object list `DPList <pyemaps.kdiffs.html#pyemaps.kdiffs.DPList>`_
     :type dpl: DPList
+
     :param cShow: Plot control annotation. `True` (default): plot the control parameters on lower left corner; `False` do not plot.
     :type cShow: bool, optional
+
     :param kShow: Whether to display Kikuchi lines.
     :type kShow: bool 
+
     :param iShow: Whether to display Miller indexes.
     :type iShow: bool 
+
     :param layout: layout format. individual (default): plotting one by one, table: plotting in a table of 3 columns  
     :type layout: str, optional 
+
     :param bSave: Whether to save the diplay into a .png image file.
     :type bSave: bool    
+
     :param bClose: Whether to close plotting window when finished. Default: False - users must close it. 
     :type bClose: bool, optional  
     
     """
     from pyemaps import DPList
 
     if not dpl or not isinstance(dpl, DPList):
@@ -516,22 +522,27 @@
               bSave = False,
               bClose = False):
     """
     Render dynamic diffraction pattern generated by pyemaps.
 
     :param bimgs: Optional. Dynamic difraction pattern object list `BImgList <pyemaps.ddiffs.html#pyemaps.ddiffs.BlochImgs>`_
     :type bimgs: BlochImgs 
+
     :param cShow: Plot control annotation. `True` (default): plot the control parameters on lower left corner; `False` do not plot.
     :type cShow: bool, optional
+
     :param bColor: Optional. Whether to display the image in predefined color map.
     :type bColor: bool 
+
     :param layout: layout format. individual (default): plotting one by one, table: plotting in a table of 3 columns  
     :type layout: str, optional
+
     :param bSave: Optional. Whether to save the image into a .im3 image file.
     :type bSave: bool    
+
     :param bClose: Whether to close plotting window when finished. Default: False - users must close it. 
     :type bClose: bool, optional  
     
     """
     from pyemaps import BImgList
 
     if not bimgs or not isinstance(bimgs, BImgList):
@@ -566,24 +577,30 @@
                bClose = False):     # close the plotting window when done  
     
     """
     Render stereodiagram generated by pyemaps.
 
     :param slist: Stereodiagram output from `generateStereo <pyemaps.crystals.html#pyemaps.crystals.Crystal.generateStereo>`_.
     :type slist: list, required
+
     :param cShow: Plot control annotation. `True` (default): plot the control parameters on lower left corner; `False` do not plot.
     :type cShow: bool, optional
+
     :param iShow: Whether to display Miller indexes or not.
     :type iShow: bool, optional
+
     :param zLimit: Miller indexes cutoff number.
-    :type zLimit: int, optional  
+    :type zLimit: int, optional 
+
     :param layout: layout format. individual (default): plotting one by one in sequence, table: plotting in a table of 3 columns  
     :type layout: str, optional 
+
     :param bSave: Whether to save the image into a .png image file.
     :type bSave: bool, optional  
+    
     :param bClose: Whether to close plotting window when finished. Default: False - users must close it. 
     :type bClose: bool, optional  
 
 
 
     .. note::
 
@@ -624,8 +641,107 @@
 
 def _getGridPos(i, nCols = 3):
     
     ncols = i % nCols
 
     nrows = i // nCols
 
-    return nrows, ncols
+    return nrows, ncols
+
+# image display for ediom module
+
+
+def normalizeImage(img):
+    if img is None:
+        print("Probe error: image file empty")
+        return False
+    y0 = np.mean(img, dtype=np.float32)
+    medImg = np.std(img, dtype=np.float32)
+
+    Ymin1 = y0 - 3.0 * medImg
+    Ymin = np.amin(img)
+    if Ymin < Ymin1: Ymin = Ymin1
+
+    Ymax1 = y0 + 3.0 * medImg
+    Ymax = np.amax(img)
+    if Ymax > Ymax1: Ymax = Ymax1
+
+    if Ymin >= Ymax:
+        print("not finding right min-max: ")
+        return False
+    ran = Ymax-Ymin
+
+    img[img < Ymin] = Ymin
+    img[img > Ymax] = Ymax
+    img = (img - Ymin)/ran
+    return True
+
+def displayXImage(img, 
+                fsize=(0,0), 
+                bColor= False, 
+                isMask = False, 
+                bIndexed=False, 
+                iShow = False, 
+                ds = None,
+                suptitle = ''):   
+        """
+        Internal ediom helper function displaying image.
+
+        :return:  
+        :rtype: None
+        
+        """
+        
+        import matplotlib.pyplot as plt
+        import matplotlib.patches as patches
+        from matplotlib.colors import LinearSegmentedColormap
+        clrs = ["#2973A5", "cyan", "limegreen", "yellow", "red"]
+        qedDPI = 600
+        gclrs=plt.get_cmap('gray')
+        EDIOM_TITLE = 'Pyemaps Preview - Ediom Diffraction Pattern Indexing'
+
+        nr,nc = fsize
+
+        if isMask:
+            bsize = (0.5, 0.5*int(nr/nc))
+        else:
+            bsize = (1.0, 1.0*int(nr/nc))
+
+        fig, ax = plt.subplots(figsize=bsize, dpi=qedDPI)
+        
+        fig.canvas.set_window_title(EDIOM_TITLE)
+        # ax.set_xlabel(suptitle, fontsize=1.5)
+        fig.suptitle(suptitle, va='top', fontsize=1.5)
+        
+        clrMap = gclrs #default to grey
+        if bColor:
+            clrMap = LinearSegmentedColormap.from_list("mycmap", clrs)
+        plt.imshow(img, cmap = clrMap)
+
+        ax.set_axis_off()
+        
+        count = 0
+        if ds is not None:
+            for d in ds:
+                cx, cy, rad, indx, itype = d
+                
+                if bIndexed and itype != 2 and count != 0:
+                    continue
+
+                centre = (cx, cy)
+                
+                circle = plt.Circle(centre, rad, 
+                                    fill=False, 
+                                    linewidth = 0.1, 
+                                    # alpha=0.6, 
+                                    color='white')
+                ax.add_patch(circle)
+                count += 1
+
+                if iShow:
+                    ax.text(centre[0],centre[1], 
+                        str(indx),
+                        {'color': 'red', 'fontsize': 1.4},
+                        horizontalalignment='center',
+                        verticalalignment='bottom')
+        
+        plt.show()
```

### Comparing `pyemaps-1.0.6/ediom/ediom.py` & `pyemaps-1.0.7/ediom/ediom.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/ediom/ediom_dec.py` & `pyemaps-1.0.7/ediom/ediom_dec.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
 
     clrs = ["#2973A5", "cyan", "limegreen", "yellow", "red"]
     qedDPI = 600
     gclrs=plt.get_cmap('gray')
     EDIOM_TITLE = 'Pyemaps Preview - Ediom Diffraction Pattern Indexing'
 
-    # @staticmethod
     def _imgNormalize(img):
         if img is None:
             print("Probe error: image file empty")
             return False
         y0 = np.mean(img, dtype=np.float32)
         medImg = np.std(img, dtype=np.float32)
 
@@ -333,14 +332,15 @@
                       fsize=(nc,nr), 
                       iShow=True, 
                       ds=kdisk,
                       suptitle = 'Matching Database Diffraction Pattern')
 
         return 0
     
+    @staticmethod
     def release_ediom(self):
         """
         Releases ediom internal memory. 
         
         This must be called after completing or existing from DP search and indexing calls.
 
         See an example of typical usage in sample code *al_ediom.py*
@@ -904,14 +904,67 @@
         # if bDebug:
         #     _displayFitImage(2*xnr, xnc)
         # _displayFitMap(mcol, mrow)
         
 
         return 0
 
+    def generateADF(self, 
+                    imgfn, 
+                    center=(0.0, 0.0), 
+                    rads = (0.0, 0.0),
+                    scol = 0.0,
+                    bShow=False):
+        """
+        generate an Annular Dark Field(ADF) image from an experimental image.
+
+        :param imgfn: experimental image file name. 
+        :type imgfn: string, required
+        
+        :param center: The center of ADF detector.
+        :type cc: tuple of floats
+
+        :param rads: a pair of radius for inner and outer ADF detector.
+        :type rads: tuple, optional.
+
+        :param scol: The size of the output image along column direction.
+        :type scol: float, optional
+
+        :param bShow: whether to display the resulting ADF image.
+        :type bShow: boolean, optional, default `False`
+
+        :return: status code, 0 successful, otherwise failed
+        :rtype: integer
+
+        """
+        if not isinstance(scol, (int, float)) or scol <= 0:
+            print(f'The size of the output image along column direction must be numeral and positive')
+            return
+        
+        if not isinstance(center, tuple) or len(center) !=2 or \
+           not all(isinstance(x, (int, float)) for x in center):
+            print(f'Invalid ADF detector center')
+            return
+        
+        if not isinstance(rads, tuple) or len(rads) !=2 or \
+           not all(isinstance(x, (int, float)) for x in rads) or \
+           rads[0] == rads[1]:
+            print(f'Invalid ADF detector inner and outer radius, it must be a pair of numerals')
+            return
+                   
+        ret = ediom.getADF(imgfn, center[0], center[1], rads[0], rads[1], scol)
+        if ret != 0:
+            print(f'Failed to generate ADF image for experimental image {imgfn}')
+            return
+        
+        if bShow:
+            self.viewExpImage()
+        
+    
+
     target.indexExpDP = indexExpDP
 
     # DP database functions
     target.loadDPDB = loadDPDB
     target.peekDBDPAt = peekDBDPAt
 
     target.viewExpImage = viewExpImage
@@ -919,10 +972,12 @@
     target.release_ediom = release_ediom
     target.printDPIndexDetails = printDPIndexDetails
     target.importSHExpImage = importSHExpImage
     target.importRawExpImage = importRawExpImage
     target.importExpImageFromNPY = importExpImageFromNPY
 
     target.showMatchingIndexMap = showMatchingIndexMap
-    
+
+    # Annular Dark Field
+    target.generateADF = generateADF
 
     return target
```

### Comparing `pyemaps-1.0.6/emcontrols.py` & `pyemaps-1.0.7/emcontrols.py`

 * *Files 1% similar despite different names*

```diff
@@ -929,8 +929,23 @@
 
         if len(simstr) == 0 and len(cstr) != 0:
             return cstr
 
         if len(simstr) != 0 and len(cstr) == 0:
             return simstr
 
-        return ';'.join(emcstrs)
+        return ';'.join(emcstrs)
+    
+    @staticmethod
+    def def_dict(): 
+        retdict={}
+        for k in DEF_EMC:
+
+            if k == 'simc':
+                for sk, sv in DEF_SIMC.items():
+                    retdict[sk] = sv
+                continue
+
+            retdict[k] = DEF_EMC[k]['defval']
+
+
+        return retdict
```

### Comparing `pyemaps-1.0.6/errors.py` & `pyemaps-1.0.7/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,7 +242,16 @@
     Crystal construction simulation errors.
     
     '''
     def __init__(self, message=''):
         self.message = str(f'Error generating mxtal: {message}')
         super().__init__(self.message)
 
+
+class XDPImageError(Exception):
+    '''
+    Experimental diffraction pattern image object errors.
+    
+    '''
+    def __init__(self, message=''):
+        self.message = str(f'{message}')
+        super().__init__(self.message)
```

### Comparing `pyemaps-1.0.6/fileutils.py` & `pyemaps-1.0.7/fileutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 def find_pyemaps_datahome(home_type='crystals'):
     '''
     Detects enviroment variable set by PYEMAPS_DATA and return the
     diretcory set by the variable or return current working directory.
     
     :param home_type: Type of home directory
     :type home_type: string, optional
+    
     :return: data home path.
     :rtype: string
 
     Folder names depending by *home_type* input:
 
     1. **crystals**: all crystal data files.
     2. **bloch**: all dynamic simulation output files.
```

### Comparing `pyemaps-1.0.6/kdiffs.py` & `pyemaps-1.0.7/kdiffs.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # along with pyemaps.  If not, see <https://www.gnu.org/licenses/>.
 
 # Contact supprort@emlabsoftware.com for any questions and comments.
 # 
 # Author:     EMLab Solutions, Inc.
 # Date:       May 07, 2022    
 # '''
+
 '''
 Kinematic diffraction module is designed to handle kinematic simulation
 data. It is composed of Point, Line and Disk class objects.
 
 '''
 from . import EMC, SIMC
 from . import DPError, PointError, LineError, PIndexError, \
@@ -38,40 +39,51 @@
 from . import XMAX, YMAX
 #int: Diffraction simulation output limits
 
 DEF_MODE = 1 
 #int: Default diffraction simulation mode, normal
 
 def _double_eq(a,b):
+
     '''
+
     For internal testing only
+
     '''
     return abs(a-b) <= DIFF_PRECISION
 
 class Point:
+
     '''
+
     Coordinates of kinematic diffraction pattern object.
     
     '''
     def __init__(self, p=(0.0, 0.0)):
 
         setattr(self, 'x', p[0])
         setattr(self, 'y', p[1])
 
     @property
     def x(self):
+
         '''
+
         X coordinate
+
         '''
         return self._x
     
     @property
     def y(self):
+
         '''
+
         Y coordinate
+
         '''
         return self._y
 
     @x.setter
     def x(self, v):
         
         try:
@@ -147,51 +159,60 @@
     def __repr__(self):
         return str("({}, {})".format(self._x, self._y))
 
     def __iter__(self):
         return iter((self._x, self._y))
 
 class Line:
+
     '''
+
     Kikuchi line representation in kinematic diffraction patterns.
     
     '''
     def __init__(self, pt1 = Point(), pt2=Point(), intensity=0, type=1):
         
         setattr(self, 'pt1', pt1)  
         setattr(self, 'pt2', pt2)    
         setattr(self, 'intensity', intensity)    
         setattr(self, 'type', type)
 
     @property
     def pt1(self):
+
         '''
+
         The first end point of a Line
 
         '''
         return self._pt1
 
     @property
     def pt2(self):
+
         '''
+
         The second end point of a Line
 
         '''
         return self._pt2
     
     @property
     def type(self):
+
         '''
+
         The type of a Line: Kikuchi line or HOLZ line
 
         '''
         return self._type
     
     @property
     def intensity(self):
+
         '''
         Line intensity
 
         '''
         return self._intensity
 
     @pt1.setter
@@ -250,30 +271,35 @@
     def __key__(self):
         return (self._pt1, self._pt2, self._intensity)
     
     def __hash__(self):
         return hash(self.__key__())
     
     def __isub__(self, other):
+
         '''
+
         This operator override is for shifting the line by fixed amount 
         by 2D vector
 
         '''
         if isinstance(other, Point):
             self._pt1 -= other
             self._pt2 -= other
             return self
         
         raise LineError("substraction of Line class from non-Point class type not supported")
     
     def __iadd__(self, other):
+
         '''
+
         This operator override is for shifting the line by fixed amount when
         other line object has the same pt1 and ot2
+
         '''
         if isinstance(other, Point):
             self._pt1 += other
             self._pt2 += other
             return self
         
         raise LineError("addition of different type not supported")
@@ -310,15 +336,17 @@
 
     def __iter__(self):
         x1, y1 = self._pt1
         x2, y2 = self._pt2
         return iter((x1,y1,x2,y2,self._intensity))
 
     def calOpacity(self, l, h):
+
         """
+    
         Calculate the line opacity based on its intensity value
 
         0.2 -> lowest intensity
         0.35-> highest intensity
 
         """
         if h==l:
@@ -345,43 +373,50 @@
         x1, y1 = self._pt1
         x2, y2 = self._pt2
         return {'pt1': (x1,y1),
                 'pt2': (x2,y2), 
                 'int': self._intensity}
 
 class Index:
+
     '''
+    
     Miller Indexes of a diffracted beam representation in kinematic
     diffraction pattern.
 
     '''
     def __init__(self, I0=(0,0,0)):
 
         setattr(self, 'I1', I0[0])
         setattr(self, 'I2', I0[1])
         setattr(self, 'I3', I0[2])
 
     @property
     def I1(self):
+
         '''
+    
         The first element of Miller Index of a diffracted beam
 
         '''
         return self._I1
 
     @property
     def I2(self):
+
         '''
+        
         The second element of Miller Index of a diffracted beam
 
         '''
         return self._I2
 
     @property
     def I3(self):
+
         '''
         The third element of Miller Index of a diffracted beam
 
         '''
         return self._I3
         
     @I1.setter
@@ -443,43 +478,51 @@
 
         raise PIndexError('cannot compare with non-Index type')
     
     def __iter__(self):
         return iter((self._I1, self._I2, self._I3))
 
 class Disk:
+
     '''
+    
     Diffracted beams representation in kinematic diffraction patterns
 
     '''
     def __init__(self, c=Point(), r=0.0, i=Index()):
 
         setattr(self, 'c', c)
         setattr(self, 'r', r)
         setattr(self, 'idx', i)
 
     @property 
     def c(self):
+
         '''
+        
         The center point of a diffracted beam.
 
         '''
         return self._c
     
     @property
     def r(self):
+
         '''
+        
         The radius of a diffracted beam.
 
         '''
         return self._r
     
     @property
     def idx(self):
+
         '''
+        
         The Miller index of a diffracted beam.
 
         '''
         return self._idx
 
     @c.setter
     def c(self, cv):
@@ -515,28 +558,33 @@
 
         if not (self._c == other.c):
             return False
 
         return True
     
     def __iadd__(self, other):
+
         '''
+        
         This operator override is for shifting the line when
         other line object has the same pt1 and ot2
+        
         '''
         if isinstance(other, Point):
             self._c += other
             return self
         
         raise DiskError('addition cannot be done with non-Disk type')
     
     def __isub__(self, other):
         '''
+        
         This operator override is for shifting the line when
         other line object has the same pt1 and ot2
+        
         '''
         if isinstance(other, Point):
             self._c -= other
             return self
         
         raise DiskError('substraction cannot be done with non-Point type')
     
@@ -562,15 +610,17 @@
     def __repr__(self):
           
         return "index: " + repr(self._idx) + " " + \
                "center: " + repr(self._c) + " " + \
                str("radius: {}".format(self._r))
 
     def to_dict(self):
+
         '''
+        
         Creates a diffracted beam object from a dict pyton object
 
         '''
         dd = {}  
         dd['c'] = self._c.__key__()
         dd['idx'] = self._idx.__key__()
         dd['r'] = self._r
@@ -593,24 +643,28 @@
 
     def __iter__(self):
         cx, cy = self._c
         i1, i2, i3 = self._idx
         return iter((cx, cy, self._r, i1, i2, i3))
 
 class diffPattern:
+
     '''
+    
     Create a kinematic diffraction pattern based on the pyemaps
     kinematic simulation output in python dict object.
 
     See :doc:Visualization for how to visualize 
     kinematic diffraction patterns using this object.
 
     '''
     def __init__(self, diff_dict):
+
         '''
+
         :param diff_dict: Only accepts output from pyemaps kinematic diffraction run.
         :type diff_dict: dict, required
 
         '''
         if not diff_dict or not isinstance(diff_dict, dict):
             raise DPError("failed to construct diffraction pattern object")
 
@@ -643,50 +697,90 @@
             elif k == 'nums':
                 
                 for k1, v1 in v.items():
                     setattr(self, k1, v1)
 
     @property
     def klines(self):
-        ''' Kikuchi lines array '''
+
+        ''' 
+        
+        Kikuchi lines array 
+        
+        '''
         return self._klines
 
     @property
     def hlines(self):
-        ''' Holz lines array '''
+
+        ''' 
+        
+        Holz lines array 
+        
+        '''
         return self._hlines
 
     @property
     def disks(self):
-        ''' Disks array '''
+
+        ''' 
+        
+        Disks array 
+        
+        '''
         return self._disks
 
     @property
     def nklines(self):
-        ''' Number of Kikuchi lines '''
+
+        ''' 
+        
+        Number of Kikuchi lines 
+        
+        '''
         return self._nklines
 
     @property
     def nhlines(self):
-        ''' Number of HOLZ lines '''
+
+        ''' 
+        
+        Number of HOLZ lines 
+        
+        '''
         return self._nhlines
 
     @property
     def ndisks(self):
-        ''' Number of Disks '''
+
+        ''' 
+        
+        Number of Disks 
+        
+        '''
         return self._ndisks
 
     @property
     def shift(self):
-        ''' Shifts of the diffraction pattern '''
+
+        ''' 
+        
+        Shifts of the diffraction pattern 
+        
+        '''
         return self._shift
 
     @property
     def name(self):
-        ''' Crystal name '''
+
+        ''' 
+        
+        Crystal name 
+        
+        '''
         return self._name
 
     @klines.setter
     def klines(self, kls):
         
         if not hasattr(kls, "__len__"):
             raise DPError("klines data invalid")
@@ -870,15 +964,20 @@
         sDiff.append(str(f'\n# of HOLZ lines (hline): {self._nhlines}'))
         for i, h in enumerate(self._hlines):
             sDiff.append(str("hline# {}:".format(i+1)).ljust(10) + repr(h))
         
         return "\n".join(sDiff)
 
     def _difference(self, other):
-        '''Internal testing use only'''
+
+        '''
+        
+        Internal testing use only
+        
+        '''
         # A - B (self - other)
         if not isinstance(other, diffPattern):
             raise DPError("DP object does not compare with objects of DP types")
         
         kdiff = []
         for sk in self._klines:
             if not (sk in other):
@@ -901,15 +1000,17 @@
         
         retdict['klines'] = [kl.to_dict() for kl in self._klines]
         retdict['hlines'] = [hl.to_dict() for hl in self._hlines]
         retdict['disks'] = [d.to_dict() for d in self._disks]
         return retdict
 
 class Diffraction:
+
     '''
+
     List of DP objects and its associated EMControl objects.
 
     '''
     def __init__(self, name, mode=DEF_MODE):
         
         setattr(self, 'name', name)
         setattr(self, 'mode', mode)
@@ -952,30 +1053,43 @@
                not isinstance(emc, EMC):
                 raise DPListError('invalid data found in DP list')
 
         self._diffList = dpl
 
     # Adding new diffraction patterns
     def add(self, emc, diffP):
+
         '''
+        
         Append a new kenematic diffraction pattern with its associated 
         controls
+        
         '''
         if not isinstance(diffP, diffPattern):
             raise DPListError('failed to add DP')
 
 
         self.diffList.append((emc, diffP))
     
     def sort(self):
-        ''' Sorting diffraction list by controls'''
+
+        ''' 
+        
+        Sorting diffraction list by controls
+        
+        '''
         self._diffList.sort(key=lambda x: x[0])
             
     def __eq__(self, other):
-        '''Test if two diffraction list is the same'''
+
+        '''
+        
+        Test if two diffraction list is the same
+        
+        '''
         if not isinstance(other, Diffraction):
             return False
         
         if self._name != other.name or self._mode != other.mode:
             return False
 
         if len(self._diffList) != len(other.diffList):
@@ -994,28 +1108,37 @@
                 continue
             else:
                 break
         
         return found
             
     def __getitem__(self, key):
+
         '''
+        
         Array like method for retrieving DP
+        
         '''
         return self._diffList[key]
             
     def clear(self):
+
         '''
+
         Empty the DP list, leaving it as empty.
-        New diffraction patterns can be started
+
         '''
         self._diffList.clear()
 
     def _report_difference(self, other):
-        """ internal testing call"""
+        """ 
+        
+        internal testing call
+        
+        """
         if not isinstance(other, Diffraction):
             raise DPListError('connt report difference between two different type of objects')
         
         rep = []
         if self == other:
             return rep
```

### Comparing `pyemaps-1.0.6/license.txt` & `pyemaps-1.0.7/license.txt`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/pyemaps.egg-info/PKG-INFO` & `pyemaps-1.0.7/pyemaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.6
+Version: 1.0.7
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyemaps-1.0.6/pyemaps.egg-info/SOURCES.txt` & `pyemaps-1.0.7/pyemaps.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 errors.py
 fileutils.py
 kdiffs.py
 license.txt
 pyproject.toml
 setup.cfg
 setup.py
+stackimg.py
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/CifFile/src/lib/lex.yy.c
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/CifFile/src/lib/py_star_scan.c
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/CifFile/src/lib/star_scanner.h
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/ediom/DPIndex.cpp
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/ediom/DPIndex.h
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/ediom/EmlabLib.h
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/ediom/EmlabPars.h
@@ -138,25 +139,25 @@
 ediom/ediom.py
 ediom/ediom_dec.py
 pyemaps.egg-info/PKG-INFO
 pyemaps.egg-info/SOURCES.txt
 pyemaps.egg-info/dependency_links.txt
 pyemaps.egg-info/requires.txt
 pyemaps.egg-info/top_level.txt
+samples/adf.py
 samples/al.img
 samples/al_db.bin
 samples/al_dpgen.py
 samples/al_ediom.py
 samples/powder.py
 samples/si_bloch.py
 samples/si_constructor.py
 samples/si_csf.py
 samples/si_dif.py
 samples/si_lacbed.py
 samples/si_pyemaps.py
-samples/si_rawblochimgs.py
 samples/si_scm.py
 samples/si_stereo.py
 scattering/__init__.py
 scattering/sct_dec.py
 spg/__init__.py
 spg/spg_dec.py
```

### Comparing `pyemaps-1.0.6/samples/al.img` & `pyemaps-1.0.7/samples/al.img`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/al_db.bin` & `pyemaps-1.0.7/samples/al_db.bin`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/al_ediom.py` & `pyemaps-1.0.7/samples/al_ediom.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 def test_dp_indexing(cname = 'Aluminium'):
     '''
     Searches and indexes imported diffraction pattern images
     by theoretical diffraction patterns generated by pyemaps.
     '''
     from pyemaps import Crystal as cr
+    from pyemaps import StackImage, XDPImageError
    
     cryst = cr.from_builtin(cname)
 
     # ------------load existing DP database from file-----------------
     # dbfn = getDBFile()
 
     # or 
@@ -71,49 +72,52 @@
     res = 200
     ret, dbfn = cryst.generateDPDB(emc=EMC(zone=(0,0,1)), res = res, xa = xa0)
 
     if ret != 0:
         print(f'failed to generate a diffraction patterns databaes')
         return -1
 
-    ret, mr, mc =cryst.loadDPDB(dbfn = dbfn, bShowDBMap=True)
+    # ret, mr, mc =cryst.loadDPDB(dbfn = dbfn, bShowDBMap=True)
     
-    if ret != 0 or mr <= 0 or mc <=0:
-        print(f"Error loading DP database from file {dbfn} into ediom module")
-        cryst.release_ediom()
-        exit(1)
+    # if ret != 0 or mr <= 0 or mc <=0:
+    #     print(f"Error loading DP database from file {dbfn} into ediom module")
+    #     cryst.release_ediom()
+    #     exit(1)
 
     xifn = getDPImageFn()
+    alimg = StackImage(xifn)
     try:
-       cryst.importSHExpImage(xifn, bShow=True)
-    except Exception as e:
-        cryst.release_ediom()
-        raise ValueError from e
-
+      
     # DPs or peaks search and indexing parameters 
-    # See pyemaps documents for explanation of the parameters below
-    cryst.indexExpDP(cc                 = 29.0,                 
-                     sigma              = 3.0,                  
-                     img_center         = (99.923, 99.919),     
-                     rmin               = 10,                   
-                     search_box         = 10.0,
-                     scaling_option     = (1,2), 
-                     filter_threshold   = 0.0,
-                     peak_threshold     = 0.8)
+    # See pyemaps documents for explanation of the parameters
+        alimg.indexImage(dbfn,
+                        cc                 = 29.0,                 # Camera constant
+                        sigma              = 3.0,                  # Peak width measurement
+                        img_center         = (99.923, 99.919),     # Image or DP image center location
+                        rmin               = 10,                   
+                        search_box         = 10.0,
+                        scaling_option     = (1,2), 
+                        filter_threshold   = 0.0,
+                        peak_threshold     = 0.8)
+        
+    except XDPImageError as e:
+        print(f'Error indexing image {e.message}')
+        return
+
     
     # display diffractiom pattern in the database that best match the image pattern
-    cryst.showMatchedDBDP()
+    StackImage.showMatchedDBDP()
 
     # show stereo projection location that corresponds to the matched diffraction pattern
-    cryst.showMatchingIndexMap(mr, mc)
+    # StackImage.showMatchingIndexMap(mr, mc)
 
     # print match diffraction details
-    cryst.printDPIndexDetails()
+    # StackImage.printDPIndexDetails()
 
     # release ediom module memory.
-    cryst.release_ediom()
+    # StackImage.release_ediom()
 
 
 if __name__ == '__main__':
     
     test_dp_indexing()
```

### Comparing `pyemaps-1.0.6/samples/powder.py` & `pyemaps-1.0.7/samples/powder.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_bloch.py` & `pyemaps-1.0.7/samples/si_bloch.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_constructor.py` & `pyemaps-1.0.7/samples/si_constructor.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_csf.py` & `pyemaps-1.0.7/samples/si_csf.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_dif.py` & `pyemaps-1.0.7/samples/si_dif.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_lacbed.py` & `pyemaps-1.0.7/samples/si_lacbed.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_pyemaps.py` & `pyemaps-1.0.7/samples/si_pyemaps.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_rawblochimgs.py` & `pyemaps-1.0.7/samples/adf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 """
 This file is part of pyemaps
 ___________________________
 
 pyemaps is free software for non-comercial use: you can 
 redistribute it and/or modify it under the terms of the GNU General 
 Public License as published by the Free Software Foundation, either 
@@ -14,34 +16,58 @@
 
 You should have received a copy of the GNU General Public License
 along with pyemaps.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact supprort@emlabsoftware.com for any questions and comments.
 ___________________________
 
-An example of using pyemaps crystal and diffraction modules to 
-1) create a crystal from built-in data for Silicon 
-2) generate kinematical diffraction patterns
-3) display the diffraction pattern using pyemaps's built-in plot function 
-
-See https://emlab-solutions.github.io/pyemaps/ for pemaps usage
-
 Author:     EMLab Solutions, Inc.
-Date:       May 07, 2022    
+Date:       May 27, 2023  
+
+This sample code is to demostrate basic usage of pyemaps' ediom
+module (Electron Diffraction Indexing and Orientation Mapping)
+to obtain anular dark field image from an experimental diffraction 
+image input.
+
+This script is for demonstration and only available in full pyemaps
+package. 
+
+Contact:
+    support@emlabsoftware.com 
+for price information.
 
 """
+import os
+from pathlib import Path
+from pyemaps import StackImage, EM_INT
+
+current_file = Path(os.path.abspath(__file__))
+samples_path = current_file.parent.absolute()
+
+def getADFFn():
+    '''
+    Imports sample experimental diffraction pattern image
+    with preprietory 8-bytes header. 
+    '''
+    return os.path.join(samples_path, 'adftest30x30.im3')
+
+def test_adf():
+    '''
+    Searches and indexes imported diffraction pattern images
+    by theoretical diffraction patterns generated by pyemaps.
+    '''
+    
+    adfn = getADFFn()
+    img = StackImage(adfn,ndtype = EM_INT)
+    # adfimgfn = getADFFn()
+    img.generateADF(center = (256.0, 256.0), 
+                    rads = (50.0,200.0), 
+                    scol = 30,
+                    bShow = True)
+
+    # # release ediom module memory.
+    # release_ediom()
+
 if __name__ == '__main__':
     
-    from pyemaps import Crystal as cr
-    from pyemaps import CrystalClassError
-    from pyemaps import BlochError
-    try:
-        si = cr.from_builtin('Silicon')
-
-        bimgs = si.generateBloch(sample_thickness=(200, 1000, 100), bSave=True)
-
-    except (CrystalClassError, BlochError) as e:
-        print(f'error: generate and write bloch image data1: {e.message}')
-    except Exception as e:
-        print(f'error: generate and write bloch image data2: ' + str(e))
-   
-   
+    test_adf()
+
```

### Comparing `pyemaps-1.0.6/samples/si_scm.py` & `pyemaps-1.0.7/samples/si_scm.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/samples/si_stereo.py` & `pyemaps-1.0.7/samples/si_stereo.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/scattering/__init__.py` & `pyemaps-1.0.7/scattering/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 # Contact supprort@emlabsoftware.com for any questions and comments.
 # ___________________________
 # '''
 
 # root directory for all emaps modules
-from .scattering import sct
+from .scattering import sct
```

### Comparing `pyemaps-1.0.6/setup.cfg` & `pyemaps-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/setup.py` & `pyemaps-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,18 +113,18 @@
 install_requires_common = [
             'numpy >= 1.21.2',
             'matplotlib >= 3.2.1',
             ]
 
 dif_source = [
             'diff_types.f90', 
+            'diff_memalloc.f90',
             'diffract.f90',
             'scattering.f90', 
             'spgra.f90',
-            'diff_memalloc.f90',
             'crystal_mem.f90', 
             'emaps_consts.f90',
             'xtal0.f90', 
             'helper.f90', 
             'asf.f90', 
             'atom.f',
             'metric.f', 
@@ -540,16 +540,17 @@
             sources                 =get_ediom_sources(),
             extra_objects           =[],
             include_dirs            =get_ediom_includes(),
             library_dirs            =get_ediom_libs(),
             libraries               =[],
             define_macros           = pyemaps_build_defs,
             undef_macros            = pyemaps_build_undefs,
-            extra_link_args         =[],
-            swig_opts               =['-python']
+            extra_link_args         =[] 
+            
+            # swig_opts               =['-python']
 )
 
 def get_version(f):
     version = {}
     with open(f + ".py") as fp:
         exec(fp.read(), version)
     
@@ -574,14 +575,15 @@
       py_modules                        = ['pyemaps.crystals',
                                            'pyemaps.kdiffs',
                                            'pyemaps.ddiffs',
                                            'pyemaps.display',
                                            'pyemaps.errors',
                                            'pyemaps.fileutils',
                                            'pyemaps.emcontrols',
+                                           'pyemaps.stackimg',
                                            'pyemaps.CifFile.CifFile_module',
                                            'pyemaps.CifFile.yapps3_compiled_rt',
                                            'pyemaps.CifFile.YappsStarParser_1_1',
                                            'pyemaps.CifFile.YappsStarParser_1_0',
                                            'pyemaps.CifFile.YappsStarParser_STAR2',
                                            'pyemaps.CifFile.YappsStarParser_2_0',
                                            'pyemaps.CifFile.StarFile',
```

### Comparing `pyemaps-1.0.6/spg/__init__.py` & `pyemaps-1.0.7/spg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.6/spg/spg_dec.py` & `pyemaps-1.0.7/spg/spg_dec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from . import spgseek as spgra
 
 SPG_SYMMETRY_MAXCOL = spgra.getsymmetrymaxlen() #48
 
 SPG_SETTING_MAX = spgra.getspgallsettingmax() #6
 
 SPG_SYMMETRY_MAXLEN = spgra.getsymmetryitemlen() #20
```

