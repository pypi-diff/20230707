# Comparing `tmp/partitura-1.3.0.tar.gz` & `tmp/partitura-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partitura-1.3.0.tar", last modified: Sat Jun 10 09:51:19 2023, max compression
+gzip compressed data, was "partitura-1.3.1.tar", last modified: Fri Jul  7 09:31:50 2023, max compression
```

## Comparing `partitura-1.3.0.tar` & `partitura-1.3.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.524998 partitura-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-10 09:51:11.000000 partitura-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-10 09:51:19.524998 partitura-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-10 09:51:11.000000 partitura-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.512998 partitura-1.3.0/partitura/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.516998 partitura-1.3.0/partitura/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   335762 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/musicxml.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.krn
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.mei
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.mid
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.musicxml
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/directions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.516998 partitura-1.3.0/partitura/io/
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportaudio.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    71850 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmei.py
--rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    35404 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmusicxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportparangonada.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importkern.py
--rw-r--r--   0 runner    (1001) docker     (123)    26363 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    42676 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmei.py
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmidi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmusic21.py
--rw-r--r--   0 runner    (1001) docker     (123)    56313 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmusicxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importnakamura.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importparangonada.py
--rw-r--r--   0 runner    (1001) docker     (123)    31691 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchfile_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchlines_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchlines_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/musescore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.520998 partitura-1.3.0/partitura/musicanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/key_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/note_array_to_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    38131 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/note_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/performance_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/performance_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/pitch_spelling.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/tonal_tension.py
--rw-r--r--   0 runner    (1001) docker     (123)    35763 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/voice_separation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)   152462 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.520998 partitura-1.3.0/partitura/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)   110587 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/music.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/synth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.512998 partitura-1.3.0/partitura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:51:19.524998 partitura-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-10 09:51:11.000000 partitura-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.524998 partitura-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_kern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_key_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_load_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_load_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_m21_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_match_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    74764 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_match_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_mei.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_merge_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_metrical_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_midi_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_midi_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_nakamura.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_new_divs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_note_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_note_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_octave_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_parangonada.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_part_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_partial_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_performance_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_performance_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_pianoroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_pitch_spelling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_quarter_adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_rest_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_time_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_tonal_tension.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_voice_estimation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10316 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.152798 partitura-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-07-07 09:31:40.000000 partitura-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-07 09:31:50.152798 partitura-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-07 09:31:40.000000 partitura-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.140798 partitura-1.3.1/partitura/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.140798 partitura-1.3.1/partitura/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   335762 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/assets/musicxml.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/assets/score_example.krn
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/assets/score_example.mei
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/assets/score_example.mid
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/assets/score_example.musicxml
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/directions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.144798 partitura-1.3.1/partitura/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/exportaudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/exportmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71850 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/exportmei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/exportmidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35318 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/exportmusicxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/exportparangonada.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importkern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42685 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importmei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importmidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importmusic21.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56230 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importmusicxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importnakamura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/importparangonada.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/matchfile_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25882 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/matchfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29228 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/matchlines_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40242 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/matchlines_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/io/musescore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.148798 partitura-1.3.1/partitura/musicanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/key_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21781 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/note_array_to_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37809 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/note_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34663 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/performance_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/performance_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/pitch_spelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/tonal_tension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35740 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/musicanalysis/voice_separation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152494 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.148798 partitura-1.3.1/partitura/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110930 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/utils/music.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/utils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-07-07 09:31:40.000000 partitura-1.3.1/partitura/utils/synth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.140798 partitura-1.3.1/partitura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-07 09:31:50.000000 partitura-1.3.1/partitura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-07 09:31:50.000000 partitura-1.3.1/partitura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:31:50.000000 partitura-1.3.1/partitura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 09:31:50.000000 partitura-1.3.1/partitura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:31:50.000000 partitura-1.3.1/partitura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:31:50.152798 partitura-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-07 09:31:40.000000 partitura-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:31:50.152798 partitura-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_kern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_key_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_load_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_load_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_m21_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_match_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74764 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_match_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_mei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_merge_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_metrical_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_midi_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_midi_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_nakamura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_new_divs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_note_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_note_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_octave_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_parangonada.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_part_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_partial_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_performance_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_performance_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_pianoroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_pitch_spelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_quarter_adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_rest_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_time_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_tonal_tension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_voice_estimation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10316 2023-07-07 09:31:40.000000 partitura-1.3.1/tests/test_xml.py
```

### Comparing `partitura-1.3.0/LICENSE` & `partitura-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/PKG-INFO` & `partitura-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partitura
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package for handling symbolic musical information
 Home-page: https://github.com/CPJKU/partitura
 Author: Maarten Grachten, Carlos Cancino-Chacón, Silvan Peter, Emmanouil Karystinaios, Francesco Foscarin, Thassilo Gadermaier
 Author-email: partitura-users@googlegroups.com
 License: Apache 2.0
 Keywords: music notation musicxml midi
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `partitura-1.3.0/README.md` & `partitura-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/__init__.py` & `partitura-1.3.1/partitura/__init__.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/assets/musicxml.xsd` & `partitura-1.3.1/partitura/assets/musicxml.xsd`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/assets/score_example.mei` & `partitura-1.3.1/partitura/assets/score_example.mei`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/assets/score_example.musicxml` & `partitura-1.3.1/partitura/assets/score_example.musicxml`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/directions.py` & `partitura-1.3.1/partitura/directions.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/display.py` & `partitura-1.3.1/partitura/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         return None
 
     prvw_sfx = ".preview.{}".format(fmt)
 
     with TemporaryFile() as xml_fh, NamedTemporaryFile(
         suffix=prvw_sfx, delete=False
     ) as img_fh:
-
         # save part to musicxml in file handle xml_fh
         save_musicxml(score_data, xml_fh)
         # rewind read pointer of file handle before we pass it to musicxml2ly
         xml_fh.seek(0)
 
         img_stem = img_fh.name[: -len(prvw_sfx)]
```

### Comparing `partitura-1.3.0/partitura/io/__init__.py` & `partitura-1.3.1/partitura/io/__init__.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/io/exportaudio.py` & `partitura-1.3.1/partitura/io/exportaudio.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/io/exportmatch.py` & `partitura-1.3.1/partitura/io/exportmatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,15 @@
 
 from partitura.utils.misc import (
     PathLike,
     deprecated_alias,
     deprecated_parameter,
 )
 
-from partitura.musicanalysis.performance_codec import (
-    get_time_maps_from_alignment
-)
+from partitura.musicanalysis.performance_codec import get_time_maps_from_alignment
 
 __all__ = ["save_match"]
 
 
 @deprecated_parameter("magaloff_zeilinger_quirk")
 def matchfile_from_alignment(
     alignment: List[dict],
@@ -203,19 +201,17 @@
     scoreprop_lines = defaultdict(list)
 
     # For score notes
     score_info = dict()
     # Info for sorting lines
     snote_sort_info = dict()
     for (mnum, msd, msb), m in zip(measure_starts, measures):
-
         time_signatures = spart.iter_all(score.TimeSignature, m.start, m.end)
 
         for tsig in time_signatures:
-
             time_divs = int(tsig.start.t)
             time_beats = float(beat_map(time_divs))
             dpq = int(spart.quarter_duration_map(time_divs))
             beat = int((time_beats - msb) // 1)
 
             ts_num, ts_den, _ = spart.time_signature_map(tsig.start.t)
 
@@ -278,15 +274,14 @@
             )
 
         # Get all notes in the measure
         snotes = spart.iter_all(score.Note, m.start, m.end, include_subclasses=True)
         # Beginning of each measure
 
         for snote in snotes:
-
             onset_divs, offset_divs = snote.start.t, snote.start.t + snote.duration_tied
             duration_divs = offset_divs - onset_divs
 
             onset_beats, offset_beats = beat_map([onset_divs, offset_divs])
 
             dpq = int(spart.quarter_duration_map(onset_divs))
 
@@ -374,15 +369,14 @@
             float(ptime_to_stime_map(pnote["note_on"])),
             pnote["midi_pitch"],
         )
 
     sort_stime = []
     note_lines = []
     for al_note in alignment:
-
         label = al_note["label"]
 
         if label == "match":
             snote = score_info[al_note["score_id"]]
             pnote = perf_info[al_note["performance_id"]]
             snote_note_line = MatchSnoteNote(version=version, snote=snote, note=pnote)
             note_lines.append(snote_note_line)
```

### Comparing `partitura-1.3.0/partitura/io/exportmei.py` & `partitura-1.3.1/partitura/io/exportmei.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/io/exportmidi.py` & `partitura-1.3.1/partitura/io/exportmidi.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 def map_to_track_channel(note_keys, mode):
     ch_helper = {}
     tr_helper = {}
     track = {}
     channel = {}
-    for (pg, p, v) in note_keys:
+    for pg, p, v in note_keys:
         if mode == 0:
             trk = tr_helper.setdefault(p, len(tr_helper))
             ch1 = ch_helper.setdefault(p, {})
             ch2 = ch1.setdefault(v, len(ch1) + 1)
             track[(pg, p, v)] = trk
             channel[(pg, p, v)] = ch2
         elif mode == 1:
@@ -283,17 +283,17 @@
         note starts at 0). If "pad_bar", the "incomplete" bar  of
         the anacrusis is padded with silence. Defaults to 'shift'.
         If "time_sig_change", the time signature is changed to match
         the duration of the measure. This also ensure the beat and
         downbeats position are coherent in case of incomplete measures
         later in the score.
     minimum_ppq : int, optional
-        Minimum ppq to use for the MIDI file. If the ppq of the score is less, 
+        Minimum ppq to use for the MIDI file. If the ppq of the score is less,
         it will be doubled until it is above the threshold. This is useful
-        because some libraries like miditok require a certain minimum ppq to 
+        because some libraries like miditok require a certain minimum ppq to
         work properly.
 
     Returns
     -------
     None or MidiFile
         If no output is specified using `out`, the function returns
         a `MidiFile` object. Otherwise, the function returns None.
@@ -311,15 +311,15 @@
             "`score_data` should be a `Score`, a `Part`, a `PartGroup"
             f" or a list of  `Part` instances but is {type(score_data)}"
         )
     ppq = get_ppq(parts)
     # double it until it is above the minimum level.
     # Doubling instead of setting it ensure that the common divisors stay the same.
     while ppq < minimum_ppq:
-        ppq = ppq*2
+        ppq = ppq * 2
 
     events = defaultdict(lambda: defaultdict(list))
     meta_events = defaultdict(lambda: defaultdict(list))
 
     event_keys = OrderedDict()
     tempos = {}
 
@@ -342,15 +342,14 @@
             ftp = -time_signatures[0][0] / (time_signatures[0][1] / 4)
         else:
             raise Exception(
                 'Invalid anacrusis_behavior value, must be one of ("shift", "pad_bar")'
             )
 
     for qm, part in zip(quarter_maps, score.iter_parts(parts)):
-
         pg = get_partgroup(part)
 
         notes = part.notes_tied
 
         def to_ppq(t):
             # convert div times to new ppq
             return int(ppq * (qm(t) - ftp))
@@ -363,72 +362,85 @@
         if anacrusis_behavior == "time_sig_change":
             # Change time signature to match the duration of the measure
             # This ensure the beat and downbeats position are coherent
             # in case of incomplete measures later in the score.
             all_ts = list(part.iter_all(score.TimeSignature))
             ts_changing_time = [ts.start.t for ts in all_ts]
             for measure in part.iter_all(score.Measure):
-                m_duration_beat = part.beat_map(measure.end.t) - part.beat_map(measure.start.t)
+                m_duration_beat = part.beat_map(measure.end.t) - part.beat_map(
+                    measure.start.t
+                )
                 m_ts = part.time_signature_map(measure.start.t)
                 if m_duration_beat != m_ts[0]:
                     # add ts change
                     # TODO: add support for changing the beat type if number of beats is not integer
                     meta_events[part][to_ppq(measure.start.t)].append(
                         MetaMessage(
-                            "time_signature", numerator=int(m_duration_beat), denominator=int(m_ts[1])
+                            "time_signature",
+                            numerator=int(m_duration_beat),
+                            denominator=int(m_ts[1]),
                         )
                     )
-                    ts_changing_time.append(measure.start.t) # keep track of changing the ts
+                    ts_changing_time.append(
+                        measure.start.t
+                    )  # keep track of changing the ts
                     # now go back to original ts if there is no ts change after this measure
                     if not any([ts_t > measure.start.t for ts_t in ts_changing_time]):
                         meta_events[part][to_ppq(measure.end.t)].append(
                             MetaMessage(
-                                "time_signature", numerator=int(m_ts[0]), denominator=int(m_ts[1])
+                                "time_signature",
+                                numerator=int(m_ts[0]),
+                                denominator=int(m_ts[1]),
                             )
                         )
             # filter out the multiple ts changes at the same time
             # this happens when multiple measure in a row have wrong duration
             for t in meta_events[part].keys():
                 if len(meta_events[part][t]) == 2:
                     meta_events[part][t] = meta_events[part][t][1:]
 
             # now add the normal time signature change
             for ts in part.iter_all(score.TimeSignature):
                 if ts.start.t in ts_changing_time:
-                #don't add if something is already added at this time to cover the case of a ts change when the first measure is shorter/longer
+                    # don't add if something is already added at this time to cover the case of a ts change when the first measure is shorter/longer
                     pass
                 else:
                     meta_events[part][to_ppq(ts.start.t)].append(
                         MetaMessage(
-                            "time_signature", numerator=ts.beats, denominator=ts.beat_type
+                            "time_signature",
+                            numerator=ts.beats,
+                            denominator=ts.beat_type,
                         )
                     )
-        else: # just add the time signature that are explicit in partitura
+        else:  # just add the time signature that are explicit in partitura
             for i, ts in enumerate(part.iter_all(score.TimeSignature)):
                 if anacrusis_behavior == "pad_bar" and i == 0:
                     # shift the first time signature to 0 so MIDI players can pick up the correct measure position
                     meta_events[part][0].append(
                         MetaMessage(
-                        "time_signature", numerator=ts.beats, denominator=ts.beat_type
+                            "time_signature",
+                            numerator=ts.beats,
+                            denominator=ts.beat_type,
                         )
-                    )   
-                else: #follow the position in the partitura part
+                    )
+                else:  # follow the position in the partitura part
                     meta_events[part][to_ppq(ts.start.t)].append(
                         MetaMessage(
-                            "time_signature", numerator=ts.beats, denominator=ts.beat_type
+                            "time_signature",
+                            numerator=ts.beats,
+                            denominator=ts.beat_type,
                         )
                     )
 
         for ks in part.iter_all(score.KeySignature):
             meta_events[part][to_ppq(ks.start.t)].append(
                 MetaMessage("key_signature", key=ks.name)
             )
 
         for note in notes:
-
             # key is a tuple (part_group, part, voice) that will be
             # converted into a (track, channel) pair.
             key = (pg, part, note.voice)
             events[key][to_ppq(note.start.t)].append(
                 Message("note_on", note=note.midi_pitch)
             )
             events[key][to_ppq(note.start.t + note.duration_tied)].append(
```

### Comparing `partitura-1.3.0/partitura/io/exportmusicxml.py` & `partitura-1.3.1/partitura/io/exportmusicxml.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,21 +39,19 @@
 
 
 def range_number_from_counter(e, label, counter):
     key = (label, e)
     number = counter.get(key, None)
 
     if number is None:
-
         number = 1 + sum(1 for o in counter.keys() if o[0] == label)
         assert number is not None
         counter[key] = number
 
     else:
-
         del counter[key]
 
     return number
 
 
 def filter_string(s):
     """
@@ -72,49 +70,42 @@
     # <voice>
     # <type>
     # <notations>
 
     note_e = etree.Element("note")
 
     if note.id is not None:
-
         note_id = note.id
         # make sure note_id is unique by appending _x to the note_id for the
         # x-th repetition of the id
         counter[note_id] = counter.get(note_id, 0) + 1
 
         if counter[note_id] > 1:
-
             note_id += "_{}".format(counter[note_id])
 
         note_e.attrib["id"] = filter_string(note_id)
 
     if isinstance(note, score.Note):
-
         if isinstance(note, score.GraceNote):
-
             if note.grace_type == "acciaccatura":
-
                 etree.SubElement(note_e, "grace", slash="yes")
 
             else:
-
                 etree.SubElement(note_e, "grace")
 
         pitch_e = etree.SubElement(note_e, "pitch")
 
         etree.SubElement(pitch_e, "step").text = "{}".format(note.step)
 
         if note.alter not in (None, 0):
             etree.SubElement(pitch_e, "alter").text = "{}".format(note.alter)
 
         etree.SubElement(pitch_e, "octave").text = "{}".format(note.octave)
 
     elif isinstance(note, score.UnpitchedNote):
-
         unpitch_e = etree.SubElement(note_e, "unpitched")
 
         etree.SubElement(unpitch_e, "display-step").text = "{}".format(note.step)
 
         etree.SubElement(unpitch_e, "display-octave").text = "{}".format(note.octave)
 
         if note.notehead is not None:
@@ -126,36 +117,31 @@
                 nh_e.attrib["filled"] = "no"
 
     elif isinstance(note, score.Rest):
         if not note.hidden:
             etree.SubElement(note_e, "rest")
 
     if not isinstance(note, score.GraceNote):
-
         duration_e = etree.SubElement(note_e, "duration")
         duration_e.text = "{:d}".format(int(dur))
 
     notations = []
 
     if note.tie_prev is not None:
-
         etree.SubElement(note_e, "tie", type="stop")
         notations.append(etree.Element("tied", type="stop"))
 
     if note.tie_next is not None:
-
         etree.SubElement(note_e, "tie", type="start")
         notations.append(etree.Element("tied", type="start"))
 
     if voice not in (None, 0):
-
         etree.SubElement(note_e, "voice").text = "{}".format(voice)
 
     if note.fermata is not None:
-
         notations.append(etree.Element("fermata"))
 
     if note.articulations:
         articulations = []
         for articulation in note.articulations:
             if articulation in ARTICULATIONS:
                 articulations.append(etree.Element(articulation))
@@ -163,19 +149,17 @@
             articulations_e = etree.Element("articulations")
             articulations_e.extend(articulations)
             notations.append(articulations_e)
 
     sym_dur = note.symbolic_duration or {}
 
     if sym_dur.get("type") is not None:
-
         etree.SubElement(note_e, "type").text = sym_dur["type"]
 
     for i in range(sym_dur.get("dots", 0)):
-
         etree.SubElement(note_e, "dot")
 
     if (
         sym_dur.get("actual_notes") is not None
         and sym_dur.get("normal_notes") is not None
     ):
         time_mod_e = etree.SubElement(note_e, "time-modification")
@@ -185,76 +169,67 @@
         normal_e.text = str(sym_dur["normal_notes"])
 
     if note.staff is not None:
         if note.staff != 1 or n_of_staves > 1:
             etree.SubElement(note_e, "staff").text = "{}".format(note.staff)
 
     for slur in note.slur_stops:
-
         number = range_number_from_counter(slur, "slur", counter)
 
         notations.append(etree.Element("slur", number="{}".format(number), type="stop"))
 
     for slur in note.slur_starts:
-
         number = range_number_from_counter(slur, "slur", counter)
 
         notations.append(
             etree.Element("slur", number="{}".format(number), type="start")
         )
 
     for tuplet in note.tuplet_stops:
         tuplet_key = ("tuplet", tuplet)
         number = counter.get(tuplet_key, None)
 
         if number is None:
-
             number = 1
             counter[tuplet_key] = number
 
         else:
-
             del counter[tuplet_key]
 
         notations.append(
             etree.Element("tuplet", number="{}".format(number), type="stop")
         )
 
     for tuplet in note.tuplet_starts:
         tuplet_key = ("tuplet", tuplet)
         number = counter.get(tuplet_key, None)
 
         if number is None:
-
             number = 1 + sum(1 for o in counter.keys() if o[0] == "tuplet")
             counter[tuplet_key] = number
 
         else:
-
             del counter[tuplet_key]
 
         notations.append(
             etree.Element("tuplet", number="{}".format(number), type="start")
         )
 
     if notations:
-
         notations_e = etree.SubElement(note_e, "notations")
         notations_e.extend(notations)
 
     return note_e
 
 
 def do_note(note, measure_end, part, voice, counter, n_of_staves):
     if isinstance(note, score.GraceNote):
-
         dur_divs = 0
 
     else:
-
         dur_divs = note.end.t - note.start.t
 
     note_e = make_note_el(note, dur_divs, voice, counter, n_of_staves)
 
     return (note.start.t, dur_divs, note_e)
 
 
@@ -326,65 +301,56 @@
     by_onset = defaultdict(list)
     for note in notes:
         if not isinstance(note, score.GraceNote):
             by_onset[note.start.t].append(note)
     onsets = sorted(by_onset.keys())
 
     for o in onsets:
-
         chord_dur = min(n.duration for n in by_onset[o])
 
         for n in by_onset[o]:
-
             if n.duration > chord_dur:
-
                 voice = find_free_voice(voice_spans, n.start.t, n.end.t)
                 voice_spans.append((n.start.t, n.end.t, voice))
                 extraneous[voice].append(n)
                 notes.remove(n)
 
     # now remove any notes that exceed next onset
     by_onset = defaultdict(list)
     for note in notes:
         by_onset[note.start.t].append(note)
     onsets = sorted(by_onset.keys())
 
     for o1, o2 in iter_current_next(onsets):
-
         for n in by_onset[o1]:
-
             if o1 + n.duration > o2:
-
                 voice = find_free_voice(voice_spans, n.start.t, n.end.t)
                 voice_spans.append((n.start.t, n.end.t, voice))
                 extraneous[voice].append(n)
                 notes.remove(n)
 
     return extraneous
 
 
 def find_free_voice(voice_spans, start, end):
     free_voice = min(voice for _, _, voice in voice_spans) + 1
 
     for vstart, vend, voice in voice_spans:
-
         if (end > vstart) and (start < vend):
-
             free_voice = max(free_voice, voice + 1)
 
     return free_voice
 
 
 def remove_voice_polyphony(notes_by_voice):
     voice_spans = [(-math.inf, math.inf, max(notes_by_voice.keys()))]
     extraneous = defaultdict(list)
     # n_orig = sum(len(nn) for nn in notes_by_voice.values())
 
     for voice, vnotes in notes_by_voice.items():
-
         v_extr = remove_voice_polyphony_single(vnotes, voice_spans)
 
         for new_voice, new_vnotes in v_extr.items():
             extraneous[new_voice].extend(new_vnotes)
 
     # n_1 = sum(len(nn) for nn in notes_by_voice.values())
     # n_2 = sum(len(nn) for nn in extraneous.values())
@@ -442,15 +408,14 @@
     #                               start=start, end=end,
     #                               include_subclasses=True)
     # notes_by_voice = partition(lambda n: n.voice or 0, notes)
 
     voices_e = defaultdict(list)
 
     for voice in sorted(notes_by_voice.keys()):
-
         voice_notes = notes_by_voice[voice]
         # sort by pitch
         voice_notes.sort(
             key=lambda n: n.midi_pitch if hasattr(n, "midi_pitch") else -1, reverse=True
         )
         # grace notes should precede other notes at the same onset
         voice_notes.sort(key=lambda n: not isinstance(n, score.GraceNote))
@@ -521,61 +486,48 @@
     repeat_start = part.iter_all(score.Repeat, start, end)
     repeat_end = part.iter_all(score.Repeat, start.next, end.next, mode="ending")
     ending_start = part.iter_all(score.Ending, start, end)
     ending_end = part.iter_all(score.Ending, start.next, end.next, mode="ending")
     by_onset = defaultdict(list)
 
     for obj in fermata:
-
         by_onset[obj.start.t].append(etree.Element("fermata"))
 
     for obj in repeat_start:
-
         if obj.start is not None:
-
             by_onset[obj.start.t].append(etree.Element("repeat", direction="forward"))
 
     for obj in ending_start:
-
         if obj.start is not None:
-
             by_onset[obj.start.t].append(
                 etree.Element("ending", type="start", number=str(obj.number))
             )
 
     for obj in repeat_end:
-
         if obj.end is not None:
-
             by_onset[obj.end.t].append(etree.Element("repeat", direction="backward"))
 
     for obj in ending_end:
-
         if obj.end is not None:
-
             by_onset[obj.end.t].append(
                 etree.Element("ending", type="stop", number=str(obj.number))
             )
 
     result = []
 
     for onset in sorted(by_onset.keys()):
-
         attrib = {}
 
         if onset == start.t:
-
             attrib["location"] = "left"
 
         elif onset == end.t:
-
             attrib["location"] = "right"
 
         else:
-
             attrib["location"] = "middle"
 
         barline_e = etree.Element("barline", **attrib)
 
         barline_e.extend(by_onset[onset])
         result.append((onset, None, barline_e))
 
@@ -600,41 +552,37 @@
 
 
 def forward_backup_if_needed(t, t_prev):
     result = []
     gap = 0
 
     if t > t_prev:
-
         gap = t - t_prev
         e = etree.Element("forward")
         ee = etree.SubElement(e, "duration")
         ee.text = "{:d}".format(int(gap))
         result.append((t_prev, gap, e))
 
     elif t < t_prev:
-
         gap = t_prev - t
         e = etree.Element("backup")
         ee = etree.SubElement(e, "duration")
         ee.text = "{:d}".format(int(gap))
         result.append((t_prev, -gap, e))
 
     return result, gap
 
 
 def merge_with_voice(notes, other, measure_start):
     by_onset = defaultdict(list)
 
     for onset, dur, el in notes:
-
         by_onset[onset].append((dur, el))
 
     for onset, dur, el in other:
-
         by_onset[onset].append((dur, el))
 
     result = []
     last_t = measure_start
     fb_cost = 0
     # order to insert simultaneously starting elements; it is important to put
     # notes last, since they update the position, and thus would lead to
@@ -647,24 +595,20 @@
         "sound": 4,
         "harmony": 5,
         "note": 6,
     }
     last_note_onset = measure_start
 
     for onset in sorted(by_onset.keys()):
-
         elems = by_onset[onset]
         elems.sort(key=lambda x: order.get(x[1].tag, len(order)))
 
         for dur, el in elems:
-
             if el.tag == "note":
-
                 if el.find("chord") is not None:
-
                     last_t = last_note_onset
 
                 last_note_onset = onset
 
             els, cost = forward_backup_if_needed(onset, last_t)
             fb_cost += cost
             result.extend(els)
@@ -691,37 +635,31 @@
         cost[0] = 0
 
     # get the voice for which merging notes and other has lowest cost
     merge_voice = sorted(cost.items(), key=itemgetter(1))[0][0]
     result = []
     pos = measure_start
     for i, voice in enumerate(sorted(notes.keys())):
-
         if voice == merge_voice:
-
             elements = merged[voice]
 
         else:
-
             elements = notes[voice]
 
         # backup/forward when switching voices if necessary
         if elements:
-
             gap = elements[0][0] - pos
 
             if gap < 0:
-
                 e = etree.Element("backup")
                 ee = etree.SubElement(e, "duration")
                 ee.text = "{:d}".format(-int(gap))
                 result.append(e)
 
             elif gap > 0:
-
                 e = etree.Element("forward")
                 ee = etree.SubElement(e, "duration")
                 ee.text = "{:d}".format(gap)
                 result.append(e)
 
         result.extend([e for _, _, e in elements])
 
@@ -746,20 +684,18 @@
 
     for direction in directions:
         text = direction.raw_text or direction.text
         e0 = etree.Element("direction")
         e1 = etree.SubElement(e0, "direction-type")
 
         if getattr(direction, "wedge", False):
-
             number = range_number_from_counter(direction, "wedge", counter)
             e2 = etree.SubElement(e1, "wedge", number="{}".format(number), type="stop")
 
         else:
-
             number = range_number_from_counter(direction, "wedge", counter)
             etree.SubElement(e1, "dashes", number="{}".format(number), type="stop")
 
         elem = (direction.end.t, None, e0)
         result.append(elem)
 
     tempos = part.iter_all(score.Tempo, start, end)
@@ -774,15 +710,14 @@
         # result.append((tempo.start.t, None, e0))
         e3 = etree.Element(
             "sound", tempo="{}".format(int(to_quarter_tempo(unit, tempo.bpm)))
         )
         result.append((tempo.start.t, None, e3))
 
     for direction in directions:
-
         text = direction.raw_text or direction.text
 
         if text in PEDAL_DIRECTIONS:
             # Pedal directions create an element for start
             # and an element for ending
 
             # Use end of the segment as ending of the pedal sign
@@ -827,47 +762,43 @@
                 elem = (ped_end.t, None, e0e)
                 result.append(elem)
         else:
             e0 = etree.Element("direction")
             e1 = etree.SubElement(e0, "direction-type")
 
             if text in DYN_DIRECTIONS:
-
                 e2 = etree.SubElement(e1, "dynamics")
                 etree.SubElement(e2, text)
 
             elif getattr(direction, "wedge", False):
-
                 if isinstance(direction, score.IncreasingLoudnessDirection):
                     wtype = "crescendo"
                 else:
                     wtype = "diminuendo"
 
                 number = range_number_from_counter(direction, "wedge", counter)
                 e2 = etree.SubElement(
                     e1, "wedge", number="{}".format(number), type=wtype
                 )
 
             else:
-
                 e2 = etree.SubElement(e1, "words")
                 e2.text = filter_string(text)
 
                 if (
                     isinstance(direction, score.DynamicDirection)
                     and direction.end is not None
                 ):
                     e3 = etree.SubElement(e0, "direction-type")
                     number = range_number_from_counter(direction, "dashes", counter)
                     etree.SubElement(
                         e3, "dashes", number="{}".format(number), type="start"
                     )
 
             if direction.staff is not None and direction.staff != 1:
-
                 e5 = etree.SubElement(e0, "staff")
                 e5.text = str(direction.staff)
 
             elem = (direction.start.t, None, e0)
             result.append(elem)
 
     return result
@@ -885,15 +816,19 @@
         function.text = h.text
         kind_e = etree.SubElement(harmony_e, "kind", text="")
         kind_e.text = "none"
         result.append((h.start.t, None, harmony_e))
     harmony = part.iter_all(score.ChordSymbol, start, end)
     for h in harmony:
         harmony_e = etree.Element("harmony", print_frame="no")
-        kind_e = etree.SubElement(harmony_e, "kind", text=h.kind) if h.kind is not None else etree.SubElement(harmony_e, "kind", text="")
+        kind_e = (
+            etree.SubElement(harmony_e, "kind", text=h.kind)
+            if h.kind is not None
+            else etree.SubElement(harmony_e, "kind", text="")
+        )
         kind_e.text = "none"
         root_e = etree.SubElement(harmony_e, "root")
         root_step_e = etree.SubElement(root_e, "root-step")
         root_step_e.text = h.root
         if h.bass is not None:
             bass_e = etree.SubElement(harmony_e, "bass")
             bass_step_e = etree.SubElement(bass_e, "bass-step")
@@ -930,79 +865,66 @@
     for o in part.iter_all(score.Staff, start, end):
         by_start[o.start.t].append(o)
 
     # sort clefs by number before adding them to by_start
     clefs_by_start = defaultdict(list)
 
     for o in part.iter_all(score.Clef, start, end):
-
         clefs_by_start[o.start.t].append(o)
 
     for t, clefs in clefs_by_start.items():
-
         clefs.sort(key=lambda clef: getattr(clef, "number", 0))
         by_start[t].extend(clefs)
 
     result = []
 
     # hacky: flag to include staves element before the first clef
     staves_included = False
 
     for t in sorted(by_start.keys()):
-
         attr_e = etree.Element("attributes")
 
         for o in by_start[t]:
-
             if isinstance(o, int):
-
                 etree.SubElement(attr_e, "divisions").text = "{}".format(o)
 
             elif isinstance(o, score.KeySignature):
-
                 ks_e = etree.SubElement(attr_e, "key")
                 etree.SubElement(ks_e, "fifths").text = "{}".format(o.fifths)
 
                 if o.mode:
-
                     etree.SubElement(ks_e, "mode").text = "{}".format(o.mode)
 
             elif isinstance(o, score.TimeSignature):
-
                 ts_e = etree.SubElement(attr_e, "time")
                 etree.SubElement(ts_e, "beats").text = "{}".format(o.beats)
                 etree.SubElement(ts_e, "beat-type").text = "{}".format(o.beat_type)
 
             elif isinstance(o, score.Clef):
-
                 if not staves_included:
                     staves_e = etree.SubElement(attr_e, "staves")
                     staves_e.text = "{}".format(len(clefs))
                     staves_included = True
 
                 clef_e = etree.SubElement(attr_e, "clef")
 
                 if o.staff and o.staff != 1:
-
                     clef_e.set("number", "{}".format(o.staff))
 
                 etree.SubElement(clef_e, "sign").text = "{}".format(o.sign)
                 etree.SubElement(clef_e, "line").text = "{}".format(o.line)
 
                 if o.octave_change:
-
                     etree.SubElement(clef_e, "clef-octave-change").text = "{}".format(
                         o.octave_change
                     )
             elif isinstance(o, score.Staff):
                 staff_e = etree.SubElement(attr_e, "staff-details")
                 if o.lines:
-                    etree.SubElement(staff_e, "staff-lines").text = "{}".format(
-                        o.lines
-                    )
+                    etree.SubElement(staff_e, "staff-lines").text = "{}".format(o.lines)
 
         result.append((t, None, attr_e))
 
     return result
 
 
 @deprecated_alias(parts="score_data")
@@ -1095,15 +1017,14 @@
             if pg.group_name is not None:
                 name_e = etree.SubElement(pg_e, "group-name")
                 name_e.text = pg.group_name
 
             group_stack.append(pg)
 
     for part in score_data:
-
         handle_parents(part)
 
         # handle part list entry
         scorepart_e = etree.SubElement(partlist_e, "score-part", id=part.id)
 
         partname_e = etree.SubElement(scorepart_e, "part-name")
         if part.part_name:
@@ -1114,60 +1035,53 @@
             partabbrev_e.text = filter_string(part.part_abbreviation)
 
         # write the part itself
 
         part_e = etree.SubElement(root, "part", id=part.id)
 
         for measure in part.iter_all(score.Measure):
-
             part_e.append(etree.Comment(MEASURE_SEP_COMMENT))
             attrib = {}
 
             if measure.number is not None:
-
                 attrib["number"] = str(measure.number)
 
             measure_e = etree.SubElement(part_e, "measure", **attrib)
             contents = linearize_measure_contents(
                 part, measure.start, measure.end, state
             )
             measure_e.extend(contents)
 
     close_group_stack()
 
     if out:
-
         if hasattr(out, "write"):
-
             out.write(
                 etree.tostring(
                     root.getroottree(),
                     encoding="UTF-8",
                     xml_declaration=True,
                     pretty_print=True,
                     doctype=DOCTYPE,
                 )
             )
 
         else:
-
             with open(out, "wb") as f:
-
                 f.write(
                     etree.tostring(
                         root.getroottree(),
                         encoding="UTF-8",
                         xml_declaration=True,
                         pretty_print=True,
                         doctype=DOCTYPE,
                     )
                 )
 
     else:
-
         return etree.tostring(
             root.getroottree(),
             encoding="UTF-8",
             xml_declaration=True,
             pretty_print=True,
             doctype=DOCTYPE,
         )
```

### Comparing `partitura-1.3.0/partitura/io/exportparangonada.py` & `partitura-1.3.1/partitura/io/exportparangonada.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         ("ppartid", "U256"),
     ]
 
     array = []
     # for all dicts create an appropriate entry in an array:
     # match = 0, deletion  = 1, insertion = 2
     for no, i in enumerate(alignment):
-
         if i["label"] == "match":
             array.append((no, "0", i["score_id"], str(i["performance_id"])))
         elif i["label"] == "insertion":
             array.append((no, "2", "undefined", str(i["performance_id"])))
         elif i["label"] == "deletion":
             array.append((no, "1", i["score_id"], "undefined"))
 
@@ -108,34 +107,34 @@
     """
 
     score_note_array = ensure_notearray(score_data)
 
     perf_note_array = ensure_notearray(performance_data)
 
     valid_score_note_array_fields = [
-                    "onset_beat",
-                    "duration_beat",
-                    "onset_quarter",
-                    "duration_quarter",
-                    "onset_div",
-                    "duration_div",
-                    "pitch",
-                    "voice",
-                    "id"
-                ]
+        "onset_beat",
+        "duration_beat",
+        "onset_quarter",
+        "duration_quarter",
+        "onset_div",
+        "duration_div",
+        "pitch",
+        "voice",
+        "id",
+    ]
 
     valid_perf_note_array_fields = [
-                    "onset_sec",
-                    "duration_sec",
-                    "pitch",
-                    "velocity",
-                    "track",
-                    "channel",
-                    "id",
-                ]
+        "onset_sec",
+        "duration_sec",
+        "pitch",
+        "velocity",
+        "track",
+        "channel",
+        "id",
+    ]
 
     ffields = [
         ("velocity", "<f4"),
         ("timing", "<f4"),
         ("articulation", "<f4"),
         ("id", "U256"),
     ]
