# Comparing `tmp/pyomorfi-1.0.0.tar.gz` & `tmp/pyomorfi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyomorfi-1.0.0.tar", last modified: Thu Jul  6 21:36:20 2023, max compression
+gzip compressed data, was "pyomorfi-1.0.1.tar", last modified: Fri Jul  7 10:40:49 2023, max compression
```

## Comparing `pyomorfi-1.0.0.tar` & `pyomorfi-1.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:36:20.992455 pyomorfi-1.0.0/
--rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-05 20:13:22.000000 pyomorfi-1.0.0/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     2131 2023-07-06 21:36:20.992517 pyomorfi-1.0.0/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1487 2023-07-06 21:20:13.000000 pyomorfi-1.0.0/README.md
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:36:20.986185 pyomorfi-1.0.0/pyomorfi/
--rw-r--r--   0 iikka      (501) staff       (20)     1170 2023-07-06 21:35:23.000000 pyomorfi-1.0.0/pyomorfi/__init__.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:36:20.988815 pyomorfi-1.0.0/pyomorfi/omorfi/
--rw-r--r--   0 iikka      (501) staff       (20)     2566 2023-07-06 21:35:09.000000 pyomorfi-1.0.0/pyomorfi/omorfi/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)     7574 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/analyser.py
--rw-r--r--   0 iikka      (501) staff       (20)    54353 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/analysis.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:36:20.989272 pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/
--rw-r--r--   0 iikka      (501) staff       (20)     1110 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)     7583 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/disamparsulator.py
--rw-r--r--   0 iikka      (501) staff       (20)     7204 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/evidence.py
--rw-r--r--   0 iikka      (501) staff       (20)     3065 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/matcher.py
--rw-r--r--   0 iikka      (501) staff       (20)     3046 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/doc.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:36:20.990473 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/
--rw-r--r--   0 iikka      (501) staff       (20)      965 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/__init__.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     8784 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/gradation.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     7040 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/guess_feats.py
--rwxr-xr-x   0 iikka      (501) staff       (20)   249160 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/guess_new_class.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     4685 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/parse_csv_data.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    10833 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/plurale_tantum.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    28252 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/stub.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     2555 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/wordmap.py
--rw-r--r--   0 iikka      (501) staff       (20)     1826 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/error_logging.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:36:20.992317 pyomorfi-1.0.0/pyomorfi/omorfi/formats/
--rw-r--r--   0 iikka      (501) staff       (20)     1068 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/__init__.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    16572 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/apertium_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     3649 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/experimental_xml_formatter.py
--rw-r--r--   0 iikka      (501) staff       (20)     6725 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/fileformats.py
--rw-r--r--   0 iikka      (501) staff       (20)     3448 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    21027 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/ftb3_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    17939 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/giella_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     1368 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/kotus_sanalista_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    13475 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/labeled_segments_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     3736 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/lexc_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    10877 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/monodix_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     4812 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/no_tags_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    29793 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/omor_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     7908 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/regex_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)    13705 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/tdt_formatter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     7555 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/formats/twolc_formatter.py
--rw-r--r--   0 iikka      (501) staff       (20)     1629 2023-07-05 22:46:17.000000 pyomorfi-1.0.0/pyomorfi/omorfi/generator.py
--rw-r--r--   0 iikka      (501) staff       (20)     6370 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/guesser.py
--rw-r--r--   0 iikka      (501) staff       (20)      452 2023-07-06 20:00:23.000000 pyomorfi-1.0.0/pyomorfi/omorfi/hfst.py
--rw-r--r--   0 iikka      (501) staff       (20)     2212 2023-07-05 22:44:38.000000 pyomorfi-1.0.0/pyomorfi/omorfi/hyphenator.py
--rw-r--r--   0 iikka      (501) staff       (20)     2638 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/labelsegmenter.py
--rw-r--r--   0 iikka      (501) staff       (20)     1958 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/lemmatiser.py
--rw-r--r--   0 iikka      (501) staff       (20)    14985 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/omorfi.py
--rw-r--r--   0 iikka      (501) staff       (20)     2105 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/segmenter.py
--rwxr-xr-x   0 iikka      (501) staff       (20)     5880 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/settings.py
--rw-r--r--   0 iikka      (501) staff       (20)     5896 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/string_manglers.py
--rw-r--r--   0 iikka      (501) staff       (20)    12851 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/token.py
--rw-r--r--   0 iikka      (501) staff       (20)    12227 2023-07-05 20:13:03.000000 pyomorfi-1.0.0/pyomorfi/omorfi/tokeniser.py
--rw-r--r--   0 iikka      (501) staff       (20)   674393 2023-07-06 20:49:10.000000 pyomorfi-1.0.0/pyomorfi/omorfi.analyse.kfst
--rw-r--r--   0 iikka      (501) staff       (20)  3032363 2023-07-06 20:49:40.000000 pyomorfi-1.0.0/pyomorfi/omorfi.describe.kfst
--rw-r--r--   0 iikka      (501) staff       (20)  2839631 2023-07-06 20:49:55.000000 pyomorfi-1.0.0/pyomorfi/omorfi.generate.kfst
--rw-r--r--   0 iikka      (501) staff       (20)  1017656 2023-07-06 20:49:19.000000 pyomorfi-1.0.0/pyomorfi/omorfi.segment.kfst
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-06 21:36:20.987139 pyomorfi-1.0.0/pyomorfi.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     2131 2023-07-06 21:36:20.000000 pyomorfi-1.0.0/pyomorfi.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     2064 2023-07-06 21:36:20.000000 pyomorfi-1.0.0/pyomorfi.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-06 21:36:20.000000 pyomorfi-1.0.0/pyomorfi.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-06 21:36:20.000000 pyomorfi-1.0.0/pyomorfi.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        9 2023-07-06 21:36:20.000000 pyomorfi-1.0.0/pyomorfi.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:24.000000 pyomorfi-1.0.0/pyproject.toml
--rw-r--r--   0 iikka      (501) staff       (20)      915 2023-07-06 21:36:20.992745 pyomorfi-1.0.0/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:40:49.917753 pyomorfi-1.0.1/
+-rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-05 20:13:22.000000 pyomorfi-1.0.1/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     2131 2023-07-07 10:40:49.917827 pyomorfi-1.0.1/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1487 2023-07-06 21:20:13.000000 pyomorfi-1.0.1/README.md
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:40:49.908925 pyomorfi-1.0.1/pyomorfi/
+-rw-r--r--   0 iikka      (501) staff       (20)     1170 2023-07-06 21:35:23.000000 pyomorfi-1.0.1/pyomorfi/__init__.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:40:49.913554 pyomorfi-1.0.1/pyomorfi/omorfi/
+-rw-r--r--   0 iikka      (501) staff       (20)     2566 2023-07-06 21:35:09.000000 pyomorfi-1.0.1/pyomorfi/omorfi/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)     7574 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/analyser.py
+-rw-r--r--   0 iikka      (501) staff       (20)    54353 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/analysis.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:40:49.914087 pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/
+-rw-r--r--   0 iikka      (501) staff       (20)     1110 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)     7583 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/disamparsulator.py
+-rw-r--r--   0 iikka      (501) staff       (20)     7204 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/evidence.py
+-rw-r--r--   0 iikka      (501) staff       (20)     3065 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/matcher.py
+-rw-r--r--   0 iikka      (501) staff       (20)     3046 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/doc.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:40:49.915500 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/
+-rw-r--r--   0 iikka      (501) staff       (20)      965 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/__init__.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     8784 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/gradation.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     7040 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/guess_feats.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)   249160 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/guess_new_class.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     4685 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/parse_csv_data.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    10833 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/plurale_tantum.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    28252 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/stub.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     2555 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/wordmap.py
+-rw-r--r--   0 iikka      (501) staff       (20)     1826 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/error_logging.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:40:49.917640 pyomorfi-1.0.1/pyomorfi/omorfi/formats/
+-rw-r--r--   0 iikka      (501) staff       (20)     1068 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/__init__.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    16572 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/apertium_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     3649 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/experimental_xml_formatter.py
+-rw-r--r--   0 iikka      (501) staff       (20)     6725 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/fileformats.py
+-rw-r--r--   0 iikka      (501) staff       (20)     3448 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    21027 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/ftb3_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    17939 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/giella_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     1368 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/kotus_sanalista_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    13475 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/labeled_segments_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     3736 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/lexc_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    10877 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/monodix_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     4812 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/no_tags_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    29793 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/omor_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     7908 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/regex_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)    13705 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/tdt_formatter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     7555 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/formats/twolc_formatter.py
+-rw-r--r--   0 iikka      (501) staff       (20)     1629 2023-07-05 22:46:17.000000 pyomorfi-1.0.1/pyomorfi/omorfi/generator.py
+-rw-r--r--   0 iikka      (501) staff       (20)     6370 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/guesser.py
+-rw-r--r--   0 iikka      (501) staff       (20)      452 2023-07-06 20:00:23.000000 pyomorfi-1.0.1/pyomorfi/omorfi/hfst.py
+-rw-r--r--   0 iikka      (501) staff       (20)     2212 2023-07-05 22:44:38.000000 pyomorfi-1.0.1/pyomorfi/omorfi/hyphenator.py
+-rw-r--r--   0 iikka      (501) staff       (20)     2638 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/labelsegmenter.py
+-rw-r--r--   0 iikka      (501) staff       (20)     1958 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/lemmatiser.py
+-rw-r--r--   0 iikka      (501) staff       (20)    14985 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/omorfi.py
+-rw-r--r--   0 iikka      (501) staff       (20)     2105 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/segmenter.py
+-rwxr-xr-x   0 iikka      (501) staff       (20)     5880 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/settings.py
+-rw-r--r--   0 iikka      (501) staff       (20)     5896 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/string_manglers.py
+-rw-r--r--   0 iikka      (501) staff       (20)    12851 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/token.py
+-rw-r--r--   0 iikka      (501) staff       (20)    12227 2023-07-05 20:13:03.000000 pyomorfi-1.0.1/pyomorfi/omorfi/tokeniser.py
+-rw-r--r--   0 iikka      (501) staff       (20)   674393 2023-07-06 20:49:10.000000 pyomorfi-1.0.1/pyomorfi/omorfi.analyse.kfst
+-rw-r--r--   0 iikka      (501) staff       (20)  3032363 2023-07-06 20:49:40.000000 pyomorfi-1.0.1/pyomorfi/omorfi.describe.kfst
+-rw-r--r--   0 iikka      (501) staff       (20)  2839631 2023-07-06 20:49:55.000000 pyomorfi-1.0.1/pyomorfi/omorfi.generate.kfst
+-rw-r--r--   0 iikka      (501) staff       (20)  1017656 2023-07-06 20:49:19.000000 pyomorfi-1.0.1/pyomorfi/omorfi.segment.kfst
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:40:49.909885 pyomorfi-1.0.1/pyomorfi.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     2131 2023-07-07 10:40:49.000000 pyomorfi-1.0.1/pyomorfi.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     2064 2023-07-07 10:40:49.000000 pyomorfi-1.0.1/pyomorfi.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-07 10:40:49.000000 pyomorfi-1.0.1/pyomorfi.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-07 10:40:49.000000 pyomorfi-1.0.1/pyomorfi.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        9 2023-07-07 10:40:49.000000 pyomorfi-1.0.1/pyomorfi.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:24.000000 pyomorfi-1.0.1/pyproject.toml
+-rw-r--r--   0 iikka      (501) staff       (20)      915 2023-07-07 10:40:49.918052 pyomorfi-1.0.1/setup.cfg
```

### Comparing `pyomorfi-1.0.0/LICENSE` & `pyomorfi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/PKG-INFO` & `pyomorfi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyomorfi
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pure-python implementation of the Omorfi library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyOmorfi
 
 This is a pure-python implementation of Omorfi, a free and open source morphological analyzer for Finnish.
