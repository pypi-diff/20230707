# Comparing `tmp/lexikos-0.0.1rc5.tar.gz` & `tmp/lexikos-0.0.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1rc5.tar", last modified: Fri Jun 16 10:13:59 2023, max compression
+gzip compressed data, was "lexikos-0.0.1rc6.tar", last modified: Fri Jul  7 10:18:43 2023, max compression
```

## Comparing `lexikos-0.0.1rc5.tar` & `lexikos-0.0.1rc6.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.761545 lexikos-0.0.1rc5/
--rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc5/LICENSE
--rw-r--r--   0 mac        (502) staff       (20)       41 2023-06-14 04:34:25.000000 lexikos-0.0.1rc5/MANIFEST.in
--rw-r--r--   0 mac        (502) staff       (20)    29774 2023-06-16 10:13:59.761819 lexikos-0.0.1rc5/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)    16050 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/README.md
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.724793 lexikos-0.0.1rc5/lexikos/
--rw-r--r--   0 mac        (502) staff       (20)      105 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/__init__.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.720392 lexikos-0.0.1rc5/lexikos/dict/
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.727176 lexikos-0.0.1rc5/lexikos/dict/asr-data/
--rw-r--r--   0 mac        (502) staff       (20)      406 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/asr-data/austalk_en_au.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2618 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/asr-data/sc_cw_en_au.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.731688 lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/
--rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
--rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.741535 lexikos-0.0.1rc5/lexikos/dict/synthetic/
--rw-r--r--   0 mac        (502) staff       (20)     2953 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/bookbot_en_v1-v2_lexicon.tsv
--rw-r--r--   0 mac        (502) staff       (20)   114117 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/common-voice-accent-gb_lexicon.tsv
--rw-r--r--   0 mac        (502) staff       (20)      231 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/common-voice-accent-id_lexicon.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1690872 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/librispeech-lexicon-en-id.tsv
--rw-r--r--   0 mac        (502) staff       (20)   202316 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/wu_lexicon.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.761183 lexikos-0.0.1rc5/lexikos/dict/wikipron/
--rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1927152 2023-06-14 09:36:53.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1841107 2023-06-14 08:45:02.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)     5360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/g2p.py
--rw-r--r--   0 mac        (502) staff       (20)     2823 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/lexicon.py
--rw-r--r--   0 mac        (502) staff       (20)     3360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/normalizer.py
--rw-r--r--   0 mac        (502) staff       (20)     1354 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/t5.py
--rw-r--r--   0 mac        (502) staff       (20)      722 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/utils.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.726527 lexikos-0.0.1rc5/lexikos.egg-info/
--rw-r--r--   0 mac        (502) staff       (20)    29774 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)     1375 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (502) staff       (20)        1 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (502) staff       (20)       51 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/requires.txt
--rw-r--r--   0 mac        (502) staff       (20)        8 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/top_level.txt
--rw-r--r--   0 mac        (502) staff       (20)      821 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/pyproject.toml
--rw-r--r--   0 mac        (502) staff       (20)       50 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/requirements.txt
--rw-r--r--   0 mac        (502) staff       (20)      113 2023-06-16 10:13:59.762347 lexikos-0.0.1rc5/setup.cfg
--rw-r--r--   0 mac        (502) staff       (20)     1187 2023-06-14 04:32:35.000000 lexikos-0.0.1rc5/setup.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.584329 lexikos-0.0.1rc6/
+-rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc6/LICENSE
+-rw-r--r--   0 mac        (502) staff       (20)       41 2023-06-14 04:34:25.000000 lexikos-0.0.1rc6/MANIFEST.in
+-rw-r--r--   0 mac        (502) staff       (20)    29774 2023-07-07 10:18:43.584766 lexikos-0.0.1rc6/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)    16050 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/README.md
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.362490 lexikos-0.0.1rc6/lexikos/
+-rw-r--r--   0 mac        (502) staff       (20)      105 2023-07-07 10:17:38.000000 lexikos-0.0.1rc6/lexikos/__init__.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.351400 lexikos-0.0.1rc6/lexikos/dict/
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.369103 lexikos-0.0.1rc6/lexikos/dict/asr-data/
+-rw-r--r--   0 mac        (502) staff       (20)      406 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/dict/asr-data/austalk_en_au.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2618 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/dict/asr-data/sc_cw_en_au.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.382251 lexikos-0.0.1rc6/lexikos/dict/cmudict-ipa/
+-rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc6/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc6/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.448200 lexikos-0.0.1rc6/lexikos/dict/synthetic/
+-rw-r--r--   0 mac        (502) staff       (20)     2953 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/bookbot_en_v1-v2_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   119802 2023-07-07 10:05:53.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-au_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   146283 2023-07-07 10:05:57.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-ca_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   114117 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-gb_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)      231 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-id_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   351806 2023-07-07 10:05:56.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-in_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    31065 2023-07-07 10:05:53.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-nz_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   635155 2023-07-07 10:05:55.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-us_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1690872 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/librispeech-lexicon-en-id.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   202316 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/dict/synthetic/wu_lexicon.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.581493 lexikos-0.0.1rc6/lexikos/dict/wikipron/
+-rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_au_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_in_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1927152 2023-06-14 09:36:53.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1841107 2023-06-14 08:45:02.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_us_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     5360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc6/lexikos/g2p.py
+-rw-r--r--   0 mac        (502) staff       (20)     2823 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/lexikos/lexicon.py
+-rw-r--r--   0 mac        (502) staff       (20)     3360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc6/lexikos/normalizer.py
+-rw-r--r--   0 mac        (502) staff       (20)     1354 2023-06-14 04:29:02.000000 lexikos-0.0.1rc6/lexikos/t5.py
+-rw-r--r--   0 mac        (502) staff       (20)      722 2023-06-14 04:29:02.000000 lexikos-0.0.1rc6/lexikos/utils.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-07-07 10:18:43.366942 lexikos-0.0.1rc6/lexikos.egg-info/
+-rw-r--r--   0 mac        (502) staff       (20)    29774 2023-07-07 10:18:43.000000 lexikos-0.0.1rc6/lexikos.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)     1665 2023-07-07 10:18:43.000000 lexikos-0.0.1rc6/lexikos.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (502) staff       (20)        1 2023-07-07 10:18:43.000000 lexikos-0.0.1rc6/lexikos.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (502) staff       (20)       51 2023-07-07 10:18:43.000000 lexikos-0.0.1rc6/lexikos.egg-info/requires.txt
+-rw-r--r--   0 mac        (502) staff       (20)        8 2023-07-07 10:18:43.000000 lexikos-0.0.1rc6/lexikos.egg-info/top_level.txt
+-rw-r--r--   0 mac        (502) staff       (20)      821 2023-07-07 10:17:53.000000 lexikos-0.0.1rc6/pyproject.toml
+-rw-r--r--   0 mac        (502) staff       (20)       50 2023-06-16 10:13:39.000000 lexikos-0.0.1rc6/requirements.txt
+-rw-r--r--   0 mac        (502) staff       (20)      113 2023-07-07 10:18:43.586002 lexikos-0.0.1rc6/setup.cfg
+-rw-r--r--   0 mac        (502) staff       (20)     1187 2023-06-14 04:32:35.000000 lexikos-0.0.1rc6/setup.py
```

### Comparing `lexikos-0.0.1rc5/LICENSE` & `lexikos-0.0.1rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/PKG-INFO` & `lexikos-0.0.1rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc5
+Version: 0.0.1rc6
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lexikos-0.0.1rc5/README.md` & `lexikos-0.0.1rc6/README.md`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/asr-data/sc_cw_en_au.tsv` & `lexikos-0.0.1rc6/lexikos/dict/asr-data/sc_cw_en_au.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv` & `lexikos-0.0.1rc6/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv` & `lexikos-0.0.1rc6/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/synthetic/bookbot_en_v1-v2_lexicon.tsv` & `lexikos-0.0.1rc6/lexikos/dict/synthetic/bookbot_en_v1-v2_lexicon.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/synthetic/common-voice-accent-gb_lexicon.tsv` & `lexikos-0.0.1rc6/lexikos/dict/synthetic/common-voice-accent-gb_lexicon.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/synthetic/librispeech-lexicon-en-id.tsv` & `lexikos-0.0.1rc6/lexikos/dict/synthetic/librispeech-lexicon-en-id.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/synthetic/wu_lexicon.tsv` & `lexikos-0.0.1rc6/lexikos/dict/synthetic/wu_lexicon.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_broad.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_au_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_narrow.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_au_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_broad.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_ca_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_broad.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_in_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_narrow.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_in_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_broad.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_nz_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_broad.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_uk_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_broad.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_us_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_narrow.tsv` & `lexikos-0.0.1rc6/lexikos/dict/wikipron/eng_latn_us_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/g2p.py` & `lexikos-0.0.1rc6/lexikos/g2p.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/lexicon.py` & `lexikos-0.0.1rc6/lexikos/lexicon.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/normalizer.py` & `lexikos-0.0.1rc6/lexikos/normalizer.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/t5.py` & `lexikos-0.0.1rc6/lexikos/t5.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos/utils.py` & `lexikos-0.0.1rc6/lexikos/utils.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc5/lexikos.egg-info/PKG-INFO` & `lexikos-0.0.1rc6/lexikos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc5
+Version: 0.0.1rc6
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lexikos-0.0.1rc5/lexikos.egg-info/SOURCES.txt` & `lexikos-0.0.1rc6/lexikos.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -17,16 +17,21 @@
 lexikos.egg-info/requires.txt
 lexikos.egg-info/top_level.txt
 lexikos/dict/asr-data/austalk_en_au.tsv
 lexikos/dict/asr-data/sc_cw_en_au.tsv
 lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
 lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
 lexikos/dict/synthetic/bookbot_en_v1-v2_lexicon.tsv
+lexikos/dict/synthetic/common-voice-accent-au_lexicon.tsv
+lexikos/dict/synthetic/common-voice-accent-ca_lexicon.tsv
 lexikos/dict/synthetic/common-voice-accent-gb_lexicon.tsv
 lexikos/dict/synthetic/common-voice-accent-id_lexicon.tsv
+lexikos/dict/synthetic/common-voice-accent-in_lexicon.tsv
+lexikos/dict/synthetic/common-voice-accent-nz_lexicon.tsv
+lexikos/dict/synthetic/common-voice-accent-us_lexicon.tsv
 lexikos/dict/synthetic/librispeech-lexicon-en-id.tsv
 lexikos/dict/synthetic/wu_lexicon.tsv
 lexikos/dict/wikipron/eng_latn.tsv
 lexikos/dict/wikipron/eng_latn_au_broad.tsv
 lexikos/dict/wikipron/eng_latn_au_narrow.tsv
 lexikos/dict/wikipron/eng_latn_ca_broad.tsv
 lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
```

### Comparing `lexikos-0.0.1rc5/pyproject.toml` & `lexikos-0.0.1rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexikos"
-version = "0.0.1rc5"
+version = "0.0.1rc6"
 description = "A collection of pronunciation dictionaries and neural grapheme-to-phoneme models."
 readme = "README.md"
 authors = [{ name="w11wo", email="wilson@bookbotkids.com" }, { name="anantoj", email="gg.ananto@gmail.com" }, { name="DavidSamuell", email="davidsamuel.7878@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lexikos-0.0.1rc5/setup.py` & `lexikos-0.0.1rc6/setup.py`

 * *Files identical despite different names*