```

### Comparing `partitura-1.3.0/partitura/io/importkern.py` & `partitura-1.3.1/partitura/io/importkern.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
                             "Dropping Opening Tie of note {} at position {} measure {}".format(
                                 dnote.midi_pitch, dnote.start.t, m_num
                             )
                         )
                         self.tie_dict["open"].pop(index)
                         self._handle_ties()
             else:
-                for (oid, cid) in list(
+                for oid, cid in list(
                     zip(self.tie_dict["open"], self.tie_dict["close"])
                 ):
                     self.nid_dict[oid].tie_next = self.nid_dict[cid]
                     self.nid_dict[cid].tie_prev = self.nid_dict[oid]
         except Exception:
             raise ValueError(
                 "Tie Mismatch! Uneven amount of closing to open tie brackets."
@@ -193,17 +193,15 @@
                 "Slur Mismatch! Uneven amount of closing to open slur brackets. Skipping slur parsing.",
                 ImportWarning,
             )
             # raise ValueError(
             #     "Slur Mismatch! Uneven amount of closing to open slur brackets."
             # )
         else:
-            for (oid, cid) in list(
-                zip(self.slur_dict["open"], self.slur_dict["close"])
-            ):
+            for oid, cid in list(zip(self.slur_dict["open"], self.slur_dict["close"])):
                 self.part.add(score.Slur(self.nid_dict[oid], self.nid_dict[cid]))
 
     def _handle_metersig(self, metersig):
         m = metersig[2:]
         numerator, denominator = map(eval, m.split("/"))
         new_time_signature = score.TimeSignature(numerator, denominator)
         self.part.add(new_time_signature, self.position)
```

### Comparing `partitura-1.3.0/partitura/io/importmatch.py` & `partitura-1.3.1/partitura/io/importmatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         try:
             ml = parser.from_matchline(line)
             if isinstance(getattr(ml, "Value", None), Version):
                 version = ml.Value
                 return version
 
         except MatchError:
-
             pass
 
     return version
 
 
 def parse_matchline(
     line: str,
@@ -192,22 +191,31 @@
 
     version = get_version(raw_lines[0])
 
     from_matchline_methods = FROM_MATCHLINE_METHODSV1
     if version < Version(1, 0, 0):
         from_matchline_methods = FROM_MATCHLINE_METHODSV0
 
-    parsed_lines = [
-        parse_matchline(line, from_matchline_methods, version) for line in raw_lines
-    ]
-
-    parsed_lines = [pl for pl in parsed_lines if pl is not None]
+    parsed_lines = list()
+    # Functionality to remove duplicate lines
+    for i, line in enumerate(raw_lines):
+        if line in raw_lines[i + 1 :] and line != "":
+            warnings.warn(f"Duplicate line found in matchfile: {line}")
+            continue
+        parsed_line = parse_matchline(line, from_matchline_methods, version)
+        if parsed_line is None:
+            warnings.warn(f"Could not empty parse line: {line} ")
+            continue
+        parsed_lines.append(parsed_line)
 
     mf = MatchFile(lines=parsed_lines)
 
+    # Validate match for duplicate snote_ids or pnote_ids
+    validate_match_ids(mf)
+
     return mf
 
 
 @deprecated_alias(fn="filename", create_part="create_score")
 def load_match(
     filename: PathLike,
     create_score: bool = False,
@@ -526,15 +534,14 @@
         rest = score.Rest()
         part.add(rest, start=0, end=t * divs)
         onset_in_divs += t * divs
         offset = 0
         t = t - t % beats_map(min_time)
 
     for b0, b1 in iter_current_next(bars, end=bars[-1] + 1):
-
         bar_times.setdefault(b0, t)
         if t < 0:
             t = 0
 
         else:
             # multiply by diff between consecutive bar numbers
             n_bars = b1 - b0
@@ -679,40 +686,45 @@
 
         # Check if the note is tied and if so, add the tie information
         if is_tied:
             found = False
             # iterate over all notes in the Timeline that end at the starting point.
             for el in part_note.start.iter_ending(score.Note):
                 if isinstance(el, score.Note):
-                    condition = el.step == note_attributes["step"] and el.octave == note_attributes["octave"] and el.alter == note_attributes["alter"]
+                    condition = (
+                        el.step == note_attributes["step"]
+                        and el.octave == note_attributes["octave"]
+                        and el.alter == note_attributes["alter"]
+                    )
                     if condition:
                         el.tie_next = part_note
                         part_note.tie_prev = el
                         found = True
                         break
             if not found:
                 warnings.warn(
-                    "Tie information found, but no previous note found to tie to for note {}.".format(part_note.id)
+                    "Tie information found, but no previous note found to tie to for note {}.".format(
+                        part_note.id
+                    )
                 )
 
     # add time signatures
-    for (ts_beat_time, ts_bar, tsg) in ts:
+    for ts_beat_time, ts_bar, tsg in ts:
         ts_beats = tsg.numerator
         ts_beat_type = tsg.denominator
         # check if time signature is in a known measure (from notes)
         if ts_bar in bar_times.keys():
             bar_start_divs = int(divs * (bar_times[ts_bar] - offset))  # in quarters
             bar_start_divs = max(0, bar_start_divs)
         else:
             bar_start_divs = 0
         part.add(score.TimeSignature(ts_beats, ts_beat_type), bar_start_divs)
 
     # add key signatures
-    for (ks_beat_time, ks_bar, keys) in mf.key_signatures:
-
+    for ks_beat_time, ks_bar, keys in mf.key_signatures:
         if ks_bar in bar_times.keys():
             bar_start_divs = int(divs * (bar_times[ks_bar] - offset))  # in quarters
             bar_start_divs = max(0, bar_start_divs)
         else:
             bar_start_divs = 0
 
         # TODO
@@ -823,15 +835,14 @@
             MIDI pitch to split staff into upper and lower. Default is 55
         only_missing: bool
             If True, only add staff to those notes that do not have staff info already.
     x"""
     # assign staffs using a hard limit
     notes = part.notes_tied
     for n in notes:
-
         if only_missing and n.staff:
             continue
 
         if n.midi_pitch > split:
             staff = 1
         else:
             staff = 2
@@ -843,10 +854,70 @@
             n_tied.staff = staff
             n_tied = n_tied.tie_next
 
     part.add(score.Clef(staff=1, sign="G", line=2, octave_change=0), 0)
     part.add(score.Clef(staff=2, sign="F", line=4, octave_change=0), 0)
 
 
-if __name__ == "__main__":
+def validate_match_ids(mf):
+    """
+    Check a matchfile for duplicate snote and note IDs.
+
+    This function will:
+    - remove all deletions with a score ID that occurs in multiple lines.
+    - remove all insertions with a performance ID that occurs in multiple lines.
+
+    Handles cases with conflicting match/insertion(s) and match/deletion(s) tuples
+    with any number of insertions or deletions and a single match by keeping
+    only the match.
+
+    Unhandled cases:
+    - multiple conflicting matches: all are kept.
+    - multiple insertions with the same ID: all are deleted.
+    - multiple deletions with the same ID: all are deleted.
 
+    Parameters
+    ----------
+    mf: MatchFile
+        MatchFile to validate
+
+    Returns
+    -------
+    Updates the representation of the matchfile by removing match lines.
+    """
+
+    # Check if the matchfile is valid (i.e. check for snote duplicates)
+    sids = np.array([n.Anchor for n in mf.snotes])
+    # First check if score ids are unique
+    sids_unique, counts = np.unique(sids, return_counts=True)
+    sids_to_check = sids_unique[np.where(counts > 1)[0]]
+    if len(sids_to_check) > 0:
+        indices_to_del = []
+        for i, line in enumerate(mf.lines):
+            if isinstance(line, BaseDeletionLine):
+                if line.Anchor in sids_to_check:
+                    indices_to_del.append(i)
+        warnings.warn(
+            "Matchfile contains duplicate score notes. "
+            "Removing {} deletions.".format(len(indices_to_del))
+        )
+        mf.lines = np.delete(mf.lines, indices_to_del)
+
+    # Check if the matchfile is valid (i.e. check for performance note duplicates)
+    pids = np.array([n.Id for n in mf.notes])
+    pids_unique, counts = np.unique(pids, return_counts=True)
+    pids_to_check = pids_unique[np.where(counts > 1)[0]]
+    if len(pids_to_check) > 0:
+        indices_to_del = []
+        for i, line in enumerate(mf.lines):
+            if isinstance(line, BaseInsertionLine):
+                if line.Id in pids_to_check:
+                    indices_to_del.append(i)
+        warnings.warn(
+            "Matchfile contains duplicate performance notes. "
+            "Removing {} insertions.".format(len(indices_to_del))
+        )
+        mf.lines = np.delete(mf.lines, indices_to_del)
+
+
+if __name__ == "__main__":
     pass
```

### Comparing `partitura-1.3.0/partitura/io/importmei.py` & `partitura-1.3.1/partitura/io/importmei.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,15 +485,16 @@
             part_list.append(new_staffgroup)
         return part_list
 
     # functions to parse the content of parts
 
     def _note_el_to_accid_int(self, note_el) -> int:
         """Accidental strings to integer pitch.
-        It consider the two values of accid and accid.ges (when the accidental is implicit in the bar)"""
+        It consider the two values of accid and accid.ges (when the accidental is implicit in the bar)
+        """
         if note_el.get("accid") is not None:
             return SIGN_TO_ALTER[note_el.get("accid")]
         elif note_el.get("accid.ges") is not None:
             return SIGN_TO_ALTER[note_el.get("accid.ges")]
         elif note_el.find(self._ns_name("accid")) is not None:
             if note_el.find(self._ns_name("accid")).get("accid") is not None:
                 return SIGN_TO_ALTER[note_el.find(self._ns_name("accid")).get("accid")]
```

### Comparing `partitura-1.3.0/partitura/io/importmidi.py` & `partitura-1.3.1/partitura/io/importmidi.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,80 +120,72 @@
 
     if merge_tracks:
         mid_merge = mido.merge_tracks(mid.tracks)
         tracks = [(0, mid_merge)]
     else:
         tracks = [(i, u) for i, u in enumerate(mid.tracks)]
     for i, track in tracks:
-
         notes = []
         controls = []
         programs = []
 
         t = 0
         ttick = 0
 
         sounding_notes = {}
 
         for msg in track:
-
             # update time deltas when they arrive
             t = t + msg.time * time_conversion_factor
             ttick = ttick + msg.time
 
             if msg.type == "set_tempo":
-
                 mpq = msg.tempo
                 time_conversion_factor = mpq / (ppq * 10**6)
 
             elif msg.type == "control_change":
-
                 controls.append(
                     dict(
                         time=t,
                         time_tick=ttick,
                         number=msg.control,
                         value=msg.value,
                         track=i,
                         channel=msg.channel,
                     )
                 )
 
             elif msg.type == "program_change":
-
                 programs.append(
                     dict(
                         time=t,
                         time_tick=ttick,
                         program=msg.program,
                         track=i,
                         channel=msg.channel,
                     )
                 )
 
             else:
-
                 note_on = msg.type == "note_on"
                 note_off = msg.type == "note_off"
 
                 if not (note_on or note_off):
                     continue
 
                 # hash sounding note
                 note = note_hash(msg.channel, msg.note)
 
                 # start note if it's a 'note on' event with velocity > 0
                 if note_on and msg.velocity > 0:
-
                     # save the onset time and velocity
                     sounding_notes[note] = (t, ttick, msg.velocity)
 
                 # end note if it's a 'note off' event or 'note on' with velocity 0
                 elif note_off or (note_on and msg.velocity == 0):
-
                     if note not in sounding_notes:
                         warnings.warn("ignoring MIDI message %s" % msg)
                         continue
 
                     # append the note to the list associated with the channel
 
                     notes.append(
@@ -360,15 +352,14 @@
         # dictionary for storing the last onset time and velocity for each
         # individual note (i.e. same pitch and channel)
         sounding_notes = {}
         # current time (will be updated by delta times in messages)
         t_raw = 0
 
         for msg in track:
-
             t_raw = t_raw + msg.time
 
             if msg.type not in relevant:
                 continue
 
             if quantization_unit:
                 t = quantize(t_raw, quantization_unit)
@@ -389,21 +380,19 @@
                     continue
 
                 # hash sounding note
                 note = note_hash(msg.channel, msg.note)
 
                 # start note if it's a 'note on' event with velocity > 0
                 if note_on and msg.velocity > 0:
-
                     # save the onset time and velocity
                     sounding_notes[note] = (t, msg.velocity)
 
                 # end note if it's a 'note off' event or 'note on' with velocity 0
                 elif note_off or (note_on and msg.velocity == 0):
-
                     if note not in sounding_notes:
                         warnings.warn("ignoring MIDI message %s" % msg)
                         continue
 
                     # append the note to the list associated with the channel
                     notes[msg.channel].append(
                         (sounding_notes[note][0], msg.note, t - sounding_notes[note][0])
@@ -424,15 +413,14 @@
 
         for ch, ch_notes in notes.items():
             # if there are any notes, store the notes along with key sig / time
             # sig / tempo information under the key (track_nr, ch_nr)
             if len(ch_notes) > 0:
                 notes_by_track_ch[(track_nr, ch)] = ch_notes
 
-
     tr_ch_keys = sorted(notes_by_track_ch.keys())
     group_part_voice_keys, part_names, group_names = assign_group_part_voice(
         part_voice_assign_mode, tr_ch_keys, track_names_by_track
     )
 
     # for key and time sigs:
     track_to_part_mapping = make_track_to_part_mapping(
```

### Comparing `partitura-1.3.0/partitura/io/importmusic21.py` & `partitura-1.3.1/partitura/io/importmusic21.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import numpy as np
 from fractions import Fraction
 
 try:
     import music21 as m21
     from music21.stream import Score as M21Score
 except ImportError:
-
     m21 = None
 
     class M21Score(object):
         pass
 
 
 def load_music21(m21_score: M21Score) -> pt.score.Score:
```

### Comparing `partitura-1.3.0/partitura/io/importmusicxml.py` & `partitura-1.3.1/partitura/io/importmusicxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     structure = []
     current_group = None
     part_dict = {}
 
     for e in partlist:
         if e.tag == "part-group":
             if e.get("type") == "start":
-
                 gr_name = get_value_from_tag(e, "group-name", str)
                 gr_symbol = get_value_from_tag(e, "group-symbol", str)
                 gr_number = get_value_from_attribute(e, "number", int)
                 new_group = score.PartGroup(gr_symbol, gr_name, gr_number)
 
                 if current_group is None:
                     current_group = new_group
@@ -258,25 +257,23 @@
 
         title = scid
 
     score_identification_el = document.find("identification")
 
     # The identification tag has preference over credit
     if score_identification_el is not None:
-
         copyright = get_value_from_tag(score_identification_el, "rights", str)
 
         for cel in score_identification_el.findall("creator"):
             if get_value_from_attribute(cel, "type", str) == "composer":
                 composer = str(cel.text)
             if get_value_from_attribute(cel, "type", str) == "lyricist":
                 lyricist = str(cel.text)
 
     for cel in document.findall("credit"):
-
         credit_type = get_value_from_tag(cel, "credit-type", str)
         if credit_type == "title" and title is None:
             title = get_value_from_tag(cel, "credit-words", str)
 
         elif credit_type == "subtitle" and subtitle is None:
             subtitle = get_value_from_tag(cel, "credit-words", str)
 
@@ -313,15 +310,14 @@
         The ElementTree representation of the MusicXML document
     part_dict : dict
         A dictionary with key--value pairs (part_id, Part instance), as returned
         by the _parse_partlist() function.
     """
 
     for part_el in document.findall("part"):
-
         part_id = part_el.get("id", "P1")
         part = part_dict.get(part_id, score.Part(part_id))
 
         position = 0
         ongoing = {}
         doc_order = 0
         # add new page and system at start of part
@@ -411,15 +407,14 @@
                         part.remove(o_i)
                 else:
                     part.remove(o)
 
         # check whether all grace notes have a main note
         for gn in part.iter_all(score.GraceNote):
             if gn.main_note is None:
-
                 for no in part.iter_all(
                     score.Note,
                     include_subclasses=False,
                     start=gn.start.t,
                     end=gn.start.t + 1,
                 ):
                     if no.voice == gn.voice:
@@ -452,40 +447,40 @@
         #                 note.octave -= OCTAVE_SHIFTS[shift.shift_size] if shift.shift_size in OCTAVE_SHIFTS.keys() else 0
         #             elif shift.shift_type == "down":
         #                 note.octave += OCTAVE_SHIFTS[shift.shift_size] if shift.shift_size in OCTAVE_SHIFTS.keys() else 0
         #     shift.applied = True
 
 
 def _handle_measure(measure_el, position, part, ongoing, doc_order, measure_counter):
-    """ Parse a <measure>...</measure> element, adding it and its contents to the part.
-    
+    """Parse a <measure>...</measure> element, adding it and its contents to the part.
+
     Parameters
     ----------
     measure_el : etree.Element
         An etree Element instance with a <measure> tag
     position : int
         The starting time of the measure
     part : score.Part
         The part object to which the measure belongs.
     ongoing : dict
         A dict specifying the score.Page and score.System of the measure
     doc_order : int
         The index of the first note element in the current measure in the xml file.
     measure_counter : int
         The index of the <measure> tag in the xml file, starting from 1
-    
+
     Returns
     -------
     measure_maxtime : int
         The ending time of the measure
     doc_order : int
         The index of the first note element in the next measure in the xml file.
-        
+
     """
-    
+
     # make a measure object
     measure = make_measure(measure_el, measure_counter)
 
     # add the start of the measure to the time line
     part.add(measure, position)
 
     # keep track of the position within the measure
@@ -493,15 +488,14 @@
     measure_start = position
     # keep track of the previous note (in case of <chord>)
     prev_note = None
     # used to keep track of the duration of the measure
     measure_maxtime = measure_start
     trailing_children = []
     for i, e in enumerate(measure_el):
-
         if e.tag == "backup":
             # <xs:documentation>The backup and forward elements are required
             # to coordinate multiple voices in one part, including music on
             # multiple staves. The backup type is generally used to move
             # between voices and staves. Thus the backup element does not
             # include voice or staff elements. Duration values should always
             # be positive, and should not cross measure boundaries or
@@ -604,15 +598,15 @@
             warnings.warn("ignoring tag {0}".format(e.tag), stacklevel=2)
 
     for obj in trailing_children:
         part.add(obj, measure_maxtime)
 
     # add end time of measure
     part.add(measure, None, measure_maxtime)
-    
+
     return measure_maxtime, doc_order
 
 
 def _handle_harmony(e, position, part):
     """Handle a <harmony> element."""
     if e.find("function") is not None:
         text = e.find("function").text
@@ -631,21 +625,19 @@
         warnings.warn("ignoring empty <harmony> tag", stacklevel=2)
 
 
 def _handle_repeat(e, position, part, ongoing):
     key = "repeat"
 
     if e.get("direction") == "forward":
-
         o = score.Repeat()
         ongoing[key] = o
         part.add(o, position)
 
     elif e.get("direction") == "backward":
-
         o = ongoing.pop(key, None)
 
         if o is None:
             # implicit repeat start: create Repeat
             # object and add it at the beginning of
             # the self retroactively
             o = score.Repeat()
@@ -656,34 +648,30 @@
 
 
 def _handle_ending(e, position, part, ongoing):
     # key = "ending"
     key = ("ending", getattr(e, "number", "0"))
 
     if e.get("type") == "start":
-
         o = score.Ending(e.get("number"))
         ongoing[key] = o
         part.add(o, position)
 
     elif e.get("type") in ("stop", "discontinue"):
-
         o = ongoing.pop(key, None)
 
         if o is None:
-
             warnings.warn(
                 "Found ending[stop] without a preceding ending[start]\n"
                 + "Single measure bracket is assumed"
             )
             o = score.Ending(e.get("number"))
             part.add(o, None, position)
 
         else:
-
             part.add(o, None, position)
 
 
 def _handle_new_page(position, part, ongoing):
     if "page" in ongoing:
         if position == 0:
             # ignore non-informative new-page at start of score
@@ -697,15 +685,14 @@
     page = score.Page(page_nr)
     part.add(page, position)
     ongoing["page"] = page
 
 
 def _handle_new_system(position, part, ongoing):
     if "system" in ongoing:
-
         if position == 0:
             # ignore non-informative new-system at start of score
             return
 
         # end current page
         part.add(ongoing["system"], None, position)
         system_nr = ongoing["system"].number + 1
@@ -721,21 +708,21 @@
     """
     Parameters
     ----------
     xml_measure : etree.Element
         An etree Element instance with a <measure> tag
     measure_counter : int
         The index of the <measure> tag in the xml file, starting from 1
-    
+
     Returns
     -------
     measure : score.Measure
         A measure object with a number and optional name attribute
     """
-    
+
     measure = score.Measure()
 
     measure.number = measure_counter
     measure.name = get_value_from_attribute(xml_measure, "number", str)
 
     return measure
 
@@ -768,25 +755,22 @@
         part.add(score.Clef(**clef), position)
 
 
 def get_offset(e):
     offset = e.find("offset")
 
     if offset is None:
-
         return None
 
     else:
-
         sounding = offset.attrib.get("sound", "no")
         return int(offset.text) if sounding == "yes" else 0
 
 
 def _handle_direction(e, position, part, ongoing):
-
     # <!--
     #     A direction is a musical indication that is not attached
     #     to a specific note. Two or more may be combined to
     #     indicate starts and stops of wedges, dashes, etc.
 
     #     By default, a series of direction-type elements and a
     #     series of child elements of a direction-type within a
@@ -865,44 +849,40 @@
                     )
                     starting_directions.append(direction)
 
         elif dt.tag == "words":
             # first child of direction-type is words, there may be subsequent
             # words items, so we loop:
             for child in direction_type:
-
                 # try to make a direction out of words
                 parse_result = parse_direction(child.text)
                 starting_directions.extend(parse_result)
 
         elif dt.tag == "wedge":
-
             number = get_value_from_attribute(dt, "number", int) or 1
             key = ("wedge", number)
             wedge_type = get_value_from_attribute(dt, "type", str)
 
             if wedge_type in ("crescendo", "diminuendo"):
                 if wedge_type == "crescendo":
                     o = score.IncreasingLoudnessDirection(wedge_type, wedge=True)
                 else:
                     o = score.DecreasingLoudnessDirection(wedge_type, wedge=True)
                 starting_directions.append(o)
                 ongoing[key] = o
 
             elif wedge_type == "stop":
-
                 o = ongoing.get(key)
                 if o is not None:
                     ending_directions.append(o)
                     del ongoing[key]
                 else:
                     warnings.warn("Did not find a wedge start element for wedge stop!")
 
         elif dt.tag == "dashes":
-
             # start/stop/continue
             dashes_type = get_value_from_attribute(dt, "type", str)
             number = get_value_from_attribute(dt, "number", int) or 1
             dashes_keys[("dashes", number)] = dashes_type
             # TODO: for now we ignore dashes_type == continue, because it exists
             # only as a function of the visual appearance. However, if dashes
             # that are continued over a system are stopped at the end of the
@@ -925,27 +905,25 @@
                 )
 
                 starting_directions.append(o)
 
                 ongoing[key] = o
 
             elif octave_shift_type == "stop":
-
                 o = ongoing.get(key)
                 if o is not None:
                     ending_directions.append(o)
                     del ongoing[key]
 
                 else:
                     warnings.warn(
                         "Did not find a octave_shift start element for octave_shift stop!"
                     )
 
         elif dt.tag == "pedal":
-
             # start/stop
             pedal_type = get_value_from_attribute(dt, "type", str)
             pedal_line = get_value_from_attribute(dt, "line", str) == "yes"
 
             number = get_value_from_attribute(dt, "number", int) or 1
             key = ("pedal", number)
             if pedal_type == "start":
@@ -956,15 +934,14 @@
                 o = score.SustainPedalDirection(staff=staff, line=pedal_line)
 
                 starting_directions.append(o)
 
                 ongoing[key] = o
 
             elif pedal_type == "stop":
-
                 o = ongoing.get(key)
                 if o is not None:
                     ending_directions.append(o)
                     del ongoing[key]
 
                 else:
                     warnings.warn("Did not find a pedal start element for pedal stop!")
@@ -976,21 +953,18 @@
                         "not supported. Ignoring direction."
                     )
 
         else:
             warnings.warn("ignoring direction type: {} {}".format(dt.tag, dt.attrib))
 
     for dashes_key, dashes_type in dashes_keys.items():
-
         if dashes_type == "start":
-
             ongoing[dashes_key] = starting_directions
 
         elif dashes_type == "stop":
-
             oo = ongoing.get(dashes_key)
             if oo is None:
                 warnings.warn("Dashes end without dashes start")
             else:
                 ending_directions.extend(oo)
                 del ongoing[dashes_key]
 
@@ -1163,15 +1137,14 @@
     if "tempo" in e.attrib:
         tempo = score.Tempo(int(e.attrib["tempo"]), "q")
         # part.add_starting_object(position, tempo)
         _add_tempo_if_unique(position, part, tempo)
 
 
 def _handle_note(e, position, part, ongoing, prev_note, doc_order):
-
     # get some common features of element if available
     duration = get_value_from_tag(e, "duration", int) or 0
     # elements may have an explicit temporal offset
     # offset = get_value_from_tag(e, 'offset', int) or 0
     staff = get_value_from_tag(e, "staff", int) or 1
     voice = get_value_from_tag(e, "voice", int) or 1
 
@@ -1217,15 +1190,14 @@
         ornaments = get_ornaments(ornaments_e)
     else:
         ornaments = {}
 
     pitch = e.find("pitch")
     unpitch = e.find("unpitched")
     if pitch is not None:
-
         step = get_value_from_tag(pitch, "step", str)
         alter = get_value_from_tag(pitch, "alter", int)
         octave = get_value_from_tag(pitch, "octave", int)
 
         grace = e.find("grace")
 
         if grace is not None:
@@ -1300,62 +1272,52 @@
             doc_order=doc_order,
         )
 
     part.add(note, position, position + duration)
 
     ties = e.findall("tie")
     if len(ties) > 0:
-
         tie_key = ("tie", getattr(note, "midi_pitch", "rest"))
         tie_types = set(tie.attrib["type"] for tie in ties)
 
         if "stop" in tie_types:
-
             tie_prev = ongoing.get(tie_key, None)
 
             if tie_prev:
-
                 note.tie_prev = tie_prev
                 tie_prev.tie_next = note
                 del ongoing[tie_key]
 
         if "start" in tie_types:
-
             ongoing[tie_key] = note
 
     notations = e.find("notations")
 
     if notations is not None:
-
         if notations.find("fermata") is not None:
-
             fermata = score.Fermata(note)
             part.add(fermata, position)
             note.fermata = fermata
 
         starting_slurs, stopping_slurs = handle_slurs(
             notations, ongoing, note, position
         )
 
         for slur in starting_slurs:
-
             part.add(slur, position)
 
         for slur in stopping_slurs:
-
             part.add(slur, end=position + duration)
 
         starting_tups, stopping_tups = handle_tuplets(notations, ongoing, note)
 
         for tup in starting_tups:
-
             part.add(tup, position)
 
         for tup in stopping_tups:
-
             part.add(tup, end=position + duration)
 
     new_position = position + duration
 
     return new_position, note
 
 
@@ -1373,39 +1335,34 @@
     # by their numbers; First note that tuplets do not always
     # have a number attribute, then 1 is implied.
     tuplets.sort(
         key=lambda x: get_value_from_attribute(x, "number", int) or note.voice or 1
     )
 
     for tuplet_e in tuplets:
-
         tuplet_number = get_value_from_attribute(tuplet_e, "number", int) or note.voice
         tuplet_type = get_value_from_attribute(tuplet_e, "type", str)
         start_tuplet_key = ("start_tuplet", tuplet_number)
         stop_tuplet_key = ("stop_tuplet", tuplet_number)
 
         if tuplet_type == "start":
-
             # check if we have a stopped_tuplet in ongoing that corresponds to
             # this start
             tuplet = ongoing.pop(stop_tuplet_key, None)
 
             if tuplet is None:
-
                 tuplet = score.Tuplet(note)
                 ongoing[start_tuplet_key] = tuplet
 
             else:
-
                 tuplet.start_note = note
 
             starting_tuplets.append(tuplet)
 
         elif tuplet_type == "stop":
-
             tuplet = ongoing.pop(start_tuplet_key, None)
             if tuplet is None:
                 # tuplet stop occurs before tuplet start in document order, that
                 # is a valid scenario
                 tuplet = score.Tuplet(None, note)
                 ongoing[stop_tuplet_key] = tuplet
             else:
@@ -1436,30 +1393,27 @@
     # by their numbers; First note that slurs do not always
     # have a number attribute, then 1 is implied.
     slurs.sort(
         key=lambda x: get_value_from_attribute(x, "number", int) or note.voice or 1
     )
 
     for slur_e in slurs:
-
         slur_number = get_value_from_attribute(slur_e, "number", int) or note.voice
         slur_type = get_value_from_attribute(slur_e, "type", str)
         start_slur_key = ("start_slur", slur_number)
         stop_slur_key = ("stop_slur", slur_number)
 
         if slur_type == "start":
-
             # check if we have a stopped_slur in ongoing that corresponds to
             # this stop
             slur = ongoing.pop(stop_slur_key, None)
 
             # if slur.end_note.start.t < position then the slur stop is
             # rogue. We drop it and treat the slur start like a fresh start
             if slur is None or slur.end_note.start.t < position:
-
                 if slur and slur.end_note.start.t < position:
                     msg = (
                         "Dropping slur {} starting at {} ({}) and ending "
                         "at {} ({})".format(
                             slur_number,
                             position,
                             note.id,
@@ -1473,25 +1427,22 @@
                     # remove the reference to the slur in the end note
                     slur.end_note.slur_stops.remove(slur)
 
                 slur = score.Slur(note)
                 ongoing[start_slur_key] = slur
 
             else:
-
                 slur.start_note = note
 
             starting_slurs.append(slur)
 
         elif slur_type == "stop":
-
             slur = ongoing.pop(start_slur_key, None)
 
             if slur is None or slur.start_note.start.t > position:
-
                 if slur and slur.start_note.start.t > position:
                     msg = (
                         "Dropping slur {} starting at {} ({}) and ending "
                         "at {} ({})".format(
                             slur_number,
                             slur.start_note.start.t,
                             slur.start_note.id,
@@ -1507,15 +1458,14 @@
 
                 # slur stop occurs before slur start in document order, that
                 # is a valid scenario
                 slur = score.Slur(None, note)
                 ongoing[stop_slur_key] = slur
 
             else:
-
                 slur.end_note = note
 
             stopping_slurs.append(slur)
 
     return starting_slurs, stopping_slurs
```

### Comparing `partitura-1.3.0/partitura/io/importnakamura.py` & `partitura-1.3.1/partitura/io/importnakamura.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/io/importparangonada.py` & `partitura-1.3.1/partitura/io/importparangonada.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     )
 
     columns = raw_array[0]
     dtypes = [NOTE_ARRAY_DTYPES.get(c, (c, "U256")) for c in columns]
 
     struct_array = np.empty(len(raw_array) - 1, dtype=dtypes)
     for i, (c, dt) in enumerate(zip(columns, dtypes)):
-
         if dt[-1] == "i4":
             # Weird behavior trying to cast 0.0 as an integer
             struct_array[c] = raw_array[1:, i].astype(float).astype(int)
         else:
             struct_array[c] = raw_array[1:, i].astype(dt[-1])
 
     return struct_array
```

### Comparing `partitura-1.3.0/partitura/io/matchfile_base.py` & `partitura-1.3.1/partitura/io/matchfile_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -591,19 +591,17 @@
 
     @classmethod
     def prepare_kwargs_from_matchline(
         cls,
         matchline: str,
         pos: int = 0,
     ) -> Dict:
-
         match_pattern = cls.pattern.search(matchline, pos)
 
         if match_pattern is not None:
-
             (
                 anchor_str,
                 note_name_str,
                 modifier_str,
                 octave_str,
                 measure_str,
                 beat_str,
@@ -636,15 +634,14 @@
             )
 
         else:
             raise MatchError("Input match line does not fit the expected pattern.")
 
 
 class BaseNoteLine(MatchLine):
-
     # All derived classes should include at least
     # these field names
     field_names = (
         "Id",
         "Onset",
         "Offset",
         "Velocity",
@@ -679,24 +676,22 @@
 
     @property
     def Duration(self):
         return self.Offset - self.Onset
 
 
 class BaseSnoteNoteLine(MatchLine):
-
     out_pattern = "{SnoteLine}-{NoteLine}"
 
     def __init__(
         self,
         version: Version,
         snote: BaseSnoteLine,
         note: BaseNoteLine,
     ) -> None:
-
         super().__init__(version)
 
         self.snote = snote
         self.note = note
 
         self.field_names = self.snote.field_names + self.note.field_names
 
@@ -710,15 +705,14 @@
     def matchline(self) -> str:
         return self.out_pattern.format(
             SnoteLine=self.snote.matchline,
             NoteLine=self.note.matchline,
         )
 
     def __str__(self) -> str:
-
         """
         Prints the printing the match line
         """
         r = [self.__class__.__name__]
         r += [" Snote"] + [
             "   {0}: {1}".format(fn, getattr(self.snote, fn, None))
             for fn in self.snote.field_names
@@ -771,19 +765,17 @@
             note=note,
         )
 
         return kwargs
 
 
 class BaseDeletionLine(MatchLine):
-
     out_pattern = "{SnoteLine}-deletion."
 
     def __init__(self, version: Version, snote: BaseSnoteLine) -> None:
-
         super().__init__(version)
 
         self.snote = snote
 
         self.field_names = self.snote.field_names
 
         self.field_types = self.snote.field_types
@@ -804,31 +796,28 @@
     @classmethod
     def prepare_kwargs_from_matchline(
         cls,
         matchline: str,
         snote_class: BaseSnoteLine,
         version: Version,
     ) -> Dict:
-
         snote = snote_class.from_matchline(matchline, version=version)
 
         kwargs = dict(
             version=version,
             snote=snote,
         )
 
         return kwargs
 
 
 class BaseInsertionLine(MatchLine):
-
     out_pattern = "insertion-{NoteLine}"
 
     def __init__(self, version: Version, note: BaseNoteLine) -> None:
-
         super().__init__(version)
 
         self.note = note
 
         self.field_names = self.note.field_names
 
         self.field_types = self.note.field_types
@@ -849,37 +838,34 @@
     @classmethod
     def prepare_kwargs_from_matchline(
         cls,
         matchline: str,
         note_class: BaseNoteLine,
         version: Version,
     ) -> Dict:
-
         note = note_class.from_matchline(matchline, version=version)
 
         kwargs = dict(
             version=version,
             note=note,
         )
 
         return kwargs
 
 
 class BaseOrnamentLine(MatchLine):
-
     # These field names and types need to be expanded
     # with the attributes of the note
     field_names = ("Anchor",)
     field_types = (str,)
     format_fun = dict(Anchor=format_string)
     out_pattern = "ornament({Anchor})-{NoteLine}"
     ornament_pattern: re.Pattern = re.compile(r"ornament\((?P<Anchor>[^\)]*)\)-")
 
     def __init__(self, version: Version, anchor: str, note: BaseNoteLine) -> None:
-
         super().__init__(version)
 
         self.note = note
 
         self.field_names = self.field_names + self.note.field_names
 
         self.field_types = self.field_types + self.note.field_types
@@ -903,15 +889,14 @@
     @classmethod
     def prepare_kwargs_from_matchline(
         cls,
         matchline: str,
         note_class: BaseNoteLine,
         version: Version,
     ) -> Dict:
-
         anchor_pattern = cls.ornament_pattern.search(matchline)
 
         if anchor_pattern is None:
             raise MatchError("")
 
         anchor = interpret_as_string(anchor_pattern.group("Anchor"))
         note = note_class.from_matchline(matchline, version=version)
@@ -953,49 +938,45 @@
     @classmethod
     def prepare_kwargs_from_matchline(
         cls,
         matchline: str,
         version: Version,
         pos: int = 0,
     ) -> Dict:
-
         kwargs = None
         # pattern = re.compile(cls.base_pattern.format(pedal_type=pedal_type))
 
         match_pattern = cls.pattern.search(matchline, pos=pos)
 
         if match_pattern is not None:
-
             time_str, value_str = match_pattern.groups()
 
             kwargs = dict(
                 version=version,
                 time=interpret_as_int(time_str),
                 value=interpret_as_int(value_str),
             )
 
         return kwargs
 
 
 class BaseSustainPedalLine(BasePedalLine):
-
     pattern = re.compile(r"sustain\((?P<Time>[^,]+),(?P<Value>[^,]+)\)\.")
     out_pattern: str = "sustain({Time},{Value})."
 
     def __init__(
         self,
         version: Version,
         time: int,
         value: int,
     ):
         super().__init__(version=version, time=time, value=value)
 
 
 class BaseSoftPedalLine(BasePedalLine):
-
     pattern = re.compile(r"soft\((?P<Time>[^,]+),(?P<Value>[^,]+)\)\.")
     out_pattern: str = "soft({Time},{Value})."
 
     def __init__(
         self,
         version: Version,
         time: int,
@@ -1018,15 +999,14 @@
     Class for representing MatchFiles
     """
 
     version: Version
     lines: np.ndarray
 
     def __init__(self, lines: Iterable[MatchLine]) -> None:
-
         # check that all lines have the same version
         same_version = all([line.version == lines[0].version for line in lines])
 
         if not same_version:
             raise ValueError("All lines should have the same version")
 
         self.lines = np.array(lines)
@@ -1183,15 +1163,14 @@
                 if k[2] != keysigs[-1][2]:
                     keysigs.append(k)
 
         return keysigs
 
     @property
     def key_sig_lines(self):
-
         ml = [
             line
             for line in self.lines
             if getattr(line, "Attribute", None) == "keySignature"
         ]
 
         return ml
```

### Comparing `partitura-1.3.0/partitura/io/matchfile_utils.py` & `partitura-1.3.1/partitura/io/matchfile_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,14 @@
     return str(value)
 
 
 old_string_pat = re.compile(r"'(?P<value>.+)'")
 
 
 def interpret_as_string_old(value: str) -> str:
-
     val = old_string_pat.match(value)
     if val is not None:
         return val.group("value").strip()
     else:
         return value.strip()
 
 
@@ -268,15 +267,14 @@
     def __init__(
         self,
         numerator: int,
         denominator: int = 1,
         tuple_div: Optional[int] = None,
         add_components: Optional[List[Tuple[int, int, Optional[int]]]] = None,
     ) -> None:
-
         self.numerator = numerator
         self.denominator = denominator
         self.tuple_div = tuple_div
         self.add_components = add_components
         self.bound_integers(1024)
 
     def _str(
@@ -455,15 +453,14 @@
         # Cast as float since the ability to return an instance of a strict
         # subclass of float is deprecated, and may be removed in a future
         # version of Python. (following a deprecation warning)
         return float(self.numerator / (self.denominator * (self.tuple_div or 1)))
 
     @classmethod
     def from_string(cls, string: str, allow_additions: bool = True):
-
         m = rational_pattern.match(string)
         m2 = double_rational_pattern.match(string)
         m3 = integer_pattern.match(string)
         if m:
             groups = m.groups()
             return cls(*[int(g) for g in groups])
         elif m2:
@@ -533,15 +530,14 @@
 def format_fractional_rational(value: FractionalSymbolicDuration) -> str:
     """
     Format fractional symbolic duration as string and ensure that the output
     is always rational ("a/b")
     """
 
     if value.denominator == 1 and value.tuple_div is None:
-
         out = f"{value.numerator}/1"
 
     else:
         out = str(value)
 
     return out
 
@@ -584,30 +580,27 @@
 
 def format_list(value: List[Any]) -> str:
     formatted_string = f"[{','.join([str(v) for v in value])}]"
     return formatted_string
 
 
 def format_accidental(value: Optional[int]) -> str:
-
     alter = "n" if value == 0 else ALTER_SIGNS[value]
 
     return alter
 
 
 def format_accidental_old(value: Optional[int]) -> str:
-
     if value is None:
         return "-"
     else:
         return format_accidental(value)
 
 
 def format_pnote_id(value: Any) -> str:
-
     pnote_id = f"n{str(value)}" if not str(value).startswith("n") else str(value)
 
     return pnote_id
 
 
 ## Methods for parsing special attributes
 
@@ -680,15 +673,14 @@
         name = keylist[fifths + 7]
 
         ks = f"{name} {suffix}"
 
         return ks
 
     def __str__(self):
-
         if self.fmt == "v1.0.0":
             ks = fifths_mode_to_key_name(self.fifths, self.mode)
 
             if self.fifths_alt is not None:
                 ks = f"{ks}/{fifths_mode_to_key_name(self.fifths_alt, self.mode_alt)}"
 
         if self.fmt == "v0.3.0":
@@ -701,41 +693,38 @@
             ks = self.fifths_mode_to_key_name_v0_1_0(self.fifths, self.mode)
 
         if self.is_list:
             return format_list([ks] + self.other_components)
         return ks
 
     def __eq__(self, ks: MatchKeySignature) -> bool:
-
         crit = (
             self.fifths == ks.fifths
             and self.mode == ks.mode
             and self.fifths_alt == ks.fifths_alt
             and self.mode_alt == ks.mode_alt
             and self.other_components == ks.other_components
         )
 
         return crit
 
     @classmethod
     def _parse_key_signature(cls, kstr: str) -> MatchKeySignature:
-
         # import pdb
         # pdb.set_trace()
         ksinfo = key_signature_pattern.search(kstr)
 
         if ksinfo is None:
             fmt = "v1.0.0"
             ksinfo = kstr.split("/")
             fifths1, mode1 = key_name_to_fifths_mode(ksinfo[0].upper())
             fifths2, mode2 = None, None
             if len(ksinfo) == 2:
                 fifths2, mode2 = key_name_to_fifths_mode(ksinfo[1].upper())
         else:
-
             fmt = "v0.3.0"
             step1, alter1, mode1, step2, alter2, mode2 = ksinfo.groups()
             mode1_str = "m" if mode1.lower() in ("minor", "min") else ""
             fifths1, mode1 = key_name_to_fifths_mode(
                 f"{step1.upper()}{alter1}{mode1_str}"
             )
 
@@ -775,15 +764,14 @@
                 fifths, mode = key_name_to_fifths_mode(
                     f"{step.upper()}{alter_str}{mode_str}"
                 )
 
                 return cls(fifths=fifths, mode=mode, fmt="v0.1.0")
 
         if len(content) > 0:
-
             ksigs = [cls._parse_key_signature(ksig) for ksig in content]
 
             ks = ksigs[0]
             ks.other_components = ksigs[1:] if len(ksigs) > 1 else []
 
             return ks
 
@@ -834,23 +822,21 @@
         super().__init__()
         self.numerator = numerator
         self.denominator = denominator
         self.other_components = other_components
         self.is_list = is_list
 
     def __str__(self):
-
         ts = f"{self.numerator}/{self.denominator}"
         if self.is_list:
             return format_list([ts] + self.other_components)
         else:
             return ts
 
     def __eq__(self, ts: MatchKeySignature) -> bool:
-
         crit = (
             (self.numerator == ts.numerator)
             and (self.denominator == ts.denominator)
             and (self.other_components == ts.other_components)
         )
         return crit
 
@@ -867,15 +853,14 @@
             denominator=denominator,
             other_components=other_components,
             is_list=is_list,
         )
 
 
 def interpret_as_time_signature(value: str) -> MatchTimeSignature:
-
     ts = MatchTimeSignature.from_string(value)
     return ts
 
 
 def format_time_signature(value: MatchTimeSignature) -> str:
     value.is_list = False
     return str(value)
@@ -908,15 +893,14 @@
     Convert name in snake_case to camelCase
     """
     parts = field_name.split("_")
 
     camel_case = f"{parts[0].lower()}"
 
     if len(parts) > 1:
-
         camel_case += "".join([p.title() for p in parts[1:]])
 
     return camel_case
 
 
 def get_kwargs_from_matchline(
     matchline: str,
@@ -939,15 +923,14 @@
     kwargs : dict
 
     """
     kwargs = None
     match_pattern = pattern.search(matchline, pos=pos)
 
     if match_pattern is not None:
-
         kwargs = dict(
             [
                 (to_snake_case(fn), class_dict[fn][0](match_pattern.group(fn)))
                 for fn in field_names
             ]
         )
```

### Comparing `partitura-1.3.0/partitura/io/matchlines_v0.py` & `partitura-1.3.1/partitura/io/matchlines_v0.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,14 @@
         self,
         version: Version,
         attribute: str,
         value: Any,
         value_type: type,
         format_fun: Callable[Any, str],
     ) -> None:
-
         if version >= Version(1, 0, 0):
             raise ValueError("The version must be < 1.0.0")
 
         super().__init__(
             version=version,
             attribute=attribute,
             value=value,
@@ -290,15 +289,14 @@
     Version(0, 3, 0): default_meta_attributes,
     Version(0, 4, 0): default_meta_attributes,
     Version(0, 5, 0): default_meta_attributes,
 }
 
 
 class MatchMeta(MatchLine):
-
     field_names = (
         "Attribute",
         "Value",
         "Measure",
         "TimeInBeats",
     )
 
@@ -318,15 +316,14 @@
         attribute: str,
         value: Any,
         value_type: type,
         format_fun: Callable[Any, str],
         measure: int,
         time_in_beats: float,
     ) -> None:
-
         if version >= Version(1, 0, 0):
             raise ValueError("The version must be < 1.0.0")
 
         super().__init__(version)
 
         self.field_types = (
             str,
@@ -378,15 +375,14 @@
             raise ValueError(f"{version} is not specified for this class.")
 
         match_pattern = cls.pattern.search(matchline, pos=pos)
 
         class_dict = META_LINE[version]
 
         if match_pattern is not None:
-
             (
                 attribute,
                 value_str,
                 measure_str,
                 time_in_beats_str,
             ) = match_pattern.groups()
 
@@ -677,15 +673,14 @@
         modifier: int,
         octave: int,
         onset: int,
         offset: int,
         velocity: int,
         **kwargs,
     ) -> None:
-
         if version not in NOTE_LINE:
             raise ValueError(
                 f"Unknown version {version}!. "
                 f"Supported versions are {list(NOTE_LINE.keys())}"
             )
 
         step, alter, octave = ensure_pitch_spelling_format(note_name, modifier, octave)
@@ -716,29 +711,27 @@
 
         self.NoteName = step
         self.Modifier = alter
         self.Octave = octave
         self.AdjOffset = offset
 
         if "adj_offset" in kwargs:
-
             self.AdjOffset = kwargs["adj_offset"]
 
     @property
     def AdjDuration(self) -> float:
         return self.AdjOffset - self.Onset
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         pos: int = 0,
         version: Version = LAST_VERSION,
     ) -> MatchNote:
-
         if version >= Version(1, 0, 0):
             raise ValueError(f"{version} >= Version(1, 0, 0)")
 
         kwargs = get_kwargs_from_matchline(
             matchline=matchline,
             pattern=NOTE_LINE[version]["pattern"],
             field_names=NOTE_LINE[version]["field_names"],
@@ -756,28 +749,26 @@
 class MatchSnoteNote(BaseSnoteNoteLine):
     def __init__(
         self,
         version: Version,
         snote: MatchSnote,
         note: MatchNote,
     ) -> None:
-
         super().__init__(
             version=version,
             snote=snote,
             note=note,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LAST_VERSION,
     ) -> MatchSnoteNote:
-
         if version >= Version(1, 0, 0):
             raise ValueError(f"{version} >= Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             snote_class=MatchSnote,
             note_class=MatchNote,
@@ -785,27 +776,25 @@
         )
 
         return cls(**kwargs)
 
 
 class MatchSnoteDeletion(BaseDeletionLine):
     def __init__(self, version: Version, snote: MatchSnote) -> None:
-
         super().__init__(
             version=version,
             snote=snote,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LAST_VERSION,
     ) -> MatchSnoteDeletion:
-
         if version >= Version(1, 0, 0):
             raise ValueError(f"{version} >= Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             snote_class=MatchSnote,
             version=version,
@@ -830,59 +819,54 @@
     def __init__(self, version: Version, snote: MatchSnote) -> None:
         super().__init__(version=version, snote=snote)
         self.pattern = re.compile(rf"{self.snote.pattern.pattern}-no_played_note\.")
 
 
 class MatchInsertionNote(BaseInsertionLine):
     def __init__(self, version: Version, note: MatchNote) -> None:
-
         super().__init__(
             version=version,
             note=note,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LAST_VERSION,
     ) -> MatchInsertionNote:
-
         if version >= Version(1, 0, 0):
             raise ValueError(f"{version} >= Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             note_class=MatchNote,
             version=version,
         )
 
         return cls(**kwargs)
 
 
 class MatchHammerBounceNote(MatchInsertionNote):
-
     out_pattern = "hammer_bounce-{NoteLine}"
 
     def __init__(self, version: Version, note: MatchNote) -> None:
         super().__init__(version=version, note=note)
         self.pattern = re.compile(f"hammer_bounce-{self.note.pattern.pattern}")
 
 
 class MatchTrailingPlayedNote(MatchInsertionNote):
-
     out_pattern = "trailing_played_note-{NoteLine}"
 
     def __init__(self, version: Version, note: MatchNote) -> None:
         super().__init__(version=version, note=note)
         self.pattern = re.compile(f"trailing_played_note-{self.note.pattern.pattern}")
 
 
 class MatchTrillNote(BaseOrnamentLine):
-
     out_pattern = "trill({Anchor})-{NoteLine}"
     ornament_pattern: re.Pattern = re.compile(r"trill\((?P<Anchor>[^\)]*)\)-")
 
     def __init__(
         self,
         version: Version,
         anchor: str,
@@ -896,15 +880,14 @@
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LAST_VERSION,
     ) -> MatchTrillNote:
-
         if version >= Version(1, 0, 0):
             raise ValueError(f"{version} >= Version(1, 0, 0)")
 
         anchor_pattern = cls.ornament_pattern.search(matchline)
 
         if anchor_pattern is None:
             raise MatchError("")
@@ -920,29 +903,27 @@
 class MatchSustainPedal(BaseSustainPedalLine):
     def __init__(
         self,
         version: Version,
         time: int,
         value: int,
     ) -> None:
-
         super().__init__(
             version=version,
             time=time,
             value=value,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LAST_VERSION,
         pos: int = 0,
     ) -> MatchSustainPedal:
-
         if version >= Version(1, 0, 0):
             raise ValueError(f"{version} less than 1.0.0")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             version=version,
             pos=pos,
@@ -957,29 +938,27 @@
 class MatchSoftPedal(BaseSoftPedalLine):
     def __init__(
         self,
         version: Version,
         time: int,
         value: int,
     ) -> None:
-
         super().__init__(
             version=version,
             time=time,
             value=value,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LAST_VERSION,
         pos: int = 0,
     ) -> MatchSoftPedal:
-
         if version >= Version(1, 0, 0):
             raise ValueError(f"{version} should be less than 1.0.0")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             version=version,
             pos=pos,
@@ -1021,15 +1000,14 @@
     if matchline.startswith("info"):
         return parse(MatchInfo)
 
     if line.startswith("meta"):
         return parse(MatchMeta)
 
     if line.startswith("snote"):
-
         for mlt in [
             MatchSnoteNote,
             MatchSnoteDeletion,
             MatchSnoteTrailingScore,
             MatchSnoteNoPlayedNote,
         ]:
             matchline = parse(mlt)
```

### Comparing `partitura-1.3.0/partitura/io/matchlines_v1.py` & `partitura-1.3.1/partitura/io/matchlines_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,14 @@
         self,
         version: Version,
         attribute: str,
         value: Any,
         value_type: type,
         format_fun: Callable[Any, str],
     ) -> None:
-
         if version < Version(1, 0, 0):
             raise ValueError("The version must be >= 1.0.0")
 
         super().__init__(
             version=version,
             attribute=attribute,
             value=value,
@@ -191,15 +190,14 @@
         else:
             raise MatchError("Input match line does not fit the expected pattern.")
 
     @classmethod
     def from_instance(
         cls, instance: BaseInfoLine, version: Version = LATEST_VERSION
     ) -> MatchInfo:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseInfoLine):
             raise ValueError("`instance` needs to be a subclass of `BaseInfoLine`")
 
         class_dict = INFO_LINE[version]
@@ -246,15 +244,14 @@
 
 SCOREPROP_ATTRIBUTE_EQUIVALENCES = dict(
     beatSubdivision="beatSubDivision",
 )
 
 
 class MatchScoreProp(MatchLine):
-
     field_names = (
         "Attribute",
         "Value",
         "Measure",
         "Beat",
         "Offset",
         "TimeInBeats",
@@ -281,15 +278,14 @@
         value_type: type,
         format_fun: Callable[Any, str],
         measure: int,
         beat: int,
         offset: FractionalSymbolicDuration,
         time_in_beats: float,
     ) -> None:
-
         if version < Version(1, 0, 0):
             raise ValueError("The version must be >= 1.0.0")
 
         super().__init__(version)
 
         self.field_types = (
             str,
@@ -347,15 +343,14 @@
             raise ValueError(f"{version} is not specified for this class.")
 
         match_pattern = cls.pattern.search(matchline, pos=pos)
 
         class_dict = SCOREPROP_LINE[version]
 
         if match_pattern is not None:
-
             (
                 attribute,
                 value_str,
                 measure_str,
                 beat_str,
                 offset_str,
                 time_in_beats_str,
@@ -397,15 +392,14 @@
         instance: MatchLine,
         version: Version = LATEST_VERSION,
         measure: Optional[int] = None,
         beat: Optional[int] = None,
         offset: Optional[FractionalSymbolicDuration] = None,
         time_in_beats: Optional[float] = None,
     ) -> MatchScoreProp:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, MatchLine):
             raise ValueError("`instance` needs to be a subclass of `MatchLine`")
 
         # ensure that at least the basic attributes are in the field names of the match line
@@ -507,15 +501,14 @@
         version: Version,
         start_in_beats_unfolded: float,
         end_in_beats_unfolded: float,
         start_in_beats_original: float,
         end_in_beats_original: float,
         repeat_end_type: List[str],
     ) -> None:
-
         if version not in SECTION_LINE:
             raise ValueError(
                 f"Unknown version {version}!. "
                 f"Supported versions are {list(SECTION_LINE.keys())}"
             )
         super().__init__(version)
 
@@ -545,15 +538,14 @@
                 f"Supported versions are {list(SECTION_LINE.keys())}"
             )
 
         match_pattern = cls.pattern.search(matchline, pos=pos)
         class_dict = SECTION_LINE[version]
 
         if match_pattern is not None:
-
             kwargs = dict(
                 [
                     (to_snake_case(fn), class_dict[fn][0](match_pattern.group(fn)))
                     for fn in cls.field_names
                 ]
             )
 
@@ -584,15 +576,14 @@
         version: Version,
         measure: int,
         beat: int,
         offset: FractionalSymbolicDuration,
         onset_in_beats: float,
         annotation_type: List[str],
     ) -> None:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         super().__init__(
             version=version,
             measure=measure,
             beat=beat,
@@ -609,15 +600,14 @@
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         pos: int = 0,
         version: Version = LATEST_VERSION,
     ) -> MatchStime:
-
         if version not in STIME_LINE:
             raise ValueError(
                 f"Unknown version {version}!. "
                 f"Supported versions are {list(STIME_LINE.keys())}"
             )
 
         kwargs = get_kwargs_from_matchline(
@@ -643,15 +633,14 @@
 
 class MatchPtime(BasePtimeLine):
     def __init__(
         self,
         version: Version,
         onsets: List[int],
     ) -> None:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         super().__init__(
             version=version,
             onsets=onsets,
         )
@@ -664,15 +653,14 @@
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         pos: int = 0,
         version: Version = LATEST_VERSION,
     ) -> MatchStime:
-
         if version not in PTIME_LINE:
             raise ValueError(
                 f"Unknown version {version}!. "
                 f"Supported versions are {list(STIME_LINE.keys())}"
             )
 
         kwargs = get_kwargs_from_matchline(
@@ -686,15 +674,14 @@
         if kwargs is None:
             raise MatchError("Input match line does not fit the expected pattern.")
 
         return cls(version=version, **kwargs)
 
 
 class MatchSnote(BaseSnoteLine):
-
     format_fun = dict(
         Anchor=format_string,
         NoteName=lambda x: str(x.upper()),
         Modifier=format_accidental_old,
         Octave=format_int,
         Measure=format_int,
         Beat=format_int,
@@ -716,15 +703,14 @@
         beat: int,
         offset: FractionalSymbolicDuration,
         duration: FractionalSymbolicDuration,
         onset_in_beats: float,
         offset_in_beats: float,
         score_attributes_list: List[str],
     ) -> None:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
         super().__init__(
             version=version,
             anchor=anchor,
             note_name=note_name,
             modifier=modifier,
@@ -812,15 +798,14 @@
         "Channel": (interpret_as_int, format_int, int),
         "Track": (interpret_as_int, format_int, int),
     }
 }
 
 
 class MatchNote(BaseNoteLine):
-
     field_names = (
         "Id",
         "MidiPitch",
         "Onset",
         "Offset",
         "Velocity",
         "Channel",
@@ -848,15 +833,14 @@
         midi_pitch: int,
         onset: int,
         offset: int,
         velocity: int,
         channel: int,
         track: int,
     ) -> None:
-
         if version not in NOTE_LINE:
             raise ValueError(
                 f"Unknown version {version}!. "
                 f"Supported versions are {list(NOTE_LINE.keys())}"
             )
 
         super().__init__(
@@ -879,15 +863,14 @@
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         pos: int = 0,
         version: Version = LATEST_VERSION,
     ) -> MatchNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         kwargs = get_kwargs_from_matchline(
             matchline=matchline,
             pattern=cls.pattern,
             field_names=cls.field_names,
@@ -903,23 +886,21 @@
 
     @classmethod
     def from_instance(
         cls,
         instance: BaseNoteLine,
         version: Version = LATEST_VERSION,
     ) -> MatchNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseNoteLine):
             raise ValueError("`instance` needs to be a subclass of `BaseNoteLine`")
 
         if instance.version < Version(1, 0, 0):
-
             return cls(
                 version=version,
                 id=instance.Id,
                 midi_pitch=instance.MidiPitch,
                 onset=int(np.round(instance.Onset)),
                 offset=int(np.round(instance.Offset)),
                 velocity=instance.Velocity,
@@ -943,15 +924,14 @@
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LATEST_VERSION,
     ) -> MatchSnoteNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             stime_class=MatchStime,
             ptime_class=MatchPtime,
@@ -964,28 +944,26 @@
 class MatchSnoteNote(BaseSnoteNoteLine):
     def __init__(
         self,
         version: Version,
         snote: BaseSnoteLine,
         note: BaseNoteLine,
     ) -> None:
-
         super().__init__(
             version=version,
             snote=snote,
             note=note,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LATEST_VERSION,
     ) -> MatchSnoteNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             snote_class=MatchSnote,
             note_class=MatchNote,
@@ -994,15 +972,14 @@
 
         return cls(**kwargs)
 
     @classmethod
     def from_instance(
         cls, instance: BaseSnoteNoteLine, version: Version
     ) -> MatchSnoteNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseSnoteNoteLine):
             raise ValueError("`instance` needs to be a subclass of `BaseSnoteNoteLine`")
 
         return cls(
@@ -1010,27 +987,25 @@
             snote=MatchSnote.from_instance(instance.snote, version=version),
             note=MatchNote.from_instance(instance.note, version=version),
         )
 
 
 class MatchSnoteDeletion(BaseDeletionLine):
     def __init__(self, version: Version, snote: MatchSnote) -> None:
-
         super().__init__(
             version=version,
             snote=snote,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LATEST_VERSION,
     ) -> MatchSnoteDeletion:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             snote_class=MatchSnote,
             version=version,
@@ -1038,42 +1013,39 @@
 
         return cls(**kwargs)
 
     @classmethod
     def from_instance(
         cls, instance: BaseDeletionLine, version: Version
     ) -> MatchSnoteNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseDeletionLine):
             raise ValueError("`instance` needs to be a subclass of `BaseDeletionLine`")
 
         return cls(
             version=version,
             snote=MatchSnote.from_instance(instance.snote, version=version),
         )
 
 
 class MatchInsertionNote(BaseInsertionLine):
     def __init__(self, version: Version, note: MatchNote) -> None:
-
         super().__init__(
             version=version,
             note=note,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LATEST_VERSION,
     ) -> MatchInsertionNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             note_class=MatchNote,
             version=version,
@@ -1081,29 +1053,27 @@
 
         return cls(**kwargs)
 
     @classmethod
     def from_instance(
         cls, instance: BaseInsertionLine, version: Version
     ) -> MatchInsertionNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseInsertionLine):
             raise ValueError("`instance` needs to be a subclass of `BaseInsertionLine`")
 
         return cls(
             version=version,
             note=MatchNote.from_instance(instance.note, version=version),
         )
 
 
 class MatchOrnamentNote(BaseOrnamentLine):
-
     field_names = (
         "Anchor",
         "OrnamentType",
     )
     field_types = (
         str,
         list,
@@ -1138,15 +1108,14 @@
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LATEST_VERSION,
     ) -> MatchOrnamentNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         anchor_pattern = cls.ornament_pattern.search(matchline)
 
         if anchor_pattern is None:
             raise MatchError("Input match line does not fit the expected pattern.")
@@ -1159,15 +1128,14 @@
             ornament_type=interpret_as_list(anchor_pattern.group("OrnamentType")),
         )
 
     @classmethod
     def from_instance(
         cls, instance: BaseOrnamentLine, version: Version
     ) -> MatchOrnamentNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseOrnamentLine):
             raise ValueError("`instance` needs to be a subclass of `BaseOrnamentLine`")
 
         return cls(
@@ -1183,29 +1151,27 @@
 class MatchSustainPedal(BaseSustainPedalLine):
     def __init__(
         self,
         version: Version,
         time: int,
         value: int,
     ) -> None:
-
         super().__init__(
             version=version,
             time=time,
             value=value,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LATEST_VERSION,
         pos: int = 0,
     ) -> MatchSustainPedal:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             version=version,
             pos=pos,
@@ -1216,15 +1182,14 @@
 
         return cls(**kwargs)
 
     @classmethod
     def from_instance(
         cls, instance: BaseSustainPedalLine, version: Version
     ) -> MatchOrnamentNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseSustainPedalLine):
             raise ValueError(
                 "`instance` needs to be a subclass of `BaseSustainPedalLine`"
             )
@@ -1239,29 +1204,27 @@
 class MatchSoftPedal(BaseSoftPedalLine):
     def __init__(
         self,
         version: Version,
         time: int,
         value: int,
     ) -> None:
-
         super().__init__(
             version=version,
             time=time,
             value=value,
         )
 
     @classmethod
     def from_matchline(
         cls,
         matchline: str,
         version: Version = LATEST_VERSION,
         pos: int = 0,
     ) -> MatchSoftPedal:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         kwargs = cls.prepare_kwargs_from_matchline(
             matchline=matchline,
             version=version,
             pos=pos,
@@ -1274,15 +1237,14 @@
 
     @classmethod
     def from_instance(
         cls,
         instance: BaseSoftPedalLine,
         version: Version,
     ) -> MatchOrnamentNote:
-
         if version < Version(1, 0, 0):
             raise ValueError(f"{version} < Version(1, 0, 0)")
 
         if not isinstance(instance, BaseSoftPedalLine):
             raise ValueError("`instance` needs to be a subclass of `BaseSoftPedalLine`")
 
         return cls(
@@ -1340,15 +1302,14 @@
     attribute: str,
     value: Any,
     measure: int,
     beat: int,
     offset: FractionalSymbolicDuration,
     time_in_beats: float,
 ) -> MatchScoreProp:
-
     class_dict = SCOREPROP_LINE[version]
 
     _, format_fun, dtype = class_dict[attribute]
 
     ml = MatchScoreProp(
         version=version,
         attribute=attribute,
@@ -1368,15 +1329,14 @@
     version: Version,
     start_in_beats_unfolded: float,
     end_in_beats_unfolded: float,
     start_in_beats_original: float,
     end_in_beats_original: float,
     repeat_end_type: Union[str, List[str]],
 ) -> MatchSection:
-
     ml = MatchSection(
         version=version,
         start_in_beats_unfolded=start_in_beats_unfolded,
         start_in_beats_original=start_in_beats_original,
         end_in_beats_unfolded=end_in_beats_unfolded,
         end_in_beats_original=end_in_beats_original,
         repeat_end_type=[repeat_end_type]
@@ -1402,26 +1362,24 @@
     MatchLine
          A new matchline with the equivalent of the input matchline in
          the specified version.
     """
     from partitura.io.matchlines_v0 import MatchMeta
 
     if isinstance(matchline, BaseInfoLine):
-
         if (
             matchline.Attribute in INFO_LINE[version]
             or matchline.Attribute in INFO_ATTRIBUTE_EQUIVALENCES
         ):
             return MatchInfo.from_instance(instance=matchline, version=version)
 
         if (
             matchline.Attribute in SCOREPROP_LINE[version]
             or matchline.Attribute in SCOREPROP_ATTRIBUTE_EQUIVALENCES
         ):
-
             return MatchScoreProp.from_instance(instance=matchline, version=version)
 
     if isinstance(matchline, MatchMeta):
         return MatchScoreProp.from_instance(instance=matchline, version=version)
 
     if isinstance(matchline, BaseSnoteNoteLine):
         return MatchSnoteNote.from_instance(instance=matchline, version=version)
```

### Comparing `partitura-1.3.0/partitura/io/musescore.py` & `partitura-1.3.1/partitura/io/musescore.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         result = shutil.which("mscore3")
 
     if result is None:
         if platform.system() == "Linux":
             pass
 
         elif platform.system() == "Darwin":
-
             result = shutil.which("/Applications/MuseScore 3.app/Contents/MacOS/mscore")
 
         elif platform.system() == "Windows":
             result = shutil.which(r"C:\Program Files\MuseScore 3\bin\MuseScore3.exe")
 
     return result
 
@@ -104,34 +103,30 @@
         One or more part or partgroup objects
 
     """
 
     mscore_exec = find_musescore3()
 
     if not mscore_exec:
-
         raise MuseScoreNotFoundException()
 
     xml_fh = os.path.splitext(os.path.basename(filename))[0] + ".musicxml"
 
     cmd = [mscore_exec, "-o", xml_fh, filename]
 
     try:
-
         ps = subprocess.run(cmd, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
 
         if ps.returncode != 0:
-
             raise FileImportException(
                 (
                     "Command {} failed with code {}. MuseScore " "error messages:\n {}"
                 ).format(cmd, ps.returncode, ps.stderr.decode("UTF-8"))
             )
     except FileNotFoundError as f:
-
         raise FileImportException(
             'Executing "{}" returned  {}.'.format(" ".join(cmd), f)
         )
 
     score = load_musicxml(
         filename=xml_fh,
         validate=validate,
@@ -171,19 +166,17 @@
     -------
     out : Optional[PathLike]
        Path to the output generated image (or None if no image was generated)
     """
     mscore_exec = find_musescore3()
 
     if not mscore_exec:
-
         return None
 
     if fmt not in ("png", "pdf"):
-
         warnings.warn("warning: unsupported output format")
         return None
 
     # with NamedTemporaryFile(suffix='.musicxml') as xml_fh, \
     #      NamedTemporaryFile(suffix='.{}'.format(fmt)) as img_fh:
     with TemporaryDirectory() as tmpdir:
         xml_fh = Path(tmpdir) / "score.musicxml"
@@ -198,15 +191,14 @@
             "-r",
             "{}".format(int(dpi)),
             "-o",
             os.fspath(img_fh),
             os.fspath(xml_fh),
         ]
         try:
-
             ps = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
             if ps.returncode != 0:
                 warnings.warn(
                     "Command {} failed with code {}; stdout: {}; stderr: {}".format(
                         cmd,
                         ps.returncode,
@@ -215,28 +207,26 @@
                     ),
                     SyntaxWarning,
                     stacklevel=2,
                 )
                 return None
 
         except FileNotFoundError as f:
-
             warnings.warn(
                 'Executing "{}" returned  {}.'.format(" ".join(cmd), f),
                 ImportWarning,
                 stacklevel=2,
             )
             return None
 
         # LOGGER.error('Command "{}" returned with code {}; stdout: {}; stderr: {}'
         #              .format(' '.join(cmd), ps.returncode, ps.stdout.decode('UTF-8'),
         #                      ps.stderr.decode('UTF-8')))
 
         if fmt == "png":
-
             if PIL_EXISTS:
                 # get all generated image files
                 img_files = glob.glob(
                     os.path.join(img_fh.parent, img_fh.stem + "-*.png")
                 )
                 concatenate_images(
                     filenames=img_files,
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/__init__.py` & `partitura-1.3.1/partitura/musicanalysis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     "make_note_features",
     "make_rest_features",
     "encode_performance",
     "decode_performance",
     "compute_note_array",
     "full_note_array",
     "make_performance_features",
-    "note_array_to_score"
+    "note_array_to_score",
 ]
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/key_identification.py` & `partitura-1.3.1/partitura/musicanalysis/key_identification.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/musicanalysis/meter.py` & `partitura-1.3.1/partitura/musicanalysis/meter.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/partitura/musicanalysis/note_array_to_score.py` & `partitura-1.3.1/partitura/musicanalysis/note_array_to_score.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,87 +1,110 @@
 from partitura.score import ScoreLike, Part
-from partitura.utils import (estimate_symbolic_duration, estimate_clef_properties, key_name_to_fifths_mode, fifths_mode_to_key_name)
+from partitura.utils import (
+    estimate_symbolic_duration,
+    estimate_clef_properties,
+    key_name_to_fifths_mode,
+    fifths_mode_to_key_name,
+)
 import warnings
 import numpy as np
 from typing import Union
 import numpy.lib.recfunctions as rfn
 from fractions import Fraction
 import partitura.musicanalysis as analysis
 import partitura.score as score
 
 
 def create_divs_from_beats(note_array: np.ndarray):
     """
     Append onset_div and duration_div fields to the note array.
-    Assumes beats are in uniform units across the whole array 
+    Assumes beats are in uniform units across the whole array
     (no time signature change that modifies beat unit, e.g., 4/4 to 6/8).
 
     This function may result in an error if time signature changes that affect the ratio of beat/div are present.
     Parameters
     ----------
     note_array: np.ndarray
-        The note array to which the divs fields will be added. 
+        The note array to which the divs fields will be added.
         Normally only beat onset and duration are provided.
 
     Returns
     -------
     note_array: np.ndarray
         The note array with the divs fields added.
     divs: int
         the divs per beat
-    
+
     """
-    duration_fractions = [Fraction(float(ix)).limit_denominator(256) for ix in note_array["duration_beat"]]
-    onset_fractions = [Fraction(float(ix)).limit_denominator(256) for ix in note_array["onset_beat"]]
+    duration_fractions = [
+        Fraction(float(ix)).limit_denominator(256) for ix in note_array["duration_beat"]
+    ]
+    onset_fractions = [
+        Fraction(float(ix)).limit_denominator(256) for ix in note_array["onset_beat"]
+    ]
     divs = np.lcm.reduce(
-        [Fraction(float(ix)).limit_denominator(256).denominator for ix in np.unique(note_array["duration_beat"])])
-    onset_divs = list(map(lambda r: int(divs * r.numerator / r.denominator), onset_fractions))
+        [
+            Fraction(float(ix)).limit_denominator(256).denominator
+            for ix in np.unique(note_array["duration_beat"])
+        ]
+    )
+    onset_divs = list(
+        map(lambda r: int(divs * r.numerator / r.denominator), onset_fractions)
+    )
     min_onset_div = min(onset_divs)
     if min_onset_div < 0:
         onset_divs = list(map(lambda x: x - min_onset_div, onset_divs))
-    duration_divs = list(map(lambda r: int(divs * r.numerator / r.denominator), duration_fractions))
-    na_divs = np.array(list(zip(onset_divs, duration_divs)), dtype=[("onset_div", int), ("duration_div", int)])
+    duration_divs = list(
+        map(lambda r: int(divs * r.numerator / r.denominator), duration_fractions)
+    )
+    na_divs = np.array(
+        list(zip(onset_divs, duration_divs)),
+        dtype=[("onset_div", int), ("duration_div", int)],
+    )
     return rfn.merge_arrays((note_array, na_divs), flatten=True, usemask=False), divs
 
 
 def create_beats_from_divs(note_array: np.ndarray, divs: int):
     """
     Append onset_beats and duration_beasts fields to the note array.
     Returns beats in quarters.
 
     Parameters
     ----------
     note_array: np.ndarray
-        The note array to which the divs fields will be added. 
+        The note array to which the divs fields will be added.
         Normally only beat onset and duration are provided.
     divs: int
         Divs/ticks per quarter note.
 
     Returns
     -------
     note_array: np.ndarray
         The note array with the divs fields added.
-    
+
     """
-    onset_beats = list(note_array["onset_div"]/divs)
-    duration_beats = list(note_array["duration_div"]/divs)
-    na_beats = np.array(list(zip(onset_beats, duration_beats)), dtype=[("onset_beat", float), ("duration_beat", float)])
+    onset_beats = list(note_array["onset_div"] / divs)
+    duration_beats = list(note_array["duration_div"] / divs)
+    na_beats = np.array(
+        list(zip(onset_beats, duration_beats)),
+        dtype=[("onset_beat", float), ("duration_beat", float)],
+    )
     return rfn.merge_arrays((note_array, na_beats), flatten=True, usemask=False)
 
 
 def create_part(
-        ticks: int,
-        note_array: np.ndarray,
-        key_sigs: list = None,
-        time_sigs: list = None,
-        part_id: str = None,
-        part_name: str = None,
-        sanitize: bool = True,
-        anacrusis_divs: int = 0,
-        barebones: bool = False,
+    ticks: int,
+    note_array: np.ndarray,
+    key_sigs: list = None,
+    time_sigs: list = None,
+    part_id: str = None,
+    part_name: str = None,
+    sanitize: bool = True,
+    anacrusis_divs: int = 0,
+    barebones: bool = False,
 ):
     """
     Create a part from a note array and a list of key signatures.
 
     Parameters
     ----------
     ticks: int
@@ -105,34 +128,34 @@
 
     Returns
     -------
     part : partitura.score.Part
         The part created from the note array and key signatures.
     """
 
-
     warnings.warn("create_part", stacklevel=2)
 
-    part = Part(part_id, part_name=part_name, )
+    part = Part(
+        part_id,
+        part_name=part_name,
+    )
     part.set_quarter_duration(0, ticks)
 
-    clef = score.Clef(
-        staff=1, **estimate_clef_properties(note_array["pitch"])
-    )
+    clef = score.Clef(staff=1, **estimate_clef_properties(note_array["pitch"]))
     part.add(clef, 0)
 
     # key sig
     if key_sigs is not None:
         for t_start, name, t_end in key_sigs:
             fifths, mode = key_name_to_fifths_mode(name)
             t_start, t_end = int(t_start), int(t_end)
             part.add(score.KeySignature(fifths, mode), t_start, t_end)
     else:
         warnings.warn("No key signatures added")
-        
+
     # time sig
     if time_sigs is not None:
         for ts_start, num, den, ts_end in time_sigs:
             time_sig = score.TimeSignature(num.item(), den.item())
             part.add(time_sig, ts_start, ts_end)
     else:
         warnings.warn("No time signatures added")
@@ -145,15 +168,15 @@
         if n["duration_div"] > 0:
             note = score.Note(
                 step=n["step"],
                 octave=n["octave"],
                 alter=n["alter"],
                 voice=int(n["voice"] or 0),
                 id=n["id"],
-                symbolic_duration=estimate_symbolic_duration(n["duration_div"], ticks)
+                symbolic_duration=estimate_symbolic_duration(n["duration_div"], ticks),
             )
         else:
             note = score.GraceNote(
                 grace_type="appoggiatura",
                 step=n["step"],
                 octave=n["octave"],
                 alter=n["alter"],
@@ -186,25 +209,26 @@
         score.sanitize_part(part)
 
     warnings.warn("done create_part", stacklevel=2)
     return part
 
 
 def note_array_to_score(
-        note_array: Union[np.ndarray, list],
-        name_id: str = "",
-        divs: int = None,
-        key_sigs: list = None,
-        time_sigs: list = None,
-        part_name: str = "",
-        assign_note_ids: bool = True,
-        estimate_key: bool = False,
-        estimate_time: bool = False,
-        sanitize: bool = True,
-        return_part: bool = False) -> ScoreLike:
+    note_array: Union[np.ndarray, list],
+    name_id: str = "",
+    divs: int = None,
+    key_sigs: list = None,
+    time_sigs: list = None,
+    part_name: str = "",
+    assign_note_ids: bool = True,
+    estimate_key: bool = False,
+    estimate_time: bool = False,
+    sanitize: bool = True,
+    return_part: bool = False,
+) -> ScoreLike:
     """
     A generic function to transform an enriched note_array to part or Score.
 
     The function can be used for many different occasions, i.e. part_from_graph, part from note_array, part from midi score import, etc.
     This function requires a note array that contains time signatures and key signatures (optional - can also estimate it automatically).
     Note array should contain the following fields:
     - onset_div or onset_beat
@@ -259,15 +283,15 @@
         - pitch
         - ts_beats (optional)
         - ts_beat_type (optional)
         - key_mode(optional)
         - key_fifths(optional)
         - id (optional)
     divs : int (optional)
-        Divs/ticks per quarter note. 
+        Divs/ticks per quarter note.
         If not given, it is estimated assuming a beats in quarters.
     key_sigs: list (optional)
         A list of key signatures. Each key signature is a tuple of the form (onset, key_name, offset).
         Overridden by note_array fields "key_mode" and "key_fifths".
         Overrides estimate_key.
     time_sigs: list (optional)
         A list of time signatures. Each time signature is a tuple of the form (onset, ts_num, ts_den, offset).
@@ -288,18 +312,26 @@
     -------
     part or score : Part or Score
         a Part object or a Score object, depending on return_part.
     """
 
     if isinstance(note_array, list):
         parts = [
-            note_array_to_score(note_array=x, name_id=str(i), assign_note_ids=assign_note_ids,
-                                return_part=True, divs=divs, estimate_key=estimate_key, sanitize=sanitize,
-                                part_name=name_id+"_P"+str(i)) for
-            i, x in enumerate(note_array)]
+            note_array_to_score(
+                note_array=x,
+                name_id=str(i),
+                assign_note_ids=assign_note_ids,
+                return_part=True,
+                divs=divs,
+                estimate_key=estimate_key,
+                sanitize=sanitize,
+                part_name=name_id + "_P" + str(i),
+            )
+            for i, x in enumerate(note_array)
+        ]
         return score.Score(partlist=parts)
 
     # Input validation
     if not isinstance(note_array, np.ndarray):
         raise TypeError("The note array does not have the correct format.")
 
     if len(note_array) == 0:
@@ -307,216 +339,239 @@
 
     dtypes = note_array.dtype.names
 
     ts_case = ["ts_beats", "ts_beat_type"]
     ks_case = ["key_fifths", "key_mode"]
 
     case1 = ["onset_beat", "duration_beat", "pitch"]
-    case1_ex = ["onset_div", "duration_div"] 
+    case1_ex = ["onset_div", "duration_div"]
     case2 = ["onset_div", "duration_div", "pitch"]
-    case2_ex = ["onset_beat", "duration_beat"] 
+    case2_ex = ["onset_beat", "duration_beat"]
     # case3 = ["onset_div", "duration_div", "onset_beat", "duration_beat", "pitch"]
 
     if not (all([x in dtypes for x in case1]) or all([x in dtypes for x in case2])):
         raise ValueError("not all necessary note array fields are available")
-    
+
     # sort the array
     onset_time = "onset_div"
     duration_time = "duration_div"
     if all([x not in dtypes for x in case1_ex]):
         onset_time = "onset_beat"
         duration_time = "duration_beat"
 
     # Order Lexicographically
-    sort_idx = np.lexsort((note_array[duration_time], note_array["pitch"], note_array[onset_time]))
+    sort_idx = np.lexsort(
+        (note_array[duration_time], note_array["pitch"], note_array[onset_time])
+    )
     note_array = note_array[sort_idx]
 
     # case 1, estimate divs
     if all([x in dtypes for x in case1] and [x not in dtypes for x in case1_ex]):
         # estimate onset_divs and duration_divs, assumes all beat times as quarters
         note_array, divs_ = create_divs_from_beats(note_array)
         if divs is not None and divs != divs_:
             raise ValueError("estimated divs don't correspond to input divs")
-        else: 
+        else:
             divs = divs_
 
-        # case 1: convert key sig times to divs 
+        # case 1: convert key sig times to divs
         if key_sigs is not None:
             key_sigs = np.array(key_sigs)
             if key_sigs.shape[1] == 2:
-                key_sigs[:,0] = (key_sigs[:,0] / divs).astype(int)
+                key_sigs[:, 0] = (key_sigs[:, 0] / divs).astype(int)
             elif key_sigs.shape[1] == 3:
-                key_sigs[:,0] = (key_sigs[:,0] / divs).astype(int)
-                key_sigs[:,2] = (key_sigs[:,2] / divs).astype(int)
+                key_sigs[:, 0] = (key_sigs[:, 0] / divs).astype(int)
+                key_sigs[:, 2] = (key_sigs[:, 2] / divs).astype(int)
             else:
                 raise ValueError("key_sigs is given in a wrong format")
-            
-        # case 1: convert time sig times to divs 
+
+        # case 1: convert time sig times to divs
         if time_sigs is not None:
             time_sigs = np.array(time_sigs)
             if time_sigs.shape[1] == 3:
-                time_sigs[:,0] = (time_sigs[:,0] / divs).astype(int)
+                time_sigs[:, 0] = (time_sigs[:, 0] / divs).astype(int)
             elif time_sigs.shape[1] == 4:
-                time_sigs[:,0] = (time_sigs[:,0] / divs).astype(int)
-                time_sigs[:,3] = (time_sigs[:,3] / divs).astype(int)
+                time_sigs[:, 0] = (time_sigs[:, 0] / divs).astype(int)
+                time_sigs[:, 3] = (time_sigs[:, 3] / divs).astype(int)
             else:
                 raise ValueError("time_sigs is given in a wrong format")
 
     # case 2, estimate beats
     if all([x in dtypes for x in case2] and [x not in dtypes for x in case2_ex]):
         # estimate onset_beats and duration_beats in quarters
-        if divs is None :
+        if divs is None:
             raise ValueError("Divs/ticks need to be specified")
-        else: 
+        else:
             note_array = create_beats_from_divs(note_array, divs)
 
     if divs is None:
         # find first note with nonzero duration (in case score starts with grace_note).
         for idx, dur in enumerate(note_array["duration_beat"]):
             if dur != 0:
                 break
         if all([x in dtypes for x in ts_case]):
-            divs = int((note_array[idx]["duration_div"] / note_array[idx]["duration_beat"]) /
-                    (4 / note_array[idx]["ts_beat_type"] ))
-        else:    
-            divs = int(note_array[idx]["duration_div"] / note_array[idx]["duration_beat"])
+            divs = int(
+                (note_array[idx]["duration_div"] / note_array[idx]["duration_beat"])
+                / (4 / note_array[idx]["ts_beat_type"])
+            )
+        else:
+            divs = int(
+                note_array[idx]["duration_div"] / note_array[idx]["duration_beat"]
+            )
 
     # Test Note array for negative durations
     if not np.all(note_array["duration_div"] >= 0):
         raise ValueError("Note array contains negative durations.")
     if not np.all(note_array["duration_beat"] >= 0):
         raise ValueError("Note array contains negative durations.")
-    
+
     # Test for negative divs
     if not np.all(note_array["onset_div"] >= 0):
         raise ValueError("Negative divs found in note_array.")
-    
+
     # handle time signatures
-    if all([x in dtypes for x in ts_case]): 
+    if all([x in dtypes for x in ts_case]):
         time_sigs = [[0, note_array[0]["ts_beats"], note_array[0]["ts_beat_type"]]]
         for n in note_array:
-            if n["ts_beats"] != time_sigs[-1][1] or n["ts_beat_type"] != time_sigs[-1][2]:
+            if (
+                n["ts_beats"] != time_sigs[-1][1]
+                or n["ts_beat_type"] != time_sigs[-1][2]
+            ):
                 time_sigs.append([n["onset_div"], n["ts_beats"], n["ts_beat_type"]])
         global_time_sigs = np.array(time_sigs)
     elif time_sigs is not None:
         global_time_sigs = time_sigs
     elif estimate_time:
         global_time_sigs = [[0, 4, 4]]
-    else: 
+    else:
         global_time_sigs = None
 
     if global_time_sigs is not None:
         global_time_sigs = np.array(global_time_sigs)
         if global_time_sigs.shape[1] == 3:
             # for convenience, we add the end times for each time signature
-            ts_end_times = np.r_[global_time_sigs[1:, 0], np.max(note_array["onset_div"]+note_array["duration_div"])]
+            ts_end_times = np.r_[
+                global_time_sigs[1:, 0],
+                np.max(note_array["onset_div"] + note_array["duration_div"]),
+            ]
             global_time_sigs = np.column_stack((global_time_sigs, ts_end_times))
         elif global_time_sigs.shape[1] == 4:
             pass
         else:
             raise ValueError("time_sigs is given in a wrong format")
 
         # make sure there is a time signature from the beginning
         global_time_sigs[0, 0] = 0
-    
-
 
     # Note id creation or re-assignment
     if "id" not in dtypes:
         note_ids = ["{}n{:4d}".format(name_id, i) for i in range(len(note_array))]
-        note_array = rfn.append_fields(note_array, "id", np.array(note_ids, dtype='<U256'))
+        note_array = rfn.append_fields(
+            note_array, "id", np.array(note_ids, dtype="<U256")
+        )
     elif assign_note_ids or np.all(note_array["id"] == note_array["id"][0]):
         note_ids = ["{}n{:4d}".format(name_id, i) for i in range(len(note_array))]
         note_array["id"] = np.array(note_ids)
 
-    
-
     # estimate voice
     if "voice" in dtypes:
         estimate_voice_info = False
         part_voice_list = note_array["voice"]
     else:
         estimate_voice_info = True
         part_voice_list = np.full(len(note_array), np.inf)
 
     if estimate_voice_info:
         warnings.warn("voice estimation", stacklevel=2)
         # TODO: deal with zero duration notes in note_array.
         # Zero duration notes are currently deleted
         estimated_voices = analysis.estimate_voices(note_array)
         assert len(part_voice_list) == len(estimated_voices)
-        for i, (part_voice, voice_est) in enumerate(zip(part_voice_list, estimated_voices)):
+        for i, (part_voice, voice_est) in enumerate(
+            zip(part_voice_list, estimated_voices)
+        ):
             # Not sure if correct.
             if part_voice != np.inf:
                 estimated_voices[i] = part_voice
-        note_array = rfn.append_fields(note_array, "voice", np.array(estimated_voices, dtype=int))
+        note_array = rfn.append_fields(
+            note_array, "voice", np.array(estimated_voices, dtype=int)
+        )
 
     # estimate pitch spelling
-    if not all(x in dtypes for x in ['step', 'alter', 'octave']):
+    if not all(x in dtypes for x in ["step", "alter", "octave"]):
         warnings.warn("pitch spelling")
         spelling_global = analysis.estimate_spelling(note_array)
         note_array = rfn.merge_arrays((note_array, spelling_global), flatten=True)
 
     # handle or estimate key signature
-    if all([x in dtypes for x in ks_case]): 
-        global_key_sigs = [[0, fifths_mode_to_key_name(note_array[0]["ks_fifths"], note_array[0]["ks_mode"])]]
+    if all([x in dtypes for x in ks_case]):
+        global_key_sigs = [
+            [
+                0,
+                fifths_mode_to_key_name(
+                    note_array[0]["ks_fifths"], note_array[0]["ks_mode"]
+                ),
+            ]
+        ]
         for n in note_array:
-            global_key_sigs.append([n["onset_div"], fifths_mode_to_key_name(n["ks_fifths"], n["ks_mode"])])
+            global_key_sigs.append(
+                [n["onset_div"], fifths_mode_to_key_name(n["ks_fifths"], n["ks_mode"])]
+            )
         else:
             global_key_sigs = key_sigs
     elif key_sigs is not None:
         global_key_sigs = key_sigs
     elif estimate_key:
         k_name = analysis.estimate_key(note_array)
         global_key_sigs = [[0, k_name]]
     else:
         global_key_sigs = None
 
     if global_key_sigs is not None:
         global_key_sigs = np.array(global_key_sigs)
         if global_key_sigs.shape[1] == 2:
             # for convenience, we add the end times for each time signature
-            ks_end_times = np.r_[global_key_sigs[1:, 0], np.max(note_array["onset_div"]+note_array["duration_div"])]
+            ks_end_times = np.r_[
+                global_key_sigs[1:, 0],
+                np.max(note_array["onset_div"] + note_array["duration_div"]),
+            ]
             global_key_sigs = np.column_stack((global_key_sigs, ks_end_times))
         elif global_key_sigs.shape[1] == 3:
             pass
         else:
             raise ValueError("key_sigs is given in a wrong format")
-        
+
         # make sure there is a key signature from the beginning
         global_key_sigs[0, 0] = 0
-        
+
     # Steps for dealing with anacrusis measure.
     anacrusis_mask = np.zeros(len(note_array), dtype=bool)
     anacrusis_mask[note_array["onset_beat"] < 0] = True
 
     if np.all(anacrusis_mask == False):
         anacrusis_divs = 0
     else:
         last_neg_beat = np.max(note_array[anacrusis_mask]["onset_beat"])
         last_neg_divs = np.max(note_array[anacrusis_mask]["onset_div"])
-        if all([x in dtypes for x in ts_case]): 
+        if all([x in dtypes for x in ts_case]):
             beat_type = np.max(note_array[anacrusis_mask]["ts_beat_type"])
         else:
             beat_type = 4
         difference_from_zero = (0 - last_neg_beat) * divs * (4 / beat_type)
         anacrusis_divs = int(last_neg_divs + difference_from_zero)
 
-        
-    
     # Create the part
     part = create_part(
         ticks=divs,
         note_array=note_array,
         key_sigs=global_key_sigs,
         time_sigs=global_time_sigs,
         part_id=name_id,
         part_name=part_name,
         sanitize=sanitize,
-        anacrusis_divs=anacrusis_divs
+        anacrusis_divs=anacrusis_divs,
     )
     # Return Part or Score
     if return_part:
         return part
     else:
         return score.Score(partlist=[part], id=name_id)
-
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/note_features.py` & `partitura-1.3.1/partitura/musicanalysis/note_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from partitura.score import ScoreLike
 
 __all__ = [
     "list_note_feats_functions",
     "list_note_feature_functions",
     "print_note_feats_functions",
     "print_note_feature_functions",
-    "make_note_feats", 
+    "make_note_feats",
     "make_note_features",
     "make_rest_feats",
     "make_rest_features",
     "compute_note_array",
     "full_note_array",
 ]
 
@@ -77,15 +77,14 @@
 def make_note_features(
     part: ScoreLike,
     feature_functions: Union[List, str],
     add_idx: bool = False,
     include_empty_features: bool = True,
     force_fixed_size: bool = False,
 ) -> Tuple[np.ndarray, List]:
-
     """Compute the specified feature functions for a part.
 
     The function returns the computed feature functions as a N x M
     array, where N equals `len(part.notes_tied)` and M equals the
     total number of descriptors of all feature functions that occur in
     part.
 
@@ -139,24 +138,37 @@
         raise TypeError(
             "feature_functions variable {} needs to be list or all".format(
                 feature_functions
             )
         )
 
     for bf in feature_functions:
+        # skip time_signature_feature if force_fixed_size is True
+        if force_fixed_size and (
+            bf == "time_signature_feature" or bf == time_signature_feature
+        ):
+            continue
+        # skip metrical_feature if force_fixed_size is True
+        if force_fixed_size and (bf == "metrical_feature" or bf == metrical_feature):
+            continue
+
         if isinstance(bf, str):
             # get function by name from module
             func = getattr(sys.modules[__name__], bf)
         elif isinstance(bf, types.FunctionType):
             func = bf
-        elif force_fixed_size and bf == "time_signature_feature":
-            continue
         else:
             warnings.warn("Ignoring unknown feature function {}".format(bf))
-        bf, bn = func(na, part, include_empty_features=(True if force_fixed_size else include_empty_features))
+        bf, bn = func(
+            na,
+            part,
+            include_empty_features=(
+                True if force_fixed_size else include_empty_features
+            ),
+        )
         # check if the size and number of the feature function are correct
         if bf.size != 0:
             if bf.shape[1] != len(bn):
                 msg = (
                     "number of feature names {} does not equal "
                     "number of feature {}".format(len(bn), bf.shape[1])
                 )
@@ -316,21 +328,22 @@
 make_note_feats = make_note_features
 make_rest_feats = make_rest_features
 list_note_feature_functions = list_note_feats_functions
 print_note_feature_functions = print_note_feats_functions
 
 
 def compute_note_array(
-    part : ScoreLike,
+    part: ScoreLike,
     include_pitch_spelling=False,
     include_key_signature=False,
     include_time_signature=False,
     include_metrical_position=False,
     include_grace_notes=False,
     feature_functions=None,
+    force_fixed_size=False,
 ):
     """
     Create an extended note array from this part.
 
     1) Without arguments this returns a structured array of onsets, offsets,
     pitch, and ID information: equivalent to part.note_array()
 
@@ -372,14 +385,18 @@
         grace note and the grace type "" for non grace notes).
         Default is False
     feature_functions : list or str
         A list of feature functions. Elements of the list can be either
         the functions themselves or the names of a feature function as
         strings (or a mix). The feature functions specified by name are
         looked up in the `featuremixer.featurefunctions` module.
+    force_fixed_size : bool (default: False)
+        If True, the output array uses only features that have a fixed
+        size with no new entries added.
+
 
     Returns:
 
     note_array : structured array
     """
     if isinstance(part, score.Score):
         part = score.merge_parts(part.parts)
@@ -391,20 +408,22 @@
         include_key_signature=include_key_signature,
         include_time_signature=include_time_signature,
         include_metrical_position=include_metrical_position,
         include_grace_notes=include_grace_notes,
     )
 
     if feature_functions is not None:
-        feature_data_struct = make_note_feats(part, feature_functions, add_idx=True)
+        feature_data_struct = make_note_feats(
+            part, feature_functions, add_idx=True, force_fixed_size=force_fixed_size
+        )
         note_array_joined = np.lib.recfunctions.join_by("id", na, feature_data_struct)
         note_array = note_array_joined.data
-        sort_idx = np.lexsort((note_array["duration_div"], 
-                               note_array["pitch"], 
-                               note_array["onset_div"]))
+        sort_idx = np.lexsort(
+            (note_array["duration_div"], note_array["pitch"], note_array["onset_div"])
+        )
         note_array = note_array[sort_idx]
     else:
         note_array = na
     return note_array
 
 
 def full_note_array(part):
@@ -495,15 +514,19 @@
         else {n.id: n for n in part.rests}
     )
     indices = np.nonzero(na["is_grace"])[0]
     for i, index in enumerate(indices):
         grace = grace_notes[i]
         n_grace = np.count_nonzero(grace_notes["onset_beat"] == grace["onset_beat"])
         W[index, 1] = n_grace
-        W[index, 2] = n_grace - sum(1 for _ in notes[grace["id"]].iter_grace_seq()) + 1 if grace["id"] not in (None, 'None', "") else 0
+        W[index, 2] = (
+            n_grace - sum(1 for _ in notes[grace["id"]].iter_grace_seq()) + 1
+            if grace["id"] not in (None, "None", "")
+            else 0
+        )
     return W, feature_names
 
 
 def loudness_direction_feature(na, part, **kwargs):
     """The loudness directions in part.
 
     This function returns a varying number of descriptors, depending
@@ -529,14 +552,15 @@
 
     directions = list(part.iter_all(score.LoudnessDirection, include_subclasses=True))
     if "include_empty_features" in kwargs.keys():
         force_size = kwargs["include_empty_features"]
     else:
         force_size = False
     if force_size:
+
         def to_name(d):
             if isinstance(d, score.ConstantLoudnessDirection):
                 if d.text in constant:
                     return d.text
                 else:
                     return "unknown_constant"
             elif isinstance(d, score.ImpulsiveLoudnessDirection):
@@ -544,26 +568,27 @@
                     return d.text
                 else:
                     return "unknown_impulsive"
             elif isinstance(d, score.IncreasingLoudnessDirection):
                 return "loudness_incr"
             elif isinstance(d, score.DecreasingLoudnessDirection):
                 return "loudness_decr"
+
     else:
+
         def to_name(d):
             if isinstance(d, score.ConstantLoudnessDirection):
                 return d.text
             elif isinstance(d, score.ImpulsiveLoudnessDirection):
                 return d.text
             elif isinstance(d, score.IncreasingLoudnessDirection):
                 return "loudness_incr"
             elif isinstance(d, score.DecreasingLoudnessDirection):
                 return "loudness_decr"
 
-
     feature_by_name = {}
     for d in directions:
         j, bf = feature_by_name.setdefault(
             to_name(d), (len(feature_by_name), np.zeros(N))
         )
         bf += feature_function_activation(d)(onsets)
 
@@ -591,26 +616,40 @@
 
     Some possible descriptors:
     * adagio : directions like 'adagio', 'molto adagio'
 
     """
     onsets = na["onset_div"]
     N = len(onsets)
-    constant = ["adagio", "largo", "lento", "grave", "larghetto", "adagietto", "andante",
-                "andantino", "moderato", "allegretto", "allegro", "vivace", "presto", "prestissimo",
-                "unknown_constant"]
+    constant = [
+        "adagio",
+        "largo",
+        "lento",
+        "grave",
+        "larghetto",
+        "adagietto",
+        "andante",
+        "andantino",
+        "moderato",
+        "allegretto",
+        "allegro",
+        "vivace",
+        "presto",
+        "prestissimo",
+        "unknown_constant",
+    ]
     names = constant + ["tempo_incr", "tempo_decr"]
     directions = list(part.iter_all(score.TempoDirection, include_subclasses=True))
 
-
     if "include_empty_features" in kwargs.keys():
         force_size = kwargs["include_empty_features"]
     else:
         force_size = False
     if force_size:
+
         def to_name(d):
             if isinstance(d, score.ResetTempoDirection):
                 ref = d.reference_tempo
                 if ref:
                     if ref.text in constant:
                         return ref.text
                     else:
@@ -625,15 +664,17 @@
                     return d.text
                 else:
                     return "unknown_constant"
             elif isinstance(d, score.IncreasingTempoDirection):
                 return "tempo_incr"
             elif isinstance(d, score.DecreasingTempoDirection):
                 return "tempo_decr"
+
     else:
+
         def to_name(d):
             if isinstance(d, score.ResetTempoDirection):
                 ref = d.reference_tempo
                 if ref:
                     return ref.text
                 else:
                     return d.text
@@ -647,15 +688,14 @@
     feature_by_name = {}
     for d in directions:
         j, bf = feature_by_name.setdefault(
             to_name(d), (len(feature_by_name), np.zeros(N))
         )
         bf += feature_function_activation(d)(onsets)
 
-
     if not force_size:
         M = len(feature_by_name) if len(feature_by_name) > 0 else 1
         names = [None] * M
     W = np.zeros((len(onsets), len(names)))
     for name, (j, bf) in feature_by_name.items():
         if force_size:
             j = names.index(name)
@@ -677,20 +717,23 @@
     constant_names = ["staccato", "tenuto", "accent", "marcato", "unknown_articulation"]
 
     if "include_empty_features" in kwargs.keys():
         force_size = kwargs["include_empty_features"]
     else:
         force_size = False
     if force_size:
+
         def to_name(d):
             if d.text in constant_names:
                 return d.text
             else:
-                return "unknown_direction"
+                return "unknown_articulation"
+
     else:
+
         def to_name(d):
             return d.text
 
     feature_by_name = {}
 
     for d in directions:
         j, bf = feature_by_name.setdefault(
@@ -718,55 +761,29 @@
 
 def feature_function_activation(direction):
     epsilon = 1e-6
 
     if isinstance(
         direction, (score.DynamicLoudnessDirection, score.DynamicTempoDirection)
     ):
-        # a dynamic direction will be encoded as a ramp from d.start.t to
-        # d.end.t, and then a step from d.end.t to the start of the next
-        # constant direction.
-
-        # There are two potential issues:
-
-        # Issue 1. d.end is None (e.g. just a ritardando without dashes). In this case
+        # a dynamic direction will be encoded as a ramp from d.start.t to d.end.t
+        # if d.end is None (e.g. just a ritardando without dashes)
         if direction.end:
             direction_end = direction.end.t
         else:
             # assume the end of d is the end of the measure:
             measure = next(direction.start.iter_prev(score.Measure, eq=True), None)
             if measure:
                 direction_end = measure.start.t
             else:
                 # no measure, unlikely, but not impossible.
-                direction_end = direction.start.t
-
-        if isinstance(direction, score.TempoDirection):
-            next_dir = next(
-                direction.start.iter_next(score.ConstantTempoDirection), None
-            )
-        if isinstance(direction, score.ArticulationDirection):
-            next_dir = next(
-                direction.start.iter_next(score.ConstantArticulationDirection), None
-            )
-        else:
-            next_dir = next(
-                direction.start.iter_next(score.ConstantLoudnessDirection), None
-            )
+                direction_end = direction.start.t + 1
 
-        if next_dir:
-            # TODO: what do we do when next_dir is too far away?
-            sustained_end = next_dir.start.t
-        else:
-            # Issue 2. there is no next constant direction. In that case the
-            # feature function will be a ramp with a quarter note ramp
-            sustained_end = direction_end + direction.start.quarter
-
-        x = [direction.start.t, direction_end - epsilon, sustained_end - epsilon]
-        y = [0, 1, 1]
+        x = [direction.start.t, direction_end, direction_end + epsilon]
+        y = [0, 1, 0]
 
     elif isinstance(
         direction,
         (
             score.ConstantLoudnessDirection,
             score.ConstantArticulationDirection,
             score.ConstantTempoDirection,
@@ -929,15 +946,14 @@
     if fix_size:
         M = len(names)
     else:
         M = len(feature_by_name) if len(feature_by_name) > 0 else 1
         names = [None] * M
     W = np.zeros((N, M))
 
-
     for name, (j, bf) in feature_by_name.items():
         if fix_size:
             j = names.index(name)
         else:
             names[j] = name
         W[:, j] = bf
 
@@ -995,15 +1011,14 @@
     notes = part.notes_tied if not np.all(na["pitch"] == 0) else part.rests
     ts_map = part.time_signature_map
     bm = part.beat_map
     feature_by_name = {}
     eps = 10**-6
 
     for i, n in enumerate(notes):
-
         beats, beat_type, mus_beats = ts_map(n.start.t).astype(int)
         measure = next(n.start.iter_prev(score.Measure, eq=True), None)
 
         if measure:
             measure_start = measure.start.t
         else:
             measure_start = 0
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/performance_codec.py` & `partitura-1.3.1/partitura/musicanalysis/performance_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 
 __all__ = ["encode_performance", "decode_performance", "to_matched_score"]
 
 
 #### Full Codecs ####
 
 
-@deprecated_alias(part='score', ppart="performance")
+@deprecated_alias(part="score", ppart="performance")
 def encode_performance(
     score: ScoreLike,
     performance: PerformanceLike,
     alignment: list,
     return_u_onset_idx=False,
     beat_normalization: str = "beat_period",  # "beat_period_log", "beat_period_ratio", "beat_period_ratio_log", "beat_period_standardized"
-    tempo_smooth: Union[str, Callable] = "average"
+    tempo_smooth: Union[str, Callable] = "average",
 ):
     """
     Encode expressive parameters from a matched performance
 
 
     Parameters
     ----------
@@ -73,15 +73,15 @@
     (time_params, unique_onset_idxs) = encode_tempo(
         score_onsets=m_score["onset"],
         performed_onsets=m_score["p_onset"],
         score_durations=m_score["duration"],
         performed_durations=m_score["p_duration"],
         return_u_onset_idx=True,
         beat_normalization=beat_normalization,
-        tempo_smooth=tempo_smooth
+        tempo_smooth=tempo_smooth,
     )
 
     # Get dynamics-related parameters
     dynamics_params = np.array(m_score["velocity"] / 127.0, dtype=[("velocity", "f4")])
 
     # Fixing random error
     parameters = time_params
@@ -89,23 +89,23 @@
 
     if return_u_onset_idx:
         return parameters, snote_ids, unique_onset_idxs
     else:
         return parameters, snote_ids
 
 
-@deprecated_alias(part='score')
+@deprecated_alias(part="score")
 def decode_performance(
     score: ScoreLike,
     performance_array: np.ndarray,
     snote_ids=None,
     part_id=None,
     part_name=None,
     return_alignment=False,
-    beat_normalization: str = "beat_period", # "beat_period_log", "beat_period_ratio", "beat_period_ratio_log", "beat_period_standardized"
+    beat_normalization: str = "beat_period",  # "beat_period_log", "beat_period_ratio", "beat_period_ratio_log", "beat_period_standardized"
     *args,
     **kwargs
 ) -> PerformedPart:
     """
     Given a Part (score) and a performance array return a PerformedPart.
 
     Parameters
@@ -127,31 +127,31 @@
     alignment: list (optional)
         A list of dicts for the alignment.
     """
 
     snotes = score.note_array()
 
     if snote_ids is None:
-        snote_ids = [n['id'] for n in snotes]
+        snote_ids = [n["id"] for n in snotes]
         snote_info = snotes
     else:
-        snote_info = snotes[np.isin(snotes['id'], snote_ids)]
+        snote_info = snotes[np.isin(snotes["id"], snote_ids)]
 
     # sort
     sort_idx = np.lexsort((snote_info["pitch"], snote_info["onset_div"]))
 
     onsets = snote_info["onset_beat"][sort_idx]
     durations = snote_info["duration_beat"][sort_idx]
     pitches = snote_info["pitch"][sort_idx]
 
     pitches = np.clip(pitches, 1, 127)
 
     dynamics_params = performance_array["velocity"][sort_idx]
     if beat_normalization != "beat_period":
-        norm_params = list(TEMPO_NORMALIZATION[beat_normalization]['param_names'])
+        norm_params = list(TEMPO_NORMALIZATION[beat_normalization]["param_names"])
     else:
         norm_params = []
     time_params = performance_array[
         list(("beat_period", "timing", "articulation_log")) + norm_params
     ][sort_idx]
 
     onsets_durations = decode_time(
@@ -184,29 +184,33 @@
     # * rescale according to default values?
     ppart = PerformedPart(id=part_id, part_name=part_name, notes=notes)
 
     if return_alignment:
         alignment = []
         for snote, pnote in zip(snote_info, ppart.notes):
             alignment.append(
-                dict(label="match", score_id=snote['id'], performance_id=pnote["id"])
+                dict(label="match", score_id=snote["id"], performance_id=pnote["id"])
             )
 
         return ppart, alignment
     else:
-
         return ppart
 
+
 #### Time and Articulation Codecs ####
 
-def decode_time(score_onsets,
-                score_durations,
-                parameters,
-                normalization = "beat_period",
-                *args, **kwargs):
+
+def decode_time(
+    score_onsets,
+    score_durations,
+    parameters,
+    normalization="beat_period",
+    *args,
+    **kwargs
+):
     """
     Decode a performance into onsets and durations in seconds
     for each note in the score.
     """
     score_onsets = score_onsets.astype(float, copy=False)
     score_durations = score_durations.astype(float, copy=False)
 
@@ -218,24 +222,37 @@
     )
     unique_onset_idxs = score_info["unique_onset_idxs"]
     diff_u_onset_score = score_info["diff_u_onset"]
 
     # reconstruct the time by the extra parameters, for testing the inversion.
     # In practice, always reconstruct the time by beat_period.
     if normalization != "beat_period":
-        tempo_param_names = list(TEMPO_NORMALIZATION[normalization]['param_names'])
+        tempo_param_names = list(TEMPO_NORMALIZATION[normalization]["param_names"])
         time_param = np.array(
-            [tuple(np.mean(rfn.structured_to_unstructured(parameters[tempo_param_names][uix]), axis=0),) for uix in unique_onset_idxs],
-            dtype=[(tp, "f4") for tp in tempo_param_names]
+            [
+                tuple(
+                    np.mean(
+                        rfn.structured_to_unstructured(
+                            parameters[tempo_param_names][uix]
+                        ),
+                        axis=0,
+                    ),
+                )
+                for uix in unique_onset_idxs
+            ],
+            dtype=[(tp, "f4") for tp in tempo_param_names],
         )
-        beat_period = TEMPO_NORMALIZATION[normalization]['rescale'](time_param)
+        beat_period = TEMPO_NORMALIZATION[normalization]["rescale"](time_param)
 
     else:
         time_param = np.array(
-            [tuple([np.mean(parameters["beat_period"][uix])]) for uix in unique_onset_idxs],
+            [
+                tuple([np.mean(parameters["beat_period"][uix])])
+                for uix in unique_onset_idxs
+            ],
             dtype=[("beat_period", "f4")],
         )
         beat_period = time_param["beat_period"]
 
     ioi_perf = diff_u_onset_score * beat_period
 
     eq_onset = np.cumsum(np.r_[0, ioi_perf])
@@ -261,15 +278,14 @@
     score_durations, performed_durations, unique_onset_idxs, beat_period
 ):
     """
     Encode articulation
     """
     articulation = np.zeros_like(score_durations)
     for idx, bp in zip(unique_onset_idxs, beat_period):
-
         sd = score_durations[idx]
         pd = performed_durations[idx]
 
         # indices of notes with duration 0 (grace notes)
         grace_mask = sd <= 0
 
         # Grace notes have an articulation ratio of 1
@@ -292,16 +308,16 @@
 
 def encode_tempo(
     score_onsets: np.ndarray,
     performed_onsets: np.ndarray,
     score_durations,
     performed_durations,
     return_u_onset_idx: bool = False,
-    beat_normalization: str = "beat_period", # "beat_period_log", "beat_period_ratio", "beat_period_ratio_log", "beat_period_standardized"
-    tempo_smooth: Union[str, Callable] = "average"  # "average" or "derivative"
+    beat_normalization: str = "beat_period",  # "beat_period_log", "beat_period_ratio", "beat_period_ratio_log", "beat_period_standardized"
+    tempo_smooth: Union[str, Callable] = "average",  # "average" or "derivative"
 ) -> np.ndarray:
     """
     Compute time-related performance parameters from a performance
     """
     if score_onsets.shape != performed_onsets.shape:
         raise ValueError("The performance and the score should be of " "the same size")
 
@@ -344,16 +360,18 @@
     eq_onsets = (
         np.cumsum(np.r_[0, beat_period[:-1] * np.diff(s_onsets)])
         + performance[unique_onset_idxs[0], 0].mean()
     )
 
     # Compute tempo parameter and normalize
     if beat_normalization != "beat_period":
-        tempo_params = np.array(TEMPO_NORMALIZATION[beat_normalization]['scale'](beat_period))
-        tempo_param_names = list(TEMPO_NORMALIZATION[beat_normalization]['param_names'])
+        tempo_params = np.array(
+            TEMPO_NORMALIZATION[beat_normalization]["scale"](beat_period)
+        )
+        tempo_param_names = list(TEMPO_NORMALIZATION[beat_normalization]["param_names"])
 
     # Compute articulation parameter
     articulation_param = encode_articulation(
         score_durations=score[:, 1],
         performed_durations=performance[:, 1],
         unique_onset_idxs=unique_onset_idxs,
         beat_period=beat_period,
@@ -450,17 +468,15 @@
 
     # unique score onsets
     unique_s_onsets = score_info["u_onset"]
     # equivalent onsets
     eq_onsets = perf_info["u_onset"]
 
     # Monotonize times
-    eq_onset_mt, unique_s_onsets_mt = monotonize_times(
-        eq_onsets, x=unique_s_onsets
-    )
+    eq_onset_mt, unique_s_onsets_mt = monotonize_times(eq_onsets, x=unique_s_onsets)
 
     # Estimate Beat Period
     perf_iois = np.diff(eq_onset_mt)
     s_iois = np.diff(unique_s_onsets_mt)
     beat_period = perf_iois / s_iois
 
     tempo_fun = interp1d(
@@ -471,27 +487,34 @@
         fill_value=(beat_period[0], beat_period[-1]),
     )
 
     if input_onsets is None:
         input_onsets = unique_s_onsets[:-1]
 
     tempo_curve = tempo_fun(input_onsets)
-
-    assert((tempo_curve >= 0).all())
+    if not (tempo_curve >= 0).all():
+        warnings.warn(
+            "The estimated tempo curve is not always positive. "
+            "This might be due to a bad alignment."
+        )
     if return_onset_idxs:
         return tempo_curve, input_onsets, unique_onset_idxs
     else:
         return tempo_curve, input_onsets
 
 
-def tempo_by_derivative(score_onsets, performed_onsets,
-                        score_durations, performed_durations,
-                        unique_onset_idxs=None,
-                        input_onsets=None,
-                        return_onset_idxs=False):
+def tempo_by_derivative(
+    score_onsets,
+    performed_onsets,
+    score_durations,
+    performed_durations,
+    unique_onset_idxs=None,
+    input_onsets=None,
+    return_onset_idxs=False,
+):
     """
     Computes a tempo curve using the derivative of the average performed
     onset times of all notes belonging to the same score onset with respect
     to that score onset. This results in a curve that is smoother than the
     tempo estimated using `tempo_by_average`.
 
     Parameters
@@ -538,36 +561,40 @@
 
     # Get unique onsets if no provided
     if unique_onset_idxs is None:
         # Get indices of the unique onsets (quantize score onsets)
         unique_onset_idxs = get_unique_onset_idxs((1e4 * score_onsets).astype(int))
 
     # Get score information
-    score_info = get_unique_seq(onsets=score_onsets,
-                                offsets=score_onsets + score_durations,
-                                unique_onset_idxs=unique_onset_idxs,
-                                return_diff=False)
+    score_info = get_unique_seq(
+        onsets=score_onsets,
+        offsets=score_onsets + score_durations,
+        unique_onset_idxs=unique_onset_idxs,
+        return_diff=False,
+    )
     # Get performance information
-    perf_info = get_unique_seq(onsets=performed_onsets,
-                               offsets=performed_onsets + performed_durations,
-                               unique_onset_idxs=unique_onset_idxs,
-                               return_diff=False)
+    perf_info = get_unique_seq(
+        onsets=performed_onsets,
+        offsets=performed_onsets + performed_durations,
+        unique_onset_idxs=unique_onset_idxs,
+        return_diff=False,
+    )
 
     # unique score onsets
-    unique_s_onsets = score_info['u_onset']
+    unique_s_onsets = score_info["u_onset"]
     # equivalent onsets
-    eq_onsets = perf_info['u_onset']
+    eq_onsets = perf_info["u_onset"]
 
     # Monotonize times
-    eq_onset_mt, unique_s_onsets_mt = monotonize_times(eq_onsets,
-                                                       x=unique_s_onsets)
+    eq_onset_mt, unique_s_onsets_mt = monotonize_times(eq_onsets, x=unique_s_onsets)
     # Function that that interpolates the equivalent performed onsets
     # as a function of the score onset.
-    onset_fun = interp1d(unique_s_onsets_mt, eq_onset_mt, kind='linear',
-                         fill_value='extrapolate')
+    onset_fun = interp1d(
+        unique_s_onsets_mt, eq_onset_mt, kind="linear", fill_value="extrapolate"
+    )
 
     if input_onsets is None:
         input_onsets = unique_s_onsets[:-1]
 
     tempo_curve = derivative(onset_fun, input_onsets, dx=0.5)
 
     if return_onset_idxs:
@@ -575,19 +602,21 @@
     else:
         return tempo_curve, input_onsets
 
 
 #### Alignment Processing ####
 
 
-@deprecated_alias(part='score', ppart="performance")
-def to_matched_score(score: ScoreLike,
-                     performance: PerformanceLike,
-                     alignment: list,
-                     include_score_markings=False):
+@deprecated_alias(part="score", ppart="performance")
+def to_matched_score(
+    score: ScoreLike,
+    performance: PerformanceLike,
+    alignment: list,
+    include_score_markings=False,
+):
     """
     Returns a mixed score-performance note array
     consisting of matched notes in the alignment.
 
     Args:
         score (score.ScoreLike): score information
         performance (performance.PerformanceLike): performance information
@@ -603,57 +632,67 @@
     # remove repetitions from aligment note ids
     for a in alignment:
         if a["label"] == "match":
             a["score_id"] = str(a["score_id"])
 
     feature_functions = None
     if include_score_markings:
-        feature_functions = ["loudness_direction_feature", "articulation_feature",
-                             "tempo_direction_feature", "slur_feature"]
+        feature_functions = [
+            "loudness_direction_feature",
+            "articulation_feature",
+            "tempo_direction_feature",
+            "slur_feature",
+        ]
 
     na = note_features.compute_note_array(score, feature_functions=feature_functions)
     p_na = performance.note_array()
-    part_by_id = dict((n['id'], na[na['id'] == n['id']]) for n in na)
-    ppart_by_id = dict((n['id'], p_na[p_na['id'] == n['id']]) for n in p_na)
+    part_by_id = dict((n["id"], na[na["id"] == n["id"]]) for n in na)
+    ppart_by_id = dict((n["id"], p_na[p_na["id"] == n["id"]]) for n in p_na)
 
     # pair matched score and performance notes
     note_pairs = [
         (part_by_id[a["score_id"]], ppart_by_id[a["performance_id"]])
         for a in alignment
         if (a["label"] == "match" and a["score_id"] in part_by_id)
     ]
     ms = []
     # sort according to onset (primary) and pitch (secondary)
-    pitch_onset = [(sn['pitch'].item(), sn['onset_div'].item()) for sn, _ in note_pairs]
+    pitch_onset = [(sn["pitch"].item(), sn["onset_div"].item()) for sn, _ in note_pairs]
     sort_order = np.lexsort(list(zip(*pitch_onset)))
     snote_ids = []
     for i in sort_order:
         sn, n = note_pairs[int(i)]
-        sn_on, sn_off = [sn['onset_beat'], sn['onset_beat'] + sn['duration_beat']]
+        sn_on, sn_off = [sn["onset_beat"], sn["onset_beat"] + sn["duration_beat"]]
         sn_dur = sn_off - sn_on
         # hack for notes with negative durations
         n_dur = max(n["duration_sec"], 60 / 200 * 0.25)
-        pair_info = (sn_on, sn_dur, sn['pitch'], n["onset_sec"], n_dur, n["velocity"])
+        pair_info = (sn_on, sn_dur, sn["pitch"], n["onset_sec"], n_dur, n["velocity"])
         if include_score_markings:
-            pair_info += (sn['voice'].item(), )
-            pair_info += tuple([sn[field].item() for field in sn.dtype.names if "feature" in field])
+            pair_info += (sn["voice"].item(),)
+            pair_info += tuple(
+                [sn[field].item() for field in sn.dtype.names if "feature" in field]
+            )
         ms.append(pair_info)
-        snote_ids.append(sn['id'].item())
+        snote_ids.append(sn["id"].item())
 
     fields = [
         ("onset", "f4"),
         ("duration", "f4"),
         ("pitch", "i4"),
         ("p_onset", "f4"),
         ("p_duration", "f4"),
         ("velocity", "i4"),
     ]
     if include_score_markings:
         fields += [("voice", "i4")]
-        fields += [(field, sn.dtype.fields[field][0]) for field in sn.dtype.fields if "feature" in field]
+        fields += [
+            (field, sn.dtype.fields[field][0])
+            for field in sn.dtype.fields
+            if "feature" in field
+        ]
 
     return np.array(ms, dtype=fields), snote_ids
 
 
 def get_time_maps_from_alignment(
     ppart_or_note_array, spart_or_note_array, alignment, remove_ornaments=True
 ):
@@ -770,15 +809,14 @@
         (index_in_score_note_array, index_in_performance_notearray)
     """
     # Get matched notes
     matched_idxs = []
     for al in alignment:
         # Get only matched notes (i.e., ignore inserted or deleted notes)
         if al["label"] == "match":
-
             # if ppart_note_array['id'].dtype != type(al['performance_id']):
             if not isinstance(ppart_note_array["id"], type(al["performance_id"])):
                 p_id = str(al["performance_id"])
             else:
                 p_id = al["performance_id"]
 
             p_idx = int(np.where(ppart_note_array["id"] == p_id)[0])
@@ -795,20 +833,23 @@
 #### Sequence Processing: onset-wise/note-wise/monotonicity/uniqueness ####
 
 
 def get_unique_seq(onsets, offsets, unique_onset_idxs=None, return_diff=False):
     """
     Get unique onsets of a sequence of notes
     """
-    eps = np.finfo(float).eps
 
     first_time = np.min(onsets)
 
     # ensure last score time is later than last onset
-    last_time = max(np.max(onsets) + eps, np.max(offsets))
+    if np.max(onsets) == np.max(offsets):
+        # last note without duration (grace note)
+        last_time = np.max(onsets) + 1
+    else:
+        last_time = np.max(offsets)
 
     total_dur = last_time - first_time
 
     if unique_onset_idxs is None:
         # unique_onset_idxs = unique_onset_idx(score[:, 0])
         unique_onset_idxs = get_unique_onset_idxs(onsets)
 
@@ -864,21 +905,20 @@
         return unique_onset_idxs, unique_onsets
     else:
         return unique_onset_idxs
 
 
 def notewise_to_onsetwise(notewise_inputs, unique_onset_idxs):
     """Agregate basis functions per onset"""
-    
+
     if notewise_inputs.ndim == 1:
         shape = len(unique_onset_idxs)
     else:
         shape = (len(unique_onset_idxs),) + notewise_inputs.shape[1:]
     onsetwise_inputs = np.zeros(shape, dtype=notewise_inputs.dtype)
-    
 
     for i, uix in enumerate(unique_onset_idxs):
         try:
             onsetwise_inputs[i] = notewise_inputs[uix].mean(0)
         except TypeError:
             for tn in notewise_inputs.dtype.names:
                 onsetwise_inputs[i][tn] = notewise_inputs[uix][tn].mean()
@@ -889,84 +929,88 @@
     """Expand onsetwise predictions for each note"""
     n_notes = sum([len(uix) for uix in unique_onset_idxs])
     if onsetwise_input.ndim == 1:
         shape = n_notes
     else:
         shape = (n_notes,) + onsetwise_input.shape[1:]
     notewise_inputs = np.zeros(shape, dtype=onsetwise_input.dtype)
-    
+
     for i, uix in enumerate(unique_onset_idxs):
         notewise_inputs[uix] = onsetwise_input[[i]]
     return notewise_inputs
 
 
 #### Temo Parameter Normalizations ####
 
 
 def bp_scale(beat_period):
     return [beat_period]
 
 
 def bp_rescale(tempo_params):
-    return tempo_params['beat_period']
+    return tempo_params["beat_period"]
 
 
 def beat_period_log_scale(beat_period):
     return [np.log2(beat_period)]
 
 
 def beat_period_log_rescale(tempo_params):
-    return 2 ** tempo_params['beat_period_log']
+    return 2 ** tempo_params["beat_period_log"]
 
 
 def beat_period_standardized_scale(beat_period):
     beat_period_std = np.std(beat_period) * np.ones_like(beat_period)
     beat_period_mean = np.mean(beat_period) * np.ones_like(beat_period)
     beat_period_standardized = (beat_period - beat_period_mean) / beat_period_std
     return [beat_period_standardized, beat_period_mean, beat_period_std]
 
 
 def beat_period_standardized_rescale(tempo_params):
-    return (tempo_params['beat_period_standardized'] * tempo_params['beat_period_std']
-            + tempo_params['beat_period_mean'])
+    return (
+        tempo_params["beat_period_standardized"] * tempo_params["beat_period_std"]
+        + tempo_params["beat_period_mean"]
+    )
 
 
 def beat_period_ratio_scale(beat_period):
     beat_period_mean = np.mean(beat_period) * np.ones_like(beat_period)
     beat_period_ratio = beat_period / beat_period_mean
     return [beat_period_ratio, beat_period_mean]
 
 
 def beat_period_ratio_rescale(tempo_params):
-    return tempo_params['beat_period_ratio'] * tempo_params['beat_period_mean']
+    return tempo_params["beat_period_ratio"] * tempo_params["beat_period_mean"]
 
 
 def beat_period_ratio_log_scale(beat_period):
     beat_period_ratio, beat_period_mean = beat_period_ratio_scale(beat_period)
     return [np.log2(beat_period_ratio), beat_period_mean]
 
 
 def beat_period_ratio_log_rescale(tempo_params):
-    return (2 ** tempo_params['beat_period_ratio_log'] * tempo_params['beat_period_mean'])
+    return 2 ** tempo_params["beat_period_ratio_log"] * tempo_params["beat_period_mean"]
 
 
 TEMPO_NORMALIZATION = dict(
-    beat_period=dict(scale=bp_scale,
-                     rescale=bp_rescale,
-                     param_names=('beat_period',)),
-    beat_period_log=dict(scale=beat_period_log_scale,
-                         rescale=beat_period_log_rescale,
-                         param_names=('beat_period_log',)),
-    beat_period_ratio=dict(scale=beat_period_ratio_scale,
-                           rescale=beat_period_ratio_rescale,
-                           param_names=('beat_period_ratio',
-                                        'beat_period_mean')),
-    beat_period_ratio_log=dict(scale=beat_period_ratio_log_scale,
-                               rescale=beat_period_ratio_log_rescale,
-                               param_names=('beat_period_ratio_log',
-                                            'beat_period_mean')),
-    beat_period_standardized=dict(scale=beat_period_standardized_scale,
-                                  rescale=beat_period_standardized_rescale,
-                                  param_names=('beat_period_standardized',
-                                               'beat_period_mean', 'beat_period_std'))
+    beat_period=dict(scale=bp_scale, rescale=bp_rescale, param_names=("beat_period",)),
+    beat_period_log=dict(
+        scale=beat_period_log_scale,
+        rescale=beat_period_log_rescale,
+        param_names=("beat_period_log",),
+    ),
+    beat_period_ratio=dict(
+        scale=beat_period_ratio_scale,
+        rescale=beat_period_ratio_rescale,
+        param_names=("beat_period_ratio", "beat_period_mean"),
+    ),
+    beat_period_ratio_log=dict(
+        scale=beat_period_ratio_log_scale,
+        rescale=beat_period_ratio_log_rescale,
+        param_names=("beat_period_ratio_log", "beat_period_mean"),
+    ),
+    beat_period_standardized=dict(
+        scale=beat_period_standardized_scale,
+        rescale=beat_period_standardized_rescale,
+        param_names=("beat_period_standardized", "beat_period_mean", "beat_period_std"),
+    ),
 )
-
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/performance_features.py` & `partitura-1.3.1/partitura/musicanalysis/performance_features.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,68 +6,73 @@
 """
 
 import sys
 import types
 from typing import Union, List
 import warnings
 import numpy as np
-import matplotlib.pyplot as plt
-from scipy import stats
-from scipy.optimize import least_squares
 from scipy.signal import find_peaks
 import numpy.lib.recfunctions as rfn
 from partitura.score import ScoreLike
 from partitura.performance import PerformanceLike, PerformedPart
 from partitura.utils.generic import interp1d
-from partitura.musicanalysis.performance_codec import to_matched_score, onsetwise_to_notewise, encode_tempo
+from partitura.musicanalysis.performance_codec import (
+    to_matched_score,
+    onsetwise_to_notewise,
+    encode_tempo,
+)
 
 
 __all__ = [
     "make_performance_features",
 ]
 
-# ordinal 
+# ordinal
 OLS = ["ppp", "pp", "p", "mp", "mf", "f", "ff", "fff"]
 
 
 class InvalidPerformanceFeatureException(Exception):
     pass
 
-def make_performance_features(score: ScoreLike,
-                              performance: PerformanceLike,
-                              alignment: list,
-                              feature_functions: Union[List, str],
-                              add_idx: bool = True
-                              ):
+
+def make_performance_features(
+    score: ScoreLike,
+    performance: PerformanceLike,
+    alignment: list,
+    feature_functions: Union[List, str],
+    add_idx: bool = True,
+):
     """
-    Compute the performance features. This function is defined in the same 
+    Compute the performance features. This function is defined in the same
     style of note_features.make_note_features
 
     Parameters
     ----------
     score : partitura.score.ScoreLike
         Score information, can be a part, score
     performance : partitura.performance.PerformanceLike
         Performance information, can be a ppart, performance
     alignment : list
         The score--performance alignment, a list of dictionaries
     feature_functions : list or str
         A list of performance feature functions. Elements of the list can be either
         the functions themselves or the names of a feature function as
-        strings (or a mix). 
-        currently implemented: 
+        strings (or a mix).
+        currently implemented:
         asynchrony_feature, articulation_feature, dynamics_feature, pedal_feature
     add_idx: bool
         add score note idx column to feature array
 
     Returns
     -------
     performance_features : structured array
     """
-    m_score, unique_onset_idxs, snote_ids = compute_matched_score(score, performance, alignment)
+    m_score, unique_onset_idxs, snote_ids = compute_matched_score(
+        score, performance, alignment
+    )
 
     acc = []
     if isinstance(feature_functions, str) and feature_functions == "all":
         feature_functions = list_performance_feats_functions()
     elif not isinstance(feature_functions, list):
         raise TypeError(
             "feature_functions variable {} needs to be list or 'all'".format(
@@ -101,36 +106,46 @@
                 )
                 msg = "NaNs or Infs found in the following feature: {} ".format(
                     ", ".join(np.array(features.dtype.names)[problematic])
                 )
                 raise InvalidPerformanceFeatureException(msg)
 
             # prefix feature names by function name
-            feature_names = ["{}.{}".format(func.__name__, n) for n in features.dtype.names]
-            features = rfn.rename_fields(features, dict(zip(features.dtype.names, feature_names)))
+            feature_names = [
+                "{}.{}".format(func.__name__, n) for n in features.dtype.names
+            ]
+            features = rfn.rename_fields(
+                features, dict(zip(features.dtype.names, feature_names))
+            )
 
             acc.append(features)
 
     if add_idx:
-        acc.append(np.array([(idx) for idx in snote_ids], dtype = [("id","U256")]))
+        acc.append(np.array([(idx) for idx in snote_ids], dtype=[("id", "U256")]))
 
     performance_features = rfn.merge_arrays(acc, flatten=True, usemask=False)
     full_performance_features = rfn.join_by("id", performance_features, m_score)
     full_performance_features = full_performance_features.data
 
-    sort_idx = np.lexsort((full_performance_features["duration"],
-                           full_performance_features["pitch"], 
-                           full_performance_features["onset"]))
+    sort_idx = np.lexsort(
+        (
+            full_performance_features["duration"],
+            full_performance_features["pitch"],
+            full_performance_features["onset"],
+        )
+    )
     full_performance_features = full_performance_features[sort_idx]
-    return  full_performance_features
+    return full_performance_features
 
 
-def compute_matched_score(score: ScoreLike, 
-                            performance: PerformanceLike,
-                            alignment: list,):
+def compute_matched_score(
+    score: ScoreLike,
+    performance: PerformanceLike,
+    alignment: list,
+):
     """
     Compute the matched score and add the score features
 
     Parameters
     ----------
     score : partitura.score.ScoreLike
         Score information, can be a part, score
@@ -141,26 +156,37 @@
 
     Returns
     -------
     m_score : np strutured array
     unique_onset_idxs : list
     """
 
-    m_score, snote_ids = to_matched_score(score, performance, alignment, include_score_markings=True)
+    m_score, snote_ids = to_matched_score(
+        score, performance, alignment, include_score_markings=True
+    )
     (time_params, unique_onset_idxs) = encode_tempo(
         score_onsets=m_score["onset"],
         performed_onsets=m_score["p_onset"],
         score_durations=m_score["duration"],
         performed_durations=m_score["p_duration"],
         return_u_onset_idx=True,
-        tempo_smooth="average"
+        tempo_smooth="average",
+    )
+    m_score = rfn.append_fields(
+        m_score,
+        ["beat_period", "timing", "articulation_log", "id"],
+        [
+            time_params["beat_period"],
+            time_params["timing"],
+            time_params["articulation_log"],
+            snote_ids,
+        ],
+        ["f4", "f4", "f4", "U256"],
+        usemask=False,
     )
-    m_score = rfn.append_fields(m_score, ["beat_period", "id"], 
-                                [time_params['beat_period'], snote_ids], 
-                                ["f4", "U256"], usemask=False,)
     return m_score, unique_onset_idxs, snote_ids
 
 
 def list_performance_feats_functions():
     """Return a list of all feature function names defined in this module.
 
     The feature function names listed here can be specified by name in
@@ -201,152 +227,178 @@
         member = getattr(sys.modules[__name__], name)
         if member.__doc__:
             print(
                 " " * doc_indent + member.__doc__.replace("\n", " " * doc_indent + "\n")
             )
 
 
-
 # alias
 list_performance_feature_functions = list_performance_feats_functions
 print_performance_feature_functions = print_performance_feats_functions
 
 ### Asynchrony
 
-def asynchrony_feature(m_score: np.ndarray,
-                     unique_onset_idxs: list,
-                     performance: PerformanceLike):
+
+def asynchrony_feature(
+    m_score: np.ndarray, unique_onset_idxs: list, performance: PerformanceLike
+):
     """
-    Compute the asynchrony attributes from the alignment. 
+    Compute the asynchrony attributes from the alignment.
 
     Parameters
     ----------
     m_score : list
-        correspondance between score and performance notes, with score markings. 
+        correspondance between score and performance notes, with score markings.
     unique_onset_idxs : list
         a list of arrays with the note indexes that have the same onset
     performance: PerformedPart
         The original PerformedPart object
-    
+
     Returns
     -------
     async_ : structured array
         structured array (broadcasted to the note level) with the following fields
-            delta [0, 1]: the largest time difference (in seconds) between onsets in this group 
-            pitch_cor [-1, 1]: correlation between timing and pitch, min-scaling 
+            delta [0, 1]: the largest time difference (in seconds) between onsets in this group
+            pitch_cor [-1, 1]: correlation between timing and pitch, min-scaling
             vel_cor [-1, 1]: correlation between timing and velocity, min-scaling
-            voice_std [0, 1]: std of the avg timing (in seconds) of each voice in this group 
+            voice_std [0, 1]: std of the avg timing (in seconds) of each voice in this group
     """
-    
-    async_ = np.zeros(len(unique_onset_idxs), dtype=[(
-        "delta", "f4"), ("pitch_cor", "f4"), ("vel_cor", "f4"), ("voice_std", "f4")])
-    for i, onset_idxs in enumerate(unique_onset_idxs):
 
+    async_ = np.zeros(
+        len(unique_onset_idxs),
+        dtype=[
+            ("delta", "f4"),
+            ("pitch_cor", "f4"),
+            ("vel_cor", "f4"),
+            ("voice_std", "f4"),
+        ],
+    )
+    for i, onset_idxs in enumerate(unique_onset_idxs):
         note_group = m_score[onset_idxs]
 
-        onset_times = note_group['p_onset']
+        onset_times = note_group["p_onset"]
         delta = min(onset_times.max() - onset_times.min(), 1)
-        async_[i]['delta'] = delta 
+        async_[i]["delta"] = delta
 
-        midi_pitch = note_group['pitch']
-        midi_pitch = midi_pitch - midi_pitch.min() # min-scaling
+        midi_pitch = note_group["pitch"]
+        midi_pitch = midi_pitch - midi_pitch.min()  # min-scaling
         onset_times = onset_times - onset_times.min()
-        cor = (-1) * np.corrcoef(midi_pitch, onset_times)[0, 1] if (
-            len(midi_pitch) > 1 and sum(midi_pitch) != 0 and sum(onset_times) != 0) else 0
+        cor = (
+            (-1) * np.corrcoef(midi_pitch, onset_times)[0, 1]
+            if (len(midi_pitch) > 1 and sum(midi_pitch) != 0 and sum(onset_times) != 0)
+            else 0
+        )
         # cor=nan if there is only one note in the group
-        async_[i]['pitch_cor'] = cor
+        async_[i]["pitch_cor"] = cor
 
-        assert not np.isnan(cor) 
+        assert not np.isnan(cor)
 
-        midi_vel = note_group['velocity'].astype(float)
+        midi_vel = note_group["velocity"].astype(float)
         midi_vel = midi_vel - midi_vel.min()
-        cor = (-1) * np.corrcoef(midi_vel, onset_times)[0, 1] if (
-            sum(midi_vel) != 0 and sum(onset_times) != 0) else 0
-        async_[i]['vel_cor'] = cor
+        cor = (
+            (-1) * np.corrcoef(midi_vel, onset_times)[0, 1]
+            if (sum(midi_vel) != 0 and sum(onset_times) != 0)
+            else 0
+        )
+        async_[i]["vel_cor"] = cor
 
-        assert not np.isnan(cor) 
+        assert not np.isnan(cor)
 
-        voices = np.unique(note_group['voice'])
+        voices = np.unique(note_group["voice"])
         voices_onsets = []
         for voice in voices:
-            note_in_voice = note_group[note_group['voice'] == voice]
-            voices_onsets.append(note_in_voice['p_onset'].mean())
-        async_[i]['voice_std'] = min(np.std(np.array(voices_onsets)), 1)
-    
+            note_in_voice = note_group[note_group["voice"] == voice]
+            voices_onsets.append(note_in_voice["p_onset"].mean())
+        async_[i]["voice_std"] = min(np.std(np.array(voices_onsets)), 1)
+
     return onsetwise_to_notewise(async_, unique_onset_idxs)
 
 
-### Dynamics 
+### Dynamics
 
 
 ### Articulation
 
-def articulation_feature(m_score : np.ndarray, 
-                         unique_onset_idxs: list,
-                         performance: PerformanceLike,
-                         return_mask=False):
+
+def articulation_feature(
+    m_score: np.ndarray,
+    unique_onset_idxs: list,
+    performance: PerformanceLike,
+    return_mask=False,
+):
     """
     Compute the articulation attributes (key overlap ratio) from the alignment.
     Key overlap ratio is the ratio between key overlap time (KOT) and IOI, result in a value between (-1, inf)
         -1 is the dummy value. For normalization purposes we empirically cap the maximum to 5.
-    
+
     References
     ----------
     ..  [1] B.Repp: Acoustics, Perception, and Production of Legato Articulation on a Digital Piano
-    
+
     Parameters
     ----------
     m_score : list
-        correspondance between score and performance notes, with score markings. 
+        correspondance between score and performance notes, with score markings.
     unique_onset_idxs : list
         a list of arrays with the note indexes that have the same onset
     performance: PerformedPart
         The original PerformedPart object
     return_mask : bool
         if true, return a boolean mask of legato notes, staccato notes and repeated notes
 
     Returns
     -------
     kor_ : structured array (1, n_notes)
         structured array on the note level with fields kor (-1, 5]
-    """  
-    
-    m_score = rfn.append_fields(m_score, "offset", m_score['onset'] + m_score['duration'], usemask=False)
-    m_score = rfn.append_fields(m_score, "p_offset", m_score['p_onset'] + m_score['p_duration'], usemask=False)
+    """
+
+    m_score = rfn.append_fields(
+        m_score, "offset", m_score["onset"] + m_score["duration"], usemask=False
+    )
+    m_score = rfn.append_fields(
+        m_score, "p_offset", m_score["p_onset"] + m_score["p_duration"], usemask=False
+    )
 
     kor_ = np.full(len(m_score), -1, dtype=[("kor", "f4")])
     if return_mask:
-        mask = np.full(len(m_score), False, dtype=[("legato", "?"), ("staccato", "?"), ("repeated", "?")])
+        mask = np.full(
+            len(m_score),
+            False,
+            dtype=[("legato", "?"), ("staccato", "?"), ("repeated", "?")],
+        )
 
     # consider the note transition by each voice
-    for voice in np.unique(m_score['voice']):
-        match_voiced = m_score[m_score['voice'] == voice]
+    for voice in np.unique(m_score["voice"]):
+        match_voiced = m_score[m_score["voice"] == voice]
         for _, note_info in enumerate(match_voiced):
-
-            if note_info['onset'] == match_voiced['onset'].max():  # last beat
+            if note_info["onset"] == match_voiced["onset"].max():  # last beat
                 break
-            next_note_info = get_next_note(note_info, match_voiced) # find most plausible transition
+            next_note_info = get_next_note(
+                note_info, match_voiced
+            )  # find most plausible transition
 
-            if next_note_info: # in some cases no meaningful transition
+            if next_note_info:  # in some cases no meaningful transition
                 j = np.where(m_score == note_info)[0].item()  # original position
 
-                if (note_info['offset'] == next_note_info['onset']):
-                    kor_[j]['kor'] =  get_kor(note_info, next_note_info)
+                if note_info["offset"] == next_note_info["onset"]:
+                    kor_[j]["kor"] = get_kor(note_info, next_note_info)
+
+                if return_mask:  # return the
+                    if (note_info["slur_feature.slur_incr"] > 0) or (
+                        note_info["slur_feature.slur_decr"] > 0
+                    ):
+                        mask[j]["legato"] = True
+
+                    if note_info["articulation"] == "staccato":
+                        mask[j]["staccato"] = True
+
+                    # KOR for repeated notes
+                    if note_info["pitch"] == next_note_info["pitch"]:
+                        mask[j]["repeated"] = True
 
-                if return_mask: # return the 
-                    if (note_info['slur_feature.slur_incr'] > 0) or (note_info['slur_feature.slur_decr'] > 0): 
-                        mask[j]['legato'] = True
-
-                    if note_info['articulation'] == 'staccato':
-                        mask[j]['staccato'] =  True
-
-                    # KOR for repeated notes 
-                    if (note_info['pitch'] == next_note_info['pitch']):
-                        mask[j]['repeated'] =  True
-    
     if return_mask:
         return kor_, mask
     else:
         return kor_
 
 
 def get_kor(e1, e2):
@@ -365,132 +417,141 @@
 
     Returns
     -------
     kor : float
         Key overlap ratio
 
     """
-    kot = e1['p_offset'] - e2['p_onset']
-    ioi = e2['p_onset'] - e1['p_onset']
+    kot = e1["p_offset"] - e2["p_onset"]
+    ioi = e2["p_onset"] - e1["p_onset"]
 
     if ioi <= 0:
         kor = 0
 
     kor = kot / ioi
-    
+
     return min(kor, 5)
 
 
 def get_next_note(note_info, match_voiced):
     """
-    get the next note in the same voice that's a reasonable transition 
-   
+    get the next note in the same voice that's a reasonable transition
+
     Parameters
     ----------
     note_info : np.ndarray
         the row of current note
     match_voiced : np.ndarray
         all notes in the same voice
 
     Returns
     -------
     next_position : np.ndarray
         the next note
     """
 
-    next_position = min(o for o in match_voiced['onset'] if o > note_info['onset'])
+    next_position = min(o for o in match_voiced["onset"] if o > note_info["onset"])
 
     # if the next note is not immediate successor of the previous one...
-    if next_position != note_info['onset'] + note_info['duration']:
+    if next_position != note_info["onset"] + note_info["duration"]:
         return None
-    
-    next_position_notes = match_voiced[match_voiced['onset'] == next_position]
+
+    next_position_notes = match_voiced[match_voiced["onset"] == next_position]
 
     # from the notes in the next position, find the one that's closest pitch-wise.
-    closest_idx = np.abs((next_position_notes['pitch'] - note_info['pitch'])).argmin()
+    closest_idx = np.abs((next_position_notes["pitch"] - note_info["pitch"])).argmin()
 
     return next_position_notes[closest_idx]
 
 
-### Pedals 
+### Pedals
+
 
-def pedal_feature(m_score : list, 
-                unique_onset_idxs: list,
-                performance: PerformanceLike):
+def pedal_feature(m_score: list, unique_onset_idxs: list, performance: PerformanceLike):
     """
-    Compute the pedal features. 
+    Compute the pedal features.
 
     Parameters
     ----------
     m_score : list
-        correspondance between score and performance notes, with score markings. 
+        correspondance between score and performance notes, with score markings.
     unique_onset_idxs : list
         a list of arrays with the note indexes that have the same onset
     performance: PerformedPart
         The original PerformedPart object
-        
+
     Returns
     -------
     pedal_ : structured array (4, n_notes) with fields
         onset_value [0, 127]: The interpolated pedal value at the onset
         offset_value [0, 127]: The interpolated pedal value at the key offset
         to_prev_release [0, 10]: delta time from note onset to the previous pedal release 'peak'
         to_next_release [0, 10]: delta time from note offset to the next pedal release 'peak'
         (think about something relates to the real duration)
-    """  
-    
+    """
+
     onset_offset_pedals, ramp_func = pedal_ramp(performance.performedparts[0], m_score)
 
     x = np.linspace(0, 100, 200)
     y = ramp_func(x)
 
     peaks, _ = find_peaks(-y, prominence=10)
     peak_timepoints = x[peaks]
 
-    release_times = np.zeros(len(m_score), dtype=[("to_prev_release", "f4"), ("to_next_release", "f4")])
+    release_times = np.zeros(
+        len(m_score), dtype=[("to_prev_release", "f4"), ("to_next_release", "f4")]
+    )
     for i, note in enumerate(m_score):
-        peaks_before = peak_timepoints[note['p_onset'] >= peak_timepoints]
-        peaks_after = peak_timepoints[(note['p_onset'] + note['p_duration']) <= peak_timepoints]
+        peaks_before = peak_timepoints[note["p_onset"] >= peak_timepoints]
+        peaks_after = peak_timepoints[
+            (note["p_onset"] + note["p_duration"]) <= peak_timepoints
+        ]
         if len(peaks_before):
-            release_times[i]["to_prev_release"] = min(note['p_onset'] - peaks_before.max(), 10)
+            release_times[i]["to_prev_release"] = min(
+                note["p_onset"] - peaks_before.max(), 10
+            )
         if len(peaks_after):
-            release_times[i]["to_next_release"] = min(peaks_after.min() - (note['p_onset'] + note['p_duration']), 10)
-
-    # plt.plot(x[peaks], y[peaks], "x")
-    # plt.plot(x, y)
-    # plt.show()
+            release_times[i]["to_next_release"] = min(
+                peaks_after.min() - (note["p_onset"] + note["p_duration"]), 10
+            )
 
-    return rfn.merge_arrays([onset_offset_pedals, release_times], flatten=True, usemask=False)
+    return rfn.merge_arrays(
+        [onset_offset_pedals, release_times], flatten=True, usemask=False
+    )
 
 
-def pedal_ramp(ppart: PerformedPart,
-               m_score: np.ndarray):
+def pedal_ramp(ppart: PerformedPart, m_score: np.ndarray):
     """Pedal ramp in the same shape as the m_score.
 
     Returns:
     * pramp : a ramp function that ranges from 0
                   to 127 with the change of sustain pedal
     """
     pedal_controls = ppart.controls
     W = np.zeros((len(m_score), 2))
-    onset_timepoints = m_score['p_onset']
-    offset_timepoints = m_score['p_onset'] + m_score['p_duration']
+    onset_timepoints = m_score["p_onset"]
+    offset_timepoints = m_score["p_onset"] + m_score["p_duration"]
 
-    timepoints = [control['time'] for control in pedal_controls]
-    values = [control['value'] for control in pedal_controls]
+    timepoints = [control["time"] for control in pedal_controls]
+    values = [control["value"] for control in pedal_controls]
 
-    if len(timepoints) <= 1: # the case there is no pedal
+    if len(timepoints) <= 1:  # the case there is no pedal
         timepoints, values = [0, 0], [0, 0]
 
     agg_ramp_func = interp1d(timepoints, values, bounds_error=False, fill_value=0)
     W[:, 0] = agg_ramp_func(onset_timepoints)
     W[:, 1] = agg_ramp_func(offset_timepoints)
 
     # Filter out NaN values
     W[np.isnan(W)] = 0.0
 
-    return np.array([tuple(i) for i in W], dtype=[("onset_value", "f4"), ("offset_value", "f4")]), agg_ramp_func
+    return (
+        np.array(
+            [tuple(i) for i in W], dtype=[("onset_value", "f4"), ("offset_value", "f4")]
+        ),
+        agg_ramp_func,
+    )
 
 
 ### Phrasing
 
 ### Tempo
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/pitch_spelling.py` & `partitura-1.3.1/partitura/musicanalysis/pitch_spelling.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
 
         chroma_vector_list.append(chroma_vector.copy())
 
     return np.array(chroma_vector_list)
 
 
 def compute_morph_array(chroma_array, chroma_vector_array):
-
     n = len(chroma_array)
     # Line 1: Initialize morph array
     morph_array = np.empty(n, dtype=int)
 
     # Compute m0
     # Line 2
     init_morph = np.array([0, 1, 1, 2, 2, 3, 4, 4, 5, 5, 6, 6], dtype=int)
@@ -229,15 +228,14 @@
         # Line 24
         morph_array[j] = np.argmax(morph_strength)
 
     return morph_array
 
 
 def compute_ocm_chord_list(sorted_ocp, chroma_array, morph_array):
-
     # Lines 1-3
     ocm_array = np.column_stack((sorted_ocp[:, 0], chroma_array, morph_array)).astype(
         int
     )
 
     # Alternative implementation of lines 4--9
     unique_onsets = np.unique(ocm_array[:, 0])
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/tonal_tension.py` & `partitura-1.3.1/partitura/musicanalysis/tonal_tension.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,45 +245,41 @@
 
 class CloudDiameter(TonalTension):
     """
     Compute cloud diameter
     """
 
     def compute_tension(self, cloud, scale_factor=SCALE_FACTOR, **kwargs):
-
         if len(cloud) > 1:
             return cloud_diameter(cloud) * scale_factor
         else:
             return 0.0
 
 
 class TensileStrain(TonalTension):
     """
     Compute tensile strain
     """
 
     def __init__(
         self, tonic_idx=0, mode="major", w=DEFAULT_WEIGHTS, alpha=ALPHA, beta=BETA
     ):
-
         self.update_key(tonic_idx, mode, w, alpha, beta)
 
     def compute_tension(
         self, cloud, duration, scale_factor=SCALE_FACTOR, *args, **kwargs
     ):
-
         if duration.sum() == 0:
             return 0
 
         cloud_ce = center_of_effect(cloud, duration)
 
         return e_distance(cloud_ce, self.key_ce) * scale_factor
 
     def update_key(self, tonic_idx, mode, w=DEFAULT_WEIGHTS, alpha=ALPHA, beta=BETA):
-
         if mode in ("major", None, 1):
             self.key_ce = major_key(tonic_idx, w=w)
         elif mode in ("minor", -1):
             self.key_ce = minor_key(tonic_idx, w=w, alpha=alpha, beta=beta)
 
 
 class CloudMomentum(TonalTension):
@@ -293,15 +289,14 @@
 
     def __init__(self):
         self.prev_ce = None
 
     def compute_tension(
         self, cloud, duration, reset=False, scale_factor=SCALE_FACTOR, *args, **kwargs
     ):
-
         if duration.sum() == 0:
             return 0
 
         if reset:
             self.prev_ce = None
         cloud_ce = center_of_effect(cloud, duration)
 
@@ -324,15 +319,14 @@
         [NOTES_BY_FIFTHS.index((n["step"], n["alter"])) for n in note_array],
         dtype=int,
     )
     return note_idxs
 
 
 def prepare_note_array(note_info):
-
     note_array = ensure_notearray(
         note_info, include_pitch_spelling=True, include_key_signature=True
     )
 
     onset_unit, duration_unit = get_time_units_from_note_array(note_array)
 
     pitch_spelling_fields = ("step", "alter", "octave")
```

### Comparing `partitura-1.3.0/partitura/musicanalysis/voice_separation.py` & `partitura-1.3.1/partitura/musicanalysis/voice_separation.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,24 +120,22 @@
 
     # grace_by_key = defaultdict(list)
 
     # for (pitch, onset, dur, i) in input_array[grace_note_idxs]:
     #     grace_by_key[i].append(
 
     if monophonic_voices:
-
         # identity mapping
         idx_equivs = dict((n, n) for n in notearray["id"])
         input_array = notearray
 
     else:
-
         note_by_key = defaultdict(list)
 
-        for (pitch, onset, dur, i) in notearray:
+        for pitch, onset, dur, i in notearray:
             note_by_key[(onset, dur)].append(i)
 
         # dict that maps first chord note index to the list of all note indices
         # of the same chord
         idx_equivs = dict(
             (argmax_pitch(np.array(idx), notearray["pitch"]), np.array(idx))
             for idx in note_by_key.values()
@@ -266,15 +264,14 @@
     mcost = ma.masked_array(con_cost, mask=mask)
 
     # Initialize list of best assignments
     best_assignment = []
 
     # while there are fewer than n_assignments
     while len(best_assignment) < n_assignments:
-
         # Get the remaining minimal cost
         next_best = mcost.min(1).argmin()
         next_assig = mcost.argmin(1)[next_best]
 
         # append minimal assignment to the list
         best_assignment.append((next_best, next_assig))
 
@@ -363,15 +360,14 @@
         Voice of the note. Setting this attribute also sets the voice
         of associated grace notes (experimental...)
     velocity : int or `None`
         MIDI velocity of the note
     """
 
     def __init__(self, pitch, onset, duration, note_id, velocity=None, voice=None):
-
         # ID of the note
         self.id = note_id
         self.pitch = pitch
         self.onset = onset
         self.duration = duration
         self.offset = onset + duration
 
@@ -419,15 +415,14 @@
 
 class VSChord(object):
     """
     Base class to hold chords
     """
 
     def __init__(self, notes, rep_note="highest"):
-
         if any([n.onset != notes[0].onset for n in notes]):
             raise ValueError("All notes in the chord must have the same onset")
         if any([n.offset != notes[0].offset for n in notes]):
             raise ValueError("All notes in the chord must have the same offset")
         self.notes = notes
 
         self.pitches = np.array([n.pitch for n in self.notes])
@@ -466,30 +461,28 @@
 
 class Voice(object):
     """
     Class to hold a voice as a list of NoteStream
     """
 
     def __init__(self, stream_or_streams, voice=None):
-
         if isinstance(stream_or_streams, list):
             self.streams = stream_or_streams
         elif isinstance(stream_or_streams, NoteStream):
             self.streams = [stream_or_streams]
 
         self._voice = voice
 
         if len(self.streams) > 0:
             self._setup_voice()
 
         else:
             self.notes = []
 
     def _setup_voice(self):
-
         # sort stream by onset
         self.streams.sort(key=lambda x: x.onset)
 
         # array notes in the stream
         self.notes = []
         for stream in self.streams:
             self.notes += list(stream.notes)
@@ -545,15 +538,14 @@
 
 class VoiceManager(object):
     """
     Manage the progress of several voices
     """
 
     def __init__(self, num_voices):
-
         self.num_voices = num_voices
 
         self.voices = [Voice([], voice) for voice in range(self.num_voices)]
 
     def __getitem__(self, index):
         return self.voices[index]
 
@@ -574,15 +566,14 @@
 
 class VSBaseScore(object):
     """
     Base class for holding score-like objects for voice separation
     """
 
     def __init__(self, notes):
-
         # Set list of notes
         self.notes = notes
 
         if len(self.notes) > 0:
             self._setup_score()
 
     def _setup_score(self):
@@ -675,15 +666,14 @@
 
     def __len__(self):
         return len(self.unique_timepoints)
 
 
 class NoteStream(VSBaseScore):
     def __init__(self, notes=[], voice="auto", prev_stream=None, next_stream=None):
-
         super(NoteStream, self).__init__(notes)
         self._voice = voice
         self.prev_stream = prev_stream
         self.next_stream = next_stream
 
         if len(self.notes) > 0:
             if self._voice == "auto":
@@ -734,15 +724,14 @@
     @property
     def last(self):
         return self.notes[self.note_onsets.argmax()]
 
 
 class Contig(VSBaseScore):
     def __init__(self, notes, is_maxcontig=False):
-
         super(Contig, self).__init__(notes)
         self._is_maxcontig = is_maxcontig
         # Onset time of the contig
         self.n_voices = np.array([self.num_sound_notes(tp) for tp in self.utp])
 
         self.onset = self.utp[np.where(self.n_voices == self.n_voices.max())].min()
         self.n_voices = self.n_voices.max()
@@ -754,15 +743,14 @@
         self.duration = self.offset - self.offset
 
         # initialize streams as a list for each voice in the contig
         streams = [[] for i in range(self.n_voices)]
 
         for on in self.unique_onsets[np.where(self.unique_onsets >= self.onset)[0]]:
             for i, note in enumerate(self.sounding_notes(on)):
-
                 if note not in streams[i]:
                     streams[i].append(note)
 
         self.streams = [NoteStream(stream) for stream in streams]
 
         # set voices for if the contig is maximal
         self._set_voices_for_maxcontig()
@@ -804,15 +792,14 @@
     TODO:
     * rename this class or simplify to avoid overlap in naming
       conventions with the main package
     * better handle grace notes
     """
 
     def __init__(self, score, delete_gracenotes=False):
-
         # Score
         self.score = score
 
         if delete_gracenotes:
             # TODO: Handle grace notes correctly
             self.score = self.score[score["duration"] != 0]
         else:
@@ -843,15 +830,14 @@
                         np.argmin(abs(candidate_notes["pitch"] - grace_note["pitch"]))
                     ]
                 )
 
         self.notes = []
 
         for n in self.score:
-
             note = VSNote(
                 pitch=n["pitch"],
                 onset=n["onset"],
                 duration=n["duration"],
                 note_id=n["id"],
             )
 
@@ -906,15 +892,14 @@
                 ("duration", "f4"),
                 ("voice", "i4"),
                 ("id", type(self.notes[0].id)),
             ],
         )
 
     def make_contigs(self):