```

### Comparing `pyomorfi-1.0.0/README.md` & `pyomorfi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/__init__.py` & `pyomorfi-1.0.1/pyomorfi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/__init__.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/analyser.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/analyser.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/analysis.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/analysis.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/__init__.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/disamparsulator.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/disamparsulator.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/evidence.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/evidence.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/disamparsulate/matcher.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/disamparsulate/matcher.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/doc.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/doc.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/__init__.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/gradation.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/gradation.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/guess_feats.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/guess_feats.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/guess_new_class.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/guess_new_class.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/parse_csv_data.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/parse_csv_data.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/plurale_tantum.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/plurale_tantum.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/stub.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/stub.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/entryguessing/wordmap.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/entryguessing/wordmap.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/error_logging.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/error_logging.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/__init__.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/apertium_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/apertium_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/experimental_xml_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/experimental_xml_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/fileformats.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/fileformats.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/ftb3_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/ftb3_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/giella_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/giella_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/kotus_sanalista_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/kotus_sanalista_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/labeled_segments_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/labeled_segments_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/lexc_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/lexc_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/monodix_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/monodix_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/no_tags_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/no_tags_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/omor_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/omor_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/regex_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/regex_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/tdt_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/tdt_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/formats/twolc_formatter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/formats/twolc_formatter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/generator.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/generator.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/guesser.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/guesser.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/hyphenator.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/hyphenator.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/labelsegmenter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/labelsegmenter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/lemmatiser.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/lemmatiser.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/omorfi.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/omorfi.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/segmenter.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/segmenter.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/settings.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/settings.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/string_manglers.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/string_manglers.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/token.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/token.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi/tokeniser.py` & `pyomorfi-1.0.1/pyomorfi/omorfi/tokeniser.py`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi.analyse.kfst` & `pyomorfi-1.0.1/pyomorfi/omorfi.analyse.kfst`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi.describe.kfst` & `pyomorfi-1.0.1/pyomorfi/omorfi.describe.kfst`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi.generate.kfst` & `pyomorfi-1.0.1/pyomorfi/omorfi.generate.kfst`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi/omorfi.segment.kfst` & `pyomorfi-1.0.1/pyomorfi/omorfi.segment.kfst`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/pyomorfi.egg-info/PKG-INFO` & `pyomorfi-1.0.1/pyomorfi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyomorfi
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pure-python implementation of the Omorfi library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyOmorfi
 
 This is a pure-python implementation of Omorfi, a free and open source morphological analyzer for Finnish.
```

### Comparing `pyomorfi-1.0.0/pyomorfi.egg-info/SOURCES.txt` & `pyomorfi-1.0.1/pyomorfi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyomorfi-1.0.0/setup.cfg` & `pyomorfi-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyomorfi
-version = 1.0.0
+version = 1.0.1
 author = Iikka Hauhio
 author_email = iikka.hauhio@helsinki.fi
 description = A pure-python implementation of the Omorfi library that provides Finnish morphological analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = finnish nlp morphology
 license = GNU GPLv3
@@ -21,15 +21,15 @@
 [options]
 packages = 
 	pyomorfi
 	pyomorfi.omorfi
 	pyomorfi.omorfi.disamparsulate
 	pyomorfi.omorfi.entryguessing
 	pyomorfi.omorfi.formats
-python_requires = >=3.9
+python_requires = >=3.8
 install_requires = 
 	kfst
 
 [options.package_data]
 pyomorfi = *.kfst
 
 [egg_info]
```