-
         # number of voices at each time point in the score
         n_voices = np.array([len(sn) for sn in self])
 
         self.num_voices = np.max(n_voices)
 
         # if len(n_voices) > 5:
         #     if n_voices[:-3].max() < n_voices[-3:].max():
@@ -931,30 +916,27 @@
         n_voice_changes = np.r_[len(self[0]), np.diff(n_voices)]
 
         # initialize segment boundaries with changes in number of voices
         segment_boundaries = n_voice_changes != 0
 
         # Look for voice status changes
         for i, sn in enumerate(self):
-
             # an array of booleans that indicate whether each currently sounding note
             # was sounding in the previous time point (segment)
             note_sounding_in_prev_segment = np.array([n in self[i - 1] for n in sn])
 
             # Update the segment boundary if:
             # * there are sounding notes in the previous segment; and
             # * there is a change in number of voices in the current segment
             if any(note_sounding_in_prev_segment) and n_voice_changes[i] != 0:
-
                 # indices of the sounding notes belonging to the previous time point
                 prev_sounding_note_idxs = np.where(note_sounding_in_prev_segment)[0]
 
                 # Update segment boundaries
                 for psnix in prev_sounding_note_idxs:
-
                     # get sounding note
                     prev_sounding_note = sn[psnix]
                     # Get index of the timepoint of the onset of the prev_sounding_note
                     timepoint_idx = np.where(self.utp == prev_sounding_note.onset)[0]
 
                     # update segment boundaries
                     segment_boundaries[timepoint_idx] = True
@@ -964,15 +946,14 @@
         # List for the number of voices per contig
         self._voices_per_contig = []
         # Initial onset of the contig
         self._contigs_init_onsets = []
 
         # iterate over timepoints, sounding notes and segment boundaries
         for tp, sn, sb, nv in zip(self.utp, self, segment_boundaries, n_voices):
-
             # If there is a segment boundary and there are sounding notes
             # (i.e. do not make empty contigs)
             if sb and len(sn) > 0:
                 # initialize the contig
                 self.contig_dict[tp] = sn
                 # keep the timepoint
                 last_tp = tp
@@ -1022,15 +1003,14 @@
         b_unassigned = []
 
         # The loop iterates until all notes have been assigned a voice,
         # or there is no more score left
         while keep_loop:
             # Cristalization process around the maximal contigs
             for mci in maximal_contigs_idxs:
-
                 # Get voice manager corresponding to the current
                 # maximal contig
                 vm = voice_managers_dict[mci]
                 try:
                     # forward contig
                     f_contig = self.contigs[mci + (nix - 1)]
                 except IndexError:
@@ -1059,15 +1039,14 @@
                 if f_contig is not None:
                     # If there is still a next contig
                     if next_contig is not None:
                         # If the next neighbor contig has not yet
                         # been assigned (assigne voice wrt the closest
                         # maximal contig)
                         if not next_contig.has_voice_info:
-
                             # flag voices without a connection in
                             # the previous step in the loop
                             for es in f_unassigned:
                                 vm[es].last.skip_contig += 1
 
                             # Compute connection cost
                             cost = pairwise_cost(vm, next_contig)
```

### Comparing `partitura-1.3.0/partitura/performance.py` & `partitura-1.3.1/partitura/performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,14 @@
         ensure_unique_tracks: bool = True,
     ) -> None:
         self.id = id
 
         if isinstance(performedparts, PerformedPart):
             self.performedparts = [performedparts]
         elif isinstance(performedparts, Itertype):
-
             if not all([isinstance(pp, PerformedPart) for pp in performedparts]):
                 raise ValueError(
                     "`performedparts` should be a list of  `PerformedPart` objects!"
                 )
             self.performedparts = list(performedparts)
         else:
             raise ValueError(
@@ -412,17 +411,15 @@
                 ]
             )
         )
 
         track_map = dict([(tid, ti) for ti, tid in enumerate(unique_track_ids)])
 
         for i, ppart in enumerate(self):
-
             for note in ppart.notes:
-
                 note["track"] = track_map[(i, note.get("track", -1))]
 
             for control in ppart.controls:
                 control["track"] = track_map[(i, control.get("track", -1))]
 
             for program in ppart.programs:
                 program["track"] = track_map[(i, program.get("track", -1))]
```

### Comparing `partitura-1.3.0/partitura/score.py` & `partitura-1.3.1/partitura/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         -------
         function
             The mapping function
 
         """
         # operations to avoid None values and filter them efficiently.
         m_it = self.measures
-        
+
         measures = np.array(
             [
                 [
                     m.start.t,
                     m.end.t,
                     (m_it[i - 1].number if m.number == None else m.number),
                 ]
@@ -383,15 +383,14 @@
                         inter_function(input).astype(int),
                         measure_inter_function(input).astype(int),
                     )
 
             return int_interp1d
 
     def _time_interpolator(self, quarter=False, inv=False, musical_beat=False):
-
         if len(self._points) < 2:
             return lambda x: np.zeros(len(x))
 
         keypoints = defaultdict(lambda: [None, None])
         _ = keypoints[self.first_point.t]
         _ = keypoints[self.last_point.t]
         for t, q in zip(self._quarter_times, self._quarter_durations):
@@ -430,21 +429,19 @@
                 (keypoints[:-1, 2] * np.diff(keypoints[:, 0])) / keypoints[:-1, 1]
             ),
         ]
 
         m1 = next(self.first_point.iter_starting(Measure), None)
 
         if m1 and m1.start is not None and m1.end is not None:
-
             f = interp1d(x, y)
             actual_dur = np.diff(f((m1.start.t, m1.end.t)))[0]
             ts = next(m1.start.iter_starting(TimeSignature), None)
 
             if ts:
-
                 normal_dur = ts.beats
                 if quarter:
                     normal_dur *= 4 / ts.beat_type
                 if musical_beat:
                     normal_dur = ts.musical_beats
                 if actual_dur < normal_dur:
                     y -= actual_dur
@@ -639,17 +636,15 @@
         Returns
         -------
         list
             List of Segment objects
 
         """
         add_segments(self)
-        return [
-            e for e in self.iter_all(Segment, include_subclasses=False)
-        ]
+        return [e for e in self.iter_all(Segment, include_subclasses=False)]
 
     def quarter_durations(self, start=None, end=None):
         """Return an Nx2 array with quarter duration (second column)
         and their respective times (first column).
 
         When a start and or end time is specified, the returned
         array will contain only the entries within those bounds.
@@ -1455,47 +1450,43 @@
         starting_items = [
             o
             for _, oo in starting_items_lists
             for o in sorted(oo, key=lambda x: x.duration or -1)
         ]
 
         if ending_items:
-
             result.append("{}".format(tree).rstrip())
 
             if starting_items:
                 tree.next_item()
             else:
                 tree.last_item()
 
             result.append("{}ending objects".format(tree))
             tree.push()
             result.append("{}".format(tree).rstrip())
 
             for i, item in enumerate(ending_items):
-
                 if i == (len(ending_items) - 1):
                     tree.last_item()
                 else:
                     tree.next_item()
 
                 result.append("{}{}".format(tree, item))
 
             tree.pop()
 
         if starting_items:
-
             result.append("{}".format(tree).rstrip())
             tree.last_item()
             result.append("{}starting objects".format(tree))
             tree.push()
             result.append("{}".format(tree).rstrip())
 
             for i, item in enumerate(starting_items):
-
                 if i == (len(starting_items) - 1):
                     tree.last_item()
                 else:
                     tree.next_item()
                 result.append("{}{}".format(tree, item))
 
             tree.pop()
@@ -2156,15 +2147,14 @@
         See parameters
     octave_change : int
         See parameters
 
     """
 
     def __init__(self, staff, sign, line, octave_change):
-
         super().__init__()
         self.staff = staff
         self.sign = sign
         self.line = line
         self.octave_change = octave_change
 
     def __str__(self):
@@ -2568,15 +2558,14 @@
         self.number = number
         self.lines = lines
 
     def __str__(self):
         return f"{super().__str__()} number={self.number} lines={self.lines}"
 
 
-
 class KeySignature(TimedObject):
     """Key signature.
 
     Parameters
     ----------
     fifths : number
         Number of sharps (positive) or flats (negative)
@@ -2673,46 +2662,46 @@
         self.text = text
         self.staff = staff
 
     def __str__(self):
         return f'{super().__str__()} "{self.text}"'
 
 
-
 class OctaveShiftDirection(TimedObject):
     """An octave shift direction.
 
     Parameters
     ----------
 
     """
+
     def __init__(self, shift_type, shift_size=8, staff=None):
         super().__init__()
         self.shift_type = shift_type
         self.shift_size = shift_size
         self.staff = staff
         self.applied = False
 
     def __str__(self):
         return f'{super().__str__()} "{self.shift_type}"'
 
 
 class Harmony(TimedObject):
     """A harmony element in the score not currently used.
 
-        Parameters
-        ----------
-        text : str
-            The harmony text
+    Parameters
+    ----------
+    text : str
+        The harmony text
 
-        Attributes
-        ----------
-        text : str
-            See parameters
-        """
+    Attributes
+    ----------
+    text : str
+        See parameters
+    """
 
     def __init__(self, text):
         super().__init__()
         self.text = text
         # assert issubclass(note, GenericNote)
 
     def __str__(self):
@@ -2740,14 +2729,15 @@
 
     def __str__(self):
         return f'{super().__str__()} "{self.text}"'
 
 
 class ChordSymbol(TimedObject):
     """A harmony element in the score usually for Chord Symbols."""
+
     def __init__(self, root, kind, bass=None):
         super().__init__()
         self.kind = kind
         self.root = root
         self.bass = bass
 
     def __str__(self):
@@ -2763,25 +2753,31 @@
     number : int
         The interval number (e.g. 1, 2, 3, 4, 5, 6, 7, ...)
     quality : str
         The interval quality (e.g. M, m, P, A, d, dd, AA)
     direction : str
         The interval direction (e.g. up, down)
     """
+
     def __init__(self, number, quality, direction="up"):
         self.number = number
         self.quality = quality
         self.direction = direction
         self.validate()
 
     def validate(self):
         number = self.number % 7
         number = 7 if number == 0 else number
-        assert self.quality+str(number) in INTERVALCLASSES, f"Interval {number}{self.quality} not found"
-        assert self.direction in ["up", "down"], f"Interval direction {self.direction} not found"
+        assert (
+            self.quality + str(number) in INTERVALCLASSES
+        ), f"Interval {number}{self.quality} not found"
+        assert self.direction in [
+            "up",
+            "down",
+        ], f"Interval direction {self.direction} not found"
 
     def __str__(self):
         return f'{super().__str__()} "{self.number}{self.quality}"'
 
 
 class Direction(TimedObject):
     """Base class for performance directions in the score."""
@@ -3177,15 +3173,14 @@
             o_new = set()
             tp = start
             while tp != end:
                 # make a new timepoint, corresponding to tp
                 tp_new = part.get_or_add_point(tp.t + delta)
                 o_gen = (o for oo in tp.starting_objects.values() for o in oo)
                 for o in o_gen:
-
                     # special cases:
 
                     # don't include some TimedObjects in the unfolded part
                     if isinstance(
                         o,
                         (
                             Repeat,
@@ -3322,15 +3317,14 @@
 
     for ts_start, ts_end, measure_dur in zip(
         ts_start_times, ts_end_times, beats_per_measure
     ):
         pos = ts_start
 
         while pos < ts_end:
-
             measure_start = pos
             measure_end_beats = min(beat_map(pos) + measure_dur, beat_map(end))
             measure_end = min(ts_end, inv_beat_map(measure_end_beats))
             # any existing measures between measure_start and measure_end
             existing_measure = next(
                 part.iter_all(Measure, measure_start, measure_end), None
             )
@@ -3344,15 +3338,19 @@
                         existing_measure.number = mcounter
                         mcounter += 1
                     continue
 
                 else:
                     measure_end = existing_measure.start.t
 
-            part.add(Measure(number=mcounter, name=str(mcounter)), int(measure_start), int(measure_end))
+            part.add(
+                Measure(number=mcounter, name=str(mcounter)),
+                int(measure_start),
+                int(measure_end),
+            )
 
             # if measure exists but was not at measure_start,
             # a filler measure is added with number mcounter
             if existing_measure:
                 pos = existing_measure.end.t
                 existing_measure.number = mcounter + 1
                 mcounter = mcounter + 2
@@ -3582,15 +3580,14 @@
     # then split/tie any notes that do not have a fractional/dot duration
     divs_map = part.quarter_duration_map
     max_splits = 3
     failed = 0
     succeeded = 0
     for i, note in enumerate(list(part.iter_all(Note))):
         if note.symbolic_duration is None:
-
             splits = find_tie_split(
                 note.start.t, note.end.t, int(divs_map(note.start.t)), max_splits
             )
 
             if splits:
                 succeeded += 1
                 split_note(part, note, splits)
@@ -3622,37 +3619,30 @@
 
 
 def _set_end_times(part, cls):
     acc = []
     t = None
 
     for obj in part.iter_all(cls, include_subclasses=True):
-
         if obj.start == t:
-
             if obj.end is None:
-
                 acc.append(obj)
 
         else:
-
             for o in acc:
-
                 part.add(o, end=obj.start.t)
 
             acc = []
 
             if obj.end is None:
-
                 acc.append(obj)
 
             t = obj.start
 
     for o in acc:
-
         part.add(o, end=part.last_point.t)
 
 
 def split_note(part, note, splits):
     # non-public
 
     # TODO: we shouldn't do this, but for now it's a good sanity check
@@ -3724,28 +3714,25 @@
     normal_notes = 2
 
     candidates = []
     prev_end = None
 
     # 1. group consecutive notes without symbolic_duration
     for note in part.iter_all(GenericNote, include_subclasses=True):
-
         if note.symbolic_duration is None:
             if note.start.t == prev_end:
                 candidates[-1].append(note)
             else:
                 candidates.append([note])
             prev_end = note.end.t
 
     # 2. within each group
     for group in candidates:
-
         # 3. search for the predefined list of tuplets
         for actual_notes in search_for_tuplets:
-
             if actual_notes > len(group):
                 # tuplet requires more notes than we have
                 continue
 
             tup_start = 0
 
             while tup_start <= (len(group) - actual_notes):
@@ -3755,15 +3742,14 @@
 
                 if len(durs) > 1:
                     # notes have different durations (possibly valid but not
                     # supported here)
                     # continue
                     tup_start += 1
                 else:
-
                     start = note_tuplet[0].start.t
                     end = note_tuplet[-1].end.t
                     total_dur = end - start
 
                     # total duration of tuplet notes must be integer-divisble by
                     # normal_notes
                     if total_dur % normal_notes > 0:
@@ -3809,15 +3795,14 @@
     remove_grace_counter = 0
     elements_to_remove = []
     for gn in part.iter_all(GraceNote):
         if gn.main_note is None:
             for no in part.iter_all(
                 Note, include_subclasses=False, start=gn.start.t, end=gn.start.t + 1
             ):
-
                 if no.voice == gn.voice:
                     gn.last_grace_note_in_seq.grace_next = no
 
         if gn.main_note is None:
             elements_to_remove.append(gn)
             remove_grace_counter += 1
 
@@ -4000,15 +3985,14 @@
         current_volta_total_number = 0
 
         for ss in boundary_times[:-1]:
             se = segment_info[ss]["end"]
 
             # loop through the boundaries at the end of current segment
             for boundary_type in boundaries[se].keys():
-
                 # REPEATS
                 if boundary_type == "repeat_start":
                     segment_info[ss]["to"].append(segment_info[se]["ID"])
                 if boundary_type == "repeat_end":
                     if "volta_end" not in list(boundaries[se].keys()):
                         segment_info[ss]["to"].append(segment_info[se]["ID"])
                         repeat_start = boundaries[se][boundary_type].start.t
@@ -4069,15 +4053,15 @@
                     if str(current_volta_total_number) in current_volta_numbers:
                         # else just go to the segment after the last
                         segment_info[ss]["to"].append(
                             segment_info[current_volta_end]["ID"]
                         )
 
                 # NAVIGATION SYMBOLS
-                
+
                 # Navigation1_ = destinations that should only be used after all others
                 # Navigation2_ = destinations that are used *after* a jump
                 if boundary_type == "coda":
                     # if a coda symbol is passed just continue
                     segment_info[ss]["to"].append(segment_info[se]["ID"])
                     segment_info[se]["type"] = "leap_end"
                     segment_info[se]["info"].append("Coda")
@@ -4099,30 +4083,30 @@
                     segment_info[se]["info"].append("segno")
 
                 if boundary_type == "dalsegno":
                     segment_info[ss]["to"].append(segment_info[se]["ID"])
                     # find the segno and jump there
                     segno_time = destinations["segno"][0]
                     segment_info[ss]["to"].append(
-                        "Navigation1_" + segment_info[segno_time]["ID"] 
+                        "Navigation1_" + segment_info[segno_time]["ID"]
                     )
                     segment_info[ss]["to"].append(
-                        "Navigation2_" + segment_info[se]["ID"] 
+                        "Navigation2_" + segment_info[se]["ID"]
                     )
                     segment_info[ss]["type"] = "leap_start"
                     segment_info[ss]["info"].append("dal segno")
 
                 if boundary_type == "dacapo":
                     segment_info[ss]["to"].append(segment_info[se]["ID"])
                     # jump to the start
                     segment_info[ss]["to"].append(
                         "Navigation1_" + segment_info[part.first_point.t]["ID"]
                     )
                     segment_info[ss]["to"].append(
-                        "Navigation2_" + segment_info[se]["ID"] 
+                        "Navigation2_" + segment_info[se]["ID"]
                     )
                     segment_info[ss]["type"] = "leap_start"
                     segment_info[ss]["info"].append("da capo")
 
                 if boundary_type == "fine":
                     segment_info[ss]["to"].append(segment_info[se]["ID"])
                     # jump to the start
@@ -4236,16 +4220,17 @@
         + "\t segment "
         + "{:<20}".format(
             str(part.beat_map(segments[p].start.t))
             + " - "
             + str(part.beat_map(segments[p].end.t))
         )
         + "\t duration: "
-        + "{:<6}".format(str(part.beat_map(segments[p].end.t) - \
-                             part.beat_map(segments[p].start.t)))
+        + "{:<6}".format(
+            str(part.beat_map(segments[p].end.t) - part.beat_map(segments[p].start.t))
+        )
         + "\t info: "
         + str(segments[p].info)
         for p in segments.keys()
     ]
     return "\n".join(string_list)
 
 
@@ -4275,15 +4260,14 @@
         path_list,
         segments,
         used_segment_jumps=None,
         no_repeats=False,
         all_repeats=False,
         jumped=False,
     ):
-
         self.path = path_list
         self.segments = segments
         if used_segment_jumps is None:
             self.used_segment_jumps = defaultdict(list)
         else:
             self.used_segment_jumps = used_segment_jumps
         self.ended = False
@@ -4349,28 +4333,28 @@
             no_repeats=self.no_repeats,
             all_repeats=self.all_repeats,
             jumped=self.jumped,
         )
         for key in self.used_segment_jumps:
             for used_dest in self.used_segment_jumps[key]:
                 new_path.used_segment_jumps[key].append(used_dest)
-        
+
         return new_path
 
     def make_copy_with_jump_to(self, destination, ignore_leap_info=True):
         """
         create a copy of this path instance with an added jump.
         If the jump is a leap (dal segno, da capo, al coda)
         and leap information is not ignored,
         set the new Path to subsequently follow the the shortest version.
         """
         new_path = self.copy()
         new_path.used_segment_jumps[new_path.path[-1]].append(destination)
         new_path.path.append(destination)
-        
+
         if (
             new_path.segments[destination].type == "leap_end"
             and new_path.segments[new_path.path[-2]].type == "leap_start"
         ):
             if not new_path.jumped:
                 new_path.jumped = True
                 for segid in new_path.segments.keys():
@@ -4382,33 +4366,33 @@
                         # add the waiting destinations
                         to += seg.await_to
                         # replace destinations
                         seg.to = to
                     # delete used destinations
                     new_path.used_segment_jumps[segid] = list()
                 # add the jump destination to the used ones
-                new_path.used_segment_jumps[new_path.path[-2]].append(destination)      
-                        
+                new_path.used_segment_jumps[new_path.path[-2]].append(destination)
+
             if not ignore_leap_info:
                 new_path.no_repeats = True
         return new_path
 
     @property
-    def list_of_destinations_from_last_segment(self):    
+    def list_of_destinations_from_last_segment(self):
         destinations = list(self.segments[self.path[-1]].to)
         previously_used_destinations = self.used_segment_jumps[self.path[-1]]
         # only continue in order of the sequence, after full consumption, start at zero
         # if the full or minimal sequence is forced,
         # return only the single possible jump destination, else return possibly many.
-        
-        if len(previously_used_destinations) != 0:       
+
+        if len(previously_used_destinations) != 0:
             last_destination = previously_used_destinations[-1]
             last_destination_count = previously_used_destinations.count(
                 last_destination
-            )               
+            )
             last_destination_index = [
                 i for i, n in enumerate(destinations * 100) if n == last_destination
             ][last_destination_count - 1]
             last_destination_index %= len(destinations)
 
         if self.no_repeats:
             # currently this is in higher priority than the full sequence
@@ -4854,21 +4838,23 @@
                     else None
                 )
                 if reassign == "voice":
                     if isinstance(e, GenericNote):
                         e.voice = e.voice + sum(maximum_voices[:p_ind])
                 elif reassign == "staff":
                     if isinstance(e, (GenericNote, Words, Direction)):
-
-                        e.staff = (e.staff if e.staff is not None else 1) + sum(maximum_staves[:p_ind])
+                        e.staff = (e.staff if e.staff is not None else 1) + sum(
+                            maximum_staves[:p_ind]
+                        )
                     elif isinstance(
                         e, Clef
                     ):  # TODO: to update if "number" get changed in "staff"
-
-                        e.staff = (e.staff if e.staff is not None else 1) + sum(maximum_staves[:p_ind])
+                        e.staff = (e.staff if e.staff is not None else 1) + sum(
+                            maximum_staves[:p_ind]
+                        )
                 new_part.add(e, start=new_start, end=new_end)
 
                 # new_part.add(copy.deepcopy(e), start=new_start, end=new_end)
     return new_part
 
 
 def is_a_within_b(a, b, wholly=False):
```

### Comparing `partitura-1.3.0/partitura/utils/__init__.py` & `partitura-1.3.1/partitura/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,9 +75,9 @@
     "fifths_mode_to_key_name",
     "key_mode_to_int",
     "pitch_spelling_to_midi_pitch",
     "pitch_spelling_to_note_name",
     "show_diff",
     "PrettyPrintTree",
     "synthesize",
-    "normalize"
+    "normalize",
 ]
```

### Comparing `partitura-1.3.0/partitura/utils/generic.py` & `partitura-1.3.1/partitura/utils/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,26 +110,23 @@
     ('start', 'end')
 
     """
     iterable = iter(iterable)
 
     cur = start
     try:
-
         if cur is _sentinel:
             cur = next(iterable)
 
         while True:
-
             nxt = next(iterable)
             yield (cur, nxt)
             cur = nxt
 
     except StopIteration:
-
         if cur is not _sentinel and end is not _sentinel:
             yield (cur, end)
 
 
 def iter_subclasses(cls, _seen=None):
     """
     iter_subclasses(cls)
@@ -566,22 +563,20 @@
             copy=copy,
             bounds_error=bounds_error,
             fill_value=fill_value,
             assume_sorted=assume_sorted,
         )
 
     else:
-
         # If there is only one value for x and y, assume that the method
         # will always return the same value for any input.
 
         def interp_fun(
             input_var: Union[float, int, np.ndarray]
         ) -> Callable[[Union[float, int, np.ndarray]], np.ndarray]:
-
             if y.ndim > 1:
                 result = np.broadcast_to(y, (len(np.atleast_1d(input_var)), y.shape[1]))
             else:
                 result = np.broadcast_to(y, (len(np.atleast_1d(input_var)),))
 
             if not isinstance(input_var, np.ndarray):
                 # the output of scipy's interp1d is always an array
@@ -631,28 +626,29 @@
     x : np.ndarray or None
         The input variable of sequence s(x).
     Returns
     -------
     s_mono: np.ndarray
        a monotonic sequence that has been linearly interpolated using a subset of s
     x_mono: np.ndarray
-        The input of the monotonic sequence. 
+        The input of the monotonic sequence.
     """
     eps = np.finfo(float).eps
 
     _s = np.r_[np.min(s) - eps, s, np.max(s) + eps]
     if x is not None:
         _x = np.r_[np.min(x) - eps, x, np.max(x) + eps]
     else:
         _x = np.r_[-eps, np.arange(len(s)), len(s) - 1 + eps]
 
     s_mono = np.maximum.accumulate(s)
     mask = np.r_[False, True, (np.diff(s_mono) != 0), False]
     x_mono = _x[1:-1]
     s_mono = interp1d(_x[mask], _s[mask], fill_value="extrapolate")(x_mono)
-    
+
     return s_mono, x_mono
 
+
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `partitura-1.3.0/partitura/utils/misc.py` & `partitura-1.3.1/partitura/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,14 @@
     # Initialize new image
     new_image = Image.new(mode=mode, size=output_size, color=0)
 
     # coordinates to place the image
     anchor_x = 0
     anchor_y = 0
     for img, size in zip(images, image_sizes):
-
         new_image.paste(img, (anchor_x, anchor_y))
 
         # update coordinates according to the concatenation mode
         if concat_mode == "vertical":
             anchor_y += size[1]
 
         elif concat_mode == "horizontal":
```

### Comparing `partitura-1.3.0/partitura/utils/music.py` & `partitura-1.3.1/partitura/utils/music.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 import partitura
 from tempfile import TemporaryDirectory
 import os
 
 try:
     import miditok
     from miditok.midi_tokenizer import MIDITokenizer
-    import miditoolkit 
+    import miditoolkit
 except ImportError:
     miditok = None
     miditoolkit = None
+
     class MIDITokenizer(object):
         pass
 
+
 from partitura.utils.misc import deprecated_alias
 
 if TYPE_CHECKING:
     # Import typing info for typing annotations.
     # For this to work we need to import annotations from __future__
     # Solution from
     # https://medium.com/quick-code/python-type-hinting-eliminating-importerror-due-to-circular-imports-265dfb0580f8
@@ -273,21 +275,47 @@
     for specific in ["dd", "d", "m", "M", "A", "AA"]
 ] + [
     f"{specific}{generic}"
     for generic in [1, 4, 5]
     for specific in ["dd", "d", "P", "A", "AA"]
 ]
 
-INTERVAL_TO_SEMITONES = dict(zip(INTERVALCLASSES, [
-    generic+specific for generic in [1, 3, 8, 10] for specific in [-2, -1, 0, 1, 2, 3]
-] + [generic+specific for generic in [0, 5, 7] for specific in [-2, -1, 0, 1, 2]]))
-
+INTERVAL_TO_SEMITONES = dict(
+    zip(
+        INTERVALCLASSES,
+        [
+            generic + specific
+            for generic in [1, 3, 8, 10]
+            for specific in [-2, -1, 0, 1, 2, 3]
+        ]
+        + [
+            generic + specific
+            for generic in [0, 5, 7]
+            for specific in [-2, -1, 0, 1, 2]
+        ],
+    )
+)
 
-STEPS = {"C": 0, "D": 1, "E": 2, "F": 3, "G": 4, "A": 5, "B": 6, 0: "C", 1: "D", 2: "E", 3: "F", 4: "G", 5: "A", 6: "B"}
 
+STEPS = {
+    "C": 0,
+    "D": 1,
+    "E": 2,
+    "F": 3,
+    "G": 4,
+    "A": 5,
+    "B": 6,
+    0: "C",
+    1: "D",
+    2: "E",
+    3: "F",
+    4: "G",
+    5: "A",
+    6: "B",
+}
 
 
 MUSICAL_BEATS = {6: 2, 9: 3, 12: 4}
 
 # Standard tuning frequency of A4 in Hz
 A4 = 440.0
 
@@ -402,28 +430,28 @@
     inverval
 
     """
     op = lambda x, y: abs(x + y) % 7 if direction == "up" else abs(x - y) % 7
     if interval == "P1":
         pass
     else:
-        step = STEPS[op(STEPS[step.capitalize()], interval-1)]
+        step = STEPS[op(STEPS[step.capitalize()], interval - 1)]
     return step
 
 
 def _transpose_note(note, interval):
     """
     Transpose a note by a given interval.
     Parameters
     ----------
     note
     inverval
 
     """
-    if interval.quality+str(interval.number) == "P1":
+    if interval.quality + str(interval.number) == "P1":
         pass
     else:
         # TODO work for arbitrary octave.
         prev_step = note.step.capitalize()
         note.step = transpose_step(prev_step, interval.number, interval.direction)
         if STEPS[note.step] - STEPS[prev_step] < 0 and interval.direction == "up":
             note.octave += 1
@@ -434,15 +462,17 @@
         prev_alter = note.alter if note.alter is not None else 0
         prev_pc = MIDI_BASE_CLASS[prev_step.lower()] + prev_alter
         tmp_pc = MIDI_BASE_CLASS[note.step.lower()]
         if interval.direction == "up":
             diff_sm = tmp_pc - prev_pc if tmp_pc >= prev_pc else tmp_pc + 12 - prev_pc
         else:
             diff_sm = prev_pc - tmp_pc if prev_pc >= tmp_pc else prev_pc + 12 - tmp_pc
-        note.alter = INTERVAL_TO_SEMITONES[interval.quality+str(interval.number)] - diff_sm
+        note.alter = (
+            INTERVAL_TO_SEMITONES[interval.quality + str(interval.number)] - diff_sm
+        )
 
 
 def transpose(score: ScoreLike, interval: Interval) -> ScoreLike:
     """
     Transpose a score by a given interval.
 
     Parameters
@@ -454,14 +484,15 @@
 
     Returns
     -------
     Score
         Transposed score.
     """
     import partitura.score as s
+
     new_score = copy.deepcopy(score)
     if isinstance(score, s.Score):
         for part in new_score.parts:
             transpose(part, interval)
     elif isinstance(score, s.Part):
         for note in score.notes_tied:
             _transpose_note(note, interval)
@@ -667,15 +698,14 @@
     "ff": -2,
     "bbb": -3,
     "-": None,
 }
 
 
 def ensure_pitch_spelling_format(step, alter, octave):
-
     if step.lower() not in MIDI_BASE_CLASS:
         if step.lower() != "r":
             raise ValueError("Invalid `step`")
 
     if isinstance(alter, str):
         try:
             alter = SIGN_TO_ALTER[alter]
@@ -957,22 +987,20 @@
     'q..'
 
     >>> format_symbolic_duration({'type': '16th'})
     '16th'
 
     """
     if symbolic_dur is None:
-
         return "unknown"
 
     else:
         result = (symbolic_dur.get("type") or "") + "." * symbolic_dur.get("dots", 0)
 
         if "actual_notes" in symbolic_dur and "normal_notes" in symbolic_dur:
-
             result += "_{}/{}".format(
                 symbolic_dur["actual_notes"], symbolic_dur["normal_notes"]
             )
 
         return result
 
 
@@ -1708,15 +1736,14 @@
     score and a performance.
 
     """
     input_note_array = ensure_notearray(input_note_array)
     target_note_array = ensure_notearray(target_note_array)
 
     if fields is not None:
-
         if isinstance(fields, (list, tuple)):
             onset_key, duration_key = fields
         elif isinstance(fields, str):
             onset_key = fields
             duration_key = None
 
             if duration_key is None and check_duration:
@@ -1857,15 +1884,14 @@
         control_dict[c["track"]][c["channel"]][c["number"]].append(
             (c["time"], c["value"])
         )
 
     for track in control_dict:
         for channel in control_dict[track]:
             for number, ct in control_dict[track][channel].items():
-
                 cta = np.array(ct)
                 cinterp = interp1d(
                     x=cta[:, 0],
                     y=cta[:, 1],
                     kind="previous",
                     bounds_error=False,
                     fill_value=(cta[0, 1], cta[-1, 1]),
@@ -2563,15 +2589,14 @@
 
     # field for divs_pq
     if divs_per_quarter:
         fields += [("divs_pq", "i4")]
 
     note_array = []
     for note in note_list:
-
         note_info = tuple()
         note_on_div = note.start.t
         note_off_div = note.start.t + note.duration_tied
         note_dur_div = note_off_div - note_on_div
 
         if beat_map is not None:
             note_on_beat, note_off_beat = beat_map([note_on_div, note_off_div])
@@ -2758,15 +2783,14 @@
         ]
     # fields for staff
     if include_staff:
         fields += [("staff", "i4")]
 
     rest_array = []
     for rest in rest_list:
-
         rest_info = tuple()
         rest_on_div = rest.start.t
         rest_off_div = rest.start.t + rest.duration_tied
         rest_dur_div = rest_off_div - rest_on_div
 
         if beat_map is not None:
             note_on_beat, note_off_beat = beat_map([rest_on_div, rest_off_div])
@@ -2871,22 +2895,20 @@
     while cond:
         rest_array, filter_idx = collapse_rests(rest_array)
         cond = len(filter_idx) > 0
     return rest_array
 
 
 def update_note_ids_after_unfolding(part):
-
     note_id_dict = defaultdict(list)
 
     for n in part.notes:
         note_id_dict[n.id].append(n)
 
     for nid, notes in note_id_dict.items():
-
         if nid is None:
             continue
 
         notes.sort(key=lambda x: x.start.t)
 
         for i, note in enumerate(notes):
             note.id = f"{note.id}-{i+1}"
@@ -2984,17 +3006,15 @@
         ("channel", "i4"),
         ("id", "U256"),
     ]
 
     pnote_array = np.zeros(len(snote_array), dtype=ppart_fields)
 
     if isinstance(velocity, np.ndarray):
-
         if velocity.ndim == 2:
-
             velocity_fun = interp1d(
                 x=velocity[:, 0],
                 y=velocity[:, 1],
                 kind="previous",
                 bounds_error=False,
                 fill_value=(velocity[0, 1], velocity[-1, 1]),
             )
@@ -3022,25 +3042,23 @@
         [np.where(snote_array["onset_beat"] == u)[0] for u in unique_onsets],
         dtype=object,
     )
 
     iois = np.diff(unique_onsets)
 
     if callable(bpm) or isinstance(bpm, np.ndarray):
-
         if callable(bpm):
             # bpm parameter is a callable that returns a bpm value
             # for each score onset
             bp = 60 / bpm(unique_onsets)
             bp_duration = (
                 60 / bpm(snote_array["onset_beat"]) * snote_array["duration_beat"]
             )
 
         elif isinstance(bpm, np.ndarray):
-
             if bpm.ndim != 2:
                 raise ValueError("`bpm` should be a 2D array")
 
             bpm_fun = interp1d(
                 x=bpm[:, 0],
                 y=bpm[:, 1],
                 kind="previous",
@@ -3205,15 +3223,15 @@
     """
     Get a slice of a PeformedPart by time
 
     Parameters
     ----------
     ppart : `PerformedPart` object
     start_time : float
-        Starting time in seconds 
+        Starting time in seconds
     end_time : float
         End time in seconds
     clip_note_off : bool
         Clip note_off time to end_time
     reindex_notes : bool
         Reindex notes in slice starting from n0
 
@@ -3230,98 +3248,106 @@
 
     if start_time > end_time:
         raise ValueError("Start time not less than end time!")
 
     # create a new (empty) instance of a PerformedPart
     # single dummy note added to be able to set sustain_pedal_threshold in __init__
     # -> check `adjust_offsets_w_sustain` in partitura.performance
-    ppart_slice = PerformedPart([{'note_on': 0, 'note_off': 0}])
+    ppart_slice = PerformedPart([{"note_on": 0, "note_off": 0}])
 
     # get ppq if PerformedPart contains it,
     # else skip time_tick info when e.g. created with 'load_performance_midi'
     try:
         ppq = ppart.ppq
         ppart_slice.ppq = ppq
     except AttributeError:
         ppq = None
 
     if ppart.controls:
         controls_slice = []
         for cc in ppart.controls:
-            if cc['time'] >= start_time and cc['time'] <= end_time:
+            if cc["time"] >= start_time and cc["time"] <= end_time:
                 new_cc = cc.copy()
-                new_cc['time'] -= start_time
+                new_cc["time"] -= start_time
                 if ppq:
-                    new_cc['time_tick'] = int(2 * ppq * cc['time'])
+                    new_cc["time_tick"] = int(2 * ppq * cc["time"])
                 controls_slice.append(new_cc)
         ppart_slice.controls = controls_slice
-    
+
     if ppart.programs:
         programs_slice = []
         for pr in ppart.programs:
-            if pr['time'] >= start_time and pr['time'] <= end_time:
+            if pr["time"] >= start_time and pr["time"] <= end_time:
                 new_pr = pr.copy()
-                new_pr['time'] -= start_time
+                new_pr["time"] -= start_time
                 if ppq:
-                    new_pr['time_tick'] = int(2 * ppq * pr['time'])
+                    new_pr["time_tick"] = int(2 * ppq * pr["time"])
                 programs_slice.append(new_pr)
         ppart_slice.programs = programs_slice
 
     notes_slice = []
     note_id = 0
-    for note in ppart.notes: 
+    for note in ppart.notes:
         # collect previous sounding notes at start_time
         if note["note_on"] < start_time and note["note_off"] > start_time:
             new_note = note.copy()
-            new_note['note_on'] = 0.
+            new_note["note_on"] = 0.0
             if clip_note_off:
-                new_note['note_off'] = min(note['note_off'] - start_time, end_time - start_time)
-            else: 
-                new_note['note_off'] = note['note_off'] - start_time
+                new_note["note_off"] = min(
+                    note["note_off"] - start_time, end_time - start_time
+                )
+            else:
+                new_note["note_off"] = note["note_off"] - start_time
             if ppq:
-                new_note['note_on_tick'] = 0
-                new_note['note_off_tick'] = int(2 * ppq * new_note['note_off'])
+                new_note["note_on_tick"] = 0
+                new_note["note_off_tick"] = int(2 * ppq * new_note["note_off"])
             if reindex_notes:
-                new_note['id'] = f"n{note_id}"
+                new_note["id"] = f"n{note_id}"
                 note_id += 1
             notes_slice.append(new_note)
         # todo - combine both cases
-        if note['note_on'] >= start_time: 
-            if note['note_on'] < end_time:
+        if note["note_on"] >= start_time:
+            if note["note_on"] < end_time:
                 new_note = note.copy()
-                new_note['note_on'] -= start_time
+                new_note["note_on"] -= start_time
                 if clip_note_off:
-                    new_note['note_off'] = min(note['note_off'] - start_time, end_time - start_time)
-                else: 
-                    new_note['note_off'] = note['note_off'] - start_time
+                    new_note["note_off"] = min(
+                        note["note_off"] - start_time, end_time - start_time
+                    )
+                else:
+                    new_note["note_off"] = note["note_off"] - start_time
                 if ppq:
-                    new_note['note_on_tick'] = int(2 * ppq * new_note['note_on'])
-                    new_note['note_off_tick'] = int(2 * ppq * new_note['note_off'])
+                    new_note["note_on_tick"] = int(2 * ppq * new_note["note_on"])
+                    new_note["note_off_tick"] = int(2 * ppq * new_note["note_off"])
                 if reindex_notes:
-                    new_note['id'] = 'n' + str(note_id)
+                    new_note["id"] = "n" + str(note_id)
                     note_id += 1
                 notes_slice.append(new_note)
-            # assumes notes in list are sorted by onset time   
-            else: 
-                break               
-    
+            # assumes notes in list are sorted by onset time
+            else:
+                break
+
     ppart_slice.notes = notes_slice
-    
-    # set threshold property after creating notes list to update 'sound_offset' values 
+
+    # set threshold property after creating notes list to update 'sound_offset' values
     ppart_slice.sustain_pedal_threshold = ppart.sustain_pedal_threshold
 
     if ppart.id:
-        ppart_slice.id = ppart.id + '_slice_{}s_to_{}s'.format(start_time, end_time)     
+        ppart_slice.id = ppart.id + "_slice_{}s_to_{}s".format(start_time, end_time)
     if ppart.part_name:
-        ppart_slice.part_name = ppart.part_name 
+        ppart_slice.part_name = ppart.part_name
 
     return ppart_slice
 
 
-def tokenize(score_data : ScoreLike, tokenizer : MIDITokenizer, incomplete_bar_behaviour : str = "pad_bar"):
+def tokenize(
+    score_data: ScoreLike,
+    tokenizer: MIDITokenizer,
+    incomplete_bar_behaviour: str = "pad_bar",
+):
     """
     Tokenize a score using a tokenizer from miditok.
     Parameters
     ----------
     score_data : Score, list, Part, or PartGroup
         The musical score to be saved. A :class:`partitura.score.Score` object,
         a :class:`partitura.score.Part`, a :class:`partitura.score.PartGroup` or
@@ -3336,21 +3362,28 @@
     Returns
     -------
     ppart_slice :  `Tokens` object
         Tokens as produced by the miditok library.
     """
 
     if miditok is None or miditoolkit is None:
-        raise ImportError("Miditok and miditoolkit must be installed for this function to work")
+        raise ImportError(
+            "Miditok and miditoolkit must be installed for this function to work"
+        )
     with TemporaryDirectory() as tmpdir:
         temp_midi_path = os.path.join(tmpdir, "temp_midi.mid")
-        partitura.io.exportmidi.save_score_midi(score_data, out = temp_midi_path, anacrusis_behavior=incomplete_bar_behaviour, part_voice_assign_mode = 4, minimum_ppq = 480 )
+        partitura.io.exportmidi.save_score_midi(
+            score_data,
+            out=temp_midi_path,
+            anacrusis_behavior=incomplete_bar_behaviour,
+            part_voice_assign_mode=4,
+            minimum_ppq=480,
+        )
         midi = miditoolkit.MidiFile(temp_midi_path)
         tokens = tokenizer(midi)
     return tokens
 
 
-
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `partitura-1.3.0/partitura/utils/synth.py` & `partitura-1.3.1/partitura/utils/synth.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,39 +316,36 @@
 
 class DistributedHarmonics(object):
     def __init__(
         self,
         n_harmonics: int,
         weights: Union[np.ndarray, str] = "equal",
     ) -> None:
-
         self.n_harmonics = n_harmonics
         self.weights = weights
 
         if self.weights == "equal":
             self.weights = 1.0 / (self.n_harmonics + 1) * np.ones(self.n_harmonics + 1)
 
         self._overtones = np.arange(1, self.n_harmonics + 2)
 
     def __call__(self, freq: float) -> Tuple[np.ndarray]:
-
         return self._overtones * freq, self.weights
 
 
 class ShepardTones(object):
     """
     Generate Shepard Tones
     """
 
     def __init__(
         self,
         min_freq: Union[float, int] = 77.8,
         max_freq: Union[float, int] = 2349,
     ) -> None:
-
         self.min_freq = min_freq
         self.max_freq = max_freq
 
         x_freq = np.linspace(self.min_freq, self.max_freq, 1000)
 
         weights = np.hanning(len(x_freq) + 2) + 0.001
         weights /= max(weights)
@@ -357,15 +354,14 @@
             x=x_freq,
             y=weights[1:-1],
             bounds_error=False,
             fill_value=weights.min(),
         )
 
     def __call__(self, freq) -> Tuple[np.ndarray]:
-
         min_freq = self.min_f(freq)
 
         freqs = 2 ** np.arange(5) * min_freq
 
         return freqs, self.shepard_weights_fun(freqs)
 
     def min_f(self, freq: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
@@ -481,23 +477,21 @@
 
     if harmonic_dist is None:
 
         def harmonic_dist(x):
             return x, 1
 
     elif isinstance(harmonic_dist, int):
-
         harmonic_dist = DistributedHarmonics(harmonic_dist)
 
     elif isinstance(harmonic_dist, str):
         if harmonic_dist in ("shepard",):
             harmonic_dist = ShepardTones()
 
-    for (f, oif, dur) in zip(freq_in_hz, onsets_in_frames, duration):
-
+    for f, oif, dur in zip(freq_in_hz, onsets_in_frames, duration):
         freqs, weights = harmonic_dist(f)
 
         note = additive_synthesis(
             freqs=freqs,
             duration=dur,
             samplerate=samplerate,
             weights=weights,
```

### Comparing `partitura-1.3.0/partitura.egg-info/PKG-INFO` & `partitura-1.3.1/partitura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partitura
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package for handling symbolic musical information
 Home-page: https://github.com/CPJKU/partitura
 Author: Maarten Grachten, Carlos Cancino-Chacón, Silvan Peter, Emmanouil Karystinaios, Francesco Foscarin, Thassilo Gadermaier
 Author-email: partitura-users@googlegroups.com
 License: Apache 2.0
 Keywords: music notation musicxml midi
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `partitura-1.3.0/partitura.egg-info/SOURCES.txt` & `partitura-1.3.1/partitura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/setup.py` & `partitura-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 NAME = "partitura"
 DESCRIPTION = "A package for handling symbolic musical information"
 KEYWORDS = "music notation musicxml midi"
 URL = "https://github.com/CPJKU/partitura"
 EMAIL = "partitura-users@googlegroups.com"
 AUTHOR = "Maarten Grachten, Carlos Cancino-Chacón, Silvan Peter, Emmanouil Karystinaios, Francesco Foscarin, Thassilo Gadermaier"
 REQUIRES_PYTHON = ">=3.7"
-VERSION = "1.3.0"
+VERSION = "1.3.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["numpy", "scipy", "lxml", "lark-parser", "xmlschema", "mido"]
 
 # What packages are optional?
 EXTRAS = {}
```

### Comparing `partitura-1.3.0/tests/test_deprecations.py` & `partitura-1.3.1/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_display.py` & `partitura-1.3.1/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_harmony.py` & `partitura-1.3.1/tests/test_harmony.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_kern.py` & `partitura-1.3.1/tests/test_kern.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_key_estimation.py` & `partitura-1.3.1/tests/test_key_estimation.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_load_performance.py` & `partitura-1.3.1/tests/test_load_performance.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_load_score.py` & `partitura-1.3.1/tests/test_load_score.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_m21_import.py` & `partitura-1.3.1/tests/test_m21_import.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_match_export.py` & `partitura-1.3.1/tests/test_match_export.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_match_import.py` & `partitura-1.3.1/tests/test_match_import.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_mei.py` & `partitura-1.3.1/tests/test_mei.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_merge_parts.py` & `partitura-1.3.1/tests/test_merge_parts.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_metrical_position.py` & `partitura-1.3.1/tests/test_metrical_position.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_midi_export.py` & `partitura-1.3.1/tests/test_midi_export.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_midi_import.py` & `partitura-1.3.1/tests/test_midi_import.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_nakamura.py` & `partitura-1.3.1/tests/test_nakamura.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_new_divs.py` & `partitura-1.3.1/tests/test_new_divs.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_note_array.py` & `partitura-1.3.1/tests/test_note_array.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_note_features.py` & `partitura-1.3.1/tests/test_note_features.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_octave_shift.py` & `partitura-1.3.1/tests/test_octave_shift.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_parangonada.py` & `partitura-1.3.1/tests/test_parangonada.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_part_properties.py` & `partitura-1.3.1/tests/test_part_properties.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_partial_measures.py` & `partitura-1.3.1/tests/test_partial_measures.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_performance.py` & `partitura-1.3.1/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_performance_codec.py` & `partitura-1.3.1/tests/test_performance_codec.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_performance_features.py` & `partitura-1.3.1/tests/test_performance_features.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_pianoroll.py` & `partitura-1.3.1/tests/test_pianoroll.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_pitch_spelling.py` & `partitura-1.3.1/tests/test_pitch_spelling.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_quarter_adjust.py` & `partitura-1.3.1/tests/test_quarter_adjust.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_rest_array.py` & `partitura-1.3.1/tests/test_rest_array.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_synth.py` & `partitura-1.3.1/tests/test_synth.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_time_estimation.py` & `partitura-1.3.1/tests/test_time_estimation.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_times.py` & `partitura-1.3.1/tests/test_times.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_tonal_tension.py` & `partitura-1.3.1/tests/test_tonal_tension.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_transpose.py` & `partitura-1.3.1/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_utils.py` & `partitura-1.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_voice_estimation.py` & `partitura-1.3.1/tests/test_voice_estimation.py`

 * *Files identical despite different names*

### Comparing `partitura-1.3.0/tests/test_xml.py` & `partitura-1.3.1/tests/test_xml.py`

 * *Files identical despite different names*

